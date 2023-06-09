# Comparing `tmp/yplib-0.1.3.tar.gz` & `tmp/yplib-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-0.1.3.tar", last modified: Fri Jun  9 02:32:01 2023, max compression
+gzip compressed data, was "dist\yplib-0.1.4.tar", last modified: Fri Jun  9 02:37:03 2023, max compression
```

## Comparing `yplib-0.1.3.tar` & `yplib-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 02:32:01.633429 yplib-0.1.3/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-0.1.3/LICENSE
--rw-rw-rw-   0        0        0      567 2023-06-09 02:32:01.632952 yplib-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      178 2023-06-08 01:05:32.000000 yplib-0.1.3/README.md
--rw-rw-rw-   0        0        0       42 2023-06-09 02:32:01.633491 yplib-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      561 2023-06-09 02:28:24.000000 yplib-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-09 02:32:01.629492 yplib-0.1.3/yplib/
--rw-rw-rw-   0        0        0     8181 2023-06-09 02:31:43.000000 yplib-0.1.3/yplib/__init__.py
--rw-rw-rw-   0        0        0     2609 2023-06-09 02:24:26.000000 yplib-0.1.3/yplib/line_stack_temp.py
-drwxrwxrwx   0        0        0        0 2023-06-09 02:32:01.632266 yplib-0.1.3/yplib.egg-info/
--rw-rw-rw-   0        0        0      567 2023-06-09 02:32:01.000000 yplib-0.1.3/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      185 2023-06-09 02:32:01.000000 yplib-0.1.3/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 02:32:01.000000 yplib-0.1.3/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-09 02:32:01.000000 yplib-0.1.3/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 02:37:03.482164 yplib-0.1.4/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0      567 2023-06-09 02:37:03.481537 yplib-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      178 2023-06-08 01:05:32.000000 yplib-0.1.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-09 02:37:03.482606 yplib-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      561 2023-06-09 02:36:43.000000 yplib-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 02:37:03.478402 yplib-0.1.4/yplib/
+-rw-rw-rw-   0        0        0     8305 2023-06-09 02:36:17.000000 yplib-0.1.4/yplib/__init__.py
+-rw-rw-rw-   0        0        0     2609 2023-06-09 02:24:26.000000 yplib-0.1.4/yplib/line_stack_temp.py
+drwxrwxrwx   0        0        0        0 2023-06-09 02:37:03.481176 yplib-0.1.4/yplib.egg-info/
+-rw-rw-rw-   0        0        0      567 2023-06-09 02:37:03.000000 yplib-0.1.4/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      185 2023-06-09 02:37:03.000000 yplib-0.1.4/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 02:37:03.000000 yplib-0.1.4/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-09 02:37:03.000000 yplib-0.1.4/yplib.egg-info/top_level.txt
```

### Comparing `yplib-0.1.3/LICENSE` & `yplib-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-0.1.3/PKG-INFO` & `yplib-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yplib
-Version: 0.1.3
+Version: 0.1.4
 Summary: util
 Home-page: https://github.com/pypa/sampleproject
 Author: yangpu
 Author-email: wantwaterfish@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yplib-0.1.3/setup.py` & `yplib-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="0.1.3",
+  version="0.1.4",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/pypa/sampleproject",
   packages=setuptools.find_packages(),
```

### Comparing `yplib-0.1.3/yplib/__init__.py` & `yplib-0.1.4/yplib/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,17 +3,16 @@
 import json
 import os
 import uuid
 from datetime import datetime
 
 import xlrd
 import xlwt
-import random
-from line_stack_temp import line_stack_temp_html
-
+# import random
+from yplib.line_stack_temp import line_stack_temp_html
 
 def log(a1='tag', a2='', a3='', a4='', a5='', a6='', a7='', a8='', a9='', a10='', a11='', a12='',
         a13='', a14='', a15='', a16='', a17='', a18='', a19='', a20=''):
     l = [a1, a2, a3, a4, a5, a6, a7, a8, a9, a10,
          a11, a12, a13, a14, a15, a16, a17, a18, a19, a20]
     d = ''
     for one in l:
@@ -224,20 +223,24 @@
 #     '[{"name":"Email","data":[120,132,101,134,90,230,210]},{"name":"Union Ads","data":[220,182,191,234,290,330,310]},{"name":"Video Ads","data":[150,232,201,154,190,330,410]},{"name":"Direct","data":[320,332,301,334,390,330,320]},{"name":"Search Engine","data":[820,932,901,934,1290,1330,1320]}]')
 #
 # x_list = []
 # y_list = []
 #
 # # to_chart(x_list, y_list)
 #
-# for i in range(100):  # 0 1 2 3 4 5
+# # x 轴有 100 个
+# # 100 个横坐标
+# for i in range(100):
 #     x_list.append(i)
 #
+# # 有 10 条线
 # for i in range(10):  # 0 1 2 3 4 55
 #     n = {}
 #     n['name'] = str(int(random.uniform(0, 1000)))
 #     data = []
+#     # 每条线有 100 个纵坐标, 与 x_list 中的对应起来
 #     for i in range(100):
 #         data.append(int(random.uniform(0, 1000)))
 #     n['data'] = data
 #     y_list.append(n)
 #
 # to_chart(x_list, y_list)
```

### Comparing `yplib-0.1.3/yplib/line_stack_temp.py` & `yplib-0.1.4/yplib/line_stack_temp.py`

 * *Files identical despite different names*

### Comparing `yplib-0.1.3/yplib.egg-info/PKG-INFO` & `yplib-0.1.4/yplib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yplib
-Version: 0.1.3
+Version: 0.1.4
 Summary: util
 Home-page: https://github.com/pypa/sampleproject
 Author: yangpu
 Author-email: wantwaterfish@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

