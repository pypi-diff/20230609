# Comparing `tmp/pyNekobin-1.1.tar.gz` & `tmp/pyNekobin-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyNekobin-1.1.tar", last modified: Fri Jun  9 06:12:07 2023, max compression
+gzip compressed data, was "pyNekobin-2.1.tar", last modified: Fri Jun  9 06:25:44 2023, max compression
```

## Comparing `pyNekobin-1.1.tar` & `pyNekobin-2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 06:12:07.477273 pyNekobin-1.1/
--rw-rw-rw-   0        0        0     1052 2023-06-09 04:43:38.000000 pyNekobin-1.1/LICENSE
--rw-rw-rw-   0        0        0     3544 2023-06-09 06:12:07.476257 pyNekobin-1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2658 2023-06-09 06:11:40.000000 pyNekobin-1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-09 06:12:07.406244 pyNekobin-1.1/nekobin/
--rw-rw-rw-   0        0        0       50 2023-06-09 05:33:33.000000 pyNekobin-1.1/nekobin/__init__.py
--rw-rw-rw-   0        0        0     4312 2023-06-09 06:01:48.000000 pyNekobin-1.1/nekobin/main.py
-drwxrwxrwx   0        0        0        0 2023-06-09 06:12:07.473261 pyNekobin-1.1/pyNekobin.egg-info/
--rw-rw-rw-   0        0        0     3544 2023-06-09 06:12:07.000000 pyNekobin-1.1/pyNekobin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      226 2023-06-09 06:12:07.000000 pyNekobin-1.1/pyNekobin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 06:12:07.000000 pyNekobin-1.1/pyNekobin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-09 06:12:07.000000 pyNekobin-1.1/pyNekobin.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-09 06:12:07.000000 pyNekobin-1.1/pyNekobin.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-09 06:12:07.478259 pyNekobin-1.1/setup.cfg
--rw-rw-rw-   0        0        0     1654 2023-06-09 05:23:14.000000 pyNekobin-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:25:44.684325 pyNekobin-2.1/
+-rw-rw-rw-   0        0        0     1052 2023-06-09 04:43:38.000000 pyNekobin-2.1/LICENSE
+-rw-rw-rw-   0        0        0     3625 2023-06-09 06:25:44.672276 pyNekobin-2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2739 2023-06-09 06:15:18.000000 pyNekobin-2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-09 06:25:44.646271 pyNekobin-2.1/nekobin/
+-rw-rw-rw-   0        0        0       50 2023-06-09 06:12:36.000000 pyNekobin-2.1/nekobin/__init__.py
+-rw-rw-rw-   0        0        0     4339 2023-06-09 06:25:11.000000 pyNekobin-2.1/nekobin/main.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:25:44.669278 pyNekobin-2.1/pyNekobin.egg-info/
+-rw-rw-rw-   0        0        0     3625 2023-06-09 06:25:44.000000 pyNekobin-2.1/pyNekobin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      226 2023-06-09 06:25:44.000000 pyNekobin-2.1/pyNekobin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 06:25:44.000000 pyNekobin-2.1/pyNekobin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-09 06:25:44.000000 pyNekobin-2.1/pyNekobin.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-09 06:25:44.000000 pyNekobin-2.1/pyNekobin.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-09 06:25:44.684325 pyNekobin-2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1654 2023-06-09 05:23:14.000000 pyNekobin-2.1/setup.py
```

### Comparing `pyNekobin-1.1/LICENSE` & `pyNekobin-2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyNekobin-1.1/PKG-INFO` & `pyNekobin-2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pyNekobin
-Version: 1.1
+Version: 2.1
 Summary: Paste codes to Nekobin.com with python
 Home-page: https://github.com/Nusab19/pyNekobin
