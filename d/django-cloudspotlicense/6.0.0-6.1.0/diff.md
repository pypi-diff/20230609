# Comparing `tmp/django-cloudspotlicense-6.0.0.tar.gz` & `tmp/django-cloudspotlicense-6.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\django-cloudspotlicense-6.0.0.tar", last modified: Wed Jun  7 15:38:05 2023, max compression
+gzip compressed data, was "dist\django-cloudspotlicense-6.1.0.tar", last modified: Fri Jun  9 09:21:37 2023, max compression
```

## Comparing `django-cloudspotlicense-6.0.0.tar` & `django-cloudspotlicense-6.1.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 15:38:05.000000 django-cloudspotlicense-6.0.0/
-drwxrwxrwx   0        0        0        0 2023-06-07 15:38:05.000000 django-cloudspotlicense-6.0.0/django_cloudspotlicense/
--rw-rw-rw-   0        0        0       66 2022-10-05 08:35:57.000000 django-cloudspotlicense-6.0.0/django_cloudspotlicense/admin.py
--rw-rw-rw-   0        0        0      183 2022-10-05 10:03:35.000000 django-cloudspotlicense-6.0.0/django_cloudspotlicense/apps.py
--rw-rw-rw-   0        0        0      244 2023-06-07 15:33:19.000000 django-cloudspotlicense-6.0.0/django_cloudspotlicense/config.py
--rw-rw-rw-   0        0        0      246 2022-10-19 14:26:18.000000 django-cloudspotlicense-6.0.0/django_cloudspotlicense/context_processors.py
--rw-rw-rw-   0        0        0      905 2022-10-05 12:22:39.000000 django-cloudspotlicense-6.0.0/django_cloudspotlicense/helpers.py
-drwxrwxrwx   0        0        0        0 2023-06-07 15:38:05.000000 django-cloudspotlicense-6.0.0/django_cloudspotlicense/migrations/
--rw-rw-rw-   0        0        0     3881 2022-10-05 11:36:48.000000 django-cloudspotlicense-6.0.0/django_cloudspotlicense/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      452 2022-10-17 09:58:41.000000 django-cloudspotlicense-6.0.0/django_cloudspotlicense/migrations/0002_cloudspotcompany_users.py
--rw-rw-rw-   0        0        0      505 2022-10-17 09:59:00.000000 django-cloudspotlicense-6.0.0/django_cloudspotlicense/migrations/0003_alter_cloudspotcompany_users.py
--rw-rw-rw-   0        0        0        0 2022-10-05 08:35:57.000000 django-cloudspotlicense-6.0.0/django_cloudspotlicense/migrations/__init__.py
--rw-rw-rw-   0        0        0     2987 2023-06-07 15:33:48.000000 django-cloudspotlicense-6.0.0/django_cloudspotlicense/mixins.py
--rw-rw-rw-   0        0        0     1515 2023-05-12 07:05:12.000000 django-cloudspotlicense-6.0.0/django_cloudspotlicense/models.py
-drwxrwxrwx   0        0        0        0 2023-06-07 15:38:05.000000 django-cloudspotlicense-6.0.0/django_cloudspotlicense/templates/
-drwxrwxrwx   0        0        0        0 2023-06-07 15:38:05.000000 django-cloudspotlicense-6.0.0/django_cloudspotlicense/templates/auth/
--rw-rw-rw-   0        0        0      634 2022-10-05 10:05:52.000000 django-cloudspotlicense-6.0.0/django_cloudspotlicense/templates/auth/login.html
--rw-rw-rw-   0        0        0      496 2022-10-17 09:51:34.000000 django-cloudspotlicense-6.0.0/django_cloudspotlicense/templates/auth/select_company.html
-drwxrwxrwx   0        0        0        0 2023-06-07 15:38:05.000000 django-cloudspotlicense-6.0.0/django_cloudspotlicense/templatetags/
--rw-rw-rw-   0        0        0      377 2023-03-13 08:55:48.000000 django-cloudspotlicense-6.0.0/django_cloudspotlicense/templatetags/license_tags.py
--rw-rw-rw-   0        0        0        0 2022-12-09 12:36:09.000000 django-cloudspotlicense-6.0.0/django_cloudspotlicense/templatetags/__init__.py
--rw-rw-rw-   0        0        0       63 2022-10-05 08:35:57.000000 django-cloudspotlicense-6.0.0/django_cloudspotlicense/tests.py
--rw-rw-rw-   0        0        0     1019 2023-03-08 12:37:58.000000 django-cloudspotlicense-6.0.0/django_cloudspotlicense/urls.py
--rw-rw-rw-   0        0        0      401 2023-06-07 15:34:10.000000 django-cloudspotlicense-6.0.0/django_cloudspotlicense/utils.py
--rw-rw-rw-   0        0        0    14577 2023-06-07 15:33:36.000000 django-cloudspotlicense-6.0.0/django_cloudspotlicense/views.py
--rw-rw-rw-   0        0        0       69 2023-06-07 15:37:09.000000 django-cloudspotlicense-6.0.0/django_cloudspotlicense/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 15:38:05.000000 django-cloudspotlicense-6.0.0/django_cloudspotlicense.egg-info/
--rw-rw-rw-   0        0        0        1 2023-06-07 15:38:04.000000 django-cloudspotlicense-6.0.0/django_cloudspotlicense.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     8123 2023-06-07 15:38:04.000000 django-cloudspotlicense-6.0.0/django_cloudspotlicense.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       31 2023-06-07 15:38:04.000000 django-cloudspotlicense-6.0.0/django_cloudspotlicense.egg-info/requires.txt
--rw-rw-rw-   0        0        0     1148 2023-06-07 15:38:04.000000 django-cloudspotlicense-6.0.0/django_cloudspotlicense.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       24 2023-06-07 15:38:04.000000 django-cloudspotlicense-6.0.0/django_cloudspotlicense.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35821 2021-04-16 13:14:04.000000 django-cloudspotlicense-6.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0       93 2022-10-05 14:15:21.000000 django-cloudspotlicense-6.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     8123 2023-06-07 15:38:05.000000 django-cloudspotlicense-6.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     7259 2023-03-08 12:16:04.000000 django-cloudspotlicense-6.0.0/README.md
--rw-rw-rw-   0        0        0       86 2023-06-07 15:38:05.000000 django-cloudspotlicense-6.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1401 2023-06-07 15:37:21.000000 django-cloudspotlicense-6.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 09:21:37.000000 django-cloudspotlicense-6.1.0/
+drwxrwxrwx   0        0        0        0 2023-06-09 09:21:37.000000 django-cloudspotlicense-6.1.0/django_cloudspotlicense/
+-rw-rw-rw-   0        0        0       66 2022-10-05 08:35:57.000000 django-cloudspotlicense-6.1.0/django_cloudspotlicense/admin.py
+-rw-rw-rw-   0        0        0      183 2022-10-05 10:03:35.000000 django-cloudspotlicense-6.1.0/django_cloudspotlicense/apps.py
+-rw-rw-rw-   0        0        0      244 2023-06-07 15:51:33.000000 django-cloudspotlicense-6.1.0/django_cloudspotlicense/config.py
+-rw-rw-rw-   0        0        0      246 2022-10-19 14:26:18.000000 django-cloudspotlicense-6.1.0/django_cloudspotlicense/context_processors.py
+-rw-rw-rw-   0        0        0      905 2022-10-05 12:22:39.000000 django-cloudspotlicense-6.1.0/django_cloudspotlicense/helpers.py
+drwxrwxrwx   0        0        0        0 2023-06-09 09:21:37.000000 django-cloudspotlicense-6.1.0/django_cloudspotlicense/migrations/
+-rw-rw-rw-   0        0        0     3881 2022-10-05 11:36:48.000000 django-cloudspotlicense-6.1.0/django_cloudspotlicense/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      452 2022-10-17 09:58:41.000000 django-cloudspotlicense-6.1.0/django_cloudspotlicense/migrations/0002_cloudspotcompany_users.py
+-rw-rw-rw-   0        0        0      505 2022-10-17 09:59:00.000000 django-cloudspotlicense-6.1.0/django_cloudspotlicense/migrations/0003_alter_cloudspotcompany_users.py
+-rw-rw-rw-   0        0        0        0 2022-10-05 08:35:57.000000 django-cloudspotlicense-6.1.0/django_cloudspotlicense/migrations/__init__.py
+-rw-rw-rw-   0        0        0     2987 2023-06-07 15:51:33.000000 django-cloudspotlicense-6.1.0/django_cloudspotlicense/mixins.py
+-rw-rw-rw-   0        0        0     1515 2023-05-12 07:05:12.000000 django-cloudspotlicense-6.1.0/django_cloudspotlicense/models.py
+drwxrwxrwx   0        0        0        0 2023-06-09 09:21:36.000000 django-cloudspotlicense-6.1.0/django_cloudspotlicense/templates/
+drwxrwxrwx   0        0        0        0 2023-06-09 09:21:37.000000 django-cloudspotlicense-6.1.0/django_cloudspotlicense/templates/auth/
+-rw-rw-rw-   0        0        0      634 2022-10-05 10:05:52.000000 django-cloudspotlicense-6.1.0/django_cloudspotlicense/templates/auth/login.html
+-rw-rw-rw-   0        0        0      496 2022-10-17 09:51:34.000000 django-cloudspotlicense-6.1.0/django_cloudspotlicense/templates/auth/select_company.html
+drwxrwxrwx   0        0        0        0 2023-06-09 09:21:37.000000 django-cloudspotlicense-6.1.0/django_cloudspotlicense/templatetags/
+-rw-rw-rw-   0        0        0      377 2023-03-13 08:55:48.000000 django-cloudspotlicense-6.1.0/django_cloudspotlicense/templatetags/license_tags.py
+-rw-rw-rw-   0        0        0        0 2022-12-09 12:36:09.000000 django-cloudspotlicense-6.1.0/django_cloudspotlicense/templatetags/__init__.py
+-rw-rw-rw-   0        0        0       63 2022-10-05 08:35:57.000000 django-cloudspotlicense-6.1.0/django_cloudspotlicense/tests.py
+-rw-rw-rw-   0        0        0     1019 2023-03-08 12:37:58.000000 django-cloudspotlicense-6.1.0/django_cloudspotlicense/urls.py
+-rw-rw-rw-   0        0        0      401 2023-06-07 15:51:33.000000 django-cloudspotlicense-6.1.0/django_cloudspotlicense/utils.py
+-rw-rw-rw-   0        0        0    15952 2023-06-09 09:19:51.000000 django-cloudspotlicense-6.1.0/django_cloudspotlicense/views.py
+-rw-rw-rw-   0        0        0       69 2023-06-09 09:19:51.000000 django-cloudspotlicense-6.1.0/django_cloudspotlicense/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 09:21:37.000000 django-cloudspotlicense-6.1.0/django_cloudspotlicense.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-06-09 09:21:36.000000 django-cloudspotlicense-6.1.0/django_cloudspotlicense.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0    10292 2023-06-09 09:21:36.000000 django-cloudspotlicense-6.1.0/django_cloudspotlicense.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       31 2023-06-09 09:21:36.000000 django-cloudspotlicense-6.1.0/django_cloudspotlicense.egg-info/requires.txt
+-rw-rw-rw-   0        0        0     1148 2023-06-09 09:21:36.000000 django-cloudspotlicense-6.1.0/django_cloudspotlicense.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       24 2023-06-09 09:21:36.000000 django-cloudspotlicense-6.1.0/django_cloudspotlicense.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35821 2021-04-16 13:14:04.000000 django-cloudspotlicense-6.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0       93 2022-10-05 14:15:21.000000 django-cloudspotlicense-6.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    10292 2023-06-09 09:21:37.000000 django-cloudspotlicense-6.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     9428 2023-06-09 09:19:51.000000 django-cloudspotlicense-6.1.0/README.md
+-rw-rw-rw-   0        0        0       86 2023-06-09 09:21:37.000000 django-cloudspotlicense-6.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1401 2023-06-09 09:19:51.000000 django-cloudspotlicense-6.1.0/setup.py
```

### Comparing `django-cloudspotlicense-6.0.0/django_cloudspotlicense/helpers.py` & `django-cloudspotlicense-6.1.0/django_cloudspotlicense/helpers.py`

 * *Files identical despite different names*

### Comparing `django-cloudspotlicense-6.0.0/django_cloudspotlicense/migrations/0001_initial.py` & `django-cloudspotlicense-6.1.0/django_cloudspotlicense/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-cloudspotlicense-6.0.0/django_cloudspotlicense/mixins.py` & `django-cloudspotlicense-6.1.0/django_cloudspotlicense/mixins.py`

 * *Files identical despite different names*

### Comparing `django-cloudspotlicense-6.0.0/django_cloudspotlicense/models.py` & `django-cloudspotlicense-6.1.0/django_cloudspotlicense/models.py`

 * *Files identical despite different names*

### Comparing `django-cloudspotlicense-6.0.0/django_cloudspotlicense/templates/auth/login.html` & `django-cloudspotlicense-6.1.0/django_cloudspotlicense/templates/auth/login.html`

 * *Files identical despite different names*

### Comparing `django-cloudspotlicense-6.0.0/django_cloudspotlicense/urls.py` & `django-cloudspotlicense-6.1.0/django_cloudspotlicense/urls.py`

 * *Files identical despite different names*

### Comparing `django-cloudspotlicense-6.0.0/django_cloudspotlicense/views.py` & `django-cloudspotlicense-6.1.0/django_cloudspotlicense/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,16 +76,21 @@
             user.pin = api.user.pin
             user.is_active = True
             user.save()
             
         except ObjectDoesNotExist:
             
             # We don't know the user, so we create them
