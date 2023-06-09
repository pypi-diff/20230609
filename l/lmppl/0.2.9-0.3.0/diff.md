# Comparing `tmp/lmppl-0.2.9.tar.gz` & `tmp/lmppl-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmppl-0.2.9.tar", last modified: Tue May 16 11:35:52 2023, max compression
+gzip compressed data, was "lmppl-0.3.0.tar", last modified: Fri Jun  9 18:33:52 2023, max compression
```

## Comparing `lmppl-0.2.9.tar` & `lmppl-0.3.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-05-16 11:35:52.669463 lmppl-0.2.9/
--rw-r--r--   0 asahi      (501) staff       (20)     1064 2023-02-07 11:28:13.000000 lmppl-0.2.9/LICENSE.txt
--rw-r--r--   0 asahi      (501) staff       (20)     5200 2023-05-16 11:35:52.669600 lmppl-0.2.9/PKG-INFO
--rw-r--r--   0 asahi      (501) staff       (20)     4437 2023-02-09 18:23:49.000000 lmppl-0.2.9/README.md
-drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-05-16 11:35:52.666670 lmppl-0.2.9/lmppl/
--rw-r--r--   0 asahi      (501) staff       (20)      150 2023-04-05 16:38:19.000000 lmppl-0.2.9/lmppl/__init__.py
-drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-05-16 11:35:52.668318 lmppl-0.2.9/lmppl/lmppl_cl/
--rw-r--r--   0 asahi      (501) staff       (20)        0 2023-02-07 11:25:50.000000 lmppl-0.2.9/lmppl/lmppl_cl/__init__.py
--rw-r--r--   0 asahi      (501) staff       (20)     2688 2023-05-12 20:52:46.000000 lmppl-0.2.9/lmppl/openai_models.py
--rw-r--r--   0 asahi      (501) staff       (20)     8992 2023-05-16 11:35:34.000000 lmppl-0.2.9/lmppl/ppl_encoder_decoder_lm.py
--rw-r--r--   0 asahi      (501) staff       (20)     7128 2023-05-16 11:35:00.000000 lmppl-0.2.9/lmppl/ppl_mlm.py
--rw-r--r--   0 asahi      (501) staff       (20)     5954 2023-05-16 11:34:43.000000 lmppl-0.2.9/lmppl/ppl_recurrent_lm.py
--rw-r--r--   0 asahi      (501) staff       (20)      227 2023-02-07 13:19:37.000000 lmppl-0.2.9/lmppl/util.py
-drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-05-16 11:35:52.668107 lmppl-0.2.9/lmppl.egg-info/
--rw-r--r--   0 asahi      (501) staff       (20)     5200 2023-05-16 11:35:52.000000 lmppl-0.2.9/lmppl.egg-info/PKG-INFO
--rw-r--r--   0 asahi      (501) staff       (20)      399 2023-05-16 11:35:52.000000 lmppl-0.2.9/lmppl.egg-info/SOURCES.txt
--rw-r--r--   0 asahi      (501) staff       (20)        1 2023-05-16 11:35:52.000000 lmppl-0.2.9/lmppl.egg-info/dependency_links.txt
--rw-r--r--   0 asahi      (501) staff       (20)       79 2023-05-16 11:35:52.000000 lmppl-0.2.9/lmppl.egg-info/requires.txt
--rw-r--r--   0 asahi      (501) staff       (20)        6 2023-05-16 11:35:52.000000 lmppl-0.2.9/lmppl.egg-info/top_level.txt
--rw-r--r--   0 asahi      (501) staff       (20)       38 2023-05-16 11:35:52.670075 lmppl-0.2.9/setup.cfg
--rw-r--r--   0 asahi      (501) staff       (20)     1760 2023-05-16 11:35:38.000000 lmppl-0.2.9/setup.py
-drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-05-16 11:35:52.669185 lmppl-0.2.9/test/
--rw-r--r--   0 asahi      (501) staff       (20)     1249 2023-02-09 19:14:51.000000 lmppl-0.2.9/test/test_analogy.py
--rw-r--r--   0 asahi      (501) staff       (20)     2261 2023-02-12 13:50:45.000000 lmppl-0.2.9/test/test_model_with_simple_input.py
+drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-06-09 18:33:52.507824 lmppl-0.3.0/
+-rw-r--r--   0 asahi      (501) staff       (20)     1064 2023-02-07 11:28:13.000000 lmppl-0.3.0/LICENSE.txt
+-rw-r--r--   0 asahi      (501) staff       (20)     5200 2023-06-09 18:33:52.508050 lmppl-0.3.0/PKG-INFO
+-rw-r--r--   0 asahi      (501) staff       (20)     4437 2023-02-09 18:23:49.000000 lmppl-0.3.0/README.md
+drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-06-09 18:33:52.503419 lmppl-0.3.0/lmppl/
+-rw-r--r--   0 asahi      (501) staff       (20)      150 2023-04-05 16:38:19.000000 lmppl-0.3.0/lmppl/__init__.py
+drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-06-09 18:33:52.505833 lmppl-0.3.0/lmppl/lmppl_cl/
+-rw-r--r--   0 asahi      (501) staff       (20)        0 2023-02-07 11:25:50.000000 lmppl-0.3.0/lmppl/lmppl_cl/__init__.py
+-rw-r--r--   0 asahi      (501) staff       (20)     2688 2023-05-12 20:52:46.000000 lmppl-0.3.0/lmppl/openai_models.py
+-rw-r--r--   0 asahi      (501) staff       (20)     9585 2023-06-09 18:33:17.000000 lmppl-0.3.0/lmppl/ppl_encoder_decoder_lm.py
+-rw-r--r--   0 asahi      (501) staff       (20)     7128 2023-05-16 11:35:00.000000 lmppl-0.3.0/lmppl/ppl_mlm.py
+-rw-r--r--   0 asahi      (501) staff       (20)     6589 2023-06-09 18:24:04.000000 lmppl-0.3.0/lmppl/ppl_recurrent_lm.py
+-rw-r--r--   0 asahi      (501) staff       (20)      227 2023-02-07 13:19:37.000000 lmppl-0.3.0/lmppl/util.py
+drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-06-09 18:33:52.505413 lmppl-0.3.0/lmppl.egg-info/
+-rw-r--r--   0 asahi      (501) staff       (20)     5200 2023-06-09 18:33:52.000000 lmppl-0.3.0/lmppl.egg-info/PKG-INFO
+-rw-r--r--   0 asahi      (501) staff       (20)      399 2023-06-09 18:33:52.000000 lmppl-0.3.0/lmppl.egg-info/SOURCES.txt
+-rw-r--r--   0 asahi      (501) staff       (20)        1 2023-06-09 18:33:52.000000 lmppl-0.3.0/lmppl.egg-info/dependency_links.txt
+-rw-r--r--   0 asahi      (501) staff       (20)       79 2023-06-09 18:33:52.000000 lmppl-0.3.0/lmppl.egg-info/requires.txt
+-rw-r--r--   0 asahi      (501) staff       (20)        6 2023-06-09 18:33:52.000000 lmppl-0.3.0/lmppl.egg-info/top_level.txt
+-rw-r--r--   0 asahi      (501) staff       (20)       38 2023-06-09 18:33:52.508580 lmppl-0.3.0/setup.cfg
+-rw-r--r--   0 asahi      (501) staff       (20)     1760 2023-06-09 18:33:24.000000 lmppl-0.3.0/setup.py
+drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-06-09 18:33:52.507398 lmppl-0.3.0/test/
+-rw-r--r--   0 asahi      (501) staff       (20)     1249 2023-02-09 19:14:51.000000 lmppl-0.3.0/test/test_analogy.py
+-rw-r--r--   0 asahi      (501) staff       (20)     2261 2023-02-12 13:50:45.000000 lmppl-0.3.0/test/test_model_with_simple_input.py
```

### Comparing `lmppl-0.2.9/LICENSE.txt` & `lmppl-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lmppl-0.2.9/PKG-INFO` & `lmppl-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: lmppl
-Version: 0.2.9
+Version: 0.3.0
 Summary: Calculate perplexity on the text with pre-trained language models.
 Home-page: https://github.com/asahi417/lmppl
 Author: Asahi Ushio
 Author-email: asahi1992ushio@gmail.com
 License: MIT License
