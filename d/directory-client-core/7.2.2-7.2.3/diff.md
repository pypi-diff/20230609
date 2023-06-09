# Comparing `tmp/directory_client_core-7.2.2-py3-none-any.whl.zip` & `tmp/directory_client_core-7.2.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 8151 bytes, number of entries: 10
--rw-r--r--  2.0 unx        0 b- defN 23-May-24 09:53 directory_client_core/__init__.py
--rw-r--r--  2.0 unx      876 b- defN 23-May-24 09:53 directory_client_core/authentication.py
--rw-r--r--  2.0 unx     4876 b- defN 23-May-24 09:53 directory_client_core/base.py
--rw-r--r--  2.0 unx      381 b- defN 23-May-24 09:53 directory_client_core/cache_control.py
--rw-r--r--  2.0 unx     5008 b- defN 23-May-24 09:53 directory_client_core/helpers.py
--rw-r--r--  2.0 unx     1091 b- defN 23-May-24 09:54 directory_client_core-7.2.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     5267 b- defN 23-May-24 09:54 directory_client_core-7.2.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-24 09:54 directory_client_core-7.2.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       22 b- defN 23-May-24 09:54 directory_client_core-7.2.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      907 b- defN 23-May-24 09:54 directory_client_core-7.2.2.dist-info/RECORD
-10 files, 18520 bytes uncompressed, 6569 bytes compressed:  64.5%
+Zip file size: 8148 bytes, number of entries: 10
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-09 14:56 directory_client_core/__init__.py
+-rw-r--r--  2.0 unx      876 b- defN 23-Jun-09 14:56 directory_client_core/authentication.py
+-rw-r--r--  2.0 unx     4876 b- defN 23-Jun-09 14:56 directory_client_core/base.py
+-rw-r--r--  2.0 unx      381 b- defN 23-Jun-09 14:56 directory_client_core/cache_control.py
+-rw-r--r--  2.0 unx     5008 b- defN 23-Jun-09 14:56 directory_client_core/helpers.py
+-rw-r--r--  2.0 unx     1091 b- defN 23-Jun-09 14:56 directory_client_core-7.2.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5267 b- defN 23-Jun-09 14:56 directory_client_core-7.2.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-09 14:56 directory_client_core-7.2.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       22 b- defN 23-Jun-09 14:56 directory_client_core-7.2.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      907 b- defN 23-Jun-09 14:56 directory_client_core-7.2.3.dist-info/RECORD
+10 files, 18520 bytes uncompressed, 6566 bytes compressed:  64.5%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: directory_client_core/cache_control.py
 Comment: 
 
 Filename: directory_client_core/helpers.py
 Comment: 
 
-Filename: directory_client_core-7.2.2.dist-info/LICENSE
+Filename: directory_client_core-7.2.3.dist-info/LICENSE
 Comment: 
 
-Filename: directory_client_core-7.2.2.dist-info/METADATA
+Filename: directory_client_core-7.2.3.dist-info/METADATA
 Comment: 
 
-Filename: directory_client_core-7.2.2.dist-info/WHEEL
+Filename: directory_client_core-7.2.3.dist-info/WHEEL
 Comment: 
 
-Filename: directory_client_core-7.2.2.dist-info/top_level.txt
+Filename: directory_client_core-7.2.3.dist-info/top_level.txt
 Comment: 
 
-Filename: directory_client_core-7.2.2.dist-info/RECORD
+Filename: directory_client_core-7.2.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `directory_client_core-7.2.2.dist-info/LICENSE` & `directory_client_core-7.2.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `directory_client_core-7.2.2.dist-info/METADATA` & `directory_client_core-7.2.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: directory-client-core
-Version: 7.2.2
+Version: 7.2.3
 Summary: Python common code for Directory API clients.
 Home-page: https://github.com/uktrade/directory-client-core
 Author: Department for International Trade
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
@@ -22,15 +22,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 Requires-Dist: requests (<3.0.0,>=2.21.0)
 Requires-Dist: monotonic (<3.0,>=1.2)
-Requires-Dist: sigauth (<=5.2.0,>=4.0.1)
+Requires-Dist: sigauth (<=5.2.1,>=4.0.1)
 Requires-Dist: django (<=4.2,>=3.2.18)
 Requires-Dist: w3lib (<2.0.0,>=1.19.0)
 Provides-Extra: test
 Requires-Dist: flake8 (==5.0.4) ; extra == 'test'
 Requires-Dist: freezegun (==1.0.0) ; extra == 'test'
 Requires-Dist: pytest-django (==4.1.0) ; extra == 'test'
 Requires-Dist: pytest-sugar (==0.9.5) ; extra == 'test'
```

## Comparing `directory_client_core-7.2.2.dist-info/RECORD` & `directory_client_core-7.2.3.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 directory_client_core/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 directory_client_core/authentication.py,sha256=O8pHGxAeJNXQW3Lbp5UH0t27bVNuC0713TbyHkvQwgc,876
 directory_client_core/base.py,sha256=E0__Zvam04P0tpui1BfAee08jF0XGszzjKK55tYUFcM,4876
 directory_client_core/cache_control.py,sha256=wbkMabzKYZqOfP6HeO-ebZu4mpL0gYMUevpE1ICLTw0,381
 directory_client_core/helpers.py,sha256=tJxXGDS6Bg5ZaX6y2OkLHOYnngLQWIssX2lclWJGzxw,5008
-directory_client_core-7.2.2.dist-info/LICENSE,sha256=y-ArErAQz98OorLek2xntwEp9bo3ZcqfQMtAIcjBdvQ,1091
-directory_client_core-7.2.2.dist-info/METADATA,sha256=tmW_mFq9sNtAPgXhSwe155Z6Gz92dNfv5kTmkx8ErKA,5267
-directory_client_core-7.2.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-directory_client_core-7.2.2.dist-info/top_level.txt,sha256=hX51yuY3cBj41kaAYbfK-nJQlF8tuTg6gVVRtqIXCg4,22
-directory_client_core-7.2.2.dist-info/RECORD,,
+directory_client_core-7.2.3.dist-info/LICENSE,sha256=y-ArErAQz98OorLek2xntwEp9bo3ZcqfQMtAIcjBdvQ,1091
+directory_client_core-7.2.3.dist-info/METADATA,sha256=ep-BBXP-pJfa-dRDzLWYzzwykvht0HCLLPLoYwBFxTw,5267
+directory_client_core-7.2.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+directory_client_core-7.2.3.dist-info/top_level.txt,sha256=hX51yuY3cBj41kaAYbfK-nJQlF8tuTg6gVVRtqIXCg4,22
+directory_client_core-7.2.3.dist-info/RECORD,,
```

