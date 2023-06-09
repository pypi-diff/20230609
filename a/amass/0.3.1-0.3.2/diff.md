# Comparing `tmp/amass-0.3.1.tar.gz` & `tmp/amass-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amass-0.3.1.tar", max compression
+gzip compressed data, was "amass-0.3.2.tar", max compression
```

## Comparing `amass-0.3.1.tar` & `amass-0.3.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11342 2023-06-08 17:43:11.891934 amass-0.3.1/LICENSE
--rw-r--r--   0        0        0       36 2023-06-08 17:43:11.891934 amass-0.3.1/README.md
--rw-r--r--   0        0        0    13684 2023-06-08 17:43:11.891934 amass-0.3.1/amass/__init__.py
--rw-r--r--   0        0        0     2752 2023-06-08 17:43:11.891934 amass-0.3.1/amass/cli.py
--rw-r--r--   0        0        0     1628 2023-06-08 17:43:11.891934 amass-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      882 1970-01-01 00:00:00.000000 amass-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    11342 2023-06-09 09:28:01.926913 amass-0.3.2/LICENSE
+-rw-r--r--   0        0        0       36 2023-06-09 09:28:01.926913 amass-0.3.2/README.md
+-rw-r--r--   0        0        0    14891 2023-06-09 09:28:01.926913 amass-0.3.2/amass/__init__.py
+-rw-r--r--   0        0        0     2324 2023-06-09 09:28:01.926913 amass-0.3.2/amass/cli.py
+-rw-r--r--   0        0        0     1628 2023-06-09 09:28:01.926913 amass-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      882 1970-01-01 00:00:00.000000 amass-0.3.2/PKG-INFO
```

### Comparing `amass-0.3.1/LICENSE` & `amass-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `amass-0.3.1/amass/__init__.py` & `amass-0.3.2/amass/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,25 @@
 import json
 import re
 from abc import ABC, abstractmethod
 from base64 import b64encode
 from dataclasses import asdict, dataclass
 from enum import Enum
 from pathlib import Path
-from typing import Any, Dict, Iterable, Optional, Pattern, Set, Type, Union
+from typing import (
+    Any,
+    Dict,
+    Iterable,
+    List,
+    Optional,
+    Pattern,
+    Set,
+    Type,
+    Union,
+)
 from warnings import warn
 
 import aiohttp
 import tomlkit
 from bs4 import BeautifulSoup
 from packaging.specifiers import SpecifierSet
 from packaging.version import InvalidVersion, Version
@@ -262,14 +272,15 @@
 
 @dataclass
 class LockedDependency:
     name: str
     version: str
     provider: Provider
     assets: Iterable[AssetFile]
+    maps: List[str]
 
     def __post_init__(self) -> None:
         # Handle nested serializer
         assets = []
         for a in self.assets:
             if not isinstance(a, AssetFile):
                 assets.append(AssetFile(**a))
@@ -339,23 +350,31 @@
                 with open(file, "rb") as f:
                     content = f.read()
                     asset.check_integrity(content=content)
 
         if generated_files != found_files:
             raise RuntimeError("Sets of files do not match")
 
+    def create_maps(self, *, directory: Path) -> None:
+        for dependency in self.dependencies:
+            for map in dependency.maps:
+                file = directory / dependency.name / map
+                file.parent.mkdir(exist_ok=True, parents=True)
+                file.touch(exist_ok=False)
+
 
 @dataclass
 class Dependency:
     name: str
     provider: Provider
     specifiers: SpecifierSet = SpecifierSet("")
     include_filter: Optional[Set[Pattern[str]]] = None
     resolved_version: Optional[Version] = None
     assets: Optional[Iterable[AssetFile]] = None
+    maps: Optional[List[str]] = None
 
     def __post_init__(self) -> None:
         if self.include_filter is not None:
             self.include_filter = {re.compile(f) for f in self.include_filter}
 
     def resolve_version(self, *, versions: Set[Version]) -> Version:
         if not versions:
@@ -372,14 +391,15 @@
             raise RuntimeError(f"The version is not set for {self.name}")
 
         return LockedDependency(
             name=self.name,
             version=str(self.resolved_version),
             provider=self.provider,
             assets=self.assets,
+            maps=[] if self.maps is None else self.maps,
         )
 
     async def update_assets(
         self, *, session: aiohttp.ClientSession, semaphore: asyncio.Semaphore
     ) -> None:
         versions = await self._find_versions(
             session=session, semaphore=semaphore
@@ -431,23 +451,45 @@
 
 def parse_lock_file(*, content: Dict[str, Any]) -> LockFile:
     lock_file = LockFile(
         dependencies=[LockedDependency(**d) for d in content["dependencies"]]
     )
 
     if lock_file.content != content:
-        raise ValueError("Lock files do not match")
+        raise ValueError(
+            f"Lock files do not match: {lock_file.content['content_hash']}"
+        )
 
     return lock_file
 
 
 def generate_lock_file(*, dependencies: Iterable[Dependency]) -> LockFile:
     return LockFile(dependencies=[d.locked for d in dependencies])
 
 
+async def parse_toml_file(*, content: str) -> LockFile:
+    document = tomlkit.parse(content)
+
+    dependencies = parse_dependencies(
+        dependencies=document["tool"]["amass"]["dependencies"]
+    )
+
+    semaphore = asyncio.Semaphore(value=CONCURRENT_REQUESTS)
+    async with aiohttp.ClientSession() as session:
+        tasks = [
+            dependency.update_assets(session=session, semaphore=semaphore)
+            for dependency in dependencies
+        ]
+        await asyncio.gather(*tasks)
+
+    lock_file = generate_lock_file(dependencies=dependencies)
+
+    return lock_file
+
+
 def parse_dependencies(
     *, dependencies: tomlkit.items.Table
 ) -> Iterable[Dependency]:
     parsed = []
 
     for name, meta in dependencies.items():
         include = meta.get("include")
@@ -460,17 +502,23 @@
         version = meta.get("version")
 
         if version == "*":
             version = ""
 
         provider = meta.get("provider", "cdnjs")
 
+        maps = list(meta.get("maps", []))
+
         parsed.append(
             Dependency(
                 name=name,
                 specifiers=SpecifierSet(version),
                 include_filter=include_filter,
                 provider=Provider[provider.upper()],
+                maps=maps,
             )
         )
 
     return parsed
+
+
+CONCURRENT_REQUESTS = 5
```

