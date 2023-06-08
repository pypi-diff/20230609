# Comparing `tmp/flytekitplugins-huggingface-1.6.2b0.tar.gz` & `tmp/flytekitplugins-huggingface-1.6.2b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-huggingface-1.6.2b0.tar", last modified: Thu Jun  1 20:41:55 2023, max compression
+gzip compressed data, was "flytekitplugins-huggingface-1.6.2b1.tar", last modified: Thu Jun  8 23:49:45 2023, max compression
```

## Comparing `flytekitplugins-huggingface-1.6.2b0.tar` & `flytekitplugins-huggingface-1.6.2b1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:55.687838 flytekitplugins-huggingface-1.6.2b0/
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-06-01 20:41:55.687838 flytekitplugins-huggingface-1.6.2b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-01 20:41:31.000000 flytekitplugins-huggingface-1.6.2b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:55.687838 flytekitplugins-huggingface-1.6.2b0/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:55.687838 flytekitplugins-huggingface-1.6.2b0/flytekitplugins/huggingface/
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-01 20:41:31.000000 flytekitplugins-huggingface-1.6.2b0/flytekitplugins/huggingface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-06-01 20:41:31.000000 flytekitplugins-huggingface-1.6.2b0/flytekitplugins/huggingface/sd_transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:55.687838 flytekitplugins-huggingface-1.6.2b0/flytekitplugins_huggingface.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-06-01 20:41:55.000000 flytekitplugins-huggingface-1.6.2b0/flytekitplugins_huggingface.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-01 20:41:55.000000 flytekitplugins-huggingface-1.6.2b0/flytekitplugins_huggingface.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 20:41:55.000000 flytekitplugins-huggingface-1.6.2b0/flytekitplugins_huggingface.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-01 20:41:55.000000 flytekitplugins-huggingface-1.6.2b0/flytekitplugins_huggingface.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-01 20:41:55.000000 flytekitplugins-huggingface-1.6.2b0/flytekitplugins_huggingface.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-01 20:41:55.000000 flytekitplugins-huggingface-1.6.2b0/flytekitplugins_huggingface.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-01 20:41:55.000000 flytekitplugins-huggingface-1.6.2b0/flytekitplugins_huggingface.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 20:41:55.687838 flytekitplugins-huggingface-1.6.2b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-01 20:41:50.000000 flytekitplugins-huggingface-1.6.2b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:45.947244 flytekitplugins-huggingface-1.6.2b1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-06-08 23:49:45.947244 flytekitplugins-huggingface-1.6.2b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-08 23:49:15.000000 flytekitplugins-huggingface-1.6.2b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:45.947244 flytekitplugins-huggingface-1.6.2b1/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:45.947244 flytekitplugins-huggingface-1.6.2b1/flytekitplugins/huggingface/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-08 23:49:15.000000 flytekitplugins-huggingface-1.6.2b1/flytekitplugins/huggingface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-06-08 23:49:15.000000 flytekitplugins-huggingface-1.6.2b1/flytekitplugins/huggingface/sd_transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:45.947244 flytekitplugins-huggingface-1.6.2b1/flytekitplugins_huggingface.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-06-08 23:49:45.000000 flytekitplugins-huggingface-1.6.2b1/flytekitplugins_huggingface.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-08 23:49:45.000000 flytekitplugins-huggingface-1.6.2b1/flytekitplugins_huggingface.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 23:49:45.000000 flytekitplugins-huggingface-1.6.2b1/flytekitplugins_huggingface.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-08 23:49:45.000000 flytekitplugins-huggingface-1.6.2b1/flytekitplugins_huggingface.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-08 23:49:45.000000 flytekitplugins-huggingface-1.6.2b1/flytekitplugins_huggingface.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-08 23:49:45.000000 flytekitplugins-huggingface-1.6.2b1/flytekitplugins_huggingface.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-08 23:49:45.000000 flytekitplugins-huggingface-1.6.2b1/flytekitplugins_huggingface.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 23:49:45.947244 flytekitplugins-huggingface-1.6.2b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-08 23:49:38.000000 flytekitplugins-huggingface-1.6.2b1/setup.py
```

### Comparing `flytekitplugins-huggingface-1.6.2b0/PKG-INFO` & `flytekitplugins-huggingface-1.6.2b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-huggingface
-Version: 1.6.2b0
+Version: 1.6.2b1
 Summary: Hugging Face plugin for flytekit
 Home-page: https://github.com/flyteorg/flytekit/tree/master/plugins/flytekit-huggingface
 Author: Evan Sadler
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-huggingface-1.6.2b0/README.md` & `flytekitplugins-huggingface-1.6.2b1/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins-huggingface-1.6.2b0/flytekitplugins/huggingface/sd_transformers.py` & `flytekitplugins-huggingface-1.6.2b1/flytekitplugins/huggingface/sd_transformers.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-huggingface-1.6.2b0/flytekitplugins_huggingface.egg-info/PKG-INFO` & `flytekitplugins-huggingface-1.6.2b1/flytekitplugins_huggingface.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-huggingface
-Version: 1.6.2b0
+Version: 1.6.2b1
 Summary: Hugging Face plugin for flytekit
 Home-page: https://github.com/flyteorg/flytekit/tree/master/plugins/flytekit-huggingface
 Author: Evan Sadler
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-huggingface-1.6.2b0/setup.py` & `flytekitplugins-huggingface-1.6.2b1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = [
     "flytekit>=1.3.0b2,<2.0.0",
     "datasets>=2.4.0",
 ]
 
-__version__ = "1.6.2b0"
+__version__ = "1.6.2b1"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="Evan Sadler",
     description="Hugging Face plugin for flytekit",
     url="https://github.com/flyteorg/flytekit/tree/master/plugins/flytekit-huggingface",
```