-Download-URL: https://github.com/asahi417/lmppl/archive/v0.2.9.tar.gz
+Download-URL: https://github.com/asahi417/lmppl/archive/v0.3.0.tar.gz
 Keywords: language model,t5,gpt3,bert,perplexity,nlp
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lmppl-0.2.9/README.md` & `lmppl-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `lmppl-0.2.9/lmppl/openai_models.py` & `lmppl-0.3.0/lmppl/openai_models.py`

 * *Files identical despite different names*

### Comparing `lmppl-0.2.9/lmppl/ppl_encoder_decoder_lm.py` & `lmppl-0.3.0/lmppl/ppl_encoder_decoder_lm.py`

 * *Files 6% similar despite different names*

```diff
@@ -96,16 +96,21 @@
 
         # load model
         self.device_map = device_map
         self.tokenizer, self.model, self.config = get_lm(
             model, use_auth_token=use_auth_token, torch_dtype=torch_dtype, device_map=self.device_map,
             low_cpu_mem_usage=low_cpu_mem_usage, hf_cache_dir=hf_cache_dir, trust_remote_code=trust_remote_code,
             offload_folder=offload_folder)
+
+        self.pad_token_initialized = False
         if self.tokenizer.pad_token is None:
-            self.tokenizer.pad_token = "<<PAD>>"
+            self.tokenizer.add_special_tokens({'pad_token': "<<PAD>>"})
+            self.model.resize_token_embeddings(len(self.tokenizer))
+            self.pad_token_initialized = True
+
         if max_length_encoder is None:
             self.max_length_encoder = None
         else:
             self.max_length_encoder = max_length_encoder if max_length_encoder is not None else self.tokenizer.model_max_length
             assert self.max_length_encoder <= self.tokenizer.model_max_length, f"{self.max_length_encoder} > {self.tokenizer.model_max_length}"
         if max_length_decoder is None:
             self.max_length_decoder = None
@@ -174,23 +179,35 @@
                     output = self.model(**{k: v.to(self.device) for k, v in model_inputs.items()})
                 else:
                     model_inputs["labels"] = label
                     output = self.model(**{k: v.cuda() for k, v in model_inputs.items()})
                     model_inputs["labels"] = label.to(self.device)
 
                 # model run & loss conversion into likelihood
+                logits = output['logits']
+                if self.pad_token_initialized:
+                    logits = logits[:, :, :-1]
                 valid_length = (model_inputs["labels"] != PAD_TOKEN_LABEL_ID).sum(dim=-1)
-                loss = self.loss_fct(output['logits'].view(-1, self.config.vocab_size), model_inputs["labels"].view(-1))
-                loss = loss.view(len(output['logits']), -1)
+                loss = self.loss_fct(logits.view(-1, self.config.vocab_size), model_inputs["labels"].view(-1))
+                loss = loss.view(len(logits), -1)
                 loss = torch.sum(loss, -1) / valid_length
                 loss_list += loss.cpu().tolist()
 
                 if FORCE_RESET:
                     del model_inputs
                     del loss
                     del output
                     gc.collect()
                     torch.cuda.empty_cache()
 
         # conversion to perplexity
         ppl = [exp(i) for i in loss_list]
         return ppl[0] if single_input else ppl
+
+
+if __name__ == '__main__':
+
+    # scorer = LM("gpt2")
+    scorer = EncoderDecoderLM("t5-small")
+    _x = 'sentiment classification: I dropped my laptop on my knee, and someone stole my coffee.'
+    print(scorer.get_perplexity(input_texts=[_x] * 2, output_texts=['I am happy.', 'I am sad.']))
+
```

