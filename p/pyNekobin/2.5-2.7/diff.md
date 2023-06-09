# Comparing `tmp/pyNekobin-2.5.tar.gz` & `tmp/pyNekobin-2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyNekobin-2.5.tar", last modified: Fri Jun  9 10:42:33 2023, max compression
+gzip compressed data, was "pyNekobin-2.7.tar", last modified: Fri Jun  9 14:59:36 2023, max compression
```

## Comparing `pyNekobin-2.5.tar` & `pyNekobin-2.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 10:42:33.702330 pyNekobin-2.5/
--rw-rw-rw-   0        0        0     1052 2023-06-09 04:43:38.000000 pyNekobin-2.5/LICENSE
--rw-rw-rw-   0        0        0     3965 2023-06-09 10:42:33.700325 pyNekobin-2.5/PKG-INFO
--rw-rw-rw-   0        0        0     3081 2023-06-09 10:04:54.000000 pyNekobin-2.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-09 10:42:33.637317 pyNekobin-2.5/nekobin/
--rw-rw-rw-   0        0        0       52 2023-06-09 10:20:25.000000 pyNekobin-2.5/nekobin/__init__.py
--rw-rw-rw-   0        0        0     4355 2023-06-09 10:21:13.000000 pyNekobin-2.5/nekobin/main.py
-drwxrwxrwx   0        0        0        0 2023-06-09 10:42:33.698339 pyNekobin-2.5/pyNekobin.egg-info/
--rw-rw-rw-   0        0        0     3965 2023-06-09 10:42:33.000000 pyNekobin-2.5/pyNekobin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      226 2023-06-09 10:42:33.000000 pyNekobin-2.5/pyNekobin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 10:42:33.000000 pyNekobin-2.5/pyNekobin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-09 10:42:33.000000 pyNekobin-2.5/pyNekobin.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-09 10:42:33.000000 pyNekobin-2.5/pyNekobin.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-09 10:42:33.702330 pyNekobin-2.5/setup.cfg
--rw-rw-rw-   0        0        0     1639 2023-06-09 10:21:50.000000 pyNekobin-2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 14:59:36.455880 pyNekobin-2.7/
+-rw-rw-rw-   0        0        0     1052 2023-06-09 04:43:38.000000 pyNekobin-2.7/LICENSE
+-rw-rw-rw-   0        0        0     4154 2023-06-09 14:59:36.454880 pyNekobin-2.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3270 2023-06-09 14:58:44.000000 pyNekobin-2.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-09 14:59:36.425034 pyNekobin-2.7/nekobin/
+-rw-rw-rw-   0        0        0       52 2023-06-09 14:59:15.000000 pyNekobin-2.7/nekobin/__init__.py
+-rw-rw-rw-   0        0        0     4355 2023-06-09 10:21:13.000000 pyNekobin-2.7/nekobin/main.py
+drwxrwxrwx   0        0        0        0 2023-06-09 14:59:36.452883 pyNekobin-2.7/pyNekobin.egg-info/
+-rw-rw-rw-   0        0        0     4154 2023-06-09 14:59:36.000000 pyNekobin-2.7/pyNekobin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      226 2023-06-09 14:59:36.000000 pyNekobin-2.7/pyNekobin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 14:59:36.000000 pyNekobin-2.7/pyNekobin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-09 14:59:36.000000 pyNekobin-2.7/pyNekobin.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-09 14:59:36.000000 pyNekobin-2.7/pyNekobin.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-09 14:59:36.455880 pyNekobin-2.7/setup.cfg
+-rw-rw-rw-   0        0        0     1639 2023-06-09 10:21:50.000000 pyNekobin-2.7/setup.py
```

### Comparing `pyNekobin-2.5/LICENSE` & `pyNekobin-2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyNekobin-2.5/PKG-INFO` & `pyNekobin-2.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pyNekobin
-Version: 2.5
+Version: 2.7
 Summary: Paste codes to Nekobin.com with python
 Home-page: https://github.com/Nusab19/pyNekobin
-Download-URL: https://github.com/Nusab19/pyNekobin/releases/tag/pyNekobin-2.5
+Download-URL: https://github.com/Nusab19/pyNekobin/releases/tag/pyNekobin-2.7
 Author: Nusab Taha
 Author-email: nusabtaha33@gmail.com
 License: MIT
 Keywords: Nekobin,pyNekobin,Paste Code,Paste Bin
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Education
@@ -54,31 +54,33 @@
 ```
 
 To paste text to Nekobin, you can use the `paste()` method:
 
 ```python
 async def main():
     result = await nb.paste("Hello, world!")
+    
     if result.ok:
