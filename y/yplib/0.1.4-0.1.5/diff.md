# Comparing `tmp/yplib-0.1.4.tar.gz` & `tmp/yplib-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-0.1.4.tar", last modified: Fri Jun  9 02:37:03 2023, max compression
+gzip compressed data, was "dist\yplib-0.1.5.tar", last modified: Fri Jun  9 02:43:35 2023, max compression
```

## Comparing `yplib-0.1.4.tar` & `yplib-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 02:37:03.482164 yplib-0.1.4/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-0.1.4/LICENSE
--rw-rw-rw-   0        0        0      567 2023-06-09 02:37:03.481537 yplib-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0      178 2023-06-08 01:05:32.000000 yplib-0.1.4/README.md
--rw-rw-rw-   0        0        0       42 2023-06-09 02:37:03.482606 yplib-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      561 2023-06-09 02:36:43.000000 yplib-0.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-09 02:37:03.478402 yplib-0.1.4/yplib/
--rw-rw-rw-   0        0        0     8305 2023-06-09 02:36:17.000000 yplib-0.1.4/yplib/__init__.py
--rw-rw-rw-   0        0        0     2609 2023-06-09 02:24:26.000000 yplib-0.1.4/yplib/line_stack_temp.py
-drwxrwxrwx   0        0        0        0 2023-06-09 02:37:03.481176 yplib-0.1.4/yplib.egg-info/
--rw-rw-rw-   0        0        0      567 2023-06-09 02:37:03.000000 yplib-0.1.4/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      185 2023-06-09 02:37:03.000000 yplib-0.1.4/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 02:37:03.000000 yplib-0.1.4/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-09 02:37:03.000000 yplib-0.1.4/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 02:43:35.187311 yplib-0.1.5/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0      567 2023-06-09 02:43:35.186647 yplib-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      178 2023-06-08 01:05:32.000000 yplib-0.1.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-09 02:43:35.187311 yplib-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      561 2023-06-09 02:43:02.000000 yplib-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 02:43:35.184132 yplib-0.1.5/yplib/
+-rw-rw-rw-   0        0        0     8315 2023-06-09 02:42:50.000000 yplib-0.1.5/yplib/__init__.py
+-rw-rw-rw-   0        0        0     2609 2023-06-09 02:24:26.000000 yplib-0.1.5/yplib/line_stack_temp.py
+drwxrwxrwx   0        0        0        0 2023-06-09 02:43:35.186129 yplib-0.1.5/yplib.egg-info/
+-rw-rw-rw-   0        0        0      567 2023-06-09 02:43:35.000000 yplib-0.1.5/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      185 2023-06-09 02:43:35.000000 yplib-0.1.5/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 02:43:35.000000 yplib-0.1.5/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-09 02:43:35.000000 yplib-0.1.5/yplib.egg-info/top_level.txt
```

### Comparing `yplib-0.1.4/LICENSE` & `yplib-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-0.1.4/PKG-INFO` & `yplib-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yplib
-Version: 0.1.4
+Version: 0.1.5
 Summary: util
 Home-page: https://github.com/pypa/sampleproject
 Author: yangpu
 Author-email: wantwaterfish@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yplib-0.1.4/setup.py` & `yplib-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="0.1.4",
+  version="0.1.5",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/pypa/sampleproject",
   packages=setuptools.find_packages(),
```

### Comparing `yplib-0.1.4/yplib/__init__.py` & `yplib-0.1.5/yplib/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,24 +188,24 @@
     for y_one in y_list:
         y_one['type'] = 'line'
         y_one['stack'] = 'Total'
         series.append(y_one)
 
     one_line = html_list_one
     if one_line.find(chart_name_html) > -1:
-        one_line = one_line.replace(chart_name_html, chart_name)
+        one_line = one_line.replace(chart_name_html, str(chart_name))
     if one_line.find(x_list_html) > -1:
         # ['Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat', 'Sun']
         one_line = one_line.replace(x_list_html, str(x_list))
     if one_line.find(legend_html) > -1:
         one_line = one_line.replace(legend_html, str(legend))
     if one_line.find(series_html) > -1:
         one_line = one_line.replace(series_html, str(series))
     r_list.append(one_line)
-    list_to_txt(r_list, chart_name, 'html', False, '.html')
+    list_to_txt(r_list, str(chart_name), 'html', False, '.html')
 
 
 # list_to_txt([1,2,3], 'p')
 # list_to_txt_fixed_file_name([1,2,3], 'p')
 #
 #
 # li = txt_to_list('D:\code\python3\packaging_tutorial\yplib\data\p_20230609_081711_78ff6.txt')
```

### Comparing `yplib-0.1.4/yplib/line_stack_temp.py` & `yplib-0.1.5/yplib/line_stack_temp.py`

 * *Files identical despite different names*

### Comparing `yplib-0.1.4/yplib.egg-info/PKG-INFO` & `yplib-0.1.5/yplib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yplib
-Version: 0.1.4
+Version: 0.1.5
 Summary: util
 Home-page: https://github.com/pypa/sampleproject
 Author: yangpu
 Author-email: wantwaterfish@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

