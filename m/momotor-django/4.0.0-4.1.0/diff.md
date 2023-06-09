# Comparing `tmp/momotor-django-4.0.0.tar.gz` & `tmp/momotor-django-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "momotor-django-4.0.0.tar", last modified: Fri Dec  9 07:54:00 2022, max compression
+gzip compressed data, was "momotor-django-4.1.0.tar", last modified: Fri Jun  9 07:45:20 2023, max compression
```

## Comparing `momotor-django-4.0.0.tar` & `momotor-django-4.1.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-09 07:54:00.000000 momotor-django-4.0.0/
--rw-r--r--   0 root         (0) root         (0)     1801 2022-12-09 07:54:00.000000 momotor-django-4.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      657 2022-12-09 07:26:37.000000 momotor-django-4.0.0/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2022-12-09 07:54:00.000000 momotor-django-4.0.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2224 2022-12-09 07:26:37.000000 momotor-django-4.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-09 07:54:00.000000 momotor-django-4.0.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-09 07:54:00.000000 momotor-django-4.0.0/src/momotor/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-09 07:54:00.000000 momotor-django-4.0.0/src/momotor/django/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-09 07:53:21.000000 momotor-django-4.0.0/src/momotor/django/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      860 2022-12-09 07:26:37.000000 momotor-django-4.0.0/src/momotor/django/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      178 2022-12-09 07:26:37.000000 momotor-django-4.0.0/src/momotor/django/apps.py
--rw-rw-rw-   0 root         (0) root         (0)    18614 2022-12-09 07:26:37.000000 momotor-django-4.0.0/src/momotor/django/connection.py
--rw-rw-rw-   0 root         (0) root         (0)      509 2022-12-09 07:26:37.000000 momotor-django-4.0.0/src/momotor/django/defaults.py
--rw-rw-rw-   0 root         (0) root         (0)     1163 2022-12-09 07:53:21.000000 momotor-django-4.0.0/src/momotor/django/fields.py
--rw-rw-rw-   0 root         (0) root         (0)      621 2022-12-09 07:53:21.000000 momotor-django-4.0.0/src/momotor/django/forms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-09 07:54:00.000000 momotor-django-4.0.0/src/momotor/django/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      546 2022-12-09 07:26:37.000000 momotor-django-4.0.0/src/momotor/django/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-09 07:53:21.000000 momotor-django-4.0.0/src/momotor/django/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      229 2022-12-09 07:26:37.000000 momotor-django-4.0.0/src/momotor/django/models.py
--rw-rw-rw-   0 root         (0) root         (0)       60 2022-12-09 07:26:37.000000 momotor-django-4.0.0/src/momotor/django/tests.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-09 07:54:00.000000 momotor-django-4.0.0/src/momotor/django/token_store/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-09 07:53:21.000000 momotor-django-4.0.0/src/momotor/django/token_store/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2562 2022-12-09 07:53:21.000000 momotor-django-4.0.0/src/momotor/django/token_store/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1349 2022-12-09 07:26:37.000000 momotor-django-4.0.0/src/momotor/django/token_store/cache.py
--rw-rw-rw-   0 root         (0) root         (0)      338 2022-12-09 07:26:37.000000 momotor-django-4.0.0/src/momotor/django/token_store/dummy.py
--rw-rw-rw-   0 root         (0) root         (0)      532 2022-12-09 07:26:37.000000 momotor-django-4.0.0/src/momotor/django/token_store/memory.py
--rw-rw-rw-   0 root         (0) root         (0)     1738 2022-12-09 07:26:37.000000 momotor-django-4.0.0/src/momotor/django/token_store/model.py
--rw-rw-rw-   0 root         (0) root         (0)       22 2022-12-09 07:52:27.000000 momotor-django-4.0.0/src/momotor/django/version.py
--rw-rw-rw-   0 root         (0) root         (0)       63 2022-12-09 07:26:37.000000 momotor-django-4.0.0/src/momotor/django/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-09 07:54:00.000000 momotor-django-4.0.0/src/momotor_django.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1801 2022-12-09 07:53:59.000000 momotor-django-4.0.0/src/momotor_django.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      921 2022-12-09 07:54:00.000000 momotor-django-4.0.0/src/momotor_django.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-09 07:53:59.000000 momotor-django-4.0.0/src/momotor_django.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-09 07:53:59.000000 momotor-django-4.0.0/src/momotor_django.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      139 2022-12-09 07:53:59.000000 momotor-django-4.0.0/src/momotor_django.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2022-12-09 07:53:59.000000 momotor-django-4.0.0/src/momotor_django.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:45:20.000000 momotor-django-4.1.0/
+-rw-r--r--   0 root         (0) root         (0)     1840 2023-06-09 07:45:20.000000 momotor-django-4.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      657 2022-08-22 08:11:03.000000 momotor-django-4.1.0/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-09 07:45:20.000000 momotor-django-4.1.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2258 2023-06-09 07:44:52.000000 momotor-django-4.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:45:20.000000 momotor-django-4.1.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:45:20.000000 momotor-django-4.1.0/src/momotor/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:45:20.000000 momotor-django-4.1.0/src/momotor/django/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-09 07:44:52.000000 momotor-django-4.1.0/src/momotor/django/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      860 2022-08-22 08:11:03.000000 momotor-django-4.1.0/src/momotor/django/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      178 2022-08-22 08:11:03.000000 momotor-django-4.1.0/src/momotor/django/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)    18614 2023-06-09 07:44:52.000000 momotor-django-4.1.0/src/momotor/django/connection.py
+-rw-rw-rw-   0 root         (0) root         (0)      509 2022-08-22 08:11:03.000000 momotor-django-4.1.0/src/momotor/django/defaults.py
+-rw-rw-rw-   0 root         (0) root         (0)     1163 2023-06-09 07:44:52.000000 momotor-django-4.1.0/src/momotor/django/fields.py
+-rw-rw-rw-   0 root         (0) root         (0)      621 2023-06-09 07:44:52.000000 momotor-django-4.1.0/src/momotor/django/forms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:45:20.000000 momotor-django-4.1.0/src/momotor/django/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)      546 2022-08-22 08:11:03.000000 momotor-django-4.1.0/src/momotor/django/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-09 07:44:52.000000 momotor-django-4.1.0/src/momotor/django/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      229 2022-08-22 08:11:03.000000 momotor-django-4.1.0/src/momotor/django/models.py
+-rw-rw-rw-   0 root         (0) root         (0)       60 2022-08-22 08:11:03.000000 momotor-django-4.1.0/src/momotor/django/tests.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:45:20.000000 momotor-django-4.1.0/src/momotor/django/token_store/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-09 07:44:52.000000 momotor-django-4.1.0/src/momotor/django/token_store/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2562 2023-06-09 07:44:52.000000 momotor-django-4.1.0/src/momotor/django/token_store/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1349 2022-08-22 08:11:03.000000 momotor-django-4.1.0/src/momotor/django/token_store/cache.py
+-rw-rw-rw-   0 root         (0) root         (0)      338 2022-08-22 08:11:03.000000 momotor-django-4.1.0/src/momotor/django/token_store/dummy.py
+-rw-rw-rw-   0 root         (0) root         (0)      532 2022-08-22 08:11:03.000000 momotor-django-4.1.0/src/momotor/django/token_store/memory.py
+-rw-rw-rw-   0 root         (0) root         (0)     1738 2022-08-22 08:11:03.000000 momotor-django-4.1.0/src/momotor/django/token_store/model.py
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-06-09 07:44:31.000000 momotor-django-4.1.0/src/momotor/django/version.py
+-rw-rw-rw-   0 root         (0) root         (0)       63 2022-08-22 08:11:03.000000 momotor-django-4.1.0/src/momotor/django/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:45:20.000000 momotor-django-4.1.0/src/momotor_django.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1840 2023-06-09 07:45:19.000000 momotor-django-4.1.0/src/momotor_django.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      921 2023-06-09 07:45:19.000000 momotor-django-4.1.0/src/momotor_django.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 07:45:19.000000 momotor-django-4.1.0/src/momotor_django.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 07:45:19.000000 momotor-django-4.1.0/src/momotor_django.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      135 2023-06-09 07:45:19.000000 momotor-django-4.1.0/src/momotor_django.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-09 07:45:19.000000 momotor-django-4.1.0/src/momotor_django.egg-info/top_level.txt
```

### Comparing `momotor-django-4.0.0/PKG-INFO` & `momotor-django-4.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: momotor-django
-Version: 4.0.0
+Version: 4.1.0
 Summary: Momotor bindings for the Django project
 Home-page: https://momotor.org/
 Author: Erik Scheffers
 Author-email: e.t.j.scheffers@tue.nl
 License: UNKNOWN
