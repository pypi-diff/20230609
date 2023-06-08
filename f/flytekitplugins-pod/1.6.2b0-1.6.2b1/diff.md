# Comparing `tmp/flytekitplugins-pod-1.6.2b0.tar.gz` & `tmp/flytekitplugins-pod-1.6.2b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-pod-1.6.2b0.tar", last modified: Thu Jun  1 20:41:56 2023, max compression
+gzip compressed data, was "flytekitplugins-pod-1.6.2b1.tar", last modified: Thu Jun  8 23:49:46 2023, max compression
```

## Comparing `flytekitplugins-pod-1.6.2b0.tar` & `flytekitplugins-pod-1.6.2b1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:56.035843 flytekitplugins-pod-1.6.2b0/
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-01 20:41:56.035843 flytekitplugins-pod-1.6.2b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-06-01 20:41:31.000000 flytekitplugins-pod-1.6.2b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:56.035843 flytekitplugins-pod-1.6.2b0/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:56.035843 flytekitplugins-pod-1.6.2b0/flytekitplugins/pod/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-01 20:41:31.000000 flytekitplugins-pod-1.6.2b0/flytekitplugins/pod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-06-01 20:41:31.000000 flytekitplugins-pod-1.6.2b0/flytekitplugins/pod/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:56.035843 flytekitplugins-pod-1.6.2b0/flytekitplugins_pod.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-01 20:41:56.000000 flytekitplugins-pod-1.6.2b0/flytekitplugins_pod.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-01 20:41:56.000000 flytekitplugins-pod-1.6.2b0/flytekitplugins_pod.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 20:41:56.000000 flytekitplugins-pod-1.6.2b0/flytekitplugins_pod.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-01 20:41:56.000000 flytekitplugins-pod-1.6.2b0/flytekitplugins_pod.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-01 20:41:56.000000 flytekitplugins-pod-1.6.2b0/flytekitplugins_pod.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-01 20:41:56.000000 flytekitplugins-pod-1.6.2b0/flytekitplugins_pod.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 20:41:56.035843 flytekitplugins-pod-1.6.2b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-01 20:41:50.000000 flytekitplugins-pod-1.6.2b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:46.483246 flytekitplugins-pod-1.6.2b1/
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-08 23:49:46.483246 flytekitplugins-pod-1.6.2b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-06-08 23:49:15.000000 flytekitplugins-pod-1.6.2b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:46.479246 flytekitplugins-pod-1.6.2b1/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:46.479246 flytekitplugins-pod-1.6.2b1/flytekitplugins/pod/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-08 23:49:15.000000 flytekitplugins-pod-1.6.2b1/flytekitplugins/pod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-06-08 23:49:15.000000 flytekitplugins-pod-1.6.2b1/flytekitplugins/pod/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:46.483246 flytekitplugins-pod-1.6.2b1/flytekitplugins_pod.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-08 23:49:46.000000 flytekitplugins-pod-1.6.2b1/flytekitplugins_pod.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-08 23:49:46.000000 flytekitplugins-pod-1.6.2b1/flytekitplugins_pod.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 23:49:46.000000 flytekitplugins-pod-1.6.2b1/flytekitplugins_pod.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-08 23:49:46.000000 flytekitplugins-pod-1.6.2b1/flytekitplugins_pod.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-08 23:49:46.000000 flytekitplugins-pod-1.6.2b1/flytekitplugins_pod.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-08 23:49:46.000000 flytekitplugins-pod-1.6.2b1/flytekitplugins_pod.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 23:49:46.483246 flytekitplugins-pod-1.6.2b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-08 23:49:38.000000 flytekitplugins-pod-1.6.2b1/setup.py
```

### Comparing `flytekitplugins-pod-1.6.2b0/PKG-INFO` & `flytekitplugins-pod-1.6.2b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-pod
-Version: 1.6.2b0
+Version: 1.6.2b1
 Summary: Flytekit plugin to support K8s Pod tasks
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-pod-1.6.2b0/README.md` & `flytekitplugins-pod-1.6.2b1/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins-pod-1.6.2b0/flytekitplugins/pod/task.py` & `flytekitplugins-pod-1.6.2b1/flytekitplugins/pod/task.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-pod-1.6.2b0/flytekitplugins_pod.egg-info/PKG-INFO` & `flytekitplugins-pod-1.6.2b1/flytekitplugins_pod.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-pod
-Version: 1.6.2b0
+Version: 1.6.2b1
 Summary: Flytekit plugin to support K8s Pod tasks
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-pod-1.6.2b0/setup.py` & `flytekitplugins-pod-1.6.2b1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = [
     "flytekit>=1.3.0b2,<2.0.0",
     "kubernetes>=12.0.1",
 ]
 
-__version__ = "1.6.2b0"
+__version__ = "1.6.2b1"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="Flytekit plugin to support K8s Pod tasks",
```

