# Comparing `tmp/pyarmor-webui-2.0.zip` & `tmp/pyarmor-webui-2.1.zip`

## zipinfo {}

```diff
@@ -1,58 +1,58 @@
-Zip file size: 355832 bytes, number of entries: 56
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-20 06:09 pyarmor-webui-2.0/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-20 06:09 pyarmor-webui-2.0/pyarmor_webui.egg-info/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-20 06:09 pyarmor-webui-2.0/test/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-20 06:09 pyarmor-webui-2.0/static/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-20 06:09 pyarmor-webui-2.0/data/
--rw-r--r--  2.0 unx     5581 b- defN 23-May-20 06:09 pyarmor-webui-2.0/PKG-INFO
--rw-r--r--  2.0 unx     9079 b- defN 23-May-12 06:28 pyarmor-webui-2.0/server.py
--rw-r--r--  2.0 unx    18983 b- defN 23-May-12 14:58 pyarmor-webui-2.0/handler.py
--rw-r--r--  2.0 unx     1068 b- defN 19-Dec-31 08:11 pyarmor-webui-2.0/LICENSE
--rwxr-xr-x  2.0 unx        0 b- defN 20-Mar-27 08:49 pyarmor-webui-2.0/__init__.py
--rw-r--r--  2.0 unx    16393 b- defN 23-May-12 23:59 pyarmor-webui-2.0/handler8.py
--rw-r--r--  2.0 unx     2241 b- defN 23-May-20 05:57 pyarmor-webui-2.0/setup.py
--rw-r--r--  2.0 unx       59 b- defN 23-May-20 06:09 pyarmor-webui-2.0/setup.cfg
--rw-r--r--  2.0 unx     3521 b- defN 23-May-12 06:36 pyarmor-webui-2.0/README.rst
--rw-r--r--  2.0 unx     5581 b- defN 23-May-20 06:09 pyarmor-webui-2.0/pyarmor_webui.egg-info/PKG-INFO
--rw-r--r--  2.0 unx     1323 b- defN 23-May-20 06:09 pyarmor-webui-2.0/pyarmor_webui.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx       61 b- defN 23-May-20 06:09 pyarmor-webui-2.0/pyarmor_webui.egg-info/entry_points.txt
--rw-r--r--  2.0 unx       15 b- defN 23-May-20 06:09 pyarmor-webui-2.0/pyarmor_webui.egg-info/requires.txt
--rw-r--r--  2.0 unx        8 b- defN 23-May-20 06:09 pyarmor-webui-2.0/pyarmor_webui.egg-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-May-20 06:09 pyarmor-webui-2.0/pyarmor_webui.egg-info/dependency_links.txt
--rwxr-xr-x  2.0 unx     1027 b- defN 20-Apr-27 09:39 pyarmor-webui-2.0/test/pack_one_folder_bundle.robot
--rwxr-xr-x  2.0 unx      693 b- defN 20-Oct-30 08:30 pyarmor-webui-2.0/test/generate_expired_license.robot
--rwxr-xr-x  2.0 unx     1475 b- defN 20-Apr-27 09:39 pyarmor-webui-2.0/test/pack_one_file_bundle_with_outer_license.robot
--rwxr-xr-x  2.0 unx     1245 b- defN 20-Jan-19 10:10 pyarmor-webui-2.0/test/obfuscate_multiple_entries.robot
--rwxr-xr-x  2.0 unx      890 b- defN 20-Apr-27 09:40 pyarmor-webui-2.0/test/generate_machine_license.robot
--rwxr-xr-x  2.0 unx     1164 b- defN 20-Jan-19 10:08 pyarmor-webui-2.0/test/obfuscate_one_script.robot
--rw-r--r--  2.0 unx     1899 b- defN 20-Apr-27 09:25 pyarmor-webui-2.0/test/README.md
--rwxr-xr-x  2.0 unx      777 b- defN 20-Apr-27 09:41 pyarmor-webui-2.0/test/generate_extra_data_license.robot
--rwxr-xr-x  2.0 unx     1230 b- defN 20-Jan-19 10:30 pyarmor-webui-2.0/test/obfuscate_one_package.robot
--rwxr-xr-x  2.0 unx     6422 b- defN 23-May-12 10:17 pyarmor-webui-2.0/test/resource.robot
--rwxr-xr-x  2.0 unx     1358 b- defN 20-Apr-27 09:39 pyarmor-webui-2.0/test/pack_with_data_file.robot
--rwxr-xr-x  2.0 unx     1139 b- defN 20-Apr-27 09:38 pyarmor-webui-2.0/test/pack_one_file_bundle.robot
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-20 06:09 pyarmor-webui-2.0/static/css/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-20 06:09 pyarmor-webui-2.0/static/js/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-20 06:09 pyarmor-webui-2.0/static/img/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-20 06:09 pyarmor-webui-2.0/static/fonts/
--rw-r--r--  2.0 unx     4286 b- defN 23-May-12 23:42 pyarmor-webui-2.0/static/favicon.ico
--rw-r--r--  2.0 unx      898 b- defN 23-May-12 23:42 pyarmor-webui-2.0/static/index.html
--rw-r--r--  2.0 unx    19211 b- defN 23-May-12 23:42 pyarmor-webui-2.0/static/reqwest.js
--rw-r--r--  2.0 unx     1166 b- defN 23-May-12 23:42 pyarmor-webui-2.0/static/css/app.9402d9fa.css
--rw-r--r--  2.0 unx   191299 b- defN 23-May-12 23:42 pyarmor-webui-2.0/static/css/chunk-vendors.b79ff3a2.css
--rw-r--r--  2.0 unx   716206 b- defN 23-May-12 23:42 pyarmor-webui-2.0/static/js/chunk-vendors.62e477e4.js
--rw-r--r--  2.0 unx   106859 b- defN 23-May-12 23:42 pyarmor-webui-2.0/static/js/app.8da2b1ed.js
--rw-r--r--  2.0 unx      890 b- defN 23-May-12 23:42 pyarmor-webui-2.0/static/img/cog.svg
--rw-r--r--  2.0 unx      207 b- defN 23-May-12 23:42 pyarmor-webui-2.0/static/img/folder-solid.svg
--rw-r--r--  2.0 unx      356 b- defN 23-May-12 23:42 pyarmor-webui-2.0/static/img/tablet-alt.svg
--rw-r--r--  2.0 unx      339 b- defN 23-May-12 23:42 pyarmor-webui-2.0/static/img/shield-alt.svg
--rw-r--r--  2.0 unx      935 b- defN 23-May-12 23:42 pyarmor-webui-2.0/static/img/calendar-alt.svg
--rw-r--r--  2.0 unx    14781 b- defN 23-May-12 23:42 pyarmor-webui-2.0/static/img/logo.a8954ff0.png
--rw-r--r--  2.0 unx      734 b- defN 23-May-12 23:42 pyarmor-webui-2.0/static/img/registered.svg
--rw-r--r--  2.0 unx      446 b- defN 23-May-12 23:42 pyarmor-webui-2.0/static/img/calendar-minus.svg
--rw-r--r--  2.0 unx      349 b- defN 23-May-12 23:42 pyarmor-webui-2.0/static/img/calendar.svg
--rw-r--r--  2.0 unx      307 b- defN 23-May-12 23:42 pyarmor-webui-2.0/static/img/folder.svg
--rw-r--r--  2.0 unx    28200 b- defN 23-May-12 23:42 pyarmor-webui-2.0/static/fonts/element-icons.535877f5.woff
--rw-r--r--  2.0 unx    55956 b- defN 23-May-12 23:42 pyarmor-webui-2.0/static/fonts/element-icons.732389de.ttf
--rw-r--r--  2.0 unx      205 b- defN 23-May-20 06:08 pyarmor-webui-2.0/data/copy_license.py
-56 files, 1226863 bytes uncompressed, 346950 bytes compressed:  71.7%
+Zip file size: 361995 bytes, number of entries: 56
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-09 14:29 pyarmor-webui-2.1/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-09 14:29 pyarmor-webui-2.1/pyarmor_webui.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-09 14:29 pyarmor-webui-2.1/test/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-09 14:29 pyarmor-webui-2.1/static/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-09 14:29 pyarmor-webui-2.1/data/
+-rw-r--r--  2.0 unx     5850 b- defN 23-Jun-09 14:29 pyarmor-webui-2.1/PKG-INFO
+-rw-r--r--  2.0 unx     9109 b- defN 23-May-21 08:01 pyarmor-webui-2.1/server.py
+-rw-r--r--  2.0 unx    18983 b- defN 23-May-12 14:58 pyarmor-webui-2.1/handler.py
+-rw-r--r--  2.0 unx     1068 b- defN 19-Dec-31 08:11 pyarmor-webui-2.1/LICENSE
+-rwxr-xr-x  2.0 unx        0 b- defN 20-Mar-27 08:49 pyarmor-webui-2.1/__init__.py
+-rw-r--r--  2.0 unx    18071 b- defN 23-Jun-08 23:28 pyarmor-webui-2.1/handler8.py
+-rw-r--r--  2.0 unx     2241 b- defN 23-Jun-08 17:14 pyarmor-webui-2.1/setup.py
+-rw-r--r--  2.0 unx       59 b- defN 23-Jun-09 14:29 pyarmor-webui-2.1/setup.cfg
+-rw-r--r--  2.0 unx     3710 b- defN 23-Jun-09 14:28 pyarmor-webui-2.1/README.rst
+-rw-r--r--  2.0 unx     5850 b- defN 23-Jun-09 14:29 pyarmor-webui-2.1/pyarmor_webui.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx     1323 b- defN 23-Jun-09 14:29 pyarmor-webui-2.1/pyarmor_webui.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx       61 b- defN 23-Jun-09 14:29 pyarmor-webui-2.1/pyarmor_webui.egg-info/entry_points.txt
+-rw-r--r--  2.0 unx       15 b- defN 23-Jun-09 14:29 pyarmor-webui-2.1/pyarmor_webui.egg-info/requires.txt
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-09 14:29 pyarmor-webui-2.1/pyarmor_webui.egg-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-09 14:29 pyarmor-webui-2.1/pyarmor_webui.egg-info/dependency_links.txt
+-rwxr-xr-x  2.0 unx     1027 b- defN 20-Apr-27 09:39 pyarmor-webui-2.1/test/pack_one_folder_bundle.robot
+-rwxr-xr-x  2.0 unx      693 b- defN 20-Oct-30 08:30 pyarmor-webui-2.1/test/generate_expired_license.robot
+-rwxr-xr-x  2.0 unx     1475 b- defN 20-Apr-27 09:39 pyarmor-webui-2.1/test/pack_one_file_bundle_with_outer_license.robot
+-rwxr-xr-x  2.0 unx     1245 b- defN 20-Jan-19 10:10 pyarmor-webui-2.1/test/obfuscate_multiple_entries.robot
+-rwxr-xr-x  2.0 unx      890 b- defN 20-Apr-27 09:40 pyarmor-webui-2.1/test/generate_machine_license.robot
+-rwxr-xr-x  2.0 unx     1164 b- defN 20-Jan-19 10:08 pyarmor-webui-2.1/test/obfuscate_one_script.robot
+-rw-r--r--  2.0 unx     1899 b- defN 20-Apr-27 09:25 pyarmor-webui-2.1/test/README.md
+-rwxr-xr-x  2.0 unx      777 b- defN 20-Apr-27 09:41 pyarmor-webui-2.1/test/generate_extra_data_license.robot
+-rwxr-xr-x  2.0 unx     1230 b- defN 20-Jan-19 10:30 pyarmor-webui-2.1/test/obfuscate_one_package.robot
+-rwxr-xr-x  2.0 unx     6422 b- defN 23-May-12 10:17 pyarmor-webui-2.1/test/resource.robot
+-rwxr-xr-x  2.0 unx     1358 b- defN 20-Apr-27 09:39 pyarmor-webui-2.1/test/pack_with_data_file.robot
+-rwxr-xr-x  2.0 unx     1139 b- defN 20-Apr-27 09:38 pyarmor-webui-2.1/test/pack_one_file_bundle.robot
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-09 14:29 pyarmor-webui-2.1/static/css/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-09 14:29 pyarmor-webui-2.1/static/js/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-09 14:29 pyarmor-webui-2.1/static/img/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-09 14:29 pyarmor-webui-2.1/static/fonts/
+-rw-r--r--  2.0 unx     4286 b- defN 23-Jun-08 21:14 pyarmor-webui-2.1/static/favicon.ico
+-rw-r--r--  2.0 unx      898 b- defN 23-Jun-08 21:14 pyarmor-webui-2.1/static/index.html
+-rw-r--r--  2.0 unx    19211 b- defN 23-Jun-08 21:14 pyarmor-webui-2.1/static/reqwest.js
+-rw-r--r--  2.0 unx   191299 b- defN 23-Jun-08 21:14 pyarmor-webui-2.1/static/css/chunk-vendors.b79ff3a2.css
+-rw-r--r--  2.0 unx     1166 b- defN 23-Jun-08 21:14 pyarmor-webui-2.1/static/css/app.b33816dc.css
+-rw-r--r--  2.0 unx   126894 b- defN 23-Jun-08 21:14 pyarmor-webui-2.1/static/js/app.d802fb34.js
+-rw-r--r--  2.0 unx   718168 b- defN 23-Jun-08 21:14 pyarmor-webui-2.1/static/js/chunk-vendors.4afc1da0.js
+-rw-r--r--  2.0 unx      890 b- defN 23-Jun-08 21:14 pyarmor-webui-2.1/static/img/cog.svg
+-rw-r--r--  2.0 unx      207 b- defN 23-Jun-08 21:14 pyarmor-webui-2.1/static/img/folder-solid.svg
+-rw-r--r--  2.0 unx      356 b- defN 23-Jun-08 21:14 pyarmor-webui-2.1/static/img/tablet-alt.svg
+-rw-r--r--  2.0 unx      339 b- defN 23-Jun-08 21:14 pyarmor-webui-2.1/static/img/shield-alt.svg
+-rw-r--r--  2.0 unx      935 b- defN 23-Jun-08 21:14 pyarmor-webui-2.1/static/img/calendar-alt.svg
+-rw-r--r--  2.0 unx    14781 b- defN 23-Jun-08 21:14 pyarmor-webui-2.1/static/img/logo.a8954ff0.png
+-rw-r--r--  2.0 unx      734 b- defN 23-Jun-08 21:14 pyarmor-webui-2.1/static/img/registered.svg
+-rw-r--r--  2.0 unx      446 b- defN 23-Jun-08 21:14 pyarmor-webui-2.1/static/img/calendar-minus.svg
+-rw-r--r--  2.0 unx      349 b- defN 23-Jun-08 21:14 pyarmor-webui-2.1/static/img/calendar.svg
+-rw-r--r--  2.0 unx      307 b- defN 23-Jun-08 21:14 pyarmor-webui-2.1/static/img/folder.svg
+-rw-r--r--  2.0 unx    28200 b- defN 23-Jun-08 21:14 pyarmor-webui-2.1/static/fonts/element-icons.535877f5.woff
+-rw-r--r--  2.0 unx    55956 b- defN 23-Jun-08 21:14 pyarmor-webui-2.1/static/fonts/element-icons.732389de.ttf
+-rw-r--r--  2.0 unx      205 b- defN 23-May-20 06:08 pyarmor-webui-2.1/data/copy_license.py
+56 files, 1251295 bytes uncompressed, 353113 bytes compressed:  71.8%
```

## zipnote {}

```diff
@@ -1,169 +1,169 @@
-Filename: pyarmor-webui-2.0/
+Filename: pyarmor-webui-2.1/
 Comment: 
 
-Filename: pyarmor-webui-2.0/pyarmor_webui.egg-info/
+Filename: pyarmor-webui-2.1/pyarmor_webui.egg-info/
 Comment: 
 
-Filename: pyarmor-webui-2.0/test/
+Filename: pyarmor-webui-2.1/test/
 Comment: 
 
-Filename: pyarmor-webui-2.0/static/
+Filename: pyarmor-webui-2.1/static/
 Comment: 
 
-Filename: pyarmor-webui-2.0/data/
+Filename: pyarmor-webui-2.1/data/
 Comment: 
 
-Filename: pyarmor-webui-2.0/PKG-INFO
+Filename: pyarmor-webui-2.1/PKG-INFO
 Comment: 
 
-Filename: pyarmor-webui-2.0/server.py
+Filename: pyarmor-webui-2.1/server.py
 Comment: 
 
-Filename: pyarmor-webui-2.0/handler.py
+Filename: pyarmor-webui-2.1/handler.py
 Comment: 
 
-Filename: pyarmor-webui-2.0/LICENSE
+Filename: pyarmor-webui-2.1/LICENSE
 Comment: 
 
-Filename: pyarmor-webui-2.0/__init__.py
+Filename: pyarmor-webui-2.1/__init__.py
 Comment: 
 
-Filename: pyarmor-webui-2.0/handler8.py
+Filename: pyarmor-webui-2.1/handler8.py
 Comment: 
 
-Filename: pyarmor-webui-2.0/setup.py
+Filename: pyarmor-webui-2.1/setup.py
 Comment: 
 
-Filename: pyarmor-webui-2.0/setup.cfg
+Filename: pyarmor-webui-2.1/setup.cfg
 Comment: 
 
-Filename: pyarmor-webui-2.0/README.rst
+Filename: pyarmor-webui-2.1/README.rst
 Comment: 
 
-Filename: pyarmor-webui-2.0/pyarmor_webui.egg-info/PKG-INFO
+Filename: pyarmor-webui-2.1/pyarmor_webui.egg-info/PKG-INFO
 Comment: 
 
-Filename: pyarmor-webui-2.0/pyarmor_webui.egg-info/SOURCES.txt
+Filename: pyarmor-webui-2.1/pyarmor_webui.egg-info/SOURCES.txt
 Comment: 
 
-Filename: pyarmor-webui-2.0/pyarmor_webui.egg-info/entry_points.txt
+Filename: pyarmor-webui-2.1/pyarmor_webui.egg-info/entry_points.txt
 Comment: 
 
-Filename: pyarmor-webui-2.0/pyarmor_webui.egg-info/requires.txt
+Filename: pyarmor-webui-2.1/pyarmor_webui.egg-info/requires.txt
 Comment: 
 
-Filename: pyarmor-webui-2.0/pyarmor_webui.egg-info/top_level.txt
+Filename: pyarmor-webui-2.1/pyarmor_webui.egg-info/top_level.txt
 Comment: 
 
-Filename: pyarmor-webui-2.0/pyarmor_webui.egg-info/dependency_links.txt
+Filename: pyarmor-webui-2.1/pyarmor_webui.egg-info/dependency_links.txt
 Comment: 
 
-Filename: pyarmor-webui-2.0/test/pack_one_folder_bundle.robot
+Filename: pyarmor-webui-2.1/test/pack_one_folder_bundle.robot
 Comment: 
 
-Filename: pyarmor-webui-2.0/test/generate_expired_license.robot
+Filename: pyarmor-webui-2.1/test/generate_expired_license.robot
 Comment: 
 
-Filename: pyarmor-webui-2.0/test/pack_one_file_bundle_with_outer_license.robot
+Filename: pyarmor-webui-2.1/test/pack_one_file_bundle_with_outer_license.robot
 Comment: 
 
-Filename: pyarmor-webui-2.0/test/obfuscate_multiple_entries.robot
+Filename: pyarmor-webui-2.1/test/obfuscate_multiple_entries.robot
 Comment: 
 
-Filename: pyarmor-webui-2.0/test/generate_machine_license.robot
+Filename: pyarmor-webui-2.1/test/generate_machine_license.robot
 Comment: 
 
-Filename: pyarmor-webui-2.0/test/obfuscate_one_script.robot
+Filename: pyarmor-webui-2.1/test/obfuscate_one_script.robot
 Comment: 
 
-Filename: pyarmor-webui-2.0/test/README.md
+Filename: pyarmor-webui-2.1/test/README.md
 Comment: 
 
-Filename: pyarmor-webui-2.0/test/generate_extra_data_license.robot
+Filename: pyarmor-webui-2.1/test/generate_extra_data_license.robot
 Comment: 
 
-Filename: pyarmor-webui-2.0/test/obfuscate_one_package.robot
+Filename: pyarmor-webui-2.1/test/obfuscate_one_package.robot
 Comment: 
 
-Filename: pyarmor-webui-2.0/test/resource.robot
+Filename: pyarmor-webui-2.1/test/resource.robot
 Comment: 
 
-Filename: pyarmor-webui-2.0/test/pack_with_data_file.robot
+Filename: pyarmor-webui-2.1/test/pack_with_data_file.robot
 Comment: 
 
-Filename: pyarmor-webui-2.0/test/pack_one_file_bundle.robot
+Filename: pyarmor-webui-2.1/test/pack_one_file_bundle.robot
 Comment: 
 
-Filename: pyarmor-webui-2.0/static/css/
+Filename: pyarmor-webui-2.1/static/css/
 Comment: 
 
-Filename: pyarmor-webui-2.0/static/js/
+Filename: pyarmor-webui-2.1/static/js/
 Comment: 
 
-Filename: pyarmor-webui-2.0/static/img/
+Filename: pyarmor-webui-2.1/static/img/
 Comment: 
 
-Filename: pyarmor-webui-2.0/static/fonts/
+Filename: pyarmor-webui-2.1/static/fonts/
 Comment: 
 
-Filename: pyarmor-webui-2.0/static/favicon.ico
+Filename: pyarmor-webui-2.1/static/favicon.ico
 Comment: 
 
-Filename: pyarmor-webui-2.0/static/index.html
+Filename: pyarmor-webui-2.1/static/index.html
 Comment: 
 
-Filename: pyarmor-webui-2.0/static/reqwest.js
+Filename: pyarmor-webui-2.1/static/reqwest.js
 Comment: 
 
-Filename: pyarmor-webui-2.0/static/css/app.9402d9fa.css
+Filename: pyarmor-webui-2.1/static/css/chunk-vendors.b79ff3a2.css
 Comment: 
 
-Filename: pyarmor-webui-2.0/static/css/chunk-vendors.b79ff3a2.css
+Filename: pyarmor-webui-2.1/static/css/app.b33816dc.css
 Comment: 
 
-Filename: pyarmor-webui-2.0/static/js/chunk-vendors.62e477e4.js
+Filename: pyarmor-webui-2.1/static/js/app.d802fb34.js
 Comment: 
 
-Filename: pyarmor-webui-2.0/static/js/app.8da2b1ed.js
+Filename: pyarmor-webui-2.1/static/js/chunk-vendors.4afc1da0.js
 Comment: 
 
-Filename: pyarmor-webui-2.0/static/img/cog.svg
+Filename: pyarmor-webui-2.1/static/img/cog.svg
 Comment: 
 
-Filename: pyarmor-webui-2.0/static/img/folder-solid.svg
+Filename: pyarmor-webui-2.1/static/img/folder-solid.svg
 Comment: 
 
-Filename: pyarmor-webui-2.0/static/img/tablet-alt.svg
+Filename: pyarmor-webui-2.1/static/img/tablet-alt.svg
 Comment: 
 
-Filename: pyarmor-webui-2.0/static/img/shield-alt.svg
+Filename: pyarmor-webui-2.1/static/img/shield-alt.svg
 Comment: 
 
-Filename: pyarmor-webui-2.0/static/img/calendar-alt.svg
+Filename: pyarmor-webui-2.1/static/img/calendar-alt.svg
 Comment: 
 
-Filename: pyarmor-webui-2.0/static/img/logo.a8954ff0.png
+Filename: pyarmor-webui-2.1/static/img/logo.a8954ff0.png
 Comment: 
 
-Filename: pyarmor-webui-2.0/static/img/registered.svg
+Filename: pyarmor-webui-2.1/static/img/registered.svg
 Comment: 
 
-Filename: pyarmor-webui-2.0/static/img/calendar-minus.svg
+Filename: pyarmor-webui-2.1/static/img/calendar-minus.svg
 Comment: 
 
-Filename: pyarmor-webui-2.0/static/img/calendar.svg
+Filename: pyarmor-webui-2.1/static/img/calendar.svg
 Comment: 
 
-Filename: pyarmor-webui-2.0/static/img/folder.svg
+Filename: pyarmor-webui-2.1/static/img/folder.svg
 Comment: 
 
-Filename: pyarmor-webui-2.0/static/fonts/element-icons.535877f5.woff
+Filename: pyarmor-webui-2.1/static/fonts/element-icons.535877f5.woff
 Comment: 
 
-Filename: pyarmor-webui-2.0/static/fonts/element-icons.732389de.ttf
+Filename: pyarmor-webui-2.1/static/fonts/element-icons.732389de.ttf
 Comment: 
 
-Filename: pyarmor-webui-2.0/data/copy_license.py
+Filename: pyarmor-webui-2.1/data/copy_license.py
 Comment: 
 
 Zip file comment:
```

