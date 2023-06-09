# Comparing `tmp/manhattan_manage-0.9.8.tar.gz` & `tmp/manhattan_manage-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/manhattan_manage-0.9.8.tar", last modified: Mon Sep 30 17:51:48 2019, max compression
+gzip compressed data, was "dist/manhattan_manage-0.9.9.tar", last modified: Tue Oct  1 22:06:01 2019, max compression
```

## Comparing `manhattan_manage-0.9.8.tar` & `manhattan_manage-0.9.9.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2019-09-30 17:51:48.000000 manhattan_manage-0.9.8/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1100 2019-08-05 17:36:45.000000 manhattan_manage-0.9.8/LICENSE
--rw-r--r--   0 anthony   (1000) anthony   (1000)      125 2019-08-05 17:36:45.000000 manhattan_manage-0.9.8/MANIFEST.in
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1079 2019-09-30 17:51:48.000000 manhattan_manage-0.9.8/PKG-INFO
--rw-r--r--   0 anthony   (1000) anthony   (1000)      162 2019-08-05 17:36:45.000000 manhattan_manage-0.9.8/README.md
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2019-09-30 17:51:48.000000 manhattan_manage-0.9.8/manhattan_manage/
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2019-09-30 17:51:48.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan/
--rw-r--r--   0 anthony   (1000) anthony   (1000)       55 2019-08-05 17:36:45.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan/__init__.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2019-09-30 17:51:48.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     6280 2019-09-02 23:50:53.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/__init__.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1751 2019-08-05 17:36:45.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/commands.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     5036 2019-08-13 14:50:39.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/config.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2019-09-30 17:51:48.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/templates/
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2019-09-30 17:51:48.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/templates/manhattan/
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2019-09-30 17:51:48.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/templates/manhattan/manage/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     8911 2019-09-03 10:37:11.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/templates/manhattan/manage/base.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2019-09-30 17:51:48.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/templates/manhattan/manage/components/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1744 2019-08-05 17:36:45.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/templates/manhattan/manage/components/boxes.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4579 2019-08-05 17:36:45.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/templates/manhattan/manage/components/breadcrumb.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2777 2019-08-05 17:36:45.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/templates/manhattan/manage/components/changes.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)    16937 2019-08-05 17:36:45.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/templates/manhattan/manage/components/dataset.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)    21157 2019-08-05 17:36:45.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/templates/manhattan/manage/components/form.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)    17225 2019-08-05 17:37:10.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/templates/manhattan/manage/components/heading.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     8678 2019-08-05 17:36:45.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/templates/manhattan/manage/components/nav.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)    19985 2019-08-20 01:25:35.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/templates/manhattan/manage/components/results.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2610 2019-08-08 23:16:42.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/templates/manhattan/manage/components/sessions.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1339 2019-08-05 17:36:45.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/templates/manhattan/manage/components/status.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2019-09-30 17:51:48.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/templates/manhattan/manage/emails/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     6469 2019-08-05 17:36:45.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/templates/manhattan/manage/emails/base.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)    10316 2019-08-05 17:36:45.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/templates/manhattan/manage/emails/components.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2019-09-30 17:51:48.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/templates/manhattan/manage/errors/
--rw-r--r--   0 anthony   (1000) anthony   (1000)       11 2019-08-05 17:36:45.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/templates/manhattan/manage/errors/40X.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)        3 2019-08-05 17:36:45.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/templates/manhattan/manage/errors/500.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2019-09-30 17:51:48.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/templates/manhattan/manage/generics/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2950 2019-08-05 17:36:45.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/templates/manhattan/manage/generics/add.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)      603 2019-08-05 17:36:45.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/templates/manhattan/manage/generics/change_log.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2790 2019-08-05 17:36:45.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/templates/manhattan/manage/generics/delete.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2968 2019-08-05 17:36:45.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/templates/manhattan/manage/generics/duplicate.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1628 2019-08-05 17:36:45.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/templates/manhattan/manage/generics/gallery.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1578 2019-08-05 17:36:45.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/templates/manhattan/manage/generics/list.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2037 2019-08-05 17:36:45.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/templates/manhattan/manage/generics/order.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2019-09-30 17:51:48.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/templates/manhattan/manage/generics/publishing/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2654 2019-08-05 17:36:45.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/templates/manhattan/manage/generics/publishing/publish.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2722 2019-08-05 17:36:45.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/templates/manhattan/manage/generics/publishing/revert.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2812 2019-08-05 17:36:45.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/templates/manhattan/manage/generics/publishing/unpublish.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2019-09-30 17:51:48.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/templates/manhattan/manage/generics/related/
--rw-r--r--   0 anthony   (1000) anthony   (1000)       54 2019-08-05 17:36:45.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/templates/manhattan/manage/generics/related/list.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2019-09-30 17:51:48.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/templates/manhattan/manage/generics/seo/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2394 2019-08-05 17:36:45.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/templates/manhattan/manage/generics/seo/update.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2959 2019-08-05 17:36:45.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/templates/manhattan/manage/generics/update.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2306 2019-08-05 17:36:45.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/templates/manhattan/manage/generics/view.html
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3112 2019-08-05 17:36:45.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/templates/manhattan/manage/minimal.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2019-09-30 17:51:48.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/tests/
--rw-r--r--   0 anthony   (1000) anthony   (1000)        0 2019-08-05 17:36:45.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/tests/__init__.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1305 2019-08-05 17:36:45.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/utils.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2019-09-30 17:51:48.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/views/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1432 2019-08-05 17:36:45.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/views/__init__.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3462 2019-08-05 17:36:45.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/views/add.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     5945 2019-09-24 17:58:37.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/views/change_log.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4070 2019-08-14 02:08:41.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/views/delete.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4658 2019-08-05 17:36:45.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/views/duplicate.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)    17193 2019-09-30 17:50:08.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/views/factories.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)    10458 2019-09-24 17:58:22.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/views/list.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     5210 2019-08-05 17:36:45.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/views/order.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2019-09-30 17:51:48.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/views/related/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1253 2019-08-05 17:36:45.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/views/related/__init__.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3204 2019-08-05 17:36:45.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/views/related/add.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1732 2019-08-05 17:36:45.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/views/related/change_log.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1631 2019-08-05 17:36:45.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/views/related/delete.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4666 2019-08-05 17:36:45.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/views/related/factories.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     8779 2019-09-24 23:11:04.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/views/related/list.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3600 2019-08-05 17:36:45.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/views/related/order.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3164 2019-08-05 17:36:45.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/views/related/update.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3216 2019-08-05 17:36:45.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/views/related/view.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     5090 2019-08-05 17:36:45.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/views/typeahead.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4532 2019-08-05 17:36:45.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/views/update.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1924 2019-08-05 17:36:45.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/views/utils.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2358 2019-08-05 17:36:45.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/views/view.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2019-09-30 17:51:48.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan_manage.egg-info/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1079 2019-09-30 17:51:48.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan_manage.egg-info/PKG-INFO
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4297 2019-09-30 17:51:48.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan_manage.egg-info/SOURCES.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)        1 2019-09-30 17:51:48.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan_manage.egg-info/dependency_links.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)       10 2019-09-30 17:51:48.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan_manage.egg-info/namespace_packages.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)      280 2019-09-30 17:51:48.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan_manage.egg-info/requires.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)       10 2019-09-30 17:51:48.000000 manhattan_manage-0.9.8/manhattan_manage/manhattan_manage.egg-info/top_level.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)       79 2019-09-30 17:51:48.000000 manhattan_manage-0.9.8/setup.cfg
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4722 2019-09-30 17:50:30.000000 manhattan_manage-0.9.8/setup.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2019-10-01 22:06:01.000000 manhattan_manage-0.9.9/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1100 2019-08-05 17:36:45.000000 manhattan_manage-0.9.9/LICENSE
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      125 2019-08-05 17:36:45.000000 manhattan_manage-0.9.9/MANIFEST.in
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1079 2019-10-01 22:06:01.000000 manhattan_manage-0.9.9/PKG-INFO
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      162 2019-08-05 17:36:45.000000 manhattan_manage-0.9.9/README.md
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2019-10-01 22:06:01.000000 manhattan_manage-0.9.9/manhattan_manage/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2019-10-01 22:06:01.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       55 2019-08-05 17:36:45.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan/__init__.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2019-10-01 22:06:01.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6280 2019-09-02 23:50:53.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/__init__.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1751 2019-08-05 17:36:45.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/commands.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5036 2019-08-13 14:50:39.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/config.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2019-10-01 22:06:01.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/templates/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2019-10-01 22:06:01.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/templates/manhattan/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2019-10-01 22:06:01.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/templates/manhattan/manage/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     8911 2019-09-03 10:37:11.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/templates/manhattan/manage/base.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2019-10-01 22:06:01.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/templates/manhattan/manage/components/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1744 2019-08-05 17:36:45.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/templates/manhattan/manage/components/boxes.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4579 2019-08-05 17:36:45.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/templates/manhattan/manage/components/breadcrumb.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2777 2019-08-05 17:36:45.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/templates/manhattan/manage/components/changes.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    16937 2019-08-05 17:36:45.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/templates/manhattan/manage/components/dataset.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    21157 2019-08-05 17:36:45.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/templates/manhattan/manage/components/form.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    17238 2019-10-01 21:51:32.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/templates/manhattan/manage/components/heading.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     9000 2019-10-01 21:51:38.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/templates/manhattan/manage/components/nav.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    19985 2019-08-20 01:25:35.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/templates/manhattan/manage/components/results.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2610 2019-08-08 23:16:42.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/templates/manhattan/manage/components/sessions.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1339 2019-08-05 17:36:45.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/templates/manhattan/manage/components/status.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2019-10-01 22:06:01.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/templates/manhattan/manage/emails/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6469 2019-08-05 17:36:45.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/templates/manhattan/manage/emails/base.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    10316 2019-08-05 17:36:45.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/templates/manhattan/manage/emails/components.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2019-10-01 22:06:01.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/templates/manhattan/manage/errors/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       11 2019-08-05 17:36:45.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/templates/manhattan/manage/errors/40X.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)        3 2019-08-05 17:36:45.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/templates/manhattan/manage/errors/500.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2019-10-01 22:06:01.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/templates/manhattan/manage/generics/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2950 2019-08-05 17:36:45.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/templates/manhattan/manage/generics/add.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      603 2019-08-05 17:36:45.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/templates/manhattan/manage/generics/change_log.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2790 2019-08-05 17:36:45.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/templates/manhattan/manage/generics/delete.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2968 2019-08-05 17:36:45.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/templates/manhattan/manage/generics/duplicate.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1628 2019-08-05 17:36:45.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/templates/manhattan/manage/generics/gallery.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1578 2019-08-05 17:36:45.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/templates/manhattan/manage/generics/list.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2037 2019-08-05 17:36:45.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/templates/manhattan/manage/generics/order.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2019-10-01 22:06:01.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/templates/manhattan/manage/generics/publishing/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2654 2019-08-05 17:36:45.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/templates/manhattan/manage/generics/publishing/publish.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2722 2019-08-05 17:36:45.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/templates/manhattan/manage/generics/publishing/revert.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2812 2019-08-05 17:36:45.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/templates/manhattan/manage/generics/publishing/unpublish.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2019-10-01 22:06:01.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/templates/manhattan/manage/generics/related/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       54 2019-08-05 17:36:45.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/templates/manhattan/manage/generics/related/list.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2019-10-01 22:06:01.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/templates/manhattan/manage/generics/seo/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2394 2019-08-05 17:36:45.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/templates/manhattan/manage/generics/seo/update.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2959 2019-08-05 17:36:45.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/templates/manhattan/manage/generics/update.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2306 2019-08-05 17:36:45.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/templates/manhattan/manage/generics/view.html
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3112 2019-08-05 17:36:45.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/templates/manhattan/manage/minimal.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2019-10-01 22:06:01.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/tests/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)        0 2019-08-05 17:36:45.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/tests/__init__.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1305 2019-08-05 17:36:45.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/utils.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2019-10-01 22:06:01.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/views/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1432 2019-08-05 17:36:45.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/views/__init__.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3462 2019-08-05 17:36:45.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/views/add.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5945 2019-09-24 17:58:37.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/views/change_log.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4070 2019-08-14 02:08:41.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/views/delete.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4658 2019-08-05 17:36:45.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/views/duplicate.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    17193 2019-09-30 17:50:08.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/views/factories.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    10458 2019-09-24 17:58:22.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/views/list.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5210 2019-08-05 17:36:45.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/views/order.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2019-10-01 22:06:01.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/views/related/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1253 2019-08-05 17:36:45.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/views/related/__init__.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3204 2019-08-05 17:36:45.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/views/related/add.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1732 2019-08-05 17:36:45.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/views/related/change_log.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1631 2019-08-05 17:36:45.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/views/related/delete.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4666 2019-08-05 17:36:45.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/views/related/factories.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     8779 2019-09-24 23:11:04.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/views/related/list.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3600 2019-08-05 17:36:45.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/views/related/order.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3164 2019-08-05 17:36:45.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/views/related/update.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3216 2019-08-05 17:36:45.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/views/related/view.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5090 2019-08-05 17:36:45.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/views/typeahead.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4532 2019-08-05 17:36:45.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/views/update.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1924 2019-08-05 17:36:45.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/views/utils.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2358 2019-08-05 17:36:45.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/views/view.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2019-10-01 22:06:01.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan_manage.egg-info/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1079 2019-10-01 22:06:01.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan_manage.egg-info/PKG-INFO
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4297 2019-10-01 22:06:01.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan_manage.egg-info/SOURCES.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)        1 2019-10-01 22:06:01.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan_manage.egg-info/dependency_links.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       10 2019-10-01 22:06:01.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan_manage.egg-info/namespace_packages.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      280 2019-10-01 22:06:01.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan_manage.egg-info/requires.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       10 2019-10-01 22:06:01.000000 manhattan_manage-0.9.9/manhattan_manage/manhattan_manage.egg-info/top_level.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       79 2019-10-01 22:06:01.000000 manhattan_manage-0.9.9/setup.cfg
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4722 2019-10-01 22:01:04.000000 manhattan_manage-0.9.9/setup.py
```

### Comparing `manhattan_manage-0.9.8/LICENSE` & `manhattan_manage-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `manhattan_manage-0.9.8/PKG-INFO` & `manhattan_manage-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manhattan_manage
-Version: 0.9.8
+Version: 0.9.9
 Summary: Classes and views for managing documents in a manhattan project.
 Home-page: https://git.getme.co.uk/manhattan/manhattan_manage
 Author: Anthony Blackshaw
 Author-email: ant@getme.co.uk
 Maintainer: The Getme development team
 Maintainer-email: devs@getme.co.uk
 License: MIT
```

