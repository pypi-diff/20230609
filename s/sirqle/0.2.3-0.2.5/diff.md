# Comparing `tmp/sirqle-0.2.3.tar.gz` & `tmp/sirqle-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sirqle-0.2.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "sirqle-0.2.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sirqle-0.2.3.tar` & `sirqle-0.2.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      683 2023-04-13 10:02:21.646915 sirqle-0.2.3/.github/workflows/bump.yml
--rw-r--r--   0        0        0     1917 2022-11-07 10:40:09.758048 sirqle-0.2.3/.gitignore
--rw-r--r--   0        0        0     1149 2023-04-12 17:02:21.974466 sirqle-0.2.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      636 2023-06-08 13:37:27.496997 sirqle-0.2.3/CHANGELOG.md
--rw-r--r--   0        0        0    11357 2023-05-16 15:49:30.858005 sirqle-0.2.3/LICENSE
--rw-r--r--   0        0        0     1089 2023-06-06 09:14:00.389308 sirqle-0.2.3/Makefile
--rw-r--r--   0        0        0     3341 2023-04-12 17:02:21.974466 sirqle-0.2.3/README.md
--rw-r--r--   0        0        0      846 2022-10-22 22:08:14.497554 sirqle-0.2.3/docs/gen_ref_pages.py
--rw-r--r--   0        0        0     1636 2023-04-12 17:02:21.974466 sirqle-0.2.3/docs/index.md
--rw-r--r--   0        0        0      153 2022-11-07 11:23:18.775395 sirqle-0.2.3/docs/reference.md
--rw-r--r--   0        0        0      155 2023-02-01 08:04:46.168879 sirqle-0.2.3/mkdocs.yml
--rw-r--r--   0        0        0     1337 2023-06-08 13:58:13.914115 sirqle-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      294 2023-02-01 08:04:46.164879 sirqle-0.2.3/requirements.txt
--rw-r--r--   0        0        0      884 2023-02-01 08:04:46.164879 sirqle-0.2.3/requirements_dev.txt
--rw-r--r--   0        0        0       38 2022-11-02 17:12:51.611854 sirqle-0.2.3/setup.py
--rw-r--r--   0        0        0      126 2023-04-12 17:01:06.634486 sirqle-0.2.3/src/sirqle/__init__.py
--rw-r--r--   0        0        0    10552 2023-06-08 13:57:47.026094 sirqle-0.2.3/src/sirqle/query.py
--rw-r--r--   0        0        0        0 2022-10-11 09:32:28.171344 sirqle-0.2.3/tests/__init__.py
--rw-r--r--   0        0        0     1208 2023-04-13 10:02:21.650915 sirqle-0.2.3/tests/test_create.py
--rw-r--r--   0        0        0     3447 2023-04-12 17:02:21.974466 sirqle-0.2.3/tests/test_insert.py
--rw-r--r--   0        0        0     4318 1970-01-01 00:00:00.000000 sirqle-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0      683 2023-04-13 10:02:21.646915 sirqle-0.2.5/.github/workflows/bump.yml
+-rw-r--r--   0        0        0     1917 2022-11-07 10:40:09.758048 sirqle-0.2.5/.gitignore
+-rw-r--r--   0        0        0     1149 2023-04-12 17:02:21.974466 sirqle-0.2.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      946 2023-06-09 17:07:33.977131 sirqle-0.2.5/CHANGELOG.md
+-rw-r--r--   0        0        0    11357 2023-05-16 15:49:30.858005 sirqle-0.2.5/LICENSE
+-rw-r--r--   0        0        0     1089 2023-06-06 09:14:00.389308 sirqle-0.2.5/Makefile
+-rw-r--r--   0        0        0     3341 2023-04-12 17:02:21.974466 sirqle-0.2.5/README.md
+-rw-r--r--   0        0        0      846 2022-10-22 22:08:14.497554 sirqle-0.2.5/docs/gen_ref_pages.py
+-rw-r--r--   0        0        0     1636 2023-04-12 17:02:21.974466 sirqle-0.2.5/docs/index.md
+-rw-r--r--   0        0        0      153 2022-11-07 11:23:18.775395 sirqle-0.2.5/docs/reference.md
+-rw-r--r--   0        0        0      155 2023-02-01 08:04:46.168879 sirqle-0.2.5/mkdocs.yml
+-rw-r--r--   0        0        0     1337 2023-06-09 17:07:32.205129 sirqle-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      294 2023-02-01 08:04:46.164879 sirqle-0.2.5/requirements.txt
+-rw-r--r--   0        0        0      884 2023-02-01 08:04:46.164879 sirqle-0.2.5/requirements_dev.txt
+-rw-r--r--   0        0        0       38 2022-11-02 17:12:51.611854 sirqle-0.2.5/setup.py
+-rw-r--r--   0        0        0      126 2023-04-12 17:01:06.634486 sirqle-0.2.5/src/sirqle/__init__.py
+-rw-r--r--   0        0        0    10952 2023-06-09 17:07:22.205124 sirqle-0.2.5/src/sirqle/query.py
+-rw-r--r--   0        0        0        0 2022-10-11 09:32:28.171344 sirqle-0.2.5/tests/__init__.py
+-rw-r--r--   0        0        0     1208 2023-04-13 10:02:21.650915 sirqle-0.2.5/tests/test_create.py
+-rw-r--r--   0        0        0     3447 2023-04-12 17:02:21.974466 sirqle-0.2.5/tests/test_insert.py
+-rw-r--r--   0        0        0     4318 1970-01-01 00:00:00.000000 sirqle-0.2.5/PKG-INFO
```

### Comparing `sirqle-0.2.3/.github/workflows/bump.yml` & `sirqle-0.2.5/.github/workflows/bump.yml`

 * *Files identical despite different names*

### Comparing `sirqle-0.2.3/.gitignore` & `sirqle-0.2.5/.gitignore`

 * *Files identical despite different names*

### Comparing `sirqle-0.2.3/.pre-commit-config.yaml` & `sirqle-0.2.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `sirqle-0.2.3/LICENSE` & `sirqle-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sirqle-0.2.3/Makefile` & `sirqle-0.2.5/Makefile`

 * *Files identical despite different names*