## Comparing `pyarmor-webui-2.0/PKG-INFO` & `pyarmor-webui-2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pyarmor-webui
-Version: 2.0
+Version: 2.1
 Summary: A webui tool used to obfuscate and pack python scripts based on pyarmor
 Home-page: https://github.com/dashingsoft/pyarmor-webui
 Author: Jondy Zhao
 Author-email: pyarmor@163.com
 License: MIT License
 Description: pyarmor-webui
         =============
@@ -49,14 +49,24 @@
         - `snapshots <https://github.com/dashingsoft/pyarmor-webui/tree/master/snapshots>`_
         - `pyarmor <https://github.com/dashingsoft/pyarmor>`_
         - `pyarmor-vue <https://github.com/dashingsoft/pyarmor-vue>`_
         
         Change Logs
         -----------
         
+        2.1
+        ~~~~~
+        New feature:
+        * Add language Japanese
+        
+        Fix Pyarmor 8 issues:
+        * Fix registration need confirm in the console
+        * Fix license file doesn't work issue
+        * Fix obfuscating package issues
+        
         2.0
         ~~~~~
         * Support Pyarmor 8.0+
         * Add option `-7` to use Pyarmor 7 commands
         
         1.4.1
         ~~~~~
```

## Comparing `pyarmor-webui-2.0/server.py` & `pyarmor-webui-2.1/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,33 +24,33 @@
     from .handler import RootHandler
     from .handler8 import RootHandler as RootHandler8
 except Exception:
     from .handler import RootHandler
     from .handler8 import RootHandler as RootHandler8
 
 
-__version__ = '2.0'
+__version__ = '2.1'
 
 __config__ = {
     'version': __version__,
     'wwwroot': os.path.join(os.path.dirname(__file__), 'static'),
     'basepath': os.path.dirname(__file__),
     'homepath': os.path.expanduser(os.path.join('~', '.pyarmor')),
 }
 
 
 def _fix_up_win_console_freeze():
-    import win32api
-    import ctypes
     try:
-        win32api.SetConsoleTitle("Pyarmor Webui")
+        from ctypes import windll
+        from win32api import GetStdHandle, SetConsoleTitle
+        SetConsoleTitle("Pyarmor Webui")
         # Disable quick edit in CMD, as it can freeze the application
-        handle = win32api.GetStdHandle(-10)
+        handle = GetStdHandle(-10)
         if handle != -1 and handle is not None:
-            ctypes.windll.kernel32.SetConsoleMode(handle, 128)
+            windll.kernel32.SetConsoleMode(handle, 128)
     except Exception:
         pass
 
 
 class HelperHandler(BaseHTTPRequestHandler):
 
     server_version = "HelperHTTP/" + __version__
```

## Comparing `pyarmor-webui-2.0/handler.py` & `pyarmor-webui-2.1/handler.py`

 * *Files identical despite different names*

## Comparing `pyarmor-webui-2.0/LICENSE` & `pyarmor-webui-2.1/LICENSE`

 * *Files identical despite different names*

## Comparing `pyarmor-webui-2.0/handler8.py` & `pyarmor-webui-2.1/handler8.py`

 * *Files 3% similar despite different names*

```diff
@@ -91,15 +91,15 @@
             i = args['filedata'].find('base64,') + len('base64,')
             f.write(urlsafe_b64decode(args['filedata'][i:]))
 
         cmd_args = ['reg']
         is_initial = filename.endswith('.txt')
         if is_initial:
             self._check_arg('product', args)
-            cmd_args.extend(['-p', args.get('product')])
+            cmd_args.extend(['-y', '-p', args.get('product')])
             if filename[-8:-4].isdigit() and filename[-9] == '-':
                 if int(filename[-8:-4]) < 4000:
                     cmd_args.append('-u')
         cmd_args.append(filename)
         call_pyarmor(cmd_args, homepath=self._config['homepath'])
 
         if is_initial:
@@ -268,15 +268,22 @@
             call_pyinstaller(pyi_options)
 
         else:
             if args.get('noRuntime'):
                 cmd_args.append('--no-runtime')
 
             if name:
-                output = os.path.join(output, name)
+                cmd_args.append('-i')
+
+            if args.get('platforms'):
+                pnames = args.get('platforms')
+                if any([x.startswith('themida.') for x in pnames]):
+                    cmd_args.append('--enable-themida')
+                    pnames = [x.replace('themida', 'windows') for x in pnames]
+                cmd_args.extend(['--platform', ','.join(pnames)])
 
             cmd_args.extend(['--output', output])
 
         restrict_mode = args.get('restrictMode', DEFAULT_RESTRICT_FLAG)
         if restrict_mode & NO_RESTRICT_FLAG:
             call_pyarmor(['cfg', 'restrict_module', '0'], homepath=homepath)
         if restrict_mode & RESTRICT_PACKAGE_FLAG:
@@ -292,29 +299,41 @@
         if args.get('bccMode'):
             cmd_args.append('--enable-bcc')
         if args.get('rftMode'):
             cmd_args.append('--enable-rft')
         if args.get('mixStrings'):
             cmd_args.append('--mix-str')
 
-        if target == 3 or args.get('licenseFile') in ('false', 'outer'):
+        licfile = args.get('licenseFile')
+        if target == 3 or licfile in ('false', 'outer'):
+            cmd_args.append('--outer')
+        elif licfile not in ('true', None, ''):
+            if licfile.endswith('license.lic'):
+                raise RuntimeError('This license file "%s" is not '
+                                   'for Pyarmor 8' % licfile)
+            if not os.path.exists(licfile):
+                raise RuntimeError('no found license file "%s"' % licfile)
             cmd_args.append('--outer')
 
         if args.get('plugins'):
             plugins = ' '.join(args.get('plugins'))
             call_pyarmor(['cfg', 'plugins', '+', plugins], homepath=homepath)
 
         include = args.get('include', 'exact')
         excludes = args.get('exclude', [])
 
         for x in excludes:
             cmd_args.extend(['--exclude', os.path.join('*', x)])
 
         if include == 'exact':
             cmd_args.extend([os.path.join(src, x) for x in entries])
+        elif name and not target:
+            if include == 'all':
+                cmd_args.append('-r')
+            cmd_args.append(src)
         else:
             inputs = [(x.is_file(), x.path) for x in os.scandir(src)
                       if x not in excludes and not x.name.startswith('.')]
             if include == 'all':
                 cmd_args.append('-r')
                 cmd_args.extend([b for a, b in inputs if not a])
             cmd_args.extend([b for a, b in inputs if a and b.endswith('.py')])
@@ -324,14 +343,32 @@
             if os.path.exists(output):
                 if len(output) < 4:
                     # Do not rmtree too short path
                     raise RuntimeError('Output path "%s" is not empty', output)
                 logging.info('Clean output path "%s"', output)
                 shutil.rmtree(output)
             shutil.move(distpath, output)
+
+        if isinstance(licfile, str) and os.path.exists(licfile):
+            licpath = os.path.join(output, entryname if target == 1 else '')
+            if target not in (2, 3):
+                def is_runtime_package(p):
+                    names = os.listdir(p)
+                    return '__init__.py' in names and any([
+                        x.startswith('pyarmor_runtime.') for x in names])
+
+                for x in os.scandir(licpath):
+                    if x.is_dir() and x.name.startswith('pyarmor_runtime_') \
+                       and is_runtime_package(x.path):
+                        licpath = x.path
+                        break
+                else:
+                    raise RuntimeError('no found runtime package')
+            shutil.copy2(licfile, licpath)
+
         return output
 
     def _build_temp(self, args, debug=False):
         self._build_data(args)
 
         name = 'project-%s' % self.temp_id
         path = os.path.join(self._get_path(), name)
```

## Comparing `pyarmor-webui-2.0/setup.py` & `pyarmor-webui-2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from sys import platform
 from setuptools import setup
 
