# Comparing `tmp/arcusapi-0.1.1.tar.gz` & `tmp/arcusapi-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcusapi-0.1.1.tar", last modified: Wed Jun  7 23:04:44 2023, max compression
+gzip compressed data, was "arcusapi-0.1.2.tar", last modified: Thu Jun  8 22:35:17 2023, max compression
```

## Comparing `arcusapi-0.1.1.tar` & `arcusapi-0.1.2.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-06-07 23:04:44.006601 arcusapi-0.1.1/
--rw-r--r--   0 ardasahiner   (501) staff       (20)    11344 2023-03-04 18:52:55.000000 arcusapi-0.1.1/LICENSE
--rw-r--r--   0 ardasahiner   (501) staff       (20)     1749 2023-06-07 23:04:44.006445 arcusapi-0.1.1/PKG-INFO
--rw-r--r--   0 ardasahiner   (501) staff       (20)     1222 2023-05-04 02:08:54.000000 arcusapi-0.1.1/README.md
-drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-06-07 23:04:43.996507 arcusapi-0.1.1/arcus/
--rw-r--r--   0 ardasahiner   (501) staff       (20)      857 2023-04-03 00:47:45.000000 arcusapi-0.1.1/arcus/__init__.py
--rw-r--r--   0 ardasahiner   (501) staff       (20)     4497 2023-05-25 18:25:11.000000 arcusapi-0.1.1/arcus/api_client.py
--rw-r--r--   0 ardasahiner   (501) staff       (20)     1514 2023-05-04 22:31:56.000000 arcusapi-0.1.1/arcus/config.py
--rw-r--r--   0 ardasahiner   (501) staff       (20)     1463 2023-05-04 22:31:56.000000 arcusapi-0.1.1/arcus/constants.py
-drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-06-07 23:04:43.996735 arcusapi-0.1.1/arcus/model/
--rw-r--r--   0 ardasahiner   (501) staff       (20)      687 2023-04-04 21:01:24.000000 arcusapi-0.1.1/arcus/model/__init__.py
-drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-06-07 23:04:43.998211 arcusapi-0.1.1/arcus/model/shared/
--rw-r--r--   0 ardasahiner   (501) staff       (20)      889 2023-04-03 00:47:45.000000 arcusapi-0.1.1/arcus/model/shared/__init__.py
--rw-r--r--   0 ardasahiner   (501) staff       (20)     1703 2023-05-04 22:31:56.000000 arcusapi-0.1.1/arcus/model/shared/config.py
--rw-r--r--   0 ardasahiner   (501) staff       (20)     2716 2023-05-04 22:51:20.000000 arcusapi-0.1.1/arcus/model/shared/data.py
--rw-r--r--   0 ardasahiner   (501) staff       (20)     5894 2023-05-18 19:12:04.000000 arcusapi-0.1.1/arcus/model/shared/metrics.py
--rw-r--r--   0 ardasahiner   (501) staff       (20)    10126 2023-05-25 18:25:11.000000 arcusapi-0.1.1/arcus/model/shared/trial.py
-drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-06-07 23:04:43.999704 arcusapi-0.1.1/arcus/model/torch/
--rw-r--r--   0 ardasahiner   (501) staff       (20)     1223 2023-06-03 20:38:00.000000 arcusapi-0.1.1/arcus/model/torch/__init__.py
-drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-06-07 23:04:44.001292 arcusapi-0.1.1/arcus/model/torch/data/
--rw-r--r--   0 ardasahiner   (501) staff       (20)     1143 2023-06-03 20:38:00.000000 arcusapi-0.1.1/arcus/model/torch/data/__init__.py
--rw-r--r--   0 ardasahiner   (501) staff       (20)     4745 2023-06-03 20:38:00.000000 arcusapi-0.1.1/arcus/model/torch/data/data_client.py
--rw-r--r--   0 ardasahiner   (501) staff       (20)     6588 2023-06-03 20:38:00.000000 arcusapi-0.1.1/arcus/model/torch/data/data_loader.py
--rw-r--r--   0 ardasahiner   (501) staff       (20)      990 2023-04-03 00:47:45.000000 arcusapi-0.1.1/arcus/model/torch/data/data_types.py
--rw-r--r--   0 ardasahiner   (501) staff       (20)     1936 2023-04-03 00:47:45.000000 arcusapi-0.1.1/arcus/model/torch/data/dataset.py
--rw-r--r--   0 ardasahiner   (501) staff       (20)     7924 2023-06-03 20:38:00.000000 arcusapi-0.1.1/arcus/model/torch/data/lightning_utils.py
--rw-r--r--   0 ardasahiner   (501) staff       (20)     2868 2023-05-04 22:31:56.000000 arcusapi-0.1.1/arcus/model/torch/data/tensor.py
--rw-r--r--   0 ardasahiner   (501) staff       (20)     3391 2023-06-03 20:38:00.000000 arcusapi-0.1.1/arcus/model/torch/metrics.py
-drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-06-07 23:04:44.002564 arcusapi-0.1.1/arcus/model/torch/model/
--rw-r--r--   0 ardasahiner   (501) staff       (20)      787 2023-04-04 21:01:24.000000 arcusapi-0.1.1/arcus/model/torch/model/__init__.py
--rw-r--r--   0 ardasahiner   (501) staff       (20)     2129 2023-04-04 21:01:24.000000 arcusapi-0.1.1/arcus/model/torch/model/embedding_getter.py
--rw-r--r--   0 ardasahiner   (501) staff       (20)      706 2023-04-04 21:01:24.000000 arcusapi-0.1.1/arcus/model/torch/model/model_types.py
--rw-r--r--   0 ardasahiner   (501) staff       (20)    12970 2023-05-04 02:08:54.000000 arcusapi-0.1.1/arcus/model/torch/model/module.py
--rw-r--r--   0 ardasahiner   (501) staff       (20)     1186 2023-04-27 17:14:10.000000 arcusapi-0.1.1/arcus/model/torch/model/utils.py
--rw-r--r--   0 ardasahiner   (501) staff       (20)    11404 2023-06-03 20:38:00.000000 arcusapi-0.1.1/arcus/model/torch/trainer.py
--rw-r--r--   0 ardasahiner   (501) staff       (20)     3839 2023-06-03 20:38:00.000000 arcusapi-0.1.1/arcus/model/torch/utils.py
-drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-06-07 23:04:44.003013 arcusapi-0.1.1/arcus/prompt/
--rw-r--r--   0 ardasahiner   (501) staff       (20)      610 2023-04-03 00:47:45.000000 arcusapi-0.1.1/arcus/prompt/__init.py
-drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-06-07 23:04:44.003435 arcusapi-0.1.1/arcus/prompt/text/
--rw-r--r--   0 ardasahiner   (501) staff       (20)      673 2023-04-03 00:47:45.000000 arcusapi-0.1.1/arcus/prompt/text/__init__.py
-drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-06-07 23:04:44.004189 arcusapi-0.1.1/arcus/prompt/text/chains/
--rw-r--r--   0 ardasahiner   (501) staff       (20)      615 2023-06-04 07:01:05.000000 arcusapi-0.1.1/arcus/prompt/text/chains/__init__.py
--rw-r--r--   0 ardasahiner   (501) staff       (20)    10988 2023-06-04 07:01:05.000000 arcusapi-0.1.1/arcus/prompt/text/chains/retrieval_qa.py
--rw-r--r--   0 ardasahiner   (501) staff       (20)     1087 2023-05-18 19:12:04.000000 arcusapi-0.1.1/arcus/prompt/text/config.py
-drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-06-07 23:04:44.004996 arcusapi-0.1.1/arcus/prompt/text/llms/
--rw-r--r--   0 ardasahiner   (501) staff       (20)      664 2023-04-03 00:47:45.000000 arcusapi-0.1.1/arcus/prompt/text/llms/__init__.py
--rw-r--r--   0 ardasahiner   (501) staff       (20)     1591 2023-04-03 00:47:45.000000 arcusapi-0.1.1/arcus/prompt/text/llms/llm.py
--rw-r--r--   0 ardasahiner   (501) staff       (20)     3898 2023-06-03 00:30:26.000000 arcusapi-0.1.1/arcus/prompt/text/llms/openai.py
-drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-06-07 23:04:44.005828 arcusapi-0.1.1/arcusapi.egg-info/
--rw-r--r--   0 ardasahiner   (501) staff       (20)     1749 2023-06-07 23:04:43.000000 arcusapi-0.1.1/arcusapi.egg-info/PKG-INFO
--rw-r--r--   0 ardasahiner   (501) staff       (20)     1297 2023-06-07 23:04:43.000000 arcusapi-0.1.1/arcusapi.egg-info/SOURCES.txt
--rw-r--r--   0 ardasahiner   (501) staff       (20)        1 2023-06-07 23:04:43.000000 arcusapi-0.1.1/arcusapi.egg-info/dependency_links.txt
--rw-r--r--   0 ardasahiner   (501) staff       (20)      104 2023-06-07 23:04:43.000000 arcusapi-0.1.1/arcusapi.egg-info/requires.txt
--rw-r--r--   0 ardasahiner   (501) staff       (20)        6 2023-06-07 23:04:43.000000 arcusapi-0.1.1/arcusapi.egg-info/top_level.txt
--rw-r--r--   0 ardasahiner   (501) staff       (20)      747 2023-06-07 22:48:56.000000 arcusapi-0.1.1/pyproject.toml
--rw-r--r--   0 ardasahiner   (501) staff       (20)       38 2023-06-07 23:04:44.006641 arcusapi-0.1.1/setup.cfg
-drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-06-07 23:04:44.006244 arcusapi-0.1.1/tests/
--rw-r--r--   0 ardasahiner   (501) staff       (20)     3516 2023-05-04 22:31:56.000000 arcusapi-0.1.1/tests/test_api_client.py
--rw-r--r--   0 ardasahiner   (501) staff       (20)     3613 2023-04-03 00:47:45.000000 arcusapi-0.1.1/tests/test_constants.py
+drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-06-08 22:35:17.562734 arcusapi-0.1.2/
+-rw-r--r--   0 ardasahiner   (501) staff       (20)    11344 2023-03-04 18:52:55.000000 arcusapi-0.1.2/LICENSE
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     1790 2023-06-08 22:35:17.562533 arcusapi-0.1.2/PKG-INFO
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     1222 2023-05-04 02:08:54.000000 arcusapi-0.1.2/README.md
+drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-06-08 22:35:17.551182 arcusapi-0.1.2/arcus/
+-rw-r--r--   0 ardasahiner   (501) staff       (20)      857 2023-04-03 00:47:45.000000 arcusapi-0.1.2/arcus/__init__.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     4497 2023-05-25 18:25:11.000000 arcusapi-0.1.2/arcus/api_client.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     1514 2023-05-04 22:31:56.000000 arcusapi-0.1.2/arcus/config.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     1463 2023-05-04 22:31:56.000000 arcusapi-0.1.2/arcus/constants.py
+drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-06-08 22:35:17.551451 arcusapi-0.1.2/arcus/model/
+-rw-r--r--   0 ardasahiner   (501) staff       (20)      727 2023-06-08 22:34:47.000000 arcusapi-0.1.2/arcus/model/__init__.py
+drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-06-08 22:35:17.553223 arcusapi-0.1.2/arcus/model/shared/
+-rw-r--r--   0 ardasahiner   (501) staff       (20)      889 2023-04-03 00:47:45.000000 arcusapi-0.1.2/arcus/model/shared/__init__.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     1703 2023-05-04 22:31:56.000000 arcusapi-0.1.2/arcus/model/shared/config.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     2716 2023-05-04 22:51:20.000000 arcusapi-0.1.2/arcus/model/shared/data.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     5894 2023-05-18 19:12:04.000000 arcusapi-0.1.2/arcus/model/shared/metrics.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)    10126 2023-05-25 18:25:11.000000 arcusapi-0.1.2/arcus/model/shared/trial.py
+drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-06-08 22:35:17.554889 arcusapi-0.1.2/arcus/model/torch/
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     1223 2023-06-08 21:50:19.000000 arcusapi-0.1.2/arcus/model/torch/__init__.py
+drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-06-08 22:35:17.556902 arcusapi-0.1.2/arcus/model/torch/data/
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     1143 2023-06-08 21:50:19.000000 arcusapi-0.1.2/arcus/model/torch/data/__init__.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     4745 2023-06-08 21:50:19.000000 arcusapi-0.1.2/arcus/model/torch/data/data_client.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     6588 2023-06-08 21:50:19.000000 arcusapi-0.1.2/arcus/model/torch/data/data_loader.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)      990 2023-04-03 00:47:45.000000 arcusapi-0.1.2/arcus/model/torch/data/data_types.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     1936 2023-04-03 00:47:45.000000 arcusapi-0.1.2/arcus/model/torch/data/dataset.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     7924 2023-06-08 21:50:20.000000 arcusapi-0.1.2/arcus/model/torch/data/lightning_utils.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     2868 2023-05-04 22:31:56.000000 arcusapi-0.1.2/arcus/model/torch/data/tensor.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     3391 2023-06-08 21:50:19.000000 arcusapi-0.1.2/arcus/model/torch/metrics.py
+drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-06-08 22:35:17.558421 arcusapi-0.1.2/arcus/model/torch/model/
+-rw-r--r--   0 ardasahiner   (501) staff       (20)      787 2023-04-04 21:01:24.000000 arcusapi-0.1.2/arcus/model/torch/model/__init__.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     2129 2023-04-04 21:01:24.000000 arcusapi-0.1.2/arcus/model/torch/model/embedding_getter.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)      706 2023-04-04 21:01:24.000000 arcusapi-0.1.2/arcus/model/torch/model/model_types.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)    12970 2023-05-04 02:08:54.000000 arcusapi-0.1.2/arcus/model/torch/model/module.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     1186 2023-04-27 17:14:10.000000 arcusapi-0.1.2/arcus/model/torch/model/utils.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)    11404 2023-06-08 21:50:20.000000 arcusapi-0.1.2/arcus/model/torch/trainer.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     3839 2023-06-08 21:50:19.000000 arcusapi-0.1.2/arcus/model/torch/utils.py
+drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-06-08 22:35:17.558847 arcusapi-0.1.2/arcus/prompt/
+-rw-r--r--   0 ardasahiner   (501) staff       (20)      610 2023-04-03 00:47:45.000000 arcusapi-0.1.2/arcus/prompt/__init.py
+drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-06-08 22:35:17.559428 arcusapi-0.1.2/arcus/prompt/text/
+-rw-r--r--   0 ardasahiner   (501) staff       (20)      673 2023-04-03 00:47:45.000000 arcusapi-0.1.2/arcus/prompt/text/__init__.py
+drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-06-08 22:35:17.560242 arcusapi-0.1.2/arcus/prompt/text/chains/
+-rw-r--r--   0 ardasahiner   (501) staff       (20)      615 2023-06-04 07:01:05.000000 arcusapi-0.1.2/arcus/prompt/text/chains/__init__.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)    10988 2023-06-08 21:50:20.000000 arcusapi-0.1.2/arcus/prompt/text/chains/retrieval_qa.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     1087 2023-05-18 19:12:04.000000 arcusapi-0.1.2/arcus/prompt/text/config.py
+drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-06-08 22:35:17.561054 arcusapi-0.1.2/arcus/prompt/text/llms/
+-rw-r--r--   0 ardasahiner   (501) staff       (20)      664 2023-04-03 00:47:45.000000 arcusapi-0.1.2/arcus/prompt/text/llms/__init__.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     1591 2023-04-03 00:47:45.000000 arcusapi-0.1.2/arcus/prompt/text/llms/llm.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     3898 2023-06-03 00:30:26.000000 arcusapi-0.1.2/arcus/prompt/text/llms/openai.py
+drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-06-08 22:35:17.561884 arcusapi-0.1.2/arcusapi.egg-info/
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     1790 2023-06-08 22:35:17.000000 arcusapi-0.1.2/arcusapi.egg-info/PKG-INFO
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     1297 2023-06-08 22:35:17.000000 arcusapi-0.1.2/arcusapi.egg-info/SOURCES.txt
+-rw-r--r--   0 ardasahiner   (501) staff       (20)        1 2023-06-08 22:35:17.000000 arcusapi-0.1.2/arcusapi.egg-info/dependency_links.txt
+-rw-r--r--   0 ardasahiner   (501) staff       (20)      159 2023-06-08 22:35:17.000000 arcusapi-0.1.2/arcusapi.egg-info/requires.txt
+-rw-r--r--   0 ardasahiner   (501) staff       (20)        6 2023-06-08 22:35:17.000000 arcusapi-0.1.2/arcusapi.egg-info/top_level.txt
+-rw-r--r--   0 ardasahiner   (501) staff       (20)      848 2023-06-08 22:34:47.000000 arcusapi-0.1.2/pyproject.toml
+-rw-r--r--   0 ardasahiner   (501) staff       (20)       38 2023-06-08 22:35:17.562800 arcusapi-0.1.2/setup.cfg
+drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-06-08 22:35:17.562276 arcusapi-0.1.2/tests/
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     3516 2023-05-04 22:31:56.000000 arcusapi-0.1.2/tests/test_api_client.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     3613 2023-04-03 00:47:45.000000 arcusapi-0.1.2/tests/test_constants.py
```

### Comparing `arcusapi-0.1.1/LICENSE` & `arcusapi-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.1/PKG-INFO` & `arcusapi-0.1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: arcusapi
-Version: 0.1.1
+Version: 0.1.2
 Summary: Arcus Data Exchange Client SDK.
 Author-email: "Arcus Inc." <sdk@arcus.co>
 Project-URL: Homepage, https://www.arcus.co
 Project-URL: Documentation, https://app.arcus.co/docs
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: <3.11,>=3.8
+Requires-Python: <4.0,>=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: torch
+Provides-Extra: all
 License-File: LICENSE
 
 # Arcus Data Exchange Client SDK
 
 The Arcus Data Exchange is a two-sided auction house that matches Data Consumers
 with Data Publishers. Data Consumers leverage data from the auction to improve 
 their AI applications’ performance, while Data Publishers monetize and distribute
