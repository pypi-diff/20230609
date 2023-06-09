# Comparing `tmp/yplib-0.1.8.tar.gz` & `tmp/yplib-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-0.1.8.tar", last modified: Fri Jun  9 07:02:50 2023, max compression
+gzip compressed data, was "dist\yplib-0.1.9.tar", last modified: Fri Jun  9 07:59:35 2023, max compression
```

## Comparing `yplib-0.1.8.tar` & `yplib-0.1.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 07:02:50.595928 yplib-0.1.8/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-0.1.8/LICENSE
--rw-rw-rw-   0        0        0      567 2023-06-09 07:02:50.595499 yplib-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0      178 2023-06-08 01:05:32.000000 yplib-0.1.8/README.md
--rw-rw-rw-   0        0        0       42 2023-06-09 07:02:50.595928 yplib-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      561 2023-06-09 07:02:30.000000 yplib-0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-09 07:02:50.592400 yplib-0.1.8/yplib/
--rw-rw-rw-   0        0        0     9475 2023-06-09 07:02:02.000000 yplib-0.1.8/yplib/__init__.py
--rw-rw-rw-   0        0        0     2609 2023-06-09 02:24:26.000000 yplib-0.1.8/yplib/line_stack_temp.py
-drwxrwxrwx   0        0        0        0 2023-06-09 07:02:50.594189 yplib-0.1.8/yplib.egg-info/
--rw-rw-rw-   0        0        0      567 2023-06-09 07:02:50.000000 yplib-0.1.8/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      185 2023-06-09 07:02:50.000000 yplib-0.1.8/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 07:02:50.000000 yplib-0.1.8/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-09 07:02:50.000000 yplib-0.1.8/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 07:59:35.690467 yplib-0.1.9/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0      567 2023-06-09 07:59:35.690155 yplib-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      178 2023-06-08 01:05:32.000000 yplib-0.1.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-09 07:59:35.690999 yplib-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      561 2023-06-09 07:59:17.000000 yplib-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 07:59:35.686970 yplib-0.1.9/yplib/
+-rw-rw-rw-   0        0        0     9490 2023-06-09 07:58:57.000000 yplib-0.1.9/yplib/__init__.py
+-rw-rw-rw-   0        0        0     2609 2023-06-09 02:24:26.000000 yplib-0.1.9/yplib/line_stack_temp.py
+drwxrwxrwx   0        0        0        0 2023-06-09 07:59:35.689643 yplib-0.1.9/yplib.egg-info/
+-rw-rw-rw-   0        0        0      567 2023-06-09 07:59:35.000000 yplib-0.1.9/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      185 2023-06-09 07:59:35.000000 yplib-0.1.9/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 07:59:35.000000 yplib-0.1.9/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-09 07:59:35.000000 yplib-0.1.9/yplib.egg-info/top_level.txt
```

### Comparing `yplib-0.1.8/LICENSE` & `yplib-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-0.1.8/PKG-INFO` & `yplib-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yplib
-Version: 0.1.8
+Version: 0.1.9
 Summary: util
 Home-page: https://github.com/pypa/sampleproject
 Author: yangpu
 Author-email: wantwaterfish@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yplib-0.1.8/setup.py` & `yplib-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="0.1.8",
+  version="0.1.9",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/pypa/sampleproject",
   packages=setuptools.find_packages(),
```

### Comparing `yplib-0.1.8/yplib/__init__.py` & `yplib-0.1.9/yplib/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,16 +77,17 @@
 # fixed_name : 是否固定文件名
 # file_path : 文件路径
 def list_to_txt(list_data, file_name, file_path='data', fixed_name=False, suffix='.txt'):
     file_name = str(file_name)
     while file_path.endswith('/'):
         file_path = file_path[0:-1]
     check_file(file_path)
-    file_name = file_name + suffix
     if fixed_name is False:
+        file_name = file_name + suffix
+    else:
         file_name = get_file_name(file_name, suffix)
     file_name_path = file_name
     if file_path != '':
         file_name_path = file_path + '/' + file_name
     text_file = open(file_name_path, 'a', encoding='utf-8')
     for one in list_data:
         if can_use_json(one):
```

### Comparing `yplib-0.1.8/yplib/line_stack_temp.py` & `yplib-0.1.9/yplib/line_stack_temp.py`

 * *Files identical despite different names*

### Comparing `yplib-0.1.8/yplib.egg-info/PKG-INFO` & `yplib-0.1.9/yplib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yplib
-Version: 0.1.8
+Version: 0.1.9
 Summary: util
 Home-page: https://github.com/pypa/sampleproject
 Author: yangpu
 Author-email: wantwaterfish@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

