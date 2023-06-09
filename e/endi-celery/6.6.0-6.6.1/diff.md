# Comparing `tmp/endi_celery-6.6.0.tar.gz` & `tmp/endi_celery-6.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "endi_celery-6.6.0.tar", last modified: Thu May 25 15:55:42 2023, max compression
+gzip compressed data, was "endi_celery-6.6.1.tar", last modified: Fri Jun  9 15:06:03 2023, max compression
```

## Comparing `endi_celery-6.6.0.tar` & `endi_celery-6.6.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-05-25 15:55:42.267074 endi_celery-6.6.0/
--rw-r--r--   0 gas       (1000) gas       (1000)        6 2023-05-25 15:55:13.000000 endi_celery-6.6.0/CURRENT_VERSION
--rw-r--r--   0 gas       (1000) gas       (1000)    35147 2020-06-24 14:37:06.000000 endi_celery-6.6.0/LICENSE.txt
--rw-r--r--   0 gas       (1000) gas       (1000)      186 2020-06-24 14:37:06.000000 endi_celery-6.6.0/MANIFEST.in
--rw-r--r--   0 gas       (1000) gas       (1000)     3178 2023-05-25 15:55:42.267074 endi_celery-6.6.0/PKG-INFO
--rw-r--r--   0 gas       (1000) gas       (1000)     2601 2023-04-24 10:03:13.000000 endi_celery-6.6.0/README.rst
--rw-r--r--   0 gas       (1000) gas       (1000)     5047 2023-05-25 15:22:08.000000 endi_celery-6.6.0/development.ini
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-05-25 15:55:42.264074 endi_celery-6.6.0/endi_celery/
--rw-r--r--   0 gas       (1000) gas       (1000)     4535 2023-04-24 10:04:13.000000 endi_celery-6.6.0/endi_celery/__init__.py
--rw-r--r--   0 gas       (1000) gas       (1000)     1787 2023-01-11 11:06:17.000000 endi_celery-6.6.0/endi_celery/conf.py
--rw-r--r--   0 gas       (1000) gas       (1000)      585 2023-01-11 11:00:06.000000 endi_celery-6.6.0/endi_celery/exception.py
--rw-r--r--   0 gas       (1000) gas       (1000)      504 2021-09-10 16:39:28.000000 endi_celery-6.6.0/endi_celery/hacks.py
--rw-r--r--   0 gas       (1000) gas       (1000)      753 2023-01-11 11:00:06.000000 endi_celery-6.6.0/endi_celery/interfaces.py
--rw-r--r--   0 gas       (1000) gas       (1000)      482 2023-01-11 11:48:27.000000 endi_celery-6.6.0/endi_celery/locks.py
--rw-r--r--   0 gas       (1000) gas       (1000)     5742 2022-12-09 15:12:22.000000 endi_celery-6.6.0/endi_celery/mail.py
--rw-r--r--   0 gas       (1000) gas       (1000)     7225 2022-12-09 15:12:22.000000 endi_celery-6.6.0/endi_celery/models.py
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-05-25 15:55:42.265075 endi_celery-6.6.0/endi_celery/parsers/
--rw-r--r--   0 gas       (1000) gas       (1000)     2162 2023-01-12 14:56:56.000000 endi_celery-6.6.0/endi_celery/parsers/__init__.py
--rw-r--r--   0 gas       (1000) gas       (1000)     2870 2023-05-11 15:37:23.000000 endi_celery-6.6.0/endi_celery/parsers/isacompta.py
--rw-r--r--   0 gas       (1000) gas       (1000)     3288 2023-01-18 08:46:47.000000 endi_celery-6.6.0/endi_celery/parsers/quadra.py
--rw-r--r--   0 gas       (1000) gas       (1000)     2966 2023-01-11 11:02:40.000000 endi_celery-6.6.0/endi_celery/parsers/sage.py
--rw-r--r--   0 gas       (1000) gas       (1000)     3891 2023-04-24 10:04:13.000000 endi_celery-6.6.0/endi_celery/parsers/sage_generation_expert.py
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-05-25 15:55:42.265075 endi_celery-6.6.0/endi_celery/schedulers/
--rw-r--r--   0 gas       (1000) gas       (1000)       29 2020-06-24 14:37:06.000000 endi_celery-6.6.0/endi_celery/schedulers/__init__.py
--rw-r--r--   0 gas       (1000) gas       (1000)      427 2022-12-09 15:12:22.000000 endi_celery-6.6.0/endi_celery/schedulers/tasks.py
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-05-25 15:55:42.266075 endi_celery-6.6.0/endi_celery/tasks/
--rw-r--r--   0 gas       (1000) gas       (1000)     8087 2022-12-09 15:12:22.000000 endi_celery-6.6.0/endi_celery/tasks/__init__.py
--rw-r--r--   0 gas       (1000) gas       (1000)    39473 2023-05-25 15:25:03.000000 endi_celery-6.6.0/endi_celery/tasks/accounting_measure_compute.py
--rw-r--r--   0 gas       (1000) gas       (1000)    12003 2023-01-17 16:14:55.000000 endi_celery-6.6.0/endi_celery/tasks/accounting_parser.py
--rw-r--r--   0 gas       (1000) gas       (1000)    29193 2023-01-12 16:49:34.000000 endi_celery-6.6.0/endi_celery/tasks/csv_import.py
--rw-r--r--   0 gas       (1000) gas       (1000)    13542 2023-05-25 15:32:59.000000 endi_celery-6.6.0/endi_celery/tasks/export.py
--rw-r--r--   0 gas       (1000) gas       (1000)     4856 2022-12-09 15:12:23.000000 endi_celery-6.6.0/endi_celery/tasks/mail.py
--rw-r--r--   0 gas       (1000) gas       (1000)     1064 2023-05-25 15:25:03.000000 endi_celery-6.6.0/endi_celery/tasks/notification.py
--rw-r--r--   0 gas       (1000) gas       (1000)     3267 2022-03-03 10:44:16.000000 endi_celery-6.6.0/endi_celery/tasks/tasks.py
--rw-r--r--   0 gas       (1000) gas       (1000)     6687 2022-12-09 15:12:23.000000 endi_celery-6.6.0/endi_celery/tasks/utils.py
--rw-r--r--   0 gas       (1000) gas       (1000)     2765 2022-03-03 10:44:16.000000 endi_celery-6.6.0/endi_celery/transactional_task.py
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-05-25 15:55:42.264074 endi_celery-6.6.0/endi_celery.egg-info/
--rw-r--r--   0 gas       (1000) gas       (1000)     3178 2023-05-25 15:55:41.000000 endi_celery-6.6.0/endi_celery.egg-info/PKG-INFO
--rw-r--r--   0 gas       (1000) gas       (1000)     1106 2023-05-25 15:55:42.000000 endi_celery-6.6.0/endi_celery.egg-info/SOURCES.txt
--rw-r--r--   0 gas       (1000) gas       (1000)        1 2023-05-25 15:55:41.000000 endi_celery-6.6.0/endi_celery.egg-info/dependency_links.txt
--rw-r--r--   0 gas       (1000) gas       (1000)       82 2023-05-25 15:55:41.000000 endi_celery-6.6.0/endi_celery.egg-info/entry_points.txt
--rw-r--r--   0 gas       (1000) gas       (1000)        1 2020-11-23 12:28:56.000000 endi_celery-6.6.0/endi_celery.egg-info/not-zip-safe
--rw-r--r--   0 gas       (1000) gas       (1000)       80 2023-05-25 15:55:42.000000 endi_celery-6.6.0/endi_celery.egg-info/requires.txt
--rw-r--r--   0 gas       (1000) gas       (1000)       12 2023-05-25 15:55:42.000000 endi_celery-6.6.0/endi_celery.egg-info/top_level.txt
--rw-r--r--   0 gas       (1000) gas       (1000)     2934 2021-03-25 17:57:51.000000 endi_celery-6.6.0/prod_example.ini
--rw-r--r--   0 gas       (1000) gas       (1000)       53 2020-06-24 14:37:06.000000 endi_celery-6.6.0/pytest.ini
--rw-r--r--   0 gas       (1000) gas       (1000)       81 2022-01-12 14:56:54.000000 endi_celery-6.6.0/requirements.txt
--rw-r--r--   0 gas       (1000) gas       (1000)       38 2023-05-25 15:55:42.267074 endi_celery-6.6.0/setup.cfg
--rw-r--r--   0 gas       (1000) gas       (1000)     1326 2023-01-17 16:18:35.000000 endi_celery-6.6.0/setup.py
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-06-09 15:06:03.615957 endi_celery-6.6.1/
+-rw-r--r--   0 gas       (1000) gas       (1000)        6 2023-06-09 15:05:26.000000 endi_celery-6.6.1/CURRENT_VERSION
+-rw-r--r--   0 gas       (1000) gas       (1000)    35147 2020-06-24 14:37:06.000000 endi_celery-6.6.1/LICENSE.txt
+-rw-r--r--   0 gas       (1000) gas       (1000)      186 2020-06-24 14:37:06.000000 endi_celery-6.6.1/MANIFEST.in
+-rw-r--r--   0 gas       (1000) gas       (1000)     3178 2023-06-09 15:06:03.614957 endi_celery-6.6.1/PKG-INFO
+-rw-r--r--   0 gas       (1000) gas       (1000)     2601 2023-04-24 10:03:13.000000 endi_celery-6.6.1/README.rst
+-rw-r--r--   0 gas       (1000) gas       (1000)     5047 2023-05-25 15:22:08.000000 endi_celery-6.6.1/development.ini
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-06-09 15:06:03.608957 endi_celery-6.6.1/endi_celery/
+-rw-r--r--   0 gas       (1000) gas       (1000)     4535 2023-04-24 10:04:13.000000 endi_celery-6.6.1/endi_celery/__init__.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     1787 2023-01-11 11:06:17.000000 endi_celery-6.6.1/endi_celery/conf.py
+-rw-r--r--   0 gas       (1000) gas       (1000)      585 2023-01-11 11:00:06.000000 endi_celery-6.6.1/endi_celery/exception.py
+-rw-r--r--   0 gas       (1000) gas       (1000)      504 2021-09-10 16:39:28.000000 endi_celery-6.6.1/endi_celery/hacks.py
+-rw-r--r--   0 gas       (1000) gas       (1000)      753 2023-01-11 11:00:06.000000 endi_celery-6.6.1/endi_celery/interfaces.py
+-rw-r--r--   0 gas       (1000) gas       (1000)      482 2023-01-11 11:48:27.000000 endi_celery-6.6.1/endi_celery/locks.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     5742 2022-12-09 15:12:22.000000 endi_celery-6.6.1/endi_celery/mail.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     7225 2022-12-09 15:12:22.000000 endi_celery-6.6.1/endi_celery/models.py
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-06-09 15:06:03.611957 endi_celery-6.6.1/endi_celery/parsers/
+-rw-r--r--   0 gas       (1000) gas       (1000)     2162 2023-01-12 14:56:56.000000 endi_celery-6.6.1/endi_celery/parsers/__init__.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     2870 2023-05-11 15:37:23.000000 endi_celery-6.6.1/endi_celery/parsers/isacompta.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     3288 2023-01-18 08:46:47.000000 endi_celery-6.6.1/endi_celery/parsers/quadra.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     2966 2023-01-11 11:02:40.000000 endi_celery-6.6.1/endi_celery/parsers/sage.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     3891 2023-04-24 10:04:13.000000 endi_celery-6.6.1/endi_celery/parsers/sage_generation_expert.py
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-06-09 15:06:03.611957 endi_celery-6.6.1/endi_celery/schedulers/
+-rw-r--r--   0 gas       (1000) gas       (1000)       29 2020-06-24 14:37:06.000000 endi_celery-6.6.1/endi_celery/schedulers/__init__.py
+-rw-r--r--   0 gas       (1000) gas       (1000)      427 2022-12-09 15:12:22.000000 endi_celery-6.6.1/endi_celery/schedulers/tasks.py
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-06-09 15:06:03.614957 endi_celery-6.6.1/endi_celery/tasks/
+-rw-r--r--   0 gas       (1000) gas       (1000)     8087 2022-12-09 15:12:22.000000 endi_celery-6.6.1/endi_celery/tasks/__init__.py
+-rw-r--r--   0 gas       (1000) gas       (1000)    39473 2023-05-25 15:25:03.000000 endi_celery-6.6.1/endi_celery/tasks/accounting_measure_compute.py
+-rw-r--r--   0 gas       (1000) gas       (1000)    12003 2023-01-17 16:14:55.000000 endi_celery-6.6.1/endi_celery/tasks/accounting_parser.py
+-rw-r--r--   0 gas       (1000) gas       (1000)    29193 2023-01-12 16:49:34.000000 endi_celery-6.6.1/endi_celery/tasks/csv_import.py
+-rw-r--r--   0 gas       (1000) gas       (1000)    16307 2023-06-09 15:05:17.000000 endi_celery-6.6.1/endi_celery/tasks/export.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     4856 2022-12-09 15:12:23.000000 endi_celery-6.6.1/endi_celery/tasks/mail.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     1064 2023-05-25 15:25:03.000000 endi_celery-6.6.1/endi_celery/tasks/notification.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     3267 2022-03-03 10:44:16.000000 endi_celery-6.6.1/endi_celery/tasks/tasks.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     6687 2022-12-09 15:12:23.000000 endi_celery-6.6.1/endi_celery/tasks/utils.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     2765 2022-03-03 10:44:16.000000 endi_celery-6.6.1/endi_celery/transactional_task.py
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-06-09 15:06:03.610957 endi_celery-6.6.1/endi_celery.egg-info/
+-rw-r--r--   0 gas       (1000) gas       (1000)     3178 2023-06-09 15:06:02.000000 endi_celery-6.6.1/endi_celery.egg-info/PKG-INFO
+-rw-r--r--   0 gas       (1000) gas       (1000)     1106 2023-06-09 15:06:03.000000 endi_celery-6.6.1/endi_celery.egg-info/SOURCES.txt
+-rw-r--r--   0 gas       (1000) gas       (1000)        1 2023-06-09 15:06:03.000000 endi_celery-6.6.1/endi_celery.egg-info/dependency_links.txt
+-rw-r--r--   0 gas       (1000) gas       (1000)       82 2023-06-09 15:06:03.000000 endi_celery-6.6.1/endi_celery.egg-info/entry_points.txt
+-rw-r--r--   0 gas       (1000) gas       (1000)        1 2020-11-23 12:28:56.000000 endi_celery-6.6.1/endi_celery.egg-info/not-zip-safe
+-rw-r--r--   0 gas       (1000) gas       (1000)       80 2023-06-09 15:06:03.000000 endi_celery-6.6.1/endi_celery.egg-info/requires.txt
+-rw-r--r--   0 gas       (1000) gas       (1000)       12 2023-06-09 15:06:03.000000 endi_celery-6.6.1/endi_celery.egg-info/top_level.txt
+-rw-r--r--   0 gas       (1000) gas       (1000)     2934 2021-03-25 17:57:51.000000 endi_celery-6.6.1/prod_example.ini
+-rw-r--r--   0 gas       (1000) gas       (1000)       53 2020-06-24 14:37:06.000000 endi_celery-6.6.1/pytest.ini
+-rw-r--r--   0 gas       (1000) gas       (1000)       81 2022-01-12 14:56:54.000000 endi_celery-6.6.1/requirements.txt
+-rw-r--r--   0 gas       (1000) gas       (1000)       38 2023-06-09 15:06:03.615957 endi_celery-6.6.1/setup.cfg
+-rw-r--r--   0 gas       (1000) gas       (1000)     1326 2023-01-17 16:18:35.000000 endi_celery-6.6.1/setup.py
```

### Comparing `endi_celery-6.6.0/LICENSE.txt` & `endi_celery-6.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `endi_celery-6.6.0/PKG-INFO` & `endi_celery-6.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: endi_celery
-Version: 6.6.0
+Version: 6.6.1
 Summary: endi_celery
 Home-page: https://framagit.org/endi/endi_celery
 Author: Coopérer Pour Entreprendre
 Author-email: contact@endi.coop
 License: GPLv3
 Keywords: web wsgi bfg pylons pyramid celery
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `endi_celery-6.6.0/README.rst` & `endi_celery-6.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `endi_celery-6.6.0/development.ini` & `endi_celery-6.6.1/development.ini`

 * *Files identical despite different names*

