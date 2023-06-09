# Comparing `tmp/PanjSim-1.0.3.tar.gz` & `tmp/PanjSim-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PanjSim-1.0.3.tar", last modified: Fri Jun  9 03:09:49 2023, max compression
+gzip compressed data, was "PanjSim-1.0.4.tar", last modified: Fri Jun  9 05:56:47 2023, max compression
```

## Comparing `PanjSim-1.0.3.tar` & `PanjSim-1.0.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 03:09:49.624508 PanjSim-1.0.3/
--rw-rw-rw-   0        0        0     1091 2023-06-06 13:41:52.000000 PanjSim-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     5169 2023-06-09 03:09:49.622503 PanjSim-1.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-09 03:09:49.514505 PanjSim-1.0.3/PanjSim/
--rw-rw-rw-   0        0        0    57337 2023-06-06 01:55:37.000000 PanjSim-1.0.3/PanjSim/Countrys.py
--rw-rw-rw-   0        0        0       40 2023-06-05 03:38:25.000000 PanjSim-1.0.3/PanjSim/__init__.py
--rw-rw-rw-   0        0        0     2853 2023-06-06 01:26:56.000000 PanjSim-1.0.3/PanjSim/client.py
--rw-rw-rw-   0        0        0     2472 2023-06-09 02:45:24.000000 PanjSim-1.0.3/PanjSim/errors.py
--rw-rw-rw-   0        0        0     4938 2023-06-09 02:46:33.000000 PanjSim-1.0.3/PanjSim/http_client.py
-drwxrwxrwx   0        0        0        0 2023-06-09 03:09:49.572507 PanjSim-1.0.3/PanjSim/products/
--rw-rw-rw-   0        0        0        0 2023-06-04 01:16:18.000000 PanjSim-1.0.3/PanjSim/products/__init__.py
--rw-rw-rw-   0        0        0      988 2023-06-06 01:29:31.000000 PanjSim-1.0.3/PanjSim/products/products.py
-drwxrwxrwx   0        0        0        0 2023-06-09 03:09:49.582503 PanjSim-1.0.3/PanjSim/purchase/
--rw-rw-rw-   0        0        0        0 2023-06-04 02:57:26.000000 PanjSim-1.0.3/PanjSim/purchase/__init__.py
--rw-rw-rw-   0        0        0     1109 2023-06-05 00:44:28.000000 PanjSim-1.0.3/PanjSim/purchase/management.py
--rw-rw-rw-   0        0        0     1757 2023-06-05 04:14:39.000000 PanjSim-1.0.3/PanjSim/purchase/purchase.py
-drwxrwxrwx   0        0        0        0 2023-06-09 03:09:49.599507 PanjSim-1.0.3/PanjSim/types/
--rw-rw-rw-   0        0        0      124 2023-06-06 01:41:13.000000 PanjSim-1.0.3/PanjSim/types/__init__.py
--rw-rw-rw-   0        0        0     1302 2023-06-06 01:32:51.000000 PanjSim-1.0.3/PanjSim/types/_operators.py
--rw-rw-rw-   0        0        0      335 2023-06-06 01:38:10.000000 PanjSim-1.0.3/PanjSim/types/_order.py
--rw-rw-rw-   0        0        0     7621 2023-06-06 01:38:43.000000 PanjSim-1.0.3/PanjSim/types/_products.py
-drwxrwxrwx   0        0        0        0 2023-06-09 03:09:49.608502 PanjSim-1.0.3/PanjSim/user/
--rw-rw-rw-   0        0        0        0 2023-06-04 00:41:18.000000 PanjSim-1.0.3/PanjSim/user/__init__.py
--rw-rw-rw-   0        0        0     1309 2023-06-05 02:57:45.000000 PanjSim-1.0.3/PanjSim/user/user.py
-drwxrwxrwx   0        0        0        0 2023-06-09 03:09:49.617508 PanjSim-1.0.3/PanjSim/vendor/
--rw-rw-rw-   0        0        0        0 2023-06-04 01:16:18.000000 PanjSim-1.0.3/PanjSim/vendor/__init__.py
--rw-rw-rw-   0        0        0     1877 2023-06-04 04:03:39.000000 PanjSim-1.0.3/PanjSim/vendor/vendor.py
-drwxrwxrwx   0        0        0        0 2023-06-09 03:09:49.566511 PanjSim-1.0.3/PanjSim.egg-info/
--rw-rw-rw-   0        0        0     5169 2023-06-09 03:09:49.000000 PanjSim-1.0.3/PanjSim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      644 2023-06-09 03:09:49.000000 PanjSim-1.0.3/PanjSim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 03:09:49.000000 PanjSim-1.0.3/PanjSim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-09 03:09:49.000000 PanjSim-1.0.3/PanjSim.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-09 03:09:49.000000 PanjSim-1.0.3/PanjSim.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3849 2023-06-09 03:08:46.000000 PanjSim-1.0.3/README.md
--rw-rw-rw-   0        0        0       99 2023-06-06 04:27:45.000000 PanjSim-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-09 03:09:49.624508 PanjSim-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1432 2023-06-09 03:08:25.000000 PanjSim-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 05:56:47.719193 PanjSim-1.0.4/
+-rw-rw-rw-   0        0        0     1091 2023-06-06 13:41:52.000000 PanjSim-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0     5218 2023-06-09 05:56:47.717192 PanjSim-1.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-09 05:56:47.574200 PanjSim-1.0.4/PanjSim/
+-rw-rw-rw-   0        0        0    57337 2023-06-06 01:55:37.000000 PanjSim-1.0.4/PanjSim/Countrys.py
+-rw-rw-rw-   0        0        0       40 2023-06-05 03:38:25.000000 PanjSim-1.0.4/PanjSim/__init__.py
+-rw-rw-rw-   0        0        0     2876 2023-06-09 05:55:19.000000 PanjSim-1.0.4/PanjSim/client.py
+-rw-rw-rw-   0        0        0     2472 2023-06-09 02:45:24.000000 PanjSim-1.0.4/PanjSim/errors.py
+-rw-rw-rw-   0        0        0     4938 2023-06-09 02:46:33.000000 PanjSim-1.0.4/PanjSim/http_client.py
+drwxrwxrwx   0        0        0        0 2023-06-09 05:56:47.660186 PanjSim-1.0.4/PanjSim/products/
+-rw-rw-rw-   0        0        0        0 2023-06-04 01:16:18.000000 PanjSim-1.0.4/PanjSim/products/__init__.py
+-rw-rw-rw-   0        0        0      988 2023-06-06 01:29:31.000000 PanjSim-1.0.4/PanjSim/products/products.py
+drwxrwxrwx   0        0        0        0 2023-06-09 05:56:47.673187 PanjSim-1.0.4/PanjSim/purchase/
+-rw-rw-rw-   0        0        0        0 2023-06-04 02:57:26.000000 PanjSim-1.0.4/PanjSim/purchase/__init__.py
+-rw-rw-rw-   0        0        0     1109 2023-06-05 00:44:28.000000 PanjSim-1.0.4/PanjSim/purchase/management.py
+-rw-rw-rw-   0        0        0     1757 2023-06-05 04:14:39.000000 PanjSim-1.0.4/PanjSim/purchase/purchase.py
+drwxrwxrwx   0        0        0        0 2023-06-09 05:56:47.696192 PanjSim-1.0.4/PanjSim/types/
+-rw-rw-rw-   0        0        0      124 2023-06-06 01:41:13.000000 PanjSim-1.0.4/PanjSim/types/__init__.py
+-rw-rw-rw-   0        0        0     1302 2023-06-06 01:32:51.000000 PanjSim-1.0.4/PanjSim/types/_operators.py
+-rw-rw-rw-   0        0        0      335 2023-06-06 01:38:10.000000 PanjSim-1.0.4/PanjSim/types/_order.py
+-rw-rw-rw-   0        0        0     7621 2023-06-06 01:38:43.000000 PanjSim-1.0.4/PanjSim/types/_products.py
+drwxrwxrwx   0        0        0        0 2023-06-09 05:56:47.706193 PanjSim-1.0.4/PanjSim/user/
+-rw-rw-rw-   0        0        0        0 2023-06-04 00:41:18.000000 PanjSim-1.0.4/PanjSim/user/__init__.py
+-rw-rw-rw-   0        0        0     1309 2023-06-05 02:57:45.000000 PanjSim-1.0.4/PanjSim/user/user.py
+drwxrwxrwx   0        0        0        0 2023-06-09 05:56:47.713193 PanjSim-1.0.4/PanjSim/vendor/
+-rw-rw-rw-   0        0        0        0 2023-06-04 01:16:18.000000 PanjSim-1.0.4/PanjSim/vendor/__init__.py
+-rw-rw-rw-   0        0        0     1877 2023-06-04 04:03:39.000000 PanjSim-1.0.4/PanjSim/vendor/vendor.py
+drwxrwxrwx   0        0        0        0 2023-06-09 05:56:47.654190 PanjSim-1.0.4/PanjSim.egg-info/
+-rw-rw-rw-   0        0        0     5218 2023-06-09 05:56:47.000000 PanjSim-1.0.4/PanjSim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      644 2023-06-09 05:56:47.000000 PanjSim-1.0.4/PanjSim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 05:56:47.000000 PanjSim-1.0.4/PanjSim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-09 05:56:47.000000 PanjSim-1.0.4/PanjSim.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-09 05:56:47.000000 PanjSim-1.0.4/PanjSim.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3894 2023-06-09 05:46:58.000000 PanjSim-1.0.4/README.md
+-rw-rw-rw-   0        0        0       99 2023-06-06 04:27:45.000000 PanjSim-1.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-09 05:56:47.720196 PanjSim-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1432 2023-06-09 05:45:49.000000 PanjSim-1.0.4/setup.py
```

### Comparing `PanjSim-1.0.3/LICENSE` & `PanjSim-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `PanjSim-1.0.3/PKG-INFO` & `PanjSim-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PanjSim
-Version: 1.0.3
+Version: 1.0.4
 Summary: A simple Python API for 5sim.net
 Home-page: https://github.com/abbas-bachari/PanjSim
 Author: Abbas Bachari
 Author-email: abbas-bachari@hotmail.com
 License: MIT
 Project-URL: Homepage, https://github.com/abbas-bachari/PanjSim
 Project-URL: Documentation, https://github.com/abbas-bachari/PanjSim
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![PanjSim](https://img.shields.io/badge/PanjSim%20-Version%201.0.3-green?style=plastic&logo=codemagic)](https://python.org)
+[![PanjSim](https://img.shields.io/badge/PanjSim%20-Version%201.0.4-green?style=plastic&logo=codemagic)](https://python.org)
 [![python](https://img.shields.io/badge/Python%20-3.7+-green?style=plastic&logo=Python)](https://python.org)
 
 
 
 
 # What is PanjSim ? ([فارسی](https://github.com/abbas-bachari/PanjSim/blob/main/README-fa.md))
 A simple Python API for [5sim.net](https://5sim.net)
@@ -50,15 +50,19 @@
 ``` bash
 pip install git+https://github.com/abbas-bachari/PanjSim.git
 ```
 
 Alternatively, install from [PyPI](https://pypi.org/project/PanjSim/):
 
 ```bash
