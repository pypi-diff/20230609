# Comparing `tmp/MDRMF-0.0.3.tar.gz` & `tmp/MDRMF-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MDRMF-0.0.3.tar", last modified: Tue Jun  6 17:41:25 2023, max compression
+gzip compressed data, was "MDRMF-0.0.4.tar", last modified: Fri Jun  9 09:54:47 2023, max compression
```

## Comparing `MDRMF-0.0.3.tar` & `MDRMF-0.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 17:41:25.994315 MDRMF-0.0.3/
-drwxrwxrwx   0        0        0        0 2023-06-06 17:41:25.946315 MDRMF-0.0.3/MDRMF/
--rw-rw-rw-   0        0        0      284 2023-06-06 17:40:38.000000 MDRMF-0.0.3/MDRMF/__init__.py
--rw-rw-rw-   0        0        0     3839 2023-06-06 07:35:43.000000 MDRMF-0.0.3/MDRMF/dataset.py
--rw-rw-rw-   0        0        0     2002 2023-06-02 06:30:06.000000 MDRMF-0.0.3/MDRMF/evaluator.py
--rw-rw-rw-   0        0        0     6928 2023-06-06 17:32:00.000000 MDRMF-0.0.3/MDRMF/experimenter.py
--rw-rw-rw-   0        0        0     3808 2023-06-02 13:46:50.000000 MDRMF-0.0.3/MDRMF/featurizer.py
--rw-rw-rw-   0        0        0     1727 2023-06-06 08:00:32.000000 MDRMF-0.0.3/MDRMF/model.py
-drwxrwxrwx   0        0        0        0 2023-06-06 17:41:25.989311 MDRMF-0.0.3/MDRMF/models/
--rw-rw-rw-   0        0        0       86 2023-05-23 10:56:06.000000 MDRMF-0.0.3/MDRMF/models/__init__.py
--rw-rw-rw-   0        0        0     3950 2023-06-06 07:36:51.000000 MDRMF-0.0.3/MDRMF/models/modeller.py
--rw-rw-rw-   0        0        0     3634 2023-06-06 17:37:35.000000 MDRMF-0.0.3/MDRMF/models/rfmodeller.py
--rw-rw-rw-   0        0        0     2643 2023-06-02 14:00:31.000000 MDRMF-0.0.3/MDRMF/moleculeloader.py
-drwxrwxrwx   0        0        0        0 2023-06-06 17:41:25.974316 MDRMF-0.0.3/MDRMF.egg-info/
--rw-rw-rw-   0        0        0      436 2023-06-06 17:41:25.000000 MDRMF-0.0.3/MDRMF.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      346 2023-06-06 17:41:25.000000 MDRMF-0.0.3/MDRMF.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 17:41:25.000000 MDRMF-0.0.3/MDRMF.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-06 17:41:25.000000 MDRMF-0.0.3/MDRMF.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      436 2023-06-06 17:41:25.993317 MDRMF-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      172 2023-05-11 07:27:32.000000 MDRMF-0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-06-06 17:41:25.995314 MDRMF-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      553 2023-06-05 18:45:57.000000 MDRMF-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 09:54:47.023737 MDRMF-0.0.4/
+drwxrwxrwx   0        0        0        0 2023-06-09 09:54:46.978728 MDRMF-0.0.4/MDRMF/
+-rw-rw-rw-   0        0        0      284 2023-06-09 09:54:16.000000 MDRMF-0.0.4/MDRMF/__init__.py
+-rw-rw-rw-   0        0        0     3839 2023-06-06 07:35:43.000000 MDRMF-0.0.4/MDRMF/dataset.py
+-rw-rw-rw-   0        0        0     2002 2023-06-02 06:30:06.000000 MDRMF-0.0.4/MDRMF/evaluator.py
+-rw-rw-rw-   0        0        0     7639 2023-06-09 08:07:30.000000 MDRMF-0.0.4/MDRMF/experimenter.py
+-rw-rw-rw-   0        0        0     3808 2023-06-02 13:46:50.000000 MDRMF-0.0.4/MDRMF/featurizer.py
+-rw-rw-rw-   0        0        0     1727 2023-06-06 08:00:32.000000 MDRMF-0.0.4/MDRMF/model.py
+drwxrwxrwx   0        0        0        0 2023-06-09 09:54:47.017723 MDRMF-0.0.4/MDRMF/models/
+-rw-rw-rw-   0        0        0       86 2023-05-23 10:56:06.000000 MDRMF-0.0.4/MDRMF/models/__init__.py
+-rw-rw-rw-   0        0        0     3950 2023-06-06 07:36:51.000000 MDRMF-0.0.4/MDRMF/models/modeller.py
+-rw-rw-rw-   0        0        0     3634 2023-06-06 17:37:35.000000 MDRMF-0.0.4/MDRMF/models/rfmodeller.py
+-rw-rw-rw-   0        0        0     2643 2023-06-02 14:00:31.000000 MDRMF-0.0.4/MDRMF/moleculeloader.py
+drwxrwxrwx   0        0        0        0 2023-06-09 09:54:47.004745 MDRMF-0.0.4/MDRMF.egg-info/
+-rw-rw-rw-   0        0        0      436 2023-06-09 09:54:46.000000 MDRMF-0.0.4/MDRMF.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      346 2023-06-09 09:54:46.000000 MDRMF-0.0.4/MDRMF.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 09:54:46.000000 MDRMF-0.0.4/MDRMF.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-09 09:54:46.000000 MDRMF-0.0.4/MDRMF.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      436 2023-06-09 09:54:47.020720 MDRMF-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      172 2023-05-11 07:27:32.000000 MDRMF-0.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-09 09:54:47.024746 MDRMF-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      553 2023-06-09 09:53:50.000000 MDRMF-0.0.4/setup.py
```

### Comparing `MDRMF-0.0.3/MDRMF/dataset.py` & `MDRMF-0.0.4/MDRMF/dataset.py`

 * *Files identical despite different names*

### Comparing `MDRMF-0.0.3/MDRMF/evaluator.py` & `MDRMF-0.0.4/MDRMF/evaluator.py`

 * *Files identical despite different names*

### Comparing `MDRMF-0.0.3/MDRMF/experimenter.py` & `MDRMF-0.0.4/MDRMF/experimenter.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,48 @@
 import yaml
 import os
 import pandas as pd
 import inspect
 import time
 import shutil
