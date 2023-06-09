# Comparing `tmp/automation_file_dev-0.0.6.tar.gz` & `tmp/automation_file_dev-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automation_file_dev-0.0.6.tar", last modified: Thu Jun  8 08:52:27 2023, max compression
+gzip compressed data, was "automation_file_dev-0.0.7.tar", last modified: Fri Jun  9 03:59:58 2023, max compression
```

## Comparing `automation_file_dev-0.0.6.tar` & `automation_file_dev-0.0.7.tar`

### file list

```diff
@@ -1,57 +1,69 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 08:52:27.878464 automation_file_dev-0.0.6/
--rw-rw-rw-   0        0        0     1085 2023-05-18 06:36:21.000000 automation_file_dev-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     1306 2023-06-08 08:52:27.877443 automation_file_dev-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      679 2023-05-30 06:22:36.000000 automation_file_dev-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-08 08:52:27.773573 automation_file_dev-0.0.6/automation_file_dev.egg-info/
--rw-rw-rw-   0        0        0     1306 2023-06-08 08:52:27.000000 automation_file_dev-0.0.6/automation_file_dev.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1638 2023-06-08 08:52:27.000000 automation_file_dev-0.0.6/automation_file_dev.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 08:52:27.000000 automation_file_dev-0.0.6/automation_file_dev.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       79 2023-06-08 08:52:27.000000 automation_file_dev-0.0.6/automation_file_dev.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-08 08:52:27.000000 automation_file_dev-0.0.6/automation_file_dev.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-08 08:52:27.777207 automation_file_dev-0.0.6/file_automation/
--rw-rw-rw-   0        0        0     1835 2023-06-08 08:50:54.000000 automation_file_dev-0.0.6/file_automation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-08 08:52:27.781738 automation_file_dev-0.0.6/file_automation/local/
--rw-rw-rw-   0        0        0        0 2023-05-29 02:05:02.000000 automation_file_dev-0.0.6/file_automation/local/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-08 08:52:27.789337 automation_file_dev-0.0.6/file_automation/local/dir/
--rw-rw-rw-   0        0        0        0 2023-05-18 06:38:51.000000 automation_file_dev-0.0.6/file_automation/local/dir/__init__.py
--rw-rw-rw-   0        0        0     2135 2023-06-08 06:26:10.000000 automation_file_dev-0.0.6/file_automation/local/dir/dir_process.py
-drwxrwxrwx   0        0        0        0 2023-06-08 08:52:27.795548 automation_file_dev-0.0.6/file_automation/local/file/
--rw-rw-rw-   0        0        0        0 2023-05-18 06:38:46.000000 automation_file_dev-0.0.6/file_automation/local/file/__init__.py
--rw-rw-rw-   0        0        0     3716 2023-06-08 06:40:19.000000 automation_file_dev-0.0.6/file_automation/local/file/file_process.py
-drwxrwxrwx   0        0        0        0 2023-06-08 08:52:27.802602 automation_file_dev-0.0.6/file_automation/local/zip/
--rw-rw-rw-   0        0        0        0 2023-05-19 07:24:05.000000 automation_file_dev-0.0.6/file_automation/local/zip/__init__.py
--rw-rw-rw-   0        0        0     3626 2023-06-08 07:15:08.000000 automation_file_dev-0.0.6/file_automation/local/zip/zip_process.py
-drwxrwxrwx   0        0        0        0 2023-06-08 08:52:27.804762 automation_file_dev-0.0.6/file_automation/remote/
--rw-rw-rw-   0        0        0        0 2023-05-29 02:05:15.000000 automation_file_dev-0.0.6/file_automation/remote/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-08 08:52:27.810499 automation_file_dev-0.0.6/file_automation/remote/google_drive/
--rw-rw-rw-   0        0        0        0 2023-05-29 02:05:24.000000 automation_file_dev-0.0.6/file_automation/remote/google_drive/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-08 08:52:27.816759 automation_file_dev-0.0.6/file_automation/remote/google_drive/delete/
--rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file_dev-0.0.6/file_automation/remote/google_drive/delete/__init__.py
--rw-rw-rw-   0        0        0      648 2023-06-08 07:37:31.000000 automation_file_dev-0.0.6/file_automation/remote/google_drive/delete/delete_manager.py
-drwxrwxrwx   0        0        0        0 2023-06-08 08:52:27.823659 automation_file_dev-0.0.6/file_automation/remote/google_drive/dir/
--rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file_dev-0.0.6/file_automation/remote/google_drive/dir/__init__.py
--rw-rw-rw-   0        0        0      876 2023-06-08 07:41:43.000000 automation_file_dev-0.0.6/file_automation/remote/google_drive/dir/folder_manager.py
-drwxrwxrwx   0        0        0        0 2023-06-08 08:52:27.832175 automation_file_dev-0.0.6/file_automation/remote/google_drive/download/
--rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file_dev-0.0.6/file_automation/remote/google_drive/download/__init__.py
--rw-rw-rw-   0        0        0     2139 2023-06-08 07:46:57.000000 automation_file_dev-0.0.6/file_automation/remote/google_drive/download/download_file.py
--rw-rw-rw-   0        0        0     2153 2023-06-08 08:45:58.000000 automation_file_dev-0.0.6/file_automation/remote/google_drive/driver_instance.py
-drwxrwxrwx   0        0        0        0 2023-06-08 08:52:27.839775 automation_file_dev-0.0.6/file_automation/remote/google_drive/search/
--rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file_dev-0.0.6/file_automation/remote/google_drive/search/__init__.py
--rw-rw-rw-   0        0        0     2308 2023-06-08 07:49:23.000000 automation_file_dev-0.0.6/file_automation/remote/google_drive/search/search_drive.py
-drwxrwxrwx   0        0        0        0 2023-06-08 08:52:27.846881 automation_file_dev-0.0.6/file_automation/remote/google_drive/share/
--rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file_dev-0.0.6/file_automation/remote/google_drive/share/__init__.py
--rw-rw-rw-   0        0        0     2524 2023-06-08 07:55:10.000000 automation_file_dev-0.0.6/file_automation/remote/google_drive/share/share_file.py
-drwxrwxrwx   0        0        0        0 2023-06-08 08:52:27.852923 automation_file_dev-0.0.6/file_automation/remote/google_drive/upload/
--rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file_dev-0.0.6/file_automation/remote/google_drive/upload/__init__.py
--rw-rw-rw-   0        0        0     3823 2023-06-08 08:10:58.000000 automation_file_dev-0.0.6/file_automation/remote/google_drive/upload/upload_to_driver.py
-drwxrwxrwx   0        0        0        0 2023-06-08 08:52:27.857236 automation_file_dev-0.0.6/file_automation/utils/
--rw-rw-rw-   0        0        0        0 2023-05-18 07:59:01.000000 automation_file_dev-0.0.6/file_automation/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-08 08:52:27.867623 automation_file_dev-0.0.6/file_automation/utils/exception/
--rw-rw-rw-   0        0        0        0 2023-05-18 07:59:15.000000 automation_file_dev-0.0.6/file_automation/utils/exception/__init__.py
--rw-rw-rw-   0        0        0       46 2023-06-05 01:25:46.000000 automation_file_dev-0.0.6/file_automation/utils/exception/exception_tags.py
--rw-rw-rw-   0        0        0      165 2023-05-19 07:56:11.000000 automation_file_dev-0.0.6/file_automation/utils/exception/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-06-08 08:52:27.874981 automation_file_dev-0.0.6/file_automation/utils/logging/
--rw-rw-rw-   0        0        0        0 2023-06-08 03:44:59.000000 automation_file_dev-0.0.6/file_automation/utils/logging/__init__.py
--rw-rw-rw-   0        0        0      372 2023-06-08 05:31:05.000000 automation_file_dev-0.0.6/file_automation/utils/logging/loggin_instance.py
--rw-rw-rw-   0        0        0     1008 2023-06-08 08:52:08.000000 automation_file_dev-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-08 08:52:27.879499 automation_file_dev-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-09 03:59:58.497772 automation_file_dev-0.0.7/
+-rw-rw-rw-   0        0        0     1085 2023-05-18 06:36:21.000000 automation_file_dev-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     1306 2023-06-09 03:59:58.496778 automation_file_dev-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      679 2023-05-30 06:22:36.000000 automation_file_dev-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-09 03:59:58.222350 automation_file_dev-0.0.7/automation_file_dev.egg-info/
+-rw-rw-rw-   0        0        0     1306 2023-06-09 03:59:58.000000 automation_file_dev-0.0.7/automation_file_dev.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2012 2023-06-09 03:59:58.000000 automation_file_dev-0.0.7/automation_file_dev.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 03:59:58.000000 automation_file_dev-0.0.7/automation_file_dev.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       79 2023-06-09 03:59:58.000000 automation_file_dev-0.0.7/automation_file_dev.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-09 03:59:58.000000 automation_file_dev-0.0.7/automation_file_dev.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 03:59:58.234372 automation_file_dev-0.0.7/file_automation/
+-rw-rw-rw-   0        0        0     1804 2023-06-08 09:31:05.000000 automation_file_dev-0.0.7/file_automation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 03:59:58.239369 automation_file_dev-0.0.7/file_automation/local/
+-rw-rw-rw-   0        0        0        0 2023-05-29 02:05:02.000000 automation_file_dev-0.0.7/file_automation/local/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 03:59:58.251374 automation_file_dev-0.0.7/file_automation/local/dir/
+-rw-rw-rw-   0        0        0        0 2023-05-18 06:38:51.000000 automation_file_dev-0.0.7/file_automation/local/dir/__init__.py
+-rw-rw-rw-   0        0        0     2135 2023-06-08 06:26:10.000000 automation_file_dev-0.0.7/file_automation/local/dir/dir_process.py
+drwxrwxrwx   0        0        0        0 2023-06-09 03:59:58.266027 automation_file_dev-0.0.7/file_automation/local/file/
+-rw-rw-rw-   0        0        0        0 2023-05-18 06:38:46.000000 automation_file_dev-0.0.7/file_automation/local/file/__init__.py
+-rw-rw-rw-   0        0        0     3716 2023-06-08 06:40:19.000000 automation_file_dev-0.0.7/file_automation/local/file/file_process.py
+drwxrwxrwx   0        0        0        0 2023-06-09 03:59:58.280993 automation_file_dev-0.0.7/file_automation/local/zip/
+-rw-rw-rw-   0        0        0        0 2023-05-19 07:24:05.000000 automation_file_dev-0.0.7/file_automation/local/zip/__init__.py
+-rw-rw-rw-   0        0        0     3626 2023-06-08 07:15:08.000000 automation_file_dev-0.0.7/file_automation/local/zip/zip_process.py
+drwxrwxrwx   0        0        0        0 2023-06-09 03:59:58.286447 automation_file_dev-0.0.7/file_automation/remote/
+-rw-rw-rw-   0        0        0        0 2023-05-29 02:05:15.000000 automation_file_dev-0.0.7/file_automation/remote/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 03:59:58.297843 automation_file_dev-0.0.7/file_automation/remote/google_drive/
+-rw-rw-rw-   0        0        0        0 2023-05-29 02:05:24.000000 automation_file_dev-0.0.7/file_automation/remote/google_drive/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 03:59:58.307351 automation_file_dev-0.0.7/file_automation/remote/google_drive/delete/
+-rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file_dev-0.0.7/file_automation/remote/google_drive/delete/__init__.py
+-rw-rw-rw-   0        0        0      648 2023-06-08 07:37:31.000000 automation_file_dev-0.0.7/file_automation/remote/google_drive/delete/delete_manager.py
+drwxrwxrwx   0        0        0        0 2023-06-09 03:59:58.320163 automation_file_dev-0.0.7/file_automation/remote/google_drive/dir/
+-rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file_dev-0.0.7/file_automation/remote/google_drive/dir/__init__.py
+-rw-rw-rw-   0        0        0      876 2023-06-08 07:41:43.000000 automation_file_dev-0.0.7/file_automation/remote/google_drive/dir/folder_manager.py
+drwxrwxrwx   0        0        0        0 2023-06-09 03:59:58.332163 automation_file_dev-0.0.7/file_automation/remote/google_drive/download/
+-rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file_dev-0.0.7/file_automation/remote/google_drive/download/__init__.py
+-rw-rw-rw-   0        0        0     2139 2023-06-08 07:46:57.000000 automation_file_dev-0.0.7/file_automation/remote/google_drive/download/download_file.py
+-rw-rw-rw-   0        0        0     2153 2023-06-08 08:45:58.000000 automation_file_dev-0.0.7/file_automation/remote/google_drive/driver_instance.py
+drwxrwxrwx   0        0        0        0 2023-06-09 03:59:58.345661 automation_file_dev-0.0.7/file_automation/remote/google_drive/search/
+-rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file_dev-0.0.7/file_automation/remote/google_drive/search/__init__.py
+-rw-rw-rw-   0        0        0     2308 2023-06-08 07:49:23.000000 automation_file_dev-0.0.7/file_automation/remote/google_drive/search/search_drive.py
+drwxrwxrwx   0        0        0        0 2023-06-09 03:59:58.359727 automation_file_dev-0.0.7/file_automation/remote/google_drive/share/
+-rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file_dev-0.0.7/file_automation/remote/google_drive/share/__init__.py
+-rw-rw-rw-   0        0        0     2524 2023-06-08 07:55:10.000000 automation_file_dev-0.0.7/file_automation/remote/google_drive/share/share_file.py
+drwxrwxrwx   0        0        0        0 2023-06-09 03:59:58.371732 automation_file_dev-0.0.7/file_automation/remote/google_drive/upload/
+-rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file_dev-0.0.7/file_automation/remote/google_drive/upload/__init__.py
+-rw-rw-rw-   0        0        0     3823 2023-06-08 08:10:58.000000 automation_file_dev-0.0.7/file_automation/remote/google_drive/upload/upload_to_driver.py
+drwxrwxrwx   0        0        0        0 2023-06-09 03:59:58.377642 automation_file_dev-0.0.7/file_automation/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-18 07:59:01.000000 automation_file_dev-0.0.7/file_automation/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 03:59:58.387084 automation_file_dev-0.0.7/file_automation/utils/callback/
+-rw-rw-rw-   0        0        0        0 2023-03-31 01:55:17.000000 automation_file_dev-0.0.7/file_automation/utils/callback/__init__.py
+-rw-rw-rw-   0        0        0     4679 2023-06-09 03:57:57.000000 automation_file_dev-0.0.7/file_automation/utils/callback/callback_function_executor.py
+drwxrwxrwx   0        0        0        0 2023-06-09 03:59:58.416934 automation_file_dev-0.0.7/file_automation/utils/exception/
+-rw-rw-rw-   0        0        0        0 2023-05-18 07:59:15.000000 automation_file_dev-0.0.7/file_automation/utils/exception/__init__.py
+-rw-rw-rw-   0        0        0      726 2023-06-08 09:16:50.000000 automation_file_dev-0.0.7/file_automation/utils/exception/exception_tags.py
+-rw-rw-rw-   0        0        0      541 2023-06-08 09:16:50.000000 automation_file_dev-0.0.7/file_automation/utils/exception/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-06-09 03:59:58.436299 automation_file_dev-0.0.7/file_automation/utils/executor/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 automation_file_dev-0.0.7/file_automation/utils/executor/__init__.py
+-rw-rw-rw-   0        0        0     6396 2023-06-09 03:57:57.000000 automation_file_dev-0.0.7/file_automation/utils/executor/action_executor.py
+drwxrwxrwx   0        0        0        0 2023-06-09 03:59:58.456850 automation_file_dev-0.0.7/file_automation/utils/json/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 automation_file_dev-0.0.7/file_automation/utils/json/__init__.py
+-rw-rw-rw-   0        0        0     1299 2023-06-08 09:16:50.000000 automation_file_dev-0.0.7/file_automation/utils/json/json_file.py
+drwxrwxrwx   0        0        0        0 2023-06-09 03:59:58.474202 automation_file_dev-0.0.7/file_automation/utils/logging/
+-rw-rw-rw-   0        0        0        0 2023-06-08 03:44:59.000000 automation_file_dev-0.0.7/file_automation/utils/logging/__init__.py
+-rw-rw-rw-   0        0        0      372 2023-06-08 05:31:05.000000 automation_file_dev-0.0.7/file_automation/utils/logging/loggin_instance.py
+drwxrwxrwx   0        0        0        0 2023-06-09 03:59:58.490770 automation_file_dev-0.0.7/file_automation/utils/scheduler/
+-rw-rw-rw-   0        0        0        0 2023-05-31 01:17:46.000000 automation_file_dev-0.0.7/file_automation/utils/scheduler/__init__.py
+-rw-rw-rw-   0        0        0     6250 2023-05-31 06:04:47.000000 automation_file_dev-0.0.7/file_automation/utils/scheduler/extend_apscheduler.py
+-rw-rw-rw-   0        0        0     1008 2023-06-09 03:59:33.000000 automation_file_dev-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-09 03:59:58.498773 automation_file_dev-0.0.7/setup.cfg
```

### Comparing `automation_file_dev-0.0.6/LICENSE` & `automation_file_dev-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `automation_file_dev-0.0.6/PKG-INFO` & `automation_file_dev-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automation_file_dev
-Version: 0.0.6
+Version: 0.0.7
 Author-email: JE-Chen <zenmailman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/JE-Chen/Integration-testing-environment
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: MacOS X
```

