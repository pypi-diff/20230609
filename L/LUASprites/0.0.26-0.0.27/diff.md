# Comparing `tmp/LUASprites-0.0.26.tar.gz` & `tmp/LUASprites-0.0.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LUASprites-0.0.26.tar", last modified: Thu Jun  8 20:36:22 2023, max compression
+gzip compressed data, was "LUASprites-0.0.27.tar", last modified: Fri Jun  9 04:32:18 2023, max compression
```

## Comparing `LUASprites-0.0.26.tar` & `LUASprites-0.0.27.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 ajsteinhauser   (501) staff       (20)        0 2023-06-08 20:36:22.186428 LUASprites-0.0.26/
--rw-r--r--   0 ajsteinhauser   (501) staff       (20)     1071 2023-06-08 19:47:22.000000 LUASprites-0.0.26/LICENSE.txt
--rw-r--r--   0 ajsteinhauser   (501) staff       (20)       45 2023-06-08 19:47:22.000000 LUASprites-0.0.26/MANIFEST.in
--rw-r--r--   0 ajsteinhauser   (501) staff       (20)      968 2023-06-08 20:36:22.186481 LUASprites-0.0.26/PKG-INFO
--rw-r--r--   0 ajsteinhauser   (501) staff       (20)      514 2023-06-08 19:47:22.000000 LUASprites-0.0.26/README.md
--rw-r--r--   0 ajsteinhauser   (501) staff       (20)      119 2023-06-08 19:47:22.000000 LUASprites-0.0.26/requirements.txt
--rw-r--r--   0 ajsteinhauser   (501) staff       (20)      144 2023-06-08 20:36:22.186659 LUASprites-0.0.26/setup.cfg
--rw-r--r--   0 ajsteinhauser   (501) staff       (20)      995 2023-06-08 20:36:00.000000 LUASprites-0.0.26/setup.py
-drwxr-xr-x   0 ajsteinhauser   (501) staff       (20)        0 2023-06-08 20:36:22.184337 LUASprites-0.0.26/src/
-drwxr-xr-x   0 ajsteinhauser   (501) staff       (20)        0 2023-06-08 20:36:22.186177 LUASprites-0.0.26/src/LUASprites.egg-info/
--rw-r--r--   0 ajsteinhauser   (501) staff       (20)      968 2023-06-08 20:36:22.000000 LUASprites-0.0.26/src/LUASprites.egg-info/PKG-INFO
--rw-r--r--   0 ajsteinhauser   (501) staff       (20)      320 2023-06-08 20:36:22.000000 LUASprites-0.0.26/src/LUASprites.egg-info/SOURCES.txt
--rw-r--r--   0 ajsteinhauser   (501) staff       (20)        1 2023-06-08 20:36:22.000000 LUASprites-0.0.26/src/LUASprites.egg-info/dependency_links.txt
--rw-r--r--   0 ajsteinhauser   (501) staff       (20)       49 2023-06-08 20:36:22.000000 LUASprites-0.0.26/src/LUASprites.egg-info/entry_points.txt
--rw-r--r--   0 ajsteinhauser   (501) staff       (20)      119 2023-06-08 20:36:22.000000 LUASprites-0.0.26/src/LUASprites.egg-info/requires.txt
--rw-r--r--   0 ajsteinhauser   (501) staff       (20)       10 2023-06-08 20:36:22.000000 LUASprites-0.0.26/src/LUASprites.egg-info/top_level.txt
-drwxr-xr-x   0 ajsteinhauser   (501) staff       (20)        0 2023-06-08 20:36:22.186306 LUASprites-0.0.26/src/spritegen/
--rw-r--r--   0 ajsteinhauser   (501) staff       (20)     9924 2023-06-08 20:35:23.000000 LUASprites-0.0.26/src/spritegen/cli.py
+drwxr-xr-x   0 ajsteinhauser   (501) staff       (20)        0 2023-06-09 04:32:18.268834 LUASprites-0.0.27/
+-rw-r--r--   0 ajsteinhauser   (501) staff       (20)     1071 2023-06-08 19:47:22.000000 LUASprites-0.0.27/LICENSE.txt
+-rw-r--r--   0 ajsteinhauser   (501) staff       (20)       45 2023-06-08 19:47:22.000000 LUASprites-0.0.27/MANIFEST.in
+-rw-r--r--   0 ajsteinhauser   (501) staff       (20)      968 2023-06-09 04:32:18.268914 LUASprites-0.0.27/PKG-INFO
+-rw-r--r--   0 ajsteinhauser   (501) staff       (20)      514 2023-06-08 19:47:22.000000 LUASprites-0.0.27/README.md
+-rw-r--r--   0 ajsteinhauser   (501) staff       (20)      119 2023-06-08 19:47:22.000000 LUASprites-0.0.27/requirements.txt
+-rw-r--r--   0 ajsteinhauser   (501) staff       (20)      144 2023-06-09 04:32:18.269141 LUASprites-0.0.27/setup.cfg
+-rw-r--r--   0 ajsteinhauser   (501) staff       (20)      995 2023-06-09 04:32:08.000000 LUASprites-0.0.27/setup.py
+drwxr-xr-x   0 ajsteinhauser   (501) staff       (20)        0 2023-06-09 04:32:18.266018 LUASprites-0.0.27/src/
+drwxr-xr-x   0 ajsteinhauser   (501) staff       (20)        0 2023-06-09 04:32:18.268348 LUASprites-0.0.27/src/LUASprites.egg-info/
+-rw-r--r--   0 ajsteinhauser   (501) staff       (20)      968 2023-06-09 04:32:18.000000 LUASprites-0.0.27/src/LUASprites.egg-info/PKG-INFO
+-rw-r--r--   0 ajsteinhauser   (501) staff       (20)      320 2023-06-09 04:32:18.000000 LUASprites-0.0.27/src/LUASprites.egg-info/SOURCES.txt
+-rw-r--r--   0 ajsteinhauser   (501) staff       (20)        1 2023-06-09 04:32:18.000000 LUASprites-0.0.27/src/LUASprites.egg-info/dependency_links.txt
+-rw-r--r--   0 ajsteinhauser   (501) staff       (20)       49 2023-06-09 04:32:18.000000 LUASprites-0.0.27/src/LUASprites.egg-info/entry_points.txt
+-rw-r--r--   0 ajsteinhauser   (501) staff       (20)      119 2023-06-09 04:32:18.000000 LUASprites-0.0.27/src/LUASprites.egg-info/requires.txt
+-rw-r--r--   0 ajsteinhauser   (501) staff       (20)       10 2023-06-09 04:32:18.000000 LUASprites-0.0.27/src/LUASprites.egg-info/top_level.txt
+drwxr-xr-x   0 ajsteinhauser   (501) staff       (20)        0 2023-06-09 04:32:18.268544 LUASprites-0.0.27/src/spritegen/
+-rw-r--r--   0 ajsteinhauser   (501) staff       (20)     9923 2023-06-09 04:31:13.000000 LUASprites-0.0.27/src/spritegen/cli.py
```

### Comparing `LUASprites-0.0.26/LICENSE.txt` & `LUASprites-0.0.27/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `LUASprites-0.0.26/PKG-INFO` & `LUASprites-0.0.27/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LUASprites
-Version: 0.0.26
+Version: 0.0.27
 Summary: Generate spritesheets and lua modules for easy image reference
 Home-page: https://github.com/AJSteinhauser/LUASprites
 Author: AJ Steinhauser
 Author-email: ajsteinhauser11@gmail.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
```

