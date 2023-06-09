# Comparing `tmp/gisting_test-0.1.5.tar.gz` & `tmp/gisting_test-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gisting_test-0.1.5.tar", last modified: Fri Jun  9 17:54:09 2023, max compression
+gzip compressed data, was "gisting_test-0.1.6.tar", last modified: Fri Jun  9 18:39:40 2023, max compression
```

## Comparing `gisting_test-0.1.5.tar` & `gisting_test-0.1.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 owaiszahid   (501) staff       (20)        0 2023-06-09 17:54:09.454478 gisting_test-0.1.5/
--rw-r--r--   0 owaiszahid   (501) staff       (20)      288 2023-06-09 17:54:09.454361 gisting_test-0.1.5/PKG-INFO
-drwxr-xr-x   0 owaiszahid   (501) staff       (20)        0 2023-06-09 17:54:09.450405 gisting_test-0.1.5/gisting_test/
--rw-r--r--   0 owaiszahid   (501) staff       (20)       18 2023-06-01 17:36:38.000000 gisting_test-0.1.5/gisting_test/__init__.py
-drwxr-xr-x   0 owaiszahid   (501) staff       (20)        0 2023-06-09 17:54:09.453720 gisting_test-0.1.5/gisting_test/src/
--rw-r--r--   0 owaiszahid   (501) staff       (20)        0 2023-06-01 17:49:51.000000 gisting_test-0.1.5/gisting_test/src/__init__.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)    11076 2023-05-30 23:00:39.000000 gisting_test-0.1.5/gisting_test/src/arguments.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)     3462 2023-05-30 23:00:39.000000 gisting_test-0.1.5/gisting_test/src/benchmarking.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)     8769 2023-06-09 17:51:45.000000 gisting_test-0.1.5/gisting_test/src/compress.py
-drwxr-xr-x   0 owaiszahid   (501) staff       (20)        0 2023-06-09 17:54:09.454172 gisting_test-0.1.5/gisting_test/src/data/
--rw-r--r--   0 owaiszahid   (501) staff       (20)        0 2023-05-30 23:00:39.000000 gisting_test-0.1.5/gisting_test/src/data/__init__.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)     8550 2023-05-30 23:00:39.000000 gisting_test-0.1.5/gisting_test/src/data/gist.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)      554 2023-05-30 23:00:39.000000 gisting_test-0.1.5/gisting_test/src/data/utils.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)    21595 2023-05-30 23:00:39.000000 gisting_test-0.1.5/gisting_test/src/generation_utils.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)     4748 2023-05-30 23:00:39.000000 gisting_test-0.1.5/gisting_test/src/gist_caching.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)    34287 2023-05-30 23:00:39.000000 gisting_test-0.1.5/gisting_test/src/gist_llama.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)    41427 2023-05-30 23:00:39.000000 gisting_test-0.1.5/gisting_test/src/gist_t5.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)     2954 2023-05-30 23:00:39.000000 gisting_test-0.1.5/gisting_test/src/integrations.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)     4277 2023-05-30 23:00:39.000000 gisting_test-0.1.5/gisting_test/src/metrics.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)    13819 2023-05-30 23:00:39.000000 gisting_test-0.1.5/gisting_test/src/train.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)    52559 2023-05-30 23:00:39.000000 gisting_test-0.1.5/gisting_test/src/trainer_seq2seq.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)      426 2023-05-30 23:00:39.000000 gisting_test-0.1.5/gisting_test/src/utils.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)     7880 2023-05-30 23:00:39.000000 gisting_test-0.1.5/gisting_test/src/weight_diff.py
-drwxr-xr-x   0 owaiszahid   (501) staff       (20)        0 2023-06-09 17:54:09.450990 gisting_test-0.1.5/gisting_test.egg-info/
--rw-r--r--   0 owaiszahid   (501) staff       (20)      288 2023-06-09 17:54:09.000000 gisting_test-0.1.5/gisting_test.egg-info/PKG-INFO
--rw-r--r--   0 owaiszahid   (501) staff       (20)      703 2023-06-09 17:54:09.000000 gisting_test-0.1.5/gisting_test.egg-info/SOURCES.txt
--rw-r--r--   0 owaiszahid   (501) staff       (20)        1 2023-06-09 17:54:09.000000 gisting_test-0.1.5/gisting_test.egg-info/dependency_links.txt
--rw-r--r--   0 owaiszahid   (501) staff       (20)       52 2023-06-09 17:54:09.000000 gisting_test-0.1.5/gisting_test.egg-info/top_level.txt
--rw-r--r--   0 owaiszahid   (501) staff       (20)       38 2023-06-09 17:54:09.454518 gisting_test-0.1.5/setup.cfg
--rw-r--r--   0 owaiszahid   (501) staff       (20)      411 2023-06-09 17:53:24.000000 gisting_test-0.1.5/setup.py
+drwxr-xr-x   0 owaiszahid   (501) staff       (20)        0 2023-06-09 18:39:40.803686 gisting_test-0.1.6/
+-rw-r--r--   0 owaiszahid   (501) staff       (20)      288 2023-06-09 18:39:40.803573 gisting_test-0.1.6/PKG-INFO
+drwxr-xr-x   0 owaiszahid   (501) staff       (20)        0 2023-06-09 18:39:40.799250 gisting_test-0.1.6/gisting_test/
+-rw-r--r--   0 owaiszahid   (501) staff       (20)       18 2023-06-01 17:36:38.000000 gisting_test-0.1.6/gisting_test/__init__.py
+drwxr-xr-x   0 owaiszahid   (501) staff       (20)        0 2023-06-09 18:39:40.802909 gisting_test-0.1.6/gisting_test/src/
+-rw-r--r--   0 owaiszahid   (501) staff       (20)        0 2023-06-01 17:49:51.000000 gisting_test-0.1.6/gisting_test/src/__init__.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)    11076 2023-05-30 23:00:39.000000 gisting_test-0.1.6/gisting_test/src/arguments.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)     3462 2023-05-30 23:00:39.000000 gisting_test-0.1.6/gisting_test/src/benchmarking.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)     9051 2023-06-09 18:39:18.000000 gisting_test-0.1.6/gisting_test/src/compress.py
+drwxr-xr-x   0 owaiszahid   (501) staff       (20)        0 2023-06-09 18:39:40.803351 gisting_test-0.1.6/gisting_test/src/data/
+-rw-r--r--   0 owaiszahid   (501) staff       (20)        0 2023-05-30 23:00:39.000000 gisting_test-0.1.6/gisting_test/src/data/__init__.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)     8550 2023-05-30 23:00:39.000000 gisting_test-0.1.6/gisting_test/src/data/gist.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)      554 2023-05-30 23:00:39.000000 gisting_test-0.1.6/gisting_test/src/data/utils.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)    21595 2023-05-30 23:00:39.000000 gisting_test-0.1.6/gisting_test/src/generation_utils.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)     4748 2023-05-30 23:00:39.000000 gisting_test-0.1.6/gisting_test/src/gist_caching.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)    34287 2023-05-30 23:00:39.000000 gisting_test-0.1.6/gisting_test/src/gist_llama.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)    41427 2023-05-30 23:00:39.000000 gisting_test-0.1.6/gisting_test/src/gist_t5.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)     2954 2023-05-30 23:00:39.000000 gisting_test-0.1.6/gisting_test/src/integrations.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)     4277 2023-05-30 23:00:39.000000 gisting_test-0.1.6/gisting_test/src/metrics.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)    13819 2023-05-30 23:00:39.000000 gisting_test-0.1.6/gisting_test/src/train.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)    52559 2023-05-30 23:00:39.000000 gisting_test-0.1.6/gisting_test/src/trainer_seq2seq.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)      426 2023-05-30 23:00:39.000000 gisting_test-0.1.6/gisting_test/src/utils.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)     7880 2023-05-30 23:00:39.000000 gisting_test-0.1.6/gisting_test/src/weight_diff.py
+drwxr-xr-x   0 owaiszahid   (501) staff       (20)        0 2023-06-09 18:39:40.799794 gisting_test-0.1.6/gisting_test.egg-info/
+-rw-r--r--   0 owaiszahid   (501) staff       (20)      288 2023-06-09 18:39:40.000000 gisting_test-0.1.6/gisting_test.egg-info/PKG-INFO
+-rw-r--r--   0 owaiszahid   (501) staff       (20)      703 2023-06-09 18:39:40.000000 gisting_test-0.1.6/gisting_test.egg-info/SOURCES.txt
+-rw-r--r--   0 owaiszahid   (501) staff       (20)        1 2023-06-09 18:39:40.000000 gisting_test-0.1.6/gisting_test.egg-info/dependency_links.txt
+-rw-r--r--   0 owaiszahid   (501) staff       (20)       52 2023-06-09 18:39:40.000000 gisting_test-0.1.6/gisting_test.egg-info/top_level.txt
+-rw-r--r--   0 owaiszahid   (501) staff       (20)       38 2023-06-09 18:39:40.803722 gisting_test-0.1.6/setup.cfg
+-rw-r--r--   0 owaiszahid   (501) staff       (20)      411 2023-06-09 18:39:33.000000 gisting_test-0.1.6/setup.py
```

### Comparing `gisting_test-0.1.5/gisting_test/src/arguments.py` & `gisting_test-0.1.6/gisting_test/src/arguments.py`

 * *Files identical despite different names*

### Comparing `gisting_test-0.1.5/gisting_test/src/benchmarking.py` & `gisting_test-0.1.6/gisting_test/src/benchmarking.py`

 * *Files identical despite different names*

### Comparing `gisting_test-0.1.5/gisting_test/src/compress.py` & `gisting_test-0.1.6/gisting_test/src/compress.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 """Gist compression demo."""
 
 from typing import Optional
 
 import fire
 import torch
