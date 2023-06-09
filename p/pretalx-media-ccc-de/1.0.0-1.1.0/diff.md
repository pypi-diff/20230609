# Comparing `tmp/pretalx-media-ccc-de-1.0.0.tar.gz` & `tmp/pretalx-media-ccc-de-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretalx-media-ccc-de-1.0.0.tar", last modified: Mon Oct 31 23:10:31 2022, max compression
+gzip compressed data, was "pretalx-media-ccc-de-1.1.0.tar", last modified: Fri Jun  9 13:20:33 2023, max compression
```

## Comparing `pretalx-media-ccc-de-1.0.0.tar` & `pretalx-media-ccc-de-1.1.0.tar`

### file list

```diff
@@ -1,95 +1,99 @@
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:10:31.003737 pretalx-media-ccc-de-1.0.0/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      553 2019-07-10 20:57:31.000000 pretalx-media-ccc-de-1.0.0/LICENSE
--rw-r--r--   0 rixx      (1000) rixx      (1000)      256 2022-01-27 19:06:49.000000 pretalx-media-ccc-de-1.0.0/MANIFEST.in
--rw-r--r--   0 rixx      (1000) rixx      (1000)      142 2019-07-10 20:57:31.000000 pretalx-media-ccc-de-1.0.0/Makefile
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1232 2022-10-31 23:10:31.003737 pretalx-media-ccc-de-1.0.0/PKG-INFO
--rw-r--r--   0 rixx      (1000) rixx      (1000)      912 2019-07-10 20:57:31.000000 pretalx-media-ccc-de-1.0.0/README.rst
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:10:30.990403 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/
--rw-r--r--   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:09:26.000000 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/__init__.py
--rw-r--r--   0 rixx      (1000) rixx      (1000)      578 2022-10-31 23:10:13.000000 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/apps.py
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1372 2021-12-14 11:47:59.000000 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/forms.py
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:10:30.993736 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:10:30.987070 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/ar/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:10:30.993736 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/ar/LC_MESSAGES/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      463 2022-10-31 00:02:40.000000 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 rixx      (1000) rixx      (1000)     2129 2022-10-31 23:09:37.000000 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:10:30.987070 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/ca/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:10:30.993736 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/ca/LC_MESSAGES/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      380 2022-10-31 00:02:40.000000 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/ca/LC_MESSAGES/django.mo
--rw-r--r--   0 rixx      (1000) rixx      (1000)     2043 2022-10-31 23:09:37.000000 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/ca/LC_MESSAGES/django.po
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:10:30.987070 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/cs/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:10:30.993736 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/cs/LC_MESSAGES/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      460 2022-10-31 00:02:40.000000 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0 rixx      (1000) rixx      (1000)     2126 2022-10-31 23:09:37.000000 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/cs/LC_MESSAGES/django.po
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:10:30.987070 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/de_DE/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:10:30.993736 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/de_DE/LC_MESSAGES/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      893 2022-10-31 00:02:40.000000 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/de_DE/LC_MESSAGES/django.mo
--rw-r--r--   0 rixx      (1000) rixx      (1000)     2640 2022-10-31 23:09:37.000000 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/de_DE/LC_MESSAGES/django.po
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:10:30.987070 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/de_DE/de/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:10:30.993736 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/de_DE/de/LC_MESSAGES/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      625 2021-07-02 10:27:24.000000 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/de_DE/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:10:30.987070 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/de_Formal/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:10:30.997070 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/de_Formal/LC_MESSAGES/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      337 2022-10-31 00:02:40.000000 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/de_Formal/LC_MESSAGES/django.mo
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1996 2022-10-31 23:09:37.000000 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/de_Formal/LC_MESSAGES/django.po
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1996 2022-10-31 00:08:24.000000 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/django.pot
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:10:30.987070 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/el/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:10:30.997070 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/el/LC_MESSAGES/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      380 2022-10-31 00:02:40.000000 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/el/LC_MESSAGES/django.mo
--rw-r--r--   0 rixx      (1000) rixx      (1000)     2043 2022-10-31 23:09:37.000000 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/el/LC_MESSAGES/django.po
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:10:30.987070 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/en_Mozilla/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:10:30.997070 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/en_Mozilla/LC_MESSAGES/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      337 2021-12-14 00:10:24.000000 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/en_Mozilla/LC_MESSAGES/django.mo
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1996 2021-10-26 13:05:58.000000 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/en_Mozilla/LC_MESSAGES/django.po
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:10:30.987070 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/es/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:10:30.997070 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/es/LC_MESSAGES/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      380 2022-10-31 00:02:40.000000 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 rixx      (1000) rixx      (1000)     2043 2022-10-31 23:09:37.000000 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:10:30.987070 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/es_MX/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:10:30.997070 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/es_MX/LC_MESSAGES/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      380 2022-10-31 00:02:40.000000 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/es_MX/LC_MESSAGES/django.mo
--rw-r--r--   0 rixx      (1000) rixx      (1000)     2043 2022-10-31 23:09:37.000000 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/es_MX/LC_MESSAGES/django.po
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:10:30.987070 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/fr_FR/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:10:30.997070 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/fr_FR/LC_MESSAGES/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      337 2022-10-31 00:02:40.000000 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/fr_FR/LC_MESSAGES/django.mo
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1996 2022-10-31 23:09:37.000000 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/fr_FR/LC_MESSAGES/django.po
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:10:30.987070 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/it/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:10:30.997070 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/it/LC_MESSAGES/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      380 2022-10-31 00:02:40.000000 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 rixx      (1000) rixx      (1000)     2043 2022-10-31 23:09:37.000000 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:10:30.987070 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/ja_JP/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:10:31.000403 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/ja_JP/LC_MESSAGES/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      337 2022-10-31 00:02:40.000000 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/ja_JP/LC_MESSAGES/django.mo
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1996 2022-10-31 23:09:37.000000 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/ja_JP/LC_MESSAGES/django.po
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:10:30.987070 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/pt_BR/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:10:31.000403 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      379 2022-10-31 00:02:40.000000 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0 rixx      (1000) rixx      (1000)     2042 2022-10-31 23:09:37.000000 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:10:30.987070 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/zh_Hant/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:10:31.000403 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/zh_Hant/LC_MESSAGES/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      373 2021-07-28 19:29:04.000000 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/zh_Hant/LC_MESSAGES/django.mo
--rw-r--r--   0 rixx      (1000) rixx      (1000)     2043 2021-07-02 10:27:24.000000 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/zh_Hant/LC_MESSAGES/django.po
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:10:30.990403 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/zh_TW/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:10:31.003737 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/zh_TW/LC_MESSAGES/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      337 2022-10-31 00:02:40.000000 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/zh_TW/LC_MESSAGES/django.mo
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1996 2022-10-31 23:09:37.000000 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/zh_TW/LC_MESSAGES/django.po
--rw-r--r--   0 rixx      (1000) rixx      (1000)      691 2021-12-14 11:47:59.000000 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/recording.py
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1776 2021-12-14 11:48:01.000000 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/signals.py
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:10:30.990403 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/static/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:10:31.003737 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/static/pretalx_media_ccc_de/
--rw-r--r--   0 rixx      (1000) rixx      (1000)        0 2019-07-10 20:57:32.000000 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/static/pretalx_media_ccc_de/.gitkeep
--rw-r--r--   0 rixx      (1000) rixx      (1000)     2074 2021-12-14 11:48:01.000000 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/tasks.py
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:10:30.990403 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/templates/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:10:31.003737 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/templates/pretalx_media_ccc_de/
--rw-r--r--   0 rixx      (1000) rixx      (1000)        0 2019-07-10 20:57:32.000000 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/templates/pretalx_media_ccc_de/.gitkeep
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1443 2021-08-24 22:55:04.000000 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/templates/pretalx_media_ccc_de/settings.html
--rw-r--r--   0 rixx      (1000) rixx      (1000)      300 2022-07-11 16:34:44.000000 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/urls.py
--rw-r--r--   0 rixx      (1000) rixx      (1000)     2535 2021-12-14 11:48:01.000000 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/views.py
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:10:30.993736 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de.egg-info/
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1232 2022-10-31 23:10:30.000000 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de.egg-info/PKG-INFO
--rw-r--r--   0 rixx      (1000) rixx      (1000)     2477 2022-10-31 23:10:30.000000 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de.egg-info/SOURCES.txt
--rw-r--r--   0 rixx      (1000) rixx      (1000)        1 2022-10-31 23:10:30.000000 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de.egg-info/dependency_links.txt
--rw-r--r--   0 rixx      (1000) rixx      (1000)       78 2022-10-31 23:10:30.000000 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de.egg-info/entry_points.txt
--rw-r--r--   0 rixx      (1000) rixx      (1000)       21 2022-10-31 23:10:30.000000 pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de.egg-info/top_level.txt
--rw-r--r--   0 rixx      (1000) rixx      (1000)      530 2022-10-31 23:10:31.003737 pretalx-media-ccc-de-1.0.0/setup.cfg
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1081 2022-10-31 23:10:03.000000 pretalx-media-ccc-de-1.0.0/setup.py
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.530774 pretalx-media-ccc-de-1.1.0/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      553 2019-07-10 20:57:31.000000 pretalx-media-ccc-de-1.1.0/LICENSE
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      256 2022-01-27 19:06:49.000000 pretalx-media-ccc-de-1.1.0/MANIFEST.in
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      142 2019-07-10 20:57:31.000000 pretalx-media-ccc-de-1.1.0/Makefile
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1212 2023-06-09 13:20:33.530774 pretalx-media-ccc-de-1.1.0/PKG-INFO
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      912 2019-07-10 20:57:31.000000 pretalx-media-ccc-de-1.1.0/README.rst
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.527441 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:09:26.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/__init__.py
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      578 2023-06-09 13:20:14.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/apps.py
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1370 2022-12-19 14:09:09.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/forms.py
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.527441 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.524108 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/ar/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.527441 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      463 2023-05-13 03:03:13.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     2129 2023-06-09 13:19:33.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.524108 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/ca/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.527441 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/ca/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      380 2023-05-13 03:03:13.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/ca/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     2043 2023-06-09 13:19:33.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/ca/LC_MESSAGES/django.po
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.524108 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/cs/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.527441 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      460 2023-05-13 03:03:13.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     2126 2023-06-09 13:19:33.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/cs/LC_MESSAGES/django.po
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.524108 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/de_DE/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.527441 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/de_DE/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      893 2023-06-07 09:14:31.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/de_DE/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     2640 2023-06-09 13:19:33.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/de_DE/LC_MESSAGES/django.po
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.524108 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/de_DE/de/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.527441 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/de_DE/de/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      625 2021-07-02 10:27:24.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/de_DE/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.524108 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/de_Formal/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.527441 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/de_Formal/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      337 2023-05-13 03:03:13.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/de_Formal/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1996 2023-06-09 13:19:33.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/de_Formal/LC_MESSAGES/django.po
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1996 2023-06-07 09:15:13.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/django.pot
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.524108 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/el/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.527441 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/el/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      380 2023-05-13 03:03:13.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/el/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     2043 2023-06-09 13:19:33.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/el/LC_MESSAGES/django.po
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.524108 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/en_Mozilla/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.527441 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/en_Mozilla/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      337 2023-05-13 03:03:13.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/en_Mozilla/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1996 2023-06-09 13:19:33.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/en_Mozilla/LC_MESSAGES/django.po
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.524108 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/es/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.530774 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/es/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      380 2023-05-13 03:03:13.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     2043 2023-06-09 13:19:33.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.524108 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/es_MX/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.530774 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/es_MX/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      380 2023-05-13 03:03:13.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/es_MX/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     2043 2023-06-09 13:19:33.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/es_MX/LC_MESSAGES/django.po
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.524108 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/fr_FR/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.530774 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/fr_FR/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      337 2023-05-13 03:03:13.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/fr_FR/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1996 2023-06-09 13:19:33.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/fr_FR/LC_MESSAGES/django.po
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.524108 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/it/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.530774 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/it/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      380 2023-05-13 03:03:13.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     2043 2023-06-09 13:19:33.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.524108 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/ja_JP/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.530774 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/ja_JP/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      337 2023-05-13 03:03:13.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/ja_JP/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1996 2023-06-09 13:19:33.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/ja_JP/LC_MESSAGES/django.po
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.524108 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/pt_BR/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.530774 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      379 2023-05-13 03:03:13.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     2042 2023-06-09 13:19:33.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.524108 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/pt_PT/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.530774 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/pt_PT/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      337 2023-05-13 03:03:13.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/pt_PT/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1996 2023-02-19 15:38:17.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/pt_PT/LC_MESSAGES/django.po
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.524108 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/zh_Hant/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.530774 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/zh_Hant/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      373 2021-07-28 19:29:04.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/zh_Hant/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     2043 2021-07-02 10:27:24.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/zh_Hant/LC_MESSAGES/django.po
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.524108 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/zh_TW/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.530774 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      337 2023-05-13 03:03:13.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/zh_TW/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1996 2023-06-09 13:19:33.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/zh_TW/LC_MESSAGES/django.po
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      691 2021-12-14 11:47:59.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/recording.py
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1776 2021-12-14 11:48:01.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/signals.py
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.524108 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/static/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.530774 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/static/pretalx_media_ccc_de/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)        0 2019-07-10 20:57:32.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/static/pretalx_media_ccc_de/.gitkeep
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     2074 2021-12-14 11:48:01.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/tasks.py
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.524108 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/templates/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.530774 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/templates/pretalx_media_ccc_de/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)        0 2019-07-10 20:57:32.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/templates/pretalx_media_ccc_de/.gitkeep
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1443 2021-08-24 22:55:04.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/templates/pretalx_media_ccc_de/settings.html
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      300 2022-07-11 16:34:44.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/urls.py
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     2625 2023-06-09 13:18:43.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/views.py
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.527441 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de.egg-info/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1212 2023-06-09 13:20:33.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de.egg-info/PKG-INFO
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     2589 2023-06-09 13:20:33.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de.egg-info/SOURCES.txt
+-rw-r--r--   0 rixx      (1000) rixx      (1000)        1 2023-06-09 13:20:33.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de.egg-info/dependency_links.txt
+-rw-r--r--   0 rixx      (1000) rixx      (1000)       79 2023-06-09 13:20:33.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de.egg-info/entry_points.txt
+-rw-r--r--   0 rixx      (1000) rixx      (1000)       21 2023-06-09 13:20:33.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de.egg-info/top_level.txt
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      530 2023-06-09 13:20:33.530774 pretalx-media-ccc-de-1.1.0/setup.cfg
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1081 2023-06-09 13:20:20.000000 pretalx-media-ccc-de-1.1.0/setup.py
```

### Comparing `pretalx-media-ccc-de-1.0.0/LICENSE` & `pretalx-media-ccc-de-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pretalx-media-ccc-de-1.0.0/PKG-INFO` & `pretalx-media-ccc-de-1.1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: pretalx-media-ccc-de
-Version: 1.0.0
+Version: 1.1.0
 Summary: Pull recordings from media.ccc.de and embed them in talk pages
 Home-page: https://github.com/pretalx/pretalx-media-ccc-de.git
 Author: Tobias Kunze
 Author-email: r@rixx.de
 License: Apache Software License
