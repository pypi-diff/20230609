# Comparing `tmp/lofigui-0.2.2.tar.gz` & `tmp/lofigui-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lofigui-0.2.2.tar", max compression
+gzip compressed data, was "lofigui-0.2.3.tar", max compression
```

## Comparing `lofigui-0.2.2.tar` & `lofigui-0.2.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1981 2023-06-09 11:54:12.200982 lofigui-0.2.2/README.md
--rw-r--r--   0        0        0      118 2023-06-09 11:55:58.042620 lofigui-0.2.2/lofigui/__init__.py
--rw-r--r--   0        0        0      755 2023-06-09 11:55:58.053453 lofigui-0.2.2/lofigui/context.py
--rw-r--r--   0        0        0     1233 2023-06-09 11:55:58.064287 lofigui-0.2.2/lofigui/markdown.py
--rw-r--r--   0        0        0      702 2023-06-09 11:55:58.042620 lofigui-0.2.2/lofigui/options.py
--rw-r--r--   0        0        0      280 2023-06-09 11:55:58.053453 lofigui-0.2.2/lofigui/print.py
--rw-r--r--   0        0        0      396 2023-06-09 11:56:07.630117 lofigui-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     2631 1970-01-01 00:00:00.000000 lofigui-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1981 2023-06-09 11:54:12.200982 lofigui-0.2.3/README.md
+-rw-r--r--   0        0        0      118 2023-06-09 11:55:58.042620 lofigui-0.2.3/lofigui/__init__.py
+-rw-r--r--   0        0        0      755 2023-06-09 11:55:58.053453 lofigui-0.2.3/lofigui/context.py
+-rw-r--r--   0        0        0     1233 2023-06-09 11:55:58.064287 lofigui-0.2.3/lofigui/markdown.py
+-rw-r--r--   0        0        0      702 2023-06-09 11:55:58.042620 lofigui-0.2.3/lofigui/options.py
+-rw-r--r--   0        0        0      280 2023-06-09 11:55:58.053453 lofigui-0.2.3/lofigui/print.py
+-rw-r--r--   0        0        0      396 2023-06-09 13:15:19.755573 lofigui-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     2631 1970-01-01 00:00:00.000000 lofigui-0.2.3/PKG-INFO
```

### Comparing `lofigui-0.2.2/README.md` & `lofigui-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `lofigui-0.2.2/lofigui/context.py` & `lofigui-0.2.3/lofigui/context.py`

 * *Files identical despite different names*

### Comparing `lofigui-0.2.2/lofigui/markdown.py` & `lofigui-0.2.3/lofigui/markdown.py`

 * *Files identical despite different names*

### Comparing `lofigui-0.2.2/lofigui/options.py` & `lofigui-0.2.3/lofigui/options.py`

 * *Files identical despite different names*

### Comparing `lofigui-0.2.2/PKG-INFO` & `lofigui-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lofigui
-Version: 0.2.2
+Version: 0.2.3
 Summary: Lofi GUI tooling
 License: MIT
 Author: Humphrey Drummond
 Author-email: hum3@drummond.info
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