-from transformers import AutoConfig, AutoTokenizer, LlamaTokenizer
+from transformers import AutoConfig, AutoTokenizer, LlamaTokenizer, BitsAndBytesConfig , StoppingCriteria, StoppingCriteriaList
+
+quantization_config = BitsAndBytesConfig(
+    load_in_8bit=True,
+    llm_int8_threshold=6.0,
+)
 
 from . import gist_llama, gist_t5, weight_diff
 from .gist_llama import GistLlamaForCausalLM
 from .gist_t5 import GistT5ForConditionalGeneration
 
 
 def humanbytes(B):
@@ -96,25 +101,28 @@
             path_diff=model_name_or_path,
             test_inference=False,
             cache_dir=cache_dir,
         )
     else:
         model = model_cls.from_pretrained(
             model_name_or_path,
+            torch_dtype=torch.bfloat16,
             config=config,
+            quantization_config=quantization_config,
+            load_in_8bit=True,
             cache_dir=cache_dir,
             device_map = "auto"
         )
 
     dtypes = {
         "bf16": torch.bfloat16,
         "fp16": torch.float16,
         "fp32": torch.float,
     }
-    model = model.to(dtypes[precision]).cuda().eval()
+    #model = model.to(dtypes[precision]).cuda().eval()
 
     # Load tokenizer. It must already have gist token defined.
     print("Loading tokenizer")
     if is_llama:
         tokenizer = LlamaTokenizer.from_pretrained(model_name_or_path)
         tokenizer.pad_token = tokenizer.eos_token
         tokenizer.padding_side = "left"
