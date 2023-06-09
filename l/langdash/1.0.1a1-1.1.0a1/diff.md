# Comparing `tmp/langdash-1.0.1a1.tar.gz` & `tmp/langdash-1.1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langdash-1.0.1a1.tar", last modified: Thu Jun  8 05:13:08 2023, max compression
+gzip compressed data, was "langdash-1.1.0a1.tar", last modified: Fri Jun  9 06:59:32 2023, max compression
```

## Comparing `langdash-1.0.1a1.tar` & `langdash-1.1.0a1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-08 05:13:08.089345 langdash-1.0.1a1/
--rw-rw-r--   0 user      (1000) user      (1000)    10786 2023-05-30 02:56:17.000000 langdash-1.0.1a1/LICENSE.txt
--rw-rw-r--   0 user      (1000) user      (1000)       35 2023-05-31 17:16:19.000000 langdash-1.0.1a1/MANIFEST.in
--rw-rw-r--   0 user      (1000) user      (1000)     2713 2023-06-08 05:13:08.089345 langdash-1.0.1a1/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1804 2023-06-08 05:12:48.000000 langdash-1.0.1a1/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-08 05:13:08.089345 langdash-1.0.1a1/langdash/
--rw-rw-r--   0 user      (1000) user      (1000)       64 2023-06-08 05:11:44.000000 langdash-1.0.1a1/langdash/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    21883 2023-06-07 02:26:23.000000 langdash-1.0.1a1/langdash/chains.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-08 05:13:08.085345 langdash-1.0.1a1/langdash/classify/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:31.000000 langdash-1.0.1a1/langdash/classify/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1973 2023-06-06 03:06:05.000000 langdash-1.0.1a1/langdash/classify/token_qa.py
--rw-rw-r--   0 user      (1000) user      (1000)     6224 2023-06-07 02:26:23.000000 langdash-1.0.1a1/langdash/core.py
--rw-rw-r--   0 user      (1000) user      (1000)      779 2023-06-06 03:06:05.000000 langdash-1.0.1a1/langdash/infer.py
--rw-rw-r--   0 user      (1000) user      (1000)     1555 2023-06-06 03:06:05.000000 langdash-1.0.1a1/langdash/llm.py
--rw-rw-r--   0 user      (1000) user      (1000)     7006 2023-06-07 02:26:23.000000 langdash-1.0.1a1/langdash/llm_session.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-08 05:13:08.089345 langdash-1.0.1a1/langdash/models/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-04 22:40:10.000000 langdash-1.0.1a1/langdash/models/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1886 2023-06-06 03:06:05.000000 langdash-1.0.1a1/langdash/models/_bpe.py
--rw-rw-r--   0 user      (1000) user      (1000)     6418 2023-06-07 19:42:20.000000 langdash-1.0.1a1/langdash/models/llama_cpp.py
--rw-rw-r--   0 user      (1000) user      (1000)      689 2023-06-06 03:06:05.000000 langdash-1.0.1a1/langdash/models/mock.py
--rw-rw-r--   0 user      (1000) user      (1000)     7973 2023-06-07 02:26:23.000000 langdash-1.0.1a1/langdash/models/rwkv_cpp.py
--rw-rw-r--   0 user      (1000) user      (1000)      989 2023-06-07 02:26:23.000000 langdash-1.0.1a1/langdash/models/sentence_transformers.py
--rw-rw-r--   0 user      (1000) user      (1000)     6920 2023-06-07 02:26:23.000000 langdash-1.0.1a1/langdash/models/transformers.py
--rw-rw-r--   0 user      (1000) user      (1000)      837 2023-06-06 03:06:05.000000 langdash-1.0.1a1/langdash/response.py
--rw-rw-r--   0 user      (1000) user      (1000)     2577 2023-06-06 03:06:05.000000 langdash-1.0.1a1/langdash/sampling.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-08 05:13:08.089345 langdash-1.0.1a1/langdash/search/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:40.000000 langdash-1.0.1a1/langdash/search/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1117 2023-06-07 02:26:23.000000 langdash-1.0.1a1/langdash/search/embedding_search.py
--rw-rw-r--   0 user      (1000) user      (1000)      947 2023-06-07 02:26:23.000000 langdash-1.0.1a1/langdash/search/engine.py
--rw-rw-r--   0 user      (1000) user      (1000)     2787 2023-06-07 02:26:23.000000 langdash-1.0.1a1/langdash/search/multichoice_search.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-08 05:13:08.089345 langdash-1.0.1a1/langdash.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)     2713 2023-06-08 05:13:08.000000 langdash-1.0.1a1/langdash.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1239 2023-06-08 05:13:08.000000 langdash-1.0.1a1/langdash.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-06-08 05:13:08.000000 langdash-1.0.1a1/langdash.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)      167 2023-06-08 05:13:08.000000 langdash-1.0.1a1/langdash.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        9 2023-06-08 05:13:08.000000 langdash-1.0.1a1/langdash.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-06-08 05:13:08.089345 langdash-1.0.1a1/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1560 2023-06-07 02:26:23.000000 langdash-1.0.1a1/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-09 06:59:32.296508 langdash-1.1.0a1/
+-rw-rw-r--   0 user      (1000) user      (1000)    10786 2023-05-30 02:56:17.000000 langdash-1.1.0a1/LICENSE.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       35 2023-05-31 17:16:19.000000 langdash-1.1.0a1/MANIFEST.in
+-rw-rw-r--   0 user      (1000) user      (1000)     2713 2023-06-09 06:59:32.296508 langdash-1.1.0a1/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1804 2023-06-08 05:12:48.000000 langdash-1.1.0a1/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-09 06:59:32.296508 langdash-1.1.0a1/langdash/
+-rw-rw-r--   0 user      (1000) user      (1000)       64 2023-06-09 06:59:24.000000 langdash-1.1.0a1/langdash/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    22212 2023-06-09 06:56:17.000000 langdash-1.1.0a1/langdash/chains.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-09 06:59:32.292508 langdash-1.1.0a1/langdash/classify/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:31.000000 langdash-1.1.0a1/langdash/classify/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1973 2023-06-06 03:06:05.000000 langdash-1.1.0a1/langdash/classify/token_qa.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6224 2023-06-07 02:26:23.000000 langdash-1.1.0a1/langdash/core.py
+-rw-rw-r--   0 user      (1000) user      (1000)      793 2023-06-09 06:56:17.000000 langdash-1.1.0a1/langdash/infer.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1555 2023-06-06 03:06:05.000000 langdash-1.1.0a1/langdash/llm.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7006 2023-06-07 02:26:23.000000 langdash-1.1.0a1/langdash/llm_session.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-09 06:59:32.296508 langdash-1.1.0a1/langdash/models/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-04 22:40:10.000000 langdash-1.1.0a1/langdash/models/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1886 2023-06-06 03:06:05.000000 langdash-1.1.0a1/langdash/models/_bpe.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6492 2023-06-09 06:56:17.000000 langdash-1.1.0a1/langdash/models/llama_cpp.py
+-rw-rw-r--   0 user      (1000) user      (1000)      689 2023-06-06 03:06:05.000000 langdash-1.1.0a1/langdash/models/mock.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7973 2023-06-07 02:26:23.000000 langdash-1.1.0a1/langdash/models/rwkv_cpp.py
+-rw-rw-r--   0 user      (1000) user      (1000)      989 2023-06-07 02:26:23.000000 langdash-1.1.0a1/langdash/models/sentence_transformers.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7460 2023-06-09 06:56:17.000000 langdash-1.1.0a1/langdash/models/transformers.py
+-rw-rw-r--   0 user      (1000) user      (1000)      837 2023-06-06 03:06:05.000000 langdash-1.1.0a1/langdash/response.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2759 2023-06-09 06:56:17.000000 langdash-1.1.0a1/langdash/sampling.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-09 06:59:32.296508 langdash-1.1.0a1/langdash/search/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:40.000000 langdash-1.1.0a1/langdash/search/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1120 2023-06-09 06:56:17.000000 langdash-1.1.0a1/langdash/search/embedding_search.py
+-rw-rw-r--   0 user      (1000) user      (1000)      984 2023-06-09 06:56:17.000000 langdash-1.1.0a1/langdash/search/engine.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2821 2023-06-09 06:56:17.000000 langdash-1.1.0a1/langdash/search/multichoice_search.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-09 06:59:32.296508 langdash-1.1.0a1/langdash.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)     2713 2023-06-09 06:59:32.000000 langdash-1.1.0a1/langdash.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1239 2023-06-09 06:59:32.000000 langdash-1.1.0a1/langdash.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-06-09 06:59:32.000000 langdash-1.1.0a1/langdash.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      167 2023-06-09 06:59:32.000000 langdash-1.1.0a1/langdash.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        9 2023-06-09 06:59:32.000000 langdash-1.1.0a1/langdash.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-06-09 06:59:32.296508 langdash-1.1.0a1/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1560 2023-06-07 02:26:23.000000 langdash-1.1.0a1/setup.py
```

### Comparing `langdash-1.0.1a1/LICENSE.txt` & `langdash-1.1.0a1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `langdash-1.0.1a1/PKG-INFO` & `langdash-1.1.0a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langdash
-Version: 1.0.1a1
+Version: 1.1.0a1
 Summary: A simple library for interfacing with language models.
 Home-page: https://git.mysymphony.jp.net/nana/langdash
 Author: Nana Mochizuki
 Author-email: nana@mysymphony.jp.net
 Project-URL: Source, https://git.mysymphony.jp.net/nana/langdash
 Project-URL: Documentation, https://langdash.readthedocs.io/en/latest/
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `langdash-1.0.1a1/README.md` & `langdash-1.1.0a1/README.md`

 * *Files identical despite different names*

### Comparing `langdash-1.0.1a1/langdash/chains.py` & `langdash-1.1.0a1/langdash/chains.py`

 * *Files 2% similar despite different names*

```diff
@@ -283,16 +283,15 @@
     Args:
       cache_store (LDChainCacheStore): The cache store.
     """
     if self._model != cache_store._model:
       raise ValueError("model mismatch for LDChainCacheStore")
     if self._model_kwargs != cache_store._model_kwargs:
       warnings.warn(
-        "model kwargs does not match LDChainCacheStore, unexpected behavior might occur",
-        UserWarning
+        "model kwargs does not match LDChainCacheStore, unexpected behavior might occur"
       )
     self._state_cache = cache_store._dict
 
   def save_cache_store(self) -> LDChainCacheStore:
     """ Saves the cache store into an object. """
     return LDChainCacheStore(
       _dict=copy.deepcopy(self._state_cache),
@@ -498,25 +497,30 @@
   ) -> LDNodeGenerator:
     raise NotImplementedError("__call__")
 
 
 class LDText(LDNode):
   """ Constant text node """
 
-  def __init__(self, ld: "Langdash", text: str):
+  def __init__(
+    self, ld: "Langdash", text: str, add_special_tokens: bool = False
+  ):
     super().__init__(ld)
     self._text = text
+    self._add_special_tokens = add_special_tokens
 
   def __repr__(self):
     return f"<Text>\n{self._text}\n</Text>"
 
   def __call__(
     self, session: "LLMGenerationSession", args: LDNodeArgs
   ) -> LDNodeGenerator:
-    tokens_counter = session.inject(self._text)
+    tokens_counter = session.inject(
+      self._text, add_special_tokens=self._add_special_tokens
+    )
     yield RespInject(tokens_counter=tokens_counter)
 
 
 class LDFormatArg(LDNode):
   """ Format argument node """
 
   def __init__(self, ld: "Langdash", text: str):
@@ -588,14 +592,17 @@
   ) -> LDNodeGenerator:
     for i, respinfer in enumerate(
       session.infer(end=self._end, args=self._infer_args)
     ):
       if i == 0:
         if self._padleft and respinfer.tokstr.startswith(self._padleft):
           respinfer.tokstr = respinfer.tokstr[len(self._padleft):]
+      elif respinfer.tokid == -1: # end
+        if self._padleft and respinfer.running_infer.startswith(self._padleft):
+          respinfer.running_infer = respinfer.running_infer[len(self._padleft):]
       yield respinfer
 
 
 class LDChoice(LDNode):
   """ Choice node """
 
   def __init__(
```

### Comparing `langdash-1.0.1a1/langdash/classify/token_qa.py` & `langdash-1.1.0a1/langdash/classify/token_qa.py`

 * *Files identical despite different names*

### Comparing `langdash-1.0.1a1/langdash/core.py` & `langdash-1.1.0a1/langdash/core.py`

 * *Files identical despite different names*

### Comparing `langdash-1.0.1a1/langdash/infer.py` & `langdash-1.1.0a1/langdash/infer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from dataclasses import dataclass
+import warnings
 
 
 @dataclass
 class InferArgs:
   """
   Data class for inference arguments.
   
