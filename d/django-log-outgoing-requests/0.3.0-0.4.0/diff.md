# Comparing `tmp/django-log-outgoing-requests-0.3.0.tar.gz` & `tmp/django-log-outgoing-requests-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-log-outgoing-requests-0.3.0.tar", last modified: Thu Jun  8 15:50:35 2023, max compression
+gzip compressed data, was "django-log-outgoing-requests-0.4.0.tar", last modified: Fri Jun  9 10:19:38 2023, max compression
```

## Comparing `django-log-outgoing-requests-0.3.0.tar` & `django-log-outgoing-requests-0.4.0.tar`

### file list

```diff
@@ -1,50 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:50:35.588390 django-log-outgoing-requests-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-08 15:50:30.000000 django-log-outgoing-requests-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-08 15:50:30.000000 django-log-outgoing-requests-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-06-08 15:50:35.588390 django-log-outgoing-requests-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-06-08 15:50:30.000000 django-log-outgoing-requests-0.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:50:35.584390 django-log-outgoing-requests-0.3.0/django_log_outgoing_requests.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-06-08 15:50:35.000000 django-log-outgoing-requests-0.3.0/django_log_outgoing_requests.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-08 15:50:35.000000 django-log-outgoing-requests-0.3.0/django_log_outgoing_requests.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 15:50:35.000000 django-log-outgoing-requests-0.3.0/django_log_outgoing_requests.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 15:50:35.000000 django-log-outgoing-requests-0.3.0/django_log_outgoing_requests.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-08 15:50:35.000000 django-log-outgoing-requests-0.3.0/django_log_outgoing_requests.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-08 15:50:35.000000 django-log-outgoing-requests-0.3.0/django_log_outgoing_requests.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:50:35.588390 django-log-outgoing-requests-0.3.0/log_outgoing_requests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:50:30.000000 django-log-outgoing-requests-0.3.0/log_outgoing_requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-08 15:50:30.000000 django-log-outgoing-requests-0.3.0/log_outgoing_requests/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-08 15:50:30.000000 django-log-outgoing-requests-0.3.0/log_outgoing_requests/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-06-08 15:50:30.000000 django-log-outgoing-requests-0.3.0/log_outgoing_requests/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-06-08 15:50:30.000000 django-log-outgoing-requests-0.3.0/log_outgoing_requests/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-08 15:50:30.000000 django-log-outgoing-requests-0.3.0/log_outgoing_requests/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-08 15:50:30.000000 django-log-outgoing-requests-0.3.0/log_outgoing_requests/datastructures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-06-08 15:50:30.000000 django-log-outgoing-requests-0.3.0/log_outgoing_requests/formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-06-08 15:50:30.000000 django-log-outgoing-requests-0.3.0/log_outgoing_requests/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:50:35.584390 django-log-outgoing-requests-0.3.0/log_outgoing_requests/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:50:35.584390 django-log-outgoing-requests-0.3.0/log_outgoing_requests/locale/nl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:50:35.588390 django-log-outgoing-requests-0.3.0/log_outgoing_requests/locale/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-06-08 15:50:30.000000 django-log-outgoing-requests-0.3.0/log_outgoing_requests/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-06-08 15:50:30.000000 django-log-outgoing-requests-0.3.0/log_outgoing_requests/locale/nl/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-08 15:50:30.000000 django-log-outgoing-requests-0.3.0/log_outgoing_requests/log_requests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:50:35.588390 django-log-outgoing-requests-0.3.0/log_outgoing_requests/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     4799 2023-06-08 15:50:30.000000 django-log-outgoing-requests-0.3.0/log_outgoing_requests/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-06-08 15:50:30.000000 django-log-outgoing-requests-0.3.0/log_outgoing_requests/migrations/0002_outgoingrequestslogconfig_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-08 15:50:30.000000 django-log-outgoing-requests-0.3.0/log_outgoing_requests/migrations/0003_alter_outgoingrequestslog_options_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:50:30.000000 django-log-outgoing-requests-0.3.0/log_outgoing_requests/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-06-08 15:50:30.000000 django-log-outgoing-requests-0.3.0/log_outgoing_requests/models.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:50:30.000000 django-log-outgoing-requests-0.3.0/log_outgoing_requests/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:50:35.584390 django-log-outgoing-requests-0.3.0/log_outgoing_requests/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:50:35.584390 django-log-outgoing-requests-0.3.0/log_outgoing_requests/static/log_outgoing_requests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:50:35.588390 django-log-outgoing-requests-0.3.0/log_outgoing_requests/static/log_outgoing_requests/css/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-08 15:50:30.000000 django-log-outgoing-requests-0.3.0/log_outgoing_requests/static/log_outgoing_requests/css/admin.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:50:35.584390 django-log-outgoing-requests-0.3.0/log_outgoing_requests/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:50:35.588390 django-log-outgoing-requests-0.3.0/log_outgoing_requests/templates/log_outgoing_requests/
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-08 15:50:30.000000 django-log-outgoing-requests-0.3.0/log_outgoing_requests/templates/log_outgoing_requests/change_form.html
--rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-06-08 15:50:30.000000 django-log-outgoing-requests-0.3.0/log_outgoing_requests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-06-08 15:50:35.592390 django-log-outgoing-requests-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 15:50:30.000000 django-log-outgoing-requests-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:50:35.588390 django-log-outgoing-requests-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-06-08 15:50:30.000000 django-log-outgoing-requests-0.3.0/tests/test_admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-08 15:50:30.000000 django-log-outgoing-requests-0.3.0/tests/test_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8064 2023-06-08 15:50:30.000000 django-log-outgoing-requests-0.3.0/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-06-08 15:50:30.000000 django-log-outgoing-requests-0.3.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:19:38.866729 django-log-outgoing-requests-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-09 10:19:34.000000 django-log-outgoing-requests-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-09 10:19:34.000000 django-log-outgoing-requests-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-06-09 10:19:38.866729 django-log-outgoing-requests-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-06-09 10:19:34.000000 django-log-outgoing-requests-0.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:19:38.862729 django-log-outgoing-requests-0.4.0/django_log_outgoing_requests.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-06-09 10:19:38.000000 django-log-outgoing-requests-0.4.0/django_log_outgoing_requests.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-06-09 10:19:38.000000 django-log-outgoing-requests-0.4.0/django_log_outgoing_requests.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 10:19:38.000000 django-log-outgoing-requests-0.4.0/django_log_outgoing_requests.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 10:19:38.000000 django-log-outgoing-requests-0.4.0/django_log_outgoing_requests.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-09 10:19:38.000000 django-log-outgoing-requests-0.4.0/django_log_outgoing_requests.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-09 10:19:38.000000 django-log-outgoing-requests-0.4.0/django_log_outgoing_requests.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:19:38.862729 django-log-outgoing-requests-0.4.0/log_outgoing_requests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 10:19:34.000000 django-log-outgoing-requests-0.4.0/log_outgoing_requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-06-09 10:19:34.000000 django-log-outgoing-requests-0.4.0/log_outgoing_requests/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-09 10:19:34.000000 django-log-outgoing-requests-0.4.0/log_outgoing_requests/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-06-09 10:19:34.000000 django-log-outgoing-requests-0.4.0/log_outgoing_requests/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-06-09 10:19:34.000000 django-log-outgoing-requests-0.4.0/log_outgoing_requests/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-09 10:19:34.000000 django-log-outgoing-requests-0.4.0/log_outgoing_requests/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-09 10:19:34.000000 django-log-outgoing-requests-0.4.0/log_outgoing_requests/datastructures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-06-09 10:19:34.000000 django-log-outgoing-requests-0.4.0/log_outgoing_requests/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-06-09 10:19:34.000000 django-log-outgoing-requests-0.4.0/log_outgoing_requests/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:19:38.858729 django-log-outgoing-requests-0.4.0/log_outgoing_requests/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:19:38.858729 django-log-outgoing-requests-0.4.0/log_outgoing_requests/locale/nl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:19:38.862729 django-log-outgoing-requests-0.4.0/log_outgoing_requests/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-06-09 10:19:34.000000 django-log-outgoing-requests-0.4.0/log_outgoing_requests/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-06-09 10:19:34.000000 django-log-outgoing-requests-0.4.0/log_outgoing_requests/locale/nl/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-09 10:19:34.000000 django-log-outgoing-requests-0.4.0/log_outgoing_requests/log_requests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:19:38.866729 django-log-outgoing-requests-0.4.0/log_outgoing_requests/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     4799 2023-06-09 10:19:34.000000 django-log-outgoing-requests-0.4.0/log_outgoing_requests/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-06-09 10:19:34.000000 django-log-outgoing-requests-0.4.0/log_outgoing_requests/migrations/0002_outgoingrequestslogconfig_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-09 10:19:34.000000 django-log-outgoing-requests-0.4.0/log_outgoing_requests/migrations/0003_alter_outgoingrequestslog_options_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-06-09 10:19:34.000000 django-log-outgoing-requests-0.4.0/log_outgoing_requests/migrations/0004_alter_outgoingrequestslog_hostname_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 10:19:34.000000 django-log-outgoing-requests-0.4.0/log_outgoing_requests/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7133 2023-06-09 10:19:34.000000 django-log-outgoing-requests-0.4.0/log_outgoing_requests/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 10:19:34.000000 django-log-outgoing-requests-0.4.0/log_outgoing_requests/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:19:38.862729 django-log-outgoing-requests-0.4.0/log_outgoing_requests/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:19:38.862729 django-log-outgoing-requests-0.4.0/log_outgoing_requests/static/log_outgoing_requests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:19:38.866729 django-log-outgoing-requests-0.4.0/log_outgoing_requests/static/log_outgoing_requests/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-09 10:19:34.000000 django-log-outgoing-requests-0.4.0/log_outgoing_requests/static/log_outgoing_requests/css/admin.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-06-09 10:19:34.000000 django-log-outgoing-requests-0.4.0/log_outgoing_requests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-06-09 10:19:38.866729 django-log-outgoing-requests-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 10:19:34.000000 django-log-outgoing-requests-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:19:38.866729 django-log-outgoing-requests-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-06-09 10:19:34.000000 django-log-outgoing-requests-0.4.0/tests/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-09 10:19:34.000000 django-log-outgoing-requests-0.4.0/tests/test_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8064 2023-06-09 10:19:34.000000 django-log-outgoing-requests-0.4.0/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-06-09 10:19:34.000000 django-log-outgoing-requests-0.4.0/tests/test_utils.py
```

### Comparing `django-log-outgoing-requests-0.3.0/LICENSE` & `django-log-outgoing-requests-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-log-outgoing-requests-0.3.0/PKG-INFO` & `django-log-outgoing-requests-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-log-outgoing-requests
-Version: 0.3.0
+Version: 0.4.0
 Summary: Log outgoing requests made by the requests python library
 Home-page: https://github.com/maykinmedia/django-log-outgoing-requests
 Author: Maykin Media
 Author-email: support@maykinmedia.nl
 License: MIT
 Project-URL: Documentation, http://django-log-outgoing-requests.readthedocs.io/en/latest/
 Project-URL: Changelog, https://github.com/maykinmedia/django-log-outgoing-requests/blob/main/CHANGELOG.rst
