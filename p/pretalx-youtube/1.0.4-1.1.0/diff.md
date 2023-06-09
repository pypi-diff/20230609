# Comparing `tmp/pretalx-youtube-1.0.4.tar.gz` & `tmp/pretalx-youtube-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretalx-youtube-1.0.4.tar", last modified: Mon Oct 31 23:20:26 2022, max compression
+gzip compressed data, was "pretalx-youtube-1.1.0.tar", last modified: Fri Jun  9 13:07:01 2023, max compression
```

## Comparing `pretalx-youtube-1.0.4.tar` & `pretalx-youtube-1.1.0.tar`

### file list

```diff
@@ -1,87 +1,95 @@
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:20:26.235533 pretalx-youtube-1.0.4/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      553 2021-12-15 01:11:11.000000 pretalx-youtube-1.0.4/LICENSE
--rw-r--r--   0 rixx      (1000) rixx      (1000)      230 2022-01-28 01:52:30.000000 pretalx-youtube-1.0.4/MANIFEST.in
--rw-r--r--   0 rixx      (1000) rixx      (1000)      142 2021-12-15 01:09:31.000000 pretalx-youtube-1.0.4/Makefile
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1496 2022-10-31 23:20:26.235533 pretalx-youtube-1.0.4/PKG-INFO
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1210 2021-12-15 01:28:25.000000 pretalx-youtube-1.0.4/README.rst
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:20:26.228866 pretalx-youtube-1.0.4/pretalx_youtube/
--rw-r--r--   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:19:32.000000 pretalx-youtube-1.0.4/pretalx_youtube/__init__.py
--rw-r--r--   0 rixx      (1000) rixx      (1000)      540 2022-10-31 23:20:04.000000 pretalx-youtube-1.0.4/pretalx_youtube/apps.py
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1561 2022-07-11 16:28:02.000000 pretalx-youtube-1.0.4/pretalx_youtube/forms.py
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:20:26.228866 pretalx-youtube-1.0.4/pretalx_youtube/locale/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:20:26.222199 pretalx-youtube-1.0.4/pretalx_youtube/locale/ar/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:20:26.228866 pretalx-youtube-1.0.4/pretalx_youtube/locale/ar/LC_MESSAGES/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      463 2022-10-31 00:02:40.000000 pretalx-youtube-1.0.4/pretalx_youtube/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1675 2022-10-31 23:19:24.000000 pretalx-youtube-1.0.4/pretalx_youtube/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:20:26.222199 pretalx-youtube-1.0.4/pretalx_youtube/locale/ca/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:20:26.232199 pretalx-youtube-1.0.4/pretalx_youtube/locale/ca/LC_MESSAGES/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      380 2022-10-31 00:02:40.000000 pretalx-youtube-1.0.4/pretalx_youtube/locale/ca/LC_MESSAGES/django.mo
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1589 2022-10-31 23:19:24.000000 pretalx-youtube-1.0.4/pretalx_youtube/locale/ca/LC_MESSAGES/django.po
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:20:26.222199 pretalx-youtube-1.0.4/pretalx_youtube/locale/cs/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:20:26.232199 pretalx-youtube-1.0.4/pretalx_youtube/locale/cs/LC_MESSAGES/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      460 2022-10-31 00:02:40.000000 pretalx-youtube-1.0.4/pretalx_youtube/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1672 2022-10-31 23:19:24.000000 pretalx-youtube-1.0.4/pretalx_youtube/locale/cs/LC_MESSAGES/django.po
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:20:26.222199 pretalx-youtube-1.0.4/pretalx_youtube/locale/de_DE/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:20:26.232199 pretalx-youtube-1.0.4/pretalx_youtube/locale/de_DE/LC_MESSAGES/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      337 2022-10-31 00:02:40.000000 pretalx-youtube-1.0.4/pretalx_youtube/locale/de_DE/LC_MESSAGES/django.mo
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1542 2022-10-31 23:19:24.000000 pretalx-youtube-1.0.4/pretalx_youtube/locale/de_DE/LC_MESSAGES/django.po
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:20:26.225533 pretalx-youtube-1.0.4/pretalx_youtube/locale/de_Formal/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:20:26.232199 pretalx-youtube-1.0.4/pretalx_youtube/locale/de_Formal/LC_MESSAGES/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      337 2022-10-31 00:02:40.000000 pretalx-youtube-1.0.4/pretalx_youtube/locale/de_Formal/LC_MESSAGES/django.mo
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1542 2022-10-31 23:19:24.000000 pretalx-youtube-1.0.4/pretalx_youtube/locale/de_Formal/LC_MESSAGES/django.po
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1542 2022-10-31 00:08:24.000000 pretalx-youtube-1.0.4/pretalx_youtube/locale/django.pot
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:20:26.225533 pretalx-youtube-1.0.4/pretalx_youtube/locale/el/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:20:26.232199 pretalx-youtube-1.0.4/pretalx_youtube/locale/el/LC_MESSAGES/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      380 2022-10-31 00:02:40.000000 pretalx-youtube-1.0.4/pretalx_youtube/locale/el/LC_MESSAGES/django.mo
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1589 2022-10-31 23:19:24.000000 pretalx-youtube-1.0.4/pretalx_youtube/locale/el/LC_MESSAGES/django.po
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:20:26.225533 pretalx-youtube-1.0.4/pretalx_youtube/locale/es/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:20:26.232199 pretalx-youtube-1.0.4/pretalx_youtube/locale/es/LC_MESSAGES/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      380 2022-10-31 00:02:40.000000 pretalx-youtube-1.0.4/pretalx_youtube/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1589 2022-10-31 23:19:24.000000 pretalx-youtube-1.0.4/pretalx_youtube/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:20:26.225533 pretalx-youtube-1.0.4/pretalx_youtube/locale/es_MX/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:20:26.235533 pretalx-youtube-1.0.4/pretalx_youtube/locale/es_MX/LC_MESSAGES/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      380 2022-10-31 00:02:40.000000 pretalx-youtube-1.0.4/pretalx_youtube/locale/es_MX/LC_MESSAGES/django.mo
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1589 2022-10-31 23:19:24.000000 pretalx-youtube-1.0.4/pretalx_youtube/locale/es_MX/LC_MESSAGES/django.po
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:20:26.225533 pretalx-youtube-1.0.4/pretalx_youtube/locale/fr_FR/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:20:26.235533 pretalx-youtube-1.0.4/pretalx_youtube/locale/fr_FR/LC_MESSAGES/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      337 2022-10-31 00:02:40.000000 pretalx-youtube-1.0.4/pretalx_youtube/locale/fr_FR/LC_MESSAGES/django.mo
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1542 2022-10-31 23:19:24.000000 pretalx-youtube-1.0.4/pretalx_youtube/locale/fr_FR/LC_MESSAGES/django.po
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:20:26.225533 pretalx-youtube-1.0.4/pretalx_youtube/locale/it/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:20:26.235533 pretalx-youtube-1.0.4/pretalx_youtube/locale/it/LC_MESSAGES/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      380 2022-10-31 00:02:40.000000 pretalx-youtube-1.0.4/pretalx_youtube/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1589 2022-10-31 23:19:24.000000 pretalx-youtube-1.0.4/pretalx_youtube/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:20:26.225533 pretalx-youtube-1.0.4/pretalx_youtube/locale/ja_JP/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:20:26.235533 pretalx-youtube-1.0.4/pretalx_youtube/locale/ja_JP/LC_MESSAGES/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      337 2022-10-31 00:02:40.000000 pretalx-youtube-1.0.4/pretalx_youtube/locale/ja_JP/LC_MESSAGES/django.mo
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1542 2022-10-31 23:19:24.000000 pretalx-youtube-1.0.4/pretalx_youtube/locale/ja_JP/LC_MESSAGES/django.po
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:20:26.225533 pretalx-youtube-1.0.4/pretalx_youtube/locale/pt_BR/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:20:26.235533 pretalx-youtube-1.0.4/pretalx_youtube/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      379 2022-10-31 00:02:40.000000 pretalx-youtube-1.0.4/pretalx_youtube/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1588 2022-10-31 23:19:24.000000 pretalx-youtube-1.0.4/pretalx_youtube/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:20:26.225533 pretalx-youtube-1.0.4/pretalx_youtube/locale/zh_TW/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:20:26.235533 pretalx-youtube-1.0.4/pretalx_youtube/locale/zh_TW/LC_MESSAGES/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      337 2022-10-31 00:02:40.000000 pretalx-youtube-1.0.4/pretalx_youtube/locale/zh_TW/LC_MESSAGES/django.mo
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1542 2022-10-31 23:19:24.000000 pretalx-youtube-1.0.4/pretalx_youtube/locale/zh_TW/LC_MESSAGES/django.po
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:20:26.235533 pretalx-youtube-1.0.4/pretalx_youtube/migrations/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      973 2021-12-15 01:24:02.000000 pretalx-youtube-1.0.4/pretalx_youtube/migrations/0001_initial.py
--rw-r--r--   0 rixx      (1000) rixx      (1000)        0 2021-12-15 01:19:02.000000 pretalx-youtube-1.0.4/pretalx_youtube/migrations/__init__.py
--rw-r--r--   0 rixx      (1000) rixx      (1000)      820 2021-12-15 01:24:02.000000 pretalx-youtube-1.0.4/pretalx_youtube/models.py
--rw-r--r--   0 rixx      (1000) rixx      (1000)      372 2021-12-15 01:24:02.000000 pretalx-youtube-1.0.4/pretalx_youtube/recording.py
--rw-r--r--   0 rixx      (1000) rixx      (1000)      841 2021-12-15 01:21:10.000000 pretalx-youtube-1.0.4/pretalx_youtube/signals.py
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:20:26.225533 pretalx-youtube-1.0.4/pretalx_youtube/static/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:20:26.235533 pretalx-youtube-1.0.4/pretalx_youtube/static/pretalx_youtube/
--rw-r--r--   0 rixx      (1000) rixx      (1000)        0 2021-12-15 01:09:31.000000 pretalx-youtube-1.0.4/pretalx_youtube/static/pretalx_youtube/.gitkeep
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:20:26.225533 pretalx-youtube-1.0.4/pretalx_youtube/templates/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:20:26.235533 pretalx-youtube-1.0.4/pretalx_youtube/templates/pretalx_youtube/
--rw-r--r--   0 rixx      (1000) rixx      (1000)        0 2021-12-15 01:09:31.000000 pretalx-youtube-1.0.4/pretalx_youtube/templates/pretalx_youtube/.gitkeep
--rw-r--r--   0 rixx      (1000) rixx      (1000)      821 2021-12-15 01:23:22.000000 pretalx-youtube-1.0.4/pretalx_youtube/templates/pretalx_youtube/settings.html
--rw-r--r--   0 rixx      (1000) rixx      (1000)      602 2022-07-11 16:28:30.000000 pretalx-youtube-1.0.4/pretalx_youtube/urls.py
--rw-r--r--   0 rixx      (1000) rixx      (1000)     2587 2021-12-15 01:21:43.000000 pretalx-youtube-1.0.4/pretalx_youtube/views.py
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:20:26.228866 pretalx-youtube-1.0.4/pretalx_youtube.egg-info/
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1496 2022-10-31 23:20:26.000000 pretalx-youtube-1.0.4/pretalx_youtube.egg-info/PKG-INFO
--rw-r--r--   0 rixx      (1000) rixx      (1000)     2033 2022-10-31 23:20:26.000000 pretalx-youtube-1.0.4/pretalx_youtube.egg-info/SOURCES.txt
--rw-r--r--   0 rixx      (1000) rixx      (1000)        1 2022-10-31 23:20:26.000000 pretalx-youtube-1.0.4/pretalx_youtube.egg-info/dependency_links.txt
--rw-r--r--   0 rixx      (1000) rixx      (1000)       68 2022-10-31 23:20:26.000000 pretalx-youtube-1.0.4/pretalx_youtube.egg-info/entry_points.txt
--rw-r--r--   0 rixx      (1000) rixx      (1000)       16 2022-10-31 23:20:26.000000 pretalx-youtube-1.0.4/pretalx_youtube.egg-info/top_level.txt
--rw-r--r--   0 rixx      (1000) rixx      (1000)      530 2022-10-31 23:20:26.238866 pretalx-youtube-1.0.4/setup.cfg
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1045 2022-10-31 23:19:53.000000 pretalx-youtube-1.0.4/setup.py
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:07:01.231899 pretalx-youtube-1.1.0/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      553 2021-12-15 01:11:11.000000 pretalx-youtube-1.1.0/LICENSE
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      230 2022-01-28 01:52:30.000000 pretalx-youtube-1.1.0/MANIFEST.in
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      142 2021-12-15 01:09:31.000000 pretalx-youtube-1.1.0/Makefile
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1476 2023-06-09 13:07:01.231899 pretalx-youtube-1.1.0/PKG-INFO
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1210 2021-12-15 01:28:25.000000 pretalx-youtube-1.1.0/README.rst
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:07:01.228565 pretalx-youtube-1.1.0/pretalx_youtube/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:19:32.000000 pretalx-youtube-1.1.0/pretalx_youtube/__init__.py
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      540 2023-06-09 13:06:24.000000 pretalx-youtube-1.1.0/pretalx_youtube/apps.py
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1859 2023-06-09 13:06:24.000000 pretalx-youtube-1.1.0/pretalx_youtube/forms.py
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:07:01.228565 pretalx-youtube-1.1.0/pretalx_youtube/locale/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:07:01.225232 pretalx-youtube-1.1.0/pretalx_youtube/locale/ar/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:07:01.228565 pretalx-youtube-1.1.0/pretalx_youtube/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      463 2023-06-09 13:06:52.000000 pretalx-youtube-1.1.0/pretalx_youtube/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1675 2023-06-09 13:05:07.000000 pretalx-youtube-1.1.0/pretalx_youtube/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:07:01.225232 pretalx-youtube-1.1.0/pretalx_youtube/locale/ca/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:07:01.228565 pretalx-youtube-1.1.0/pretalx_youtube/locale/ca/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      380 2023-06-09 13:06:52.000000 pretalx-youtube-1.1.0/pretalx_youtube/locale/ca/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1589 2023-06-09 13:05:07.000000 pretalx-youtube-1.1.0/pretalx_youtube/locale/ca/LC_MESSAGES/django.po
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:07:01.225232 pretalx-youtube-1.1.0/pretalx_youtube/locale/cs/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:07:01.228565 pretalx-youtube-1.1.0/pretalx_youtube/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1308 2023-06-09 13:06:52.000000 pretalx-youtube-1.1.0/pretalx_youtube/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     2030 2023-06-09 13:06:24.000000 pretalx-youtube-1.1.0/pretalx_youtube/locale/cs/LC_MESSAGES/django.po
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:07:01.225232 pretalx-youtube-1.1.0/pretalx_youtube/locale/de_DE/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:07:01.231899 pretalx-youtube-1.1.0/pretalx_youtube/locale/de_DE/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      337 2023-06-09 13:06:52.000000 pretalx-youtube-1.1.0/pretalx_youtube/locale/de_DE/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1542 2023-06-09 13:05:07.000000 pretalx-youtube-1.1.0/pretalx_youtube/locale/de_DE/LC_MESSAGES/django.po
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:07:01.225232 pretalx-youtube-1.1.0/pretalx_youtube/locale/de_Formal/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:07:01.231899 pretalx-youtube-1.1.0/pretalx_youtube/locale/de_Formal/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      337 2023-06-09 13:06:52.000000 pretalx-youtube-1.1.0/pretalx_youtube/locale/de_Formal/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1542 2023-06-09 13:05:07.000000 pretalx-youtube-1.1.0/pretalx_youtube/locale/de_Formal/LC_MESSAGES/django.po
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1542 2023-06-07 09:15:13.000000 pretalx-youtube-1.1.0/pretalx_youtube/locale/django.pot
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:07:01.228565 pretalx-youtube-1.1.0/pretalx_youtube/locale/el/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:07:01.231899 pretalx-youtube-1.1.0/pretalx_youtube/locale/el/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      380 2023-06-09 13:06:52.000000 pretalx-youtube-1.1.0/pretalx_youtube/locale/el/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1589 2023-06-09 13:05:07.000000 pretalx-youtube-1.1.0/pretalx_youtube/locale/el/LC_MESSAGES/django.po
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:07:01.228565 pretalx-youtube-1.1.0/pretalx_youtube/locale/en_Mozilla/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:07:01.231899 pretalx-youtube-1.1.0/pretalx_youtube/locale/en_Mozilla/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      337 2023-05-13 03:03:13.000000 pretalx-youtube-1.1.0/pretalx_youtube/locale/en_Mozilla/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1542 2023-02-19 15:38:17.000000 pretalx-youtube-1.1.0/pretalx_youtube/locale/en_Mozilla/LC_MESSAGES/django.po
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:07:01.228565 pretalx-youtube-1.1.0/pretalx_youtube/locale/es/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:07:01.231899 pretalx-youtube-1.1.0/pretalx_youtube/locale/es/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      380 2023-06-09 13:06:52.000000 pretalx-youtube-1.1.0/pretalx_youtube/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1589 2023-06-09 13:05:07.000000 pretalx-youtube-1.1.0/pretalx_youtube/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:07:01.228565 pretalx-youtube-1.1.0/pretalx_youtube/locale/es_MX/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:07:01.231899 pretalx-youtube-1.1.0/pretalx_youtube/locale/es_MX/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      380 2023-06-09 13:06:52.000000 pretalx-youtube-1.1.0/pretalx_youtube/locale/es_MX/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1589 2023-06-09 13:05:07.000000 pretalx-youtube-1.1.0/pretalx_youtube/locale/es_MX/LC_MESSAGES/django.po
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:07:01.228565 pretalx-youtube-1.1.0/pretalx_youtube/locale/fr_FR/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:07:01.231899 pretalx-youtube-1.1.0/pretalx_youtube/locale/fr_FR/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      337 2023-06-09 13:06:52.000000 pretalx-youtube-1.1.0/pretalx_youtube/locale/fr_FR/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1542 2023-06-09 13:05:07.000000 pretalx-youtube-1.1.0/pretalx_youtube/locale/fr_FR/LC_MESSAGES/django.po
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:07:01.228565 pretalx-youtube-1.1.0/pretalx_youtube/locale/it/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:07:01.231899 pretalx-youtube-1.1.0/pretalx_youtube/locale/it/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      380 2023-06-09 13:06:52.000000 pretalx-youtube-1.1.0/pretalx_youtube/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1589 2023-06-09 13:05:07.000000 pretalx-youtube-1.1.0/pretalx_youtube/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:07:01.228565 pretalx-youtube-1.1.0/pretalx_youtube/locale/ja_JP/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:07:01.231899 pretalx-youtube-1.1.0/pretalx_youtube/locale/ja_JP/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      337 2023-06-09 13:06:52.000000 pretalx-youtube-1.1.0/pretalx_youtube/locale/ja_JP/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1542 2023-06-09 13:05:07.000000 pretalx-youtube-1.1.0/pretalx_youtube/locale/ja_JP/LC_MESSAGES/django.po
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:07:01.228565 pretalx-youtube-1.1.0/pretalx_youtube/locale/pt_BR/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:07:01.231899 pretalx-youtube-1.1.0/pretalx_youtube/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      379 2023-06-09 13:06:52.000000 pretalx-youtube-1.1.0/pretalx_youtube/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1588 2023-06-09 13:05:07.000000 pretalx-youtube-1.1.0/pretalx_youtube/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:07:01.228565 pretalx-youtube-1.1.0/pretalx_youtube/locale/pt_PT/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:07:01.231899 pretalx-youtube-1.1.0/pretalx_youtube/locale/pt_PT/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      337 2023-05-13 03:03:13.000000 pretalx-youtube-1.1.0/pretalx_youtube/locale/pt_PT/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1542 2023-02-19 15:38:17.000000 pretalx-youtube-1.1.0/pretalx_youtube/locale/pt_PT/LC_MESSAGES/django.po
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:07:01.228565 pretalx-youtube-1.1.0/pretalx_youtube/locale/zh_TW/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:07:01.231899 pretalx-youtube-1.1.0/pretalx_youtube/locale/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      337 2023-06-09 13:06:52.000000 pretalx-youtube-1.1.0/pretalx_youtube/locale/zh_TW/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1542 2023-06-09 13:05:07.000000 pretalx-youtube-1.1.0/pretalx_youtube/locale/zh_TW/LC_MESSAGES/django.po
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:07:01.231899 pretalx-youtube-1.1.0/pretalx_youtube/migrations/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      972 2023-06-09 13:06:24.000000 pretalx-youtube-1.1.0/pretalx_youtube/migrations/0001_initial.py
+-rw-r--r--   0 rixx      (1000) rixx      (1000)        0 2021-12-15 01:19:02.000000 pretalx-youtube-1.1.0/pretalx_youtube/migrations/__init__.py
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      820 2021-12-15 01:24:02.000000 pretalx-youtube-1.1.0/pretalx_youtube/models.py
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      372 2021-12-15 01:24:02.000000 pretalx-youtube-1.1.0/pretalx_youtube/recording.py
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      841 2021-12-15 01:21:10.000000 pretalx-youtube-1.1.0/pretalx_youtube/signals.py
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:07:01.228565 pretalx-youtube-1.1.0/pretalx_youtube/static/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:07:01.231899 pretalx-youtube-1.1.0/pretalx_youtube/static/pretalx_youtube/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)        0 2021-12-15 01:09:31.000000 pretalx-youtube-1.1.0/pretalx_youtube/static/pretalx_youtube/.gitkeep
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:07:01.228565 pretalx-youtube-1.1.0/pretalx_youtube/templates/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:07:01.231899 pretalx-youtube-1.1.0/pretalx_youtube/templates/pretalx_youtube/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)        0 2021-12-15 01:09:31.000000 pretalx-youtube-1.1.0/pretalx_youtube/templates/pretalx_youtube/.gitkeep
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      821 2021-12-15 01:23:22.000000 pretalx-youtube-1.1.0/pretalx_youtube/templates/pretalx_youtube/settings.html
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      602 2022-07-11 16:28:30.000000 pretalx-youtube-1.1.0/pretalx_youtube/urls.py
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     2587 2021-12-15 01:21:43.000000 pretalx-youtube-1.1.0/pretalx_youtube/views.py
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:07:01.228565 pretalx-youtube-1.1.0/pretalx_youtube.egg-info/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1476 2023-06-09 13:07:01.000000 pretalx-youtube-1.1.0/pretalx_youtube.egg-info/PKG-INFO
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     2247 2023-06-09 13:07:01.000000 pretalx-youtube-1.1.0/pretalx_youtube.egg-info/SOURCES.txt
+-rw-r--r--   0 rixx      (1000) rixx      (1000)        1 2023-06-09 13:07:01.000000 pretalx-youtube-1.1.0/pretalx_youtube.egg-info/dependency_links.txt
+-rw-r--r--   0 rixx      (1000) rixx      (1000)       69 2023-06-09 13:07:01.000000 pretalx-youtube-1.1.0/pretalx_youtube.egg-info/entry_points.txt
+-rw-r--r--   0 rixx      (1000) rixx      (1000)       16 2023-06-09 13:07:01.000000 pretalx-youtube-1.1.0/pretalx_youtube.egg-info/top_level.txt
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      530 2023-06-09 13:07:01.231899 pretalx-youtube-1.1.0/setup.cfg
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1045 2023-06-09 13:06:24.000000 pretalx-youtube-1.1.0/setup.py
```

### Comparing `pretalx-youtube-1.0.4/LICENSE` & `pretalx-youtube-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pretalx-youtube-1.0.4/PKG-INFO` & `pretalx-youtube-1.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: pretalx-youtube
-Version: 1.0.4
+Version: 1.1.0
 Summary: Embed YouTube videos as session recordings
 Home-page: https://github.com/pretalx/pretalx-youtube
 Author: Tobias Kunze
 Author-email: r@rixx.de
 License: Apache Software License
