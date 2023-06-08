# Comparing `tmp/django-theme-academy-0.3.8.tar.gz` & `tmp/django-theme-academy-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-theme-academy-0.3.8.tar", last modified: Tue May 30 18:58:22 2023, max compression
+gzip compressed data, was "django-theme-academy-0.3.9.tar", last modified: Thu Jun  8 23:22:36 2023, max compression
```

## Comparing `django-theme-academy-0.3.8.tar` & `django-theme-academy-0.3.9.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 glenn      (504) admin       (80)        0 2023-05-30 18:58:22.822860 django-theme-academy-0.3.8/
--rw-r--r--   0 glenn      (504) admin       (80)     1458 2022-11-18 23:00:44.000000 django-theme-academy-0.3.8/LICENSE.txt
--rw-r--r--   0 glenn      (504) admin       (80)      151 2023-02-01 18:15:07.000000 django-theme-academy-0.3.8/MANIFEST.in
--rw-r--r--   0 glenn      (504) admin       (80)     6432 2023-05-30 18:58:22.822909 django-theme-academy-0.3.8/PKG-INFO
--rw-r--r--   0 glenn      (504) admin       (80)     5533 2023-05-17 18:37:12.000000 django-theme-academy-0.3.8/README.md
-drwxr-xr-x   0 glenn      (504) admin       (80)        0 2023-05-30 18:58:22.818280 django-theme-academy-0.3.8/academy_theme/
--rw-r--r--   0 glenn      (504) admin       (80)       22 2023-05-30 18:57:37.000000 django-theme-academy-0.3.8/academy_theme/__init__.py
--rw-r--r--   0 glenn      (504) admin       (80)      130 2022-11-18 23:00:44.000000 django-theme-academy-0.3.8/academy_theme/apps.py
--rw-r--r--   0 glenn      (504) admin       (80)     1496 2023-02-01 18:15:07.000000 django-theme-academy-0.3.8/academy_theme/context_processors.py
--rw-r--r--   0 glenn      (504) admin       (80)        0 2022-11-18 23:00:44.000000 django-theme-academy-0.3.8/academy_theme/models.py
--rw-r--r--   0 glenn      (504) admin       (80)        0 2022-11-18 23:00:44.000000 django-theme-academy-0.3.8/academy_theme/py.typed
-drwxr-xr-x   0 glenn      (504) admin       (80)        0 2023-05-30 18:58:22.816176 django-theme-academy-0.3.8/academy_theme/static/
-drwxr-xr-x   0 glenn      (504) admin       (80)        0 2023-05-30 18:58:22.816384 django-theme-academy-0.3.8/academy_theme/static/academy_theme/
-drwxr-xr-x   0 glenn      (504) admin       (80)        0 2023-05-30 18:58:22.819496 django-theme-academy-0.3.8/academy_theme/static/academy_theme/css/
--rw-r--r--   0 glenn      (504) admin       (80)     3451 2023-02-01 18:15:07.000000 django-theme-academy-0.3.8/academy_theme/static/academy_theme/css/_globals.scss
--rw-r--r--   0 glenn      (504) admin       (80)     3618 2022-11-18 23:00:44.000000 django-theme-academy-0.3.8/academy_theme/static/academy_theme/css/_mixins.scss
--rw-r--r--   0 glenn      (504) admin       (80)      711 2023-02-01 18:15:07.000000 django-theme-academy-0.3.8/academy_theme/static/academy_theme/css/_page.scss
--rw-r--r--   0 glenn      (504) admin       (80)     1105 2022-11-18 23:00:44.000000 django-theme-academy-0.3.8/academy_theme/static/academy_theme/css/_ribbon.scss
-drwxr-xr-x   0 glenn      (504) admin       (80)        0 2023-05-30 18:58:22.819879 django-theme-academy-0.3.8/academy_theme/static/academy_theme/css/boostrap-5.1.3/
--rw-r--r--   0 glenn      (504) admin       (80)     4484 2022-11-18 23:00:44.000000 django-theme-academy-0.3.8/academy_theme/static/academy_theme/css/boostrap-5.1.3/_breakpoints.scss
--rw-r--r--   0 glenn      (504) admin       (80)    10621 2022-11-18 23:00:44.000000 django-theme-academy-0.3.8/academy_theme/static/academy_theme/css/boostrap-5.1.3/_functions.scss
--rw-r--r--   0 glenn      (504) admin       (80)    67864 2022-11-18 23:00:44.000000 django-theme-academy-0.3.8/academy_theme/static/academy_theme/css/boostrap-5.1.3/_variables.scss
--rw-r--r--   0 glenn      (504) admin       (80)     7542 2022-11-19 23:57:54.000000 django-theme-academy-0.3.8/academy_theme/static/academy_theme/css/theme.css
--rw-r--r--   0 glenn      (504) admin       (80)     3009 2022-11-18 23:00:44.000000 django-theme-academy-0.3.8/academy_theme/static/academy_theme/css/theme.css.map
--rw-r--r--   0 glenn      (504) admin       (80)      315 2022-11-18 23:00:44.000000 django-theme-academy-0.3.8/academy_theme/static/academy_theme/css/theme.scss
-drwxr-xr-x   0 glenn      (504) admin       (80)        0 2023-05-30 18:58:22.821376 django-theme-academy-0.3.8/academy_theme/static/academy_theme/images/
--rw-r--r--   0 glenn      (504) admin       (80)    11518 2022-11-18 23:00:44.000000 django-theme-academy-0.3.8/academy_theme/static/academy_theme/images/android-chrome-192x192.png
--rw-r--r--   0 glenn      (504) admin       (80)    30901 2022-11-18 23:00:44.000000 django-theme-academy-0.3.8/academy_theme/static/academy_theme/images/android-chrome-512x512.png
--rw-r--r--   0 glenn      (504) admin       (80)    10286 2022-11-18 23:00:44.000000 django-theme-academy-0.3.8/academy_theme/static/academy_theme/images/apple-touch-icon.png
--rw-r--r--   0 glenn      (504) admin       (80)      624 2022-11-18 23:00:44.000000 django-theme-academy-0.3.8/academy_theme/static/academy_theme/images/favicon-16x16.png
--rw-r--r--   0 glenn      (504) admin       (80)     1425 2022-11-18 23:00:44.000000 django-theme-academy-0.3.8/academy_theme/static/academy_theme/images/favicon-32x32.png
--rw-r--r--   0 glenn      (504) admin       (80)    15406 2022-11-18 23:00:44.000000 django-theme-academy-0.3.8/academy_theme/static/academy_theme/images/favicon.ico
--rw-r--r--   0 glenn      (504) admin       (80)   135992 2022-11-18 23:00:44.000000 django-theme-academy-0.3.8/academy_theme/static/academy_theme/images/logo.png
--rw-r--r--   0 glenn      (504) admin       (80)    15629 2022-11-18 23:00:44.000000 django-theme-academy-0.3.8/academy_theme/static/academy_theme/images/logo.svg
--rw-r--r--   0 glenn      (504) admin       (80)      263 2022-11-18 23:00:44.000000 django-theme-academy-0.3.8/academy_theme/static/academy_theme/images/site.webmanifest
-drwxr-xr-x   0 glenn      (504) admin       (80)        0 2023-05-30 18:58:22.821590 django-theme-academy-0.3.8/academy_theme/static/academy_theme/js/
--rw-r--r--   0 glenn      (504) admin       (80)      173 2022-11-18 23:00:44.000000 django-theme-academy-0.3.8/academy_theme/static/academy_theme/js/theme.js
-drwxr-xr-x   0 glenn      (504) admin       (80)        0 2023-05-30 18:58:22.816478 django-theme-academy-0.3.8/academy_theme/templates/
-drwxr-xr-x   0 glenn      (504) admin       (80)        0 2023-05-30 18:58:22.821892 django-theme-academy-0.3.8/academy_theme/templates/academy_theme/
--rw-r--r--   0 glenn      (504) admin       (80)     1271 2023-02-01 18:15:07.000000 django-theme-academy-0.3.8/academy_theme/templates/academy_theme/base--wildewidgets.html
--rw-r--r--   0 glenn      (504) admin       (80)     5507 2023-05-30 18:57:10.000000 django-theme-academy-0.3.8/academy_theme/templates/academy_theme/base.html
-drwxr-xr-x   0 glenn      (504) admin       (80)        0 2023-05-30 18:58:22.821998 django-theme-academy-0.3.8/academy_theme/templates/academy_theme/templatetags/
--rw-r--r--   0 glenn      (504) admin       (80)      153 2022-11-18 23:00:44.000000 django-theme-academy-0.3.8/academy_theme/templates/academy_theme/templatetags/breadcrumb.html
-drwxr-xr-x   0 glenn      (504) admin       (80)        0 2023-05-30 18:58:22.822201 django-theme-academy-0.3.8/academy_theme/templatetags/
--rw-r--r--   0 glenn      (504) admin       (80)        0 2022-11-18 23:00:44.000000 django-theme-academy-0.3.8/academy_theme/templatetags/__init__.py
--rw-r--r--   0 glenn      (504) admin       (80)      666 2022-11-18 23:00:44.000000 django-theme-academy-0.3.8/academy_theme/templatetags/academy_theme.py
--rw-r--r--   0 glenn      (504) admin       (80)        0 2022-11-18 23:00:44.000000 django-theme-academy-0.3.8/academy_theme/urls.py
--rw-r--r--   0 glenn      (504) admin       (80)        0 2022-11-18 23:00:44.000000 django-theme-academy-0.3.8/academy_theme/views.py
--rw-r--r--   0 glenn      (504) admin       (80)     1381 2023-05-17 18:37:12.000000 django-theme-academy-0.3.8/academy_theme/wildewidgets.py
-drwxr-xr-x   0 glenn      (504) admin       (80)        0 2023-05-30 18:58:22.822752 django-theme-academy-0.3.8/django_theme_academy.egg-info/
--rw-r--r--   0 glenn      (504) admin       (80)     6432 2023-05-30 18:58:22.000000 django-theme-academy-0.3.8/django_theme_academy.egg-info/PKG-INFO
--rw-r--r--   0 glenn      (504) admin       (80)     1891 2023-05-30 18:58:22.000000 django-theme-academy-0.3.8/django_theme_academy.egg-info/SOURCES.txt
--rw-r--r--   0 glenn      (504) admin       (80)        1 2023-05-30 18:58:22.000000 django-theme-academy-0.3.8/django_theme_academy.egg-info/dependency_links.txt
--rw-r--r--   0 glenn      (504) admin       (80)       29 2023-05-30 18:58:22.000000 django-theme-academy-0.3.8/django_theme_academy.egg-info/requires.txt
--rw-r--r--   0 glenn      (504) admin       (80)       14 2023-05-30 18:58:22.000000 django-theme-academy-0.3.8/django_theme_academy.egg-info/top_level.txt
--rw-r--r--   0 glenn      (504) admin       (80)      796 2023-05-30 18:58:22.823167 django-theme-academy-0.3.8/setup.cfg
--rw-r--r--   0 glenn      (504) admin       (80)     1278 2023-05-30 18:57:37.000000 django-theme-academy-0.3.8/setup.py
+drwxr-xr-x   0 glenn      (504) admin       (80)        0 2023-06-08 23:22:36.078962 django-theme-academy-0.3.9/
+-rw-r--r--   0 glenn      (504) admin       (80)     1458 2022-11-18 23:00:44.000000 django-theme-academy-0.3.9/LICENSE.txt
+-rw-r--r--   0 glenn      (504) admin       (80)      151 2023-02-01 18:15:07.000000 django-theme-academy-0.3.9/MANIFEST.in
+-rw-r--r--   0 glenn      (504) admin       (80)     6432 2023-06-08 23:22:36.079051 django-theme-academy-0.3.9/PKG-INFO
+-rw-r--r--   0 glenn      (504) admin       (80)     5533 2023-05-17 18:37:12.000000 django-theme-academy-0.3.9/README.md
+drwxr-xr-x   0 glenn      (504) admin       (80)        0 2023-06-08 23:22:36.074755 django-theme-academy-0.3.9/academy_theme/
+-rw-r--r--   0 glenn      (504) admin       (80)       22 2023-06-08 23:21:53.000000 django-theme-academy-0.3.9/academy_theme/__init__.py
+-rw-r--r--   0 glenn      (504) admin       (80)      130 2022-11-18 23:00:44.000000 django-theme-academy-0.3.9/academy_theme/apps.py
+-rw-r--r--   0 glenn      (504) admin       (80)     1496 2023-02-01 18:15:07.000000 django-theme-academy-0.3.9/academy_theme/context_processors.py
+-rw-r--r--   0 glenn      (504) admin       (80)        0 2022-11-18 23:00:44.000000 django-theme-academy-0.3.9/academy_theme/models.py
+-rw-r--r--   0 glenn      (504) admin       (80)        0 2022-11-18 23:00:44.000000 django-theme-academy-0.3.9/academy_theme/py.typed
+drwxr-xr-x   0 glenn      (504) admin       (80)        0 2023-06-08 23:22:36.072970 django-theme-academy-0.3.9/academy_theme/static/
+drwxr-xr-x   0 glenn      (504) admin       (80)        0 2023-06-08 23:22:36.073184 django-theme-academy-0.3.9/academy_theme/static/academy_theme/
+drwxr-xr-x   0 glenn      (504) admin       (80)        0 2023-06-08 23:22:36.075860 django-theme-academy-0.3.9/academy_theme/static/academy_theme/css/
+-rw-r--r--   0 glenn      (504) admin       (80)     3451 2023-02-01 18:15:07.000000 django-theme-academy-0.3.9/academy_theme/static/academy_theme/css/_globals.scss
+-rw-r--r--   0 glenn      (504) admin       (80)     3583 2023-06-08 22:52:44.000000 django-theme-academy-0.3.9/academy_theme/static/academy_theme/css/_mixins.scss
+-rw-r--r--   0 glenn      (504) admin       (80)      645 2023-06-08 23:07:21.000000 django-theme-academy-0.3.9/academy_theme/static/academy_theme/css/_page.scss
+-rw-r--r--   0 glenn      (504) admin       (80)     1105 2022-11-18 23:00:44.000000 django-theme-academy-0.3.9/academy_theme/static/academy_theme/css/_ribbon.scss
+drwxr-xr-x   0 glenn      (504) admin       (80)        0 2023-06-08 23:22:36.076350 django-theme-academy-0.3.9/academy_theme/static/academy_theme/css/boostrap-5.1.3/
+-rw-r--r--   0 glenn      (504) admin       (80)     4484 2022-11-18 23:00:44.000000 django-theme-academy-0.3.9/academy_theme/static/academy_theme/css/boostrap-5.1.3/_breakpoints.scss
+-rw-r--r--   0 glenn      (504) admin       (80)    10621 2022-11-18 23:00:44.000000 django-theme-academy-0.3.9/academy_theme/static/academy_theme/css/boostrap-5.1.3/_functions.scss
+-rw-r--r--   0 glenn      (504) admin       (80)    67864 2022-11-18 23:00:44.000000 django-theme-academy-0.3.9/academy_theme/static/academy_theme/css/boostrap-5.1.3/_variables.scss
+-rw-r--r--   0 glenn      (504) admin       (80)     7484 2023-06-08 23:06:32.000000 django-theme-academy-0.3.9/academy_theme/static/academy_theme/css/theme.css
+-rw-r--r--   0 glenn      (504) admin       (80)     3009 2022-11-18 23:00:44.000000 django-theme-academy-0.3.9/academy_theme/static/academy_theme/css/theme.css.map
+-rw-r--r--   0 glenn      (504) admin       (80)      315 2022-11-18 23:00:44.000000 django-theme-academy-0.3.9/academy_theme/static/academy_theme/css/theme.scss
+drwxr-xr-x   0 glenn      (504) admin       (80)        0 2023-06-08 23:22:36.077554 django-theme-academy-0.3.9/academy_theme/static/academy_theme/images/
+-rw-r--r--   0 glenn      (504) admin       (80)    11518 2022-11-18 23:00:44.000000 django-theme-academy-0.3.9/academy_theme/static/academy_theme/images/android-chrome-192x192.png
+-rw-r--r--   0 glenn      (504) admin       (80)    30901 2022-11-18 23:00:44.000000 django-theme-academy-0.3.9/academy_theme/static/academy_theme/images/android-chrome-512x512.png
+-rw-r--r--   0 glenn      (504) admin       (80)    10286 2022-11-18 23:00:44.000000 django-theme-academy-0.3.9/academy_theme/static/academy_theme/images/apple-touch-icon.png
+-rw-r--r--   0 glenn      (504) admin       (80)      624 2022-11-18 23:00:44.000000 django-theme-academy-0.3.9/academy_theme/static/academy_theme/images/favicon-16x16.png
+-rw-r--r--   0 glenn      (504) admin       (80)     1425 2022-11-18 23:00:44.000000 django-theme-academy-0.3.9/academy_theme/static/academy_theme/images/favicon-32x32.png
+-rw-r--r--   0 glenn      (504) admin       (80)    15406 2022-11-18 23:00:44.000000 django-theme-academy-0.3.9/academy_theme/static/academy_theme/images/favicon.ico
+-rw-r--r--   0 glenn      (504) admin       (80)   135992 2022-11-18 23:00:44.000000 django-theme-academy-0.3.9/academy_theme/static/academy_theme/images/logo.png
+-rw-r--r--   0 glenn      (504) admin       (80)    15629 2022-11-18 23:00:44.000000 django-theme-academy-0.3.9/academy_theme/static/academy_theme/images/logo.svg
+-rw-r--r--   0 glenn      (504) admin       (80)      263 2022-11-18 23:00:44.000000 django-theme-academy-0.3.9/academy_theme/static/academy_theme/images/site.webmanifest
+drwxr-xr-x   0 glenn      (504) admin       (80)        0 2023-06-08 23:22:36.077654 django-theme-academy-0.3.9/academy_theme/static/academy_theme/js/
+-rw-r--r--   0 glenn      (504) admin       (80)      173 2022-11-18 23:00:44.000000 django-theme-academy-0.3.9/academy_theme/static/academy_theme/js/theme.js
+drwxr-xr-x   0 glenn      (504) admin       (80)        0 2023-06-08 23:22:36.073277 django-theme-academy-0.3.9/academy_theme/templates/
+drwxr-xr-x   0 glenn      (504) admin       (80)        0 2023-06-08 23:22:36.077918 django-theme-academy-0.3.9/academy_theme/templates/academy_theme/
+-rw-r--r--   0 glenn      (504) admin       (80)     1271 2023-02-01 18:15:07.000000 django-theme-academy-0.3.9/academy_theme/templates/academy_theme/base--wildewidgets.html
+-rw-r--r--   0 glenn      (504) admin       (80)     5507 2023-05-30 18:57:10.000000 django-theme-academy-0.3.9/academy_theme/templates/academy_theme/base.html
+drwxr-xr-x   0 glenn      (504) admin       (80)        0 2023-06-08 23:22:36.078040 django-theme-academy-0.3.9/academy_theme/templates/academy_theme/templatetags/
+-rw-r--r--   0 glenn      (504) admin       (80)      153 2022-11-18 23:00:44.000000 django-theme-academy-0.3.9/academy_theme/templates/academy_theme/templatetags/breadcrumb.html
+drwxr-xr-x   0 glenn      (504) admin       (80)        0 2023-06-08 23:22:36.078250 django-theme-academy-0.3.9/academy_theme/templatetags/
+-rw-r--r--   0 glenn      (504) admin       (80)        0 2022-11-18 23:00:44.000000 django-theme-academy-0.3.9/academy_theme/templatetags/__init__.py
+-rw-r--r--   0 glenn      (504) admin       (80)      666 2022-11-18 23:00:44.000000 django-theme-academy-0.3.9/academy_theme/templatetags/academy_theme.py
+-rw-r--r--   0 glenn      (504) admin       (80)        0 2022-11-18 23:00:44.000000 django-theme-academy-0.3.9/academy_theme/urls.py
+-rw-r--r--   0 glenn      (504) admin       (80)        0 2022-11-18 23:00:44.000000 django-theme-academy-0.3.9/academy_theme/views.py
+-rw-r--r--   0 glenn      (504) admin       (80)     1381 2023-05-17 18:37:12.000000 django-theme-academy-0.3.9/academy_theme/wildewidgets.py
+drwxr-xr-x   0 glenn      (504) admin       (80)        0 2023-06-08 23:22:36.078846 django-theme-academy-0.3.9/django_theme_academy.egg-info/
+-rw-r--r--   0 glenn      (504) admin       (80)     6432 2023-06-08 23:22:36.000000 django-theme-academy-0.3.9/django_theme_academy.egg-info/PKG-INFO
+-rw-r--r--   0 glenn      (504) admin       (80)     1891 2023-06-08 23:22:36.000000 django-theme-academy-0.3.9/django_theme_academy.egg-info/SOURCES.txt
+-rw-r--r--   0 glenn      (504) admin       (80)        1 2023-06-08 23:22:36.000000 django-theme-academy-0.3.9/django_theme_academy.egg-info/dependency_links.txt
+-rw-r--r--   0 glenn      (504) admin       (80)       29 2023-06-08 23:22:36.000000 django-theme-academy-0.3.9/django_theme_academy.egg-info/requires.txt
+-rw-r--r--   0 glenn      (504) admin       (80)       14 2023-06-08 23:22:36.000000 django-theme-academy-0.3.9/django_theme_academy.egg-info/top_level.txt
+-rw-r--r--   0 glenn      (504) admin       (80)      796 2023-06-08 23:22:36.079351 django-theme-academy-0.3.9/setup.cfg
+-rw-r--r--   0 glenn      (504) admin       (80)     1278 2023-06-08 23:21:53.000000 django-theme-academy-0.3.9/setup.py
```

### Comparing `django-theme-academy-0.3.8/LICENSE.txt` & `django-theme-academy-0.3.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-theme-academy-0.3.8/PKG-INFO` & `django-theme-academy-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-theme-academy
-Version: 0.3.8
+Version: 0.3.9
 Summary: A Tabler-based, fixed left sidebar django theme.
 Home-page: https://github.com/caltechads/django-theme-academy
 Author: Caltech IMSS ADS
 Author-email: imss-ads-staff@caltech.edu
 Keywords: django
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `django-theme-academy-0.3.8/README.md` & `django-theme-academy-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `django-theme-academy-0.3.8/academy_theme/context_processors.py` & `django-theme-academy-0.3.9/academy_theme/context_processors.py`

 * *Files identical despite different names*

### Comparing `django-theme-academy-0.3.8/academy_theme/static/academy_theme/css/_globals.scss` & `django-theme-academy-0.3.9/academy_theme/static/academy_theme/css/_globals.scss`

 * *Files identical despite different names*

### Comparing `django-theme-academy-0.3.8/academy_theme/static/academy_theme/css/_mixins.scss` & `django-theme-academy-0.3.9/academy_theme/static/academy_theme/css/_mixins.scss`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 
 */
 
 @mixin all-caps-horizontal-links() {
   margin: 0;
   font-size: 0.8em;
   a, a:visited {
-    color: $color-white!important;
     text-transform: uppercase;
     font-weight: bold;
   }
   li {
     display: inline-block;
     padding-left: 1.25em;
     &:first-child {
```