@@ -14,11 +15,11 @@
     typical_mass: Mass parameter. If set, generation will use typical sampling
     max_rep_ctx: Maximum number of tokens to look back for repetition penalty
     rep_penalty: Repetition penalty, applied to logits for every token
   """
   min_new_tokens: int = 0
   max_new_tokens: int = 512
   temperature: float = 1.0
-  top_p: float = 0.0
-  typical_mass: float = 0.0
+  top_p: float = 0.
+  typical_mass: float = 0.
   max_rep_ctx: int = 64
   rep_penalty: float = 1.0
```

### Comparing `langdash-1.0.1a1/langdash/llm.py` & `langdash-1.1.0a1/langdash/llm.py`

 * *Files identical despite different names*

### Comparing `langdash-1.0.1a1/langdash/llm_session.py` & `langdash-1.1.0a1/langdash/llm_session.py`

 * *Files identical despite different names*

### Comparing `langdash-1.0.1a1/langdash/models/_bpe.py` & `langdash-1.1.0a1/langdash/models/_bpe.py`

 * *Files identical despite different names*

### Comparing `langdash-1.0.1a1/langdash/models/llama_cpp.py` & `langdash-1.1.0a1/langdash/models/llama_cpp.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 
   def _eval(self, token: int):
     return self._llama.eval([token])
 
   def _eval_mult(self, tokens: List[int]):
     return self._llama.eval(tokens)
 
-  def _next_token_probs(self):
+  def next_token_probs(self):
     if self._next_token is None:
       if self._logits is None:
         raise ValueError("cannot predict next probability for empty input")
       logits = self._logits
     else:
       logits = self._eval(self._next_token[0])
     return sampling.logits_to_probs(logits).tolist()
@@ -118,15 +118,14 @@
   def _on_first_inject(self):
     self._llama.model.reset()
     self._eval(self._bos_token)
 
   def _infer(self, end: Optional[Union[str, int]],
              args: InferArgs) -> Generator[RespInfer, None, None]:
     generated = ""
-    ctx: List[int] = []
     buffered_tokens = b""
 
     if isinstance(end, str):
       if len(end) == 0:
         end = self._eos_token
       elif args.min_new_tokens > 0:
         endtoks = self.tokenize(end)
@@ -155,16 +154,15 @@
         self._next_token = None
 
       if end != self._eos_token:  # no early endoftext
         self._logits[self._eos_token] = -inf
       elif args.min_new_tokens > 0 and i < args.min_new_tokens:
         self._logits[end] = -inf
 
-      tokid = sampling.sample(self._logits, args, ctx)
-      ctx.append(tokid)
+      tokid = sampling.sample(self._logits, args, self._llama.model.eval_tokens)
 
       if tokid == end:  # implies end is int
         break
 
       tokstr_b = self._llama.vocab[tokid]
 
       try:
@@ -187,15 +185,17 @@
 
       except UnicodeDecodeError:
         buffered_tokens += tokstr_b
 
       self._logits = self._eval(tokid)
 
     if buffered_tokens:
-      generated += buffered_tokens.decode("utf-8", errors="ignore")
+      tokstr = buffered_tokens.decode("utf-8", errors="ignore")
+      generated += tokstr
+      yield RespInfer(tokid=tokid, tokstr=tokstr, running_infer=generated)
     yield RespInfer(tokid=-1, tokstr="", running_infer=generated)
 
 
 class LlamaCppModel(LLM[LlamaCppSession]):
   """
   llama.cpp model.
   """
```

### Comparing `langdash-1.0.1a1/langdash/models/mock.py` & `langdash-1.1.0a1/langdash/models/mock.py`

 * *Files identical despite different names*

### Comparing `langdash-1.0.1a1/langdash/models/rwkv_cpp.py` & `langdash-1.1.0a1/langdash/models/rwkv_cpp.py`

 * *Files identical despite different names*

### Comparing `langdash-1.0.1a1/langdash/models/sentence_transformers.py` & `langdash-1.1.0a1/langdash/models/sentence_transformers.py`

 * *Files identical despite different names*

### Comparing `langdash-1.0.1a1/langdash/models/transformers.py` & `langdash-1.1.0a1/langdash/models/transformers.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,18 +48,25 @@
 
   _next_token: Optional[Tuple[int, str]]
 
   def __init__(self, *args, **kwargs):
     super().__init__(*args, **kwargs)
 
     def load_model(llm: TransformersModel):
-      model = transformers.AutoModelForCausalLM.from_pretrained(llm._model_name)
-      tokenizer = transformers.AutoTokenizer.from_pretrained(
-        llm._tokenizer_name
-      )
+      if isinstance(llm._model, str):
+        model = transformers.AutoModelForCausalLM.from_pretrained(
+          llm._model, **llm._model_kwargs
+        )
+      else:
+        model = llm._model
+
+      if isinstance(llm._tokenizer, str):
+        tokenizer = transformers.AutoTokenizer.from_pretrained(llm._tokenizer)
+      else:
+        tokenizer = llm._tokenizer
 
       if isinstance(
         tokenizer, (transformers.GPT2Tokenizer, transformers.GPT2TokenizerFast)
       ):
         buffered_token_head = set(
           v for k, v in tokenizer.get_vocab().items() if "\u0122" in k
         )
@@ -212,22 +219,29 @@
 
 class TransformersModel(LLM[TransformersSession]):
   """
   transformers model.
   """
   Session = TransformersSession
 
-  def __init__(self, model_name: str, tokenizer_name: Optional[str] = None):
+  def __init__(
+    self,
+    model: Union[str, transformers.PreTrainedModel],
+    tokenizer: Optional[Union[str, transformers.PreTrainedTokenizer]] = None,
+    **model_kwargs
+  ):
     """
     Creates a template for a language model powered by the transformers library.
     
     Args:
-      model_name (str):
-        The name of the model.
-      tokenizer_name (str):
-        The name of the tokenizer.
-        If None, the model_name will be used to detect the tokenizer.
+      model (Union[str, transformers.PreTrainedModel]):
+        The name of the model, or the model class itself.
+      tokenizer (Optional[Union[str, transformers.PreTrainedTokenizer]]):
+        The name of the tokenizer, or the tokenizer class itself.
+        Defaults to `None`. If not set, the name of the model will be used to detect the tokenizer.
     """
-    if tokenizer_name is None:
-      tokenizer_name = model_name
-    self._model_name = model_name
-    self._tokenizer_name = tokenizer_name
+    if tokenizer is None:
+      assert isinstance(model, str), "model must be string if tokenizer is None"
+      tokenizer = model
+    self._model = model
+    self._tokenizer = tokenizer
+    self._model_kwargs = model_kwargs
```

### Comparing `langdash-1.0.1a1/langdash/response.py` & `langdash-1.1.0a1/langdash/response.py`

 * *Files identical despite different names*

### Comparing `langdash-1.0.1a1/langdash/sampling.py` & `langdash-1.1.0a1/langdash/sampling.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,80 +1,86 @@
-from typing import List
+from typing import Sequence
 from langdash.infer import InferArgs
 
 import torch
 from torch.nn import functional as F
 
 
+def _sample_greedy(probs: torch.Tensor) -> torch.Tensor:
+  argmax = torch.argmax(probs)
+  probs[:] = 0.
+  probs[argmax] = 1.
+  return probs
+
+
 @torch.jit.script
-def _sample_top_p(logits: torch.Tensor, top_p: float) -> torch.Tensor:
+def _sample_top_p(probs: torch.Tensor, top_p: float) -> torch.Tensor:
   assert 0.0 <= top_p <= 1.0, "top_p must be in [0.0, 1.0]"
-  probs = F.softmax(logits, dim=-1)
   sorted_probs = torch.sort(probs, descending=True)[0]
   cumulative_probs = torch.cumsum(sorted_probs, dim=-1)
   cutoff = float(sorted_probs[torch.argmax((cumulative_probs > top_p).long())])
   probs[probs < cutoff] = 0
   return probs
 
 
 @torch.jit.script
-def _sample_typical(logits: torch.Tensor, mass: float) -> torch.Tensor:
+def _sample_typical(
+  probs: torch.Tensor, logits: torch.Tensor, mass: float
+) -> torch.Tensor:
   # https://github.com/huggingface/transformers/compare/main...cimeister:typicalsampling:typical-pr
   assert 0.0 <= mass <= 1.0, "typical mass must be in [0.0, 1.0]"
-
-  probs = F.softmax(logits, dim=-1)
   normalized = -torch.log(probs)
   ent = torch.nansum(normalized * probs, dim=-1, keepdim=True)
 
   shifted_scores = torch.abs(logits - ent)
   sorted_scores, sorted_indices = torch.sort(shifted_scores, descending=False)
   sorted_logits = logits.gather(-1, sorted_indices)
   cumulative_probs = sorted_logits.softmax(dim=-1).cumsum(dim=-1)
 
   I = (cumulative_probs < mass).sum()
   probs[shifted_scores > sorted_scores[I]] = 0.
   return probs
 
 
 def _output_probs(
-  logits: torch.FloatTensor, args: InferArgs, ctx: List[int]
+  logits: torch.FloatTensor, args: InferArgs, ctx: Sequence[int]
 ) -> torch.Tensor:
   # apply repetition penalty
   if args.rep_penalty != 1.0:
     rep_penalty = args.rep_penalty
     assert 0.0 <= rep_penalty, "rep_penalty must be in [0.0, inf]"
     for _, tok in zip(range(args.max_rep_ctx), reversed(ctx)):
       if logits[tok] < 0.0:
         logits[tok] *= rep_penalty
       else:
         logits[tok] /= rep_penalty
 
-  # probabilities
-  if args.typical_mass > 0.0:
-    # typical
-    probs = _sample_typical(logits, args.typical_mass)
-  else:
-    # top-p
-    probs = _sample_top_p(logits, args.top_p)
+  probs = logits_to_probs(logits)
 
-  # apply temperature
-  if args.temperature != 1.0:
-    probs = probs.pow(1.0 / args.temperature)
+  if args.temperature == 0.0:
+    probs = _sample_greedy(probs)
+  else:
+    if args.typical_mass > 0.0:
+      probs = _sample_typical(probs, logits, args.typical_mass)
+    if args.top_p > 0.0:
+      probs = _sample_top_p(probs, args.top_p)
+    if args.temperature != 1.0:
+      probs = probs.pow(1.0 / args.temperature)
 
   return probs
 
 
 def sample(*args, **kwargs) -> int:
   """
   Sample from a distribution of tokens specified by *logits*.
   
   Args:
     logits (torch.FloatTensor): Logits to sample from.
     args (InferArgs): Sampling arguments.