-Platform: UNKNOWN
 License-File: LICENSE
 
 Youtube integration
 ===================
 
 This is a plugin for `pretalx`_ that provides an integration with Youtube, allowing you to embed recordings on talk pages.
 
@@ -40,9 +39,7 @@
 Copyright 2021 Tobias Kunze
 
 Released under the terms of the Apache License 2.0
 
 
 .. _pretalx: https://github.com/pretalx/pretalx
 .. _pretalx development setup: https://docs.pretalx.org/en/latest/developer/setup.html
-
-
```

### Comparing `pretalx-youtube-1.0.4/README.rst` & `pretalx-youtube-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `pretalx-youtube-1.0.4/pretalx_youtube/apps.py` & `pretalx-youtube-1.1.0/pretalx_youtube/apps.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,11 +9,11 @@
     class PretalxPluginMeta:
         name = gettext_lazy("YouTube integration")
         author = "Tobias Kunze"
         description = gettext_lazy(
             "Embed YouTube videos as session recordings, and retrieve them via an API."
         )
         visible = True
-        version = "1.0.4"
+        version = "1.1.0"
 
     def ready(self):
         from . import signals  # NOQA
```

### Comparing `pretalx-youtube-1.0.4/pretalx_youtube/forms.py` & `pretalx-youtube-1.1.0/pretalx_youtube/forms.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from django import forms
 from django.utils.translation import gettext_lazy as _
 
 from .models import YouTubeLink
 
 
 class YouTubeUrlForm(forms.Form):