+# Install:
 pip install PanjSim
+
+# Update:
+pip install -U PanjSim
 ```
 <hr>
 
 ## user manual
 
 ###  Client
```

### Comparing `PanjSim-1.0.3/PanjSim/Countrys.py` & `PanjSim-1.0.4/PanjSim/Countrys.py`

 * *Files identical despite different names*

### Comparing `PanjSim-1.0.3/PanjSim/client.py` & `PanjSim-1.0.4/PanjSim/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         return response.json()
     
     def get_notification(self,lang:str) -> dict[str, Any]:
         '* lang: Language of notification, ru/en'
         endpoint = f"/v1/guest/flash/{lang}"
         response = self.session.get(endpoint)
         return response.json()
-    def find_low_price(self,product:str,limit:int=10) -> dict|list:
+    def find_low_price(self,product:str,limit:int=10,available:int=1) -> dict|list:
         '''
         * if limit = 1 return dict low country price else return cost list
         + return {'cost': 8.4, 'count': 2741, 'rate': 6.84, 'contry': 'india', 'operator': 'virtual4'}
         + or: 
         + return [{'cost': 8.4, 'count': 2741, 'rate': 6.84, 'contry': 'india', 'operator': 'virtual4'}]
         '''
         product_price=self.Products().get_prices(product=product)
