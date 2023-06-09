# Comparing `tmp/ironbot-0.0.5.tar.gz` & `tmp/ironbot-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ironbot-0.0.5.tar", max compression
+gzip compressed data, was "ironbot-0.0.6.tar", max compression
```

## Comparing `ironbot-0.0.5.tar` & `ironbot-0.0.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35149 2023-06-01 22:19:22.270689 ironbot-0.0.5/LICENSE
--rw-r--r--   0        0        0     1939 2023-06-05 22:40:55.330531 ironbot-0.0.5/README.md
--rw-r--r--   0        0        0        0 2023-06-03 00:02:15.086424 ironbot-0.0.5/ironbot/__init__.py
--rw-r--r--   0        0        0     1057 2023-06-03 00:04:34.846656 ironbot-0.0.5/ironbot/__main__.py
--rw-r--r--   0        0        0     2654 2023-06-09 04:39:25.712529 ironbot-0.0.5/ironbot/models.py
--rw-r--r--   0        0        0     1069 2023-06-09 05:41:45.789123 ironbot-0.0.5/ironbot/parsers.py
--rw-r--r--   0        0        0     2070 2023-06-09 05:43:22.012933 ironbot-0.0.5/ironbot/scrappers.py
--rw-r--r--   0        0        0     1616 2023-06-09 05:46:40.642018 ironbot-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     3292 1970-01-01 00:00:00.000000 ironbot-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-01 22:19:22.270689 ironbot-0.0.6/LICENSE
+-rw-r--r--   0        0        0     1939 2023-06-05 22:40:55.330531 ironbot-0.0.6/README.md
+-rw-r--r--   0        0        0        0 2023-06-03 00:02:15.086424 ironbot-0.0.6/ironbot/__init__.py
+-rw-r--r--   0        0        0     1057 2023-06-03 00:04:34.846656 ironbot-0.0.6/ironbot/__main__.py
+-rw-r--r--   0        0        0     2654 2023-06-09 04:39:25.712529 ironbot-0.0.6/ironbot/models.py
+-rw-r--r--   0        0        0     1069 2023-06-09 05:41:45.000000 ironbot-0.0.6/ironbot/parsers.py
+-rw-r--r--   0        0        0     2070 2023-06-09 05:50:32.158425 ironbot-0.0.6/ironbot/scrappers.py
+-rw-r--r--   0        0        0     1616 2023-06-09 05:51:58.332208 ironbot-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     3292 1970-01-01 00:00:00.000000 ironbot-0.0.6/PKG-INFO
```

### Comparing `ironbot-0.0.5/LICENSE` & `ironbot-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ironbot-0.0.5/README.md` & `ironbot-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `ironbot-0.0.5/ironbot/__main__.py` & `ironbot-0.0.6/ironbot/__main__.py`

 * *Files identical despite different names*

### Comparing `ironbot-0.0.5/ironbot/models.py` & `ironbot-0.0.6/ironbot/models.py`

 * *Files identical despite different names*

### Comparing `ironbot-0.0.5/ironbot/parsers.py` & `ironbot-0.0.6/ironbot/parsers.py`

 * *Files identical despite different names*

### Comparing `ironbot-0.0.5/ironbot/scrappers.py` & `ironbot-0.0.6/ironbot/scrappers.py`

 * *Files identical despite different names*

### Comparing `ironbot-0.0.5/pyproject.toml` & `ironbot-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ironbot"
-version = "0.0.5"
+version = "0.0.6"
 description = "CLI to get information about Ironman professional races"
 authors = ["Eduardo Cuducos <4732915+cuducos@users.noreply.github.com>"]
 license = "GPLv3"
 readme = "README.md"
 repository = "https://github.com/cuducos/ironbot/"
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `ironbot-0.0.5/PKG-INFO` & `ironbot-0.0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ironbot
-Version: 0.0.5
+Version: 0.0.6
 Summary: CLI to get information about Ironman professional races
 Home-page: https://github.com/cuducos/ironbot/
 License: GPLv3
 Keywords: triathlon,Ironamn,Professional triathletes,Professional triathlon races
 Author: Eduardo Cuducos
 Author-email: 4732915+cuducos@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
```