-
     video_id = forms.URLField(required=False)
 
     def __init__(self, *args, **kwargs):
         self.submission = kwargs.pop("submission")
 
         youtube = getattr(self.submission, "youtube_link", None)
         if youtube:
@@ -21,22 +20,29 @@
         super().__init__(*args, **kwargs)
         self.fields["video_id"].label = self.submission.title
 
     def clean_video_id(self):
         data = self.cleaned_data["video_id"]
         if not data:
             return data
-        if "youtube.com" not in data:
+        # Get ID from youtube.com and youtu.be URLs
+        if "youtube.com" in data:
+            try:
+                url = urlparse(data)
+                qs = parse_qs(url.query)
+                return qs["v"][0]
+            except Exception as e:
+                raise forms.ValidationError(_("Failed to parse the URL!") + f" {e}")
+        elif "youtu.be" in data:
+            try:
+                return data.split("/")[-1]
+            except Exception as e:
+                raise forms.ValidationError(_("Failed to parse the URL!") + f" {e}")
+        else:
             raise forms.ValidationError(_("Please provide a YouTube URL!"))
-        try:
-            url = urlparse(data)
-            qs = parse_qs(url.query)
-            return qs["v"][0]
-        except Exception as e:
-            raise forms.ValidationError(_("Failed to parse the URL!") + f" {e}")
 
     def save(self):
         video_id = self.cleaned_data.get("video_id")
         if video_id:
             YouTubeLink.objects.update_or_create(
                 submission=self.submission, defaults={"video_id": video_id}
             )
