# Comparing `tmp/pytest-beeprint-0.1.0.tar.gz` & `tmp/pytest-beeprint-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-beeprint-0.1.0.tar", last modified: Fri Jun  9 00:38:42 2023, max compression
+gzip compressed data, was "pytest-beeprint-0.1.1.tar", last modified: Fri Jun  9 01:12:46 2023, max compression
```

## Comparing `pytest-beeprint-0.1.0.tar` & `pytest-beeprint-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 rodrigo    (501) wheel        (0)        0 2023-06-09 00:38:42.416570 pytest-beeprint-0.1.0/
--rw-r--r--   0 rodrigo    (501) wheel        (0)      155 2023-06-09 00:38:41.000000 pytest-beeprint-0.1.0/HISTORY.rst
--rw-r--r--   0 rodrigo    (501) wheel        (0)     1210 2023-06-09 00:38:41.000000 pytest-beeprint-0.1.0/LICENSE
--rw-r--r--   0 rodrigo    (501) wheel        (0)      117 2023-06-09 00:38:41.000000 pytest-beeprint-0.1.0/MANIFEST.in
--rw-r--r--   0 rodrigo    (501) wheel        (0)     2727 2023-06-09 00:38:42.416443 pytest-beeprint-0.1.0/PKG-INFO
--rw-r--r--   0 rodrigo    (501) wheel        (0)     1598 2023-06-09 00:38:41.000000 pytest-beeprint-0.1.0/README.rst
-drwxr-xr-x   0 rodrigo    (501) wheel        (0)        0 2023-06-09 00:38:42.416255 pytest-beeprint-0.1.0/pytest_beeprint.egg-info/
--rw-r--r--   0 rodrigo    (501) wheel        (0)     2727 2023-06-09 00:38:42.000000 pytest-beeprint-0.1.0/pytest_beeprint.egg-info/PKG-INFO
--rw-r--r--   0 rodrigo    (501) wheel        (0)      306 2023-06-09 00:38:42.000000 pytest-beeprint-0.1.0/pytest_beeprint.egg-info/SOURCES.txt
--rw-r--r--   0 rodrigo    (501) wheel        (0)        1 2023-06-09 00:38:42.000000 pytest-beeprint-0.1.0/pytest_beeprint.egg-info/dependency_links.txt
--rw-r--r--   0 rodrigo    (501) wheel        (0)       36 2023-06-09 00:38:42.000000 pytest-beeprint-0.1.0/pytest_beeprint.egg-info/entry_points.txt
--rw-r--r--   0 rodrigo    (501) wheel        (0)       23 2023-06-09 00:38:42.000000 pytest-beeprint-0.1.0/pytest_beeprint.egg-info/requires.txt
--rw-r--r--   0 rodrigo    (501) wheel        (0)       16 2023-06-09 00:38:42.000000 pytest-beeprint-0.1.0/pytest_beeprint.egg-info/top_level.txt
--rw-r--r--   0 rodrigo    (501) wheel        (0)     2212 2023-06-09 00:38:41.000000 pytest-beeprint-0.1.0/pytest_beeprint.py
--rw-r--r--   0 rodrigo    (501) wheel        (0)       38 2023-06-09 00:38:42.416607 pytest-beeprint-0.1.0/setup.cfg
--rw-r--r--   0 rodrigo    (501) wheel        (0)     1517 2023-06-09 00:38:41.000000 pytest-beeprint-0.1.0/setup.py
+drwxr-xr-x   0 rodrigo    (501) wheel        (0)        0 2023-06-09 01:12:46.180818 pytest-beeprint-0.1.1/
+-rw-r--r--   0 rodrigo    (501) wheel        (0)      209 2023-06-09 01:12:45.000000 pytest-beeprint-0.1.1/HISTORY.rst
+-rw-r--r--   0 rodrigo    (501) wheel        (0)     1210 2023-06-09 01:12:45.000000 pytest-beeprint-0.1.1/LICENSE
+-rw-r--r--   0 rodrigo    (501) wheel        (0)      117 2023-06-09 01:12:45.000000 pytest-beeprint-0.1.1/MANIFEST.in
+-rw-r--r--   0 rodrigo    (501) wheel        (0)     2490 2023-06-09 01:12:46.180664 pytest-beeprint-0.1.1/PKG-INFO
+-rw-r--r--   0 rodrigo    (501) wheel        (0)     1307 2023-06-09 01:12:45.000000 pytest-beeprint-0.1.1/README.rst
+drwxr-xr-x   0 rodrigo    (501) wheel        (0)        0 2023-06-09 01:12:46.180456 pytest-beeprint-0.1.1/pytest_beeprint.egg-info/
+-rw-r--r--   0 rodrigo    (501) wheel        (0)     2490 2023-06-09 01:12:46.000000 pytest-beeprint-0.1.1/pytest_beeprint.egg-info/PKG-INFO
+-rw-r--r--   0 rodrigo    (501) wheel        (0)      306 2023-06-09 01:12:46.000000 pytest-beeprint-0.1.1/pytest_beeprint.egg-info/SOURCES.txt
+-rw-r--r--   0 rodrigo    (501) wheel        (0)        1 2023-06-09 01:12:46.000000 pytest-beeprint-0.1.1/pytest_beeprint.egg-info/dependency_links.txt
+-rw-r--r--   0 rodrigo    (501) wheel        (0)       36 2023-06-09 01:12:46.000000 pytest-beeprint-0.1.1/pytest_beeprint.egg-info/entry_points.txt
+-rw-r--r--   0 rodrigo    (501) wheel        (0)       23 2023-06-09 01:12:46.000000 pytest-beeprint-0.1.1/pytest_beeprint.egg-info/requires.txt
+-rw-r--r--   0 rodrigo    (501) wheel        (0)       16 2023-06-09 01:12:46.000000 pytest-beeprint-0.1.1/pytest_beeprint.egg-info/top_level.txt
+-rw-r--r--   0 rodrigo    (501) wheel        (0)     2212 2023-06-09 01:12:45.000000 pytest-beeprint-0.1.1/pytest_beeprint.py
+-rw-r--r--   0 rodrigo    (501) wheel        (0)       38 2023-06-09 01:12:46.180876 pytest-beeprint-0.1.1/setup.cfg
+-rw-r--r--   0 rodrigo    (501) wheel        (0)     1517 2023-06-09 01:12:45.000000 pytest-beeprint-0.1.1/setup.py
```

### Comparing `pytest-beeprint-0.1.0/LICENSE` & `pytest-beeprint-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-beeprint-0.1.0/PKG-INFO` & `pytest-beeprint-0.1.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-beeprint
-Version: 0.1.0
+Version: 0.1.1
 Summary: use icdiff for better error messages in pytest assertions
 Home-page: https://github.com/hjwp/pytest-beeprint
 Author: Rodrigo Ferreira de Souza
 Author-email: rodfersou@gmail.com
 Maintainer: Rodrigo Ferreira de Souza
 Maintainer-email: rodfersou@gmail.com
 License: Unlicense