### Comparing `sirqle-0.2.3/README.md` & `sirqle-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `sirqle-0.2.3/docs/gen_ref_pages.py` & `sirqle-0.2.5/docs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `sirqle-0.2.3/docs/index.md` & `sirqle-0.2.5/docs/index.md`

 * *Files identical despite different names*

### Comparing `sirqle-0.2.3/pyproject.toml` & `sirqle-0.2.5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sirqle"
-version = "0.2.3"
+version = "0.2.5"
 authors = [{ name = "Pythia Dev Team", email = "dev@pythia.social" }]
 description = "SurrealDB Query interface"
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = ["python-dotenv", "surrealdb>=0.3.0"]
 license = { file = "LICENSE" }
 [project.urls]
@@ -49,15 +49,15 @@
 include_trailing_comma = true
 force_grid_wrap = 0
 use_parentheses = true
 ensure_newline_before_comments = true
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.2.3"
+version = "0.2.5"
 version_files = ["pyproject.toml:version"]
 tag_format = "v$version"
 bump_message = "bump: $current_version → $new_version [skip ci]"
 
 
 [tool.pytest.ini_options]
 testpaths = 'tests'
```

### Comparing `sirqle-0.2.3/requirements_dev.txt` & `sirqle-0.2.5/requirements_dev.txt`

 * *Files identical despite different names*

### Comparing `sirqle-0.2.3/src/sirqle/query.py` & `sirqle-0.2.5/src/sirqle/query.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 from typing import List, Optional, Tuple
 from urllib.parse import urlparse
 from warnings import warn
 
 from dotenv import dotenv_values
 from surrealdb.http import SurrealHTTP
-from surrealdb.ws import Surreal
+from surrealdb.ws import ConnectionState, Surreal
 
 PARAMS = ["URL", "NAMESPACE", "USERNAME", "PASSWORD", "DATABASE"]
 
 
 CLIENT = {
     "ws": Surreal,
     "wss": Surreal,
@@ -20,35 +20,33 @@
 }
 
 
 class Config:
     def __init__(
         self,
         env_file: str = ".db_conf",
-        client: Optional[SurrealHTTP] = None,
+        client: Optional[SurrealHTTP | Surreal] = None,
         url: Optional[str] = None,
         namespace: Optional[str] = None,
         database: Optional[str] = None,
         username: Optional[str] = None,
         password: Optional[str] = None,
     ) -> None:
         """Generate a Config class is used to configure the connection the database.
 
         It uses the `SurrealHTTP` client from the `surrealdb` library
 
         Args:
+            env_file: the name of an env file
+            client: a predefined Surreal client
             url: the URL to the database
             namespace: the namespace in the database
             database: the name of the database
             username: the username used for authentication
             password: the password used for authentication
-            client: an `SurrealHTTP` client configured beforehand
-            from_env: if it's set to True, it will load an `.db_conf`
-                file that has all the previous arguments set
-
         """
         if client:
             self.client = client
         elif os.path.isfile(env_file):
             conf = dotenv_values(env_file)
             if set(PARAMS).issubset(set(conf.keys())):
                 scheme = str(urlparse(conf["URL"]).scheme)
@@ -66,17 +64,23 @@
             )
         elif url:
             scheme = str(urlparse(url).scheme)
             if scheme in ["wss", "ws"]:
                 self.client = CLIENT[scheme](url=url)
 
     async def signup(self, user: str, password: str) -> str:
+        if isinstance(self.client, Surreal):
+            if self.client.client_state != ConnectionState.CONNECTED:
+                await self.client.connect()
         return await self.client.signup({"user": user, "pass": password})
 
     async def signin(self, user: str, password: str) -> str:
+        if isinstance(self.client, Surreal):
+            if self.client.client_state != ConnectionState.CONNECTED:
+                await self.client.connect()
         return await self.client.signin({"user": user, "pass": password})
 
 
 class Query:
     def __init__(self, config: Config | None = None):
         """Create a `Query` class
 
@@ -318,14 +322,17 @@
     def _end(self):
         self.query = self.query.strip()
         if self.query[-1] != ";":
             self.query += ";"
 
     async def _execute_query(self):
         self._end()
+        if isinstance(self.client, Surreal):
+            if self.client.client_state != ConnectionState.CONNECTED:
+                await self.client.connect()
         res = await self.client.query(self.query)
         self.last_query = self.query
         self.query = ""
         return res
 
     async def execute(self):
         """Execute the query.
```

### Comparing `sirqle-0.2.3/tests/test_create.py` & `sirqle-0.2.5/tests/test_create.py`

 * *Files identical despite different names*

### Comparing `sirqle-0.2.3/tests/test_insert.py` & `sirqle-0.2.5/tests/test_insert.py`

 * *Files identical despite different names*

### Comparing `sirqle-0.2.3/PKG-INFO` & `sirqle-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sirqle
-Version: 0.2.3
+Version: 0.2.5
 Summary: SurrealDB Query interface
 Author-email: Pythia Dev Team <dev@pythia.social>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: python-dotenv
 Requires-Dist: surrealdb>=0.3.0
 Requires-Dist: pre-commit ; extra == "dev"
```