```

### Comparing `pretalx-youtube-1.0.4/pretalx_youtube/locale/ar/LC_MESSAGES/django.po` & `pretalx-youtube-1.1.0/pretalx_youtube/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretalx-youtube-1.0.4/pretalx_youtube/locale/ca/LC_MESSAGES/django.po` & `pretalx-youtube-1.1.0/pretalx_youtube/locale/ca/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretalx-youtube-1.0.4/pretalx_youtube/locale/cs/LC_MESSAGES/django.po` & `pretalx-youtube-1.1.0/pretalx_youtube/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files 5% similar despite different names*

```diff
@@ -12,16 +12,15 @@
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n >= 2 && n "
-"<= 4 && n % 1 == 0) ? 1: (n % 1 != 0 ) ? 2 : 3;\n"
+"Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
 #: local/pretalx-youtube/pretalx_youtube/apps.py:10
 msgid "YouTube integration"
 msgstr ""
 
 #: local/pretalx-youtube/pretalx_youtube/apps.py:13
 msgid ""
```

### Comparing `pretalx-youtube-1.0.4/pretalx_youtube/locale/de_DE/LC_MESSAGES/django.po` & `pretalx-youtube-1.1.0/pretalx_youtube/locale/de_DE/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretalx-youtube-1.0.4/pretalx_youtube/locale/de_Formal/LC_MESSAGES/django.po` & `pretalx-youtube-1.1.0/pretalx_youtube/locale/de_Formal/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretalx-youtube-1.0.4/pretalx_youtube/locale/django.pot` & `pretalx-youtube-1.1.0/pretalx_youtube/locale/django.pot`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-31 00:08+0000\n"
+"POT-Creation-Date: 2023-06-07 09:15+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -22,19 +22,19 @@
 msgstr ""
 
 #: local/pretalx-youtube/pretalx_youtube/apps.py:13
 msgid ""
 "Embed YouTube videos as session recordings, and retrieve them via an API."
 msgstr ""
 
