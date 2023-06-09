# Comparing `tmp/consoleprint-1.3.5.tar.gz` & `tmp/consoleprint-1.3.6.tar.gz`

## Comparing `consoleprint-1.3.5.tar` & `consoleprint-1.3.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 consoleprint-1.3.5/src/ConsolePrint/__init__.py
--rw-r--r--   0        0        0     9717 2020-02-02 00:00:00.000000 consoleprint-1.3.5/src/ConsolePrint/animate.py
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 consoleprint-1.3.5/src/ConsolePrint/console2file.py
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 consoleprint-1.3.5/src/ConsolePrint/loading.py
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 consoleprint-1.3.5/tests/tests.py
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 consoleprint-1.3.5/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 consoleprint-1.3.5/LICENSE
--rw-r--r--   0        0        0     3839 2020-02-02 00:00:00.000000 consoleprint-1.3.5/README.md
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 consoleprint-1.3.5/pyproject.toml
--rw-r--r--   0        0        0     4392 2020-02-02 00:00:00.000000 consoleprint-1.3.5/PKG-INFO
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 consoleprint-1.3.6/src/ConsolePrint/__init__.py
+-rw-r--r--   0        0        0     9717 2020-02-02 00:00:00.000000 consoleprint-1.3.6/src/ConsolePrint/animate.py
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 consoleprint-1.3.6/src/ConsolePrint/console2file.py
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 consoleprint-1.3.6/src/ConsolePrint/loading.py
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 consoleprint-1.3.6/tests/tests.py
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 consoleprint-1.3.6/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 consoleprint-1.3.6/LICENSE
+-rw-r--r--   0        0        0     3839 2020-02-02 00:00:00.000000 consoleprint-1.3.6/README.md
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 consoleprint-1.3.6/pyproject.toml
+-rw-r--r--   0        0        0     4392 2020-02-02 00:00:00.000000 consoleprint-1.3.6/PKG-INFO
```

### Comparing `consoleprint-1.3.5/src/ConsolePrint/animate.py` & `consoleprint-1.3.6/src/ConsolePrint/animate.py`

 * *Files identical despite different names*

### Comparing `consoleprint-1.3.5/src/ConsolePrint/console2file.py` & `consoleprint-1.3.6/src/ConsolePrint/console2file.py`

 * *Files identical despite different names*

### Comparing `consoleprint-1.3.5/src/ConsolePrint/loading.py` & `consoleprint-1.3.6/src/ConsolePrint/loading.py`

 * *Files identical despite different names*

### Comparing `consoleprint-1.3.5/tests/tests.py` & `consoleprint-1.3.6/tests/tests.py`

 * *Files identical despite different names*

### Comparing `consoleprint-1.3.5/LICENSE` & `consoleprint-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `consoleprint-1.3.5/README.md` & `consoleprint-1.3.6/README.md`

 * *Files identical despite different names*

### Comparing `consoleprint-1.3.5/pyproject.toml` & `consoleprint-1.3.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ConsolePrint"
-version = "1.3.5"
+version = "1.3.6"
 authors = [
   { name="Udemezue Iloabachie", email="udemezue@gmail.com" },
 ]
 description = "A package to animate and beautify print output to console"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `consoleprint-1.3.5/PKG-INFO` & `consoleprint-1.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ConsolePrint
-Version: 1.3.5
+Version: 1.3.6
 Summary: A package to animate and beautify print output to console
 Project-URL: Homepage, https://github.com/iloabachie/ConsolePrint
 Project-URL: Bug Tracker, https://github.com/iloabachie/ConsolePrint/issues
 Author-email: Udemezue Iloabachie <udemezue@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

