# Comparing `tmp/redflagbpm-0.0.8.tar.gz` & `tmp/redflagbpm-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redflagbpm-0.0.8.tar", last modified: Tue Sep  6 16:54:21 2022, max compression
+gzip compressed data, was "redflagbpm-0.0.9.tar", last modified: Tue Sep  6 17:08:42 2022, max compression
```

## Comparing `redflagbpm-0.0.8.tar` & `redflagbpm-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 gdressino  (1000) gdressino  (1000)        0 2022-09-06 16:54:21.875643 redflagbpm-0.0.8/
--rw-rw-r--   0 gdressino  (1000) gdressino  (1000)     1068 2022-06-04 18:30:39.000000 redflagbpm-0.0.8/LICENCE
--rw-rw-r--   0 gdressino  (1000) gdressino  (1000)      547 2022-09-06 16:54:21.875643 redflagbpm-0.0.8/PKG-INFO
--rw-rw-r--   0 gdressino  (1000) gdressino  (1000)       29 2022-06-04 18:30:39.000000 redflagbpm-0.0.8/README.md
--rw-rw-r--   0 gdressino  (1000) gdressino  (1000)       86 2022-06-04 18:30:39.000000 redflagbpm-0.0.8/pyproject.toml
--rw-rw-r--   0 gdressino  (1000) gdressino  (1000)       38 2022-09-06 16:54:21.875643 redflagbpm-0.0.8/setup.cfg
--rw-rw-r--   0 gdressino  (1000) gdressino  (1000)      865 2022-09-06 16:54:10.000000 redflagbpm-0.0.8/setup.py
-drwxrwxr-x   0 gdressino  (1000) gdressino  (1000)        0 2022-09-06 16:54:21.871643 redflagbpm-0.0.8/src/
-drwxrwxr-x   0 gdressino  (1000) gdressino  (1000)        0 2022-09-06 16:54:21.871643 redflagbpm-0.0.8/src/redflagbpm/
--rw-rw-r--   0 gdressino  (1000) gdressino  (1000)     5061 2022-09-06 16:53:19.000000 redflagbpm-0.0.8/src/redflagbpm/BPMService.py
--rw-rw-r--   0 gdressino  (1000) gdressino  (1000)    14286 2022-08-23 20:37:45.000000 redflagbpm-0.0.8/src/redflagbpm/Services.py
--rw-rw-r--   0 gdressino  (1000) gdressino  (1000)      499 2022-08-09 15:16:53.000000 redflagbpm-0.0.8/src/redflagbpm/__init__.py
-drwxrwxr-x   0 gdressino  (1000) gdressino  (1000)        0 2022-09-06 16:54:21.875643 redflagbpm-0.0.8/src/redflagbpm.egg-info/
--rw-rw-r--   0 gdressino  (1000) gdressino  (1000)      547 2022-09-06 16:54:21.000000 redflagbpm-0.0.8/src/redflagbpm.egg-info/PKG-INFO
--rw-rw-r--   0 gdressino  (1000) gdressino  (1000)      313 2022-09-06 16:54:21.000000 redflagbpm-0.0.8/src/redflagbpm.egg-info/SOURCES.txt
--rw-rw-r--   0 gdressino  (1000) gdressino  (1000)        1 2022-09-06 16:54:21.000000 redflagbpm-0.0.8/src/redflagbpm.egg-info/dependency_links.txt
--rw-rw-r--   0 gdressino  (1000) gdressino  (1000)       22 2022-09-06 16:54:21.000000 redflagbpm-0.0.8/src/redflagbpm.egg-info/requires.txt
--rw-rw-r--   0 gdressino  (1000) gdressino  (1000)       11 2022-09-06 16:54:21.000000 redflagbpm-0.0.8/src/redflagbpm.egg-info/top_level.txt
+drwxrwxr-x   0 gdressino  (1000) gdressino  (1000)        0 2022-09-06 17:08:42.548104 redflagbpm-0.0.9/
+-rw-rw-r--   0 gdressino  (1000) gdressino  (1000)     1068 2022-06-04 18:30:39.000000 redflagbpm-0.0.9/LICENCE
+-rw-rw-r--   0 gdressino  (1000) gdressino  (1000)      547 2022-09-06 17:08:42.548104 redflagbpm-0.0.9/PKG-INFO
+-rw-rw-r--   0 gdressino  (1000) gdressino  (1000)       29 2022-06-04 18:30:39.000000 redflagbpm-0.0.9/README.md
+-rw-rw-r--   0 gdressino  (1000) gdressino  (1000)       86 2022-06-04 18:30:39.000000 redflagbpm-0.0.9/pyproject.toml
+-rw-rw-r--   0 gdressino  (1000) gdressino  (1000)       38 2022-09-06 17:08:42.548104 redflagbpm-0.0.9/setup.cfg
+-rw-rw-r--   0 gdressino  (1000) gdressino  (1000)      865 2022-09-06 17:08:33.000000 redflagbpm-0.0.9/setup.py
+drwxrwxr-x   0 gdressino  (1000) gdressino  (1000)        0 2022-09-06 17:08:42.544103 redflagbpm-0.0.9/src/
+drwxrwxr-x   0 gdressino  (1000) gdressino  (1000)        0 2022-09-06 17:08:42.548104 redflagbpm-0.0.9/src/redflagbpm/
+-rw-rw-r--   0 gdressino  (1000) gdressino  (1000)     5061 2022-09-06 16:53:19.000000 redflagbpm-0.0.9/src/redflagbpm/BPMService.py
+-rw-rw-r--   0 gdressino  (1000) gdressino  (1000)    14285 2022-09-06 17:07:26.000000 redflagbpm-0.0.9/src/redflagbpm/Services.py
+-rw-rw-r--   0 gdressino  (1000) gdressino  (1000)      499 2022-08-09 15:16:53.000000 redflagbpm-0.0.9/src/redflagbpm/__init__.py
+drwxrwxr-x   0 gdressino  (1000) gdressino  (1000)        0 2022-09-06 17:08:42.548104 redflagbpm-0.0.9/src/redflagbpm.egg-info/
+-rw-rw-r--   0 gdressino  (1000) gdressino  (1000)      547 2022-09-06 17:08:42.000000 redflagbpm-0.0.9/src/redflagbpm.egg-info/PKG-INFO
+-rw-rw-r--   0 gdressino  (1000) gdressino  (1000)      313 2022-09-06 17:08:42.000000 redflagbpm-0.0.9/src/redflagbpm.egg-info/SOURCES.txt
+-rw-rw-r--   0 gdressino  (1000) gdressino  (1000)        1 2022-09-06 17:08:42.000000 redflagbpm-0.0.9/src/redflagbpm.egg-info/dependency_links.txt
+-rw-rw-r--   0 gdressino  (1000) gdressino  (1000)       22 2022-09-06 17:08:42.000000 redflagbpm-0.0.9/src/redflagbpm.egg-info/requires.txt
+-rw-rw-r--   0 gdressino  (1000) gdressino  (1000)       11 2022-09-06 17:08:42.000000 redflagbpm-0.0.9/src/redflagbpm.egg-info/top_level.txt
```

### Comparing `redflagbpm-0.0.8/LICENCE` & `redflagbpm-0.0.9/LICENCE`

 * *Files identical despite different names*

### Comparing `redflagbpm-0.0.8/PKG-INFO` & `redflagbpm-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redflagbpm
-Version: 0.0.8
+Version: 0.0.9
 Summary: BPM service extension
 Home-page: https://gitlab.com/redflagdev/redflagbpm-python
 Author: Germán Dressino
 Author-email: gdressino@redflag.dev
 Project-URL: Bug Tracker, https://gitlab.com/redflagdev/redflagbpm-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `redflagbpm-0.0.8/setup.py` & `redflagbpm-0.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="redflagbpm",