### Comparing `automation_file_dev-0.0.6/README.md` & `automation_file_dev-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `automation_file_dev-0.0.6/automation_file_dev.egg-info/PKG-INFO` & `automation_file_dev-0.0.7/automation_file_dev.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automation-file-dev
-Version: 0.0.6
+Version: 0.0.7
 Author-email: JE-Chen <zenmailman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/JE-Chen/Integration-testing-environment
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: MacOS X
```

### Comparing `automation_file_dev-0.0.6/automation_file_dev.egg-info/SOURCES.txt` & `automation_file_dev-0.0.7/automation_file_dev.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

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

### Comparing `automation_file_dev-0.0.6/file_automation/__init__.py` & `automation_file_dev-0.0.7/file_automation/__init__.py`

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

### Comparing `automation_file_dev-0.0.6/file_automation/local/dir/dir_process.py` & `automation_file_dev-0.0.7/file_automation/local/dir/dir_process.py`

 * *Files identical despite different names*

### Comparing `automation_file_dev-0.0.6/file_automation/local/file/file_process.py` & `automation_file_dev-0.0.7/file_automation/local/file/file_process.py`

 * *Files identical despite different names*

### Comparing `automation_file_dev-0.0.6/file_automation/local/zip/zip_process.py` & `automation_file_dev-0.0.7/file_automation/local/zip/zip_process.py`

 * *Files identical despite different names*