@@ -24,27 +24,19 @@
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ===============
 pytest-beeprint
 ===============
 
-.. image:: https://img.shields.io/pypi/v/pytest-beeprint.svg
-    :target: https://pypi.org/project/pytest-beeprint
-    :alt: PyPI version
-
-.. image:: https://img.shields.io/conda/vn/conda-forge/pytest-beeprint.svg
-    :target: https://anaconda.org/conda-forge/pytest-beeprint
-    :alt: conda-forge version
-
 .. image:: https://img.shields.io/pypi/pyversions/pytest-beeprint.svg
     :target: https://pypi.org/project/pytest-beeprint
     :alt: Python versions
 
-Better diffs in `pytest`_ assertion error messages using  `ICDiff`_.
+Better diffs in `pytest`_ assertion error messages using  `beeprint`_ and `ICDiff`_.
 
 Usage
 -----
 
     pip install pytest-beeprint
 
 Once you've installed it, ``pytest`` will produce nice colourised diffs for any ``assert ==`` :
@@ -72,13 +64,19 @@
 .. _`pytest-icdiff`: https://github.com/hjwp/pytest-icdiff
 .. _`icdiff`: https://www.jefftk.com/icdiff
 .. _`beeprint`: https://github.com/panyanyany/beeprint
 
 History
 -------
 
+0.1.1 (2023-06-08)
+~~~~~~~~~~~~~~~~~~
+
+- Fix README
+
+
 0.1.0 (2023-06-09)
 ~~~~~~~~~~~~~~~~~~
 
 * Forked from: https://github.com/hjwp/pytest-icdiff
 * Changed to use beeprint instead
 * Fix Tests
