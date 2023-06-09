# Comparing `tmp/dead_code_finder-0.0.2.tar.gz` & `tmp/dead_code_finder-0.0.3.tar.gz`

## Comparing `dead_code_finder-0.0.2.tar` & `dead_code_finder-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 dead_code_finder-0.0.2/.flake8
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 dead_code_finder-0.0.2/Makefile
--rw-r--r--   0        0        0     3169 2020-02-02 00:00:00.000000 dead_code_finder-0.0.2/notes
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 dead_code_finder-0.0.2/requirements-dev.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dead_code_finder-0.0.2/requirements.txt
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 dead_code_finder-0.0.2/dead_code_finder/Makefile
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dead_code_finder-0.0.2/dead_code_finder/__init__.py
--rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 dead_code_finder-0.0.2/dead_code_finder/cli.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 dead_code_finder-0.0.2/dead_code_finder/tests/module_a.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 dead_code_finder-0.0.2/dead_code_finder/tests/module_b.py
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 dead_code_finder-0.0.2/dead_code_finder/tests/test_dead_code_finder.py
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 dead_code_finder-0.0.2/dead_code_finder/tests/test_case1/hello_world.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 dead_code_finder-0.0.2/dead_code_finder/tests/test_case1/subdir/one_more_file.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 dead_code_finder-0.0.2/dead_code_finder/tests/test_case1/subdir/another_subdir/__init__.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 dead_code_finder-0.0.2/.gitignore
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 dead_code_finder-0.0.2/README.md
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 dead_code_finder-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 dead_code_finder-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 dead_code_finder-0.0.3/.flake8
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 dead_code_finder-0.0.3/Makefile
+-rw-r--r--   0        0        0     3169 2020-02-02 00:00:00.000000 dead_code_finder-0.0.3/notes
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 dead_code_finder-0.0.3/requirements-dev.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dead_code_finder-0.0.3/requirements.txt
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 dead_code_finder-0.0.3/dead_code_finder/Makefile
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dead_code_finder-0.0.3/dead_code_finder/__init__.py
+-rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 dead_code_finder-0.0.3/dead_code_finder/cli.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 dead_code_finder-0.0.3/dead_code_finder/tests/module_a.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 dead_code_finder-0.0.3/dead_code_finder/tests/module_b.py
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 dead_code_finder-0.0.3/dead_code_finder/tests/test_dead_code_finder.py
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 dead_code_finder-0.0.3/dead_code_finder/tests/test_case1/hello_world.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 dead_code_finder-0.0.3/dead_code_finder/tests/test_case1/subdir/one_more_file.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 dead_code_finder-0.0.3/dead_code_finder/tests/test_case1/subdir/another_subdir/__init__.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 dead_code_finder-0.0.3/.gitignore
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 dead_code_finder-0.0.3/README.md
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 dead_code_finder-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 dead_code_finder-0.0.3/PKG-INFO
```

### Comparing `dead_code_finder-0.0.2/notes` & `dead_code_finder-0.0.3/notes`

 * *Files identical despite different names*

### Comparing `dead_code_finder-0.0.2/requirements-dev.txt` & `dead_code_finder-0.0.3/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `dead_code_finder-0.0.2/dead_code_finder/cli.py` & `dead_code_finder-0.0.3/dead_code_finder/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,16 +11,20 @@
 VariableName = str
 
 
 def find_python_filenames(paths: List[Pathname]):
     """Recursively searches for Python filenames in provided paths."""
     filenames = []
     for path in paths:
-        filenames += [os.path.join(dp, f) for dp, dn, filenames in os.walk(path)
-                  for f in filenames if os.path.splitext(f)[1] == '.py']
+        if os.path.isfile(path):
+            if os.path.splitext(path)[1] == ".py":
+                filenames.append(path)
+        else:
+            filenames += [os.path.join(dp, f) for dp, dn, filenames in os.walk(path)
+                          for f in filenames if os.path.splitext(f)[1] == ".py"]
     return filenames
 
 
 def read_files(filenames: List[Filename]) -> Dict[Filename, FileContent]:
     files = {}
     for filename in filenames:
         with open(filename, "r") as f:
```

### Comparing `dead_code_finder-0.0.2/dead_code_finder/tests/test_dead_code_finder.py` & `dead_code_finder-0.0.3/dead_code_finder/tests/test_dead_code_finder.py`

 * *Files identical despite different names*

### Comparing `dead_code_finder-0.0.2/.gitignore` & `dead_code_finder-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `dead_code_finder-0.0.2/pyproject.toml` & `dead_code_finder-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dead-code-finder"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
     {name = "Albertas Gimbutas", email = "albertasgim@gmail.com"},
 ]
 description = "Find and remove dead code."
 readme = "README.md"
 requires-python = ">= 3.8"
 classifiers = [
```

### Comparing `dead_code_finder-0.0.2/PKG-INFO` & `dead_code_finder-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dead-code-finder
-Version: 0.0.2
+Version: 0.0.3
 Summary: Find and remove dead code.
 Author-email: Albertas Gimbutas <albertasgim@gmail.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

