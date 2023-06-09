# Comparing `tmp/tejapi-0.1.8.tar.gz` & `tmp/tejapi-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\tejapi-0.1.8.tar", last modified: Fri Sep  7 04:56:17 2018, max compression
+gzip compressed data, was "dist\tejapi-0.1.9.tar", last modified: Tue Dec 11 08:15:24 2018, max compression
```

## Comparing `tejapi-0.1.8.tar` & `tejapi-0.1.9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2018-09-07 04:56:17.000000 tejapi-0.1.8/
--rw-rw-rw-   0        0        0      446 2018-09-07 04:56:17.000000 tejapi-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0      247 2018-09-07 04:43:53.000000 tejapi-0.1.8/README.md
--rw-rw-rw-   0        0        0      175 2018-09-07 04:56:17.000000 tejapi-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1356 2018-09-07 04:56:13.000000 tejapi-0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2018-09-07 04:56:17.000000 tejapi-0.1.8/tejapi/
--rw-rw-rw-   0        0        0      120 2018-09-07 04:27:55.000000 tejapi-0.1.8/tejapi/api_config.py
--rw-rw-rw-   0        0        0     3042 2018-05-18 08:27:07.000000 tejapi-0.1.8/tejapi/connection.py
-drwxrwxrwx   0        0        0        0 2018-09-07 04:56:17.000000 tejapi-0.1.8/tejapi/errors/
--rw-rw-rw-   0        0        0     1609 2018-03-26 08:07:44.000000 tejapi-0.1.8/tejapi/errors/tej_error.py
--rw-rw-rw-   0        0        0        0 2018-01-08 04:05:44.000000 tejapi-0.1.8/tejapi/errors/__init__.py
--rw-rw-rw-   0        0        0     1631 2018-09-07 04:42:01.000000 tejapi-0.1.8/tejapi/get.py
--rw-rw-rw-   0        0        0      530 2018-03-27 05:45:16.000000 tejapi-0.1.8/tejapi/message.py
-drwxrwxrwx   0        0        0        0 2018-09-07 04:56:17.000000 tejapi-0.1.8/tejapi/model/
--rw-rw-rw-   0        0        0     1129 2018-03-27 05:45:26.000000 tejapi-0.1.8/tejapi/model/data.py
--rw-rw-rw-   0        0        0     1970 2018-03-27 05:45:43.000000 tejapi-0.1.8/tejapi/model/database.py
--rw-rw-rw-   0        0        0      472 2018-03-27 05:45:51.000000 tejapi-0.1.8/tejapi/model/datatable.py
--rw-rw-rw-   0        0        0      117 2018-01-08 04:05:44.000000 tejapi-0.1.8/tejapi/model/data_list.py
--rw-rw-rw-   0        0        0     2081 2018-03-27 05:45:57.000000 tejapi-0.1.8/tejapi/model/data_mixin.py
--rw-rw-rw-   0        0        0      738 2018-01-08 04:05:44.000000 tejapi-0.1.8/tejapi/model/merged_data_list.py
--rw-rw-rw-   0        0        0      792 2018-01-08 04:05:44.000000 tejapi-0.1.8/tejapi/model/model_base.py
--rw-rw-rw-   0        0        0     1475 2018-03-27 05:46:10.000000 tejapi-0.1.8/tejapi/model/model_list.py
--rw-rw-rw-   0        0        0      168 2018-01-08 04:05:44.000000 tejapi-0.1.8/tejapi/model/paginated_list.py
--rw-rw-rw-   0        0        0        0 2018-01-08 04:05:44.000000 tejapi-0.1.8/tejapi/model/__init__.py
-drwxrwxrwx   0        0        0        0 2018-09-07 04:56:17.000000 tejapi-0.1.8/tejapi/operations/
--rw-rw-rw-   0        0        0      852 2018-03-27 05:46:14.000000 tejapi-0.1.8/tejapi/operations/data_list.py
--rw-rw-rw-   0        0        0      846 2018-05-09 06:26:21.000000 tejapi-0.1.8/tejapi/operations/get.py
--rw-rw-rw-   0        0        0     1591 2018-05-18 08:26:57.000000 tejapi-0.1.8/tejapi/operations/list.py
--rw-rw-rw-   0        0        0      255 2018-01-08 04:05:44.000000 tejapi-0.1.8/tejapi/operations/operation.py
--rw-rw-rw-   0        0        0        0 2018-01-08 04:05:44.000000 tejapi-0.1.8/tejapi/operations/__init__.py
--rw-rw-rw-   0        0        0     3488 2018-03-26 08:03:29.000000 tejapi-0.1.8/tejapi/util.py
-drwxrwxrwx   0        0        0        0 2018-09-07 04:56:17.000000 tejapi-0.1.8/tejapi/utils/
--rw-rw-rw-   0        0        0      234 2018-03-27 05:46:23.000000 tejapi-0.1.8/tejapi/utils/api_key_util.py
--rw-rw-rw-   0        0        0       63 2018-03-27 06:08:01.000000 tejapi-0.1.8/tejapi/utils/__init__.py
--rw-rw-rw-   0        0        0       18 2018-03-26 08:02:30.000000 tejapi-0.1.8/tejapi/version.py
--rw-rw-rw-   0        0        0      218 2018-03-26 08:08:27.000000 tejapi-0.1.8/tejapi/__init__.py
-drwxrwxrwx   0        0        0        0 2018-09-07 04:56:17.000000 tejapi-0.1.8/tejapi.egg-info/
--rw-rw-rw-   0        0        0        1 2018-09-07 04:56:16.000000 tejapi-0.1.8/tejapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      446 2018-09-07 04:56:16.000000 tejapi-0.1.8/tejapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       93 2018-09-07 04:56:16.000000 tejapi-0.1.8/tejapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0      821 2018-09-07 04:56:17.000000 tejapi-0.1.8/tejapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2018-09-07 04:56:16.000000 tejapi-0.1.8/tejapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2018-12-11 08:15:24.000000 tejapi-0.1.9/
+-rw-rw-rw-   0        0        0      446 2018-12-11 08:15:24.000000 tejapi-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      247 2018-09-07 04:43:53.000000 tejapi-0.1.9/README.md
+-rw-rw-rw-   0        0        0      175 2018-12-11 08:15:24.000000 tejapi-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1356 2018-12-11 08:12:41.000000 tejapi-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2018-12-11 08:15:24.000000 tejapi-0.1.9/tejapi/
+-rw-rw-rw-   0        0        0      141 2018-12-11 08:08:13.000000 tejapi-0.1.9/tejapi/api_config.py
+-rw-rw-rw-   0        0        0     3042 2018-09-20 04:30:50.000000 tejapi-0.1.9/tejapi/connection.py
+drwxrwxrwx   0        0        0        0 2018-12-11 08:15:24.000000 tejapi-0.1.9/tejapi/errors/
+-rw-rw-rw-   0        0        0     1609 2018-03-26 08:07:44.000000 tejapi-0.1.9/tejapi/errors/tej_error.py
+-rw-rw-rw-   0        0        0        0 2018-01-08 04:05:44.000000 tejapi-0.1.9/tejapi/errors/__init__.py
+-rw-rw-rw-   0        0        0     1631 2018-09-07 04:42:01.000000 tejapi-0.1.9/tejapi/get.py
+-rw-rw-rw-   0        0        0      530 2018-03-27 05:45:16.000000 tejapi-0.1.9/tejapi/message.py
+drwxrwxrwx   0        0        0        0 2018-12-11 08:15:24.000000 tejapi-0.1.9/tejapi/model/
+-rw-rw-rw-   0        0        0     1129 2018-03-27 05:45:26.000000 tejapi-0.1.9/tejapi/model/data.py
+-rw-rw-rw-   0        0        0     1970 2018-03-27 05:45:43.000000 tejapi-0.1.9/tejapi/model/database.py
+-rw-rw-rw-   0        0        0      472 2018-03-27 05:45:51.000000 tejapi-0.1.9/tejapi/model/datatable.py
+-rw-rw-rw-   0        0        0      117 2018-01-08 04:05:44.000000 tejapi-0.1.9/tejapi/model/data_list.py
+-rw-rw-rw-   0        0        0     2101 2018-12-11 08:10:41.000000 tejapi-0.1.9/tejapi/model/data_mixin.py
+-rw-rw-rw-   0        0        0      738 2018-01-08 04:05:44.000000 tejapi-0.1.9/tejapi/model/merged_data_list.py
+-rw-rw-rw-   0        0        0      792 2018-01-08 04:05:44.000000 tejapi-0.1.9/tejapi/model/model_base.py
+-rw-rw-rw-   0        0        0     1475 2018-03-27 05:46:10.000000 tejapi-0.1.9/tejapi/model/model_list.py
+-rw-rw-rw-   0        0        0      168 2018-01-08 04:05:44.000000 tejapi-0.1.9/tejapi/model/paginated_list.py
+-rw-rw-rw-   0        0        0        0 2018-01-08 04:05:44.000000 tejapi-0.1.9/tejapi/model/__init__.py
+drwxrwxrwx   0        0        0        0 2018-12-11 08:15:24.000000 tejapi-0.1.9/tejapi/operations/
+-rw-rw-rw-   0        0        0      852 2018-03-27 05:46:14.000000 tejapi-0.1.9/tejapi/operations/data_list.py
+-rw-rw-rw-   0        0        0      846 2018-12-11 07:57:35.000000 tejapi-0.1.9/tejapi/operations/get.py
+-rw-rw-rw-   0        0        0     1591 2018-12-11 08:09:02.000000 tejapi-0.1.9/tejapi/operations/list.py
+-rw-rw-rw-   0        0        0      255 2018-01-08 04:05:44.000000 tejapi-0.1.9/tejapi/operations/operation.py
+-rw-rw-rw-   0        0        0        0 2018-01-08 04:05:44.000000 tejapi-0.1.9/tejapi/operations/__init__.py
+-rw-rw-rw-   0        0        0     3550 2018-12-11 08:07:37.000000 tejapi-0.1.9/tejapi/util.py
+drwxrwxrwx   0        0        0        0 2018-12-11 08:15:24.000000 tejapi-0.1.9/tejapi/utils/
+-rw-rw-rw-   0        0        0      234 2018-03-27 05:46:23.000000 tejapi-0.1.9/tejapi/utils/api_key_util.py
+-rw-rw-rw-   0        0        0       63 2018-03-27 06:08:01.000000 tejapi-0.1.9/tejapi/utils/__init__.py
+-rw-rw-rw-   0        0        0       18 2018-03-26 08:02:30.000000 tejapi-0.1.9/tejapi/version.py
+-rw-rw-rw-   0        0        0      218 2018-03-26 08:08:27.000000 tejapi-0.1.9/tejapi/__init__.py
+drwxrwxrwx   0        0        0        0 2018-12-11 08:15:24.000000 tejapi-0.1.9/tejapi.egg-info/
+-rw-rw-rw-   0        0        0        1 2018-12-11 08:15:23.000000 tejapi-0.1.9/tejapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      446 2018-12-11 08:15:23.000000 tejapi-0.1.9/tejapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       93 2018-12-11 08:15:23.000000 tejapi-0.1.9/tejapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      821 2018-12-11 08:15:24.000000 tejapi-0.1.9/tejapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2018-12-11 08:15:23.000000 tejapi-0.1.9/tejapi.egg-info/top_level.txt
```

### Comparing `tejapi-0.1.8/setup.py` & `tejapi-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 ]
 
 setup(
     name='tejapi',
     description='Package for access tej database from REST API',
     keywords=['tej', 'API', 'data', 'financial', 'economic'],
     long_description='A Python library for TEJ RESTful API.  For more information, please access https://api.tej.com.tw .',
-    version='0.1.8',
+    version='0.1.9',
     author='tej',
     author_email='tej@tej.com.tw',
     maintainer='tej api Development Team',
     maintainer_email='tej@tej.com',
     url='https://api.tej.com.tw',
     license='MIT',
     install_requires=install_requires,
```

### Comparing `tejapi-0.1.8/tejapi/connection.py` & `tejapi-0.1.9/tejapi/connection.py`

 * *Files identical despite different names*

### Comparing `tejapi-0.1.8/tejapi/errors/tej_error.py` & `tejapi-0.1.9/tejapi/errors/tej_error.py`

 * *Files identical despite different names*

### Comparing `tejapi-0.1.8/tejapi/get.py` & `tejapi-0.1.9/tejapi/get.py`

 * *Files identical despite different names*

### Comparing `tejapi-0.1.8/tejapi/message.py` & `tejapi-0.1.9/tejapi/message.py`

 * *Files identical despite different names*

### Comparing `tejapi-0.1.8/tejapi/model/data.py` & `tejapi-0.1.9/tejapi/model/data.py`

 * *Files identical despite different names*

### Comparing `tejapi-0.1.8/tejapi/model/database.py` & `tejapi-0.1.9/tejapi/model/database.py`

 * *Files identical despite different names*

### Comparing `tejapi-0.1.8/tejapi/model/data_mixin.py` & `tejapi-0.1.9/tejapi/model/data_mixin.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
         # ensure pandas gets a list of lists
         if data and isinstance(data, list) and not isinstance(data[0], list):
             data = [data]
         if 'columns' in self.meta.keys():
             df = pd.DataFrame(data=data, columns=self.columns)
             for index, type in enumerate(self.column_types):
-                if type == 'Date':
+                if type == 'Date' or type=='datetime':
                     df[self.columns[index]] = df[self.columns[index]].apply(pd.to_datetime)
         else:
             df = pd.DataFrame(data=data, columns=self.column_names)
             # ensure our first column of time series data is of pd.datetime
             df[self.column_names[0]] = df[self.column_names[0]].apply(pd.to_datetime)
             df.set_index(self.column_names[0], inplace=True)
```

### Comparing `tejapi-0.1.8/tejapi/model/merged_data_list.py` & `tejapi-0.1.9/tejapi/model/merged_data_list.py`

 * *Files identical despite different names*

### Comparing `tejapi-0.1.8/tejapi/model/model_base.py` & `tejapi-0.1.9/tejapi/model/model_base.py`

 * *Files identical despite different names*

### Comparing `tejapi-0.1.8/tejapi/model/model_list.py` & `tejapi-0.1.9/tejapi/model/model_list.py`

 * *Files identical despite different names*

### Comparing `tejapi-0.1.8/tejapi/operations/data_list.py` & `tejapi-0.1.9/tejapi/operations/data_list.py`

 * *Files identical despite different names*

### Comparing `tejapi-0.1.8/tejapi/operations/get.py` & `tejapi-0.1.9/tejapi/operations/get.py`

 * *Files identical despite different names*

### Comparing `tejapi-0.1.8/tejapi/operations/list.py` & `tejapi-0.1.9/tejapi/operations/list.py`

 * *Files identical despite different names*

### Comparing `tejapi-0.1.8/tejapi/util.py` & `tejapi-0.1.9/tejapi/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from inflection import parameterize
 import dateutil.parser
+from .api_config import ApiConfig
 import re
 from six import string_types
 
 
 class Util(object):
     @staticmethod
     def constructed_path(path, params={}):
@@ -51,15 +52,15 @@
     @staticmethod
     def convert_to_date(value):
         if isinstance(value, string_types) and re.search(r'^\d{4}-\d{2}-\d{2}$', value):
             # convert to datetime.date
             return dateutil.parser.parse(value).date()
         elif isinstance(value, string_types) and re.search(r'^\d{4}-\d{2}-\d{2}T[\d:\.]+Z$', value):
             # convert to datetime.datetime, default timezone is utc
-            return dateutil.parser.parse(value)
+            return dateutil.parser.parse(value,ignoretz=ApiConfig.ignoretz)
         else:
             return value
 
     @staticmethod
     def convert_options(**options):
         new_options = dict()
         if 'params' in options.keys():
```

### Comparing `tejapi-0.1.8/tejapi.egg-info/SOURCES.txt` & `tejapi-0.1.9/tejapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