### Comparing `django-theme-academy-0.3.8/academy_theme/static/academy_theme/css/_page.scss` & `django-theme-academy-0.3.9/academy_theme/static/academy_theme/css/_page.scss`

 * *Files 15% similar despite different names*

```diff
@@ -29,13 +29,9 @@
     &__contact {
       line-height: 1.4;
       color: $color-black-text;
       a, a:visited {
         color: $color-black-text;
       }
     }
-
-    &__links {
-      @include all-caps-horizontal-links();
-    }
   }
 }
```

### Comparing `django-theme-academy-0.3.8/academy_theme/static/academy_theme/css/_ribbon.scss` & `django-theme-academy-0.3.9/academy_theme/static/academy_theme/css/_ribbon.scss`

 * *Files identical despite different names*

### Comparing `django-theme-academy-0.3.8/academy_theme/static/academy_theme/css/boostrap-5.1.3/_breakpoints.scss` & `django-theme-academy-0.3.9/academy_theme/static/academy_theme/css/boostrap-5.1.3/_breakpoints.scss`

 * *Files identical despite different names*

### Comparing `django-theme-academy-0.3.8/academy_theme/static/academy_theme/css/boostrap-5.1.3/_functions.scss` & `django-theme-academy-0.3.9/academy_theme/static/academy_theme/css/boostrap-5.1.3/_functions.scss`

 * *Files identical despite different names*

