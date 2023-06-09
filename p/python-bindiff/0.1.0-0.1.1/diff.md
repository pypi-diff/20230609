# Comparing `tmp/python-bindiff-0.1.0.tar.gz` & `tmp/python-bindiff-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-bindiff-0.1.0.tar", last modified: Sun Apr 16 22:57:08 2023, max compression
+gzip compressed data, was "python-bindiff-0.1.1.tar", last modified: Fri Jun  9 15:54:41 2023, max compression
```

## Comparing `python-bindiff-0.1.0.tar` & `python-bindiff-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:57:08.019195 python-bindiff-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-16 22:57:07.000000 python-bindiff-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-04-16 22:57:08.019195 python-bindiff-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-04-16 22:57:07.000000 python-bindiff-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:57:08.019195 python-bindiff-0.1.0/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3741 2023-04-16 22:57:07.000000 python-bindiff-0.1.0/bin/bindiffer
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:57:08.019195 python-bindiff-0.1.0/bindiff/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-16 22:57:07.000000 python-bindiff-0.1.0/bindiff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10414 2023-04-16 22:57:07.000000 python-bindiff-0.1.0/bindiff/bindiff.py
--rw-r--r--   0 runner    (1001) docker     (123)     7407 2023-04-16 22:57:07.000000 python-bindiff-0.1.0/bindiff/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-04-16 22:57:07.000000 python-bindiff-0.1.0/bindiff/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:57:08.019195 python-bindiff-0.1.0/python_bindiff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-04-16 22:57:07.000000 python-bindiff-0.1.0/python_bindiff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-16 22:57:08.000000 python-bindiff-0.1.0/python_bindiff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 22:57:07.000000 python-bindiff-0.1.0/python_bindiff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-16 22:57:07.000000 python-bindiff-0.1.0/python_bindiff.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-16 22:57:07.000000 python-bindiff-0.1.0/python_bindiff.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 22:57:08.019195 python-bindiff-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-04-16 22:57:07.000000 python-bindiff-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:54:41.793646 python-bindiff-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-09 15:54:35.000000 python-bindiff-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-06-09 15:54:41.793646 python-bindiff-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-06-09 15:54:35.000000 python-bindiff-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:54:41.793646 python-bindiff-0.1.1/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3741 2023-06-09 15:54:35.000000 python-bindiff-0.1.1/bin/bindiffer
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:54:41.793646 python-bindiff-0.1.1/bindiff/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-09 15:54:35.000000 python-bindiff-0.1.1/bindiff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10468 2023-06-09 15:54:35.000000 python-bindiff-0.1.1/bindiff/bindiff.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17780 2023-06-09 15:54:35.000000 python-bindiff-0.1.1/bindiff/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-06-09 15:54:35.000000 python-bindiff-0.1.1/bindiff/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:54:41.793646 python-bindiff-0.1.1/python_bindiff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-06-09 15:54:41.000000 python-bindiff-0.1.1/python_bindiff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-09 15:54:41.000000 python-bindiff-0.1.1/python_bindiff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 15:54:41.000000 python-bindiff-0.1.1/python_bindiff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-09 15:54:41.000000 python-bindiff-0.1.1/python_bindiff.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-09 15:54:41.000000 python-bindiff-0.1.1/python_bindiff.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 15:54:41.793646 python-bindiff-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-06-09 15:54:35.000000 python-bindiff-0.1.1/setup.py
```

### Comparing `python-bindiff-0.1.0/LICENSE` & `python-bindiff-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-bindiff-0.1.0/PKG-INFO` & `python-bindiff-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: python-bindiff
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python wrapper to manipulate bindiff files
 Home-page: https://github.com/quarkslab/python-bindiff
 Author: Robin David
 Author-email: rdavid@quarkslab.com
 License: AGPL-3.0
 Project-URL: Documentation, https://quarkslab.github.io/diffing-portal/differs/bindiff.html#python-bindiff
 Project-URL: Bug Tracker, https://github.com/quarkslab/python-bindiff/issues
 Project-URL: Source, https://github.com/quarkslab/python-bindiff
 Classifier: Topic :: Security
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Python Bindiff
 
 ``python-bindiff`` is a python module aiming to give a friendly interface to launch
 and manipulate bindiff between two binary iles.