-#: local/pretalx-youtube/pretalx_youtube/forms.py:29
+#: local/pretalx-youtube/pretalx_youtube/forms.py:28
 msgid "Please provide a YouTube URL!"
 msgstr ""
 
-#: local/pretalx-youtube/pretalx_youtube/forms.py:35
+#: local/pretalx-youtube/pretalx_youtube/forms.py:34
 msgid "Failed to parse the URL!"
 msgstr ""
 
 #: local/pretalx-youtube/pretalx_youtube/templates/pretalx_youtube/settings.html:7
 msgid "Set up YouTube embeds"
 msgstr ""
```

### Comparing `pretalx-youtube-1.0.4/pretalx_youtube/locale/el/LC_MESSAGES/django.po` & `pretalx-youtube-1.1.0/pretalx_youtube/locale/el/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretalx-youtube-1.0.4/pretalx_youtube/locale/es/LC_MESSAGES/django.po` & `pretalx-youtube-1.1.0/pretalx_youtube/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretalx-youtube-1.0.4/pretalx_youtube/locale/es_MX/LC_MESSAGES/django.po` & `pretalx-youtube-1.1.0/pretalx_youtube/locale/es_MX/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretalx-youtube-1.0.4/pretalx_youtube/locale/fr_FR/LC_MESSAGES/django.po` & `pretalx-youtube-1.1.0/pretalx_youtube/locale/fr_FR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretalx-youtube-1.0.4/pretalx_youtube/locale/it/LC_MESSAGES/django.po` & `pretalx-youtube-1.1.0/pretalx_youtube/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretalx-youtube-1.0.4/pretalx_youtube/locale/ja_JP/LC_MESSAGES/django.po` & `pretalx-youtube-1.1.0/pretalx_youtube/locale/ja_JP/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretalx-youtube-1.0.4/pretalx_youtube/locale/pt_BR/LC_MESSAGES/django.po` & `pretalx-youtube-1.1.0/pretalx_youtube/locale/zh_TW/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
 #: local/pretalx-youtube/pretalx_youtube/apps.py:10
 msgid "YouTube integration"
 msgstr ""
 
 #: local/pretalx-youtube/pretalx_youtube/apps.py:13
 msgid ""
