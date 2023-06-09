# Comparing `tmp/flexigurator-0.3.1.tar.gz` & `tmp/flexigurator-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flexigurator-0.3.1.tar", max compression
+gzip compressed data, was "flexigurator-0.3.2.tar", max compression
```

## Comparing `flexigurator-0.3.1.tar` & `flexigurator-0.3.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     2373 2023-06-02 13:39:37.460070 flexigurator-0.3.1/README.md
--rw-r--r--   0        0        0      166 2023-06-02 13:39:37.460070 flexigurator-0.3.1/flexigurator/__init__.py
--rw-r--r--   0        0        0     1421 2023-06-02 13:39:37.460070 flexigurator-0.3.1/flexigurator/config_patch.py
--rw-r--r--   0        0        0        0 2023-06-02 13:39:37.460070 flexigurator-0.3.1/flexigurator/form/__init__.py
--rw-r--r--   0        0        0     4777 2023-06-02 13:39:37.460070 flexigurator-0.3.1/flexigurator/form/form.py
--rw-r--r--   0        0        0     5790 2023-06-02 13:39:37.460070 flexigurator-0.3.1/flexigurator/form/jinja_templates/config_form.html
--rw-r--r--   0        0        0     3550 2023-06-02 13:39:37.460070 flexigurator-0.3.1/flexigurator/form/jinja_templates/index.html
--rw-r--r--   0        0        0     2481 2023-06-02 13:39:37.460070 flexigurator-0.3.1/flexigurator/placeholder.py
--rw-r--r--   0        0        0     1083 2023-06-02 13:39:37.464070 flexigurator-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     2999 1970-01-01 00:00:00.000000 flexigurator-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     2373 2023-06-09 16:06:41.114365 flexigurator-0.3.2/README.md
+-rw-r--r--   0        0        0      166 2023-06-09 16:06:41.114365 flexigurator-0.3.2/flexigurator/__init__.py
+-rw-r--r--   0        0        0     1523 2023-06-09 16:06:41.114365 flexigurator-0.3.2/flexigurator/config_patch.py
+-rw-r--r--   0        0        0        0 2023-06-09 16:06:41.114365 flexigurator-0.3.2/flexigurator/form/__init__.py
+-rw-r--r--   0        0        0     4777 2023-06-09 16:06:41.114365 flexigurator-0.3.2/flexigurator/form/form.py
+-rw-r--r--   0        0        0     5790 2023-06-09 16:06:41.114365 flexigurator-0.3.2/flexigurator/form/jinja_templates/config_form.html
+-rw-r--r--   0        0        0     3550 2023-06-09 16:06:41.114365 flexigurator-0.3.2/flexigurator/form/jinja_templates/index.html
+-rw-r--r--   0        0        0     2481 2023-06-09 16:06:41.114365 flexigurator-0.3.2/flexigurator/placeholder.py
+-rw-r--r--   0        0        0     1083 2023-06-09 16:06:41.114365 flexigurator-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     2999 1970-01-01 00:00:00.000000 flexigurator-0.3.2/PKG-INFO
```

### Comparing `flexigurator-0.3.1/README.md` & `flexigurator-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `flexigurator-0.3.1/flexigurator/config_patch.py` & `flexigurator-0.3.2/flexigurator/config_patch.py`

 * *Files 16% similar despite different names*

```diff
@@ -26,18 +26,21 @@
     """
     if isinstance(data, dict):
         data = ConfZDataSource(data)
 
     if not isinstance(data, list):
         data = [data]
 
-    patched_sources = config_class.CONFIG_SOURCES
+    original_sources = config_class.CONFIG_SOURCES
+    patched_sources: list[ConfZSource]
 
-    if patched_sources is None:
+    if original_sources is None:
         patched_sources = []
-    elif not isinstance(patched_sources, list):
-        patched_sources = [patched_sources]
+    elif not isinstance(original_sources, list):
+        patched_sources = [original_sources]
+    else:
+        patched_sources = list(original_sources)
 
     patched_sources += data
 
     with config_class.change_config_sources(patched_sources):
         yield
```

### Comparing `flexigurator-0.3.1/flexigurator/form/form.py` & `flexigurator-0.3.2/flexigurator/form/form.py`

 * *Files identical despite different names*

### Comparing `flexigurator-0.3.1/flexigurator/form/jinja_templates/config_form.html` & `flexigurator-0.3.2/flexigurator/form/jinja_templates/config_form.html`

 * *Files identical despite different names*

### Comparing `flexigurator-0.3.1/flexigurator/form/jinja_templates/index.html` & `flexigurator-0.3.2/flexigurator/form/jinja_templates/index.html`

 * *Files identical despite different names*

### Comparing `flexigurator-0.3.1/flexigurator/placeholder.py` & `flexigurator-0.3.2/flexigurator/placeholder.py`

 * *Files identical despite different names*

### Comparing `flexigurator-0.3.1/pyproject.toml` & `flexigurator-0.3.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flexigurator"
-version = "0.3.1"
+version = "0.3.2"
 description = "Python Configuration solution."
 authors = ["Thomas Bos <thymer.bos217@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 pydantic = "^1.10.8"
```

### Comparing `flexigurator-0.3.1/PKG-INFO` & `flexigurator-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flexigurator
-Version: 0.3.1
+Version: 0.3.2
 Summary: Python Configuration solution.
 Author: Thomas Bos
 Author-email: thymer.bos217@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: confz (>=1.8.1,<2.0.0)
```

