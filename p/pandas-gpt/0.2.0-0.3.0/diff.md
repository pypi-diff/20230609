# Comparing `tmp/pandas-gpt-0.2.0.tar.gz` & `tmp/pandas-gpt-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandas-gpt-0.2.0.tar", last modified: Thu Jun  8 21:12:35 2023, max compression
+gzip compressed data, was "pandas-gpt-0.3.0.tar", last modified: Thu Jun  8 22:40:01 2023, max compression
```

## Comparing `pandas-gpt-0.2.0.tar` & `pandas-gpt-0.3.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 21:12:35.036770 pandas-gpt-0.2.0/
--rw-r--r--   0 root         (0) root         (0)     1073 2023-06-08 21:12:20.000000 pandas-gpt-0.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1871 2023-06-08 21:12:35.036770 pandas-gpt-0.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1671 2023-06-08 21:12:20.000000 pandas-gpt-0.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 21:12:35.035770 pandas-gpt-0.2.0/pandas_gpt/
--rw-r--r--   0 root         (0) root         (0)     3426 2023-06-08 21:12:20.000000 pandas-gpt-0.2.0/pandas_gpt/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 21:12:35.036770 pandas-gpt-0.2.0/pandas_gpt.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1871 2023-06-08 21:12:35.000000 pandas-gpt-0.2.0/pandas_gpt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      224 2023-06-08 21:12:35.000000 pandas-gpt-0.2.0/pandas_gpt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 21:12:35.000000 pandas-gpt-0.2.0/pandas_gpt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-06-08 21:12:35.000000 pandas-gpt-0.2.0/pandas_gpt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-06-08 21:12:35.000000 pandas-gpt-0.2.0/pandas_gpt.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      273 2023-06-08 21:12:20.000000 pandas-gpt-0.2.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-08 21:12:35.037770 pandas-gpt-0.2.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 22:40:01.521957 pandas-gpt-0.3.0/
+-rw-r--r--   0 root         (0) root         (0)     1073 2023-06-08 22:39:48.000000 pandas-gpt-0.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2159 2023-06-08 22:40:01.521957 pandas-gpt-0.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1959 2023-06-08 22:39:48.000000 pandas-gpt-0.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 22:40:01.520957 pandas-gpt-0.3.0/pandas_gpt/
+-rw-r--r--   0 root         (0) root         (0)     3438 2023-06-08 22:39:48.000000 pandas-gpt-0.3.0/pandas_gpt/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 22:40:01.521957 pandas-gpt-0.3.0/pandas_gpt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2159 2023-06-08 22:40:01.000000 pandas-gpt-0.3.0/pandas_gpt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      224 2023-06-08 22:40:01.000000 pandas-gpt-0.3.0/pandas_gpt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 22:40:01.000000 pandas-gpt-0.3.0/pandas_gpt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-06-08 22:40:01.000000 pandas-gpt-0.3.0/pandas_gpt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-06-08 22:40:01.000000 pandas-gpt-0.3.0/pandas_gpt.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      273 2023-06-08 22:39:48.000000 pandas-gpt-0.3.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-08 22:40:01.521957 pandas-gpt-0.3.0/setup.cfg
```

### Comparing `pandas-gpt-0.2.0/LICENSE` & `pandas-gpt-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pandas-gpt-0.2.0/PKG-INFO` & `pandas-gpt-0.3.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,15 @@
-Metadata-Version: 2.1
-Name: pandas-gpt
-Version: 0.2.0
-Summary: Power up your data science workflow with ChatGPT
-Author: Ryan Vandersmith
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # `pandas-gpt` [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/rvanasa/pandas-gpt/blob/main/notebooks/pandas_gpt_demo.ipynb)
 
 > ### Power up your data science workflow with ChatGPT.
 
 ---
 
