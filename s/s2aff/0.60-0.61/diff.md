# Comparing `tmp/s2aff-0.60.tar.gz` & `tmp/s2aff-0.61.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s2aff-0.60.tar", last modified: Mon Jun  5 17:04:35 2023, max compression
+gzip compressed data, was "s2aff-0.61.tar", last modified: Thu Jun  8 22:04:18 2023, max compression
```

## Comparing `s2aff-0.60.tar` & `s2aff-0.61.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-06-05 17:04:35.343626 s2aff-0.60/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    11357 2023-05-08 19:46:34.000000 s2aff-0.60/LICENSE
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      204 2023-06-05 17:04:35.343340 s2aff-0.60/PKG-INFO
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     7169 2023-05-08 19:46:34.000000 s2aff-0.60/README.md
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-06-05 17:04:35.331721 s2aff-0.60/data/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:05:25.000000 s2aff-0.60/data/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4126 2022-06-27 22:34:39.000000 s2aff-0.60/data/combine_gold.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1431 2023-05-08 19:46:34.000000 s2aff-0.60/data/download_latest_ror.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-06-05 17:04:35.332407 s2aff-0.60/data/ner_model/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:07:05.000000 s2aff-0.60/data/ner_model/__init__.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-06-05 17:04:35.336709 s2aff-0.60/s2aff/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    12306 2023-06-05 17:03:17.000000 s2aff-0.60/s2aff/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     2022 2023-05-25 22:59:38.000000 s2aff-0.60/s2aff/consts.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      812 2023-05-08 19:46:34.000000 s2aff-0.60/s2aff/data.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    10789 2023-05-08 19:46:34.000000 s2aff-0.60/s2aff/features.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4829 2023-05-08 19:46:34.000000 s2aff-0.60/s2aff/file_cache.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    10466 2023-05-15 17:55:03.000000 s2aff-0.60/s2aff/lightgbm_helpers.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    13725 2023-05-22 17:08:00.000000 s2aff-0.60/s2aff/model.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    36032 2023-06-01 18:34:10.000000 s2aff-0.60/s2aff/ror.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     2182 2023-05-08 19:46:34.000000 s2aff-0.60/s2aff/text.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-06-05 17:04:35.338834 s2aff-0.60/s2aff/timo/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 19:46:34.000000 s2aff-0.60/s2aff/timo/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1644 2023-05-08 19:46:34.000000 s2aff-0.60/s2aff/timo/integration_test.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     5308 2023-05-15 17:57:34.000000 s2aff-0.60/s2aff/timo/interface.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-06-05 17:04:35.338102 s2aff-0.60/s2aff.egg-info/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      204 2023-06-05 17:04:35.000000 s2aff-0.60/s2aff.egg-info/PKG-INFO
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      747 2023-06-05 17:04:35.000000 s2aff-0.60/s2aff.egg-info/SOURCES.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        1 2023-06-05 17:04:35.000000 s2aff-0.60/s2aff.egg-info/dependency_links.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      156 2023-06-05 17:04:35.000000 s2aff-0.60/s2aff.egg-info/requires.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)       19 2023-06-05 17:04:35.000000 s2aff-0.60/s2aff.egg-info/top_level.txt
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-06-05 17:04:35.342856 s2aff-0.60/scripts/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:06:14.000000 s2aff-0.60/scripts/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     3044 2023-05-15 17:57:54.000000 s2aff-0.60/scripts/approximate_runtime_and_memory_usage.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4491 2023-05-15 17:57:54.000000 s2aff-0.60/scripts/evaluate_first_stage_ranker.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     6352 2023-05-15 17:57:54.000000 s2aff-0.60/scripts/generate_lightgbm_training_data.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     8836 2023-05-08 19:46:34.000000 s2aff-0.60/scripts/train_lightgbm_reranker.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-08 19:46:34.000000 s2aff-0.60/scripts/train_ner_model.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1318 2023-05-08 19:46:34.000000 s2aff-0.60/scripts/update_openalex_works_counts.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)       38 2023-06-05 17:04:35.343802 s2aff-0.60/setup.cfg
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-06-05 17:03:45.000000 s2aff-0.60/setup.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-06-08 22:04:18.084178 s2aff-0.61/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    11357 2023-05-08 19:46:34.000000 s2aff-0.61/LICENSE
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      204 2023-06-08 22:04:18.083997 s2aff-0.61/PKG-INFO
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     7169 2023-05-08 19:46:34.000000 s2aff-0.61/README.md
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-06-08 22:04:18.075549 s2aff-0.61/data/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:05:25.000000 s2aff-0.61/data/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4126 2022-06-27 22:34:39.000000 s2aff-0.61/data/combine_gold.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1431 2023-05-08 19:46:34.000000 s2aff-0.61/data/download_latest_ror.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-06-08 22:04:18.076131 s2aff-0.61/data/ner_model/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:07:05.000000 s2aff-0.61/data/ner_model/__init__.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-06-08 22:04:18.080333 s2aff-0.61/s2aff/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    12314 2023-06-08 21:55:55.000000 s2aff-0.61/s2aff/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     2022 2023-05-25 22:59:38.000000 s2aff-0.61/s2aff/consts.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      812 2023-05-08 19:46:34.000000 s2aff-0.61/s2aff/data.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    10789 2023-05-08 19:46:34.000000 s2aff-0.61/s2aff/features.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4829 2023-05-08 19:46:34.000000 s2aff-0.61/s2aff/file_cache.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    10466 2023-05-15 17:55:03.000000 s2aff-0.61/s2aff/lightgbm_helpers.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    13725 2023-05-22 17:08:00.000000 s2aff-0.61/s2aff/model.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    36032 2023-06-01 18:34:10.000000 s2aff-0.61/s2aff/ror.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     2182 2023-05-08 19:46:34.000000 s2aff-0.61/s2aff/text.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-06-08 22:04:18.081689 s2aff-0.61/s2aff/timo/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 19:46:34.000000 s2aff-0.61/s2aff/timo/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1644 2023-05-08 19:46:34.000000 s2aff-0.61/s2aff/timo/integration_test.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     5308 2023-05-15 17:57:34.000000 s2aff-0.61/s2aff/timo/interface.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-06-08 22:04:18.081107 s2aff-0.61/s2aff.egg-info/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      204 2023-06-08 22:04:18.000000 s2aff-0.61/s2aff.egg-info/PKG-INFO
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      747 2023-06-08 22:04:18.000000 s2aff-0.61/s2aff.egg-info/SOURCES.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        1 2023-06-08 22:04:18.000000 s2aff-0.61/s2aff.egg-info/dependency_links.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      156 2023-06-08 22:04:18.000000 s2aff-0.61/s2aff.egg-info/requires.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)       19 2023-06-08 22:04:18.000000 s2aff-0.61/s2aff.egg-info/top_level.txt
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-06-08 22:04:18.083690 s2aff-0.61/scripts/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:06:14.000000 s2aff-0.61/scripts/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     3044 2023-05-15 17:57:54.000000 s2aff-0.61/scripts/approximate_runtime_and_memory_usage.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4491 2023-05-15 17:57:54.000000 s2aff-0.61/scripts/evaluate_first_stage_ranker.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     6352 2023-05-15 17:57:54.000000 s2aff-0.61/scripts/generate_lightgbm_training_data.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     8836 2023-05-08 19:46:34.000000 s2aff-0.61/scripts/train_lightgbm_reranker.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-08 19:46:34.000000 s2aff-0.61/scripts/train_ner_model.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1318 2023-05-08 19:46:34.000000 s2aff-0.61/scripts/update_openalex_works_counts.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)       38 2023-06-08 22:04:18.084233 s2aff-0.61/setup.cfg
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-06-08 22:00:05.000000 s2aff-0.61/setup.py
```

### Comparing `s2aff-0.60/LICENSE` & `s2aff-0.61/LICENSE`

 * *Files identical despite different names*

### Comparing `s2aff-0.60/README.md` & `s2aff-0.61/README.md`

 * *Files identical despite different names*

### Comparing `s2aff-0.60/data/combine_gold.py` & `s2aff-0.61/data/combine_gold.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.60/data/download_latest_ror.py` & `s2aff-0.61/data/download_latest_ror.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.60/s2aff/__init__.py` & `s2aff-0.61/s2aff/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 ch.setLevel(logging.INFO)
 logger.addHandler(ch)
 
 
 def process_item(input, ror_index, look_for_grid_and_isni, no_candidates_output_text, pairwise_model, top_k_first_stage, pairwise_model_threshold, no_ror_output_text, pairwise_model_delta_threshold, number_of_top_candidates_to_return):
     counter, raw_affiliation, ner_prediction, len_raw_affiliations, id_ = input
     # Do some work here
