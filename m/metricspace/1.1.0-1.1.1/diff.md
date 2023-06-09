# Comparing `tmp/metricspace-1.1.0.tar.gz` & `tmp/metricspace-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metricspace-1.1.0.tar", last modified: Fri Jun  9 01:06:51 2023, max compression
+gzip compressed data, was "metricspace-1.1.1.tar", last modified: Fri Jun  9 19:35:01 2023, max compression
```

## Comparing `metricspace-1.1.0.tar` & `metricspace-1.1.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 01:06:51.388279 metricspace-1.1.0/
--rw-rw-rw-   0        0        0     1092 2023-06-08 22:39:10.000000 metricspace-1.1.0/LICENSE
--rw-rw-rw-   0        0        0     9091 2023-06-09 01:06:51.387278 metricspace-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     6624 2023-06-08 22:39:10.000000 metricspace-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-09 01:06:51.337729 metricspace-1.1.0/docs/
-drwxrwxrwx   0        0        0        0 2023-06-09 01:06:51.346266 metricspace-1.1.0/docs/source/
--rw-rw-rw-   0        0        0     1195 2023-06-08 22:39:10.000000 metricspace-1.1.0/docs/source/conf.py
-drwxrwxrwx   0        0        0        0 2023-06-09 01:06:51.347266 metricspace-1.1.0/examples/
--rw-rw-rw-   0        0        0     1201 2023-06-08 22:39:10.000000 metricspace-1.1.0/examples/ex_distances.py
-drwxrwxrwx   0        0        0        0 2023-06-09 01:06:51.348266 metricspace-1.1.0/metricspace/
--rw-rw-rw-   0        0        0      210 2023-06-08 23:41:51.000000 metricspace-1.1.0/metricspace/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 01:06:51.380277 metricspace-1.1.0/metricspace/entropy/
--rw-rw-rw-   0        0        0      310 2023-06-08 22:39:10.000000 metricspace-1.1.0/metricspace/entropy/__init__.py
--rw-rw-rw-   0        0        0      898 2023-06-08 22:39:10.000000 metricspace-1.1.0/metricspace/entropy/histbi.py
--rw-rw-rw-   0        0        0      540 2023-06-08 22:39:10.000000 metricspace-1.1.0/metricspace/entropy/histinfo.py
--rw-rw-rw-   0        0        0      687 2023-06-08 22:39:10.000000 metricspace-1.1.0/metricspace/entropy/histjabi.py
--rw-rw-rw-   0        0        0      703 2023-06-08 22:39:10.000000 metricspace-1.1.0/metricspace/entropy/histtpbi.py
--rw-rw-rw-   0        0        0      987 2023-06-08 22:39:10.000000 metricspace-1.1.0/metricspace/entropy/tblxbi.py
--rw-rw-rw-   0        0        0      405 2023-06-08 22:39:10.000000 metricspace-1.1.0/metricspace/entropy/tblxinfo.py
--rw-rw-rw-   0        0        0     1322 2023-06-08 22:39:10.000000 metricspace-1.1.0/metricspace/entropy/tblxtpbi.py
-drwxrwxrwx   0        0        0        0 2023-06-09 01:06:51.383277 metricspace-1.1.0/metricspace/model/
--rw-rw-rw-   0        0        0      119 2023-06-08 22:39:10.000000 metricspace-1.1.0/metricspace/model/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 01:06:51.385277 metricspace-1.1.0/metricspace/model/calculate_spkd/
--rw-rw-rw-   0        0        0       74 2023-06-08 22:39:10.000000 metricspace-1.1.0/metricspace/model/calculate_spkd/__init__.py
--rw-rw-rw-   0        0        0     7994 2023-06-08 22:39:10.000000 metricspace-1.1.0/metricspace/model/calculate_spkd/spkd_functions.py
--rw-rw-rw-   0        0        0     6263 2023-06-08 22:39:10.000000 metricspace-1.1.0/metricspace/model/distclust.py
--rw-rw-rw-   0        0        0     2253 2023-06-08 22:39:10.000000 metricspace-1.1.0/metricspace/model/spkd.py
-drwxrwxrwx   0        0        0        0 2023-06-09 01:06:51.386278 metricspace-1.1.0/metricspace/validate/
--rw-rw-rw-   0        0        0      386 2023-06-08 22:39:10.000000 metricspace-1.1.0/metricspace/validate/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 01:06:51.372043 metricspace-1.1.0/metricspace.egg-info/
--rw-rw-rw-   0        0        0     9091 2023-06-09 01:06:51.000000 metricspace-1.1.0/metricspace.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      743 2023-06-09 01:06:51.000000 metricspace-1.1.0/metricspace.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 01:06:51.000000 metricspace-1.1.0/metricspace.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-06-09 01:06:51.000000 metricspace-1.1.0/metricspace.egg-info/requires.txt
--rw-rw-rw-   0        0        0       44 2023-06-09 01:06:51.000000 metricspace-1.1.0/metricspace.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1405 2023-06-09 01:06:17.000000 metricspace-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-09 01:06:51.388279 metricspace-1.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-09 19:35:01.384063 metricspace-1.1.1/
+-rw-rw-rw-   0        0        0     1092 2023-06-08 22:39:10.000000 metricspace-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0     9091 2023-06-09 19:35:01.383063 metricspace-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6624 2023-06-08 22:39:10.000000 metricspace-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-09 19:35:01.335993 metricspace-1.1.1/docs/
+drwxrwxrwx   0        0        0        0 2023-06-09 19:35:01.345530 metricspace-1.1.1/docs/source/
+-rw-rw-rw-   0        0        0     1195 2023-06-08 22:39:10.000000 metricspace-1.1.1/docs/source/conf.py
+drwxrwxrwx   0        0        0        0 2023-06-09 19:35:01.346530 metricspace-1.1.1/examples/
+-rw-rw-rw-   0        0        0     1201 2023-06-08 22:39:10.000000 metricspace-1.1.1/examples/ex_distances.py
+drwxrwxrwx   0        0        0        0 2023-06-09 19:35:01.347530 metricspace-1.1.1/metricspace/
+-rw-rw-rw-   0        0        0      175 2023-06-09 16:05:12.000000 metricspace-1.1.1/metricspace/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 19:35:01.377259 metricspace-1.1.1/metricspace/entropy/
+-rw-rw-rw-   0        0        0      310 2023-06-08 22:39:10.000000 metricspace-1.1.1/metricspace/entropy/__init__.py
+-rw-rw-rw-   0        0        0      898 2023-06-08 22:39:10.000000 metricspace-1.1.1/metricspace/entropy/histbi.py
+-rw-rw-rw-   0        0        0      540 2023-06-08 22:39:10.000000 metricspace-1.1.1/metricspace/entropy/histinfo.py
+-rw-rw-rw-   0        0        0      687 2023-06-08 22:39:10.000000 metricspace-1.1.1/metricspace/entropy/histjabi.py
+-rw-rw-rw-   0        0        0      703 2023-06-08 22:39:10.000000 metricspace-1.1.1/metricspace/entropy/histtpbi.py
+-rw-rw-rw-   0        0        0      987 2023-06-08 22:39:10.000000 metricspace-1.1.1/metricspace/entropy/tblxbi.py
+-rw-rw-rw-   0        0        0      405 2023-06-08 22:39:10.000000 metricspace-1.1.1/metricspace/entropy/tblxinfo.py
+-rw-rw-rw-   0        0        0     1322 2023-06-08 22:39:10.000000 metricspace-1.1.1/metricspace/entropy/tblxtpbi.py
+drwxrwxrwx   0        0        0        0 2023-06-09 19:35:01.379258 metricspace-1.1.1/metricspace/model/
+-rw-rw-rw-   0        0        0      119 2023-06-08 22:39:10.000000 metricspace-1.1.1/metricspace/model/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 19:35:01.381259 metricspace-1.1.1/metricspace/model/calculate_spkd/
+-rw-rw-rw-   0        0        0       74 2023-06-08 22:39:10.000000 metricspace-1.1.1/metricspace/model/calculate_spkd/__init__.py
+-rw-rw-rw-   0        0        0     7994 2023-06-08 22:39:10.000000 metricspace-1.1.1/metricspace/model/calculate_spkd/spkd_functions.py
+-rw-rw-rw-   0        0        0     6263 2023-06-08 22:39:10.000000 metricspace-1.1.1/metricspace/model/distclust.py
+-rw-rw-rw-   0        0        0     2253 2023-06-08 22:39:10.000000 metricspace-1.1.1/metricspace/model/spkd.py
+drwxrwxrwx   0        0        0        0 2023-06-09 19:35:01.382068 metricspace-1.1.1/metricspace/validate/
+-rw-rw-rw-   0        0        0      386 2023-06-08 22:39:10.000000 metricspace-1.1.1/metricspace/validate/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 19:35:01.368256 metricspace-1.1.1/metricspace.egg-info/
+-rw-rw-rw-   0        0        0     9091 2023-06-09 19:35:01.000000 metricspace-1.1.1/metricspace.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      743 2023-06-09 19:35:01.000000 metricspace-1.1.1/metricspace.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 19:35:01.000000 metricspace-1.1.1/metricspace.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-06-09 19:35:01.000000 metricspace-1.1.1/metricspace.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       44 2023-06-09 19:35:01.000000 metricspace-1.1.1/metricspace.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1429 2023-06-09 19:34:45.000000 metricspace-1.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-09 19:35:01.384063 metricspace-1.1.1/setup.cfg
```

### Comparing `metricspace-1.1.0/LICENSE` & `metricspace-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `metricspace-1.1.0/PKG-INFO` & `metricspace-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metricspace
-Version: 1.1.0
+Version: 1.1.1
 Summary: A python translation of code originally theorized in: Metric-space analysis of spike trains: theory, algorithms, and application Jonathan D. Victor and Keith Purpura Network 8, 127-164 (1997)
 Author-email: Flynn OConnell <flynnoconnell@gmail.com>, Jonathan D Victor <jdvicto@med.cornell.edu>
 License: MIT License
         
         Copyright (c) 2023 Flynn OConnell
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: metricspace Version: 1.1.0 Summary: A python
+Metadata-Version: 2.1 Name: metricspace Version: 1.1.1 Summary: A python
 translation of code originally theorized in: Metric-space analysis of spike
 trains: theory, algorithms, and application Jonathan D. Victor and Keith
 Purpura Network 8, 127-164 (1997) Author-email: Flynn OConnell
 gmail.com>, Jonathan D Victor
 med.cornell.edu> License: MIT License Copyright (c) 2023 Flynn OConnell
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
```

