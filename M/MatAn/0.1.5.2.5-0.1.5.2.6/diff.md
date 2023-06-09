# Comparing `tmp/MatAn-0.1.5.2.5-py3-none-any.whl.zip` & `tmp/MatAn-0.1.5.2.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,17 @@
-Zip file size: 14506 bytes, number of entries: 5
--rw-r--r--  2.0 unx    34670 b- defN 23-Jun-09 11:50 MatAn-0.1.5.2.5.dist-info/LICENSE
--rw-r--r--  2.0 unx     4161 b- defN 23-Jun-09 11:50 MatAn-0.1.5.2.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-09 11:50 MatAn-0.1.5.2.5.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-Jun-09 11:50 MatAn-0.1.5.2.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      396 b- defN 23-Jun-09 11:50 MatAn-0.1.5.2.5.dist-info/RECORD
-5 files, 39320 bytes uncompressed, 13766 bytes compressed:  65.0%
+Zip file size: 23260 bytes, number of entries: 15
+-rw-r--r--  2.0 unx       71 b- defN 23-Jun-09 12:31 matan/__init__.py
+-rw-r--r--  2.0 unx     4803 b- defN 23-May-08 17:43 matan/files.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-09 12:13 matan/matan.py
+-rw-r--r--  2.0 unx      155 b- defN 23-May-29 20:55 matan/misc.py
+-rw-r--r--  2.0 unx     2658 b- defN 23-Jun-09 11:44 matan/properties.py
+-rw-r--r--  2.0 unx    17272 b- defN 23-Jun-09 12:25 matan/sample.py
+-rw-r--r--  2.0 unx      155 b- defN 23-May-29 20:55 misc/__init__.py
+-rw-r--r--  2.0 unx     2659 b- defN 23-May-29 20:57 properties/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-09 11:58 tests/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-09 12:08 tests/test.py
+-rw-r--r--  2.0 unx    34670 b- defN 23-Jun-09 12:32 MatAn-0.1.5.2.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4161 b- defN 23-Jun-09 12:32 MatAn-0.1.5.2.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-09 12:32 MatAn-0.1.5.2.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-Jun-09 12:32 MatAn-0.1.5.2.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1115 b- defN 23-Jun-09 12:32 MatAn-0.1.5.2.6.dist-info/RECORD
+15 files, 67823 bytes uncompressed, 21440 bytes compressed:  68.4%
```

## zipnote {}

```diff
@@ -1,16 +1,46 @@
-Filename: MatAn-0.1.5.2.5.dist-info/LICENSE
+Filename: matan/__init__.py
 Comment: 
 
-Filename: MatAn-0.1.5.2.5.dist-info/METADATA
+Filename: matan/files.py
 Comment: 
 
-Filename: MatAn-0.1.5.2.5.dist-info/WHEEL
+Filename: matan/matan.py
 Comment: 
 
-Filename: MatAn-0.1.5.2.5.dist-info/top_level.txt
+Filename: matan/misc.py
 Comment: 
 
-Filename: MatAn-0.1.5.2.5.dist-info/RECORD
+Filename: matan/properties.py
+Comment: 
+
+Filename: matan/sample.py
+Comment: 
+
+Filename: misc/__init__.py
+Comment: 
+
+Filename: properties/__init__.py
+Comment: 
+
+Filename: tests/__init__.py
+Comment: 
+
+Filename: tests/test.py
+Comment: 
+
+Filename: MatAn-0.1.5.2.6.dist-info/LICENSE
+Comment: 
+
+Filename: MatAn-0.1.5.2.6.dist-info/METADATA
+Comment: 
+
+Filename: MatAn-0.1.5.2.6.dist-info/WHEEL
+Comment: 
+
+Filename: MatAn-0.1.5.2.6.dist-info/top_level.txt
+Comment: 
+
+Filename: MatAn-0.1.5.2.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `MatAn-0.1.5.2.5.dist-info/LICENSE` & `MatAn-0.1.5.2.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `MatAn-0.1.5.2.5.dist-info/METADATA` & `MatAn-0.1.5.2.6.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MatAn
-Version: 0.1.5.2.5
+Version: 0.1.5.2.6
 Summary: Material analysis package to plot or extract properties like tensile modulus etc. 
 Home-page: https://codeberg.org/309631/matan
 Author: Igor Cudnik
 Author-email: igor.cudnik@student.put.poznan.pl
 License: GPLv3
 Keywords: material analysis,ISO 527,ISO 527-1,polymers analysis
 Classifier: Development Status :: 3 - Alpha
@@ -14,16 +14,16 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: matplotlib
 Requires-Dist: numpy
+Requires-Dist: matplotlib
 
 **This package is still under development. Be aware of often updates!**
 # MaTan
 
 Shortcut comes from **Mat**erial **An**analysis - ultimately is should contains modules allowing user to calculate metals and polymers properties from tensile, HDT (polymers) and DSC tests, as well as the others. There are few similar  packages in PyPI, but none of them I found good to me, so I wrote new one. 
 
 For now it includes:
```

