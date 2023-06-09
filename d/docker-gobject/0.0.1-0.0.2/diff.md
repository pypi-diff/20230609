# Comparing `tmp/docker_gobject-0.0.1.tar.gz` & `tmp/docker_gobject-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docker_gobject-0.0.1.tar", last modified: Fri Jun  2 03:33:49 2023, max compression
+gzip compressed data, was "docker_gobject-0.0.2.tar", last modified: Fri Jun  9 18:37:17 2023, max compression
```

## Comparing `docker_gobject-0.0.1.tar` & `docker_gobject-0.0.2.tar`

### file list

```diff
@@ -1,25 +1,28 @@
-drwxr-xr-x   0 cameron   (1000) cameron   (1000)        0 2023-06-02 03:33:49.936012 docker_gobject-0.0.1/
--rw-r--r--   0 cameron   (1000) cameron   (1000)     3078 2023-05-30 18:10:49.000000 docker_gobject-0.0.1/.gitignore
--rw-r--r--   0 cameron   (1000) cameron   (1000)      659 2023-06-02 03:33:49.936012 docker_gobject-0.0.1/PKG-INFO
--rw-r--r--   0 cameron   (1000) cameron   (1000)       73 2023-05-29 17:13:27.000000 docker_gobject-0.0.1/README.md
-drwxr-xr-x   0 cameron   (1000) cameron   (1000)        0 2023-06-02 03:33:49.933012 docker_gobject-0.0.1/docker_gobject/
-drwxr-xr-x   0 cameron   (1000) cameron   (1000)        0 2023-06-02 03:33:49.935012 docker_gobject-0.0.1/docker_gobject/.vscode/
--rw-r--r--   0 cameron   (1000) cameron   (1000)       51 2023-05-05 13:47:29.000000 docker_gobject-0.0.1/docker_gobject/.vscode/settings.json
--rw-r--r--   0 cameron   (1000) cameron   (1000)     2207 2023-06-02 03:29:22.000000 docker_gobject-0.0.1/docker_gobject/__init__.py
--rw-r--r--   0 cameron   (1000) cameron   (1000)      573 2023-06-02 03:32:08.000000 docker_gobject-0.0.1/docker_gobject/__main__.py
--rw-r--r--   0 cameron   (1000) cameron   (1000)      897 2023-02-26 06:15:01.000000 docker_gobject-0.0.1/docker_gobject/authentication.py
--rw-r--r--   0 cameron   (1000) cameron   (1000)     1577 2023-06-02 03:32:51.000000 docker_gobject-0.0.1/docker_gobject/client.py
--rw-r--r--   0 cameron   (1000) cameron   (1000)    18339 2023-06-01 02:00:32.000000 docker_gobject-0.0.1/docker_gobject/container.py
--rw-r--r--   0 cameron   (1000) cameron   (1000)     1333 2023-06-02 03:31:56.000000 docker_gobject-0.0.1/docker_gobject/containers.py
--rw-r--r--   0 cameron   (1000) cameron   (1000)     5426 2023-06-01 02:45:23.000000 docker_gobject-0.0.1/docker_gobject/image.py
--rw-r--r--   0 cameron   (1000) cameron   (1000)     1105 2023-06-02 03:31:35.000000 docker_gobject-0.0.1/docker_gobject/images.py
--rw-r--r--   0 cameron   (1000) cameron   (1000)     2627 2023-05-29 17:27:21.000000 docker_gobject-0.0.1/docker_gobject/monitor.py
--rw-r--r--   0 cameron   (1000) cameron   (1000)     2681 2023-06-02 03:33:33.000000 docker_gobject-0.0.1/docker_gobject/session.py
-drwxr-xr-x   0 cameron   (1000) cameron   (1000)        0 2023-06-02 03:33:49.934013 docker_gobject-0.0.1/docker_gobject.egg-info/
--rw-r--r--   0 cameron   (1000) cameron   (1000)      659 2023-06-02 03:33:49.000000 docker_gobject-0.0.1/docker_gobject.egg-info/PKG-INFO
--rw-r--r--   0 cameron   (1000) cameron   (1000)      531 2023-06-02 03:33:49.000000 docker_gobject-0.0.1/docker_gobject.egg-info/SOURCES.txt
--rw-r--r--   0 cameron   (1000) cameron   (1000)        1 2023-06-02 03:33:49.000000 docker_gobject-0.0.1/docker_gobject.egg-info/dependency_links.txt
--rw-r--r--   0 cameron   (1000) cameron   (1000)       10 2023-06-02 03:33:49.000000 docker_gobject-0.0.1/docker_gobject.egg-info/requires.txt
--rw-r--r--   0 cameron   (1000) cameron   (1000)       15 2023-06-02 03:33:49.000000 docker_gobject-0.0.1/docker_gobject.egg-info/top_level.txt
--rw-r--r--   0 cameron   (1000) cameron   (1000)      759 2023-05-31 03:40:18.000000 docker_gobject-0.0.1/pyproject.toml
--rw-r--r--   0 cameron   (1000) cameron   (1000)       38 2023-06-02 03:33:49.937012 docker_gobject-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:37:17.444800 docker_gobject-0.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:37:17.440800 docker_gobject-0.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:37:17.440800 docker_gobject-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-09 18:37:07.000000 docker_gobject-0.0.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-06-09 18:37:07.000000 docker_gobject-0.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-09 18:37:17.440800 docker_gobject-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-09 18:37:07.000000 docker_gobject-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:37:17.440800 docker_gobject-0.0.2/docker_gobject/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:37:17.440800 docker_gobject-0.0.2/docker_gobject/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-09 18:37:07.000000 docker_gobject-0.0.2/docker_gobject/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-06-09 18:37:07.000000 docker_gobject-0.0.2/docker_gobject/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-09 18:37:07.000000 docker_gobject-0.0.2/docker_gobject/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-09 18:37:07.000000 docker_gobject-0.0.2/docker_gobject/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-06-09 18:37:07.000000 docker_gobject-0.0.2/docker_gobject/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18339 2023-06-09 18:37:07.000000 docker_gobject-0.0.2/docker_gobject/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-06-09 18:37:07.000000 docker_gobject-0.0.2/docker_gobject/containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-06-09 18:37:07.000000 docker_gobject-0.0.2/docker_gobject/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-09 18:37:07.000000 docker_gobject-0.0.2/docker_gobject/images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-06-09 18:37:07.000000 docker_gobject-0.0.2/docker_gobject/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-06-09 18:37:07.000000 docker_gobject-0.0.2/docker_gobject/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:37:17.440800 docker_gobject-0.0.2/docker_gobject.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-09 18:37:17.000000 docker_gobject-0.0.2/docker_gobject.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-09 18:37:17.000000 docker_gobject-0.0.2/docker_gobject.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 18:37:17.000000 docker_gobject-0.0.2/docker_gobject.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-09 18:37:17.000000 docker_gobject-0.0.2/docker_gobject.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-09 18:37:17.000000 docker_gobject-0.0.2/docker_gobject.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-09 18:37:07.000000 docker_gobject-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 18:37:17.444800 docker_gobject-0.0.2/setup.cfg
```

### Comparing `docker_gobject-0.0.1/.gitignore` & `docker_gobject-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `docker_gobject-0.0.1/PKG-INFO` & `docker_gobject-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docker_gobject
-Version: 0.0.1
+Version: 0.0.2
 Summary: GObject wrapper for Docker Engine
 Author-email: Cameron Dahl <cameron@cameorndahl.com>
 Project-URL: Homepage, https://github.com/cameronthecoder/docker_gobject
 Project-URL: Bug Tracker, https://github.com/pypa/docker_gobject/issues
 Keywords: pygobject,gtk,gtk4,docker,wrapper,python,python3,libsoup,soup,glib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `docker_gobject-0.0.1/docker_gobject/__init__.py` & `docker_gobject-0.0.2/docker_gobject/__init__.py`

 * *Files identical despite different names*

### Comparing `docker_gobject-0.0.1/docker_gobject/__main__.py` & `docker_gobject-0.0.2/docker_gobject/__main__.py`

 * *Files identical despite different names*

### Comparing `docker_gobject-0.0.1/docker_gobject/authentication.py` & `docker_gobject-0.0.2/docker_gobject/authentication.py`

 * *Files identical despite different names*

### Comparing `docker_gobject-0.0.1/docker_gobject/client.py` & `docker_gobject-0.0.2/docker_gobject/client.py`

 * *Files identical despite different names*

### Comparing `docker_gobject-0.0.1/docker_gobject/container.py` & `docker_gobject-0.0.2/docker_gobject/container.py`

 * *Files identical despite different names*

### Comparing `docker_gobject-0.0.1/docker_gobject/containers.py` & `docker_gobject-0.0.2/docker_gobject/containers.py`

 * *Files identical despite different names*

### Comparing `docker_gobject-0.0.1/docker_gobject/image.py` & `docker_gobject-0.0.2/docker_gobject/image.py`

 * *Files identical despite different names*

### Comparing `docker_gobject-0.0.1/docker_gobject/images.py` & `docker_gobject-0.0.2/docker_gobject/images.py`

 * *Files identical despite different names*

### Comparing `docker_gobject-0.0.1/docker_gobject/monitor.py` & `docker_gobject-0.0.2/docker_gobject/monitor.py`

 * *Files identical despite different names*

### Comparing `docker_gobject-0.0.1/docker_gobject/session.py` & `docker_gobject-0.0.2/docker_gobject/session.py`

 * *Files identical despite different names*

### Comparing `docker_gobject-0.0.1/docker_gobject.egg-info/PKG-INFO` & `docker_gobject-0.0.2/docker_gobject.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docker-gobject
-Version: 0.0.1
+Version: 0.0.2
 Summary: GObject wrapper for Docker Engine
 Author-email: Cameron Dahl <cameron@cameorndahl.com>
 Project-URL: Homepage, https://github.com/cameronthecoder/docker_gobject
 Project-URL: Bug Tracker, https://github.com/pypa/docker_gobject/issues
 Keywords: pygobject,gtk,gtk4,docker,wrapper,python,python3,libsoup,soup,glib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `docker_gobject-0.0.1/pyproject.toml` & `docker_gobject-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "docker_gobject"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Cameron Dahl", email="cameron@cameorndahl.com" },
 ]
 description = "GObject wrapper for Docker Engine"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