```

### Comparing `arcusapi-0.1.1/README.md` & `arcusapi-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.1/arcus/__init__.py` & `arcusapi-0.1.2/arcus/__init__.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.1/arcus/api_client.py` & `arcusapi-0.1.2/arcus/api_client.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.1/arcus/config.py` & `arcusapi-0.1.2/arcus/config.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.1/arcus/constants.py` & `arcusapi-0.1.2/arcus/constants.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.1/arcus/model/__init__.py` & `arcusapi-0.1.2/arcus/model/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,9 +10,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 from . import shared  # noqa: F401
-from . import torch  # noqa: F401
+
+try:
+    from . import torch  # noqa: F401
+except ImportError:
+    pass
+
 from .shared import Config  # noqa: F401
```

### Comparing `arcusapi-0.1.1/arcus/model/shared/__init__.py` & `arcusapi-0.1.2/arcus/model/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.1/arcus/model/shared/config.py` & `arcusapi-0.1.2/arcus/model/shared/config.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.1/arcus/model/shared/data.py` & `arcusapi-0.1.2/arcus/model/shared/data.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.1/arcus/model/shared/metrics.py` & `arcusapi-0.1.2/arcus/model/shared/metrics.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.1/arcus/model/shared/trial.py` & `arcusapi-0.1.2/arcus/model/shared/trial.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.1/arcus/model/torch/__init__.py` & `arcusapi-0.1.2/arcus/model/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.1/arcus/model/torch/data/__init__.py` & `arcusapi-0.1.2/arcus/model/torch/data/__init__.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.1/arcus/model/torch/data/data_client.py` & `arcusapi-0.1.2/arcus/model/torch/data/data_client.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.1/arcus/model/torch/data/data_loader.py` & `arcusapi-0.1.2/arcus/model/torch/data/data_loader.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.1/arcus/model/torch/data/data_types.py` & `arcusapi-0.1.2/arcus/model/torch/data/data_types.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.1/arcus/model/torch/data/dataset.py` & `arcusapi-0.1.2/arcus/model/torch/data/dataset.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.1/arcus/model/torch/data/lightning_utils.py` & `arcusapi-0.1.2/arcus/model/torch/data/lightning_utils.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.1/arcus/model/torch/data/tensor.py` & `arcusapi-0.1.2/arcus/model/torch/data/tensor.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.1/arcus/model/torch/metrics.py` & `arcusapi-0.1.2/arcus/model/torch/metrics.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.1/arcus/model/torch/model/__init__.py` & `arcusapi-0.1.2/arcus/model/torch/model/__init__.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.1/arcus/model/torch/model/embedding_getter.py` & `arcusapi-0.1.2/arcus/model/torch/model/embedding_getter.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.1/arcus/model/torch/model/model_types.py` & `arcusapi-0.1.2/arcus/model/torch/model/model_types.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.1/arcus/model/torch/model/module.py` & `arcusapi-0.1.2/arcus/model/torch/model/module.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.1/arcus/model/torch/model/utils.py` & `arcusapi-0.1.2/arcus/model/torch/model/utils.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.1/arcus/model/torch/trainer.py` & `arcusapi-0.1.2/arcus/model/torch/trainer.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.1/arcus/model/torch/utils.py` & `arcusapi-0.1.2/arcus/model/torch/utils.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.1/arcus/prompt/__init.py` & `arcusapi-0.1.2/arcus/prompt/__init.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.1/arcus/prompt/text/__init__.py` & `arcusapi-0.1.2/arcus/prompt/text/__init__.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.1/arcus/prompt/text/chains/__init__.py` & `arcusapi-0.1.2/arcus/prompt/text/chains/__init__.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.1/arcus/prompt/text/chains/retrieval_qa.py` & `arcusapi-0.1.2/arcus/prompt/text/chains/retrieval_qa.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.1/arcus/prompt/text/config.py` & `arcusapi-0.1.2/arcus/prompt/text/config.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.1/arcus/prompt/text/llms/__init__.py` & `arcusapi-0.1.2/arcus/prompt/text/llms/__init__.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.1/arcus/prompt/text/llms/llm.py` & `arcusapi-0.1.2/arcus/prompt/text/llms/llm.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.1/arcus/prompt/text/llms/openai.py` & `arcusapi-0.1.2/arcus/prompt/text/llms/openai.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.1/arcusapi.egg-info/PKG-INFO` & `arcusapi-0.1.2/arcusapi.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: arcusapi
-Version: 0.1.1
+Version: 0.1.2
 Summary: Arcus Data Exchange Client SDK.
 Author-email: "Arcus Inc." <sdk@arcus.co>
 Project-URL: Homepage, https://www.arcus.co
 Project-URL: Documentation, https://app.arcus.co/docs
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: <3.11,>=3.8
+Requires-Python: <4.0,>=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: torch
+Provides-Extra: all
 License-File: LICENSE
 
 # Arcus Data Exchange Client SDK
 
 The Arcus Data Exchange is a two-sided auction house that matches Data Consumers
 with Data Publishers. Data Consumers leverage data from the auction to improve 
 their AI applications’ performance, while Data Publishers monetize and distribute
```

### Comparing `arcusapi-0.1.1/arcusapi.egg-info/SOURCES.txt` & `arcusapi-0.1.2/arcusapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.1/tests/test_api_client.py` & `arcusapi-0.1.2/tests/test_api_client.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.1/tests/test_constants.py` & `arcusapi-0.1.2/tests/test_constants.py`

 * *Files identical despite different names*