### Comparing `manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/__init__.py` & `manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/__init__.py`

 * *Files identical despite different names*

### Comparing `manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/commands.py` & `manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/commands.py`

 * *Files identical despite different names*

### Comparing `manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/config.py` & `manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/config.py`

 * *Files identical despite different names*

### Comparing `manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/templates/manhattan/manage/base.html` & `manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/templates/manhattan/manage/base.html`

 * *Files identical despite different names*

### Comparing `manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/templates/manhattan/manage/components/boxes.html` & `manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/templates/manhattan/manage/components/boxes.html`

 * *Files identical despite different names*

### Comparing `manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/templates/manhattan/manage/components/breadcrumb.html` & `manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/templates/manhattan/manage/components/breadcrumb.html`

 * *Files identical despite different names*

### Comparing `manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/templates/manhattan/manage/components/changes.html` & `manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/templates/manhattan/manage/components/changes.html`

 * *Files identical despite different names*

### Comparing `manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/templates/manhattan/manage/components/dataset.html` & `manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/templates/manhattan/manage/components/dataset.html`

 * *Files identical despite different names*

### Comparing `manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/templates/manhattan/manage/components/form.html` & `manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/templates/manhattan/manage/components/form.html`

 * *Files identical despite different names*

### Comparing `manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/templates/manhattan/manage/components/heading.html` & `manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/templates/manhattan/manage/components/heading.html`

 * *Files 0% similar despite different names*

