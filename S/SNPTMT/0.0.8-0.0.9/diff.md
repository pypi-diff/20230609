# Comparing `tmp/SNPTMT-0.0.8.tar.gz` & `tmp/SNPTMT-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SNPTMT-0.0.8.tar", last modified: Sun May 28 16:07:25 2023, max compression
+gzip compressed data, was "SNPTMT-0.0.9.tar", last modified: Sun May 28 16:20:02 2023, max compression
```

## Comparing `SNPTMT-0.0.8.tar` & `SNPTMT-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 andrewshatalov   (501) staff       (20)        0 2023-05-28 16:07:25.103114 SNPTMT-0.0.8/
--rw-r--r--   0 andrewshatalov   (501) staff       (20)     1111 2023-05-27 08:38:07.000000 SNPTMT-0.0.8/LICENSE
--rw-r--r--   0 andrewshatalov   (501) staff       (20)      571 2023-05-28 16:07:25.103188 SNPTMT-0.0.8/PKG-INFO
--rw-r--r--   0 andrewshatalov   (501) staff       (20)        8 2023-05-26 20:22:56.000000 SNPTMT-0.0.8/README.md
-drwxr-xr-x   0 andrewshatalov   (501) staff       (20)        0 2023-05-28 16:07:25.102083 SNPTMT-0.0.8/SNPTMT/
--rw-r--r--   0 andrewshatalov   (501) staff       (20)      332 2023-05-27 08:58:59.000000 SNPTMT-0.0.8/SNPTMT/__init__.py
--rw-r--r--   0 andrewshatalov   (501) staff       (20)     8728 2023-05-28 16:06:27.000000 SNPTMT-0.0.8/SNPTMT/snptmt.py
-drwxr-xr-x   0 andrewshatalov   (501) staff       (20)        0 2023-05-28 16:07:25.102740 SNPTMT-0.0.8/SNPTMT.egg-info/
--rw-r--r--   0 andrewshatalov   (501) staff       (20)      571 2023-05-28 16:07:25.000000 SNPTMT-0.0.8/SNPTMT.egg-info/PKG-INFO
--rw-r--r--   0 andrewshatalov   (501) staff       (20)      312 2023-05-28 16:07:25.000000 SNPTMT-0.0.8/SNPTMT.egg-info/SOURCES.txt
--rw-r--r--   0 andrewshatalov   (501) staff       (20)        1 2023-05-28 16:07:25.000000 SNPTMT-0.0.8/SNPTMT.egg-info/dependency_links.txt
--rw-r--r--   0 andrewshatalov   (501) staff       (20)        7 2023-05-28 16:07:25.000000 SNPTMT-0.0.8/SNPTMT.egg-info/top_level.txt
--rw-r--r--   0 andrewshatalov   (501) staff       (20)       38 2023-05-28 16:07:25.103464 SNPTMT-0.0.8/setup.cfg
--rw-r--r--   0 andrewshatalov   (501) staff       (20)      945 2023-05-28 16:06:44.000000 SNPTMT-0.0.8/setup.py
+drwxr-xr-x   0 andrewshatalov   (501) staff       (20)        0 2023-05-28 16:20:02.509743 SNPTMT-0.0.9/
+-rw-r--r--   0 andrewshatalov   (501) staff       (20)     1111 2023-05-27 08:38:07.000000 SNPTMT-0.0.9/LICENSE
+-rw-r--r--   0 andrewshatalov   (501) staff       (20)      571 2023-05-28 16:20:02.509821 SNPTMT-0.0.9/PKG-INFO
+-rw-r--r--   0 andrewshatalov   (501) staff       (20)        8 2023-05-26 20:22:56.000000 SNPTMT-0.0.9/README.md
+drwxr-xr-x   0 andrewshatalov   (501) staff       (20)        0 2023-05-28 16:20:02.508669 SNPTMT-0.0.9/SNPTMT/
+-rw-r--r--   0 andrewshatalov   (501) staff       (20)      332 2023-05-27 08:58:59.000000 SNPTMT-0.0.9/SNPTMT/__init__.py
+-rw-r--r--   0 andrewshatalov   (501) staff       (20)     8740 2023-05-28 16:19:42.000000 SNPTMT-0.0.9/SNPTMT/snptmt.py
+drwxr-xr-x   0 andrewshatalov   (501) staff       (20)        0 2023-05-28 16:20:02.509340 SNPTMT-0.0.9/SNPTMT.egg-info/
+-rw-r--r--   0 andrewshatalov   (501) staff       (20)      571 2023-05-28 16:20:02.000000 SNPTMT-0.0.9/SNPTMT.egg-info/PKG-INFO
+-rw-r--r--   0 andrewshatalov   (501) staff       (20)      312 2023-05-28 16:20:02.000000 SNPTMT-0.0.9/SNPTMT.egg-info/SOURCES.txt
+-rw-r--r--   0 andrewshatalov   (501) staff       (20)        1 2023-05-28 16:20:02.000000 SNPTMT-0.0.9/SNPTMT.egg-info/dependency_links.txt
+-rw-r--r--   0 andrewshatalov   (501) staff       (20)        7 2023-05-28 16:20:02.000000 SNPTMT-0.0.9/SNPTMT.egg-info/top_level.txt
+-rw-r--r--   0 andrewshatalov   (501) staff       (20)       38 2023-05-28 16:20:02.510088 SNPTMT-0.0.9/setup.cfg
+-rw-r--r--   0 andrewshatalov   (501) staff       (20)      945 2023-05-28 16:19:49.000000 SNPTMT-0.0.9/setup.py
```

### Comparing `SNPTMT-0.0.8/LICENSE` & `SNPTMT-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `SNPTMT-0.0.8/PKG-INFO` & `SNPTMT-0.0.9/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SNPTMT
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python module for searching for a new popular topics in the message threade
 Home-page: https://github.com/FIvER4IK/snptmt
 Download-URL: 
 Author: FIvER4IK
 Author-email: andrewshatalov3@gmail.com
 Keywords: clusters clustering short text search new popular topics message thread
 Classifier: Programming Language :: Python
```

### Comparing `SNPTMT-0.0.8/SNPTMT/snptmt.py` & `SNPTMT-0.0.9/SNPTMT/snptmt.py`

 * *Files 0% similar despite different names*

```diff
@@ -152,15 +152,15 @@
     #add points from prev clustering to list prev_points
     prev_points = []
     for points in half_cluster_dict.values():
         prev_points.extend(points)
     
     #make actual indexes
     prev_points = list(map(lambda x: x + start_message, prev_points))
-    
+    ssssssssssss
     #print(prev_points)
     
     #add new points to prev_points
     for i in range(start_message, end_message+1):
         prev_points.append(i)
         
     #print(prev_points)
```

### Comparing `SNPTMT-0.0.8/SNPTMT.egg-info/PKG-INFO` & `SNPTMT-0.0.9/SNPTMT.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SNPTMT
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python module for searching for a new popular topics in the message threade
 Home-page: https://github.com/FIvER4IK/snptmt
 Download-URL: 
 Author: FIvER4IK
 Author-email: andrewshatalov3@gmail.com
 Keywords: clusters clustering short text search new popular topics message thread
 Classifier: Programming Language :: Python
```

### Comparing `SNPTMT-0.0.8/setup.py` & `SNPTMT-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 def readme():
   with open('README.md', 'r') as f:
     return f.read()
 
-version = '0.0.8'
+version = '0.0.9'
 
 setup(
     name='SNPTMT',
     version=version,
 
     author='FIvER4IK',
     author_email='andrewshatalov3@gmail.com',
```

