# Comparing `tmp/yplib-0.0.7.tar.gz` & `tmp/yplib-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-0.0.7.tar", last modified: Thu Jun  8 03:18:34 2023, max compression
+gzip compressed data, was "dist\yplib-0.0.9.tar", last modified: Thu Jun  8 06:11:42 2023, max compression
```

## Comparing `yplib-0.0.7.tar` & `yplib-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 03:18:34.475913 yplib-0.0.7/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-0.0.7/LICENSE
--rw-rw-rw-   0        0        0      567 2023-06-08 03:18:34.475790 yplib-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      178 2023-06-08 01:05:32.000000 yplib-0.0.7/README.md
--rw-rw-rw-   0        0        0       42 2023-06-08 03:18:34.475913 yplib-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      561 2023-06-08 03:18:24.000000 yplib-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-08 03:18:34.473039 yplib-0.0.7/yplib/
--rw-rw-rw-   0        0        0     3155 2023-06-08 03:18:17.000000 yplib-0.0.7/yplib/__init__.py
--rw-rw-rw-   0        0        0       43 2023-06-08 00:54:48.000000 yplib-0.0.7/yplib/example.py
-drwxrwxrwx   0        0        0        0 2023-06-08 03:18:34.475178 yplib-0.0.7/yplib.egg-info/
--rw-rw-rw-   0        0        0      567 2023-06-08 03:18:34.000000 yplib-0.0.7/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      177 2023-06-08 03:18:34.000000 yplib-0.0.7/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 03:18:34.000000 yplib-0.0.7/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-08 03:18:34.000000 yplib-0.0.7/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-08 06:11:42.219187 yplib-0.0.9/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      567 2023-06-08 06:11:42.218962 yplib-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      178 2023-06-08 01:05:32.000000 yplib-0.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-08 06:11:42.219561 yplib-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      561 2023-06-08 06:11:07.000000 yplib-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 06:11:42.216271 yplib-0.0.9/yplib/
+-rw-rw-rw-   0        0        0     3280 2023-06-08 06:09:36.000000 yplib-0.0.9/yplib/__init__.py
+-rw-rw-rw-   0        0        0       43 2023-06-08 00:54:48.000000 yplib-0.0.9/yplib/example.py
+drwxrwxrwx   0        0        0        0 2023-06-08 06:11:42.218414 yplib-0.0.9/yplib.egg-info/
+-rw-rw-rw-   0        0        0      567 2023-06-08 06:11:42.000000 yplib-0.0.9/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      177 2023-06-08 06:11:42.000000 yplib-0.0.9/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 06:11:42.000000 yplib-0.0.9/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-08 06:11:42.000000 yplib-0.0.9/yplib.egg-info/top_level.txt
```

### Comparing `yplib-0.0.7/LICENSE` & `yplib-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-0.0.7/PKG-INFO` & `yplib-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yplib
-Version: 0.0.7
+Version: 0.0.9
 Summary: util
 Home-page: https://github.com/pypa/sampleproject
 Author: yangpu
 Author-email: wantwaterfish@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yplib-0.0.7/setup.py` & `yplib-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="0.0.7",
+  version="0.0.9",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/pypa/sampleproject",
   packages=setuptools.find_packages(),
```

### Comparing `yplib-0.0.7/yplib/__init__.py` & `yplib-0.0.9/yplib/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 import uuid
 from datetime import datetime
 
 import xlrd
 import xlwt
 
 
+def log(tag='tag'):
+    print(datetime.today().strftime('%Y-%m-%d %H:%M:%S') + ' ' + str(tag))
+
+
 # 检查文件夹是否存在,不存在,就创建新的
 def check_file(file_name):
     if os.path.exists(file_name) is False:
         os.mkdir(file_name)
 
 
 # 获得文件名称
@@ -47,14 +51,15 @@
         data_all.append(line)
     return data_all
 
 
 def list_to_excel(list_data, file_name, file_path='data'):
     while file_path.endswith('/'):
         file_path = file_path[0:-1]
+    check_file(file_path)
     # 2. 创建Excel工作薄
     myWorkbook = xlwt.Workbook()
     # 3. 添加Excel工作表
     mySheet = myWorkbook.add_sheet(str(file_name))
     # 4. 写入数据
     # myStyle = xlwt.easyxf('font: name Times New Roman, color-index red, bold on')  # 数据格式
     m = 0
@@ -86,10 +91,10 @@
     book = xlrd.open_workbook(file_name)  # 打开一个excel
     sheet = book.sheet_by_index(sheet_index)  # 根据顺序获取sheet
     data_list = list()
     for i in range(sheet.nrows):  # 0 1 2 3 4 5
         rows = sheet.row_values(i)
         row_data = []
         for j in range(len(rows)):
-            row_data.append(str(rows(i)[j]).strip())
+            row_data.append(str(rows[j]).strip())
         data_list.append(row_data)
     return data_list
```

### Comparing `yplib-0.0.7/yplib.egg-info/PKG-INFO` & `yplib-0.0.9/yplib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yplib
-Version: 0.0.7
+Version: 0.0.9
 Summary: util
 Home-page: https://github.com/pypa/sampleproject
 Author: yangpu
 Author-email: wantwaterfish@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

