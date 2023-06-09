# Comparing `tmp/nb_helpers-0.5.3.tar.gz` & `tmp/nb_helpers-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nb_helpers-0.5.3.tar", last modified: Tue May 30 20:43:29 2023, max compression
+gzip compressed data, was "nb_helpers-0.6.0.tar", last modified: Fri Jun  9 21:35:47 2023, max compression
```

## Comparing `nb_helpers-0.5.3.tar` & `nb_helpers-0.6.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:43:29.277111 nb_helpers-0.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-30 20:43:17.000000 nb_helpers-0.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-05-30 20:43:29.277111 nb_helpers-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8915 2023-05-30 20:43:17.000000 nb_helpers-0.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:43:29.277111 nb_helpers-0.5.3/nb_helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-30 20:43:17.000000 nb_helpers-0.5.3/nb_helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11177 2023-05-30 20:43:17.000000 nb_helpers-0.5.3/nb_helpers/_modidx.py
--rw-r--r--   0 runner    (1001) docker     (123)     6950 2023-05-30 20:43:17.000000 nb_helpers-0.5.3/nb_helpers/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-05-30 20:43:17.000000 nb_helpers-0.5.3/nb_helpers/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-05-30 20:43:17.000000 nb_helpers-0.5.3/nb_helpers/colab.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-05-30 20:43:17.000000 nb_helpers-0.5.3/nb_helpers/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-05-30 20:43:17.000000 nb_helpers-0.5.3/nb_helpers/export.py
--rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-05-30 20:43:17.000000 nb_helpers-0.5.3/nb_helpers/run.py
--rw-r--r--   0 runner    (1001) docker     (123)    12069 2023-05-30 20:43:17.000000 nb_helpers-0.5.3/nb_helpers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-05-30 20:43:17.000000 nb_helpers-0.5.3/nb_helpers/wandb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:43:29.277111 nb_helpers-0.5.3/nb_helpers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-05-30 20:43:29.000000 nb_helpers-0.5.3/nb_helpers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-30 20:43:29.000000 nb_helpers-0.5.3/nb_helpers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 20:43:29.000000 nb_helpers-0.5.3/nb_helpers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-30 20:43:29.000000 nb_helpers-0.5.3/nb_helpers.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 20:43:29.000000 nb_helpers-0.5.3/nb_helpers.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-30 20:43:29.000000 nb_helpers-0.5.3/nb_helpers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-30 20:43:29.000000 nb_helpers-0.5.3/nb_helpers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-30 20:43:17.000000 nb_helpers-0.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 20:43:29.277111 nb_helpers-0.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-05-30 20:43:17.000000 nb_helpers-0.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 21:35:47.945246 nb_helpers-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-09 21:35:34.000000 nb_helpers-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-06-09 21:35:47.945246 nb_helpers-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8915 2023-06-09 21:35:34.000000 nb_helpers-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 21:35:47.941246 nb_helpers-0.6.0/nb_helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-09 21:35:34.000000 nb_helpers-0.6.0/nb_helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11322 2023-06-09 21:35:34.000000 nb_helpers-0.6.0/nb_helpers/_modidx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6950 2023-06-09 21:35:34.000000 nb_helpers-0.6.0/nb_helpers/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-06-09 21:35:34.000000 nb_helpers-0.6.0/nb_helpers/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-06-09 21:35:34.000000 nb_helpers-0.6.0/nb_helpers/colab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-06-09 21:35:34.000000 nb_helpers-0.6.0/nb_helpers/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-06-09 21:35:34.000000 nb_helpers-0.6.0/nb_helpers/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-06-09 21:35:34.000000 nb_helpers-0.6.0/nb_helpers/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12417 2023-06-09 21:35:34.000000 nb_helpers-0.6.0/nb_helpers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-06-09 21:35:34.000000 nb_helpers-0.6.0/nb_helpers/wandb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 21:35:47.945246 nb_helpers-0.6.0/nb_helpers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-06-09 21:35:47.000000 nb_helpers-0.6.0/nb_helpers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-09 21:35:47.000000 nb_helpers-0.6.0/nb_helpers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 21:35:47.000000 nb_helpers-0.6.0/nb_helpers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-09 21:35:47.000000 nb_helpers-0.6.0/nb_helpers.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 21:35:47.000000 nb_helpers-0.6.0/nb_helpers.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-09 21:35:47.000000 nb_helpers-0.6.0/nb_helpers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-09 21:35:47.000000 nb_helpers-0.6.0/nb_helpers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-09 21:35:34.000000 nb_helpers-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 21:35:47.945246 nb_helpers-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-06-09 21:35:34.000000 nb_helpers-0.6.0/setup.py
```

### Comparing `nb_helpers-0.5.3/LICENSE` & `nb_helpers-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nb_helpers-0.5.3/PKG-INFO` & `nb_helpers-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nb_helpers
-Version: 0.5.3
+Version: 0.6.0
 Summary: A set of tools for nb handling
 Home-page: https://github.com/wandb/nb_helpers/tree/main/
 Author: Thomas Capelle
 Author-email: tcapelle@wandb.com
 License: MIT License
 Keywords: jupyter notebook
 Platform: UNKNOWN
