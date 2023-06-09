# Comparing `tmp/KapoorLabs-Lightning-5.1.0.tar.gz` & `tmp/KapoorLabs-Lightning-5.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/c/Users/rando/Downloads/Python_Workspace/KapoorLabs-Lightning/dist/.tmp-w8gquhdx/KapoorLabs-Lightning-5.1.0.tar", last modified: Sat Jun  3 13:57:46 2023, max compression
+gzip compressed data, was "/mnt/c/Users/rando/Downloads/Python_Workspace/KapoorLabs-Lightning/dist/.tmp-rorsfp6o/KapoorLabs-Lightning-5.1.1.tar", last modified: Fri Jun  9 17:47:25 2023, max compression
```

## Comparing `KapoorLabs-Lightning-5.1.0.tar` & `KapoorLabs-Lightning-5.1.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-03 13:57:46.361976 KapoorLabs-Lightning-5.1.0/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-03 13:57:44.984099 KapoorLabs-Lightning-5.1.0/.github/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-03 13:57:45.231732 KapoorLabs-Lightning-5.1.0/.github/workflows/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2795 2023-05-15 12:36:30.000000 KapoorLabs-Lightning-5.1.0/.github/workflows/test_and_deploy.yml
--rwxrwxrwx   0 debian    (1000) debian    (1000)      991 2023-05-15 12:16:03.000000 KapoorLabs-Lightning-5.1.0/.gitignore
--rwxrwxrwx   0 debian    (1000) debian    (1000)      864 2023-05-15 12:16:19.000000 KapoorLabs-Lightning-5.1.0/.pre-commit-config.yaml
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1487 2023-05-15 12:16:03.000000 KapoorLabs-Lightning-5.1.0/LICENSE
--rwxrwxrwx   0 debian    (1000) debian    (1000)       96 2023-05-15 12:16:03.000000 KapoorLabs-Lightning-5.1.0/MANIFEST.in
--rwxrwxrwx   0 debian    (1000) debian    (1000)     3746 2023-06-03 13:57:46.363329 KapoorLabs-Lightning-5.1.0/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2435 2023-05-15 12:16:03.000000 KapoorLabs-Lightning-5.1.0/README.md
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-03 13:57:45.405348 KapoorLabs-Lightning-5.1.0/licenses/
--rwxrwxrwx   0 debian    (1000) debian    (1000)    11358 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.1.0/licenses/Apache-2
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1487 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.1.0/licenses/BSD-3
--rwxrwxrwx   0 debian    (1000) debian    (1000)    35148 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.1.0/licenses/GPL-3
--rwxrwxrwx   0 debian    (1000) debian    (1000)     7653 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.1.0/licenses/LGPL-3
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1080 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.1.0/licenses/MIT
--rwxrwxrwx   0 debian    (1000) debian    (1000)    16726 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.1.0/licenses/MPL-2
--rwxrwxrwx   0 debian    (1000) debian    (1000)      270 2023-05-15 12:16:03.000000 KapoorLabs-Lightning-5.1.0/pyproject.toml
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1734 2023-06-03 13:57:46.372376 KapoorLabs-Lightning-5.1.0/setup.cfg
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-03 13:57:45.008059 KapoorLabs-Lightning-5.1.0/src/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-03 13:57:45.637494 KapoorLabs-Lightning-5.1.0/src/KapoorLabs_Lightning.egg-info/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     3746 2023-06-03 13:57:43.000000 KapoorLabs-Lightning-5.1.0/src/KapoorLabs_Lightning.egg-info/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1157 2023-06-03 13:57:44.000000 KapoorLabs-Lightning-5.1.0/src/KapoorLabs_Lightning.egg-info/SOURCES.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-06-03 13:57:43.000000 KapoorLabs-Lightning-5.1.0/src/KapoorLabs_Lightning.egg-info/dependency_links.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       72 2023-06-03 13:57:43.000000 KapoorLabs-Lightning-5.1.0/src/KapoorLabs_Lightning.egg-info/entry_points.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       87 2023-06-03 13:57:43.000000 KapoorLabs-Lightning-5.1.0/src/KapoorLabs_Lightning.egg-info/requires.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       21 2023-06-03 13:57:43.000000 KapoorLabs-Lightning-5.1.0/src/KapoorLabs_Lightning.egg-info/top_level.txt
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-03 13:57:46.202700 KapoorLabs-Lightning-5.1.0/src/kapoorlabs_lightning/
--rwxrwxrwx   0 debian    (1000) debian    (1000)      859 2023-05-26 19:51:02.000000 KapoorLabs-Lightning-5.1.0/src/kapoorlabs_lightning/__init__.py
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-03 13:57:46.311787 KapoorLabs-Lightning-5.1.0/src/kapoorlabs_lightning/_tests/
--rwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-05-15 12:20:06.000000 KapoorLabs-Lightning-5.1.0/src/kapoorlabs_lightning/_tests/__init__.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     3106 2023-05-15 12:33:24.000000 KapoorLabs-Lightning-5.1.0/src/kapoorlabs_lightning/_tests/test_pytorch_models.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      160 2023-06-03 13:57:43.000000 KapoorLabs-Lightning-5.1.0/src/kapoorlabs_lightning/_version.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)       75 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.1.0/src/kapoorlabs_lightning/caped.yaml
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2065 2023-05-15 12:33:19.000000 KapoorLabs-Lightning-5.1.0/src/kapoorlabs_lightning/graph_functions.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)       68 2023-05-26 14:17:53.000000 KapoorLabs-Lightning-5.1.0/src/kapoorlabs_lightning/kapoorlabs.yaml
--rwxrwxrwx   0 debian    (1000) debian    (1000)    34411 2023-06-03 13:55:57.000000 KapoorLabs-Lightning-5.1.0/src/kapoorlabs_lightning/lightning_trainer.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     3537 2023-05-26 19:09:09.000000 KapoorLabs-Lightning-5.1.0/src/kapoorlabs_lightning/optimizers.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    15630 2023-05-27 20:24:35.000000 KapoorLabs-Lightning-5.1.0/src/kapoorlabs_lightning/pytorch_datasets.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     3801 2023-05-26 14:17:53.000000 KapoorLabs-Lightning-5.1.0/src/kapoorlabs_lightning/pytorch_loggers.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      762 2023-05-15 12:20:06.000000 KapoorLabs-Lightning-5.1.0/src/kapoorlabs_lightning/pytorch_losses.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    16569 2023-06-02 16:45:22.000000 KapoorLabs-Lightning-5.1.0/src/kapoorlabs_lightning/pytorch_models.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1809 2023-06-03 13:57:05.000000 KapoorLabs-Lightning-5.1.0/src/kapoorlabs_lightning/pytorch_transforms.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     3123 2023-05-15 12:33:24.000000 KapoorLabs-Lightning-5.1.0/src/kapoorlabs_lightning/schedulers.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      615 2023-05-15 12:16:03.000000 KapoorLabs-Lightning-5.1.0/tox.ini
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-09 17:47:25.437089 KapoorLabs-Lightning-5.1.1/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-09 17:47:24.473457 KapoorLabs-Lightning-5.1.1/.github/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-09 17:47:24.631779 KapoorLabs-Lightning-5.1.1/.github/workflows/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2795 2023-05-15 12:36:30.000000 KapoorLabs-Lightning-5.1.1/.github/workflows/test_and_deploy.yml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      991 2023-05-15 12:16:03.000000 KapoorLabs-Lightning-5.1.1/.gitignore
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      864 2023-05-15 12:16:19.000000 KapoorLabs-Lightning-5.1.1/.pre-commit-config.yaml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1487 2023-05-15 12:16:03.000000 KapoorLabs-Lightning-5.1.1/LICENSE
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       96 2023-05-15 12:16:03.000000 KapoorLabs-Lightning-5.1.1/MANIFEST.in
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     3746 2023-06-09 17:47:25.438096 KapoorLabs-Lightning-5.1.1/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2435 2023-05-15 12:16:03.000000 KapoorLabs-Lightning-5.1.1/README.md
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-09 17:47:24.796703 KapoorLabs-Lightning-5.1.1/licenses/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    11358 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.1.1/licenses/Apache-2
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1487 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.1.1/licenses/BSD-3
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    35148 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.1.1/licenses/GPL-3
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     7653 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.1.1/licenses/LGPL-3
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1080 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.1.1/licenses/MIT
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    16726 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.1.1/licenses/MPL-2
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      270 2023-05-15 12:16:03.000000 KapoorLabs-Lightning-5.1.1/pyproject.toml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1734 2023-06-09 17:47:25.443458 KapoorLabs-Lightning-5.1.1/setup.cfg
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-09 17:47:24.490638 KapoorLabs-Lightning-5.1.1/src/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-09 17:47:24.945895 KapoorLabs-Lightning-5.1.1/src/KapoorLabs_Lightning.egg-info/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     3746 2023-06-09 17:47:23.000000 KapoorLabs-Lightning-5.1.1/src/KapoorLabs_Lightning.egg-info/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1157 2023-06-09 17:47:24.000000 KapoorLabs-Lightning-5.1.1/src/KapoorLabs_Lightning.egg-info/SOURCES.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-06-09 17:47:23.000000 KapoorLabs-Lightning-5.1.1/src/KapoorLabs_Lightning.egg-info/dependency_links.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       72 2023-06-09 17:47:23.000000 KapoorLabs-Lightning-5.1.1/src/KapoorLabs_Lightning.egg-info/entry_points.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       87 2023-06-09 17:47:23.000000 KapoorLabs-Lightning-5.1.1/src/KapoorLabs_Lightning.egg-info/requires.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       21 2023-06-09 17:47:23.000000 KapoorLabs-Lightning-5.1.1/src/KapoorLabs_Lightning.egg-info/top_level.txt
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-09 17:47:25.334430 KapoorLabs-Lightning-5.1.1/src/kapoorlabs_lightning/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      859 2023-05-26 19:51:02.000000 KapoorLabs-Lightning-5.1.1/src/kapoorlabs_lightning/__init__.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-09 17:47:25.410187 KapoorLabs-Lightning-5.1.1/src/kapoorlabs_lightning/_tests/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-05-15 12:20:06.000000 KapoorLabs-Lightning-5.1.1/src/kapoorlabs_lightning/_tests/__init__.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     3106 2023-05-15 12:33:24.000000 KapoorLabs-Lightning-5.1.1/src/kapoorlabs_lightning/_tests/test_pytorch_models.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      160 2023-06-09 17:47:23.000000 KapoorLabs-Lightning-5.1.1/src/kapoorlabs_lightning/_version.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       75 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.1.1/src/kapoorlabs_lightning/caped.yaml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2065 2023-05-15 12:33:19.000000 KapoorLabs-Lightning-5.1.1/src/kapoorlabs_lightning/graph_functions.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       68 2023-05-26 14:17:53.000000 KapoorLabs-Lightning-5.1.1/src/kapoorlabs_lightning/kapoorlabs.yaml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    34543 2023-06-09 17:46:49.000000 KapoorLabs-Lightning-5.1.1/src/kapoorlabs_lightning/lightning_trainer.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     3537 2023-05-26 19:09:09.000000 KapoorLabs-Lightning-5.1.1/src/kapoorlabs_lightning/optimizers.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    15688 2023-06-05 14:50:17.000000 KapoorLabs-Lightning-5.1.1/src/kapoorlabs_lightning/pytorch_datasets.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     3801 2023-05-26 14:17:53.000000 KapoorLabs-Lightning-5.1.1/src/kapoorlabs_lightning/pytorch_loggers.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      762 2023-05-15 12:20:06.000000 KapoorLabs-Lightning-5.1.1/src/kapoorlabs_lightning/pytorch_losses.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    16569 2023-06-02 16:45:22.000000 KapoorLabs-Lightning-5.1.1/src/kapoorlabs_lightning/pytorch_models.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1809 2023-06-03 13:57:05.000000 KapoorLabs-Lightning-5.1.1/src/kapoorlabs_lightning/pytorch_transforms.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     3123 2023-05-15 12:33:24.000000 KapoorLabs-Lightning-5.1.1/src/kapoorlabs_lightning/schedulers.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      615 2023-05-15 12:16:03.000000 KapoorLabs-Lightning-5.1.1/tox.ini
```

### Comparing `KapoorLabs-Lightning-5.1.0/.github/workflows/test_and_deploy.yml` & `KapoorLabs-Lightning-5.1.1/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.1.0/.gitignore` & `KapoorLabs-Lightning-5.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.1.0/.pre-commit-config.yaml` & `KapoorLabs-Lightning-5.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.1.0/LICENSE` & `KapoorLabs-Lightning-5.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.1.0/PKG-INFO` & `KapoorLabs-Lightning-5.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KapoorLabs-Lightning
-Version: 5.1.0
+Version: 5.1.1
 Summary: Lightning modules for KapoorLabs specific projects
 Home-page: https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning
 Author: Varun Kapoor
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning#README.md
```

### Comparing `KapoorLabs-Lightning-5.1.0/README.md` & `KapoorLabs-Lightning-5.1.1/README.md`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.1.0/licenses/Apache-2` & `KapoorLabs-Lightning-5.1.1/licenses/Apache-2`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.1.0/licenses/BSD-3` & `KapoorLabs-Lightning-5.1.1/licenses/BSD-3`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.1.0/licenses/GPL-3` & `KapoorLabs-Lightning-5.1.1/licenses/GPL-3`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.1.0/licenses/LGPL-3` & `KapoorLabs-Lightning-5.1.1/licenses/LGPL-3`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.1.0/licenses/MIT` & `KapoorLabs-Lightning-5.1.1/licenses/MIT`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.1.0/licenses/MPL-2` & `KapoorLabs-Lightning-5.1.1/licenses/MPL-2`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.1.0/setup.cfg` & `KapoorLabs-Lightning-5.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.1.0/src/KapoorLabs_Lightning.egg-info/PKG-INFO` & `KapoorLabs-Lightning-5.1.1/src/KapoorLabs_Lightning.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KapoorLabs-Lightning
-Version: 5.1.0
+Version: 5.1.1
 Summary: Lightning modules for KapoorLabs specific projects
 Home-page: https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning
 Author: Varun Kapoor
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning#README.md
```

