# Comparing `tmp/crdb-0.8.0.tar.gz` & `tmp/crdb-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crdb-0.8.0.tar", last modified: Wed May 10 16:56:07 2023, max compression
+gzip compressed data, was "crdb-0.9.0.tar", last modified: Wed May 17 12:04:22 2023, max compression
```

## Comparing `crdb-0.8.0.tar` & `crdb-0.9.0.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:56:07.855631 crdb-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-10 16:55:55.000000 crdb-0.8.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:56:07.847631 crdb-0.8.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:56:07.851631 crdb-0.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-10 16:55:55.000000 crdb-0.8.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-10 16:55:55.000000 crdb-0.8.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-10 16:55:55.000000 crdb-0.8.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-10 16:55:55.000000 crdb-0.8.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-10 16:55:55.000000 crdb-0.8.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-10 16:55:55.000000 crdb-0.8.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-10 16:55:55.000000 crdb-0.8.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-10 16:55:55.000000 crdb-0.8.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-10 16:55:55.000000 crdb-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-10 16:55:55.000000 crdb-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-05-10 16:56:07.855631 crdb-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-05-10 16:55:55.000000 crdb-0.8.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:56:07.851631 crdb-0.8.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-10 16:55:55.000000 crdb-0.8.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-10 16:55:55.000000 crdb-0.8.0/docs/build.py
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-10 16:55:55.000000 crdb-0.8.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-05-10 16:55:55.000000 crdb-0.8.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-10 16:55:55.000000 crdb-0.8.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-10 16:55:55.000000 crdb-0.8.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-10 16:55:55.000000 crdb-0.8.0/docs/reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-10 16:55:55.000000 crdb-0.8.0/docs/spelling_wordlist.txt
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-10 16:55:55.000000 crdb-0.8.0/get_valid_names.py
--rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-05-10 16:55:55.000000 crdb-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-10 16:56:07.855631 crdb-0.8.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:56:07.847631 crdb-0.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:56:07.855631 crdb-0.8.0/src/crdb/
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-10 16:55:55.000000 crdb-0.8.0/src/crdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-10 16:55:55.000000 crdb-0.8.0/src/crdb/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-05-10 16:55:55.000000 crdb-0.8.0/src/crdb/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    22743 2023-05-10 16:55:55.000000 crdb-0.8.0/src/crdb/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    14332 2023-05-10 16:55:55.000000 crdb-0.8.0/src/crdb/crdb_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-05-10 16:55:55.000000 crdb-0.8.0/src/crdb/experimental.py
--rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-05-10 16:55:55.000000 crdb-0.8.0/src/crdb/mpl.py
--rw-r--r--   0 runner    (1001) docker     (123)     9328 2023-05-10 16:55:55.000000 crdb-0.8.0/src/crdb/solarsystem_abundances2003.dat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:56:07.855631 crdb-0.8.0/src/crdb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-05-10 16:56:07.000000 crdb-0.8.0/src/crdb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-10 16:56:07.000000 crdb-0.8.0/src/crdb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 16:56:07.000000 crdb-0.8.0/src/crdb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-10 16:56:07.000000 crdb-0.8.0/src/crdb.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-10 16:56:07.000000 crdb-0.8.0/src/crdb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-10 16:56:07.000000 crdb-0.8.0/src/crdb.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:56:07.855631 crdb-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-10 16:55:55.000000 crdb-0.8.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-10 16:55:55.000000 crdb-0.8.0/tests/test_experimental.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-05-10 16:55:55.000000 crdb-0.8.0/tests/test_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-10 16:55:55.000000 crdb-0.8.0/tests/test_mpl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:04:22.308790 crdb-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-17 12:04:12.000000 crdb-0.9.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:04:22.300790 crdb-0.9.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:04:22.304790 crdb-0.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-17 12:04:12.000000 crdb-0.9.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-17 12:04:12.000000 crdb-0.9.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-17 12:04:12.000000 crdb-0.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-17 12:04:12.000000 crdb-0.9.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-17 12:04:12.000000 crdb-0.9.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-17 12:04:12.000000 crdb-0.9.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-17 12:04:12.000000 crdb-0.9.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-17 12:04:12.000000 crdb-0.9.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-17 12:04:12.000000 crdb-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-17 12:04:12.000000 crdb-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-05-17 12:04:22.308790 crdb-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-05-17 12:04:12.000000 crdb-0.9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:04:22.304790 crdb-0.9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-17 12:04:12.000000 crdb-0.9.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-17 12:04:12.000000 crdb-0.9.0/docs/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-17 12:04:12.000000 crdb-0.9.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-05-17 12:04:12.000000 crdb-0.9.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-17 12:04:12.000000 crdb-0.9.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-17 12:04:12.000000 crdb-0.9.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-17 12:04:12.000000 crdb-0.9.0/docs/reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-17 12:04:12.000000 crdb-0.9.0/docs/spelling_wordlist.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-17 12:04:12.000000 crdb-0.9.0/get_valid_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-05-17 12:04:12.000000 crdb-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-17 12:04:22.308790 crdb-0.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:04:22.300790 crdb-0.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:04:22.304790 crdb-0.9.0/src/crdb/
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-17 12:04:12.000000 crdb-0.9.0/src/crdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-17 12:04:12.000000 crdb-0.9.0/src/crdb/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-05-17 12:04:12.000000 crdb-0.9.0/src/crdb/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22811 2023-05-17 12:04:12.000000 crdb-0.9.0/src/crdb/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14332 2023-05-17 12:04:12.000000 crdb-0.9.0/src/crdb/crdb_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-05-17 12:04:12.000000 crdb-0.9.0/src/crdb/experimental.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7266 2023-05-17 12:04:12.000000 crdb-0.9.0/src/crdb/mpl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9328 2023-05-17 12:04:12.000000 crdb-0.9.0/src/crdb/solarsystem_abundances2003.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-17 12:04:12.000000 crdb-0.9.0/src/crdb/units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:04:22.304790 crdb-0.9.0/src/crdb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-05-17 12:04:22.000000 crdb-0.9.0/src/crdb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-17 12:04:22.000000 crdb-0.9.0/src/crdb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 12:04:22.000000 crdb-0.9.0/src/crdb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-17 12:04:22.000000 crdb-0.9.0/src/crdb.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-17 12:04:22.000000 crdb-0.9.0/src/crdb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-17 12:04:22.000000 crdb-0.9.0/src/crdb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:04:22.308790 crdb-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-17 12:04:12.000000 crdb-0.9.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-05-17 12:04:12.000000 crdb-0.9.0/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-17 12:04:12.000000 crdb-0.9.0/tests/test_experimental.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-17 12:04:12.000000 crdb-0.9.0/tests/test_mpl.py
```

### Comparing `crdb-0.8.0/.github/workflows/publish.yml` & `crdb-0.9.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `crdb-0.8.0/.github/workflows/test.yml` & `crdb-0.9.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `crdb-0.8.0/.gitignore` & `crdb-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `crdb-0.8.0/.pre-commit-config.yaml` & `crdb-0.9.0/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -12,19 +12,19 @@
       - id: debug-statements
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
       - id: black
   # Ruff linter; replaces flake8, pydocstyle, isort
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: 'v0.0.265'
+    rev: 'v0.0.267'
     hooks:
       - id: ruff
         args: [--fix, --exit-non-zero-on-fix]
   # Python type checking
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: 'v1.2.0'
+    rev: 'v1.3.0'
     hooks:
     - id: mypy
       additional_dependencies: [numpy]
       args: [src]
       pass_filenames: false
```