```

### Comparing `gisting_test-0.1.5/gisting_test/src/data/gist.py` & `gisting_test-0.1.6/gisting_test/src/data/gist.py`

 * *Files identical despite different names*

### Comparing `gisting_test-0.1.5/gisting_test/src/data/utils.py` & `gisting_test-0.1.6/gisting_test/src/data/utils.py`

 * *Files identical despite different names*

### Comparing `gisting_test-0.1.5/gisting_test/src/generation_utils.py` & `gisting_test-0.1.6/gisting_test/src/generation_utils.py`

 * *Files identical despite different names*

### Comparing `gisting_test-0.1.5/gisting_test/src/gist_caching.py` & `gisting_test-0.1.6/gisting_test/src/gist_caching.py`

 * *Files identical despite different names*

### Comparing `gisting_test-0.1.5/gisting_test/src/gist_llama.py` & `gisting_test-0.1.6/gisting_test/src/gist_llama.py`

 * *Files identical despite different names*

### Comparing `gisting_test-0.1.5/gisting_test/src/gist_t5.py` & `gisting_test-0.1.6/gisting_test/src/gist_t5.py`

 * *Files identical despite different names*

### Comparing `gisting_test-0.1.5/gisting_test/src/integrations.py` & `gisting_test-0.1.6/gisting_test/src/integrations.py`

 * *Files identical despite different names*

### Comparing `gisting_test-0.1.5/gisting_test/src/metrics.py` & `gisting_test-0.1.6/gisting_test/src/metrics.py`

 * *Files identical despite different names*

### Comparing `gisting_test-0.1.5/gisting_test/src/train.py` & `gisting_test-0.1.6/gisting_test/src/train.py`

 * *Files identical despite different names*

### Comparing `gisting_test-0.1.5/gisting_test/src/trainer_seq2seq.py` & `gisting_test-0.1.6/gisting_test/src/trainer_seq2seq.py`

 * *Files identical despite different names*

### Comparing `gisting_test-0.1.5/gisting_test/src/weight_diff.py` & `gisting_test-0.1.6/gisting_test/src/weight_diff.py`

 * *Files identical despite different names*

### Comparing `gisting_test-0.1.5/gisting_test.egg-info/SOURCES.txt` & `gisting_test-0.1.6/gisting_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