-Project-URL: Documentation, https://momotor.org/doc/engine/momotor-django/release/4.0.0/
+Project-URL: Documentation, https://momotor.org/doc/engine/momotor-django/release/4.1.0/
 Project-URL: Source, https://gitlab.tue.nl/momotor/engine-py3/momotor-django/
 Project-URL: Tracker, https://gitlab.tue.nl/momotor/engine-py3/momotor-django/issues
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 
 This package is a part of [Momotor](https://momotor.org/), a tool for automated processing of digital content.
```

### Comparing `momotor-django-4.0.0/README.md` & `momotor-django-4.1.0/README.md`

 * *Files identical despite different names*

### Comparing `momotor-django-4.0.0/setup.py` & `momotor-django-4.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         'Documentation': f'https://momotor.org/doc/engine/momotor-django/{"dev" if is_dev else "release"}/{full_version}/',
         'Source': 'https://gitlab.tue.nl/momotor/engine-py3/momotor-django/',
         'Tracker': 'https://gitlab.tue.nl/momotor/engine-py3/momotor-django/issues',
     },
     install_requires=[
         'asgiref',
         'backoff',
-        'django>=3.2.0,<4.2.0',
+        'django>=3.2.0,<5',
         'protobuf',
         'momotor-engine-proto~=4.0',
         'momotor-engine-shared~=1.1'
     ],
     extras_require={
         'docs': [
             'Sphinx',
@@ -60,10 +60,11 @@
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3 :: Only',
         'Framework :: Django',
         'Framework :: Django :: 3.2',
         'Framework :: Django :: 4.0',
         'Framework :: Django :: 4.1',
+        'Framework :: Django :: 4.2',
         'License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)',
     ],
 )
