# Comparing `tmp/automation_file-0.0.5.tar.gz` & `tmp/automation_file-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automation_file-0.0.5.tar", last modified: Thu Jun  8 08:54:28 2023, max compression
+gzip compressed data, was "automation_file-0.0.6.tar", last modified: Fri Jun  9 05:46:25 2023, max compression
```

## Comparing `automation_file-0.0.5.tar` & `automation_file-0.0.6.tar`

### file list

```diff
@@ -1,57 +1,69 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 08:54:28.567284 automation_file-0.0.5/
--rw-rw-rw-   0        0        0     1085 2023-05-18 06:36:21.000000 automation_file-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     1302 2023-06-08 08:54:28.565863 automation_file-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      679 2023-05-30 06:22:36.000000 automation_file-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-08 08:54:28.441870 automation_file-0.0.5/automation_file.egg-info/
--rw-rw-rw-   0        0        0     1302 2023-06-08 08:54:28.000000 automation_file-0.0.5/automation_file.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1618 2023-06-08 08:54:28.000000 automation_file-0.0.5/automation_file.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 08:54:28.000000 automation_file-0.0.5/automation_file.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       79 2023-06-08 08:54:28.000000 automation_file-0.0.5/automation_file.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-08 08:54:28.000000 automation_file-0.0.5/automation_file.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-08 08:54:28.446410 automation_file-0.0.5/file_automation/
--rw-rw-rw-   0        0        0     1835 2023-06-08 08:50:54.000000 automation_file-0.0.5/file_automation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-08 08:54:28.449410 automation_file-0.0.5/file_automation/local/
--rw-rw-rw-   0        0        0        0 2023-05-29 02:05:02.000000 automation_file-0.0.5/file_automation/local/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-08 08:54:28.459905 automation_file-0.0.5/file_automation/local/dir/
--rw-rw-rw-   0        0        0        0 2023-05-18 06:38:51.000000 automation_file-0.0.5/file_automation/local/dir/__init__.py
--rw-rw-rw-   0        0        0     2135 2023-06-08 06:26:10.000000 automation_file-0.0.5/file_automation/local/dir/dir_process.py
-drwxrwxrwx   0        0        0        0 2023-06-08 08:54:28.467459 automation_file-0.0.5/file_automation/local/file/
--rw-rw-rw-   0        0        0        0 2023-05-18 06:38:46.000000 automation_file-0.0.5/file_automation/local/file/__init__.py
--rw-rw-rw-   0        0        0     3716 2023-06-08 06:40:19.000000 automation_file-0.0.5/file_automation/local/file/file_process.py
-drwxrwxrwx   0        0        0        0 2023-06-08 08:54:28.478551 automation_file-0.0.5/file_automation/local/zip/
--rw-rw-rw-   0        0        0        0 2023-05-19 07:24:05.000000 automation_file-0.0.5/file_automation/local/zip/__init__.py
--rw-rw-rw-   0        0        0     3626 2023-06-08 07:15:08.000000 automation_file-0.0.5/file_automation/local/zip/zip_process.py
-drwxrwxrwx   0        0        0        0 2023-06-08 08:54:28.480550 automation_file-0.0.5/file_automation/remote/
--rw-rw-rw-   0        0        0        0 2023-05-29 02:05:15.000000 automation_file-0.0.5/file_automation/remote/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-08 08:54:28.490804 automation_file-0.0.5/file_automation/remote/google_drive/
--rw-rw-rw-   0        0        0        0 2023-05-29 02:05:24.000000 automation_file-0.0.5/file_automation/remote/google_drive/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-08 08:54:28.497906 automation_file-0.0.5/file_automation/remote/google_drive/delete/
--rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file-0.0.5/file_automation/remote/google_drive/delete/__init__.py
--rw-rw-rw-   0        0        0      648 2023-06-08 07:37:31.000000 automation_file-0.0.5/file_automation/remote/google_drive/delete/delete_manager.py
-drwxrwxrwx   0        0        0        0 2023-06-08 08:54:28.508711 automation_file-0.0.5/file_automation/remote/google_drive/dir/
--rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file-0.0.5/file_automation/remote/google_drive/dir/__init__.py
--rw-rw-rw-   0        0        0      876 2023-06-08 07:41:43.000000 automation_file-0.0.5/file_automation/remote/google_drive/dir/folder_manager.py
-drwxrwxrwx   0        0        0        0 2023-06-08 08:54:28.515735 automation_file-0.0.5/file_automation/remote/google_drive/download/
--rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file-0.0.5/file_automation/remote/google_drive/download/__init__.py
--rw-rw-rw-   0        0        0     2139 2023-06-08 07:46:57.000000 automation_file-0.0.5/file_automation/remote/google_drive/download/download_file.py
--rw-rw-rw-   0        0        0     2153 2023-06-08 08:45:58.000000 automation_file-0.0.5/file_automation/remote/google_drive/driver_instance.py
-drwxrwxrwx   0        0        0        0 2023-06-08 08:54:28.525374 automation_file-0.0.5/file_automation/remote/google_drive/search/
--rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file-0.0.5/file_automation/remote/google_drive/search/__init__.py
--rw-rw-rw-   0        0        0     2308 2023-06-08 07:49:23.000000 automation_file-0.0.5/file_automation/remote/google_drive/search/search_drive.py
-drwxrwxrwx   0        0        0        0 2023-06-08 08:54:28.532884 automation_file-0.0.5/file_automation/remote/google_drive/share/
--rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file-0.0.5/file_automation/remote/google_drive/share/__init__.py
--rw-rw-rw-   0        0        0     2524 2023-06-08 07:55:10.000000 automation_file-0.0.5/file_automation/remote/google_drive/share/share_file.py
-drwxrwxrwx   0        0        0        0 2023-06-08 08:54:28.542973 automation_file-0.0.5/file_automation/remote/google_drive/upload/
--rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file-0.0.5/file_automation/remote/google_drive/upload/__init__.py
--rw-rw-rw-   0        0        0     3823 2023-06-08 08:10:58.000000 automation_file-0.0.5/file_automation/remote/google_drive/upload/upload_to_driver.py
-drwxrwxrwx   0        0        0        0 2023-06-08 08:54:28.546227 automation_file-0.0.5/file_automation/utils/
--rw-rw-rw-   0        0        0        0 2023-05-18 07:59:01.000000 automation_file-0.0.5/file_automation/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-08 08:54:28.555910 automation_file-0.0.5/file_automation/utils/exception/
--rw-rw-rw-   0        0        0        0 2023-05-18 07:59:15.000000 automation_file-0.0.5/file_automation/utils/exception/__init__.py
--rw-rw-rw-   0        0        0       46 2023-06-05 01:25:46.000000 automation_file-0.0.5/file_automation/utils/exception/exception_tags.py
--rw-rw-rw-   0        0        0      165 2023-05-19 07:56:11.000000 automation_file-0.0.5/file_automation/utils/exception/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-06-08 08:54:28.562337 automation_file-0.0.5/file_automation/utils/logging/
--rw-rw-rw-   0        0        0        0 2023-06-08 03:44:59.000000 automation_file-0.0.5/file_automation/utils/logging/__init__.py
--rw-rw-rw-   0        0        0      372 2023-06-08 05:31:05.000000 automation_file-0.0.5/file_automation/utils/logging/loggin_instance.py
--rw-rw-rw-   0        0        0     1004 2023-06-08 08:54:08.000000 automation_file-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-08 08:54:28.568295 automation_file-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-09 05:46:25.792537 automation_file-0.0.6/
+-rw-rw-rw-   0        0        0     1085 2023-05-18 06:36:21.000000 automation_file-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     1302 2023-06-09 05:46:25.791539 automation_file-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      679 2023-05-30 06:22:36.000000 automation_file-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-09 05:46:25.645502 automation_file-0.0.6/automation_file.egg-info/
+-rw-rw-rw-   0        0        0     1302 2023-06-09 05:46:25.000000 automation_file-0.0.6/automation_file.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1992 2023-06-09 05:46:25.000000 automation_file-0.0.6/automation_file.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 05:46:25.000000 automation_file-0.0.6/automation_file.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       79 2023-06-09 05:46:25.000000 automation_file-0.0.6/automation_file.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-09 05:46:25.000000 automation_file-0.0.6/automation_file.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 05:46:25.650508 automation_file-0.0.6/file_automation/
+-rw-rw-rw-   0        0        0     1804 2023-06-08 09:31:05.000000 automation_file-0.0.6/file_automation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 05:46:25.653504 automation_file-0.0.6/file_automation/local/
+-rw-rw-rw-   0        0        0        0 2023-05-29 02:05:02.000000 automation_file-0.0.6/file_automation/local/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 05:46:25.660505 automation_file-0.0.6/file_automation/local/dir/
+-rw-rw-rw-   0        0        0        0 2023-05-18 06:38:51.000000 automation_file-0.0.6/file_automation/local/dir/__init__.py
+-rw-rw-rw-   0        0        0     2135 2023-06-08 06:26:10.000000 automation_file-0.0.6/file_automation/local/dir/dir_process.py
+drwxrwxrwx   0        0        0        0 2023-06-09 05:46:25.670613 automation_file-0.0.6/file_automation/local/file/
+-rw-rw-rw-   0        0        0        0 2023-05-18 06:38:46.000000 automation_file-0.0.6/file_automation/local/file/__init__.py
+-rw-rw-rw-   0        0        0     3716 2023-06-08 06:40:19.000000 automation_file-0.0.6/file_automation/local/file/file_process.py
+drwxrwxrwx   0        0        0        0 2023-06-09 05:46:25.678519 automation_file-0.0.6/file_automation/local/zip/
+-rw-rw-rw-   0        0        0        0 2023-05-19 07:24:05.000000 automation_file-0.0.6/file_automation/local/zip/__init__.py
+-rw-rw-rw-   0        0        0     3626 2023-06-08 07:15:08.000000 automation_file-0.0.6/file_automation/local/zip/zip_process.py
+drwxrwxrwx   0        0        0        0 2023-06-09 05:46:25.682525 automation_file-0.0.6/file_automation/remote/
+-rw-rw-rw-   0        0        0        0 2023-05-29 02:05:15.000000 automation_file-0.0.6/file_automation/remote/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 05:46:25.690523 automation_file-0.0.6/file_automation/remote/google_drive/
+-rw-rw-rw-   0        0        0        0 2023-05-29 02:05:24.000000 automation_file-0.0.6/file_automation/remote/google_drive/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 05:46:25.697100 automation_file-0.0.6/file_automation/remote/google_drive/delete/
+-rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file-0.0.6/file_automation/remote/google_drive/delete/__init__.py
+-rw-rw-rw-   0        0        0      648 2023-06-08 07:37:31.000000 automation_file-0.0.6/file_automation/remote/google_drive/delete/delete_manager.py
+drwxrwxrwx   0        0        0        0 2023-06-09 05:46:25.705069 automation_file-0.0.6/file_automation/remote/google_drive/dir/
+-rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file-0.0.6/file_automation/remote/google_drive/dir/__init__.py
+-rw-rw-rw-   0        0        0      876 2023-06-08 07:41:43.000000 automation_file-0.0.6/file_automation/remote/google_drive/dir/folder_manager.py
+drwxrwxrwx   0        0        0        0 2023-06-09 05:46:25.712107 automation_file-0.0.6/file_automation/remote/google_drive/download/
+-rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file-0.0.6/file_automation/remote/google_drive/download/__init__.py
+-rw-rw-rw-   0        0        0     2139 2023-06-08 07:46:57.000000 automation_file-0.0.6/file_automation/remote/google_drive/download/download_file.py
+-rw-rw-rw-   0        0        0     2153 2023-06-08 08:45:58.000000 automation_file-0.0.6/file_automation/remote/google_drive/driver_instance.py
+drwxrwxrwx   0        0        0        0 2023-06-09 05:46:25.719516 automation_file-0.0.6/file_automation/remote/google_drive/search/
+-rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file-0.0.6/file_automation/remote/google_drive/search/__init__.py
+-rw-rw-rw-   0        0        0     2308 2023-06-08 07:49:23.000000 automation_file-0.0.6/file_automation/remote/google_drive/search/search_drive.py
+drwxrwxrwx   0        0        0        0 2023-06-09 05:46:25.726118 automation_file-0.0.6/file_automation/remote/google_drive/share/
+-rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file-0.0.6/file_automation/remote/google_drive/share/__init__.py
+-rw-rw-rw-   0        0        0     2524 2023-06-08 07:55:10.000000 automation_file-0.0.6/file_automation/remote/google_drive/share/share_file.py
+drwxrwxrwx   0        0        0        0 2023-06-09 05:46:25.733042 automation_file-0.0.6/file_automation/remote/google_drive/upload/
+-rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file-0.0.6/file_automation/remote/google_drive/upload/__init__.py
+-rw-rw-rw-   0        0        0     3823 2023-06-08 08:10:58.000000 automation_file-0.0.6/file_automation/remote/google_drive/upload/upload_to_driver.py
+drwxrwxrwx   0        0        0        0 2023-06-09 05:46:25.738710 automation_file-0.0.6/file_automation/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-18 07:59:01.000000 automation_file-0.0.6/file_automation/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 05:46:25.745761 automation_file-0.0.6/file_automation/utils/callback/
+-rw-rw-rw-   0        0        0        0 2023-03-31 01:55:17.000000 automation_file-0.0.6/file_automation/utils/callback/__init__.py
+-rw-rw-rw-   0        0        0     4679 2023-06-09 03:57:57.000000 automation_file-0.0.6/file_automation/utils/callback/callback_function_executor.py
+drwxrwxrwx   0        0        0        0 2023-06-09 05:46:25.757215 automation_file-0.0.6/file_automation/utils/exception/
+-rw-rw-rw-   0        0        0        0 2023-05-18 07:59:15.000000 automation_file-0.0.6/file_automation/utils/exception/__init__.py
+-rw-rw-rw-   0        0        0      726 2023-06-08 09:16:50.000000 automation_file-0.0.6/file_automation/utils/exception/exception_tags.py
+-rw-rw-rw-   0        0        0      541 2023-06-08 09:16:50.000000 automation_file-0.0.6/file_automation/utils/exception/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-06-09 05:46:25.765132 automation_file-0.0.6/file_automation/utils/executor/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 automation_file-0.0.6/file_automation/utils/executor/__init__.py
+-rw-rw-rw-   0        0        0     6396 2023-06-09 03:57:57.000000 automation_file-0.0.6/file_automation/utils/executor/action_executor.py
+drwxrwxrwx   0        0        0        0 2023-06-09 05:46:25.773208 automation_file-0.0.6/file_automation/utils/json/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 automation_file-0.0.6/file_automation/utils/json/__init__.py
+-rw-rw-rw-   0        0        0     1299 2023-06-08 09:16:50.000000 automation_file-0.0.6/file_automation/utils/json/json_file.py
+drwxrwxrwx   0        0        0        0 2023-06-09 05:46:25.780130 automation_file-0.0.6/file_automation/utils/logging/
+-rw-rw-rw-   0        0        0        0 2023-06-08 03:44:59.000000 automation_file-0.0.6/file_automation/utils/logging/__init__.py
+-rw-rw-rw-   0        0        0      372 2023-06-08 05:31:05.000000 automation_file-0.0.6/file_automation/utils/logging/loggin_instance.py
+drwxrwxrwx   0        0        0        0 2023-06-09 05:46:25.787568 automation_file-0.0.6/file_automation/utils/scheduler/
+-rw-rw-rw-   0        0        0        0 2023-05-31 01:17:46.000000 automation_file-0.0.6/file_automation/utils/scheduler/__init__.py
+-rw-rw-rw-   0        0        0     6250 2023-05-31 06:04:47.000000 automation_file-0.0.6/file_automation/utils/scheduler/extend_apscheduler.py
+-rw-rw-rw-   0        0        0     1004 2023-06-09 05:46:03.000000 automation_file-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-09 05:46:25.793539 automation_file-0.0.6/setup.cfg
```

### Comparing `automation_file-0.0.5/LICENSE` & `automation_file-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `automation_file-0.0.5/PKG-INFO` & `automation_file-0.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automation_file
-Version: 0.0.5
+Version: 0.0.6
 Author-email: JE-Chen <zenmailman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/JE-Chen/Integration-testing-environment
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: MacOS X
```

