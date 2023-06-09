# Comparing `tmp/django-all-in-one-accessibility-1.2.tar.gz` & `tmp/django-all-in-one-accessibility-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-all-in-one-accessibility-1.2.tar", last modified: Wed Jun  7 12:02:59 2023, max compression
+gzip compressed data, was "django-all-in-one-accessibility-1.3.tar", last modified: Fri Jun  9 09:51:01 2023, max compression
```

## Comparing `django-all-in-one-accessibility-1.2.tar` & `django-all-in-one-accessibility-1.3.tar`

### file list

```diff
@@ -1,31 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 12:02:59.175747 django-all-in-one-accessibility-1.2/
--rw-rw-rw-   0        0        0     3991 2023-06-07 12:02:59.175747 django-all-in-one-accessibility-1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2868 2023-06-07 11:25:43.000000 django-all-in-one-accessibility-1.2/README.rst
--rw-rw-rw-   0        0        0     2876 2023-06-07 12:02:46.000000 django-all-in-one-accessibility-1.2/Readme.md
-drwxrwxrwx   0        0        0        0 2023-06-07 12:02:59.148577 django-all-in-one-accessibility-1.2/accessibility/
--rw-rw-rw-   0        0        0        0 2023-06-06 10:32:03.000000 django-all-in-one-accessibility-1.2/accessibility/__init__.py
--rw-rw-rw-   0        0        0      687 2023-06-06 10:53:45.000000 django-all-in-one-accessibility-1.2/accessibility/admin.py
--rw-rw-rw-   0        0        0      106 2023-06-06 10:32:03.000000 django-all-in-one-accessibility-1.2/accessibility/apps.py
--rw-rw-rw-   0        0        0      527 2023-06-06 10:58:34.000000 django-all-in-one-accessibility-1.2/accessibility/context_processors.py
-drwxrwxrwx   0        0        0        0 2023-06-07 12:02:59.150570 django-all-in-one-accessibility-1.2/accessibility/migrations/
--rw-rw-rw-   0        0        0     2019 2023-06-06 10:39:45.000000 django-all-in-one-accessibility-1.2/accessibility/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2023-06-06 10:32:03.000000 django-all-in-one-accessibility-1.2/accessibility/migrations/__init__.py
--rw-rw-rw-   0        0        0     1922 2023-06-06 10:38:52.000000 django-all-in-one-accessibility-1.2/accessibility/models.py
--rw-rw-rw-   0        0        0       63 2023-06-06 10:32:03.000000 django-all-in-one-accessibility-1.2/accessibility/tests.py
--rw-rw-rw-   0        0        0      162 2023-06-06 10:33:50.000000 django-all-in-one-accessibility-1.2/accessibility/urls.py
--rw-rw-rw-   0        0        0      239 2023-06-06 10:34:08.000000 django-all-in-one-accessibility-1.2/accessibility/views.py
-drwxrwxrwx   0        0        0        0 2023-06-07 12:02:59.165770 django-all-in-one-accessibility-1.2/aioa_accessibility/
--rw-rw-rw-   0        0        0        0 2023-06-06 10:30:59.000000 django-all-in-one-accessibility-1.2/aioa_accessibility/__init__.py
--rw-rw-rw-   0        0        0      429 2023-06-06 10:30:59.000000 django-all-in-one-accessibility-1.2/aioa_accessibility/asgi.py
--rw-rw-rw-   0        0        0     3349 2023-06-06 10:43:35.000000 django-all-in-one-accessibility-1.2/aioa_accessibility/settings.py
--rw-rw-rw-   0        0        0      834 2023-06-06 10:32:54.000000 django-all-in-one-accessibility-1.2/aioa_accessibility/urls.py
--rw-rw-rw-   0        0        0      429 2023-06-06 10:30:59.000000 django-all-in-one-accessibility-1.2/aioa_accessibility/wsgi.py
-drwxrwxrwx   0        0        0        0 2023-06-07 12:02:59.174747 django-all-in-one-accessibility-1.2/django_all_in_one_accessibility.egg-info/
--rw-rw-rw-   0        0        0     3991 2023-06-07 12:02:59.000000 django-all-in-one-accessibility-1.2/django_all_in_one_accessibility.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      748 2023-06-07 12:02:59.000000 django-all-in-one-accessibility-1.2/django_all_in_one_accessibility.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 12:02:59.000000 django-all-in-one-accessibility-1.2/django_all_in_one_accessibility.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-06-07 12:02:59.000000 django-all-in-one-accessibility-1.2/django_all_in_one_accessibility.egg-info/requires.txt
--rw-rw-rw-   0        0        0       33 2023-06-07 12:02:59.000000 django-all-in-one-accessibility-1.2/django_all_in_one_accessibility.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1079 2023-06-07 12:01:08.000000 django-all-in-one-accessibility-1.2/pyproject.toml
--rw-rw-rw-   0        0        0     1032 2023-06-07 12:02:59.176743 django-all-in-one-accessibility-1.2/setup.cfg
--rw-rw-rw-   0        0        0       37 2023-06-07 04:23:51.000000 django-all-in-one-accessibility-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 09:51:01.167836 django-all-in-one-accessibility-1.3/
+-rw-rw-rw-   0        0        0     3956 2023-06-09 09:51:01.168829 django-all-in-one-accessibility-1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2841 2023-06-09 09:50:31.000000 django-all-in-one-accessibility-1.3/Readme.md
+drwxrwxrwx   0        0        0        0 2023-06-09 09:51:01.135712 django-all-in-one-accessibility-1.3/accessibility/
+-rw-rw-rw-   0        0        0        0 2023-06-06 10:32:03.000000 django-all-in-one-accessibility-1.3/accessibility/__init__.py
+-rw-rw-rw-   0        0        0      687 2023-06-06 10:53:45.000000 django-all-in-one-accessibility-1.3/accessibility/admin.py
+-rw-rw-rw-   0        0        0      106 2023-06-06 10:32:03.000000 django-all-in-one-accessibility-1.3/accessibility/apps.py
+-rw-rw-rw-   0        0        0      527 2023-06-06 10:58:34.000000 django-all-in-one-accessibility-1.3/accessibility/context_processors.py
+drwxrwxrwx   0        0        0        0 2023-06-09 09:51:01.138670 django-all-in-one-accessibility-1.3/accessibility/migrations/
+-rw-rw-rw-   0        0        0     2019 2023-06-06 10:39:45.000000 django-all-in-one-accessibility-1.3/accessibility/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0        0 2023-06-06 10:32:03.000000 django-all-in-one-accessibility-1.3/accessibility/migrations/__init__.py
+-rw-rw-rw-   0        0        0     1922 2023-06-06 10:38:52.000000 django-all-in-one-accessibility-1.3/accessibility/models.py
+-rw-rw-rw-   0        0        0       63 2023-06-06 10:32:03.000000 django-all-in-one-accessibility-1.3/accessibility/tests.py
+-rw-rw-rw-   0        0        0      162 2023-06-06 10:33:50.000000 django-all-in-one-accessibility-1.3/accessibility/urls.py
+-rw-rw-rw-   0        0        0      239 2023-06-06 10:34:08.000000 django-all-in-one-accessibility-1.3/accessibility/views.py
+drwxrwxrwx   0        0        0        0 2023-06-09 09:51:01.155859 django-all-in-one-accessibility-1.3/aioa_accessibility/
+-rw-rw-rw-   0        0        0        0 2023-06-06 10:30:59.000000 django-all-in-one-accessibility-1.3/aioa_accessibility/__init__.py
+-rw-rw-rw-   0        0        0      429 2023-06-06 10:30:59.000000 django-all-in-one-accessibility-1.3/aioa_accessibility/asgi.py
+-rw-rw-rw-   0        0        0     3349 2023-06-06 10:43:35.000000 django-all-in-one-accessibility-1.3/aioa_accessibility/settings.py
+-rw-rw-rw-   0        0        0      834 2023-06-06 10:32:54.000000 django-all-in-one-accessibility-1.3/aioa_accessibility/urls.py
+-rw-rw-rw-   0        0        0      429 2023-06-06 10:30:59.000000 django-all-in-one-accessibility-1.3/aioa_accessibility/wsgi.py
+drwxrwxrwx   0        0        0        0 2023-06-09 09:51:01.165873 django-all-in-one-accessibility-1.3/django_all_in_one_accessibility.egg-info/
+-rw-rw-rw-   0        0        0     3956 2023-06-09 09:51:01.000000 django-all-in-one-accessibility-1.3/django_all_in_one_accessibility.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      737 2023-06-09 09:51:01.000000 django-all-in-one-accessibility-1.3/django_all_in_one_accessibility.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 09:51:01.000000 django-all-in-one-accessibility-1.3/django_all_in_one_accessibility.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-06-09 09:51:01.000000 django-all-in-one-accessibility-1.3/django_all_in_one_accessibility.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       33 2023-06-09 09:51:01.000000 django-all-in-one-accessibility-1.3/django_all_in_one_accessibility.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1079 2023-06-09 09:49:49.000000 django-all-in-one-accessibility-1.3/pyproject.toml
+-rw-rw-rw-   0        0        0     1032 2023-06-09 09:51:01.170851 django-all-in-one-accessibility-1.3/setup.cfg
+-rw-rw-rw-   0        0        0       37 2023-06-07 04:23:51.000000 django-all-in-one-accessibility-1.3/setup.py
```

### Comparing `django-all-in-one-accessibility-1.2/PKG-INFO` & `django-all-in-one-accessibility-1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-all-in-one-accessibility
-Version: 1.2
+Version: 1.3
 Summary: All in One Accessibility widget makes it easy for users to customize their experience in a single click tap or press of a button
 Home-page: https://www.skynettechnologies.com
 Author: Skynet Technologies USA LLC
 Author-email: Skynet Technologies USA LLC <developer3@skynettechnologies.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -32,15 +32,15 @@
 It uses the accessibility interface which handles UI and design related adjustments. All in One Accessibility app enhances your Django website accessibility to people with hearing or vision impairments, motor impaired, color blind, dyslexia, cognitive & learning impairments, seizure and epileptic, and ADHD problems. It uses the accessibility interface which handles UI and design related adjustments.
 
 [`django-all-in-one-accessibility-introduction`](https://www.youtube.com/watch?v=PPQMWSzroAA) - introduction of All in One Accessibility widget .
 
 ---
 
 ## Installation
--   Run `pip install django-all-in-one-accessibility==1.2`
+-   Run `pip install django-all-in-one-accessibility==1.3`
 -   Add `accessibility` in `settings.INSTALLED_APPS`
 -   Add `accessibility.context_processors.admin_AIOA` in `settings.TEMPLATES context_processors`
 -   Add `<script id="aioa-adawidget" src="{{ AIOA_URL }}"></script>`put this line in your base.html footer
 -   Run `python manage.py migrate`
 -   Run `python manage.py runserver` for Restart your application server
 
 ---
@@ -84,15 +84,15 @@
 ```python
   <footer>
     <script id="aioa-adawidget" src="{{ AIOA_URL }}"></script>
   </footer>
 ```
 
 ### Migrate
-Migrate your app Restart your app with this command
+Migrate your app
 ```python
 python manage.py migrate
 
 ```
 
 ### Restart 
 Restart your app server with this command and check the admin panel the model is ready to use
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-all-in-one-accessibility Version: 1.2
+Metadata-Version: 2.1 Name: django-all-in-one-accessibility Version: 1.3
 Summary: All in One Accessibility widget makes it easy for users to customize
 their experience in a single click tap or press of a button Home-page: https://
 www.skynettechnologies.com Author: Skynet Technologies USA LLC Author-email:
 Skynet Technologies USA LLC
 skynettechnologies.com> Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: Web Environment Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2 Classifier: Intended Audience ::
@@ -23,15 +23,15 @@
 interface which handles UI and design related adjustments. All in One
 Accessibility app enhances your Django website accessibility to people with
 hearing or vision impairments, motor impaired, color blind, dyslexia, cognitive
 & learning impairments, seizure and epileptic, and ADHD problems. It uses the
 accessibility interface which handles UI and design related adjustments.
 [`django-all-in-one-accessibility-introduction`](https://www.youtube.com/
 watch?v=PPQMWSzroAA) - introduction of All in One Accessibility widget . --- ##
-Installation - Run `pip install django-all-in-one-accessibility==1.2` - Add
+Installation - Run `pip install django-all-in-one-accessibility==1.3` - Add
 `accessibility` in `settings.INSTALLED_APPS` - Add
 `accessibility.context_processors.admin_AIOA` in `settings.TEMPLATES
 context_processors` - Add `
 `put this line in your base.html footer - Run `python manage.py migrate` - Run
 `python manage.py runserver` for Restart your application server --- ## Usage
 ### Settings.INSTALLED_APPS Just add `accessibility` in to your
 setting.INSTALLED_APPS: ```python INSTALLED_APPS = [ 'django.contrib.admin',
@@ -42,11 +42,10 @@
 setting.TEMPLATES: ```python TEMPLATES = [ { 'BACKEND':
 'django.template.backends.django.DjangoTemplates', 'DIRS': [], 'APP_DIRS':
 True, 'OPTIONS': { 'context_processors':
 [ 'accessibility.context_processors.admin_AIOA', ], }, }, ] ``` ### Base.html
 Just add this tag in your base.html footer(your main template of django
 website) `
 `: ```python
-  ``` ### Migrate Migrate your app Restart your app with this command ```python
-python manage.py migrate ``` ### Restart Restart your app server with this
-command and check the admin panel the model is ready to use ```python python
-manage.py runserver ```
+  ``` ### Migrate Migrate your app ```python python manage.py migrate ``` ###
+Restart Restart your app server with this command and check the admin panel the
+model is ready to use ```python python manage.py runserver ```
```

### Comparing `django-all-in-one-accessibility-1.2/README.rst` & `django-all-in-one-accessibility-1.3/Readme.md`

 * *Files 3% similar despite different names*

```diff
@@ -3,47 +3,47 @@
 - 2 Minute installation
 - Screen Reader, dynamic widget color and position, supports multiple languages (40 languages)
 - Reduces the risk of time-consuming accessibility lawsuits.
 - Use apps to connect to external services and manage data flows
 
 It uses the accessibility interface which handles UI and design related adjustments. All in One Accessibility app enhances your Django website accessibility to people with hearing or vision impairments, motor impaired, color blind, dyslexia, cognitive & learning impairments, seizure and epileptic, and ADHD problems. It uses the accessibility interface which handles UI and design related adjustments.
 
-[`django-all-in-one-accessibility-introduction`](https://www.youtube.com/watch?v=PPQMWSzroAA) - Introduction of All in One Accessibility widget .
+[`django-all-in-one-accessibility-introduction`](https://www.youtube.com/watch?v=PPQMWSzroAA) - introduction of All in One Accessibility widget .
 
 ---
 
 ## Installation
--   Run `pip install django-all-in-one-accessibility==1.0`
+-   Run `pip install django-all-in-one-accessibility==1.3`
 -   Add `accessibility` in `settings.INSTALLED_APPS`
 -   Add `accessibility.context_processors.admin_AIOA` in `settings.TEMPLATES context_processors`
 -   Add `<script id="aioa-adawidget" src="{{ AIOA_URL }}"></script>`put this line in your base.html footer
 -   Run `python manage.py migrate`
 -   Run `python manage.py runserver` for Restart your application server
 
 ---
 
 ## Usage
 
 ### Settings.INSTALLED_APPS
-Just add accessibility in to your setting.INSTALLED_APPS:
+Just add `accessibility` in to your setting.INSTALLED_APPS:
 
 ```python
 INSTALLED_APPS = [
     'django.contrib.admin',
     'django.contrib.auth',
     'django.contrib.contenttypes',
     'django.contrib.sessions',
     'django.contrib.messages',
     'django.contrib.staticfiles',
     'accessibility',
 ]
 ```
 
 ### Settings.TEMPLATES
-Just add 'accessibility.context_processors.admin_AIOA' in your setting.TEMPLATES:
+Just add `accessibility.context_processors.admin_AIOA` in your setting.TEMPLATES:
 ```python
 TEMPLATES = [
     {
         'BACKEND': 'django.template.backends.django.DjangoTemplates',
         'DIRS': [],
         'APP_DIRS': True,
         'OPTIONS': {
@@ -52,26 +52,28 @@
             ],
         },
     },
 ]
 ```
 
 ### Base.html
-Just add this tag in your base.html footer(your main template of django website) '<script id="aioa-adawidget" src="{{ AIOA_URL }}"></script>':
+Just add this tag in your base.html footer(your main template of django website) `<script id="aioa-adawidget" src="{{ AIOA_URL }}"></script>`:
 ```python
   <footer>
     <script id="aioa-adawidget" src="{{ AIOA_URL }}"></script>
   </footer>
 ```
 
 ### Migrate
-Migrate your app Restart your app with this command
+Migrate your app
 ```python
 python manage.py migrate
 
 ```
 
 ### Restart 
 Restart your app server with this command and check the admin panel the model is ready to use
 ```python
 python manage.py runserver
-```
+```
+
+
```

#### html2text {}

```diff
@@ -7,31 +7,30 @@
 Use apps to connect to external services and manage data flows It uses the
 accessibility interface which handles UI and design related adjustments. All in
 One Accessibility app enhances your Django website accessibility to people with
 hearing or vision impairments, motor impaired, color blind, dyslexia, cognitive
 & learning impairments, seizure and epileptic, and ADHD problems. It uses the
 accessibility interface which handles UI and design related adjustments.
 [`django-all-in-one-accessibility-introduction`](https://www.youtube.com/
-watch?v=PPQMWSzroAA) - Introduction of All in One Accessibility widget . --- ##
-Installation - Run `pip install django-all-in-one-accessibility==1.0` - Add
+watch?v=PPQMWSzroAA) - introduction of All in One Accessibility widget . --- ##
+Installation - Run `pip install django-all-in-one-accessibility==1.3` - Add
 `accessibility` in `settings.INSTALLED_APPS` - Add
 `accessibility.context_processors.admin_AIOA` in `settings.TEMPLATES
 context_processors` - Add `
 `put this line in your base.html footer - Run `python manage.py migrate` - Run
 `python manage.py runserver` for Restart your application server --- ## Usage
-### Settings.INSTALLED_APPS Just add accessibility in to your
+### Settings.INSTALLED_APPS Just add `accessibility` in to your
 setting.INSTALLED_APPS: ```python INSTALLED_APPS = [ 'django.contrib.admin',
 'django.contrib.auth', 'django.contrib.contenttypes',
 'django.contrib.sessions', 'django.contrib.messages',
 'django.contrib.staticfiles', 'accessibility', ] ``` ### Settings.TEMPLATES
-Just add 'accessibility.context_processors.admin_AIOA' in your
+Just add `accessibility.context_processors.admin_AIOA` in your
 setting.TEMPLATES: ```python TEMPLATES = [ { 'BACKEND':
 'django.template.backends.django.DjangoTemplates', 'DIRS': [], 'APP_DIRS':
 True, 'OPTIONS': { 'context_processors':
 [ 'accessibility.context_processors.admin_AIOA', ], }, }, ] ``` ### Base.html
 Just add this tag in your base.html footer(your main template of django
-website) '
-': ```python
-  ``` ### Migrate Migrate your app Restart your app with this command ```python
-python manage.py migrate ``` ### Restart Restart your app server with this
-command and check the admin panel the model is ready to use ```python python
-manage.py runserver ```
+website) `
+`: ```python
+  ``` ### Migrate Migrate your app ```python python manage.py migrate ``` ###
+Restart Restart your app server with this command and check the admin panel the
+model is ready to use ```python python manage.py runserver ```
```

### Comparing `django-all-in-one-accessibility-1.2/accessibility/admin.py` & `django-all-in-one-accessibility-1.3/accessibility/admin.py`

 * *Files identical despite different names*

### Comparing `django-all-in-one-accessibility-1.2/accessibility/context_processors.py` & `django-all-in-one-accessibility-1.3/accessibility/context_processors.py`

 * *Files identical despite different names*

### Comparing `django-all-in-one-accessibility-1.2/accessibility/migrations/0001_initial.py` & `django-all-in-one-accessibility-1.3/accessibility/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-all-in-one-accessibility-1.2/accessibility/models.py` & `django-all-in-one-accessibility-1.3/accessibility/models.py`

 * *Files identical despite different names*

### Comparing `django-all-in-one-accessibility-1.2/aioa_accessibility/settings.py` & `django-all-in-one-accessibility-1.3/aioa_accessibility/settings.py`

 * *Files identical despite different names*

### Comparing `django-all-in-one-accessibility-1.2/aioa_accessibility/urls.py` & `django-all-in-one-accessibility-1.3/aioa_accessibility/urls.py`

 * *Files identical despite different names*

### Comparing `django-all-in-one-accessibility-1.2/django_all_in_one_accessibility.egg-info/PKG-INFO` & `django-all-in-one-accessibility-1.3/django_all_in_one_accessibility.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-all-in-one-accessibility
-Version: 1.2
+Version: 1.3
 Summary: All in One Accessibility widget makes it easy for users to customize their experience in a single click tap or press of a button
 Home-page: https://www.skynettechnologies.com
 Author: Skynet Technologies USA LLC
 Author-email: Skynet Technologies USA LLC <developer3@skynettechnologies.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -32,15 +32,15 @@
 It uses the accessibility interface which handles UI and design related adjustments. All in One Accessibility app enhances your Django website accessibility to people with hearing or vision impairments, motor impaired, color blind, dyslexia, cognitive & learning impairments, seizure and epileptic, and ADHD problems. It uses the accessibility interface which handles UI and design related adjustments.
 
 [`django-all-in-one-accessibility-introduction`](https://www.youtube.com/watch?v=PPQMWSzroAA) - introduction of All in One Accessibility widget .
 
 ---
 
 ## Installation
--   Run `pip install django-all-in-one-accessibility==1.2`
+-   Run `pip install django-all-in-one-accessibility==1.3`
 -   Add `accessibility` in `settings.INSTALLED_APPS`
 -   Add `accessibility.context_processors.admin_AIOA` in `settings.TEMPLATES context_processors`
 -   Add `<script id="aioa-adawidget" src="{{ AIOA_URL }}"></script>`put this line in your base.html footer
 -   Run `python manage.py migrate`
 -   Run `python manage.py runserver` for Restart your application server
 
 ---
@@ -84,15 +84,15 @@
 ```python
   <footer>
     <script id="aioa-adawidget" src="{{ AIOA_URL }}"></script>
   </footer>
 ```
 
 ### Migrate
-Migrate your app Restart your app with this command
+Migrate your app
 ```python
 python manage.py migrate
 
 ```
 
 ### Restart 
 Restart your app server with this command and check the admin panel the model is ready to use
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-all-in-one-accessibility Version: 1.2
+Metadata-Version: 2.1 Name: django-all-in-one-accessibility Version: 1.3
 Summary: All in One Accessibility widget makes it easy for users to customize
 their experience in a single click tap or press of a button Home-page: https://
 www.skynettechnologies.com Author: Skynet Technologies USA LLC Author-email:
 Skynet Technologies USA LLC
 skynettechnologies.com> Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: Web Environment Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2 Classifier: Intended Audience ::
@@ -23,15 +23,15 @@
 interface which handles UI and design related adjustments. All in One
 Accessibility app enhances your Django website accessibility to people with
 hearing or vision impairments, motor impaired, color blind, dyslexia, cognitive
 & learning impairments, seizure and epileptic, and ADHD problems. It uses the
 accessibility interface which handles UI and design related adjustments.
 [`django-all-in-one-accessibility-introduction`](https://www.youtube.com/
 watch?v=PPQMWSzroAA) - introduction of All in One Accessibility widget . --- ##
-Installation - Run `pip install django-all-in-one-accessibility==1.2` - Add
+Installation - Run `pip install django-all-in-one-accessibility==1.3` - Add
 `accessibility` in `settings.INSTALLED_APPS` - Add
 `accessibility.context_processors.admin_AIOA` in `settings.TEMPLATES
 context_processors` - Add `
 `put this line in your base.html footer - Run `python manage.py migrate` - Run
 `python manage.py runserver` for Restart your application server --- ## Usage
 ### Settings.INSTALLED_APPS Just add `accessibility` in to your
 setting.INSTALLED_APPS: ```python INSTALLED_APPS = [ 'django.contrib.admin',
@@ -42,11 +42,10 @@
 setting.TEMPLATES: ```python TEMPLATES = [ { 'BACKEND':
 'django.template.backends.django.DjangoTemplates', 'DIRS': [], 'APP_DIRS':
 True, 'OPTIONS': { 'context_processors':
 [ 'accessibility.context_processors.admin_AIOA', ], }, }, ] ``` ### Base.html
 Just add this tag in your base.html footer(your main template of django
 website) `
 `: ```python
-  ``` ### Migrate Migrate your app Restart your app with this command ```python
-python manage.py migrate ``` ### Restart Restart your app server with this
-command and check the admin panel the model is ready to use ```python python
-manage.py runserver ```
+  ``` ### Migrate Migrate your app ```python python manage.py migrate ``` ###
+Restart Restart your app server with this command and check the admin panel the
+model is ready to use ```python python manage.py runserver ```
```

### Comparing `django-all-in-one-accessibility-1.2/django_all_in_one_accessibility.egg-info/SOURCES.txt` & `django-all-in-one-accessibility-1.3/django_all_in_one_accessibility.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-README.rst
 Readme.md
 pyproject.toml
 setup.cfg
 setup.py
 accessibility/__init__.py
 accessibility/admin.py
 accessibility/apps.py
```

### Comparing `django-all-in-one-accessibility-1.2/pyproject.toml` & `django-all-in-one-accessibility-1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "django-all-in-one-accessibility"
-version = "1.2"
+version = "1.3"
 authors = [
   { name="Skynet Technologies USA LLC", email="developer3@skynettechnologies.com" },
 ]
 description = "All in One Accessibility widget makes it easy for users to customize their experience in a single click tap or press of a button"
 readme = "Readme.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `django-all-in-one-accessibility-1.2/setup.cfg` & `django-all-in-one-accessibility-1.3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2064 6a61 6e67 6f2d 616c 6c2d 696e   = django-all-in
 00000020: 2d6f 6e65 2d61 6363 6573 7369 6269 6c69  -one-accessibili
 00000030: 7479 0d0a 7665 7273 696f 6e20 3d20 312e  ty..version = 1.
-00000040: 300d 0a64 6573 6372 6970 7469 6f6e 203d  0..description =
+00000040: 330d 0a64 6573 6372 6970 7469 6f6e 203d  3..description =
 00000050: 2041 2044 6a61 6e67 6f20 4170 7020 6261   A Django App ba
 00000060: 7365 6420 6f6e 2061 7373 6973 7469 7665  sed on assistive
 00000070: 2074 6563 686e 6f6c 6f67 7920 7468 6174   technology that
 00000080: 2068 656c 7073 206f 7267 616e 697a 6174   helps organizat
 00000090: 696f 6e73 2065 6e68 616e 6365 2074 6865  ions enhance the
 000000a0: 2061 6363 6573 7369 6269 6c69 7479 2061   accessibility a
 000000b0: 6e64 2075 7361 6269 6c69 7479 206f 6620  nd usability of
```

