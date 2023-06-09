# Comparing `tmp/fw_client-0.5.0-py3-none-any.whl.zip` & `tmp/fw_client-0.5.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 8289 bytes, number of entries: 9
+Zip file size: 8284 bytes, number of entries: 9
 -rw-r--r--  2.0 unx      391 b- defN 80-Jan-01 00:00 fw_client/__init__.py
 -rw-r--r--  2.0 unx    11552 b- defN 80-Jan-01 00:00 fw_client/client.py
 -rw-r--r--  2.0 unx     3435 b- defN 80-Jan-01 00:00 fw_client/config.py
 -rw-r--r--  2.0 unx      193 b- defN 80-Jan-01 00:00 fw_client/errors.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 fw_client/py.typed
--rw-r--r--  2.0 unx     1078 b- defN 80-Jan-01 00:00 fw_client-0.5.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     1653 b- defN 80-Jan-01 00:00 fw_client-0.5.0.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fw_client-0.5.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx      679 b- defN 16-Jan-01 00:00 fw_client-0.5.0.dist-info/RECORD
-9 files, 19069 bytes uncompressed, 7131 bytes compressed:  62.6%
+-rw-r--r--  2.0 unx     1078 b- defN 80-Jan-01 00:00 fw_client-0.5.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1645 b- defN 80-Jan-01 00:00 fw_client-0.5.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fw_client-0.5.1.dist-info/WHEEL
+?rw-r--r--  2.0 unx      679 b- defN 16-Jan-01 00:00 fw_client-0.5.1.dist-info/RECORD
+9 files, 19061 bytes uncompressed, 7126 bytes compressed:  62.6%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: fw_client/errors.py
 Comment: 
 
 Filename: fw_client/py.typed
 Comment: 
 
-Filename: fw_client-0.5.0.dist-info/LICENSE
+Filename: fw_client-0.5.1.dist-info/LICENSE
 Comment: 
 
-Filename: fw_client-0.5.0.dist-info/METADATA
+Filename: fw_client-0.5.1.dist-info/METADATA
 Comment: 
 
-Filename: fw_client-0.5.0.dist-info/WHEEL
+Filename: fw_client-0.5.1.dist-info/WHEEL
 Comment: 
 
-Filename: fw_client-0.5.0.dist-info/RECORD
+Filename: fw_client-0.5.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `fw_client-0.5.0.dist-info/LICENSE` & `fw_client-0.5.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fw_client-0.5.0.dist-info/METADATA` & `fw_client-0.5.1.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: fw-client
-Version: 0.5.0
+Version: 0.5.1
 Summary: Flywheel HTTP API client.
 Home-page: https://gitlab.com/flywheel-io/tools/lib/fw-client
 License: MIT
 Keywords: Flywheel,API,HTTP,client
 Author: Flywheel
 Author-email: support@flywheel.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: fw-http-client (>=1.2.3,<2.0.0)
+Requires-Dist: fw-http-client (>=1.3,<2.0)
 Requires-Dist: memoization (>=0,<1)
-Requires-Dist: packaging (>=21.3,<22.0)
+Requires-Dist: packaging (>=23,<24)
 Requires-Dist: requests (>=2.27.1,<3.0.0)
 Requires-Dist: urllib3 (>=1.26,<2.0)
 Project-URL: Documentation, https://gitlab.com/flywheel-io/tools/lib/fw-client
 Project-URL: Repository, https://gitlab.com/flywheel-io/tools/lib/fw-client
 Description-Content-Type: text/markdown
 
 # fw-client
```

## Comparing `fw_client-0.5.0.dist-info/RECORD` & `fw_client-0.5.1.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 fw_client/__init__.py,sha256=JckKuAkkc0FupgEPEX0cWU0KU3hjlRcq4QpTWVLKBN4,391
 fw_client/client.py,sha256=b4alhe1NT-R0RNWQmwQCAC92U9tcMKMac2wquHfwsE4,11552
 fw_client/config.py,sha256=wdCb0Qsgn2y7uoHcGOXo2_58QZJ2Bu4mIxHXfRqn_Wo,3435
 fw_client/errors.py,sha256=MOALg8T0Z9KTR4MFeTz7BacTWLIlkddTOJocSBqXDFc,193
 fw_client/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-fw_client-0.5.0.dist-info/LICENSE,sha256=l6rSIY1z68PIZljFVsWf7vH6pbhZay7Yz2EKgbsR8q0,1078
-fw_client-0.5.0.dist-info/METADATA,sha256=jByHR2-mVCI4gf4srMpMTYXuJdNTBFmzLNOI5osXYqo,1653
-fw_client-0.5.0.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-fw_client-0.5.0.dist-info/RECORD,,
+fw_client-0.5.1.dist-info/LICENSE,sha256=l6rSIY1z68PIZljFVsWf7vH6pbhZay7Yz2EKgbsR8q0,1078
+fw_client-0.5.1.dist-info/METADATA,sha256=2V4E_2cgcm1q6O8kEZQLbtfdxyTqUd2lTBJe3CWElKY,1645
+fw_client-0.5.1.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+fw_client-0.5.1.dist-info/RECORD,,
```

