# Comparing `tmp/python_strategies_breezeconnect-1.0.tar.gz` & `tmp/python_strategies_breezeconnect-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_strategies_breezeconnect-1.0.tar", last modified: Fri Jun  9 09:34:05 2023, max compression
+gzip compressed data, was "python_strategies_breezeconnect-2.0.tar", last modified: Fri Jun  9 09:43:09 2023, max compression
```

## Comparing `python_strategies_breezeconnect-1.0.tar` & `python_strategies_breezeconnect-2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 09:34:05.147163 python_strategies_breezeconnect-1.0/
--rw-rw-rw-   0        0        0     1113 2023-06-09 09:29:34.000000 python_strategies_breezeconnect-1.0/LICENSE
--rw-rw-rw-   0        0        0     1256 2023-06-09 09:34:05.145760 python_strategies_breezeconnect-1.0/PKG-INFO
--rw-rw-rw-   0        0        0      731 2023-06-09 09:26:14.000000 python_strategies_breezeconnect-1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-09 09:34:05.082725 python_strategies_breezeconnect-1.0/python_strategies/
--rw-rw-rw-   0        0        0       58 2023-06-09 09:24:56.000000 python_strategies_breezeconnect-1.0/python_strategies/__init__.py
--rw-rw-rw-   0        0        0    18205 2023-06-09 09:29:49.000000 python_strategies_breezeconnect-1.0/python_strategies/python_strategies.py
-drwxrwxrwx   0        0        0        0 2023-06-09 09:34:05.142277 python_strategies_breezeconnect-1.0/python_strategies_breezeconnect.egg-info/
--rw-rw-rw-   0        0        0     1256 2023-06-09 09:34:04.000000 python_strategies_breezeconnect-1.0/python_strategies_breezeconnect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      369 2023-06-09 09:34:04.000000 python_strategies_breezeconnect-1.0/python_strategies_breezeconnect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 09:34:04.000000 python_strategies_breezeconnect-1.0/python_strategies_breezeconnect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-06-09 09:34:04.000000 python_strategies_breezeconnect-1.0/python_strategies_breezeconnect.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-06-09 09:34:04.000000 python_strategies_breezeconnect-1.0/python_strategies_breezeconnect.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-09 09:34:05.147163 python_strategies_breezeconnect-1.0/setup.cfg
--rw-rw-rw-   0        0        0      787 2023-06-09 09:32:50.000000 python_strategies_breezeconnect-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 09:43:09.946557 python_strategies_breezeconnect-2.0/
+-rw-rw-rw-   0        0        0     1113 2023-06-09 09:29:34.000000 python_strategies_breezeconnect-2.0/LICENSE
+-rw-rw-rw-   0        0        0     1274 2023-06-09 09:43:09.941171 python_strategies_breezeconnect-2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      749 2023-06-09 09:42:38.000000 python_strategies_breezeconnect-2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-09 09:43:09.896136 python_strategies_breezeconnect-2.0/python_strategies/
+-rw-rw-rw-   0        0        0       58 2023-06-09 09:24:56.000000 python_strategies_breezeconnect-2.0/python_strategies/__init__.py
+-rw-rw-rw-   0        0        0    18215 2023-06-09 09:43:03.000000 python_strategies_breezeconnect-2.0/python_strategies/python_strategies.py
+drwxrwxrwx   0        0        0        0 2023-06-09 09:43:09.937172 python_strategies_breezeconnect-2.0/python_strategies_breezeconnect.egg-info/
+-rw-rw-rw-   0        0        0     1274 2023-06-09 09:43:09.000000 python_strategies_breezeconnect-2.0/python_strategies_breezeconnect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      369 2023-06-09 09:43:09.000000 python_strategies_breezeconnect-2.0/python_strategies_breezeconnect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 09:43:09.000000 python_strategies_breezeconnect-2.0/python_strategies_breezeconnect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-06-09 09:43:09.000000 python_strategies_breezeconnect-2.0/python_strategies_breezeconnect.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-06-09 09:43:09.000000 python_strategies_breezeconnect-2.0/python_strategies_breezeconnect.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-09 09:43:09.947927 python_strategies_breezeconnect-2.0/setup.cfg
+-rw-rw-rw-   0        0        0      787 2023-06-09 09:41:39.000000 python_strategies_breezeconnect-2.0/setup.py
```

### Comparing `python_strategies_breezeconnect-1.0/LICENSE` & `python_strategies_breezeconnect-2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_strategies_breezeconnect-1.0/PKG-INFO` & `python_strategies_breezeconnect-2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: python_strategies_breezeconnect
-Version: 1.0
+Version: 2.0
 Summary: breeze connect strategies in python
 Home-page: https://github.com/pypa/sampleproject
 Author: UAT python strategy Breeze Connect
 Author-email: test@mail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# python_strategies
+# UAT  python_strategies
 
-## Steps to install Strategy Library
+## Steps to install Strategy Library for UAT
 
 
 ```python
 
-pip install python_strategies_breezeconnect
+pip install python_strategies_breezeconnect==2.0
 
 ```
 
 
 ## code usage
 
 ```python
```

### Comparing `python_strategies_breezeconnect-1.0/README.md` & `python_strategies_breezeconnect-2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-# python_strategies
+# UAT  python_strategies
 
-## Steps to install Strategy Library
+## Steps to install Strategy Library for UAT
 
 
 ```python
 
-pip install python_strategies_breezeconnect
+pip install python_strategies_breezeconnect==2.0
 
 ```
 
 
 ## code usage
 
 ```python
```

### Comparing `python_strategies_breezeconnect-1.0/python_strategies/python_strategies.py` & `python_strategies_breezeconnect-2.0/python_strategies/python_strategies.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 
 class Strategies:
     
     #initialize strategy object
     def __init__(self,app_key,secret_key,api_session,max_profit,max_loss):
         
         
-        self.maxloss = max_loss
-        self.maxprofit = max_profit
+        self.maxloss = int(max_loss)
+        self.maxprofit = int(max_profit)
         self.calllock = threading.Lock()
         self.putlock = threading.Lock()
         self.currentcall = 0
         self.currentput = 0
         self.flag = False
         self.client = BreezeConnect(app_key)
         self.client.generate_session(secret_key,api_session)
```

### Comparing `python_strategies_breezeconnect-1.0/python_strategies_breezeconnect.egg-info/PKG-INFO` & `python_strategies_breezeconnect-2.0/python_strategies_breezeconnect.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: python-strategies-breezeconnect
-Version: 1.0
+Version: 2.0
 Summary: breeze connect strategies in python
 Home-page: https://github.com/pypa/sampleproject
 Author: UAT python strategy Breeze Connect
 Author-email: test@mail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# python_strategies
+# UAT  python_strategies
 
-## Steps to install Strategy Library
+## Steps to install Strategy Library for UAT
 
 
 ```python
 
-pip install python_strategies_breezeconnect
+pip install python_strategies_breezeconnect==2.0
 
 ```
 
 
 ## code usage
 
 ```python
```

### Comparing `python_strategies_breezeconnect-1.0/setup.py` & `python_strategies_breezeconnect-2.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="python_strategies_breezeconnect",
-    version="1.0",
+    version="2.0",
     author="UAT python strategy Breeze Connect",
     author_email="test@mail.com",
     description="breeze connect strategies in python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=['uat-breeze-connect','nest_asyncio'],
     url="https://github.com/pypa/sampleproject",
```

