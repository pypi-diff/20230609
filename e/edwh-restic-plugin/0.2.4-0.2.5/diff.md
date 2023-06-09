# Comparing `tmp/edwh_restic_plugin-0.2.4.tar.gz` & `tmp/edwh_restic_plugin-0.2.5.tar.gz`

## Comparing `edwh_restic_plugin-0.2.4.tar` & `edwh_restic_plugin-0.2.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     3946 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.4/CHANGELOG.md
--rwxr-xr-x   0        0        0      115 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.4/examples/captain-hooks/backup_files.sh
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.4/examples/captain-hooks/backup_minecraft.py
--rwxr-xr-x   0        0        0      593 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.4/examples/captain-hooks/backup_stream.sh
--rwxr-xr-x   0        0        0      279 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.4/examples/captain-hooks/backup_stream_sql.sh
--rwxr-xr-x   0        0        0      154 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.4/examples/captain-hooks/restore_files.sh
--rwxr-xr-x   0        0        0      439 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.4/examples/captain-hooks/restore_stream.sh
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.4/src/edwh_restic_plugin/__about__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.4/src/edwh_restic_plugin/__init__.py
--rw-r--r--   0        0        0    30054 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.4/src/edwh_restic_plugin/tasks.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.4/tests/__init__.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.4/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.4/LICENSE.txt
--rw-r--r--   0        0        0     6571 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.4/README.md
--rw-r--r--   0        0        0     3630 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     7629 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     4176 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.5/CHANGELOG.md
+-rwxr-xr-x   0        0        0      115 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.5/examples/captain-hooks/backup_files.sh
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.5/examples/captain-hooks/backup_minecraft.py
+-rwxr-xr-x   0        0        0      593 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.5/examples/captain-hooks/backup_stream.sh
+-rwxr-xr-x   0        0        0      279 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.5/examples/captain-hooks/backup_stream_sql.sh
+-rwxr-xr-x   0        0        0      154 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.5/examples/captain-hooks/restore_files.sh
+-rwxr-xr-x   0        0        0      439 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.5/examples/captain-hooks/restore_stream.sh
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.5/src/edwh_restic_plugin/__about__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.5/src/edwh_restic_plugin/__init__.py
+-rw-r--r--   0        0        0    30094 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.5/src/edwh_restic_plugin/tasks.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.5/tests/__init__.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.5/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.5/LICENSE.txt
+-rw-r--r--   0        0        0     6571 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.5/README.md
+-rw-r--r--   0        0        0     3630 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     7629 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.5/PKG-INFO
```

### Comparing `edwh_restic_plugin-0.2.4/CHANGELOG.md` & `edwh_restic_plugin-0.2.5/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.2.5 (2023-06-09)
+### Fix
+* Fixed that the status codes of the [succes] and [failure] are a bit clearer ([`1d3fe77`](https://github.com/educationwarehouse/edwh-restic-plugin/commit/1d3fe773a7481811efff23ec0a5eade565c91caa))
+
 ## v0.2.4 (2023-06-09)
 ### Fix
 * Fixed a bug where it prints error and succes multiple times for the same file ([`4bfa7d2`](https://github.com/educationwarehouse/edwh-restic-plugin/commit/4bfa7d27c50097619a2620b6f38b27a0f217eb04))
 
 ## v0.2.3 (2023-06-09)
 ### Fix
 * Small updates to color-coding and clearer prints. also fixed a bug where a error will print for every sh script that failed ([`5c9f164`](https://github.com/educationwarehouse/edwh-restic-plugin/commit/5c9f1642ae25c084a426592fd6c4fca40ca9d5d7))
```

### Comparing `edwh_restic_plugin-0.2.4/examples/captain-hooks/backup_minecraft.py` & `edwh_restic_plugin-0.2.5/examples/captain-hooks/backup_minecraft.py`

 * *Files identical despite different names*

### Comparing `edwh_restic_plugin-0.2.4/examples/captain-hooks/backup_stream.sh` & `edwh_restic_plugin-0.2.5/examples/captain-hooks/backup_stream.sh`

 * *Files identical despite different names*

### Comparing `edwh_restic_plugin-0.2.4/src/edwh_restic_plugin/tasks.py` & `edwh_restic_plugin-0.2.5/src/edwh_restic_plugin/tasks.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,14 +189,16 @@
                     print(f"stderr:{ran_script.stderr}")
                 else:
                     print("no output found!")
 
             snapshot = self.get_snapshot_from(ran_script.stdout)
             snapshots_created.append(snapshot)
 
+        print("\n\nfile status codes")
+
         for idx in range(len(file_codes)):
             if file_codes[idx] == 0:
                 print(files[idx], tag="success", tag_color="green", color='white', format='underline')
             else:
                 print("in", files[idx], tag="failure", tag_color="red", color='white', format='underline')
 
         # send message with backup. see message for more info
```

### Comparing `edwh_restic_plugin-0.2.4/LICENSE.txt` & `edwh_restic_plugin-0.2.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edwh_restic_plugin-0.2.4/README.md` & `edwh_restic_plugin-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `edwh_restic_plugin-0.2.4/pyproject.toml` & `edwh_restic_plugin-0.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edwh_restic_plugin-0.2.4/PKG-INFO` & `edwh_restic_plugin-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edwh-restic-plugin
-Version: 0.2.4
+Version: 0.2.5
 Project-URL: Documentation, https://github.com/educationwarehouse/edwh-restic-plugin#readme
 Project-URL: Issues, https://github.com/educationwarehouse/edwh-restic-plugin/issues
 Project-URL: Source, https://github.com/educationwarehouse/edwh-restic-plugin
 Author-email: Remco Boerma <remco.b@educationwarehouse.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

