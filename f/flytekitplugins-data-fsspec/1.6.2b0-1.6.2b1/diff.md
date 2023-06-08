# Comparing `tmp/flytekitplugins-data-fsspec-1.6.2b0.tar.gz` & `tmp/flytekitplugins-data-fsspec-1.6.2b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-data-fsspec-1.6.2b0.tar", last modified: Thu Jun  1 20:41:52 2023, max compression
+gzip compressed data, was "flytekitplugins-data-fsspec-1.6.2b1.tar", last modified: Thu Jun  8 23:49:41 2023, max compression
```

## Comparing `flytekitplugins-data-fsspec-1.6.2b0.tar` & `flytekitplugins-data-fsspec-1.6.2b1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:52.859803 flytekitplugins-data-fsspec-1.6.2b0/
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-06-01 20:41:52.859803 flytekitplugins-data-fsspec-1.6.2b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-01 20:41:31.000000 flytekitplugins-data-fsspec-1.6.2b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:52.859803 flytekitplugins-data-fsspec-1.6.2b0/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:52.859803 flytekitplugins-data-fsspec-1.6.2b0/flytekitplugins/fsspec/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:31.000000 flytekitplugins-data-fsspec-1.6.2b0/flytekitplugins/fsspec/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:52.859803 flytekitplugins-data-fsspec-1.6.2b0/flytekitplugins_data_fsspec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-06-01 20:41:52.000000 flytekitplugins-data-fsspec-1.6.2b0/flytekitplugins_data_fsspec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-01 20:41:52.000000 flytekitplugins-data-fsspec-1.6.2b0/flytekitplugins_data_fsspec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 20:41:52.000000 flytekitplugins-data-fsspec-1.6.2b0/flytekitplugins_data_fsspec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-01 20:41:52.000000 flytekitplugins-data-fsspec-1.6.2b0/flytekitplugins_data_fsspec.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-01 20:41:52.000000 flytekitplugins-data-fsspec-1.6.2b0/flytekitplugins_data_fsspec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-01 20:41:52.000000 flytekitplugins-data-fsspec-1.6.2b0/flytekitplugins_data_fsspec.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 20:41:52.859803 flytekitplugins-data-fsspec-1.6.2b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-06-01 20:41:50.000000 flytekitplugins-data-fsspec-1.6.2b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:41.731221 flytekitplugins-data-fsspec-1.6.2b1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-06-08 23:49:41.731221 flytekitplugins-data-fsspec-1.6.2b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-08 23:49:15.000000 flytekitplugins-data-fsspec-1.6.2b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:41.727221 flytekitplugins-data-fsspec-1.6.2b1/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:41.727221 flytekitplugins-data-fsspec-1.6.2b1/flytekitplugins/fsspec/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:15.000000 flytekitplugins-data-fsspec-1.6.2b1/flytekitplugins/fsspec/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:41.731221 flytekitplugins-data-fsspec-1.6.2b1/flytekitplugins_data_fsspec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-06-08 23:49:41.000000 flytekitplugins-data-fsspec-1.6.2b1/flytekitplugins_data_fsspec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-08 23:49:41.000000 flytekitplugins-data-fsspec-1.6.2b1/flytekitplugins_data_fsspec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 23:49:41.000000 flytekitplugins-data-fsspec-1.6.2b1/flytekitplugins_data_fsspec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-08 23:49:41.000000 flytekitplugins-data-fsspec-1.6.2b1/flytekitplugins_data_fsspec.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-08 23:49:41.000000 flytekitplugins-data-fsspec-1.6.2b1/flytekitplugins_data_fsspec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-08 23:49:41.000000 flytekitplugins-data-fsspec-1.6.2b1/flytekitplugins_data_fsspec.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 23:49:41.731221 flytekitplugins-data-fsspec-1.6.2b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-06-08 23:49:38.000000 flytekitplugins-data-fsspec-1.6.2b1/setup.py
```

### Comparing `flytekitplugins-data-fsspec-1.6.2b0/PKG-INFO` & `flytekitplugins-data-fsspec-1.6.2b1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-data-fsspec
-Version: 1.6.2b0
+Version: 1.6.2b1
 Summary: This is a deprecated plugin as of flytekit 1.5
 Home-page: https://github.com/flyteorg/flytekit/tree/master/plugins/flytekit-data-fsspec
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `flytekitplugins-data-fsspec-1.6.2b0/flytekitplugins_data_fsspec.egg-info/PKG-INFO` & `flytekitplugins-data-fsspec-1.6.2b1/flytekitplugins_data_fsspec.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-data-fsspec
-Version: 1.6.2b0
+Version: 1.6.2b1
 Summary: This is a deprecated plugin as of flytekit 1.5
 Home-page: https://github.com/flyteorg/flytekit/tree/master/plugins/flytekit-data-fsspec
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `flytekitplugins-data-fsspec-1.6.2b0/setup.py` & `flytekitplugins-data-fsspec-1.6.2b1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "fsspec"
 
 microlib_name = f"flytekitplugins-data-{PLUGIN_NAME}"
 
 plugin_requires = []
 
-__version__ = "1.6.2b0"
+__version__ = "1.6.2b1"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="This is a deprecated plugin as of flytekit 1.5",
```