### Comparing `LUASprites-0.0.26/README.md` & `LUASprites-0.0.27/README.md`

 * *Files identical despite different names*

### Comparing `LUASprites-0.0.26/setup.py` & `LUASprites-0.0.27/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 with open("requirements.txt", "r", encoding="utf-8") as fh:
     requirements = fh.read()
 
 
 setup(
     name = 'LUASprites',
-    version = '0.0.26',
+    version = '0.0.27',
     author = 'AJ Steinhauser',
     author_email = 'ajsteinhauser11@gmail.com',
     license = 'MIT License',
     description = 'Generate spritesheets and lua modules for easy image reference',
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = 'https://github.com/AJSteinhauser/LUASprites',
```

### Comparing `LUASprites-0.0.26/src/LUASprites.egg-info/PKG-INFO` & `LUASprites-0.0.27/src/LUASprites.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LUASprites
-Version: 0.0.26
+Version: 0.0.27
 Summary: Generate spritesheets and lua modules for easy image reference
 Home-page: https://github.com/AJSteinhauser/LUASprites
 Author: AJ Steinhauser
 Author-email: ajsteinhauser11@gmail.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
```

### Comparing `LUASprites-0.0.26/src/spritegen/cli.py` & `LUASprites-0.0.27/src/spritegen/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -280,8 +280,7 @@
     buildTree(trees,sprites)
     outputFolder = getOutputFolder(path)
     packImages(trees,name, outputFolder)
     outputType = getOutputType()
     generateLuaOutput(outputType,name,trees, outputFolder)
     print("Finished...")
     time.sleep(1)   
-
```