-    ctx (List[int]): List of tokens generated so far.
+    ctx (Sequence[int]): Sequence of tokens generated so far.
   
   Returns:
     The token sampled.
   """
   probs = _output_probs(*args, **kwargs)
   return int(torch.multinomial(probs, num_samples=1)[0])
```

### Comparing `langdash-1.0.1a1/langdash/search/embedding_search.py` & `langdash-1.1.0a1/langdash/search/embedding_search.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,8 +32,8 @@
     max_documents: int = 1
   ) -> Generator[Tuple[str, float], None, None]:
     embd = self._embd_session.embed([text])
     if max_documents == -1:
       max_documents = len(self._documents)
     D, I = self._embds.search(embd, max_documents)
     for d, i in zip(D[0], I[0]):
-      yield self._documents[i], d
+      yield i, self._documents[i], d
```

### Comparing `langdash-1.0.1a1/langdash/search/engine.py` & `langdash-1.1.0a1/langdash/search/engine.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,19 +16,20 @@
     """
     raise NotImplementedError("add")
 
   def search(
     self,
     text: str,
     max_documents: int = 1
-  ) -> Generator[Tuple[str, float], None, None]:
+  ) -> Generator[Tuple[int, str, float], None, None]:
     """
     Search for documents relating to text in the engine.
 
     Args:
       text (str): The text to search for in the documents.
       max_documents (int): The maximum number of documents to search through. Default is 1.
 
     Returns:
-      A generator of tuples containing the document and its relevance score to the search text.
+      A generator of tuples containing the index of the document, its content
+      and its relevance score to the search text.
     """
     raise NotImplementedError("search")