@@ -61,15 +61,15 @@
         new=[]
         
         for k in product_price_data:
             v=product_price_data[k]
             nv=[]
             for x,y in v.items():
                 
-                if y['count'] >=100:
+                if y['count'] >= available:
                     nv.append((x,y))
 
             
             _sorted = sorted(nv, key=lambda x:x[1].get('cost'))
             if _sorted:
                 dat=_sorted[0][1]
                 dat['contry']=k
```

### Comparing `PanjSim-1.0.3/PanjSim/errors.py` & `PanjSim-1.0.4/PanjSim/errors.py`

 * *Files identical despite different names*

### Comparing `PanjSim-1.0.3/PanjSim/http_client.py` & `PanjSim-1.0.4/PanjSim/http_client.py`

 * *Files identical despite different names*

### Comparing `PanjSim-1.0.3/PanjSim/products/products.py` & `PanjSim-1.0.4/PanjSim/products/products.py`

 * *Files identical despite different names*

### Comparing `PanjSim-1.0.3/PanjSim/purchase/management.py` & `PanjSim-1.0.4/PanjSim/purchase/management.py`

 * *Files identical despite different names*

### Comparing `PanjSim-1.0.3/PanjSim/purchase/purchase.py` & `PanjSim-1.0.4/PanjSim/purchase/purchase.py`

 * *Files identical despite different names*

### Comparing `PanjSim-1.0.3/PanjSim/types/_operators.py` & `PanjSim-1.0.4/PanjSim/types/_operators.py`

 * *Files identical despite different names*

### Comparing `PanjSim-1.0.3/PanjSim/types/_products.py` & `PanjSim-1.0.4/PanjSim/types/_products.py`

 * *Files identical despite different names*

### Comparing `PanjSim-1.0.3/PanjSim/user/user.py` & `PanjSim-1.0.4/PanjSim/user/user.py`

 * *Files identical despite different names*

### Comparing `PanjSim-1.0.3/PanjSim/vendor/vendor.py` & `PanjSim-1.0.4/PanjSim/vendor/vendor.py`

 * *Files identical despite different names*

### Comparing `PanjSim-1.0.3/PanjSim.egg-info/PKG-INFO` & `PanjSim-1.0.4/PanjSim.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PanjSim
-Version: 1.0.3
+Version: 1.0.4
 Summary: A simple Python API for 5sim.net
 Home-page: https://github.com/abbas-bachari/PanjSim
 Author: Abbas Bachari
 Author-email: abbas-bachari@hotmail.com
 License: MIT
 Project-URL: Homepage, https://github.com/abbas-bachari/PanjSim
 Project-URL: Documentation, https://github.com/abbas-bachari/PanjSim
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![PanjSim](https://img.shields.io/badge/PanjSim%20-Version%201.0.3-green?style=plastic&logo=codemagic)](https://python.org)
+[![PanjSim](https://img.shields.io/badge/PanjSim%20-Version%201.0.4-green?style=plastic&logo=codemagic)](https://python.org)
 [![python](https://img.shields.io/badge/Python%20-3.7+-green?style=plastic&logo=Python)](https://python.org)
 
 
 
 
 # What is PanjSim ? ([فارسی](https://github.com/abbas-bachari/PanjSim/blob/main/README-fa.md))
 A simple Python API for [5sim.net](https://5sim.net)
@@ -50,15 +50,19 @@
 ``` bash
 pip install git+https://github.com/abbas-bachari/PanjSim.git
 ```
 
 Alternatively, install from [PyPI](https://pypi.org/project/PanjSim/):
 
 ```bash
+# Install:
 pip install PanjSim
+
+# Update:
+pip install -U PanjSim
 ```
 <hr>
 
 ## user manual
 
 ###  Client
```

### Comparing `PanjSim-1.0.3/PanjSim.egg-info/SOURCES.txt` & `PanjSim-1.0.4/PanjSim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PanjSim-1.0.3/README.md` & `PanjSim-1.0.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![PanjSim](https://img.shields.io/badge/PanjSim%20-Version%201.0.3-green?style=plastic&logo=codemagic)](https://python.org)
+[![PanjSim](https://img.shields.io/badge/PanjSim%20-Version%201.0.4-green?style=plastic&logo=codemagic)](https://python.org)
 [![python](https://img.shields.io/badge/Python%20-3.7+-green?style=plastic&logo=Python)](https://python.org)
 
 
 
 
 # What is PanjSim ? ([فارسی](https://github.com/abbas-bachari/PanjSim/blob/main/README-fa.md))
 A simple Python API for [5sim.net](https://5sim.net)
@@ -24,15 +24,19 @@
 ``` bash
 pip install git+https://github.com/abbas-bachari/PanjSim.git
 ```
 
 Alternatively, install from [PyPI](https://pypi.org/project/PanjSim/):
 
 ```bash
+# Install:
 pip install PanjSim
+
+# Update:
+pip install -U PanjSim
 ```
 <hr>
 
 ## user manual
 
 ###  Client
```

### Comparing `PanjSim-1.0.3/setup.py` & `PanjSim-1.0.4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='PanjSim',
-    version='1.0.3',
+    version='1.0.4',
     author='Abbas Bachari',
     author_email='abbas-bachari@hotmail.com',
     description='A simple Python API for 5sim.net',
     long_description=open('README.md',encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     license='MIT',
     packages=find_packages(),
```

