# Comparing `tmp/django-graphene-firebase-auth-0.0.7.tar.gz` & `tmp/django-graphene-firebase-auth-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-graphene-firebase-auth-0.0.7.tar", last modified: Mon Mar 14 16:28:29 2022, max compression
+gzip compressed data, was "dist/django-graphene-firebase-auth-0.0.8.tar", last modified: Tue Mar 15 11:05:30 2022, max compression
```

## Comparing `django-graphene-firebase-auth-0.0.7.tar` & `django-graphene-firebase-auth-0.0.8.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 eba       (1000) eba       (1000)        0 2022-03-14 16:28:29.000000 django-graphene-firebase-auth-0.0.7/
--rw-rw-r--   0 eba       (1000) eba       (1000)       34 2022-03-13 08:16:48.000000 django-graphene-firebase-auth-0.0.7/MANIFEST.in
--rw-rw-r--   0 eba       (1000) eba       (1000)     2569 2022-03-13 08:16:48.000000 django-graphene-firebase-auth-0.0.7/README.md
--rw-rw-r--   0 eba       (1000) eba       (1000)     1116 2022-03-14 16:28:27.000000 django-graphene-firebase-auth-0.0.7/setup.py
-drwxrwxr-x   0 eba       (1000) eba       (1000)        0 2022-03-14 16:28:29.000000 django-graphene-firebase-auth-0.0.7/firebase_auth/
--rw-rw-r--   0 eba       (1000) eba       (1000)      162 2022-03-13 08:16:48.000000 django-graphene-firebase-auth-0.0.7/firebase_auth/models.py
--rw-rw-r--   0 eba       (1000) eba       (1000)       37 2022-03-14 14:48:09.000000 django-graphene-firebase-auth-0.0.7/firebase_auth/auth.py
--rw-rw-r--   0 eba       (1000) eba       (1000)      846 2022-03-13 08:16:48.000000 django-graphene-firebase-auth-0.0.7/firebase_auth/forms.py
--rw-rw-r--   0 eba       (1000) eba       (1000)      418 2022-03-13 08:16:48.000000 django-graphene-firebase-auth-0.0.7/firebase_auth/apps.py
--rw-rw-r--   0 eba       (1000) eba       (1000)       61 2022-03-13 08:16:48.000000 django-graphene-firebase-auth-0.0.7/firebase_auth/__init__.py
--rw-rw-r--   0 eba       (1000) eba       (1000)     2057 2022-03-14 16:28:27.000000 django-graphene-firebase-auth-0.0.7/firebase_auth/authentication.py
-drwxrwxr-x   0 eba       (1000) eba       (1000)        0 2022-03-14 16:28:29.000000 django-graphene-firebase-auth-0.0.7/main/
--rw-rw-r--   0 eba       (1000) eba       (1000)      176 2022-03-13 08:16:48.000000 django-graphene-firebase-auth-0.0.7/main/wsgi.py
--rw-rw-r--   0 eba       (1000) eba       (1000)        0 2022-03-13 08:16:48.000000 django-graphene-firebase-auth-0.0.7/main/__init__.py
--rw-rw-r--   0 eba       (1000) eba       (1000)      170 2022-03-13 08:16:48.000000 django-graphene-firebase-auth-0.0.7/main/urls.py
--rw-rw-r--   0 eba       (1000) eba       (1000)     2966 2022-03-13 08:16:48.000000 django-graphene-firebase-auth-0.0.7/main/settings.py
--rw-rw-r--   0 eba       (1000) eba       (1000)       38 2022-03-14 16:28:29.000000 django-graphene-firebase-auth-0.0.7/setup.cfg
--rw-rw-r--   0 eba       (1000) eba       (1000)     1070 2022-03-13 08:16:48.000000 django-graphene-firebase-auth-0.0.7/LICENSE
-drwxrwxr-x   0 eba       (1000) eba       (1000)        0 2022-03-14 16:28:29.000000 django-graphene-firebase-auth-0.0.7/django_graphene_firebase_auth.egg-info/
--rw-rw-r--   0 eba       (1000) eba       (1000)       22 2022-03-14 16:28:29.000000 django-graphene-firebase-auth-0.0.7/django_graphene_firebase_auth.egg-info/requires.txt
--rw-rw-r--   0 eba       (1000) eba       (1000)       33 2022-03-14 16:28:29.000000 django-graphene-firebase-auth-0.0.7/django_graphene_firebase_auth.egg-info/top_level.txt
--rw-rw-r--   0 eba       (1000) eba       (1000)      723 2022-03-14 16:28:29.000000 django-graphene-firebase-auth-0.0.7/django_graphene_firebase_auth.egg-info/SOURCES.txt
--rw-rw-r--   0 eba       (1000) eba       (1000)        1 2022-03-14 16:28:29.000000 django-graphene-firebase-auth-0.0.7/django_graphene_firebase_auth.egg-info/dependency_links.txt
--rw-rw-r--   0 eba       (1000) eba       (1000)     4113 2022-03-14 16:28:29.000000 django-graphene-firebase-auth-0.0.7/django_graphene_firebase_auth.egg-info/PKG-INFO
--rw-rw-r--   0 eba       (1000) eba       (1000)     4113 2022-03-14 16:28:29.000000 django-graphene-firebase-auth-0.0.7/PKG-INFO
-drwxrwxr-x   0 eba       (1000) eba       (1000)        0 2022-03-14 16:28:29.000000 django-graphene-firebase-auth-0.0.7/package_tests/
--rw-rw-r--   0 eba       (1000) eba       (1000)      393 2022-03-13 08:16:48.000000 django-graphene-firebase-auth-0.0.7/package_tests/models.py
-drwxrwxr-x   0 eba       (1000) eba       (1000)        0 2022-03-14 16:28:29.000000 django-graphene-firebase-auth-0.0.7/package_tests/tests/
--rw-rw-r--   0 eba       (1000) eba       (1000)      965 2022-03-13 08:16:48.000000 django-graphene-firebase-auth-0.0.7/package_tests/tests/test_forms.py
--rw-rw-r--   0 eba       (1000) eba       (1000)     1548 2022-03-13 08:16:48.000000 django-graphene-firebase-auth-0.0.7/package_tests/tests/helpers.py
--rw-rw-r--   0 eba       (1000) eba       (1000)     5475 2022-03-13 08:16:48.000000 django-graphene-firebase-auth-0.0.7/package_tests/tests/test_authentication.py
--rw-rw-r--   0 eba       (1000) eba       (1000)        0 2022-03-13 08:16:48.000000 django-graphene-firebase-auth-0.0.7/package_tests/tests/__init__.py
--rw-rw-r--   0 eba       (1000) eba       (1000)      100 2022-03-13 08:16:48.000000 django-graphene-firebase-auth-0.0.7/package_tests/apps.py
--rw-rw-r--   0 eba       (1000) eba       (1000)        0 2022-03-13 08:16:48.000000 django-graphene-firebase-auth-0.0.7/package_tests/__init__.py
+drwxrwxr-x   0 eba       (1000) eba       (1000)        0 2022-03-15 11:05:30.000000 django-graphene-firebase-auth-0.0.8/
+-rw-rw-r--   0 eba       (1000) eba       (1000)       34 2022-03-13 08:16:48.000000 django-graphene-firebase-auth-0.0.8/MANIFEST.in
+-rw-rw-r--   0 eba       (1000) eba       (1000)     2569 2022-03-13 08:16:48.000000 django-graphene-firebase-auth-0.0.8/README.md
+-rw-rw-r--   0 eba       (1000) eba       (1000)     1116 2022-03-15 11:05:10.000000 django-graphene-firebase-auth-0.0.8/setup.py
+drwxrwxr-x   0 eba       (1000) eba       (1000)        0 2022-03-15 11:05:30.000000 django-graphene-firebase-auth-0.0.8/firebase_auth/
+-rw-rw-r--   0 eba       (1000) eba       (1000)      162 2022-03-13 08:16:48.000000 django-graphene-firebase-auth-0.0.8/firebase_auth/models.py
+-rw-rw-r--   0 eba       (1000) eba       (1000)       37 2022-03-14 14:48:09.000000 django-graphene-firebase-auth-0.0.8/firebase_auth/auth.py
+-rw-rw-r--   0 eba       (1000) eba       (1000)      846 2022-03-13 08:16:48.000000 django-graphene-firebase-auth-0.0.8/firebase_auth/forms.py
+-rw-rw-r--   0 eba       (1000) eba       (1000)      418 2022-03-13 08:16:48.000000 django-graphene-firebase-auth-0.0.8/firebase_auth/apps.py
+-rw-rw-r--   0 eba       (1000) eba       (1000)       61 2022-03-13 08:16:48.000000 django-graphene-firebase-auth-0.0.8/firebase_auth/__init__.py
+-rw-rw-r--   0 eba       (1000) eba       (1000)     2048 2022-03-15 11:05:10.000000 django-graphene-firebase-auth-0.0.8/firebase_auth/authentication.py
+drwxrwxr-x   0 eba       (1000) eba       (1000)        0 2022-03-15 11:05:30.000000 django-graphene-firebase-auth-0.0.8/main/
+-rw-rw-r--   0 eba       (1000) eba       (1000)      176 2022-03-13 08:16:48.000000 django-graphene-firebase-auth-0.0.8/main/wsgi.py
+-rw-rw-r--   0 eba       (1000) eba       (1000)        0 2022-03-13 08:16:48.000000 django-graphene-firebase-auth-0.0.8/main/__init__.py
+-rw-rw-r--   0 eba       (1000) eba       (1000)      170 2022-03-13 08:16:48.000000 django-graphene-firebase-auth-0.0.8/main/urls.py
+-rw-rw-r--   0 eba       (1000) eba       (1000)     2966 2022-03-13 08:16:48.000000 django-graphene-firebase-auth-0.0.8/main/settings.py
+-rw-rw-r--   0 eba       (1000) eba       (1000)       38 2022-03-15 11:05:30.000000 django-graphene-firebase-auth-0.0.8/setup.cfg
+-rw-rw-r--   0 eba       (1000) eba       (1000)     1070 2022-03-13 08:16:48.000000 django-graphene-firebase-auth-0.0.8/LICENSE
+drwxrwxr-x   0 eba       (1000) eba       (1000)        0 2022-03-15 11:05:30.000000 django-graphene-firebase-auth-0.0.8/django_graphene_firebase_auth.egg-info/
+-rw-rw-r--   0 eba       (1000) eba       (1000)       22 2022-03-15 11:05:30.000000 django-graphene-firebase-auth-0.0.8/django_graphene_firebase_auth.egg-info/requires.txt
+-rw-rw-r--   0 eba       (1000) eba       (1000)       33 2022-03-15 11:05:30.000000 django-graphene-firebase-auth-0.0.8/django_graphene_firebase_auth.egg-info/top_level.txt
+-rw-rw-r--   0 eba       (1000) eba       (1000)      723 2022-03-15 11:05:30.000000 django-graphene-firebase-auth-0.0.8/django_graphene_firebase_auth.egg-info/SOURCES.txt
+-rw-rw-r--   0 eba       (1000) eba       (1000)        1 2022-03-15 11:05:30.000000 django-graphene-firebase-auth-0.0.8/django_graphene_firebase_auth.egg-info/dependency_links.txt
+-rw-rw-r--   0 eba       (1000) eba       (1000)     4113 2022-03-15 11:05:30.000000 django-graphene-firebase-auth-0.0.8/django_graphene_firebase_auth.egg-info/PKG-INFO
+-rw-rw-r--   0 eba       (1000) eba       (1000)     4113 2022-03-15 11:05:30.000000 django-graphene-firebase-auth-0.0.8/PKG-INFO
+drwxrwxr-x   0 eba       (1000) eba       (1000)        0 2022-03-15 11:05:30.000000 django-graphene-firebase-auth-0.0.8/package_tests/
+-rw-rw-r--   0 eba       (1000) eba       (1000)      393 2022-03-13 08:16:48.000000 django-graphene-firebase-auth-0.0.8/package_tests/models.py
+drwxrwxr-x   0 eba       (1000) eba       (1000)        0 2022-03-15 11:05:30.000000 django-graphene-firebase-auth-0.0.8/package_tests/tests/
+-rw-rw-r--   0 eba       (1000) eba       (1000)      965 2022-03-13 08:16:48.000000 django-graphene-firebase-auth-0.0.8/package_tests/tests/test_forms.py
+-rw-rw-r--   0 eba       (1000) eba       (1000)     1548 2022-03-13 08:16:48.000000 django-graphene-firebase-auth-0.0.8/package_tests/tests/helpers.py
+-rw-rw-r--   0 eba       (1000) eba       (1000)     5475 2022-03-13 08:16:48.000000 django-graphene-firebase-auth-0.0.8/package_tests/tests/test_authentication.py
+-rw-rw-r--   0 eba       (1000) eba       (1000)        0 2022-03-13 08:16:48.000000 django-graphene-firebase-auth-0.0.8/package_tests/tests/__init__.py
+-rw-rw-r--   0 eba       (1000) eba       (1000)      100 2022-03-13 08:16:48.000000 django-graphene-firebase-auth-0.0.8/package_tests/apps.py
+-rw-rw-r--   0 eba       (1000) eba       (1000)        0 2022-03-13 08:16:48.000000 django-graphene-firebase-auth-0.0.8/package_tests/__init__.py
```

### Comparing `django-graphene-firebase-auth-0.0.7/README.md` & `django-graphene-firebase-auth-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `django-graphene-firebase-auth-0.0.7/setup.py` & `django-graphene-firebase-auth-0.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.7'
+VERSION = '0.0.8'
 DESCRIPTION = 'Firebase authentication with django graphene'
 LONG_DESCRIPTION = 'A firebase authentication with django graphene.'
 
 # Setting up
 setup(
     name="django-graphene-firebase-auth",
     version=VERSION,
```

