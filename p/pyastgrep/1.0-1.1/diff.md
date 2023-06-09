# Comparing `tmp/pyastgrep-1.0.tar.gz` & `tmp/pyastgrep-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyastgrep-1.0.tar", last modified: Mon Apr 17 15:42:17 2023, max compression
+gzip compressed data, was "pyastgrep-1.1.tar", last modified: Fri Jun  9 13:42:58 2023, max compression
```

## Comparing `pyastgrep-1.0.tar` & `pyastgrep-1.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-04-17 15:42:17.788971 pyastgrep-1.0/
--rw-r--r--   0 luke      (1000) luke      (1000)      378 2022-10-17 13:09:58.000000 pyastgrep-1.0/.gitattributes
--rw-r--r--   0 luke      (1000) luke      (1000)     1771 2022-11-07 12:01:43.000000 pyastgrep-1.0/.gitignore
--rw-rw-rw-   0 luke      (1000) luke      (1000)    14968 2023-04-17 15:42:17.788971 pyastgrep-1.0/PKG-INFO
--rw-r--r--   0 luke      (1000) luke      (1000)    14121 2023-02-20 15:44:13.000000 pyastgrep-1.0/README.rst
--rw-r--r--   0 luke      (1000) luke      (1000)      755 2023-04-17 15:02:16.000000 pyastgrep-1.0/pyproject.toml
--rw-r--r--   0 luke      (1000) luke      (1000)     1135 2023-04-17 15:42:17.788971 pyastgrep-1.0/setup.cfg
--rw-r--r--   0 luke      (1000) luke      (1000)       38 2022-10-21 16:01:47.000000 pyastgrep-1.0/setup.py
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-04-17 15:42:17.784970 pyastgrep-1.0/src/
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-04-17 15:42:17.788971 pyastgrep-1.0/src/pyastgrep/
--rw-r--r--   0 luke      (1000) luke      (1000)       20 2023-04-17 15:41:15.000000 pyastgrep-1.0/src/pyastgrep/__init__.py
--rw-r--r--   0 luke      (1000) luke      (1000)     3158 2022-11-18 11:57:27.000000 pyastgrep-1.0/src/pyastgrep/asts.py
--rw-r--r--   0 luke      (1000) luke      (1000)     3930 2022-11-16 20:46:57.000000 pyastgrep-1.0/src/pyastgrep/cli.py
--rw-r--r--   0 luke      (1000) luke      (1000)      890 2022-11-25 07:36:32.000000 pyastgrep-1.0/src/pyastgrep/dump.py
--rw-r--r--   0 luke      (1000) luke      (1000)     3244 2023-02-20 15:43:43.000000 pyastgrep-1.0/src/pyastgrep/files.py
--rw-r--r--   0 luke      (1000) luke      (1000)     7904 2023-04-17 15:37:35.000000 pyastgrep-1.0/src/pyastgrep/ignores.py
--rw-r--r--   0 luke      (1000) luke      (1000)     4276 2023-04-17 14:55:13.000000 pyastgrep-1.0/src/pyastgrep/printer.py
--rw-r--r--   0 luke      (1000) luke      (1000)     4207 2023-04-17 14:55:57.000000 pyastgrep-1.0/src/pyastgrep/search.py
--rw-r--r--   0 luke      (1000) luke      (1000)      696 2022-11-14 14:54:35.000000 pyastgrep-1.0/src/pyastgrep/xml.py
--rw-r--r--   0 luke      (1000) luke      (1000)      366 2022-11-06 20:21:35.000000 pyastgrep-1.0/src/pyastgrep/xpath2.py
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-04-17 15:42:17.788971 pyastgrep-1.0/src/pyastgrep.egg-info/
--rw-r-----   0 luke      (1000) luke      (1000)    14968 2023-04-17 15:42:17.000000 pyastgrep-1.0/src/pyastgrep.egg-info/PKG-INFO
--rw-r-----   0 luke      (1000) luke      (1000)      698 2023-04-17 15:42:17.000000 pyastgrep-1.0/src/pyastgrep.egg-info/SOURCES.txt
--rw-r-----   0 luke      (1000) luke      (1000)        1 2023-04-17 15:42:17.000000 pyastgrep-1.0/src/pyastgrep.egg-info/dependency_links.txt
--rw-r-----   0 luke      (1000) luke      (1000)       81 2023-04-17 15:42:17.000000 pyastgrep-1.0/src/pyastgrep.egg-info/entry_points.txt
--rw-r-----   0 luke      (1000) luke      (1000)       58 2023-04-17 15:42:17.000000 pyastgrep-1.0/src/pyastgrep.egg-info/requires.txt
--rw-r-----   0 luke      (1000) luke      (1000)       10 2023-04-17 15:42:17.000000 pyastgrep-1.0/src/pyastgrep.egg-info/top_level.txt
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-04-17 15:42:17.788971 pyastgrep-1.0/tests/
--rw-r--r--   0 luke      (1000) luke      (1000)     6800 2022-11-25 07:33:14.000000 pyastgrep-1.0/tests/test_cli.py
--rw-r--r--   0 luke      (1000) luke      (1000)      733 2022-11-06 19:59:49.000000 pyastgrep-1.0/tests/test_encodings.py
--rw-r--r--   0 luke      (1000) luke      (1000)      648 2022-11-07 12:52:05.000000 pyastgrep-1.0/tests/test_errors.py
--rw-r--r--   0 luke      (1000) luke      (1000)     3591 2023-02-20 15:21:15.000000 pyastgrep-1.0/tests/test_ignores.py
--rw-r--r--   0 luke      (1000) luke      (1000)      449 2022-11-25 08:08:17.000000 pyastgrep-1.0/tests/test_parsing.py
--rw-r--r--   0 luke      (1000) luke      (1000)     2190 2022-11-07 12:01:43.000000 pyastgrep-1.0/tests/test_printing.py
--rw-r--r--   0 luke      (1000) luke      (1000)      410 2023-02-20 15:45:50.000000 pyastgrep-1.0/tests/test_symlinks.py
--rw-r--r--   0 luke      (1000) luke      (1000)     1682 2022-11-07 12:01:43.000000 pyastgrep-1.0/tests/test_xml.py
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-06-09 13:42:58.005910 pyastgrep-1.1/
+-rw-r--r--   0 luke      (1000) luke      (1000)      378 2022-10-17 13:09:58.000000 pyastgrep-1.1/.gitattributes
+-rw-r--r--   0 luke      (1000) luke      (1000)     1771 2022-11-07 12:01:43.000000 pyastgrep-1.1/.gitignore
+-rw-rw-rw-   0 luke      (1000) luke      (1000)    14968 2023-06-09 13:42:58.005910 pyastgrep-1.1/PKG-INFO
+-rw-r--r--   0 luke      (1000) luke      (1000)    14121 2023-02-20 15:44:13.000000 pyastgrep-1.1/README.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)      755 2023-04-17 15:02:16.000000 pyastgrep-1.1/pyproject.toml
+-rw-r--r--   0 luke      (1000) luke      (1000)     1135 2023-06-09 13:42:58.005910 pyastgrep-1.1/setup.cfg
+-rw-r--r--   0 luke      (1000) luke      (1000)       38 2022-10-21 16:01:47.000000 pyastgrep-1.1/setup.py
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-06-09 13:42:57.997910 pyastgrep-1.1/src/
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-06-09 13:42:58.001910 pyastgrep-1.1/src/pyastgrep/
+-rw-r--r--   0 luke      (1000) luke      (1000)       20 2023-06-09 13:42:38.000000 pyastgrep-1.1/src/pyastgrep/__init__.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     3158 2022-11-18 11:57:27.000000 pyastgrep-1.1/src/pyastgrep/asts.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     3930 2022-11-16 20:46:57.000000 pyastgrep-1.1/src/pyastgrep/cli.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      890 2022-11-25 07:36:32.000000 pyastgrep-1.1/src/pyastgrep/dump.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     3244 2023-02-20 15:43:43.000000 pyastgrep-1.1/src/pyastgrep/files.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     7934 2023-06-09 13:41:41.000000 pyastgrep-1.1/src/pyastgrep/ignores.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     4276 2023-04-17 14:55:13.000000 pyastgrep-1.1/src/pyastgrep/printer.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     4207 2023-04-17 14:55:57.000000 pyastgrep-1.1/src/pyastgrep/search.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      696 2022-11-14 14:54:35.000000 pyastgrep-1.1/src/pyastgrep/xml.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      366 2022-11-06 20:21:35.000000 pyastgrep-1.1/src/pyastgrep/xpath2.py
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-06-09 13:42:58.005910 pyastgrep-1.1/src/pyastgrep.egg-info/
+-rw-r-----   0 luke      (1000) luke      (1000)    14968 2023-06-09 13:42:57.000000 pyastgrep-1.1/src/pyastgrep.egg-info/PKG-INFO
+-rw-r-----   0 luke      (1000) luke      (1000)      698 2023-06-09 13:42:57.000000 pyastgrep-1.1/src/pyastgrep.egg-info/SOURCES.txt
+-rw-r-----   0 luke      (1000) luke      (1000)        1 2023-06-09 13:42:57.000000 pyastgrep-1.1/src/pyastgrep.egg-info/dependency_links.txt
+-rw-r-----   0 luke      (1000) luke      (1000)       81 2023-06-09 13:42:57.000000 pyastgrep-1.1/src/pyastgrep.egg-info/entry_points.txt
+-rw-r-----   0 luke      (1000) luke      (1000)       58 2023-06-09 13:42:57.000000 pyastgrep-1.1/src/pyastgrep.egg-info/requires.txt
+-rw-r-----   0 luke      (1000) luke      (1000)       10 2023-06-09 13:42:57.000000 pyastgrep-1.1/src/pyastgrep.egg-info/top_level.txt
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-06-09 13:42:58.005910 pyastgrep-1.1/tests/
+-rw-r--r--   0 luke      (1000) luke      (1000)     6800 2022-11-25 07:33:14.000000 pyastgrep-1.1/tests/test_cli.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      733 2022-11-06 19:59:49.000000 pyastgrep-1.1/tests/test_encodings.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      648 2022-11-07 12:52:05.000000 pyastgrep-1.1/tests/test_errors.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     4093 2023-06-09 13:41:41.000000 pyastgrep-1.1/tests/test_ignores.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      449 2022-11-25 08:08:17.000000 pyastgrep-1.1/tests/test_parsing.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     2190 2022-11-07 12:01:43.000000 pyastgrep-1.1/tests/test_printing.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      410 2023-02-20 15:45:50.000000 pyastgrep-1.1/tests/test_symlinks.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     1682 2022-11-07 12:01:43.000000 pyastgrep-1.1/tests/test_xml.py
```

### Comparing `pyastgrep-1.0/.gitignore` & `pyastgrep-1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pyastgrep-1.0/PKG-INFO` & `pyastgrep-1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyastgrep
-Version: 1.0
+Version: 1.1
 Summary: A query tool for Python abstract syntax trees
 Home-page: https://github.com/spookylukey/pyastgrep
 Author: Luke Plant
 License: MIT
 Keywords: xpath xml ast asts syntax query css grep
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
```

### Comparing `pyastgrep-1.0/README.rst` & `pyastgrep-1.1/README.rst`

 * *Files identical despite different names*

### Comparing `pyastgrep-1.0/pyproject.toml` & `pyastgrep-1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyastgrep-1.0/setup.cfg` & `pyastgrep-1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyastgrep-1.0/src/pyastgrep/asts.py` & `pyastgrep-1.1/src/pyastgrep/asts.py`

 * *Files identical despite different names*

### Comparing `pyastgrep-1.0/src/pyastgrep/cli.py` & `pyastgrep-1.1/src/pyastgrep/cli.py`

 * *Files identical despite different names*

### Comparing `pyastgrep-1.0/src/pyastgrep/dump.py` & `pyastgrep-1.1/src/pyastgrep/dump.py`

 * *Files identical despite different names*

### Comparing `pyastgrep-1.0/src/pyastgrep/files.py` & `pyastgrep-1.1/src/pyastgrep/files.py`

 * *Files identical despite different names*

### Comparing `pyastgrep-1.0/src/pyastgrep/ignores.py` & `pyastgrep-1.1/src/pyastgrep/ignores.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
     ):
         # DirWalker is immutable outside __init__
         self.glob: str = glob
         if pathspecs is None:
             pathspecs = []
         if init_global_pathspecs:
             global_gitignore = get_global_gitignore()