### Comparing `automation_file_dev-0.0.6/file_automation/remote/google_drive/delete/delete_manager.py` & `automation_file_dev-0.0.7/file_automation/remote/google_drive/delete/delete_manager.py`

 * *Files identical despite different names*

### Comparing `automation_file_dev-0.0.6/file_automation/remote/google_drive/dir/folder_manager.py` & `automation_file_dev-0.0.7/file_automation/remote/google_drive/dir/folder_manager.py`

 * *Files identical despite different names*

### Comparing `automation_file_dev-0.0.6/file_automation/remote/google_drive/download/download_file.py` & `automation_file_dev-0.0.7/file_automation/remote/google_drive/download/download_file.py`

 * *Files identical despite different names*

### Comparing `automation_file_dev-0.0.6/file_automation/remote/google_drive/driver_instance.py` & `automation_file_dev-0.0.7/file_automation/remote/google_drive/driver_instance.py`

 * *Files identical despite different names*

### Comparing `automation_file_dev-0.0.6/file_automation/remote/google_drive/search/search_drive.py` & `automation_file_dev-0.0.7/file_automation/remote/google_drive/search/search_drive.py`

 * *Files identical despite different names*

### Comparing `automation_file_dev-0.0.6/file_automation/remote/google_drive/share/share_file.py` & `automation_file_dev-0.0.7/file_automation/remote/google_drive/share/share_file.py`

 * *Files identical despite different names*

### Comparing `automation_file_dev-0.0.6/file_automation/remote/google_drive/upload/upload_to_driver.py` & `automation_file_dev-0.0.7/file_automation/remote/google_drive/upload/upload_to_driver.py`

 * *Files identical despite different names*

### Comparing `automation_file_dev-0.0.6/pyproject.toml` & `automation_file_dev-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # This is dev version
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "automation_file_dev"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
     { name = "JE-Chen", email = "zenmailman@gmail.com" },
 ]
 description = ""
 readme = { file = "README.md", content-type = "text/markdown" }
 requires-python = ">=3.8"
 license = { text = "MIT" }
```

