# Comparing `tmp/pymca-5.8.2-py2.py3-none-any.whl.zip` & `tmp/pymca-5.8.4-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
 Zip file size: 5501 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat     5930 b- defN 23-May-16 09:41 pymca-5.8.2.data/scripts/pymca_launcher
--rw-rw-rw-  2.0 fat       31 b- defN 23-May-16 09:38 pymca-5.8.2.data/scripts/pymca_launcher.bat
--rw-rw-rw-  2.0 fat     1817 b- defN 23-May-16 09:41 pymca-5.8.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1775 b- defN 23-May-16 09:41 pymca-5.8.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-May-16 09:41 pymca-5.8.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 23-May-16 09:41 pymca-5.8.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      570 b- defN 23-May-16 09:41 pymca-5.8.2.dist-info/RECORD
+-rw-rw-rw-  2.0 fat     5930 b- defN 23-Jun-09 12:28 pymca-5.8.4.data/scripts/pymca_launcher
+-rw-rw-rw-  2.0 fat       31 b- defN 23-May-16 09:38 pymca-5.8.4.data/scripts/pymca_launcher.bat
+-rw-rw-rw-  2.0 fat     1817 b- defN 23-Jun-09 12:28 pymca-5.8.4.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1775 b- defN 23-Jun-09 12:28 pymca-5.8.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Jun-09 12:28 pymca-5.8.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 23-Jun-09 12:28 pymca-5.8.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      570 b- defN 23-Jun-09 12:28 pymca-5.8.4.dist-info/RECORD
 7 files, 10239 bytes uncompressed, 4485 bytes compressed:  56.2%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
-Filename: pymca-5.8.2.data/scripts/pymca_launcher
+Filename: pymca-5.8.4.data/scripts/pymca_launcher
 Comment: 
 
-Filename: pymca-5.8.2.data/scripts/pymca_launcher.bat
+Filename: pymca-5.8.4.data/scripts/pymca_launcher.bat
 Comment: 
 
-Filename: pymca-5.8.2.dist-info/LICENSE
+Filename: pymca-5.8.4.dist-info/LICENSE
 Comment: 
 
-Filename: pymca-5.8.2.dist-info/METADATA
+Filename: pymca-5.8.4.dist-info/METADATA
 Comment: 
 
-Filename: pymca-5.8.2.dist-info/WHEEL
+Filename: pymca-5.8.4.dist-info/WHEEL
 Comment: 
 
-Filename: pymca-5.8.2.dist-info/top_level.txt
+Filename: pymca-5.8.4.dist-info/top_level.txt
 Comment: 
 
-Filename: pymca-5.8.2.dist-info/RECORD
+Filename: pymca-5.8.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `pymca-5.8.2.data/scripts/pymca_launcher` & `pymca-5.8.4.data/scripts/pymca_launcher`

 * *Files identical despite different names*

## Comparing `pymca-5.8.2.dist-info/LICENSE` & `pymca-5.8.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pymca-5.8.2.dist-info/METADATA` & `pymca-5.8.4.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymca
-Version: 5.8.2
+Version: 5.8.4
 Summary: pymca
 Author: V.A. Sole - ESRF
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: MacOS X
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Intended Audience :: Education
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 License-File: LICENSE
-Requires-Dist: PyMca5 (>=5.8.2)
+Requires-Dist: PyMca5 (>=5.8.4)
 Requires-Dist: h5py
 Requires-Dist: numpy
 Requires-Dist: matplotlib
 
 pymca
 =====
```