### Comparing `endi_celery-6.6.0/endi_celery/__init__.py` & `endi_celery-6.6.1/endi_celery/__init__.py`

 * *Files identical despite different names*

### Comparing `endi_celery-6.6.0/endi_celery/conf.py` & `endi_celery-6.6.1/endi_celery/conf.py`

 * *Files identical despite different names*

### Comparing `endi_celery-6.6.0/endi_celery/exception.py` & `endi_celery-6.6.1/endi_celery/exception.py`

 * *Files identical despite different names*

### Comparing `endi_celery-6.6.0/endi_celery/interfaces.py` & `endi_celery-6.6.1/endi_celery/interfaces.py`

 * *Files identical despite different names*

### Comparing `endi_celery-6.6.0/endi_celery/mail.py` & `endi_celery-6.6.1/endi_celery/mail.py`

 * *Files identical despite different names*

### Comparing `endi_celery-6.6.0/endi_celery/models.py` & `endi_celery-6.6.1/endi_celery/models.py`

 * *Files identical despite different names*

### Comparing `endi_celery-6.6.0/endi_celery/parsers/__init__.py` & `endi_celery-6.6.1/endi_celery/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `endi_celery-6.6.0/endi_celery/parsers/isacompta.py` & `endi_celery-6.6.1/endi_celery/parsers/isacompta.py`

 * *Files identical despite different names*