### Comparing `automation_file-0.0.5/README.md` & `automation_file-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `automation_file-0.0.5/automation_file.egg-info/PKG-INFO` & `automation_file-0.0.6/automation_file.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automation-file
-Version: 0.0.5
+Version: 0.0.6
 Author-email: JE-Chen <zenmailman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/JE-Chen/Integration-testing-environment
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: MacOS X
```

### Comparing `automation_file-0.0.5/automation_file.egg-info/SOURCES.txt` & `automation_file-0.0.6/automation_file.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -26,12 +26,20 @@
 file_automation/remote/google_drive/search/__init__.py
 file_automation/remote/google_drive/search/search_drive.py
 file_automation/remote/google_drive/share/__init__.py
 file_automation/remote/google_drive/share/share_file.py
 file_automation/remote/google_drive/upload/__init__.py
 file_automation/remote/google_drive/upload/upload_to_driver.py
 file_automation/utils/__init__.py
+file_automation/utils/callback/__init__.py
+file_automation/utils/callback/callback_function_executor.py
 file_automation/utils/exception/__init__.py
 file_automation/utils/exception/exception_tags.py
 file_automation/utils/exception/exceptions.py
+file_automation/utils/executor/__init__.py
+file_automation/utils/executor/action_executor.py
+file_automation/utils/json/__init__.py
+file_automation/utils/json/json_file.py
 file_automation/utils/logging/__init__.py