@@ -31,15 +31,15 @@
 Provides-Extra: docs
 Provides-Extra: release
 License-File: LICENSE
 
 django-log-outgoing-requests
 =================================================
 
-:Version: 0.3.0
+:Version: 0.4.0
 :Source: https://github.com/maykinmedia/django-log-outgoing-requests
 :Keywords: logging, django, requests
 :PythonVersion: 3.8+
 
 |build-status| |code-quality| |black| |coverage| |docs|
 
 |python-versions| |django-versions| |pypi-version|
```

### Comparing `django-log-outgoing-requests-0.3.0/README.rst` & `django-log-outgoing-requests-0.4.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 django-log-outgoing-requests
 =================================================
 
-:Version: 0.3.0
+:Version: 0.4.0
 :Source: https://github.com/maykinmedia/django-log-outgoing-requests
 :Keywords: logging, django, requests
 :PythonVersion: 3.8+
 
 |build-status| |code-quality| |black| |coverage| |docs|
 
 |python-versions| |django-versions| |pypi-version|
```

### Comparing `django-log-outgoing-requests-0.3.0/django_log_outgoing_requests.egg-info/PKG-INFO` & `django-log-outgoing-requests-0.4.0/django_log_outgoing_requests.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-log-outgoing-requests
-Version: 0.3.0
+Version: 0.4.0
 Summary: Log outgoing requests made by the requests python library
 Home-page: https://github.com/maykinmedia/django-log-outgoing-requests
 Author: Maykin Media
 Author-email: support@maykinmedia.nl
 License: MIT
 Project-URL: Documentation, http://django-log-outgoing-requests.readthedocs.io/en/latest/
 Project-URL: Changelog, https://github.com/maykinmedia/django-log-outgoing-requests/blob/main/CHANGELOG.rst
