# Comparing `tmp/zeno_build-0.0.1.tar.gz` & `tmp/zeno_build-0.0.2.tar.gz`

## Comparing `zeno_build-0.0.1.tar` & `zeno_build-0.0.2.tar`

### file list

```diff
@@ -1,39 +1,42 @@
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 zeno_build-0.0.1/zeno_build/__init__.py
--rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 zeno_build-0.0.1/zeno_build/cache_utils.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 zeno_build-0.0.1/zeno_build/version.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 zeno_build-0.0.1/zeno_build/evaluation/__init__.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 zeno_build-0.0.1/zeno_build/evaluation/text_features/__init__.py
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 zeno_build-0.0.1/zeno_build/evaluation/text_features/exact_match.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 zeno_build-0.0.1/zeno_build/evaluation/text_features/length.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 zeno_build-0.0.1/zeno_build/evaluation/text_metrics/__init__.py
--rw-r--r--   0        0        0    15356 2020-02-02 00:00:00.000000 zeno_build-0.0.1/zeno_build/evaluation/text_metrics/critique.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 zeno_build-0.0.1/zeno_build/experiments/__init__.py
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 zeno_build-0.0.1/zeno_build/experiments/experiment_run.py
--rw-r--r--   0        0        0     4001 2020-02-02 00:00:00.000000 zeno_build-0.0.1/zeno_build/experiments/search_space.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 zeno_build-0.0.1/zeno_build/models/__init__.py
--rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 zeno_build-0.0.1/zeno_build/models/chat_generate.py
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 zeno_build-0.0.1/zeno_build/models/dataset_config.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 zeno_build-0.0.1/zeno_build/models/global_models.py
--rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 zeno_build-0.0.1/zeno_build/models/lm_config.py
--rw-r--r--   0        0        0     3170 2020-02-02 00:00:00.000000 zeno_build-0.0.1/zeno_build/models/text_generate.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 zeno_build-0.0.1/zeno_build/models/providers/__init__.py
--rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 zeno_build-0.0.1/zeno_build/models/providers/cohere_utils.py
--rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 zeno_build-0.0.1/zeno_build/models/providers/huggingface_utils.py
--rw-r--r--   0        0        0     5801 2020-02-02 00:00:00.000000 zeno_build-0.0.1/zeno_build/models/providers/openai_utils.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 zeno_build-0.0.1/zeno_build/optimizers/__init__.py
--rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 zeno_build-0.0.1/zeno_build/optimizers/base.py
--rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 zeno_build-0.0.1/zeno_build/optimizers/random.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 zeno_build-0.0.1/zeno_build/optimizers/standard.py
--rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 zeno_build-0.0.1/zeno_build/optimizers/vizier.py
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 zeno_build-0.0.1/zeno_build/prompts/__init__.py
--rw-r--r--   0        0        0     3033 2020-02-02 00:00:00.000000 zeno_build-0.0.1/zeno_build/prompts/chat_prompt.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 zeno_build-0.0.1/zeno_build/prompts/prompt_utils.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 zeno_build-0.0.1/zeno_build/reporting/__init__.py
--rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 zeno_build-0.0.1/zeno_build/reporting/aggregate_results.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 zeno_build-0.0.1/zeno_build/reporting/reporting_utils.py
--rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 zeno_build-0.0.1/zeno_build/reporting/visualize.py
--rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 zeno_build-0.0.1/.gitignore
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 zeno_build-0.0.1/LICENSE
--rw-r--r--   0        0        0     3413 2020-02-02 00:00:00.000000 zeno_build-0.0.1/README.md
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 zeno_build-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     5396 2020-02-02 00:00:00.000000 zeno_build-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 zeno_build-0.0.2/zeno_build/__init__.py
+-rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 zeno_build-0.0.2/zeno_build/cache_utils.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 zeno_build-0.0.2/zeno_build/version.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 zeno_build-0.0.2/zeno_build/evaluation/__init__.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 zeno_build-0.0.2/zeno_build/evaluation/text_features/__init__.py
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 zeno_build-0.0.2/zeno_build/evaluation/text_features/capitalization.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 zeno_build-0.0.2/zeno_build/evaluation/text_features/exact_match.py
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 zeno_build-0.0.2/zeno_build/evaluation/text_features/frequency.py
+-rw-r--r--   0        0        0     2470 2020-02-02 00:00:00.000000 zeno_build-0.0.2/zeno_build/evaluation/text_features/length.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 zeno_build-0.0.2/zeno_build/evaluation/text_metrics/__init__.py
+-rw-r--r--   0        0        0    16370 2020-02-02 00:00:00.000000 zeno_build-0.0.2/zeno_build/evaluation/text_metrics/critique.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 zeno_build-0.0.2/zeno_build/experiments/__init__.py
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 zeno_build-0.0.2/zeno_build/experiments/experiment_run.py
+-rw-r--r--   0        0        0     4904 2020-02-02 00:00:00.000000 zeno_build-0.0.2/zeno_build/experiments/search_space.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 zeno_build-0.0.2/zeno_build/models/__init__.py
+-rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 zeno_build-0.0.2/zeno_build/models/chat_generate.py
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 zeno_build-0.0.2/zeno_build/models/dataset_config.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 zeno_build-0.0.2/zeno_build/models/global_models.py
+-rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 zeno_build-0.0.2/zeno_build/models/lm_config.py
+-rw-r--r--   0        0        0     3170 2020-02-02 00:00:00.000000 zeno_build-0.0.2/zeno_build/models/text_generate.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 zeno_build-0.0.2/zeno_build/models/providers/__init__.py
+-rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 zeno_build-0.0.2/zeno_build/models/providers/cohere_utils.py
+-rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 zeno_build-0.0.2/zeno_build/models/providers/huggingface_utils.py
+-rw-r--r--   0        0        0     6896 2020-02-02 00:00:00.000000 zeno_build-0.0.2/zeno_build/models/providers/openai_utils.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 zeno_build-0.0.2/zeno_build/optimizers/__init__.py
+-rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 zeno_build-0.0.2/zeno_build/optimizers/base.py
+-rw-r--r--   0        0        0     4080 2020-02-02 00:00:00.000000 zeno_build-0.0.2/zeno_build/optimizers/exhaustive.py
+-rw-r--r--   0        0        0     3294 2020-02-02 00:00:00.000000 zeno_build-0.0.2/zeno_build/optimizers/random.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 zeno_build-0.0.2/zeno_build/optimizers/standard.py
+-rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 zeno_build-0.0.2/zeno_build/optimizers/vizier.py
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 zeno_build-0.0.2/zeno_build/prompts/__init__.py
+-rw-r--r--   0        0        0     3033 2020-02-02 00:00:00.000000 zeno_build-0.0.2/zeno_build/prompts/chat_prompt.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 zeno_build-0.0.2/zeno_build/prompts/prompt_utils.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 zeno_build-0.0.2/zeno_build/reporting/__init__.py
+-rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 zeno_build-0.0.2/zeno_build/reporting/aggregate_results.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 zeno_build-0.0.2/zeno_build/reporting/reporting_utils.py
+-rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 zeno_build-0.0.2/zeno_build/reporting/visualize.py
+-rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 zeno_build-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 zeno_build-0.0.2/LICENSE
+-rw-r--r--   0        0        0     3413 2020-02-02 00:00:00.000000 zeno_build-0.0.2/README.md
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 zeno_build-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5396 2020-02-02 00:00:00.000000 zeno_build-0.0.2/PKG-INFO
```

