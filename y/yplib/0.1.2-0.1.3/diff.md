# Comparing `tmp/yplib-0.1.2.tar.gz` & `tmp/yplib-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-0.1.2.tar", last modified: Fri Jun  9 02:18:56 2023, max compression
+gzip compressed data, was "dist\yplib-0.1.3.tar", last modified: Fri Jun  9 02:32:01 2023, max compression
```

## Comparing `yplib-0.1.2.tar` & `yplib-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 02:18:56.775154 yplib-0.1.2/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      567 2023-06-09 02:18:56.774637 yplib-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      178 2023-06-08 01:05:32.000000 yplib-0.1.2/README.md
--rw-rw-rw-   0        0        0       42 2023-06-09 02:18:56.775154 yplib-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      561 2023-06-09 02:18:27.000000 yplib-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-09 02:18:56.772016 yplib-0.1.2/yplib/
--rw-rw-rw-   0        0        0     8130 2023-06-09 02:18:08.000000 yplib-0.1.2/yplib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 02:18:56.774137 yplib-0.1.2/yplib.egg-info/
--rw-rw-rw-   0        0        0      567 2023-06-09 02:18:56.000000 yplib-0.1.2/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      160 2023-06-09 02:18:56.000000 yplib-0.1.2/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 02:18:56.000000 yplib-0.1.2/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-09 02:18:56.000000 yplib-0.1.2/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 02:32:01.633429 yplib-0.1.3/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      567 2023-06-09 02:32:01.632952 yplib-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      178 2023-06-08 01:05:32.000000 yplib-0.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-09 02:32:01.633491 yplib-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      561 2023-06-09 02:28:24.000000 yplib-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 02:32:01.629492 yplib-0.1.3/yplib/
+-rw-rw-rw-   0        0        0     8181 2023-06-09 02:31:43.000000 yplib-0.1.3/yplib/__init__.py
+-rw-rw-rw-   0        0        0     2609 2023-06-09 02:24:26.000000 yplib-0.1.3/yplib/line_stack_temp.py
+drwxrwxrwx   0        0        0        0 2023-06-09 02:32:01.632266 yplib-0.1.3/yplib.egg-info/
+-rw-rw-rw-   0        0        0      567 2023-06-09 02:32:01.000000 yplib-0.1.3/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      185 2023-06-09 02:32:01.000000 yplib-0.1.3/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 02:32:01.000000 yplib-0.1.3/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-09 02:32:01.000000 yplib-0.1.3/yplib.egg-info/top_level.txt
```

### Comparing `yplib-0.1.2/LICENSE` & `yplib-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-0.1.2/PKG-INFO` & `yplib-0.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yplib
-Version: 0.1.2
+Version: 0.1.3
 Summary: util
 Home-page: https://github.com/pypa/sampleproject
 Author: yangpu
 Author-email: wantwaterfish@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yplib-0.1.2/setup.py` & `yplib-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="0.1.2",
+  version="0.1.3",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/pypa/sampleproject",
   packages=setuptools.find_packages(),
```

### Comparing `yplib-0.1.2/yplib/__init__.py` & `yplib-0.1.3/yplib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import os
 import uuid
 from datetime import datetime
 
 import xlrd
 import xlwt
 import random
+from line_stack_temp import line_stack_temp_html
 
 
 def log(a1='tag', a2='', a3='', a4='', a5='', a6='', a7='', a8='', a9='', a10='', a11='', a12='',
         a13='', a14='', a15='', a16='', a17='', a18='', a19='', a20=''):
     l = [a1, a2, a3, a4, a5, a6, a7, a8, a9, a10,
          a11, a12, a13, a14, a15, a16, a17, a18, a19, a20]
     d = ''
@@ -157,17 +158,18 @@
 #                 data: [320, 332, 301, 334, 390, 330, 320],
 #             },
 #             {
 #                 name: 'Search Engine',
 #                 data: [820, 932, 901, 934, 1290, 1330, 1320],
 #             },
 #         ]
-def to_chart(x_list, y_list, chart_name='折线图堆叠'):
-    current_path = os.path.abspath(__file__)
-    html_list = open(current_path[0:current_path.find('__init__')] + 'line-stack-temp.html', 'r', encoding='utf-8').readlines()
+def to_chart(x_list, y_list, chart_name='stack_line'):
+    # current_path = os.path.abspath(__file__)
+    # html_list = open(current_path[0:current_path.find('__init__')] + 'line-stack-temp.html', 'r', encoding='utf-8').readlines()
+    html_list_one = line_stack_temp_html()
     chart_name_html = '-chart_name-'
     x_list_html = '-x_list-'
     legend_html = '-legend-'
     series_html = '-series-'
     r_list = []
     # data: ['Email', 'Union Ads', 'Video Ads', 'Direct', 'Search Engine']
     legend_data = []
@@ -185,25 +187,25 @@
     #             }
     series = []
     for y_one in y_list:
         y_one['type'] = 'line'
         y_one['stack'] = 'Total'
         series.append(y_one)
 
-    for one_line in html_list:
-        if one_line.find(chart_name_html) > -1:
-            one_line = one_line.replace(chart_name_html, chart_name)
-        if one_line.find(x_list_html) > -1:
-            # ['Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat', 'Sun']
-            one_line = one_line.replace(x_list_html, str(x_list))
-        if one_line.find(legend_html) > -1:
-            one_line = one_line.replace(legend_html, str(legend))
-        if one_line.find(series_html) > -1:
-            one_line = one_line.replace(series_html, str(series))
-        r_list.append(one_line)
+    one_line = html_list_one
+    if one_line.find(chart_name_html) > -1:
+        one_line = one_line.replace(chart_name_html, chart_name)
+    if one_line.find(x_list_html) > -1:
+        # ['Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat', 'Sun']
+        one_line = one_line.replace(x_list_html, str(x_list))
+    if one_line.find(legend_html) > -1:
+        one_line = one_line.replace(legend_html, str(legend))
+    if one_line.find(series_html) > -1:
+        one_line = one_line.replace(series_html, str(series))
+    r_list.append(one_line)
     list_to_txt(r_list, chart_name, 'html', False, '.html')
 
 
 # list_to_txt([1,2,3], 'p')
 # list_to_txt_fixed_file_name([1,2,3], 'p')
 #
 #
```

### Comparing `yplib-0.1.2/yplib.egg-info/PKG-INFO` & `yplib-0.1.3/yplib.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yplib
-Version: 0.1.2
+Version: 0.1.3
 Summary: util
 Home-page: https://github.com/pypa/sampleproject
 Author: yangpu
 Author-email: wantwaterfish@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

