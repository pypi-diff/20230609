# Comparing `tmp/mitol-django-google-sheets-deferrals-2023.5.30.tar.gz` & `tmp/mitol-django-google-sheets-deferrals-2023.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mitol-django-google-sheets-deferrals-2023.5.30.tar", last modified: Tue May 30 13:53:51 2023, max compression
+gzip compressed data, was "mitol-django-google-sheets-deferrals-2023.6.9.tar", last modified: Fri Jun  9 18:09:31 2023, max compression
```

## Comparing `mitol-django-google-sheets-deferrals-2023.5.30.tar` & `mitol-django-google-sheets-deferrals-2023.6.9.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 13:53:51.293285 mitol-django-google-sheets-deferrals-2023.5.30/
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-05-30 13:53:50.000000 mitol-django-google-sheets-deferrals-2023.5.30/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     4652 2023-05-30 13:53:51.293285 mitol-django-google-sheets-deferrals-2023.5.30/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      625 2023-05-30 13:53:50.000000 mitol-django-google-sheets-deferrals-2023.5.30/backend_shim.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 13:53:51.289285 mitol-django-google-sheets-deferrals-2023.5.30/mitol/
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-05-30 13:53:50.000000 mitol-django-google-sheets-deferrals-2023.5.30/mitol/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 13:53:51.289285 mitol-django-google-sheets-deferrals-2023.5.30/mitol/google_sheets_deferrals/
--rw-r--r--   0 runner    (1001) docker     (122)      882 2023-05-30 13:53:50.000000 mitol-django-google-sheets-deferrals-2023.5.30/mitol/google_sheets_deferrals/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)     4105 2023-05-30 13:53:50.000000 mitol-django-google-sheets-deferrals-2023.5.30/mitol/google_sheets_deferrals/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      210 2023-05-30 13:53:50.000000 mitol-django-google-sheets-deferrals-2023.5.30/mitol/google_sheets_deferrals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6038 2023-05-30 13:53:50.000000 mitol-django-google-sheets-deferrals-2023.5.30/mitol/google_sheets_deferrals/api.py
--rw-r--r--   0 runner    (1001) docker     (122)      511 2023-05-30 13:53:50.000000 mitol-django-google-sheets-deferrals-2023.5.30/mitol/google_sheets_deferrals/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)      276 2023-05-30 13:53:50.000000 mitol-django-google-sheets-deferrals-2023.5.30/mitol/google_sheets_deferrals/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)      838 2023-05-30 13:53:50.000000 mitol-django-google-sheets-deferrals-2023.5.30/mitol/google_sheets_deferrals/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 13:53:51.289285 mitol-django-google-sheets-deferrals-2023.5.30/mitol/google_sheets_deferrals/management/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 13:53:51.293285 mitol-django-google-sheets-deferrals-2023.5.30/mitol/google_sheets_deferrals/management/commands/
--rw-r--r--   0 runner    (1001) docker     (122)     1067 2023-05-30 13:53:50.000000 mitol-django-google-sheets-deferrals-2023.5.30/mitol/google_sheets_deferrals/management/commands/process_deferral_requests.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 13:53:51.293285 mitol-django-google-sheets-deferrals-2023.5.30/mitol/google_sheets_deferrals/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     1081 2023-05-30 13:53:50.000000 mitol-django-google-sheets-deferrals-2023.5.30/mitol/google_sheets_deferrals/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-30 13:53:50.000000 mitol-django-google-sheets-deferrals-2023.5.30/mitol/google_sheets_deferrals/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      400 2023-05-30 13:53:50.000000 mitol-django-google-sheets-deferrals-2023.5.30/mitol/google_sheets_deferrals/models.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-30 13:53:50.000000 mitol-django-google-sheets-deferrals-2023.5.30/mitol/google_sheets_deferrals/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 13:53:51.293285 mitol-django-google-sheets-deferrals-2023.5.30/mitol/google_sheets_deferrals/settings/
--rw-r--r--   0 runner    (1001) docker     (122)     1942 2023-05-30 13:53:50.000000 mitol-django-google-sheets-deferrals-2023.5.30/mitol/google_sheets_deferrals/settings/google_sheets_deferrals.py
--rw-r--r--   0 runner    (1001) docker     (122)     4433 2023-05-30 13:53:50.000000 mitol-django-google-sheets-deferrals-2023.5.30/mitol/google_sheets_deferrals/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 13:53:51.293285 mitol-django-google-sheets-deferrals-2023.5.30/mitol_django_google_sheets_deferrals.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4652 2023-05-30 13:53:51.000000 mitol-django-google-sheets-deferrals-2023.5.30/mitol_django_google_sheets_deferrals.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1132 2023-05-30 13:53:51.000000 mitol-django-google-sheets-deferrals-2023.5.30/mitol_django_google_sheets_deferrals.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-30 13:53:51.000000 mitol-django-google-sheets-deferrals-2023.5.30/mitol_django_google_sheets_deferrals.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-30 13:53:51.000000 mitol-django-google-sheets-deferrals-2023.5.30/mitol_django_google_sheets_deferrals.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (122)       93 2023-05-30 13:53:51.000000 mitol-django-google-sheets-deferrals-2023.5.30/mitol_django_google_sheets_deferrals.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-30 13:53:51.000000 mitol-django-google-sheets-deferrals-2023.5.30/mitol_django_google_sheets_deferrals.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-30 13:53:51.000000 mitol-django-google-sheets-deferrals-2023.5.30/mitol_django_google_sheets_deferrals.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-30 13:53:51.293285 mitol-django-google-sheets-deferrals-2023.5.30/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     5673 2023-05-30 13:53:50.000000 mitol-django-google-sheets-deferrals-2023.5.30/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 18:09:31.061163 mitol-django-google-sheets-deferrals-2023.6.9/
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-06-09 18:09:30.000000 mitol-django-google-sheets-deferrals-2023.6.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     4651 2023-06-09 18:09:31.053163 mitol-django-google-sheets-deferrals-2023.6.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      625 2023-06-09 18:09:30.000000 mitol-django-google-sheets-deferrals-2023.6.9/backend_shim.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 18:09:31.049163 mitol-django-google-sheets-deferrals-2023.6.9/mitol/
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-06-09 18:09:30.000000 mitol-django-google-sheets-deferrals-2023.6.9/mitol/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 18:09:31.049163 mitol-django-google-sheets-deferrals-2023.6.9/mitol/google_sheets_deferrals/
+-rw-r--r--   0 runner    (1001) docker     (122)     1192 2023-06-09 18:09:30.000000 mitol-django-google-sheets-deferrals-2023.6.9/mitol/google_sheets_deferrals/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)     4105 2023-06-09 18:09:30.000000 mitol-django-google-sheets-deferrals-2023.6.9/mitol/google_sheets_deferrals/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      209 2023-06-09 18:09:30.000000 mitol-django-google-sheets-deferrals-2023.6.9/mitol/google_sheets_deferrals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      375 2023-06-09 18:09:30.000000 mitol-django-google-sheets-deferrals-2023.6.9/mitol/google_sheets_deferrals/admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6038 2023-06-09 18:09:30.000000 mitol-django-google-sheets-deferrals-2023.6.9/mitol/google_sheets_deferrals/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      511 2023-06-09 18:09:30.000000 mitol-django-google-sheets-deferrals-2023.6.9/mitol/google_sheets_deferrals/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)      276 2023-06-09 18:09:30.000000 mitol-django-google-sheets-deferrals-2023.6.9/mitol/google_sheets_deferrals/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)      838 2023-06-09 18:09:30.000000 mitol-django-google-sheets-deferrals-2023.6.9/mitol/google_sheets_deferrals/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 18:09:31.049163 mitol-django-google-sheets-deferrals-2023.6.9/mitol/google_sheets_deferrals/management/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 18:09:31.049163 mitol-django-google-sheets-deferrals-2023.6.9/mitol/google_sheets_deferrals/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)     1067 2023-06-09 18:09:30.000000 mitol-django-google-sheets-deferrals-2023.6.9/mitol/google_sheets_deferrals/management/commands/process_deferral_requests.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 18:09:31.049163 mitol-django-google-sheets-deferrals-2023.6.9/mitol/google_sheets_deferrals/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     1081 2023-06-09 18:09:30.000000 mitol-django-google-sheets-deferrals-2023.6.9/mitol/google_sheets_deferrals/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-09 18:09:30.000000 mitol-django-google-sheets-deferrals-2023.6.9/mitol/google_sheets_deferrals/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      400 2023-06-09 18:09:30.000000 mitol-django-google-sheets-deferrals-2023.6.9/mitol/google_sheets_deferrals/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-09 18:09:30.000000 mitol-django-google-sheets-deferrals-2023.6.9/mitol/google_sheets_deferrals/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 18:09:31.049163 mitol-django-google-sheets-deferrals-2023.6.9/mitol/google_sheets_deferrals/settings/
+-rw-r--r--   0 runner    (1001) docker     (122)     1942 2023-06-09 18:09:30.000000 mitol-django-google-sheets-deferrals-2023.6.9/mitol/google_sheets_deferrals/settings/google_sheets_deferrals.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4433 2023-06-09 18:09:30.000000 mitol-django-google-sheets-deferrals-2023.6.9/mitol/google_sheets_deferrals/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 18:09:31.053163 mitol-django-google-sheets-deferrals-2023.6.9/mitol_django_google_sheets_deferrals.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4651 2023-06-09 18:09:31.000000 mitol-django-google-sheets-deferrals-2023.6.9/mitol_django_google_sheets_deferrals.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1171 2023-06-09 18:09:31.000000 mitol-django-google-sheets-deferrals-2023.6.9/mitol_django_google_sheets_deferrals.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-09 18:09:31.000000 mitol-django-google-sheets-deferrals-2023.6.9/mitol_django_google_sheets_deferrals.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-06-09 18:09:31.000000 mitol-django-google-sheets-deferrals-2023.6.9/mitol_django_google_sheets_deferrals.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       93 2023-06-09 18:09:31.000000 mitol-django-google-sheets-deferrals-2023.6.9/mitol_django_google_sheets_deferrals.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-06-09 18:09:31.000000 mitol-django-google-sheets-deferrals-2023.6.9/mitol_django_google_sheets_deferrals.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-09 18:09:30.000000 mitol-django-google-sheets-deferrals-2023.6.9/mitol_django_google_sheets_deferrals.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-09 18:09:31.061163 mitol-django-google-sheets-deferrals-2023.6.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     5672 2023-06-09 18:09:30.000000 mitol-django-google-sheets-deferrals-2023.6.9/setup.py
```

### Comparing `mitol-django-google-sheets-deferrals-2023.5.30/PKG-INFO` & `mitol-django-google-sheets-deferrals-2023.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mitol-django-google-sheets-deferrals
-Version: 2023.5.30
+Version: 2023.6.9
 Summary: Library to handle Deferral requests using Google Sheets integrations in Django
 License: BSD 3-Clause License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `mitol-django-google-sheets-deferrals-2023.5.30/backend_shim.py` & `mitol-django-google-sheets-deferrals-2023.6.9/backend_shim.py`

 * *Files identical despite different names*

