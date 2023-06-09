# Comparing `tmp/sekoia_automation_sdk-1.3.1.tar.gz` & `tmp/sekoia_automation_sdk-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sekoia_automation_sdk-1.3.1.tar", max compression
+gzip compressed data, was "sekoia_automation_sdk-1.3.2.tar", max compression
```

## Comparing `sekoia_automation_sdk-1.3.1.tar` & `sekoia_automation_sdk-1.3.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1066 2023-06-08 14:38:05.977886 sekoia_automation_sdk-1.3.1/LICENSE
--rw-r--r--   0        0        0     8422 2023-06-08 14:38:05.977886 sekoia_automation_sdk-1.3.1/README.md
--rw-r--r--   0        0        0     2114 2023-06-08 14:38:05.977886 sekoia_automation_sdk-1.3.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-08 14:38:05.977886 sekoia_automation_sdk-1.3.1/sekoia_automation/__init__.py
--rw-r--r--   0        0        0    11420 2023-06-08 14:38:05.977886 sekoia_automation_sdk-1.3.1/sekoia_automation/action.py
--rw-r--r--   0        0        0     4964 2023-06-08 14:38:05.977886 sekoia_automation_sdk-1.3.1/sekoia_automation/cli.py
--rw-r--r--   0        0        0      548 2023-06-08 14:38:05.977886 sekoia_automation_sdk-1.3.1/sekoia_automation/config.py
--rw-r--r--   0        0        0     6955 2023-06-08 14:38:05.977886 sekoia_automation_sdk-1.3.1/sekoia_automation/connector/__init__.py
--rw-r--r--   0        0        0     2313 2023-06-08 14:38:05.977886 sekoia_automation_sdk-1.3.1/sekoia_automation/connector/workers.py
--rw-r--r--   0        0        0      426 2023-06-08 14:38:05.977886 sekoia_automation_sdk-1.3.1/sekoia_automation/constants.py
--rw-r--r--   0        0        0      869 2023-06-08 14:38:05.977886 sekoia_automation_sdk-1.3.1/sekoia_automation/exceptions.py
--rw-r--r--   0        0        0      399 2023-06-08 14:38:05.977886 sekoia_automation_sdk-1.3.1/sekoia_automation/metrics/__init__.py
--rw-r--r--   0        0        0      383 2023-06-08 14:38:05.977886 sekoia_automation_sdk-1.3.1/sekoia_automation/metrics/base.py
--rw-r--r--   0        0        0     1185 2023-06-08 14:38:05.977886 sekoia_automation_sdk-1.3.1/sekoia_automation/metrics/prometheus.py
--rw-r--r--   0        0        0    15640 2023-06-08 14:38:05.977886 sekoia_automation_sdk-1.3.1/sekoia_automation/module.py
--rw-r--r--   0        0        0        0 2023-06-08 14:38:05.977886 sekoia_automation_sdk-1.3.1/sekoia_automation/scripts/__init__.py
--rw-r--r--   0        0        0     6605 2023-06-08 14:38:05.977886 sekoia_automation_sdk-1.3.1/sekoia_automation/scripts/documentation/generate.py
--rw-r--r--   0        0        0     2669 2023-06-08 14:38:05.977886 sekoia_automation_sdk-1.3.1/sekoia_automation/scripts/documentation/templates/module.md
--rw-r--r--   0        0        0     7581 2023-06-08 14:38:05.977886 sekoia_automation_sdk-1.3.1/sekoia_automation/scripts/files_generator.py
--rw-r--r--   0        0        0      144 2023-06-08 14:38:05.977886 sekoia_automation_sdk-1.3.1/sekoia_automation/scripts/new_module/template/cookiecutter.json
--rw-r--r--   0        0        0      301 2023-06-08 14:38:05.977886 sekoia_automation_sdk-1.3.1/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/Dockerfile
--rw-r--r--   0        0        0      225 2023-06-08 14:38:05.977886 sekoia_automation_sdk-1.3.1/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/main.py
--rw-r--r--   0        0        0      417 2023-06-08 14:38:05.977886 sekoia_automation_sdk-1.3.1/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/manifest.json
--rw-r--r--   0        0        0      647 2023-06-08 14:38:05.977886 sekoia_automation_sdk-1.3.1/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-08 14:38:05.977886 sekoia_automation_sdk-1.3.1/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/tests/__init__.py
--rw-r--r--   0        0        0      358 2023-06-08 14:38:05.977886 sekoia_automation_sdk-1.3.1/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/tests/conftest.py
--rw-r--r--   0        0        0      368 2023-06-08 14:38:05.977886 sekoia_automation_sdk-1.3.1/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/{{cookiecutter.module_name.lower().replace(" ", "_")}}_modules/__init__.py
--rw-r--r--   0        0        0      140 2023-06-08 14:38:05.977886 sekoia_automation_sdk-1.3.1/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/{{cookiecutter.module_name.lower().replace(" ", "_")}}_modules/models.py
--rw-r--r--   0        0        0    10011 2023-06-08 14:38:05.977886 sekoia_automation_sdk-1.3.1/sekoia_automation/scripts/openapi.py
--rwxr-xr-x   0        0        0    14390 2023-06-08 14:38:05.977886 sekoia_automation_sdk-1.3.1/sekoia_automation/scripts/sync_library.py
--rw-r--r--   0        0        0     6094 2023-06-08 14:38:05.977886 sekoia_automation_sdk-1.3.1/sekoia_automation/storage.py
--rw-r--r--   0        0        0    14267 2023-06-08 14:38:05.981886 sekoia_automation_sdk-1.3.1/sekoia_automation/trigger.py
--rw-r--r--   0        0        0     1294 2023-06-08 14:38:05.981886 sekoia_automation_sdk-1.3.1/sekoia_automation/utils.py
--rw-r--r--   0        0        0     9717 1970-01-01 00:00:00.000000 sekoia_automation_sdk-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-06-09 13:20:32.278060 sekoia_automation_sdk-1.3.2/LICENSE
+-rw-r--r--   0        0        0     8422 2023-06-09 13:20:32.278060 sekoia_automation_sdk-1.3.2/README.md
+-rw-r--r--   0        0        0     2114 2023-06-09 13:20:32.278060 sekoia_automation_sdk-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-09 13:20:32.278060 sekoia_automation_sdk-1.3.2/sekoia_automation/__init__.py
+-rw-r--r--   0        0        0    11420 2023-06-09 13:20:32.278060 sekoia_automation_sdk-1.3.2/sekoia_automation/action.py
+-rw-r--r--   0        0        0     5193 2023-06-09 13:20:32.278060 sekoia_automation_sdk-1.3.2/sekoia_automation/cli.py
+-rw-r--r--   0        0        0      548 2023-06-09 13:20:32.278060 sekoia_automation_sdk-1.3.2/sekoia_automation/config.py
+-rw-r--r--   0        0        0     6955 2023-06-09 13:20:32.278060 sekoia_automation_sdk-1.3.2/sekoia_automation/connector/__init__.py
+-rw-r--r--   0        0        0     2313 2023-06-09 13:20:32.278060 sekoia_automation_sdk-1.3.2/sekoia_automation/connector/workers.py
+-rw-r--r--   0        0        0      426 2023-06-09 13:20:32.278060 sekoia_automation_sdk-1.3.2/sekoia_automation/constants.py
+-rw-r--r--   0        0        0      869 2023-06-09 13:20:32.278060 sekoia_automation_sdk-1.3.2/sekoia_automation/exceptions.py
+-rw-r--r--   0        0        0      399 2023-06-09 13:20:32.278060 sekoia_automation_sdk-1.3.2/sekoia_automation/metrics/__init__.py
+-rw-r--r--   0        0        0      383 2023-06-09 13:20:32.278060 sekoia_automation_sdk-1.3.2/sekoia_automation/metrics/base.py
+-rw-r--r--   0        0        0     1185 2023-06-09 13:20:32.278060 sekoia_automation_sdk-1.3.2/sekoia_automation/metrics/prometheus.py
+-rw-r--r--   0        0        0    15640 2023-06-09 13:20:32.278060 sekoia_automation_sdk-1.3.2/sekoia_automation/module.py
+-rw-r--r--   0        0        0        0 2023-06-09 13:20:32.278060 sekoia_automation_sdk-1.3.2/sekoia_automation/scripts/__init__.py
+-rw-r--r--   0        0        0     6605 2023-06-09 13:20:32.278060 sekoia_automation_sdk-1.3.2/sekoia_automation/scripts/documentation/generate.py
+-rw-r--r--   0        0        0     2669 2023-06-09 13:20:32.278060 sekoia_automation_sdk-1.3.2/sekoia_automation/scripts/documentation/templates/module.md
+-rw-r--r--   0        0        0     7581 2023-06-09 13:20:32.278060 sekoia_automation_sdk-1.3.2/sekoia_automation/scripts/files_generator.py
+-rw-r--r--   0        0        0      144 2023-06-09 13:20:32.278060 sekoia_automation_sdk-1.3.2/sekoia_automation/scripts/new_module/template/cookiecutter.json
+-rw-r--r--   0        0        0      301 2023-06-09 13:20:32.278060 sekoia_automation_sdk-1.3.2/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/Dockerfile
+-rw-r--r--   0        0        0      225 2023-06-09 13:20:32.278060 sekoia_automation_sdk-1.3.2/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/main.py
+-rw-r--r--   0        0        0      417 2023-06-09 13:20:32.278060 sekoia_automation_sdk-1.3.2/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/manifest.json
+-rw-r--r--   0        0        0      708 2023-06-09 13:20:32.278060 sekoia_automation_sdk-1.3.2/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-09 13:20:32.278060 sekoia_automation_sdk-1.3.2/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/tests/__init__.py
+-rw-r--r--   0        0        0      358 2023-06-09 13:20:32.278060 sekoia_automation_sdk-1.3.2/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/tests/conftest.py
+-rw-r--r--   0        0        0      368 2023-06-09 13:20:32.278060 sekoia_automation_sdk-1.3.2/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/{{cookiecutter.module_name.lower().replace(" ", "_")}}_modules/__init__.py
+-rw-r--r--   0        0        0      140 2023-06-09 13:20:32.278060 sekoia_automation_sdk-1.3.2/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/{{cookiecutter.module_name.lower().replace(" ", "_")}}_modules/models.py
+-rw-r--r--   0        0        0    10011 2023-06-09 13:20:32.282060 sekoia_automation_sdk-1.3.2/sekoia_automation/scripts/openapi.py
+-rwxr-xr-x   0        0        0    13698 2023-06-09 13:20:32.282060 sekoia_automation_sdk-1.3.2/sekoia_automation/scripts/sync_library.py
+-rw-r--r--   0        0        0     6094 2023-06-09 13:20:32.282060 sekoia_automation_sdk-1.3.2/sekoia_automation/storage.py
+-rw-r--r--   0        0        0    14267 2023-06-09 13:20:32.282060 sekoia_automation_sdk-1.3.2/sekoia_automation/trigger.py
+-rw-r--r--   0        0        0     1294 2023-06-09 13:20:32.282060 sekoia_automation_sdk-1.3.2/sekoia_automation/utils.py
+-rw-r--r--   0        0        0     9717 1970-01-01 00:00:00.000000 sekoia_automation_sdk-1.3.2/PKG-INFO
```

### Comparing `sekoia_automation_sdk-1.3.1/LICENSE` & `sekoia_automation_sdk-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.1/README.md` & `sekoia_automation_sdk-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.1/pyproject.toml` & `sekoia_automation_sdk-1.3.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "sekoia-automation-sdk"
 
