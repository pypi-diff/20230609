# Comparing `tmp/gisting_test-0.1.4.tar.gz` & `tmp/gisting_test-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gisting_test-0.1.4.tar", last modified: Sat Jun  3 02:44:27 2023, max compression
+gzip compressed data, was "gisting_test-0.1.5.tar", last modified: Fri Jun  9 17:54:09 2023, max compression
```

## Comparing `gisting_test-0.1.4.tar` & `gisting_test-0.1.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 owaiszahid   (501) staff       (20)        0 2023-06-03 02:44:27.417678 gisting_test-0.1.4/
--rw-r--r--   0 owaiszahid   (501) staff       (20)      288 2023-06-03 02:44:27.417552 gisting_test-0.1.4/PKG-INFO
-drwxr-xr-x   0 owaiszahid   (501) staff       (20)        0 2023-06-03 02:44:27.412756 gisting_test-0.1.4/gisting_test/
--rw-r--r--   0 owaiszahid   (501) staff       (20)       18 2023-06-01 17:36:38.000000 gisting_test-0.1.4/gisting_test/__init__.py
-drwxr-xr-x   0 owaiszahid   (501) staff       (20)        0 2023-06-03 02:44:27.416760 gisting_test-0.1.4/gisting_test/src/
--rw-r--r--   0 owaiszahid   (501) staff       (20)        0 2023-06-01 17:49:51.000000 gisting_test-0.1.4/gisting_test/src/__init__.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)    11076 2023-05-30 23:00:39.000000 gisting_test-0.1.4/gisting_test/src/arguments.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)     3462 2023-05-30 23:00:39.000000 gisting_test-0.1.4/gisting_test/src/benchmarking.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)     8814 2023-06-03 02:43:55.000000 gisting_test-0.1.4/gisting_test/src/compress.py
-drwxr-xr-x   0 owaiszahid   (501) staff       (20)        0 2023-06-03 02:44:27.417309 gisting_test-0.1.4/gisting_test/src/data/
--rw-r--r--   0 owaiszahid   (501) staff       (20)        0 2023-05-30 23:00:39.000000 gisting_test-0.1.4/gisting_test/src/data/__init__.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)     8550 2023-05-30 23:00:39.000000 gisting_test-0.1.4/gisting_test/src/data/gist.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)      554 2023-05-30 23:00:39.000000 gisting_test-0.1.4/gisting_test/src/data/utils.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)    21595 2023-05-30 23:00:39.000000 gisting_test-0.1.4/gisting_test/src/generation_utils.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)     4748 2023-05-30 23:00:39.000000 gisting_test-0.1.4/gisting_test/src/gist_caching.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)    34287 2023-05-30 23:00:39.000000 gisting_test-0.1.4/gisting_test/src/gist_llama.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)    41427 2023-05-30 23:00:39.000000 gisting_test-0.1.4/gisting_test/src/gist_t5.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)     2954 2023-05-30 23:00:39.000000 gisting_test-0.1.4/gisting_test/src/integrations.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)     4277 2023-05-30 23:00:39.000000 gisting_test-0.1.4/gisting_test/src/metrics.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)    13819 2023-05-30 23:00:39.000000 gisting_test-0.1.4/gisting_test/src/train.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)    52559 2023-05-30 23:00:39.000000 gisting_test-0.1.4/gisting_test/src/trainer_seq2seq.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)      426 2023-05-30 23:00:39.000000 gisting_test-0.1.4/gisting_test/src/utils.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)     7880 2023-05-30 23:00:39.000000 gisting_test-0.1.4/gisting_test/src/weight_diff.py
-drwxr-xr-x   0 owaiszahid   (501) staff       (20)        0 2023-06-03 02:44:27.413666 gisting_test-0.1.4/gisting_test.egg-info/
--rw-r--r--   0 owaiszahid   (501) staff       (20)      288 2023-06-03 02:44:27.000000 gisting_test-0.1.4/gisting_test.egg-info/PKG-INFO
--rw-r--r--   0 owaiszahid   (501) staff       (20)      703 2023-06-03 02:44:27.000000 gisting_test-0.1.4/gisting_test.egg-info/SOURCES.txt
--rw-r--r--   0 owaiszahid   (501) staff       (20)        1 2023-06-03 02:44:27.000000 gisting_test-0.1.4/gisting_test.egg-info/dependency_links.txt
--rw-r--r--   0 owaiszahid   (501) staff       (20)       52 2023-06-03 02:44:27.000000 gisting_test-0.1.4/gisting_test.egg-info/top_level.txt
--rw-r--r--   0 owaiszahid   (501) staff       (20)       38 2023-06-03 02:44:27.417722 gisting_test-0.1.4/setup.cfg
--rw-r--r--   0 owaiszahid   (501) staff       (20)      411 2023-06-03 02:44:18.000000 gisting_test-0.1.4/setup.py
+drwxr-xr-x   0 owaiszahid   (501) staff       (20)        0 2023-06-09 17:54:09.454478 gisting_test-0.1.5/
+-rw-r--r--   0 owaiszahid   (501) staff       (20)      288 2023-06-09 17:54:09.454361 gisting_test-0.1.5/PKG-INFO
+drwxr-xr-x   0 owaiszahid   (501) staff       (20)        0 2023-06-09 17:54:09.450405 gisting_test-0.1.5/gisting_test/
+-rw-r--r--   0 owaiszahid   (501) staff       (20)       18 2023-06-01 17:36:38.000000 gisting_test-0.1.5/gisting_test/__init__.py
+drwxr-xr-x   0 owaiszahid   (501) staff       (20)        0 2023-06-09 17:54:09.453720 gisting_test-0.1.5/gisting_test/src/
+-rw-r--r--   0 owaiszahid   (501) staff       (20)        0 2023-06-01 17:49:51.000000 gisting_test-0.1.5/gisting_test/src/__init__.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)    11076 2023-05-30 23:00:39.000000 gisting_test-0.1.5/gisting_test/src/arguments.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)     3462 2023-05-30 23:00:39.000000 gisting_test-0.1.5/gisting_test/src/benchmarking.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)     8769 2023-06-09 17:51:45.000000 gisting_test-0.1.5/gisting_test/src/compress.py
+drwxr-xr-x   0 owaiszahid   (501) staff       (20)        0 2023-06-09 17:54:09.454172 gisting_test-0.1.5/gisting_test/src/data/
+-rw-r--r--   0 owaiszahid   (501) staff       (20)        0 2023-05-30 23:00:39.000000 gisting_test-0.1.5/gisting_test/src/data/__init__.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)     8550 2023-05-30 23:00:39.000000 gisting_test-0.1.5/gisting_test/src/data/gist.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)      554 2023-05-30 23:00:39.000000 gisting_test-0.1.5/gisting_test/src/data/utils.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)    21595 2023-05-30 23:00:39.000000 gisting_test-0.1.5/gisting_test/src/generation_utils.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)     4748 2023-05-30 23:00:39.000000 gisting_test-0.1.5/gisting_test/src/gist_caching.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)    34287 2023-05-30 23:00:39.000000 gisting_test-0.1.5/gisting_test/src/gist_llama.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)    41427 2023-05-30 23:00:39.000000 gisting_test-0.1.5/gisting_test/src/gist_t5.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)     2954 2023-05-30 23:00:39.000000 gisting_test-0.1.5/gisting_test/src/integrations.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)     4277 2023-05-30 23:00:39.000000 gisting_test-0.1.5/gisting_test/src/metrics.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)    13819 2023-05-30 23:00:39.000000 gisting_test-0.1.5/gisting_test/src/train.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)    52559 2023-05-30 23:00:39.000000 gisting_test-0.1.5/gisting_test/src/trainer_seq2seq.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)      426 2023-05-30 23:00:39.000000 gisting_test-0.1.5/gisting_test/src/utils.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)     7880 2023-05-30 23:00:39.000000 gisting_test-0.1.5/gisting_test/src/weight_diff.py
+drwxr-xr-x   0 owaiszahid   (501) staff       (20)        0 2023-06-09 17:54:09.450990 gisting_test-0.1.5/gisting_test.egg-info/
+-rw-r--r--   0 owaiszahid   (501) staff       (20)      288 2023-06-09 17:54:09.000000 gisting_test-0.1.5/gisting_test.egg-info/PKG-INFO
+-rw-r--r--   0 owaiszahid   (501) staff       (20)      703 2023-06-09 17:54:09.000000 gisting_test-0.1.5/gisting_test.egg-info/SOURCES.txt
+-rw-r--r--   0 owaiszahid   (501) staff       (20)        1 2023-06-09 17:54:09.000000 gisting_test-0.1.5/gisting_test.egg-info/dependency_links.txt
+-rw-r--r--   0 owaiszahid   (501) staff       (20)       52 2023-06-09 17:54:09.000000 gisting_test-0.1.5/gisting_test.egg-info/top_level.txt
+-rw-r--r--   0 owaiszahid   (501) staff       (20)       38 2023-06-09 17:54:09.454518 gisting_test-0.1.5/setup.cfg
+-rw-r--r--   0 owaiszahid   (501) staff       (20)      411 2023-06-09 17:53:24.000000 gisting_test-0.1.5/setup.py
```

### Comparing `gisting_test-0.1.4/gisting_test/src/arguments.py` & `gisting_test-0.1.5/gisting_test/src/arguments.py`

 * *Files identical despite different names*

### Comparing `gisting_test-0.1.4/gisting_test/src/benchmarking.py` & `gisting_test-0.1.5/gisting_test/src/benchmarking.py`

 * *Files identical despite different names*

### Comparing `gisting_test-0.1.4/gisting_test/src/compress.py` & `gisting_test-0.1.5/gisting_test/src/compress.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,14 @@
     else:
         model = model_cls.from_pretrained(
             model_name_or_path,
             config=config,
             cache_dir=cache_dir,
             device_map = "auto"
         )
