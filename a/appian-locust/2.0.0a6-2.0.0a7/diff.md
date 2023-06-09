# Comparing `tmp/appian-locust-2.0.0a6.tar.gz` & `tmp/appian-locust-2.0.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "appian-locust-2.0.0a6.tar", last modified: Thu Jun  8 19:11:07 2023, max compression
+gzip compressed data, was "appian-locust-2.0.0a7.tar", last modified: Fri Jun  9 16:15:02 2023, max compression
```

## Comparing `appian-locust-2.0.0a6.tar` & `appian-locust-2.0.0a7.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:11:07.367953 appian-locust-2.0.0a6/
--rw-rw-rw-   0 root         (0) root         (0)    11358 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5403 2023-06-08 19:11:07.367953 appian-locust-2.0.0a6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4829 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:11:07.366952 appian-locust-2.0.0a6/appian_locust/
--rw-rw-rw-   0 root         (0) root         (0)      775 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9573 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/_actions.py
--rw-rw-rw-   0 root         (0) root         (0)      786 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/_admin.py
--rw-rw-rw-   0 root         (0) root         (0)     2479 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/_base.py
--rw-rw-rw-   0 root         (0) root         (0)     6282 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/_design.py
--rw-rw-rw-   0 root         (0) root         (0)     6206 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/_feature_toggle_helper.py
--rw-rw-rw-   0 root         (0) root         (0)     7830 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/_grid_interactor.py
--rw-rw-rw-   0 root         (0) root         (0)    53252 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/_interactor.py
--rw-rw-rw-   0 root         (0) root         (0)     5171 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/_locust_error_handler.py
--rw-rw-rw-   0 root         (0) root         (0)     7789 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/_news.py
--rw-rw-rw-   0 root         (0) root         (0)     1025 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/_portals.py
--rw-rw-rw-   0 root         (0) root         (0)    16614 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/_records.py
--rw-rw-rw-   0 root         (0) root         (0)     7380 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/_records_helper.py
--rw-rw-rw-   0 root         (0) root         (0)     7464 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/_reports.py
--rw-rw-rw-   0 root         (0) root         (0)     3016 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/_save_request_builder.py
--rw-rw-rw-   0 root         (0) root         (0)     9934 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/_sites.py
--rw-rw-rw-   0 root         (0) root         (0)     4514 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/_task_opener.py
--rw-rw-rw-   0 root         (0) root         (0)     7644 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/_tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     2365 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/_ui_reconciler.py
--rw-rw-rw-   0 root         (0) root         (0)     1636 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/actions_info.py
--rw-rw-rw-   0 root         (0) root         (0)    14940 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/appianclient.py
--rw-rw-rw-   0 root         (0) root         (0)      354 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/application.py
--rw-rw-rw-   0 root         (0) root         (0)     3950 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/application_uiform.py
--rw-rw-rw-   0 root         (0) root         (0)      358 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/design_object.py
--rw-rw-rw-   0 root         (0) root         (0)      205 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/design_object_type.py
--rw-rw-rw-   0 root         (0) root         (0)     1068 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/design_object_uiform.py
--rw-rw-rw-   0 root         (0) root         (0)     6234 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/design_uiform.py
--rw-rw-rw-   0 root         (0) root         (0)      859 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1792 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/feature_flag.py
--rw-rw-rw-   0 root         (0) root         (0)    16346 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/helper.py
--rwxrwxrwx   0 root         (0) root         (0)     1431 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/loadDriverUtils.py
--rw-rw-rw-   0 root         (0) root         (0)      862 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/logger.py
--rw-rw-rw-   0 root         (0) root         (0)     4198 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/news_info.py
--rw-rw-rw-   0 root         (0) root         (0)     3051 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/record_list_uiform.py
--rw-rw-rw-   0 root         (0) root         (0)     1320 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/record_uiform.py
--rw-rw-rw-   0 root         (0) root         (0)      998 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/records_info.py
--rw-rw-rw-   0 root         (0) root         (0)     1712 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/reports_info.py
--rw-rw-rw-   0 root         (0) root         (0)     2104 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/site_helper.py
--rw-rw-rw-   0 root         (0) root         (0)      990 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/site_objects.py
--rw-rw-rw-   0 root         (0) root         (0)     1261 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/sites_info.py
--rw-rw-rw-   0 root         (0) root         (0)     1611 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/tasks_info.py
--rw-rw-rw-   0 root         (0) root         (0)     2211 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/tempo_navigator.py
--rw-rw-rw-   0 root         (0) root         (0)    73573 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/uiform.py
--rw-rw-rw-   0 root         (0) root         (0)    15051 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/visitor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:11:07.367953 appian-locust-2.0.0a6/appian_locust.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5403 2023-06-08 19:11:07.000000 appian-locust-2.0.0a6/appian_locust.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1521 2023-06-08 19:11:07.000000 appian-locust-2.0.0a6/appian_locust.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 19:11:07.000000 appian-locust-2.0.0a6/appian_locust.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-06-08 19:11:07.000000 appian-locust-2.0.0a6/appian_locust.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-06-08 19:11:07.000000 appian-locust-2.0.0a6/appian_locust.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      595 2023-06-08 19:11:07.368953 appian-locust-2.0.0a6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1088 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 16:15:02.535519 appian-locust-2.0.0a7/
+-rw-rw-rw-   0 root         (0) root         (0)    11358 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5403 2023-06-09 16:15:02.535519 appian-locust-2.0.0a7/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4829 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 16:15:02.534519 appian-locust-2.0.0a7/appian_locust/
+-rw-rw-rw-   0 root         (0) root         (0)      775 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9573 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/_actions.py
+-rw-rw-rw-   0 root         (0) root         (0)      786 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/_admin.py
+-rw-rw-rw-   0 root         (0) root         (0)     2479 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     6282 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/_design.py
+-rw-rw-rw-   0 root         (0) root         (0)     6206 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/_feature_toggle_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)     7830 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/_grid_interactor.py
+-rw-rw-rw-   0 root         (0) root         (0)    51994 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/_interactor.py
+-rw-rw-rw-   0 root         (0) root         (0)     5171 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/_locust_error_handler.py
+-rw-rw-rw-   0 root         (0) root         (0)     7789 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/_news.py
+-rw-rw-rw-   0 root         (0) root         (0)     1025 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/_portals.py
+-rw-rw-rw-   0 root         (0) root         (0)    16614 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/_records.py
+-rw-rw-rw-   0 root         (0) root         (0)     7380 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/_records_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)     7464 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/_reports.py
+-rw-rw-rw-   0 root         (0) root         (0)     3016 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/_save_request_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)     9934 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/_sites.py
+-rw-rw-rw-   0 root         (0) root         (0)     4514 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/_task_opener.py
+-rw-rw-rw-   0 root         (0) root         (0)     7644 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/_tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2365 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/_ui_reconciler.py
+-rw-rw-rw-   0 root         (0) root         (0)     1636 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/actions_info.py
+-rw-rw-rw-   0 root         (0) root         (0)    14940 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/appianclient.py
+-rw-rw-rw-   0 root         (0) root         (0)      354 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/application.py
+-rw-rw-rw-   0 root         (0) root         (0)     3950 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/application_uiform.py
+-rw-rw-rw-   0 root         (0) root         (0)      358 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/design_object.py
+-rw-rw-rw-   0 root         (0) root         (0)      205 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/design_object_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     1068 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/design_object_uiform.py
+-rw-rw-rw-   0 root         (0) root         (0)     6234 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/design_uiform.py
+-rw-rw-rw-   0 root         (0) root         (0)      859 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1792 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/feature_flag.py
+-rw-rw-rw-   0 root         (0) root         (0)    16346 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/helper.py
+-rwxrwxrwx   0 root         (0) root         (0)     1431 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/loadDriverUtils.py
+-rw-rw-rw-   0 root         (0) root         (0)      862 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/logger.py
+-rw-rw-rw-   0 root         (0) root         (0)     4198 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/news_info.py
+-rw-rw-rw-   0 root         (0) root         (0)     3051 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/record_list_uiform.py
+-rw-rw-rw-   0 root         (0) root         (0)     1320 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/record_uiform.py
+-rw-rw-rw-   0 root         (0) root         (0)      998 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/records_info.py
+-rw-rw-rw-   0 root         (0) root         (0)     1712 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/reports_info.py
+-rw-rw-rw-   0 root         (0) root         (0)     3311 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/site_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)      990 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/site_objects.py
+-rw-rw-rw-   0 root         (0) root         (0)     1261 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/sites_info.py
+-rw-rw-rw-   0 root         (0) root         (0)     1611 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/tasks_info.py
+-rw-rw-rw-   0 root         (0) root         (0)     2211 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/tempo_navigator.py
+-rw-rw-rw-   0 root         (0) root         (0)    73573 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/uiform.py
+-rw-rw-rw-   0 root         (0) root         (0)    15051 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/appian_locust/visitor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 16:15:02.535519 appian-locust-2.0.0a7/appian_locust.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5403 2023-06-09 16:15:02.000000 appian-locust-2.0.0a7/appian_locust.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1521 2023-06-09 16:15:02.000000 appian-locust-2.0.0a7/appian_locust.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 16:15:02.000000 appian-locust-2.0.0a7/appian_locust.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-06-09 16:15:02.000000 appian-locust-2.0.0a7/appian_locust.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-06-09 16:15:02.000000 appian-locust-2.0.0a7/appian_locust.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      595 2023-06-09 16:15:02.535519 appian-locust-2.0.0a7/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1088 2023-06-09 16:14:53.000000 appian-locust-2.0.0a7/setup.py
```

### Comparing `appian-locust-2.0.0a6/LICENSE` & `appian-locust-2.0.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a6/PKG-INFO` & `appian-locust-2.0.0a7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appian-locust
-Version: 2.0.0a6
+Version: 2.0.0a7
 Summary: Tools and functions to make testing Appian with Locust easier
 Home-page: https://gitlab.com/appian-oss/appian-locust
 Author: Appian Performance & Reliability Engineering Squad
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `appian-locust-2.0.0a6/README.rst` & `appian-locust-2.0.0a7/README.rst`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a6/appian_locust/__init__.py` & `appian-locust-2.0.0a7/appian_locust/__init__.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a6/appian_locust/_actions.py` & `appian-locust-2.0.0a7/appian_locust/_actions.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a6/appian_locust/_admin.py` & `appian-locust-2.0.0a7/appian_locust/_admin.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a6/appian_locust/_base.py` & `appian-locust-2.0.0a7/appian_locust/_base.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a6/appian_locust/_design.py` & `appian-locust-2.0.0a7/appian_locust/_design.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a6/appian_locust/_feature_toggle_helper.py` & `appian-locust-2.0.0a7/appian_locust/_feature_toggle_helper.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a6/appian_locust/_grid_interactor.py` & `appian-locust-2.0.0a7/appian_locust/_grid_interactor.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a6/appian_locust/_interactor.py` & `appian-locust-2.0.0a7/appian_locust/_interactor.py`

 * *Files 3% similar despite different names*

```diff
@@ -266,54 +266,23 @@
             if not self.portals_mode:
                 username = get_username(self.auth)
                 test_response_for_error(resp, uri, raise_error=check_login, username=username)
             if self.record_mode:
                 self.write_response_to_lib_folder(label, resp)
             return resp
 
