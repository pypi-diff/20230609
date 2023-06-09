# Comparing `tmp/graphene_django_firebase_auth-0.0.21.tar.gz` & `tmp/graphene_django_firebase_auth-0.0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphene_django_firebase_auth-0.0.21.tar", last modified: Fri Jun  9 10:28:08 2023, max compression
+gzip compressed data, was "graphene_django_firebase_auth-0.0.22.tar", last modified: Fri Jun  9 10:30:13 2023, max compression
```

## Comparing `graphene_django_firebase_auth-0.0.21.tar` & `graphene_django_firebase_auth-0.0.22.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:28:08.559977 graphene_django_firebase_auth-0.0.21/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-09 10:27:56.000000 graphene_django_firebase_auth-0.0.21/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-09 10:27:56.000000 graphene_django_firebase_auth-0.0.21/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-06-09 10:28:08.559977 graphene_django_firebase_auth-0.0.21/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-06-09 10:27:56.000000 graphene_django_firebase_auth-0.0.21/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:28:08.559977 graphene_django_firebase_auth-0.0.21/firebase_auth/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-09 10:27:56.000000 graphene_django_firebase_auth-0.0.21/firebase_auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-09 10:27:56.000000 graphene_django_firebase_auth-0.0.21/firebase_auth/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-06-09 10:27:56.000000 graphene_django_firebase_auth-0.0.21/firebase_auth/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-09 10:27:56.000000 graphene_django_firebase_auth-0.0.21/firebase_auth/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-09 10:27:56.000000 graphene_django_firebase_auth-0.0.21/firebase_auth/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:28:08.559977 graphene_django_firebase_auth-0.0.21/graphene_django_firebase_auth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-06-09 10:28:08.000000 graphene_django_firebase_auth-0.0.21/graphene_django_firebase_auth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-09 10:28:08.000000 graphene_django_firebase_auth-0.0.21/graphene_django_firebase_auth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 10:28:08.000000 graphene_django_firebase_auth-0.0.21/graphene_django_firebase_auth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-09 10:28:08.000000 graphene_django_firebase_auth-0.0.21/graphene_django_firebase_auth.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-09 10:28:08.000000 graphene_django_firebase_auth-0.0.21/graphene_django_firebase_auth.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 10:28:08.559977 graphene_django_firebase_auth-0.0.21/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-09 10:27:56.000000 graphene_django_firebase_auth-0.0.21/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:30:13.142427 graphene_django_firebase_auth-0.0.22/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-09 10:30:03.000000 graphene_django_firebase_auth-0.0.22/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-09 10:30:03.000000 graphene_django_firebase_auth-0.0.22/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-06-09 10:30:13.142427 graphene_django_firebase_auth-0.0.22/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-06-09 10:30:03.000000 graphene_django_firebase_auth-0.0.22/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:30:13.142427 graphene_django_firebase_auth-0.0.22/firebase_auth/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-09 10:30:03.000000 graphene_django_firebase_auth-0.0.22/firebase_auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-09 10:30:03.000000 graphene_django_firebase_auth-0.0.22/firebase_auth/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-06-09 10:30:03.000000 graphene_django_firebase_auth-0.0.22/firebase_auth/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-09 10:30:03.000000 graphene_django_firebase_auth-0.0.22/firebase_auth/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-09 10:30:03.000000 graphene_django_firebase_auth-0.0.22/firebase_auth/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:30:13.142427 graphene_django_firebase_auth-0.0.22/graphene_django_firebase_auth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-06-09 10:30:13.000000 graphene_django_firebase_auth-0.0.22/graphene_django_firebase_auth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-09 10:30:13.000000 graphene_django_firebase_auth-0.0.22/graphene_django_firebase_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 10:30:13.000000 graphene_django_firebase_auth-0.0.22/graphene_django_firebase_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-09 10:30:13.000000 graphene_django_firebase_auth-0.0.22/graphene_django_firebase_auth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-09 10:30:13.000000 graphene_django_firebase_auth-0.0.22/graphene_django_firebase_auth.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 10:30:13.142427 graphene_django_firebase_auth-0.0.22/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-09 10:30:03.000000 graphene_django_firebase_auth-0.0.22/setup.py
```

### Comparing `graphene_django_firebase_auth-0.0.21/LICENSE` & `graphene_django_firebase_auth-0.0.22/LICENSE`

 * *Files identical despite different names*

### Comparing `graphene_django_firebase_auth-0.0.21/PKG-INFO` & `graphene_django_firebase_auth-0.0.22/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphene_django_firebase_auth
-Version: 0.0.21
+Version: 0.0.22
 Summary: Authentication provider for graphene-django and Google Firebase's Authentication service.
 Home-page: https://github.com/dspacejs/graphene-django-firebase-auth
 Author: Daniel Spajic
 Author-email: daniel@danieljs.tech
 License: MIT
 Keywords: graphene django firebase auth
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `graphene_django_firebase_auth-0.0.21/README.md` & `graphene_django_firebase_auth-0.0.22/README.md`

 * *Files identical despite different names*

### Comparing `graphene_django_firebase_auth-0.0.21/firebase_auth/authentication.py` & `graphene_django_firebase_auth-0.0.22/firebase_auth/authentication.py`

 * *Files identical despite different names*

### Comparing `graphene_django_firebase_auth-0.0.21/firebase_auth/forms.py` & `graphene_django_firebase_auth-0.0.22/firebase_auth/forms.py`

 * *Files identical despite different names*

### Comparing `graphene_django_firebase_auth-0.0.21/graphene_django_firebase_auth.egg-info/PKG-INFO` & `graphene_django_firebase_auth-0.0.22/graphene_django_firebase_auth.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphene-django-firebase-auth
-Version: 0.0.21
+Version: 0.0.22
 Summary: Authentication provider for graphene-django and Google Firebase's Authentication service.
 Home-page: https://github.com/dspacejs/graphene-django-firebase-auth
 Author: Daniel Spajic
 Author-email: daniel@danieljs.tech
 License: MIT
 Keywords: graphene django firebase auth
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `graphene_django_firebase_auth-0.0.21/setup.py` & `graphene_django_firebase_auth-0.0.22/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 from setuptools import setup
 
 
 README = open(os.path.join(os.path.dirname(__file__), 'README.md')).read()
-VERSION = '0.0.21'
+VERSION = '0.0.22'
 
 setup(
     name='graphene_django_firebase_auth',
     version=VERSION,
     author='Daniel Spajic',
     author_email='daniel@danieljs.tech',
     description=(
```

