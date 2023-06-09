# Comparing `tmp/ol-openedx-logging-0.0.1.tar.gz` & `tmp/ol-openedx-logging-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ol-openedx-logging-0.0.1.tar", last modified: Fri Jun  9 17:13:39 2023, max compression
+gzip compressed data, was "dist/ol-openedx-logging-0.1.0.tar", last modified: Fri Sep 10 14:52:35 2021, max compression
```

## Comparing `ol-openedx-logging-0.0.1.tar` & `ol-openedx-logging-0.1.0.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxr-xr-x   0 michaeldavidson   (501) staff       (20)        0 2023-06-09 17:13:39.573313 ol-openedx-logging-0.0.1/
--rw-r--r--   0 michaeldavidson   (501) staff       (20)       12 2023-06-09 17:13:38.000000 ol-openedx-logging-0.0.1/MANIFEST.in
--rw-r--r--   0 michaeldavidson   (501) staff       (20)      211 2023-06-09 17:13:39.573180 ol-openedx-logging-0.0.1/PKG-INFO
--rw-r--r--   0 michaeldavidson   (501) staff       (20)        0 2023-06-09 17:13:38.000000 ol-openedx-logging-0.0.1/__init__.py
--rw-r--r--   0 michaeldavidson   (501) staff       (20)      625 2023-06-09 17:13:38.000000 ol-openedx-logging-0.0.1/backend_shim.py
-drwxr-xr-x   0 michaeldavidson   (501) staff       (20)        0 2023-06-09 17:13:39.571878 ol-openedx-logging-0.0.1/ol_openedx_logging/
--rw-r--r--   0 michaeldavidson   (501) staff       (20)        0 2023-06-09 17:13:38.000000 ol-openedx-logging-0.0.1/ol_openedx_logging/__init__.py
--rw-r--r--   0 michaeldavidson   (501) staff       (20)      604 2023-06-09 17:13:38.000000 ol-openedx-logging-0.0.1/ol_openedx_logging/app.py
-drwxr-xr-x   0 michaeldavidson   (501) staff       (20)        0 2023-06-09 17:13:39.573011 ol-openedx-logging-0.0.1/ol_openedx_logging/settings/
--rw-r--r--   0 michaeldavidson   (501) staff       (20)        0 2023-06-09 17:13:38.000000 ol-openedx-logging-0.0.1/ol_openedx_logging/settings/__init__.py
--rw-r--r--   0 michaeldavidson   (501) staff       (20)     3037 2023-06-09 17:13:38.000000 ol-openedx-logging-0.0.1/ol_openedx_logging/settings/production.py
-drwxr-xr-x   0 michaeldavidson   (501) staff       (20)        0 2023-06-09 17:13:39.572778 ol-openedx-logging-0.0.1/ol_openedx_logging.egg-info/
--rw-r--r--   0 michaeldavidson   (501) staff       (20)      211 2023-06-09 17:13:39.000000 ol-openedx-logging-0.0.1/ol_openedx_logging.egg-info/PKG-INFO
--rw-r--r--   0 michaeldavidson   (501) staff       (20)      492 2023-06-09 17:13:39.000000 ol-openedx-logging-0.0.1/ol_openedx_logging.egg-info/SOURCES.txt
--rw-r--r--   0 michaeldavidson   (501) staff       (20)        1 2023-06-09 17:13:39.000000 ol-openedx-logging-0.0.1/ol_openedx_logging.egg-info/dependency_links.txt
--rw-r--r--   0 michaeldavidson   (501) staff       (20)      149 2023-06-09 17:13:39.000000 ol-openedx-logging-0.0.1/ol_openedx_logging.egg-info/entry_points.txt
--rw-r--r--   0 michaeldavidson   (501) staff       (20)        1 2023-06-09 17:13:39.000000 ol-openedx-logging-0.0.1/ol_openedx_logging.egg-info/namespace_packages.txt
--rw-r--r--   0 michaeldavidson   (501) staff       (20)       44 2023-06-09 17:13:39.000000 ol-openedx-logging-0.0.1/ol_openedx_logging.egg-info/requires.txt
--rw-r--r--   0 michaeldavidson   (501) staff       (20)       20 2023-06-09 17:13:39.000000 ol-openedx-logging-0.0.1/ol_openedx_logging.egg-info/top_level.txt
--rw-r--r--   0 michaeldavidson   (501) staff       (20)       38 2023-06-09 17:13:39.573355 ol-openedx-logging-0.0.1/setup.cfg
--rw-r--r--   0 michaeldavidson   (501) staff       (20)      902 2023-06-09 17:13:38.000000 ol-openedx-logging-0.0.1/setup.py
+drwxr-xr-x   0 tmacey    (1000) tmacey    (1000)        0 2021-09-10 14:52:35.340026 ol-openedx-logging-0.1.0/
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)       12 2021-09-10 14:52:35.000000 ol-openedx-logging-0.1.0/MANIFEST.in
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)      241 2021-09-10 14:52:35.340026 ol-openedx-logging-0.1.0/PKG-INFO
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)       38 2021-09-10 14:52:35.340026 ol-openedx-logging-0.1.0/setup.cfg
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)      874 2021-09-10 14:52:35.000000 ol-openedx-logging-0.1.0/setup.py
+drwxr-xr-x   0 tmacey    (1000) tmacey    (1000)        0 2021-09-10 14:52:35.336693 ol-openedx-logging-0.1.0/src/
+drwxr-xr-x   0 tmacey    (1000) tmacey    (1000)        0 2021-09-10 14:52:35.336693 ol-openedx-logging-0.1.0/src/ol_openedx_logging/
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)        0 2021-09-10 14:52:35.000000 ol-openedx-logging-0.1.0/src/ol_openedx_logging/__init__.py
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)      604 2021-09-10 14:52:35.000000 ol-openedx-logging-0.1.0/src/ol_openedx_logging/app.py
+drwxr-xr-x   0 tmacey    (1000) tmacey    (1000)        0 2021-09-10 14:52:35.340026 ol-openedx-logging-0.1.0/src/ol_openedx_logging/settings/
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)        0 2021-09-10 14:52:35.000000 ol-openedx-logging-0.1.0/src/ol_openedx_logging/settings/__init__.py
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)     1417 2021-09-10 14:52:35.000000 ol-openedx-logging-0.1.0/src/ol_openedx_logging/settings/production.py
+drwxr-xr-x   0 tmacey    (1000) tmacey    (1000)        0 2021-09-10 14:52:35.336693 ol-openedx-logging-0.1.0/src/ol_openedx_logging.egg-info/
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)      241 2021-09-10 14:52:35.000000 ol-openedx-logging-0.1.0/src/ol_openedx_logging.egg-info/PKG-INFO
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)      508 2021-09-10 14:52:35.000000 ol-openedx-logging-0.1.0/src/ol_openedx_logging.egg-info/SOURCES.txt
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)        1 2021-09-10 14:52:35.000000 ol-openedx-logging-0.1.0/src/ol_openedx_logging.egg-info/dependency_links.txt
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)      150 2021-09-10 14:52:35.000000 ol-openedx-logging-0.1.0/src/ol_openedx_logging.egg-info/entry_points.txt
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)        1 2021-09-10 14:52:35.000000 ol-openedx-logging-0.1.0/src/ol_openedx_logging.egg-info/namespace_packages.txt
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)       44 2021-09-10 14:52:35.000000 ol-openedx-logging-0.1.0/src/ol_openedx_logging.egg-info/requires.txt
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)       19 2021-09-10 14:52:35.000000 ol-openedx-logging-0.1.0/src/ol_openedx_logging.egg-info/top_level.txt
```

### Comparing `ol-openedx-logging-0.0.1/ol_openedx_logging/app.py` & `ol-openedx-logging-0.1.0/src/ol_openedx_logging/app.py`

 * *Files identical despite different names*

### Comparing `ol-openedx-logging-0.0.1/setup.py` & `ol-openedx-logging-0.1.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,25 +10,25 @@
         'lms.djangoapp': [
             'ol_openedx_logging = ol_openedx_logging.app:EdxLoggingLMS',
         ],
         'cms.djangoapp': [
             'ol_openedx_logging = ol_openedx_logging.app:EdxLoggingCMS',
         ],
     },
-    'install_requires': (
-        'Django>2.0',
-        'python-json-logger<3.0.0,>=2.0.2',
-    ),
-    'license': 'BSD-3-Clause',
     'name': 'ol-openedx-logging',
-    'namespace_packages': (
-    ),
-    'package_data': {
+    'version': '0.1.0',
+    'package_dir': {
+        '': 'src',
     },
     'packages': (
-        '',
         'ol_openedx_logging',
         'ol_openedx_logging.settings',
     ),
-    'python_requires': '>=3.8',
-    'version': '0.0.1',
+    'namespace_packages': (
+    ),
+    'package_data': {
+    },
+    'install_requires': (
+        'Django>2.0',
+        'python-json-logger<3.0.0,>=2.0.2',
+    ),
 })
```