-            if global_gitignore:
+            if global_gitignore and global_gitignore.exists():
                 pathspecs.append(pathspec_for_gitignore(global_gitignore, is_global_gitignore=True))
             # POSIX hidden files:
             pathspecs.append(PathSpec([GitWildMatchPattern(".*")]))
         self.pathspecs: list[PathSpecLike] = pathspecs
         self.start_directory: Path | None = start_directory
         self.working_dir = working_dir
         self.absolute_base: bool = absolute_base
```

### Comparing `pyastgrep-1.0/src/pyastgrep/printer.py` & `pyastgrep-1.1/src/pyastgrep/printer.py`

 * *Files identical despite different names*

### Comparing `pyastgrep-1.0/src/pyastgrep/search.py` & `pyastgrep-1.1/src/pyastgrep/search.py`

 * *Files identical despite different names*

### Comparing `pyastgrep-1.0/src/pyastgrep/xml.py` & `pyastgrep-1.1/src/pyastgrep/xml.py`

 * *Files identical despite different names*

### Comparing `pyastgrep-1.0/src/pyastgrep.egg-info/PKG-INFO` & `pyastgrep-1.1/src/pyastgrep.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyastgrep
-Version: 1.0
+Version: 1.1
 Summary: A query tool for Python abstract syntax trees
 Home-page: https://github.com/spookylukey/pyastgrep
 Author: Luke Plant
 License: MIT
 Keywords: xpath xml ast asts syntax query css grep
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
```

### Comparing `pyastgrep-1.0/src/pyastgrep.egg-info/SOURCES.txt` & `pyastgrep-1.1/src/pyastgrep.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyastgrep-1.0/tests/test_cli.py` & `pyastgrep-1.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `pyastgrep-1.0/tests/test_encodings.py` & `pyastgrep-1.1/tests/test_encodings.py`

 * *Files identical despite different names*