-file_automation/utils/logging/loggin_instance.py
+file_automation/utils/logging/loggin_instance.py
+file_automation/utils/scheduler/__init__.py
+file_automation/utils/scheduler/extend_apscheduler.py
```

### Comparing `automation_file-0.0.5/file_automation/__init__.py` & `automation_file-0.0.6/file_automation/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,14 @@
 from file_automation.remote.google_drive.share.share_file import \
     share_file_to_anyone, share_file_to_domain, share_file_to_user
 from file_automation.remote.google_drive.delete.delete_manager import delete_file
 from file_automation.remote.google_drive.download.download_file import download_file, download_file_from_folder
 
 __all__ = [
     "copy_file", "rename_file", "remove_file", "copy_all_file_to_dir", "copy_specify_extension_file",
-    "copy_dir", "create_dir", "copy_specify_extension_file", "remove_dir_tree",
-    "zip_dir", "zip_file", "zip_info", "zip_file_info", "set_zip_password", "unzip_file", "read_zip_file",
+    "copy_dir", "create_dir", "remove_dir_tree", "zip_dir", "zip_file", "zip_info",
+    "zip_file_info", "set_zip_password", "unzip_file", "read_zip_file",
     "unzip_all", "driver_instance", "search_all_file", "search_field", "search_file_mimetype",
     "upload_dir_to_folder", "upload_to_folder", "upload_dir_to_drive", "upload_to_drive",
     "add_folder", "share_file_to_anyone", "share_file_to_domain", "share_file_to_user",
     "delete_file", "download_file", "download_file_from_folder"
 ]