### Comparing `crdb-0.8.0/CONTRIBUTING.rst` & `crdb-0.9.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `crdb-0.8.0/LICENSE` & `crdb-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `crdb-0.8.0/PKG-INFO` & `crdb-0.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crdb
-Version: 0.8.0
+Version: 0.9.0
 Summary: CRDB Python frontend
 Maintainer: Hans Dembinski
 Maintainer-email: hans.dembinski@gmail.com
 License: MIT
 Project-URL: repository, https://github.com/crdb-project/crdb
 Project-URL: documentation, https://lpsc.in2p3.fr/crdb
 Classifier: Development Status :: 4 - Beta
```

### Comparing `crdb-0.8.0/README.rst` & `crdb-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `crdb-0.8.0/docs/conf.py` & `crdb-0.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `crdb-0.8.0/pyproject.toml` & `crdb-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `crdb-0.8.0/src/crdb/__init__.py` & `crdb-0.9.0/src/crdb/__init__.py`

 * *Files identical despite different names*

### Comparing `crdb-0.8.0/src/crdb/cli.py` & `crdb-0.9.0/src/crdb/cli.py`

 * *Files identical despite different names*

### Comparing `crdb-0.8.0/src/crdb/core.py` & `crdb-0.9.0/src/crdb/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,14 +145,15 @@
     'Be',
     'Bi',
     'Bk',
     'Br',
     'C',
     'C-Fe-group',
     'C-bar',
