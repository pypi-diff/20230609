# Comparing `tmp/sakyum-0.0.7.tar.gz` & `tmp/sakyum-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sakyum-0.0.7.tar", last modified: Tue Apr  4 00:47:59 2023, max compression
+gzip compressed data, was "sakyum-0.0.8.tar", last modified: Fri Jun  9 17:49:34 2023, max compression
```

## Comparing `sakyum-0.0.7.tar` & `sakyum-0.0.8.tar`

### file list

```diff
@@ -1,68 +1,70 @@
-drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-04-04 00:47:59.336402 sakyum-0.0.7/
--rw-rw-r--   0 usman     (1000) usman     (1000)     1166 2023-04-04 00:44:37.000000 sakyum-0.0.7/CHANGELOG
--rw-rw-r--   0 usman     (1000) usman     (1000)     1077 2023-03-20 02:44:09.000000 sakyum-0.0.7/LICENSE
--rw-rw-r--   0 usman     (1000) usman     (1000)       82 2023-03-20 02:44:09.000000 sakyum-0.0.7/MANIFEST.in
--rw-rw-r--   0 usman     (1000) usman     (1000)     5944 2023-04-04 00:47:59.336402 sakyum-0.0.7/PKG-INFO
--rw-rw-r--   0 usman     (1000) usman     (1000)     2918 2023-04-04 00:45:56.000000 sakyum-0.0.7/README.md
--rw-rw-r--   0 usman     (1000) usman     (1000)      398 2023-03-27 02:17:42.000000 sakyum-0.0.7/requirements.txt
-drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-04-04 00:47:59.104292 sakyum-0.0.7/sakyum/
--rw-rw-r--   0 usman     (1000) usman     (1000)      729 2023-04-04 00:44:38.000000 sakyum-0.0.7/sakyum/__init__.py
--rw-rw-r--   0 usman     (1000) usman     (1000)      489 2023-03-20 02:44:11.000000 sakyum-0.0.7/sakyum/api.py
-drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-04-04 00:47:59.192334 sakyum-0.0.7/sakyum/auth/
--rw-rw-r--   0 usman     (1000) usman     (1000)       93 2023-03-27 01:38:36.000000 sakyum-0.0.7/sakyum/auth/__init__.py
--rw-rw-r--   0 usman     (1000) usman     (1000)     1342 2023-04-04 00:44:38.000000 sakyum-0.0.7/sakyum/auth/admin.py
--rw-rw-r--   0 usman     (1000) usman     (1000)     1687 2023-03-27 01:38:36.000000 sakyum-0.0.7/sakyum/auth/forms.py
--rw-rw-r--   0 usman     (1000) usman     (1000)     1320 2023-03-27 01:38:36.000000 sakyum-0.0.7/sakyum/auth/models.py
--rw-rw-r--   0 usman     (1000) usman     (1000)     6007 2023-03-27 01:38:36.000000 sakyum-0.0.7/sakyum/auth/routes.py
--rw-rw-r--   0 usman     (1000) usman     (1000)    20077 2023-03-27 01:38:36.000000 sakyum-0.0.7/sakyum/base.py
--rw-rw-r--   0 usman     (1000) usman     (1000)     4725 2023-03-27 01:38:36.000000 sakyum-0.0.7/sakyum/blueprint.py
-drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-04-04 00:47:59.196336 sakyum-0.0.7/sakyum/contrib/
--rw-rw-r--   0 usman     (1000) usman     (1000)      594 2023-03-27 01:38:36.000000 sakyum-0.0.7/sakyum/contrib/__init__.py
--rw-rw-r--   0 usman     (1000) usman     (1000)      451 2023-03-27 01:38:36.000000 sakyum-0.0.7/sakyum/database.py
-drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-04-04 00:47:59.232353 sakyum-0.0.7/sakyum/mute/
--rw-rw-r--   0 usman     (1000) usman     (1000)      584 2023-03-27 01:38:36.000000 sakyum-0.0.7/sakyum/mute/__init__.py
--rw-rw-r--   0 usman     (1000) usman     (1000)     1514 2023-03-27 01:38:36.000000 sakyum-0.0.7/sakyum/mute/app.py
--rw-rw-r--   0 usman     (1000) usman     (1000)     2899 2023-03-27 01:38:36.000000 sakyum-0.0.7/sakyum/mute/page.py
--rw-rw-r--   0 usman     (1000) usman     (1000)     3155 2023-03-27 01:38:36.000000 sakyum-0.0.7/sakyum/mute/project.py
-drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-04-04 00:47:59.232353 sakyum-0.0.7/sakyum/static/
-drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-04-04 00:47:58.988238 sakyum-0.0.7/sakyum/static/default_style/
-drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-04-04 00:47:59.236355 sakyum-0.0.7/sakyum/static/default_style/css/
--rw-rw-r--   0 usman     (1000) usman     (1000)     6831 2023-03-20 02:44:12.000000 sakyum-0.0.7/sakyum/static/default_style/css/style.css
-drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-04-04 00:47:59.240357 sakyum-0.0.7/sakyum/static/default_style/js/
--rw-rw-r--   0 usman     (1000) usman     (1000)      127 2023-03-20 02:44:12.000000 sakyum-0.0.7/sakyum/static/default_style/js/index.js
-drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-04-04 00:47:59.260366 sakyum-0.0.7/sakyum/static/default_style/media/
--rw-rw-r--   0 usman     (1000) usman     (1000)     3767 2023-03-20 02:44:12.000000 sakyum-0.0.7/sakyum/static/default_style/media/alert.png
--rw-rw-r--   0 usman     (1000) usman     (1000)     1460 2023-03-20 02:44:12.000000 sakyum-0.0.7/sakyum/static/default_style/media/default_img.png
--rw-rw-r--   0 usman     (1000) usman     (1000)     3767 2023-03-20 02:44:12.000000 sakyum-0.0.7/sakyum/static/default_style/media/favicon.ico
--rw-rw-r--   0 usman     (1000) usman     (1000)        0 2023-03-20 02:44:12.000000 sakyum-0.0.7/sakyum/static/do_nothing.txt
-drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-04-04 00:47:59.000244 sakyum-0.0.7/sakyum/templates/
-drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-04-04 00:47:59.308389 sakyum-0.0.7/sakyum/templates/default_errors/
--rw-rw-r--   0 usman     (1000) usman     (1000)      141 2023-03-20 02:44:12.000000 sakyum-0.0.7/sakyum/templates/default_errors/400.html
--rw-rw-r--   0 usman     (1000) usman     (1000)      142 2023-03-20 02:44:12.000000 sakyum-0.0.7/sakyum/templates/default_errors/401.html
--rw-rw-r--   0 usman     (1000) usman     (1000)      139 2023-03-20 02:44:12.000000 sakyum-0.0.7/sakyum/templates/default_errors/403.html
--rw-rw-r--   0 usman     (1000) usman     (1000)      139 2023-03-20 02:44:12.000000 sakyum-0.0.7/sakyum/templates/default_errors/404.html
--rw-rw-r--   0 usman     (1000) usman     (1000)      144 2023-03-20 02:44:12.000000 sakyum-0.0.7/sakyum/templates/default_errors/406.html
--rw-rw-r--   0 usman     (1000) usman     (1000)      152 2023-03-20 02:44:12.000000 sakyum-0.0.7/sakyum/templates/default_errors/415.html
--rw-rw-r--   0 usman     (1000) usman     (1000)      147 2023-03-20 02:44:12.000000 sakyum-0.0.7/sakyum/templates/default_errors/429.html
--rw-rw-r--   0 usman     (1000) usman     (1000)      151 2023-03-20 02:44:12.000000 sakyum-0.0.7/sakyum/templates/default_errors/500.html
--rw-rw-r--   0 usman     (1000) usman     (1000)      146 2023-03-20 02:44:12.000000 sakyum-0.0.7/sakyum/templates/default_errors/501.html
--rw-rw-r--   0 usman     (1000) usman     (1000)      142 2023-03-20 02:44:12.000000 sakyum-0.0.7/sakyum/templates/default_errors/502.html
--rw-rw-r--   0 usman     (1000) usman     (1000)      150 2023-03-20 02:44:12.000000 sakyum-0.0.7/sakyum/templates/default_errors/503.html
--rw-rw-r--   0 usman     (1000) usman     (1000)      146 2023-03-20 02:44:12.000000 sakyum-0.0.7/sakyum/templates/default_errors/504.html
-drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-04-04 00:47:59.332400 sakyum-0.0.7/sakyum/templates/default_page/
--rw-rw-r--   0 usman     (1000) usman     (1000)     3092 2023-03-20 02:44:12.000000 sakyum-0.0.7/sakyum/templates/default_page/admin_change_password.html
--rw-rw-r--   0 usman     (1000) usman     (1000)      622 2023-03-27 01:38:36.000000 sakyum-0.0.7/sakyum/templates/default_page/admin_change_profile_image.html
--rw-rw-r--   0 usman     (1000) usman     (1000)     2262 2023-03-20 02:44:12.000000 sakyum-0.0.7/sakyum/templates/default_page/admin_login.html
--rw-rw-r--   0 usman     (1000) usman     (1000)     3150 2023-03-20 02:44:12.000000 sakyum-0.0.7/sakyum/templates/default_page/admin_register.html
--rw-rw-r--   0 usman     (1000) usman     (1000)     4152 2023-03-27 01:38:36.000000 sakyum-0.0.7/sakyum/templates/default_page/default.html
--rw-rw-r--   0 usman     (1000) usman     (1000)     1025 2023-03-25 13:28:16.000000 sakyum-0.0.7/sakyum/templates/default_page/default_base.html
--rw-rw-r--   0 usman     (1000) usman     (1000)      504 2023-03-20 02:44:12.000000 sakyum-0.0.7/sakyum/templates/default_page/default_index.html
--rw-rw-r--   0 usman     (1000) usman     (1000)     8739 2023-03-27 01:38:36.000000 sakyum-0.0.7/sakyum/utils.py
-drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-04-04 00:47:59.156317 sakyum-0.0.7/sakyum.egg-info/
--rw-rw-r--   0 usman     (1000) usman     (1000)     5944 2023-04-04 00:47:56.000000 sakyum-0.0.7/sakyum.egg-info/PKG-INFO
--rw-rw-r--   0 usman     (1000) usman     (1000)     1639 2023-04-04 00:47:58.000000 sakyum-0.0.7/sakyum.egg-info/SOURCES.txt
--rw-rw-r--   0 usman     (1000) usman     (1000)        1 2023-04-04 00:47:56.000000 sakyum-0.0.7/sakyum.egg-info/dependency_links.txt
--rw-rw-r--   0 usman     (1000) usman     (1000)      398 2023-04-04 00:47:56.000000 sakyum-0.0.7/sakyum.egg-info/requires.txt
--rw-rw-r--   0 usman     (1000) usman     (1000)        7 2023-04-04 00:47:56.000000 sakyum-0.0.7/sakyum.egg-info/top_level.txt
--rw-rw-r--   0 usman     (1000) usman     (1000)       38 2023-04-04 00:47:59.340403 sakyum-0.0.7/setup.cfg
--rw-rw-r--   0 usman     (1000) usman     (1000)     2415 2023-04-04 00:44:38.000000 sakyum-0.0.7/setup.py
+drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-06-09 17:49:34.388300 sakyum-0.0.8/
+-rw-rw-r--   0 usman     (1000) usman     (1000)     1309 2023-06-09 17:39:22.000000 sakyum-0.0.8/CHANGELOG
+-rw-rw-r--   0 usman     (1000) usman     (1000)     1077 2023-06-08 02:53:33.000000 sakyum-0.0.8/LICENSE
+-rw-rw-r--   0 usman     (1000) usman     (1000)       82 2023-06-08 02:53:33.000000 sakyum-0.0.8/MANIFEST.in
+-rw-rw-r--   0 usman     (1000) usman     (1000)     6426 2023-06-09 17:49:34.384300 sakyum-0.0.8/PKG-INFO
+-rw-rw-r--   0 usman     (1000) usman     (1000)     2996 2023-06-09 17:44:39.000000 sakyum-0.0.8/README.md
+drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-06-09 17:49:34.276288 sakyum-0.0.8/media/
+-rw-rw-r--   0 usman     (1000) usman     (1000)    33115 2023-06-09 17:06:35.000000 sakyum-0.0.8/media/sakyum_default_page.png
+-rw-rw-r--   0 usman     (1000) usman     (1000)      412 2023-06-09 13:53:26.000000 sakyum-0.0.8/requirements.txt
+drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-06-09 17:49:34.304291 sakyum-0.0.8/sakyum/
+-rw-rw-r--   0 usman     (1000) usman     (1000)      725 2023-06-09 14:23:38.000000 sakyum-0.0.8/sakyum/__init__.py
+-rw-rw-r--   0 usman     (1000) usman     (1000)      489 2023-06-08 20:31:39.000000 sakyum-0.0.8/sakyum/api.py
+drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-06-09 17:49:34.324293 sakyum-0.0.8/sakyum/auth/
+-rw-rw-r--   0 usman     (1000) usman     (1000)       46 2023-06-08 17:44:37.000000 sakyum-0.0.8/sakyum/auth/__init__.py
+-rw-rw-r--   0 usman     (1000) usman     (1000)     1298 2023-06-08 20:40:43.000000 sakyum-0.0.8/sakyum/auth/admin.py
+-rw-rw-r--   0 usman     (1000) usman     (1000)     1643 2023-06-08 20:41:07.000000 sakyum-0.0.8/sakyum/auth/forms.py
+-rw-rw-r--   0 usman     (1000) usman     (1000)     1280 2023-06-09 14:26:48.000000 sakyum-0.0.8/sakyum/auth/models.py
+-rw-rw-r--   0 usman     (1000) usman     (1000)     6069 2023-06-09 14:28:34.000000 sakyum-0.0.8/sakyum/auth/routes.py
+-rw-rw-r--   0 usman     (1000) usman     (1000)    21240 2023-06-09 17:13:59.000000 sakyum-0.0.8/sakyum/base.py
+-rw-rw-r--   0 usman     (1000) usman     (1000)     4711 2023-06-09 14:10:59.000000 sakyum-0.0.8/sakyum/blueprint.py
+drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-06-09 17:49:34.324293 sakyum-0.0.8/sakyum/contrib/
+-rw-rw-r--   0 usman     (1000) usman     (1000)      619 2023-06-09 14:28:59.000000 sakyum-0.0.8/sakyum/contrib/__init__.py
+-rw-rw-r--   0 usman     (1000) usman     (1000)      437 2023-06-09 14:08:46.000000 sakyum-0.0.8/sakyum/database.py
+drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-06-09 17:49:34.336295 sakyum-0.0.8/sakyum/mute/
+-rw-rw-r--   0 usman     (1000) usman     (1000)      581 2023-06-08 20:49:28.000000 sakyum-0.0.8/sakyum/mute/__init__.py
+-rw-rw-r--   0 usman     (1000) usman     (1000)     1517 2023-06-08 20:50:10.000000 sakyum-0.0.8/sakyum/mute/app.py
+-rw-rw-r--   0 usman     (1000) usman     (1000)     2899 2023-06-08 20:53:35.000000 sakyum-0.0.8/sakyum/mute/page.py
+-rw-rw-r--   0 usman     (1000) usman     (1000)     3400 2023-06-08 20:51:58.000000 sakyum-0.0.8/sakyum/mute/project.py
+drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-06-09 17:49:34.336295 sakyum-0.0.8/sakyum/static/
+drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-06-09 17:49:34.256286 sakyum-0.0.8/sakyum/static/default_style/
+drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-06-09 17:49:34.340295 sakyum-0.0.8/sakyum/static/default_style/css/
+-rw-rw-r--   0 usman     (1000) usman     (1000)     6831 2023-06-08 02:53:33.000000 sakyum-0.0.8/sakyum/static/default_style/css/style.css
+drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-06-09 17:49:34.340295 sakyum-0.0.8/sakyum/static/default_style/js/
+-rw-rw-r--   0 usman     (1000) usman     (1000)      127 2023-06-08 02:53:33.000000 sakyum-0.0.8/sakyum/static/default_style/js/index.js
+drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-06-09 17:49:34.344295 sakyum-0.0.8/sakyum/static/default_style/media/
+-rw-rw-r--   0 usman     (1000) usman     (1000)     3767 2023-06-08 02:53:33.000000 sakyum-0.0.8/sakyum/static/default_style/media/alert.png
+-rw-rw-r--   0 usman     (1000) usman     (1000)     1460 2023-06-08 02:53:33.000000 sakyum-0.0.8/sakyum/static/default_style/media/default_img.png
+-rw-rw-r--   0 usman     (1000) usman     (1000)     3767 2023-06-08 02:53:33.000000 sakyum-0.0.8/sakyum/static/default_style/media/favicon.ico
+-rw-rw-r--   0 usman     (1000) usman     (1000)        0 2023-06-09 17:10:52.000000 sakyum-0.0.8/sakyum/static/do_nothing.txt
+drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-06-09 17:49:34.260286 sakyum-0.0.8/sakyum/templates/
+drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-06-09 17:49:34.368298 sakyum-0.0.8/sakyum/templates/default_errors/
+-rw-rw-r--   0 usman     (1000) usman     (1000)      141 2023-06-08 20:59:20.000000 sakyum-0.0.8/sakyum/templates/default_errors/400.html
+-rw-rw-r--   0 usman     (1000) usman     (1000)      142 2023-06-08 20:59:37.000000 sakyum-0.0.8/sakyum/templates/default_errors/401.html
+-rw-rw-r--   0 usman     (1000) usman     (1000)      139 2023-06-08 20:59:53.000000 sakyum-0.0.8/sakyum/templates/default_errors/403.html
+-rw-rw-r--   0 usman     (1000) usman     (1000)      139 2023-06-08 21:00:12.000000 sakyum-0.0.8/sakyum/templates/default_errors/404.html
+-rw-rw-r--   0 usman     (1000) usman     (1000)      144 2023-06-08 21:00:24.000000 sakyum-0.0.8/sakyum/templates/default_errors/406.html
+-rw-rw-r--   0 usman     (1000) usman     (1000)      152 2023-06-08 21:00:35.000000 sakyum-0.0.8/sakyum/templates/default_errors/415.html
+-rw-rw-r--   0 usman     (1000) usman     (1000)      147 2023-06-08 21:00:48.000000 sakyum-0.0.8/sakyum/templates/default_errors/429.html
+-rw-rw-r--   0 usman     (1000) usman     (1000)      151 2023-06-08 21:00:58.000000 sakyum-0.0.8/sakyum/templates/default_errors/500.html
+-rw-rw-r--   0 usman     (1000) usman     (1000)      146 2023-06-08 21:01:10.000000 sakyum-0.0.8/sakyum/templates/default_errors/501.html
+-rw-rw-r--   0 usman     (1000) usman     (1000)      142 2023-06-08 21:01:21.000000 sakyum-0.0.8/sakyum/templates/default_errors/502.html
+-rw-rw-r--   0 usman     (1000) usman     (1000)      150 2023-06-08 21:01:42.000000 sakyum-0.0.8/sakyum/templates/default_errors/503.html
+-rw-rw-r--   0 usman     (1000) usman     (1000)      146 2023-06-08 21:02:17.000000 sakyum-0.0.8/sakyum/templates/default_errors/504.html
+drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-06-09 17:49:34.384300 sakyum-0.0.8/sakyum/templates/default_page/
+-rw-rw-r--   0 usman     (1000) usman     (1000)     3092 2023-06-08 21:03:30.000000 sakyum-0.0.8/sakyum/templates/default_page/admin_change_password.html
+-rw-rw-r--   0 usman     (1000) usman     (1000)      622 2023-06-08 21:04:03.000000 sakyum-0.0.8/sakyum/templates/default_page/admin_change_profile_image.html
+-rw-rw-r--   0 usman     (1000) usman     (1000)     2262 2023-06-08 21:04:15.000000 sakyum-0.0.8/sakyum/templates/default_page/admin_login.html
+-rw-rw-r--   0 usman     (1000) usman     (1000)     3150 2023-06-08 21:04:26.000000 sakyum-0.0.8/sakyum/templates/default_page/admin_register.html
+-rw-rw-r--   0 usman     (1000) usman     (1000)     4156 2023-06-08 17:44:37.000000 sakyum-0.0.8/sakyum/templates/default_page/default.html
+-rw-rw-r--   0 usman     (1000) usman     (1000)     1025 2023-06-08 21:04:49.000000 sakyum-0.0.8/sakyum/templates/default_page/default_base.html
+-rw-rw-r--   0 usman     (1000) usman     (1000)      509 2023-06-08 21:03:15.000000 sakyum-0.0.8/sakyum/templates/default_page/default_index.html
+-rw-rw-r--   0 usman     (1000) usman     (1000)     8715 2023-06-09 14:08:31.000000 sakyum-0.0.8/sakyum/utils.py
+drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-06-09 17:49:34.312292 sakyum-0.0.8/sakyum.egg-info/
+-rw-rw-r--   0 usman     (1000) usman     (1000)     6426 2023-06-09 17:49:33.000000 sakyum-0.0.8/sakyum.egg-info/PKG-INFO
+-rw-rw-r--   0 usman     (1000) usman     (1000)     1669 2023-06-09 17:49:34.000000 sakyum-0.0.8/sakyum.egg-info/SOURCES.txt
+-rw-rw-r--   0 usman     (1000) usman     (1000)        1 2023-06-09 17:49:33.000000 sakyum-0.0.8/sakyum.egg-info/dependency_links.txt
+-rw-rw-r--   0 usman     (1000) usman     (1000)      398 2023-06-09 17:49:33.000000 sakyum-0.0.8/sakyum.egg-info/requires.txt
+-rw-rw-r--   0 usman     (1000) usman     (1000)        7 2023-06-09 17:49:33.000000 sakyum-0.0.8/sakyum.egg-info/top_level.txt
+-rw-rw-r--   0 usman     (1000) usman     (1000)       38 2023-06-09 17:49:34.388300 sakyum-0.0.8/setup.cfg
+-rw-rw-r--   0 usman     (1000) usman     (1000)     2568 2023-06-09 17:16:11.000000 sakyum-0.0.8/setup.py
```

### Comparing `sakyum-0.0.7/CHANGELOG` & `sakyum-0.0.8/CHANGELOG`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 Change Log
 ==========
 
+0.0.8 (09/june/2023)
+------------------
+- Eight Release
+
+OS compatibility
+
+Making sakyum to be compatible with windows OS as well as other OS
+
 0.0.7 (4/april/2023)
 ------------------
 - Seventh Release
 
 This release mostly is for adding more docs and examples.
 
 - Sixth Release
```