```

### Comparing `automation_file-0.0.5/file_automation/local/dir/dir_process.py` & `automation_file-0.0.6/file_automation/local/dir/dir_process.py`

 * *Files identical despite different names*

### Comparing `automation_file-0.0.5/file_automation/local/file/file_process.py` & `automation_file-0.0.6/file_automation/local/file/file_process.py`

 * *Files identical despite different names*

### Comparing `automation_file-0.0.5/file_automation/local/zip/zip_process.py` & `automation_file-0.0.6/file_automation/local/zip/zip_process.py`

 * *Files identical despite different names*

### Comparing `automation_file-0.0.5/file_automation/remote/google_drive/delete/delete_manager.py` & `automation_file-0.0.6/file_automation/remote/google_drive/delete/delete_manager.py`

 * *Files identical despite different names*

### Comparing `automation_file-0.0.5/file_automation/remote/google_drive/dir/folder_manager.py` & `automation_file-0.0.6/file_automation/remote/google_drive/dir/folder_manager.py`

 * *Files identical despite different names*

### Comparing `automation_file-0.0.5/file_automation/remote/google_drive/download/download_file.py` & `automation_file-0.0.6/file_automation/remote/google_drive/download/download_file.py`

 * *Files identical despite different names*

### Comparing `automation_file-0.0.5/file_automation/remote/google_drive/driver_instance.py` & `automation_file-0.0.6/file_automation/remote/google_drive/driver_instance.py`

 * *Files identical despite different names*

### Comparing `automation_file-0.0.5/file_automation/remote/google_drive/search/search_drive.py` & `automation_file-0.0.6/file_automation/remote/google_drive/search/search_drive.py`

 * *Files identical despite different names*

### Comparing `automation_file-0.0.5/file_automation/remote/google_drive/share/share_file.py` & `automation_file-0.0.6/file_automation/remote/google_drive/share/share_file.py`

 * *Files identical despite different names*

### Comparing `automation_file-0.0.5/file_automation/remote/google_drive/upload/upload_to_driver.py` & `automation_file-0.0.6/file_automation/remote/google_drive/upload/upload_to_driver.py`

 * *Files identical despite different names*

### Comparing `automation_file-0.0.5/pyproject.toml` & `automation_file-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # This is dev version
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "automation_file"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
     { name = "JE-Chen", email = "zenmailman@gmail.com" },
 ]
 description = ""
 readme = { file = "README.md", content-type = "text/markdown" }
 requires-python = ">=3.8"
 license = { text = "MIT" }
```

