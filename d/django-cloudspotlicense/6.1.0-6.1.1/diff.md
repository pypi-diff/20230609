# Comparing `tmp/django-cloudspotlicense-6.1.0.tar.gz` & `tmp/django-cloudspotlicense-6.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\django-cloudspotlicense-6.1.0.tar", last modified: Fri Jun  9 09:21:37 2023, max compression
+gzip compressed data, was "dist\django-cloudspotlicense-6.1.1.tar", last modified: Fri Jun  9 09:41:13 2023, max compression
```

## Comparing `django-cloudspotlicense-6.1.0.tar` & `django-cloudspotlicense-6.1.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 09:21:37.000000 django-cloudspotlicense-6.1.0/
-drwxrwxrwx   0        0        0        0 2023-06-09 09:21:37.000000 django-cloudspotlicense-6.1.0/django_cloudspotlicense/
--rw-rw-rw-   0        0        0       66 2022-10-05 08:35:57.000000 django-cloudspotlicense-6.1.0/django_cloudspotlicense/admin.py
--rw-rw-rw-   0        0        0      183 2022-10-05 10:03:35.000000 django-cloudspotlicense-6.1.0/django_cloudspotlicense/apps.py
--rw-rw-rw-   0        0        0      244 2023-06-07 15:51:33.000000 django-cloudspotlicense-6.1.0/django_cloudspotlicense/config.py
--rw-rw-rw-   0        0        0      246 2022-10-19 14:26:18.000000 django-cloudspotlicense-6.1.0/django_cloudspotlicense/context_processors.py
--rw-rw-rw-   0        0        0      905 2022-10-05 12:22:39.000000 django-cloudspotlicense-6.1.0/django_cloudspotlicense/helpers.py
-drwxrwxrwx   0        0        0        0 2023-06-09 09:21:37.000000 django-cloudspotlicense-6.1.0/django_cloudspotlicense/migrations/
--rw-rw-rw-   0        0        0     3881 2022-10-05 11:36:48.000000 django-cloudspotlicense-6.1.0/django_cloudspotlicense/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      452 2022-10-17 09:58:41.000000 django-cloudspotlicense-6.1.0/django_cloudspotlicense/migrations/0002_cloudspotcompany_users.py
--rw-rw-rw-   0        0        0      505 2022-10-17 09:59:00.000000 django-cloudspotlicense-6.1.0/django_cloudspotlicense/migrations/0003_alter_cloudspotcompany_users.py
--rw-rw-rw-   0        0        0        0 2022-10-05 08:35:57.000000 django-cloudspotlicense-6.1.0/django_cloudspotlicense/migrations/__init__.py
--rw-rw-rw-   0        0        0     2987 2023-06-07 15:51:33.000000 django-cloudspotlicense-6.1.0/django_cloudspotlicense/mixins.py
--rw-rw-rw-   0        0        0     1515 2023-05-12 07:05:12.000000 django-cloudspotlicense-6.1.0/django_cloudspotlicense/models.py
-drwxrwxrwx   0        0        0        0 2023-06-09 09:21:36.000000 django-cloudspotlicense-6.1.0/django_cloudspotlicense/templates/
-drwxrwxrwx   0        0        0        0 2023-06-09 09:21:37.000000 django-cloudspotlicense-6.1.0/django_cloudspotlicense/templates/auth/
--rw-rw-rw-   0        0        0      634 2022-10-05 10:05:52.000000 django-cloudspotlicense-6.1.0/django_cloudspotlicense/templates/auth/login.html
--rw-rw-rw-   0        0        0      496 2022-10-17 09:51:34.000000 django-cloudspotlicense-6.1.0/django_cloudspotlicense/templates/auth/select_company.html
-drwxrwxrwx   0        0        0        0 2023-06-09 09:21:37.000000 django-cloudspotlicense-6.1.0/django_cloudspotlicense/templatetags/
--rw-rw-rw-   0        0        0      377 2023-03-13 08:55:48.000000 django-cloudspotlicense-6.1.0/django_cloudspotlicense/templatetags/license_tags.py
--rw-rw-rw-   0        0        0        0 2022-12-09 12:36:09.000000 django-cloudspotlicense-6.1.0/django_cloudspotlicense/templatetags/__init__.py
--rw-rw-rw-   0        0        0       63 2022-10-05 08:35:57.000000 django-cloudspotlicense-6.1.0/django_cloudspotlicense/tests.py
--rw-rw-rw-   0        0        0     1019 2023-03-08 12:37:58.000000 django-cloudspotlicense-6.1.0/django_cloudspotlicense/urls.py
--rw-rw-rw-   0        0        0      401 2023-06-07 15:51:33.000000 django-cloudspotlicense-6.1.0/django_cloudspotlicense/utils.py
--rw-rw-rw-   0        0        0    15952 2023-06-09 09:19:51.000000 django-cloudspotlicense-6.1.0/django_cloudspotlicense/views.py
--rw-rw-rw-   0        0        0       69 2023-06-09 09:19:51.000000 django-cloudspotlicense-6.1.0/django_cloudspotlicense/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 09:21:37.000000 django-cloudspotlicense-6.1.0/django_cloudspotlicense.egg-info/
--rw-rw-rw-   0        0        0        1 2023-06-09 09:21:36.000000 django-cloudspotlicense-6.1.0/django_cloudspotlicense.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0    10292 2023-06-09 09:21:36.000000 django-cloudspotlicense-6.1.0/django_cloudspotlicense.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       31 2023-06-09 09:21:36.000000 django-cloudspotlicense-6.1.0/django_cloudspotlicense.egg-info/requires.txt
--rw-rw-rw-   0        0        0     1148 2023-06-09 09:21:36.000000 django-cloudspotlicense-6.1.0/django_cloudspotlicense.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       24 2023-06-09 09:21:36.000000 django-cloudspotlicense-6.1.0/django_cloudspotlicense.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35821 2021-04-16 13:14:04.000000 django-cloudspotlicense-6.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0       93 2022-10-05 14:15:21.000000 django-cloudspotlicense-6.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0    10292 2023-06-09 09:21:37.000000 django-cloudspotlicense-6.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     9428 2023-06-09 09:19:51.000000 django-cloudspotlicense-6.1.0/README.md
--rw-rw-rw-   0        0        0       86 2023-06-09 09:21:37.000000 django-cloudspotlicense-6.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1401 2023-06-09 09:19:51.000000 django-cloudspotlicense-6.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 09:41:13.000000 django-cloudspotlicense-6.1.1/
+drwxrwxrwx   0        0        0        0 2023-06-09 09:41:13.000000 django-cloudspotlicense-6.1.1/django_cloudspotlicense/
+-rw-rw-rw-   0        0        0       66 2022-10-05 08:35:57.000000 django-cloudspotlicense-6.1.1/django_cloudspotlicense/admin.py
+-rw-rw-rw-   0        0        0      183 2022-10-05 10:03:35.000000 django-cloudspotlicense-6.1.1/django_cloudspotlicense/apps.py
+-rw-rw-rw-   0        0        0      244 2023-06-07 15:51:33.000000 django-cloudspotlicense-6.1.1/django_cloudspotlicense/config.py
+-rw-rw-rw-   0        0        0      246 2022-10-19 14:26:18.000000 django-cloudspotlicense-6.1.1/django_cloudspotlicense/context_processors.py
+-rw-rw-rw-   0        0        0      905 2022-10-05 12:22:39.000000 django-cloudspotlicense-6.1.1/django_cloudspotlicense/helpers.py
+drwxrwxrwx   0        0        0        0 2023-06-09 09:41:13.000000 django-cloudspotlicense-6.1.1/django_cloudspotlicense/migrations/
+-rw-rw-rw-   0        0        0     3881 2022-10-05 11:36:48.000000 django-cloudspotlicense-6.1.1/django_cloudspotlicense/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      452 2022-10-17 09:58:41.000000 django-cloudspotlicense-6.1.1/django_cloudspotlicense/migrations/0002_cloudspotcompany_users.py
+-rw-rw-rw-   0        0        0      505 2022-10-17 09:59:00.000000 django-cloudspotlicense-6.1.1/django_cloudspotlicense/migrations/0003_alter_cloudspotcompany_users.py
+-rw-rw-rw-   0        0        0        0 2022-10-05 08:35:57.000000 django-cloudspotlicense-6.1.1/django_cloudspotlicense/migrations/__init__.py
+-rw-rw-rw-   0        0        0     2987 2023-06-07 15:51:33.000000 django-cloudspotlicense-6.1.1/django_cloudspotlicense/mixins.py
+-rw-rw-rw-   0        0        0     1515 2023-05-12 07:05:12.000000 django-cloudspotlicense-6.1.1/django_cloudspotlicense/models.py
+drwxrwxrwx   0        0        0        0 2023-06-09 09:41:13.000000 django-cloudspotlicense-6.1.1/django_cloudspotlicense/templates/
+drwxrwxrwx   0        0        0        0 2023-06-09 09:41:13.000000 django-cloudspotlicense-6.1.1/django_cloudspotlicense/templates/auth/
+-rw-rw-rw-   0        0        0      634 2022-10-05 10:05:52.000000 django-cloudspotlicense-6.1.1/django_cloudspotlicense/templates/auth/login.html
+-rw-rw-rw-   0        0        0      496 2022-10-17 09:51:34.000000 django-cloudspotlicense-6.1.1/django_cloudspotlicense/templates/auth/select_company.html
+drwxrwxrwx   0        0        0        0 2023-06-09 09:41:13.000000 django-cloudspotlicense-6.1.1/django_cloudspotlicense/templatetags/
+-rw-rw-rw-   0        0        0      377 2023-03-13 08:55:48.000000 django-cloudspotlicense-6.1.1/django_cloudspotlicense/templatetags/license_tags.py
+-rw-rw-rw-   0        0        0        0 2022-12-09 12:36:09.000000 django-cloudspotlicense-6.1.1/django_cloudspotlicense/templatetags/__init__.py
+-rw-rw-rw-   0        0        0       63 2022-10-05 08:35:57.000000 django-cloudspotlicense-6.1.1/django_cloudspotlicense/tests.py
+-rw-rw-rw-   0        0        0     1019 2023-03-08 12:37:58.000000 django-cloudspotlicense-6.1.1/django_cloudspotlicense/urls.py
+-rw-rw-rw-   0        0        0      401 2023-06-07 15:51:33.000000 django-cloudspotlicense-6.1.1/django_cloudspotlicense/utils.py
+-rw-rw-rw-   0        0        0    16199 2023-06-09 09:39:27.000000 django-cloudspotlicense-6.1.1/django_cloudspotlicense/views.py
+-rw-rw-rw-   0        0        0       69 2023-06-09 09:39:27.000000 django-cloudspotlicense-6.1.1/django_cloudspotlicense/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 09:41:13.000000 django-cloudspotlicense-6.1.1/django_cloudspotlicense.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-06-09 09:41:13.000000 django-cloudspotlicense-6.1.1/django_cloudspotlicense.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0    10292 2023-06-09 09:41:13.000000 django-cloudspotlicense-6.1.1/django_cloudspotlicense.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       31 2023-06-09 09:41:13.000000 django-cloudspotlicense-6.1.1/django_cloudspotlicense.egg-info/requires.txt
+-rw-rw-rw-   0        0        0     1148 2023-06-09 09:41:13.000000 django-cloudspotlicense-6.1.1/django_cloudspotlicense.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       24 2023-06-09 09:41:13.000000 django-cloudspotlicense-6.1.1/django_cloudspotlicense.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35821 2021-04-16 13:14:04.000000 django-cloudspotlicense-6.1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0       93 2022-10-05 14:15:21.000000 django-cloudspotlicense-6.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    10292 2023-06-09 09:41:13.000000 django-cloudspotlicense-6.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     9428 2023-06-09 09:19:51.000000 django-cloudspotlicense-6.1.1/README.md
+-rw-rw-rw-   0        0        0       86 2023-06-09 09:41:13.000000 django-cloudspotlicense-6.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1401 2023-06-09 09:39:27.000000 django-cloudspotlicense-6.1.1/setup.py
```

### Comparing `django-cloudspotlicense-6.1.0/django_cloudspotlicense/helpers.py` & `django-cloudspotlicense-6.1.1/django_cloudspotlicense/helpers.py`

 * *Files identical despite different names*

### Comparing `django-cloudspotlicense-6.1.0/django_cloudspotlicense/migrations/0001_initial.py` & `django-cloudspotlicense-6.1.1/django_cloudspotlicense/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-cloudspotlicense-6.1.0/django_cloudspotlicense/mixins.py` & `django-cloudspotlicense-6.1.1/django_cloudspotlicense/mixins.py`

 * *Files identical despite different names*

### Comparing `django-cloudspotlicense-6.1.0/django_cloudspotlicense/models.py` & `django-cloudspotlicense-6.1.1/django_cloudspotlicense/models.py`

 * *Files identical despite different names*

### Comparing `django-cloudspotlicense-6.1.0/django_cloudspotlicense/templates/auth/login.html` & `django-cloudspotlicense-6.1.1/django_cloudspotlicense/templates/auth/login.html`

 * *Files identical despite different names*

### Comparing `django-cloudspotlicense-6.1.0/django_cloudspotlicense/urls.py` & `django-cloudspotlicense-6.1.1/django_cloudspotlicense/urls.py`

 * *Files identical despite different names*

### Comparing `django-cloudspotlicense-6.1.0/django_cloudspotlicense/views.py` & `django-cloudspotlicense-6.1.1/django_cloudspotlicense/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -316,20 +316,22 @@
             return JsonResponse({ 'status' : ResponseStatus.OBJECT_UPDATED })
         elif event == 'user.created':
             user_email = data['user_email']
             user_first_name = data['user_first_name']
             user_last_name = data['user_last_name']
             user_pin = data['user_pin']
             user_pwd = data['user_pwd'] # This will contain a dummy password, we don't need to know the actual password