### Comparing `sakyum-0.0.7/LICENSE` & `sakyum-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `sakyum-0.0.7/PKG-INFO` & `sakyum-0.0.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: sakyum
-Version: 0.0.7
+Version: 0.0.8
 Summary: An extension of flask web framework that erase the complexity of structuring flask project blueprint, packages, and other annoying stuffs
 Home-page: https://sakyum.readthedocs.io
 Author: Usman Musa
 Author-email: usmanmusa1920@gmail.com
-License: UNKNOWN
+License: MIT
+Download-URL: https://pypi.org/project/sakyum
+Project-URL: Documentation, https://sakyum.readthedocs.io
+Project-URL: Source, https://github.com/usmanmusa1920/sakyum
 Description: 
         # Sakyum
         
         An extension of flask web framework that erase the complexity of structuring flask project blueprint, packages, and other annoying stuffs.
         
         ## Installation
         
-        Install and update the latest release from <a href="https://pypi.org/project/sakyum">pypi</a>. Basically the library was uploaded using `sdist` (Source Distribution) and this software (library) it might not be compatible with `windows operating system` but it works on other `OS` such as `linux` and `macOS`, but very soon the version that will be compatible with **windows operating system** will be release, stay tuned.
+        Install and update the latest release from <a href="https://pypi.org/project/sakyum">pypi</a>. Basically the library was uploaded using `sdist` (Source Distribution) and this software (library) as from `v0.0.8` it is now compatible with `windows OS` and others as well, such as `linux`, `macOS` and possibly some others too!.
         
         ```
         pip install --upgrade sakyum
         ```
         
         ## Create flask project using sakyum
         
@@ -79,25 +82,38 @@
         
         visit `http://127.0.0.1:5000/exam` this will take you to your app landing page (exam)
         
         visit `http://127.0.0.1:5000/admin` this will take you to admin page. From there you are ready to go.
         
         See more documentations <a href="https://sakyum.readthedocs.io">here!</a>
         
+        ### Sakyum default page
+        
+        ![Sakyum default page](./media/sakyum_default_page.png)
+        
         ## Useful links
         
         - Documentation: https://sakyum.readthedocs.io
         - Repository: https://github.com/usmanmusa1920/sakyum
+        - Docker example: https://github.com/usmanmusa1920/sakyum/tree/master/example/sakyum-docker
         
         Pull requests are welcome
         
         
         Change Log
         ==========
         
+        0.0.8 (09/june/2023)
+        ------------------
+        - Eight Release
+        
+        OS compatibility
+        
+        Making sakyum to be compatible with windows OS as well as other OS
+        
         0.0.7 (4/april/2023)
         ------------------
         - Seventh Release
         
         This release mostly is for adding more docs and examples.
         
         - Sixth Release
@@ -115,20 +131,20 @@
         Database migration is added using `alembic`
         
         Some error pages, default page were added but still you can customise it in your project sub folder (the package with the same name of your project in your project directory) in a file called `route.py`. Also an admin directory within your project templates folder is added too!
         
         Possibly other well things are added which include auth system for `users` and more.
         
 Keywords: sakyum
-Platform: UNKNOWN
+Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
-Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
```

#### html2text {}

```diff
@@ -1,65 +1,70 @@
-Metadata-Version: 2.1 Name: sakyum Version: 0.0.7 Summary: An extension of
+Metadata-Version: 2.1 Name: sakyum Version: 0.0.8 Summary: An extension of
 flask web framework that erase the complexity of structuring flask project
 blueprint, packages, and other annoying stuffs Home-page: https://
 sakyum.readthedocs.io Author: Usman Musa Author-email: usmanmusa1920@gmail.com
-License: UNKNOWN Description: # Sakyum An extension of flask web framework that
-erase the complexity of structuring flask project blueprint, packages, and
-other annoying stuffs. ## Installation Install and update the latest release
-from pypi. Basically the library was uploaded using `sdist` (Source
-Distribution) and this software (library) it might not be compatible with
-`windows operating system` but it works on other `OS` such as `linux` and
-`macOS`, but very soon the version that will be compatible with **windows
-operating system** will be release, stay tuned. ``` pip install --upgrade
-sakyum ``` ## Create flask project using sakyum After the installation paste
-the following command on your termianl ``` python -c "from sakyum import
-project; project('schoolsite')" ``` This will create a project called
-`schoolsite` now cd into the `schoolsite` directory, if you do `ls` within the
-directory you just enter you will see a module called `thunder.py` and some
-directories (some in the form of package) `media`, `static`, `templates` and a
-directory with the same name of your base directory name, in our case it is
-`schoolsite`. Boot up the flask server by running the below command ``` python
-thunder.py boot ``` Now visit the local url `http://127.0.0.1:5000` this will
-show you index page of your project ## Create flask app within your project
-(schoolsite) For you to start an app within your project `schoolsite` shutdown
-the flask development server by pressing ( CTRL+C ) and then run the following
-command, by giving the name you want your app to be, in our case we will call
-our app `exam` ``` python thunder.py create_app -a exam ``` this will create an
-app (a new package called `exam`) within your project `(schoolsite)` ##
-Register an app Once the app is created open a file `schoolsite/routes.py` and
-import your `exam` blueprint which is in (`exam/views.py`), default name given
-to an app blueprint, is the app name so our `exam` app blueprint name is
-`exam`, after importing it, append (register) the app blueprint in a list
-called `reg_blueprints` in that same file of `schoolsite/routes.py` importing
-blueprint ```py from exam.views import exam ``` registering blueprint ```py
-reg_blueprints = [ blueprint.default, blueprint.errors, blueprint.auth, base,
-exam, ] ``` once you register the app, boot up the flask webserver again by ```
-python thunder.py boot ``` visit `http://127.0.0.1:5000` which is your project
-landing page visit `http://127.0.0.1:5000/exam` this will take you to your app
-landing page (exam) visit `http://127.0.0.1:5000/admin` this will take you to
-admin page. From there you are ready to go. See more documentations here! ##
-Useful links - Documentation: https://sakyum.readthedocs.io - Repository:
-https://github.com/usmanmusa1920/sakyum Pull requests are welcome Change Log
-========== 0.0.7 (4/april/2023) ------------------ - Seventh Release This
-release mostly is for adding more docs and examples. - Sixth Release Alembic is
-included as dependency (in the require module list). - Fifth Release In fifith
-release, we handle how default user file system tricks is, things like when
-user change his profile picture. - Fourth Release In this release we handle how
-we can customise the admin html page by inheriting (extends) it in our project
-templates/admin directory, and the admin page on how to bind models in the
-admin. Also I refactor other libraries that this package needs with their
-corresponding versions in the setup.py and requirements.txt files. In this
-release good documentations is well packed. Database migration is added using
-`alembic` Some error pages, default page were added but still you can customise
-it in your project sub folder (the package with the same name of your project
-in your project directory) in a file called `route.py`. Also an admin directory
-within your project templates folder is added too! Possibly other well things
-are added which include auth system for `users` and more. Keywords: sakyum
-Platform: UNKNOWN Classifier: Development Status :: 5 - Production/Stable
+License: MIT Download-URL: https://pypi.org/project/sakyum Project-URL:
+Documentation, https://sakyum.readthedocs.io Project-URL: Source, https://
+github.com/usmanmusa1920/sakyum Description: # Sakyum An extension of flask web
+framework that erase the complexity of structuring flask project blueprint,
+packages, and other annoying stuffs. ## Installation Install and update the
+latest release from pypi. Basically the library was uploaded using `sdist`
+(Source Distribution) and this software (library) as from `v0.0.8` it is now
+compatible with `windows OS` and others as well, such as `linux`, `macOS` and
+possibly some others too!. ``` pip install --upgrade sakyum ``` ## Create flask
+project using sakyum After the installation paste the following command on your
+termianl ``` python -c "from sakyum import project; project('schoolsite')" ```
+This will create a project called `schoolsite` now cd into the `schoolsite`
+directory, if you do `ls` within the directory you just enter you will see a
+module called `thunder.py` and some directories (some in the form of package)
+`media`, `static`, `templates` and a directory with the same name of your base
+directory name, in our case it is `schoolsite`. Boot up the flask server by
+running the below command ``` python thunder.py boot ``` Now visit the local
+url `http://127.0.0.1:5000` this will show you index page of your project ##
+Create flask app within your project (schoolsite) For you to start an app
+within your project `schoolsite` shutdown the flask development server by
+pressing ( CTRL+C ) and then run the following command, by giving the name you
+want your app to be, in our case we will call our app `exam` ``` python
+thunder.py create_app -a exam ``` this will create an app (a new package called
+`exam`) within your project `(schoolsite)` ## Register an app Once the app is
+created open a file `schoolsite/routes.py` and import your `exam` blueprint
+which is in (`exam/views.py`), default name given to an app blueprint, is the
+app name so our `exam` app blueprint name is `exam`, after importing it, append
+(register) the app blueprint in a list called `reg_blueprints` in that same
+file of `schoolsite/routes.py` importing blueprint ```py from exam.views import
+exam ``` registering blueprint ```py reg_blueprints = [ blueprint.default,
+blueprint.errors, blueprint.auth, base, exam, ] ``` once you register the app,
+boot up the flask webserver again by ``` python thunder.py boot ``` visit
+`http://127.0.0.1:5000` which is your project landing page visit `http://
+127.0.0.1:5000/exam` this will take you to your app landing page (exam) visit
+`http://127.0.0.1:5000/admin` this will take you to admin page. From there you
+are ready to go. See more documentations here! ### Sakyum default page ![Sakyum
+default page](./media/sakyum_default_page.png) ## Useful links - Documentation:
+https://sakyum.readthedocs.io - Repository: https://github.com/usmanmusa1920/
+sakyum - Docker example: https://github.com/usmanmusa1920/sakyum/tree/master/
+example/sakyum-docker Pull requests are welcome Change Log ========== 0.0.8
+(09/june/2023) ------------------ - Eight Release OS compatibility Making
+sakyum to be compatible with windows OS as well as other OS 0.0.7 (4/april/
+2023) ------------------ - Seventh Release This release mostly is for adding
+more docs and examples. - Sixth Release Alembic is included as dependency (in
+the require module list). - Fifth Release In fifith release, we handle how
+default user file system tricks is, things like when user change his profile
+picture. - Fourth Release In this release we handle how we can customise the
+admin html page by inheriting (extends) it in our project templates/admin
+directory, and the admin page on how to bind models in the admin. Also I
+refactor other libraries that this package needs with their corresponding
+versions in the setup.py and requirements.txt files. In this release good
+documentations is well packed. Database migration is added using `alembic` Some
+error pages, default page were added but still you can customise it in your
+project sub folder (the package with the same name of your project in your
+project directory) in a file called `route.py`. Also an admin directory within
+your project templates folder is added too! Possibly other well things are
+added which include auth system for `users` and more. Keywords: sakyum
+Platform: any Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment Classifier: Intended Audience ::
 Developers Classifier: Natural Language :: English Classifier: Operating System
-:: POSIX :: Linux Classifier: License :: OSI Approved :: MIT License
+:: OS Independent Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.10 Requires-Python: >=3.6 Description-
 Content-Type: text/markdown
```

### Comparing `sakyum-0.0.7/README.md` & `sakyum-0.0.8/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 # Sakyum
 
 An extension of flask web framework that erase the complexity of structuring flask project blueprint, packages, and other annoying stuffs.
 
 ## Installation
 
-Install and update the latest release from <a href="https://pypi.org/project/sakyum">pypi</a>. Basically the library was uploaded using `sdist` (Source Distribution) and this software (library) it might not be compatible with `windows operating system` but it works on other `OS` such as `linux` and `macOS`, but very soon the version that will be compatible with **windows operating system** will be release, stay tuned.
+Install and update the latest release from <a href="https://pypi.org/project/sakyum">pypi</a>. Basically the library was uploaded using `sdist` (Source Distribution) and this software (library) as from `v0.0.8` it is now compatible with `windows OS` and others as well, such as `linux`, `macOS` and possibly some others too!.
 
 ```
 pip install --upgrade sakyum
 ```
 
 ## Create flask project using sakyum
 