### Comparing `django-graphene-firebase-auth-0.0.7/firebase_auth/forms.py` & `django-graphene-firebase-auth-0.0.8/firebase_auth/forms.py`

 * *Files identical despite different names*

### Comparing `django-graphene-firebase-auth-0.0.7/firebase_auth/authentication.py` & `django-graphene-firebase-auth-0.0.8/firebase_auth/authentication.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,16 +15,16 @@
         encoded_token = request.META.get('HTTP_AUTHORIZATION').replace('jwt ', '')
         decoded_token = None
 
         try:
             decoded_token = auth.verify_id_token(encoded_token, firebase_app, True)
         except ValueError:
             pass
-        # except auth.AuthError:
-        #     pass
+        except Exception:
+            pass
         return decoded_token
 
     def _register_unregistered_user(self, firebase_uid):
         user = None
         form = UserRegistrationForm(data={
             'firebase_uid': firebase_uid,
         })
```

### Comparing `django-graphene-firebase-auth-0.0.7/main/settings.py` & `django-graphene-firebase-auth-0.0.8/main/settings.py`

 * *Files identical despite different names*

### Comparing `django-graphene-firebase-auth-0.0.7/LICENSE` & `django-graphene-firebase-auth-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `django-graphene-firebase-auth-0.0.7/django_graphene_firebase_auth.egg-info/SOURCES.txt` & `django-graphene-firebase-auth-0.0.8/django_graphene_firebase_auth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-graphene-firebase-auth-0.0.7/django_graphene_firebase_auth.egg-info/PKG-INFO` & `django-graphene-firebase-auth-0.0.8/django_graphene_firebase_auth.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-graphene-firebase-auth
-Version: 0.0.7
+Version: 0.0.8
 Summary: Firebase authentication with django graphene
 Home-page: UNKNOWN
 Author: Eba Alemayehu
 Author-email: <ebaalemayhu3@gmail.com>
 License: UNKNOWN
 Description: 
         # graphene-django-firebase-auth
```

### Comparing `django-graphene-firebase-auth-0.0.7/PKG-INFO` & `django-graphene-firebase-auth-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-graphene-firebase-auth
-Version: 0.0.7
+Version: 0.0.8
 Summary: Firebase authentication with django graphene
 Home-page: UNKNOWN
 Author: Eba Alemayehu
 Author-email: <ebaalemayhu3@gmail.com>
 License: UNKNOWN
 Description: 
         # graphene-django-firebase-auth
```

### Comparing `django-graphene-firebase-auth-0.0.7/package_tests/tests/test_forms.py` & `django-graphene-firebase-auth-0.0.8/package_tests/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `django-graphene-firebase-auth-0.0.7/package_tests/tests/helpers.py` & `django-graphene-firebase-auth-0.0.8/package_tests/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `django-graphene-firebase-auth-0.0.7/package_tests/tests/test_authentication.py` & `django-graphene-firebase-auth-0.0.8/package_tests/tests/test_authentication.py`

 * *Files identical despite different names*

