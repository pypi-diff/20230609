# Comparing `tmp/yplib-0.1.6.tar.gz` & `tmp/yplib-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-0.1.6.tar", last modified: Fri Jun  9 03:18:24 2023, max compression
+gzip compressed data, was "dist\yplib-0.1.7.tar", last modified: Fri Jun  9 06:55:22 2023, max compression
```

## Comparing `yplib-0.1.6.tar` & `yplib-0.1.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 03:18:24.251492 yplib-0.1.6/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-0.1.6/LICENSE
--rw-rw-rw-   0        0        0      567 2023-06-09 03:18:24.251386 yplib-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0      178 2023-06-08 01:05:32.000000 yplib-0.1.6/README.md
--rw-rw-rw-   0        0        0       42 2023-06-09 03:18:24.252512 yplib-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      561 2023-06-09 03:18:09.000000 yplib-0.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-09 03:18:24.248525 yplib-0.1.6/yplib/
--rw-rw-rw-   0        0        0     8379 2023-06-09 03:18:03.000000 yplib-0.1.6/yplib/__init__.py
--rw-rw-rw-   0        0        0     2609 2023-06-09 02:24:26.000000 yplib-0.1.6/yplib/line_stack_temp.py
-drwxrwxrwx   0        0        0        0 2023-06-09 03:18:24.250575 yplib-0.1.6/yplib.egg-info/
--rw-rw-rw-   0        0        0      567 2023-06-09 03:18:24.000000 yplib-0.1.6/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      185 2023-06-09 03:18:24.000000 yplib-0.1.6/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 03:18:24.000000 yplib-0.1.6/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-09 03:18:24.000000 yplib-0.1.6/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 06:55:22.933893 yplib-0.1.7/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0      567 2023-06-09 06:55:22.933893 yplib-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0      178 2023-06-08 01:05:32.000000 yplib-0.1.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-09 06:55:22.934853 yplib-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      561 2023-06-09 06:37:22.000000 yplib-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:55:22.930889 yplib-0.1.7/yplib/
+-rw-rw-rw-   0        0        0     9540 2023-06-09 06:37:38.000000 yplib-0.1.7/yplib/__init__.py
+-rw-rw-rw-   0        0        0     2609 2023-06-09 02:24:26.000000 yplib-0.1.7/yplib/line_stack_temp.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:55:22.933421 yplib-0.1.7/yplib.egg-info/
+-rw-rw-rw-   0        0        0      567 2023-06-09 06:55:22.000000 yplib-0.1.7/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      185 2023-06-09 06:55:22.000000 yplib-0.1.7/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 06:55:22.000000 yplib-0.1.7/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-09 06:55:22.000000 yplib-0.1.7/yplib.egg-info/top_level.txt
```

### Comparing `yplib-0.1.6/LICENSE` & `yplib-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-0.1.6/PKG-INFO` & `yplib-0.1.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yplib
-Version: 0.1.6
+Version: 0.1.7
 Summary: util
 Home-page: https://github.com/pypa/sampleproject
 Author: yangpu
 Author-email: wantwaterfish@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yplib-0.1.6/setup.py` & `yplib-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="0.1.6",
+  version="0.1.7",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/pypa/sampleproject",
   packages=setuptools.find_packages(),
```

### Comparing `yplib-0.1.6/yplib/__init__.py` & `yplib-0.1.7/yplib/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 from datetime import datetime
 
 import xlrd
 import xlwt
 # import random
 from yplib.line_stack_temp import line_stack_temp_html
 
+
+# 记录日志, 如果是对象会转化为 json
 def log(a1='tag', a2='', a3='', a4='', a5='', a6='', a7='', a8='', a9='', a10='', a11='', a12='',
         a13='', a14='', a15='', a16='', a17='', a18='', a19='', a20=''):
     l = [a1, a2, a3, a4, a5, a6, a7, a8, a9, a10,
          a11, a12, a13, a14, a15, a16, a17, a18, a19, a20]
     d = ''
     for one in l:
         if can_use_json(one):