@@ -24,22 +25,19 @@
 --------------
 
 The module relies on [python-binexport](https://github.com/quarkslab/python-binexport)
 to extract programs .BinExport and then directly interact with the binary ``differ``
 (of zynamics) to perform the diff. The generated diff file is then correlated
 with the two binaries to be able to navigate the changes.
 
-Dependencies
+Installation
 ------------
 
-Python bindiff relies on:
+    pip install python-bindiff
 
-* [python-binexport](https://github.com/quarkslab/python-binexport)
-* click *(for ``bindiffer``)*
-* python-magic *(for ``bindiffer``)*
 
 Usage as a python module
 ------------------------
 
 The simplest way to get the programs diffed is:
 
 ```python
```

### Comparing `python-bindiff-0.1.0/README.md` & `python-bindiff-0.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -7,22 +7,19 @@
 --------------
 
 The module relies on [python-binexport](https://github.com/quarkslab/python-binexport)
 to extract programs .BinExport and then directly interact with the binary ``differ``
 (of zynamics) to perform the diff. The generated diff file is then correlated
 with the two binaries to be able to navigate the changes.
 
-Dependencies
+Installation
 ------------
 
-Python bindiff relies on:
+    pip install python-bindiff
 
-* [python-binexport](https://github.com/quarkslab/python-binexport)
-* click *(for ``bindiffer``)*
-* python-magic *(for ``bindiffer``)*
 
 Usage as a python module
 ------------------------
 
 The simplest way to get the programs diffed is:
 
 ```python
```

### Comparing `python-bindiff-0.1.0/bin/bindiffer` & `python-bindiff-0.1.1/bin/bindiffer`

 * *Files identical despite different names*

### Comparing `python-bindiff-0.1.0/bindiff/bindiff.py` & `python-bindiff-0.1.1/bindiff/bindiff.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,14 +70,16 @@
 class BinDiff(BindiffFile):
     """
     BinDiff class. Parse the diffing result of Bindiff and apply it to the two
     ProgramBinExport given. All the diff result is embedded in the two programs
     object so after loading the class can be dropped if needed.
 
     .. warning:: the two programs given are mutated into :py:class:`ProgramBinDiff` object
+                 which inherit :py:class:`SimilarityMixin` and :py:class:`DictMatchMixin` which provides
+                 additional attributes and method to the class.
     """
 
     def __init__(self, primary: Union[ProgramBinExport, str], secondary: Union[ProgramBinExport, str], diff_file: str):
         """
         :param primary: first program diffed
         :param secondary: second program diffed
         :param diff_file: diffing file as generated by bindiff (differ more specifically)
@@ -95,31 +97,27 @@
 
     @staticmethod
     def _convert_program_classes(p: ProgramBinExport) -> None:
         """
         Internal method to mutate a ProgramBinExport into ProgramBinDiff.
 
         :param p: program to mutate
-        :return: None (perform all the side effect on the program)
         """
         p.__class__ = ProgramBinDiff
         for f in p.values():
             f.__class__ = FunctionBinDiff
             for bb in f.values():
                 bb.__class__ = BasicBlockBinDiff
                 for i in bb.values():
                     i.__class__ = InstructionBinDiff
 
     def _map_diff_on_programs(self) -> None:
         """
         From a diffing result, maps functions, basic blocks and instructions of primary and secondary
-
-        :return: None
         """
-
         # Map similarity and confidence on both programs
         self.primary.similarity, self.secondary.similarity = self.similarity, self.similarity
         self.primary.confidence, self.secondary.confidence = self.confidence, self.confidence
 
         for match in self.function_matches:
             f1 = self.primary[match.address1]
             f2 = self.secondary[match.address2]
@@ -161,15 +159,15 @@
         """
         Static method to diff two binexport files against each other and storing
         the diffing result in the given file
 
         :param p1_path: primary file path
         :param p2_path: secondary file path
         :param out_diff: diffing output file
-        :return: int (0 if successfull, -x otherwise)
+        :return: True if successful, False otherwise
         """
 
         # Make sure the bindiff binary is okay before doing any diffing
         BinDiff.assert_installation_ok()
 
         tmp_dir = Path(tempfile.mkdtemp())
         f1 = Path(p1_path)
@@ -244,16 +242,14 @@
         retcode = BinDiff.raw_diffing(p1_binexport, p2_binexport, diff_out)
         return BinDiff(p1_binexport, p2_binexport, diff_out) if retcode else None
 
     @staticmethod
     def _configure_bindiff_path() -> None:
         """
         Check BinDiff access paths
-
-        :return: None
         """
         if not _check_environ():
             if not _check_default_path():
                 if not _check_path():
                     logging.warning(f"Can't find a valid bindiff executable. (should be available in PATH or"
                                     f"as ${BINDIFF_PATH_ENV} env variable")
```

### Comparing `python-bindiff-0.1.0/bindiff/types.py` & `python-bindiff-0.1.1/bindiff/types.py`

 * *Files identical despite different names*

### Comparing `python-bindiff-0.1.0/python_bindiff.egg-info/PKG-INFO` & `python-bindiff-0.1.1/python_bindiff.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: python-bindiff
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python wrapper to manipulate bindiff files
 Home-page: https://github.com/quarkslab/python-bindiff
 Author: Robin David
 Author-email: rdavid@quarkslab.com
 License: AGPL-3.0
 Project-URL: Documentation, https://quarkslab.github.io/diffing-portal/differs/bindiff.html#python-bindiff
 Project-URL: Bug Tracker, https://github.com/quarkslab/python-bindiff/issues
 Project-URL: Source, https://github.com/quarkslab/python-bindiff
 Classifier: Topic :: Security
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Python Bindiff
 
 ``python-bindiff`` is a python module aiming to give a friendly interface to launch
 and manipulate bindiff between two binary iles.
@@ -24,22 +25,19 @@
 --------------
 
 The module relies on [python-binexport](https://github.com/quarkslab/python-binexport)
 to extract programs .BinExport and then directly interact with the binary ``differ``
 (of zynamics) to perform the diff. The generated diff file is then correlated
 with the two binaries to be able to navigate the changes.
 
-Dependencies
+Installation
 ------------
 
-Python bindiff relies on:
+    pip install python-bindiff
 
-* [python-binexport](https://github.com/quarkslab/python-binexport)
-* click *(for ``bindiffer``)*
-* python-magic *(for ``bindiffer``)*
 
 Usage as a python module
 ------------------------
 
 The simplest way to get the programs diffed is:
 
 ```python
```

### Comparing `python-bindiff-0.1.0/setup.py` & `python-bindiff-0.1.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,27 +2,28 @@
 from setuptools import setup
 
 with open("README.md") as f:
     README = f.read()
 
 setup(
     name='python-bindiff',
-    version='0.1.0',
+    version='0.1.1',
     description='Python wrapper to manipulate bindiff files',
     author='Robin David',
     author_email='rdavid@quarkslab.com',
     url='https://github.com/quarkslab/python-bindiff',
     long_description_content_type='text/markdown',
     long_description=README,
     packages=['bindiff'],
     project_urls={
         "Documentation": "https://quarkslab.github.io/diffing-portal/differs/bindiff.html#python-bindiff",
         "Bug Tracker": "https://github.com/quarkslab/python-bindiff/issues",
         "Source": "https://github.com/quarkslab/python-bindiff"
     },
+    python_requires='>=3.9',
     install_requires=[
         'python-magic',
         'click',
         'python-binexport'
     ],
     license="AGPL-3.0",
     classifiers=[
```