-Platform: UNKNOWN
 License-File: LICENSE
 
 media.ccc.de recordings
 ==========================
 
 This is a plugin for `pretalx`_. 
 
@@ -37,9 +36,7 @@
 Copyright 2018 Tobias Kunze
 
 Released under the terms of the Apache License 2.0
 
 
 .. _pretalx: https://github.com/pretalx/pretalx
 .. _pretalx development setup: https://docs.pretalx.org/en/latest/developer/setup.html
-
-
```

### Comparing `pretalx-media-ccc-de-1.0.0/README.rst` & `pretalx-media-ccc-de-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/apps.py` & `pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/apps.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,12 +9,12 @@
     class PretalxPluginMeta:
         name = gettext_lazy("media.ccc.de recordings")
         author = "Tobias Kunze"
         description = gettext_lazy(
             "Pull recordings from media.ccc.de and embed them in talk pages"
         )
         visible = True
-        version = "1.0.0"
+        version = "1.1.0"
 
     def ready(self):
         from . import signals  # NOQA
         from . import tasks  # NOQA
```

### Comparing `pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/forms.py` & `pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/forms.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from django import forms
 from django.utils.translation import gettext_lazy as _
 from hierarkey.forms import HierarkeyForm
 
 
 class MediaCCCDeSettingsForm(HierarkeyForm):
