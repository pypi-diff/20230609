# Comparing `tmp/snaptrade-1.0.8-py3-none-any.whl.zip` & `tmp/snaptrade-1.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 10887 bytes, number of entries: 11
+Zip file size: 11110 bytes, number of entries: 11
 -rw-rw-r--  2.0 unx        0 b- defN 22-Aug-31 19:37 snaptrade/__init__.py
 -rw-rw-r--  2.0 unx     2458 b- defN 22-Nov-04 17:57 snaptrade/utils.py
--rw-rw-r--  2.0 unx       73 b- defN 22-Aug-31 19:37 snaptrade/api_client/__init__.py
+-rw-rw-r--  2.0 unx      248 b- defN 23-Apr-21 13:56 snaptrade/api_client/__init__.py
 -rw-rw-r--  2.0 unx    22752 b- defN 23-Jan-19 19:31 snaptrade/api_client/endpoints.json
--rw-rw-r--  2.0 unx    29589 b- defN 23-Jan-19 19:31 snaptrade/api_client/snaptrade_api_client.py
+-rw-rw-r--  2.0 unx    29589 b- defN 23-Apr-21 13:56 snaptrade/api_client/snaptrade_api_client.py
 -rw-rw-r--  2.0 unx        0 b- defN 22-Aug-31 19:32 tests/__init__.py
--rw-rw-r--  2.0 unx      548 b- defN 23-Jan-19 19:32 snaptrade-1.0.8.dist-info/LICENSE
--rw-rw-r--  2.0 unx     4342 b- defN 23-Jan-19 19:32 snaptrade-1.0.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jan-19 19:32 snaptrade-1.0.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx       16 b- defN 23-Jan-19 19:32 snaptrade-1.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      898 b- defN 23-Jan-19 19:32 snaptrade-1.0.8.dist-info/RECORD
-11 files, 60768 bytes uncompressed, 9357 bytes compressed:  84.6%
+-rw-rw-r--  2.0 unx      548 b- defN 23-Apr-21 13:57 snaptrade-1.0.9.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     4531 b- defN 23-Apr-21 13:57 snaptrade-1.0.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-21 13:57 snaptrade-1.0.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       16 b- defN 23-Apr-21 13:57 snaptrade-1.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      899 b- defN 23-Apr-21 13:57 snaptrade-1.0.9.dist-info/RECORD
+11 files, 61133 bytes uncompressed, 9580 bytes compressed:  84.3%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: snaptrade/api_client/snaptrade_api_client.py
 Comment: 
 
 Filename: tests/__init__.py
 Comment: 
 
-Filename: snaptrade-1.0.8.dist-info/LICENSE
+Filename: snaptrade-1.0.9.dist-info/LICENSE
 Comment: 
 
-Filename: snaptrade-1.0.8.dist-info/METADATA
+Filename: snaptrade-1.0.9.dist-info/METADATA
 Comment: 
 
-Filename: snaptrade-1.0.8.dist-info/WHEEL
+Filename: snaptrade-1.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: snaptrade-1.0.8.dist-info/top_level.txt
+Filename: snaptrade-1.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: snaptrade-1.0.8.dist-info/RECORD
+Filename: snaptrade-1.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## snaptrade/api_client/__init__.py

```diff
@@ -1 +1,2 @@
 from snaptrade.api_client.snaptrade_api_client import SnapTradeAPIClient
+print("*** This Python Package has been deprecated and is no longer receiving support. Please use our maintained SDK here: https://pypi.org/project/snaptrade-python-sdk/ ***")
```

## Comparing `snaptrade-1.0.8.dist-info/LICENSE` & `snaptrade-1.0.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `snaptrade-1.0.8.dist-info/METADATA` & `snaptrade-1.0.9.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 Metadata-Version: 2.1
 Name: snaptrade
-Version: 1.0.8
+Version: 1.0.9
 Summary: A Python implementation of SnapTrade API client library
-Classifier: Development Status :: 5 - Production/Stable
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Development Status :: 7 - Inactive
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: pycryptodome
 
+
 # SnapTrade-Python
-A SnapTrade python client library to help you make requests to the [SnapTrade API][1] endpoints more easily.
 
+This Python Package has been deprecated and is no longer receiving support. Please use our maintained SDK here: https://pypi.org/project/snaptrade-python-sdk/
+
+A SnapTrade python client library to help you make requests to the [SnapTrade API][1] endpoints more easily.
 
 If you need help or have any questions, send us an email at [api@snaptrade.com][contact].
 
 ## Requirements and Installation
 ### Python version requirements
 * Python 3.6 or later
 
@@ -99,7 +104,9 @@
 [Connections Endpoints]: https://github.com/passiv/snaptrade-python-sdk/blob/main/docs/connections-endpoints.md
 [Reference Data Endpoints]: https://github.com/passiv/snaptrade-python-sdk/blob/main/docs/reference-data-endpoints.md
 [Reporting Endpoints]: https://github.com/passiv/snaptrade-python-sdk/blob/main/docs/reporting-endpoints.md
 [Trading Endpoints]: https://github.com/passiv/snaptrade-python-sdk/blob/main/docs/trading-endpoints.md
 [Development Tools Endpoints]: https://github.com/passiv/snaptrade-python-sdk/blob/main/docs/development-tools-endpoint.md
 [Installing using pip and virtual environments]: https://packaging.python.org/en/latest/guides/installing-using-pip-and-virtual-environments/
 [2]: LICENSE
+
+
```

