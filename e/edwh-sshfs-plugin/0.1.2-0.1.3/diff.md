# Comparing `tmp/edwh_sshfs_plugin-0.1.2.tar.gz` & `tmp/edwh_sshfs_plugin-0.1.3.tar.gz`

## Comparing `edwh_sshfs_plugin-0.1.2.tar` & `edwh_sshfs_plugin-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,24 @@
--rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.2/CHANGELOG.md
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.2/src/edwh_sshfs_plugin/__about__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.2/src/edwh_sshfs_plugin/__init__.py
--rw-r--r--   0        0        0     7927 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.2/src/edwh_sshfs_plugin/fabfile.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.2/tests/conftest.py
--rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.2/tests/test_sshfs.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.2/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.2/LICENSE.txt
--rw-r--r--   0        0        0     2135 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.2/README.md
--rw-r--r--   0        0        0     4102 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3364 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     4980 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.3/CHANGELOG.md
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.3/test.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.3/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.3/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.3/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.3/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.3/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.3/src/edwh_sshfs_plugin/__about__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.3/src/edwh_sshfs_plugin/__init__.py
+-rw-r--r--   0        0        0     7942 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.3/src/edwh_sshfs_plugin/fabfile.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.3/tests/conftest.py
+-rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.3/tests/test_sshfs.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.3/tests/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.3/tests/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.3/tests/.pytest_cache/README.md
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.3/tests/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.3/tests/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.3/tests/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.3/tests/sshfs_test_dir/hi.txt
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.3/LICENSE.txt
+-rw-r--r--   0        0        0     2135 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.3/README.md
+-rw-r--r--   0        0        0     4102 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3364 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.3/PKG-INFO
```

### Comparing `edwh_sshfs_plugin-0.1.2/CHANGELOG.md` & `edwh_sshfs_plugin-0.1.3/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.1.3 (2023-06-09)
+### Fix
+* Plumbum sshfs import could still give a sshfs import error. this is due to it for some reason not always giving a commandNotFound ([`0100f8f`](https://github.com/educationwarehouse/edwh-sshfs-plugin/commit/0100f8fa9ec664f1a07a269e8c89873560dbd139))
+
 ## v0.1.2 (2023-05-31)
 ### Fix
 * **import:** Don't crash the entire edwh tool if sshfs is not installed! ([`03b8365`](https://github.com/educationwarehouse/edwh-sshfs-plugin/commit/03b836576b36d3c814a9678ad0b98fd12a7e246f))
 
 ## v0.1.1 (2023-05-25)
 ### Fix
 * Set umask to highest permission level ([`c8c7362`](https://github.com/educationwarehouse/edwh-sshfs-plugin/commit/c8c7362b8ea77c0ec62672bdaaa798b388806c89))
```

### Comparing `edwh_sshfs_plugin-0.1.2/src/edwh_sshfs_plugin/fabfile.py` & `edwh_sshfs_plugin-0.1.3/src/edwh_sshfs_plugin/fabfile.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from plumbum import BG
 from plumbum.commands.processes import CommandNotFound
 from fabric import task
 import anyio
 
 try:
     from plumbum.cmd import ssh, sshfs
-except CommandNotFound:
+except (ImportError, CommandNotFound):
     warnings.warn("edwh sshfs plugin is installed but sshfs is missing. "
                   "Please check README.md#installation on how to fix this! "
                   "The commands in this plugin will NOT work unless this is fixed.")
 
 STOP_RUNNING = False
```

### Comparing `edwh_sshfs_plugin-0.1.2/tests/test_sshfs.py` & `edwh_sshfs_plugin-0.1.3/tests/test_sshfs.py`

 * *Files identical despite different names*

### Comparing `edwh_sshfs_plugin-0.1.2/LICENSE.txt` & `edwh_sshfs_plugin-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edwh_sshfs_plugin-0.1.2/README.md` & `edwh_sshfs_plugin-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `edwh_sshfs_plugin-0.1.2/pyproject.toml` & `edwh_sshfs_plugin-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edwh_sshfs_plugin-0.1.2/PKG-INFO` & `edwh_sshfs_plugin-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edwh-sshfs-plugin
-Version: 0.1.2
+Version: 0.1.3
 Summary: sshfs project with a plugin to be discovered from the edwh package
 Project-URL: Documentation, https://github.com/educationwarehouse/edwh-sshfs-plugin#readme
 Project-URL: Issues, https://github.com/educationwarehouse/edwh-sshfs-plugin/issues
 Project-URL: Source, https://github.com/educationwarehouse/edwh-sshfs-plugin
 Author-email: Remco Boerma <remco.b@educationwarehouse.nl>, Robin van der Noord <robin.vdn@educationwarehouse.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
```