-version = "1.3.1"
+version = "1.3.2"
 description = "SDK to create SEKOIA.IO playbook modules"
 license = "MIT"
 readme = "README.md"
 authors = ["SEKOIA.IO"]
 packages = [
     { include = "sekoia_automation" },
 ]
```

### Comparing `sekoia_automation_sdk-1.3.1/sekoia_automation/action.py` & `sekoia_automation_sdk-1.3.2/sekoia_automation/action.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.1/sekoia_automation/cli.py` & `sekoia_automation_sdk-1.3.2/sekoia_automation/cli.py`

 * *Files 13% similar despite different names*

```diff
@@ -146,30 +146,34 @@
         ..., envvar="PLAYBOOK_API_KEY", help="Secret key to connect to the Playbook API"
     ),
     modules_path: Path = typer.Option(".", help="Path to the playbook modules"),
     module: str = typer.Option("", help="Module to deploy. Default to all modules"),
     check_image_on_registry: bool = typer.Option(
         False, help="Whether to check registry for existing image"
     ),
-    registry_pat: str = typer.Option(
-        "", envvar="REGISTRY_PAT", help="Docker registry personal access token"
+    registry: OptionalStr = typer.Option(
+        None, envvar="REGISTRY", help="Docker registry"
     ),
-    registry_user: str = typer.Option(
-        "", envvar="REGISTRY_USER", help="Docker registry username"
+    namespace: OptionalStr = typer.Option(
+        None, envvar="NAMESPACE", help="Docker namespace use by the images"
+    ),
+    registry_pat: OptionalStr = typer.Option(
+        None, envvar="REGISTRY_PAT", help="Docker registry personal access token"
     ),
 ):
     """
     Synchronize the module library to Sekoia.io
     """
     SyncLibrary(
-        playbook_url,
-        api_key,
-        modules_path,
-        registry_pat,
-        registry_user,
-        module,
-        check_image_on_registry,
+        playbook_url=playbook_url,
+        api_key=api_key,
+        modules_path=modules_path,
+        module=module,
+        registry_check=check_image_on_registry,
+        registry=registry,
+        namespace=namespace,
+        registry_pat=registry_pat,
     ).execute()
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `sekoia_automation_sdk-1.3.1/sekoia_automation/config.py` & `sekoia_automation_sdk-1.3.2/sekoia_automation/config.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.1/sekoia_automation/connector/__init__.py` & `sekoia_automation_sdk-1.3.2/sekoia_automation/connector/__init__.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.1/sekoia_automation/connector/workers.py` & `sekoia_automation_sdk-1.3.2/sekoia_automation/connector/workers.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.1/sekoia_automation/exceptions.py` & `sekoia_automation_sdk-1.3.2/sekoia_automation/exceptions.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.1/sekoia_automation/metrics/prometheus.py` & `sekoia_automation_sdk-1.3.2/sekoia_automation/metrics/prometheus.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.1/sekoia_automation/module.py` & `sekoia_automation_sdk-1.3.2/sekoia_automation/module.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.1/sekoia_automation/scripts/documentation/generate.py` & `sekoia_automation_sdk-1.3.2/sekoia_automation/scripts/documentation/generate.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.1/sekoia_automation/scripts/documentation/templates/module.md` & `sekoia_automation_sdk-1.3.2/sekoia_automation/scripts/documentation/templates/module.md`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.1/sekoia_automation/scripts/files_generator.py` & `sekoia_automation_sdk-1.3.2/sekoia_automation/scripts/files_generator.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.1/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/pyproject.toml` & `sekoia_automation_sdk-1.3.2/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -26,7 +26,13 @@
 line-length = 119
 target-version = ['py38']
 include = '\.pyi?$'
 
 [tool.isort]
 profile = "black"
 line_length = 119
+
+[tool.coverage.run]
+omit = [
+    "tests/*",
+    "main.py",
+]
```

### Comparing `sekoia_automation_sdk-1.3.1/sekoia_automation/scripts/openapi.py` & `sekoia_automation_sdk-1.3.2/sekoia_automation/scripts/openapi.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.1/sekoia_automation/scripts/sync_library.py` & `sekoia_automation_sdk-1.3.2/sekoia_automation/scripts/sync_library.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,49 +1,55 @@
 #!/usr/bin/env python3
 
 """
 Load module library into database via the API
 """
+import base64
 import json
 import re
 from base64 import b64encode
 from pathlib import Path
 from posixpath import join as urljoin
 from typing import Any
 
 import requests
 import typer
-from requests.auth import HTTPBasicAuth
 from rich import print
 
 
 class SyncLibrary:
-    DOCKER_PREFIX = "automation-module-"
+    DOCKER_REGISTRY = "ghcr.io"
+    DOCKER_NAMESPACE = "sekoia-io"
+    DOCKER_PREFIX = "automation-module"
 
     def __init__(
         self,
         playbook_url: str,
         api_key: str,
         modules_path: Path,
-        registry_pat: str | None = None,
-        registry_user: str | None = None,
         module: str = "",
         registry_check: bool = False,
+        registry: str | None = None,
+        namespace: str | None = None,
+        registry_pat: str | None = None,
     ):
-        self.registry_pat = registry_pat
-        self.registry_user = registry_user
         self.playbook_url = playbook_url
         self.api_key = api_key
         self.headers = {
             "Authorization": f"Bearer {self.api_key}",
             "Accept": "application/json",
         }
         self.modules_path = modules_path
         self.module = module
+
         self.registry_check = registry_check
+        self.registry = registry or self.DOCKER_REGISTRY
+        self.namespace = namespace or self.DOCKER_NAMESPACE
+        # In case of a public image any base64 encoded token works
+        self.registry_pat = registry_pat or "none"
 
     def pprint(
         self, created: list, updated: list, up_to_date: list, errors: list, nb_tabs: int
     ):
         """Pretty print information on the current sync
 
         Args:
@@ -259,68 +265,45 @@
             path_to_use = pnglogo_path
         else:
             return None
 
         with path_to_use.open("rb") as f:
             return f"{prefix}{b64encode(f.read()).decode('utf-8')}"
 
-    def check_image_on_registry(
-        self, docker_image: str, docker_image_version: str
-    ) -> bool:
+    def check_image_on_registry(self, docker_image: str, version: str) -> bool:
         """Checks if a Docker image exists on a registry
 
         If no registry is specified in the Module's manifest, we use a default value
         If the docker image name in the Module's manifest begins with a registry,
         this custom registry is used for the verification instead
         An image is considered to contain the registry path if it contains at least 2 /
         They delimit the path and the pathinfo fields
-        e.g. my_registry.com/v2/my_docker_image
+        e.g. my_registry.com/sekoia-io/my_docker_image
 
         Args:
             docker_image (str): Docker image name as specified in the manifest
-            docker_image_version (str): Docker image version
+            version (str): Docker image version
 
         Returns:
             bool: True if the image exists on the registry or if we don't have access
                 to a registry
                   False otherwise
         """
-        assert self.registry_user and self.registry_pat
-        auth = HTTPBasicAuth(self.registry_user, self.registry_pat)
-
         if match := re.match(r"(.*?)/(.*)/(.*)", docker_image):
-            registry_path = match[1]
-            registry_pathinfo = match[2]
+            registry = match[1]
+            namespace = match[2]
             image_name = match[3]
         else:
-            registry_path = "ghcr.io"
-            registry_pathinfo = "v2/sekoialab"
+            registry = self.registry
+            namespace = self.namespace
             image_name = docker_image
 
+        token = base64.b64encode(self.registry_pat.encode()).decode()
         response = requests.get(
-            f"https://{registry_path}/token",
-            params={
-                "service": registry_path,
-                "scope": "repository:<repo>:pull",
-                "client_id": "symphony-docker-image",
-            },
-            auth=auth,
-        )
-        if not response.ok:
-            print(
-                f"[bold red][!] Authentication against the docker registry "
-                f"failed with status {response.status_code}"
-            )
-            raise typer.Exit(code=1)
-
-        token = response.json()["token"]
-
-        response = requests.get(
-            f"https://{registry_path}/{registry_pathinfo}/{image_name}/manifests/\
-{docker_image_version}",
+            f"https://{registry}/v2/{namespace}/{image_name}/manifests/{version}",
             headers={
                 "Authorization": f"Bearer {token}",
                 "Accept": "application/vnd.docker.distribution.manifest.v2+json",
             },
         )
 
         return response.status_code == 200
@@ -400,20 +383,14 @@
 
         If the class was instanciated with the path to a given module, this method will
         attempt to load this module
 
         Otherwise, it will attempt to load all modules present in the library path
         specified
         """
-        if self.registry_check and not (self.registry_pat and self.registry_user):
-            print(
-                "[bold red][!] Credentials must be provided to check image in registry"
-            )
-            raise typer.Exit(code=1)
-
         if not self.module:
             library_path = self.modules_path.absolute()
             print("Library path: ", library_path)
             self.load(
                 library_path=library_path,
             )
         else:
@@ -421,9 +398,9 @@
                 module_path=self.modules_path.joinpath(self.module).absolute(),
             )
 
     def _get_module_docker_name(self, manifest: dict) -> str:
         if docker := manifest.get("docker"):
             return docker
         if slug := manifest.get("slug"):
-            return f"{self.DOCKER_PREFIX}{slug}"
+            return f"{self.registry}/{self.namespace}/{self.DOCKER_PREFIX}-{slug}"
         raise ValueError("Impossible to generate image name")
```

### Comparing `sekoia_automation_sdk-1.3.1/sekoia_automation/storage.py` & `sekoia_automation_sdk-1.3.2/sekoia_automation/storage.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.1/sekoia_automation/trigger.py` & `sekoia_automation_sdk-1.3.2/sekoia_automation/trigger.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.1/sekoia_automation/utils.py` & `sekoia_automation_sdk-1.3.2/sekoia_automation/utils.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.1/PKG-INFO` & `sekoia_automation_sdk-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sekoia-automation-sdk
-Version: 1.3.1
+Version: 1.3.2
 Summary: SDK to create SEKOIA.IO playbook modules
 Home-page: https://sekoia.io/
 License: MIT
 Keywords: SDK,SEKOIA.IO,automation,playbook
 Author: SEKOIA.IO
 Requires-Python: >=3.10,<3.12
 Classifier: Intended Audience :: Developers
```