@@ -71,13 +71,18 @@
 
 visit `http://127.0.0.1:5000/exam` this will take you to your app landing page (exam)
 
 visit `http://127.0.0.1:5000/admin` this will take you to admin page. From there you are ready to go.
 
 See more documentations <a href="https://sakyum.readthedocs.io">here!</a>
 
+### Sakyum default page
+
+![Sakyum default page](./media/sakyum_default_page.png)
+
 ## Useful links
 
 - Documentation: https://sakyum.readthedocs.io
 - Repository: https://github.com/usmanmusa1920/sakyum
+- Docker example: https://github.com/usmanmusa1920/sakyum/tree/master/example/sakyum-docker
 
 Pull requests are welcome
```

#### html2text {}

```diff
@@ -1,37 +1,38 @@
  # Sakyum An extension of flask web framework that erase the complexity of
 structuring flask project blueprint, packages, and other annoying stuffs. ##
 Installation Install and update the latest release from pypi. Basically the
 library was uploaded using `sdist` (Source Distribution) and this software
-(library) it might not be compatible with `windows operating system` but it
-works on other `OS` such as `linux` and `macOS`, but very soon the version that
-will be compatible with **windows operating system** will be release, stay
-tuned. ``` pip install --upgrade sakyum ``` ## Create flask project using
-sakyum After the installation paste the following command on your termianl ```
-python -c "from sakyum import project; project('schoolsite')" ``` This will
-create a project called `schoolsite` now cd into the `schoolsite` directory, if
-you do `ls` within the directory you just enter you will see a module called
-`thunder.py` and some directories (some in the form of package) `media`,
-`static`, `templates` and a directory with the same name of your base directory
-name, in our case it is `schoolsite`. Boot up the flask server by running the
-below command ``` python thunder.py boot ``` Now visit the local url `http://
-127.0.0.1:5000` this will show you index page of your project ## Create flask
-app within your project (schoolsite) For you to start an app within your
-project `schoolsite` shutdown the flask development server by pressing ( CTRL+C
-) and then run the following command, by giving the name you want your app to
-be, in our case we will call our app `exam` ``` python thunder.py create_app -
-a exam ``` this will create an app (a new package called `exam`) within your
-project `(schoolsite)` ## Register an app Once the app is created open a file
-`schoolsite/routes.py` and import your `exam` blueprint which is in (`exam/
-views.py`), default name given to an app blueprint, is the app name so our
-`exam` app blueprint name is `exam`, after importing it, append (register) the
-app blueprint in a list called `reg_blueprints` in that same file of
-`schoolsite/routes.py` importing blueprint ```py from exam.views import exam
-``` registering blueprint ```py reg_blueprints = [ blueprint.default,
-blueprint.errors, blueprint.auth, base, exam, ] ``` once you register the app,
-boot up the flask webserver again by ``` python thunder.py boot ``` visit
-`http://127.0.0.1:5000` which is your project landing page visit `http://
-127.0.0.1:5000/exam` this will take you to your app landing page (exam) visit
-`http://127.0.0.1:5000/admin` this will take you to admin page. From there you
-are ready to go. See more documentations here! ## Useful links - Documentation:
-https://sakyum.readthedocs.io - Repository: https://github.com/usmanmusa1920/
-sakyum Pull requests are welcome
+(library) as from `v0.0.8` it is now compatible with `windows OS` and others as
+well, such as `linux`, `macOS` and possibly some others too!. ``` pip install -
+-upgrade sakyum ``` ## Create flask project using sakyum After the installation
+paste the following command on your termianl ``` python -c "from sakyum import
+project; project('schoolsite')" ``` This will create a project called
+`schoolsite` now cd into the `schoolsite` directory, if you do `ls` within the
+directory you just enter you will see a module called `thunder.py` and some
+directories (some in the form of package) `media`, `static`, `templates` and a
+directory with the same name of your base directory name, in our case it is
+`schoolsite`. Boot up the flask server by running the below command ``` python
+thunder.py boot ``` Now visit the local url `http://127.0.0.1:5000` this will
+show you index page of your project ## Create flask app within your project
+(schoolsite) For you to start an app within your project `schoolsite` shutdown
+the flask development server by pressing ( CTRL+C ) and then run the following
+command, by giving the name you want your app to be, in our case we will call
+our app `exam` ``` python thunder.py create_app -a exam ``` this will create an
+app (a new package called `exam`) within your project `(schoolsite)` ##
+Register an app Once the app is created open a file `schoolsite/routes.py` and
+import your `exam` blueprint which is in (`exam/views.py`), default name given
+to an app blueprint, is the app name so our `exam` app blueprint name is
+`exam`, after importing it, append (register) the app blueprint in a list
+called `reg_blueprints` in that same file of `schoolsite/routes.py` importing
+blueprint ```py from exam.views import exam ``` registering blueprint ```py
+reg_blueprints = [ blueprint.default, blueprint.errors, blueprint.auth, base,
+exam, ] ``` once you register the app, boot up the flask webserver again by ```
+python thunder.py boot ``` visit `http://127.0.0.1:5000` which is your project
+landing page visit `http://127.0.0.1:5000/exam` this will take you to your app
+landing page (exam) visit `http://127.0.0.1:5000/admin` this will take you to
+admin page. From there you are ready to go. See more documentations here! ###
+Sakyum default page ![Sakyum default page](./media/sakyum_default_page.png) ##
+Useful links - Documentation: https://sakyum.readthedocs.io - Repository:
+https://github.com/usmanmusa1920/sakyum - Docker example: https://github.com/
+usmanmusa1920/sakyum/tree/master/example/sakyum-docker Pull requests are
+welcome
```

### Comparing `sakyum-0.0.7/sakyum/__init__.py` & `sakyum-0.0.8/sakyum/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,19 +9,19 @@
      / /_|  /_/  / /  / /  \/ |
   /_/ /  | /  | / /__/ /      |
   
   An extension of flask web framework that erase the complexity of structuring flask project blueprint, packages, and other annoying stuffs
 """
 
 
-__title__ = "sakyum"
-__version__ = "0.0.7"
-__author__ = "Usman Musa"
-__author_email__ = "usmanmusa1920@gmail.com"
-__author_website__ = "https://usmanmusa1920.github.io"
-__repository__ = "https://github.com/usmanmusa1920/sakyum"
-__website__ = "https://sakyum.readthedocs.io"
-__copyright__ = "Copyright (C) 2022 - 2023 Usman Musa"
+__title__ = 'sakyum'
+__version__ = '0.0.8'
+__author__ = 'Usman Musa'
+__author_email__ = 'usmanmusa1920@gmail.com'
+__author_website__ = 'https://usmanmusa1920.github.io'
+__repository__ = 'https://github.com/usmanmusa1920/sakyum'
+__url__ = 'https://sakyum.readthedocs.io'
+__copyright__ = 'Copyright (C) 2022 - 2023 Usman Musa'
 
 
 from .base import Boot
 from .api import project
```

### Comparing `sakyum-0.0.7/sakyum/auth/admin.py` & `sakyum-0.0.8/sakyum/auth/admin.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,31 @@
-# from sakyum software, your (schoolsite) project auth admin.py file
+# -*- coding: utf-8 -*-
+
 from flask_login import current_user
 from flask import redirect, request, url_for
 from flask_admin.contrib.sqla import ModelView
 
 
 class UserAdminView(ModelView):
   can_delete = True  # enable model deletion
   can_create = True  # enable model deletion
   can_edit = True  # enable model deletion
   page_size = 50  # the number of entries to display on the list view
 
   # This is used to list the various columns in the order you want them.
-  column_list = ("username", "email", "password", "date_created", "authenticated", "is_superuser")
+  column_list = ('username', 'email', 'password', 'date_created', 'authenticated', 'is_superuser')
   # Columns that you want to be searchable in the model.
-  column_searchable_list = ("username", "email", "password", "date_joined", "authenticated", "is_superuser")
+  column_searchable_list = ('username', 'email', 'password', 'date_joined', 'authenticated', 'is_superuser')
   # The column that the view should be sorted with by default (when the view is loaded for
   # the first time). The second parameter True tells flask-admin to sort it in descending order.
-  column_default_sort = ("username", True)
+  column_default_sort = ('username', True)
   # List of columns that can be used to filter.
-  column_filters = ("username",)
+  column_filters = ('username',)
   
 
   def is_accessible(self):
     return current_user.is_authenticated
     
     
   def inaccessible_callback(self, name, **kwargs):
     # redirect to login page if user doesn't have access
-    return redirect(url_for("auth.adminLogin", next=request.url))
+    return redirect(url_for('auth.adminLogin', next=request.url))
```

### Comparing `sakyum-0.0.7/sakyum/auth/forms.py` & `sakyum-0.0.8/sakyum/auth/forms.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,35 @@
-# from sakyum software, your (schoolsite) project auth forms.py file
+# -*- coding: utf-8 -*-
+
 from flask_wtf import FlaskForm
 from wtforms import StringField, PasswordField
 from wtforms.validators import DataRequired, Length, Email, EqualTo, ValidationError
 from .models import User
 
 
 class RegisterForm(FlaskForm):
-  username = StringField("Username", validators=[DataRequired(), Length(min=2, max=30)])
-  email = StringField("Email", validators=[DataRequired(), Email()])
+  username = StringField('Username', validators=[DataRequired(), Length(min=2, max=30)])
+  email = StringField('Email', validators=[DataRequired(), Email()])
   # picture = FileField('Update Profile Picture', validators=[FileAllowed(['jpg', 'png'])])
-  password = PasswordField("Password", validators=[DataRequired(), Length(min=6)])
-  confirm_password = PasswordField("Confirm Password", validators=[DataRequired(), EqualTo("password"), Length(min=6)])
+  password = PasswordField('Password', validators=[DataRequired(), Length(min=6)])
+  confirm_password = PasswordField('Confirm Password', validators=[DataRequired(), EqualTo('password'), Length(min=6)])
   
   def validate_username(self, username):
     user = User.query.filter_by(username=username.data).first()
     if user:
-      raise ValidationError("That username is taken. Please choose a different one.")
+      raise ValidationError('That username is taken. Please choose a different one.')
       
   def validate_email(self, email):
     user = User.query.filter_by(email=email.data).first()
     if user:
-      raise ValidationError("That email is taken. Please choose a different one.")
+      raise ValidationError('That email is taken. Please choose a different one.')
       
 
 class LoginForm(FlaskForm):
-  username = StringField("Username", validators=[DataRequired(), Length(min=2, max=20)])
-  password = PasswordField("Password", validators=[DataRequired(), Length(min=6)])
+  username = StringField('Username', validators=[DataRequired(), Length(min=2, max=20)])
+  password = PasswordField('Password', validators=[DataRequired(), Length(min=6)])
   
   
 class ChangePasswordForm(FlaskForm):
-  old_password = PasswordField("Old Password", validators=[DataRequired(), Length(min=6)])
-  password1 = PasswordField("Password", validators=[DataRequired(), Length(min=6)])
-  password2 = PasswordField("Confirm Password", validators=[DataRequired(), EqualTo("password1"), Length(min=6)])
+  old_password = PasswordField('Old Password', validators=[DataRequired(), Length(min=6)])
+  password1 = PasswordField('Password', validators=[DataRequired(), Length(min=6)])
+  password2 = PasswordField('Confirm Password', validators=[DataRequired(), EqualTo('password1'), Length(min=6)])
```

### Comparing `sakyum-0.0.7/sakyum/auth/models.py` & `sakyum-0.0.8/sakyum/auth/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# from sakyum software, your (schoolsite) project auth models.py file
+# -*- coding: utf-8 -*-
+
 from datetime import datetime
 from sakyum.contrib import db, login_manager
 from flask_login import UserMixin
 
 
 @login_manager.user_loader
 def load_user(user_id):
@@ -21,20 +22,20 @@
   is_admin = db.Column(db.Boolean, default=False)
 
   def is_active(self):
     """True, as all users are active."""
     return True
 
   def get_id(self):
-    """Return the user id to satisfy Flask-Login's requirements."""
+    """Return the user id to satisfy Flask-Login`s requirements."""
     return self.id
 
   def is_authenticated(self):
     """Return True if the user is authenticated."""
     return self.authenticated
 
   def is_anonymous(self):
-    """False, as anonymous users aren't supported."""
+    """False, as anonymous users aren`t supported."""
     return False
 
   def __repr__(self):
-    return f"User('{self.username}', '{self.email}'"
+    return f'User(\'{self.username}\', \'{self.email}\')'
```

### Comparing `sakyum-0.0.7/sakyum/auth/routes.py` & `sakyum-0.0.8/sakyum/auth/routes.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,169 +1,171 @@
-# from sakyum software, your (schoolsite) project auth routes.py file
+# -*- coding: utf-8 -*-
+
 import os
 import secrets
 from werkzeug.utils import secure_filename
 from flask import render_template, request, redirect, url_for, flash, send_from_directory, send_file
 from flask_login import login_user, current_user, logout_user, fresh_login_required, login_required
 from sakyum.utils import footer_style
 from sakyum.blueprint import auth
 from sakyum.contrib import db, bcrypt
 from .models import User
 from .forms import LoginForm, ChangePasswordForm, RegisterForm
 
 
-upload_folder = os.environ.get("FLASK_UPLOAD_FOLDER")
-origin_path = os.environ.get("FLASK_ORIGIN_PATH")
-allowed_extensions = os.environ.get("FLASK_ALLOWED_EXTENSIONS")
+OS_SEP = os.path.sep # platform-specific path separator (for linux `/`, for windows `\\`)
+UPLOAD_FOLDER = os.environ.get('FLASK_UPLOAD_FOLDER')
+ORIGIN_PATH = os.environ.get('FLASK_ORIGIN_PATH')
+ALLOWED_EXTENSIONS = os.environ.get('FLASK_ALLOWED_EXTENSIONS')
 
 
-@auth.route("/admin/register/", methods=["POST", "GET"])
+@auth.route('/admin/register/', methods=['POST', 'GET'])
 @login_required
 def adminRegister():
   form = RegisterForm()
   if form.validate_on_submit():
     username  = form.username.data
     email  = form.email.data
     raw_password2 = form.confirm_password.data
-    hashed_password = bcrypt.generate_password_hash(raw_password2).decode("utf-8")
+    hashed_password = bcrypt.generate_password_hash(raw_password2).decode('utf-8')
     user = User(username=username, email=email, password=hashed_password)
     db.session.add(user)
     db.session.commit()
-    flash("Your created new user, the user is able to log in", "success")
-    return redirect(url_for("auth.adminLogin"))
+    flash('Your created new user, the user is able to log in', 'success')
+    return redirect(url_for('auth.adminLogin'))
   context = {
-    "head_title": "admin register",
-    "footer_style": footer_style,
-    "form": form,
+    'head_title': 'admin register',
+    'footer_style': footer_style,
+    'form': form,
   }
-  return render_template("admin_register.html", context=context)
+  return render_template('admin_register.html', context=context)
   
 
-@auth.route("/admin/login/", methods=["POST", "GET"])
+@auth.route('/admin/login/', methods=['POST', 'GET'])
 def adminLogin():
   if current_user.is_authenticated:
-    return redirect(url_for("base.index"))
+    return redirect(url_for('base.index'))
   form = LoginForm()
   if form.validate_on_submit():
     username = form.username.data
     password = form.password.data
     user = User.query.filter_by(username=username).first()
     if user and bcrypt.check_password_hash(user.password, password):
       login_user(user, remember=True)
-      flash("You are now logged in!", "success")
-      next_page = request.args.get("next")
-      return redirect(next_page) if next_page else redirect(url_for("admin.index"))
+      flash('You are now logged in!', 'success')
+      next_page = request.args.get('next')
+      return redirect(next_page) if next_page else redirect(url_for('admin.index'))
     else:
-      flash("Login Unsuccessful. Please check username and password", "error")
+      flash('Login Unsuccessful. Please check username and password', 'error')
   context = {
-    "head_title": "admin login",
-    "footer_style": footer_style,
-    "form": form,
+    'head_title': 'admin login',
+    'footer_style': footer_style,
+    'form': form,
   }
-  return render_template("admin_login.html", context=context)
+  return render_template('admin_login.html', context=context)
   
 
-@auth.route("/admin/change/password/", methods=["POST", "GET"])
+@auth.route('/admin/change/password/', methods=['POST', 'GET'])
 @fresh_login_required
 def adminChangePassword():
   """
-    the `admin_change_password.html` below is located in the sakyum package (templates/default_page/admin_change_password.html)
+  The `admin_change_password.html` below is located in the sakyum package (templates/default_page/admin_change_password.html)
   """
   form = ChangePasswordForm()
-  if request.method == "POST":
+  if request.method == 'POST':
     old_password = form.old_password.data
     password1 = form.password1.data
     password2 = form.password2.data
     user = User.query.filter_by(username=current_user.username).first()
     if user and bcrypt.check_password_hash(user.password, old_password):
       if password1 == password2:
-        hashed_password = bcrypt.generate_password_hash(password2).decode("utf-8")
+        hashed_password = bcrypt.generate_password_hash(password2).decode('utf-8')
         user.password = hashed_password
         db.session.commit()
         logout_user()
-        flash("Your password has changed!", "succes")
-        return redirect(url_for("auth.adminLogin"))
+        flash('Your password has changed!', 'succes')
+        return redirect(url_for('auth.adminLogin'))
       else:
-        flash("The two password fields didn't match!", "error")
+        flash('The two password fields didn`t match!', 'error')
     else:
-      flash("Cross check your login credentials!", "error")
+      flash('Cross check your login credentials!', 'error')
   context = {
-    "head_title": "admin change password",
-    "footer_style": footer_style,
-    "form": form,
+    'head_title': 'admin change password',
+    'footer_style': footer_style,
+    'form': form,
   }
-  return render_template("admin_change_password.html", context=context)
+  return render_template('admin_change_password.html', context=context)
   
 
-@auth.route("/admin/logout/", methods=["POST", "GET"])
+@auth.route('/admin/logout/', methods=['POST', 'GET'])
 @login_required
 def adminLogout():
   logout_user()
-  flash("You logged out!", "info")
-  return redirect(url_for("auth.adminLogin"))
+  flash('You logged out!', 'info')
+  return redirect(url_for('auth.adminLogin'))
   
 
 def allowed_file(filename):
-  return "." in filename and filename.rsplit(".", 1)[1].lower() in allowed_extensions
+  return '.' in filename and filename.rsplit('.', 1)[1].lower() in ALLOWED_EXTENSIONS
   
 
-@auth.route("/profile_image/<path:filename>")
+@auth.route('/profile_image/<path:filename>')
 @login_required
 def profile_image(filename):
   """
-  this function help to show current user profile image, it won't download it
+  This function help to show current user profile image, it won't download it
   like the `download_file` function below does
   """
-  return send_file(upload_folder + "/" + filename)
+  return send_file(UPLOAD_FOLDER + OS_SEP + filename)
   
 
-@auth.route("/media/<path:filename>")
+@auth.route('/media/<path:filename>')
 @login_required
 def download_file(filename):
   """
-  if we use this to show current user profile image, it won't show instead it will download it,
+  If we use this to show current user profile image, it won't show instead it will download it,
   so it meant for downloading media file
   """
-  return send_from_directory(upload_folder, filename, as_attachment=True)
+  return send_from_directory(UPLOAD_FOLDER, filename, as_attachment=True)
   
 
 def picture_name(pic_name):
   random_hex = secrets.token_hex(8)
   _, f_ext = os.path.splitext(pic_name)
   picture_fn = random_hex + f_ext
-  new_name = _ + "_" + picture_fn
+  new_name = _ + '_' + picture_fn
   return new_name
   
 
-@auth.route("/admin/change_profile_image/", methods=["POST", "GET"])
+@auth.route('/admin/change_profile_image/', methods=['POST', 'GET'])
 @login_required
 def changeProfileImage():
-  if request.method == "POST":
+  if request.method == 'POST':
     # check if the post request has the file part
-    if "file" not in request.files:
-      flash("No file part")
+    if 'file' not in request.files:
+      flash('No file part')
       return redirect(request.url)
-    file = request.files["file"]
+    file = request.files['file']
     # If the user does not select a file, the browser submits an
     # empty file without a filename.
-    if file.filename == "":
-      flash("No selected file")
+    if file.filename == '':
+      flash('No selected file')
       return redirect(request.url)
     if file and allowed_file(file.filename):
       filename = secure_filename(file.filename)
       file_name = picture_name(filename)
-      file.save(os.path.join(upload_folder, file_name))
+      file.save(os.path.join(UPLOAD_FOLDER, file_name))
       user = User.query.filter_by(username=current_user.username).first()
       if user:
-        if user.user_img != "default_img.png":
-          r = str(origin_path) + "/media/" + user.user_img
+        if user.user_img != 'default_img.png':
+          r = str(ORIGIN_PATH) + OS_SEP + 'media' + OS_SEP + user.user_img
           if os.path.exists(r):
             os.remove(r)
         user.user_img = file_name
         db.session.commit()
-      flash("Your profile image has been changed!", "success")
-      return redirect(url_for("base.index")) # it will redirect to the home page
+      flash('Your profile image has been changed!', 'success')
+      return redirect(url_for('base.index')) # it will redirect to the home page
   context = {
-    "head_title": "admin change profile image",
-    "footer_style": footer_style,
+    'head_title': 'admin change profile image',
+    'footer_style': footer_style,
   }
-  return render_template("admin_change_profile_image.html", context=context)
+  return render_template('admin_change_profile_image.html', context=context)
```

### Comparing `sakyum-0.0.7/sakyum/base.py` & `sakyum-0.0.8/sakyum/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
 
 import os
 import sys
 import shlex
 import logging
 import argparse
+import platform
 import subprocess as sp
 
 from pathlib import Path
 
 from .mute import thunder_dummy
 from .mute.page import _js
 from .mute.page import _css
@@ -32,312 +33,346 @@
   DEBUG     ---  10
   INFO      ---  20
   WARNING   ---  30  (default)
   ERROR     ---  40
   CRITICAL  ---  50
 """
 
-formatter = "[+] [%(asctime)s] [%(levelname)s] %(message)s"
+formatter = '[+] [%(asctime)s] [%(levelname)s] %(message)s'
 logging.basicConfig(format = formatter)
-logger = logging.getLogger(__name__)
-logger.setLevel(logging.DEBUG)
+LOGGER = logging.getLogger(__name__)
+LOGGER.setLevel(logging.DEBUG)
 
 # used for relative path to default image to copy for a project (only)
 ORIGIN = Path(__file__).resolve().parent
+OS_SEP = os.path.sep # platform-specific path separator (for linux `/`, for windows `\\`)
 
 
 class BaseStructure:
   """base structure class"""
 
   def __init__(self, is_software=True):
     """base structure class initializer"""
     self.is_software = is_software
-    self.fls_cmd = "touch"
-    self._exs_first = ["index", "style"]
-    self._exs_last = [".html", ".css", ".js"]
+    self.fls_cmd = 'touch'
+    self._exs_first = ['index', 'style']
+    self._exs_last = ['.html', '.css', '.js']
     
 
-  def append_exs_to_file(self, fls_name=False, _exs_=".py", name=None):
-    """append .py extension for files if _exs_ value is ".py" or type is str, else if _exs_ type is list, make list of static files `["index.html", "index.js", "style.css"]` """
+  def append_exs_to_file(self, fls_name=False, _exs_='.py', name=None):
+    """
+    append .py extension for files if _exs_ value is '.py' or type is str, else if _exs_ type is list, make list of static files `['index.html', 'index.js', 'style.css']`
+    """
 
     if type(_exs_) == list:
       name, exst = self._exs_first, self._exs_last
       lst = []
       
       for i in exst:
         if i == exst[1]: # css
           idx = name[1]
-          lst.append(f"{idx}{i}")
+          lst.append(f'{idx}{i}')
         if i == exst[0] or i == exst[2]: # html & js
           for j in exst:
             if j != exst[1]:
               idx = name[0]
-              if f"{idx}{j}" in lst:
+              if f'{idx}{j}' in lst:
                 pass
               else:
-                lst.append(f"{idx}{j}")
+                lst.append(f'{idx}{j}')
       return lst
     if type(_exs_) == str:
-      return [i+f"{_exs_}" for i in fls_name]
+      return [i+f'{_exs_}' for i in fls_name]
       
 
-  def file_content(self, _exs=False, content=None, file_name="index", dir_togo=None, route_go=True):
+  def file_content(self, _exs=False, content=None, file_name='index', dir_togo=None, route_go=True):
     """insert content in a file"""
     if _exs:
-      with open(f"{file_name}{_exs}", "w") as pay_fls:
-        pay_fls.write(f"{content}")
+      with open(f'{file_name}{_exs}', 'w') as pay_fls:
+        pay_fls.write(f'{content}')
     else:
-      with open(f"{file_name}", "w") as pay_fls:
-        pay_fls.write(f"{content}")
+      with open(f'{file_name}', 'w') as pay_fls:
+        pay_fls.write(f'{content}')
     if route_go:
       os.chdir(dir_togo)
 
 
   def instanciate_default_img(self):
     """instanciate user default image"""
-    with open(str(ORIGIN) + "/static/default_style/media/default_img.png", mode="rb") as img_read:
+    file_path = os.path.join(ORIGIN, 'static', 'default_style', 'media', 'default_img.png')
+    with open(file_path, mode='rb') as img_read:
       img_read_data = img_read.read()
-    with open("default_img.png", mode="wb") as img_write:
+    with open('default_img.png', mode='wb') as img_write:
       img_write.write(img_read_data)
       
 
   def file_opt(self, _dir, tree=True, _here=False, _where=False):
-    """make dir tree if `tree=True` and get into it, if `_here` or `_where` is equal to True"""
+    """
+    make dir tree if `tree=True` and get into it, if `_here` or `_where` is equal to True
+    """
+
+    # we can use any of the below three variables to make our code compatible with many OS
+    os_name = os.name # nt or posix
+    platform_name_1 = sys.platform # win32 or linux or darwin or android
+    platform_name_2 = platform.system() # Windows, Darwin, Linux, etc.
+
     if tree:
-      sp.run(["mkdir", "-p", _dir])
+      if os_name == 'nt':
+      # if platform_name_1 == 'win32':
+      # if platform_name_2 == 'Windows':
+        os.makedirs(_dir, exist_ok=True)
+        # The exist_ok=True argument ensures that the function
+        # does not raise an exception if the directory already exists.
+      elif os_name == 'posix':
+      # elif platform_name_1 == 'linux' or platform_name_1 == 'darwin' or platform_name_1 == 'android':
+      # elif platform_name_2 == 'Linux' or platform_name_2 == 'Darwin':
+        sp.run(['mkdir', '-p', _dir])
+      else:
+        err_compt = f'{__title__.capitalize()} v{__version__} is not compatible with your OS'
+        print()
+        LOGGER.error(err_compt)
+        print()
+        exit()
     if _here:
       os.chdir(os.path.join(_here, _dir))
     if _where:
       os.chdir(_where)
 
 
   def validateProjectOrAppName(self, name, type_of=False):
     """validate project or app name"""
     if type_of:
-      proj_or_app = "project"
+      proj_or_app = 'project'
     else:
-      proj_or_app = "app"
-    un_accept_char = "@-/\\^+#&*!=%$?.>'<,'\";:`~|}{][)("
+      proj_or_app = 'app'
+    un_accept_char = '@-/\\^+#&*!=%$?.>\'<,"\';:`~|}{][)('
     for i in un_accept_char:
       if i in name:
-        name_err = f"[{un_accept_char}] are characters that are not allowed to be in your {proj_or_app} name, we found `{i}` in the name ({name})\n"
+        name_err = f'[{un_accept_char}] are characters that are not allowed to be in your {proj_or_app} name, we found `{i}` in the name ({name})\n'
         print()
-        logger.error(name_err)
+        LOGGER.error(name_err)
         exit()
       
 
   def into_file(self, fls, fls_cmd, file=None, app_default_dummy=None, is_static_file=False, is_app=False, proj_nm=None):
-    """create files within current directory of `self.file_opt()`
+    """
+    create files within current directory of `self.file_opt()`
     is_app: if it is True, that mean it will do operation of making app files,
     else it will make for the entire project
     """
     
     if is_app:
       for _fls in fls:
-        app_name = os.getcwd().split("/")[-1]
-        sp.run(shlex.split(f"{fls_cmd} {_fls}"))
+        app_name = os.getcwd().split(OS_SEP)[-1]
+        sp.run(shlex.split(f'{fls_cmd} {_fls}'))
         if is_static_file:
           # building app default files (html, css, js)
-          self.file_content(file_name=_fls, content=f"{app_default_dummy}", route_go=False)
+          self.file_content(file_name=_fls, content=f'{app_default_dummy}', route_go=False)
         else:
           # building app default files (__init__.py, admin.py, forms.py, models.py, views.py)
-          if _fls == "__init__.py":
-            self.file_content(file_name=_fls, content=f"# from {__title__} software, your app ({app_name}) {_fls} file\n{app_init_dummy()}", route_go=False)
-          elif _fls == "admin.py":
-            self.file_content(file_name=_fls, content=f"# from {__title__} software, your app ({app_name}) {_fls} file\n{app_admin_dummy()}", route_go=False)
-          elif _fls == "forms.py":
-            self.file_content(file_name=_fls, content=f"# from {__title__} software, your app ({app_name}) {_fls} file\n{app_forms_dummy()}", route_go=False)
-          elif _fls == "models.py":
-            self.file_content(file_name=_fls, content=f"# from {__title__} software, your app ({app_name}) {_fls} file\n{app_models_dummy()}", route_go=False)
-          elif _fls == "views.py":
-            self.file_content(file_name=_fls, content=f"# from {__title__} software, your app ({app_name}) {_fls} file\n{app_views_dummy(app_name)}", route_go=False)
+          if _fls == '__init__.py':
+            self.file_content(file_name=_fls, content=f'# from {__title__} software, your app ({app_name}) {_fls} file\n{app_init_dummy()}', route_go=False)
+          elif _fls == 'admin.py':
+            self.file_content(file_name=_fls, content=f'# from {__title__} software, your app ({app_name}) {_fls} file\n{app_admin_dummy()}', route_go=False)
+          elif _fls == 'forms.py':
+            self.file_content(file_name=_fls, content=f'# from {__title__} software, your app ({app_name}) {_fls} file\n{app_forms_dummy()}', route_go=False)
+          elif _fls == 'models.py':
+            self.file_content(file_name=_fls, content=f'# from {__title__} software, your app ({app_name}) {_fls} file\n{app_models_dummy()}', route_go=False)
+          elif _fls == 'views.py':
+            self.file_content(file_name=_fls, content=f'# from {__title__} software, your app ({app_name}) {_fls} file\n{app_views_dummy(app_name)}', route_go=False)
     else:
       for _fls in fls:
         if _fls[:-3] == file:
-          sp.run(shlex.split(f"{fls_cmd} {_fls}"))
+          sp.run(shlex.split(f'{fls_cmd} {_fls}'))
           self.file_content(
-            file_name=_fls,content=f"# Your project {_fls} file\n{thunder_dummy(proj_nm)}", route_go=False
+            file_name=_fls,content=f'# Your project {_fls} file\n{thunder_dummy(proj_nm)}', route_go=False
             ) # building the run module `thunder.py`
             
 
   def dir_tree(self, proj_name=None):
-    """create a directory tree where file will reserved as well as modules too"""
+    """
+    create a directory tree where file will reserved as well as modules too
+    """
     self.validateProjectOrAppName(proj_name, type_of=True)
-    dirs = [proj_name, f"{proj_name}/{proj_name}", "media", "templates", "static"]
+    dirs = [proj_name, f'{proj_name}{OS_SEP}{proj_name}', 'media', 'templates', 'static']
     
     # default files of project sub folder, except `thunder` which is for project base dir
-    fls_name = ["__init__", "config", "routes", "secret", "thunder"]
+    fls_name = ['__init__', 'config', 'routes', 'secret', 'thunder']
     fls = self.append_exs_to_file(fls_name=fls_name) # appending extensions to files
     _here = os.getcwd() # initial `cwd` where the project was e.g `Desktop`
     
     # check if the project already exist
     if os.path.exists(os.path.join(_here, proj_name)):
-      print(f"\nProject ({proj_name}) already exist in this directory\n\t" + os.path.realpath(proj_name))
-      logger.info(_here)
+      print(f'\nProject ({proj_name}) already exist in this directory\n\t' + os.path.realpath(proj_name))
+      LOGGER.info(_here)
       print()
     else:
       # making directories trees and their default files in the loop
       for _dir in dirs:
-        if _dir == dirs[0] + "/" + dirs[0]:
+        if _dir == dirs[0] + OS_SEP + dirs[0]:
           self.file_opt(_dir, _here=_here)
           # create default modules inside project sub dir
           for _fls in fls:
-            if _fls[:-3] != "thunder":
-              sp.run(shlex.split(f"{self.fls_cmd} {_fls}"))
+            if _fls[:-3] != 'thunder':
+              sp.run(shlex.split(f'{self.fls_cmd} {_fls}'))
               # building project default files (__init__.py, config.py, routes.py, secret.py)
-              if _fls == "__init__.py":
-                self.file_content(file_name=_fls, content=f"# from {__title__} software, your ({proj_name}) project {_fls} file\n{pro_init_dummy()}", route_go=False)
-              elif _fls == "config.py":
-                self.file_content(file_name=_fls, content=f"# from {__title__} software, your ({proj_name}) project {_fls} file\n{pro_config_dummy(proj_name)}", route_go=False)
-              elif _fls == "routes.py":
-                self.file_content(file_name=_fls, content=f"# from {__title__} software, your ({proj_name}) project {_fls} file\n{pro_routes_dummy(proj_name)}", route_go=False)
-              elif _fls == "secret.py":
-                self.file_content(file_name=_fls, content=f"# from {__title__} software, your ({proj_name}) project {_fls} file\n{pro_secret_dummy()}", route_go=False)
+              if _fls == '__init__.py':
+                self.file_content(file_name=_fls, content=f'# from {__title__} software, your ({proj_name}) project {_fls} file\n{pro_init_dummy()}', route_go=False)
+              elif _fls == 'config.py':
+                self.file_content(file_name=_fls, content=f'# from {__title__} software, your ({proj_name}) project {_fls} file\n{pro_config_dummy(proj_name)}', route_go=False)
+              elif _fls == 'routes.py':
+                self.file_content(file_name=_fls, content=f'# from {__title__} software, your ({proj_name}) project {_fls} file\n{pro_routes_dummy(proj_name)}', route_go=False)
+              elif _fls == 'secret.py':
+                self.file_content(file_name=_fls, content=f'# from {__title__} software, your ({proj_name}) project {_fls} file\n{pro_secret_dummy()}', route_go=False)
           os.chdir(_here)
           
 
         if _dir == dirs[0]:
           self.file_opt(_dir, _here=_here)