+            license_token = data['license_token'] if data['license_token'] != '' else None # Initial token (generated by License server), we need this so other events are able to find the user
             
             # Check if the user already exists
             try:
                 user = UserModel.objects.get(username=user_email)
                 return JsonResponse({ 'status' : ResponseStatus.OBJECT_EXISTS, 'error' : { 'message' : 'User already exists.' }}, status=HTTPStatus.BAD_REQUEST)
             except UserModel.DoesNotExist:
                 user = UserModel.objects.create_user(username=user_email, email=user_email, password=user_pwd, **{
                     'first_name' : user_first_name,
                     'last_name' : user_last_name,
                     'pin' : user_pin,
+                    'license_token' : license_token
                 })
             
             return JsonResponse({ 'status' : ResponseStatus.OBJECT_CREATED, 'id' : user.id })
```

### Comparing `django-cloudspotlicense-6.1.0/django_cloudspotlicense.egg-info/PKG-INFO` & `django-cloudspotlicense-6.1.1/django_cloudspotlicense.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: django-cloudspotlicense
-Version: 6.1.0
+Version: 6.1.1
 Summary: Django package to integrate the authentication of the Cloudspot License Server in other django applications
 Home-page: https://github.com/Ecosy-EU/django-cloudspotlicense
 Author: Alexander Schillemans
 Author-email: alexander.schillemans@lhs.global
 License: GPL-3.0-or-later