```diff
@@ -303,15 +303,15 @@
                 {%- set url = None  -%}
                 {%- if item.endpoint and item.query.allowed -%}
                     {%- set url = item.query.url -%}
                 {%- endif -%}
 
                 {%- set active = item.is_active -%}
 
-                {{ tab(text, url, active) }}
+                {{ tab(text, url, active, **item.data) }}
             {%- endfor %}
         </div>
     {% endif %}
 {%- endmacro %}
 
 {#
     Tab
```

### Comparing `manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/templates/manhattan/manage/components/nav.html` & `manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/templates/manhattan/manage/components/nav.html`

 * *Files 3% similar despite different names*

```diff
@@ -155,47 +155,57 @@
     A mixin used in conjunction with the python generated navigation items to
     build the link element.
 #}
 {% macro nav_link(item) -%}
     {% set badge = item.badge %}
     {% set icon = item.data.icon  %}
     {% set link = item.query %}
+    {% set data = item.data.copy() %}
+    {% set class = item.data.pop('class', None) %}
 
     {% if item.endpoint -%}
         {% if link.allowed -%}
             <a
+                {%- if item.fixed_url -%}
+                    href="{{ item.fixed_url }}"
+                {% else %}
+                    href="{{ link.url }}"
+                {% endif %}
                 class="
                     [ mh-nav-item__link ]
                     [
                         mh-nav-link
                         {{ 'mh-nav-link--active' if item.is_active }}
                     ]
+                    {% if class %}{{ class }}{% endif %}
                 "
-                href="{{ link.url }}"
-                >
+                {{ data|xmlattr }}
+            >
                 {{ nav_link_label(item.label, badge, icon) }}
             </a>
         {%- else -%}
             <span class="
                 [ mh-nav-item__link ]
                 [ mh-nav-link  mh-nav-link--disabled ]
-                ">
+                {% if class %}{{ class }}{% endif %}
+                "
+                {{ data|xmlattr }}
+            >
                 {{ nav_link_label(item.label, badge, icon) }}
             </span>
         {%- endif %}
-    {%- elif item.fixed_url -%}
-        <a
-            class="[ mh-nav-item__link ]  [ mh-nav-link ]"
-            href="{{ item.fixed_url }}"
-            target="_blank"
-            >
-            {{ nav_link_label(item.label, badge, icon) }}
-        </a>
     {%- else -%}
-        <span class="[ mh-nav-item__link ]  [ mh-nav-link ]">
+        <span
+            class="
+                [ mh-nav-item__link ]
+                [ mh-nav-link ]
+                {% if class %}{{ class }}{% endif %}
+            "
+            {{ data|xmlattr }}
+        >
             {{ nav_link_label(item.label, badge, icon) }}
         </span>
     {%- endif %}
 {%- endmacro %}
 
 {#
     Nav link text
```