@@ -31,15 +31,15 @@
 Provides-Extra: docs
 Provides-Extra: release
 License-File: LICENSE
 
 django-log-outgoing-requests
 =================================================
 
-:Version: 0.3.0
+:Version: 0.4.0
 :Source: https://github.com/maykinmedia/django-log-outgoing-requests
 :Keywords: logging, django, requests
 :PythonVersion: 3.8+
 
 |build-status| |code-quality| |black| |coverage| |docs|
 
 |python-versions| |django-versions| |pypi-version|
```

### Comparing `django-log-outgoing-requests-0.3.0/django_log_outgoing_requests.egg-info/SOURCES.txt` & `django-log-outgoing-requests-0.4.0/django_log_outgoing_requests.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -23,14 +23,14 @@
 log_outgoing_requests/py.typed
 log_outgoing_requests/utils.py
 log_outgoing_requests/locale/nl/LC_MESSAGES/django.mo
 log_outgoing_requests/locale/nl/LC_MESSAGES/django.po
 log_outgoing_requests/migrations/0001_initial.py
 log_outgoing_requests/migrations/0002_outgoingrequestslogconfig_and_more.py
 log_outgoing_requests/migrations/0003_alter_outgoingrequestslog_options_and_more.py
+log_outgoing_requests/migrations/0004_alter_outgoingrequestslog_hostname_and_more.py
 log_outgoing_requests/migrations/__init__.py
 log_outgoing_requests/static/log_outgoing_requests/css/admin.css