+import datetime
 from typing import List
 from MDRMF.evaluator import Evaluator
 import MDRMF.models as mfm
 from MDRMF import Dataset, MoleculeLoader, Featurizer, Model
 
 class Experimenter:
 
     def __init__(self, config_file: str):
         #self.config_file = config_file
-        #self.experiments = self._load_config()
 
         self.config_file = os.path.join(os.path.dirname(os.path.dirname(os.path.realpath(__file__))), config_file)
         self.experiments = self._load_config()
-        self.root_dir = "Experiment_Root"
+
+        # Generate ids
+        self.protocol_name = self.get_protocol_name()
+        id = self.generate_id(self.protocol_name)
 
         # Setting up root directory
+        self.root_dir = id
         os.makedirs(self.root_dir, exist_ok=True)
     
-        # Copy settings file to root dir
-        destination_file_path = os.path.join(self.root_dir, "settings.yaml")
-        shutil.copy(self.config_file, destination_file_path)
+        self.create_meta_data()
+
+    def get_protocol_name(self) -> str:
+        try:
+            return self.experiments[0][0]['Protocol_name']
+        except KeyError as exc:
+            return "protocol"
+
+    def generate_id(self, protocol_name: str) -> str:
+        current_time = datetime.datetime.now()
+        formatted_time = current_time.strftime('%y%m%d-%H%M%S')  # YYMMDD-HHMMSS
+        id = f"{protocol_name}-{formatted_time}"
+        return id
 
     def _load_config(self) -> List[dict]:
         with open(self.config_file, 'r') as stream:
             try:
                 config = yaml.safe_load(stream)
             except yaml.YAMLError as exc:
                 print(exc)
@@ -36,14 +50,22 @@
 
         # If there is only one experiment, make it into a list
         if isinstance(config, dict):
             config = [config]
 
         return [config]
     
+    def create_meta_data(self):
+        destination_file_path = os.path.join(self.root_dir, "settings.yaml")
+        shutil.copy(self.config_file, destination_file_path)
+
+        meta_destination = os.path.join(self.root_dir, "meta_data.txt")
+        with open(meta_destination, "w") as f:
+            f.write(self.root_dir)
+    
     def conduct_all_experiments(self):
 
         start_time = time.time()
  
         for config in self.experiments:
             for experiment in config:
                 key, value = list(experiment.items())[0]
```

### Comparing `MDRMF-0.0.3/MDRMF/featurizer.py` & `MDRMF-0.0.4/MDRMF/featurizer.py`

 * *Files identical despite different names*

### Comparing `MDRMF-0.0.3/MDRMF/model.py` & `MDRMF-0.0.4/MDRMF/model.py`

 * *Files identical despite different names*

### Comparing `MDRMF-0.0.3/MDRMF/models/modeller.py` & `MDRMF-0.0.4/MDRMF/models/modeller.py`

 * *Files identical despite different names*

### Comparing `MDRMF-0.0.3/MDRMF/models/rfmodeller.py` & `MDRMF-0.0.4/MDRMF/models/rfmodeller.py`

 * *Files identical despite different names*

### Comparing `MDRMF-0.0.3/MDRMF/moleculeloader.py` & `MDRMF-0.0.4/MDRMF/moleculeloader.py`

 * *Files identical despite different names*

### Comparing `MDRMF-0.0.3/setup.py` & `MDRMF-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name='MDRMF',
-    version='0.0.3',
+    version='0.0.4',
     packages=find_packages(),
     description='Multidrug Resistance Machine Fishing',
     author='Jacob Molin Nielsen',
     author_email='jacob.molin@me.com',
     url='https://github.com/MolinDiscovery/MDRMF',  # use the URL to the github repo
-    download_url='https://github.com/MolinDiscovery/MDRMF/archive/v0.0.3.tar.gz',
+    download_url='https://github.com/MolinDiscovery/MDRMF/archive/v0.0.4.tar.gz',
     keywords=['machine fishing', 'drug discovery', 'machine learning', 'pool based active learning'],
     classifiers=[],
 )
```

