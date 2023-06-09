# Comparing `tmp/edwh_restic_plugin-0.2.7.tar.gz` & `tmp/edwh_restic_plugin-0.3.0.tar.gz`

## Comparing `edwh_restic_plugin-0.2.7.tar` & `edwh_restic_plugin-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     4912 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.7/CHANGELOG.md
--rwxr-xr-x   0        0        0      115 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.7/examples/captain-hooks/backup_files.sh
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.7/examples/captain-hooks/backup_minecraft.py
--rwxr-xr-x   0        0        0      593 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.7/examples/captain-hooks/backup_stream.sh
--rwxr-xr-x   0        0        0      279 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.7/examples/captain-hooks/backup_stream_sql.sh
--rwxr-xr-x   0        0        0      154 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.7/examples/captain-hooks/restore_files.sh
--rwxr-xr-x   0        0        0      439 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.7/examples/captain-hooks/restore_stream.sh
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.7/src/edwh_restic_plugin/__about__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.7/src/edwh_restic_plugin/__init__.py
--rw-r--r--   0        0        0    30288 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.7/src/edwh_restic_plugin/tasks.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.7/tests/__init__.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.7/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.7/LICENSE.txt
--rw-r--r--   0        0        0     6571 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.7/README.md
--rw-r--r--   0        0        0     3630 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     7629 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     5167 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.0/CHANGELOG.md
+-rwxr-xr-x   0        0        0      115 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.0/examples/captain-hooks/backup_files.sh
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.0/examples/captain-hooks/backup_minecraft.py
+-rwxr-xr-x   0        0        0      593 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.0/examples/captain-hooks/backup_stream.sh
+-rwxr-xr-x   0        0        0      279 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.0/examples/captain-hooks/backup_stream_sql.sh
+-rwxr-xr-x   0        0        0      154 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.0/examples/captain-hooks/restore_files.sh
+-rwxr-xr-x   0        0        0      439 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.0/examples/captain-hooks/restore_stream.sh
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.0/src/edwh_restic_plugin/__about__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.0/src/edwh_restic_plugin/__init__.py
+-rw-r--r--   0        0        0    30353 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.0/src/edwh_restic_plugin/tasks.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.0/LICENSE.txt
+-rw-r--r--   0        0        0     6571 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.0/README.md
+-rw-r--r--   0        0        0     3630 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     7629 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.0/PKG-INFO
```

### Comparing `edwh_restic_plugin-0.2.7/CHANGELOG.md` & `edwh_restic_plugin-0.3.0/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.3.0 (2023-06-09)
+### Feature
+* Edwh-restic-plugin now exist with the highest status code one of the given shell scripts gave it ([`281f600`](https://github.com/educationwarehouse/edwh-restic-plugin/commit/281f600082cba3853b1bc35efda93ea50ea8f3b5))
+
 ## v0.2.7 (2023-06-09)
 ### Fix
 * Made it now so it gets the result is captured even when throwing exception ([`fad076a`](https://github.com/educationwarehouse/edwh-restic-plugin/commit/fad076aab666925c2bb795a2705500215f7500c5))
 
 ## v0.2.6 (2023-06-09)
 ### Fix
 * Made it so the tasks.py doesn't throw an error when the shell throws an error. this is done by adding hide=verbose and removing the if vebose.... the reason also why we aren't using pty=true and warn=true is because pty=true NEVER prints to stderr(see https://docs.pyinvoke.org/en/stable/api/runners.html#invoke.runners.Runner.run and the the pty part) ([`ff4f819`](https://github.com/educationwarehouse/edwh-restic-plugin/commit/ff4f819a4df93889aad3b6155373cc17b42dcc02))
```

### Comparing `edwh_restic_plugin-0.2.7/examples/captain-hooks/backup_minecraft.py` & `edwh_restic_plugin-0.3.0/examples/captain-hooks/backup_minecraft.py`

 * *Files identical despite different names*

### Comparing `edwh_restic_plugin-0.2.7/examples/captain-hooks/backup_stream.sh` & `edwh_restic_plugin-0.3.0/examples/captain-hooks/backup_stream.sh`

 * *Files identical despite different names*

### Comparing `edwh_restic_plugin-0.2.7/src/edwh_restic_plugin/tasks.py` & `edwh_restic_plugin-0.3.0/src/edwh_restic_plugin/tasks.py`

 * *Files 0% similar despite different names*

```diff
@@ -179,45 +179,48 @@
             # run the script by default with pty=True, when the script crashes run the script again but then grab the stdout
 
             try:
                 print(f"{file} output:")
                 ran_script: invoke.runners.Result = c.run(file, hide=True, pty=True)
                 file_codes.append(0)
             except invoke.exceptions.UnexpectedExit as e:
-                file_codes.append(1)
                 ran_script = e.result
+                file_codes.append(e.result.exited)
 
             if verbose:
                 print(f"{file} output:")
                 if ran_script.stdout:
                     print(f"stdout:{ran_script.stdout}")
                 else:
                     print("no output found!")
 
             snapshot = self.get_snapshot_from(ran_script.stdout)
             snapshots_created.append(snapshot)
 
-        print("\n\nfile status codes")
-
-        for idx in range(len(file_codes)):
-            if file_codes[idx] == 0:
-                print(files[idx], tag="success", tag_color="green", color='white', format='underline')
-            else:
-                print("in", files[idx], tag="failure", tag_color="red", color='white', format='underline')
-
         # send message with backup. see message for more info
         # also if a tag in tags is None it will be removed by fix_tags
         if verb != "restore":
             tags = fix_tags(["message"] + snapshots_created)
             c.run(
                 f"restic {self.hostarg} -r {self.uri} backup --tag {','.join(tags)} --stdin --stdin-filename message",
                 in_stream=io.StringIO(message),
                 hide=True
             )
 
+        print("\n\nfile status codes:")
+
+        for idx in range(len(file_codes)):
+            if file_codes[idx] == 0:
+                print(files[idx], tag="success", tag_color="green", color='white')
+            else:
+                print("in", files[idx], tag="failure", tag_color="red", color='white')
+
+        if worst_status_code := max(file_codes) > 0:
+            exit(worst_status_code)
+
     def backup(self, c, verbose: bool, target: str, message: str):
         """
         Backs up the specified target.
 
         Args:
         - verbose (bool): A flag indicating whether to display verbose output.
         - target (str): The target of the backup.
```

### Comparing `edwh_restic_plugin-0.2.7/LICENSE.txt` & `edwh_restic_plugin-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edwh_restic_plugin-0.2.7/README.md` & `edwh_restic_plugin-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `edwh_restic_plugin-0.2.7/pyproject.toml` & `edwh_restic_plugin-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edwh_restic_plugin-0.2.7/PKG-INFO` & `edwh_restic_plugin-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edwh-restic-plugin
-Version: 0.2.7
+Version: 0.3.0
 Project-URL: Documentation, https://github.com/educationwarehouse/edwh-restic-plugin#readme
 Project-URL: Issues, https://github.com/educationwarehouse/edwh-restic-plugin/issues
 Project-URL: Source, https://github.com/educationwarehouse/edwh-restic-plugin
 Author-email: Remco Boerma <remco.b@educationwarehouse.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