-    def get_webapi(self, uri: str, headers: Optional[Dict[str, Any]] = None, label: Optional[str] = None,
-                   queryparameters: Dict[str, Any] = {}) -> Response:
-        """
-        Same as ``get_page``. Additionally it accepts the query parameter to add query parameter while running "GET" operation
-        Args:
-            uri: API URI to be called
-            headers: header for the REST API Call
-            label: the label to be displayed by locust
-            queryparameters: Queries/Filters
-
-        Returns: Json response of GET operation
-
-        To set custom headers
-
-        >>> headers = self.appian._interactor.setup_request_headers()
-        ... headers['Is-Admin'] = 'true'
-        ... self.appian._interactor.get_webapi('/suite/webapi/headers', headers=headers)
-
-        To set custom query parameters
-
-        >>> params = {'age': 5, 'start-date': '10-05-2020'}
-        ... self.appian._interactor.get_webapi('/suite/webapi/query', queryparameters=params)
-        """
-        querystring = []
-        for k, v in queryparameters.items():
-            querystring.append("{}={}".format(k, v))
-
-        uri += "?" + "&".join(querystring)
-        resp = self.get_page(uri, headers=headers, label=label)
-        return resp
-
     def upload_document_to_server(self, file_path: str, is_encrypted: bool = False) -> int:
