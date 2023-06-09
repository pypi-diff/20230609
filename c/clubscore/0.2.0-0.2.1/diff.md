# Comparing `tmp/clubscore-0.2.0.tar.gz` & `tmp/clubscore-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clubscore-0.2.0.tar", last modified: Wed May 31 14:51:47 2023, max compression
+gzip compressed data, was "clubscore-0.2.1.tar", last modified: Fri Jun  9 15:53:19 2023, max compression
```

## Comparing `clubscore-0.2.0.tar` & `clubscore-0.2.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-05-31 14:51:47.385681 clubscore-0.2.0/
--rw-r--r--   0 dave       (501) staff       (20)     1071 2023-05-05 17:29:41.000000 clubscore-0.2.0/LICENSE
--rw-r--r--   0 dave       (501) staff       (20)      909 2023-05-31 14:51:47.384397 clubscore-0.2.0/PKG-INFO
--rw-r--r--   0 dave       (501) staff       (20)       23 2023-05-06 09:41:10.000000 clubscore-0.2.0/README.md
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-05-31 14:51:47.367269 clubscore-0.2.0/clubscore/
--rw-r--r--   0 dave       (501) staff       (20)      752 2023-05-09 16:58:15.000000 clubscore-0.2.0/clubscore/API.py
--rw-r--r--   0 dave       (501) staff       (20)        0 2023-05-06 08:36:10.000000 clubscore-0.2.0/clubscore/__init__.py
--rw-r--r--   0 dave       (501) staff       (20)     4453 2023-05-31 14:13:09.000000 clubscore-0.2.0/clubscore/bot.py
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-05-31 14:51:47.380027 clubscore-0.2.0/clubscore/objects/
--rw-r--r--   0 dave       (501) staff       (20)     5233 2023-05-16 22:07:16.000000 clubscore-0.2.0/clubscore/objects/CONTAINER.py
--rw-r--r--   0 dave       (501) staff       (20)     2408 2023-05-16 22:07:16.000000 clubscore-0.2.0/clubscore/objects/IMG.py
--rw-r--r--   0 dave       (501) staff       (20)     1151 2023-02-04 00:33:04.000000 clubscore-0.2.0/clubscore/objects/RECTANGLE.py
--rw-r--r--   0 dave       (501) staff       (20)     3966 2023-05-16 22:26:38.000000 clubscore-0.2.0/clubscore/objects/TEXT.py
--rw-r--r--   0 dave       (501) staff       (20)        0 2023-05-06 08:36:10.000000 clubscore-0.2.0/clubscore/objects/__init__.py
--rw-r--r--   0 dave       (501) staff       (20)     4203 2023-05-27 10:59:14.000000 clubscore-0.2.0/clubscore/utils.py
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-05-31 14:51:47.371676 clubscore-0.2.0/clubscore.egg-info/
--rw-r--r--   0 dave       (501) staff       (20)      909 2023-05-31 14:51:47.000000 clubscore-0.2.0/clubscore.egg-info/PKG-INFO
--rw-r--r--   0 dave       (501) staff       (20)      452 2023-05-31 14:51:47.000000 clubscore-0.2.0/clubscore.egg-info/SOURCES.txt
--rw-r--r--   0 dave       (501) staff       (20)        1 2023-05-31 14:51:47.000000 clubscore-0.2.0/clubscore.egg-info/dependency_links.txt
--rw-r--r--   0 dave       (501) staff       (20)       85 2023-05-31 14:51:47.000000 clubscore-0.2.0/clubscore.egg-info/requires.txt
--rw-r--r--   0 dave       (501) staff       (20)       10 2023-05-31 14:51:47.000000 clubscore-0.2.0/clubscore.egg-info/top_level.txt
--rw-r--r--   0 dave       (501) staff       (20)       38 2023-05-31 14:51:47.385883 clubscore-0.2.0/setup.cfg
--rw-r--r--   0 dave       (501) staff       (20)     1220 2023-05-31 14:49:04.000000 clubscore-0.2.0/setup.py
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-05-31 14:51:47.381893 clubscore-0.2.0/tests/
--rw-r--r--   0 dave       (501) staff       (20)     1961 2023-05-11 23:19:07.000000 clubscore-0.2.0/tests/test_templates.py
--rw-r--r--   0 dave       (501) staff       (20)      881 2023-05-11 23:17:53.000000 clubscore-0.2.0/tests/test_utils.py
+drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-06-09 15:53:19.101120 clubscore-0.2.1/
+-rw-r--r--   0 dave       (501) staff       (20)     1071 2023-05-05 17:29:41.000000 clubscore-0.2.1/LICENSE
+-rw-r--r--   0 dave       (501) staff       (20)      909 2023-06-09 15:53:19.100841 clubscore-0.2.1/PKG-INFO
+-rw-r--r--   0 dave       (501) staff       (20)       23 2023-05-06 09:41:10.000000 clubscore-0.2.1/README.md
+drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-06-09 15:53:19.092351 clubscore-0.2.1/clubscore/
+-rw-r--r--   0 dave       (501) staff       (20)      752 2023-05-09 16:58:15.000000 clubscore-0.2.1/clubscore/API.py
+-rw-r--r--   0 dave       (501) staff       (20)        0 2023-05-06 08:36:10.000000 clubscore-0.2.1/clubscore/__init__.py
+-rw-r--r--   0 dave       (501) staff       (20)     4441 2023-06-03 20:22:54.000000 clubscore-0.2.1/clubscore/bot.py
+drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-06-09 15:53:19.098355 clubscore-0.2.1/clubscore/objects/
+-rw-r--r--   0 dave       (501) staff       (20)     5233 2023-05-16 22:07:16.000000 clubscore-0.2.1/clubscore/objects/CONTAINER.py
+-rw-r--r--   0 dave       (501) staff       (20)     2408 2023-05-16 22:07:16.000000 clubscore-0.2.1/clubscore/objects/IMG.py
+-rw-r--r--   0 dave       (501) staff       (20)     1151 2023-02-04 00:33:04.000000 clubscore-0.2.1/clubscore/objects/RECTANGLE.py
+-rw-r--r--   0 dave       (501) staff       (20)     3966 2023-05-16 22:26:38.000000 clubscore-0.2.1/clubscore/objects/TEXT.py
+-rw-r--r--   0 dave       (501) staff       (20)        0 2023-05-06 08:36:10.000000 clubscore-0.2.1/clubscore/objects/__init__.py
+-rw-r--r--   0 dave       (501) staff       (20)     4237 2023-06-09 15:50:58.000000 clubscore-0.2.1/clubscore/utils.py
+drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-06-09 15:53:19.094943 clubscore-0.2.1/clubscore.egg-info/
+-rw-r--r--   0 dave       (501) staff       (20)      909 2023-06-09 15:53:19.000000 clubscore-0.2.1/clubscore.egg-info/PKG-INFO
+-rw-r--r--   0 dave       (501) staff       (20)      452 2023-06-09 15:53:19.000000 clubscore-0.2.1/clubscore.egg-info/SOURCES.txt
+-rw-r--r--   0 dave       (501) staff       (20)        1 2023-06-09 15:53:19.000000 clubscore-0.2.1/clubscore.egg-info/dependency_links.txt
+-rw-r--r--   0 dave       (501) staff       (20)       85 2023-06-09 15:53:19.000000 clubscore-0.2.1/clubscore.egg-info/requires.txt
+-rw-r--r--   0 dave       (501) staff       (20)       10 2023-06-09 15:53:19.000000 clubscore-0.2.1/clubscore.egg-info/top_level.txt
+-rw-r--r--   0 dave       (501) staff       (20)       38 2023-06-09 15:53:19.101220 clubscore-0.2.1/setup.cfg
+-rw-r--r--   0 dave       (501) staff       (20)     1220 2023-06-09 15:51:26.000000 clubscore-0.2.1/setup.py
+drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-06-09 15:53:19.099784 clubscore-0.2.1/tests/
+-rw-r--r--   0 dave       (501) staff       (20)     1961 2023-05-11 23:19:07.000000 clubscore-0.2.1/tests/test_templates.py
+-rw-r--r--   0 dave       (501) staff       (20)      881 2023-05-11 23:17:53.000000 clubscore-0.2.1/tests/test_utils.py
```

### Comparing `clubscore-0.2.0/LICENSE` & `clubscore-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `clubscore-0.2.0/PKG-INFO` & `clubscore-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clubscore
-Version: 0.2.0
+Version: 0.2.1
 Summary: A package for creating customizable templates in XML
 Home-page: https://github.com/davegimo/clubscore
 Author: Davide Gimondo
 Author-email: davegimo@gmail.com
 License: MIT
 Keywords: my-package,example,demo
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `clubscore-0.2.0/clubscore/API.py` & `clubscore-0.2.1/clubscore/API.py`

 * *Files identical despite different names*

### Comparing `clubscore-0.2.0/clubscore/bot.py` & `clubscore-0.2.1/clubscore/bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     d = {}
     d["bot"] = bot
     d["user_id"] = message.from_user.id
     d["name"] = message.from_user.first_name
     d["lastname"] = message.from_user.last_name
     d["username"] = message.from_user.username
     d["command"] = command
