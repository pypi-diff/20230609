# Comparing `tmp/pascal_voc-0.0.4.tar.gz` & `tmp/pascal_voc-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pascal_voc-0.0.4.tar", last modified: Thu Jun  8 20:53:57 2023, max compression
+gzip compressed data, was "pascal_voc-0.0.5.tar", last modified: Thu Jun  8 22:24:56 2023, max compression
```

## Comparing `pascal_voc-0.0.4.tar` & `pascal_voc-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0 alexander  (1000) alexander  (1000)        0 2023-06-08 20:53:57.665713 pascal_voc-0.0.4/
--rwxrwxrwx   0 alexander  (1000) alexander  (1000)     3099 2023-06-08 20:53:57.665488 pascal_voc-0.0.4/PKG-INFO
--rwxrwxrwx   0 alexander  (1000) alexander  (1000)     2642 2023-02-28 17:56:32.000000 pascal_voc-0.0.4/README.md
-drwxrwxrwx   0 alexander  (1000) alexander  (1000)        0 2023-06-08 20:53:57.662505 pascal_voc-0.0.4/pascal/
--rwxrwxrwx   0 alexander  (1000) alexander  (1000)      111 2023-06-08 20:39:24.000000 pascal_voc-0.0.4/pascal/__init__.py
--rwxrwxrwx   0 alexander  (1000) alexander  (1000)    16327 2023-06-08 20:39:24.000000 pascal_voc-0.0.4/pascal/main.py
-drwxrwxrwx   0 alexander  (1000) alexander  (1000)        0 2023-06-08 20:53:57.664961 pascal_voc-0.0.4/pascal_voc.egg-info/
--rwxrwxrwx   0 alexander  (1000) alexander  (1000)     3099 2023-06-08 20:53:57.000000 pascal_voc-0.0.4/pascal_voc.egg-info/PKG-INFO
--rwxrwxrwx   0 alexander  (1000) alexander  (1000)      236 2023-06-08 20:53:57.000000 pascal_voc-0.0.4/pascal_voc.egg-info/SOURCES.txt
--rwxrwxrwx   0 alexander  (1000) alexander  (1000)        1 2023-06-08 20:53:57.000000 pascal_voc-0.0.4/pascal_voc.egg-info/dependency_links.txt
--rwxrwxrwx   0 alexander  (1000) alexander  (1000)       26 2023-06-08 20:53:57.000000 pascal_voc-0.0.4/pascal_voc.egg-info/requires.txt
--rwxrwxrwx   0 alexander  (1000) alexander  (1000)        7 2023-06-08 20:53:57.000000 pascal_voc-0.0.4/pascal_voc.egg-info/top_level.txt
--rwxrwxrwx   0 alexander  (1000) alexander  (1000)      434 2023-06-08 20:52:50.000000 pascal_voc-0.0.4/pyproject.toml
--rwxrwxrwx   0 alexander  (1000) alexander  (1000)       38 2023-06-08 20:53:57.665793 pascal_voc-0.0.4/setup.cfg
--rwxrwxrwx   0 alexander  (1000) alexander  (1000)      625 2023-06-08 20:51:39.000000 pascal_voc-0.0.4/setup.py
+drwxrwxrwx   0 alexander  (1000) alexander  (1000)        0 2023-06-08 22:24:56.862708 pascal_voc-0.0.5/
+-rwxrwxrwx   0 alexander  (1000) alexander  (1000)     3152 2023-06-08 22:24:56.862476 pascal_voc-0.0.5/PKG-INFO
+-rwxrwxrwx   0 alexander  (1000) alexander  (1000)     2694 2023-06-08 22:04:18.000000 pascal_voc-0.0.5/README.md
+drwxrwxrwx   0 alexander  (1000) alexander  (1000)        0 2023-06-08 22:24:56.859458 pascal_voc-0.0.5/pascal/
+-rwxrwxrwx   0 alexander  (1000) alexander  (1000)      111 2023-06-08 20:39:24.000000 pascal_voc-0.0.5/pascal/__init__.py
+-rwxrwxrwx   0 alexander  (1000) alexander  (1000)    16384 2023-06-08 22:22:44.000000 pascal_voc-0.0.5/pascal/main.py
+drwxrwxrwx   0 alexander  (1000) alexander  (1000)        0 2023-06-08 22:24:56.861941 pascal_voc-0.0.5/pascal_voc.egg-info/
+-rwxrwxrwx   0 alexander  (1000) alexander  (1000)     3152 2023-06-08 22:24:56.000000 pascal_voc-0.0.5/pascal_voc.egg-info/PKG-INFO
+-rwxrwxrwx   0 alexander  (1000) alexander  (1000)      236 2023-06-08 22:24:56.000000 pascal_voc-0.0.5/pascal_voc.egg-info/SOURCES.txt
+-rwxrwxrwx   0 alexander  (1000) alexander  (1000)        1 2023-06-08 22:24:56.000000 pascal_voc-0.0.5/pascal_voc.egg-info/dependency_links.txt
+-rwxrwxrwx   0 alexander  (1000) alexander  (1000)       26 2023-06-08 22:24:56.000000 pascal_voc-0.0.5/pascal_voc.egg-info/requires.txt
+-rwxrwxrwx   0 alexander  (1000) alexander  (1000)        7 2023-06-08 22:24:56.000000 pascal_voc-0.0.5/pascal_voc.egg-info/top_level.txt
+-rwxrwxrwx   0 alexander  (1000) alexander  (1000)      434 2023-06-08 22:24:39.000000 pascal_voc-0.0.5/pyproject.toml
+-rwxrwxrwx   0 alexander  (1000) alexander  (1000)       38 2023-06-08 22:24:56.862794 pascal_voc-0.0.5/setup.cfg
+-rwxrwxrwx   0 alexander  (1000) alexander  (1000)      625 2023-06-08 22:24:39.000000 pascal_voc-0.0.5/setup.py
```

### Comparing `pascal_voc-0.0.4/PKG-INFO` & `pascal_voc-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pascal_voc
-Version: 0.0.4
+Version: 0.0.5
 Summary: Tool to work with annotation formats
 Author: Alexander Barmin
 Author-email: Alexander Barmin <barmin1@mail.ru>
 License: MIT
 Project-URL: Homepage, https://github.com/Alek-dr/PascalVOC
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -105,11 +105,15 @@
         yolo = ann.to_yolo(label_map)
         out_name = f"{file.stem}.txt"
         with open(out_name, "w") as f:
             f.write(yolo)
 ```
 
 #### Installation
-
+From source 
 ```
 python setup.py install
 ```
+Using pip
+```
+pip install pascal-voc
+```
```

