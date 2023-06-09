# Comparing `tmp/mitol-django-google-sheets-refunds-2023.5.23.tar.gz` & `tmp/mitol-django-google-sheets-refunds-2023.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mitol-django-google-sheets-refunds-2023.5.23.tar", last modified: Tue May 23 12:08:37 2023, max compression
+gzip compressed data, was "mitol-django-google-sheets-refunds-2023.6.9.tar", last modified: Fri Jun  9 18:32:17 2023, max compression
```

## Comparing `mitol-django-google-sheets-refunds-2023.5.23.tar` & `mitol-django-google-sheets-refunds-2023.6.9.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 12:08:37.404707 mitol-django-google-sheets-refunds-2023.5.23/
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-05-23 12:08:36.000000 mitol-django-google-sheets-refunds-2023.5.23/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     4587 2023-05-23 12:08:37.400707 mitol-django-google-sheets-refunds-2023.5.23/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      625 2023-05-23 12:08:36.000000 mitol-django-google-sheets-refunds-2023.5.23/backend_shim.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 12:08:37.400707 mitol-django-google-sheets-refunds-2023.5.23/mitol/
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-05-23 12:08:36.000000 mitol-django-google-sheets-refunds-2023.5.23/mitol/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 12:08:37.400707 mitol-django-google-sheets-refunds-2023.5.23/mitol/google_sheets_refunds/
--rw-r--r--   0 runner    (1001) docker     (122)      872 2023-05-23 12:08:36.000000 mitol-django-google-sheets-refunds-2023.5.23/mitol/google_sheets_refunds/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)     4044 2023-05-23 12:08:36.000000 mitol-django-google-sheets-refunds-2023.5.23/mitol/google_sheets_refunds/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      202 2023-05-23 12:08:36.000000 mitol-django-google-sheets-refunds-2023.5.23/mitol/google_sheets_refunds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5437 2023-05-23 12:08:36.000000 mitol-django-google-sheets-refunds-2023.5.23/mitol/google_sheets_refunds/api.py
--rw-r--r--   0 runner    (1001) docker     (122)      444 2023-05-23 12:08:36.000000 mitol-django-google-sheets-refunds-2023.5.23/mitol/google_sheets_refunds/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)      264 2023-05-23 12:08:36.000000 mitol-django-google-sheets-refunds-2023.5.23/mitol/google_sheets_refunds/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)      805 2023-05-23 12:08:36.000000 mitol-django-google-sheets-refunds-2023.5.23/mitol/google_sheets_refunds/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 12:08:37.400707 mitol-django-google-sheets-refunds-2023.5.23/mitol/google_sheets_refunds/management/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 12:08:37.400707 mitol-django-google-sheets-refunds-2023.5.23/mitol/google_sheets_refunds/management/commands/
--rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-05-23 12:08:36.000000 mitol-django-google-sheets-refunds-2023.5.23/mitol/google_sheets_refunds/management/commands/process_refund_requests.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 12:08:37.400707 mitol-django-google-sheets-refunds-2023.5.23/mitol/google_sheets_refunds/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     1076 2023-05-23 12:08:36.000000 mitol-django-google-sheets-refunds-2023.5.23/mitol/google_sheets_refunds/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 12:08:36.000000 mitol-django-google-sheets-refunds-2023.5.23/mitol/google_sheets_refunds/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      395 2023-05-23 12:08:36.000000 mitol-django-google-sheets-refunds-2023.5.23/mitol/google_sheets_refunds/models.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 12:08:36.000000 mitol-django-google-sheets-refunds-2023.5.23/mitol/google_sheets_refunds/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 12:08:37.400707 mitol-django-google-sheets-refunds-2023.5.23/mitol/google_sheets_refunds/settings/
--rw-r--r--   0 runner    (1001) docker     (122)     1896 2023-05-23 12:08:36.000000 mitol-django-google-sheets-refunds-2023.5.23/mitol/google_sheets_refunds/settings/google_sheets_refunds.py
--rw-r--r--   0 runner    (1001) docker     (122)     4687 2023-05-23 12:08:36.000000 mitol-django-google-sheets-refunds-2023.5.23/mitol/google_sheets_refunds/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 12:08:37.400707 mitol-django-google-sheets-refunds-2023.5.23/mitol_django_google_sheets_refunds.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4587 2023-05-23 12:08:37.000000 mitol-django-google-sheets-refunds-2023.5.23/mitol_django_google_sheets_refunds.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1086 2023-05-23 12:08:37.000000 mitol-django-google-sheets-refunds-2023.5.23/mitol_django_google_sheets_refunds.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-23 12:08:37.000000 mitol-django-google-sheets-refunds-2023.5.23/mitol_django_google_sheets_refunds.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-23 12:08:37.000000 mitol-django-google-sheets-refunds-2023.5.23/mitol_django_google_sheets_refunds.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (122)       93 2023-05-23 12:08:37.000000 mitol-django-google-sheets-refunds-2023.5.23/mitol_django_google_sheets_refunds.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-23 12:08:37.000000 mitol-django-google-sheets-refunds-2023.5.23/mitol_django_google_sheets_refunds.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-23 12:08:37.000000 mitol-django-google-sheets-refunds-2023.5.23/mitol_django_google_sheets_refunds.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-23 12:08:37.404707 mitol-django-google-sheets-refunds-2023.5.23/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     5594 2023-05-23 12:08:36.000000 mitol-django-google-sheets-refunds-2023.5.23/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 18:32:17.708766 mitol-django-google-sheets-refunds-2023.6.9/
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-06-09 18:32:17.000000 mitol-django-google-sheets-refunds-2023.6.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     4586 2023-06-09 18:32:17.708766 mitol-django-google-sheets-refunds-2023.6.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      625 2023-06-09 18:32:17.000000 mitol-django-google-sheets-refunds-2023.6.9/backend_shim.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 18:32:17.708766 mitol-django-google-sheets-refunds-2023.6.9/mitol/
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-06-09 18:32:17.000000 mitol-django-google-sheets-refunds-2023.6.9/mitol/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 18:32:17.708766 mitol-django-google-sheets-refunds-2023.6.9/mitol/google_sheets_refunds/
+-rw-r--r--   0 runner    (1001) docker     (122)     1060 2023-06-09 18:32:17.000000 mitol-django-google-sheets-refunds-2023.6.9/mitol/google_sheets_refunds/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)     4044 2023-06-09 18:32:17.000000 mitol-django-google-sheets-refunds-2023.6.9/mitol/google_sheets_refunds/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      201 2023-06-09 18:32:17.000000 mitol-django-google-sheets-refunds-2023.6.9/mitol/google_sheets_refunds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      359 2023-06-09 18:32:17.000000 mitol-django-google-sheets-refunds-2023.6.9/mitol/google_sheets_refunds/admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5437 2023-06-09 18:32:17.000000 mitol-django-google-sheets-refunds-2023.6.9/mitol/google_sheets_refunds/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      444 2023-06-09 18:32:17.000000 mitol-django-google-sheets-refunds-2023.6.9/mitol/google_sheets_refunds/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)      264 2023-06-09 18:32:17.000000 mitol-django-google-sheets-refunds-2023.6.9/mitol/google_sheets_refunds/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)      805 2023-06-09 18:32:17.000000 mitol-django-google-sheets-refunds-2023.6.9/mitol/google_sheets_refunds/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 18:32:17.708766 mitol-django-google-sheets-refunds-2023.6.9/mitol/google_sheets_refunds/management/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 18:32:17.708766 mitol-django-google-sheets-refunds-2023.6.9/mitol/google_sheets_refunds/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-06-09 18:32:17.000000 mitol-django-google-sheets-refunds-2023.6.9/mitol/google_sheets_refunds/management/commands/process_refund_requests.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 18:32:17.708766 mitol-django-google-sheets-refunds-2023.6.9/mitol/google_sheets_refunds/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     1076 2023-06-09 18:32:17.000000 mitol-django-google-sheets-refunds-2023.6.9/mitol/google_sheets_refunds/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-09 18:32:17.000000 mitol-django-google-sheets-refunds-2023.6.9/mitol/google_sheets_refunds/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      395 2023-06-09 18:32:17.000000 mitol-django-google-sheets-refunds-2023.6.9/mitol/google_sheets_refunds/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-09 18:32:17.000000 mitol-django-google-sheets-refunds-2023.6.9/mitol/google_sheets_refunds/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 18:32:17.708766 mitol-django-google-sheets-refunds-2023.6.9/mitol/google_sheets_refunds/settings/
+-rw-r--r--   0 runner    (1001) docker     (122)     1896 2023-06-09 18:32:17.000000 mitol-django-google-sheets-refunds-2023.6.9/mitol/google_sheets_refunds/settings/google_sheets_refunds.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4687 2023-06-09 18:32:17.000000 mitol-django-google-sheets-refunds-2023.6.9/mitol/google_sheets_refunds/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 18:32:17.708766 mitol-django-google-sheets-refunds-2023.6.9/mitol_django_google_sheets_refunds.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4586 2023-06-09 18:32:17.000000 mitol-django-google-sheets-refunds-2023.6.9/mitol_django_google_sheets_refunds.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1123 2023-06-09 18:32:17.000000 mitol-django-google-sheets-refunds-2023.6.9/mitol_django_google_sheets_refunds.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-09 18:32:17.000000 mitol-django-google-sheets-refunds-2023.6.9/mitol_django_google_sheets_refunds.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-06-09 18:32:17.000000 mitol-django-google-sheets-refunds-2023.6.9/mitol_django_google_sheets_refunds.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       93 2023-06-09 18:32:17.000000 mitol-django-google-sheets-refunds-2023.6.9/mitol_django_google_sheets_refunds.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-06-09 18:32:17.000000 mitol-django-google-sheets-refunds-2023.6.9/mitol_django_google_sheets_refunds.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-09 18:32:17.000000 mitol-django-google-sheets-refunds-2023.6.9/mitol_django_google_sheets_refunds.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-09 18:32:17.708766 mitol-django-google-sheets-refunds-2023.6.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     5593 2023-06-09 18:32:17.000000 mitol-django-google-sheets-refunds-2023.6.9/setup.py
```

### Comparing `mitol-django-google-sheets-refunds-2023.5.23/PKG-INFO` & `mitol-django-google-sheets-refunds-2023.6.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mitol-django-google-sheets-refunds
-Version: 2023.5.23
+Version: 2023.6.9
 Summary: Library to handle Refund requests using Google Sheets integrations in Django
 License: BSD 3-Clause License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `mitol-django-google-sheets-refunds-2023.5.23/backend_shim.py` & `mitol-django-google-sheets-refunds-2023.6.9/backend_shim.py`

 * *Files identical despite different names*