### Comparing `django-theme-academy-0.3.8/academy_theme/static/academy_theme/css/boostrap-5.1.3/_variables.scss` & `django-theme-academy-0.3.9/academy_theme/static/academy_theme/css/boostrap-5.1.3/_variables.scss`

 * *Files identical despite different names*

### Comparing `django-theme-academy-0.3.8/academy_theme/static/academy_theme/css/theme.css` & `django-theme-academy-0.3.9/academy_theme/static/academy_theme/css/theme.css`

 * *Files 2% similar despite different names*

```diff
@@ -366,15 +366,14 @@
 }
 .ribbon_bar__content__links {
   margin: 0;
   font-size: 0.8em;
   font-size: 0.78571429em;
 }
 .ribbon_bar__content__links a, .ribbon_bar__content__links a:visited {
-  color: #ffffff !important;
   text-transform: uppercase;
   font-weight: bold;
 }
 .ribbon_bar__content__links li {
   display: inline-block;
   padding-left: 1.25em;
 }
@@ -431,15 +430,14 @@
   color: #333333;
 }
 .footer__content__links {
   margin: 0;
   font-size: 0.8em;
 }
 .footer__content__links a, .footer__content__links a:visited {
-  color: #ffffff !important;
   text-transform: uppercase;
   font-weight: bold;
 }
 .footer__content__links li {
   display: inline-block;
   padding-left: 1.25em;
 }
```