-    d["timestamp"] = datetime.datetime.now().isoformat()
+    d["timestamp"] = datetime.datetime.now()
 
 
     url = "https://clubscorestats.herokuapp.com/actions"
     payload = json.dumps(d)
     headers = {
         'Content-Type': 'application/json'
     }
```

### Comparing `clubscore-0.2.0/clubscore/objects/CONTAINER.py` & `clubscore-0.2.1/clubscore/objects/CONTAINER.py`

 * *Files identical despite different names*

### Comparing `clubscore-0.2.0/clubscore/objects/IMG.py` & `clubscore-0.2.1/clubscore/objects/IMG.py`

 * *Files identical despite different names*

### Comparing `clubscore-0.2.0/clubscore/objects/RECTANGLE.py` & `clubscore-0.2.1/clubscore/objects/RECTANGLE.py`

 * *Files identical despite different names*

### Comparing `clubscore-0.2.0/clubscore/objects/TEXT.py` & `clubscore-0.2.1/clubscore/objects/TEXT.py`

 * *Files identical despite different names*

### Comparing `clubscore-0.2.0/clubscore/utils.py` & `clubscore-0.2.1/clubscore/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,16 +81,16 @@
 
 """
 data una parola, viene restituita quella più vicina tra le disponibili in elenco
 """
 
 
 def matchWord(s, arr):