### Comparing `zeno_build-0.0.1/zeno_build/cache_utils.py` & `zeno_build-0.0.2/zeno_build/cache_utils.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.1/zeno_build/evaluation/text_features/exact_match.py` & `zeno_build-0.0.2/zeno_build/evaluation/text_features/exact_match.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.1/zeno_build/evaluation/text_features/length.py` & `zeno_build-0.0.2/zeno_build/evaluation/text_features/length.py`

 * *Files 17% similar despite different names*

```diff
@@ -56,14 +56,37 @@
         ops: Zeno options
 
     Returns:
         DistillReturn:
     """
     chat_context_lengths = []
     for data in df[ops.data_column]:
-        if not isinstance(data, ChatMessages):
+        if isinstance(data, ChatMessages):
+            chat_context_lengths.append(len(data.messages))
+        elif isinstance(data, list):
+            chat_context_lengths.append(len(data))
+        else:
             raise ValueError(
-                f"Expected {ops.data_column} column to be ChatMessages, but got "
-                f"{type(data)} instead."
+                f"Expected {ops.data_column} column to be ChatMessages, or list "
+                f"but got {type(data)} instead."
             )
-        chat_context_lengths.append(len(data.messages))
     return DistillReturn(distill_output=chat_context_lengths)
+
+
+@distill
+def doc_context_length(df: DataFrame, ops: ZenoOptions) -> DistillReturn:
+    """Length of the previous document context, e.g. for document-level translation.
+
+    Args:
+        df: Zeno DataFrame
+        ops: Zeno options
+
+    Returns:
+        DistillReturn: The document context
+    """
+    doc_context_lengths = []
+    # Count the number of times `doc_id` has appeared so far
+    doc_ids: dict[str, int] = {}
+    for x in df["doc_id"]:
+        doc_ids[x] = doc_ids.get(x, 0) + 1
+        doc_context_lengths.append(doc_ids[x])
+    return DistillReturn(distill_output=doc_context_lengths)
```

