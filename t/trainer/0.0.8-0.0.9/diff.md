# Comparing `tmp/trainer-0.0.8.tar.gz` & `tmp/trainer-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trainer-0.0.8.tar", last modified: Thu Apr 14 09:11:47 2022, max compression
+gzip compressed data, was "trainer-0.0.9.tar", last modified: Wed Apr 27 13:17:21 2022, max compression
```

## Comparing `trainer-0.0.8.tar` & `trainer-0.0.9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-14 09:11:47.454868 trainer-0.0.8/
--rw-r--r--   0 root         (0) root         (0)      338 2022-03-07 13:52:57.000000 trainer-0.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3073 2022-04-14 09:11:47.454868 trainer-0.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1491 2022-04-11 08:27:36.000000 trainer-0.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)      553 2022-02-10 09:30:27.000000 trainer-0.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       41 2022-03-11 10:53:28.000000 trainer-0.0.8/requirements.dev.txt
--rw-r--r--   0 root         (0) root         (0)       11 2022-03-16 10:00:28.000000 trainer-0.0.8/requirements.test.txt
--rw-r--r--   0 root         (0) root         (0)       47 2022-03-11 10:47:31.000000 trainer-0.0.8/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-04-14 09:11:47.454868 trainer-0.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     4662 2022-04-11 08:27:36.000000 trainer-0.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-14 09:11:47.454868 trainer-0.0.8/trainer/
--rw-r--r--   0 root         (0) root         (0)      152 2022-02-10 09:30:27.000000 trainer-0.0.8/trainer/README.md
--rw-r--r--   0 root         (0) root         (0)        6 2022-04-14 09:10:17.000000 trainer-0.0.8/trainer/VERSION
--rw-r--r--   0 root         (0) root         (0)      215 2022-03-12 00:28:47.000000 trainer-0.0.8/trainer/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4156 2022-02-10 09:30:27.000000 trainer-0.0.8/trainer/callbacks.py
--rw-r--r--   0 root         (0) root         (0)     2155 2022-04-13 10:14:36.000000 trainer-0.0.8/trainer/distribute.py
--rw-r--r--   0 root         (0) root         (0)     4551 2022-04-13 10:14:36.000000 trainer-0.0.8/trainer/generic_utils.py
--rw-r--r--   0 root         (0) root         (0)     9452 2022-04-13 10:14:36.000000 trainer-0.0.8/trainer/io.py
--rw-r--r--   0 root         (0) root         (0)      214 2022-04-14 09:05:57.000000 trainer-0.0.8/trainer/logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-14 09:11:47.454868 trainer-0.0.8/trainer/logging/
--rw-r--r--   0 root         (0) root         (0)     1991 2022-03-16 13:38:56.000000 trainer-0.0.8/trainer/logging/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5965 2022-03-12 00:28:47.000000 trainer-0.0.8/trainer/logging/aim_logger.py
--rw-r--r--   0 root         (0) root         (0)     2682 2022-03-16 13:38:56.000000 trainer-0.0.8/trainer/logging/base_dash_logger.py
--rw-r--r--   0 root         (0) root         (0)     2110 2022-03-16 13:38:56.000000 trainer-0.0.8/trainer/logging/clearml_logger.py
--rw-r--r--   0 root         (0) root         (0)     4139 2022-04-14 09:05:57.000000 trainer-0.0.8/trainer/logging/console_logger.py
--rw-r--r--   0 root         (0) root         (0)     2359 2022-03-16 13:38:56.000000 trainer-0.0.8/trainer/logging/dummy_logger.py
--rw-r--r--   0 root         (0) root         (0)     5871 2022-03-12 00:28:47.000000 trainer-0.0.8/trainer/logging/mlflow_logger.py
--rw-r--r--   0 root         (0) root         (0)     2822 2022-03-12 00:28:47.000000 trainer-0.0.8/trainer/logging/tensorboard_logger.py
--rw-r--r--   0 root         (0) root         (0)     3303 2022-03-16 13:38:56.000000 trainer-0.0.8/trainer/logging/wandb_logger.py
--rw-r--r--   0 root         (0) root         (0)     4335 2022-03-12 00:28:47.000000 trainer-0.0.8/trainer/model.py
--rw-r--r--   0 root         (0) root         (0)     3026 2022-03-12 00:28:47.000000 trainer-0.0.8/trainer/torch.py
--rw-r--r--   0 root         (0) root         (0)    68565 2022-04-14 09:09:17.000000 trainer-0.0.8/trainer/trainer.py
--rw-r--r--   0 root         (0) root         (0)     4268 2022-04-13 10:14:36.000000 trainer-0.0.8/trainer/trainer_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-14 09:11:47.454868 trainer-0.0.8/trainer/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-02 15:15:22.000000 trainer-0.0.8/trainer/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1666 2022-04-13 10:14:36.000000 trainer-0.0.8/trainer/utils/distributed.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-14 09:11:47.454868 trainer-0.0.8/trainer.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3073 2022-04-14 09:11:47.000000 trainer-0.0.8/trainer.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      883 2022-04-14 09:11:47.000000 trainer-0.0.8/trainer.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-04-14 09:11:47.000000 trainer-0.0.8/trainer.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-04-07 12:26:48.000000 trainer-0.0.8/trainer.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      224 2022-04-14 09:11:47.000000 trainer-0.0.8/trainer.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2022-04-14 09:11:47.000000 trainer-0.0.8/trainer.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-27 13:17:21.648841 trainer-0.0.9/
+-rw-r--r--   0 root         (0) root         (0)      338 2022-03-07 13:52:57.000000 trainer-0.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3073 2022-04-27 13:17:21.648841 trainer-0.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1491 2022-04-11 08:27:36.000000 trainer-0.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      553 2022-02-10 09:30:27.000000 trainer-0.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       41 2022-03-11 10:53:28.000000 trainer-0.0.9/requirements.dev.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2022-03-16 10:00:28.000000 trainer-0.0.9/requirements.test.txt
+-rw-r--r--   0 root         (0) root         (0)       47 2022-03-11 10:47:31.000000 trainer-0.0.9/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2022-04-27 13:17:21.648841 trainer-0.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     4662 2022-04-11 08:27:36.000000 trainer-0.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-27 13:17:21.648841 trainer-0.0.9/trainer/
+-rw-r--r--   0 root         (0) root         (0)      152 2022-02-10 09:30:27.000000 trainer-0.0.9/trainer/README.md
+-rw-r--r--   0 root         (0) root         (0)        7 2022-04-27 12:50:13.000000 trainer-0.0.9/trainer/VERSION
+-rw-r--r--   0 root         (0) root         (0)      215 2022-03-12 00:28:47.000000 trainer-0.0.9/trainer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4156 2022-02-10 09:30:27.000000 trainer-0.0.9/trainer/callbacks.py
+-rw-r--r--   0 root         (0) root         (0)     2155 2022-04-13 10:14:36.000000 trainer-0.0.9/trainer/distribute.py
+-rw-r--r--   0 root         (0) root         (0)     4551 2022-04-13 10:14:36.000000 trainer-0.0.9/trainer/generic_utils.py
+-rw-r--r--   0 root         (0) root         (0)     9452 2022-04-27 12:58:43.000000 trainer-0.0.9/trainer/io.py
+-rw-r--r--   0 root         (0) root         (0)      214 2022-04-14 09:05:57.000000 trainer-0.0.9/trainer/logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-27 13:17:21.648841 trainer-0.0.9/trainer/logging/
+-rw-r--r--   0 root         (0) root         (0)     1991 2022-03-16 13:38:56.000000 trainer-0.0.9/trainer/logging/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5965 2022-03-12 00:28:47.000000 trainer-0.0.9/trainer/logging/aim_logger.py
+-rw-r--r--   0 root         (0) root         (0)     2682 2022-03-16 13:38:56.000000 trainer-0.0.9/trainer/logging/base_dash_logger.py
+-rw-r--r--   0 root         (0) root         (0)     2110 2022-03-16 13:38:56.000000 trainer-0.0.9/trainer/logging/clearml_logger.py
+-rw-r--r--   0 root         (0) root         (0)     4139 2022-04-14 09:05:57.000000 trainer-0.0.9/trainer/logging/console_logger.py
+-rw-r--r--   0 root         (0) root         (0)     2359 2022-03-16 13:38:56.000000 trainer-0.0.9/trainer/logging/dummy_logger.py
+-rw-r--r--   0 root         (0) root         (0)     5871 2022-03-12 00:28:47.000000 trainer-0.0.9/trainer/logging/mlflow_logger.py
+-rw-r--r--   0 root         (0) root         (0)     2822 2022-03-12 00:28:47.000000 trainer-0.0.9/trainer/logging/tensorboard_logger.py
+-rw-r--r--   0 root         (0) root         (0)     3303 2022-03-16 13:38:56.000000 trainer-0.0.9/trainer/logging/wandb_logger.py
+-rw-r--r--   0 root         (0) root         (0)     4335 2022-03-12 00:28:47.000000 trainer-0.0.9/trainer/model.py
+-rw-r--r--   0 root         (0) root         (0)     3026 2022-03-12 00:28:47.000000 trainer-0.0.9/trainer/torch.py
+-rw-r--r--   0 root         (0) root         (0)    68568 2022-04-27 13:17:12.000000 trainer-0.0.9/trainer/trainer.py
+-rw-r--r--   0 root         (0) root         (0)     4268 2022-04-27 13:17:12.000000 trainer-0.0.9/trainer/trainer_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-27 13:17:21.648841 trainer-0.0.9/trainer/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-03-02 15:15:22.000000 trainer-0.0.9/trainer/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1666 2022-04-13 10:14:36.000000 trainer-0.0.9/trainer/utils/distributed.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-27 13:17:21.648841 trainer-0.0.9/trainer.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3073 2022-04-27 13:17:21.000000 trainer-0.0.9/trainer.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      883 2022-04-27 13:17:21.000000 trainer-0.0.9/trainer.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-04-27 13:17:21.000000 trainer-0.0.9/trainer.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-04-07 12:26:48.000000 trainer-0.0.9/trainer.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      224 2022-04-27 13:17:21.000000 trainer-0.0.9/trainer.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2022-04-27 13:17:21.000000 trainer-0.0.9/trainer.egg-info/top_level.txt
```

### Comparing `trainer-0.0.8/PKG-INFO` & `trainer-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trainer
-Version: 0.0.8
+Version: 0.0.9
 Summary: General purpose model trainer for PyTorch that is more flexible than it should be, by 🐸Coqui.
 Home-page: https://github.com/coqui-ai/Trainer
 Author: Eren Gölge
 Author-email: egolge@coqui.ai
 License: Apache2
 Project-URL: Documentation, https://github.com/coqui-ai/Trainer/
 Project-URL: Tracker, https://github.com/coqui-ai/Trainer/issues