### Comparing `django-theme-academy-0.3.8/academy_theme/static/academy_theme/css/theme.css.map` & `django-theme-academy-0.3.9/academy_theme/static/academy_theme/css/theme.css.map`

 * *Files identical despite different names*

### Comparing `django-theme-academy-0.3.8/academy_theme/static/academy_theme/images/android-chrome-192x192.png` & `django-theme-academy-0.3.9/academy_theme/static/academy_theme/images/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `django-theme-academy-0.3.8/academy_theme/static/academy_theme/images/android-chrome-512x512.png` & `django-theme-academy-0.3.9/academy_theme/static/academy_theme/images/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `django-theme-academy-0.3.8/academy_theme/static/academy_theme/images/apple-touch-icon.png` & `django-theme-academy-0.3.9/academy_theme/static/academy_theme/images/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `django-theme-academy-0.3.8/academy_theme/static/academy_theme/images/favicon-16x16.png` & `django-theme-academy-0.3.9/academy_theme/static/academy_theme/images/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `django-theme-academy-0.3.8/academy_theme/static/academy_theme/images/favicon-32x32.png` & `django-theme-academy-0.3.9/academy_theme/static/academy_theme/images/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `django-theme-academy-0.3.8/academy_theme/static/academy_theme/images/favicon.ico` & `django-theme-academy-0.3.9/academy_theme/static/academy_theme/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `django-theme-academy-0.3.8/academy_theme/static/academy_theme/images/logo.png` & `django-theme-academy-0.3.9/academy_theme/static/academy_theme/images/logo.png`

 * *Files identical despite different names*

