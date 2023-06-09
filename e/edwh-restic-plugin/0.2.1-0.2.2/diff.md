# Comparing `tmp/edwh_restic_plugin-0.2.1.tar.gz` & `tmp/edwh_restic_plugin-0.2.2.tar.gz`

## Comparing `edwh_restic_plugin-0.2.1.tar` & `edwh_restic_plugin-0.2.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     3217 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.1/CHANGELOG.md
--rwxr-xr-x   0        0        0      115 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.1/examples/captain-hooks/backup_files.sh
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.1/examples/captain-hooks/backup_minecraft.py
--rwxr-xr-x   0        0        0      593 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.1/examples/captain-hooks/backup_stream.sh
--rwxr-xr-x   0        0        0      279 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.1/examples/captain-hooks/backup_stream_sql.sh
--rwxr-xr-x   0        0        0      154 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.1/examples/captain-hooks/restore_files.sh
--rwxr-xr-x   0        0        0      439 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.1/examples/captain-hooks/restore_stream.sh
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.1/src/edwh_restic_plugin/__about__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.1/src/edwh_restic_plugin/__init__.py
--rw-r--r--   0        0        0    29514 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.1/src/edwh_restic_plugin/tasks.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.1/tests/__init__.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.1/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.1/LICENSE.txt
--rw-r--r--   0        0        0     6571 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.1/README.md
--rw-r--r--   0        0        0     3613 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     7602 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     3436 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.2/CHANGELOG.md
+-rwxr-xr-x   0        0        0      115 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.2/examples/captain-hooks/backup_files.sh
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.2/examples/captain-hooks/backup_minecraft.py
+-rwxr-xr-x   0        0        0      593 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.2/examples/captain-hooks/backup_stream.sh
+-rwxr-xr-x   0        0        0      279 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.2/examples/captain-hooks/backup_stream_sql.sh
+-rwxr-xr-x   0        0        0      154 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.2/examples/captain-hooks/restore_files.sh
+-rwxr-xr-x   0        0        0      439 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.2/examples/captain-hooks/restore_stream.sh
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.2/src/edwh_restic_plugin/__about__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.2/src/edwh_restic_plugin/__init__.py
+-rw-r--r--   0        0        0    30228 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.2/src/edwh_restic_plugin/tasks.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.2/tests/__init__.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.2/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.2/LICENSE.txt
+-rw-r--r--   0        0        0     6571 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.2/README.md
+-rw-r--r--   0        0        0     3630 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     7629 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.2/PKG-INFO
```

### Comparing `edwh_restic_plugin-0.2.1/CHANGELOG.md` & `edwh_restic_plugin-0.2.2/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.2.2 (2023-06-09)
+### Fix
+* Made verbosity better when running files using backup or restore ([`cf37f24`](https://github.com/educationwarehouse/edwh-restic-plugin/commit/cf37f2480e188a58a79c33a1e3cf4ba2ce2802c9))
+
 ## v0.2.1 (2023-06-09)
 ### Fix
 * Automatically using verbose and now always hiding restic message ([`7d6537f`](https://github.com/educationwarehouse/edwh-restic-plugin/commit/7d6537f800230c076b07996e454556620e6888c8))
 
 ## v0.2.0 (2023-05-24)
 ### Feature
 * Added restic.run, this sets up a restic enviroment with the connection choice of your choosing. this allows you to run restic commands without giving up some env variables to restic(like the $HOST or $URI). every command that is ran prints the stdout and err to the screen ([`9199495`](https://github.com/educationwarehouse/edwh-restic-plugin/commit/9199495bc2c70bf11fbd16fc7c56864b7fff99a3))
```

### Comparing `edwh_restic_plugin-0.2.1/examples/captain-hooks/backup_minecraft.py` & `edwh_restic_plugin-0.2.2/examples/captain-hooks/backup_minecraft.py`

 * *Files identical despite different names*

### Comparing `edwh_restic_plugin-0.2.1/examples/captain-hooks/backup_stream.sh` & `edwh_restic_plugin-0.2.2/examples/captain-hooks/backup_stream.sh`

 * *Files identical despite different names*

### Comparing `edwh_restic_plugin-0.2.1/src/edwh_restic_plugin/tasks.py` & `edwh_restic_plugin-0.2.2/src/edwh_restic_plugin/tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import io
 import os
 from pathlib import Path
 import re
 import sys
 import typing
 import json
+from print_color import print
 
 from tqdm import tqdm
 
 # the path where the restic command is going to be executed
 DEFAULT_BACKUP_FOLDER = Path("captain-hooks")
 # the path where the environment variables are going
 DOTENV = Path(".env")
@@ -165,27 +166,42 @@
         # set MSG in environment for sh files
         os.environ["MSG"] = message
 
         # get files by target and verb. see self.get_scripts for more info
         files = self.get_scripts(target, verb)
 
         snapshots_created = []
+        file_codes = []
         # run all backup/restore files
         for file in tqdm(files):
             if verbose:
-                print("running", file)
-
-            ran_script = c.run(file, hide=True, warn=True, pty=True)
+                print("\033[1m running", file, "\033[0m")
 
+            try:
+                ran_script = c.run(file, hide=True, pty=True)
+                file_codes.append(0)
+            except:
+                file_codes.append(1)
+                print("in", file, tag="failure", tag_color="red", color='white', format='underline', background='grey')
             if verbose:
                 print(f"{file} output:")
-                if ran_script.stdout or ran_script.stderr:
-                    print(f"out:{ran_script.stdout}\nerr:{ran_script.stderr}")
+                if ran_script.stdout:
+                    print(f"out:{ran_script.stdout}")
+                elif ran_script.stderr:
+                    print(f"err:{ran_script.stderr}")
                 else:
                     print("no output found!")
+
+            for file_code in file_codes:
+                if file_code == 0:
+                    print(file, tag="success", tag_color="green", color='white', format='underline', background='grey')
+                else:
+                    print("in", file, tag="failure", tag_color="red", color='white', format='underline',
+                          background='grey')
+
             snapshot = self.get_snapshot_from(ran_script.stdout)
             snapshots_created.append(snapshot)
 
         # send message with backup. see message for more info
         # also if a tag in tags is None it will be removed by fix_tags
         if verb != "restore":
             tags = fix_tags(["message"] + snapshots_created)
```

### Comparing `edwh_restic_plugin-0.2.1/LICENSE.txt` & `edwh_restic_plugin-0.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edwh_restic_plugin-0.2.1/README.md` & `edwh_restic_plugin-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `edwh_restic_plugin-0.2.1/pyproject.toml` & `edwh_restic_plugin-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
   "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   'invoke',
   'tqdm',
+  'print-color',
   'diceware'
 ]
 
 [project.optional-dependencies]
 dev = [
   "hatch",
   # "python-semantic-release >= 8.0.0a5",
```

### Comparing `edwh_restic_plugin-0.2.1/PKG-INFO` & `edwh_restic_plugin-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edwh-restic-plugin
-Version: 0.2.1
+Version: 0.2.2
 Project-URL: Documentation, https://github.com/educationwarehouse/edwh-restic-plugin#readme
 Project-URL: Issues, https://github.com/educationwarehouse/edwh-restic-plugin/issues
 Project-URL: Source, https://github.com/educationwarehouse/edwh-restic-plugin
 Author-email: Remco Boerma <remco.b@educationwarehouse.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Requires-Dist: diceware
 Requires-Dist: invoke
+Requires-Dist: print-color
 Requires-Dist: tqdm
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: hatch; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # edwh-restic-plugin
```