### Comparing `zeno_build-0.0.1/zeno_build/evaluation/text_metrics/critique.py` & `zeno_build-0.0.2/zeno_build/evaluation/text_metrics/critique.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,28 +128,49 @@
     # NOTE: It is necessary to mention "ops.output_column" in this function
     # to work-around a hack in Zeno (as of v0.4.11):
     # https://github.com/zeno-ml/zeno/blob/5c064e74b5276173fa354c4a546ce0d762d8f4d7/zeno/backend.py#L187  # noqa: E501
     return call_critique(df, ops, "chrf", {})
 
 
 @distill
+def comet(df: DataFrame, ops: ZenoOptions) -> DistillReturn:
+    """COMET score.
+
+    Args:
+        df: Zeno DataFrame
+        ops: Zeno options
+
+    Returns:
+        DistillReturn: COMET scores
+    """
+    # NOTE: It is necessary to mention "ops.output_column" in this function
+    # to work-around a hack in Zeno (as of v0.4.11):
+    # https://github.com/zeno-ml/zeno/blob/5c064e74b5276173fa354c4a546ce0d762d8f4d7/zeno/backend.py#L187  # noqa: E501
+    return call_critique(
+        df, ops, "comet", {"model": "unbabel_comet/wmt21-comet-qe-da"}, batch_size=150
+    )
+
+
+@distill
 def length_ratio(df: DataFrame, ops: ZenoOptions) -> DistillReturn:
     """Length ratio.
 
     Args:
         df: Zeno DataFrame
         ops: Zeno options
 
     Returns:
         DistillReturn: Length ratios
     """
     # NOTE: It is necessary to mention "ops.output_column" in this function
     # to work-around a hack in Zeno (as of v0.4.11):
     # https://github.com/zeno-ml/zeno/blob/5c064e74b5276173fa354c4a546ce0d762d8f4d7/zeno/backend.py#L187  # noqa: E501
-    return call_critique(df, ops, "length_ratio", {})
+    return call_critique(
+        df, ops, "length_ratio", {"tokenizer": {"name": "character", "config": {}}}
+    )
 
 
 @distill
 def rouge_1(df: DataFrame, ops: ZenoOptions) -> DistillReturn:
     """ROUGE-1 score.
 
     Args:
@@ -380,14 +401,30 @@
     """
     if len(df) == 0:
         return MetricReturn(metric=0)
     return MetricReturn(metric=df[ops.distill_columns["chrf"]].fillna(0).mean())
 
 
 @metric