```

### Comparing `trainer-0.0.8/README.md` & `trainer-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `trainer-0.0.8/pyproject.toml` & `trainer-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `trainer-0.0.8/setup.py` & `trainer-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `trainer-0.0.8/trainer/callbacks.py` & `trainer-0.0.9/trainer/callbacks.py`

 * *Files identical despite different names*

### Comparing `trainer-0.0.8/trainer/distribute.py` & `trainer-0.0.9/trainer/distribute.py`

 * *Files identical despite different names*

### Comparing `trainer-0.0.8/trainer/generic_utils.py` & `trainer-0.0.9/trainer/generic_utils.py`

 * *Files identical despite different names*

### Comparing `trainer-0.0.8/trainer/io.py` & `trainer-0.0.9/trainer/io.py`

 * *Files identical despite different names*

### Comparing `trainer-0.0.8/trainer/logging/__init__.py` & `trainer-0.0.9/trainer/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `trainer-0.0.8/trainer/logging/aim_logger.py` & `trainer-0.0.9/trainer/logging/aim_logger.py`

 * *Files identical despite different names*

### Comparing `trainer-0.0.8/trainer/logging/base_dash_logger.py` & `trainer-0.0.9/trainer/logging/base_dash_logger.py`

 * *Files identical despite different names*

