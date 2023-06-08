# Comparing `tmp/pandas-gpt-0.1.0.tar.gz` & `tmp/pandas-gpt-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandas-gpt-0.1.0.tar", last modified: Thu Jun  1 03:30:04 2023, max compression
+gzip compressed data, was "pandas-gpt-0.2.0.tar", last modified: Thu Jun  8 21:12:35 2023, max compression
```

## Comparing `pandas-gpt-0.1.0.tar` & `pandas-gpt-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 03:30:04.113900 pandas-gpt-0.1.0/
--rw-r--r--   0 root         (0) root         (0)     1073 2023-06-01 02:58:30.000000 pandas-gpt-0.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1902 2023-06-01 03:30:04.112900 pandas-gpt-0.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1702 2023-06-01 02:58:30.000000 pandas-gpt-0.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 03:30:04.111900 pandas-gpt-0.1.0/pandas_gpt/
--rw-r--r--   0 root         (0) root         (0)     2874 2023-06-01 02:58:30.000000 pandas-gpt-0.1.0/pandas_gpt/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 03:30:04.112900 pandas-gpt-0.1.0/pandas_gpt.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1902 2023-06-01 03:30:04.000000 pandas-gpt-0.1.0/pandas_gpt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      224 2023-06-01 03:30:04.000000 pandas-gpt-0.1.0/pandas_gpt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 03:30:04.000000 pandas-gpt-0.1.0/pandas_gpt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-06-01 03:30:04.000000 pandas-gpt-0.1.0/pandas_gpt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-06-01 03:30:04.000000 pandas-gpt-0.1.0/pandas_gpt.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      273 2023-06-01 03:29:56.000000 pandas-gpt-0.1.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-01 03:30:04.113900 pandas-gpt-0.1.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 21:12:35.036770 pandas-gpt-0.2.0/
+-rw-r--r--   0 root         (0) root         (0)     1073 2023-06-08 21:12:20.000000 pandas-gpt-0.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1871 2023-06-08 21:12:35.036770 pandas-gpt-0.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1671 2023-06-08 21:12:20.000000 pandas-gpt-0.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 21:12:35.035770 pandas-gpt-0.2.0/pandas_gpt/
+-rw-r--r--   0 root         (0) root         (0)     3426 2023-06-08 21:12:20.000000 pandas-gpt-0.2.0/pandas_gpt/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 21:12:35.036770 pandas-gpt-0.2.0/pandas_gpt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1871 2023-06-08 21:12:35.000000 pandas-gpt-0.2.0/pandas_gpt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      224 2023-06-08 21:12:35.000000 pandas-gpt-0.2.0/pandas_gpt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 21:12:35.000000 pandas-gpt-0.2.0/pandas_gpt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-06-08 21:12:35.000000 pandas-gpt-0.2.0/pandas_gpt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-06-08 21:12:35.000000 pandas-gpt-0.2.0/pandas_gpt.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      273 2023-06-08 21:12:20.000000 pandas-gpt-0.2.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-08 21:12:35.037770 pandas-gpt-0.2.0/setup.cfg
```

### Comparing `pandas-gpt-0.1.0/LICENSE` & `pandas-gpt-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pandas-gpt-0.1.0/PKG-INFO` & `pandas-gpt-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: pandas-gpt
-Version: 0.1.0
+Version: 0.2.0
 Summary: Power up your data science workflow with ChatGPT
 Author: Ryan Vandersmith
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # `pandas-gpt` [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/rvanasa/pandas-gpt/blob/main/notebooks/pandas_gpt_demo.ipynb)
 
 > ### Power up your data science workflow with ChatGPT.
 
 ---
 
 ## Installation
 
 ```bash
-pip install git+https://github.com/rvanasa/pandas-gpt
+pip install pandas-gpt
 ```
 
 Set the `OPENAI_API_KEY` environment variable to your [OpenAI API key](https://platform.openai.com/account/api-keys), or use the following code snippet:
 
 ```python
 import openai
 openai.api_key = 'sk-**********'
```

### Comparing `pandas-gpt-0.1.0/README.md` & `pandas-gpt-0.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 > ### Power up your data science workflow with ChatGPT.
 
 ---
 
 ## Installation
 
 ```bash
-pip install git+https://github.com/rvanasa/pandas-gpt
+pip install pandas-gpt
 ```
 
 Set the `OPENAI_API_KEY` environment variable to your [OpenAI API key](https://platform.openai.com/account/api-keys), or use the following code snippet:
 
 ```python
 import openai
 openai.api_key = 'sk-**********'
```

### Comparing `pandas-gpt-0.1.0/pandas_gpt/__init__.py` & `pandas-gpt-0.2.0/pandas_gpt/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 import pandas as pd
 
+verbose = False # Override default setting with `pandas_gpt.verbose = True`
+fast = False # Override default setting with `pandas_gpt.fast = True`
+
 _ask_cache = {}
 
 class Ask:
-  def __init__(self, *, verbose=False):
-    import os
-    self.verbose = verbose
+  def __init__(self, *, verbose=None):
+    self.verbose = verbose if verbose is not None else globals()['verbose']
 
   @staticmethod
   def _fill_template(template, **kw):
     import re
     from textwrap import dedent
     result = dedent(template.lstrip('\n').rstrip())
     for k, v in kw.items():
       result = result.replace(f'{{{k}}}', v)
     m = re.match(r'\{[a-zA-Z0-9_]*\}', result)
     if m:
       raise Exception(f'Expected variable: {m.group(0)}')
     return result
 
   def _get_prompt(self, goal, arg):
-    import io
-    buf = io.StringIO()
-    arg.info(buf=buf)
-    arg_summary = buf.getvalue()
-    arg_name = 'df' if isinstance(arg, pd.DataFrame) else 'data'
+    if isinstance(arg, pd.DataFrame) or isinstance(arg, pd.Series):
+      import io
+      buf = io.StringIO()
+      arg.info(buf=buf)
+      arg_summary = buf.getvalue()
+    else:
+      arg_summary = repr(arg)
+    arg_name = 'df' if isinstance(arg, pd.DataFrame) else 'index' if isinstance(arg, pd.Index) else 'data'
 
     return self._fill_template('''
       Write a Python function `process({arg_name})` which takes the following input value:
 
       {arg_name} = {arg}
 
       This is the function's purpose: {goal}
@@ -79,31 +84,35 @@
 
   def __call__(self, goal, *args):
     source = self._code(goal, *args)
     return self._eval(source, *args)
 
 
 @pd.api.extensions.register_dataframe_accessor('ask')
+@pd.api.extensions.register_series_accessor('ask')
+@pd.api.extensions.register_index_accessor('ask')
 class AskAccessor:
     def __init__(self, pandas_obj):
         self._validate(pandas_obj)
         self._obj = pandas_obj
 
     @staticmethod
     def _validate(obj):
         pass
 
     def _ask(self, **kw):
       return Ask(**kw)
 
-    def _data(self):
-      return self._obj.copy() # TODO: possibly `deep=False`
+    def _data(self, **kw):
+      if not fast and not kw.get('fast') and hasattr(self._obj, 'copy'):
+        return self._obj.copy() # TODO: possibly `deep=False`
+      return self._obj
 
     def __call__(self, goal, *args, **kw):
         ask = self._ask(**kw)
-        data = self._data()
+        data = self._data(**kw)
         return ask(goal, data, *args)
 
     def code(self, goal, *args, **kw):
         ask = self._ask(**kw)
-        data = self._data()
+        data = self._data(**kw)
         return ask.code(goal, data, *args)
```

### Comparing `pandas-gpt-0.1.0/pandas_gpt.egg-info/PKG-INFO` & `pandas-gpt-0.2.0/pandas_gpt.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: pandas-gpt
-Version: 0.1.0
+Version: 0.2.0
 Summary: Power up your data science workflow with ChatGPT
 Author: Ryan Vandersmith
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # `pandas-gpt` [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/rvanasa/pandas-gpt/blob/main/notebooks/pandas_gpt_demo.ipynb)
 
 > ### Power up your data science workflow with ChatGPT.
 
 ---
 
 ## Installation
 
 ```bash
-pip install git+https://github.com/rvanasa/pandas-gpt
+pip install pandas-gpt
 ```
 
 Set the `OPENAI_API_KEY` environment variable to your [OpenAI API key](https://platform.openai.com/account/api-keys), or use the following code snippet:
 
 ```python
 import openai
 openai.api_key = 'sk-**********'
```