### Comparing `mitol-django-google-sheets-deferrals-2023.5.30/mitol/google_sheets_deferrals/CHANGELOG.md` & `mitol-django-google-sheets-deferrals-2023.6.9/mitol/google_sheets_deferrals/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,25 @@
 
+<a id='changelog-2023.6.9'></a>
+## [2023.6.9] - 2023-06-09
+
+### Added
+
+- Added the `mitol-django-google-sheets-deferrals` app
+
+- Added implementation of filter_ignored_rows to request handler
+
+- Added DeferralRequestAdmin
+
+### Changed
+
+- Updated release version format
+
+- Set default_auto_field in app config
+
 <a id='changelog-2023.5.30'></a>
 ## [2023.5.30] - 2023-05-30
 
 ### Added
 
 - Added the `mitol-django-google-sheets-deferrals` app
```

### Comparing `mitol-django-google-sheets-deferrals-2023.5.30/mitol/google_sheets_deferrals/README.md` & `mitol-django-google-sheets-deferrals-2023.6.9/mitol/google_sheets_deferrals/README.md`

 * *Files identical despite different names*

### Comparing `mitol-django-google-sheets-deferrals-2023.5.30/mitol/google_sheets_deferrals/api.py` & `mitol-django-google-sheets-deferrals-2023.6.9/mitol/google_sheets_deferrals/api.py`

 * *Files identical despite different names*

### Comparing `mitol-django-google-sheets-deferrals-2023.5.30/mitol/google_sheets_deferrals/hooks.py` & `mitol-django-google-sheets-deferrals-2023.6.9/mitol/google_sheets_deferrals/hooks.py`

 * *Files identical despite different names*

### Comparing `mitol-django-google-sheets-deferrals-2023.5.30/mitol/google_sheets_deferrals/management/commands/process_deferral_requests.py` & `mitol-django-google-sheets-deferrals-2023.6.9/mitol/google_sheets_deferrals/management/commands/process_deferral_requests.py`

 * *Files identical despite different names*

### Comparing `mitol-django-google-sheets-deferrals-2023.5.30/mitol/google_sheets_deferrals/migrations/0001_initial.py` & `mitol-django-google-sheets-deferrals-2023.6.9/mitol/google_sheets_deferrals/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `mitol-django-google-sheets-deferrals-2023.5.30/mitol/google_sheets_deferrals/settings/google_sheets_deferrals.py` & `mitol-django-google-sheets-deferrals-2023.6.9/mitol/google_sheets_deferrals/settings/google_sheets_deferrals.py`

 * *Files identical despite different names*