-    #print(
-    #    f"\nGetting ROR candidates and reranking for: '{raw_affiliation}' ({counter + 1}/{len_raw_affiliations})\n",
-    #    end="\r",
-    #)
+    print(
+       f"\nGetting ROR candidates and reranking for: '{raw_affiliation}' ({counter + 1}/{len_raw_affiliations})\n",
+       end="\r",
+    )
     main, child, address, early_candidates = parse_ner_prediction(ner_prediction, ror_index)
     # sometimes the affiliation strings just contain GRID or ISNI ids
     # todo: some time in the future the strings may contain ROR ids too
     if look_for_grid_and_isni:
         #print("\nLooking for grid and isni...\n")
         ror_from_grid = ror_index.extract_grid_and_map_to_ror(raw_affiliation)
         #print("\nROR_FROM_GRID\n")
@@ -71,22 +71,22 @@
         display_name = ror_index.ror_dict[output_scores_and_thresh[0][0]]["name"]
     except:
         display_name = ""
 
     # make a dict of outputs
     output = {
         "raw_affiliation": raw_affiliation,
-        "ner_prediction": ner_prediction,
-        "main_from_ner": main,
-        "child_from_ner": child,
-        "address_from_ner": address,
-        "stage1_candidates": list(candidates[: number_of_top_candidates_to_return]),
-        "stage1_scores": list(scores[: number_of_top_candidates_to_return]),
+        # "ner_prediction": ner_prediction,
+        # "main_from_ner": main,
+        # "child_from_ner": child,
+        # "address_from_ner": address,
+        # "stage1_candidates": list(candidates[: number_of_top_candidates_to_return]),
+        # "stage1_scores": list(scores[: number_of_top_candidates_to_return]),
         "stage2_candidates": list(output_scores_and_thresh[0][: number_of_top_candidates_to_return]),
-        "stage2_scores": list(output_scores_and_thresh[1][: number_of_top_candidates_to_return]),
+        # "stage2_scores": list(output_scores_and_thresh[1][: number_of_top_candidates_to_return]),
         "top_candidate_display_name": display_name,
         "id": id_
     }
     #print("\nFINISHED!\n")
     return output
 
 if not multiprocessing.parent_process():