-        print("Pasted text at:", result.url)
+        print("Pasted text at:", result.url) # -> Pasted text at: https://nekobin.com/abxajsyas
     else:
-        print("Error:",  result.message)
+        print("Error:",  result.message)     # Error: Nekobin did not fulfil the request
 
 asyncio.run(main())
 ```
 
 Similarly, you can use the `read()` method to retrieve text from Nekobin:
 
 ```python
 async def main():
-    result = await nb.read("https://nekobin.com/abcdefg")
+    result = await nb.read("https://nekobin.com/abxajsyas")
+    
     if result.ok:
-        print("Retrieved text:", result.content)
+        print("Retrieved text:", result.content) # -> Retrieved text: Hello, world!
     else:
-        print("Error:", result.message)
+        print("Error:", result.message)          # -> Error: Document not found 
 
 asyncio.run(main())
 ```
 
 ## Advanced Usage
 
 As this package uses `httpx` under the hood, you can pass additional keyword arguments in each method call. You can pass any keyword argument that `httpx.AsyncClient` may take:
```

### Comparing `pyNekobin-2.5/README.md` & `pyNekobin-2.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -31,31 +31,33 @@
 ```
 
 To paste text to Nekobin, you can use the `paste()` method:
 
 ```python
 async def main():
     result = await nb.paste("Hello, world!")
+    
     if result.ok:
-        print("Pasted text at:", result.url)
+        print("Pasted text at:", result.url) # -> Pasted text at: https://nekobin.com/abxajsyas
     else:
-        print("Error:",  result.message)
+        print("Error:",  result.message)     # Error: Nekobin did not fulfil the request
 
 asyncio.run(main())
 ```
 
 Similarly, you can use the `read()` method to retrieve text from Nekobin:
 
 ```python
 async def main():
-    result = await nb.read("https://nekobin.com/abcdefg")
+    result = await nb.read("https://nekobin.com/abxajsyas")
+    
     if result.ok:
-        print("Retrieved text:", result.content)
+        print("Retrieved text:", result.content) # -> Retrieved text: Hello, world!
     else:
-        print("Error:", result.message)
+        print("Error:", result.message)          # -> Error: Document not found 
 
 asyncio.run(main())
 ```
 
 ## Advanced Usage
 
 As this package uses `httpx` under the hood, you can pass additional keyword arguments in each method call. You can pass any keyword argument that `httpx.AsyncClient` may take:
```

### Comparing `pyNekobin-2.5/nekobin/main.py` & `pyNekobin-2.7/nekobin/main.py`

 * *Files identical despite different names*

### Comparing `pyNekobin-2.5/pyNekobin.egg-info/PKG-INFO` & `pyNekobin-2.7/pyNekobin.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pyNekobin
-Version: 2.5
+Version: 2.7
 Summary: Paste codes to Nekobin.com with python
 Home-page: https://github.com/Nusab19/pyNekobin
-Download-URL: https://github.com/Nusab19/pyNekobin/releases/tag/pyNekobin-2.5
+Download-URL: https://github.com/Nusab19/pyNekobin/releases/tag/pyNekobin-2.7
 Author: Nusab Taha
 Author-email: nusabtaha33@gmail.com
 License: MIT
 Keywords: Nekobin,pyNekobin,Paste Code,Paste Bin
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Education
@@ -54,31 +54,33 @@
 ```
 
 To paste text to Nekobin, you can use the `paste()` method:
 
 ```python
 async def main():
     result = await nb.paste("Hello, world!")
+    
     if result.ok:
-        print("Pasted text at:", result.url)
+        print("Pasted text at:", result.url) # -> Pasted text at: https://nekobin.com/abxajsyas
     else:
-        print("Error:",  result.message)
+        print("Error:",  result.message)     # Error: Nekobin did not fulfil the request
 
 asyncio.run(main())
 ```
 
 Similarly, you can use the `read()` method to retrieve text from Nekobin:
 
 ```python
 async def main():
-    result = await nb.read("https://nekobin.com/abcdefg")
+    result = await nb.read("https://nekobin.com/abxajsyas")
+    
     if result.ok:
-        print("Retrieved text:", result.content)
+        print("Retrieved text:", result.content) # -> Retrieved text: Hello, world!
     else:
-        print("Error:", result.message)
+        print("Error:", result.message)          # -> Error: Document not found 
 
 asyncio.run(main())
 ```
 
 ## Advanced Usage
 
 As this package uses `httpx` under the hood, you can pass additional keyword arguments in each method call. You can pass any keyword argument that `httpx.AsyncClient` may take:
```

### Comparing `pyNekobin-2.5/setup.py` & `pyNekobin-2.7/setup.py`

 * *Files identical despite different names*