+def avg_comet(df: DataFrame, ops: ZenoOptions) -> MetricReturn:
+    """Average comet score.
+
+    Args:
+        df: Zeno DataFrame
+        ops: Zeno options
+
+    Returns:
+        MetricReturn: Average comet score
+    """
+    if len(df) == 0:
+        return MetricReturn(metric=0)
+    return MetricReturn(metric=df[ops.distill_columns["comet"]].fillna(0).mean())
+
+
+@metric
 def avg_length_ratio(df: DataFrame, ops: ZenoOptions) -> MetricReturn:
     """Average length ratio.
 
     Args:
         df: Zeno DataFrame
         ops: Zeno options
```

### Comparing `zeno_build-0.0.1/zeno_build/experiments/search_space.py` & `zeno_build-0.0.2/zeno_build/experiments/search_space.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """Search space for hyperparameter optimization."""
 
+from __future__ import annotations
+
 import json
 import os
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from typing import Any, Generic, TypeVar
 
 T = TypeVar("T")
@@ -66,15 +68,20 @@
     def value_in_scope(self, value: Any) -> bool:
         """See base class."""
         return self.lower <= value <= self.upper
 
 
 @dataclass(frozen=True)
 class Int(SearchDimension):
-    """An integer hyperparameter range."""
+    """An integer hyperparameter range.
+
+    Attributes:
+        lower: The lower bound of the range (inclusive).
+        upper: The upper bound of the range (inclusive).
+    """
 
     lower: int
     upper: int
 
     def value_in_scope(self, value: Any) -> bool:
         """See base class."""
         return self.lower <= value <= self.upper
@@ -136,7 +143,26 @@
         """See base class."""
         for k, v in params.items():
             if k not in self.dimensions:
                 return False
             if not self.dimensions[k].value_in_scope(v):
                 return False
         return True
+
+
+class CompositeSearchSpace(SearchSpace):
+    """A search space consisting of multiple search spaces."""
+
+    def __init__(self, spaces: list[SearchSpace], weights: list[float] | None = None):
+        """Initialize the search space.
+
+        Args:
+            spaces: The search spaces to combine.
+            weights: The weights of the search spaces. If None, all search spaces
+                have equal weight.
+        """
+        self.spaces = spaces
+        self.weights = weights or [1.0 / len(spaces)] * len(spaces)
+
+    def contains_params(self, params: dict[str, Any]) -> bool:
+        """Check if the parameters are contained in the search space."""
+        return any([s.contains_params(params) for s in self.spaces])
```

### Comparing `zeno_build-0.0.1/zeno_build/models/chat_generate.py` & `zeno_build-0.0.2/zeno_build/models/chat_generate.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     full_contexts: list[chat_prompt.ChatMessages],
     prompt_template: chat_prompt.ChatMessages,
     model_config: lm_config.LMConfig,
     temperature: float,
     max_tokens: int,
     top_p: float,
     context_length: int,
-    requests_per_minute: int = 50,
+    requests_per_minute: int = 300,
 ) -> list[str]:
     """Generate from a list of chat-style prompts.
 
     Args:
         variables: The variables to be replaced in the prompt template.
         prompt_template: The template for the prompt.
         api_based_model_config: The API-based model configuration.
```

### Comparing `zeno_build-0.0.1/zeno_build/models/dataset_config.py` & `zeno_build-0.0.2/zeno_build/models/dataset_config.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.1/zeno_build/models/lm_config.py` & `zeno_build-0.0.2/zeno_build/models/lm_config.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.1/zeno_build/models/text_generate.py` & `zeno_build-0.0.2/zeno_build/models/text_generate.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.1/zeno_build/models/providers/cohere_utils.py` & `zeno_build-0.0.2/zeno_build/models/providers/cohere_utils.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.1/zeno_build/models/providers/huggingface_utils.py` & `zeno_build-0.0.2/zeno_build/models/providers/huggingface_utils.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.1/zeno_build/models/providers/openai_utils.py` & `zeno_build-0.0.2/zeno_build/models/providers/openai_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import logging
 import os
 from typing import Any
 
 import aiolimiter
 import openai
 import openai.error