-Download-URL: https://github.com/Ecosy-EU/django-cloudspotlicense/archive/refs/tags/6.1.0.tar.gz
+Download-URL: https://github.com/Ecosy-EU/django-cloudspotlicense/archive/refs/tags/6.1.1.tar.gz
 Keywords: cloudspot,django
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `django-cloudspotlicense-6.1.0/django_cloudspotlicense.egg-info/SOURCES.txt` & `django-cloudspotlicense-6.1.1/django_cloudspotlicense.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-cloudspotlicense-6.1.0/LICENSE.txt` & `django-cloudspotlicense-6.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-cloudspotlicense-6.1.0/PKG-INFO` & `django-cloudspotlicense-6.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: django-cloudspotlicense
-Version: 6.1.0
+Version: 6.1.1
 Summary: Django package to integrate the authentication of the Cloudspot License Server in other django applications
 Home-page: https://github.com/Ecosy-EU/django-cloudspotlicense
 Author: Alexander Schillemans
 Author-email: alexander.schillemans@lhs.global
 License: GPL-3.0-or-later
-Download-URL: https://github.com/Ecosy-EU/django-cloudspotlicense/archive/refs/tags/6.1.0.tar.gz
+Download-URL: https://github.com/Ecosy-EU/django-cloudspotlicense/archive/refs/tags/6.1.1.tar.gz
 Keywords: cloudspot,django
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `django-cloudspotlicense-6.1.0/README.md` & `django-cloudspotlicense-6.1.1/README.md`

 * *Files identical despite different names*

### Comparing `django-cloudspotlicense-6.1.0/setup.py` & `django-cloudspotlicense-6.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
   name = 'django-cloudspotlicense',         
   packages=['django_cloudspotlicense', 'django_cloudspotlicense.migrations', 'django_cloudspotlicense.templatetags'],
   include_package_data=True,
-  version = '6.1.0',
+  version = '6.1.1',
   license='GPL-3.0-or-later',
   description = 'Django package to integrate the authentication of the Cloudspot License Server in other django applications',
   long_description=long_description,
   long_description_content_type='text/markdown',
   author = 'Alexander Schillemans',
   author_email = 'alexander.schillemans@lhs.global',
   url = 'https://github.com/Ecosy-EU/django-cloudspotlicense',
-  download_url = 'https://github.com/Ecosy-EU/django-cloudspotlicense/archive/refs/tags/6.1.0.tar.gz',
+  download_url = 'https://github.com/Ecosy-EU/django-cloudspotlicense/archive/refs/tags/6.1.1.tar.gz',
   keywords = ['cloudspot', 'django'],
   install_requires=[
           'requests',
           'cloudspot-license-api',
       ],
   classifiers=[
     'Development Status :: 3 - Alpha',
```