-    version="0.0.8",
+    version="0.0.9",
     author="Germán Dressino",
     author_email="gdressino@redflag.dev",
     description="BPM service extension",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/redflagdev/redflagbpm-python",
     project_urls={
```

### Comparing `redflagbpm-0.0.8/src/redflagbpm/BPMService.py` & `redflagbpm-0.0.9/src/redflagbpm/BPMService.py`

 * *Files identical despite different names*

### Comparing `redflagbpm-0.0.8/src/redflagbpm/Services.py` & `redflagbpm-0.0.9/src/redflagbpm/Services.py`

 * *Files 0% similar despite different names*

```diff
@@ -301,8 +301,7 @@
         return self.bpm.call("EBHBPMRuntime.setVariable",
                              body={"executionId": process_instance_id, "variableName": variableName, "value": value})
 
     def removeVariable(self, variableName: str):
         process_instance_id = self.bpm.context.getValue('execution.getProcessInstanceId()')
         self.bpm.call("EBHBPMRuntime.removeVariable",
                       body={"executionId": process_instance_id, "variableName": variableName})
-.
```

### Comparing `redflagbpm-0.0.8/src/redflagbpm.egg-info/PKG-INFO` & `redflagbpm-0.0.9/src/redflagbpm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redflagbpm
-Version: 0.0.8
+Version: 0.0.9
 Summary: BPM service extension
 Home-page: https://gitlab.com/redflagdev/redflagbpm-python
 Author: Germán Dressino
 Author-email: gdressino@redflag.dev
 Project-URL: Bug Tracker, https://gitlab.com/redflagdev/redflagbpm-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

