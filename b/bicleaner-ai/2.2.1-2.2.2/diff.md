# Comparing `tmp/bicleaner-ai-2.2.1.tar.gz` & `tmp/bicleaner-ai-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bicleaner-ai-2.2.1.tar", last modified: Mon May  8 09:15:30 2023, max compression
+gzip compressed data, was "bicleaner-ai-2.2.2.tar", last modified: Fri Jun  9 08:45:12 2023, max compression
```

## Comparing `bicleaner-ai-2.2.1.tar` & `bicleaner-ai-2.2.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 09:15:30.465664 bicleaner-ai-2.2.1/
--rw-r--r--   0 runner    (1001) docker     (122)    35147 2023-05-08 09:15:15.000000 bicleaner-ai-2.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    65558 2023-05-08 09:15:30.465664 bicleaner-ai-2.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    24077 2023-05-08 09:15:15.000000 bicleaner-ai-2.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     2039 2023-05-08 09:15:15.000000 bicleaner-ai-2.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-08 09:15:30.465664 bicleaner-ai-2.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 09:15:30.461664 bicleaner-ai-2.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 09:15:30.465664 bicleaner-ai-2.2.1/src/bicleaner_ai/
--rwxr-xr-x   0 runner    (1001) docker     (122)      112 2023-05-08 09:15:15.000000 bicleaner-ai-2.2.1/src/bicleaner_ai/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     4547 2023-05-08 09:15:15.000000 bicleaner-ai-2.2.1/src/bicleaner_ai/bicleaner_ai_classifier.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     3607 2023-05-08 09:15:15.000000 bicleaner-ai-2.2.1/src/bicleaner_ai/bicleaner_ai_download.py
--rwxr-xr-x   0 runner    (1001) docker     (122)      642 2023-05-08 09:15:15.000000 bicleaner-ai-2.2.1/src/bicleaner_ai/bicleaner_ai_download_hf.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    16502 2023-05-08 09:15:15.000000 bicleaner-ai-2.2.1/src/bicleaner_ai/bicleaner_ai_train.py
--rw-r--r--   0 runner    (1001) docker     (122)     2964 2023-05-08 09:15:15.000000 bicleaner-ai-2.2.1/src/bicleaner_ai/calibrate.py
--rw-r--r--   0 runner    (1001) docker     (122)    13926 2023-05-08 09:15:15.000000 bicleaner-ai-2.2.1/src/bicleaner_ai/classify.py
--rw-r--r--   0 runner    (1001) docker     (122)     6479 2023-05-08 09:15:15.000000 bicleaner-ai-2.2.1/src/bicleaner_ai/datagen.py
--rw-r--r--   0 runner    (1001) docker     (122)     7456 2023-05-08 09:15:15.000000 bicleaner-ai-2.2.1/src/bicleaner_ai/decomposable_attention.py
--rw-r--r--   0 runner    (1001) docker     (122)     3927 2023-05-08 09:15:15.000000 bicleaner-ai-2.2.1/src/bicleaner_ai/layers.py
--rw-r--r--   0 runner    (1001) docker     (122)     2283 2023-05-08 09:15:15.000000 bicleaner-ai-2.2.1/src/bicleaner_ai/losses.py
--rw-r--r--   0 runner    (1001) docker     (122)     6372 2023-05-08 09:15:15.000000 bicleaner-ai-2.2.1/src/bicleaner_ai/metrics.py
--rw-r--r--   0 runner    (1001) docker     (122)    25236 2023-05-08 09:15:15.000000 bicleaner-ai-2.2.1/src/bicleaner_ai/models.py
--rw-r--r--   0 runner    (1001) docker     (122)     4101 2023-05-08 09:15:15.000000 bicleaner-ai-2.2.1/src/bicleaner_ai/models_util.py
--rw-r--r--   0 runner    (1001) docker     (122)     1197 2023-05-08 09:15:15.000000 bicleaner-ai-2.2.1/src/bicleaner_ai/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (122)    13140 2023-05-08 09:15:15.000000 bicleaner-ai-2.2.1/src/bicleaner_ai/training.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     4004 2023-05-08 09:15:15.000000 bicleaner-ai-2.2.1/src/bicleaner_ai/util.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1351 2023-05-08 09:15:15.000000 bicleaner-ai-2.2.1/src/bicleaner_ai/word_freqs_list.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     3123 2023-05-08 09:15:15.000000 bicleaner-ai-2.2.1/src/bicleaner_ai/word_freqs_zipf.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1082 2023-05-08 09:15:15.000000 bicleaner-ai-2.2.1/src/bicleaner_ai/word_freqs_zipf_double_linked.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 09:15:30.465664 bicleaner-ai-2.2.1/src/bicleaner_ai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    65558 2023-05-08 09:15:30.000000 bicleaner-ai-2.2.1/src/bicleaner_ai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      950 2023-05-08 09:15:30.000000 bicleaner-ai-2.2.1/src/bicleaner_ai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-08 09:15:30.000000 bicleaner-ai-2.2.1/src/bicleaner_ai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      276 2023-05-08 09:15:30.000000 bicleaner-ai-2.2.1/src/bicleaner_ai.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      293 2023-05-08 09:15:30.000000 bicleaner-ai-2.2.1/src/bicleaner_ai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-05-08 09:15:30.000000 bicleaner-ai-2.2.1/src/bicleaner_ai.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 08:45:12.087460 bicleaner-ai-2.2.2/
+-rw-r--r--   0 runner    (1001) docker     (122)    35147 2023-06-09 08:44:45.000000 bicleaner-ai-2.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    65558 2023-06-09 08:45:12.087460 bicleaner-ai-2.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    24077 2023-06-09 08:44:45.000000 bicleaner-ai-2.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     2039 2023-06-09 08:44:45.000000 bicleaner-ai-2.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-09 08:45:12.087460 bicleaner-ai-2.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 08:45:12.083460 bicleaner-ai-2.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 08:45:12.087460 bicleaner-ai-2.2.2/src/bicleaner_ai/
+-rwxr-xr-x   0 runner    (1001) docker     (122)      112 2023-06-09 08:44:45.000000 bicleaner-ai-2.2.2/src/bicleaner_ai/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4547 2023-06-09 08:44:45.000000 bicleaner-ai-2.2.2/src/bicleaner_ai/bicleaner_ai_classifier.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3607 2023-06-09 08:44:45.000000 bicleaner-ai-2.2.2/src/bicleaner_ai/bicleaner_ai_download.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)      642 2023-06-09 08:44:45.000000 bicleaner-ai-2.2.2/src/bicleaner_ai/bicleaner_ai_download_hf.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    16502 2023-06-09 08:44:45.000000 bicleaner-ai-2.2.2/src/bicleaner_ai/bicleaner_ai_train.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2964 2023-06-09 08:44:45.000000 bicleaner-ai-2.2.2/src/bicleaner_ai/calibrate.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14123 2023-06-09 08:44:45.000000 bicleaner-ai-2.2.2/src/bicleaner_ai/classify.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6479 2023-06-09 08:44:45.000000 bicleaner-ai-2.2.2/src/bicleaner_ai/datagen.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7456 2023-06-09 08:44:45.000000 bicleaner-ai-2.2.2/src/bicleaner_ai/decomposable_attention.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3927 2023-06-09 08:44:45.000000 bicleaner-ai-2.2.2/src/bicleaner_ai/layers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2283 2023-06-09 08:44:45.000000 bicleaner-ai-2.2.2/src/bicleaner_ai/losses.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6372 2023-06-09 08:44:45.000000 bicleaner-ai-2.2.2/src/bicleaner_ai/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25236 2023-06-09 08:44:45.000000 bicleaner-ai-2.2.2/src/bicleaner_ai/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4101 2023-06-09 08:44:45.000000 bicleaner-ai-2.2.2/src/bicleaner_ai/models_util.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1197 2023-06-09 08:44:45.000000 bicleaner-ai-2.2.2/src/bicleaner_ai/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13140 2023-06-09 08:44:45.000000 bicleaner-ai-2.2.2/src/bicleaner_ai/training.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4004 2023-06-09 08:44:45.000000 bicleaner-ai-2.2.2/src/bicleaner_ai/util.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1351 2023-06-09 08:44:45.000000 bicleaner-ai-2.2.2/src/bicleaner_ai/word_freqs_list.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3123 2023-06-09 08:44:45.000000 bicleaner-ai-2.2.2/src/bicleaner_ai/word_freqs_zipf.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1082 2023-06-09 08:44:45.000000 bicleaner-ai-2.2.2/src/bicleaner_ai/word_freqs_zipf_double_linked.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 08:45:12.087460 bicleaner-ai-2.2.2/src/bicleaner_ai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    65558 2023-06-09 08:45:12.000000 bicleaner-ai-2.2.2/src/bicleaner_ai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      950 2023-06-09 08:45:12.000000 bicleaner-ai-2.2.2/src/bicleaner_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-09 08:45:12.000000 bicleaner-ai-2.2.2/src/bicleaner_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      276 2023-06-09 08:45:12.000000 bicleaner-ai-2.2.2/src/bicleaner_ai.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      293 2023-06-09 08:45:12.000000 bicleaner-ai-2.2.2/src/bicleaner_ai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-06-09 08:45:12.000000 bicleaner-ai-2.2.2/src/bicleaner_ai.egg-info/top_level.txt
```

### Comparing `bicleaner-ai-2.2.1/LICENSE` & `bicleaner-ai-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bicleaner-ai-2.2.1/PKG-INFO` & `bicleaner-ai-2.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bicleaner-ai
-Version: 2.2.1
+Version: 2.2.2
 Summary: Parallel corpus classifier, indicating the likelihood of a pair of sentences being mutual translations or not (neural version)
 Author-email: Prompsit Language Engineering <info@prompsit.com>
 Maintainer-email: Jaume Zaragoza <jzaragoza@prompsit.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

