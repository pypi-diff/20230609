# Comparing `tmp/pandas-gpt-0.3.1.tar.gz` & `tmp/pandas-gpt-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandas-gpt-0.3.1.tar", last modified: Thu Jun  8 22:48:27 2023, max compression
+gzip compressed data, was "pandas-gpt-0.4.0.tar", last modified: Fri Jun  9 04:19:08 2023, max compression
```

## Comparing `pandas-gpt-0.3.1.tar` & `pandas-gpt-0.4.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 22:48:27.253147 pandas-gpt-0.3.1/
--rw-r--r--   0 root         (0) root         (0)     1073 2023-06-08 22:48:08.000000 pandas-gpt-0.3.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2159 2023-06-08 22:48:27.253147 pandas-gpt-0.3.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1959 2023-06-08 22:48:08.000000 pandas-gpt-0.3.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 22:48:27.251147 pandas-gpt-0.3.1/pandas_gpt/
--rw-r--r--   0 root         (0) root         (0)     3528 2023-06-08 22:48:08.000000 pandas-gpt-0.3.1/pandas_gpt/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 22:48:27.253147 pandas-gpt-0.3.1/pandas_gpt.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2159 2023-06-08 22:48:27.000000 pandas-gpt-0.3.1/pandas_gpt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      224 2023-06-08 22:48:27.000000 pandas-gpt-0.3.1/pandas_gpt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 22:48:27.000000 pandas-gpt-0.3.1/pandas_gpt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-06-08 22:48:27.000000 pandas-gpt-0.3.1/pandas_gpt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-06-08 22:48:27.000000 pandas-gpt-0.3.1/pandas_gpt.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      273 2023-06-08 22:48:08.000000 pandas-gpt-0.3.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-08 22:48:27.253147 pandas-gpt-0.3.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 04:19:08.673247 pandas-gpt-0.4.0/
+-rw-r--r--   0 root         (0) root         (0)     1073 2023-06-09 04:18:47.000000 pandas-gpt-0.4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2159 2023-06-09 04:19:08.673247 pandas-gpt-0.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1959 2023-06-09 04:18:47.000000 pandas-gpt-0.4.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 04:19:08.671247 pandas-gpt-0.4.0/pandas_gpt/
+-rw-r--r--   0 root         (0) root         (0)     3740 2023-06-09 04:18:47.000000 pandas-gpt-0.4.0/pandas_gpt/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 04:19:08.672248 pandas-gpt-0.4.0/pandas_gpt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2159 2023-06-09 04:19:08.000000 pandas-gpt-0.4.0/pandas_gpt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      224 2023-06-09 04:19:08.000000 pandas-gpt-0.4.0/pandas_gpt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 04:19:08.000000 pandas-gpt-0.4.0/pandas_gpt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-06-09 04:19:08.000000 pandas-gpt-0.4.0/pandas_gpt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-06-09 04:19:08.000000 pandas-gpt-0.4.0/pandas_gpt.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      273 2023-06-09 04:18:47.000000 pandas-gpt-0.4.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-09 04:19:08.673247 pandas-gpt-0.4.0/setup.cfg
```

### Comparing `pandas-gpt-0.3.1/LICENSE` & `pandas-gpt-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pandas-gpt-0.3.1/PKG-INFO` & `pandas-gpt-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandas-gpt
-Version: 0.3.1
+Version: 0.4.0
 Summary: Power up your data science workflow with ChatGPT
 Author: Ryan Vandersmith
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # `pandas-gpt` [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/rvanasa/pandas-gpt/blob/main/notebooks/pandas_gpt_demo.ipynb)
```

### Comparing `pandas-gpt-0.3.1/README.md` & `pandas-gpt-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pandas-gpt-0.3.1/pandas_gpt/__init__.py` & `pandas-gpt-0.4.0/pandas_gpt/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -79,14 +79,17 @@
       print()
       print(result)
     return self._extract_code_block(result)
 
   def code(self, *args):
     print(self._code(*args))
 
+  def prompt(self, *args):
+    print(self._get_prompt(*args))
+
   def __call__(self, goal, *args):
     source = self._code(goal, *args)
     return self._eval(source, *args)
 
 
 @pd.api.extensions.register_dataframe_accessor('ask')
 @pd.api.extensions.register_series_accessor('ask')
@@ -113,7 +116,12 @@
         data = self._data(**kw)
         return ask(goal, data, *args)
 
     def code(self, goal, *args, **kw):
         ask = self._ask(**kw)
         data = self._data(**kw)
         return ask.code(goal, data, *args)
+
+    def prompt(self, goal, *args, **kw):
+        ask = self._ask(**kw)
+        data = self._data(**kw)
+        return ask.prompt(goal, data, *args)
```

### Comparing `pandas-gpt-0.3.1/pandas_gpt.egg-info/PKG-INFO` & `pandas-gpt-0.4.0/pandas_gpt.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandas-gpt
-Version: 0.3.1
+Version: 0.4.0
 Summary: Power up your data science workflow with ChatGPT
 Author: Ryan Vandersmith
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # `pandas-gpt` [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/rvanasa/pandas-gpt/blob/main/notebooks/pandas_gpt_demo.ipynb)
```