### Comparing `amass-0.3.1/amass/cli.py` & `amass-0.3.2/amass/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,17 +7,15 @@
 from typing import Any, Callable, Dict
 
 import aiohttp
 import click
 import tomlkit
 from pkg_resources import get_distribution
 
-from amass import generate_lock_file, parse_dependencies, parse_lock_file
-
-CONCURRENT_REQUESTS = 5
+from amass import CONCURRENT_REQUESTS, parse_lock_file, parse_toml_file
 
 
 def coroutine(f: Callable[..., Any]) -> Callable[..., Any]:
     @wraps(f)
     def wrapper(*args: Any, **kwargs: Any) -> Any:
         return asyncio.run(f(*args, **kwargs))
 
@@ -45,29 +43,15 @@
 
 @cli.command(name="lock", short_help="Lock the dependencies")
 @coroutine
 async def lock() -> None:
     with open("pyproject.toml") as f:
         content = f.read()
 
-    document = tomlkit.parse(content)
-
-    dependencies = parse_dependencies(
-        dependencies=document["tool"]["amass"]["dependencies"]
-    )
-
-    semaphore = asyncio.Semaphore(value=CONCURRENT_REQUESTS)
-    async with aiohttp.ClientSession() as session:
-        tasks = [
-            dependency.update_assets(session=session, semaphore=semaphore)
-            for dependency in dependencies
-        ]
-        await asyncio.gather(*tasks)
-
-    lock_file = generate_lock_file(dependencies=dependencies)
+    lock_file = await parse_toml_file(content=content)
 
     with open("amass.lock", "w") as f:
         f.write(json.dumps(lock_file.content, indent=2))
         f.write("\n")
 
 
 @cli.command(
@@ -89,14 +73,15 @@
             await asyncio.gather(
                 lock_file.download(
                     session=session, semaphore=semaphore, output_dir=tmp_path
                 )
             )
 
         lock_file.check_integrity(directory=tmp_path)
+        lock_file.create_maps(directory=tmp_path)
 
         output_dir = _get_settings()["output_dir"]
         if output_dir.exists():
             shutil.rmtree(output_dir)
 
         output_dir.parent.mkdir(parents=True, exist_ok=True)
         tmp_path.rename(output_dir)
```

### Comparing `amass-0.3.1/pyproject.toml` & `amass-0.3.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "amass"
-version = "0.3.1"
+version = "0.3.2"
 description = "Vendor libraries from cdnjs"
 authors = ["James Meakin <amass@jmsmkn.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/jmsmkn/amass"
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `amass-0.3.1/PKG-INFO` & `amass-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amass
-Version: 0.3.1
+Version: 0.3.2
 Summary: Vendor libraries from cdnjs
 Home-page: https://github.com/jmsmkn/amass
 License: Apache-2.0
 Author: James Meakin
 Author-email: amass@jmsmkn.com
 Requires-Python: >=3.8
 Classifier: Development Status :: 3 - Alpha
```