```

### Comparing `momotor-django-4.0.0/src/momotor/django/admin.py` & `momotor-django-4.1.0/src/momotor/django/admin.py`

 * *Files identical despite different names*

### Comparing `momotor-django-4.0.0/src/momotor/django/connection.py` & `momotor-django-4.1.0/src/momotor/django/connection.py`

 * *Files identical despite different names*

### Comparing `momotor-django-4.0.0/src/momotor/django/fields.py` & `momotor-django-4.1.0/src/momotor/django/fields.py`

 * *Files identical despite different names*

### Comparing `momotor-django-4.0.0/src/momotor/django/forms.py` & `momotor-django-4.1.0/src/momotor/django/forms.py`

 * *Files identical despite different names*

### Comparing `momotor-django-4.0.0/src/momotor/django/migrations/0001_initial.py` & `momotor-django-4.1.0/src/momotor/django/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `momotor-django-4.0.0/src/momotor/django/token_store/base.py` & `momotor-django-4.1.0/src/momotor/django/token_store/base.py`

 * *Files identical despite different names*

### Comparing `momotor-django-4.0.0/src/momotor/django/token_store/cache.py` & `momotor-django-4.1.0/src/momotor/django/token_store/cache.py`

 * *Files identical despite different names*

### Comparing `momotor-django-4.0.0/src/momotor/django/token_store/memory.py` & `momotor-django-4.1.0/src/momotor/django/token_store/memory.py`

 * *Files identical despite different names*

### Comparing `momotor-django-4.0.0/src/momotor/django/token_store/model.py` & `momotor-django-4.1.0/src/momotor/django/token_store/model.py`

 * *Files identical despite different names*

### Comparing `momotor-django-4.0.0/src/momotor_django.egg-info/PKG-INFO` & `momotor-django-4.1.0/src/momotor_django.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: momotor-django
-Version: 4.0.0
+Version: 4.1.0
 Summary: Momotor bindings for the Django project
 Home-page: https://momotor.org/
 Author: Erik Scheffers
 Author-email: e.t.j.scheffers@tue.nl
 License: UNKNOWN
-Project-URL: Documentation, https://momotor.org/doc/engine/momotor-django/release/4.0.0/
+Project-URL: Documentation, https://momotor.org/doc/engine/momotor-django/release/4.1.0/
 Project-URL: Source, https://gitlab.tue.nl/momotor/engine-py3/momotor-django/
 Project-URL: Tracker, https://gitlab.tue.nl/momotor/engine-py3/momotor-django/issues
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 
 This package is a part of [Momotor](https://momotor.org/), a tool for automated processing of digital content.
```

### Comparing `momotor-django-4.0.0/src/momotor_django.egg-info/SOURCES.txt` & `momotor-django-4.1.0/src/momotor_django.egg-info/SOURCES.txt`

 * *Files identical despite different names*

