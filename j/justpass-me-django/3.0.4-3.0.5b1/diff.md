# Comparing `tmp/justpass-me-django-3.0.4.tar.gz` & `tmp/justpass-me-django-3.0.5b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "justpass-me-django-3.0.4.tar", last modified: Thu May 18 12:00:02 2023, max compression
+gzip compressed data, was "justpass-me-django-3.0.5b1.tar", last modified: Fri Jun  9 14:03:31 2023, max compression
```

## Comparing `justpass-me-django-3.0.4.tar` & `justpass-me-django-3.0.5b1.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-05-18 12:00:02.928241 justpass-me-django-3.0.4/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1067 2023-05-15 15:42:36.000000 justpass-me-django-3.0.4/LICENSE
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     4885 2023-05-18 12:00:02.928241 justpass-me-django-3.0.4/PKG-INFO
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     3643 2023-05-18 11:58:56.000000 justpass-me-django-3.0.4/README.md
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-05-18 12:00:02.928241 justpass-me-django-3.0.4/justpass_me_django.egg-info/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     4885 2023-05-18 12:00:02.000000 justpass-me-django-3.0.4/justpass_me_django.egg-info/PKG-INFO
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      445 2023-05-18 12:00:02.000000 justpass-me-django-3.0.4/justpass_me_django.egg-info/SOURCES.txt
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        1 2023-05-18 12:00:02.000000 justpass-me-django-3.0.4/justpass_me_django.egg-info/dependency_links.txt
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        1 2023-05-15 15:48:48.000000 justpass-me-django-3.0.4/justpass_me_django.egg-info/not-zip-safe
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       58 2023-05-18 12:00:02.000000 justpass-me-django-3.0.4/justpass_me_django.egg-info/requires.txt
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       11 2023-05-18 12:00:02.000000 justpass-me-django-3.0.4/justpass_me_django.egg-info/top_level.txt
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-05-18 12:00:02.928241 justpass-me-django-3.0.4/justpassme/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     6758 2023-05-18 11:49:19.000000 justpass-me-django-3.0.4/justpassme/OIDC_CLIENT.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        0 2023-05-15 15:07:58.000000 justpass-me-django-3.0.4/justpassme/__init__.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       63 2023-05-15 15:07:58.000000 justpass-me-django-3.0.4/justpassme/admin.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      152 2023-05-15 15:13:26.000000 justpass-me-django-3.0.4/justpassme/apps.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1096 2023-05-18 11:49:19.000000 justpass-me-django-3.0.4/justpassme/helpers.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      672 2023-05-18 11:49:19.000000 justpass-me-django-3.0.4/justpassme/urls.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      168 2023-05-15 15:07:58.000000 justpass-me-django-3.0.4/justpassme/utils.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      968 2023-05-18 11:49:19.000000 justpass-me-django-3.0.4/justpassme/views.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       38 2023-05-18 12:00:02.928241 justpass-me-django-3.0.4/setup.cfg
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1688 2023-05-18 11:59:52.000000 justpass-me-django-3.0.4/setup.py
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-06-09 14:03:31.061977 justpass-me-django-3.0.5b1/
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1067 2023-05-15 16:53:18.000000 justpass-me-django-3.0.5b1/LICENSE
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     4911 2023-06-09 14:03:31.061977 justpass-me-django-3.0.5b1/PKG-INFO
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     3648 2023-05-18 19:36:39.000000 justpass-me-django-3.0.5b1/README.md
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-06-09 14:03:31.061977 justpass-me-django-3.0.5b1/justpass_me_django.egg-info/
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     4911 2023-06-09 14:03:30.000000 justpass-me-django-3.0.5b1/justpass_me_django.egg-info/PKG-INFO
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      456 2023-06-09 14:03:30.000000 justpass-me-django-3.0.5b1/justpass_me_django.egg-info/SOURCES.txt
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        1 2023-06-09 14:03:30.000000 justpass-me-django-3.0.5b1/justpass_me_django.egg-info/dependency_links.txt
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        1 2023-05-15 16:54:06.000000 justpass-me-django-3.0.5b1/justpass_me_django.egg-info/not-zip-safe
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       58 2023-06-09 14:03:30.000000 justpass-me-django-3.0.5b1/justpass_me_django.egg-info/requires.txt
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       11 2023-06-09 14:03:30.000000 justpass-me-django-3.0.5b1/justpass_me_django.egg-info/top_level.txt
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-06-09 14:03:31.061977 justpass-me-django-3.0.5b1/justpassme/
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     7896 2023-06-09 13:58:06.000000 justpass-me-django-3.0.5b1/justpassme/OIDC_CLIENT.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        0 2023-05-15 16:53:18.000000 justpass-me-django-3.0.5b1/justpassme/__init__.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       63 2023-05-15 16:53:18.000000 justpass-me-django-3.0.5b1/justpassme/admin.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      152 2023-05-15 16:53:18.000000 justpass-me-django-3.0.5b1/justpassme/apps.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1096 2023-05-15 17:40:25.000000 justpass-me-django-3.0.5b1/justpassme/helpers.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      672 2023-05-15 17:54:17.000000 justpass-me-django-3.0.5b1/justpassme/urls.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      168 2023-05-15 16:53:18.000000 justpass-me-django-3.0.5b1/justpassme/utils.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      968 2023-05-15 17:42:22.000000 justpass-me-django-3.0.5b1/justpassme/views.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1690 2023-06-09 14:03:23.000000 justpass-me-django-3.0.5b1/setup-3.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       38 2023-06-09 14:03:31.061977 justpass-me-django-3.0.5b1/setup.cfg
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1690 2023-06-09 14:03:23.000000 justpass-me-django-3.0.5b1/setup.py
```

### Comparing `justpass-me-django-3.0.4/LICENSE` & `justpass-me-django-3.0.5b1/LICENSE`

 * *Files identical despite different names*

### Comparing `justpass-me-django-3.0.4/PKG-INFO` & `justpass-me-django-3.0.5b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: justpass-me-django
-Version: 3.0.4
+Version: 3.0.5b1
 Summary: Django Integration with JustPass.me
 Home-page: https://github.com/justpass-me/justpass-me-django
