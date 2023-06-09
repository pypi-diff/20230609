# Comparing `tmp/dingdong_sonos-0.1.2.tar.gz` & `tmp/dingdong_sonos-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dingdong_sonos-0.1.2.tar", last modified: Thu Jun  8 19:10:20 2023, max compression
+gzip compressed data, was "dingdong_sonos-0.1.3.tar", last modified: Thu Jun  8 19:19:55 2023, max compression
```

## Comparing `dingdong_sonos-0.1.2.tar` & `dingdong_sonos-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,21 @@
-drwxr-xr-x   0 tim        (501) staff       (20)        0 2023-06-08 19:10:20.554172 dingdong_sonos-0.1.2/
--rw-r--r--   0 tim        (501) staff       (20)       30 2023-06-08 13:35:24.000000 dingdong_sonos-0.1.2/MANIFEST.in
--rw-r--r--   0 tim        (501) staff       (20)     1051 2023-06-08 19:10:20.553732 dingdong_sonos-0.1.2/PKG-INFO
--rw-r--r--   0 tim        (501) staff       (20)      393 2023-06-08 14:11:53.000000 dingdong_sonos-0.1.2/README.md
-drwxr-xr-x   0 tim        (501) staff       (20)        0 2023-06-08 19:10:20.545682 dingdong_sonos-0.1.2/dingdong_sonos/
--rw-r--r--   0 tim        (501) staff       (20)        0 2023-06-08 13:27:50.000000 dingdong_sonos-0.1.2/dingdong_sonos/__init__.py
--rw-r--r--   0 tim        (501) staff       (20)     3485 2023-06-08 19:07:23.000000 dingdong_sonos-0.1.2/dingdong_sonos/main.py
-drwxr-xr-x   0 tim        (501) staff       (20)        0 2023-06-08 19:10:20.550554 dingdong_sonos-0.1.2/dingdong_sonos/media/
--rw-r--r--   0 tim        (501) staff       (20)    81465 2023-06-08 13:08:24.000000 dingdong_sonos-0.1.2/dingdong_sonos/media/school-bell-sound.mp3
-drwxr-xr-x   0 tim        (501) staff       (20)        0 2023-06-08 19:10:20.549754 dingdong_sonos-0.1.2/dingdong_sonos.egg-info/
--rw-r--r--   0 tim        (501) staff       (20)     1051 2023-06-08 19:10:20.000000 dingdong_sonos-0.1.2/dingdong_sonos.egg-info/PKG-INFO
--rw-r--r--   0 tim        (501) staff       (20)      359 2023-06-08 19:10:20.000000 dingdong_sonos-0.1.2/dingdong_sonos.egg-info/SOURCES.txt
--rw-r--r--   0 tim        (501) staff       (20)        1 2023-06-08 19:10:20.000000 dingdong_sonos-0.1.2/dingdong_sonos.egg-info/dependency_links.txt
--rw-r--r--   0 tim        (501) staff       (20)       54 2023-06-08 19:10:20.000000 dingdong_sonos-0.1.2/dingdong_sonos.egg-info/entry_points.txt
--rw-r--r--   0 tim        (501) staff       (20)       47 2023-06-08 19:10:20.000000 dingdong_sonos-0.1.2/dingdong_sonos.egg-info/requires.txt
--rw-r--r--   0 tim        (501) staff       (20)       15 2023-06-08 19:10:20.000000 dingdong_sonos-0.1.2/dingdong_sonos.egg-info/top_level.txt
--rw-r--r--   0 tim        (501) staff       (20)     1110 2023-06-08 19:08:34.000000 dingdong_sonos-0.1.2/pyproject.toml
--rw-r--r--   0 tim        (501) staff       (20)       38 2023-06-08 19:10:20.554307 dingdong_sonos-0.1.2/setup.cfg
+drwxr-xr-x   0 tim        (501) staff       (20)        0 2023-06-08 19:19:55.960926 dingdong_sonos-0.1.3/
+-rw-r--r--   0 tim        (501) staff       (20)       30 2023-06-08 13:35:24.000000 dingdong_sonos-0.1.3/MANIFEST.in
+-rw-r--r--   0 tim        (501) staff       (20)     1051 2023-06-08 19:19:55.960541 dingdong_sonos-0.1.3/PKG-INFO
+-rw-r--r--   0 tim        (501) staff       (20)      393 2023-06-08 14:11:53.000000 dingdong_sonos-0.1.3/README.md
+drwxr-xr-x   0 tim        (501) staff       (20)        0 2023-06-08 19:19:55.945835 dingdong_sonos-0.1.3/dingdong_sonos/
+-rw-r--r--   0 tim        (501) staff       (20)        0 2023-06-08 13:27:50.000000 dingdong_sonos-0.1.3/dingdong_sonos/__init__.py
+-rw-r--r--   0 tim        (501) staff       (20)     3485 2023-06-08 19:07:23.000000 dingdong_sonos-0.1.3/dingdong_sonos/main.py
+drwxr-xr-x   0 tim        (501) staff       (20)        0 2023-06-08 19:19:55.958938 dingdong_sonos-0.1.3/dingdong_sonos/media/
+-rw-r--r--   0 tim        (501) staff       (20)    74532 2023-06-08 19:14:52.000000 dingdong_sonos-0.1.3/dingdong_sonos/media/pornhub.mp3
+-rw-rw-r--   0 tim        (501) staff       (20)   737826 2023-06-08 19:13:30.000000 dingdong_sonos-0.1.3/dingdong_sonos/media/quack.mp3
+-rw-r--r--   0 tim        (501) staff       (20)    81465 2023-06-08 13:08:24.000000 dingdong_sonos-0.1.3/dingdong_sonos/media/school-bell-sound.mp3
+-rw-rw-r--   0 tim        (501) staff       (20)    28212 2014-08-26 18:57:44.000000 dingdong_sonos-0.1.3/dingdong_sonos/media/wrong.mp3
+drwxr-xr-x   0 tim        (501) staff       (20)        0 2023-06-08 19:19:55.949514 dingdong_sonos-0.1.3/dingdong_sonos.egg-info/
+-rw-r--r--   0 tim        (501) staff       (20)     1051 2023-06-08 19:19:55.000000 dingdong_sonos-0.1.3/dingdong_sonos.egg-info/PKG-INFO
+-rw-r--r--   0 tim        (501) staff       (20)      454 2023-06-08 19:19:55.000000 dingdong_sonos-0.1.3/dingdong_sonos.egg-info/SOURCES.txt
+-rw-r--r--   0 tim        (501) staff       (20)        1 2023-06-08 19:19:55.000000 dingdong_sonos-0.1.3/dingdong_sonos.egg-info/dependency_links.txt
+-rw-r--r--   0 tim        (501) staff       (20)       54 2023-06-08 19:19:55.000000 dingdong_sonos-0.1.3/dingdong_sonos.egg-info/entry_points.txt
+-rw-r--r--   0 tim        (501) staff       (20)       47 2023-06-08 19:19:55.000000 dingdong_sonos-0.1.3/dingdong_sonos.egg-info/requires.txt
+-rw-r--r--   0 tim        (501) staff       (20)       15 2023-06-08 19:19:55.000000 dingdong_sonos-0.1.3/dingdong_sonos.egg-info/top_level.txt
+-rw-r--r--   0 tim        (501) staff       (20)     1110 2023-06-08 19:19:14.000000 dingdong_sonos-0.1.3/pyproject.toml
+-rw-r--r--   0 tim        (501) staff       (20)       38 2023-06-08 19:19:55.961039 dingdong_sonos-0.1.3/setup.cfg
```

### Comparing `dingdong_sonos-0.1.2/PKG-INFO` & `dingdong_sonos-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dingdong_sonos
-Version: 0.1.2
+Version: 0.1.3
 Summary: Ring the Gong
 Author-email: Tim Rohner <info@timrohner.ch>
 Project-URL: Source, https://github.com/leokster/dingdong_sonos
 Keywords: dingdong_sonos
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dingdong_sonos-0.1.2/dingdong_sonos/main.py` & `dingdong_sonos-0.1.3/dingdong_sonos/main.py`

 * *Files identical despite different names*

### Comparing `dingdong_sonos-0.1.2/dingdong_sonos/media/school-bell-sound.mp3` & `dingdong_sonos-0.1.3/dingdong_sonos/media/school-bell-sound.mp3`

 * *Files identical despite different names*

### Comparing `dingdong_sonos-0.1.2/dingdong_sonos.egg-info/PKG-INFO` & `dingdong_sonos-0.1.3/dingdong_sonos.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dingdong-sonos
-Version: 0.1.2
+Version: 0.1.3
 Summary: Ring the Gong
 Author-email: Tim Rohner <info@timrohner.ch>
 Project-URL: Source, https://github.com/leokster/dingdong_sonos
 Keywords: dingdong_sonos
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dingdong_sonos-0.1.2/pyproject.toml` & `dingdong_sonos-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "dingdong_sonos"
-version = "0.1.2"
+version = "0.1.3"
 description = "Ring the Gong"
 readme = "README.md"
 authors = [{name = "Tim Rohner", email = "info@timrohner.ch"}]
 keywords = ["dingdong_sonos"]
 # homepage = "https://github.com/leokster/dingdong_sonos"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
```