```

### Comparing `langdash-1.0.1a1/langdash/search/multichoice_search.py` & `langdash-1.1.0a1/langdash/search/multichoice_search.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,15 +54,15 @@
       self._prompts += prompt
       self._keys.append(key)
 
   def search(
     self,
     text: str,
     max_documents: int = 1
-  ) -> Generator[Tuple[str, float], None, None]:
+  ) -> Generator[Tuple[int, str, float], None, None]:
     if not self._documents:
       return
 
     if self._needs_update:
       self._update_session()
       self._needs_update = False
 
@@ -85,13 +85,13 @@
     for idx, token in enumerate(self._key_tokens):  # type: ignore
       doc_probs[idx] = tok_probs[token]
 
     doc_probs_sum = sum(doc_probs)
     for idx in range(len(doc_probs)):
       doc_probs[idx] /= doc_probs_sum
 
-    doc_probs_with_text = list(zip(self._documents, doc_probs))
-    doc_probs_with_text.sort(key=lambda x: x[1], reverse=True)
+    doc_probs_with_text = list(zip(range(len(self._documents)), self._documents, doc_probs))
+    doc_probs_with_text.sort(key=lambda x: x[2], reverse=True)
     if max_documents == -1:
       yield from iter(doc_probs_with_text)
     else:
       yield from iter(doc_probs_with_text[0:max_documents])
```

### Comparing `langdash-1.0.1a1/langdash.egg-info/PKG-INFO` & `langdash-1.1.0a1/langdash.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langdash
-Version: 1.0.1a1
+Version: 1.1.0a1
 Summary: A simple library for interfacing with language models.
 Home-page: https://git.mysymphony.jp.net/nana/langdash
 Author: Nana Mochizuki
 Author-email: nana@mysymphony.jp.net
 Project-URL: Source, https://git.mysymphony.jp.net/nana/langdash
 Project-URL: Documentation, https://langdash.readthedocs.io/en/latest/
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `langdash-1.0.1a1/langdash.egg-info/SOURCES.txt` & `langdash-1.1.0a1/langdash.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `langdash-1.0.1a1/setup.py` & `langdash-1.1.0a1/setup.py`

 * *Files identical despite different names*

