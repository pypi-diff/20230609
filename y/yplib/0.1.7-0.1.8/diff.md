# Comparing `tmp/yplib-0.1.7.tar.gz` & `tmp/yplib-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-0.1.7.tar", last modified: Fri Jun  9 06:55:22 2023, max compression
+gzip compressed data, was "dist\yplib-0.1.8.tar", last modified: Fri Jun  9 07:02:50 2023, max compression
```

## Comparing `yplib-0.1.7.tar` & `yplib-0.1.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 06:55:22.933893 yplib-0.1.7/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-0.1.7/LICENSE
--rw-rw-rw-   0        0        0      567 2023-06-09 06:55:22.933893 yplib-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0      178 2023-06-08 01:05:32.000000 yplib-0.1.7/README.md
--rw-rw-rw-   0        0        0       42 2023-06-09 06:55:22.934853 yplib-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      561 2023-06-09 06:37:22.000000 yplib-0.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-09 06:55:22.930889 yplib-0.1.7/yplib/
--rw-rw-rw-   0        0        0     9540 2023-06-09 06:37:38.000000 yplib-0.1.7/yplib/__init__.py
--rw-rw-rw-   0        0        0     2609 2023-06-09 02:24:26.000000 yplib-0.1.7/yplib/line_stack_temp.py
-drwxrwxrwx   0        0        0        0 2023-06-09 06:55:22.933421 yplib-0.1.7/yplib.egg-info/
--rw-rw-rw-   0        0        0      567 2023-06-09 06:55:22.000000 yplib-0.1.7/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      185 2023-06-09 06:55:22.000000 yplib-0.1.7/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 06:55:22.000000 yplib-0.1.7/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-09 06:55:22.000000 yplib-0.1.7/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 07:02:50.595928 yplib-0.1.8/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0      567 2023-06-09 07:02:50.595499 yplib-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0      178 2023-06-08 01:05:32.000000 yplib-0.1.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-09 07:02:50.595928 yplib-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      561 2023-06-09 07:02:30.000000 yplib-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 07:02:50.592400 yplib-0.1.8/yplib/
+-rw-rw-rw-   0        0        0     9475 2023-06-09 07:02:02.000000 yplib-0.1.8/yplib/__init__.py
+-rw-rw-rw-   0        0        0     2609 2023-06-09 02:24:26.000000 yplib-0.1.8/yplib/line_stack_temp.py
+drwxrwxrwx   0        0        0        0 2023-06-09 07:02:50.594189 yplib-0.1.8/yplib.egg-info/
+-rw-rw-rw-   0        0        0      567 2023-06-09 07:02:50.000000 yplib-0.1.8/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      185 2023-06-09 07:02:50.000000 yplib-0.1.8/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 07:02:50.000000 yplib-0.1.8/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-09 07:02:50.000000 yplib-0.1.8/yplib.egg-info/top_level.txt
```

### Comparing `yplib-0.1.7/LICENSE` & `yplib-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-0.1.7/PKG-INFO` & `yplib-0.1.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yplib
-Version: 0.1.7
+Version: 0.1.8
 Summary: util
 Home-page: https://github.com/pypa/sampleproject
 Author: yangpu
 Author-email: wantwaterfish@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yplib-0.1.7/setup.py` & `yplib-0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="0.1.7",
+  version="0.1.8",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/pypa/sampleproject",
   packages=setuptools.find_packages(),
```

### Comparing `yplib-0.1.7/yplib/__init__.py` & `yplib-0.1.8/yplib/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -214,27 +214,26 @@
     series = []
     for y_one in y_list:
         y_one['type'] = 'line'
         y_one['stack'] = 'Total'
         series.append(y_one)
 
     one_line = html_list_one
-    if one_line.find(chart_name_html) > -1:
+    if chart_name_html in one_line:
         one_line = one_line.replace(chart_name_html, str(chart_name))
-    if one_line.find(x_list_html) > -1:
+    if x_list_html in one_line:
         # ['Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat', 'Sun']
         one_line = one_line.replace(x_list_html, str(x_list))
-    if one_line.find(legend_html) > -1:
+    if legend_html in one_line:
         one_line = one_line.replace(legend_html, str(legend))
-    if one_line.find(series_html) > -1:
+    if series_html in one_line:
         one_line = one_line.replace(series_html, str(series))
     r_list.append(one_line)
     list_to_txt(r_list, str(chart_name), 'html', False, '.html')
 
-
 # list_to_txt([1,2,3], 'p')
 # list_to_txt_fixed_file_name([1,2,3], 'p')
 #
 #
 # li = txt_to_list('D:\code\python3\packaging_tutorial\yplib\data\p_20230609_081711_78ff6.txt')
 #
 # print(log())
@@ -245,19 +244,18 @@
 # log(1, 2, [1, 2])
 # log(1, 2, [{'a': 2}])
 #
 # x_list = ['Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat', 'Sun']
 # y_list = json.loads(
 #     '[{"name":"Email","data":[120,132,101,134,90,230,210]},{"name":"Union Ads","data":[220,182,191,234,290,330,310]},{"name":"Video Ads","data":[150,232,201,154,190,330,410]},{"name":"Direct","data":[320,332,301,334,390,330,320]},{"name":"Search Engine","data":[820,932,901,934,1290,1330,1320]}]')
 #
+
+#
 # x_list = []
 # y_list = []
-#
-# # to_chart(x_list, y_list)
-#
 # # x 轴有 100 个
 # # 100 个横坐标
 # for i in range(100):
 #     x_list.append(i)
 #
 # # 有 10 条线
 # for i in range(10):  # 0 1 2 3 4 55
```

### Comparing `yplib-0.1.7/yplib/line_stack_temp.py` & `yplib-0.1.8/yplib/line_stack_temp.py`

 * *Files identical despite different names*

### Comparing `yplib-0.1.7/yplib.egg-info/PKG-INFO` & `yplib-0.1.8/yplib.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yplib
-Version: 0.1.7
+Version: 0.1.8
 Summary: util
 Home-page: https://github.com/pypa/sampleproject
 Author: yangpu
 Author-email: wantwaterfish@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