### Comparing `pascal_voc-0.0.4/README.md` & `pascal_voc-0.0.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -91,11 +91,15 @@
         yolo = ann.to_yolo(label_map)
         out_name = f"{file.stem}.txt"
         with open(out_name, "w") as f:
             f.write(yolo)
 ```
 
 #### Installation
-
+From source 
 ```
 python setup.py install
 ```
+Using pip
+```
+pip install pascal-voc
+```
```

### Comparing `pascal_voc-0.0.4/pascal/main.py` & `pascal_voc-0.0.5/pascal/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -215,15 +215,16 @@
             if source:
                 database = source.find("database").text
             else:
                 database = str()
             size_tag = doc.find("size")
             width = int(size_tag.find("width").text)
             height = int(size_tag.find("height").text)
-            depth = int(size_tag.find("depth").text)
+            depth_ = size_tag.find("depth")
+            depth = int(depth_.text) if depth_ is not None else 3
             size = size_block(width, height, depth)
             segmented_ = doc.find("segmented")
             if segmented_:
                 segmented = segmented_.text
             else:
                 segmented = 0
             objects = doc.findall("object")
```

### Comparing `pascal_voc-0.0.4/pascal_voc.egg-info/PKG-INFO` & `pascal_voc-0.0.5/pascal_voc.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pascal-voc
-Version: 0.0.4
+Version: 0.0.5
 Summary: Tool to work with annotation formats
 Author: Alexander Barmin
 Author-email: Alexander Barmin <barmin1@mail.ru>
 License: MIT
 Project-URL: Homepage, https://github.com/Alek-dr/PascalVOC
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -105,11 +105,15 @@
         yolo = ann.to_yolo(label_map)
         out_name = f"{file.stem}.txt"
         with open(out_name, "w") as f:
             f.write(yolo)
 ```
 
 #### Installation
-
+From source 
 ```
 python setup.py install
 ```
+Using pip
+```
+pip install pascal-voc
+```
```

### Comparing `pascal_voc-0.0.4/setup.py` & `pascal_voc-0.0.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="pascal_voc",
-    version="0.0.4",
+    version="0.0.5",
     author="Alexander Barmin",
     author_email="barmin1@mail.ru",
     description="Tool to work with annotation formats",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     install_requires=["lxml>=4.6.2", "Pillow>=8.1.0"],
```