### Comparing `pyastgrep-1.0/tests/test_errors.py` & `pyastgrep-1.1/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `pyastgrep-1.0/tests/test_ignores.py` & `pyastgrep-1.1/tests/test_ignores.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from pathlib import Path
+from unittest.mock import patch
 
 from pathspec.gitignore import GitIgnoreSpec
 
+import pyastgrep.ignores
 from pyastgrep.files import get_files_to_search
 from pyastgrep.ignores import DirectoryPathSpec, find_gitignore_files
-from tests.utils import chdir
+from tests.utils import chdir, run_print
 
 DIR = Path(__file__).resolve().parent / "examples" / "test_ignores"
 REPO_ROOT = Path(__file__).resolve().parent.parent
 DIR_FROM_ROOT = DIR.relative_to(REPO_ROOT)
 
 
 def test_find_gitignore_files():
@@ -102,7 +104,16 @@
     assert dps_root.match_file(Path("subdir/baz"))
 
     # But path in subdir should not match an absolute rule from parent dir.
     assert not dps_root.match_file(Path("subdir/bar"))
 
     # Path in subdir should match absolute rule from same dir
     assert dps_subdir.match_file(Path("subdir/bar"))
+
+
+def test_no_global_git_ignores():
+    # Check what happens if return of get_global_gitignore is a missing file
+    with patch("pyastgrep.ignores.get_global_gitignore", lambda: Path("/non/existent/.gitignore")):
+        assert pyastgrep.ignores.get_global_gitignore() == Path("/non/existent/.gitignore")
+        # We should not crash or print any output
+        result = run_print(Path("."), "Name")
+        assert not result.stderr
```

### Comparing `pyastgrep-1.0/tests/test_printing.py` & `pyastgrep-1.1/tests/test_printing.py`

 * *Files identical despite different names*

### Comparing `pyastgrep-1.0/tests/test_xml.py` & `pyastgrep-1.1/tests/test_xml.py`

 * *Files identical despite different names*