### Comparing `endi_celery-6.6.0/endi_celery/parsers/quadra.py` & `endi_celery-6.6.1/endi_celery/parsers/quadra.py`

 * *Files identical despite different names*

### Comparing `endi_celery-6.6.0/endi_celery/parsers/sage.py` & `endi_celery-6.6.1/endi_celery/parsers/sage.py`

 * *Files identical despite different names*

### Comparing `endi_celery-6.6.0/endi_celery/parsers/sage_generation_expert.py` & `endi_celery-6.6.1/endi_celery/parsers/sage_generation_expert.py`

 * *Files identical despite different names*

### Comparing `endi_celery-6.6.0/endi_celery/tasks/__init__.py` & `endi_celery-6.6.1/endi_celery/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `endi_celery-6.6.0/endi_celery/tasks/accounting_measure_compute.py` & `endi_celery-6.6.1/endi_celery/tasks/accounting_measure_compute.py`

 * *Files identical despite different names*

### Comparing `endi_celery-6.6.0/endi_celery/tasks/accounting_parser.py` & `endi_celery-6.6.1/endi_celery/tasks/accounting_parser.py`

 * *Files identical despite different names*

### Comparing `endi_celery-6.6.0/endi_celery/tasks/csv_import.py` & `endi_celery-6.6.1/endi_celery/tasks/csv_import.py`

 * *Files identical despite different names*