### Comparing `mitol-django-google-sheets-refunds-2023.5.23/mitol/google_sheets_refunds/CHANGELOG.md` & `mitol-django-google-sheets-refunds-2023.6.9/mitol/google_sheets_refunds/CHANGELOG.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,19 @@
 
+<a id='changelog-2023.6.9'></a>
+## [2023.6.9] - 2023-06-09
+
+### Added
+
+- Added RefundRequestAdmin
+
+### Changed
+
+- Updated README with new better instructions on setup and testing locally
+
 <a id='changelog-2023.5.23'></a>
 ## [2023.5.23] - 2023-05-23
 
 ### Changed
 
 - Updated README with new better instructions on setup and testing locally
 # Changelog
```

### Comparing `mitol-django-google-sheets-refunds-2023.5.23/mitol/google_sheets_refunds/README.md` & `mitol-django-google-sheets-refunds-2023.6.9/mitol/google_sheets_refunds/README.md`

 * *Files identical despite different names*

### Comparing `mitol-django-google-sheets-refunds-2023.5.23/mitol/google_sheets_refunds/api.py` & `mitol-django-google-sheets-refunds-2023.6.9/mitol/google_sheets_refunds/api.py`

 * *Files identical despite different names*

### Comparing `mitol-django-google-sheets-refunds-2023.5.23/mitol/google_sheets_refunds/hooks.py` & `mitol-django-google-sheets-refunds-2023.6.9/mitol/google_sheets_refunds/hooks.py`

 * *Files identical despite different names*

### Comparing `mitol-django-google-sheets-refunds-2023.5.23/mitol/google_sheets_refunds/management/commands/process_refund_requests.py` & `mitol-django-google-sheets-refunds-2023.6.9/mitol/google_sheets_refunds/management/commands/process_refund_requests.py`

 * *Files identical despite different names*

### Comparing `mitol-django-google-sheets-refunds-2023.5.23/mitol/google_sheets_refunds/migrations/0001_initial.py` & `mitol-django-google-sheets-refunds-2023.6.9/mitol/google_sheets_refunds/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `mitol-django-google-sheets-refunds-2023.5.23/mitol/google_sheets_refunds/settings/google_sheets_refunds.py` & `mitol-django-google-sheets-refunds-2023.6.9/mitol/google_sheets_refunds/settings/google_sheets_refunds.py`

 * *Files identical despite different names*