-          self.into_file(fls, self.fls_cmd, file="thunder", proj_nm=proj_name) # to maker thunder file
+          self.into_file(fls, self.fls_cmd, file='thunder', proj_nm=proj_name) # to maker thunder file
           project_folder = os.getcwd() # base dir path of the project (parent dir)
           
           for static_dir in dirs[3:]: # templates & static
             if static_dir == dirs[3:][0]: # templates
               self.file_opt(static_dir, _here=project_folder) # make templates dir and cd into it
               templates_folder = os.getcwd() # base dir path of templates folder
               
               # make project dir in templates and cd into it 
               self.file_opt(proj_name, _here=templates_folder)
               # create project index.html and back to templates base dir path
-              self.file_content(self._exs_last[0], content=f"<!-- @{__title__}, {proj_name} (project) index.html page -->\n"+_html("do_nothing", is_landing=True), dir_togo=templates_folder)
+              self.file_content(self._exs_last[0], content=f'<!-- @{__title__}, {proj_name} (project) index.html page -->\n'+_html('do_nothing', is_landing=True), dir_togo=templates_folder)
 
               # make project admin dir in templates and cd into it 
-              self.file_opt("admin", _here=templates_folder)
+              self.file_opt('admin', _here=templates_folder)
               # create project admin index.html and back to project base dir path
-              self.file_content(self._exs_last[0], content=f"<!-- @{__title__}, {proj_name} (project) admin index.html page -->\n"+_html("do_nothing", is_admin=True, project_name=proj_name), dir_togo=project_folder)
+              self.file_content(self._exs_last[0], content=f'<!-- @{__title__}, {proj_name} (project) admin index.html page -->\n'+_html('do_nothing', is_admin=True, project_name=proj_name), dir_togo=project_folder)
               
             if static_dir == dirs[3:][1]: # static
               self.file_opt(static_dir, _here=project_folder) # make static dir and cd into
               static_base_dir = os.getcwd() # base dir path of static folder
               
               # make project static dir and cd into, NB: `os.getcwd()` is base dir of static dir
-              self.file_opt(proj_name, _where=os.getcwd()+"/"+proj_name)
+              self.file_opt(proj_name, _where=os.getcwd()+OS_SEP+proj_name)
               # storing the project static dir path before creating any thing and cd into media
               s_p_dir = os.getcwd()
-              self.file_opt("media", _where="media") # make media dir for project
-              self.file_opt("do_nothing", tree=False, _where=s_p_dir)
+              self.file_opt('media', _where='media') # make media dir for project
+              self.file_opt('do_nothing', tree=False, _where=s_p_dir)
               """
               going back with one step, we pass `do_nothing` as a directory name here, to avoid any error even though it do nothing if we give it a real directory name
               """
 
-              self.file_content(self._exs_last[1], file_name="style", content=f"/* @{__title__}, {proj_name} (project) style.css file */\n"+_css(), route_go=False) # create style.css
+              self.file_content(self._exs_last[1], file_name='style', content=f'/* @{__title__}, {proj_name} (project) style.css file */\n'+_css(), route_go=False) # create style.css
               
               # create index.js and back to project static base dir path
-              self.file_content(self._exs_last[2], content=f"// @{__title__}, {proj_name} (project) index.js file\n"+_js(proj_name), dir_togo=project_folder)
+              self.file_content(self._exs_last[2], content=f'// @{__title__}, {proj_name} (project) index.js file\n'+_js(proj_name), dir_togo=project_folder)
               
           # make media folder and default image inside it
           self.file_opt(dirs[2], _where=dirs[2])
           self.instanciate_default_img()
           os.chdir(_here)
 
       print()
-      logger.info(f"Project ({proj_name}) created successfully!")
+      LOGGER.info(f'Project ({proj_name}) created successfully!')
       print()
       
 
 class AppStructure(BaseStructure):
   """base structure class"""
   app_store_name = None # app name
   proj_store_name = None # project name
   
   def app_static_and_template(self, file_dummy, top_comment=False, _dir_=False, file=False, app=False, cmd=False, _here_=False):
     """
-      #: _dir_ = "template or static"
-      #: file = ["index.html"]
-      #: app = app name
-      #: cmd = "touch"
-      #: _here_ = # initial `inside project folder` where the project was created
-    """
-    if top_comment == "html":
-      top_comment = f"<!-- @{__title__}, {app} {file[0]} page -->\n"
-    if top_comment == "css":
-      top_comment = f"/* @{__title__}, {app} {file[0]} file */\n"
-    if top_comment == "js":
-      top_comment = f"// @{__title__}, {app} {file[0]} file\n"
+    #: _dir_ = 'template or static'
+    #: file = ['index.html']
+    #: app = app name
+    #: cmd = 'touch'
+    #: _here_ = # initial `inside project folder` where the project was created
+    """
+    if top_comment == 'html':
+      top_comment = f'<!-- @{__title__}, {app} {file[0]} page -->\n'
+    if top_comment == 'css':
+      top_comment = f'/* @{__title__}, {app} {file[0]} file */\n'
+    if top_comment == 'js':
+      top_comment = f'// @{__title__}, {app} {file[0]} file\n'
       
     self.file_opt(_dir_, tree=False, _here=_here_) # back to template dir
-    self.file_opt(f"{app}", _where=app) # make app dir inside `template`
-    self.into_file(file, cmd, is_static_file=True, app_default_dummy=f"{top_comment}{file_dummy}", is_app=True) # making app default file
+    self.file_opt(f'{app}', _where=app) # make app dir inside `template`
+    self.into_file(file, cmd, is_static_file=True, app_default_dummy=f'{top_comment}{file_dummy}', is_app=True) # making app default file
     
     
   def dir_tree(self, proj_app_name=None):
-    """create a directory tree where file will reserved as well as modules too"""
+    """
+    create a directory tree where file will reserved as well as modules too
+    """
     dirs = [proj_app_name]
     self.validateProjectOrAppName(proj_app_name)
 
     app_store_name = proj_app_name # store our app name
-    fls_name = ["__init__", "views", "models", "forms", "admin"]
+    fls_name = ['__init__', 'views', 'models', 'forms', 'admin']
     fls = self.append_exs_to_file(fls_name=fls_name)
-    roove_dir = ["templates", "static", "static"]
+    roove_dir = ['templates', 'static', 'static']
     _here_app = os.getcwd()  # initial `inside project folder` (parent) directory
     
     # check if the app already exist
-    app_proj_name = _here_app.split("/")[-1]
+    app_proj_name = _here_app.split(OS_SEP)[-1]
     self.proj_store_name = app_proj_name
 
     if os.path.exists(os.path.join(_here_app, proj_app_name)):
-      print(f"\nApp ({proj_app_name}) already exist in this project ({app_proj_name})\n\t" + os.path.realpath(proj_app_name))
-      logger.info(_here_app)
+      print(f'\nApp ({proj_app_name}) already exist in this project ({app_proj_name})\n\t' + os.path.realpath(proj_app_name))
+      LOGGER.info(_here_app)
       print()
     else:
       # making directories trees and their default files
       for _dir in dirs:
         if _dir == dirs[0]:
           self.file_opt(_dir, _here=_here_app)
           self.into_file(fls, self.fls_cmd, is_app=True) # to maker app default files
           
       self.app_static_and_template(
-        _html(app_store_name, project_name=self.proj_store_name, is_base_app=True), top_comment="html", _dir_=roove_dir[0], file=[self.append_exs_to_file(_exs_=[])[0]], app=proj_app_name, cmd=self.fls_cmd, _here_=_here_app
+        _html(app_store_name, project_name=self.proj_store_name, is_base_app=True), top_comment='html', _dir_=roove_dir[0], file=[self.append_exs_to_file(_exs_=[])[0]], app=proj_app_name, cmd=self.fls_cmd, _here_=_here_app
         )
       self.app_static_and_template(
-        _css(), top_comment="css", _dir_=roove_dir[1], file=[self.append_exs_to_file(_exs_=[])[2]], app=proj_app_name, cmd=self.fls_cmd, _here_=_here_app
+        _css(), top_comment='css', _dir_=roove_dir[1], file=[self.append_exs_to_file(_exs_=[])[2]], app=proj_app_name, cmd=self.fls_cmd, _here_=_here_app
         )
       self.app_static_and_template(
-        _js(proj_app_name), top_comment="js", _dir_=roove_dir[2], file=[self.append_exs_to_file(_exs_=[])[1]], app=proj_app_name, cmd=self.fls_cmd, _here_=_here_app
+        _js(proj_app_name), top_comment='js', _dir_=roove_dir[2], file=[self.append_exs_to_file(_exs_=[])[1]], app=proj_app_name, cmd=self.fls_cmd, _here_=_here_app
         )
-      self.file_opt("media") # an app media folder
-      self.file_opt("do_nothing", tree=False, _where=_here_app) # back to project dir
+      self.file_opt('media') # an app media folder
+      self.file_opt('do_nothing', tree=False, _where=_here_app) # back to project dir
       print()
-      logger.info(f"App ({proj_app_name}) created successfully! in {app_proj_name}")
+      LOGGER.info(f'App ({proj_app_name}) created successfully! in {app_proj_name}')
       print()
       
 
 def app_init(app):
   """initialize app in project"""
   AppStructure().dir_tree(app)
   exit()
   
 
 class Boot:
-  """boot up project operation, app operation, and the server"""
+  """
+  boot up project operation, app operation, and the server
+  """
   def __init__(self, p=None, d=False, h=None, db=db, model=User, pwd_hash=bcrypt):
     self.p = p # port
     self.d = d # debug
     self.h = h # host
     self.db = db # database
     self.model = model
     self.pwd_hash = pwd_hash
 
   def run(self):
     """run method for creating app and booting up server"""
     
-    error_ref_1 = f"""\n Run the command with one of this positional arguments:\n\tcreate_app   ---   ( for creating an app within your project )\n\tboot  ---   ( for booting up your server )"""
+    error_ref_1 = f'''\n Run the command with one of this positional arguments:\n\tcreate_app   ---   ( for creating an app within your project )\n\tboot  ---   ( for booting up your server )'''
 
-    error_ref_2 = f"""
- create_app:
+    error_ref_2 = f'''
+  create_app:
     usage: create_app [-h] --app  [--debug]
 
     This create an app in your project
 
     positional arguments:
                     Put positional argument of `create_app` to create app, app are create inside your project
 
@@ -354,74 +389,74 @@
 
     options:
       -h, --help        show this help message and exit
       --username , -u   What is the username?
       --email , -e      What is the email?
       --password , -p   What is the password?
 
- boot:
+  boot:
     usage: boot up server [-h] [--port] [--host] [--debug]
 
     This boot up the server
 
     positional arguments:
                     Put positional argument of `boot` to bring server up running
 
     optional arguments:
       -h, --help     show this help message and exit
       --port , -p    What is the port number?
       --host , -H    What is the host?
-      --debug , -d   Do you want debug?"""
+      --debug , -d   Do you want debug?'''
     if len(sys.argv) == 1:
       print()
-      logger.error(f"please run the module with positional argument and flag if needed\n{error_ref_1}")
+      LOGGER.error(f'please run the module with positional argument and flag if needed\n{error_ref_1}')
       exit()
 
-    if sys.argv[1] == "create_app":
+    if sys.argv[1] == 'create_app':
       # prog is the name of the program, default=sys.argv[0]
-      parser = argparse.ArgumentParser(prog="create_app", description="This create an app in your project")
+      parser = argparse.ArgumentParser(prog='create_app', description='This create an app in your project')
       # metavar make the -help to look cleaan
-      parser.add_argument("--app", "-a", required=True, type=str, metavar="", help="What is the app name")
-      parser.add_argument(dest="create_app", default="create_app", type=str, metavar="", help="Put positional argument of `create_app` to create app, app are create inside your project")
+      parser.add_argument('--app', '-a', required=True, type=str, metavar='', help='What is the app name')
+      parser.add_argument(dest='create_app', default='create_app', type=str, metavar='', help='Put positional argument of `create_app` to create app, app are create inside your project')
       args = parser.parse_args()
-      the_proj = os.getcwd().split("/")[-1]
+      the_proj = os.getcwd().split(OS_SEP)[-1]
       
       if args.app.lower() == __title__:
         print()
-        logger.error(f"Not allowed to use ({__title__}) package name as an app name\n")
+        LOGGER.error(f'Not allowed to use ({__title__}) package name as an app name\n')
         exit()
       elif args.app == the_proj:
         print()
-        logger.error(f"Not allowed to use your ({the_proj}) project name as an app name\n")
+        LOGGER.error(f'Not allowed to use your ({the_proj}) project name as an app name\n')
         exit()
       app_init(args.app)
 
-    elif sys.argv[1] == "boot":
-      parser = argparse.ArgumentParser(prog="boot up server", description="This boot up the server")
-      parser.add_argument("--port", "-p", default=5000, required=False, type=int, metavar="", help="What is the port number?")
-      parser.add_argument("--host", "-H", default=self.h, required=False, type=str, metavar="", help="What is the host?")
-      parser.add_argument("--debug", "-d", default=False, required=False, type=bool, metavar="", help="Do you want debug?")
-      parser.add_argument(dest="boot", default="boot", type=str, metavar="", help="Put positional argument of `boot` to bring server up running")
+    elif sys.argv[1] == 'boot':
+      parser = argparse.ArgumentParser(prog='boot up server', description='This boot up the server')
+      parser.add_argument('--port', '-p', default=5000, required=False, type=int, metavar='', help='What is the port number?')
+      parser.add_argument('--host', '-H', default=self.h, required=False, type=str, metavar='', help='What is the host?')
+      parser.add_argument('--debug', '-d', default=False, required=False, type=bool, metavar='', help='Do you want debug?')
+      parser.add_argument(dest='boot', default='boot', type=str, metavar='', help='Put positional argument of `boot` to bring server up running')
       args = parser.parse_args()
       self.p = args.port
       self.h = args.host
-      if os.environ.get("FLASK_DEBUG") and os.environ.get("FLASK_DEBUG") == "1":
+      if os.environ.get('FLASK_DEBUG') and os.environ.get('FLASK_DEBUG') == '1':
         self.d = True
-        logger.info(" * You have set an environment variable of `FLASK_DEBUG` to '1'")
+        LOGGER.info(' * You have set an environment variable of `FLASK_DEBUG` to \'1\'')
       else:
         self.d = args.debug
       
-      # logger.info(f"@{__title__} v{__version__} | visit: http://localhost:{args.port} (for development)")
+      # LOGGER.info(f'@{__title__} v{__version__} | visit: http://localhost:{args.port} (for development)')
       
-    elif sys.argv[1] == "create_user":
-      parser = argparse.ArgumentParser(prog="create user", description="This create user")
-      parser.add_argument("--username", "-u", required=False, type=str, metavar="", help="What is the username?")
-      parser.add_argument("--email", "-e", required=False, type=str, metavar="", help="What is the email?")
-      parser.add_argument("--password", "-p", required=False, type=str, metavar="", help="What is the password?")
-      parser.add_argument(dest="create_user", default="create_user", type=str, metavar="", help="Put positional argument of `create_user` to create user")
+    elif sys.argv[1] == 'create_user':
+      parser = argparse.ArgumentParser(prog='create user', description='This create user')
+      parser.add_argument('--username', '-u', required=False, type=str, metavar='', help='What is the username?')
+      parser.add_argument('--email', '-e', required=False, type=str, metavar='', help='What is the email?')
+      parser.add_argument('--password', '-p', required=False, type=str, metavar='', help='What is the password?')
+      parser.add_argument(dest='create_user', default='create_user', type=str, metavar='', help='Put positional argument of `create_user` to create user')
       args = parser.parse_args()
 
       from .utils import AuthCredentials
       if args.username != None:
         args_u = False
         usr = args.username
       else:
@@ -442,18 +477,18 @@
         
       auth_class = AuthCredentials(username=usr, email=mail, password=pwd, u_args=args_u, e_args=args_e, p_args=args_p)
       auth_result = auth_class.result
       username = auth_result[0]
       email = auth_result[1]
       raw_password = auth_result[2]
 
-      hashed_password = self.pwd_hash.generate_password_hash(raw_password).decode("utf-8")
+      hashed_password = self.pwd_hash.generate_password_hash(raw_password).decode('utf-8')
       user = self.model(username=username, email=email, password=hashed_password, is_admin=True)
       self.db.session.add(user)
       self.db.session.commit()
       print()
-      logger.info(f"One user record added ({username})\n")
+      LOGGER.info(f'One user record added ({username})\n')
       exit()
     else:
       print()
-      logger.error(f"use a valid positional argument and flag if needed\n{error_ref_2}")
+      LOGGER.error(f'use a valid positional argument and flag if needed\n{error_ref_2}')
       exit()
```

### Comparing `sakyum-0.0.7/sakyum/blueprint.py` & `sakyum-0.0.8/sakyum/blueprint.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,131 +8,143 @@
 # static_url_path: the URL to serve static files from
 # template_folder: the folder containing the Blueprint's templates
 # url_prefix: the path to prepend to all of the Blueprint's URLs
 # subdomain: the subdomain that this Blueprint's routes will match on by default
 # url_defaults: a dictionary of default values that this Blueprint's views will receive
 # root_path: the Blueprint's root dictionary path, whose default values is obtained from the Blueprint's import
 
