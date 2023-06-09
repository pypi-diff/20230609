# Comparing `tmp/mkdocs-table-reader-plugin-2.0.tar.gz` & `tmp/mkdocs-table-reader-plugin-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-table-reader-plugin-2.0.tar", last modified: Mon Jan 30 13:25:31 2023, max compression
+gzip compressed data, was "mkdocs-table-reader-plugin-2.0.1.tar", last modified: Fri Jun  9 14:24:32 2023, max compression
```

## Comparing `mkdocs-table-reader-plugin-2.0.tar` & `mkdocs-table-reader-plugin-2.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 13:25:31.647221 mkdocs-table-reader-plugin-2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-01-30 13:24:50.000000 mkdocs-table-reader-plugin-2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-01-30 13:25:31.647221 mkdocs-table-reader-plugin-2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-01-30 13:24:50.000000 mkdocs-table-reader-plugin-2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 13:25:31.647221 mkdocs-table-reader-plugin-2.0/mkdocs_table_reader_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 13:24:50.000000 mkdocs-table-reader-plugin-2.0/mkdocs_table_reader_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-01-30 13:24:50.000000 mkdocs-table-reader-plugin-2.0/mkdocs_table_reader_plugin/markdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     5838 2023-01-30 13:24:50.000000 mkdocs-table-reader-plugin-2.0/mkdocs_table_reader_plugin/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-01-30 13:24:50.000000 mkdocs-table-reader-plugin-2.0/mkdocs_table_reader_plugin/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-01-30 13:24:50.000000 mkdocs-table-reader-plugin-2.0/mkdocs_table_reader_plugin/safe_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-01-30 13:24:50.000000 mkdocs-table-reader-plugin-2.0/mkdocs_table_reader_plugin/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 13:25:31.647221 mkdocs-table-reader-plugin-2.0/mkdocs_table_reader_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-01-30 13:25:31.000000 mkdocs-table-reader-plugin-2.0/mkdocs_table_reader_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-01-30 13:25:31.000000 mkdocs-table-reader-plugin-2.0/mkdocs_table_reader_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-30 13:25:31.000000 mkdocs-table-reader-plugin-2.0/mkdocs_table_reader_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-01-30 13:25:31.000000 mkdocs-table-reader-plugin-2.0/mkdocs_table_reader_plugin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-01-30 13:25:31.000000 mkdocs-table-reader-plugin-2.0/mkdocs_table_reader_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-01-30 13:25:31.000000 mkdocs-table-reader-plugin-2.0/mkdocs_table_reader_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-30 13:25:31.647221 mkdocs-table-reader-plugin-2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-01-30 13:24:50.000000 mkdocs-table-reader-plugin-2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:24:32.616880 mkdocs-table-reader-plugin-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-09 14:23:54.000000 mkdocs-table-reader-plugin-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-06-09 14:24:32.616880 mkdocs-table-reader-plugin-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-06-09 14:23:54.000000 mkdocs-table-reader-plugin-2.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:24:32.616880 mkdocs-table-reader-plugin-2.0.1/mkdocs_table_reader_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 14:23:54.000000 mkdocs-table-reader-plugin-2.0.1/mkdocs_table_reader_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-09 14:23:54.000000 mkdocs-table-reader-plugin-2.0.1/mkdocs_table_reader_plugin/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5838 2023-06-09 14:23:54.000000 mkdocs-table-reader-plugin-2.0.1/mkdocs_table_reader_plugin/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-06-09 14:23:54.000000 mkdocs-table-reader-plugin-2.0.1/mkdocs_table_reader_plugin/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-06-09 14:23:54.000000 mkdocs-table-reader-plugin-2.0.1/mkdocs_table_reader_plugin/safe_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-09 14:23:54.000000 mkdocs-table-reader-plugin-2.0.1/mkdocs_table_reader_plugin/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:24:32.616880 mkdocs-table-reader-plugin-2.0.1/mkdocs_table_reader_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-06-09 14:24:32.000000 mkdocs-table-reader-plugin-2.0.1/mkdocs_table_reader_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-09 14:24:32.000000 mkdocs-table-reader-plugin-2.0.1/mkdocs_table_reader_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 14:24:32.000000 mkdocs-table-reader-plugin-2.0.1/mkdocs_table_reader_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-09 14:24:32.000000 mkdocs-table-reader-plugin-2.0.1/mkdocs_table_reader_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-09 14:24:32.000000 mkdocs-table-reader-plugin-2.0.1/mkdocs_table_reader_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-09 14:24:32.000000 mkdocs-table-reader-plugin-2.0.1/mkdocs_table_reader_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 14:24:32.616880 mkdocs-table-reader-plugin-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-06-09 14:23:54.000000 mkdocs-table-reader-plugin-2.0.1/setup.py
```

### Comparing `mkdocs-table-reader-plugin-2.0/LICENSE` & `mkdocs-table-reader-plugin-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-table-reader-plugin-2.0/PKG-INFO` & `mkdocs-table-reader-plugin-2.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-table-reader-plugin
-Version: 2.0
+Version: 2.0.1
 Summary: MkDocs plugin to directly insert tables from files into markdown.
 Home-page: https://github.com/timvink/mkdocs-table-reader-plugin
 Author: Tim Vink
 Author-email: vinktim@gmail.com
 License: MIT
 Keywords: mkdocs plugin
 Classifier: Operating System :: OS Independent