### Comparing `mitol-django-google-sheets-refunds-2023.5.23/mitol/google_sheets_refunds/utils.py` & `mitol-django-google-sheets-refunds-2023.6.9/mitol/google_sheets_refunds/utils.py`

 * *Files identical despite different names*

### Comparing `mitol-django-google-sheets-refunds-2023.5.23/mitol_django_google_sheets_refunds.egg-info/PKG-INFO` & `mitol-django-google-sheets-refunds-2023.6.9/mitol_django_google_sheets_refunds.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mitol-django-google-sheets-refunds
-Version: 2023.5.23
+Version: 2023.6.9
 Summary: Library to handle Refund requests using Google Sheets integrations in Django
 License: BSD 3-Clause License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `mitol-django-google-sheets-refunds-2023.5.23/mitol_django_google_sheets_refunds.egg-info/SOURCES.txt` & `mitol-django-google-sheets-refunds-2023.6.9/mitol_django_google_sheets_refunds.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 MANIFEST.in
 backend_shim.py
 setup.py
 mitol/__init__.py
 mitol/google_sheets_refunds/CHANGELOG.md
 mitol/google_sheets_refunds/README.md
 mitol/google_sheets_refunds/__init__.py
+mitol/google_sheets_refunds/admin.py
 mitol/google_sheets_refunds/api.py
 mitol/google_sheets_refunds/apps.py
 mitol/google_sheets_refunds/constants.py
 mitol/google_sheets_refunds/hooks.py
 mitol/google_sheets_refunds/models.py
 mitol/google_sheets_refunds/py.typed
 mitol/google_sheets_refunds/utils.py
```

### Comparing `mitol-django-google-sheets-refunds-2023.5.23/setup.py` & `mitol-django-google-sheets-refunds-2023.6.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,10 +153,10 @@
         'mitol',
         'mitol.google_sheets_refunds',
         'mitol.google_sheets_refunds.management.commands',
         'mitol.google_sheets_refunds.migrations',
         'mitol.google_sheets_refunds.settings',
     ),
     'python_requires': '>=3.8',
-    'version': '2023.5.23',
+    'version': '2023.6.9',
     'zip_safe': True,
 })
```