```

### Comparing `s2aff-0.60/s2aff/consts.py` & `s2aff-0.61/s2aff/consts.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.60/s2aff/data.py` & `s2aff-0.61/s2aff/data.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.60/s2aff/features.py` & `s2aff-0.61/s2aff/features.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.60/s2aff/file_cache.py` & `s2aff-0.61/s2aff/file_cache.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.60/s2aff/lightgbm_helpers.py` & `s2aff-0.61/s2aff/lightgbm_helpers.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.60/s2aff/model.py` & `s2aff-0.61/s2aff/model.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.60/s2aff/ror.py` & `s2aff-0.61/s2aff/ror.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.60/s2aff/text.py` & `s2aff-0.61/s2aff/text.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.60/s2aff/timo/integration_test.py` & `s2aff-0.61/s2aff/timo/integration_test.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.60/s2aff/timo/interface.py` & `s2aff-0.61/s2aff/timo/interface.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.60/s2aff.egg-info/SOURCES.txt` & `s2aff-0.61/s2aff.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `s2aff-0.60/scripts/approximate_runtime_and_memory_usage.py` & `s2aff-0.61/scripts/approximate_runtime_and_memory_usage.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.60/scripts/evaluate_first_stage_ranker.py` & `s2aff-0.61/scripts/evaluate_first_stage_ranker.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.60/scripts/generate_lightgbm_training_data.py` & `s2aff-0.61/scripts/generate_lightgbm_training_data.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.60/scripts/train_lightgbm_reranker.py` & `s2aff-0.61/scripts/train_lightgbm_reranker.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.60/scripts/train_ner_model.py` & `s2aff-0.61/scripts/train_ner_model.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.60/scripts/update_openalex_works_counts.py` & `s2aff-0.61/scripts/update_openalex_works_counts.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.60/setup.py` & `s2aff-0.61/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,13 +3,13 @@
 from os import path
 
 requirements_file = path.join(path.dirname(__file__), "requirements.in")
 requirements = [r for r in open(requirements_file).read().split("\n") if not re.match(r"^\-", r)]
 
 setuptools.setup(
     name="s2aff",
-    version="0.60",
+    version="0.61",
     url="https://github.com/allenai/S2AFF",
     packages=setuptools.find_packages(),
     install_requires=requirements,  # dependencies specified in requirements.in
     description="Semantic Scholar's Affiliation Extraction: Link Your Raw Affiliations to ROR IDs",
 )
```