```

### Comparing `pretalx-youtube-1.0.4/pretalx_youtube/locale/zh_TW/LC_MESSAGES/django.po` & `pretalx-youtube-1.1.0/pretalx_youtube/locale/en_Mozilla/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-05-17 23:58+0000\n"
+"POT-Creation-Date: 2023-02-19 15:38+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -22,19 +22,19 @@
 msgstr ""
 
 #: local/pretalx-youtube/pretalx_youtube/apps.py:13
 msgid ""
 "Embed YouTube videos as session recordings, and retrieve them via an API."
 msgstr ""
 
-#: local/pretalx-youtube/pretalx_youtube/forms.py:27
+#: local/pretalx-youtube/pretalx_youtube/forms.py:28
 msgid "Please provide a YouTube URL!"
 msgstr ""
 
-#: local/pretalx-youtube/pretalx_youtube/forms.py:33
+#: local/pretalx-youtube/pretalx_youtube/forms.py:34
 msgid "Failed to parse the URL!"
 msgstr ""
 
 #: local/pretalx-youtube/pretalx_youtube/templates/pretalx_youtube/settings.html:7
 msgid "Set up YouTube embeds"
 msgstr ""
```

### Comparing `pretalx-youtube-1.0.4/pretalx_youtube/migrations/0001_initial.py` & `pretalx-youtube-1.1.0/pretalx_youtube/migrations/0001_initial.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Generated by Django 3.2.4 on 2021-12-15 01:23
 
 from django.db import migrations, models
 import django.db.models.deletion
 
 
 class Migration(migrations.Migration):