### Comparing `endi_celery-6.6.0/endi_celery/tasks/export.py` & `endi_celery-6.6.1/endi_celery/tasks/export.py`

 * *Files 17% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 from endi_base.utils.date import format_date
 from endi_celery.conf import get_setting
 from endi_celery.models import FileGenerationJob
 from endi_celery.tasks import utils
 from endi.compute.math_utils import integer_to_amount
 from endi.export.utils import format_filename
 from endi.models.task import Task
+from endi.models.expense import ExpenseSheet
 from endi.utils.html import strip_html_tags
 
 
 MODELS_CONFIGURATION = {}
 
 logger = utils.get_logger(__name__)
 
@@ -253,17 +254,15 @@
         utils.record_failure(FileGenerationJob, job_id, errors)
     else:
         utils.record_completed(FileGenerationJob, job_id, filename=result_filename)
 
     return ""
 
 
-def _export_data_to_file(
-    headers, data, filename="export", file_format="csv"
-):
+def _export_data_to_file(headers, data, filename="export", file_format="csv"):
     """
     Generic function to export given data to given format
 
     :param list headers: List of dicts with headers data, format :
         (
             {"label": "Column label", "name": "col_1"},
             {"label": "Column label 2", "name": "col_2"},
@@ -367,8 +366,86 @@
         )
     except Exception:
         logger.exception("Error while generating export file")
         errors = [GENERATION_ERROR_MESSAGE % job_id]
         utils.record_failure(FileGenerationJob, job_id, errors)
     else:
         utils.record_completed(FileGenerationJob, job_id, filename=result_filename)
+    return ""
+
+
+@celery_app.task(bind=True)
+@cache_region("default_term", "expenses")
+def export_expenses_to_file(self, job_id, expense_ids, filename, format="csv"):
+    """
+    export expenses to file
+
+    :param int job_id: The id of the job object
+    :param list expense_ids: List of expenses ids to query
+    :param str format: The format in which we want to export
+    """
+
+    logger.debug(
+        f" + Exporting details for the following expenses's ids : {expense_ids}"
+    )
+
+    # Mark job started
+    utils.start_job(self.request, FileGenerationJob, job_id)
+
+    headers = (
+        {"label": "Numéro de pièce", "name": "official_number"},
+        {"label": "Titre", "name": "title"},
+        {"label": "Entrepreneur", "name": "user_name"},
+        {"label": "Enseigne", "name": "company_name"},
+        {"label": "Année", "name": "year"},
+        {"label": "Mois", "name": "month"},
+        {"label": "HT", "name": "ht"},
+        {"label": "TVA", "name": "tva"},
+        {"label": "TTC", "name": "ttc"},
+        {"label": "Km", "name": "km"},
+        {"label": "Justificatifs reçus et acceptés", "name": "justified"},
+        {"label": "Paiements", "name": "paid"},
+    )
+
+    expense_justified_status = {
+        0: "non",
+        1: "oui",
+    }
+    expense_paid_status = {
+        "resulted": "intégral",
+        "paid": "partiel",
+        "waiting": "en attente",
+    }
+
+    try:
+        data = []
+        query = ExpenseSheet.query().filter(ExpenseSheet.id.in_(expense_ids))
+        for expense in query:
+            row_data = {
+                "official_number": expense.official_number,
+                "title": expense.title,
+                "user_name": expense.user.label,
+                "company_name": expense.company.name,
+                "year": expense.year,
+                "month": expense.month,
+                "ht": expense.total_ht,
+                "tva": expense.total_tva,
+                "ttc": expense.total,
+                "km": expense.total_km,
+                "justified": expense_justified_status.get(
+                    expense.justified, expense.justified
+                ),
+                "paid": expense_paid_status.get(
+                    expense.paid_status, expense.paid_status
+                ),
+            }
+            data.append(row_data)
+        result_filename = _export_data_to_file(
+            headers, data, filename=filename, file_format=format
+        )
+    except Exception:
+        logger.exception("Error while generating export file")
+        errors = [GENERATION_ERROR_MESSAGE % job_id]
+        utils.record_failure(FileGenerationJob, job_id, errors)
+    else:
+        utils.record_completed(FileGenerationJob, job_id, filename=result_filename)
     return ""
```

### Comparing `endi_celery-6.6.0/endi_celery/tasks/mail.py` & `endi_celery-6.6.1/endi_celery/tasks/mail.py`

 * *Files identical despite different names*

### Comparing `endi_celery-6.6.0/endi_celery/tasks/notification.py` & `endi_celery-6.6.1/endi_celery/tasks/notification.py`

 * *Files identical despite different names*

### Comparing `endi_celery-6.6.0/endi_celery/tasks/tasks.py` & `endi_celery-6.6.1/endi_celery/tasks/tasks.py`

 * *Files identical despite different names*

### Comparing `endi_celery-6.6.0/endi_celery/tasks/utils.py` & `endi_celery-6.6.1/endi_celery/tasks/utils.py`

 * *Files identical despite different names*

### Comparing `endi_celery-6.6.0/endi_celery/transactional_task.py` & `endi_celery-6.6.1/endi_celery/transactional_task.py`

 * *Files identical despite different names*

### Comparing `endi_celery-6.6.0/endi_celery.egg-info/PKG-INFO` & `endi_celery-6.6.1/endi_celery.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: endi-celery
-Version: 6.6.0
+Version: 6.6.1
 Summary: endi_celery
 Home-page: https://framagit.org/endi/endi_celery
 Author: Coopérer Pour Entreprendre
 Author-email: contact@endi.coop
 License: GPLv3
 Keywords: web wsgi bfg pylons pyramid celery
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `endi_celery-6.6.0/endi_celery.egg-info/SOURCES.txt` & `endi_celery-6.6.1/endi_celery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `endi_celery-6.6.0/prod_example.ini` & `endi_celery-6.6.1/prod_example.ini`

 * *Files identical despite different names*

### Comparing `endi_celery-6.6.0/setup.py` & `endi_celery-6.6.1/setup.py`

 * *Files identical despite different names*

