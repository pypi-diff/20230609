# Comparing `tmp/packit_deploy-0.0.5.tar.gz` & `tmp/packit_deploy-0.0.6.tar.gz`

## Comparing `packit_deploy-0.0.5.tar` & `packit_deploy-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 packit_deploy-0.0.5/.github/workflows/test.yml
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 packit_deploy-0.0.5/config/basic/packit.yml
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 packit_deploy-0.0.5/config/noproxy/packit.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packit_deploy-0.0.5/src/__init__.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 packit_deploy-0.0.5/src/packit_deploy/__about__.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 packit_deploy-0.0.5/src/packit_deploy/__init__.py
--rw-r--r--   0        0        0     3851 2020-02-02 00:00:00.000000 packit_deploy-0.0.5/src/packit_deploy/cli.py
--rw-r--r--   0        0        0     2778 2020-02-02 00:00:00.000000 packit_deploy-0.0.5/src/packit_deploy/config.py
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 packit_deploy-0.0.5/src/packit_deploy/docker_helpers.py
--rw-r--r--   0        0        0     3801 2020-02-02 00:00:00.000000 packit_deploy-0.0.5/src/packit_deploy/packit_constellation.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 packit_deploy-0.0.5/tests/__init__.py
--rw-r--r--   0        0        0     4283 2020-02-02 00:00:00.000000 packit_deploy-0.0.5/tests/test_cli.py
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 packit_deploy-0.0.5/tests/test_config.py
--rw-r--r--   0        0        0     4618 2020-02-02 00:00:00.000000 packit_deploy-0.0.5/tests/test_integration.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 packit_deploy-0.0.5/.gitignore
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 packit_deploy-0.0.5/LICENSE.txt
--rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 packit_deploy-0.0.5/README.md
--rw-r--r--   0        0        0     3584 2020-02-02 00:00:00.000000 packit_deploy-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     3558 2020-02-02 00:00:00.000000 packit_deploy-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 packit_deploy-0.0.6/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 packit_deploy-0.0.6/config/basic/packit.yml
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 packit_deploy-0.0.6/config/noproxy/packit.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packit_deploy-0.0.6/src/__init__.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 packit_deploy-0.0.6/src/packit_deploy/__about__.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 packit_deploy-0.0.6/src/packit_deploy/__init__.py
+-rw-r--r--   0        0        0     3851 2020-02-02 00:00:00.000000 packit_deploy-0.0.6/src/packit_deploy/cli.py
+-rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 packit_deploy-0.0.6/src/packit_deploy/config.py
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 packit_deploy-0.0.6/src/packit_deploy/docker_helpers.py
+-rw-r--r--   0        0        0     3797 2020-02-02 00:00:00.000000 packit_deploy-0.0.6/src/packit_deploy/packit_constellation.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 packit_deploy-0.0.6/tests/__init__.py
+-rw-r--r--   0        0        0     4283 2020-02-02 00:00:00.000000 packit_deploy-0.0.6/tests/test_cli.py
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 packit_deploy-0.0.6/tests/test_config.py
+-rw-r--r--   0        0        0     4618 2020-02-02 00:00:00.000000 packit_deploy-0.0.6/tests/test_integration.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 packit_deploy-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 packit_deploy-0.0.6/LICENSE.txt
+-rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 packit_deploy-0.0.6/README.md
+-rw-r--r--   0        0        0     3584 2020-02-02 00:00:00.000000 packit_deploy-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     3558 2020-02-02 00:00:00.000000 packit_deploy-0.0.6/PKG-INFO
```

### Comparing `packit_deploy-0.0.5/.github/workflows/test.yml` & `packit_deploy-0.0.6/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `packit_deploy-0.0.5/config/basic/packit.yml` & `packit_deploy-0.0.6/config/basic/packit.yml`

 * *Files identical despite different names*

### Comparing `packit_deploy-0.0.5/config/noproxy/packit.yml` & `packit_deploy-0.0.6/config/noproxy/packit.yml`

 * *Files identical despite different names*

### Comparing `packit_deploy-0.0.5/src/packit_deploy/cli.py` & `packit_deploy-0.0.6/src/packit_deploy/cli.py`

 * *Files identical despite different names*

### Comparing `packit_deploy-0.0.5/src/packit_deploy/config.py` & `packit_deploy-0.0.6/src/packit_deploy/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import constellation
 from constellation import config
 
-from src.packit_deploy.docker_helpers import DockerClient
+from packit_deploy.docker_helpers import DockerClient
 
 
 class PackitConfig:
     def __init__(self, path, extra=None, options=None):
         dat = config.read_yaml(f"{path}/packit.yml")
         dat = config.config_build(path, dat, extra, options)
         self.network = config.config_string(dat, ["network"])
```

### Comparing `packit_deploy-0.0.5/src/packit_deploy/docker_helpers.py` & `packit_deploy-0.0.6/src/packit_deploy/docker_helpers.py`

 * *Files identical despite different names*

### Comparing `packit_deploy-0.0.5/src/packit_deploy/packit_constellation.py` & `packit_deploy-0.0.6/src/packit_deploy/packit_constellation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import constellation
 import docker
 from constellation import docker_util
 
-from src.packit_deploy.docker_helpers import DockerClient
+from packit_deploy.docker_helpers import DockerClient
 
 
 class PackitConstellation:
     def __init__(self, cfg):
         outpack = outpack_server_container(cfg)
         packit_db = packit_db_container(cfg)
         packit_api = packit_api_container(cfg)
```

### Comparing `packit_deploy-0.0.5/tests/test_cli.py` & `packit_deploy-0.0.6/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `packit_deploy-0.0.5/tests/test_config.py` & `packit_deploy-0.0.6/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `packit_deploy-0.0.5/tests/test_integration.py` & `packit_deploy-0.0.6/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `packit_deploy-0.0.5/LICENSE.txt` & `packit_deploy-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `packit_deploy-0.0.5/README.md` & `packit_deploy-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `packit_deploy-0.0.5/pyproject.toml` & `packit_deploy-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `packit_deploy-0.0.5/PKG-INFO` & `packit_deploy-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packit-deploy
-Version: 0.0.5
+Version: 0.0.6
 Project-URL: Documentation, https://github.com/mrc-ide/packit-deploy#readme
 Project-URL: Issues, https://github.com/mrc-ide/packit-deploy/issues
 Project-URL: Source, https://github.com/mrc-ide/packit-deploy
 Author-email: Alex Hill <alex.hill@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

