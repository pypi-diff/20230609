# Comparing `tmp/edwh_restic_plugin-0.2.5.tar.gz` & `tmp/edwh_restic_plugin-0.2.6.tar.gz`

## Comparing `edwh_restic_plugin-0.2.5.tar` & `edwh_restic_plugin-0.2.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     4176 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.5/CHANGELOG.md
--rwxr-xr-x   0        0        0      115 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.5/examples/captain-hooks/backup_files.sh
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.5/examples/captain-hooks/backup_minecraft.py
--rwxr-xr-x   0        0        0      593 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.5/examples/captain-hooks/backup_stream.sh
--rwxr-xr-x   0        0        0      279 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.5/examples/captain-hooks/backup_stream_sql.sh
--rwxr-xr-x   0        0        0      154 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.5/examples/captain-hooks/restore_files.sh
--rwxr-xr-x   0        0        0      439 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.5/examples/captain-hooks/restore_stream.sh
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.5/src/edwh_restic_plugin/__about__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.5/src/edwh_restic_plugin/__init__.py
--rw-r--r--   0        0        0    30094 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.5/src/edwh_restic_plugin/tasks.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.5/tests/__init__.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.5/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.5/LICENSE.txt
--rw-r--r--   0        0        0     6571 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.5/README.md
--rw-r--r--   0        0        0     3630 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     7629 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     4683 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.6/CHANGELOG.md
+-rwxr-xr-x   0        0        0      115 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.6/examples/captain-hooks/backup_files.sh
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.6/examples/captain-hooks/backup_minecraft.py
+-rwxr-xr-x   0        0        0      593 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.6/examples/captain-hooks/backup_stream.sh
+-rwxr-xr-x   0        0        0      279 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.6/examples/captain-hooks/backup_stream_sql.sh
+-rwxr-xr-x   0        0        0      154 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.6/examples/captain-hooks/restore_files.sh
+-rwxr-xr-x   0        0        0      439 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.6/examples/captain-hooks/restore_stream.sh
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.6/src/edwh_restic_plugin/__about__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.6/src/edwh_restic_plugin/__init__.py
+-rw-r--r--   0        0        0    30010 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.6/src/edwh_restic_plugin/tasks.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.6/tests/__init__.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.6/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.6/LICENSE.txt
+-rw-r--r--   0        0        0     6571 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.6/README.md
+-rw-r--r--   0        0        0     3630 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     7629 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.6/PKG-INFO
```

### Comparing `edwh_restic_plugin-0.2.5/CHANGELOG.md` & `edwh_restic_plugin-0.2.6/CHANGELOG.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.2.6 (2023-06-09)
+### Fix
+* Made it so the tasks.py doesn't throw an error when the shell throws an error. this is done by adding hide=verbose and removing the if vebose.... the reason also why we aren't using pty=true and warn=true is because pty=true NEVER prints to stderr(see https://docs.pyinvoke.org/en/stable/api/runners.html#invoke.runners.Runner.run and the the pty part) ([`ff4f819`](https://github.com/educationwarehouse/edwh-restic-plugin/commit/ff4f819a4df93889aad3b6155373cc17b42dcc02))
+
 ## v0.2.5 (2023-06-09)
 ### Fix
 * Fixed that the status codes of the [succes] and [failure] are a bit clearer ([`1d3fe77`](https://github.com/educationwarehouse/edwh-restic-plugin/commit/1d3fe773a7481811efff23ec0a5eade565c91caa))
 
 ## v0.2.4 (2023-06-09)
 ### Fix
 * Fixed a bug where it prints error and succes multiple times for the same file ([`4bfa7d2`](https://github.com/educationwarehouse/edwh-restic-plugin/commit/4bfa7d27c50097619a2620b6f38b27a0f217eb04))
```

### Comparing `edwh_restic_plugin-0.2.5/examples/captain-hooks/backup_minecraft.py` & `edwh_restic_plugin-0.2.6/examples/captain-hooks/backup_minecraft.py`

 * *Files identical despite different names*

### Comparing `edwh_restic_plugin-0.2.5/examples/captain-hooks/backup_stream.sh` & `edwh_restic_plugin-0.2.6/examples/captain-hooks/backup_stream.sh`

 * *Files identical despite different names*

### Comparing `edwh_restic_plugin-0.2.5/src/edwh_restic_plugin/tasks.py` & `edwh_restic_plugin-0.2.6/src/edwh_restic_plugin/tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,15 +131,15 @@
             print("no files found with target:", target)
             sys.exit(255)
 
         return files
 
     def execute_files(
         self,
-        c,
+        c: invoke.context.Context,
         target: str,
         verb: str,
         verbose: bool,
         message: str = None,
         snapshot: str = "latest",
     ):
         """
@@ -172,27 +172,22 @@
         snapshots_created = []
         file_codes = []
         # run all backup/restore files
         for file in tqdm(files):
             if verbose:
                 print("\033[1m running", file, "\033[0m")
 
+            # run the script by default with pty=True, when the script crashes run the script again but then grab the stdout
             try:
-                ran_script = c.run(file, hide=True, pty=True)
+                print(f"{file} output:")
+                ran_script: invoke.runners.Result = c.run(file, hide=verbose, pty=True)
                 file_codes.append(0)
             except:
                 file_codes.append(1)
-            if verbose:
-                print(f"{file} output:")
-                if ran_script.stdout:
-                    print(f"stdout:{ran_script.stdout}")
-                elif ran_script.stderr:
-                    print(f"stderr:{ran_script.stderr}")
-                else:
-                    print("no output found!")
+                continue
 
             snapshot = self.get_snapshot_from(ran_script.stdout)
             snapshots_created.append(snapshot)
 
         print("\n\nfile status codes")
 
         for idx in range(len(file_codes)):
```

### Comparing `edwh_restic_plugin-0.2.5/LICENSE.txt` & `edwh_restic_plugin-0.2.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edwh_restic_plugin-0.2.5/README.md` & `edwh_restic_plugin-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `edwh_restic_plugin-0.2.5/pyproject.toml` & `edwh_restic_plugin-0.2.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edwh_restic_plugin-0.2.5/PKG-INFO` & `edwh_restic_plugin-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edwh-restic-plugin
-Version: 0.2.5
+Version: 0.2.6
 Project-URL: Documentation, https://github.com/educationwarehouse/edwh-restic-plugin#readme
 Project-URL: Issues, https://github.com/educationwarehouse/edwh-restic-plugin/issues
 Project-URL: Source, https://github.com/educationwarehouse/edwh-restic-plugin
 Author-email: Remco Boerma <remco.b@educationwarehouse.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