-        '''
+        """
         Uploads a document to the server, so that it can be used in upload fields
         Args:
             uri: API URI to be called
             file_path: Path to the file to be uploaded
 
         Returns: Document Id that can be used for upload fields
-        ''',
+        """
 
         # Override default headers to avoid sending SAIL headers here
         headers = self.setup_request_headers()
         if is_encrypted:
             headers['encrypted'] = 'true'
         with open(file_path, 'rb') as f:
             resp_label = "Document.Upload." + os.path.basename(file_path).strip(" .")
```

### Comparing `appian-locust-2.0.0a6/appian_locust/_locust_error_handler.py` & `appian-locust-2.0.0a7/appian_locust/_locust_error_handler.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a6/appian_locust/_news.py` & `appian-locust-2.0.0a7/appian_locust/_news.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a6/appian_locust/_portals.py` & `appian-locust-2.0.0a7/appian_locust/_portals.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a6/appian_locust/_records.py` & `appian-locust-2.0.0a7/appian_locust/_records.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a6/appian_locust/_records_helper.py` & `appian-locust-2.0.0a7/appian_locust/_records_helper.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a6/appian_locust/_reports.py` & `appian-locust-2.0.0a7/appian_locust/_reports.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a6/appian_locust/_save_request_builder.py` & `appian-locust-2.0.0a7/appian_locust/_save_request_builder.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a6/appian_locust/_sites.py` & `appian-locust-2.0.0a7/appian_locust/_sites.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a6/appian_locust/_task_opener.py` & `appian-locust-2.0.0a7/appian_locust/_task_opener.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a6/appian_locust/_tasks.py` & `appian-locust-2.0.0a7/appian_locust/_tasks.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a6/appian_locust/_ui_reconciler.py` & `appian-locust-2.0.0a7/appian_locust/_ui_reconciler.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a6/appian_locust/actions_info.py` & `appian-locust-2.0.0a7/appian_locust/actions_info.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a6/appian_locust/appianclient.py` & `appian-locust-2.0.0a7/appian_locust/appianclient.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a6/appian_locust/application_uiform.py` & `appian-locust-2.0.0a7/appian_locust/application_uiform.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a6/appian_locust/design_object_uiform.py` & `appian-locust-2.0.0a7/appian_locust/design_object_uiform.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a6/appian_locust/design_uiform.py` & `appian-locust-2.0.0a7/appian_locust/design_uiform.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a6/appian_locust/exceptions.py` & `appian-locust-2.0.0a7/appian_locust/exceptions.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a6/appian_locust/feature_flag.py` & `appian-locust-2.0.0a7/appian_locust/feature_flag.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a6/appian_locust/helper.py` & `appian-locust-2.0.0a7/appian_locust/helper.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a6/appian_locust/loadDriverUtils.py` & `appian-locust-2.0.0a7/appian_locust/loadDriverUtils.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a6/appian_locust/logger.py` & `appian-locust-2.0.0a7/appian_locust/logger.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a6/appian_locust/news_info.py` & `appian-locust-2.0.0a7/appian_locust/news_info.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a6/appian_locust/record_list_uiform.py` & `appian-locust-2.0.0a7/appian_locust/record_list_uiform.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a6/appian_locust/record_uiform.py` & `appian-locust-2.0.0a7/appian_locust/record_uiform.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a6/appian_locust/records_info.py` & `appian-locust-2.0.0a7/appian_locust/records_info.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a6/appian_locust/reports_info.py` & `appian-locust-2.0.0a7/appian_locust/reports_info.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a6/appian_locust/site_helper.py` & `appian-locust-2.0.0a7/appian_locust/site_helper.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from requests.models import Response
-from typing import Optional
+from typing import Optional, Dict, Any
 
 from ._actions import _Actions
 from ._interactor import _Interactor
 
 
 class SiteHelper:
     """
