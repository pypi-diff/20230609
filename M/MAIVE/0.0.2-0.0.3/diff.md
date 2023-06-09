# Comparing `tmp/MAIVE-0.0.2.tar.gz` & `tmp/MAIVE-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MAIVE-0.0.2.tar", last modified: Sun Apr  2 18:26:13 2023, max compression
+gzip compressed data, was "MAIVE-0.0.3.tar", last modified: Fri Jun  9 14:09:57 2023, max compression
```

## Comparing `MAIVE-0.0.2.tar` & `MAIVE-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-02 18:26:13.028045 MAIVE-0.0.2/
--rw-rw-rw-   0        0        0     1089 2023-03-03 18:10:48.000000 MAIVE-0.0.2/LICENSE
-drwxrwxrwx   0        0        0        0 2023-04-02 18:26:13.006840 MAIVE-0.0.2/MAIVE.egg-info/
--rw-rw-rw-   0        0        0      519 2023-04-02 18:26:12.000000 MAIVE-0.0.2/MAIVE.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      175 2023-04-02 18:26:12.000000 MAIVE-0.0.2/MAIVE.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-02 18:26:12.000000 MAIVE-0.0.2/MAIVE.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-02 18:26:12.000000 MAIVE-0.0.2/MAIVE.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      519 2023-04-02 18:26:13.022608 MAIVE-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0        7 2023-04-02 18:13:25.000000 MAIVE-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-02 18:26:13.014040 MAIVE-0.0.2/maive/
--rw-rw-rw-   0        0        0        0 2023-03-30 18:55:08.000000 MAIVE-0.0.2/maive/__init__.py
--rw-rw-rw-   0        0        0    18670 2023-04-02 18:21:37.000000 MAIVE-0.0.2/maive/maive.py
--rw-rw-rw-   0        0        0       42 2023-04-02 18:26:13.028045 MAIVE-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1484 2023-04-02 18:15:18.000000 MAIVE-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 14:09:57.400982 MAIVE-0.0.3/
+-rw-rw-rw-   0        0        0     1089 2023-03-03 18:10:48.000000 MAIVE-0.0.3/LICENSE
+drwxrwxrwx   0        0        0        0 2023-06-09 14:09:57.371980 MAIVE-0.0.3/MAIVE.egg-info/
+-rw-rw-rw-   0        0        0     3255 2023-06-09 14:09:56.000000 MAIVE-0.0.3/MAIVE.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      203 2023-06-09 14:09:56.000000 MAIVE-0.0.3/MAIVE.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 14:09:56.000000 MAIVE-0.0.3/MAIVE.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       83 2023-06-09 14:09:56.000000 MAIVE-0.0.3/MAIVE.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-09 14:09:56.000000 MAIVE-0.0.3/MAIVE.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3255 2023-06-09 14:09:57.398983 MAIVE-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2780 2023-06-09 13:45:14.000000 MAIVE-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-09 14:09:57.395979 MAIVE-0.0.3/maive/
+-rw-rw-rw-   0        0        0        0 2023-03-30 18:55:08.000000 MAIVE-0.0.3/maive/__init__.py
+-rw-rw-rw-   0        0        0    43520 2023-06-09 13:41:17.000000 MAIVE-0.0.3/maive/maive.py
+-rw-rw-rw-   0        0        0       42 2023-06-09 14:09:57.400982 MAIVE-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1525 2023-06-09 14:09:18.000000 MAIVE-0.0.3/setup.py
```

### Comparing `MAIVE-0.0.2/LICENSE` & `MAIVE-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `MAIVE-0.0.2/setup.py` & `MAIVE-0.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import setuptools
 
-
-
-VERSION = "0.0.2"
-DESCRIPTION = "Mathematics for Ariticial Intelligence and Visualization Extended"
+VERSION = "0.0.3"
+DESCRIPTION = "Mathematics and Ariticial Intelligence and Visualization Extended"
  
 
 with open("README.md", "r") as fh:
     LONG_DESCRIPTION  = fh.read()
 
 setuptools.setup(
     
@@ -16,15 +14,15 @@
     version=VERSION, 
            
     author="Piyush Pant",  
     
     author_email= "piyushpant15@gmail.com",  
     
     keywords= [
-        "MAIVE", "piyush", "pant", "AI", "machine learning", "maths", "piyush pant", "mathematics for ai", "artificial intelligence"
+        "MAIVE","Artificial Intelligence", "Machine Learning", "Maths", 
     ],
      
     description=DESCRIPTION,
     
     long_description= LONG_DESCRIPTION ,      # Long description read from the the readme file
     
     long_description_content_type="text/markdown",
@@ -41,9 +39,9 @@
     
     # py_modules=["quicksample"],             # Name of the python package
     
     # package_dir={'':'quicksample/src'},     # Directory of the source code of the package
     
     
     
-    install_requires=[],                     # Install other dependencies if any
+    install_requires=["numpy", "matplotlib", "pandas", "fractions","statistics","statsmodel", "seaborn","sklearn", "tensorflow"],                     # Install other dependencies if any
 )
```