### Comparing `lmppl-0.2.9/lmppl/ppl_mlm.py` & `lmppl-0.3.0/lmppl/ppl_mlm.py`

 * *Files identical despite different names*

### Comparing `lmppl-0.2.9/lmppl/ppl_recurrent_lm.py` & `lmppl-0.3.0/lmppl/ppl_recurrent_lm.py`

 * *Files 13% similar despite different names*

```diff
@@ -63,17 +63,19 @@
         params.update({"config": self.config, "low_cpu_mem_usage": low_cpu_mem_usage})
         if torch_dtype is not None:
             params['torch_dtype'] = torch_dtype
         if device_map is not None:
             params['device_map'] = device_map
         self.model = transformers.AutoModelForCausalLM.from_pretrained(model, **params)
 
+        self.pad_token_initialized = False
         if self.tokenizer.pad_token is None:
             self.tokenizer.add_special_tokens({'pad_token': "<<PAD>>"})
             self.model.resize_token_embeddings(len(self.tokenizer))
+            self.pad_token_initialized = True
 
         if max_length is None:
             self.max_length = None
         else:
             self.max_length = max_length if max_length is not None else self.tokenizer.model_max_length
             assert self.max_length <= self.tokenizer.model_max_length, f"{self.max_length} > {self.tokenizer.model_max_length}"
 
@@ -114,36 +116,51 @@
             for s, e in tqdm(batch_id):
 
                 # run model inference
                 if self.max_length is not None:
                     model_inputs = self.tokenizer(input_texts[s:e], max_length=self.max_length, truncation=True, padding='max_length', return_tensors='pt')
                 else:
                     model_inputs = self.tokenizer(input_texts[s:e], truncation=True, padding=True, return_tensors='pt')
-
                 if 'token_type_ids' in model_inputs:
                     model_inputs.pop('token_type_ids')
 
                 output = self.model(**{k: v.to(self.device) for k, v in model_inputs.items()})
+                logit = output['logits']
+                if self.pad_token_initialized:
+                    logit = logit[:, :, :-1]
 
                 # shift the label sequence for causal inference
                 label = model_inputs['input_ids']
                 label[label == self.tokenizer.pad_token_id] = PAD_TOKEN_LABEL_ID
-                label = torch.concat([label[:, 1:], torch.tensor([[PAD_TOKEN_LABEL_ID] * label.shape[0]]).T], dim=1).to(self.device)
+
+                # Shift so that tokens < n predict n
+                shift_logits = logit[..., :-1, :].contiguous()
+                shift_label = label[:, 1:].contiguous()
 
                 # compute loss
-                valid_length = (label != PAD_TOKEN_LABEL_ID).sum(dim=-1)
-                loss = self.loss_fct(output['logits'].view(-1, self.config.vocab_size), label.view(-1))
+                valid_length = (shift_label != PAD_TOKEN_LABEL_ID).sum(dim=-1)
+                loss = self.loss_fct(shift_logits.view(-1, shift_logits.size(-1)), shift_label.view(-1))
                 loss = loss.view(len(output['logits']), -1)
                 loss = torch.sum(loss, -1) / valid_length
                 loss_list += loss.cpu().tolist()
 
                 if FORCE_RESET:
                     del model_inputs
                     del loss
                     del output
                     gc.collect()
                     torch.cuda.empty_cache()
 
-
         # conversion to perplexity
         ppl = [exp(i) for i in loss_list]
         return ppl[0] if single_input else ppl
+
+
+if __name__ == '__main__':
+
+    # scorer = LM("gpt2")
+    scorer = LM("facebook/opt-125m")
+    text = [
+        'sentiment classification: I dropped my laptop on my knee, and someone stole my coffee. I am happy.',
+        'sentiment classification: I dropped my laptop on my knee, and someone stole my coffee. I am sad.'
+    ]
+    print(scorer.get_perplexity(text))
```