@@ -23,14 +25,21 @@
         if o != '':
             d = d + ' ' + o
     lo = datetime.today().strftime('%Y-%m-%d %H:%M:%S') + d
     print(lo)
     return lo
 
 
+# 将 log 数据, 写入到文件
+def log_to_file(a1='tag', a2='', a3='', a4='', a5='', a6='', a7='', a8='', a9='', a10='', a11='', a12='',
+                a13='', a14='', a15='', a16='', a17='', a18='', a19='', a20=''):
+    lo = log(a1, a2, a3, a4, a5, a6, a7, a8, a9, a10, a11, a12, a13, a14, a15, a16, a17, a18, a19, a20)
+    list_to_txt([lo], datetime.today().strftime('%Y-%m-%d'), 'log', True)
+
+
 # 是否能用 json
 def can_use_json(data):
     if isinstance(data, dict) or isinstance(data, list) or isinstance(data, tuple) or isinstance(data, set):
         return True
     return False
 
 
@@ -44,24 +53,39 @@
 def get_file_name(file_name, suffix='.txt'):
     return str(file_name) \
         + '_' + datetime.today().strftime('%Y%m%d_%H%M%S') \
         + '_' + str(uuid.uuid4().hex).replace('-', '')[0:5] \
         + suffix
 
 
+# 去掉 str 中的 非数字字符, 然后, 再转化为 int
+def str_to_int(s):
+    if s is None or s == '':
+        return 0
+    return int(''.join(filter(lambda ch: ch in '0123456789', s)))
+
+
+# 去掉 str 中的 非数字字符, 然后, 再转化为 float
+def str_to_float(s):
+    if s is None or s == '':
+        return 0.0
+    return float(''.join(filter(lambda ch: ch in '0123456789.', s)))
+
+
 # 将 list 中的数据以 json 或者基本类型的形式写入到文件中
 # list_data : 数组数据
 # file_name : 文件名
 # fixed_name : 是否固定文件名
 # file_path : 文件路径
 def list_to_txt(list_data, file_name, file_path='data', fixed_name=False, suffix='.txt'):
     file_name = str(file_name)
     while file_path.endswith('/'):
         file_path = file_path[0:-1]
     check_file(file_path)
+    file_name = file_name + suffix
     if fixed_name is False:
         file_name = get_file_name(file_name, suffix)
     file_name_path = file_name
     if file_path != '':
         file_name_path = file_path + '/' + file_name
     text_file = open(file_name_path, 'a', encoding='utf-8')
     for one in list_data:
@@ -70,14 +94,15 @@
         else:
             s = str(one)
         text_file.write(s + '\n')
     text_file.close()
     return file_name_path
 
 
+# 将 list 中的数据写入到固定的文件中,自己设置文件后缀
 def list_to_txt_fixed_file_name(list_data, file_name):
     return list_to_txt(list_data, file_name, '', True)
 
 
 # 将 txt 文件读取到 list 中, 每一行自动过滤掉行前,行后的空格
 def txt_to_list(file_name):
     file = open(file_name, 'r', encoding='utf-8')
@@ -242,7 +267,15 @@
 #     # 每条线有 100 个纵坐标, 与 x_list 中的对应起来
 #     for i in range(100):
 #         data.append(int(random.uniform(0, 1000)))
 #     n['data'] = data
 #     y_list.append(n)
 #
 # to_chart(x_list, y_list)
+
+
+# log_to_file(1)
+# log_to_file(12)
+# log_to_file('yangpu')
+# print(str_to_int('yan123gpu'))
+# print(str_to_float('yan123gpu'))
+# print(str_to_float('yan123g.12pu'))
```

### Comparing `yplib-0.1.6/yplib/line_stack_temp.py` & `yplib-0.1.7/yplib/line_stack_temp.py`

 * *Files identical despite different names*

### Comparing `yplib-0.1.6/yplib.egg-info/PKG-INFO` & `yplib-0.1.7/yplib.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yplib
-Version: 0.1.6
+Version: 0.1.7
 Summary: util
 Home-page: https://github.com/pypa/sampleproject
 Author: yangpu
 Author-email: wantwaterfish@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

