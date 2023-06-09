# Comparing `tmp/skysurvey-0.5.3.tar.gz` & `tmp/skysurvey-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skysurvey-0.5.3.tar", last modified: Fri Jun  9 12:15:22 2023, max compression
+gzip compressed data, was "skysurvey-0.5.4.tar", last modified: Fri Jun  9 12:17:52 2023, max compression
```

## Comparing `skysurvey-0.5.3.tar` & `skysurvey-0.5.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-06-09 12:15:22.987211 skysurvey-0.5.3/
--rw-r--r--   0 rigault   (2358) staff       (20)    11357 2022-08-10 14:40:58.000000 skysurvey-0.5.3/LICENSE
--rw-r--r--   0 rigault   (2358) staff       (20)      257 2023-06-09 12:15:22.986528 skysurvey-0.5.3/PKG-INFO
--rw-r--r--   0 rigault   (2358) staff       (20)     2333 2022-09-14 19:00:29.000000 skysurvey-0.5.3/README.md
--rw-r--r--   0 rigault   (2358) staff       (20)       38 2023-06-09 12:15:22.987267 skysurvey-0.5.3/setup.cfg
--rw-r--r--   0 rigault   (2358) staff       (20)      560 2023-06-09 12:15:18.000000 skysurvey-0.5.3/setup.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-06-09 12:15:22.984296 skysurvey-0.5.3/skysurvey/
--rw-r--r--   0 rigault   (2358) staff       (20)       92 2023-06-09 12:15:13.000000 skysurvey-0.5.3/skysurvey/__init__.py
--rw-r--r--   0 rigault   (2358) staff       (20)      398 2022-08-16 14:00:03.000000 skysurvey-0.5.3/skysurvey/config.py
--rw-r--r--   0 rigault   (2358) staff       (20)        0 2023-06-02 08:51:15.000000 skysurvey-0.5.3/skysurvey/dag.py
--rw-r--r--   0 rigault   (2358) staff       (20)    27023 2023-06-02 14:37:50.000000 skysurvey-0.5.3/skysurvey/dataset.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-06-09 12:15:22.985302 skysurvey-0.5.3/skysurvey/survey/
--rw-r--r--   0 rigault   (2358) staff       (20)      101 2022-09-17 12:56:09.000000 skysurvey-0.5.3/skysurvey/survey/__init__.py
--rw-r--r--   0 rigault   (2358) staff       (20)     8645 2023-05-02 20:15:06.000000 skysurvey-0.5.3/skysurvey/survey/core.py
--rw-r--r--   0 rigault   (2358) staff       (20)    10970 2023-06-02 10:03:36.000000 skysurvey-0.5.3/skysurvey/survey/healpix.py
--rw-r--r--   0 rigault   (2358) staff       (20)     5306 2022-12-17 16:44:36.000000 skysurvey-0.5.3/skysurvey/survey/polygon.py
--rw-r--r--   0 rigault   (2358) staff       (20)     1698 2022-12-20 11:13:58.000000 skysurvey-0.5.3/skysurvey/survey/ztf.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-06-09 12:15:22.986349 skysurvey-0.5.3/skysurvey/target/
--rw-r--r--   0 rigault   (2358) staff       (20)      113 2023-05-05 08:46:40.000000 skysurvey-0.5.3/skysurvey/target/__init__.py
--rw-r--r--   0 rigault   (2358) staff       (20)    11766 2023-05-05 08:45:44.000000 skysurvey-0.5.3/skysurvey/target/collection.py
--rw-r--r--   0 rigault   (2358) staff       (20)    31327 2023-06-02 09:43:01.000000 skysurvey-0.5.3/skysurvey/target/core.py
--rw-r--r--   0 rigault   (2358) staff       (20)      391 2022-10-06 08:31:16.000000 skysurvey-0.5.3/skysurvey/target/environments.py
--rw-r--r--   0 rigault   (2358) staff       (20)      165 2022-09-17 13:52:22.000000 skysurvey-0.5.3/skysurvey/target/kilonova.py
--rw-r--r--   0 rigault   (2358) staff       (20)     2343 2023-06-03 15:35:55.000000 skysurvey-0.5.3/skysurvey/target/sncc.py
--rw-r--r--   0 rigault   (2358) staff       (20)    10070 2023-06-02 09:06:49.000000 skysurvey-0.5.3/skysurvey/target/snia.py
--rw-r--r--   0 rigault   (2358) staff       (20)      681 2023-06-02 09:01:21.000000 skysurvey-0.5.3/skysurvey/target/stars.py
--rw-r--r--   0 rigault   (2358) staff       (20)     6386 2023-06-02 09:51:33.000000 skysurvey-0.5.3/skysurvey/target/timeserie.py
--rw-r--r--   0 rigault   (2358) staff       (20)    16507 2023-05-26 07:31:27.000000 skysurvey-0.5.3/skysurvey/template.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-06-09 12:15:22.984760 skysurvey-0.5.3/skysurvey.egg-info/
--rw-r--r--   0 rigault   (2358) staff       (20)      257 2023-06-09 12:15:22.000000 skysurvey-0.5.3/skysurvey.egg-info/PKG-INFO
--rw-r--r--   0 rigault   (2358) staff       (20)      647 2023-06-09 12:15:22.000000 skysurvey-0.5.3/skysurvey.egg-info/SOURCES.txt
--rw-r--r--   0 rigault   (2358) staff       (20)        1 2023-06-09 12:15:22.000000 skysurvey-0.5.3/skysurvey.egg-info/dependency_links.txt
--rw-r--r--   0 rigault   (2358) staff       (20)       10 2023-06-09 12:15:22.000000 skysurvey-0.5.3/skysurvey.egg-info/top_level.txt
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-06-09 12:17:52.957710 skysurvey-0.5.4/
+-rw-r--r--   0 rigault   (2358) staff       (20)    11357 2022-08-10 14:40:58.000000 skysurvey-0.5.4/LICENSE
+-rw-r--r--   0 rigault   (2358) staff       (20)      257 2023-06-09 12:17:52.957531 skysurvey-0.5.4/PKG-INFO
+-rw-r--r--   0 rigault   (2358) staff       (20)     2333 2022-09-14 19:00:29.000000 skysurvey-0.5.4/README.md
+-rw-r--r--   0 rigault   (2358) staff       (20)       38 2023-06-09 12:17:52.957769 skysurvey-0.5.4/setup.cfg
+-rw-r--r--   0 rigault   (2358) staff       (20)      560 2023-06-09 12:17:44.000000 skysurvey-0.5.4/setup.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-06-09 12:17:52.955035 skysurvey-0.5.4/skysurvey/
+-rw-r--r--   0 rigault   (2358) staff       (20)       92 2023-06-09 12:17:39.000000 skysurvey-0.5.4/skysurvey/__init__.py
+-rw-r--r--   0 rigault   (2358) staff       (20)      398 2022-08-16 14:00:03.000000 skysurvey-0.5.4/skysurvey/config.py
+-rw-r--r--   0 rigault   (2358) staff       (20)        0 2023-06-02 08:51:15.000000 skysurvey-0.5.4/skysurvey/dag.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    27022 2023-06-09 12:17:31.000000 skysurvey-0.5.4/skysurvey/dataset.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-06-09 12:17:52.956115 skysurvey-0.5.4/skysurvey/survey/
+-rw-r--r--   0 rigault   (2358) staff       (20)      101 2022-09-17 12:56:09.000000 skysurvey-0.5.4/skysurvey/survey/__init__.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     8645 2023-05-02 20:15:06.000000 skysurvey-0.5.4/skysurvey/survey/core.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    10970 2023-06-02 10:03:36.000000 skysurvey-0.5.4/skysurvey/survey/healpix.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     5306 2022-12-17 16:44:36.000000 skysurvey-0.5.4/skysurvey/survey/polygon.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     1698 2022-12-20 11:13:58.000000 skysurvey-0.5.4/skysurvey/survey/ztf.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-06-09 12:17:52.957360 skysurvey-0.5.4/skysurvey/target/
+-rw-r--r--   0 rigault   (2358) staff       (20)      113 2023-05-05 08:46:40.000000 skysurvey-0.5.4/skysurvey/target/__init__.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    11766 2023-05-05 08:45:44.000000 skysurvey-0.5.4/skysurvey/target/collection.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    31327 2023-06-02 09:43:01.000000 skysurvey-0.5.4/skysurvey/target/core.py
+-rw-r--r--   0 rigault   (2358) staff       (20)      391 2022-10-06 08:31:16.000000 skysurvey-0.5.4/skysurvey/target/environments.py
+-rw-r--r--   0 rigault   (2358) staff       (20)      165 2022-09-17 13:52:22.000000 skysurvey-0.5.4/skysurvey/target/kilonova.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     2343 2023-06-03 15:35:55.000000 skysurvey-0.5.4/skysurvey/target/sncc.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    10070 2023-06-02 09:06:49.000000 skysurvey-0.5.4/skysurvey/target/snia.py
+-rw-r--r--   0 rigault   (2358) staff       (20)      681 2023-06-02 09:01:21.000000 skysurvey-0.5.4/skysurvey/target/stars.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     6386 2023-06-02 09:51:33.000000 skysurvey-0.5.4/skysurvey/target/timeserie.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    16507 2023-05-26 07:31:27.000000 skysurvey-0.5.4/skysurvey/template.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-06-09 12:17:52.955519 skysurvey-0.5.4/skysurvey.egg-info/
+-rw-r--r--   0 rigault   (2358) staff       (20)      257 2023-06-09 12:17:52.000000 skysurvey-0.5.4/skysurvey.egg-info/PKG-INFO
+-rw-r--r--   0 rigault   (2358) staff       (20)      647 2023-06-09 12:17:52.000000 skysurvey-0.5.4/skysurvey.egg-info/SOURCES.txt
+-rw-r--r--   0 rigault   (2358) staff       (20)        1 2023-06-09 12:17:52.000000 skysurvey-0.5.4/skysurvey.egg-info/dependency_links.txt
+-rw-r--r--   0 rigault   (2358) staff       (20)       10 2023-06-09 12:17:52.000000 skysurvey-0.5.4/skysurvey.egg-info/top_level.txt
```

### Comparing `skysurvey-0.5.3/LICENSE` & `skysurvey-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `skysurvey-0.5.3/README.md` & `skysurvey-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `skysurvey-0.5.3/setup.py` & `skysurvey-0.5.4/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 """
 from distutils.core import setup
 from setuptools import setup, find_packages
 
 
 packages = find_packages()
 
-VERSION = '0.5.3'
+VERSION = '0.5.4'
         
 setup(name='skysurvey',
       version=VERSION,
       description='Simulating Transient in the sky and how to observe them',
       author='Mickael Rigault',
       author_email='m.rigault@ipnl.in2p3.fr',
       url='https://github.com/MickaelRigault/skysurvey',
```

### Comparing `skysurvey-0.5.3/skysurvey/dataset.py` & `skysurvey-0.5.4/skysurvey/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -282,15 +282,15 @@
             if t0 is None:
                 t0 = self.targets.data["t0"].copy()
             
             data["phase"] = data["time"] - t0.reindex(data.index, level=0)
             data = data[data["phase"].between(*phase_range)]
 
         if detected is not None:
-            data["detection"] = data["flux"]/data["fluxerr"])
+            data["detection"] = data["flux"]/data["fluxerr"]
             if detected:
                 data = data[ data["detection"] ] > detlimit
             else:
                 data = data[ data["detection"] ] <= detlimit
 
         return data
```

### Comparing `skysurvey-0.5.3/skysurvey/survey/core.py` & `skysurvey-0.5.4/skysurvey/survey/core.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.5.3/skysurvey/survey/healpix.py` & `skysurvey-0.5.4/skysurvey/survey/healpix.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.5.3/skysurvey/survey/polygon.py` & `skysurvey-0.5.4/skysurvey/survey/polygon.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.5.3/skysurvey/survey/ztf.py` & `skysurvey-0.5.4/skysurvey/survey/ztf.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.5.3/skysurvey/target/collection.py` & `skysurvey-0.5.4/skysurvey/target/collection.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.5.3/skysurvey/target/core.py` & `skysurvey-0.5.4/skysurvey/target/core.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.5.3/skysurvey/target/sncc.py` & `skysurvey-0.5.4/skysurvey/target/sncc.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.5.3/skysurvey/target/snia.py` & `skysurvey-0.5.4/skysurvey/target/snia.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.5.3/skysurvey/target/stars.py` & `skysurvey-0.5.4/skysurvey/target/stars.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.5.3/skysurvey/target/timeserie.py` & `skysurvey-0.5.4/skysurvey/target/timeserie.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.5.3/skysurvey/template.py` & `skysurvey-0.5.4/skysurvey/template.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.5.3/skysurvey.egg-info/SOURCES.txt` & `skysurvey-0.5.4/skysurvey.egg-info/SOURCES.txt`

 * *Files identical despite different names*