-Download-URL: https://github.com/Nusab19/pyNekobin/releases/tag/pyNekobin-1.1
+Download-URL: https://github.com/Nusab19/pyNekobin/releases/tag/pyNekobin-2.1
 Author: Nusab Taha
 Author-email: nusabtaha33@gmail.com
 License: MIT
 Keywords: Nekobin,pyNekobin,Paste Code,Paste Bin
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Education
@@ -79,21 +79,27 @@
 
 ## Advanced Usage
 
 As this package uses `httpx` under the hood, you can pass additional keyword arguments in each method call. You can pass any keyword argument that `httpx.AsyncClient` may take:
 
 ```python
 from nekobin import Nekobin
+import asyncio
 
 nb = Nekobin(timeout=10, headers={}, follow_redirects=True)
 ```
 
 If you want to pass these arguments in each method call, you have that too:
 
 ```python
+from nekobin import Nekobin
+import asyncio
+
+nb = Nekobin()
+
 async def main():
     result = await nb.paste("Hello, world!", timeout=10)
     url = result.url
     print("Pasted at:", url)
 
     content = (await nb.read(url, timeout=7)).content
     print("Content:", content)
```

### Comparing `pyNekobin-1.1/README.md` & `pyNekobin-2.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -56,21 +56,27 @@
 
 ## Advanced Usage
 
 As this package uses `httpx` under the hood, you can pass additional keyword arguments in each method call. You can pass any keyword argument that `httpx.AsyncClient` may take:
 
 ```python
 from nekobin import Nekobin
+import asyncio
 
 nb = Nekobin(timeout=10, headers={}, follow_redirects=True)
 ```
 
 If you want to pass these arguments in each method call, you have that too:
 
 ```python
+from nekobin import Nekobin
+import asyncio
+
+nb = Nekobin()
+
 async def main():
     result = await nb.paste("Hello, world!", timeout=10)
     url = result.url
     print("Pasted at:", url)
 
     content = (await nb.read(url, timeout=7)).content
     print("Content:", content)
```

### Comparing `pyNekobin-1.1/nekobin/main.py` & `pyNekobin-2.1/nekobin/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
 
         Returns:
             Objectify: An Objectify instance representing the result of the paste operation.
         """
         data = {'content': text}
         try:
-            r = await self.__SES.post(self._baseUrl, json=data, **kw)
+            r = await self.__SES.post(self._baseUrl[:-1], json=data, **kw)
             r = r.json()
 
         except json.decoder.JSONDecodeError as e:
             x = {"ok": False, "message": "Failed to parse json", "error": e}
             return Objectify(x)
 
         except Exception as e:
@@ -109,14 +109,15 @@
                 "error": Exception("URL is not Valid")
             }
 
             return Objectify(x)
 
         doc = url.split('/')[-1]
         r = await self.__SES.get(self._baseUrl + doc, **kw)
+        r = r.json()
 
         if not r.get("ok"):
             x = {
                 "ok": False,
                 "message": "Document not found in Nekobin Database",
                 "error": Exception(r.get("error").replace('_', ' '))
             }
```

### Comparing `pyNekobin-1.1/pyNekobin.egg-info/PKG-INFO` & `pyNekobin-2.1/pyNekobin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pyNekobin
-Version: 1.1
+Version: 2.1
 Summary: Paste codes to Nekobin.com with python
 Home-page: https://github.com/Nusab19/pyNekobin
-Download-URL: https://github.com/Nusab19/pyNekobin/releases/tag/pyNekobin-1.1
+Download-URL: https://github.com/Nusab19/pyNekobin/releases/tag/pyNekobin-2.1
 Author: Nusab Taha
 Author-email: nusabtaha33@gmail.com
 License: MIT
 Keywords: Nekobin,pyNekobin,Paste Code,Paste Bin
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Education
@@ -79,21 +79,27 @@
 
 ## Advanced Usage
 
 As this package uses `httpx` under the hood, you can pass additional keyword arguments in each method call. You can pass any keyword argument that `httpx.AsyncClient` may take:
 
 ```python
 from nekobin import Nekobin
+import asyncio
 
 nb = Nekobin(timeout=10, headers={}, follow_redirects=True)
 ```
 
 If you want to pass these arguments in each method call, you have that too:
 
 ```python
+from nekobin import Nekobin
+import asyncio
+
+nb = Nekobin()
+
 async def main():
     result = await nb.paste("Hello, world!", timeout=10)
     url = result.url
     print("Pasted at:", url)
 
     content = (await nb.read(url, timeout=7)).content
     print("Content:", content)
```

### Comparing `pyNekobin-1.1/setup.py` & `pyNekobin-2.1/setup.py`

 * *Files identical despite different names*

