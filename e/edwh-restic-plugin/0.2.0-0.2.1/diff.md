# Comparing `tmp/edwh_restic_plugin-0.2.0.tar.gz` & `tmp/edwh_restic_plugin-0.2.1.tar.gz`

## Comparing `edwh_restic_plugin-0.2.0.tar` & `edwh_restic_plugin-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.0/CHANGELOG.md
--rwxr-xr-x   0        0        0      115 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.0/examples/captain-hooks/backup_files.sh
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.0/examples/captain-hooks/backup_minecraft.py
--rwxr-xr-x   0        0        0      593 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.0/examples/captain-hooks/backup_stream.sh
--rwxr-xr-x   0        0        0      279 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.0/examples/captain-hooks/backup_stream_sql.sh
--rwxr-xr-x   0        0        0      154 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.0/examples/captain-hooks/restore_files.sh
--rwxr-xr-x   0        0        0      439 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.0/examples/captain-hooks/restore_stream.sh
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.0/src/edwh_restic_plugin/__about__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.0/src/edwh_restic_plugin/__init__.py
--rw-r--r--   0        0        0    29512 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.0/src/edwh_restic_plugin/tasks.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.0/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.0/LICENSE.txt
--rw-r--r--   0        0        0     6571 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.0/README.md
--rw-r--r--   0        0        0     3613 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     7602 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     3217 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.1/CHANGELOG.md
+-rwxr-xr-x   0        0        0      115 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.1/examples/captain-hooks/backup_files.sh
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.1/examples/captain-hooks/backup_minecraft.py
+-rwxr-xr-x   0        0        0      593 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.1/examples/captain-hooks/backup_stream.sh
+-rwxr-xr-x   0        0        0      279 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.1/examples/captain-hooks/backup_stream_sql.sh
+-rwxr-xr-x   0        0        0      154 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.1/examples/captain-hooks/restore_files.sh
+-rwxr-xr-x   0        0        0      439 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.1/examples/captain-hooks/restore_stream.sh
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.1/src/edwh_restic_plugin/__about__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.1/src/edwh_restic_plugin/__init__.py
+-rw-r--r--   0        0        0    29514 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.1/src/edwh_restic_plugin/tasks.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.1/tests/__init__.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.1/LICENSE.txt
+-rw-r--r--   0        0        0     6571 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.1/README.md
+-rw-r--r--   0        0        0     3613 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     7602 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.2.1/PKG-INFO
```

### Comparing `edwh_restic_plugin-0.2.0/CHANGELOG.md` & `edwh_restic_plugin-0.2.1/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.2.1 (2023-06-09)
+### Fix
+* Automatically using verbose and now always hiding restic message ([`7d6537f`](https://github.com/educationwarehouse/edwh-restic-plugin/commit/7d6537f800230c076b07996e454556620e6888c8))
+
 ## v0.2.0 (2023-05-24)
 ### Feature
 * Added restic.run, this sets up a restic enviroment with the connection choice of your choosing. this allows you to run restic commands without giving up some env variables to restic(like the $HOST or $URI). every command that is ran prints the stdout and err to the screen ([`9199495`](https://github.com/educationwarehouse/edwh-restic-plugin/commit/9199495bc2c70bf11fbd16fc7c56864b7fff99a3))
 
 ## v0.1.7 (2023-05-24)
 ### Fix
 * Added pty for verbosity sometimes not giving output ([`c876af0`](https://github.com/educationwarehouse/edwh-restic-plugin/commit/c876af0fa60626837e56b4d643366cb30966212f))
```

### Comparing `edwh_restic_plugin-0.2.0/examples/captain-hooks/backup_minecraft.py` & `edwh_restic_plugin-0.2.1/examples/captain-hooks/backup_minecraft.py`

 * *Files identical despite different names*

### Comparing `edwh_restic_plugin-0.2.0/examples/captain-hooks/backup_stream.sh` & `edwh_restic_plugin-0.2.1/examples/captain-hooks/backup_stream.sh`

 * *Files identical despite different names*

### Comparing `edwh_restic_plugin-0.2.0/src/edwh_restic_plugin/tasks.py` & `edwh_restic_plugin-0.2.1/src/edwh_restic_plugin/tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,14 +188,15 @@
         # send message with backup. see message for more info
         # also if a tag in tags is None it will be removed by fix_tags
         if verb != "restore":
             tags = fix_tags(["message"] + snapshots_created)
             c.run(
                 f"restic {self.hostarg} -r {self.uri} backup --tag {','.join(tags)} --stdin --stdin-filename message",
                 in_stream=io.StringIO(message),
+                hide=True
             )
 
     def backup(self, c, verbose: bool, target: str, message: str):
         """
         Backs up the specified target.
 
         Args:
@@ -275,15 +276,14 @@
                 hide=True,
                 warn=True,
             ).stdout
             message = restore_output.strip()
             stdout = re.sub(
                 rf"\n{snapshot}(.*)\n", rf"\n{snapshot}\1 : [{message}]\n", stdout
             )
-        print(stdout)
 
 
 class LocalRepository(Repository):
     def __init__(self):
         super().__init__()
         self.password = None
         self.name = None
@@ -718,15 +718,15 @@
     # It has been decided to create a main path called 'backups' for each repository.
     # This can be changed or removed if desired.
     # A password is only passed with a few functions.
     cli_repo(connection_choice, restichostname).configure(c)
 
 
 @task
-def backup(c, target="", connection_choice=None, message=None, verbose=False):
+def backup(c, target="", connection_choice=None, message=None, verbose=True):
     """Performs a backup operation using restic on a local or remote/cloud file system.
 
     Args:
         target (str): The path of the file or directory to backup. Defaults to an empty string.
         connection_choice (str): The name of the connection to use for the backup.
             Defaults to None, which means the default connection will be used.
         message (str): A message to attach to the backup snapshot.
@@ -752,15 +752,15 @@
     # --exclude-larger-than 'size', Specified once to excludes files larger than the given size.
     # Please see 'restic help backup' for more specific information about each exclude option.
 
     cli_repo(connection_choice).backup(c, verbose, target, message)
 
 
 @task
-def restore(c, connection_choice=None, snapshot="latest", target="", verbose=False):
+def restore(c, connection_choice=None, snapshot="latest", target="", verbose=True):
     """
     The restore function restores the latest backed-up files by default and puts them in a restore folder.
 
     IMPORTANT: please provide -t for the path where the restore should go. Also remember to include -c for the service
     where the backup is stored.
 
     :param connection_choice: the service where the files are backed up, e.g., 'local' or 'openstack'.
```

### Comparing `edwh_restic_plugin-0.2.0/LICENSE.txt` & `edwh_restic_plugin-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edwh_restic_plugin-0.2.0/README.md` & `edwh_restic_plugin-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `edwh_restic_plugin-0.2.0/pyproject.toml` & `edwh_restic_plugin-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edwh_restic_plugin-0.2.0/PKG-INFO` & `edwh_restic_plugin-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edwh-restic-plugin
-Version: 0.2.0
+Version: 0.2.1
 Project-URL: Documentation, https://github.com/educationwarehouse/edwh-restic-plugin#readme
 Project-URL: Issues, https://github.com/educationwarehouse/edwh-restic-plugin/issues
 Project-URL: Source, https://github.com/educationwarehouse/edwh-restic-plugin
 Author-email: Remco Boerma <remco.b@educationwarehouse.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