-default = Blueprint("default", __name__, template_folder=template_dir(temp_from_pkg="default_page"), static_folder=static_dir("default_style", static_from_pkg=True))
-errors = Blueprint("errors", __name__, template_folder=template_dir(temp_from_pkg="default_errors"))
-auth = Blueprint("auth", __name__, template_folder=template_dir(temp_from_pkg="default_page"))
+default = Blueprint('default', __name__, template_folder=template_dir(temp_from_pkg='default_page'), static_folder=static_dir('default_style', static_from_pkg=True))
+errors = Blueprint('errors', __name__, template_folder=template_dir(temp_from_pkg='default_errors'))
+auth = Blueprint('auth', __name__, template_folder=template_dir(temp_from_pkg='default_page'))
+
+
+"""
+The `default` blueprint above is the blueprint that is been used by sakyum for linking
+it default pages (css, js, and favicon.ico) files and also it can be use for our project
+default html pages (landing page route) that is located in your project route.py file
+`<project_name>/route.py` like ` @default.route() `, but instead we use ` @base.route() `
+for that `<project_name>/routes.py` as default. We also register it in the project routes.py
+file `reg_blueprints` list to make it accessible
+
+The `errors` blueprint above is for error pages, you can overite the error pages by
+defining them in your project routes.py file `<project_name>/route.py` just like the
+way we did in here down below for some of our default error pages (400, 403, 500, etc)
+by giving your desire template file path (correspond to your project templates folder)
+for each error page
+
+The `auth` blueprint above is for the `login, logout, register, change_password` and
+other default authentication system (route) of your project, which will let you log into admin page
+"""
 
 
 def adminModelRegister(admin, reg_models, db):
   """function that will register a direct model (not model view)"""
   for reg_model in reg_models:
     admin.add_view(ModelView(reg_model, db.session))
     
-"""
-  the `default` blueprint above is the blueprint that is been used by sakyum for linking
-  it default pages (css, js, and favicon.ico) files and also it can be use for our project
-  default html pages (landing page route) that is located in your project route.py file
-  `<project_name>/route.py` like ` @default.route() `, but instead we use ` @base.route() `
-  for that `<project_name>/routes.py` as default. We also register it in the project routes.py
-  file `reg_blueprints` list to make it accessible
-
-  the `errors` blueprint above is for error pages, you can overite the error pages by
-  defining them in your project routes.py file `<project_name>/route.py` just like the
-  way we did in here down below for some of our default error pages (400, 403, 500, etc)
-  by giving your desire template file path (correspond to your project templates folder)
-  for each error page
-
-  the `auth` blueprint above is for the `login, logout, register, change_password` and
-  other default authentication system (route) of your project, which will let you log into admin page
-"""
-
 
 @errors.app_errorhandler(400)
 def error_400(error):
   context = {
-    "head_title": "error page",
-    "footer_style": footer_style,
+    'head_title': 'error page',
+    'footer_style': footer_style,
   }
-  return render_template("400.html", context=context), 400
+  return render_template('400.html', context=context), 400
+
 
 @errors.app_errorhandler(401)
 def error_401(error):
   context = {
-    "head_title": "error page",
-    "footer_style": footer_style,
+    'head_title': 'error page',
+    'footer_style': footer_style,
   }
-  return render_template("401.html", context=context), 401
+  return render_template('401.html', context=context), 401
+
 
 @errors.app_errorhandler(403)
 def error_403(error):
   context = {
-    "head_title": "error page",
-    "footer_style": footer_style,
+    'head_title': 'error page',
+    'footer_style': footer_style,
   }
-  return render_template("403.html", context=context), 403
+  return render_template('403.html', context=context), 403
+
 
 @errors.app_errorhandler(404)
 def error_404(error):
   context = {
-    "head_title": "error page",
-    "footer_style": footer_style,
+    'head_title': 'error page',
+    'footer_style': footer_style,
   }
-  return render_template("404.html", context=context), 404
+  return render_template('404.html', context=context), 404
+
 
 @errors.app_errorhandler(406)
 def error_406(error):
   context = {
-    "head_title": "error page",
-    "footer_style": footer_style,
+    'head_title': 'error page',
+    'footer_style': footer_style,
   }
-  return render_template("406.html", context=context), 406
+  return render_template('406.html', context=context), 406
+
 
 @errors.app_errorhandler(415)
 def error_415(error):
   context = {
-    "head_title": "error page",
-    "footer_style": footer_style,
+    'head_title': 'error page',
+    'footer_style': footer_style,
   }
-  return render_template("415.html", context=context), 415
+  return render_template('415.html', context=context), 415
+
 
 @errors.app_errorhandler(429)
 def error_429(error):
   context = {
-    "head_title": "error page",
-    "footer_style": footer_style,
+    'head_title': 'error page',
+    'footer_style': footer_style,
   }
-  return render_template("429.html", context=context), 429
+  return render_template('429.html', context=context), 429
+
 
 @errors.app_errorhandler(500)
 def error_500(error):
   context = {
-    "head_title": "error page",
-    "footer_style": footer_style,
+    'head_title': 'error page',
+    'footer_style': footer_style,
   }
-  return render_template("500.html", context=context), 500
+  return render_template('500.html', context=context), 500
+
 
 @errors.app_errorhandler(501)
 def error_501(error):
   context = {
-    "head_title": "error page",
-    "footer_style": footer_style,
+    'head_title': 'error page',
+    'footer_style': footer_style,
   }
-  return render_template("501.html", context=context), 501
+  return render_template('501.html', context=context), 501
+
 
 @errors.app_errorhandler(502)
 def error_502(error):
   context = {
-    "head_title": "error page",
-    "footer_style": footer_style,
+    'head_title': 'error page',
+    'footer_style': footer_style,
   }
-  return render_template("502.html", context=context), 502
+  return render_template('502.html', context=context), 502
+
 
 @errors.app_errorhandler(503)
 def error_503(error):
   context = {
-    "head_title": "error page",
-    "footer_style": footer_style,
+    'head_title': 'error page',
+    'footer_style': footer_style,
   }
-  return render_template("503.html", context=context), 503
+  return render_template('503.html', context=context), 503
+
 
 @errors.app_errorhandler(504)
 def error_504(error):
   context = {
-    "head_title": "error page",
-    "footer_style": footer_style,
+    'head_title': 'error page',
+    'footer_style': footer_style,
   }
-  return render_template("504.html", context=context), 504
+  return render_template('504.html', context=context), 504
```

### Comparing `sakyum-0.0.7/sakyum/contrib/__init__.py` & `sakyum-0.0.8/sakyum/contrib/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,18 @@
+# -*- coding: utf-8 -*-
+
 from flask_sqlalchemy import SQLAlchemy
 from flask_login import LoginManager
 from flask_bcrypt import Bcrypt
 from flask_wtf.csrf import CSRFProtect
 
 
 db = SQLAlchemy()
 bcrypt = Bcrypt()
 login_manager = LoginManager()
 # To enable CSRF protection globally for Flask, using secret key to securely sign the token
 csrf = CSRFProtect()
-login_manager.session_protection = "strong"
-login_manager.login_view = "auth.adminLogin"
-login_manager.login_message_category = "info"
-login_manager.login_message = u"You must login, in other to get access to that page"
+login_manager.session_protection = 'strong'
+login_manager.login_view = 'auth.adminLogin'
+login_manager.login_message_category = 'info'
+login_manager.login_message = u'You must login, in other to get access to that page'
 ext_lst = [db, bcrypt, login_manager, csrf]
```

### Comparing `sakyum-0.0.7/sakyum/mute/__init__.py` & `sakyum-0.0.8/sakyum/mute/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,30 +3,30 @@
 from sakyum import __title__
 from sakyum.utils import Security
 from sakyum.utils import stylePage
 
 
 secret = Security()
 secure_app = secret.passcode_salt
-f1 = "{"
-l1 = "}"
-f2 = "{{"
-l2 = "}}"
-long_comment = "\"\"\""
+f1 = '{'
+l1 = '}'
+f2 = '{{'
+l2 = '}}'
+long_comment = '"""'
 
 
 def thunder_dummy(project):
   return f"""from sakyum import Boot
 from {project}.routes import reg_blueprints
 from {project}.config import create_app
 from {project}.secret import load_env
 
 
 load_env()
 boot = Boot()
-if __name__ == "__main__":
+if __name__ == '__main__':
   boot.run()
 
 
 app = create_app(reg_blueprints)
 app.run(debug=boot.d, port=boot.p, host=boot.h)
 """
```

### Comparing `sakyum-0.0.7/sakyum/mute/app.py` & `sakyum-0.0.8/sakyum/mute/app.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,32 +14,34 @@
   """app is the application name of your project"""
   return f"""from flask import (render_template, Blueprint)
 from sakyum.utils import footer_style, template_dir, static_dir
 from sakyum.contrib import db
 # from .models import <app_models>
 # from .forms import <model_form>
 
-{app} = Blueprint("{app}", __name__, template_folder=template_dir(), static_folder=static_dir("{app}"))
 
+{app} = Blueprint('{app}', __name__, template_folder=template_dir(), static_folder=static_dir('{app}'))
 
-@{app}.route('/{app}/', methods=["GET", "POST"])
+
+@{app}.route('/{app}/', methods=['GET', 'POST'])
 def index():
   context = {f1}
-    "head_title": "{app}",
-    "footer_style": footer_style,
+    'head_title': '{app}',
+    'footer_style': footer_style,
   {l1}
-  return render_template("{app}/index.html", context=context)
+  return render_template('{app}/index.html', context=context)
 """
 
 
 def app_forms_dummy():
   return f"""from flask_wtf import FlaskForm
 from wtforms import StringField, SubmitField, TextAreaField
 from wtforms.validators import DataRequired, Length
 
+
 # write your app forms here!
 """
 
 
 def app_models_dummy():
   return f"""from datetime import datetime
 from sakyum.contrib import db
@@ -54,9 +56,10 @@
 """
 
 def app_admin_dummy():
   return f"""from flask_login import current_user
 from flask import redirect, request, url_for
 from flask_admin.contrib.sqla import ModelView
 
+
 # write your app admin model view here!
 """
```

### Comparing `sakyum-0.0.7/sakyum/mute/page.py` & `sakyum-0.0.8/sakyum/mute/page.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from . import l2
 from . import __title__
 from . import stylePage
 
 
 def _html(name, is_landing=False, is_admin=False, project_name=False, is_base_app=False):
   if is_landing:
-    return f"""{f1}% extends "default_base.html" %{l1}
+    return f"""{f1}% extends 'default_base.html' %{l1}
 
 {f1}% block head_js %{l1}
   <script src="{f2} url_for('base.static', filename='index.js') {l2}"></script>
 {f1}% endblock head_js %{l1}
 """
   if is_admin:
-    return f"""{f1}% extends "admin/master.html" %{l1}
+    return f"""{f1}% extends 'admin/master.html' %{l1}
 {f1}% block body %{l1}
   <a href="/">Go to {project_name} home page</a>
   <br>
   {f1}% if current_user.is_authenticated %{l1}
     <a href="{f2} url_for('auth.adminLogout') {l2}">logout</a>
     <br>
     <a href="{f2} url_for('auth.adminRegister') {l2}">register</a>
@@ -32,15 +32,15 @@
   {f1}% else %{l1}
     <a href="{f2} url_for('auth.adminLogin') {l2}">login</a>
   {f1}% endif %{l1}
 {f1}% endblock body %{l1}
 """
   if is_base_app:
     page_desc = stylePage(name)
-    return f"""{f1}% extends "{project_name}/index.html" %{l1}
+    return f"""{f1}% extends '{project_name}/index.html' %{l1}
 
 {f1}% block head_css %{l1}
   <!-- <link rel="stylesheet" type="text/css" href="{f2} url_for('{name}.static', filename='style.css') {l2}"> -->
 {f1}% endblock head_css %{l1}
 
 {f1}% block head_js %{l1}
   <script src="{f2} url_for('{name}.static', filename='index.js') {l2}"></script>
```

### Comparing `sakyum-0.0.7/sakyum/mute/project.py` & `sakyum-0.0.8/sakyum/mute/project.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,38 +5,44 @@
 from . import secure_app
 from . import long_comment
 
 
 def pro_init_dummy():
   return f"""from .config import create_app
 
+
 app = create_app()
 """
 
 
 def pro_secret_dummy():
   return f"""import os
 from pathlib import Path
 
-origin_path = Path(__file__).resolve().parent.parent
+
+ORIGIN_PATH = Path(__file__).resolve().parent.parent
+OS_SEP = os.path.sep # platform-specific path separator (for linux `/`, for windows `\\`)
+
 
 class Config:
-  SECRET_KEY = "{secure_app}"
-  SQLALCHEMY_DATABASE_URI = "sqlite:///"+str(origin_path)+"/default.db"
+  SECRET_KEY = '{secure_app}'
+  # The `SQLALCHEMY_DATABASE_URI` might not be compatible with windows OS,
+  # change it to your windows drive like: 'C:\path\to\your\default.db'
+  SQLALCHEMY_DATABASE_URI = 'sqlite:///'+str(ORIGIN_PATH)+OS_SEP+'default.db'
   # set optional bootswatch theme
-  FLASK_ADMIN_SWATCH = "cerulean"
-  UPLOAD_FOLDER = os.path.join(origin_path, "media")
-  ALLOWED_EXTENSIONS = ("png", "jpg", "jpeg")
+  FLASK_ADMIN_SWATCH = 'cerulean'
+  UPLOAD_FOLDER = os.path.join(ORIGIN_PATH, 'media')
+  ALLOWED_EXTENSIONS = ('png', 'jpg', 'jpeg')
   MAX_CONTENT_LENGTH = 16 * 1024 * 1024
 
 
 def load_env():
-  os.environ["FLASK_UPLOAD_FOLDER"] = Config.UPLOAD_FOLDER
-  os.environ["FLASK_ORIGIN_PATH"] = str(origin_path)
-  os.environ["FLASK_ALLOWED_EXTENSIONS"] = str(Config.ALLOWED_EXTENSIONS)
+  os.environ['FLASK_UPLOAD_FOLDER'] = Config.UPLOAD_FOLDER
+  os.environ['FLASK_ORIGIN_PATH'] = str(ORIGIN_PATH)
+  os.environ['FLASK_ALLOWED_EXTENSIONS'] = str(Config.ALLOWED_EXTENSIONS)
 """
 
 
 def pro_config_dummy(proj_name):
   return f"""from flask_admin import Admin
 from flask import Flask
 from sakyum.blueprint import adminModelRegister
@@ -64,55 +70,55 @@
     for reg_blueprint in reg_blueprints:
       app.register_blueprint(reg_blueprint)
 
 
   def admin_runner():
     # Model views allow you to add a dedicated set of admin
     # pages for managing any model in your database
-    admin = Admin(app, name="{proj_name}")
+    admin = Admin(app, name='{proj_name}')
 
 
     # rgister model to admin direct by passing every model that you
     # want to manage in admin page in the below list (reg_models)
     reg_models = [
       # User,
       # <app_model>,
     ]
     adminModelRegister(admin, reg_models, db)
     # admin model view be here!
-    admin.add_view(UserAdminView(User, db.session, name="User", category="User-section"))
+    admin.add_view(UserAdminView(User, db.session, name='User', category='User-section'))
 
   admin_runner()
   return app
 """
 
 
 def pro_routes_dummy(proj):
   return f"""from flask import (render_template, Blueprint)
 from sakyum import blueprint
 from sakyum.utils import footer_style, template_dir, static_dir, rem_blueprint
 # from <app_name>.views import <app_name>
 
 
-base = Blueprint("base", __name__, template_folder=template_dir(), static_folder=static_dir("{proj}"))
+base = Blueprint('base', __name__, template_folder=template_dir(), static_folder=static_dir('{proj}'))
 
 rem_blue = [blueprint.default, blueprint.errors, blueprint.auth, base]
 reg_blueprints = [
   blueprint.default,
   blueprint.errors,
   blueprint.auth,
   base,
   # <app_name>,
 ]
 
 
-@base.route("/", methods=["POST", "GET"])
+@base.route('/', methods=['POST', 'GET'])
 def index():
   context = {f1}
-    "project_name": "{proj}",
-    "footer_style": footer_style,
-    "blueprints_list": rem_blueprint(lst_blue=reg_blueprints, rem_blue=rem_blue),
+    'project_name': '{proj}',
+    'footer_style': footer_style,
+    'blueprints_list': rem_blueprint(lst_blue=reg_blueprints, rem_blue=rem_blue),
   {l1}
-  return render_template("{proj}/index.html", context=context)
+  return render_template('{proj}/index.html', context=context)
   
 # overwrite (customise) error pages here
 """