+            
+            # This is a dummy password, because we don't need it.
+            # The user will never be able to login with this password, because the login is handled by the License Server.
+            dummy_password = 'AreYouTryingToHackMe?' 
+            
             # Push it to the database
-            user = UserModel.objects.create_user(username=username, email=username, password=password, **{
+            user = UserModel.objects.create_user(username=username, email=username, password=dummy_password, **{
                 'first_name' : api.user.first_name,
                 'last_name' : api.user.last_name,
                 'license_token' : api.token,
                 'pin' : api.user.pin,
             })
             
             user.save()
@@ -304,8 +309,27 @@
                 user = UserModel.objects.get(username=user_username)
             except UserModel.DoesNotExist:
                 return JsonResponse({ 'status' : ResponseStatus.NOT_FOUND, 'error' : { 'message' : 'No user matched the user_username.' }}, status=HTTPStatus.NOT_FOUND)
             
             user.pin = pin
             user.save()
             
-            return JsonResponse({ 'status' : ResponseStatus.OBJECT_UPDATED })
+            return JsonResponse({ 'status' : ResponseStatus.OBJECT_UPDATED })
+        elif event == 'user.created':
+            user_email = data['user_email']
+            user_first_name = data['user_first_name']
+            user_last_name = data['user_last_name']
+            user_pin = data['user_pin']
+            user_pwd = data['user_pwd'] # This will contain a dummy password, we don't need to know the actual password
+            
+            # Check if the user already exists
+            try:
+                user = UserModel.objects.get(username=user_email)
+                return JsonResponse({ 'status' : ResponseStatus.OBJECT_EXISTS, 'error' : { 'message' : 'User already exists.' }}, status=HTTPStatus.BAD_REQUEST)
+            except UserModel.DoesNotExist:
+                user = UserModel.objects.create_user(username=user_email, email=user_email, password=user_pwd, **{
+                    'first_name' : user_first_name,
+                    'last_name' : user_last_name,
+                    'pin' : user_pin,
+                })
+            
+            return JsonResponse({ 'status' : ResponseStatus.OBJECT_CREATED, 'id' : user.id })
```

### Comparing `django-cloudspotlicense-6.0.0/django_cloudspotlicense.egg-info/PKG-INFO` & `django-cloudspotlicense-6.1.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: django-cloudspotlicense
-Version: 6.0.0
-Summary: Django package to integrate the authentication of the Cloudspot License Server in other django applications
-Home-page: https://github.com/Ecosy-EU/django-cloudspotlicense
-Author: Alexander Schillemans
-Author-email: alexander.schillemans@lhs.global
-License: GPL-3.0-or-later
-Download-URL: https://github.com/Ecosy-EU/django-cloudspotlicense/archive/refs/tags/6.0.0.tar.gz
-Keywords: cloudspot,django
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Programming Language :: Python :: 3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # django-cloudspotlicense
 Django package to integrate the authentication of the Cloudspot License Server in other django applications.
 
 
 ## Getting started
 
 ### Install
@@ -94,14 +75,72 @@
 
 Use as normal.
 
 ```python
 print(user.extra_data) # foobar
 ```
 
+## Permission checking
+
+There are a few ways to check if the current user has the correct permission on the Cloudspot License server to do an action.
+It's important that you **do not use the built-in permission checker from Django**. This will always return ```False``` on any given permission.
+
+1. **Class-based views**
+
+When using class-based views, you can import the modified ```PermissionRequiredMixin``` and ```LoginRequiredMixin```.
+When using ```PermissionRequiredMixin```, the ```LoginRequiredMixin``` is implied as an anonymous user can not have any permissions.
+
+```python
+from django_cloudspotlicense.mixins import PermissionRequiredMixin, LoginRequiredMixin
+
+# Use as is normal within Django
+# The user needs the permission 'use_dashboard' to be able to view this template
+class Dashboard(PermissionRequiredMixin, TemplateView):
+    permission_required = 'use_dashboard' # use the permission code as shown in the Cloudspot License server
+    template_name = '...'
+# OR
+# The user needs to be logged in and be assigned a company (which is always required) before he's able to see this view
+class Projects(LoginRequiredMixin, TemplateView):
+    template_name = '...'
+```
+
+2. **Functions**
+
+You can use the utility function ```has_perm()``` to check if a user has a permission.
+
+```python
+from django_cloudspotlicense.utils import has_perm
+
+if has_perm(user, 'use_dashboard'):
+    # user has the permission use_dashboard in Cloudspot License server
+else:
+    # user does not have the permission
+```
+
+**! At this moment it's not possible to check multiple permissions at once. You will need to call the function for each permission.**
+
+3. **Templates**
+
+Inside a template, you can use a templatetag to check for the correct permission.
+
+```html
+<!-- This is REQUIRED, else the tag will not work -->
+{% load license_tags %} 
+
+<!-- Use the tag 'has_perm' on a user object -->
+{% if request.user|has_perm:'list_projects' %}
+    <!-- This piece of HTML will only be rendered if the user has the 'list_projects' permission -->
+    <h3>Projects</h3>
+    <ul>
+        <li>...</li>
+    </ul>
+{% endif %}
+```
+
+
 ## Webhook
 
 This package also provides a webhook where the Cloudspot License Server will send updates to whenever the permissions for a user changes.
 The webhook is located at ```https://example.com/auth/webhook```. This webhook is automatically activated when importing the URLConf.
 
 
 ## Migrating to the License server from an existing application
@@ -259,9 +298,8 @@
 ```python
 # settings.py
 
 AUTH_USER_MODEL = 'main.User'
 ```
 
 ### 15. Migration done
-The migration is now done. Follow the quick start from step 2.
-
+The migration is now done. Follow the quick start from step 2.
```

### Comparing `django-cloudspotlicense-6.0.0/django_cloudspotlicense.egg-info/SOURCES.txt` & `django-cloudspotlicense-6.1.0/django_cloudspotlicense.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-cloudspotlicense-6.0.0/LICENSE.txt` & `django-cloudspotlicense-6.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-cloudspotlicense-6.0.0/PKG-INFO` & `django-cloudspotlicense-6.1.0/django_cloudspotlicense.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: django-cloudspotlicense
-Version: 6.0.0
+Version: 6.1.0
 Summary: Django package to integrate the authentication of the Cloudspot License Server in other django applications
 Home-page: https://github.com/Ecosy-EU/django-cloudspotlicense
 Author: Alexander Schillemans
 Author-email: alexander.schillemans@lhs.global
 License: GPL-3.0-or-later
-Download-URL: https://github.com/Ecosy-EU/django-cloudspotlicense/archive/refs/tags/6.0.0.tar.gz
+Download-URL: https://github.com/Ecosy-EU/django-cloudspotlicense/archive/refs/tags/6.1.0.tar.gz
 Keywords: cloudspot,django
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3.6
@@ -94,14 +94,72 @@
 
 Use as normal.
 
 ```python
 print(user.extra_data) # foobar
 ```
 
+## Permission checking
+
+There are a few ways to check if the current user has the correct permission on the Cloudspot License server to do an action.
+It's important that you **do not use the built-in permission checker from Django**. This will always return ```False``` on any given permission.
+
+1. **Class-based views**
+
+When using class-based views, you can import the modified ```PermissionRequiredMixin``` and ```LoginRequiredMixin```.
+When using ```PermissionRequiredMixin```, the ```LoginRequiredMixin``` is implied as an anonymous user can not have any permissions.
+
+```python
+from django_cloudspotlicense.mixins import PermissionRequiredMixin, LoginRequiredMixin
+
+# Use as is normal within Django
+# The user needs the permission 'use_dashboard' to be able to view this template
+class Dashboard(PermissionRequiredMixin, TemplateView):
+    permission_required = 'use_dashboard' # use the permission code as shown in the Cloudspot License server
+    template_name = '...'
+# OR
+# The user needs to be logged in and be assigned a company (which is always required) before he's able to see this view
+class Projects(LoginRequiredMixin, TemplateView):
+    template_name = '...'
+```
+
+2. **Functions**
+
+You can use the utility function ```has_perm()``` to check if a user has a permission.
+
+```python
+from django_cloudspotlicense.utils import has_perm
+
+if has_perm(user, 'use_dashboard'):
+    # user has the permission use_dashboard in Cloudspot License server
+else:
+    # user does not have the permission
+```
+
+**! At this moment it's not possible to check multiple permissions at once. You will need to call the function for each permission.**
+
+3. **Templates**
+
+Inside a template, you can use a templatetag to check for the correct permission.
+
+```html
+<!-- This is REQUIRED, else the tag will not work -->
+{% load license_tags %} 
+
+<!-- Use the tag 'has_perm' on a user object -->
+{% if request.user|has_perm:'list_projects' %}
+    <!-- This piece of HTML will only be rendered if the user has the 'list_projects' permission -->
+    <h3>Projects</h3>
+    <ul>
+        <li>...</li>
+    </ul>
+{% endif %}
+```
+
+
 ## Webhook
 
 This package also provides a webhook where the Cloudspot License Server will send updates to whenever the permissions for a user changes.
 The webhook is located at ```https://example.com/auth/webhook```. This webhook is automatically activated when importing the URLConf.
 
 
 ## Migrating to the License server from an existing application
```

### Comparing `django-cloudspotlicense-6.0.0/setup.py` & `django-cloudspotlicense-6.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
   name = 'django-cloudspotlicense',         
   packages=['django_cloudspotlicense', 'django_cloudspotlicense.migrations', 'django_cloudspotlicense.templatetags'],
   include_package_data=True,
-  version = '6.0.0',
+  version = '6.1.0',
   license='GPL-3.0-or-later',
   description = 'Django package to integrate the authentication of the Cloudspot License Server in other django applications',
   long_description=long_description,
   long_description_content_type='text/markdown',
   author = 'Alexander Schillemans',
   author_email = 'alexander.schillemans@lhs.global',
   url = 'https://github.com/Ecosy-EU/django-cloudspotlicense',
-  download_url = 'https://github.com/Ecosy-EU/django-cloudspotlicense/archive/refs/tags/6.0.0.tar.gz',
+  download_url = 'https://github.com/Ecosy-EU/django-cloudspotlicense/archive/refs/tags/6.1.0.tar.gz',
   keywords = ['cloudspot', 'django'],
   install_requires=[
           'requests',
           'cloudspot-license-api',
       ],
   classifiers=[
     'Development Status :: 3 - Alpha',
```