### Comparing `manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/templates/manhattan/manage/components/results.html` & `manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/templates/manhattan/manage/components/results.html`

 * *Files identical despite different names*

### Comparing `manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/templates/manhattan/manage/components/sessions.html` & `manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/templates/manhattan/manage/components/sessions.html`

 * *Files identical despite different names*

### Comparing `manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/templates/manhattan/manage/components/status.html` & `manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/templates/manhattan/manage/components/status.html`

 * *Files identical despite different names*

### Comparing `manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/templates/manhattan/manage/emails/base.html` & `manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/templates/manhattan/manage/emails/base.html`

 * *Files identical despite different names*

### Comparing `manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/templates/manhattan/manage/emails/components.html` & `manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/templates/manhattan/manage/emails/components.html`

 * *Files identical despite different names*

### Comparing `manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/templates/manhattan/manage/generics/add.html` & `manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/templates/manhattan/manage/generics/add.html`

 * *Files identical despite different names*

### Comparing `manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/templates/manhattan/manage/generics/change_log.html` & `manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/templates/manhattan/manage/generics/change_log.html`

 * *Files identical despite different names*

### Comparing `manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/templates/manhattan/manage/generics/delete.html` & `manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/templates/manhattan/manage/generics/delete.html`

 * *Files identical despite different names*