-
     media_ccc_de_id = forms.CharField(required=False)
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         event = kwargs.get("obj")
         url = "https://media.ccc.de/public/conferences/{slug}".format(
             slug=event.settings.media_ccc_de_id or event.slug
@@ -17,15 +16,14 @@
             'The slug or ID used for your event in the media.ccc.de API – defaults to your event slug. Your event\'s data has to be available at <a href="{url}">{url}</a>'
         ).format(url=url)
         if not event.settings.media_ccc_de_id:
             self.fields["media_ccc_de_id"].initial = event.slug
 
 
 class MediaCCCDeUrlForm(forms.Form):
-
     media_ccc_de_url = forms.URLField(required=False)
 
     def __init__(self, *args, **kwargs):
         self.submission = kwargs.pop("submission")
         initial = kwargs.get("initial", dict())
         initial["media_ccc_de_url"] = self.submission.event.settings.get(
             f"media_ccc_de_url_{self.submission.code}"
```

### Comparing `pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/ar/LC_MESSAGES/django.po` & `pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/ca/LC_MESSAGES/django.po` & `pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/ca/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/cs/LC_MESSAGES/django.po` & `pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/de_DE/LC_MESSAGES/django.mo` & `pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/de_DE/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/de_DE/LC_MESSAGES/django.po` & `pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/de_DE/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/de_DE/de/LC_MESSAGES/django.po` & `pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/de_DE/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/de_Formal/LC_MESSAGES/django.po` & `pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/de_Formal/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/django.pot` & `pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/el/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -4,22 +4,23 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-31 00:08+0000\n"
+"POT-Creation-Date: 2022-05-17 23:58+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: local/pretalx-media-ccc-de/pretalx_media_ccc_de/apps.py:10
 msgid "media.ccc.de recordings"
 msgstr ""
 
 #: local/pretalx-media-ccc-de/pretalx_media_ccc_de/apps.py:13
 msgid "Pull recordings from media.ccc.de and embed them in talk pages"
```

### Comparing `pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/el/LC_MESSAGES/django.po` & `pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/en_Mozilla/LC_MESSAGES/django.po` & `pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/en_Mozilla/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/es/LC_MESSAGES/django.po` & `pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/es_MX/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/es_MX/LC_MESSAGES/django.po` & `pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/fr_FR/LC_MESSAGES/django.po` & `pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/fr_FR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/it/LC_MESSAGES/django.po` & `pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
 #: local/pretalx-media-ccc-de/pretalx_media_ccc_de/apps.py:10
 msgid "media.ccc.de recordings"
 msgstr ""
 
 #: local/pretalx-media-ccc-de/pretalx_media_ccc_de/apps.py:13
 msgid "Pull recordings from media.ccc.de and embed them in talk pages"
```

### Comparing `pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/ja_JP/LC_MESSAGES/django.po` & `pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/ja_JP/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/pt_BR/LC_MESSAGES/django.po` & `pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/zh_Hant/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -4,38 +4,37 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-05-17 23:58+0000\n"
+"POT-Creation-Date: 2020-01-29 12:16+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n > 1);\n"
-
-#: local/pretalx-media-ccc-de/pretalx_media_ccc_de/apps.py:10
+"Plural-Forms: nplurals=1; plural=0;\n"
+#: local/pretalx-media-ccc-de/pretalx_media_ccc_de/__init__.py:10
 msgid "media.ccc.de recordings"
 msgstr ""
 
-#: local/pretalx-media-ccc-de/pretalx_media_ccc_de/apps.py:13
+#: local/pretalx-media-ccc-de/pretalx_media_ccc_de/__init__.py:13
 msgid "Pull recordings from media.ccc.de and embed them in talk pages"
 msgstr ""
 
 #: local/pretalx-media-ccc-de/pretalx_media_ccc_de/forms.py:17
 #, python-brace-format
 msgid ""
 "The slug or ID used for your event in the media.ccc.de API – defaults to "
-"your event slug. Your event's data has to be available at <a "
-"href=\"{url}\">{url}</a>"
+"your event slug. Your event's data has to be available at <a href="
+"\"{url}\">{url}</a>"
 msgstr ""
 
 #: local/pretalx-media-ccc-de/pretalx_media_ccc_de/templates/pretalx_media_ccc_de/settings.html:7
 msgid "Set up media.ccc.de sync"
 msgstr ""
 
 #: local/pretalx-media-ccc-de/pretalx_media_ccc_de/templates/pretalx_media_ccc_de/settings.html:19
```

### Comparing `pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/zh_Hant/LC_MESSAGES/django.po` & `pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/django.pot`

 * *Files 7% similar despite different names*

```diff
@@ -4,37 +4,37 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2020-01-29 12:16+0000\n"
+"POT-Creation-Date: 2023-06-07 09:15+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
-#: local/pretalx-media-ccc-de/pretalx_media_ccc_de/__init__.py:10
+
+#: local/pretalx-media-ccc-de/pretalx_media_ccc_de/apps.py:10
 msgid "media.ccc.de recordings"
 msgstr ""
 
-#: local/pretalx-media-ccc-de/pretalx_media_ccc_de/__init__.py:13
+#: local/pretalx-media-ccc-de/pretalx_media_ccc_de/apps.py:13
 msgid "Pull recordings from media.ccc.de and embed them in talk pages"
 msgstr ""
 
-#: local/pretalx-media-ccc-de/pretalx_media_ccc_de/forms.py:17
+#: local/pretalx-media-ccc-de/pretalx_media_ccc_de/forms.py:16
 #, python-brace-format
 msgid ""
 "The slug or ID used for your event in the media.ccc.de API – defaults to "
-"your event slug. Your event's data has to be available at <a href="
-"\"{url}\">{url}</a>"
+"your event slug. Your event's data has to be available at <a "
+"href=\"{url}\">{url}</a>"
 msgstr ""
 
 #: local/pretalx-media-ccc-de/pretalx_media_ccc_de/templates/pretalx_media_ccc_de/settings.html:7
 msgid "Set up media.ccc.de sync"
 msgstr ""
 
 #: local/pretalx-media-ccc-de/pretalx_media_ccc_de/templates/pretalx_media_ccc_de/settings.html:19
```

### Comparing `pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/locale/zh_TW/LC_MESSAGES/django.po` & `pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/zh_TW/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/recording.py` & `pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/recording.py`

 * *Files identical despite different names*

### Comparing `pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/signals.py` & `pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/signals.py`

 * *Files identical despite different names*

### Comparing `pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/tasks.py` & `pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/tasks.py`

 * *Files identical despite different names*

### Comparing `pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/templates/pretalx_media_ccc_de/settings.html` & `pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/templates/pretalx_media_ccc_de/settings.html`

 * *Files identical despite different names*

### Comparing `pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de/views.py` & `pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/views.py`

 * *Files 8% similar despite different names*

```diff
@@ -57,11 +57,13 @@
     def get_form_kwargs(self):
         kwargs = super().get_form_kwargs()
         return {"obj": self.request.event, "attribute_name": "settings", **kwargs}
 
     def get_context_data(self, *args, **kwargs):
         kwargs = super().get_context_data(**kwargs)
         kwargs["url_forms"] = [
-            MediaCCCDeUrlForm(submission=submission)
-            for submission in self.request.event.talks
+            MediaCCCDeUrlForm(submission=slot.submission)
+            for slot in self.request.event.current_schedule.talks.all()
+            .filter(is_visible=True)
+            .order_by("start")
         ]
         return kwargs
```

### Comparing `pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de.egg-info/PKG-INFO` & `pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: pretalx-media-ccc-de
-Version: 1.0.0
+Version: 1.1.0
 Summary: Pull recordings from media.ccc.de and embed them in talk pages
 Home-page: https://github.com/pretalx/pretalx-media-ccc-de.git
 Author: Tobias Kunze
 Author-email: r@rixx.de
 License: Apache Software License
-Platform: UNKNOWN
 License-File: LICENSE
 
 media.ccc.de recordings
 ==========================
 
 This is a plugin for `pretalx`_. 
 
@@ -37,9 +36,7 @@
 Copyright 2018 Tobias Kunze
 
 Released under the terms of the Apache License 2.0
 
 
 .. _pretalx: https://github.com/pretalx/pretalx
 .. _pretalx development setup: https://docs.pretalx.org/en/latest/developer/setup.html
-
-
```

### Comparing `pretalx-media-ccc-de-1.0.0/pretalx_media_ccc_de.egg-info/SOURCES.txt` & `pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -41,14 +41,16 @@
 pretalx_media_ccc_de/locale/fr_FR/LC_MESSAGES/django.po
 pretalx_media_ccc_de/locale/it/LC_MESSAGES/django.mo
 pretalx_media_ccc_de/locale/it/LC_MESSAGES/django.po
 pretalx_media_ccc_de/locale/ja_JP/LC_MESSAGES/django.mo
 pretalx_media_ccc_de/locale/ja_JP/LC_MESSAGES/django.po
 pretalx_media_ccc_de/locale/pt_BR/LC_MESSAGES/django.mo
 pretalx_media_ccc_de/locale/pt_BR/LC_MESSAGES/django.po
+pretalx_media_ccc_de/locale/pt_PT/LC_MESSAGES/django.mo
+pretalx_media_ccc_de/locale/pt_PT/LC_MESSAGES/django.po
 pretalx_media_ccc_de/locale/zh_Hant/LC_MESSAGES/django.mo
 pretalx_media_ccc_de/locale/zh_Hant/LC_MESSAGES/django.po
 pretalx_media_ccc_de/locale/zh_TW/LC_MESSAGES/django.mo
 pretalx_media_ccc_de/locale/zh_TW/LC_MESSAGES/django.po
 pretalx_media_ccc_de/static/pretalx_media_ccc_de/.gitkeep
 pretalx_media_ccc_de/templates/pretalx_media_ccc_de/.gitkeep
 pretalx_media_ccc_de/templates/pretalx_media_ccc_de/settings.html
```

### Comparing `pretalx-media-ccc-de-1.0.0/setup.cfg` & `pretalx-media-ccc-de-1.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `pretalx-media-ccc-de-1.0.0/setup.py` & `pretalx-media-ccc-de-1.1.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 
 cmdclass = {"build": CustomBuild}
 
 
 setup(
     name="pretalx-media-ccc-de",
-    version="1.0.0",
+    version="1.1.0",
     description="Pull recordings from media.ccc.de and embed them in talk pages",
     long_description=long_description,
     url="https://github.com/pretalx/pretalx-media-ccc-de.git",
     author="Tobias Kunze",
     author_email="r@rixx.de",
     license="Apache Software License",
     install_requires=[],
```

