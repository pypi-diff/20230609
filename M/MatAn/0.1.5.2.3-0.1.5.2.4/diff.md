# Comparing `tmp/MatAn-0.1.5.2.3-py3-none-any.whl.zip` & `tmp/MatAn-0.1.5.2.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 21495 bytes, number of entries: 9
--rw-r--r--  2.0 unx    17356 b- defN 23-Jun-09 11:29 matan/__init__.py
+Zip file size: 21501 bytes, number of entries: 9
+-rw-r--r--  2.0 unx    17363 b- defN 23-Jun-09 11:35 matan/__init__.py
 -rw-r--r--  2.0 unx     4803 b- defN 23-May-08 17:43 matan/files.py
 -rw-r--r--  2.0 unx      155 b- defN 23-May-29 20:55 misc/__init__.py
 -rw-r--r--  2.0 unx     2659 b- defN 23-May-29 20:57 properties/__init__.py
--rw-r--r--  2.0 unx    34670 b- defN 23-Jun-09 11:29 MatAn-0.1.5.2.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     4161 b- defN 23-Jun-09 11:29 MatAn-0.1.5.2.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-09 11:29 MatAn-0.1.5.2.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       22 b- defN 23-Jun-09 11:29 MatAn-0.1.5.2.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      694 b- defN 23-Jun-09 11:29 MatAn-0.1.5.2.3.dist-info/RECORD
-9 files, 64612 bytes uncompressed, 20313 bytes compressed:  68.6%
+-rw-r--r--  2.0 unx    34670 b- defN 23-Jun-09 11:35 MatAn-0.1.5.2.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4161 b- defN 23-Jun-09 11:35 MatAn-0.1.5.2.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-09 11:35 MatAn-0.1.5.2.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       22 b- defN 23-Jun-09 11:35 MatAn-0.1.5.2.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      694 b- defN 23-Jun-09 11:35 MatAn-0.1.5.2.4.dist-info/RECORD
+9 files, 64619 bytes uncompressed, 20319 bytes compressed:  68.6%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: misc/__init__.py
 Comment: 
 
 Filename: properties/__init__.py
 Comment: 
 
-Filename: MatAn-0.1.5.2.3.dist-info/LICENSE
+Filename: MatAn-0.1.5.2.4.dist-info/LICENSE
 Comment: 
 
-Filename: MatAn-0.1.5.2.3.dist-info/METADATA
+Filename: MatAn-0.1.5.2.4.dist-info/METADATA
 Comment: 
 
-Filename: MatAn-0.1.5.2.3.dist-info/WHEEL
+Filename: MatAn-0.1.5.2.4.dist-info/WHEEL
 Comment: 
 
-Filename: MatAn-0.1.5.2.3.dist-info/top_level.txt
+Filename: MatAn-0.1.5.2.4.dist-info/top_level.txt
 Comment: 
 
-Filename: MatAn-0.1.5.2.3.dist-info/RECORD
+Filename: MatAn-0.1.5.2.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## matan/__init__.py

```diff
@@ -1,14 +1,14 @@
-import sys
-sys.path.append("..") # Adds higher directory to python modules path.
+# import sys
+# sys.path.append("..") # Adds higher directory to python modules path.
 import numpy as np
 import matplotlib.pyplot as plt
 from typing import Union
 
-from ..properties import  *
+from ...src import  properties
 
 
 
 """
 TODO:
 Create  abstract class for properties like tensile strength, tensile modulus, etc, with pass, so using diffrent norms and materials will be easier
 Move calculation of real values into method of engineering values
```

## Comparing `MatAn-0.1.5.2.3.dist-info/LICENSE` & `MatAn-0.1.5.2.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `MatAn-0.1.5.2.3.dist-info/METADATA` & `MatAn-0.1.5.2.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MatAn
-Version: 0.1.5.2.3
+Version: 0.1.5.2.4
 Summary: Material analysis package to plot or extract properties like tensile modulus etc. 
 Home-page: https://codeberg.org/309631/matan
 Author: Igor Cudnik
 Author-email: igor.cudnik@student.put.poznan.pl
 License: GPLv3
 Keywords: material analysis,ISO 527,ISO 527-1,polymers analysis
 Classifier: Development Status :: 3 - Alpha
```