### Comparing `KapoorLabs-Lightning-5.1.0/src/KapoorLabs_Lightning.egg-info/SOURCES.txt` & `KapoorLabs-Lightning-5.1.1/src/KapoorLabs_Lightning.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.1.0/src/kapoorlabs_lightning/__init__.py` & `KapoorLabs-Lightning-5.1.1/src/kapoorlabs_lightning/__init__.py`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.1.0/src/kapoorlabs_lightning/_tests/test_pytorch_models.py` & `KapoorLabs-Lightning-5.1.1/src/kapoorlabs_lightning/_tests/test_pytorch_models.py`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.1.0/src/kapoorlabs_lightning/graph_functions.py` & `KapoorLabs-Lightning-5.1.1/src/kapoorlabs_lightning/graph_functions.py`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.1.0/src/kapoorlabs_lightning/lightning_trainer.py` & `KapoorLabs-Lightning-5.1.1/src/kapoorlabs_lightning/lightning_trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 from collections import OrderedDict
 from pathlib import Path
 from typing import List
 
 import torch
+import torch.nn.functional as F
 from lightning import Callback, LightningDataModule, LightningModule, Trainer
 from lightning.pytorch.loggers.logger import Logger
 from lightning.pytorch.utilities.types import STEP_OUTPUT
 from sklearn.cluster import KMeans
 from torch import optim
 from torch.utils.data import DataLoader, Dataset, random_split
 