@@ -32,14 +32,45 @@
         Example:
 
             >>> self.appian.site_helper.start_action("action_name")
 
         """
         return self.__actions.start_action(action_name, skip_design_call, exact_match)
 
+    def get_webapi(self, uri: str, headers: Optional[Dict[str, Any]] = None, label: Optional[str] = None,
+                   query_parameters: Dict[str, Any] = {}) -> Response:
+        """
+        Make a GET request to a web api endpoint
+        Args:
+            uri: API URI to be called
+            headers: header for the REST API Call
+            label: the label to be displayed by locust
+            query_parameters: Queries/Filters
+
+        Returns: Json response of GET operation
+
+        To set custom headers
+
+        >>> headers = self.appian._interactor.setup_request_headers()
+        ... headers['Is-Admin'] = 'true'
+        ... self.appian._interactor.get_webapi('/suite/webapi/headers', headers=headers)
+
+        To set custom query parameters
+
+        >>> params = {'age': 5, 'start-date': '10-05-2020'}
+        ... self.appian._interactor.get_webapi('/suite/webapi/query', query_parameters=params)
+        """
+        querystring = []
+        for k, v in query_parameters.items():
+            querystring.append("{}={}".format(k, v))
+
+        uri += "?" + "&".join(querystring)
+        resp = self.__interactor.get_page(uri, headers=headers, label=label)
+        return resp
+
     def fetch_content(self, opaque_id: str, locust_request_label: Optional[str]) -> Response:
         """
         Fetch a content element, such as an image
         Args:
             opaque_id: The opaque id of the content to download
             locust_request_label: label to associate request with