### Comparing `metricspace-1.1.0/README.md` & `metricspace-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `metricspace-1.1.0/docs/source/conf.py` & `metricspace-1.1.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `metricspace-1.1.0/examples/ex_distances.py` & `metricspace-1.1.1/examples/ex_distances.py`

 * *Files identical despite different names*

### Comparing `metricspace-1.1.0/metricspace/entropy/histbi.py` & `metricspace-1.1.1/metricspace/entropy/histbi.py`

 * *Files identical despite different names*

### Comparing `metricspace-1.1.0/metricspace/entropy/histinfo.py` & `metricspace-1.1.1/metricspace/entropy/histinfo.py`

 * *Files identical despite different names*

### Comparing `metricspace-1.1.0/metricspace/entropy/histjabi.py` & `metricspace-1.1.1/metricspace/entropy/histjabi.py`

 * *Files identical despite different names*

### Comparing `metricspace-1.1.0/metricspace/entropy/histtpbi.py` & `metricspace-1.1.1/metricspace/entropy/histtpbi.py`

 * *Files identical despite different names*

### Comparing `metricspace-1.1.0/metricspace/entropy/tblxbi.py` & `metricspace-1.1.1/metricspace/entropy/tblxbi.py`

 * *Files identical despite different names*

### Comparing `metricspace-1.1.0/metricspace/entropy/tblxtpbi.py` & `metricspace-1.1.1/metricspace/entropy/tblxtpbi.py`

 * *Files identical despite different names*