-Download-URL: https://github.com/justpass-me/justpass-me-django
 Author: JustPassMe
 Author-email: sameh@justpass.me
 License: MIT
+Download-URL: https://github.com/justpass-me/justpass-me-django
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
@@ -100,32 +101,24 @@
    urls_patterns= [
    '...',
    path(r'justpass/', include('justpassme.urls')),
    path('oidc/',include('mozilla_django_oidc.urls')),
    '....',
     ]
     ```
-## Note:  If you use justpass.me as 2nd factor
 
-Break your login function, Usually your login function will check for username and password, log the user in if the username and password are correct and create the user session, to support justpass.me, this has to change
-   
-   * authenticate the user
-   * if username and password are correct , check if the user has mfa or not
-       * if user has mfa then redirect to justpass.me
-       * if user doesn't have mfa then call your function to create the user session
+4. To start registration, redirct to  `justpass:start_reg`
 
-3. To start registration, redirct to  `justpass:start_reg`
 
-
-4. To start login, redirect to `justpass:start_login`
+5. To start login, redirect to `justpass:start_login`
 
    **Note:** For 2nd factor, The function expects the user's username to be in `request.session["base_username"]`
 
 
-5. Write 4 functions that handle the success and failure of registration and login, refer to them in the `settings.py` 
+6. Write 4 functions that handle the success and failure of registration and login, refer to them in the `settings.py` 
 
    You can use the four functions below as a reference.
 
    ```python
    def auth_success(request):
       return redirect('home')
          
