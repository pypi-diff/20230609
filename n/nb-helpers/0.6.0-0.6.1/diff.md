# Comparing `tmp/nb_helpers-0.6.0.tar.gz` & `tmp/nb_helpers-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nb_helpers-0.6.0.tar", last modified: Fri Jun  9 21:35:47 2023, max compression
+gzip compressed data, was "nb_helpers-0.6.1.tar", last modified: Fri Jun  9 21:58:42 2023, max compression
```

## Comparing `nb_helpers-0.6.0.tar` & `nb_helpers-0.6.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 21:35:47.945246 nb_helpers-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-09 21:35:34.000000 nb_helpers-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-06-09 21:35:47.945246 nb_helpers-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8915 2023-06-09 21:35:34.000000 nb_helpers-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 21:35:47.941246 nb_helpers-0.6.0/nb_helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-09 21:35:34.000000 nb_helpers-0.6.0/nb_helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11322 2023-06-09 21:35:34.000000 nb_helpers-0.6.0/nb_helpers/_modidx.py
--rw-r--r--   0 runner    (1001) docker     (123)     6950 2023-06-09 21:35:34.000000 nb_helpers-0.6.0/nb_helpers/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-06-09 21:35:34.000000 nb_helpers-0.6.0/nb_helpers/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-06-09 21:35:34.000000 nb_helpers-0.6.0/nb_helpers/colab.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-06-09 21:35:34.000000 nb_helpers-0.6.0/nb_helpers/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-06-09 21:35:34.000000 nb_helpers-0.6.0/nb_helpers/export.py
--rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-06-09 21:35:34.000000 nb_helpers-0.6.0/nb_helpers/run.py
--rw-r--r--   0 runner    (1001) docker     (123)    12417 2023-06-09 21:35:34.000000 nb_helpers-0.6.0/nb_helpers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-06-09 21:35:34.000000 nb_helpers-0.6.0/nb_helpers/wandb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 21:35:47.945246 nb_helpers-0.6.0/nb_helpers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-06-09 21:35:47.000000 nb_helpers-0.6.0/nb_helpers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-09 21:35:47.000000 nb_helpers-0.6.0/nb_helpers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 21:35:47.000000 nb_helpers-0.6.0/nb_helpers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-09 21:35:47.000000 nb_helpers-0.6.0/nb_helpers.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 21:35:47.000000 nb_helpers-0.6.0/nb_helpers.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-09 21:35:47.000000 nb_helpers-0.6.0/nb_helpers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-09 21:35:47.000000 nb_helpers-0.6.0/nb_helpers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-09 21:35:34.000000 nb_helpers-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 21:35:47.945246 nb_helpers-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-06-09 21:35:34.000000 nb_helpers-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 21:58:42.734192 nb_helpers-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-09 21:58:30.000000 nb_helpers-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-06-09 21:58:42.734192 nb_helpers-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8915 2023-06-09 21:58:30.000000 nb_helpers-0.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 21:58:42.730192 nb_helpers-0.6.1/nb_helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-09 21:58:30.000000 nb_helpers-0.6.1/nb_helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11322 2023-06-09 21:58:30.000000 nb_helpers-0.6.1/nb_helpers/_modidx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6950 2023-06-09 21:58:30.000000 nb_helpers-0.6.1/nb_helpers/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-06-09 21:58:30.000000 nb_helpers-0.6.1/nb_helpers/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-06-09 21:58:30.000000 nb_helpers-0.6.1/nb_helpers/colab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-06-09 21:58:30.000000 nb_helpers-0.6.1/nb_helpers/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-06-09 21:58:30.000000 nb_helpers-0.6.1/nb_helpers/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-06-09 21:58:30.000000 nb_helpers-0.6.1/nb_helpers/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12417 2023-06-09 21:58:30.000000 nb_helpers-0.6.1/nb_helpers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-06-09 21:58:30.000000 nb_helpers-0.6.1/nb_helpers/wandb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 21:58:42.730192 nb_helpers-0.6.1/nb_helpers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-06-09 21:58:42.000000 nb_helpers-0.6.1/nb_helpers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-09 21:58:42.000000 nb_helpers-0.6.1/nb_helpers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 21:58:42.000000 nb_helpers-0.6.1/nb_helpers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-09 21:58:42.000000 nb_helpers-0.6.1/nb_helpers.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 21:58:42.000000 nb_helpers-0.6.1/nb_helpers.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-09 21:58:42.000000 nb_helpers-0.6.1/nb_helpers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-09 21:58:42.000000 nb_helpers-0.6.1/nb_helpers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-09 21:58:30.000000 nb_helpers-0.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 21:58:42.734192 nb_helpers-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-06-09 21:58:30.000000 nb_helpers-0.6.1/setup.py
```

### Comparing `nb_helpers-0.6.0/LICENSE` & `nb_helpers-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nb_helpers-0.6.0/PKG-INFO` & `nb_helpers-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nb_helpers
-Version: 0.6.0
+Version: 0.6.1
 Summary: A set of tools for nb handling
 Home-page: https://github.com/wandb/nb_helpers/tree/main/
 Author: Thomas Capelle
 Author-email: tcapelle@wandb.com
 License: MIT License
 Keywords: jupyter notebook
 Platform: UNKNOWN