+    'C-group',
     'Ca',
     'Cd',
     'Ce',
     'Cl',
     'Cm',
     'Co',
     'Cr',
@@ -169,14 +170,15 @@
     'Fr',
     'Ga',
     'Gd',
     'Ge',
     'H',
     'H-He-group',
     'He',
+    'He-C-group',
     'He-bar',
     'Hf',
     'Hg',
     'Ho',
     'Ir',
     'K',
     'Kr',
@@ -210,14 +212,16 @@
     'Re',
     'Rn',
     'Ru',
     'S',
     'Sc',
     'Se',
     'Si',
+    'Si-Fe-group',
+    'Si-group',
     'Sm',
     'Sn',
     'Sr',
     'SubFe',
     'Ta',
     'Tb',
     'Te',
```

### Comparing `crdb-0.8.0/src/crdb/crdb_logo.png` & `crdb-0.9.0/src/crdb/crdb_logo.png`

 * *Files identical despite different names*

### Comparing `crdb-0.8.0/src/crdb/experimental.py` & `crdb-0.9.0/src/crdb/experimental.py`

 * *Files identical despite different names*

### Comparing `crdb-0.8.0/src/crdb/solarsystem_abundances2003.dat` & `crdb-0.9.0/src/crdb/solarsystem_abundances2003.dat`

 * *Files identical despite different names*

### Comparing `crdb-0.8.0/src/crdb.egg-info/PKG-INFO` & `crdb-0.9.0/src/crdb.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crdb
-Version: 0.8.0
+Version: 0.9.0
 Summary: CRDB Python frontend
 Maintainer: Hans Dembinski
 Maintainer-email: hans.dembinski@gmail.com
 License: MIT
 Project-URL: repository, https://github.com/crdb-project/crdb
 Project-URL: documentation, https://lpsc.in2p3.fr/crdb
 Classifier: Development Status :: 4 - Beta
```

### Comparing `crdb-0.8.0/src/crdb.egg-info/SOURCES.txt` & `crdb-0.9.0/src/crdb.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -25,17 +25,18 @@
 src/crdb/__main__.py
 src/crdb/cli.py
 src/crdb/core.py
 src/crdb/crdb_logo.png
 src/crdb/experimental.py
 src/crdb/mpl.py
 src/crdb/solarsystem_abundances2003.dat
+src/crdb/units.py
 src/crdb.egg-info/PKG-INFO
 src/crdb.egg-info/SOURCES.txt
 src/crdb.egg-info/dependency_links.txt
 src/crdb.egg-info/entry_points.txt
 src/crdb.egg-info/requires.txt
 src/crdb.egg-info/top_level.txt
 tests/test_cli.py
+tests/test_core.py
 tests/test_experimental.py
-tests/test_lib.py
 tests/test_mpl.py
```

### Comparing `crdb-0.8.0/tests/test_experimental.py` & `crdb-0.9.0/tests/test_experimental.py`

 * *Files identical despite different names*

### Comparing `crdb-0.8.0/tests/test_lib.py` & `crdb-0.9.0/tests/test_core.py`

 * *Files identical despite different names*