-log_outgoing_requests/templates/log_outgoing_requests/change_form.html
 tests/test_admin.py
 tests/test_formatter.py
 tests/test_logging.py
 tests/test_utils.py
```

### Comparing `django-log-outgoing-requests-0.3.0/log_outgoing_requests/admin.py` & `django-log-outgoing-requests-0.4.0/log_outgoing_requests/admin.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,60 +6,97 @@
 
 from .conf import settings
 from .models import OutgoingRequestsLog, OutgoingRequestsLogConfig
 
 
 @admin.register(OutgoingRequestsLog)
 class OutgoingRequestsLogAdmin(admin.ModelAdmin):
-    fields = (
-        "url",
-        "hostname",
-        "query_params",
-        "params",
-        "status_code",
-        "method",
-        "response_ms",
-        "timestamp",
-        "req_content_type",
-        "res_content_type",
-        "req_headers",
-        "res_headers",
-        "trace",
-    )
-    readonly_fields = fields
     list_display = (
         "hostname",
         "url",
         "params",
         "status_code",
         "method",
         "response_ms",
         "timestamp",
     )
     list_filter = ("method", "timestamp", "status_code", "hostname")
     search_fields = ("url", "params", "hostname")
     date_hierarchy = "timestamp"
     show_full_result_count = False
-    change_form_template = "log_outgoing_requests/change_form.html"
+
+    fieldsets = (
+        (
+            _("Request"),
+            {
+                "fields": (
+                    "method",
+                    "url",
+                    "timestamp",
+                    "query_params",
+                    "params",
+                    "req_headers",
+                    "req_content_type",
+                    "req_body_encoding",
+                    "request_body",
+                )
+            },
+        ),
+        (
+            _("Response"),
+            {
+                "fields": (
+                    "status_code",
+                    "response_ms",
+                    "res_headers",
+                    "res_content_type",
+                    "res_body_encoding",
+                    "response_body",
+                )
+            },
+        ),
+        (_("Extra"), {"fields": ("trace",)}),
+    )
+    readonly_fields = (
+        "url",
+        "timestamp",
+        "method",
+        "query_params",
+        "params",
+        "req_headers",
+        "req_content_type",
+        "request_body",
+        "status_code",
+        "response_ms",
+        "res_headers",
+        "res_content_type",
+        "response_body",
+        "trace",
+    )
 
     class Media:
         css = {
             "all": ("log_outgoing_requests/css/admin.css",),
         }
 
     def has_add_permission(self, request):
         return False
 
-    def has_change_permission(self, request, obj=None):
-        return False
-
     @admin.display(description=_("Query parameters"))
     def query_params(self, obj):
         return obj.query_params
 