-
     initial = True
 
     dependencies = [
         ("submission", "0062_cfp_settings_data"),
     ]
 
     operations = [
```

### Comparing `pretalx-youtube-1.0.4/pretalx_youtube/models.py` & `pretalx-youtube-1.1.0/pretalx_youtube/models.py`

 * *Files identical despite different names*

### Comparing `pretalx-youtube-1.0.4/pretalx_youtube/signals.py` & `pretalx-youtube-1.1.0/pretalx_youtube/signals.py`

 * *Files identical despite different names*

### Comparing `pretalx-youtube-1.0.4/pretalx_youtube/templates/pretalx_youtube/settings.html` & `pretalx-youtube-1.1.0/pretalx_youtube/templates/pretalx_youtube/settings.html`

 * *Files identical despite different names*

### Comparing `pretalx-youtube-1.0.4/pretalx_youtube/urls.py` & `pretalx-youtube-1.1.0/pretalx_youtube/urls.py`

 * *Files identical despite different names*

### Comparing `pretalx-youtube-1.0.4/pretalx_youtube/views.py` & `pretalx-youtube-1.1.0/pretalx_youtube/views.py`

 * *Files identical despite different names*

### Comparing `pretalx-youtube-1.0.4/pretalx_youtube.egg-info/PKG-INFO` & `pretalx-youtube-1.1.0/pretalx_youtube.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: pretalx-youtube
-Version: 1.0.4
+Version: 1.1.0
 Summary: Embed YouTube videos as session recordings
 Home-page: https://github.com/pretalx/pretalx-youtube
 Author: Tobias Kunze
 Author-email: r@rixx.de
 License: Apache Software License
-Platform: UNKNOWN
 License-File: LICENSE
 
 Youtube integration
 ===================
 
 This is a plugin for `pretalx`_ that provides an integration with Youtube, allowing you to embed recordings on talk pages.
 
@@ -40,9 +39,7 @@
 Copyright 2021 Tobias Kunze
 
 Released under the terms of the Apache License 2.0
 
 
 .. _pretalx: https://github.com/pretalx/pretalx
 .. _pretalx development setup: https://docs.pretalx.org/en/latest/developer/setup.html
-
-
```

### Comparing `pretalx-youtube-1.0.4/pretalx_youtube.egg-info/SOURCES.txt` & `pretalx-youtube-1.1.0/pretalx_youtube.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -26,26 +26,30 @@
 pretalx_youtube/locale/cs/LC_MESSAGES/django.po
 pretalx_youtube/locale/de_DE/LC_MESSAGES/django.mo
 pretalx_youtube/locale/de_DE/LC_MESSAGES/django.po
 pretalx_youtube/locale/de_Formal/LC_MESSAGES/django.mo
 pretalx_youtube/locale/de_Formal/LC_MESSAGES/django.po
 pretalx_youtube/locale/el/LC_MESSAGES/django.mo
 pretalx_youtube/locale/el/LC_MESSAGES/django.po
+pretalx_youtube/locale/en_Mozilla/LC_MESSAGES/django.mo
+pretalx_youtube/locale/en_Mozilla/LC_MESSAGES/django.po
 pretalx_youtube/locale/es/LC_MESSAGES/django.mo
 pretalx_youtube/locale/es/LC_MESSAGES/django.po
 pretalx_youtube/locale/es_MX/LC_MESSAGES/django.mo
 pretalx_youtube/locale/es_MX/LC_MESSAGES/django.po
 pretalx_youtube/locale/fr_FR/LC_MESSAGES/django.mo
 pretalx_youtube/locale/fr_FR/LC_MESSAGES/django.po
 pretalx_youtube/locale/it/LC_MESSAGES/django.mo
 pretalx_youtube/locale/it/LC_MESSAGES/django.po
 pretalx_youtube/locale/ja_JP/LC_MESSAGES/django.mo
 pretalx_youtube/locale/ja_JP/LC_MESSAGES/django.po
 pretalx_youtube/locale/pt_BR/LC_MESSAGES/django.mo
 pretalx_youtube/locale/pt_BR/LC_MESSAGES/django.po
+pretalx_youtube/locale/pt_PT/LC_MESSAGES/django.mo
+pretalx_youtube/locale/pt_PT/LC_MESSAGES/django.po
 pretalx_youtube/locale/zh_TW/LC_MESSAGES/django.mo
 pretalx_youtube/locale/zh_TW/LC_MESSAGES/django.po
 pretalx_youtube/migrations/0001_initial.py
 pretalx_youtube/migrations/__init__.py
 pretalx_youtube/static/pretalx_youtube/.gitkeep
 pretalx_youtube/templates/pretalx_youtube/.gitkeep
 pretalx_youtube/templates/pretalx_youtube/settings.html
```

### Comparing `pretalx-youtube-1.0.4/setup.cfg` & `pretalx-youtube-1.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `pretalx-youtube-1.0.4/setup.py` & `pretalx-youtube-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 
 cmdclass = {"build": CustomBuild}
 
 
 setup(
     name="pretalx-youtube",
-    version="1.0.4",
+    version="1.1.0",
     description="Embed YouTube videos as session recordings",
     long_description=long_description,
     url="https://github.com/pretalx/pretalx-youtube",
     author="Tobias Kunze",
     author_email="r@rixx.de",
     license="Apache Software License",
     install_requires=[],
```