```

### Comparing `nb_helpers-0.5.3/README.md` & `nb_helpers-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `nb_helpers-0.5.3/nb_helpers/_modidx.py` & `nb_helpers-0.6.0/nb_helpers/_modidx.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,21 +33,21 @@
                                   'nb_helpers.colab.create_colab_badge_cell': ('colab.html#create_colab_badge_cell', 'nb_helpers/colab.py'),
                                   'nb_helpers.colab.get_colab_url': ('colab.html#get_colab_url', 'nb_helpers/colab.py'),
                                   'nb_helpers.colab.has_colab_badge': ('colab.html#has_colab_badge', 'nb_helpers/colab.py')},
             'nb_helpers.docker': {},
             'nb_helpers.export': { 'nb_helpers.export._export_code_cell': ('export.html#_export_code_cell', 'nb_helpers/export.py'),
                                    'nb_helpers.export._export_md_cell': ('export.html#_export_md_cell', 'nb_helpers/export.py'),
                                    'nb_helpers.export._export_one': ('export.html#_export_one', 'nb_helpers/export.py'),
+                                   'nb_helpers.export.colab_github_url': ('export.html#colab_github_url', 'nb_helpers/export.py'),
                                    'nb_helpers.export.colab_url': ('export.html#colab_url', 'nb_helpers/export.py'),
                                    'nb_helpers.export.default_line_filter': ('export.html#default_line_filter', 'nb_helpers/export.py'),
-                                   'nb_helpers.export.export': ('export.html#export', 'nb_helpers/export.py'),
                                    'nb_helpers.export.export_cell': ('export.html#export_cell', 'nb_helpers/export.py'),
                                    'nb_helpers.export.export_nbs': ('export.html#export_nbs', 'nb_helpers/export.py'),
                                    'nb_helpers.export.filter_out_lines': ('export.html#filter_out_lines', 'nb_helpers/export.py'),
-                                   'nb_helpers.export.read_list_file': ('export.html#read_list_file', 'nb_helpers/export.py')},
+                                   'nb_helpers.export.remove_banner_image': ('export.html#remove_banner_image', 'nb_helpers/export.py')},
             'nb_helpers.run': { 'nb_helpers.run.CaptureShell.prettytb': ('run.html#captureshell.prettytb', 'nb_helpers/run.py'),
                                 'nb_helpers.run.exec_nb': ('run.html#exec_nb', 'nb_helpers/run.py'),
                                 'nb_helpers.run.run_nbs': ('run.html#run_nbs', 'nb_helpers/run.py'),
                                 'nb_helpers.run.run_one': ('run.html#run_one', 'nb_helpers/run.py'),
                                 'nb_helpers.run.skip_nb': ('run.html#skip_nb', 'nb_helpers/run.py')},
             'nb_helpers.utils': { 'nb_helpers.utils.RichLogger': ('utils.html#richlogger', 'nb_helpers/utils.py'),
                                   'nb_helpers.utils.RichLogger.__init__': ('utils.html#richlogger.__init__', 'nb_helpers/utils.py'),
@@ -76,14 +76,15 @@
                                   'nb_helpers.utils.get_repo': ('utils.html#get_repo', 'nb_helpers/utils.py'),
                                   'nb_helpers.utils.git_branches': ('utils.html#git_branches', 'nb_helpers/utils.py'),
                                   'nb_helpers.utils.git_current_branch': ('utils.html#git_current_branch', 'nb_helpers/utils.py'),
                                   'nb_helpers.utils.git_last_commit': ('utils.html#git_last_commit', 'nb_helpers/utils.py'),
                                   'nb_helpers.utils.git_local_repo': ('utils.html#git_local_repo', 'nb_helpers/utils.py'),
                                   'nb_helpers.utils.git_main_name': ('utils.html#git_main_name', 'nb_helpers/utils.py'),
                                   'nb_helpers.utils.git_origin_repo': ('utils.html#git_origin_repo', 'nb_helpers/utils.py'),
+                                  'nb_helpers.utils.github_url': ('utils.html#github_url', 'nb_helpers/utils.py'),
                                   'nb_helpers.utils.is_nb': ('utils.html#is_nb', 'nb_helpers/utils.py'),
                                   'nb_helpers.utils.load_list_from_file': ('utils.html#load_list_from_file', 'nb_helpers/utils.py'),
                                   'nb_helpers.utils.load_notebooks_from_file': ( 'utils.html#load_notebooks_from_file',
                                                                                  'nb_helpers/utils.py'),
                                   'nb_helpers.utils.print_output': ('utils.html#print_output', 'nb_helpers/utils.py'),
                                   'nb_helpers.utils.remove_rich_format': ('utils.html#remove_rich_format', 'nb_helpers/utils.py'),
                                   'nb_helpers.utils.search_cell': ('utils.html#search_cell', 'nb_helpers/utils.py'),
```