### Comparing `lmppl-0.2.9/lmppl.egg-info/PKG-INFO` & `lmppl-0.3.0/lmppl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: lmppl
-Version: 0.2.9
+Version: 0.3.0
 Summary: Calculate perplexity on the text with pre-trained language models.
 Home-page: https://github.com/asahi417/lmppl
 Author: Asahi Ushio
 Author-email: asahi1992ushio@gmail.com
 License: MIT License
-Download-URL: https://github.com/asahi417/lmppl/archive/v0.2.9.tar.gz
+Download-URL: https://github.com/asahi417/lmppl/archive/v0.3.0.tar.gz
 Keywords: language model,t5,gpt3,bert,perplexity,nlp
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lmppl-0.2.9/setup.py` & `lmppl-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     readme = f.read()
-VERSION = '0.2.9'
+VERSION = '0.3.0'
 NAME = 'lmppl'
 LICENSE = 'MIT License'
 setup(
     name=NAME,
     packages=find_packages(exclude=['tests', 'misc', 'asset']),
     version=VERSION,
     license=LICENSE,
```

### Comparing `lmppl-0.2.9/test/test_analogy.py` & `lmppl-0.3.0/test/test_analogy.py`

 * *Files identical despite different names*

### Comparing `lmppl-0.2.9/test/test_model_with_simple_input.py` & `lmppl-0.3.0/test/test_model_with_simple_input.py`

 * *Files identical despite different names*