-    arr_lower = [x.lower() for x in arr]
-    s_lower = s.lower()
+    arr_lower = [x.lower().replace(" ", "") for x in arr]
+    s_lower = s.lower().replace(" ", "")
 
     match = difflib.get_close_matches(s_lower, arr_lower, n=1, cutoff=0.3)
     if match:
         # Find the index of the lowercase match
         index = arr_lower.index(match[0])
         # Return the original string in its original case
         return arr[index]
```

### Comparing `clubscore-0.2.0/clubscore.egg-info/PKG-INFO` & `clubscore-0.2.1/clubscore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clubscore
-Version: 0.2.0
+Version: 0.2.1
 Summary: A package for creating customizable templates in XML
 Home-page: https://github.com/davegimo/clubscore
 Author: Davide Gimondo
 Author-email: davegimo@gmail.com
 License: MIT
 Keywords: my-package,example,demo
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `clubscore-0.2.0/setup.py` & `clubscore-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='clubscore',
-    version='0.2.0',
+    version='0.2.1',
     author='Davide Gimondo',
     author_email='davegimo@gmail.com',
     description='A package for creating customizable templates in XML',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/davegimo/clubscore',
     packages=find_packages(),
```

### Comparing `clubscore-0.2.0/tests/test_templates.py` & `clubscore-0.2.1/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `clubscore-0.2.0/tests/test_utils.py` & `clubscore-0.2.1/tests/test_utils.py`

 * *Files identical despite different names*