### Comparing `metricspace-1.1.0/metricspace/model/calculate_spkd/spkd_functions.py` & `metricspace-1.1.1/metricspace/model/calculate_spkd/spkd_functions.py`

 * *Files identical despite different names*

### Comparing `metricspace-1.1.0/metricspace/model/distclust.py` & `metricspace-1.1.1/metricspace/model/distclust.py`

 * *Files identical despite different names*

### Comparing `metricspace-1.1.0/metricspace/model/spkd.py` & `metricspace-1.1.1/metricspace/model/spkd.py`

 * *Files identical despite different names*

### Comparing `metricspace-1.1.0/metricspace.egg-info/PKG-INFO` & `metricspace-1.1.1/metricspace.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metricspace
-Version: 1.1.0
+Version: 1.1.1
 Summary: A python translation of code originally theorized in: Metric-space analysis of spike trains: theory, algorithms, and application Jonathan D. Victor and Keith Purpura Network 8, 127-164 (1997)
 Author-email: Flynn OConnell <flynnoconnell@gmail.com>, Jonathan D Victor <jdvicto@med.cornell.edu>
 License: MIT License
         
         Copyright (c) 2023 Flynn OConnell
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: metricspace Version: 1.1.0 Summary: A python
+Metadata-Version: 2.1 Name: metricspace Version: 1.1.1 Summary: A python
 translation of code originally theorized in: Metric-space analysis of spike
 trains: theory, algorithms, and application Jonathan D. Victor and Keith
 Purpura Network 8, 127-164 (1997) Author-email: Flynn OConnell
 gmail.com>, Jonathan D Victor
 med.cornell.edu> License: MIT License Copyright (c) 2023 Flynn OConnell
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
```

### Comparing `metricspace-1.1.0/metricspace.egg-info/SOURCES.txt` & `metricspace-1.1.1/metricspace.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metricspace-1.1.0/pyproject.toml` & `metricspace-1.1.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -2,22 +2,24 @@
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages]
 find = {} 
 
 [project]
-version = "1.1.0"
+version = "1.1.1"
 name = "metricspace"
 description = "A python translation of code originally theorized in: Metric-space analysis of spike trains: theory, algorithms, and application Jonathan D. Victor and Keith Purpura Network 8, 127-164 (1997)"
 authors = [
     {name = "Flynn OConnell", email = "flynnoconnell@gmail.com"},
     {name = "Jonathan D Victor", email = "jdvicto@med.cornell.edu"}
 ]
-dependencies = ["setuptools>=40.8.0", "wheel", "rs-distances"]
+
+dependencies = ["setuptools>=40.8.0", "wheel", "rs-distances", "numba", "numpy"]
+
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
@@ -28,11 +30,12 @@
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 
 [project.license]
 file = "LICENSE"
 
+
 [project.urls]
 homepage = "https://github.com/NeuroPyPy/metricspace"
 repository = "https://github.com/NeuroPyPy/metricspace"
 documentation = "http://www-users.med.cornell.edu/~jdvicto/metricdf.html#algorithm"
```