-__version__ = '2.0'
+__version__ = '2.1'
 
 with open('README.rst') as f:
     long_description = f.read()
 
 setup(
     name='pyarmor-webui',
     version=__version__,
@@ -59,10 +59,10 @@
 
     entry_points={
         'console_scripts': [
             'pyarmor-webui=pyarmor.webui.server:main',
         ],
     },
 
-    install_requires=['pyarmor~=8.2.1'] + (
+    install_requires=['pyarmor~=8.2.2'] + (
         ['pywin32'] if platform == 'win32' else []),
 )
```

## Comparing `pyarmor-webui-2.0/README.rst` & `pyarmor-webui-2.1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -41,14 +41,24 @@
 - `snapshots <https://github.com/dashingsoft/pyarmor-webui/tree/master/snapshots>`_
 - `pyarmor <https://github.com/dashingsoft/pyarmor>`_
 - `pyarmor-vue <https://github.com/dashingsoft/pyarmor-vue>`_
 
 Change Logs
 -----------
 
+2.1
+~~~~~
+New feature:
+* Add language Japanese
+
+Fix Pyarmor 8 issues:
+* Fix registration need confirm in the console
+* Fix license file doesn't work issue
+* Fix obfuscating package issues
+
 2.0
 ~~~~~
 * Support Pyarmor 8.0+
 * Add option `-7` to use Pyarmor 7 commands
 
 1.4.1
 ~~~~~
```

## Comparing `pyarmor-webui-2.0/pyarmor_webui.egg-info/PKG-INFO` & `pyarmor-webui-2.1/pyarmor_webui.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pyarmor-webui
-Version: 2.0
+Version: 2.1
 Summary: A webui tool used to obfuscate and pack python scripts based on pyarmor
 Home-page: https://github.com/dashingsoft/pyarmor-webui
 Author: Jondy Zhao
 Author-email: pyarmor@163.com
 License: MIT License
 Description: pyarmor-webui
         =============
@@ -49,14 +49,24 @@
         - `snapshots <https://github.com/dashingsoft/pyarmor-webui/tree/master/snapshots>`_
         - `pyarmor <https://github.com/dashingsoft/pyarmor>`_
         - `pyarmor-vue <https://github.com/dashingsoft/pyarmor-vue>`_
         
         Change Logs
         -----------
         
+        2.1
+        ~~~~~
+        New feature:
+        * Add language Japanese
+        
+        Fix Pyarmor 8 issues:
+        * Fix registration need confirm in the console
+        * Fix license file doesn't work issue
+        * Fix obfuscating package issues
+        
         2.0
         ~~~~~
         * Support Pyarmor 8.0+
         * Add option `-7` to use Pyarmor 7 commands
         
         1.4.1
         ~~~~~
```

## Comparing `pyarmor-webui-2.0/pyarmor_webui.egg-info/SOURCES.txt` & `pyarmor-webui-2.1/pyarmor_webui.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -6,30 +6,30 @@
 ./handler.py
 ./handler8.py
 ./server.py
 ./data/copy_license.py
 ./static/favicon.ico
 ./static/index.html
 ./static/reqwest.js
-./static/css/app.9402d9fa.css
+./static/css/app.b33816dc.css
 ./static/css/chunk-vendors.b79ff3a2.css
 ./static/fonts/element-icons.535877f5.woff
 ./static/fonts/element-icons.732389de.ttf
 ./static/img/calendar-alt.svg
 ./static/img/calendar-minus.svg
 ./static/img/calendar.svg
 ./static/img/cog.svg
 ./static/img/folder-solid.svg
 ./static/img/folder.svg
 ./static/img/logo.a8954ff0.png
 ./static/img/registered.svg
 ./static/img/shield-alt.svg
 ./static/img/tablet-alt.svg
-./static/js/app.8da2b1ed.js
-./static/js/chunk-vendors.62e477e4.js
+./static/js/app.d802fb34.js
+./static/js/chunk-vendors.4afc1da0.js
 ./test/README.md
 ./test/generate_expired_license.robot
 ./test/generate_extra_data_license.robot
 ./test/generate_machine_license.robot
 ./test/obfuscate_multiple_entries.robot
 ./test/obfuscate_one_package.robot
 ./test/obfuscate_one_script.robot
```

## Comparing `pyarmor-webui-2.0/test/pack_one_folder_bundle.robot` & `pyarmor-webui-2.1/test/pack_one_folder_bundle.robot`

 * *Files identical despite different names*

## Comparing `pyarmor-webui-2.0/test/generate_expired_license.robot` & `pyarmor-webui-2.1/test/generate_expired_license.robot`

 * *Files identical despite different names*

## Comparing `pyarmor-webui-2.0/test/pack_one_file_bundle_with_outer_license.robot` & `pyarmor-webui-2.1/test/pack_one_file_bundle_with_outer_license.robot`

 * *Files identical despite different names*

## Comparing `pyarmor-webui-2.0/test/obfuscate_multiple_entries.robot` & `pyarmor-webui-2.1/test/obfuscate_multiple_entries.robot`

 * *Files identical despite different names*

## Comparing `pyarmor-webui-2.0/test/generate_machine_license.robot` & `pyarmor-webui-2.1/test/generate_machine_license.robot`

 * *Files identical despite different names*

## Comparing `pyarmor-webui-2.0/test/obfuscate_one_script.robot` & `pyarmor-webui-2.1/test/obfuscate_one_script.robot`

 * *Files identical despite different names*

## Comparing `pyarmor-webui-2.0/test/README.md` & `pyarmor-webui-2.1/test/README.md`

 * *Files identical despite different names*

## Comparing `pyarmor-webui-2.0/test/generate_extra_data_license.robot` & `pyarmor-webui-2.1/test/generate_extra_data_license.robot`

 * *Files identical despite different names*

## Comparing `pyarmor-webui-2.0/test/obfuscate_one_package.robot` & `pyarmor-webui-2.1/test/obfuscate_one_package.robot`

 * *Files identical despite different names*

## Comparing `pyarmor-webui-2.0/test/resource.robot` & `pyarmor-webui-2.1/test/resource.robot`

 * *Files identical despite different names*

## Comparing `pyarmor-webui-2.0/test/pack_with_data_file.robot` & `pyarmor-webui-2.1/test/pack_with_data_file.robot`

 * *Files identical despite different names*

## Comparing `pyarmor-webui-2.0/test/pack_one_file_bundle.robot` & `pyarmor-webui-2.1/test/pack_one_file_bundle.robot`

 * *Files identical despite different names*

## Comparing `pyarmor-webui-2.0/static/favicon.ico` & `pyarmor-webui-2.1/static/favicon.ico`

 * *Files identical despite different names*

## Comparing `pyarmor-webui-2.0/static/index.html` & `pyarmor-webui-2.1/static/index.html`

 * *Files 25% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html lang="en"><head><meta charset="utf-8"><meta http-equiv="X-UA-Compatible" content="IE=edge"><meta name="viewport" content="width=device-width,initial-scale=1"><link rel="icon" href="/favicon.ico"><title>Pyarmor</title><link href="/css/app.9402d9fa.css" rel="preload" as="style"><link href="/css/chunk-vendors.b79ff3a2.css" rel="preload" as="style"><link href="/js/app.8da2b1ed.js" rel="preload" as="script"><link href="/js/chunk-vendors.62e477e4.js" rel="preload" as="script"><link href="/css/chunk-vendors.b79ff3a2.css" rel="stylesheet"><link href="/css/app.9402d9fa.css" rel="stylesheet"></head><body><noscript><strong>We're sorry but pyarmor-vue doesn't work properly without JavaScript enabled. Please enable it to continue.</strong></noscript><div id="app"></div><script src="/js/chunk-vendors.62e477e4.js"></script><script src="/js/app.8da2b1ed.js"></script></body></html>
+<!DOCTYPE html><html lang="en"><head><meta charset="utf-8"><meta http-equiv="X-UA-Compatible" content="IE=edge"><meta name="viewport" content="width=device-width,initial-scale=1"><link rel="icon" href="/favicon.ico"><title>Pyarmor</title><link href="/css/app.b33816dc.css" rel="preload" as="style"><link href="/css/chunk-vendors.b79ff3a2.css" rel="preload" as="style"><link href="/js/app.d802fb34.js" rel="preload" as="script"><link href="/js/chunk-vendors.4afc1da0.js" rel="preload" as="script"><link href="/css/chunk-vendors.b79ff3a2.css" rel="stylesheet"><link href="/css/app.b33816dc.css" rel="stylesheet"></head><body><noscript><strong>We're sorry but pyarmor-vue doesn't work properly without JavaScript enabled. Please enable it to continue.</strong></noscript><div id="app"></div><script src="/js/chunk-vendors.4afc1da0.js"></script><script src="/js/app.d802fb34.js"></script></body></html>
```

## Comparing `pyarmor-webui-2.0/static/reqwest.js` & `pyarmor-webui-2.1/static/reqwest.js`

 * *Files identical despite different names*

## Comparing `pyarmor-webui-2.0/static/css/chunk-vendors.b79ff3a2.css` & `pyarmor-webui-2.1/static/css/chunk-vendors.b79ff3a2.css`

 * *Files identical despite different names*

## Comparing `pyarmor-webui-2.0/static/js/chunk-vendors.62e477e4.js` & `pyarmor-webui-2.1/static/js/chunk-vendors.4afc1da0.js`

 * *Files 0% similar despite different names*

### js-beautify {}

```diff
@@ -26954,14 +26954,139 @@
                                 e.component(r.name, r)
                             }
                         };
                     t["default"] = r
                 }
             })
         },
+        c3ff: function(e, t, n) {
+            "use strict";
+            t.__esModule = !0, t.default = {
+                el: {
+                    colorpicker: {
+                        confirm: "OK",
+                        clear: "クリア"
+                    },
+                    datepicker: {
+                        now: "現在",
+                        today: "今日",
+                        cancel: "キャンセル",
+                        clear: "クリア",
+                        confirm: "OK",
+                        selectDate: "日付を選択",
+                        selectTime: "時間を選択",
+                        startDate: "開始日",
+                        startTime: "開始時間",
+                        endDate: "終了日",
+                        endTime: "終了時間",
+                        prevYear: "前年",
+                        nextYear: "翌年",
+                        prevMonth: "前月",
+                        nextMonth: "翌月",
+                        year: "年",
+                        month1: "1月",
+                        month2: "2月",
+                        month3: "3月",
+                        month4: "4月",
+                        month5: "5月",
+                        month6: "6月",
+                        month7: "7月",
+                        month8: "8月",
+                        month9: "9月",
+                        month10: "10月",
+                        month11: "11月",
+                        month12: "12月",
+                        weeks: {
+                            sun: "日",
+                            mon: "月",
+                            tue: "火",
+                            wed: "水",
+                            thu: "木",
+                            fri: "金",
+                            sat: "土"
+                        },
+                        months: {
+                            jan: "1月",
+                            feb: "2月",
+                            mar: "3月",
+                            apr: "4月",
+                            may: "5月",
+                            jun: "6月",
+                            jul: "7月",
+                            aug: "8月",
+                            sep: "9月",
+                            oct: "10月",
+                            nov: "11月",
+                            dec: "12月"
+                        }
+                    },
+                    select: {
+                        loading: "ロード中",
+                        noMatch: "データなし",
+                        noData: "データなし",
+                        placeholder: "選択してください"
+                    },
+                    cascader: {
+                        noMatch: "データなし",
+                        loading: "ロード中",
+                        placeholder: "選択してください",
+                        noData: "データなし"
+                    },
+                    pagination: {
+                        goto: "",
+                        pagesize: "件/ページ",
+                        total: "総計 {total} 件",
+                        pageClassifier: "ページ目へ"
+                    },
+                    messagebox: {
+                        title: "メッセージ",
+                        confirm: "OK",
+                        cancel: "キャンセル",
+                        error: "正しくない入力"
+                    },
+                    upload: {
+                        deleteTip: "Delキーを押して削除する",
+                        delete: "削除する",
+                        preview: "プレビュー",
+                        continue: "続行する"
+                    },
+                    table: {
+                        emptyText: "データなし",
+                        confirmFilter: "確認",
+                        resetFilter: "初期化",
+                        clearFilter: "すべて",
+                        sumText: "合計"
+                    },
+                    tree: {
+                        emptyText: "データなし"
+                    },
+                    transfer: {
+                        noMatch: "データなし",
+                        noData: "データなし",
+                        titles: ["リスト 1", "リスト 2"],
+                        filterPlaceholder: "キーワードを入力",
+                        noCheckedFormat: "総計 {total} 件",
+                        hasCheckedFormat: "{checked}/{total} を選択した"
+                    },
+                    image: {
+                        error: "FAILED"
+                    },
+                    pageHeader: {
+                        title: "Back"
+                    },
+                    popconfirm: {
+                        confirmButtonText: "Yes",
+                        cancelButtonText: "No"
+                    },
+                    empty: {
+                        description: "データなし"
+                    }
+                }
+            }
+        },
         c430: function(e, t) {
             e.exports = !1
         },
         c513: function(e, t, n) {
             var i = n("23e7"),
                 r = n("1a2d"),
                 o = n("d9b5"),
@@ -34243,8 +34368,8 @@
         },
         fe07: function(e, t, n) {},
         fed5: function(e, t) {
             t.f = Object.getOwnPropertySymbols
         }
     }
 ]);
-//# sourceMappingURL=chunk-vendors.62e477e4.js.map
+//# sourceMappingURL=chunk-vendors.4afc1da0.js.map
```

## Comparing `pyarmor-webui-2.0/static/js/app.8da2b1ed.js` & `pyarmor-webui-2.1/static/js/app.d802fb34.js`

 * *Files 19% similar despite different names*

### js-beautify {}

```diff
@@ -1,64 +1,64 @@
 (function(e) {
     function t(t) {
-        for (var o, s, i = t[0], l = t[1], c = t[2], p = 0, d = []; p < i.length; p++) s = i[p], Object.prototype.hasOwnProperty.call(r, s) && r[s] && d.push(r[s][0]), r[s] = 0;
-        for (o in l) Object.prototype.hasOwnProperty.call(l, o) && (e[o] = l[o]);
+        for (var a, s, i = t[0], l = t[1], c = t[2], p = 0, d = []; p < i.length; p++) s = i[p], Object.prototype.hasOwnProperty.call(r, s) && r[s] && d.push(r[s][0]), r[s] = 0;
+        for (a in l) Object.prototype.hasOwnProperty.call(l, a) && (e[a] = l[a]);
         u && u(t);
         while (d.length) d.shift()();
-        return n.push.apply(n, c || []), a()
+        return n.push.apply(n, c || []), o()
     }
 
-    function a() {
+    function o() {
         for (var e, t = 0; t < n.length; t++) {
-            for (var a = n[t], o = !0, i = 1; i < a.length; i++) {
-                var l = a[i];
-                0 !== r[l] && (o = !1)
+            for (var o = n[t], a = !0, i = 1; i < o.length; i++) {
+                var l = o[i];
+                0 !== r[l] && (a = !1)
             }
-            o && (n.splice(t--, 1), e = s(s.s = a[0]))
+            a && (n.splice(t--, 1), e = s(s.s = o[0]))
         }
         return e
     }
-    var o = {},
+    var a = {},
         r = {
             app: 0
         },
         n = [];
 
     function s(t) {
-        if (o[t]) return o[t].exports;
-        var a = o[t] = {
+        if (a[t]) return a[t].exports;
+        var o = a[t] = {
             i: t,
             l: !1,
             exports: {}
         };
-        return e[t].call(a.exports, a, a.exports, s), a.l = !0, a.exports
+        return e[t].call(o.exports, o, o.exports, s), o.l = !0, o.exports
     }
-    s.m = e, s.c = o, s.d = function(e, t, a) {
+    s.m = e, s.c = a, s.d = function(e, t, o) {
         s.o(e, t) || Object.defineProperty(e, t, {
             enumerable: !0,
-            get: a
+            get: o
         })
     }, s.r = function(e) {
         "undefined" !== typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
     }, s.t = function(e, t) {
         if (1 & t && (e = s(e)), 8 & t) return e;
         if (4 & t && "object" === typeof e && e && e.__esModule) return e;
-        var a = Object.create(null);
-        if (s.r(a), Object.defineProperty(a, "default", {
+        var o = Object.create(null);
+        if (s.r(o), Object.defineProperty(o, "default", {
                 enumerable: !0,
                 value: e
             }), 2 & t && "string" != typeof e)
-            for (var o in e) s.d(a, o, function(t) {
+            for (var a in e) s.d(o, a, function(t) {
                 return e[t]
-            }.bind(null, o));
-        return a
+            }.bind(null, a));
+        return o
     }, s.n = function(e) {
         var t = e && e.__esModule ? function() {
             return e["default"]
         } : function() {
             return e
         };
         return s.d(t, "a", t), t
@@ -66,38 +66,39 @@
         return Object.prototype.hasOwnProperty.call(e, t)
     }, s.p = "/";
     var i = window["webpackJsonp"] = window["webpackJsonp"] || [],
         l = i.push.bind(i);
     i.push = t, i = i.slice();
     for (var c = 0; c < i.length; c++) t(i[c]);
     var u = l;
-    n.push([0, "chunk-vendors"]), a()
+    n.push([0, "chunk-vendors"]), o()
 })({
-    0: function(e, t, a) {
-        e.exports = a("56d7")
+    0: function(e, t, o) {
+        e.exports = o("56d7")
     },
-    "073e": function(e, t, a) {},
-    "0b5d": function(e, t, a) {
+    "0b5d": function(e, t, o) {
         "use strict";
-        a("e2d0")
+        o("e2d0")
     },
-    "0c06": function(e, t, a) {},
-    "1d77": function(e, t, a) {
+    "0c06": function(e, t, o) {},
+    "0de2": function(e, t, o) {},
+    "103e": function(e, t, o) {},
+    "1d77": function(e, t, o) {
         "use strict";
-        a("58be")
+        o("58be")
     },
-    2733: function(e, t, a) {
+    2733: function(e, t, o) {
         "use strict";
-        a("a7a7")
+        o("a7a7")
     },
     "2e26": function(module, exports, __webpack_require__) {
         var _typeof = __webpack_require__("7037").default;
         __webpack_require__("d9e2"), __webpack_require__("ac1f"), __webpack_require__("00b4"), __webpack_require__("4d63"), __webpack_require__("c607"), __webpack_require__("2c3e"), __webpack_require__("25f0"), __webpack_require__("466d"), __webpack_require__("5319"), __webpack_require__("14d9"), __webpack_require__("b0c0"), __webpack_require__("fb6a"), __webpack_require__("a15b"), __webpack_require__("d3b7"),
-            function(e, t, a) {
-                module.exports ? module.exports = a() : t[e] = a()
+            function(e, t, o) {
+                module.exports ? module.exports = o() : t[e] = o()
             }("reqwest", this, (function() {
                 var context = this,
                     XHR2;
                 if ("window" in context) var doc = document,
                     byTag = "getElementsByTagName",
                     head = doc[byTag]("head")[0];
                 else try {
@@ -147,67 +148,67 @@
                     };
 
                 function succeed(e) {
                     var t = protocolRe.exec(e.url);
                     return t = t && t[1] || context.location.protocol, httpsRe.test(t) ? twoHundo.test(e.request.status) : !!e.request.response
                 }
 
-                function handleReadyState(e, t, a) {
+                function handleReadyState(e, t, o) {
                     return function() {
-                        return e._aborted ? a(e.request) : e._timedOut ? a(e.request, "Request is aborted: timeout") : void(e.request && 4 == e.request[readyState] && (e.request.onreadystatechange = noop, succeed(e) ? t(e.request) : a(e.request)))
+                        return e._aborted ? o(e.request) : e._timedOut ? o(e.request, "Request is aborted: timeout") : void(e.request && 4 == e.request[readyState] && (e.request.onreadystatechange = noop, succeed(e) ? t(e.request) : o(e.request)))
                     }
                 }
 
                 function setHeaders(e, t) {
-                    var a, o = t["headers"] || {};
-                    o["Accept"] = o["Accept"] || defaultHeaders["accept"][t["type"]] || defaultHeaders["accept"]["*"];
+                    var o, a = t["headers"] || {};
+                    a["Accept"] = a["Accept"] || defaultHeaders["accept"][t["type"]] || defaultHeaders["accept"]["*"];
                     var r = "undefined" !== typeof FormData && t["data"] instanceof FormData;
-                    for (a in t["crossOrigin"] || o[requestedWith] || (o[requestedWith] = defaultHeaders["requestedWith"]), o[contentType] || r || (o[contentType] = t["contentType"] || defaultHeaders["contentType"]), o) o.hasOwnProperty(a) && "setRequestHeader" in e && e.setRequestHeader(a, o[a])
+                    for (o in t["crossOrigin"] || a[requestedWith] || (a[requestedWith] = defaultHeaders["requestedWith"]), a[contentType] || r || (a[contentType] = t["contentType"] || defaultHeaders["contentType"]), a) a.hasOwnProperty(o) && "setRequestHeader" in e && e.setRequestHeader(o, a[o])
                 }
 
                 function setCredentials(e, t) {
                     "undefined" !== typeof t["withCredentials"] && "undefined" !== typeof e.withCredentials && (e.withCredentials = !!t["withCredentials"])
                 }
 
                 function generalCallback(e) {
                     lastValue = e
                 }
 
                 function urlappend(e, t) {
                     return e + (/\?/.test(e) ? "&" : "?") + t
                 }
 
-                function handleJsonp(e, t, a, o) {
+                function handleJsonp(e, t, o, a) {
                     var r = uniqid++,
                         n = e["jsonpCallback"] || "callback",
                         s = e["jsonpCallbackName"] || reqwest.getcallbackPrefix(r),
                         i = new RegExp("((^|\\?|&)" + n + ")=([^&]+)"),
-                        l = o.match(i),
+                        l = a.match(i),
                         c = doc.createElement("script"),
                         u = 0,
                         p = -1 !== navigator.userAgent.indexOf("MSIE 10.0");
-                    return l ? "?" === l[3] ? o = o.replace(i, "$1=" + s) : s = l[3] : o = urlappend(o, n + "=" + s), context[s] = generalCallback, c.type = "text/javascript", c.src = o, c.async = !0, "undefined" === typeof c.onreadystatechange || p || (c.htmlFor = c.id = "_reqwest_" + r), c.onload = c.onreadystatechange = function() {
+                    return l ? "?" === l[3] ? a = a.replace(i, "$1=" + s) : s = l[3] : a = urlappend(a, n + "=" + s), context[s] = generalCallback, c.type = "text/javascript", c.src = a, c.async = !0, "undefined" === typeof c.onreadystatechange || p || (c.htmlFor = c.id = "_reqwest_" + r), c.onload = c.onreadystatechange = function() {
                         if (c[readyState] && "complete" !== c[readyState] && "loaded" !== c[readyState] || u) return !1;
                         c.onload = c.onreadystatechange = null, c.onclick && c.onclick(), t(lastValue), lastValue = void 0, head.removeChild(c), u = 1
                     }, head.appendChild(c), {
                         abort: function() {
-                            c.onload = c.onreadystatechange = null, a({}, "Request is aborted: timeout", {}), lastValue = void 0, head.removeChild(c), u = 1
+                            c.onload = c.onreadystatechange = null, o({}, "Request is aborted: timeout", {}), lastValue = void 0, head.removeChild(c), u = 1
                         }
                     }
                 }
 
                 function getRequest(e, t) {
-                    var a, o = this.o,
-                        r = (o["method"] || "GET").toUpperCase(),
-                        n = "string" === typeof o ? o : o["url"],
-                        s = !1 !== o["processData"] && o["data"] && "string" !== typeof o["data"] ? reqwest.toQueryString(o["data"]) : o["data"] || null,
+                    var o, a = this.o,
+                        r = (a["method"] || "GET").toUpperCase(),
+                        n = "string" === typeof a ? a : a["url"],
+                        s = !1 !== a["processData"] && a["data"] && "string" !== typeof a["data"] ? reqwest.toQueryString(a["data"]) : a["data"] || null,
                         i = !1;
-                    return "jsonp" != o["type"] && "GET" != r || !s || (n = urlappend(n, s), s = null), "jsonp" == o["type"] ? handleJsonp(o, e, t, n) : (a = o.xhr && o.xhr(o) || xhr(o), a.open(r, n, !1 !== o["async"]), setHeaders(a, o), setCredentials(a, o), context[xDomainRequest] && a instanceof context[xDomainRequest] ? (a.onload = e, a.onerror = t, a.onprogress = function() {}, i = !0) : a.onreadystatechange = handleReadyState(this, e, t), o["before"] && o["before"](a), i ? setTimeout((function() {
-                        a.send(s)
-                    }), 200) : a.send(s), a)
+                    return "jsonp" != a["type"] && "GET" != r || !s || (n = urlappend(n, s), s = null), "jsonp" == a["type"] ? handleJsonp(a, e, t, n) : (o = a.xhr && a.xhr(a) || xhr(a), o.open(r, n, !1 !== a["async"]), setHeaders(o, a), setCredentials(o, a), context[xDomainRequest] && o instanceof context[xDomainRequest] ? (o.onload = e, o.onerror = t, o.onprogress = function() {}, i = !0) : o.onreadystatechange = handleReadyState(this, e, t), a["before"] && a["before"](o), i ? setTimeout((function() {
+                        o.send(s)
+                    }), 200) : o.send(s), o)
                 }
 
                 function Reqwest(e, t) {
                     this.o = e, this.fn = t, init.apply(this, arguments)
                 }
 
                 function setType(e) {
@@ -254,17 +255,17 @@
                         complete(resp)
                     }
 
                     function timedOut() {
                         self._timedOut = !0, self.request.abort()
                     }
 
-                    function error(e, t, a) {
-                        e = self.request, self._responseArgs.resp = e, self._responseArgs.msg = t, self._responseArgs.t = a, self._erred = !0;
-                        while (self._errorHandlers.length > 0) self._errorHandlers.shift()(e, t, a);
+                    function error(e, t, o) {
+                        e = self.request, self._responseArgs.resp = e, self._responseArgs.msg = t, self._responseArgs.t = o, self._erred = !0;
+                        while (self._errorHandlers.length > 0) self._errorHandlers.shift()(e, t, o);
                         complete(e)
                     }
                     fn = fn || function() {}, o["timeout"] && (this.timeout = setTimeout((function() {
                         timedOut()
                     }), o["timeout"])), o["success"] && (this._successHandler = function() {
                         o["success"].apply(o, arguments)
                     }), o["error"] && this._errorHandlers.push((function() {
@@ -279,62 +280,62 @@
                 }
 
                 function normalize(e) {
                     return e ? e.replace(/\r?\n/g, "\r\n") : ""
                 }
 
                 function serial(e, t) {
-                    var a, o, r, n, s = e.name,
+                    var o, a, r, n, s = e.name,
                         i = e.tagName.toLowerCase(),
                         l = function(e) {
                             e && !e["disabled"] && t(s, normalize(e["attributes"]["value"] && e["attributes"]["value"]["specified"] ? e["value"] : e["text"]))
                         };
                     if (!e.disabled && s) switch (i) {
                         case "input":
-                            /reset|button|image|file/i.test(e.type) || (a = /checkbox/i.test(e.type), o = /radio/i.test(e.type), r = e.value, (!a && !o || e.checked) && t(s, normalize(a && "" === r ? "on" : r)));
+                            /reset|button|image|file/i.test(e.type) || (o = /checkbox/i.test(e.type), a = /radio/i.test(e.type), r = e.value, (!o && !a || e.checked) && t(s, normalize(o && "" === r ? "on" : r)));
                             break;
                         case "textarea":
                             t(s, normalize(e.value));
                             break;
                         case "select":
                             if ("select-one" === e.type.toLowerCase()) l(e.selectedIndex >= 0 ? e.options[e.selectedIndex] : null);
                             else
                                 for (n = 0; e.length && n < e.length; n++) e.options[n].selected && l(e.options[n]);
                             break
                     }
                 }
 
                 function eachFormElement() {
-                    var e, t, a = this,
-                        o = function(e, t) {
-                            var o, r, n;
-                            for (o = 0; o < t.length; o++)
-                                for (n = e[byTag](t[o]), r = 0; r < n.length; r++) serial(n[r], a)
+                    var e, t, o = this,
+                        a = function(e, t) {
+                            var a, r, n;
+                            for (a = 0; a < t.length; a++)
+                                for (n = e[byTag](t[a]), r = 0; r < n.length; r++) serial(n[r], o)
                         };
-                    for (t = 0; t < arguments.length; t++) e = arguments[t], /input|select|textarea/i.test(e.tagName) && serial(e, a), o(e, ["input", "select", "textarea"])
+                    for (t = 0; t < arguments.length; t++) e = arguments[t], /input|select|textarea/i.test(e.tagName) && serial(e, o), a(e, ["input", "select", "textarea"])
                 }
 
                 function serializeQueryString() {
                     return reqwest.toQueryString(reqwest.serializeArray.apply(null, arguments))
                 }
 
                 function serializeHash() {
                     var e = {};
-                    return eachFormElement.apply((function(t, a) {
-                        t in e ? (e[t] && !isArray(e[t]) && (e[t] = [e[t]]), e[t].push(a)) : e[t] = a
+                    return eachFormElement.apply((function(t, o) {
+                        t in e ? (e[t] && !isArray(e[t]) && (e[t] = [e[t]]), e[t].push(o)) : e[t] = o
                     }), arguments), e
                 }
 
-                function buildParams(e, t, a, o) {
+                function buildParams(e, t, o, a) {
                     var r, n, s, i = /\[\]$/;
                     if (isArray(t))
-                        for (n = 0; t && n < t.length; n++) s = t[n], a || i.test(e) ? o(e, s) : buildParams(e + "[" + ("object" === _typeof(s) ? n : "") + "]", s, a, o);
+                        for (n = 0; t && n < t.length; n++) s = t[n], o || i.test(e) ? a(e, s) : buildParams(e + "[" + ("object" === _typeof(s) ? n : "") + "]", s, o, a);
                     else if (t && "[object Object]" === t.toString())
-                        for (r in t) buildParams(e + "[" + r + "]", t[r], a, o);
-                    else o(e, t)
+                        for (r in t) buildParams(e + "[" + r + "]", t[r], o, a);
+                    else a(e, t)
                 }
                 return Reqwest.prototype = {
                     abort: function() {
                         this._aborted = !0, this.request.abort()
                     },
                     retry: function() {
                         init.call(this, this.o, this.fn)
@@ -349,58 +350,54 @@
                         return this._erred ? e(this._responseArgs.resp, this._responseArgs.msg, this._responseArgs.t) : this._errorHandlers.push(e), this
                     },
                     catch: function(e) {
                         return this.fail(e)
                     }
                 }, reqwest.serializeArray = function() {
                     var e = [];
-                    return eachFormElement.apply((function(t, a) {
+                    return eachFormElement.apply((function(t, o) {
                         e.push({
                             name: t,
-                            value: a
+                            value: o
                         })
                     }), arguments), e
                 }, reqwest.serialize = function() {
                     if (0 === arguments.length) return "";
-                    var e, t, a = Array.prototype.slice.call(arguments, 0);
-                    return e = a.pop(), e && e.nodeType && a.push(e) && (e = null), e && (e = e.type), t = "map" == e ? serializeHash : "array" == e ? reqwest.serializeArray : serializeQueryString, t.apply(null, a)
+                    var e, t, o = Array.prototype.slice.call(arguments, 0);
+                    return e = o.pop(), e && e.nodeType && o.push(e) && (e = null), e && (e = e.type), t = "map" == e ? serializeHash : "array" == e ? reqwest.serializeArray : serializeQueryString, t.apply(null, o)
                 }, reqwest.toQueryString = function(e, t) {
-                    var a, o, r = t || !1,
+                    var o, a, r = t || !1,
                         n = [],
                         s = encodeURIComponent,
                         i = function(e, t) {
                             t = "function" === typeof t ? t() : null == t ? "" : t, n[n.length] = s(e) + "=" + s(t)
                         };
                     if (isArray(e))
-                        for (o = 0; e && o < e.length; o++) i(e[o]["name"], e[o]["value"]);
+                        for (a = 0; e && a < e.length; a++) i(e[a]["name"], e[a]["value"]);
                     else
-                        for (a in e) e.hasOwnProperty(a) && buildParams(a, e[a], r, i);
+                        for (o in e) e.hasOwnProperty(o) && buildParams(o, e[o], r, i);
                     return n.join("&").replace(/%20/g, "+")
                 }, reqwest.getcallbackPrefix = function() {
                     return callbackPrefix
                 }, reqwest.compat = function(e, t) {
                     return e && (e["type"] && (e["method"] = e["type"]) && delete e["type"], e["dataType"] && (e["type"] = e["dataType"]), e["jsonpCallback"] && (e["jsonpCallbackName"] = e["jsonpCallback"]) && delete e["jsonpCallback"], e["jsonp"] && (e["jsonpCallback"] = e["jsonp"])), new Reqwest(e, t)
                 }, reqwest.ajaxSetup = function(e) {
                     for (var t in e = e || {}, e) globalSetupOptions[t] = e[t]
                 }, reqwest
             }))
     },
-    "3c61": function(e, t, a) {
+    "3c61": function(e, t, o) {
         "use strict";
-        a("7458")
+        o("7458")
     },
-    "50a8": function(e, t, a) {
+    "56d7": function(e, t, o) {
         "use strict";
-        a("c3c3")
-    },
-    "56d7": function(e, t, a) {
-        "use strict";
-        a.r(t);
-        a("e260"), a("e6cf"), a("cca6"), a("a79d");
-        var o = a("2b0e"),
+        o.r(t);
+        o("e260"), o("e6cf"), o("cca6"), o("a79d");
+        var a = o("2b0e"),
             r = function() {
                 var e = this,
                     t = e._self._c;
                 return t("div", {
                     attrs: {
                         id: "app"
                     }
@@ -410,15 +407,15 @@
                         rawName: "v-show",
                         value: !e.currentPageName,
                         expression: "!currentPageName"
                     }]
                 }, [t("el-aside", [t("el-container", [t("img", {
                     staticClass: "brand-logo",
                     attrs: {
-                        src: a("cf05")
+                        src: o("cf05")
                     }
                 }), t("el-button", {
                     staticClass: "brand-text",
                     attrs: {
                         type: "text"
                     },
                     on: {
@@ -504,15 +501,19 @@
                     attrs: {
                         command: "en"
                     }
                 }, [e._v("English")]), t("el-dropdown-item", {
                     attrs: {
                         command: "zh-cn"
                     }
-                }, [e._v("简体中文")])], 1)], 1)], 1), t("el-main", {
+                }, [e._v("简体中文")]), t("el-dropdown-item", {
+                    attrs: {
+                        command: "jp"
+                    }
+                }, [e._v("日本語")])], 1)], 1)], 1), t("el-main", {
                     staticStyle: {
                         "padding-top": "0"
                     }
                 }, [t("keep-alive", [t(e.currentTabComponent, {
                     tag: "component",
                     attrs: {
                         "version-info": e.versionInfo
@@ -570,15 +571,15 @@
                     },
                     on: {
                         click: e.connectServer
                     }
                 }, [e._v(e._s(e.$t("Connect")))])], 1)], 1)], 1)
             },
             n = [],
-            s = (a("14d9"), a("fb6a"), a("d3b7"), a("159b"), function() {
+            s = (o("14d9"), o("fb6a"), o("d3b7"), o("159b"), function() {
                 var e = this,
                     t = e._self._c;
                 return t("div", {
                     staticClass: "home"
                 }, [t("h1", {
                     staticStyle: {
                         "text-align": "center"
@@ -897,23 +898,25 @@
                     },
                     on: {
                         click: e.handleRegister
                     }
                 }, [e._v(e._s(e.$t("Register")))])], 1)], 1)], 1)
             }),
             i = [],
-            l = (a("b0c0"), a("e9c4"), a("99af"), a("2e26")),
-            c = a.n(l),
-            u = a("4897"),
-            p = a.n(u),
-            d = a("b2d6"),
-            f = a.n(d),
-            h = a("f0d9"),
-            m = a.n(h),
-            v = {
+            l = (o("b0c0"), o("e9c4"), o("99af"), o("2e26")),
+            c = o.n(l),
+            u = o("4897"),
+            p = o.n(u),
+            d = o("b2d6"),
+            f = o.n(d),
+            h = o("f0d9"),
+            m = o.n(h),
+            v = o("c3ff"),
+            b = o.n(v),
+            g = {
                 "": {
                     language: "zh-CN",
                     "plural-forms": "nplurals=2; plural=n>1;"
                 },
                 "Server error: please check console output and make sure server is on": "服务器错误：请确认 pyarmor-webui 后台服务已经在运行，并检查控制台输出",
                 "Could not connect to pyarmor server, make sure it runs on %1": "无法连接到后台服务：%1",
                 "My Projects": "我的工程",
@@ -1148,164 +1151,408 @@
                 "Are you sure remove this project: %1 ?": "你确认要删除这个工程 %1 吗？",
                 "Pack obfuscated scripts successfully, the final bundle is saved: %1": "加密打包成功，输出结果：%1",
                 "Obfuscate the scripts successfully, the result is saved to %1": "加密脚本成功，输出目录：%1",
                 "The project %1 has been created": "工程 %1 已经被成功创建",
                 "The project %1 has been updated": "工程 %1 已经被更新",
                 "The license has been saved to %1": "许可证已经被保存在 %1"
             },
-            b = v,
-            g = a("b2cf").default();
-        g.loadJSON(b);
-        var y = {
+            y = g,
+            x = {
+                "": {
+                    language: "ja",
+                    "plural-forms": "nplurals=2; plural=n>1;"
+                },
+                "Server error: please check console output and make sure server is on": "サーバーエラー、pyarmorのバックグラウンドサービスは運転するに確認して、コンソールは入力にチェックしてください",
+                "Could not connect to pyarmor server, make sure it runs on %1": "バックグラウンドサービスに接続できません: %1",
+                "My Projects": "我のプロジェクト",
+                "My Licenses": "我のライセンス",
+                "Please type pyarmor server url:": "pyarmorのバクグランドサービスアドレスを入力してください：",
+                Connect: "接続",
+                "Connect Pyarmor Server": "Pyarmorサーバーへの接続",
+                "Select one license file to restrict the obfuscated script": "暗号化スクリプトライセンスのが選択",
+                "Default license, no any restrict": "デフォルトライセンスの使用",
+                "Do not include license file": "ライセンスは使用ません",
+                Home: "ホームページ",
+                "Obfuscate Script Wizard": "暗号化スクリプトウィザード",
+                "Obfuscate With Project": "プロジェクト暗号化の使用",
+                "Pack Script Wizard": "暗号化パッケージウィザード",
+                "Pack With Project": "プロジェクトパッケージの使用",
+                "Generate Expired License": "時間制限ライセンス",
+                "Fixed Machine License": "指定マシンライセンス",
+                "Full Features License": "全部フィーチャーライセンス",
+                "Register Pyarmor": "pyarmorの登録",
+                "Please type registration code or full path filename": "登録コードまたはフルパス登録ファイル名を入力してください",
+                "Product name": "製品名",
+                "Select activation file or registeration file": "アクティブ化ファイルまたは登録ファイルの選択",
+                "Activation file pyarmor-regcode-xxxx.txt is used for initial registeration, product name is required": "アクティブ化ファイル（pyarmor-regcode-xxxx.txt):第1回の登録に使用、以下に製品名を入力する必要があります",
+                "Registration file pyarmor-regfile-xxxx.zip for subsequent registration, product name is not required": "登録ファイル（pyarmor-regfile-xxxx.zip）：後続のすべての登録に使用、製品名に入力する必要がありません",
+                "Initial registration is successful, the registration file %1 has been generated, please use this file for subsequent registration": "第1回の登録はもう完成、登録ファイル %1 は生成、後で登録する場合は、この圧縮ファイルをそのまま使用してください",
+                "No activation file?": "ファイルはまだアクティブになっていませんか？",
+                "https://order.mycommerce.com/product?vendorid=200089125&productid=301044051": "https://order.mycommerce.com/product?vendorid=200089125&productid=301044051",
+                "Click here to purchase one": "ここにクリックで購入します",
+                Cancel: "取り消し",
+                Register: "登録",
+                "Register Pyarmor successfully": "Pyarmor の登録は成功しました",
+                "regfile is empty": "登録ファイルはないです",
+                "High Security": "高いセキュリティ",
+                "High Speed": "高性能",
+                "Cross platform, select one or more platforms to run obfuscated scripts": "クロスプラットフォームによる公開に使用、暗号化スクリプトを実行する目標プラットフォームのが選択します",
+                About: "に関して",
+                "Pyarmor server is not running on": "pyarmorバックグラウンドサービスは起動していません",
+                "Make sure the server is running, or click here to": "バックグラウンドサービスは運転するに確認してください、またはクリックここです",
+                "connect another server url": "ほかのアドレスのバックグラウンドサービスを接続します",
+                "Pyarmor is a powerful tool in the field of protecting and distributing python scripts.": "pyarmorは暗号化保護とPythonスクリプトの発行のための強力なツールです。",
+                "The goal of Pyarmor is to make Python applied to commercial application easily.": "pyarmorの目標はPythonをビジネスソフトウェアにより広く応用できるようにすることであります。",
+                "Project Home": "プロジェクトのホームページ",
+                "https://pyarmor.readthedocs.io/en/stable/": "https://pyarmor.readthedocs.io/en/stable/",
+                Documentation: "ドキュメント",
+                "https://pyarmor.readthedocs.io/en/stable/licenses.html": "https://pyarmor.readthedocs.io/en/stable/licenses.html",
+                "License & Purchase": "ライセンスと購入",
+                "Report Issues": "問題のレポート作成",
+                Contact: "連絡先",
+                "Copyright @ 2008 - 2023 Dashingsoft Corp.": "著作権所有 @ 2008 - 2023 西安DXソフトウェア",
+                Common: "よく用いられます",
+                Others: "その他",
+                "VM Protection": "仮想モード",
+                "Parent directory": "上位レベルのディレクトリ",
+                "Restore init value": "初期値の復元",
+                "Root path and favorite paths": "ルート目録といつも使った目録",
+                "Create new path": "新しい目録の作成",
+                "Delete an empty path": "空の目録を削除",
+                "Accept path": "現在選択されている目録を受け入れます",
+                "This is top path": "すでに最上位目録",
+                Input: "ダイアログを入力",
+                Confirm: "確認",
+                New: "作成",
+                Refresh: "リフレッシュ",
+                Expired: "有効期間",
+                Harddisk: "HDDのシリアル番号",
+                IPv4: "IPv4",
+                "Mac Address": "NIC MACアドレス",
+                "Disable Restrict Mode": "拘束モードの無効化",
+                "Extra Data": "カスタムデータ",
+                Filename: "ファイル名",
+                Name: "名",
+                Summary: "説明",
+                "Edit this license": "ライセンスの編集",
+                "Remove this license": "ライセンスの削除",
+                Src: "ソースパス",
+                Entry: "マスタースクリプト",
+                Output: "出力パス",
+                Target: "出力",
+                Path: "プロジェクトパス",
+                Title: "タイトル",
+                "Build this project": "このプロジェクトを構築します",
+                "Build with debug information in case something is wrong": "デバッグスイッチをオンにして構築します",
+                "Remove this project": "このプロジェクトを削除します",
+                "Edit this project": "このプロジェクトを編集します",
+                "Obfuscate all scripts in project": "暗号化プロジェクトのすべてのスクリプト",
+                "Building ": "構築プロジェクト ",
+                Build: "構築 ",
+                Diagnose: "構築（デバッグ）",
+                "Diagnosing project ": "コントロールモードを使用したプロジェクトの構築 ",
+                Start: "スタート",
+                "Data Files": "データファイル",
+                "Hidden Imports": "暗黙のモジュール",
+                "Binary Files": "ダイナミックライブラリファイル",
+                Icon: "アイコン",
+                "Extra Options": "他のオプション",
+                Finish: "終了",
+                "Base path for entry script, data files, binary files etc.": "全部他のファイル名の相対パス",
+                Script: "マスタースクリプト",
+                "The entry script": "ソースパスに相対するスクリプトを選択します",
+                "No obfuscated scripts in these paths": "暗号化不要なパスの除外、例えばvenv、testなど",
+                "Type module or package name, then press ENTER": "モジュール名を入力し、Enterを押します",
+                "Name an import not visible in the code of the script(s)": "スクリプトの中に暗黙にインプットされたモジユール名を入力します",
+                "Additional data files or folders to be added to the executable": "パッケージが必要なデータファイル",
+                "Type file name or path name relative to src, then press ENTER": "ソースパスに相対するファイル名を入力し、Enterを押します",
+                "Additional binary files to be added to the executable": "パッケージングが必要なバイナリダイナミックライブラリ",
+                "Type binary filename relative to src, then press ENTER": "ソースパスに相対するバイナリファイル名を入力し、Enterを押します",
+                "No Console": "コンソール",
+                "Do not provide a console window for standard I/O": "最終な実行可能ファイル実行時にコンソールを表示するかどうか",
+                "Apply icon to a Windows executable or the bundle on Mac OS X": "ソースパスに相対するアイコンファイルを入力します(WindowsとMacOS)",
+                "Any other PyInstaller options to append command line": "他のPalnstallerでサポートされているオプションを入力します",
+                "The default output path is $src/dist": "ソースパスの下のdistはデフォルト出力パス",
+                Bundle: "パッケージ化",
+                "Name to the bundled app (default: basename of entry script)": "最終にパッケージ化されたファイル名を入力します。デフォルトはマスタースクリプトの名前です",
+                "all to one folder": "ディレクトリ",
+                "all to one file": "ファイル",
+                "all to one file with outer license": "ファイル（ライセンスなし）",
+                Pack: "パッケージ",
+                Close: "閉じます",
+                Prev: "前のステップ",
+                Next: "次のステップ",
+                "Packing script ": "スクリプトをパケージンています ",
+                "Restrict Mode": "拘束モード",
+                "https://pyarmor.readthedocs.io/en/latest/mode.html#restrict-mode": "https://pyarmor.readthedocs.io/en/stable/",
+                "Select restrict mode": "拘束モードを選択します",
+                "Assert Call": "関数保護の有効化",
+                "Assert called functions are obfuscated": "呼び出された関数が暗号化されていることを確認します",
+                "Assert Import": "モジュール保護の有効化",
+                "Assert imported modules are obfuscated": "インポートされたモジュールが暗号化されていることを確認します",
+                "Disable all the restricts for the obfuscated scripts": "暗号化スクリプトに対するすべての制約と制限を無効にします",
+                "Use default restrictions": "暗号化スクリプトはデフォルトの制約と制限を使用します",
+                "Enable private mode for scripts": "プライベートモードに暗号化スクリプトを使用します",
+                "Enable restrict mode for packages": "拘束モードに暗号化パケッージを使用します",
+                "Bootstrap Code": "ブートモード",
+                "Select entry mode": "ブートコード挿入モードを選択します",
+                "Enable Suffix": "接尾辞モード",
+                "Generate runtime package with an unique suffix": "一意の接尾辞を含む実行支援パッケージを作成し、他のユーザーをインポートする暗号化パッケージの競合問題を解決します",
+                "Mixin Strings": "暗号化文字列",
+                "Mix all string values in the scripts": "スクリプト内のすべての文字列値を混同（関数、変数名を除く）",
+                "DO NOT insert bootstrap code into entry scripts": "マスタースクリプトにブートコードを挿入しないです",
+                "Insert bootstrap code into entry scripts": "マスタースクリプトにブートコードを自動挿入します（デフォルト）",
+                "Generate bootstrap code without leading dot (absolute import)": "ブートコードは絶対インポート方式を使用します（前の点はありません）",
+                "Generate bootstrap code with leading dot (relative import)": "ブートコードは、前の点を含むインポート方法を使用します",
+                "Mode 0: disable all the restricts for the obfuscated scripts": "モード 0: すべての拘束機能を無効にします",
+                "Mode 1: the obfuscated scripts can not be changed": "モード 1: 暗号化されたスクリプトは変更できません",
+                "Mode 2: mode 1 plus can not be imported by plain scripts": "モード 2: モード 1 +暗号化スクリプトは非暗号化スクリプトにインポートすることはできません",
+                "Mode 3: mode 2 plus module attributes protection": "モード 3 : 同じモード2でモジュール属性が保護されました",
+                "Mode 4: mode 3 but for package": "モード 4: 同じモード 3 でパッケージの暗号化には使用できます",
+                "Mode 5: mode 4 plus frame globals protection": "モード 5: 同じモード 4 で実行時にグローバル変数が保護されました",
+                "Mode 101: mode 1 plus module dictionary protection": "モード 101: 同じモード 1 でモジュール辞書を保護します",
+                "Mode 102: mode 2 plus module dictionary protection": "モード 102: 同じモード 2 でモジュール辞書を保護します",
+                "Mode 103: mode 3 plus module dictionary protection": "モード 103: 同じモード 3 でモジュール辞書を保護します",
+                "Mode 104: mode 4 plus module dictionary protection": "モード 104: 同じモード 4 でモジュール辞書を保護します",
+                "Mode 105: mode 5 plus module dictionary protection": "モード 105: 同じモード 5 でモジュール辞書を保護します",
+                "Bind obfuscated scripts to this serial number of harddisk": "暗号化スクリプトをハードディスクのシリアル番号にバインドします",
+                "Bind obfuscated scripts to this IPv4 address": "暗号化スクリプトを IPv4 アドレスにバインドします",
+                "Bind obfuscated scripts to this MAC address": "暗号化スクリプトをNIC Mac アドレスにバインドします",
+                Advanced: "高級",
+                "Cross Protection": "クロスプロテクション",
+                "Inject cross protection code into entry scripts before obfuscating": "暗号化時にクロスプロテクションコードをマスタースクリプトに注入してセキュリティを向上します",
+                "Package Name": "パッケージ名",
+                "Append this name to output path": "ディレクトリに含まれるパッケージの名前を入力します",
+                Platforms: "プラットフォーム",
+                License: "ライセンス",
+                Obfuscate: "暗号化",
+                "Obfuscate scripts: ": "暗号化スクリプト",
+                "Advanced Mode": "高級なモード",
+                "Disable or select advanced mode": "高級なモードの無効化または選択",
+                "Enable BCC Mode": "BBCモードを有効にします",
+                "Convert some Python functions to C functions": "変換モジュール内の Python 関数が C 関数になりました",
+                "Enable RFT Mode": "RFTモードを有効にします",
+                "Rename class/function/variable names": "モジュール内のクラス、関数、変数の名前を変更します",
+                "Change code object structure to improve security (only for x86/64 arch)": "セキュリティを向上させるためのコード構造の変更（x 86/64のみで使用可能）",
+                "Disable advanced mode": "高級なモードを無効にします",
+                "Enable advanced mode (only for x86/64 arch)": "高級なモードを有効にします（x 86/64のみで使用可能）",
+                "Enable super mode (only for Python 27, 37, 38, 39)": "スーパーモードを有効にします（Python 27、37、38、39のみサポート）",
+                "Enable advanced mode plus vm protection (only for Windows)": "高級なモードと仮想モードの両方を有効にします（Windowsプラットフォームのみで使用可能）",
+                "Enable super mode plus vm protection (only for Python 27, 37, 38, 39 in Windows)": "スーパーモードとスーパーモードの両方を有効にします（WindowsプラットフォームのPython 27、37、38、39のみサポート）",
+                "Enable super plus mode (only for Python 37, 38, 39 and x86_64)": "究極モードを有効にします（x 86 _64のPython 37、38、39を使用可能）",
+                "Obfuscate Module": "モジュール暗号化モード",
+                "Obfuscate the whole module": "モジュールオブジェクト全体を暗号化します",
+                "Obfuscate Code Object": "関数暗号化モード",
+                "Obfuscate each function (code object) in the module": "モジュール内の各関数を個別に暗号化します",
+                "Do not obfuscate functions": "関数を個別に暗号化しないです",
+                "Obfuscate each function with quick algorithm": "高速暗号化アルゴリズムを使用したモジュール内の各関数の暗号化",
+                "Obfuscate each function with complex algorithm": "複雑な暗号化アルゴリズムを使用したモジュール内の各関数の暗号化",
+                "Wrap Code Object": "動的暗号化モード",
+                "Obfuscate each function (code object) in runtime": "関数の実行終了後に暗号化を再開します",
+                "Bundle Name": "出力パッケージ名",
+                Plugins: "プラグイン",
+                "Type plugin name, then press ENTER": "プラグイン名を入力し、Enterを押します",
+                "Pack Options": "パッケージオプション",
+                "Please input any pyinstaller option": "Pylnstallerでサポートされている他のオプションを入力してください",
+                "Append this name to output path for package": "ここに入力した名前を出力ディレクトリに含める",
+                "Edit Project": "プロジェクトの編集",
+                "New Project": "プロジェクトの新規",
+                Basic: "基本",
+                Type: "タイプ",
+                "Pack all to one folder": "カタログにパッケージ化",
+                "Pack all to one file": "単一ファイルにパッケージ化",
+                "Pack all to one file with outer license": "単一ファイルにパッケージ化（ライセンスなし）",
+                "Obfuscate Mode": "暗号化モード",
+                "Advanced Options": "高級なオプション",
+                "Runtime Files": "実行支援ファイル",
+                Create: "作成",
+                Update: "更新",
+                "DO NOT generate runtime files": "実行支援ファイルを生成しないです",
+                "Generate runtime files as a module (only for Pyarmor 7)": "実行支援ファイルの生成（Pyarmor 7のみ）",
+                "Generate runtime files as a package": "実行支援パッケージの生成（デフォルト）",
+                "Please input project title": "新しいプロジェクトタイトル",
+                "Base path for scripts, include and exclude": "ソースパスは、他のファイルとディレクトリの相対パスです",
+                Scripts: "スクリプト",
+                "Select one or more entry scripts": "1つ以上のポータルスクリプトを選択します",
+                "Select one entry script": "ポータルスクリプトを選択します",
+                Include: "検索モード",
+                Exclude: "パスを除外します",
+                "Ignore the path and the .py files list here": "これらのパスの下にあるすべてのスクリプトは暗号化されません",
+                "Only the scripts list above": "リストされたスクリプトファイルのみを暗号化します",
+                "Only the .py files in the src path": "ソースパスの下にあるスクリプトファイルのみを暗号化します",
+                "All the scripts in the src path recursively": "ソースパスの下にあるすべてのスクリプトファイルを再帰に暗号化します",
+                "Edit License": "ライセンスの編集",
+                "New License": "ライセンスの作成",
+                "Leave it blank to set default name like reg-xxxxxx": "デフォルト名は reg-xxxxxx です",
+                "Expired the obfuscated scripts": "暗号化スクリプトの有効期間の設定",
+                "Enable Period Mode": "サイクルモードを有効にします",
+                "Any ascii string data to store in the license file": "カスタム文字列データ",
+                "Invalid input": "不正な入力",
+                "Please type path to create in %1": "%1 の下に入力したパスを作成します",
+                "This path has been created: %1": "パス %1 は作成されました",
+                "Are you sure to remove this path: %1 ?": "本当にこのパス %1 を削除しますか？",
+                "Are you sure remove this license: %1 ?": "本当にこのライセンス %1 を削除しますか？",
+                "Build successfully, the results saved in: %1": "構築に成功しました、出力ディレクト: %1",
+                "Are you sure remove this project: %1 ?": "本当にこのプロジェクト %1 を削除しますか？",
+                "Pack obfuscated scripts successfully, the final bundle is saved: %1": "暗号化パッケージングは成功しました、結果を出力: %1",
+                "Obfuscate the scripts successfully, the result is saved to %1": "暗号化スクリプトは成功しました、出力ディレクトリ: %1",
+                "The project %1 has been created": "ツール %1 は成功に作成されました",
+                "The project %1 has been updated": "ツール %1 は更新されました",
+                "The license has been saved to %1": "ライセンスは %1 に保存されました"
+            },
+            w = x,
+            j = o("b2cf").default();
+        j.loadJSON(y), j.loadJSON(w);
+        var _ = {
             install: function(e) {
                 e.prototype.$t = function() {
-                    return g.gettext.apply(g, arguments)
+                    return j.gettext.apply(j, arguments)
                 }
             }
         };
 
-        function x() {
-            return g.gettext.apply(g, arguments)
+        function P() {
+            return j.gettext.apply(j, arguments)
         }
 
-        function w(e) {
-            e && 0 === e.indexOf("zh") ? (p.a.use(m.a), g.setLocale("zh-CN")) : (p.a.use(f.a), g.setLocale(e))
+        function $(e) {
+            e && 0 === e.indexOf("zh") ? (p.a.use(m.a), j.setLocale("zh-CN")) : e && 0 === e.indexOf("jp") ? (p.a.use(b.a), j.setLocale("ja")) : (p.a.use(f.a), j.setLocale(e))
         }
-        var _ = [],
-            $ = function(e, t, a, o) {
+        var k = [],
+            I = function(e, t, o, a) {
                 var r = {
                     url: e,
                     method: "post",
                     type: "json",
                     crossOrigin: !0,
-                    success: a,
-                    error: o
+                    success: o,
+                    error: a
                 };
                 "undefined" !== typeof t && (r.data = JSON.stringify(t)), c()(r)
             },
-            j = new o["default"]({
+            C = new a["default"]({
                 data: function() {
                     return {
                         connected: !1,
                         serverUrl: "http://localhost:9096/"
                     }
                 },
                 methods: {
                     showError: function(e) {
-                        o["default"].prototype.$message({
+                        a["default"].prototype.$message({
                             type: "error",
-                            message: "string" === typeof e ? e : x("Server error: please check console output and make sure server is on"),
+                            message: "string" === typeof e ? e : P("Server error: please check console output and make sure server is on"),
                             showClose: !0,
                             duration: 3e4
                         })
                     },
-                    sendRequest: function(e, t, a, o, r) {
+                    sendRequest: function(e, t, o, a, r) {
                         var n = function(e) {
-                                "function" === typeof r ? r(e) : this.showError(e), this.$emit(a + "-fail")
+                                "function" === typeof r ? r(e) : this.showError(e), this.$emit(o + "-fail")
                             },
                             s = function(e) {
-                                0 === e.err ? (this.$emit(a, e.data), "function" === typeof o && o(e.data)) : n.call(this, e.data)
+                                0 === e.err ? (this.$emit(o, e.data), "function" === typeof a && a(e.data)) : n.call(this, e.data)
                             };
-                        $(e, t, s.bind(this), n.bind(this))
+                        I(e, t, s.bind(this), n.bind(this))
                     },
-                    loadRequest: function(e, t, a, o, r) {
+                    loadRequest: function(e, t, o, a, r) {
                         var n = this.$loading({
                                 lock: !0,
                                 text: r,
                                 spinner: "el-icon-loading",
                                 background: "rgba(0, 0, 0, 0.7)"
                             }),
                             s = function(e) {
-                                n.close(), this.showError(e), this.$emit(a + "-fail")
+                                n.close(), this.showError(e), this.$emit(o + "-fail")
                             },
                             i = function(e) {
-                                0 === e.err ? (n.close(), this.$emit(a, e.data), "function" === typeof o && o(e.data)) : s.call(this, e.data)
+                                0 === e.err ? (n.close(), this.$emit(o, e.data), "function" === typeof a && a(e.data)) : s.call(this, e.data)
                             };
-                        $(e, t, i.bind(this), s.bind(this))
+                        I(e, t, i.bind(this), s.bind(this))
                     },
                     connectServer: function() {
                         var e = this.serverUrl,
                             t = function t() {
-                                "/" === e ? (_ = [], this.connected = !1, this.showError(x("Could not connect to pyarmor server, make sure it runs on %1", this.serverUrl)), this.$emit("connect-changed", this.connected)) : (e = "/", $("/directory/list", {
+                                "/" === e ? (k = [], this.connected = !1, this.showError(P("Could not connect to pyarmor server, make sure it runs on %1", this.serverUrl)), this.$emit("connect-changed", this.connected)) : (e = "/", I("/directory/list", {
                                     path: "@"
-                                }, a.bind(this), t.bind(this)))
+                                }, o.bind(this), t.bind(this)))
                             },
-                            a = function(t) {
-                                0 === t.err && (this.serverUrl !== e && (this.serverUrl = e), _ = t.data.dirs, this.connected = !0, this.$emit("connect-changed", this.connected))
+                            o = function(t) {
+                                0 === t.err && (this.serverUrl !== e && (this.serverUrl = e), k = t.data.dirs, this.connected = !0, this.$emit("connect-changed", this.connected))
                             };
-                        $(this.serverUrl + "directory/list", {
+                        I(this.serverUrl + "directory/list", {
                             path: "@"
-                        }, a.bind(this), t.bind(this))
+                        }, o.bind(this), t.bind(this))
                     },
-                    queryVersion: function(e, t, a) {
-                        var o = this.serverUrl + "version";
-                        this.sendRequest(o, e, "query-version", t, a)
-                    },
-                    registerProduct: function(e, t, a) {
-                        var o = this.serverUrl + "register";
-                        this.sendRequest(o, e, "register-product", t, a)
-                    },
-                    listDirectory: function(e, t, a) {
-                        var o = this.serverUrl + "directory/list";
-                        this.sendRequest(o, e, "list-directory", t, a)
-                    },
-                    newDirectory: function(e, t, a) {
-                        var o = this.serverUrl + "directory/new";
-                        this.sendRequest(o, e, "new-directory", t, a)
-                    },
-                    removeDirectory: function(e, t, a) {
-                        var o = this.serverUrl + "directory/remove";
-                        this.sendRequest(o, e, "remove-directory", t, a)
-                    },
-                    newProject: function(e, t, a) {
-                        var o = this.serverUrl + "project/new";
-                        this.sendRequest(o, e, "new-project", t, a)
-                    },
-                    updateProject: function(e, t, a) {
-                        var o = this.serverUrl + "project/update";
-                        this.sendRequest(o, e, "update-project", t, a)
-                    },
-                    buildProject: function(e, t, a) {
-                        var o = this.serverUrl + "project/build";
-                        this.loadRequest(o, e, "build-project", t, a)
-                    },
-                    diagnoseProject: function(e, t, a) {
-                        var o = this.serverUrl + "project/diagnose";
-                        this.loadRequest(o, e, "diagnose-project", t, a)
-                    },
-                    removeProject: function(e, t, a) {
-                        var o = this.serverUrl + "project/remove";
-                        this.sendRequest(o, e, "remove-project", t, a)
-                    },
-                    listProject: function(e, t, a) {
-                        var o = this.serverUrl + "project/list";
-                        this.sendRequest(o, e, "list-project", t, a)
-                    },
-                    newLicense: function(e, t, a) {
-                        var o = this.serverUrl + "license/new";
-                        this.sendRequest(o, e, "new-license", t, a)
-                    },
-                    updateLicense: function(e, t, a) {
-                        var o = this.serverUrl + "license/update";
-                        this.sendRequest(o, e, "update-license", t, a)
-                    },
-                    removeLicense: function(e, t, a) {
-                        var o = this.serverUrl + "license/remove";
-                        this.sendRequest(o, e, "remove-license", t, a)
-                    },
-                    listLicense: function(e, t, a) {
-                        var o = this.serverUrl + "license/list";
-                        this.sendRequest(o, e, "list-license", t, a)
+                    queryVersion: function(e, t, o) {
+                        var a = this.serverUrl + "version";
+                        this.sendRequest(a, e, "query-version", t, o)
+                    },
+                    registerProduct: function(e, t, o) {
+                        var a = this.serverUrl + "register";
+                        this.sendRequest(a, e, "register-product", t, o)
+                    },
+                    listDirectory: function(e, t, o) {
+                        var a = this.serverUrl + "directory/list";
+                        this.sendRequest(a, e, "list-directory", t, o)
+                    },
+                    newDirectory: function(e, t, o) {
+                        var a = this.serverUrl + "directory/new";
+                        this.sendRequest(a, e, "new-directory", t, o)
+                    },
+                    removeDirectory: function(e, t, o) {
+                        var a = this.serverUrl + "directory/remove";
+                        this.sendRequest(a, e, "remove-directory", t, o)
+                    },
+                    newProject: function(e, t, o) {
+                        var a = this.serverUrl + "project/new";
+                        this.sendRequest(a, e, "new-project", t, o)
+                    },
+                    updateProject: function(e, t, o) {
+                        var a = this.serverUrl + "project/update";
+                        this.sendRequest(a, e, "update-project", t, o)
+                    },
+                    buildProject: function(e, t, o) {
+                        var a = this.serverUrl + "project/build";
+                        this.loadRequest(a, e, "build-project", t, o)
+                    },
+                    diagnoseProject: function(e, t, o) {
+                        var a = this.serverUrl + "project/diagnose";
+                        this.loadRequest(a, e, "diagnose-project", t, o)
+                    },
+                    removeProject: function(e, t, o) {
+                        var a = this.serverUrl + "project/remove";
+                        this.sendRequest(a, e, "remove-project", t, o)
+                    },
+                    listProject: function(e, t, o) {
+                        var a = this.serverUrl + "project/list";
+                        this.sendRequest(a, e, "list-project", t, o)
+                    },
+                    newLicense: function(e, t, o) {
+                        var a = this.serverUrl + "license/new";
+                        this.sendRequest(a, e, "new-license", t, o)
+                    },
+                    updateLicense: function(e, t, o) {
+                        var a = this.serverUrl + "license/update";
+                        this.sendRequest(a, e, "update-license", t, o)
+                    },
+                    removeLicense: function(e, t, o) {
+                        var a = this.serverUrl + "license/remove";
+                        this.sendRequest(a, e, "remove-license", t, o)
+                    },
+                    listLicense: function(e, t, o) {
+                        var a = this.serverUrl + "license/list";
+                        this.sendRequest(a, e, "list-license", t, o)
                     },
                     getFavorPath: function(e) {
-                        return "undefined" === typeof e || _.indexOf(e) > -1 ? _.slice() : _.concat(e)
+                        return "undefined" === typeof e || k.indexOf(e) > -1 ? k.slice() : k.concat(e)
                     }
                 }
             }),
-            P = {
+            S = {
                 name: "HomeTabIndex",
                 data: function() {
                     return {
                         regvalue: "",
                         reginfo: {
                             filename: "",
                             filedata: "",
@@ -1326,40 +1573,40 @@
                     openLicenseWizard: function(e) {
                         this.$emit("change-current-page", "LicensePageEdit", {
                             feature: e
                         })
                     },
                     selectFile: function(e) {
                         var t = this,
-                            a = new FileReader;
-                        this.reginfo.filename = e.name, this.reginfo.filedata = e.raw, a.onload = function(e) {
+                            o = new FileReader;
+                        this.reginfo.filename = e.name, this.reginfo.filedata = e.raw, o.onload = function(e) {
                             t.reginfo.filedata = e.target.result
-                        }, a.readAsDataURL(e.raw)
+                        }, o.readAsDataURL(e.raw)
                     },
                     removeFile: function() {
                         this.reginfo.filename = "", this.reginfo.filedata = ""
                     },
                     registerProduct: function() {
                         this.dialogVisible = !0
                     },
                     handleRegister: function() {
                         var e = this;
-                        this.$root.v8mode ? j.registerProduct(this.reginfo, (function(t) {
-                            e.dialogVisible = !1, "OK" === t ? e.$message(x("Register Pyarmor successfully")) : e.$confirm(x("Initial registration is successful, the registration file %1 has been generated, please use this file for subsequent registration", t))
-                        })) : j.registerProduct(this.regvalue, (function(t) {
-                            j.$emit("query-version", t), e.dialogVisible = !1, e.$message(x("Register Pyarmor successfully"))
+                        this.$root.v8mode ? C.registerProduct(this.reginfo, (function(t) {
+                            e.dialogVisible = !1, "OK" === t ? e.$message(P("Register Pyarmor successfully")) : e.$confirm(P("Initial registration is successful, the registration file %1 has been generated, please use this file for subsequent registration", t))
+                        })) : C.registerProduct(this.regvalue, (function(t) {
+                            C.$emit("query-version", t), e.dialogVisible = !1, e.$message(P("Register Pyarmor successfully"))
                         }))
                     }
                 }
             },
-            k = P,
-            I = (a("2733"), a("2877")),
-            C = Object(I["a"])(k, s, i, !1, null, "22a09c36", null),
-            S = C.exports,
-            D = function() {
+            O = S,
+            D = (o("2733"), o("2877")),
+            M = Object(D["a"])(O, s, i, !1, null, "22a09c36", null),
+            E = M.exports,
+            R = function() {
                 var e = this,
                     t = e._self._c;
                 return t("div", {
                     staticClass: "project-tab"
                 }, [t("el-button", {
                     attrs: {
                         size: "small"
@@ -1382,186 +1629,186 @@
                     }
                 }, [t("el-table-column", {
                     attrs: {
                         type: "expand"
                     },
                     scopedSlots: e._u([{
                         key: "default",
-                        fn: function(a) {
+                        fn: function(o) {
                             return [t("el-form", {
                                 staticClass: "home-table-expand",
                                 attrs: {
                                     "label-width": "100px",
                                     "label-position": "left",
                                     size: "mini"
                                 }
                             }, [t("el-form-item", {
                                 attrs: {
                                     label: e.$t("Src")
                                 }
-                            }, [t("span", [e._v(e._s(a.row.src))])]), t("el-form-item", {
+                            }, [t("span", [e._v(e._s(o.row.src))])]), t("el-form-item", {
                                 attrs: {
                                     label: e.$t("Entry")
                                 }
-                            }, [t("span", [e._v(e._s(a.row.entry))])]), t("el-form-item", {
+                            }, [t("span", [e._v(e._s(o.row.entry))])]), t("el-form-item", {
                                 attrs: {
                                     label: e.$t("Output")
                                 }
-                            }, [t("span", [e._v(e._s(e.getProjectOutput(a.row)))])]), t("el-form-item", {
+                            }, [t("span", [e._v(e._s(e.getProjectOutput(o.row)))])]), t("el-form-item", {
                                 attrs: {
                                     label: e.$t("Type")
                                 }
-                            }, [t("span", [e._v(e._s(e.getTargetName(a.row.buildTarget)))])]), t("el-form-item", {
+                            }, [t("span", [e._v(e._s(e.getTargetName(o.row.buildTarget)))])]), t("el-form-item", {
                                 attrs: {
                                     label: e.$t("Path")
                                 }
-                            }, [t("span", [e._v(e._s(a.row.path))])])], 1)]
+                            }, [t("span", [e._v(e._s(o.row.path))])])], 1)]
                         }
                     }])
                 }), t("el-table-column", {
                     attrs: {
                         sortable: "",
                         label: e.$t("Name"),
                         width: "180"
                     },
                     scopedSlots: e._u([{
                         key: "default",
-                        fn: function(a) {
+                        fn: function(o) {
                             return [t("el-link", {
                                 attrs: {
                                     underline: !1
                                 },
                                 on: {
                                     click: function(t) {
-                                        return e.editProject(a.row)
+                                        return e.editProject(o.row)
                                     }
                                 }
-                            }, [e._v(e._s(a.row.name))])]
+                            }, [e._v(e._s(o.row.name))])]
                         }
                     }])
                 }), t("el-table-column", {
                     attrs: {
                         prop: "title",
                         label: e.$t("Title")
                     }
                 }), t("el-table-column", {
                     attrs: {
                         align: "right"
                     },
                     scopedSlots: e._u([{
                         key: "default",
-                        fn: function(a) {
+                        fn: function(o) {
                             return [t("el-button", {
                                 attrs: {
                                     type: "text",
                                     title: e.$t("Build this project"),
                                     icon: "el-icon-s-tools",
                                     size: "medium"
                                 },
                                 on: {
                                     click: function(t) {
-                                        return e.buildProject(a.row)
+                                        return e.buildProject(o.row)
                                     }
                                 }
                             }), t("el-button", {
                                 attrs: {
                                     type: "text",
                                     title: e.$t("Build with debug information in case something is wrong"),
                                     icon: "el-icon-first-aid-kit",
                                     size: "medium"
                                 },
                                 on: {
                                     click: function(t) {
-                                        return e.diagnoseProject(a.row)
+                                        return e.diagnoseProject(o.row)
                                     }
                                 }
                             }), t("el-button", {
                                 attrs: {
                                     type: "text",
                                     title: e.$t("Remove this project"),
                                     icon: "el-icon-delete",
                                     size: "medium"
                                 },
                                 on: {
                                     click: function(t) {
-                                        return e.removeProject(a.row)
+                                        return e.removeProject(o.row)
                                     }
                                 }
                             }), t("el-button", {
                                 attrs: {
                                     type: "text",
                                     title: e.$t("Edit this project"),
                                     icon: "el-icon-edit",
                                     size: "medium"
                                 },
                                 on: {
                                     click: function(t) {
-                                        return e.editProject(a.row)
+                                        return e.editProject(o.row)
                                     }
                                 }
                             })]
                         }
                     }])
                 })], 1)], 1)
             },
-            O = [],
-            M = (a("a434"), {
+            T = [],
+            N = (o("a434"), {
                 name: "HomeTabProject",
                 data: function() {
                     return {
                         tableData: []
                     }
                 },
                 mounted: function() {
-                    j.$on("list-project", this.onListProject), j.$on("new-project", this.onProjectCreated), j.$on("remove-project", this.onProjectRemoved), j.$on("update-project", this.onProjectUpdated), this.refreshData()
+                    C.$on("list-project", this.onListProject), C.$on("new-project", this.onProjectCreated), C.$on("remove-project", this.onProjectRemoved), C.$on("update-project", this.onProjectUpdated), this.refreshData()
                 },
                 methods: {
                     getTargetName: function(e) {
-                        return x(0 === e ? "Obfuscate all scripts in project" : 1 === e ? "Pack all to one folder" : 2 === e ? "Pack all to one file" : "Pack all to one file with outer license")
+                        return P(0 === e ? "Obfuscate all scripts in project" : 1 === e ? "Pack all to one folder" : 2 === e ? "Pack all to one file" : "Pack all to one file with outer license")
                     },
                     getProjectOutput: function(e) {
                         var t = e.bundleName && e.bundleName.length ? "/" + e.bundleName : "";
                         return (e.output.length ? e.output : e.src + "/dist") + t
                     },
                     refreshData: function() {
-                        j.listProject()
+                        C.listProject()
                     },
                     newProject: function() {
                         this.$emit("change-current-page", "ProjectPageEdit")
                     },
                     buildProject: function(e) {
                         var t = this;
-                        j.buildProject(e, (function(e) {
+                        C.buildProject(e, (function(e) {
                             t.$message({
-                                message: x("Build successfully, the results saved in: %1", e),
+                                message: P("Build successfully, the results saved in: %1", e),
                                 duration: 0,
                                 showClose: !0
                             })
-                        }), x("Building ") + e.name)
+                        }), P("Building ") + e.name)
                     },
                     diagnoseProject: function(e) {
                         var t = this;
-                        j.diagnoseProject(e, (function(e) {
+                        C.diagnoseProject(e, (function(e) {
                             t.$message({
-                                message: x("Build successfully, the results saved in: %1", e),
+                                message: P("Build successfully, the results saved in: %1", e),
                                 duration: 0,
                                 showClose: !0
                             })
-                        }), x("Diagnosing project ") + e.name)
+                        }), P("Diagnosing project ") + e.name)
                     },
                     editProject: function(e) {
                         this.$emit("change-current-page", "ProjectPageEdit", {
                             projectInfo: JSON.parse(JSON.stringify(e))
                         })
                     },
                     removeProject: function(e) {
-                        this.$confirm(x("Are you sure remove this project: %1 ?", e.name), x("Confirm"), {
+                        this.$confirm(P("Are you sure remove this project: %1 ?", e.name), P("Confirm"), {
                             type: "warning"
                         }).then((function() {
-                            e["clean"] = !0, j.removeProject(e)
+                            e["clean"] = !0, C.removeProject(e)
                         }))
                     },
                     onListProject: function(e) {
                         this.tableData = e
                     },
                     onProjectCreated: function(e) {
                         0 !== this.tableData.length && this.tableData.slice(-1)[0].id === e.id || this.tableData.push(e)
@@ -1578,18 +1825,18 @@
                             if (this.tableData[t].id === e.id) {
                                 this.tableData.splice(t, 1);
                                 break
                             }
                     }
                 }
             }),
-            R = M,
-            N = (a("a764"), Object(I["a"])(R, D, O, !1, null, null, null)),
-            T = N.exports,
-            E = function() {
+            q = N,
+            L = (o("a764"), Object(D["a"])(q, R, T, !1, null, null, null)),
+            A = L.exports,
+            F = function() {
                 var e = this,
                     t = e._self._c;
                 return t("div", {
                     staticClass: "license-tab"
                 }, [t("el-button", {
                     attrs: {
                         size: "small"
@@ -1612,47 +1859,47 @@
                     }
                 }, [t("el-table-column", {
                     attrs: {
                         type: "expand"
                     },
                     scopedSlots: e._u([{
                         key: "default",
-                        fn: function(a) {
+                        fn: function(o) {
                             return [t("el-form", {
                                 staticClass: "home-table-expand",
                                 attrs: {
                                     "label-width": "180px",
                                     "label-position": "left",
                                     size: "mini"
                                 }
                             }, [t("el-form-item", {
                                 attrs: {
                                     label: e.$t("Expired")
                                 }
-                            }, [t("span", [e._v(e._s(a.row.expired))])]), t("el-form-item", {
+                            }, [t("span", [e._v(e._s(o.row.expired))])]), t("el-form-item", {
                                 attrs: {
                                     label: e.$t("Harddisk")
                                 }
-                            }, [t("span", [e._v(e._s(a.row.harddisk))])]), t("el-form-item", {
+                            }, [t("span", [e._v(e._s(o.row.harddisk))])]), t("el-form-item", {
                                 attrs: {
                                     label: e.$t("IPv4")
                                 }
-                            }, [t("span", [e._v(e._s(a.row.ipv4))])]), t("el-form-item", {
+                            }, [t("span", [e._v(e._s(o.row.ipv4))])]), t("el-form-item", {
                                 attrs: {
                                     label: e.$t("Mac Address")
                                 }
-                            }, [t("span", [e._v(e._s(a.row.mac))])]), e._e(), t("el-form-item", {
+                            }, [t("span", [e._v(e._s(o.row.mac))])]), e._e(), t("el-form-item", {
                                 attrs: {
                                     label: e.$t("Extra Data")
                                 }
-                            }, [t("span", [e._v(e._s(a.row.extraData))])]), t("el-form-item", {
+                            }, [t("span", [e._v(e._s(o.row.extraData))])]), t("el-form-item", {
                                 attrs: {
                                     label: e.$t("Filename")
                                 }
-                            }, [t("span", [e._v(e._s(a.row.filename))])])], 1)]
+                            }, [t("span", [e._v(e._s(o.row.filename))])])], 1)]
                         }
                     }])
                 }), t("el-table-column", {
                     attrs: {
                         sortable: "",
                         prop: "rcode",
                         label: e.$t("Name")
@@ -1665,72 +1912,72 @@
                     }
                 }), t("el-table-column", {
                     attrs: {
                         align: "right"
                     },
                     scopedSlots: e._u([{
                         key: "default",
-                        fn: function(a) {
+                        fn: function(o) {
                             return [t("el-button", {
                                 attrs: {
                                     type: "text",
                                     title: e.$t("Edit this license"),
                                     icon: "el-icon-edit",
                                     size: "medium"
                                 },
                                 on: {
                                     click: function(t) {
-                                        return e.editLicense(a.row)
+                                        return e.editLicense(o.row)
                                     }
                                 }
                             }), e._e(), t("el-button", {
                                 attrs: {
                                     type: "text",
                                     title: e.$t("Remove this license"),
                                     icon: "el-icon-delete",
                                     size: "medium"
                                 },
                                 on: {
                                     click: function(t) {
-                                        return e.removeLicense(a.row)
+                                        return e.removeLicense(o.row)
                                     }
                                 }
                             })]
                         }
                     }])
                 })], 1)], 1)
             },
-            q = [],
-            L = {
+            z = [],
+            B = {
                 name: "HomeTabLicense",
                 data: function() {
                     return {
                         tableData: []
                     }
                 },
                 mounted: function() {
-                    j.$on("list-license", this.onListLicense), j.$on("new-license", this.onLicenseCreated), j.$on("update-license", this.onLicenseUpdated), j.$on("remove-license", this.onLicenseRemoved), this.refreshData()
+                    C.$on("list-license", this.onListLicense), C.$on("new-license", this.onLicenseCreated), C.$on("update-license", this.onLicenseUpdated), C.$on("remove-license", this.onLicenseRemoved), this.refreshData()
                 },
                 methods: {
                     refreshData: function() {
-                        j.listLicense()
+                        C.listLicense()
                     },
                     newLicense: function() {
                         this.$emit("change-current-page", "LicensePageEdit")
                     },
                     editLicense: function(e) {
                         this.$emit("change-current-page", "LicensePageEdit", {
                             licenseInfo: JSON.parse(JSON.stringify(e))
                         })
                     },
                     removeLicense: function(e) {
-                        this.$confirm(x("Are you sure remove this license: %1 ?", e.rcode), x("Confirm"), {
+                        this.$confirm(P("Are you sure remove this license: %1 ?", e.rcode), P("Confirm"), {
                             type: "warning"
                         }).then((function() {
-                            j.removeLicense(e)
+                            C.removeLicense(e)
                         }))
                     },
                     onListLicense: function(e) {
                         this.tableData = e
                     },
                     onLicenseCreated: function(e) {
                         0 !== this.tableData.length && this.tableData.slice(-1)[0].id === e.id || this.tableData.push(e)
@@ -1747,27 +1994,27 @@
                             if (this.tableData[t].id === e.id) {
                                 this.tableData.splice(t, 1);
                                 break
                             }
                     }
                 }
             },
-            F = L,
-            A = Object(I["a"])(F, E, q, !1, null, null, null),
-            z = A.exports,
-            H = function() {
+            H = B,
+            V = Object(D["a"])(H, F, z, !1, null, null, null),
+            W = V.exports,
+            U = function() {
                 var e = this,
                     t = e._self._c;
                 return t("div", {
                     staticClass: "about"
                 }, [t("h1", {
                     staticStyle: {
                         "text-align": "center"
                     }
-                }, [e._v(e._s(e.$t("About")))]), t("p", [e._v("pyarmor-vue: 0.3.0")]), e.versionInfo.version ? t("div", [t("p", [e._v("pyarmor-server: " + e._s(e.versionInfo.server))]), t("p", [e._v("Python: " + e._s(e.versionInfo.python))]), e.versionInfo.regcode.length ? t("p", [e._v(" pyarmor (" + e._s(e.versionInfo.regcode.slice(-6)) + "): " + e._s(e.versionInfo.version) + " ")]) : t("p", [e._v("pyarmor (" + e._s(e.versionInfo.tag) + "): " + e._s(e.versionInfo.version))]), e.versionInfo.reginfo.length ? t("p", [e._v(e._s(e.versionInfo.reginfo))]) : e._e()]) : t("div", [t("p", [e._v(e._s(e.$t("Pyarmor server is not running on")) + " "), t("span", [e._v("http://localhost:9096/")]), e._v(". " + e._s(e.$t("Make sure the server is running, or click here to")) + " "), t("el-button", {
+                }, [e._v(e._s(e.$t("About")))]), t("p", [e._v("pyarmor-vue: 0.3.1")]), e.versionInfo.version ? t("div", [t("p", [e._v("pyarmor-server: " + e._s(e.versionInfo.server))]), t("p", [e._v("Python: " + e._s(e.versionInfo.python))]), e.versionInfo.regcode.length ? t("p", [e._v(" pyarmor (" + e._s(e.versionInfo.regcode.slice(-6)) + "): " + e._s(e.versionInfo.version) + " ")]) : t("p", [e._v("pyarmor (" + e._s(e.versionInfo.tag) + "): " + e._s(e.versionInfo.version))]), e.versionInfo.reginfo.length ? t("p", [e._v(e._s(e.versionInfo.reginfo))]) : e._e()]) : t("div", [t("p", [e._v(e._s(e.$t("Pyarmor server is not running on")) + " "), t("span", [e._v("http://localhost:9096/")]), e._v(". " + e._s(e.$t("Make sure the server is running, or click here to")) + " "), t("el-button", {
                     attrs: {
                         type: "text"
                     },
                     on: {
                         click: function(t) {
                             return e.$emit("connect-server")
                         }
@@ -1807,23 +2054,23 @@
                         underline: !1,
                         target: "_blank",
                         type: "primary",
                         href: "mailto:pyarmor@163.com"
                     }
                 }, [e._v(e._s(e.$t("Contact")))])], 1)]), t("p", [e._v(e._s(e.$t("Copyright @ 2008 - 2023 Dashingsoft Corp.")))])])])
             },
-            B = [],
-            V = {
+            G = [],
+            X = {
                 name: "HomeTabAbout",
                 props: ["versionInfo"]
             },
-            U = V,
-            W = (a("592d"), Object(I["a"])(U, H, B, !1, null, "0fdd9383", null)),
-            X = W.exports,
-            G = function() {
+            J = X,
+            Q = (o("8e6f"), Object(D["a"])(J, U, G, !1, null, "729657e2", null)),
+            K = Q.exports,
+            Z = function() {
                 var e = this,
                     t = e._self._c;
                 return t("div", {
                     staticClass: "project-main"
                 }, [t("el-page-header", {
                     staticStyle: {
                         "margin-bottom": "16px"
@@ -1990,16 +2237,16 @@
                     }
                 }, [e._v(" " + e._s(e.$t("Diagnose")) + " ")]), t("el-button", {
                     on: {
                         click: e.goBack
                     }
                 }, [e._v(e._s(e.$t("Close")))])], 1)], 1)], 1)], 1)
             },
-            J = [],
-            Q = (a("a9e3"), function() {
+            Y = [],
+            ee = (o("a9e3"), function() {
                 var e = this,
                     t = e._self._c;
                 return t("div", {
                     staticClass: "project-file"
                 }, [t("el-form-item", {
                     attrs: {
                         rules: e.rules.src,
@@ -2107,28 +2354,28 @@
                         callback: function(t) {
                             e.$set(e.projectInfo, "exclude", t)
                         },
                         expression: "projectInfo.exclude"
                     }
                 })], 1)], 1)
             }),
-            K = [],
-            Z = (a("d81d"), a("a15b"), {
+            te = [],
+            oe = (o("d81d"), o("a15b"), {
                 name: "ProjectInputFile",
                 props: ["projectInfo"],
                 data: function() {
                     return {
                         includeOptions: [{
-                            label: x("Only the scripts list above"),
+                            label: P("Only the scripts list above"),
                             value: "exact"
                         }, {
-                            label: x("Only the .py files in the src path"),
+                            label: P("Only the .py files in the src path"),
                             value: "list"
                         }, {
-                            label: x("All the scripts in the src path recursively"),
+                            label: P("All the scripts in the src path recursively"),
                             value: "all"
                         }],
                         rules: {
                             src: {
                                 required: !0
                             }
                         }
@@ -2142,18 +2389,18 @@
                         else {
                             var t = this.$refs.entry2.value;
                             this.projectInfo.entry = "string" === typeof t ? [t] : t
                         }
                     }
                 }
             }),
-            Y = Z,
-            ee = Object(I["a"])(Y, Q, K, !1, null, null, null),
-            te = ee.exports,
-            ae = function() {
+            ae = oe,
+            re = Object(D["a"])(ae, ee, te, !1, null, null, null),
+            ne = re.exports,
+            se = function() {
                 var e = this,
                     t = e._self._c;
                 return t("div", {
                     staticClass: "project-file"
                 }, [t("el-form-item", {
                     directives: [{
                         name: "show",
@@ -2296,56 +2543,56 @@
                         callback: function(t) {
                             e.$set(e.projectInfo, "wrapMode", t)
                         },
                         expression: "projectInfo.wrapMode"
                     }
                 })], 1)], 1)
             },
-            oe = [],
-            re = {
+            ie = [],
+            le = {
                 name: "ProjectInputFile",
                 props: ["projectInfo"],
                 data: function() {
                     return {
                         advancedModes: [{
-                            label: x("Disable advanced mode"),
+                            label: P("Disable advanced mode"),
                             value: 0
                         }, {
-                            label: x("Enable advanced mode (only for x86/64 arch)"),
+                            label: P("Enable advanced mode (only for x86/64 arch)"),
                             value: 1
                         }, {
-                            label: x("Enable super mode (only for Python 27, 37, 38, 39)"),
+                            label: P("Enable super mode (only for Python 27, 37, 38, 39)"),
                             value: 2
                         }, {
-                            label: x("Enable advanced mode plus vm protection (only for Windows)"),
+                            label: P("Enable advanced mode plus vm protection (only for Windows)"),
                             value: 3
                         }, {
-                            label: x("Enable super mode plus vm protection (only for Python 27, 37, 38, 39 in Windows)"),
+                            label: P("Enable super mode plus vm protection (only for Python 27, 37, 38, 39 in Windows)"),
                             value: 4
                         }, {
-                            label: x("Enable super plus mode (only for Python 37, 38, 39 and x86_64)"),
+                            label: P("Enable super plus mode (only for Python 37, 38, 39 and x86_64)"),
                             value: 5
                         }],
                         obfCodeModes: [{
-                            label: x("Do not obfuscate functions"),
+                            label: P("Do not obfuscate functions"),
                             value: 0
                         }, {
-                            label: x("Obfuscate each function with quick algorithm"),
+                            label: P("Obfuscate each function with quick algorithm"),
                             value: 1
                         }, {
-                            label: x("Obfuscate each function with complex algorithm"),
+                            label: P("Obfuscate each function with complex algorithm"),
                             value: 2
                         }]
                     }
                 }
             },
-            ne = re,
-            se = Object(I["a"])(ne, ae, oe, !1, null, null, null),
-            ie = se.exports,
-            le = function() {
+            ce = le,
+            ue = Object(D["a"])(ce, se, ie, !1, null, null, null),
+            pe = ue.exports,
+            de = function() {
                 var e = this,
                     t = e._self._c;
                 return t("div", {
                     staticClass: "project-target"
                 }, [t("el-form-item", {
                     attrs: {
                         label: e.$t("Output")
@@ -2500,24 +2747,24 @@
                         callback: function(t) {
                             e.packOptions = t
                         },
                         expression: "packOptions"
                     }
                 })], 1)], 1) : e._e()], 1)
             },
-            ce = [],
-            ue = {
+            fe = [],
+            he = {
                 name: "ProjectInputTarget",
                 props: ["projectInfo"],
                 computed: {
                     isPackProject: function() {
                         return this.projectInfo.buildTarget > 0
                     },
                     bundlePlaceholder: function() {
-                        return this.projectInfo.buildTarget ? x("Name to the bundled app (default: basename of entry script)") : x("Append this name to output path for package")
+                        return this.projectInfo.buildTarget ? P("Name to the bundled app (default: basename of entry script)") : P("Append this name to output path for package")
                     },
                     autoOutputSuffix: {
                         get: function() {
                             return this.outputSuffixMode
                         },
                         set: function(e) {
                             this.outputSuffixMode = e, this.projectInfo.bundleName = e ? this.projectInfo.src.split("/").pop() : ""
@@ -2534,18 +2781,18 @@
                 },
                 data: function() {
                     return {
                         outputSuffixMode: !1
                     }
                 }
             },
-            pe = ue,
-            de = Object(I["a"])(pe, le, ce, !1, null, null, null),
-            fe = de.exports,
-            he = function() {
+            me = he,
+            ve = Object(D["a"])(me, de, fe, !1, null, null, null),
+            be = ve.exports,
+            ge = function() {
                 var e = this,
                     t = e._self._c;
                 return t("div", {
                     staticClass: "project-misc"
                 }, [t("el-form-item", {
                     directives: [{
                         name: "show",
@@ -2727,16 +2974,16 @@
                         callback: function(t) {
                             e.$set(e.projectInfo, "mixStrings", t)
                         },
                         expression: "projectInfo.mixStrings"
                     }
                 })], 1)], 1)
             },
-            me = [],
-            ve = {
+            ye = [],
+            xe = {
                 name: "ProjectInputMisc",
                 props: ["projectInfo"],
                 computed: {
                     isPackProject: function() {
                         return this.projectInfo.buildTarget > 0
                     },
                     assertCall: {
@@ -2755,86 +3002,86 @@
                             e ? this.projectInfo.restrictMode |= 16 : this.projectInfo.restrictMode &= -17
                         }
                     }
                 },
                 data: function() {
                     return {
                         bootstrapModes: [{
-                            label: x("DO NOT insert bootstrap code into entry scripts"),
+                            label: P("DO NOT insert bootstrap code into entry scripts"),
                             value: 0
                         }, {
-                            label: x("Insert bootstrap code into entry scripts"),
+                            label: P("Insert bootstrap code into entry scripts"),
                             value: 1
                         }, {
-                            label: x("Generate bootstrap code without leading dot (absolute import)"),
+                            label: P("Generate bootstrap code without leading dot (absolute import)"),
                             value: 2
                         }, {
-                            label: x("Generate bootstrap code with leading dot (relative import)"),
+                            label: P("Generate bootstrap code with leading dot (relative import)"),
                             value: 3
                         }],
                         restrictModes: [{
-                            label: x("Mode 0: disable all the restricts for the obfuscated scripts"),
+                            label: P("Mode 0: disable all the restricts for the obfuscated scripts"),
                             value: 0
                         }, {
-                            label: x("Mode 1: the obfuscated scripts can not be changed"),
+                            label: P("Mode 1: the obfuscated scripts can not be changed"),
                             value: 1
                         }, {
-                            label: x("Mode 2: mode 1 plus can not be imported by plain scripts"),
+                            label: P("Mode 2: mode 1 plus can not be imported by plain scripts"),
                             value: 2
                         }, {
-                            label: x("Mode 3: mode 2 plus module attributes protection"),
+                            label: P("Mode 3: mode 2 plus module attributes protection"),
                             value: 3
                         }, {
-                            label: x("Mode 4: mode 3 but for package"),
+                            label: P("Mode 4: mode 3 but for package"),
                             value: 4
                         }, {
-                            label: x("Mode 5: mode 4 plus frame globals protection"),
+                            label: P("Mode 5: mode 4 plus frame globals protection"),
                             value: 5
                         }, {
-                            label: x("Mode 101: mode 1 plus module dictionary protection"),
+                            label: P("Mode 101: mode 1 plus module dictionary protection"),
                             value: 101
                         }, {
-                            label: x("Mode 102: mode 2 plus module dictionary protection"),
+                            label: P("Mode 102: mode 2 plus module dictionary protection"),
                             value: 102
                         }, {
-                            label: x("Mode 103: mode 3 plus module dictionary protection"),
+                            label: P("Mode 103: mode 3 plus module dictionary protection"),
                             value: 103
                         }, {
-                            label: x("Mode 104: mode 4 plus module dictionary protection"),
+                            label: P("Mode 104: mode 4 plus module dictionary protection"),
                             value: 104
                         }, {
-                            label: x("Mode 105: mode 5 plus module dictionary protection"),
+                            label: P("Mode 105: mode 5 plus module dictionary protection"),
                             value: 105
                         }],
                         restrictModes8: [{
-                            label: x("Disable all the restricts for the obfuscated scripts"),
+                            label: P("Disable all the restricts for the obfuscated scripts"),
                             value: 8
                         }, {
-                            label: x("Use default restrictions"),
+                            label: P("Use default restrictions"),
                             value: 1
                         }, {
-                            label: x("Enable private mode for scripts"),
+                            label: P("Enable private mode for scripts"),
                             value: 2
                         }, {
-                            label: x("Enable restrict mode for packages"),
+                            label: P("Enable restrict mode for packages"),
                             value: 4
                         }]
                     }
                 }
             },
-            be = ve,
-            ge = Object(I["a"])(be, he, me, !1, null, null, null),
-            ye = ge.exports,
-            xe = {
+            we = xe,
+            je = Object(D["a"])(we, ge, ye, !1, null, null, null),
+            _e = je.exports,
+            Pe = {
                 name: "ProjectPageEdit",
                 components: {
-                    ProjectInputFile: te,
-                    ProjectInputMode: ie,
-                    ProjectInputTarget: fe,
-                    ProjectInputMisc: ye
+                    ProjectInputFile: ne,
+                    ProjectInputMode: pe,
+                    ProjectInputTarget: be,
+                    ProjectInputMisc: _e
                 },
                 props: {
                     target: {
                         type: Number,
                         default: 0
                     },
                     projectInfo: {
@@ -2871,21 +3118,21 @@
                             }
                         }
                     }
                 },
                 data: function() {
                     return {
                         runtimeOptions: [{
-                            label: x("DO NOT generate runtime files"),
+                            label: P("DO NOT generate runtime files"),
                             value: -1
                         }, {
-                            label: x("Generate runtime files as a module (only for Pyarmor 7)"),
+                            label: P("Generate runtime files as a module (only for Pyarmor 7)"),
                             value: 0
                         }, {
-                            label: x("Generate runtime files as a package"),
+                            label: P("Generate runtime files as a package"),
                             value: 1
                         }]
                     }
                 },
                 computed: {
                     isEdit: function() {
                         return this.projectInfo.id
@@ -2901,56 +3148,56 @@
                 },
                 methods: {
                     goBack: function() {
                         this.$emit("close-current-page")
                     },
                     onBuild: function() {
                         var e = this;
-                        j.buildProject(this.projectInfo, (function(t) {
+                        C.buildProject(this.projectInfo, (function(t) {
                             e.$message({
-                                message: x("Build successfully, the results saved in: %1", t),
+                                message: P("Build successfully, the results saved in: %1", t),
                                 duration: 0,
                                 showClose: !0
                             })
-                        }), x("Building ") + this.projectInfo.title)
+                        }), P("Building ") + this.projectInfo.title)
                     },
                     onDiagnose: function() {
                         var e = this;
-                        j.diagnoseProject(this.projectInfo, (function(t) {
+                        C.diagnoseProject(this.projectInfo, (function(t) {
                             e.$message({
-                                message: x("Build successfully, the results saved in: %1", t),
+                                message: P("Build successfully, the results saved in: %1", t),
                                 duration: 0,
                                 showClose: !0
                             })
-                        }), x("Diagnosing project ") + this.projectInfo.title)
+                        }), P("Diagnosing project ") + this.projectInfo.title)
                     },
                     onSubmit: function() {
                         var e = this;
                         this.$refs.form.validate((function(t) {
-                            t && (e.isEdit ? j.updateProject(e.projectInfo, e.onProjectUpdated) : j.newProject(e.projectInfo, e.onProjectUpdated))
+                            t && (e.isEdit ? C.updateProject(e.projectInfo, e.onProjectUpdated) : C.newProject(e.projectInfo, e.onProjectUpdated))
                         }))
                     },
                     onProjectUpdated: function(e) {
-                        this.$message(this.isEdit ? x("The project %1 has been updated", e.name) : x("The project %1 has been created", e.name)), this.isEdit || this.goBack()
+                        this.$message(this.isEdit ? P("The project %1 has been updated", e.name) : P("The project %1 has been created", e.name)), this.isEdit || this.goBack()
                     },
                     changeProjectTitle: function() {
                         var e = this;
-                        this.$prompt(x("Please input project title"), x("Input"), {
+                        this.$prompt(P("Please input project title"), P("Input"), {
                             inputValue: this.projectInfo.title
                         }).then((function(t) {
-                            var a = t.value;
-                            e.projectInfo.title = a
+                            var o = t.value;
+                            e.projectInfo.title = o
                         }))
                     }
                 }
             },
-            we = xe,
-            _e = (a("59d9"), Object(I["a"])(we, G, J, !1, null, "5398bc94", null)),
-            $e = _e.exports,
-            je = function() {
+            $e = Pe,
+            ke = (o("59d9"), Object(D["a"])($e, Z, Y, !1, null, "5398bc94", null)),
+            Ie = ke.exports,
+            Ce = function() {
                 var e = this,
                     t = e._self._c;
                 return t("el-card", {
                     staticClass: "box-card"
                 }, [t("el-page-header", {
                     attrs: {
                         content: e.licenseInfo.id ? e.$t("Edit License") : e.$t("New License")
@@ -3037,16 +3284,16 @@
                     }
                 }, [e._v(" " + e._s(e.licenseInfo.id ? e.$t("Update") : e.$t("Create")) + " ")]), t("el-button", {
                     on: {
                         click: e.goBack
                     }
                 }, [e._v(e._s(e.$t("Cancel")))])], 1)], 1)], 1)
             },
-            Pe = [],
-            ke = (a("b64b"), function() {
+            Se = [],
+            Oe = (o("b64b"), function() {
                 var e = this,
                     t = e._self._c;
                 return t("div", [t("el-form-item", {
                     attrs: {
                         label: e.$t("Harddisk")
                     }
                 }, [t("el-input", {
@@ -3090,26 +3337,26 @@
                         callback: function(t) {
                             e.$set(e.licenseInfo, "mac", t)
                         },
                         expression: "licenseInfo.mac"
                     }
                 })], 1)], 1)
             }),
-            Ie = [],
-            Ce = {
+            De = [],
+            Me = {
                 name: "LicenseInputMachine",
                 props: ["licenseInfo"]
             },
-            Se = Ce,
-            De = Object(I["a"])(Se, ke, Ie, !1, null, null, null),
-            Oe = De.exports,
-            Me = {
+            Ee = Me,
+            Re = Object(D["a"])(Ee, Oe, De, !1, null, null, null),
+            Te = Re.exports,
+            Ne = {
                 name: "LicensePageEdit",
                 components: {
-                    LicenseInputMachine: Oe
+                    LicenseInputMachine: Te
                 },
                 props: {
                     feature: {
                         type: String,
                         default: "all"
                     },
                     licenseInfo: {
@@ -3131,15 +3378,15 @@
                 },
                 data: function() {
                     return {
                         cachedValue: JSON.stringify(this.licenseInfo),
                         rules: {
                             name: {
                                 pattern: "[-._0-9a-zA-Z]*",
-                                message: x("Invalid input"),
+                                message: P("Invalid input"),
                                 trigger: "change"
                             }
                         }
                     }
                 },
                 methods: {
                     hasFeature: function(e) {
@@ -3147,35 +3394,35 @@
                     },
                     goBack: function() {
                         this.$emit("close-current-page")
                     },
                     resetForm: function() {
                         var e = this,
                             t = JSON.parse(this.cachedValue);
-                        Object.keys(t).map((function(a) {
-                            t[a] !== e.licenseInfo[a] && (e.licenseInfo[a] = t[a])
+                        Object.keys(t).map((function(o) {
+                            t[o] !== e.licenseInfo[o] && (e.licenseInfo[o] = t[o])
                         }))
                     },
                     onSubmit: function() {
                         var e = this;
                         this.$refs["form"].validate((function(t) {
                             if (!t) return !1;
-                            var a = [];
-                            e.licenseInfo.expired && a.push(e.licenseInfo.expired), e.licenseInfo.harddisk && a.push(e.licenseInfo.harddisk), e.licenseInfo.mac && a.push(e.licenseInfo.mac), e.licenseInfo.ipv4 && a.push(e.licenseInfo.ipv4), e.licenseInfo.extraData && a.push("Extra data"), e.licenseInfo.disableRestrictMode && a.push("Disable restrict mode"), e.licenseInfo.enablePeriodMode && a.push("Enable period mode"), e.licenseInfo.summary = a.join(","), e.licenseInfo.id ? j.updateLicense(e.licenseInfo, e.onLicenseCreated) : j.newLicense(e.licenseInfo, e.onLicenseCreated)
+                            var o = [];
+                            e.licenseInfo.expired && o.push(e.licenseInfo.expired), e.licenseInfo.harddisk && o.push(e.licenseInfo.harddisk), e.licenseInfo.mac && o.push(e.licenseInfo.mac), e.licenseInfo.ipv4 && o.push(e.licenseInfo.ipv4), e.licenseInfo.extraData && o.push("Extra data"), e.licenseInfo.disableRestrictMode && o.push("Disable restrict mode"), e.licenseInfo.enablePeriodMode && o.push("Enable period mode"), e.licenseInfo.summary = o.join(","), e.licenseInfo.id ? C.updateLicense(e.licenseInfo, e.onLicenseCreated) : C.newLicense(e.licenseInfo, e.onLicenseCreated)
                         }))
                     },
                     onLicenseCreated: function(e) {
-                        this.$message(x("The license has been saved to %1", e.filename)), this.goBack()
+                        this.$message(P("The license has been saved to %1", e.filename)), this.goBack()
                     }
                 }
             },
-            Re = Me,
-            Ne = (a("59cf"), Object(I["a"])(Re, je, Pe, !1, null, "7a4ee3e2", null)),
-            Te = Ne.exports,
-            Ee = function() {
+            qe = Ne,
+            Le = (o("59cf"), Object(D["a"])(qe, Ce, Se, !1, null, "7a4ee3e2", null)),
+            Ae = Le.exports,
+            Fe = function() {
                 var e = this,
                     t = e._self._c;
                 return t("el-card", {
                     staticClass: "wizard-page"
                 }, [t("el-page-header", {
                     attrs: {
                         content: e.$t("Obfuscate Script Wizard")
@@ -3372,20 +3619,20 @@
                     on: {
                         click: e.next
                     }
                 }, [e._v(" " + e._s(e.$t("Next")) + " "), t("i", {
                     staticClass: "el-icon-arrow-right el-icon--right"
                 })])], 1)], 1)], 1)
             },
-            qe = [],
-            Le = {
+            ze = [],
+            Be = {
                 name: "ObfuscatePageWizard",
                 components: {
-                    ProjectInputFile: te,
-                    ProjectInputMisc: ye
+                    ProjectInputFile: ne,
+                    ProjectInputMisc: _e
                 },
                 props: {
                     feature: {
                         type: String,
                         default: ""
                     }
                 },
@@ -3454,25 +3701,25 @@
                     isItemVisible: function(e) {
                         return this.steps[this.active] === e
                     },
                     goBack: function() {
                         this.$emit("close-current-page")
                     },
                     obfuscateScript: function() {
-                        j.buildProject(this.projectInfo, this.onObfuscateFinished, x("Obfuscate scripts: ") + this.projectInfo.entry.join(","))
+                        C.buildProject(this.projectInfo, this.onObfuscateFinished, P("Obfuscate scripts: ") + this.projectInfo.entry.join(","))
                     },
                     onObfuscateFinished: function(e) {
-                        this.$message(x("Obfuscate the scripts successfully, the result is saved to %1", e))
+                        this.$message(P("Obfuscate the scripts successfully, the result is saved to %1", e))
                     }
                 }
             },
-            Fe = Le,
-            Ae = (a("3c61"), Object(I["a"])(Fe, Ee, qe, !1, null, "19c71758", null)),
-            ze = Ae.exports,
-            He = function() {
+            He = Be,
+            Ve = (o("3c61"), Object(D["a"])(He, Fe, ze, !1, null, "19c71758", null)),
+            We = Ve.exports,
+            Ue = function() {
                 var e = this,
                     t = e._self._c;
                 return t("el-card", {
                     staticClass: "wizard-page"
                 }, [t("el-page-header", {
                     attrs: {
                         content: e.$t("Pack Script Wizard")
@@ -3818,16 +4065,16 @@
                     on: {
                         click: e.next
                     }
                 }, [e._v(" " + e._s(e.$t("Next")) + " "), t("i", {
                     staticClass: "el-icon-arrow-right el-icon--right"
                 })])], 1)], 1)], 1)
             },
-            Be = [],
-            Ve = {
+            Ge = [],
+            Xe = {
                 name: "PackPageWizard",
                 props: {
                     feature: {
                         type: String,
                         default: ""
                     }
                 },
@@ -3861,18 +4108,18 @@
                 },
                 computed: {
                     projectInfo: function() {
                         var e = [this.formData.extraOptions],
                             t = this.formData.src;
                         return "file" === this.formData.target && e.push("--onefile"), this.formData.icon && e.push("--icon", this.formData.icon), this.formData.noConsole && e.push("--noconsole"), this.formData.hiddenImport.map((function(t) {
                             return e.push("--hidden-import", t)
-                        })), this.formData.dataFile.map((function(a) {
-                            return e.push("--add-data", t + "/" + a)
-                        })), this.formData.binaryFile.map((function(a) {
-                            return e.push("--add-binary", t + "/" + a)
+                        })), this.formData.dataFile.map((function(o) {
+                            return e.push("--add-data", t + "/" + o)
+                        })), this.formData.binaryFile.map((function(o) {
+                            return e.push("--add-binary", t + "/" + o)
                         })), {
                             src: this.formData.src,
                             entry: this.formData.entry,
                             include: "all",
                             exclude: this.formData.exclude,
                             buildTarget: this.formData.target,
                             output: this.formData.output,
@@ -3911,58 +4158,58 @@
                     isItemVisible: function(e) {
                         return this.steps[this.active] === e
                     },
                     goBack: function() {
                         this.$emit("close-current-page")
                     },
                     packScript: function() {
-                        j.buildProject(this.projectInfo, this.onPackFinished, x("Packing script ") + this.formData.entry)
+                        C.buildProject(this.projectInfo, this.onPackFinished, P("Packing script ") + this.formData.entry)
                     },
                     onPackFinished: function(e) {
-                        this.$message(x("Pack obfuscated scripts successfully, the final bundle is saved: %1", e))
+                        this.$message(P("Pack obfuscated scripts successfully, the final bundle is saved: %1", e))
                     }
                 }
             },
-            Ue = Ve,
-            We = (a("1d77"), a("0b5d"), Object(I["a"])(Ue, He, Be, !1, null, "d018edda", null)),
-            Xe = We.exports,
-            Ge = {
+            Je = Xe,
+            Qe = (o("1d77"), o("0b5d"), Object(D["a"])(Je, Ue, Ge, !1, null, "d018edda", null)),
+            Ke = Qe.exports,
+            Ze = {
                 name: "app",
                 components: {
-                    HomeTabIndex: S,
-                    HomeTabProject: T,
-                    HomeTabLicense: z,
-                    HomeTabAbout: X,
-                    ProjectPageEdit: $e,
-                    LicensePageEdit: Te,
-                    ObfuscatePageWizard: ze,
-                    PackPageWizard: Xe
+                    HomeTabIndex: E,
+                    HomeTabProject: A,
+                    HomeTabLicense: W,
+                    HomeTabAbout: K,
+                    ProjectPageEdit: Ie,
+                    LicensePageEdit: Ae,
+                    ObfuscatePageWizard: We,
+                    PackPageWizard: Ke
                 },
                 data: function() {
                     return {
                         lang: "English",
                         currentTabName: "HomeTabIndex",
                         currentPageName: "",
                         currentPageProps: {},
                         pageStack: [],
                         dialogVisible: !1,
-                        serverUrl: j.serverUrl,
+                        serverUrl: C.serverUrl,
                         v8mode: !0,
                         versionInfo: {
                             tag: "Off",
                             version: "",
                             regcode: "",
                             reginfo: "",
                             server: "",
                             python: ""
                         }
                     }
                 },
                 mounted: function() {
-                    j.$on("connect-changed", this.onServerChanged), this.connectServer(), "zh-cn" === localStorage.getItem("language") && this.changeLanguage("zh-cn")
+                    C.$on("connect-changed", this.onServerChanged), this.connectServer(), "zh-cn" === localStorage.getItem("language") ? this.changeLanguage("zh-cn") : "jp" === localStorage.getItem("language") && this.changeLanguage("jp")
                 },
                 computed: {
                     currentMode: function() {
                         return parseInt(this.versionInfo.version) > 7 ? this.v8mode ? "8" : "7+" : "7"
                     },
                     currentTabComponent: function() {
                         return this.currentTabName
@@ -3987,51 +4234,51 @@
                     onConnectSuccess: function(e) {
                         this.connected = !0, this.versionInfo.tag = e.regcode ? "" : "Trial", this.versionInfo.version = e.version, this.versionInfo.regcode = e.regcode, this.versionInfo.reginfo = e.reginfo, this.versionInfo.server = e.server, this.versionInfo.python = e.python, this.v8mode = !!e.v8mode, this.$root.v8mode = this.v8mode
                     },
                     onConnectFailed: function() {
                         this.connected = !1, this.versionInfo.tag = "Off", this.currentTabName = "HomeTabAbout"
                     },
                     onServerChanged: function(e) {
-                        e ? j.queryVersion({}, this.onConnectSuccess, this.onConnectFailed) : this.onConnectFailed()
+                        e ? C.queryVersion({}, this.onConnectSuccess, this.onConnectFailed) : this.onConnectFailed()
                     },
                     onConnectServer: function() {
-                        this.dialogVisible = !0, this.serverUrl = j.serverUrl
+                        this.dialogVisible = !0, this.serverUrl = C.serverUrl
                     },
                     connectServer: function() {
-                        this.dialogVisible = !1, "/" !== this.serverUrl.slice(-1) && (this.serverUrl += "/"), j.serverUrl = this.serverUrl, j.connectServer()
+                        this.dialogVisible = !1, "/" !== this.serverUrl.slice(-1) && (this.serverUrl += "/"), C.serverUrl = this.serverUrl, C.connectServer()
                     },
                     changeLanguage: function(e) {
-                        this.lang = "en" === e ? "English" : "简体中文", w(e);
+                        this.lang = "en" === e ? "English" : "jp" === e ? "日本語" : "简体中文", $(e);
                         var t = function e(t) {
                             t.$forceUpdate(), t.$children.forEach((function(t) {
                                 return e(t)
                             }))
                         };
                         t(this), localStorage.setItem("language", e)
                     }
                 }
             },
-            Je = Ge,
-            Qe = (a("50a8"), a("7d43"), Object(I["a"])(Je, r, n, !1, null, "a0b1b980", null)),
-            Ke = Qe.exports,
-            Ze = function() {
+            Ye = Ze,
+            et = (o("baa0"), o("5bb9"), Object(D["a"])(Ye, r, n, !1, null, "c232ea8c", null)),
+            tt = et.exports,
+            ot = function() {
                 var e = this,
                     t = e._self._c;
                 return t("div", {
                     staticClass: "about"
                 }, [e._v(" Generate Lecense ")])
             },
-            Ye = [],
-            et = {
+            at = [],
+            rt = {
                 name: "NotFoundPage"
             },
-            tt = et,
-            at = Object(I["a"])(tt, Ze, Ye, !1, null, null, null),
-            ot = at.exports,
-            rt = function() {
+            nt = rt,
+            st = Object(D["a"])(nt, ot, at, !1, null, null, null),
+            it = st.exports,
+            lt = function() {
                 var e = this,
                     t = e._self._c;
                 return t("el-select", {
                     ref: "select",
                     staticClass: "w-100",
                     attrs: {
                         clearable: "",
@@ -4058,28 +4305,28 @@
                 }, [e.prefixVisible ? t("el-breadcrumb", {
                     ref: "prefix",
                     attrs: {
                         slot: "prefix",
                         separator: "/"
                     },
                     slot: "prefix"
-                }, [e._l(e.prefix, (function(a, o) {
+                }, [e._l(e.prefix, (function(o, a) {
                     return t("el-breadcrumb-item", {
-                        key: o
+                        key: a
                     }, [t("el-button", {
                         attrs: {
                             type: "text",
                             size: "mini"
                         },
                         on: {
                             click: function(t) {
-                                return e.onEnterPrefix(o)
+                                return e.onEnterPrefix(a)
                             }
                         }
-                    }, [e._v(" " + e._s(o ? a : "@") + " ")])], 1)
+                    }, [e._v(" " + e._s(a ? o : "@") + " ")])], 1)
                 })), t("el-breadcrumb-item", {
                     key: -1
                 }, [t("el-button", {
                     attrs: {
                         type: "text",
                         size: "mini"
                     }
@@ -4150,45 +4397,45 @@
                         icon: "el-icon-check"
                     },
                     on: {
                         click: function(t) {
                             return t.stopPropagation(), e.onAcceptPath.apply(null, arguments)
                         }
                     }
-                })], 1), e._l(e.options, (function(a) {
+                })], 1), e._l(e.options, (function(o) {
                     return t("el-option", {
-                        key: a.value,
+                        key: o.value,
                         attrs: {
-                            label: a.label,
-                            value: a.value
+                            label: o.label,
+                            value: o.value
                         }
-                    }, [a.isdir ? t("el-button", {
+                    }, [o.isdir ? t("el-button", {
                         staticStyle: {
                             "margin-right": "16px"
                         },
                         attrs: {
                             size: "mini",
                             icon: "el-icon-arrow-down"
                         },
                         on: {
                             click: function(t) {
-                                return t.stopPropagation(), e.enterPath(a.value)
+                                return t.stopPropagation(), e.enterPath(o.value)
                             }
                         }
                     }) : t("span", {
                         staticStyle: {
                             "margin-right": "16px"
                         }
                     }, [t("i", {
                         staticClass: "el-icon-document"
-                    })]), t("span", [e._v(e._s(a.label))])], 1)
+                    })]), t("span", [e._v(e._s(o.label))])], 1)
                 }))], 2)
             },
-            nt = [],
-            st = (a("4de4"), {
+            ct = [],
+            ut = (o("4de4"), {
                 name: "SelectFolder",
                 model: {
                     prop: "value2",
                     event: "change2"
                 },
                 props: {
                     value2: String,
@@ -4242,56 +4489,56 @@
                         var e = this.$refs.prefix.$el.clientWidth;
                         this.inputElement.style.paddingLeft = this.prefixVisible && e > 10 ? e + "px" : ""
                     },
                     restoreInitPath: function() {
                         this.loading = !1, this.path = this.value2, this.prefix = this.splitPath(this.value2), this.value = this.prefix.length ? this.prefix.pop() : "", this.$nextTick(this.resetInputPadding), this.listRemoteDirectory("")
                     },
                     selectUpPath: function() {
-                        this.prefix.length ? (this.prefix.pop(), this.enterPath(this.joinPath(this.prefix))) : this.$message.warning(x("This is top path"))
+                        this.prefix.length ? (this.prefix.pop(), this.enterPath(this.joinPath(this.prefix))) : this.$message.warning(P("This is top path"))
                     },
                     selectRootPath: function() {
                         this.prefix = [], this.enterPath("")
                     },
                     onAcceptPath: function() {
                         var e = this;
                         "" === this.value && this.onValueChanged(this.joinPath(this.prefix)), this.$nextTick((function() {
                             e.$refs.select.blur()
                         }))
                     },
                     onCreatePath: function() {
                         var e = this;
-                        this.$prompt(x("Please type path to create in %1", this.path), x("Input"), {
+                        this.$prompt(P("Please type path to create in %1", this.path), P("Input"), {
                             inputValidator: function(e) {
                                 return e.length > 0
                             }
                         }).then((function(t) {
-                            var a = t.value;
-                            j.newDirectory([e.path, a].join("/"), (function(t) {
-                                e.$message(x("This path has been created: %1", t))
+                            var o = t.value;
+                            C.newDirectory([e.path, o].join("/"), (function(t) {
+                                e.$message(P("This path has been created: %1", t))
                             }))
                         }))
                     },
                     onDeletePath: function() {
                         var e = this;
-                        this.$confirm(x("Are you sure to remove this path: %1 ?", this.path), x("Confirm"), {}).then((function() {
-                            e.path.length > 2 && j.removeDirectory(e.path)
+                        this.$confirm(P("Are you sure to remove this path: %1 ?", this.path), P("Confirm"), {}).then((function() {
+                            e.path.length > 2 && C.removeDirectory(e.path)
                         }))
                     },
                     onEnterPrefix: function(e) {
                         this.enterPath(this.joinPath(this.prefix.slice(0, e + 1)))
                     },
                     listRemoteDirectory: function(e) {
                         var t = this;
-                        "" === e && 0 === this.prefix.length ? (this.source = j.getFavorPath(localStorage.getItem("recent.directory")).map((function(e) {
+                        "" === e && 0 === this.prefix.length ? (this.source = C.getFavorPath(localStorage.getItem("recent.directory")).map((function(e) {
                             return {
                                 label: e,
                                 value: e,
                                 isdir: !0
                             }
-                        })), this.options = this.source.slice()) : "" === e ? (this.loading = !0, j.listDirectory({
+                        })), this.options = this.source.slice()) : "" === e ? (this.loading = !0, C.listDirectory({
                             path: this.joinPath(this.prefix),
                             pattern: this.selectPattern
                         }, this.onListDirectory, this.onListDirectoryFailed)) : "<" === e || "^" === e ? this.prefix.length > 0 && this.$nextTick((function() {
                             t.inputElement.value = "", setTimeout((function() {
                                 t.enterPath(t.joinPath(t.prefix.slice(0, -1)))
                             }), 500)
                         })) : ">" === e.slice(-1) || "/" === e.slice(-1) ? (this.onFilterOptions(e.slice(0, -1)), 1 === this.options.length && this.$nextTick((function() {
@@ -4315,33 +4562,33 @@
                         }))), this.onFilterOptions("")
                     },
                     onListDirectoryFailed: function() {
                         this.loading = !1
                     },
                     onFilterOptions: function(e) {
                         var t = this;
-                        this.options = this.source.filter((function(a) {
-                            return (!t.onlyFolder || a.isdir) && a.value.indexOf(e) > -1
+                        this.options = this.source.filter((function(o) {
+                            return (!t.onlyFolder || o.isdir) && o.value.indexOf(e) > -1
                         }))
                     },
                     onVisibleChanged: function(e) {
                         e || this.$emit("change2", this.path)
                     },
                     onValueChanged: function(e) {
                         var t = this;
                         "/" === e.slice(0, 1) ? (this.path = e, this.prefix = this.splitPath(e), this.value = this.prefix.length ? this.prefix.pop() : "", this.$nextTick((function() {
                             t.resetInputPadding()
                         })), this.listRemoteDirectory("")) : this.path = this.joinPath("" === e ? this.prefix : this.prefix.concat(e)), this.path.length > 1 && this.onlyFolder && localStorage.setItem("recent.directory", this.path), this.$emit("change2", this.path)
                     }
                 }
             }),
-            it = st,
-            lt = Object(I["a"])(it, rt, nt, !1, null, null, null),
-            ct = lt.exports,
-            ut = function() {
+            pt = ut,
+            dt = Object(D["a"])(pt, lt, ct, !1, null, null, null),
+            ft = dt.exports,
+            ht = function() {
                 var e = this,
                     t = e._self._c;
                 return t("el-cascader", {
                     ref: "cascader",
                     staticClass: "w-100",
                     attrs: {
                         filterable: "",
@@ -4358,16 +4605,16 @@
                         callback: function(t) {
                             e.value = t
                         },
                         expression: "value"
                     }
                 })
             },
-            pt = [],
-            dt = (a("25f0"), {
+            mt = [],
+            vt = (o("25f0"), {
                 name: "SelectPathScript",
                 model: {
                     prop: "value2",
                     event: "change2"
                 },
                 props: {
                     value2: {
@@ -4431,60 +4678,60 @@
                     },
                     onExpandChanged: function(e) {
                         this.path = e.map((function(e) {
                             return e.toString()
                         })), "/" === this.path[0] && (this.path[0] = "")
                     },
                     listRemoteDirectory: function(e, t) {
-                        var a = this;
+                        var o = this;
                         if (!0 !== e.leaf && "" !== this.rootPath) {
-                            var o = e.level,
-                                r = 0 === o ? [] : this.path.slice(0, o - 1).concat(e.value);
-                            j.listDirectory({
+                            var a = e.level,
+                                r = 0 === a ? [] : this.path.slice(0, a - 1).concat(e.value);
+                            C.listDirectory({
                                 path: this.joinPath(this.splitPath(this.rootPath).concat(r)),
                                 pattern: this.selectPattern
-                            }, (function(o) {
-                                a.onListDirectory(e, t, o)
+                            }, (function(a) {
+                                o.onListDirectory(e, t, a)
                             }), (function() {
                                 return t()
                             }))
                         } else t()
                     },
-                    onListDirectory: function(e, t, a) {
-                        var o = this,
+                    onListDirectory: function(e, t, o) {
+                        var a = this,
                             r = e.level,
-                            n = (this.onlyFolder ? [] : a.files).map((function(e) {
+                            n = (this.onlyFolder ? [] : o.files).map((function(e) {
                                 return {
                                     label: e,
                                     value: e,
                                     leaf: !0
                                 }
-                            })).concat(a.dirs.map((function(e) {
+                            })).concat(o.dirs.map((function(e) {
                                 return {
                                     label: e,
                                     value: e
                                 }
                             })));
                         0 === r && this.value2.length > 0 && (this.value = this.multiple ? this.value2.map((function(e) {
                             return [e]
                         })) : this.value2, this.value.map((function(e) {
-                            var t = o.multiple ? e[0] : e;
+                            var t = a.multiple ? e[0] : e;
                             t.indexOf("/") > -1 && n.push({
                                 label: t,
                                 value: t,
                                 leaf: !0
                             })
                         }))), t(n.length ? n : void 0)
                     }
                 }
             }),
-            ft = dt,
-            ht = (a("586c"), Object(I["a"])(ft, ut, pt, !1, null, "222a0936", null)),
-            mt = ht.exports,
-            vt = function() {
+            bt = vt,
+            gt = (o("586c"), Object(D["a"])(bt, ht, mt, !1, null, "222a0936", null)),
+            yt = gt.exports,
+            xt = function() {
                 var e = this,
                     t = e._self._c;
                 return t("el-select", {
                     ref: "select",
                     staticClass: "w-100",
                     attrs: {
                         filterable: "",
@@ -4511,16 +4758,16 @@
                         attrs: {
                             label: e.label,
                             value: e.value
                         }
                     })
                 })), 1)
             },
-            bt = [],
-            gt = {
+            wt = [],
+            jt = {
                 name: "SelectLicenseFile",
                 model: {
                     prop: "value2",
                     event: "change2"
                 },
                 props: {
                     value2: String,
@@ -4538,52 +4785,52 @@
                     this.value = this.value2, this.refreshData()
                 },
                 methods: {
                     refreshData: function() {
                         this.listRemoteLicenses("")
                     },
                     listRemoteLicenses: function(e) {
-                        "" === e ? (this.loading = !0, j.listLicense({}, this.onListLicense, this.onListLicenseFailed)) : this.filterLicenses(e)
+                        "" === e ? (this.loading = !0, C.listLicense({}, this.onListLicense, this.onListLicenseFailed)) : this.filterLicenses(e)
                     },
                     filterLicenses: function(e) {
                         this.options = this.source.filter((function(t) {
                             return t.label.indexOf(e) > -1
                         }))
                     },
                     onValueChanged: function(e) {
                         this.$emit("change2", e)
                     },
                     onListLicense: function(e) {
                         this.loading = !1, this.source = [{
-                            label: x("Default license, no any restrict"),
+                            label: P("Default license, no any restrict"),
                             value: "true"
                         }, {
-                            label: x("Do not include license file"),
+                            label: P("Do not include license file"),
                             value: "false"
                         }].concat(e.map((function(e) {
                             return {
                                 label: [e.rcode, e.summary].join(": "),
                                 value: e.filename
                             }
                         }))), this.filterLicenses("")
                     },
                     onListLicenseFailed: function() {
                         this.loading = !1
                     }
                 }
             },
-            yt = gt,
-            xt = Object(I["a"])(yt, vt, bt, !1, null, null, null),
-            wt = xt.exports,
-            _t = function() {
+            _t = jt,
+            Pt = Object(D["a"])(_t, xt, wt, !1, null, null, null),
+            $t = Pt.exports,
+            kt = function() {
                 var e = this,
                     t = e._self._c;
                 return t("div", {
                     staticClass: "el-input-group el-input-group--prepend"
-                }, [t("div", {
+                }, [e.advanced || e.$root.v8mode ? e._e() : t("div", {
                     staticClass: "el-input-group__prepend"
                 }, [t("el-select", {
                     staticStyle: {
                         width: "160px"
                     },
                     attrs: {
                         disabled: e.advanced || e.$root.v8mode
@@ -4663,16 +4910,16 @@
                         callback: function(t) {
                             e.value = t
                         },
                         expression: "value"
                     }
                 })], 1)
             },
-            $t = [],
-            jt = {
+            It = [],
+            Ct = {
                 name: "SelectPlatform",
                 model: {
                     prop: "value2",
                     event: "change2"
                 },
                 props: {
                     value2: Array,
@@ -4682,15 +4929,15 @@
                 },
                 data: function() {
                     return {
                         level: this.value2.length && ".0" === this.value2[0][1].slice(-2) ? 1 : 0,
                         value: this.value2,
                         platforms: [
                             [{
-                                value: x("Common"),
+                                value: P("Common"),
                                 children: [{
                                     value: "windows.x86_64.7"
                                 }, {
                                     value: "linux.x86_64.7"
                                 }, {
                                     value: "darwin.x86_64.7"
                                 }, {
@@ -4706,28 +4953,28 @@
                                     value: "linux.armv7.3"
                                 }, {
                                     value: "linux.aarch32.3"
                                 }, {
                                     value: "linux.aarch64.3"
                                 }]
                             }, {
-                                value: x("Others"),
+                                value: P("Others"),
                                 children: [{
                                     value: "centos6.x86_64.7"
                                 }]
                             }, {
-                                value: x("VM Protection"),
+                                value: P("VM Protection"),
                                 children: [{
                                     value: "windows.x86_64.25"
                                 }, {
                                     value: "windows.x86.25"
                                 }]
                             }],
                             [{
-                                value: x("Common"),
+                                value: P("Common"),
                                 children: [{
                                     value: "windows.x86_64.0"
                                 }, {
                                     value: "linux.x86_64.0"
                                 }, {
                                     value: "darwin.x86_64.0"
                                 }, {
@@ -4755,15 +5002,15 @@
                                     value: "uclibc.armv7.0"
                                 }, {
                                     value: "android.aarch64.0"
                                 }, {
                                     value: "android.armv7.0"
                                 }]
                             }, {
-                                value: x("Others"),
+                                value: P("Others"),
                                 children: [{
                                     value: "vs2015.x86_64.0"
                                 }, {
                                     value: "vs2015.x86.0"
                                 }, {
                                     value: "musl.x86_64.0"
                                 }, {
@@ -4783,41 +5030,61 @@
                                 }, {
                                     value: "linux.mips64el.0"
                                 }]
                             }]
                         ],
                         platforms8: [
                             [{
-                                value: x("Common"),
+                                value: P("Common"),
                                 children: [{
                                     value: "windows.x86_64"
                                 }, {
-                                    value: "linux.x86_64"
+                                    value: "windows.x86"
                                 }, {
                                     value: "darwin.x86_64"
                                 }, {
-                                    value: "windows.x86"
+                                    value: "darwin.arm64"
+                                }, {
+                                    value: "linux.x86_64"
+                                }, {
+                                    value: "linux.aarch64"
+                                }, {
+                                    value: "linux.armv7"
                                 }, {
                                     value: "linux.x86"
                                 }]
                             }, {
-                                value: "arm",
+                                value: "Android",
                                 children: [{
-                                    value: "darwin.aarch64"
+                                    value: "android.x86_64"
                                 }, {
-                                    value: "linux.armv7"
+                                    value: "android.x86"
                                 }, {
-                                    value: "linux.aarch64"
+                                    value: "android.aarch64"
+                                }, {
+                                    value: "android.armv7"
                                 }]
                             }, {
-                                value: x("Themida Protection"),
+                                value: "Alpine Linux",
                                 children: [{
-                                    value: "windows.x86_64"
+                                    value: "alpine.x86_64"
                                 }, {
-                                    value: "windows.x86"
+                                    value: "alpine.aarch64"
+                                }]
+                            }, {
+                                value: "FreeBSD",
+                                children: [{
+                                    value: "freebsd.x86_64"
+                                }]
+                            }, {
+                                value: P("Themida Protection"),
+                                children: [{
+                                    value: "themida.x86_64"
+                                }, {
+                                    value: "themida.x86"
                                 }]
                             }]
                         ]
                     }
                 },
                 methods: {
                     onValueChanged: function(e) {
@@ -4827,176 +5094,179 @@
                 mounted: function() {
                     var e = this;
                     this.$watch("advanced", (function(t) {
                         t && 1 === e.level && (e.level = 0, e.value = [])
                     }))
                 }
             },
-            Pt = jt,
-            kt = Object(I["a"])(Pt, _t, $t, !1, null, null, null),
-            It = kt.exports,
-            Ct = (a("0fb7"), a("450d"), a("f529")),
-            St = a.n(Ct),
-            Dt = (a("9e1f"), a("6ed5")),
-            Ot = a.n(Dt),
-            Mt = (a("be4f"), a("896a")),
-            Rt = a.n(Mt),
-            Nt = (a("bc1c"), a("4726")),
-            Tt = a.n(Nt),
-            Et = (a("f92a"), a("d775")),
-            qt = a.n(Et),
-            Lt = (a("e3ea"), a("7bc3")),
-            Ft = a.n(Lt),
-            At = (a("fd71"), a("a447")),
-            zt = a.n(At),
-            Ht = (a("920a"), a("4f0c")),
-            Bt = a.n(Ht),
-            Vt = (a("bdc7"), a("aa2f")),
-            Ut = a.n(Vt),
-            Wt = (a("de31"), a("c69e")),
-            Xt = a.n(Wt),
-            Gt = (a("a769"), a("5cc3")),
-            Jt = a.n(Gt),
-            Qt = (a("a673"), a("7b31")),
-            Kt = a.n(Qt),
-            Zt = (a("adec"), a("3d2d")),
-            Yt = a.n(Zt),
-            ea = (a("28b2"), a("c7ad")),
-            ta = a.n(ea),
-            aa = (a("b0ee"), a("d180")),
-            oa = a.n(aa),
-            ra = (a("a335"), a("c0bb")),
-            na = a.n(ra),
-            sa = (a("9c49"), a("6640")),
-            ia = a.n(sa),
-            la = (a("d2ac"), a("95b0")),
-            ca = a.n(la),
-            ua = (a("b8e0"), a("a4c4")),
-            pa = a.n(ua),
-            da = (a("e2f3"), a("06f9")),
-            fa = a.n(da),
-            ha = (a("f225"), a("89a9")),
-            ma = a.n(ha),
-            va = (a("f4f9"), a("c2cc")),
-            ba = a.n(va),
-            ga = (a("7a0f"), a("0f6c")),
-            ya = a.n(ga),
-            xa = (a("cbb5"), a("8bbc")),
-            wa = a.n(xa),
-            _a = (a("e612"), a("dd87")),
-            $a = a.n(_a),
-            ja = (a("075a"), a("72aa")),
-            Pa = a.n(ja),
-            ka = (a("eca7"), a("3787")),
-            Ia = a.n(ka),
-            Ca = (a("425f"), a("4105")),
-            Sa = a.n(Ca),
-            Da = (a("b84d"), a("c216")),
-            Oa = a.n(Da),
-            Ma = (a("8f24"), a("76b9")),
-            Ra = a.n(Ma),
-            Na = (a("826b"), a("c263")),
-            Ta = a.n(Na),
-            Ea = (a("5466"), a("ecdf")),
-            qa = a.n(Ea),
-            La = (a("38a0"), a("ad41")),
-            Fa = a.n(La),
-            Aa = (a("ae26"), a("845f")),
-            za = a.n(Aa),
-            Ha = (a("1951"), a("eedf")),
-            Ba = a.n(Ha),
-            Va = (a("016f"), a("486c")),
-            Ua = a.n(Va),
-            Wa = (a("6611"), a("e772")),
-            Xa = a.n(Wa),
-            Ga = (a("1f1a"), a("4e4b")),
-            Ja = a.n(Ga),
-            Qa = (a("e960"), a("b35b")),
-            Ka = a.n(Qa),
-            Za = (a("d4df"), a("7fc1")),
-            Ya = a.n(Za),
-            eo = (a("c526"), a("1599")),
-            to = a.n(eo),
-            ao = (a("560b"), a("dcdc")),
-            oo = a.n(ao),
-            ro = (a("3c52"), a("0d7b")),
-            no = a.n(ro),
-            so = (a("fe07"), a("6ac5")),
-            io = a.n(so),
-            lo = (a("b5d8"), a("f494")),
-            co = a.n(lo),
-            uo = (a("9d4c"), a("e450")),
-            po = a.n(uo),
-            fo = (a("10cb"), a("f3ad")),
-            ho = a.n(fo),
-            mo = (a("34db"), a("3803")),
-            vo = a.n(mo),
-            bo = (a("8bd8"), a("4cb2")),
-            go = a.n(bo),
-            yo = (a("ce18"), a("f58e")),
-            xo = a.n(yo),
-            wo = (a("4ca3"), a("443e")),
-            _o = a.n(wo),
-            $o = (a("bd49"), a("18ff")),
-            jo = a.n($o),
-            Po = (a("960d"), a("defb")),
-            ko = a.n(Po),
-            Io = (a("cb70"), a("b370")),
-            Co = a.n(Io),
-            So = (a("a7cc"), a("df33")),
-            Do = a.n(So);
-        p.a.use(f.a), o["default"].use(Do.a), o["default"].use(Co.a), o["default"].use(ko.a), o["default"].use(jo.a), o["default"].use(_o.a), o["default"].use(xo.a), o["default"].use(go.a), o["default"].use(vo.a), o["default"].use(ho.a), o["default"].use(po.a), o["default"].use(co.a), o["default"].use(io.a), o["default"].use(no.a), o["default"].use(oo.a), o["default"].use(to.a), o["default"].use(Ya.a), o["default"].use(Ka.a), o["default"].use(Ja.a), o["default"].use(Xa.a), o["default"].use(Ua.a), o["default"].use(Ba.a), o["default"].use(za.a), o["default"].use(Fa.a), o["default"].use(qa.a), o["default"].use(Ta.a), o["default"].use(Ra.a), o["default"].use(Oa.a), o["default"].use(Sa.a), o["default"].use(Ia.a), o["default"].use(Pa.a), o["default"].use($a.a), o["default"].use(wa.a), o["default"].use(ya.a), o["default"].use(ba.a), o["default"].use(ma.a), o["default"].use(fa.a), o["default"].use(pa.a), o["default"].use(ca.a), o["default"].use(ia.a), o["default"].use(na.a), o["default"].use(oa.a), o["default"].use(ta.a), o["default"].use(Yt.a), o["default"].use(Kt.a), o["default"].use(Jt.a), o["default"].use(Xt.a), o["default"].use(Ut.a), o["default"].use(Bt.a), o["default"].use(zt.a), o["default"].use(Ft.a), o["default"].use(qt.a), o["default"].use(Tt.a), o["default"].prototype.$loading = Rt.a.service, o["default"].prototype.$msgbox = Ot.a, o["default"].prototype.$alert = Ot.a.alert, o["default"].prototype.$confirm = Ot.a.confirm, o["default"].prototype.$prompt = Ot.a.prompt, o["default"].prototype.$message = St.a, o["default"].use(y);
-        var Oo = {
-            "/": Ke
+            St = Ct,
+            Ot = Object(D["a"])(St, kt, It, !1, null, null, null),
+            Dt = Ot.exports,
+            Mt = (o("0fb7"), o("450d"), o("f529")),
+            Et = o.n(Mt),
+            Rt = (o("9e1f"), o("6ed5")),
+            Tt = o.n(Rt),
+            Nt = (o("be4f"), o("896a")),
+            qt = o.n(Nt),
+            Lt = (o("bc1c"), o("4726")),
+            At = o.n(Lt),
+            Ft = (o("f92a"), o("d775")),
+            zt = o.n(Ft),
+            Bt = (o("e3ea"), o("7bc3")),
+            Ht = o.n(Bt),
+            Vt = (o("fd71"), o("a447")),
+            Wt = o.n(Vt),
+            Ut = (o("920a"), o("4f0c")),
+            Gt = o.n(Ut),
+            Xt = (o("bdc7"), o("aa2f")),
+            Jt = o.n(Xt),
+            Qt = (o("de31"), o("c69e")),
+            Kt = o.n(Qt),
+            Zt = (o("a769"), o("5cc3")),
+            Yt = o.n(Zt),
+            eo = (o("a673"), o("7b31")),
+            to = o.n(eo),
+            oo = (o("adec"), o("3d2d")),
+            ao = o.n(oo),
+            ro = (o("28b2"), o("c7ad")),
+            no = o.n(ro),
+            so = (o("b0ee"), o("d180")),
+            io = o.n(so),
+            lo = (o("a335"), o("c0bb")),
+            co = o.n(lo),
+            uo = (o("9c49"), o("6640")),
+            po = o.n(uo),
+            fo = (o("d2ac"), o("95b0")),
+            ho = o.n(fo),
+            mo = (o("b8e0"), o("a4c4")),
+            vo = o.n(mo),
+            bo = (o("e2f3"), o("06f9")),
+            go = o.n(bo),
+            yo = (o("f225"), o("89a9")),
+            xo = o.n(yo),
+            wo = (o("f4f9"), o("c2cc")),
+            jo = o.n(wo),
+            _o = (o("7a0f"), o("0f6c")),
+            Po = o.n(_o),
+            $o = (o("cbb5"), o("8bbc")),
+            ko = o.n($o),
+            Io = (o("e612"), o("dd87")),
+            Co = o.n(Io),
+            So = (o("075a"), o("72aa")),
+            Oo = o.n(So),
+            Do = (o("eca7"), o("3787")),
+            Mo = o.n(Do),
+            Eo = (o("425f"), o("4105")),
+            Ro = o.n(Eo),
+            To = (o("b84d"), o("c216")),
+            No = o.n(To),
+            qo = (o("8f24"), o("76b9")),
+            Lo = o.n(qo),
+            Ao = (o("826b"), o("c263")),
+            Fo = o.n(Ao),
+            zo = (o("5466"), o("ecdf")),
+            Bo = o.n(zo),
+            Ho = (o("38a0"), o("ad41")),
+            Vo = o.n(Ho),
+            Wo = (o("ae26"), o("845f")),
+            Uo = o.n(Wo),
+            Go = (o("1951"), o("eedf")),
+            Xo = o.n(Go),
+            Jo = (o("016f"), o("486c")),
+            Qo = o.n(Jo),
+            Ko = (o("6611"), o("e772")),
+            Zo = o.n(Ko),
+            Yo = (o("1f1a"), o("4e4b")),
+            ea = o.n(Yo),
+            ta = (o("e960"), o("b35b")),
+            oa = o.n(ta),
+            aa = (o("d4df"), o("7fc1")),
+            ra = o.n(aa),
+            na = (o("c526"), o("1599")),
+            sa = o.n(na),
+            ia = (o("560b"), o("dcdc")),
+            la = o.n(ia),
+            ca = (o("3c52"), o("0d7b")),
+            ua = o.n(ca),
+            pa = (o("fe07"), o("6ac5")),
+            da = o.n(pa),
+            fa = (o("b5d8"), o("f494")),
+            ha = o.n(fa),
+            ma = (o("9d4c"), o("e450")),
+            va = o.n(ma),
+            ba = (o("10cb"), o("f3ad")),
+            ga = o.n(ba),
+            ya = (o("34db"), o("3803")),
+            xa = o.n(ya),
+            wa = (o("8bd8"), o("4cb2")),
+            ja = o.n(wa),
+            _a = (o("ce18"), o("f58e")),
+            Pa = o.n(_a),
+            $a = (o("4ca3"), o("443e")),
+            ka = o.n($a),
+            Ia = (o("bd49"), o("18ff")),
+            Ca = o.n(Ia),
+            Sa = (o("960d"), o("defb")),
+            Oa = o.n(Sa),
+            Da = (o("cb70"), o("b370")),
+            Ma = o.n(Da),
+            Ea = (o("a7cc"), o("df33")),
+            Ra = o.n(Ea);
+        p.a.use(f.a), a["default"].use(Ra.a), a["default"].use(Ma.a), a["default"].use(Oa.a), a["default"].use(Ca.a), a["default"].use(ka.a), a["default"].use(Pa.a), a["default"].use(ja.a), a["default"].use(xa.a), a["default"].use(ga.a), a["default"].use(va.a), a["default"].use(ha.a), a["default"].use(da.a), a["default"].use(ua.a), a["default"].use(la.a), a["default"].use(sa.a), a["default"].use(ra.a), a["default"].use(oa.a), a["default"].use(ea.a), a["default"].use(Zo.a), a["default"].use(Qo.a), a["default"].use(Xo.a), a["default"].use(Uo.a), a["default"].use(Vo.a), a["default"].use(Bo.a), a["default"].use(Fo.a), a["default"].use(Lo.a), a["default"].use(No.a), a["default"].use(Ro.a), a["default"].use(Mo.a), a["default"].use(Oo.a), a["default"].use(Co.a), a["default"].use(ko.a), a["default"].use(Po.a), a["default"].use(jo.a), a["default"].use(xo.a), a["default"].use(go.a), a["default"].use(vo.a), a["default"].use(ho.a), a["default"].use(po.a), a["default"].use(co.a), a["default"].use(io.a), a["default"].use(no.a), a["default"].use(ao.a), a["default"].use(to.a), a["default"].use(Yt.a), a["default"].use(Kt.a), a["default"].use(Jt.a), a["default"].use(Gt.a), a["default"].use(Wt.a), a["default"].use(Ht.a), a["default"].use(zt.a), a["default"].use(At.a), a["default"].prototype.$loading = qt.a.service, a["default"].prototype.$msgbox = Tt.a, a["default"].prototype.$alert = Tt.a.alert, a["default"].prototype.$confirm = Tt.a.confirm, a["default"].prototype.$prompt = Tt.a.prompt, a["default"].prototype.$message = Et.a, a["default"].use(_);
+        var Ta = {
+            "/": tt
         };
-        o["default"].config.productionTip = !1, o["default"].component("select-folder", ct), o["default"].component("select-path-script", mt), o["default"].component("select-license-file", wt), o["default"].component("select-platform", It), new o["default"]({
+        a["default"].config.productionTip = !1, a["default"].component("select-folder", ft), a["default"].component("select-path-script", yt), a["default"].component("select-license-file", $t), a["default"].component("select-platform", Dt), new a["default"]({
             data: {
                 currentRoute: window.location.pathname
             },
             computed: {
                 ViewComponent: function() {
-                    return Oo[this.currentRoute] || ot
+                    return Ta[this.currentRoute] || it
                 }
             },
             render: function(e) {
                 return e(this.ViewComponent)
             }
         }).$mount("#app")
     },
-    "586c": function(e, t, a) {
+    "586c": function(e, t, o) {
+        "use strict";
+        o("c504")
+    },
+    "58be": function(e, t, o) {},
+    "59cf": function(e, t, o) {
         "use strict";
-        a("c504")
+        o("0c06")
     },
-    "58be": function(e, t, a) {},
-    "592d": function(e, t, a) {
+    "59d9": function(e, t, o) {
         "use strict";
-        a("ea54")
+        o("d630")
     },
-    "59cf": function(e, t, a) {
+    "5bb9": function(e, t, o) {
         "use strict";
-        a("0c06")
+        o("103e")
     },
-    "59d9": function(e, t, a) {
+    7458: function(e, t, o) {},
+    8748: function(e, t, o) {},
+    "8d33": function(e, t, o) {},
+    "8e6f": function(e, t, o) {
         "use strict";
-        a("d630")
+        o("0de2")
     },
-    7458: function(e, t, a) {},
-    "7d43": function(e, t, a) {
+    a764: function(e, t, o) {
         "use strict";
-        a("073e")
+        o("8d33")
     },
-    "8d33": function(e, t, a) {},
-    a764: function(e, t, a) {
+    a7a7: function(e, t, o) {},
+    baa0: function(e, t, o) {
         "use strict";
-        a("8d33")
+        o("8748")
     },
-    a7a7: function(e, t, a) {},
-    c3c3: function(e, t, a) {},
-    c504: function(e, t, a) {},
-    cf05: function(e, t, a) {
-        e.exports = a.p + "img/logo.a8954ff0.png"
+    c504: function(e, t, o) {},
+    cf05: function(e, t, o) {
+        e.exports = o.p + "img/logo.a8954ff0.png"
     },
-    d630: function(e, t, a) {},
-    e2d0: function(e, t, a) {},
-    ea54: function(e, t, a) {}
+    d630: function(e, t, o) {},
+    e2d0: function(e, t, o) {}
 });
-//# sourceMappingURL=app.8da2b1ed.js.map
+//# sourceMappingURL=app.d802fb34.js.map
```

## Comparing `pyarmor-webui-2.0/static/img/cog.svg` & `pyarmor-webui-2.1/static/img/cog.svg`

 * *Files identical despite different names*

## Comparing `pyarmor-webui-2.0/static/img/calendar-alt.svg` & `pyarmor-webui-2.1/static/img/calendar-alt.svg`

 * *Files identical despite different names*

## Comparing `pyarmor-webui-2.0/static/img/logo.a8954ff0.png` & `pyarmor-webui-2.1/static/img/logo.a8954ff0.png`

 * *Files identical despite different names*

## Comparing `pyarmor-webui-2.0/static/img/registered.svg` & `pyarmor-webui-2.1/static/img/registered.svg`

 * *Files identical despite different names*

## Comparing `pyarmor-webui-2.0/static/fonts/element-icons.535877f5.woff` & `pyarmor-webui-2.1/static/fonts/element-icons.535877f5.woff`

 * *Files identical despite different names*

## Comparing `pyarmor-webui-2.0/static/fonts/element-icons.732389de.ttf` & `pyarmor-webui-2.1/static/fonts/element-icons.732389de.ttf`

 * *Files identical despite different names*

