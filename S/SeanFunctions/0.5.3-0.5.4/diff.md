# Comparing `tmp/SeanFunctions-0.5.3.tar.gz` & `tmp/SeanFunctions-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SeanFunctions-0.5.3.tar", last modified: Fri Jun  9 17:32:11 2023, max compression
+gzip compressed data, was "SeanFunctions-0.5.4.tar", last modified: Fri Jun  9 21:50:29 2023, max compression
```

## Comparing `SeanFunctions-0.5.3.tar` & `SeanFunctions-0.5.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 17:32:11.091444 SeanFunctions-0.5.3/
--rw-rw-rw-   0        0        0      274 2023-06-09 17:27:31.000000 SeanFunctions-0.5.3/.gitignore
--rw-rw-rw-   0        0        0     1087 2023-06-09 17:27:31.000000 SeanFunctions-0.5.3/LICENSE
--rw-rw-rw-   0        0        0       36 2023-06-09 17:27:31.000000 SeanFunctions-0.5.3/MANIFEST.in
--rw-rw-rw-   0        0        0      678 2023-06-09 17:32:11.090451 SeanFunctions-0.5.3/PKG-INFO
--rw-rw-rw-   0        0        0      144 2023-06-09 17:27:31.000000 SeanFunctions-0.5.3/README.md
--rw-rw-rw-   0        0        0     1157 2023-06-09 17:31:09.000000 SeanFunctions-0.5.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-09 17:32:11.091940 SeanFunctions-0.5.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-09 17:32:11.052593 SeanFunctions-0.5.3/src/
-drwxrwxrwx   0        0        0        0 2023-06-09 17:32:11.069045 SeanFunctions-0.5.3/src/SeanFunctions/
-drwxrwxrwx   0        0        0        0 2023-06-09 17:32:11.089456 SeanFunctions-0.5.3/src/SeanFunctions/Data/
--rw-rw-rw-   0        0        0    19820 2023-06-09 17:27:31.000000 SeanFunctions-0.5.3/src/SeanFunctions/Data/AtomicFormFactorConstants.csv
--rw-rw-rw-   0        0        0    14993 2023-06-09 17:27:31.000000 SeanFunctions-0.5.3/src/SeanFunctions/Data/NeutronScatteringLengths.csv
--rw-rw-rw-   0        0        0    15625 2023-06-09 17:27:31.000000 SeanFunctions-0.5.3/src/SeanFunctions/Data/NeutronScatteringLengths_Corrected.csv
--rw-rw-rw-   0        0        0       39 2023-06-09 17:27:31.000000 SeanFunctions-0.5.3/src/SeanFunctions/__init__.py
--rw-rw-rw-   0        0        0     4906 2023-06-09 17:27:31.000000 SeanFunctions-0.5.3/src/SeanFunctions/fitting.py
--rw-rw-rw-   0        0        0     9718 2023-06-09 17:27:31.000000 SeanFunctions-0.5.3/src/SeanFunctions/math.py
--rw-rw-rw-   0        0        0    15741 2023-06-09 17:27:31.000000 SeanFunctions-0.5.3/src/SeanFunctions/scattering.py
--rw-rw-rw-   0        0        0      220 2023-06-09 17:32:10.000000 SeanFunctions-0.5.3/src/SeanFunctions/version.py
-drwxrwxrwx   0        0        0        0 2023-06-09 17:32:11.084967 SeanFunctions-0.5.3/src/SeanFunctions.egg-info/
--rw-rw-rw-   0        0        0      678 2023-06-09 17:32:10.000000 SeanFunctions-0.5.3/src/SeanFunctions.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      532 2023-06-09 17:32:11.000000 SeanFunctions-0.5.3/src/SeanFunctions.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 17:32:10.000000 SeanFunctions-0.5.3/src/SeanFunctions.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-09 17:32:10.000000 SeanFunctions-0.5.3/src/SeanFunctions.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 21:50:29.223794 SeanFunctions-0.5.4/
+-rw-rw-rw-   0        0        0      274 2023-06-09 17:27:31.000000 SeanFunctions-0.5.4/.gitignore
+-rw-rw-rw-   0        0        0     1087 2023-06-09 17:27:31.000000 SeanFunctions-0.5.4/LICENSE
+-rw-rw-rw-   0        0        0       36 2023-06-09 17:27:31.000000 SeanFunctions-0.5.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     1070 2023-06-09 21:50:29.223298 SeanFunctions-0.5.4/PKG-INFO
+-rw-rw-rw-   0        0        0      536 2023-06-09 21:28:21.000000 SeanFunctions-0.5.4/README.md
+-rw-rw-rw-   0        0        0     1394 2023-06-09 21:38:26.000000 SeanFunctions-0.5.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-09 21:50:29.224290 SeanFunctions-0.5.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-09 21:50:29.191044 SeanFunctions-0.5.4/src/
+drwxrwxrwx   0        0        0        0 2023-06-09 21:50:29.199490 SeanFunctions-0.5.4/src/SeanFunctions/
+drwxrwxrwx   0        0        0        0 2023-06-09 21:50:29.222306 SeanFunctions-0.5.4/src/SeanFunctions/Data/
+-rw-rw-rw-   0        0        0    19820 2023-06-09 17:27:31.000000 SeanFunctions-0.5.4/src/SeanFunctions/Data/AtomicFormFactorConstants.csv
+-rw-rw-rw-   0        0        0    14993 2023-06-09 17:27:31.000000 SeanFunctions-0.5.4/src/SeanFunctions/Data/NeutronScatteringLengths.csv
+-rw-rw-rw-   0        0        0    15625 2023-06-09 17:27:31.000000 SeanFunctions-0.5.4/src/SeanFunctions/Data/NeutronScatteringLengths_Corrected.csv
+-rw-rw-rw-   0        0        0       65 2023-06-09 21:28:21.000000 SeanFunctions-0.5.4/src/SeanFunctions/__init__.py
+-rw-rw-rw-   0        0        0     4906 2023-06-09 17:27:31.000000 SeanFunctions-0.5.4/src/SeanFunctions/fitting.py
+-rw-rw-rw-   0        0        0     9718 2023-06-09 17:27:31.000000 SeanFunctions-0.5.4/src/SeanFunctions/math.py
+-rw-rw-rw-   0        0        0    15741 2023-06-09 17:27:31.000000 SeanFunctions-0.5.4/src/SeanFunctions/scattering.py
+drwxrwxrwx   0        0        0        0 2023-06-09 21:50:29.218834 SeanFunctions-0.5.4/src/SeanFunctions.egg-info/
+-rw-rw-rw-   0        0        0     1070 2023-06-09 21:50:29.000000 SeanFunctions-0.5.4/src/SeanFunctions.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      543 2023-06-09 21:50:29.000000 SeanFunctions-0.5.4/src/SeanFunctions.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 21:50:29.000000 SeanFunctions-0.5.4/src/SeanFunctions.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-06-09 21:50:29.000000 SeanFunctions-0.5.4/src/SeanFunctions.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-09 21:50:29.000000 SeanFunctions-0.5.4/src/SeanFunctions.egg-info/top_level.txt
```

### Comparing `SeanFunctions-0.5.3/LICENSE` & `SeanFunctions-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `SeanFunctions-0.5.3/pyproject.toml` & `SeanFunctions-0.5.4/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,52 +1,66 @@
 [project]
 name = "SeanFunctions"
-version = "0.5.3"
+version = "v0.5.4"
 # dynamic = ["version"]
 authors = [
   { name="Sean Fayfar", email="sfayfar@gmail.com" },
 ]
 description = "Collection of useful python functions"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
+dependencies = [
+    "numpy",
+    "scipy",
+    "lmfit",
+    "uncertainties",
+    "mendeleev"
+]
 
 [project.urls]
 Homepage = "https://github.com/sfayfar/SeanFunctions"
 "Bug Tracker" = "https://github.com/sfayfar/SeanFunctions/issues"
 
 
 [options]
 packages = "find:"
 python_requires = ">=3.7"
 setup_requires = "setuptools_scm"
 package_dir = "src"
 include_package_data = "True"
-install_requires = [
-    "numpy",
-    "scipy",
-    "pathlib",
-    "lmfit",
-    "uncertainties",
-    "mendeleev"
-]
 
-# [tool.setuptools.packages.find]
-# where = ["src"]
 
 [tool.setuptools.package-data]
 "SeanFunctions.Data" = ["*.csv"]
 
 [build-system]
 requires = [
     "setuptools>=61.0",
     "wheel",
     "setuptools_scm[toml]>=6.2",
 ]
 build-backend = "setuptools.build_meta"
 
-[tool.setuptools_scm]
-write_to = "src/SeanFunctions/version.py"
+
+[tool.bumpver.file_patterns]
+"pyproject.toml" = [
+    'version = "{version}"',
+]
+"src/SeanFunctions/__init__.py" = ['__version__ = "{version}"']
+"README.md" = ['{version}']
+
+
+[tool.bumpver]
+current_version = "v0.5.4"
+version_pattern = "vMAJOR.MINOR.PATCH[-TAGNUM]"
+commit_message = "bump version to {new_version}"
+commit = true
+tag = true
+push = true
+
+
+
```