@@ -58,12 +58,11 @@
 ```html
 {{ read_csv('path_to_table.csv') }}
 ```
 
 Where the path is relative to the location of your project's `mkdocs.yml` file (although you can [change that](https://timvink.github.io/mkdocs-table-reader-plugin/options) to be relative to your `docs/` directory).
 
 - There are [readers](https://timvink.github.io/mkdocs-table-reader-plugin/readers/) for `.csv`, `.fwf`, `.json`, `.xlsx`, `.yaml` and `.tsv`. There is also the `read_raw()` reader that will allow you to insert tables (or other content) already in markdown format.
-- See the [how to guides](https://timvink.github.io/mkdocs-table-reader-plugin/howto/customize-tables/) for example of various workflows
 
-## Documentation
+## Documentation and how-to guides
 
 See [timvink.github.io/mkdocs-table-reader-plugin/](https://timvink.github.io/mkdocs-table-reader-plugin/)
```

### Comparing `mkdocs-table-reader-plugin-2.0/README.md` & `mkdocs-table-reader-plugin-2.0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -37,12 +37,11 @@
 ```html
 {{ read_csv('path_to_table.csv') }}
 ```
 
 Where the path is relative to the location of your project's `mkdocs.yml` file (although you can [change that](https://timvink.github.io/mkdocs-table-reader-plugin/options) to be relative to your `docs/` directory).
 
 - There are [readers](https://timvink.github.io/mkdocs-table-reader-plugin/readers/) for `.csv`, `.fwf`, `.json`, `.xlsx`, `.yaml` and `.tsv`. There is also the `read_raw()` reader that will allow you to insert tables (or other content) already in markdown format.
-- See the [how to guides](https://timvink.github.io/mkdocs-table-reader-plugin/howto/customize-tables/) for example of various workflows
 
-## Documentation
+## Documentation and how-to guides
 
 See [timvink.github.io/mkdocs-table-reader-plugin/](https://timvink.github.io/mkdocs-table-reader-plugin/)
```

### Comparing `mkdocs-table-reader-plugin-2.0/mkdocs_table_reader_plugin/markdown.py` & `mkdocs-table-reader-plugin-2.0.1/mkdocs_table_reader_plugin/markdown.py`

 * *Files identical despite different names*

### Comparing `mkdocs-table-reader-plugin-2.0/mkdocs_table_reader_plugin/plugin.py` & `mkdocs-table-reader-plugin-2.0.1/mkdocs_table_reader_plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs-table-reader-plugin-2.0/mkdocs_table_reader_plugin/readers.py` & `mkdocs-table-reader-plugin-2.0.1/mkdocs_table_reader_plugin/readers.py`

 * *Files identical despite different names*

### Comparing `mkdocs-table-reader-plugin-2.0/mkdocs_table_reader_plugin/safe_eval.py` & `mkdocs-table-reader-plugin-2.0.1/mkdocs_table_reader_plugin/safe_eval.py`

 * *Files identical despite different names*

### Comparing `mkdocs-table-reader-plugin-2.0/mkdocs_table_reader_plugin.egg-info/PKG-INFO` & `mkdocs-table-reader-plugin-2.0.1/mkdocs_table_reader_plugin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-table-reader-plugin
-Version: 2.0
+Version: 2.0.1
 Summary: MkDocs plugin to directly insert tables from files into markdown.
 Home-page: https://github.com/timvink/mkdocs-table-reader-plugin
 Author: Tim Vink
 Author-email: vinktim@gmail.com
 License: MIT
 Keywords: mkdocs plugin
 Classifier: Operating System :: OS Independent
@@ -58,12 +58,11 @@
 ```html
 {{ read_csv('path_to_table.csv') }}
 ```
 
 Where the path is relative to the location of your project's `mkdocs.yml` file (although you can [change that](https://timvink.github.io/mkdocs-table-reader-plugin/options) to be relative to your `docs/` directory).
 
 - There are [readers](https://timvink.github.io/mkdocs-table-reader-plugin/readers/) for `.csv`, `.fwf`, `.json`, `.xlsx`, `.yaml` and `.tsv`. There is also the `read_raw()` reader that will allow you to insert tables (or other content) already in markdown format.
-- See the [how to guides](https://timvink.github.io/mkdocs-table-reader-plugin/howto/customize-tables/) for example of various workflows
 
-## Documentation
+## Documentation and how-to guides
 
 See [timvink.github.io/mkdocs-table-reader-plugin/](https://timvink.github.io/mkdocs-table-reader-plugin/)
```

### Comparing `mkdocs-table-reader-plugin-2.0/mkdocs_table_reader_plugin.egg-info/SOURCES.txt` & `mkdocs-table-reader-plugin-2.0.1/mkdocs_table_reader_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mkdocs-table-reader-plugin-2.0/setup.py` & `mkdocs-table-reader-plugin-2.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="mkdocs-table-reader-plugin",
-    version="2.0",
+    version="2.0.1",
     description="MkDocs plugin to directly insert tables from files into markdown.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="mkdocs plugin",
     url="https://github.com/timvink/mkdocs-table-reader-plugin",
     author="Tim Vink",
     author_email="vinktim@gmail.com",
```