+`pandas-gpt` is a Python library for doing almost anything with a [pandas](https://pandas.pydata.org/) DataFrame based on natural language queries. 
+
 ## Installation
 
 ```bash
 pip install pandas-gpt
 ```
 
 Set the `OPENAI_API_KEY` environment variable to your [OpenAI API key](https://platform.openai.com/account/api-keys), or use the following code snippet:
@@ -32,21 +26,27 @@
 ```python
 import pandas as pd
 import pandas_gpt
 
 df = pd.DataFrame(...)
 
 # Run Python code generated by ChatGPT
-df.ask('do something with the dataset')
+df.ask('plot x and y with nice colors')
+
+# Return a value
+model = df.ask('LightGBM model trained on the dataset')
+
+# Specify a column or index
+df['my_column'].ask('geometric mean')
 
 # Show additional output
-df.ask('do something with the dataset', verbose=True)
+df.ask('clean the dataset', verbose=True)
 
-# Print source code instead of running
-df.ask.code('do something with the dataset')
+# Print source code without running
+df.ask.code('do something interesting with the dataset')
 ```
 
 ## Alternatives
 
 - [GitHub Copilot](https://github.com/features/copilot): General-purpose code completion (paid subscription)
 - [Sketch](https://github.com/approximatelabs/sketch): AI-powered data summarization and code suggestions (works without an API key)
```

### Comparing `pandas-gpt-0.2.0/pandas_gpt/__init__.py` & `pandas-gpt-0.3.0/pandas_gpt/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pandas as pd
 
 verbose = False # Override default setting with `pandas_gpt.verbose = True`
-fast = False # Override default setting with `pandas_gpt.fast = True`
+mutable = False # Override default setting with `pandas_gpt.mutable = True`
 
 _ask_cache = {}
 
 class Ask:
   def __init__(self, *, verbose=None):
     self.verbose = verbose if verbose is not None else globals()['verbose']
 
@@ -99,15 +99,15 @@
     def _validate(obj):
         pass
 
     def _ask(self, **kw):
       return Ask(**kw)
 
     def _data(self, **kw):
-      if not fast and not kw.get('fast') and hasattr(self._obj, 'copy'):
+      if not mutable and not kw.get('mutable') and hasattr(self._obj, 'copy'):
         return self._obj.copy() # TODO: possibly `deep=False`
       return self._obj
 
     def __call__(self, goal, *args, **kw):
         ask = self._ask(**kw)
         data = self._data(**kw)
         return ask(goal, data, *args)
```

### Comparing `pandas-gpt-0.2.0/pandas_gpt.egg-info/PKG-INFO` & `pandas-gpt-0.3.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: pandas-gpt
-Version: 0.2.0
+Version: 0.3.0
 Summary: Power up your data science workflow with ChatGPT
 Author: Ryan Vandersmith
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # `pandas-gpt` [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/rvanasa/pandas-gpt/blob/main/notebooks/pandas_gpt_demo.ipynb)
 
 > ### Power up your data science workflow with ChatGPT.
 
 ---
 
+`pandas-gpt` is a Python library for doing almost anything with a [pandas](https://pandas.pydata.org/) DataFrame based on natural language queries. 
+
 ## Installation
 
 ```bash
 pip install pandas-gpt
 ```
 
 Set the `OPENAI_API_KEY` environment variable to your [OpenAI API key](https://platform.openai.com/account/api-keys), or use the following code snippet:
@@ -32,21 +34,27 @@
 ```python
 import pandas as pd
 import pandas_gpt
 
 df = pd.DataFrame(...)
 
 # Run Python code generated by ChatGPT
-df.ask('do something with the dataset')
+df.ask('plot x and y with nice colors')
+
+# Return a value
+model = df.ask('LightGBM model trained on the dataset')
+
+# Specify a column or index
+df['my_column'].ask('geometric mean')
 
 # Show additional output
-df.ask('do something with the dataset', verbose=True)
+df.ask('clean the dataset', verbose=True)
 
-# Print source code instead of running
-df.ask.code('do something with the dataset')
+# Print source code without running
+df.ask.code('do something interesting with the dataset')
 ```
 
 ## Alternatives
 
 - [GitHub Copilot](https://github.com/features/copilot): General-purpose code completion (paid subscription)
 - [Sketch](https://github.com/approximatelabs/sketch): AI-powered data summarization and code suggestions (works without an API key)
```