```

### Comparing `pytest-beeprint-0.1.0/README.rst` & `pytest-beeprint-0.1.1/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,16 @@
 ===============
 pytest-beeprint
 ===============
 
-.. image:: https://img.shields.io/pypi/v/pytest-beeprint.svg
-    :target: https://pypi.org/project/pytest-beeprint
-    :alt: PyPI version
-
-.. image:: https://img.shields.io/conda/vn/conda-forge/pytest-beeprint.svg
-    :target: https://anaconda.org/conda-forge/pytest-beeprint
-    :alt: conda-forge version
-
 .. image:: https://img.shields.io/pypi/pyversions/pytest-beeprint.svg
     :target: https://pypi.org/project/pytest-beeprint
     :alt: Python versions
 
-Better diffs in `pytest`_ assertion error messages using  `ICDiff`_.
+Better diffs in `pytest`_ assertion error messages using  `beeprint`_ and `ICDiff`_.
 
 Usage
 -----
 
     pip install pytest-beeprint
 
 Once you've installed it, ``pytest`` will produce nice colourised diffs for any ``assert ==`` :
```

### Comparing `pytest-beeprint-0.1.0/pytest_beeprint.egg-info/PKG-INFO` & `pytest-beeprint-0.1.1/pytest_beeprint.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-beeprint
-Version: 0.1.0
+Version: 0.1.1
 Summary: use icdiff for better error messages in pytest assertions
 Home-page: https://github.com/hjwp/pytest-beeprint
 Author: Rodrigo Ferreira de Souza
 Author-email: rodfersou@gmail.com
 Maintainer: Rodrigo Ferreira de Souza
 Maintainer-email: rodfersou@gmail.com
 License: Unlicense
@@ -24,27 +24,19 @@
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ===============
 pytest-beeprint
 ===============
 
-.. image:: https://img.shields.io/pypi/v/pytest-beeprint.svg
-    :target: https://pypi.org/project/pytest-beeprint
-    :alt: PyPI version
-
-.. image:: https://img.shields.io/conda/vn/conda-forge/pytest-beeprint.svg
-    :target: https://anaconda.org/conda-forge/pytest-beeprint
-    :alt: conda-forge version
-
 .. image:: https://img.shields.io/pypi/pyversions/pytest-beeprint.svg
     :target: https://pypi.org/project/pytest-beeprint
     :alt: Python versions
 
-Better diffs in `pytest`_ assertion error messages using  `ICDiff`_.
+Better diffs in `pytest`_ assertion error messages using  `beeprint`_ and `ICDiff`_.
 
 Usage
 -----
 
     pip install pytest-beeprint
 
 Once you've installed it, ``pytest`` will produce nice colourised diffs for any ``assert ==`` :
@@ -72,13 +64,19 @@
 .. _`pytest-icdiff`: https://github.com/hjwp/pytest-icdiff
 .. _`icdiff`: https://www.jefftk.com/icdiff
 .. _`beeprint`: https://github.com/panyanyany/beeprint
 
 History
 -------
 
+0.1.1 (2023-06-08)
+~~~~~~~~~~~~~~~~~~
+
+- Fix README
+
+
 0.1.0 (2023-06-09)
 ~~~~~~~~~~~~~~~~~~
 
 * Forked from: https://github.com/hjwp/pytest-icdiff
 * Changed to use beeprint instead
 * Fix Tests
```

### Comparing `pytest-beeprint-0.1.0/pytest_beeprint.py` & `pytest-beeprint-0.1.1/pytest_beeprint.py`

 * *Files identical despite different names*

### Comparing `pytest-beeprint-0.1.0/setup.py` & `pytest-beeprint-0.1.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 def read(fname):
     file_path = os.path.join(os.path.dirname(__file__), fname)
     return codecs.open(file_path, encoding="utf-8").read()
 
 
 setup(
     name="pytest-beeprint",
-    version="0.1.0",
+    version="0.1.1",
     author="Rodrigo Ferreira de Souza",
     author_email="rodfersou@gmail.com",
     maintainer="Rodrigo Ferreira de Souza",
     maintainer_email="rodfersou@gmail.com",
     license="Unlicense",
     url="https://github.com/hjwp/pytest-beeprint",
     description="use icdiff for better error messages in pytest assertions",
```