### Comparing `django-theme-academy-0.3.8/academy_theme/static/academy_theme/images/logo.svg` & `django-theme-academy-0.3.9/academy_theme/static/academy_theme/images/logo.svg`

 * *Files identical despite different names*

### Comparing `django-theme-academy-0.3.8/academy_theme/templates/academy_theme/base--wildewidgets.html` & `django-theme-academy-0.3.9/academy_theme/templates/academy_theme/base--wildewidgets.html`

 * *Files identical despite different names*

### Comparing `django-theme-academy-0.3.8/academy_theme/templates/academy_theme/base.html` & `django-theme-academy-0.3.9/academy_theme/templates/academy_theme/base.html`

 * *Files identical despite different names*

### Comparing `django-theme-academy-0.3.8/academy_theme/templatetags/academy_theme.py` & `django-theme-academy-0.3.9/academy_theme/templatetags/academy_theme.py`

 * *Files identical despite different names*

### Comparing `django-theme-academy-0.3.8/academy_theme/wildewidgets.py` & `django-theme-academy-0.3.9/academy_theme/wildewidgets.py`

 * *Files identical despite different names*

### Comparing `django-theme-academy-0.3.8/django_theme_academy.egg-info/PKG-INFO` & `django-theme-academy-0.3.9/django_theme_academy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-theme-academy
-Version: 0.3.8
+Version: 0.3.9
 Summary: A Tabler-based, fixed left sidebar django theme.
 Home-page: https://github.com/caltechads/django-theme-academy
 Author: Caltech IMSS ADS
 Author-email: imss-ads-staff@caltech.edu
 Keywords: django
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `django-theme-academy-0.3.8/django_theme_academy.egg-info/SOURCES.txt` & `django-theme-academy-0.3.9/django_theme_academy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-theme-academy-0.3.8/setup.cfg` & `django-theme-academy-0.3.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `django-theme-academy-0.3.8/setup.py` & `django-theme-academy-0.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="django-theme-academy",
-    version="0.3.8",
+    version="0.3.9",
     packages=find_packages(),
     include_package_data=True,
     package_data={'academy_theme': ["py.typed"]},
     install_requires=[
         "django-wildewidgets >= 0.13.49"
     ],
     author="Caltech IMSS ADS",
```