### Comparing `bicleaner-ai-2.2.1/README.md` & `bicleaner-ai-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `bicleaner-ai-2.2.1/pyproject.toml` & `bicleaner-ai-2.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "bicleaner-ai"
-version = "2.2.1"
+version = "2.2.2"
 license = {file = "LICENSE"}
 authors = [
     { "name" = "Prompsit Language Engineering", "email" = "info@prompsit.com" }
 ]
 maintainers = [
     { "name" = "Jaume Zaragoza", "email" = "jzaragoza@prompsit.com" }
 ]
```

### Comparing `bicleaner-ai-2.2.1/src/bicleaner_ai/bicleaner_ai_classifier.py` & `bicleaner-ai-2.2.2/src/bicleaner_ai/bicleaner_ai_classifier.py`

 * *Files identical despite different names*

### Comparing `bicleaner-ai-2.2.1/src/bicleaner_ai/bicleaner_ai_download.py` & `bicleaner-ai-2.2.2/src/bicleaner_ai/bicleaner_ai_download.py`

 * *Files identical despite different names*

### Comparing `bicleaner-ai-2.2.1/src/bicleaner_ai/bicleaner_ai_download_hf.py` & `bicleaner-ai-2.2.2/src/bicleaner_ai/bicleaner_ai_download_hf.py`

 * *Files identical despite different names*

### Comparing `bicleaner-ai-2.2.1/src/bicleaner_ai/bicleaner_ai_train.py` & `bicleaner-ai-2.2.2/src/bicleaner_ai/bicleaner_ai_train.py`

 * *Files identical despite different names*

### Comparing `bicleaner-ai-2.2.1/src/bicleaner_ai/calibrate.py` & `bicleaner-ai-2.2.2/src/bicleaner_ai/calibrate.py`

 * *Files identical despite different names*

### Comparing `bicleaner-ai-2.2.1/src/bicleaner_ai/classify.py` & `bicleaner-ai-2.2.2/src/bicleaner_ai/classify.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,14 +135,20 @@
                 from cyrtranslit import to_latin
                 args.translit = True
             except (ModuleNotFoundError, NameError):
                 logging.warning("You might want to install 'cyrtranslit'"
                                 " to transliterate before scoring."
                                 "This improves accuracy and"
                                 " does not change output text.")