### Comparing `nb_helpers-0.5.3/nb_helpers/actions.py` & `nb_helpers-0.6.0/nb_helpers/actions.py`

 * *Files identical despite different names*

### Comparing `nb_helpers-0.5.3/nb_helpers/clean.py` & `nb_helpers-0.6.0/nb_helpers/clean.py`

 * *Files identical despite different names*

### Comparing `nb_helpers-0.5.3/nb_helpers/colab.py` & `nb_helpers-0.6.0/nb_helpers/colab.py`

 * *Files identical despite different names*

### Comparing `nb_helpers-0.5.3/nb_helpers/docker.py` & `nb_helpers-0.6.0/nb_helpers/docker.py`

 * *Files identical despite different names*

### Comparing `nb_helpers-0.5.3/nb_helpers/run.py` & `nb_helpers-0.6.0/nb_helpers/run.py`

 * *Files identical despite different names*

### Comparing `nb_helpers-0.5.3/nb_helpers/utils.py` & `nb_helpers-0.6.0/nb_helpers/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/02_utils.ipynb.
 
 # %% auto 0
 __all__ = ['LOGFORMAT', 'LOGFORMAT_RICH', 'STATUS', 'CellType', 'create_table', 'remove_rich_format', 'csv_to_md', 'RichLogger',
            'is_nb', 'load_list_from_file', 'load_notebooks_from_file', 'find_nbs', 'print_output', 'search_cell',
            'search_cells', 'search_string_in_nb', 'extract_libs', 'detect_imported_libs', 'get_repo',
            'git_current_branch', 'git_branches', 'git_main_name', 'git_origin_repo', 'git_local_repo',
-           'git_last_commit', 'today']
+           'git_last_commit', 'github_url', 'today']
 
 # %% ../nbs/02_utils.ipynb 3
 import io, json, sys, re, csv, logging
 import git
 from types import SimpleNamespace
 from logging import Formatter
 from logging.handlers import RotatingFileHandler
@@ -309,47 +309,56 @@
 # %% ../nbs/02_utils.ipynb 58
 def git_main_name(fname) -> str:
     "Get the name of master/main branch"
     repo = get_repo(fname)
     branches = git_branches(repo)
     return "main" if "main" in branches else "master"
 
-# %% ../nbs/02_utils.ipynb 60
+# %% ../nbs/02_utils.ipynb 62
 def _get_github_repo_remote(repo_url):
     if "git@" in repo_url:
         github_repo = re.search(r".com:(.*).git", repo_url).group(1)
     else:
         github_repo = re.search(r".com/(.*)", repo_url).group(1)
     return github_repo
 
-# %% ../nbs/02_utils.ipynb 62
+# %% ../nbs/02_utils.ipynb 64
 def git_origin_repo(fname):
     "Get github repo name from `fname`"
     repo = get_repo(fname)
     repo_url = repo.remote().url
 
     # check if ssh or html
     if repo_url != "":
         return _get_github_repo_remote(repo_url)
     else:
         raise Exception(f"Not in a valid github repo: {fname=}")
 
-# %% ../nbs/02_utils.ipynb 64
+# %% ../nbs/02_utils.ipynb 66
 def git_local_repo(fname):
     "Get local github repo path"
     repo = get_repo(fname)
     return Path(repo.git_dir).parent.resolve()
 
-# %% ../nbs/02_utils.ipynb 66
+# %% ../nbs/02_utils.ipynb 68
 def git_last_commit(fname):
     "Gets the last commit on fname"
     repo = get_repo(fname)
     return repo.commit().hexsha
 
-# %% ../nbs/02_utils.ipynb 69
+# %% ../nbs/02_utils.ipynb 70
+def github_url(fname, branch=None):
+    "Get corresponding github URL"
+    fname = fname.resolve()
+    branch = ifnone(branch, git_main_name(fname))
+    repo = git_origin_repo(fname)
+    fname = fname.relative_to(git_local_repo(fname))
+    return f"https://github.com/{repo}/blob/{branch}/{str(fname)}"
+
+# %% ../nbs/02_utils.ipynb 73
 def today():
     "datetime object containing current date and time"
     now = datetime.now()
 
     # dd/mm/YY H:M:S
     dt_string = now.strftime("%d/%m/%Y %H:%M:%S")
     return dt_string
```

### Comparing `nb_helpers-0.5.3/nb_helpers/wandb.py` & `nb_helpers-0.6.0/nb_helpers/wandb.py`

 * *Files identical despite different names*

### Comparing `nb_helpers-0.5.3/nb_helpers.egg-info/PKG-INFO` & `nb_helpers-0.6.0/nb_helpers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nb-helpers
-Version: 0.5.3
+Version: 0.6.0
 Summary: A set of tools for nb handling
 Home-page: https://github.com/wandb/nb_helpers/tree/main/
 Author: Thomas Capelle
 Author-email: tcapelle@wandb.com
 License: MIT License
 Keywords: jupyter notebook
 Platform: UNKNOWN
```

### Comparing `nb_helpers-0.5.3/setup.py` & `nb_helpers-0.6.0/setup.py`

 * *Files identical despite different names*