-        model = torch.nn.DataParallel(model)
 
     dtypes = {
         "bf16": torch.bfloat16,
         "fp16": torch.float16,
         "fp32": torch.float,
     }
     model = model.to(dtypes[precision]).cuda().eval()
```

### Comparing `gisting_test-0.1.4/gisting_test/src/data/gist.py` & `gisting_test-0.1.5/gisting_test/src/data/gist.py`

 * *Files identical despite different names*

### Comparing `gisting_test-0.1.4/gisting_test/src/data/utils.py` & `gisting_test-0.1.5/gisting_test/src/data/utils.py`

 * *Files identical despite different names*

### Comparing `gisting_test-0.1.4/gisting_test/src/generation_utils.py` & `gisting_test-0.1.5/gisting_test/src/generation_utils.py`

 * *Files identical despite different names*

### Comparing `gisting_test-0.1.4/gisting_test/src/gist_caching.py` & `gisting_test-0.1.5/gisting_test/src/gist_caching.py`

 * *Files identical despite different names*

### Comparing `gisting_test-0.1.4/gisting_test/src/gist_llama.py` & `gisting_test-0.1.5/gisting_test/src/gist_llama.py`

 * *Files identical despite different names*

### Comparing `gisting_test-0.1.4/gisting_test/src/gist_t5.py` & `gisting_test-0.1.5/gisting_test/src/gist_t5.py`

 * *Files identical despite different names*

### Comparing `gisting_test-0.1.4/gisting_test/src/integrations.py` & `gisting_test-0.1.5/gisting_test/src/integrations.py`

 * *Files identical despite different names*

### Comparing `gisting_test-0.1.4/gisting_test/src/metrics.py` & `gisting_test-0.1.5/gisting_test/src/metrics.py`

 * *Files identical despite different names*

### Comparing `gisting_test-0.1.4/gisting_test/src/train.py` & `gisting_test-0.1.5/gisting_test/src/train.py`

 * *Files identical despite different names*

### Comparing `gisting_test-0.1.4/gisting_test/src/trainer_seq2seq.py` & `gisting_test-0.1.5/gisting_test/src/trainer_seq2seq.py`

 * *Files identical despite different names*

### Comparing `gisting_test-0.1.4/gisting_test/src/weight_diff.py` & `gisting_test-0.1.5/gisting_test/src/weight_diff.py`

 * *Files identical despite different names*

### Comparing `gisting_test-0.1.4/gisting_test.egg-info/SOURCES.txt` & `gisting_test-0.1.5/gisting_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