### Comparing `manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/templates/manhattan/manage/generics/duplicate.html` & `manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/templates/manhattan/manage/generics/duplicate.html`

 * *Files identical despite different names*

### Comparing `manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/templates/manhattan/manage/generics/gallery.html` & `manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/templates/manhattan/manage/generics/gallery.html`

 * *Files identical despite different names*

### Comparing `manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/templates/manhattan/manage/generics/list.html` & `manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/templates/manhattan/manage/generics/list.html`

 * *Files identical despite different names*

### Comparing `manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/templates/manhattan/manage/generics/order.html` & `manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/templates/manhattan/manage/generics/order.html`

 * *Files identical despite different names*

### Comparing `manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/templates/manhattan/manage/generics/publishing/publish.html` & `manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/templates/manhattan/manage/generics/publishing/publish.html`

 * *Files identical despite different names*

### Comparing `manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/templates/manhattan/manage/generics/publishing/revert.html` & `manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/templates/manhattan/manage/generics/publishing/revert.html`

 * *Files identical despite different names*

### Comparing `manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/templates/manhattan/manage/generics/publishing/unpublish.html` & `manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/templates/manhattan/manage/generics/publishing/unpublish.html`

 * *Files identical despite different names*

### Comparing `manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/templates/manhattan/manage/generics/seo/update.html` & `manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/templates/manhattan/manage/generics/seo/update.html`

 * *Files identical despite different names*