### Comparing `mitol-django-google-sheets-deferrals-2023.5.30/mitol/google_sheets_deferrals/utils.py` & `mitol-django-google-sheets-deferrals-2023.6.9/mitol/google_sheets_deferrals/utils.py`

 * *Files identical despite different names*

### Comparing `mitol-django-google-sheets-deferrals-2023.5.30/mitol_django_google_sheets_deferrals.egg-info/PKG-INFO` & `mitol-django-google-sheets-deferrals-2023.6.9/mitol_django_google_sheets_deferrals.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mitol-django-google-sheets-deferrals
-Version: 2023.5.30
+Version: 2023.6.9
 Summary: Library to handle Deferral requests using Google Sheets integrations in Django
 License: BSD 3-Clause License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `mitol-django-google-sheets-deferrals-2023.5.30/mitol_django_google_sheets_deferrals.egg-info/SOURCES.txt` & `mitol-django-google-sheets-deferrals-2023.6.9/mitol_django_google_sheets_deferrals.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 MANIFEST.in
 backend_shim.py
 setup.py
 mitol/__init__.py
 mitol/google_sheets_deferrals/CHANGELOG.md
 mitol/google_sheets_deferrals/README.md
 mitol/google_sheets_deferrals/__init__.py
+mitol/google_sheets_deferrals/admin.py
 mitol/google_sheets_deferrals/api.py
 mitol/google_sheets_deferrals/apps.py
 mitol/google_sheets_deferrals/constants.py
 mitol/google_sheets_deferrals/hooks.py
 mitol/google_sheets_deferrals/models.py
 mitol/google_sheets_deferrals/py.typed
 mitol/google_sheets_deferrals/utils.py
```

### Comparing `mitol-django-google-sheets-deferrals-2023.5.30/setup.py` & `mitol-django-google-sheets-deferrals-2023.6.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,10 +152,10 @@
         'mitol',
         'mitol.google_sheets_deferrals',
         'mitol.google_sheets_deferrals.management.commands',
         'mitol.google_sheets_deferrals.migrations',
         'mitol.google_sheets_deferrals.settings',
     ),
     'python_requires': '>=3.8',
-    'version': '2023.5.30',
+    'version': '2023.6.9',
     'zip_safe': True,
 })
```