### Comparing `SeanFunctions-0.5.3/src/SeanFunctions/Data/AtomicFormFactorConstants.csv` & `SeanFunctions-0.5.4/src/SeanFunctions/Data/AtomicFormFactorConstants.csv`

 * *Files identical despite different names*

### Comparing `SeanFunctions-0.5.3/src/SeanFunctions/Data/NeutronScatteringLengths.csv` & `SeanFunctions-0.5.4/src/SeanFunctions/Data/NeutronScatteringLengths.csv`

 * *Files identical despite different names*

### Comparing `SeanFunctions-0.5.3/src/SeanFunctions/Data/NeutronScatteringLengths_Corrected.csv` & `SeanFunctions-0.5.4/src/SeanFunctions/Data/NeutronScatteringLengths_Corrected.csv`

 * *Files identical despite different names*

### Comparing `SeanFunctions-0.5.3/src/SeanFunctions/fitting.py` & `SeanFunctions-0.5.4/src/SeanFunctions/fitting.py`

 * *Files identical despite different names*

### Comparing `SeanFunctions-0.5.3/src/SeanFunctions/math.py` & `SeanFunctions-0.5.4/src/SeanFunctions/math.py`

 * *Files identical despite different names*

### Comparing `SeanFunctions-0.5.3/src/SeanFunctions/scattering.py` & `SeanFunctions-0.5.4/src/SeanFunctions/scattering.py`

 * *Files identical despite different names*

### Comparing `SeanFunctions-0.5.3/src/SeanFunctions.egg-info/SOURCES.txt` & `SeanFunctions-0.5.4/src/SeanFunctions.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 MANIFEST.in
 README.md
 pyproject.toml
 src/SeanFunctions/__init__.py
 src/SeanFunctions/fitting.py
 src/SeanFunctions/math.py
 src/SeanFunctions/scattering.py
-src/SeanFunctions/version.py
 src/SeanFunctions.egg-info/PKG-INFO
 src/SeanFunctions.egg-info/SOURCES.txt
 src/SeanFunctions.egg-info/dependency_links.txt
+src/SeanFunctions.egg-info/requires.txt
 src/SeanFunctions.egg-info/top_level.txt
 src/SeanFunctions/Data/AtomicFormFactorConstants.csv
 src/SeanFunctions/Data/NeutronScatteringLengths.csv
 src/SeanFunctions/Data/NeutronScatteringLengths_Corrected.csv
```