@@ -401,15 +402,17 @@
     def forward(self, z):
         return self.network(z)
 
     def encoder_loss(self, y_hat, y):
         return self.loss_func(y_hat, y)
 
     def cluster_loss(self, clusters, tar_dist):
-        return self.cluster_loss_func(torch.log(clusters), tar_dist)
+        return self.cluster_loss_func(
+            F.log_softmax(clusters), F.softmax(tar_dist)
+        )
 
     def training_step(self, batch, batch_idx):
         self.compute_device = batch.device
         self.to(self.compute_device)
         self.target_distribution = self._get_target_distribution(
             self.cluster_distribution
         )
@@ -446,15 +449,18 @@
             sync_dist=True,
             rank_zero_only=True,
         )
 
         return output
 
     def on_train_epoch_end(self) -> None:
-        if self.current_epoch % self.update_interval == 0:
+        if (
+            self.current_epoch > 0
+            and self.current_epoch % self.update_interval == 0
+        ):
             net, cluster_distribution = initialize_repeat_function(
                 self.network,
                 self.loss_func,
                 self.cluster_loss_func,
                 self.train_dataloaders_inf,
                 self.optim_func,
                 self.gamma,
```

### Comparing `KapoorLabs-Lightning-5.1.0/src/kapoorlabs_lightning/optimizers.py` & `KapoorLabs-Lightning-5.1.1/src/kapoorlabs_lightning/optimizers.py`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.1.0/src/kapoorlabs_lightning/pytorch_datasets.py` & `KapoorLabs-Lightning-5.1.1/src/kapoorlabs_lightning/pytorch_datasets.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,18 +10,19 @@
 from pyntcloud import PyntCloud
 from sklearn import preprocessing
 from sklearn.decomposition import PCA
 from torch.utils.data import Dataset
 
 
 class PointCloudDataset(Dataset):
-    def __init__(self, points_dir, centre=True, scale=20.0):
+    def __init__(self, points_dir, centre=True, scale_z=1.0, scale_xy=1.0):
         self.points_dir = points_dir
         self.centre = centre
-        self.scale = scale
+        self.scale_z = scale_z
+        self.scale_xy = scale_xy
         self.p = Path(self.points_dir)
         self.files = list(self.p.glob("**/*.ply"))
 
     def __len__(self):
         return len(self.files)
 
     def __getitem__(self, idx):
@@ -29,22 +30,22 @@
         file = self.files[idx]
         point_cloud = PyntCloud.from_file(str(file))
         mean = 0
         point_cloud = torch.tensor(point_cloud.points.values)
         if self.centre:
             mean = torch.mean(point_cloud, 0)
 
-        scale = torch.tensor([[self.scale, self.scale, self.scale]])
+        scale = torch.tensor([[self.scale_z, self.scale_xy, self.scale_xy]])
         point_cloud = (point_cloud - mean) / scale
 
         return point_cloud
 
 
 class PointCloudNpzDataset(Dataset):
-    def __init__(self, npz_path, centre=True, scale=20.0):
+    def __init__(self, npz_path, centre=True, scale=1.0):
         self.npz_path = npz_path
         self.centre = centre
         self.scale = scale
         self.npzdata = np.load(npz_path)
         self.mesh_data = self.npzdata["mesh"].tolist()
         self.points_data = self.npzdata["points"].tolist()
 
@@ -456,15 +457,15 @@
 
         serial_number = self.new_df.loc[idx, "serialNumber"]
 
         return image, treatment, u, serial_number
 
 
 class VesselMNIST3D(Dataset):
-    def __init__(self, points_dir, centre=True, scale=20.0, partition="train"):
+    def __init__(self, points_dir, centre=True, scale=1.0, partition="train"):
         self.points_dir = points_dir
         self.centre = centre
         self.scale = scale
         self.p = Path(self.points_dir)
         self.partition = partition
         self.path = self.p / partition
         self.files = list(self.path.glob("**/*.ply"))
```

### Comparing `KapoorLabs-Lightning-5.1.0/src/kapoorlabs_lightning/pytorch_loggers.py` & `KapoorLabs-Lightning-5.1.1/src/kapoorlabs_lightning/pytorch_loggers.py`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.1.0/src/kapoorlabs_lightning/pytorch_losses.py` & `KapoorLabs-Lightning-5.1.1/src/kapoorlabs_lightning/pytorch_losses.py`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.1.0/src/kapoorlabs_lightning/pytorch_models.py` & `KapoorLabs-Lightning-5.1.1/src/kapoorlabs_lightning/pytorch_models.py`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.1.0/src/kapoorlabs_lightning/pytorch_transforms.py` & `KapoorLabs-Lightning-5.1.1/src/kapoorlabs_lightning/pytorch_transforms.py`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.1.0/src/kapoorlabs_lightning/schedulers.py` & `KapoorLabs-Lightning-5.1.1/src/kapoorlabs_lightning/schedulers.py`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.1.0/tox.ini` & `KapoorLabs-Lightning-5.1.1/tox.ini`

 * *Files identical despite different names*

