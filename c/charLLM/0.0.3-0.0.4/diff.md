# Comparing `tmp/charLLM-0.0.3.tar.gz` & `tmp/charLLM-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "charLLM-0.0.3.tar", last modified: Fri Jun  9 11:43:58 2023, max compression
+gzip compressed data, was "charLLM-0.0.4.tar", last modified: Fri Jun  9 14:10:50 2023, max compression
```

## Comparing `charLLM-0.0.3.tar` & `charLLM-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:43:58.122625 charLLM-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-09 11:43:58.122625 charLLM-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-09 11:41:37.000000 charLLM-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-09 11:43:58.122625 charLLM-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:43:58.122625 charLLM-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:43:58.122625 charLLM-0.0.3/src/charLLM/
--rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-06-09 11:41:37.000000 charLLM-0.0.3/src/charLLM/NPLM.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 11:41:37.000000 charLLM-0.0.3/src/charLLM/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:43:58.122625 charLLM-0.0.3/src/charLLM.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-09 11:43:58.000000 charLLM-0.0.3/src/charLLM.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-09 11:43:58.000000 charLLM-0.0.3/src/charLLM.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 11:43:58.000000 charLLM-0.0.3/src/charLLM.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-09 11:43:58.000000 charLLM-0.0.3/src/charLLM.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:10:50.756096 charLLM-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11413 2023-06-09 14:08:32.000000 charLLM-0.0.4/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-06-09 14:10:50.756096 charLLM-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-06-09 14:08:32.000000 charLLM-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-09 14:08:32.000000 charLLM-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-09 14:10:50.756096 charLLM-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:10:50.756096 charLLM-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:10:50.756096 charLLM-0.0.4/src/charLLM/
+-rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-06-09 14:08:32.000000 charLLM-0.0.4/src/charLLM/NPLM.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-09 14:08:32.000000 charLLM-0.0.4/src/charLLM/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:10:50.756096 charLLM-0.0.4/src/charLLM.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-06-09 14:10:50.000000 charLLM-0.0.4/src/charLLM.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-09 14:10:50.000000 charLLM-0.0.4/src/charLLM.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 14:10:50.000000 charLLM-0.0.4/src/charLLM.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-09 14:10:50.000000 charLLM-0.0.4/src/charLLM.egg-info/top_level.txt
```

### Comparing `charLLM-0.0.3/setup.cfg` & `charLLM-0.0.4/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [metadata]
 name = charLLM
-version = 0.0.3
+version = 0.0.4
 author = Aravind
 author_email = aravindan22052001@gmail.com
 description = Character Level Language Model implemented following "Bengio.et.al 2003"
 long_description = file: README.md
 long_description_content_type = text/markdown
-url = https://github.com/RAravindDS/Neural-Probabilistic-Language-Model
+url = https://github.com/RAravindDS/CharLLMs
 project_urls = 
-	Bug Tracker = https://github.com/RAravindDS/Neural-Probabilistic-Language-Model/issues
+	Bug Tracker = https://github.com/RAravindDS/CharLLMs/issues
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 package_dir =
```

### Comparing `charLLM-0.0.3/src/charLLM/NPLM.py` & `charLLM-0.0.4/src/charLLM/NPLM.py`

 * *Files identical despite different names*