@@ -138,7 +131,18 @@
       request.session["reg"] = True
       return redirect('home')
       
    def reg_failure(request):
       request.session["reg"] = False
       return redirect('home')
    ```
+   
+## Note:  If you use justpass.me as 2nd factor
+
+Break your login function, Usually your login function will check for username and password, log the user in if the username and password are correct and create the user session, to support justpass.me, this has to change
+   
+   * authenticate the user
+   * if username and password are correct , check if the user has mfa or not
+       * if user has mfa then redirect to justpass.me
+       * if user doesn't have mfa then call your function to create the user session
+
+
```

### Comparing `justpass-me-django-3.0.4/README.md` & `justpass-me-django-3.0.5b1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -68,32 +68,24 @@
    urls_patterns= [
    '...',
    path(r'justpass/', include('justpassme.urls')),
    path('oidc/',include('mozilla_django_oidc.urls')),
    '....',
     ]
     ```
-## Note:  If you use justpass.me as 2nd factor
 
-Break your login function, Usually your login function will check for username and password, log the user in if the username and password are correct and create the user session, to support justpass.me, this has to change
-   
-   * authenticate the user
-   * if username and password are correct , check if the user has mfa or not
-       * if user has mfa then redirect to justpass.me
-       * if user doesn't have mfa then call your function to create the user session
+4. To start registration, redirct to  `justpass:start_reg`
 
-3. To start registration, redirct to  `justpass:start_reg`
 
-
-4. To start login, redirect to `justpass:start_login`
+5. To start login, redirect to `justpass:start_login`
 
    **Note:** For 2nd factor, The function expects the user's username to be in `request.session["base_username"]`
 
 
-5. Write 4 functions that handle the success and failure of registration and login, refer to them in the `settings.py` 
+6. Write 4 functions that handle the success and failure of registration and login, refer to them in the `settings.py` 
 
    You can use the four functions below as a reference.
 
    ```python
    def auth_success(request):
       return redirect('home')
          
@@ -105,8 +97,17 @@
       request.user.save()
       request.session["reg"] = True
       return redirect('home')
       
    def reg_failure(request):
       request.session["reg"] = False
       return redirect('home')
-   ```
+   ```
+   
+## Note:  If you use justpass.me as 2nd factor
+
+Break your login function, Usually your login function will check for username and password, log the user in if the username and password are correct and create the user session, to support justpass.me, this has to change
+   
+   * authenticate the user
+   * if username and password are correct , check if the user has mfa or not
+       * if user has mfa then redirect to justpass.me
+       * if user doesn't have mfa then call your function to create the user session
```

### Comparing `justpass-me-django-3.0.4/justpass_me_django.egg-info/PKG-INFO` & `justpass-me-django-3.0.5b1/justpass_me_django.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: justpass-me-django
-Version: 3.0.4
+Version: 3.0.5b1
 Summary: Django Integration with JustPass.me
 Home-page: https://github.com/justpass-me/justpass-me-django
-Download-URL: https://github.com/justpass-me/justpass-me-django
 Author: JustPassMe
 Author-email: sameh@justpass.me
 License: MIT
+Download-URL: https://github.com/justpass-me/justpass-me-django
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
@@ -100,32 +101,24 @@
    urls_patterns= [
    '...',
    path(r'justpass/', include('justpassme.urls')),
    path('oidc/',include('mozilla_django_oidc.urls')),
    '....',
     ]
     ```
-## Note:  If you use justpass.me as 2nd factor
 
-Break your login function, Usually your login function will check for username and password, log the user in if the username and password are correct and create the user session, to support justpass.me, this has to change
-   
-   * authenticate the user
-   * if username and password are correct , check if the user has mfa or not
-       * if user has mfa then redirect to justpass.me
-       * if user doesn't have mfa then call your function to create the user session
+4. To start registration, redirct to  `justpass:start_reg`
 
-3. To start registration, redirct to  `justpass:start_reg`
 
-
-4. To start login, redirect to `justpass:start_login`
+5. To start login, redirect to `justpass:start_login`
 
    **Note:** For 2nd factor, The function expects the user's username to be in `request.session["base_username"]`
 
 
-5. Write 4 functions that handle the success and failure of registration and login, refer to them in the `settings.py` 
+6. Write 4 functions that handle the success and failure of registration and login, refer to them in the `settings.py` 
 
    You can use the four functions below as a reference.
 
    ```python
    def auth_success(request):
       return redirect('home')
          