```

### Comparing `appian-locust-2.0.0a6/appian_locust/site_objects.py` & `appian-locust-2.0.0a7/appian_locust/site_objects.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a6/appian_locust/sites_info.py` & `appian-locust-2.0.0a7/appian_locust/sites_info.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a6/appian_locust/tasks_info.py` & `appian-locust-2.0.0a7/appian_locust/tasks_info.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a6/appian_locust/tempo_navigator.py` & `appian-locust-2.0.0a7/appian_locust/tempo_navigator.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a6/appian_locust/uiform.py` & `appian-locust-2.0.0a7/appian_locust/uiform.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a6/appian_locust/visitor.py` & `appian-locust-2.0.0a7/appian_locust/visitor.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a6/appian_locust.egg-info/PKG-INFO` & `appian-locust-2.0.0a7/appian_locust.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appian-locust
-Version: 2.0.0a6
+Version: 2.0.0a7
 Summary: Tools and functions to make testing Appian with Locust easier
 Home-page: https://gitlab.com/appian-oss/appian-locust
 Author: Appian Performance & Reliability Engineering Squad
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `appian-locust-2.0.0a6/appian_locust.egg-info/SOURCES.txt` & `appian-locust-2.0.0a7/appian_locust.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a6/setup.cfg` & `appian-locust-2.0.0a7/setup.cfg`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a6/setup.py` & `appian-locust-2.0.0a7/setup.py`

 * *Files identical despite different names*