+from aiohttp import ClientSession
 from tqdm.asyncio import tqdm_asyncio
 
 from zeno_build.models import lm_config
 from zeno_build.prompts import chat_prompt
 
 
 async def _throttled_openai_completion_acreate(
@@ -69,14 +70,15 @@
         List of generated responses.
     """
     if "OPENAI_API_KEY" not in os.environ:
         raise ValueError(
             "OPENAI_API_KEY environment variable must be set when using OpenAI API."
         )
     openai.api_key = os.environ["OPENAI_API_KEY"]
+    openai.aiosession.set(ClientSession())
     limiter = aiolimiter.AsyncLimiter(requests_per_minute)
     async_responses = [
         _throttled_openai_completion_acreate(
             engine=model_config.model,
             prompt=prompt_template.to_text_prompt(
                 full_context=full_context.limit_length(context_length),
                 name_replacements=model_config.name_replacements,
@@ -85,14 +87,16 @@
             max_tokens=max_tokens,
             top_p=top_p,
             limiter=limiter,
         )
         for full_context in full_contexts
     ]
     responses = await tqdm_asyncio.gather(*async_responses)
+    # Note: will never be none because it's set, but mypy doesn't know that.
+    await openai.aiosession.get().close()  # type: ignore
     return [x["choices"][0]["text"] for x in responses]
 
 
 async def _throttled_openai_chat_completion_acreate(
     model: str,
     messages: list[dict[str, str]],
     temperature: float,
@@ -114,14 +118,29 @@
                 logging.warning(
                     "OpenAI API rate limit exceeded. Sleeping for 10 seconds."
                 )
                 await asyncio.sleep(10)
             except asyncio.exceptions.TimeoutError:
                 logging.warning("OpenAI API timeout. Sleeping for 10 seconds.")
                 await asyncio.sleep(10)
+            except openai.error.InvalidRequestError:
+                logging.warning("OpenAI API Invalid Request: Prompt was filtered")
+                return {
+                    "choices": [
+                        {"message": {"content": "Invalid Request: Prompt was filtered"}}
+                    ]
+                }
+            except openai.error.APIConnectionError:
+                logging.warning(
+                    "OpenAI API Connection Error: Error Communicating with OpenAI"
+                )
+                await asyncio.sleep(10)
+            except openai.error.Timeout:
+                logging.warning("OpenAI APITimeout Error: OpenAI Timeout")
+                await asyncio.sleep(10)
             except openai.error.APIError as e:
                 logging.warning(f"OpenAI API error: {e}")
                 break
         return {"choices": [{"message": {"content": ""}}]}
 
 
 async def generate_from_openai_chat_completion(
@@ -150,14 +169,15 @@
         List of generated responses.
     """
     if "OPENAI_API_KEY" not in os.environ:
         raise ValueError(
             "OPENAI_API_KEY environment variable must be set when using OpenAI API."
         )
     openai.api_key = os.environ["OPENAI_API_KEY"]
+    openai.aiosession.set(ClientSession())
     limiter = aiolimiter.AsyncLimiter(requests_per_minute)
     async_responses = [
         _throttled_openai_chat_completion_acreate(
             model=model_config.model,
             messages=prompt_template.to_openai_chat_completion_messages(
                 full_context=full_context.limit_length(context_length),
             ),
@@ -165,8 +185,10 @@
             max_tokens=max_tokens,
             top_p=top_p,
             limiter=limiter,
         )
         for full_context in full_contexts
     ]
     responses = await tqdm_asyncio.gather(*async_responses)
+    # Note: will never be none because it's set, but mypy doesn't know that.
+    await openai.aiosession.get().close()  # type: ignore
     return [x["choices"][0]["message"]["content"] for x in responses]
```

### Comparing `zeno_build-0.0.1/zeno_build/optimizers/base.py` & `zeno_build-0.0.2/zeno_build/optimizers/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """Base class for optimizers that run hyperparameter sweeps."""
 
 from __future__ import annotations
 
+import abc
 from collections.abc import Callable
 from typing import Any, TypeVar
 
 from pandas import DataFrame
 from zeno import DistillReturn, MetricReturn, ZenoOptions
 
 from zeno_build.experiments import search_space
 
 T = TypeVar("T")
 
 
-class Optimizer:
+class Optimizer(abc.ABC):
     """An optimizer for hyperparameter search."""
 
     def __init__(
         self,
         space: search_space.SearchSpace,
         distill_functions: list[Callable[[DataFrame, ZenoOptions], DistillReturn]],
         metric: Callable[[DataFrame, ZenoOptions], MetricReturn],
@@ -75,7 +76,17 @@
         """
         if self.num_trials is None:
             return False
         valid_param_files = self.space.get_valid_param_files(
             output_dir=output_dir, include_in_progress=include_in_progress
         )
         return len(valid_param_files) >= self.num_trials
+
+    @abc.abstractmethod
+    def get_parameters(self) -> dict[str, Any] | None:
+        """Get the next parameters to optimize.
+
+        Returns:
+            A dictionary of instantiated parameters, or None
+            if there are no more parameters to return.
+        """
+        ...
```

### Comparing `zeno_build-0.0.1/zeno_build/optimizers/random.py` & `zeno_build-0.0.2/zeno_build/optimizers/random.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from __future__ import annotations
 
 import random
 from collections.abc import Callable
 from typing import Any, TypeVar
 
+import numpy as np
 from pandas import DataFrame
 from zeno import DistillReturn, MetricReturn, ZenoOptions
 
 from zeno_build.experiments import search_space
 from zeno_build.optimizers.base import Optimizer
 
 T = TypeVar("T")
@@ -39,38 +40,50 @@
         super().__init__(space, distill_functions, metric, num_trials)
         # Set state without side-effects (for single thread)
         saved_state = random.getstate()
         random.seed(seed)
         self._state = random.getstate()
         random.setstate(saved_state)
 
-    def get_parameters(self) -> dict[str, Any]:
-        """Randomize the parameters in a space.
-
-        Args:
-            space: The space to randomize.
-
-        Returns:
-            A dictionary of randomized parameters.
-        """
-        if isinstance(self.space, search_space.CombinatorialSearchSpace):
-            saved_state = random.getstate()
-            random.setstate(self._state)
+    @staticmethod
+    def _get_parameters_from_space(
+        space: search_space.SearchSpace,
+    ) -> dict[str, Any] | None:
+        if isinstance(space, search_space.CombinatorialSearchSpace):
             params = {}
-            for name, dimension in self.space.dimensions.items():
+            for name, dimension in space.dimensions.items():
                 if isinstance(dimension, search_space.Categorical) or isinstance(
                     dimension, search_space.Discrete
                 ):
                     params[name] = random.choice(dimension.choices)
                 elif isinstance(dimension, search_space.Float):
                     params[name] = random.uniform(dimension.lower, dimension.upper)
                 elif isinstance(dimension, search_space.Int):
                     params[name] = random.randint(dimension.lower, dimension.upper)
                 elif isinstance(dimension, search_space.Constant):
                     params[name] = dimension.value
                 else:
                     raise ValueError(f"Unknown search dimension: {dimension}")
-            self._state = random.getstate()
-            random.setstate(saved_state)
+            return params
+        elif isinstance(space, search_space.CompositeSearchSpace):
+            sub_space = space.spaces[
+                np.random.choice(len(space.spaces), p=space.weights)
+            ]
+            return RandomOptimizer._get_parameters_from_space(sub_space)
         else:
-            raise NotImplementedError(f"Unsupported search space {type(self.space)}.")
+            raise NotImplementedError(f"Unsupported search space {type(space)}.")
+
+    def get_parameters(self) -> dict[str, Any] | None:
+        """Randomize the parameters in a space.
+
+        Args:
+            space: The space to randomize.
+
+        Returns:
+            A dictionary of randomized parameters.
+        """
+        saved_state = random.getstate()
+        random.setstate(self._state)
+        params = RandomOptimizer._get_parameters_from_space(self.space)
+        self._state = random.getstate()
+        random.setstate(saved_state)
         return params
```

### Comparing `zeno_build-0.0.1/zeno_build/optimizers/vizier.py` & `zeno_build-0.0.2/zeno_build/optimizers/vizier.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.1/zeno_build/prompts/chat_prompt.py` & `zeno_build-0.0.2/zeno_build/prompts/chat_prompt.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.1/zeno_build/reporting/aggregate_results.py` & `zeno_build-0.0.2/zeno_build/reporting/aggregate_results.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.1/zeno_build/reporting/reporting_utils.py` & `zeno_build-0.0.2/zeno_build/reporting/reporting_utils.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.1/zeno_build/reporting/visualize.py` & `zeno_build-0.0.2/zeno_build/reporting/visualize.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.1/.gitignore` & `zeno_build-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.1/LICENSE` & `zeno_build-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.1/README.md` & `zeno_build-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.1/pyproject.toml` & `zeno_build-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.1/PKG-INFO` & `zeno_build-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zeno_build
-Version: 0.0.1
+Version: 0.0.2
 Summary: A library for comparing multiple llm-based systems.
 Author-email: Ángel Alexander Cabrera <alex.cabrera@gmail.com>, Graham Neubig <neubig@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Zeno
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