```

### Comparing `nb_helpers-0.6.0/README.md` & `nb_helpers-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `nb_helpers-0.6.0/nb_helpers/_modidx.py` & `nb_helpers-0.6.1/nb_helpers/_modidx.py`

 * *Files identical despite different names*

### Comparing `nb_helpers-0.6.0/nb_helpers/actions.py` & `nb_helpers-0.6.1/nb_helpers/actions.py`

 * *Files identical despite different names*

### Comparing `nb_helpers-0.6.0/nb_helpers/clean.py` & `nb_helpers-0.6.1/nb_helpers/clean.py`

 * *Files identical despite different names*

### Comparing `nb_helpers-0.6.0/nb_helpers/colab.py` & `nb_helpers-0.6.1/nb_helpers/colab.py`

 * *Files identical despite different names*

### Comparing `nb_helpers-0.6.0/nb_helpers/docker.py` & `nb_helpers-0.6.1/nb_helpers/docker.py`

 * *Files identical despite different names*

### Comparing `nb_helpers-0.6.0/nb_helpers/export.py` & `nb_helpers-0.6.1/nb_helpers/export.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 # %% ../nbs/06_export.ipynb 13
 def colab_github_url(file):
     "Create a fresh colab URL from file, must be on github repo"
     gh_url = github_url(file)
     colab_url = get_colab_url(file, branch="master")
 
     return (
-        f'[![Run in Google Colab](https://www.tensorflow.org/images/colab_logo_32px.png)]({colab_url}) [Run in Google Colab]({colab_url})'
+        f'\n\n[![Run in Google Colab](https://www.tensorflow.org/images/colab_logo_32px.png)]({colab_url}) [Run in Google Colab]({colab_url})'
         ' &nbsp; '
         f'[![View source on GitHub](https://www.tensorflow.org/images/GitHub-Mark-32px.png)]({gh_url}) [View source on GitHub]({gh_url})'
         '\n\n'
     )
 
 # %% ../nbs/06_export.ipynb 16
 def colab_url(file):
@@ -119,14 +119,15 @@
 def export_nbs(
     path: Param("A path to nb files, can be a list.txt", Path, nargs="?", opt=False) = os.getcwd(),
     verbose: Param("Print errors along the way", store_true) = False,
     outpath: Param("An output folder to save the exported notebooks", Path) = Path(".") ,
 ):
     path = Path(path)
     files = find_nbs(path)
+    outpath = Path(outpath)
     
     for nb_path in files:
         if not is_nb(nb_path):
             raise Exception(f"This {nb_path} is not a notebook!")
         outfile = outpath/(nb_path.with_suffix(".md").name)
         print(f"Exporting notebook {nb_path} -> {outfile}")
         _export_one(nb_path, outfile, verbose=verbose)
```

### Comparing `nb_helpers-0.6.0/nb_helpers/run.py` & `nb_helpers-0.6.1/nb_helpers/run.py`

 * *Files identical despite different names*

### Comparing `nb_helpers-0.6.0/nb_helpers/utils.py` & `nb_helpers-0.6.1/nb_helpers/utils.py`

 * *Files identical despite different names*

### Comparing `nb_helpers-0.6.0/nb_helpers/wandb.py` & `nb_helpers-0.6.1/nb_helpers/wandb.py`

 * *Files identical despite different names*

### Comparing `nb_helpers-0.6.0/nb_helpers.egg-info/PKG-INFO` & `nb_helpers-0.6.1/nb_helpers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nb-helpers
-Version: 0.6.0
+Version: 0.6.1
 Summary: A set of tools for nb handling
 Home-page: https://github.com/wandb/nb_helpers/tree/main/
 Author: Thomas Capelle
 Author-email: tcapelle@wandb.com
 License: MIT License
 Keywords: jupyter notebook
 Platform: UNKNOWN
```

### Comparing `nb_helpers-0.6.0/setup.py` & `nb_helpers-0.6.1/setup.py`

 * *Files identical despite different names*