```

### Comparing `sakyum-0.0.7/sakyum/static/default_style/css/style.css` & `sakyum-0.0.8/sakyum/static/default_style/css/style.css`

 * *Files identical despite different names*

### Comparing `sakyum-0.0.7/sakyum/static/default_style/media/alert.png` & `sakyum-0.0.8/sakyum/static/default_style/media/alert.png`

 * *Files identical despite different names*

### Comparing `sakyum-0.0.7/sakyum/static/default_style/media/default_img.png` & `sakyum-0.0.8/sakyum/static/default_style/media/default_img.png`

 * *Files identical despite different names*

### Comparing `sakyum-0.0.7/sakyum/static/default_style/media/favicon.ico` & `sakyum-0.0.8/sakyum/static/default_style/media/favicon.ico`

 * *Files identical despite different names*

### Comparing `sakyum-0.0.7/sakyum/templates/default_page/admin_change_password.html` & `sakyum-0.0.8/sakyum/templates/default_page/admin_change_password.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <!-- default admin user change password page -->
-{% extends "default.html" %}
+{% extends 'default.html' %}
 
 {% block auth %}
   <div class="pkg_desc">
     <h1>Change user password</h1>
   </div>
   <div class="admin_auth_form">
     {% if context.form %}
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
- {% extends "default.html" %} {% block auth %}
+ {% extends 'default.html' %} {% block auth %}
 ****** Change user password ******
 {% if context.form %}
 {{ context.form.csrf_token }}  {# If whether we use: {{ context.form.csrf_token
 }} or we use: {{ context.form.hidden_tag() }} all the two is thesame #} {% if
 context.form.old_password.errors %} {{ context.form.old_password
 (placeholder="Enter old password") }}  {#
 {% for error in context.form.old_password.errors %} {{ error }} {% endfor %}
```

### Comparing `sakyum-0.0.7/sakyum/templates/default_page/admin_change_profile_image.html` & `sakyum-0.0.8/sakyum/templates/default_page/admin_change_profile_image.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <!-- default admin user change profile image page -->
-{% extends "default.html" %}
+{% extends 'default.html' %}
 
 {% block auth %}
   <div class="pkg_desc">
     <h1>Change user profile image</h1>
   </div>
   <div class="admin_auth_form">
     <form method=post enctype=multipart/form-data>
```

#### html2text {}

```diff
@@ -1,5 +1,5 @@
- {% extends "default.html" %} {% block auth %}
+ {% extends 'default.html' %} {% block auth %}
 ****** Change user profile image ******
  [File] Upload
 Download_your_current_profile_image
 {% endblock auth %}
```

### Comparing `sakyum-0.0.7/sakyum/templates/default_page/admin_login.html` & `sakyum-0.0.8/sakyum/templates/default_page/admin_login.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <!-- default admin user login page -->
-{% extends "default.html" %}
+{% extends 'default.html' %}
 
 {% block auth %}
   <div class="pkg_desc">
     <h1>Login to admin</h1>
   </div>
   <div class="admin_auth_form">
     {% if context.form %}
```

### Comparing `sakyum-0.0.7/sakyum/templates/default_page/admin_register.html` & `sakyum-0.0.8/sakyum/templates/default_page/admin_register.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <!-- default user registration page (admin) -->
-{% extends "default.html" %}
+{% extends 'default.html' %}
 
 {% block auth %}
   <div class="pkg_desc">
     <h1>Register user to admin</h1>
   </div>
   <div class="admin_auth_form">
     {% if context.form %}
```

### Comparing `sakyum-0.0.7/sakyum/templates/default_page/default.html` & `sakyum-0.0.8/sakyum/templates/default_page/default.html`

 * *Files 3% similar despite different names*

```diff
@@ -39,19 +39,19 @@
           {% if current_user.is_authenticated %}
             <img src="{{ url_for('auth.profile_image', filename=current_user.user_img) }}" alt="" class="user_default_img">
           {% else %}
             <a href="https://github.com/usmanmusa1920/sakyum" class="link_0" target="_blank">Github</a>
           {% endif %}
           <a class="link_1">|</a>
           {% if current_user.is_authenticated %}
-            <a href="{{ url_for('auth.adminRegister') }}" class="link_2">register</a>
-            <a href="{{ url_for('auth.adminLogout') }}" class="link_3">logout</a>
+            <a href="{{ url_for('auth.adminRegister') }}" class="link_2">Register</a>
+            <a href="{{ url_for('auth.adminLogout') }}" class="link_3">Logout</a>
           {% else %}
             <a href="https://sakyum.readthedocs.io" class="link_2" target="_blank">Docs</a>
-            <a href="{{ url_for('auth.adminLogin') }}" class="link_3">login</a>
+            <a href="{{ url_for('auth.adminLogin') }}" class="link_3">Login</a>
           {% endif %}
           <a onclick="test()" class="alert">
             <img src="{{ url_for('default.static', filename='media/alert.png') }}" alt="">
           </a>
         </div>
       </div>
     </div>
@@ -92,25 +92,25 @@
     </div>
 
     <div class="footer_margin_top"></div>
     <div class="footer">
       <!-- the below span tag will be visible only if the page is view with small size screen -->
       <span class="auth_route_sm">
         {% if current_user.is_authenticated %}
-          <a href="{{ url_for('auth.adminRegister') }}">register</a>
-          <a href="{{ url_for('auth.adminLogout') }}">logout</a>
+          <a href="{{ url_for('auth.adminRegister') }}">Register</a>
+          <a href="{{ url_for('auth.adminLogout') }}">Logout</a>
         {% else %}
-          <a href="{{ url_for('auth.adminLogin') }}">login</a>
+          <a href="{{ url_for('auth.adminLogin') }}">Login</a>
         {% endif %}
       </span>
       <p><pre>{{context.footer_style[1]}}
 {{context.footer_style[0]}}
 {{context.footer_style[1]}}</pre>
         <div>
-          <a href="https://github.com/usmanmusa1920/sakyum" target="_blank">Github</a>
+          <a href="https://github.com/usmanmusa1920/sakyum" target="_blank">Repository</a>
           <a>|</a>
           <a href="https://sakyum.readthedocs.io" target="_blank">Docs</a>
           <a>|</a>
           <a href="/admin">Admin</a>
         </div>
       </p>
     </div>
```

#### html2text {}

```diff
@@ -6,22 +6,22 @@
  {% block head_css %}  {% endblock head_css %}
  {% block head_js %}  {% endblock head_js %} {% if context.head_title %} {%
 block head_title %}
 {% endblock head_title %} {% else %}
 {% endif %}
 ****** Sakyum ******
 {% if current_user.is_authenticated %}  {% else %} Github {% endif %} | {% if
-current_user.is_authenticated %} register logout {% else %} Docs login {% endif
+current_user.is_authenticated %} Register Logout {% else %} Docs Login {% endif
 %}
  {% with messages = get_flashed_messages(with_categories=true) %} {% if
 messages %} {% for category, message in messages %}
 {{message}}
 {% endfor %} {% endif %} {% endwith %}
 {% block auth %}  {% endblock auth %} {% block logo %}  {% block short_info %}
 {% endblock short_info %} {% endblock logo %} {% block main %}  {% endblock
 main %}
-  {% if current_user.is_authenticated %} register logout {% else %} login {%
+  {% if current_user.is_authenticated %} Register Logout {% else %} Login {%
 endif %}
 {{context.footer_style[1]}}
 {{context.footer_style[0]}}
 {{context.footer_style[1]}}
-Github | Docs | Admin
+Repository | Docs | Admin
```

### Comparing `sakyum-0.0.7/sakyum/templates/default_page/default_base.html` & `sakyum-0.0.8/sakyum/templates/default_page/default_base.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <!-- this is the landing page when you create a project -->
-{% extends "default_index.html" %}
+{% extends 'default_index.html' %}
 
 {% block short_info %}
   {% if context.project_name %}
     <p>Your project ({{context.project_name}}) default page</p>
   {% endif %}
   <p>
     {% if current_user.is_authenticated %}
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
- {% extends "default_index.html" %} {% block short_info %} {% if
+ {% extends 'default_index.html' %} {% block short_info %} {% if
 context.project_name %}
 Your project ({{context.project_name}}) default page
 {% endif %}
 {% if current_user.is_authenticated %} Hi {{ current_user.username }}! you'r
 logged in {% else %} Login to take actions {% endif %}
 {% endblock short_info %} {% block main %} {% if context.blueprints_list|length
 > 0 %}
```

### Comparing `sakyum-0.0.7/sakyum/utils.py` & `sakyum-0.0.8/sakyum/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,63 +10,60 @@
 from pathlib import Path
 from getpass import getpass
 from sakyum import __title__
 from sakyum import __version__
 
 
 # relative path to the package folder (sakyum)
-rel_path = Path(__file__).resolve().parent
+REL_PATH = Path(__file__).resolve().parent
+OS_SEP = os.path.sep # platform-specific path separator (for linux `/`, for windows `\\`)
 
 
-def static_dir(app, static_from_pkg=False, os_name: "nt or posix"=os.name):
+def static_dir(app, static_from_pkg=False, os_name: 'nt or posix'=os.name):
   """
-    relative path to static files
-    if `static_from_pkg` is not false, it will use the directory name that is in the library package which is `static`, else it will use for project `static` directory
+  relative path to static files
+  if `static_from_pkg` is not false, it will use the directory name that is in the library package which is `static`, else it will use for project `static` directory
   """
-  if os_name == "nt":
-    if static_from_pkg:
-      return str(rel_path) + "\static\\" + app
-    return os.getcwd() + "\static\\" + app
-  else:
-    if static_from_pkg:
-      return str(rel_path) + "/static/" + app
-    return os.getcwd() + "/static/" + app
+
+  if static_from_pkg:
+      return str(REL_PATH) + OS_SEP + 'static' + OS_SEP + app
+  return os.getcwd() + OS_SEP + 'static' + OS_SEP + app
   
 
 def template_dir(temp_from_pkg=False, os_name=os.name):
   """
-    relative path to html page
-    if `temp_from_pkg` is not false, it will use the directory name that is in the library package which is `templates`, else it will use for project `templates` directory
+  relative path to html page
+  if `temp_from_pkg` is not false, it will use the directory name that is in the library package which is `templates`, else it will use for project `templates` directory
   """
-  if os_name == "nt":
-    if temp_from_pkg:
-      return str(rel_path) + "\\templates\\" + temp_from_pkg
-    return os.getcwd() + "\\templates"
-  else:
-    if temp_from_pkg:
-      return str(rel_path) + "/templates/" + temp_from_pkg
-    return os.getcwd() + "/templates"
+
+  if temp_from_pkg:
+    return str(REL_PATH) + OS_SEP + 'templates' + OS_SEP + temp_from_pkg
+  return os.getcwd() + OS_SEP + 'templates'
   
 
 def stylePage(name, version=False):
   """function for styling project/app description default pages"""
   if version:
     # it will style the description in the footer
-    desc = "@ " + name + " software - v" + version
+    desc = '@ ' + name + ' software - v' + version
     desc_center = desc.center(len(desc) + 2)
-    border = "=" * len(desc_center)
+    border = '=' * len(desc_center)
     return [desc_center, border]
 
   # it will style the description of default app pages
-  desc = "Your " + name + " application default pages"
+  desc = 'Your ' + name + ' application default pages'
   desc_center = desc.center(len(desc) + 6)
-  border = "=" * len(desc_center)
+  border = '=' * len(desc_center)
   return [desc_center, border]
   
   
+# Style for sakyum default pages:
+    # ============================
+    #  @ sakyum software - v0.0.8 
+    # ============================
 footer_style = stylePage(__title__, version=__version__)
 
 
 def rem_blueprint(lst_blue=None, rem_blue=None):
   # these are blueprint that we don't want to show on the
   # default page so we are removing them from the list
   # reason is they are not route
@@ -87,82 +84,82 @@
     self.email = email
     self.password = password
     self.u_args = u_args
     self.e_args = e_args
     self.p_args = p_args
 
     if self.u_args:
-      while self.username == None or self.username == "" or len(self.username) < 3:
+      while self.username == None or self.username == '' or len(self.username) < 3:
         if self.username == None:
-          self.username = input("Enter username: ")
+          self.username = input('Enter username: ')
           print()
-        elif self.username == "":
-          print("username can't be empty")
-          self.username = input("Enter username: ")
+        elif self.username == '':
+          print('username can\'t be empty')
+          self.username = input('Enter username: ')
           print()
         elif len((self.username)) < 3:
-          print("username must be not less than 3 character")
-          self.username = input("Enter username: ")
+          print('username must be not less than 3 character')
+          self.username = input('Enter username: ')
           print()
 
     if self.e_args:
-      while self.email == None or self.email == "":
+      while self.email == None or self.email == '':
         if self.email == None:
-          self.email = input("Enter email: ")
+          self.email = input('Enter email: ')
           print()
-        elif self.email == "":
-          print("email can't be empty")
-          self.email = input("Enter email: ")
+        elif self.email == '':
+          print('email can\'t be empty')
+          self.email = input('Enter email: ')
           print()
 
     if self.p_args:
-      while self.password == None or self.password == "" or len(self.password) < 6:
+      while self.password == None or self.password == '' or len(self.password) < 6:
         if self.password == None:
-          self.password = getpass("Enter password: ")
+          self.password = getpass('Enter password: ')
           print()
-        elif self.password == "":
-          print("password can't be empty")
-          self.password = getpass("Enter password: ")
+        elif self.password == '':
+          print('password can\'t be empty')
+          self.password = getpass('Enter password: ')
           print()
         elif len((self.password)) < 6:
-          print("password must be not less than 6 character")
-          self.password = getpass("Enter password: ")
+          print('password must be not less than 6 character')
+          self.password = getpass('Enter password: ')
           print()
         
   @property
   def validate_username(self):
     """validate username"""
     # the below while is included to check data validation
     # when user uses flags `-u` or `--username`
     while len(self.username) < 3:
-      print("username must be not less than 3 character")
-      self.username = input("Enter username: ")
+      print('username must be not less than 3 character')
+      self.username = input('Enter username: ')
       print()
     return self.username
 
   @property
   def validate_email(self):
     """email validator"""
-    pattern = re.compile(r"^[a-zA-Z0-9-_]+@[a-zA-Z0-9]+\.[a-zA-Z0-9]+")
+    pattern = re.compile(r'^[a-zA-Z0-9-_]+@[a-zA-Z0-9]+\.[a-zA-Z0-9]+')
     if re.match(pattern, self.email):
       return self.email
     while not re.match(pattern, self.email):
-      print("Put a valid email: ")
-      self.email = input("Enter email: ")
+      print('Put a valid email: ')
+      self.email = input('Enter email: ')
       print()
     return self.email
 
   @property
   def validate_password(self):
     """validate password"""
     # the below while is included to chech data validation
     # when user uses flags `-p` or `--password`
     while len(self.password) < 6:
-      print("password must be not less than 6 character")
-      self.password = getpass("Enter password: ")
+      print('password must be not less than 6 character')
+      self.password = getpass('Enter password: ')
       print()
     return self.password
 
   @property
   def result(self):
     """user credentials in a list"""
     auth_list = [self.validate_username, self.validate_email, self.validate_password]
@@ -176,46 +173,46 @@
   
   A reqular expression that matches any character that
   should never appear in base 64 encodings would be:
     [^A-Za-z0-9+/=]
   we follow the base64 pattern of [^A-Za-z0-9+/=] that should never appear in base64, (in reqex)
   """
   
-  token_sm_alpha = "abcdefghijklmnopqrstuvwxyz"
+  token_sm_alpha = 'abcdefghijklmnopqrstuvwxyz'
   token_cap_alpha = token_sm_alpha.upper()
-  token_num = "0123456789"
-  token_char = "/+="
+  token_num = '0123456789'
+  token_char = '/+='
   token_sum = token_sm_alpha + token_cap_alpha + token_num
   
   """
   We times the above variable (token_sum) by 2 (total length is 124),
   so that we will randomly select from it without any restriction,
   since we make the minimum length of the salt to be 32 and the maximum to be 64,
   and also it will randomly select from that range of (32 - 64)
   """
 
   token_times = token_sum * 2
   token_list = list(token_times)
   random.shuffle(token_list) # shuffling the above list
-  token_generate = "".join(token_list)
+  token_generate = ''.join(token_list)
   
   def __init__(self, token_generate = token_generate):
-    self.token_generate = "".join(token_generate)
+    self.token_generate = ''.join(token_generate)
     
   @property
   def passcode_salt(self):
     """
     salting our passcode with this class method
     
     By using the random sample method, where we make:
       population = self.token_generate
       k = random.randint(20, 50)
     """
 
-    salt = "".join(random.sample(self.token_generate, random.randint(20, 50)))
+    salt = ''.join(random.sample(self.token_generate, random.randint(20, 50)))
     return salt # return type is string
     
   def passcode_iteration(self, r_min, r_max, r_step):
     """
     Generating a random iteration. The iterations is not static,
     it is dynamic (every user's iteration is randomly choosen),
     by using the random method of randrange
@@ -226,41 +223,41 @@
     
   def get_hash(self, salt: str, itter: int, passwd: str) -> str:
     """
     generating our key using this class method, and also
     the return type of the key is bytes
     """
     key = hashlib.pbkdf2_hmac(
-        "sha256", # The hash digest algorithm for HMAC
-        passwd.encode("utf-8"), # Convert the password to bytes
-        salt.encode("utf-8"), # Convert the salt to bytes
+        'sha256', # The hash digest algorithm for HMAC
+        passwd.encode('utf-8'), # Convert the password to bytes
+        salt.encode('utf-8'), # Convert the salt to bytes
         itter, # iteration type is integer
         dklen=128 # Get a 128 byte key
     )
     
     """
     Base64 encoding convert the binary data (sequence of byte) into text format,
     to avoid data corruption when transfer via only text channel.
     It is Privacy enhanced Electronic Mail (PEM).
     
     We use ascii to encode the (key)
     """
     
     # encodeing the key, type is string
-    b64_encode = base64.b64encode(key).decode("ascii").strip()
+    b64_encode = base64.b64encode(key).decode('ascii').strip()
 
     # hashing our b64_encode (the second hash), type is string
     hash_result = hashlib.sha256(str.encode(str(b64_encode))).hexdigest()
 
     # salt + iteration + hash_result, type is string
-    secure_ingredient = "%s%d%s" % (salt, itter, hash_result)
+    secure_ingredient = '%s%d%s' % (salt, itter, hash_result)
     
     # return types of the list is string all, access it by print(self.get_hash.__annotations__)
     return [hash_result, secure_ingredient]
 
   def secret(self):
     r = random.randint(32, 52)
     secret = secrets.token_hex(r)
     return secret
     
   def __str__(self):
-    return f"Passcode security class"
+    return f'Passcode security class'
```

### Comparing `sakyum-0.0.7/sakyum.egg-info/PKG-INFO` & `sakyum-0.0.8/sakyum.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: sakyum
-Version: 0.0.7
+Version: 0.0.8
 Summary: An extension of flask web framework that erase the complexity of structuring flask project blueprint, packages, and other annoying stuffs
 Home-page: https://sakyum.readthedocs.io
 Author: Usman Musa
 Author-email: usmanmusa1920@gmail.com
-License: UNKNOWN
+License: MIT
+Download-URL: https://pypi.org/project/sakyum
+Project-URL: Documentation, https://sakyum.readthedocs.io
+Project-URL: Source, https://github.com/usmanmusa1920/sakyum
 Description: 
         # Sakyum
         
         An extension of flask web framework that erase the complexity of structuring flask project blueprint, packages, and other annoying stuffs.
         
         ## Installation
         
-        Install and update the latest release from <a href="https://pypi.org/project/sakyum">pypi</a>. Basically the library was uploaded using `sdist` (Source Distribution) and this software (library) it might not be compatible with `windows operating system` but it works on other `OS` such as `linux` and `macOS`, but very soon the version that will be compatible with **windows operating system** will be release, stay tuned.
+        Install and update the latest release from <a href="https://pypi.org/project/sakyum">pypi</a>. Basically the library was uploaded using `sdist` (Source Distribution) and this software (library) as from `v0.0.8` it is now compatible with `windows OS` and others as well, such as `linux`, `macOS` and possibly some others too!.
         
         ```
         pip install --upgrade sakyum
         ```
         
         ## Create flask project using sakyum
         
@@ -79,25 +82,38 @@
         
         visit `http://127.0.0.1:5000/exam` this will take you to your app landing page (exam)
         
         visit `http://127.0.0.1:5000/admin` this will take you to admin page. From there you are ready to go.
         
         See more documentations <a href="https://sakyum.readthedocs.io">here!</a>
         
+        ### Sakyum default page
+        
+        ![Sakyum default page](./media/sakyum_default_page.png)
+        
         ## Useful links
         
         - Documentation: https://sakyum.readthedocs.io
         - Repository: https://github.com/usmanmusa1920/sakyum
+        - Docker example: https://github.com/usmanmusa1920/sakyum/tree/master/example/sakyum-docker
         
         Pull requests are welcome
         
         
         Change Log
         ==========
         
+        0.0.8 (09/june/2023)
+        ------------------
+        - Eight Release
+        
+        OS compatibility
+        
+        Making sakyum to be compatible with windows OS as well as other OS
+        
         0.0.7 (4/april/2023)
         ------------------
         - Seventh Release
         
         This release mostly is for adding more docs and examples.
         
         - Sixth Release
@@ -115,20 +131,20 @@
         Database migration is added using `alembic`
         
         Some error pages, default page were added but still you can customise it in your project sub folder (the package with the same name of your project in your project directory) in a file called `route.py`. Also an admin directory within your project templates folder is added too!
         
         Possibly other well things are added which include auth system for `users` and more.
         
 Keywords: sakyum
-Platform: UNKNOWN
+Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
-Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
```

#### html2text {}

```diff
@@ -1,65 +1,70 @@
-Metadata-Version: 2.1 Name: sakyum Version: 0.0.7 Summary: An extension of
+Metadata-Version: 2.1 Name: sakyum Version: 0.0.8 Summary: An extension of
 flask web framework that erase the complexity of structuring flask project
 blueprint, packages, and other annoying stuffs Home-page: https://
 sakyum.readthedocs.io Author: Usman Musa Author-email: usmanmusa1920@gmail.com
-License: UNKNOWN Description: # Sakyum An extension of flask web framework that
-erase the complexity of structuring flask project blueprint, packages, and
-other annoying stuffs. ## Installation Install and update the latest release
-from pypi. Basically the library was uploaded using `sdist` (Source
-Distribution) and this software (library) it might not be compatible with
-`windows operating system` but it works on other `OS` such as `linux` and
-`macOS`, but very soon the version that will be compatible with **windows
-operating system** will be release, stay tuned. ``` pip install --upgrade
-sakyum ``` ## Create flask project using sakyum After the installation paste
-the following command on your termianl ``` python -c "from sakyum import
-project; project('schoolsite')" ``` This will create a project called
-`schoolsite` now cd into the `schoolsite` directory, if you do `ls` within the
-directory you just enter you will see a module called `thunder.py` and some
-directories (some in the form of package) `media`, `static`, `templates` and a
-directory with the same name of your base directory name, in our case it is
-`schoolsite`. Boot up the flask server by running the below command ``` python
-thunder.py boot ``` Now visit the local url `http://127.0.0.1:5000` this will
-show you index page of your project ## Create flask app within your project
-(schoolsite) For you to start an app within your project `schoolsite` shutdown
-the flask development server by pressing ( CTRL+C ) and then run the following
-command, by giving the name you want your app to be, in our case we will call
-our app `exam` ``` python thunder.py create_app -a exam ``` this will create an
-app (a new package called `exam`) within your project `(schoolsite)` ##
-Register an app Once the app is created open a file `schoolsite/routes.py` and
-import your `exam` blueprint which is in (`exam/views.py`), default name given
-to an app blueprint, is the app name so our `exam` app blueprint name is
-`exam`, after importing it, append (register) the app blueprint in a list
-called `reg_blueprints` in that same file of `schoolsite/routes.py` importing
-blueprint ```py from exam.views import exam ``` registering blueprint ```py
-reg_blueprints = [ blueprint.default, blueprint.errors, blueprint.auth, base,
-exam, ] ``` once you register the app, boot up the flask webserver again by ```
-python thunder.py boot ``` visit `http://127.0.0.1:5000` which is your project
-landing page visit `http://127.0.0.1:5000/exam` this will take you to your app
-landing page (exam) visit `http://127.0.0.1:5000/admin` this will take you to
-admin page. From there you are ready to go. See more documentations here! ##
-Useful links - Documentation: https://sakyum.readthedocs.io - Repository:
-https://github.com/usmanmusa1920/sakyum Pull requests are welcome Change Log
-========== 0.0.7 (4/april/2023) ------------------ - Seventh Release This
-release mostly is for adding more docs and examples. - Sixth Release Alembic is
-included as dependency (in the require module list). - Fifth Release In fifith
-release, we handle how default user file system tricks is, things like when
-user change his profile picture. - Fourth Release In this release we handle how
-we can customise the admin html page by inheriting (extends) it in our project
-templates/admin directory, and the admin page on how to bind models in the
-admin. Also I refactor other libraries that this package needs with their
-corresponding versions in the setup.py and requirements.txt files. In this
-release good documentations is well packed. Database migration is added using
-`alembic` Some error pages, default page were added but still you can customise
-it in your project sub folder (the package with the same name of your project
-in your project directory) in a file called `route.py`. Also an admin directory
-within your project templates folder is added too! Possibly other well things
-are added which include auth system for `users` and more. Keywords: sakyum
-Platform: UNKNOWN Classifier: Development Status :: 5 - Production/Stable
+License: MIT Download-URL: https://pypi.org/project/sakyum Project-URL:
+Documentation, https://sakyum.readthedocs.io Project-URL: Source, https://
+github.com/usmanmusa1920/sakyum Description: # Sakyum An extension of flask web
+framework that erase the complexity of structuring flask project blueprint,
+packages, and other annoying stuffs. ## Installation Install and update the
+latest release from pypi. Basically the library was uploaded using `sdist`
+(Source Distribution) and this software (library) as from `v0.0.8` it is now
+compatible with `windows OS` and others as well, such as `linux`, `macOS` and
+possibly some others too!. ``` pip install --upgrade sakyum ``` ## Create flask
+project using sakyum After the installation paste the following command on your
+termianl ``` python -c "from sakyum import project; project('schoolsite')" ```
+This will create a project called `schoolsite` now cd into the `schoolsite`
+directory, if you do `ls` within the directory you just enter you will see a
+module called `thunder.py` and some directories (some in the form of package)
+`media`, `static`, `templates` and a directory with the same name of your base
+directory name, in our case it is `schoolsite`. Boot up the flask server by
+running the below command ``` python thunder.py boot ``` Now visit the local
+url `http://127.0.0.1:5000` this will show you index page of your project ##
+Create flask app within your project (schoolsite) For you to start an app
+within your project `schoolsite` shutdown the flask development server by
+pressing ( CTRL+C ) and then run the following command, by giving the name you
+want your app to be, in our case we will call our app `exam` ``` python
+thunder.py create_app -a exam ``` this will create an app (a new package called
+`exam`) within your project `(schoolsite)` ## Register an app Once the app is
+created open a file `schoolsite/routes.py` and import your `exam` blueprint
+which is in (`exam/views.py`), default name given to an app blueprint, is the
+app name so our `exam` app blueprint name is `exam`, after importing it, append
+(register) the app blueprint in a list called `reg_blueprints` in that same
+file of `schoolsite/routes.py` importing blueprint ```py from exam.views import
+exam ``` registering blueprint ```py reg_blueprints = [ blueprint.default,
+blueprint.errors, blueprint.auth, base, exam, ] ``` once you register the app,
+boot up the flask webserver again by ``` python thunder.py boot ``` visit
+`http://127.0.0.1:5000` which is your project landing page visit `http://
+127.0.0.1:5000/exam` this will take you to your app landing page (exam) visit
+`http://127.0.0.1:5000/admin` this will take you to admin page. From there you
+are ready to go. See more documentations here! ### Sakyum default page ![Sakyum
+default page](./media/sakyum_default_page.png) ## Useful links - Documentation:
+https://sakyum.readthedocs.io - Repository: https://github.com/usmanmusa1920/
+sakyum - Docker example: https://github.com/usmanmusa1920/sakyum/tree/master/
+example/sakyum-docker Pull requests are welcome Change Log ========== 0.0.8
+(09/june/2023) ------------------ - Eight Release OS compatibility Making
+sakyum to be compatible with windows OS as well as other OS 0.0.7 (4/april/
+2023) ------------------ - Seventh Release This release mostly is for adding
+more docs and examples. - Sixth Release Alembic is included as dependency (in
+the require module list). - Fifth Release In fifith release, we handle how
+default user file system tricks is, things like when user change his profile
+picture. - Fourth Release In this release we handle how we can customise the
+admin html page by inheriting (extends) it in our project templates/admin
+directory, and the admin page on how to bind models in the admin. Also I
+refactor other libraries that this package needs with their corresponding
+versions in the setup.py and requirements.txt files. In this release good
+documentations is well packed. Database migration is added using `alembic` Some
+error pages, default page were added but still you can customise it in your
+project sub folder (the package with the same name of your project in your
+project directory) in a file called `route.py`. Also an admin directory within
+your project templates folder is added too! Possibly other well things are
+added which include auth system for `users` and more. Keywords: sakyum
+Platform: any Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment Classifier: Intended Audience ::
 Developers Classifier: Natural Language :: English Classifier: Operating System
-:: POSIX :: Linux Classifier: License :: OSI Approved :: MIT License
+:: OS Independent Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.10 Requires-Python: >=3.6 Description-
 Content-Type: text/markdown
```

### Comparing `sakyum-0.0.7/sakyum.egg-info/SOURCES.txt` & `sakyum-0.0.8/sakyum.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 CHANGELOG
 LICENSE
 MANIFEST.in
 README.md
 requirements.txt
 setup.py
+media/sakyum_default_page.png
 sakyum/__init__.py
 sakyum/api.py
 sakyum/base.py
 sakyum/blueprint.py
 sakyum/database.py
 sakyum/utils.py
 sakyum.egg-info/PKG-INFO
```

### Comparing `sakyum-0.0.7/setup.py` & `sakyum-0.0.8/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,72 +1,76 @@
 # -*- coding: utf-8 -*-
 
 from setuptools import setup
 from setuptools import find_packages
 
 
 setup(
-  name = "sakyum", # name of the main package (base folder)
-  version = "0.0.7",
-  description = "An extension of flask web framework that erase the complexity of structuring flask project blueprint, packages, and other annoying stuffs",
-  long_description=open("README.md").read() + "\n\n" + open("CHANGELOG").read(),
-  long_description_content_type="text/markdown",
-  python_requires=">=3.6",
-  # platforms="any",
+  name = 'sakyum', # name of the main package (base folder i.e sakyum)
+  version = '0.0.8',
+  description = 'An extension of flask web framework that erase the complexity of structuring flask project blueprint, packages, and other annoying stuffs',
+  long_description = open('README.md').read() + '\n\n' + open('CHANGELOG').read(),
+  long_description_content_type='text/markdown',
+  python_requires = '>=3.6',
+  platforms='any',
   
-  url = "https://sakyum.readthedocs.io",
-  repo = "https://github.com/usmanmusa1920/sakyum",
-  author = "Usman Musa",
-  author_email = "usmanmusa1920@gmail.com",
-  License="MIT",
+  url = 'https://sakyum.readthedocs.io',
+  download_url = 'https://pypi.org/project/sakyum',
+  author = 'Usman Musa',
+  author_email = 'usmanmusa1920@gmail.com',
+  license = 'MIT',
   classifiers = [
-    "Development Status :: 5 - Production/Stable",
-    "Environment :: Web Environment",
-    "Intended Audience :: Developers",
-    "Natural Language :: English",
-    "Operating System :: POSIX :: Linux",
-    # "Operating System :: OS Independent",
-    "License :: OSI Approved :: MIT License",
-    "Topic :: Software Development :: Libraries :: Python Modules",
-    "Programming Language :: Python",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.10",
+    'Development Status :: 5 - Production/Stable',
+    'Environment :: Web Environment',
+    'Intended Audience :: Developers',
+    'Natural Language :: English',
+    # 'Operating System :: POSIX :: Linux',
+    'Operating System :: OS Independent',
+    'License :: OSI Approved :: MIT License',
+    'Topic :: Software Development :: Libraries :: Python Modules',
+    'Programming Language :: Python',
+    'Programming Language :: Python :: 3',
+    'Programming Language :: Python :: 3.8',
+    'Programming Language :: Python :: 3.10',
   ],
   
   # used when people are searching for a module, keywords separated with a space
-  keywords="sakyum",
+  keywords = 'sakyum',
   include_package_data = True, # include files listed in MANIFEST.in
   
   # The list of packages(directories) for your library
-  packages=find_packages(), # OR packages=["sakyum"] 
-  # If your package is a single module, use this instead of "packages":
-  # py_modules=[""] # list of files (modules) that are not in any directory (at the root dir)
+  packages = find_packages(), # OR packages=['sakyum'] 
+  # If your package is a single module, use this instead of 'packages':
+  # py_modules=[''] # list of files (modules) that are not in any directory (at the root dir)
   # the libraries it depends on
   
   # List of other python modules which this module depends on. For example RPi.GPIO
   install_requires = [
-    "alembic==1.9.4",
-    "bcrypt==4.0.1",
-    "click==8.1.3",
-    "dnspython==2.3.0",
-    "email-validator==1.3.1",
-    "Flask==2.2.3",
-    "Flask-Admin==1.6.0",
-    "Flask-Bcrypt==1.0.1",
-    "Flask-Login==0.6.2",
-    "Flask-SQLAlchemy==3.0.3",
-    "Flask-WTF==1.1.1",
-    "greenlet==2.0.2",
-    "idna==3.4",
-    "importlib-metadata==6.0.0",
-    "itsdangerous==2.1.2",
-    "Jinja2==3.1.2",
-    "Mako==1.2.4",
-    "MarkupSafe==2.1.2",
-    "SQLAlchemy==1.4.45",
-    "typing-extensions==4.5.0",
-    "Werkzeug==2.2.3",
-    "WTForms==3.0.1",
-    "zipp==3.13.0",
-  ]
+    'alembic==1.9.4',
+    'bcrypt==4.0.1',
+    'click==8.1.3',
+    'dnspython==2.3.0',
+    'email-validator==1.3.1',
+    'Flask==2.2.3',
+    'Flask-Admin==1.6.0',
+    'Flask-Bcrypt==1.0.1',
+    'Flask-Login==0.6.2',
+    'Flask-SQLAlchemy==3.0.3',
+    'Flask-WTF==1.1.1',
+    'greenlet==2.0.2',
+    'idna==3.4',
+    'importlib-metadata==6.0.0',
+    'itsdangerous==2.1.2',
+    'Jinja2==3.1.2',
+    'Mako==1.2.4',
+    'MarkupSafe==2.1.2',
+    'SQLAlchemy==1.4.45',
+    'typing-extensions==4.5.0',
+    'Werkzeug==2.2.3',
+    'WTForms==3.0.1',
+    'zipp==3.13.0',
+  ],
+  project_urls={
+    'Documentation': 'https://sakyum.readthedocs.io',
+    'Source': 'https://github.com/usmanmusa1920/sakyum',
+  },
 )
```