+    @admin.display(description=_("Request body"))
+    def request_body(self, obj) -> str:
+        return obj.request_body_decoded or "-"
+
+    @admin.display(description=_("Response body"))
+    def response_body(self, obj) -> str:
+        return obj.response_body_decoded or "-"
+
 
 class ConfigAdminForm(forms.ModelForm):
     class Meta:
         model = OutgoingRequestsLogConfig
         fields = "__all__"
         help_texts = {
             "save_to_db": _(
```

### Comparing `django-log-outgoing-requests-0.3.0/log_outgoing_requests/compat.py` & `django-log-outgoing-requests-0.4.0/log_outgoing_requests/compat.py`

 * *Files identical despite different names*

### Comparing `django-log-outgoing-requests-0.3.0/log_outgoing_requests/conf.py` & `django-log-outgoing-requests-0.4.0/log_outgoing_requests/conf.py`

 * *Files identical despite different names*

### Comparing `django-log-outgoing-requests-0.3.0/log_outgoing_requests/datastructures.py` & `django-log-outgoing-requests-0.4.0/log_outgoing_requests/datastructures.py`

 * *Files identical despite different names*

### Comparing `django-log-outgoing-requests-0.3.0/log_outgoing_requests/formatters.py` & `django-log-outgoing-requests-0.4.0/log_outgoing_requests/formatters.py`

 * *Files identical despite different names*

### Comparing `django-log-outgoing-requests-0.3.0/log_outgoing_requests/handlers.py` & `django-log-outgoing-requests-0.4.0/log_outgoing_requests/handlers.py`

 * *Files identical despite different names*

### Comparing `django-log-outgoing-requests-0.3.0/log_outgoing_requests/locale/nl/LC_MESSAGES/django.po` & `django-log-outgoing-requests-0.4.0/log_outgoing_requests/locale/nl/LC_MESSAGES/django.po`

 * *Files 23% similar despite different names*

```diff
@@ -4,43 +4,64 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: 0.2.0\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-08 07:48-0500\n"
+"POT-Creation-Date: 2023-06-09 05:11-0500\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Sergei Maertens <sergei@maykinmedia.nl>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
-#: admin.py:55
+
+#: admin.py:29
+msgid "Request"
+msgstr "Request"
+
+#: admin.py:45
+msgid "Response"
+msgstr "Response"
+
+#: admin.py:57
+msgid "Extra"
+msgstr "Overig"
+
+#: admin.py:84
 msgid "Query parameters"
 msgstr "Query parameters"
 
-#: admin.py:66
+#: admin.py:88 models.py:70 models.py:151
+msgid "Request body"
+msgstr "Request inhoud"
+
+#: admin.py:92 models.py:83 models.py:160
+msgid "Response body"
+msgstr "Response inhoud"
+
+#: admin.py:103
 #, python-brace-format
 msgid ""
 "Whether request logs should be saved to the database (default: {default})."
-msgstr ""
-"Sla request logs op in de database (standaardconfiguratie: {default})."
+msgstr "Sla request logs op in de database (standaardconfiguratie: {default})."
 
-#: admin.py:69
+#: admin.py:106
 #, python-brace-format
 msgid ""
 "Whether the body of the request and response should be logged (default: "
 "{default})."
 msgstr ""
-"Sla request- en response-inhoud op in de database (standaardconfiguratie: {default})."
+"Sla request- en response-inhoud op in de database (standaardconfiguratie: "
+"{default})."
 
-#: apps.py:7 models.py:107
+#: apps.py:7 models.py:112
 msgid "Outgoing request logs"
 msgstr "Uitgaande request-logs"
 
 #: constants.py:6
 msgid "Use default"
 msgstr "Gebruik standaardconfiguratie"
 
@@ -52,144 +73,166 @@
 msgid "No"
 msgstr "Nee"
 
 #: models.py:20
 msgid "URL"
 msgstr "URL"
 
-#: models.py:23
+#: models.py:22
 msgid "The url of the outgoing request."
 msgstr "De URL waar de request heen gestuurd is."
 
-#: models.py:28
+#: models.py:27
 msgid "Hostname"
 msgstr "Hostnaam"
 
-#: models.py:31
+#: models.py:29
 msgid "The netloc/hostname part of the url."
 msgstr "De hostnaam (inclusief poort) van de URL."
 
-#: models.py:34
+#: models.py:32
 msgid "Parameters"
 msgstr "Parameters"
 
-#: models.py:36
+#: models.py:34
 msgid "The parameters (if they exist)."
 msgstr "Eventuele parameters."
 
-#: models.py:39
+#: models.py:37
 msgid "Status code"
 msgstr "HTTP-statuscode"
 
-#: models.py:42
+#: models.py:40
 msgid "The status code of the response."
 msgstr "De statuscode van de response."
 
-#: models.py:45
+#: models.py:43
 msgid "Method"
 msgstr "HTTP-methode"
 
-#: models.py:48
+#: models.py:46
 msgid "The type of request method."
 msgstr "Het soort HTTP request."
 
 #: models.py:51
 msgid "Request content type"
 msgstr "Request content-type"
 
-#: models.py:54
+#: models.py:53
 msgid "The content type of the request."
 msgstr "Het HTTP Content-Type van de request."
 
-#: models.py:57
-msgid "Response content type"
-msgstr "Response content-type"
-
-#: models.py:60
-msgid "The content type of the response."
-msgstr "Het HTTP Content-Type van de response."
-
-#: models.py:63
+#: models.py:56
 msgid "Request headers"
 msgstr "Request headers"
 
-#: models.py:65
+#: models.py:56
 msgid "The request headers."
 msgstr "De HTTP-headers van de request."
 
-#: models.py:68
-msgid "Response headers"
-msgstr "Response headers"
-
-#: models.py:70
-msgid "The response headers."
-msgstr "De HTTP-headers van de response."
+#: models.py:59
+msgid "Request encoding"
+msgstr "Request encoding"
 
-#: models.py:73
-msgid "Request body"
-msgstr "Request inhoud"
+#: models.py:63
+msgid ""
+"The encoding is either extracted from the Content-Type header or, if absent, "
+"taken from the default encoding configured for the content type. If the "
+"decoded request content is not displaying correctly, you may try changing "
+"the encoding value here."
+msgstr ""
+"De encoding is afgeleid uit de Content-Type header, of, indien niet aanwezig, "
+"uit de standaardinstellingen for het content type. Indien de request-inhoud niet "
+"goed weergegeven wordt, dan kan je een andere encoding proberen."
 
-#: models.py:75
+#: models.py:70
 msgid "The request body."
 msgstr "De content/body van de request."
 
-#: models.py:78
-msgid "Response body"
-msgstr "Response inhoud"
+#: models.py:75
+msgid "Response content type"
+msgstr "Response content-type"
+
+#: models.py:77
+msgid "The content type of the response."
+msgstr "Het HTTP Content-Type van de response."
+
+#: models.py:80
+msgid "Response headers"
+msgstr "Response headers"
 
 #: models.py:80
+msgid "The response headers."
+msgstr "De HTTP-headers van de response."
+
+#: models.py:83
 msgid "The response body."
 msgstr "De content/body van de response."
 
-#: models.py:91
+#: models.py:86
+msgid "Response encoding"
+msgstr "Response encoding"
+
+#: models.py:90
+msgid ""
+"The encoding is either extracted from the Content-Type header or, if absent, "
+"taken from the default encoding configured for the content type. If the "
+"decoded response content is not displaying correctly, you may try changing "
+"the encoding value here."
+msgstr ""
+"De encoding is afgeleid uit de Content-Type header, of, indien niet aanwezig, "
+"uit de standaardinstellingen for het content type. Indien de response-inhoud niet "
+"goed weergegeven wordt, dan kan je een andere encoding proberen."
+
+#: models.py:97
 msgid "Response in ms"
 msgstr "Duur in ms"
 
-#: models.py:93
+#: models.py:99
 msgid "This is the response time in ms."
 msgstr ""
 "De tijd dat het duurde tussen versturen van de request en ontvangen van de "
 "response, in ms."
 
-#: models.py:96
+#: models.py:102
 msgid "Timestamp"
 msgstr "Tijdstip"
 
-#: models.py:97
+#: models.py:103
 msgid "This is the date and time the API call was made."
 msgstr "Tijdstip wanneer de request gemaakt is."
 
-#: models.py:100
+#: models.py:106
 msgid "Trace"
 msgstr "Traceback"
 
-#: models.py:102
+#: models.py:107
 msgid "Text providing information in case of request failure."
 msgstr "Technische traceback indien er een crash was."
 
-#: models.py:106
+#: models.py:111
 msgid "Outgoing request log"
 msgstr "Uitgaand request logrecord"
 
-#: models.py:165
+#: models.py:174
 msgid "Save logs to database"
 msgstr "Logs opslaan in de database"
 
-#: models.py:171
+#: models.py:180
 msgid "Save request + response body"
 msgstr "Sla de inhoud van request en/of response op in de database."
 
-#: models.py:177
+#: models.py:186
 msgid "Maximal content size"
 msgstr "Maximale content-grootte"
 
-#: models.py:181
+#: models.py:190
 msgid ""
 "The maximal size of the request/response content (in bytes). If 'Require "
 "content length' is not checked, this setting has no effect."
 msgstr ""
-"De maximale grootte van de request/response-inhoud (in bytes). Inhoud die deze "
-"grootte overschrijdt, dan wordt de inhoud niet opgeslagen."
+"De maximale grootte van de request/response-inhoud (in bytes). Inhoud die "
+"deze grootte overschrijdt, dan wordt de inhoud niet opgeslagen."
 
-#: models.py:205
+#: models.py:214
 msgid "Outgoing request log configuration"
 msgstr "Uitgaande request-logging configuratie"
```

### Comparing `django-log-outgoing-requests-0.3.0/log_outgoing_requests/log_requests.py` & `django-log-outgoing-requests-0.4.0/log_outgoing_requests/log_requests.py`

 * *Files identical despite different names*

### Comparing `django-log-outgoing-requests-0.3.0/log_outgoing_requests/migrations/0001_initial.py` & `django-log-outgoing-requests-0.4.0/log_outgoing_requests/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-log-outgoing-requests-0.3.0/log_outgoing_requests/migrations/0002_outgoingrequestslogconfig_and_more.py` & `django-log-outgoing-requests-0.4.0/log_outgoing_requests/migrations/0002_outgoingrequestslogconfig_and_more.py`

 * *Files identical despite different names*

### Comparing `django-log-outgoing-requests-0.3.0/log_outgoing_requests/migrations/0003_alter_outgoingrequestslog_options_and_more.py` & `django-log-outgoing-requests-0.4.0/log_outgoing_requests/migrations/0003_alter_outgoingrequestslog_options_and_more.py`

 * *Files identical despite different names*

### Comparing `django-log-outgoing-requests-0.3.0/log_outgoing_requests/models.py` & `django-log-outgoing-requests-0.4.0/log_outgoing_requests/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,23 +15,21 @@
 logger = logging.getLogger(__name__)
 
 
 class OutgoingRequestsLog(models.Model):
     url = models.URLField(
         verbose_name=_("URL"),
         max_length=1000,
-        default="",
         help_text=_("The url of the outgoing request."),
     )
 
     # hostname is added so we can filter on it in the admin page
     hostname = models.CharField(
         verbose_name=_("Hostname"),
         max_length=255,
-        default="",
         help_text=_("The netloc/hostname part of the url."),
     )
     params = models.TextField(
         verbose_name=_("Parameters"),
         blank=True,
         help_text=_("The parameters (if they exist)."),
     )
@@ -43,66 +41,73 @@
     )
     method = models.CharField(
         verbose_name=_("Method"),
         max_length=10,
         blank=True,
         help_text=_("The type of request method."),
     )
+
+    # Request content
     req_content_type = models.CharField(
         verbose_name=_("Request content type"),
         max_length=50,
-        default="",
         help_text=_("The content type of the request."),
     )
+    req_headers = models.TextField(
+        verbose_name=_("Request headers"), help_text=_("The request headers.")
+    )
+    req_body_encoding = models.CharField(
+        _("Request encoding"),
+        max_length=24,
+        blank=True,
+        help_text=_(
+            "The encoding is either extracted from the Content-Type header or, if "
+            "absent, taken from the default encoding configured for the content type. "
+            "If the decoded request content is not displaying correctly, you may try "
+            "changing the encoding value here."
+        ),
+    )
+    req_body = models.BinaryField(
+        verbose_name=_("Request body"), default=b"", help_text=_("The request body.")
+    )
+
+    # Response content
     res_content_type = models.CharField(
         verbose_name=_("Response content type"),
         max_length=50,
-        default="",
         help_text=_("The content type of the response."),
     )
-    req_headers = models.TextField(
-        verbose_name=_("Request headers"),
-        default="",
-        help_text=_("The request headers."),
-    )
     res_headers = models.TextField(
-        verbose_name=_("Response headers"),
-        default="",
-        help_text=_("The response headers."),
-    )
-    req_body = models.BinaryField(
-        verbose_name=_("Request body"),
-        default=b"",
-        help_text=_("The request body."),
+        verbose_name=_("Response headers"), help_text=_("The response headers.")
     )
     res_body = models.BinaryField(
-        verbose_name=_("Response body"),
-        default=b"",
-        help_text=_("The response body."),
-    )
-    req_body_encoding = models.CharField(
-        max_length=24,
-        default="",
+        verbose_name=_("Response body"), default=b"", help_text=_("The response body.")
     )
     res_body_encoding = models.CharField(
+        _("Response encoding"),
         max_length=24,
-        default="",
+        blank=True,
+        help_text=_(
+            "The encoding is either extracted from the Content-Type header or, if "
+            "absent, taken from the default encoding configured for the content type. "
+            "If the decoded response content is not displaying correctly, you may try "
+            "changing the encoding value here."
+        ),
     )
     response_ms = models.PositiveIntegerField(
         verbose_name=_("Response in ms"),
         default=0,
         help_text=_("This is the response time in ms."),
     )
     timestamp = models.DateTimeField(
         verbose_name=_("Timestamp"),
         help_text=_("This is the date and time the API call was made."),
     )
     trace = models.TextField(
         verbose_name=_("Trace"),
-        default="",
         help_text=_("Text providing information in case of request failure."),
     )
 
     class Meta:
         verbose_name = _("Outgoing request log")
         verbose_name_plural = _("Outgoing request logs")
 
@@ -139,21 +144,25 @@
     @cached_property
     def request_body_decoded(self) -> str:
         """
         Decoded request body for use in template.
         """
         return self._decode_body(self.req_body, self.req_body_encoding)
 
+    request_body_decoded.short_description = _("Request body")  # type: ignore
+
     @cached_property
     def response_body_decoded(self) -> str:
         """
         Decoded response body for use in template.
         """
         return self._decode_body(self.res_body, self.res_body_encoding)
 
+    response_body_decoded.short_description = _("Response body")  # type: ignore
+
 
 def get_default_max_content_length():
     """
     Get default value for max content length from settings.
     """
     return settings.LOG_OUTGOING_REQUESTS_MAX_CONTENT_LENGTH
```

### Comparing `django-log-outgoing-requests-0.3.0/log_outgoing_requests/utils.py` & `django-log-outgoing-requests-0.4.0/log_outgoing_requests/utils.py`

 * *Files identical despite different names*

### Comparing `django-log-outgoing-requests-0.3.0/setup.cfg` & `django-log-outgoing-requests-0.4.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-log-outgoing-requests
-version = 0.3.0
+version = 0.4.0
 description = Log outgoing requests made by the requests python library
 long_description = file: README.rst
 url = https://github.com/maykinmedia/django-log-outgoing-requests
 project_urls = 
 	Documentation = http://django-log-outgoing-requests.readthedocs.io/en/latest/
 	Changelog = https://github.com/maykinmedia/django-log-outgoing-requests/blob/main/CHANGELOG.rst
 	Bug Tracker = https://github.com/maykinmedia/django-log-outgoing-requests/issues
```

### Comparing `django-log-outgoing-requests-0.3.0/tests/test_admin.py` & `django-log-outgoing-requests-0.4.0/tests/test_admin.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,16 +28,16 @@
     )
 
     response = admin_client.get(url)
     assert response.status_code == 200
 
     html = response.content.decode("utf-8")
     doc = PyQuery(html)
-    request_body = doc.find(".request-body-decoded").text()
-    response_body = doc.find(".response-body-decoded").text()
+    request_body = doc.find(".field-request_body .readonly").text()
+    response_body = doc.find(".field-response_body .readonly").text()
 
     assert request_body == "I'm a lumberjack and I'm okay."
     assert response_body == "I sleep all night and work all day."
 
 
 #
 # test override of settings
```

### Comparing `django-log-outgoing-requests-0.3.0/tests/test_formatter.py` & `django-log-outgoing-requests-0.4.0/tests/test_formatter.py`

 * *Files identical despite different names*

### Comparing `django-log-outgoing-requests-0.3.0/tests/test_logging.py` & `django-log-outgoing-requests-0.4.0/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `django-log-outgoing-requests-0.3.0/tests/test_utils.py` & `django-log-outgoing-requests-0.4.0/tests/test_utils.py`

 * *Files identical despite different names*