+        # Load rules config
+        if args.rules_config:
+            yaml_file = args.rules_config
+            args.rules_config = yaml.safe_load(args.rules_config)
+            yaml_file.close()
+
 
         logging.debug("YAML")
         logging.debug(metadata_yaml)
         args.metadata_yaml = metadata_yaml
         parser.set_defaults(**metadata_yaml)
     except:
         logging.error("Error loading metadata")
```

### Comparing `bicleaner-ai-2.2.1/src/bicleaner_ai/datagen.py` & `bicleaner-ai-2.2.2/src/bicleaner_ai/datagen.py`

 * *Files identical despite different names*

### Comparing `bicleaner-ai-2.2.1/src/bicleaner_ai/decomposable_attention.py` & `bicleaner-ai-2.2.2/src/bicleaner_ai/decomposable_attention.py`

 * *Files identical despite different names*

### Comparing `bicleaner-ai-2.2.1/src/bicleaner_ai/layers.py` & `bicleaner-ai-2.2.2/src/bicleaner_ai/layers.py`

 * *Files identical despite different names*

### Comparing `bicleaner-ai-2.2.1/src/bicleaner_ai/losses.py` & `bicleaner-ai-2.2.2/src/bicleaner_ai/losses.py`

 * *Files identical despite different names*

### Comparing `bicleaner-ai-2.2.1/src/bicleaner_ai/metrics.py` & `bicleaner-ai-2.2.2/src/bicleaner_ai/metrics.py`

 * *Files identical despite different names*

### Comparing `bicleaner-ai-2.2.1/src/bicleaner_ai/models.py` & `bicleaner-ai-2.2.2/src/bicleaner_ai/models.py`

 * *Files identical despite different names*

### Comparing `bicleaner-ai-2.2.1/src/bicleaner_ai/models_util.py` & `bicleaner-ai-2.2.2/src/bicleaner_ai/models_util.py`

 * *Files identical despite different names*

### Comparing `bicleaner-ai-2.2.1/src/bicleaner_ai/tokenizer.py` & `bicleaner-ai-2.2.2/src/bicleaner_ai/tokenizer.py`

 * *Files identical despite different names*

### Comparing `bicleaner-ai-2.2.1/src/bicleaner_ai/training.py` & `bicleaner-ai-2.2.2/src/bicleaner_ai/training.py`

 * *Files identical despite different names*

### Comparing `bicleaner-ai-2.2.1/src/bicleaner_ai/util.py` & `bicleaner-ai-2.2.2/src/bicleaner_ai/util.py`

 * *Files identical despite different names*

### Comparing `bicleaner-ai-2.2.1/src/bicleaner_ai/word_freqs_list.py` & `bicleaner-ai-2.2.2/src/bicleaner_ai/word_freqs_list.py`

 * *Files identical despite different names*

### Comparing `bicleaner-ai-2.2.1/src/bicleaner_ai/word_freqs_zipf.py` & `bicleaner-ai-2.2.2/src/bicleaner_ai/word_freqs_zipf.py`

 * *Files identical despite different names*

### Comparing `bicleaner-ai-2.2.1/src/bicleaner_ai/word_freqs_zipf_double_linked.py` & `bicleaner-ai-2.2.2/src/bicleaner_ai/word_freqs_zipf_double_linked.py`

 * *Files identical despite different names*

### Comparing `bicleaner-ai-2.2.1/src/bicleaner_ai.egg-info/PKG-INFO` & `bicleaner-ai-2.2.2/src/bicleaner_ai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bicleaner-ai
-Version: 2.2.1
+Version: 2.2.2
 Summary: Parallel corpus classifier, indicating the likelihood of a pair of sentences being mutual translations or not (neural version)
 Author-email: Prompsit Language Engineering <info@prompsit.com>
 Maintainer-email: Jaume Zaragoza <jzaragoza@prompsit.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

### Comparing `bicleaner-ai-2.2.1/src/bicleaner_ai.egg-info/SOURCES.txt` & `bicleaner-ai-2.2.2/src/bicleaner_ai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

