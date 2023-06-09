# Comparing `tmp/edwh_server_provisioning_plugin-0.3.0.tar.gz` & `tmp/edwh_server_provisioning_plugin-0.3.1.tar.gz`

## Comparing `edwh_server_provisioning_plugin-0.3.0.tar` & `edwh_server_provisioning_plugin-0.3.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    23482 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.3.0/.dcignore
--rw-r--r--   0        0        0    16037 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.3.0/CHANGELOG.md
--rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.3.0/old_documentation_in_dutch.md
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.3.0/src/edwh_server_provisioning_plugin/__about__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.3.0/src/edwh_server_provisioning_plugin/__init__.py
--rw-r--r--   0        0        0    46442 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.3.0/src/edwh_server_provisioning_plugin/server_provisioning_plugin.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.3.0/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.3.0/LICENSE.txt
--rw-r--r--   0        0        0     4332 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.3.0/readme.md
--rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    23482 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.3.1/.dcignore
+-rw-r--r--   0        0        0    16302 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.3.1/CHANGELOG.md
+-rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.3.1/old_documentation_in_dutch.md
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.3.1/src/edwh_server_provisioning_plugin/__about__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.3.1/src/edwh_server_provisioning_plugin/__init__.py
+-rw-r--r--   0        0        0    46741 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.3.1/src/edwh_server_provisioning_plugin/server_provisioning_plugin.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.3.1/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.3.1/LICENSE.txt
+-rw-r--r--   0        0        0     4332 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.3.1/readme.md
+-rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.3.1/PKG-INFO
```

### Comparing `edwh_server_provisioning_plugin-0.3.0/.dcignore` & `edwh_server_provisioning_plugin-0.3.1/.dcignore`

 * *Files identical despite different names*

### Comparing `edwh_server_provisioning_plugin-0.3.0/CHANGELOG.md` & `edwh_server_provisioning_plugin-0.3.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.3.1 (2023-06-09)
+### Fix
+* Added files_sizes which lists the file sizes from large to small with given head(amount of file to be listed) ([`d323b29`](https://github.com/educationwarehouse/server_provisioning/commit/d323b29f5a6ff9ed614f649ae82313846d6c7fd2))
+
 ## v0.3.0 (2023-05-01)
 ### Feature
 * **server_provisioning_plugin.py:** Add `install_generic_service` function to clone a generic-service repository without running `edwh setup` ([`c01f928`](https://github.com/educationwarehouse/server_provisioning/commit/c01f928634deb656dd58260f79ded41882e84749))
 
 ## v0.2.1 (2023-05-01)
 ### Fix
 * **do:** Use connection user instead of os user (for remote fab) ([`9b8de23`](https://github.com/educationwarehouse/server_provisioning/commit/9b8de238069c2f3f21097a608666788e67655b9a))
```

### Comparing `edwh_server_provisioning_plugin-0.3.0/old_documentation_in_dutch.md` & `edwh_server_provisioning_plugin-0.3.1/old_documentation_in_dutch.md`

 * *Files identical despite different names*

### Comparing `edwh_server_provisioning_plugin-0.3.0/src/edwh_server_provisioning_plugin/server_provisioning_plugin.py` & `edwh_server_provisioning_plugin-0.3.1/src/edwh_server_provisioning_plugin/server_provisioning_plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -443,14 +443,23 @@
 
 def execution_fails(c: Connection, argument: str) -> bool:
     "Returns true if the execution fails based on error level"
     return not executes_correctly(c, argument)
 
 
 @task
+def file_sizes(c, head: int = 20):
+    """
+    list the files from large to smallest
+    :param head: amount of files to be listed by the large file search
+    """
+    print("searching for large files...(this can take a minute)")
+    c.run(f"du -aBM 2>/dev/null | sort -nr | head -n {head}")
+
+@task
 def apt_install(c, packages):
     failsafe(lambda: c.sudo("apt install -y " + " ".join(packages)))
 
 
 @task
 def apt_upgrade(c, dist=False):
     failsafe(lambda: c.sudo("apt update -y"))
```

### Comparing `edwh_server_provisioning_plugin-0.3.0/LICENSE.txt` & `edwh_server_provisioning_plugin-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edwh_server_provisioning_plugin-0.3.0/pyproject.toml` & `edwh_server_provisioning_plugin-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edwh_server_provisioning_plugin-0.3.0/readme.md` & `edwh_server_provisioning_plugin-0.3.1/readme.md`

 * *Files identical despite different names*

### Comparing `edwh_server_provisioning_plugin-0.3.0/PKG-INFO` & `edwh_server_provisioning_plugin-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edwh-server-provisioning-plugin
-Version: 0.3.0
+Version: 0.3.1
 Summary: Fabric-based remote server management plugin for `edwh`
 Project-URL: Documentation, https://github.com/educationwarehouse/server_provisioning#readme
 Project-URL: Issues, https://github.com/educationwarehouse/server_provisioning/issues
 Project-URL: Source, https://github.com/educationwarehouse/server_provisioning
 Author-email: Remco Boerma <remco.b@educationwarehouse.nl>, Robin van der Noord <robin.vdn@educationwarehouse.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
```

