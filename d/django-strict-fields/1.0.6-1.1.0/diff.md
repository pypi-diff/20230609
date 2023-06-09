# Comparing `tmp/django-strict-fields-1.0.6.tar.gz` & `tmp/django_strict_fields-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-strict-fields-1.0.6.tar", max compression
+gzip compressed data, was "django_strict_fields-1.1.0.tar", max compression
```

## Comparing `django-strict-fields-1.0.6.tar` & `django_strict_fields-1.1.0.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0     1456 2022-08-26 15:31:06.021270 django-strict-fields-1.0.6/LICENSE
--rw-r--r--   0        0        0      864 2022-08-26 15:31:06.025270 django-strict-fields-1.0.6/README.rst
--rw-r--r--   0        0        0     2324 2022-08-26 15:31:34.993293 django-strict-fields-1.0.6/pyproject.toml
--rw-r--r--   0        0        0      486 2022-08-26 15:31:06.025270 django-strict-fields-1.0.6/strict_fields/__init__.py
--rw-r--r--   0        0        0     3033 2022-08-26 15:31:06.025270 django-strict-fields-1.0.6/strict_fields/apps.py
--rw-r--r--   0        0        0     2900 2022-08-26 15:31:06.025270 django-strict-fields-1.0.6/strict_fields/fields.py
--rw-r--r--   0        0        0      990 2022-08-26 15:31:06.025270 django-strict-fields-1.0.6/strict_fields/helpers.py
--rw-r--r--   0        0        0      158 2022-08-26 15:31:06.025270 django-strict-fields-1.0.6/strict_fields/version.py
--rw-r--r--   0        0        0     1735 2022-08-26 15:31:39.900989 django-strict-fields-1.0.6/setup.py
--rw-r--r--   0        0        0     2130 2022-08-26 15:31:39.901240 django-strict-fields-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1456 2023-06-09 01:14:30.542614 django_strict_fields-1.1.0/LICENSE
+-rw-r--r--   0        0        0      978 2023-06-09 01:14:30.542614 django_strict_fields-1.1.0/README.rst
+-rw-r--r--   0        0        0     2390 2023-06-09 01:15:03.442581 django_strict_fields-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      506 2023-06-09 01:14:30.542614 django_strict_fields-1.1.0/strict_fields/__init__.py
+-rw-r--r--   0        0        0     3033 2023-06-09 01:14:30.542614 django_strict_fields-1.1.0/strict_fields/apps.py
+-rw-r--r--   0        0        0     2900 2023-06-09 01:14:30.542614 django_strict_fields-1.1.0/strict_fields/fields.py
+-rw-r--r--   0        0        0      990 2023-06-09 01:14:30.542614 django_strict_fields-1.1.0/strict_fields/helpers.py
+-rw-r--r--   0        0        0      158 2023-06-09 01:14:30.542614 django_strict_fields-1.1.0/strict_fields/version.py
+-rw-r--r--   0        0        0     2296 1970-01-01 00:00:00.000000 django_strict_fields-1.1.0/PKG-INFO
```

### Comparing `django-strict-fields-1.0.6/LICENSE` & `django_strict_fields-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-strict-fields-1.0.6/README.rst` & `django_strict_fields-1.1.0/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 django-strict-fields
 ########################################################################
 
 This library is meant to help enforce stricter rules around using some of the basic model fields that Django provides.
 View the docs `here <https://django-strict-fields.readthedocs.io/>`_ to get started.
 
+Compatibility
+=============
+
+``django-strict-fields`` is compatible with Python 3.7 - 3.11 and Django 3.2 - 4.2.
+
 Documentation
 =============
 
 `View the django-strict-fields docs here
 <https://django-strict-fields.readthedocs.io/>`_.
 
 Installation
```

### Comparing `django-strict-fields-1.0.6/pyproject.toml` & `django_strict_fields-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -25,30 +25,31 @@
 name = "django-strict-fields"
 packages = [
   { include = "strict_fields" }
 ]
 exclude = [
   "*/tests/"
 ]
-version = "1.0.6"
+version = "1.1.0"
 description = "A collection of fields and utilities to help make model fields more strict."
 authors = ["Tomas Arni Jonasson"]
 classifiers = [
   "Framework :: Django",
-  "Framework :: Django :: 2.2",
   "Framework :: Django :: 3.2",
   "Framework :: Django :: 4.0",
   "Framework :: Django :: 4.1",
+  "Framework :: Django :: 4.2",
   "Intended Audience :: Developers",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3 :: Only",
   "Framework :: Django",
 ]
 license = "BSD-3-Clause"
 readme = "README.rst"
 homepage = "https://github.com/Opus10/django-strict-fields"
 repository = "https://github.com/Opus10/django-strict-fields"
@@ -64,20 +65,21 @@
 dj-database-url = "0.5.0"
 flake8 = "3.9.2"
 flake8-bugbear = "22.1.11"
 flake8-comprehensions = "3.8.0"
 flake8-import-order = "0.18.1"
 flake8-logging-format = "0.6.0"
 flake8-mutable = "1.2.0"
-git-tidy = "1.1.2"
+git-tidy = "1.2.0"
 myst-parser = "0.18.0"
 packaging = ">=19.2"
 pip = "*"
+poetry-core = "1.3.2"
 pre-commit = "2.13.0"
-psycopg2-binary = "2.9.3"
+psycopg2-binary = "2.9.6"
 pytest = "7.0.0"
 pytest-cov = "3.0.0"
 pytest-django = "4.5.2"
 pytest-dotenv = "0.5.2"
 python-magic = "=0.4.15"
 pytest-mock = "3.1.0"
 requests = "2.25.1"
```

### Comparing `django-strict-fields-1.0.6/strict_fields/apps.py` & `django_strict_fields-1.1.0/strict_fields/apps.py`

 * *Files identical despite different names*

### Comparing `django-strict-fields-1.0.6/strict_fields/fields.py` & `django_strict_fields-1.1.0/strict_fields/fields.py`

 * *Files identical despite different names*

### Comparing `django-strict-fields-1.0.6/strict_fields/helpers.py` & `django_strict_fields-1.1.0/strict_fields/helpers.py`

 * *Files identical despite different names*

### Comparing `django-strict-fields-1.0.6/PKG-INFO` & `django_strict_fields-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,48 @@
 Metadata-Version: 2.1
 Name: django-strict-fields
-Version: 1.0.6
+Version: 1.1.0
 Summary: A collection of fields and utilities to help make model fields more strict.
 Home-page: https://github.com/Opus10/django-strict-fields
 License: BSD-3-Clause
 Author: Tomas Arni Jonasson
 Requires-Python: >=3.7.0,<4
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Dist: django (>=2)
-Requires-Dist: importlib_metadata (>=4); python_version >= "3.7" and python_version < "3.8"
+Requires-Dist: importlib_metadata (>=4) ; python_version >= "3.7" and python_version < "3.8"
 Project-URL: Documentation, https://django-strict-fields.readthedocs.io
 Project-URL: Repository, https://github.com/Opus10/django-strict-fields
 Description-Content-Type: text/x-rst
 
 django-strict-fields
 ########################################################################
 
 This library is meant to help enforce stricter rules around using some of the basic model fields that Django provides.
 View the docs `here <https://django-strict-fields.readthedocs.io/>`_ to get started.
 
+Compatibility
+=============
+
+``django-strict-fields`` is compatible with Python 3.7 - 3.11 and Django 3.2 - 4.2.
+
 Documentation
 =============
 
 `View the django-strict-fields docs here
 <https://django-strict-fields.readthedocs.io/>`_.
 
 Installation
```

