# Comparing `tmp/yplib-0.1.5.tar.gz` & `tmp/yplib-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-0.1.5.tar", last modified: Fri Jun  9 02:43:35 2023, max compression
+gzip compressed data, was "dist\yplib-0.1.6.tar", last modified: Fri Jun  9 03:18:24 2023, max compression
```

## Comparing `yplib-0.1.5.tar` & `yplib-0.1.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 02:43:35.187311 yplib-0.1.5/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-0.1.5/LICENSE
--rw-rw-rw-   0        0        0      567 2023-06-09 02:43:35.186647 yplib-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0      178 2023-06-08 01:05:32.000000 yplib-0.1.5/README.md
--rw-rw-rw-   0        0        0       42 2023-06-09 02:43:35.187311 yplib-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      561 2023-06-09 02:43:02.000000 yplib-0.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-09 02:43:35.184132 yplib-0.1.5/yplib/
--rw-rw-rw-   0        0        0     8315 2023-06-09 02:42:50.000000 yplib-0.1.5/yplib/__init__.py
--rw-rw-rw-   0        0        0     2609 2023-06-09 02:24:26.000000 yplib-0.1.5/yplib/line_stack_temp.py
-drwxrwxrwx   0        0        0        0 2023-06-09 02:43:35.186129 yplib-0.1.5/yplib.egg-info/
--rw-rw-rw-   0        0        0      567 2023-06-09 02:43:35.000000 yplib-0.1.5/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      185 2023-06-09 02:43:35.000000 yplib-0.1.5/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 02:43:35.000000 yplib-0.1.5/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-09 02:43:35.000000 yplib-0.1.5/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 03:18:24.251492 yplib-0.1.6/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0      567 2023-06-09 03:18:24.251386 yplib-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      178 2023-06-08 01:05:32.000000 yplib-0.1.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-09 03:18:24.252512 yplib-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      561 2023-06-09 03:18:09.000000 yplib-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 03:18:24.248525 yplib-0.1.6/yplib/
+-rw-rw-rw-   0        0        0     8379 2023-06-09 03:18:03.000000 yplib-0.1.6/yplib/__init__.py
+-rw-rw-rw-   0        0        0     2609 2023-06-09 02:24:26.000000 yplib-0.1.6/yplib/line_stack_temp.py
+drwxrwxrwx   0        0        0        0 2023-06-09 03:18:24.250575 yplib-0.1.6/yplib.egg-info/
+-rw-rw-rw-   0        0        0      567 2023-06-09 03:18:24.000000 yplib-0.1.6/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      185 2023-06-09 03:18:24.000000 yplib-0.1.6/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 03:18:24.000000 yplib-0.1.6/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-09 03:18:24.000000 yplib-0.1.6/yplib.egg-info/top_level.txt
```

### Comparing `yplib-0.1.5/LICENSE` & `yplib-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-0.1.5/PKG-INFO` & `yplib-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yplib
-Version: 0.1.5
+Version: 0.1.6
 Summary: util
 Home-page: https://github.com/pypa/sampleproject
 Author: yangpu
 Author-email: wantwaterfish@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yplib-0.1.5/setup.py` & `yplib-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="0.1.5",
+  version="0.1.6",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/pypa/sampleproject",
   packages=setuptools.find_packages(),
```

### Comparing `yplib-0.1.5/yplib/__init__.py` & `yplib-0.1.6/yplib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 
 # 将 list 中的数据以 json 或者基本类型的形式写入到文件中
 # list_data : 数组数据
 # file_name : 文件名
 # fixed_name : 是否固定文件名
 # file_path : 文件路径
 def list_to_txt(list_data, file_name, file_path='data', fixed_name=False, suffix='.txt'):
+    file_name = str(file_name)
     while file_path.endswith('/'):
         file_path = file_path[0:-1]
     check_file(file_path)
     if fixed_name is False:
         file_name = get_file_name(file_name, suffix)
     file_name_path = file_name
     if file_path != '':
@@ -84,14 +85,15 @@
     for line in file.readlines():
         line = line.strip()
         data_all.append(line)
     return data_all
 
 
 def list_to_excel(list_data, file_name, file_path='data'):
+    file_name = str(file_name)
     while file_path.endswith('/'):
         file_path = file_path[0:-1]
     check_file(file_path)
     # 2. 创建Excel工作薄
     myWorkbook = xlwt.Workbook()
     # 3. 添加Excel工作表
     mySheet = myWorkbook.add_sheet(str(file_name))
```

### Comparing `yplib-0.1.5/yplib/line_stack_temp.py` & `yplib-0.1.6/yplib/line_stack_temp.py`

 * *Files identical despite different names*

### Comparing `yplib-0.1.5/yplib.egg-info/PKG-INFO` & `yplib-0.1.6/yplib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yplib
-Version: 0.1.5
+Version: 0.1.6
 Summary: util
 Home-page: https://github.com/pypa/sampleproject
 Author: yangpu
 Author-email: wantwaterfish@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