@@ -138,7 +131,18 @@
       request.session["reg"] = True
       return redirect('home')
       
    def reg_failure(request):
       request.session["reg"] = False
       return redirect('home')
    ```
+   
+## Note:  If you use justpass.me as 2nd factor
+
+Break your login function, Usually your login function will check for username and password, log the user in if the username and password are correct and create the user session, to support justpass.me, this has to change
+   
+   * authenticate the user
+   * if username and password are correct , check if the user has mfa or not
+       * if user has mfa then redirect to justpass.me
+       * if user doesn't have mfa then call your function to create the user session
+
+
```

### Comparing `justpass-me-django-3.0.4/justpassme/OIDC_CLIENT.py` & `justpass-me-django-3.0.5b1/justpassme/OIDC_CLIENT.py`

 * *Files 21% similar despite different names*

```diff
@@ -96,14 +96,41 @@
         try:
             kwargs = {getattr(settings,"OIDC_USERNAME_FIELD","username"): username}
             profile = User.objects.get(**kwargs)
             return [profile]
         except Exception: pass
         return self.UserModel.objects.none()
 
+    def create_user(self, claims):
+        """Return object for a newly created user account."""
+        email = claims.get("email")
+        username = self.get_username(claims)
+        kwargs = {"email":email, getattr(settings, "OIDC_USERNAME_FIELD", "username"): username}
+        return self.UserModel.objects.create_user(**kwargs)
+
+    def get_username(self, claims):
+        """Generate username based on claims."""
+        # bluntly stolen from django-browserid
+        # https://github.com/mozilla/django-browserid/blob/master/django_browserid/auth.py
+        username_algo = self.get_settings("OIDC_USERNAME_ALGO", None)
+
+        if username_algo:
+            if isinstance(username_algo, str):
+                username_algo = import_string(username_algo)
+            return username_algo(claims.get("email"))
+
+        return default_username_algo(claims.get("email"))
+
+    def create_user(self, claims):
+        """Return object for a newly created user account."""
+        email = claims.get("email")
+        username = claims.get("preferred_username")
+        return self.UserModel.objects.create_user(username, email=email)
+
+
 
 class Callback(OIDCAuthenticationCallbackView):
     """Handles the callback received from OIDC Provider"""
     def get(self, request):
         """Callback handler for OIDC authorization code flow"""
 
         if request.GET.get("error"):
```

### Comparing `justpass-me-django-3.0.4/justpassme/helpers.py` & `justpass-me-django-3.0.5b1/justpassme/helpers.py`

 * *Files identical despite different names*

### Comparing `justpass-me-django-3.0.4/justpassme/urls.py` & `justpass-me-django-3.0.5b1/justpassme/urls.py`

 * *Files identical despite different names*

### Comparing `justpass-me-django-3.0.4/justpassme/views.py` & `justpass-me-django-3.0.5b1/justpassme/views.py`

 * *Files identical despite different names*

### Comparing `justpass-me-django-3.0.4/setup.py` & `justpass-me-django-3.0.5b1/setup-3.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from setuptools import find_packages, setup
 
 setup(
     name='justpass-me-django',
-    version='3.0.4',
+    version='3.0.5b1',
     description='Django Integration with JustPass.me',
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author='JustPassMe',
     author_email = 'sameh@justpass.me',
     url = 'https://github.com/justpass-me/justpass-me-django',
     download_url='https://github.com/justpass-me/justpass-me-django',
```