### Comparing `manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/templates/manhattan/manage/generics/update.html` & `manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/templates/manhattan/manage/generics/update.html`

 * *Files identical despite different names*

### Comparing `manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/templates/manhattan/manage/generics/view.html` & `manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/templates/manhattan/manage/generics/view.html`

 * *Files identical despite different names*

### Comparing `manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/templates/manhattan/manage/minimal.html` & `manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/templates/manhattan/manage/minimal.html`

 * *Files identical despite different names*

### Comparing `manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/utils.py` & `manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/utils.py`

 * *Files identical despite different names*

### Comparing `manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/views/__init__.py` & `manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/views/__init__.py`

 * *Files identical despite different names*

### Comparing `manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/views/add.py` & `manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/views/add.py`

 * *Files identical despite different names*

### Comparing `manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/views/change_log.py` & `manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/views/change_log.py`

 * *Files identical despite different names*

### Comparing `manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/views/delete.py` & `manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/views/delete.py`

 * *Files identical despite different names*

### Comparing `manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/views/duplicate.py` & `manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/views/duplicate.py`

 * *Files identical despite different names*

### Comparing `manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/views/factories.py` & `manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/views/factories.py`

 * *Files identical despite different names*

### Comparing `manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/views/list.py` & `manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/views/list.py`

 * *Files identical despite different names*

### Comparing `manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/views/order.py` & `manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/views/order.py`

 * *Files identical despite different names*

### Comparing `manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/views/related/__init__.py` & `manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/views/related/__init__.py`

 * *Files identical despite different names*

### Comparing `manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/views/related/add.py` & `manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/views/related/add.py`

 * *Files identical despite different names*

### Comparing `manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/views/related/change_log.py` & `manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/views/related/change_log.py`

 * *Files identical despite different names*

### Comparing `manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/views/related/delete.py` & `manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/views/related/delete.py`

 * *Files identical despite different names*

### Comparing `manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/views/related/factories.py` & `manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/views/related/factories.py`

 * *Files identical despite different names*

### Comparing `manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/views/related/list.py` & `manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/views/related/list.py`

 * *Files identical despite different names*

### Comparing `manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/views/related/order.py` & `manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/views/related/order.py`

 * *Files identical despite different names*

### Comparing `manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/views/related/update.py` & `manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/views/related/update.py`

 * *Files identical despite different names*

### Comparing `manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/views/related/view.py` & `manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/views/related/view.py`

 * *Files identical despite different names*

### Comparing `manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/views/typeahead.py` & `manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/views/typeahead.py`

 * *Files identical despite different names*

### Comparing `manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/views/update.py` & `manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/views/update.py`

 * *Files identical despite different names*

### Comparing `manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/views/utils.py` & `manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/views/utils.py`

 * *Files identical despite different names*

### Comparing `manhattan_manage-0.9.8/manhattan_manage/manhattan/manage/views/view.py` & `manhattan_manage-0.9.9/manhattan_manage/manhattan/manage/views/view.py`

 * *Files identical despite different names*

### Comparing `manhattan_manage-0.9.8/manhattan_manage/manhattan_manage.egg-info/PKG-INFO` & `manhattan_manage-0.9.9/manhattan_manage/manhattan_manage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manhattan-manage
-Version: 0.9.8
+Version: 0.9.9
 Summary: Classes and views for managing documents in a manhattan project.
 Home-page: https://git.getme.co.uk/manhattan/manhattan_manage
 Author: Anthony Blackshaw
 Author-email: ant@getme.co.uk
 Maintainer: The Getme development team
 Maintainer-email: devs@getme.co.uk
 License: MIT
```

### Comparing `manhattan_manage-0.9.8/manhattan_manage/manhattan_manage.egg-info/SOURCES.txt` & `manhattan_manage-0.9.9/manhattan_manage/manhattan_manage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `manhattan_manage-0.9.8/setup.py` & `manhattan_manage-0.9.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 setup(
     name='manhattan_manage',
     namespace_packages=['manhattan'],
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='0.9.8',
+    version='0.9.9',
     description='Classes and views for managing documents in a manhattan '
                 'project.',
     long_description=long_description,
     long_description_content_type='text/markdown',
 
     # The project's main homepage (@@ add github url once public)
     url='https://git.getme.co.uk/manhattan/manhattan_manage',
```