### Comparing `trainer-0.0.8/trainer/logging/clearml_logger.py` & `trainer-0.0.9/trainer/logging/clearml_logger.py`

 * *Files identical despite different names*

### Comparing `trainer-0.0.8/trainer/logging/console_logger.py` & `trainer-0.0.9/trainer/logging/console_logger.py`

 * *Files identical despite different names*

### Comparing `trainer-0.0.8/trainer/logging/dummy_logger.py` & `trainer-0.0.9/trainer/logging/dummy_logger.py`

 * *Files identical despite different names*

### Comparing `trainer-0.0.8/trainer/logging/mlflow_logger.py` & `trainer-0.0.9/trainer/logging/mlflow_logger.py`

 * *Files identical despite different names*

### Comparing `trainer-0.0.8/trainer/logging/tensorboard_logger.py` & `trainer-0.0.9/trainer/logging/tensorboard_logger.py`

 * *Files identical despite different names*

### Comparing `trainer-0.0.8/trainer/logging/wandb_logger.py` & `trainer-0.0.9/trainer/logging/wandb_logger.py`

 * *Files identical despite different names*

### Comparing `trainer-0.0.8/trainer/model.py` & `trainer-0.0.9/trainer/model.py`

 * *Files identical despite different names*

### Comparing `trainer-0.0.8/trainer/torch.py` & `trainer-0.0.9/trainer/torch.py`

 * *Files identical despite different names*

### Comparing `trainer-0.0.8/trainer/trainer.py` & `trainer-0.0.9/trainer/trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,17 +43,16 @@
     is_apex_available,
     setup_torch_training_env,
 )
 from trainer.utils.distributed import init_distributed
 
 logger = logging.getLogger("trainer")
 
-multiprocessing.set_start_method("fork")
-
 if platform.system() != "Windows":
+    multiprocessing.set_start_method("fork")
     # https://github.com/pytorch/pytorch/issues/973
     import resource
 
     rlimit = resource.getrlimit(resource.RLIMIT_NOFILE)
     resource.setrlimit(resource.RLIMIT_NOFILE, (4096, rlimit[1]))
```

### Comparing `trainer-0.0.8/trainer/trainer_utils.py` & `trainer-0.0.9/trainer/trainer_utils.py`

 * *Files identical despite different names*

### Comparing `trainer-0.0.8/trainer/utils/distributed.py` & `trainer-0.0.9/trainer/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `trainer-0.0.8/trainer.egg-info/PKG-INFO` & `trainer-0.0.9/trainer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trainer
-Version: 0.0.8
+Version: 0.0.9
 Summary: General purpose model trainer for PyTorch that is more flexible than it should be, by 🐸Coqui.
 Home-page: https://github.com/coqui-ai/Trainer
 Author: Eren Gölge
 Author-email: egolge@coqui.ai
 License: Apache2
 Project-URL: Documentation, https://github.com/coqui-ai/Trainer/
 Project-URL: Tracker, https://github.com/coqui-ai/Trainer/issues
```

### Comparing `trainer-0.0.8/trainer.egg-info/SOURCES.txt` & `trainer-0.0.9/trainer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

