# Comparing `tmp/stable-ts-2.6.2.tar.gz` & `tmp/stable-ts-2.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stable-ts-2.6.2.tar", last modified: Tue May  9 17:17:28 2023, max compression
+gzip compressed data, was "stable-ts-2.6.3.tar", last modified: Fri Jun  9 01:27:22 2023, max compression
```

## Comparing `stable-ts-2.6.2.tar` & `stable-ts-2.6.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 17:17:28.511973 stable-ts-2.6.2/
--rw-rw-rw-   0        0        0     1082 2022-11-20 18:10:26.000000 stable-ts-2.6.2/LICENSE
--rw-rw-rw-   0        0        0    11221 2023-05-09 17:17:28.510972 stable-ts-2.6.2/PKG-INFO
--rw-rw-rw-   0        0        0    10925 2023-05-09 03:44:10.000000 stable-ts-2.6.2/README.md
--rw-rw-rw-   0        0        0       42 2023-05-09 17:17:28.511973 stable-ts-2.6.2/setup.cfg
--rw-rw-rw-   0        0        0     1100 2023-03-25 19:12:43.000000 stable-ts-2.6.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-09 17:17:28.454921 stable-ts-2.6.2/stable_ts.egg-info/
--rw-rw-rw-   0        0        0    11221 2023-05-09 17:17:28.000000 stable-ts-2.6.2/stable_ts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      597 2023-05-09 17:17:28.000000 stable-ts-2.6.2/stable_ts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 17:17:28.000000 stable-ts-2.6.2/stable_ts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2023-05-09 17:17:28.000000 stable-ts-2.6.2/stable_ts.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      110 2023-05-09 17:17:28.000000 stable-ts-2.6.2/stable_ts.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-09 17:17:28.000000 stable-ts-2.6.2/stable_ts.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-09 17:17:28.508971 stable-ts-2.6.2/stable_whisper/
--rw-rw-rw-   0        0        0      200 2023-03-17 04:40:26.000000 stable-ts-2.6.2/stable_whisper/__init__.py
--rw-rw-rw-   0        0        0       44 2023-02-15 00:11:21.000000 stable-ts-2.6.2/stable_whisper/__main__.py
--rw-rw-rw-   0        0        0       23 2023-05-09 17:08:07.000000 stable-ts-2.6.2/stable_whisper/_version.py
--rw-rw-rw-   0        0        0     7619 2023-04-28 17:05:35.000000 stable-ts-2.6.2/stable_whisper/audio.py
--rw-rw-rw-   0        0        0     4373 2023-04-24 04:50:11.000000 stable-ts-2.6.2/stable_whisper/decode.py
--rw-rw-rw-   0        0        0    15934 2023-04-28 16:52:08.000000 stable-ts-2.6.2/stable_whisper/enhancement.py
--rw-rw-rw-   0        0        0     1645 2023-05-03 19:33:54.000000 stable-ts-2.6.2/stable_whisper/quantization.py
--rw-rw-rw-   0        0        0    37293 2023-05-09 01:32:32.000000 stable-ts-2.6.2/stable_whisper/result.py
--rw-rw-rw-   0        0        0    13540 2023-05-09 17:04:10.000000 stable-ts-2.6.2/stable_whisper/stabilization.py
--rw-rw-rw-   0        0        0    20528 2023-05-08 02:53:22.000000 stable-ts-2.6.2/stable_whisper/text_output.py
--rw-rw-rw-   0        0        0    10370 2023-04-24 04:57:46.000000 stable-ts-2.6.2/stable_whisper/timing.py
--rw-rw-rw-   0        0        0     2265 2023-03-17 01:46:33.000000 stable-ts-2.6.2/stable_whisper/video_output.py
--rw-rw-rw-   0        0        0    53068 2023-05-09 17:03:34.000000 stable-ts-2.6.2/stable_whisper/whisper_word_level.py
+drwxrwxrwx   0        0        0        0 2023-06-09 01:27:22.452035 stable-ts-2.6.3/
+-rw-rw-rw-   0        0        0     1082 2022-11-20 18:10:26.000000 stable-ts-2.6.3/LICENSE
+-rw-rw-rw-   0        0        0    11608 2023-06-09 01:27:22.452035 stable-ts-2.6.3/PKG-INFO
+-rw-rw-rw-   0        0        0    11312 2023-06-09 01:22:48.000000 stable-ts-2.6.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-09 01:27:22.452035 stable-ts-2.6.3/setup.cfg
+-rw-rw-rw-   0        0        0     1100 2023-03-25 19:12:43.000000 stable-ts-2.6.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 01:27:22.385313 stable-ts-2.6.3/stable_ts.egg-info/
+-rw-rw-rw-   0        0        0    11608 2023-06-09 01:27:22.000000 stable-ts-2.6.3/stable_ts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      597 2023-06-09 01:27:22.000000 stable-ts-2.6.3/stable_ts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 01:27:22.000000 stable-ts-2.6.3/stable_ts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2023-06-09 01:27:22.000000 stable-ts-2.6.3/stable_ts.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      110 2023-06-09 01:27:22.000000 stable-ts-2.6.3/stable_ts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-09 01:27:22.000000 stable-ts-2.6.3/stable_ts.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 01:27:22.449412 stable-ts-2.6.3/stable_whisper/
+-rw-rw-rw-   0        0        0      200 2023-03-17 04:40:26.000000 stable-ts-2.6.3/stable_whisper/__init__.py
+-rw-rw-rw-   0        0        0       44 2023-02-15 00:11:21.000000 stable-ts-2.6.3/stable_whisper/__main__.py
+-rw-rw-rw-   0        0        0       23 2023-06-09 00:03:52.000000 stable-ts-2.6.3/stable_whisper/_version.py
+-rw-rw-rw-   0        0        0     7619 2023-04-28 17:05:35.000000 stable-ts-2.6.3/stable_whisper/audio.py
+-rw-rw-rw-   0        0        0     4373 2023-04-24 04:50:11.000000 stable-ts-2.6.3/stable_whisper/decode.py
+-rw-rw-rw-   0        0        0    15934 2023-04-28 16:52:08.000000 stable-ts-2.6.3/stable_whisper/enhancement.py
+-rw-rw-rw-   0        0        0     1645 2023-05-03 19:33:54.000000 stable-ts-2.6.3/stable_whisper/quantization.py
+-rw-rw-rw-   0        0        0    40573 2023-06-09 01:03:20.000000 stable-ts-2.6.3/stable_whisper/result.py
+-rw-rw-rw-   0        0        0    13540 2023-05-09 17:04:10.000000 stable-ts-2.6.3/stable_whisper/stabilization.py
+-rw-rw-rw-   0        0        0    20528 2023-05-08 02:53:22.000000 stable-ts-2.6.3/stable_whisper/text_output.py
+-rw-rw-rw-   0        0        0    10370 2023-04-24 04:57:46.000000 stable-ts-2.6.3/stable_whisper/timing.py
+-rw-rw-rw-   0        0        0     2265 2023-03-17 01:46:33.000000 stable-ts-2.6.3/stable_whisper/video_output.py
+-rw-rw-rw-   0        0        0    53432 2023-06-09 00:02:50.000000 stable-ts-2.6.3/stable_whisper/whisper_word_level.py
```

### Comparing `stable-ts-2.6.2/LICENSE` & `stable-ts-2.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `stable-ts-2.6.2/PKG-INFO` & `stable-ts-2.6.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stable-ts
-Version: 2.6.2
+Version: 2.6.3
 Summary: Modifies OpenAI's Whisper to produce more reliable timestamps.
 Home-page: https://github.com/jianfch/stable-ts
 Author: Jian
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -119,33 +119,35 @@
 result = stable_whisper.WhisperResult('audio.json')
 result.to_srt_vtt('audio.srt')
 ```
 
 ### Regrouping Words
 Stable-ts has a preset for regrouping words into different segments with more natural boundaries. 
 This preset is enabled by `regroup=True` (default). 
-But there are other built-in [regrouping methods](#regrouping-methods) that allow you to customize the regrouping logic. 
+But there are other built-in [regrouping methods](#regrouping-methods) that allow you to customize the regrouping algorithm. 
 This preset is just a predefined combination of those methods.
 
 https://user-images.githubusercontent.com/28970749/226504985-3d087539-cfa4-46d1-8eb5-7083f235b429.mp4
 
 ```python
+# The following all functionally equivalent:
 result0 = model.transcribe('audio.mp3', regroup=True) # regroup is True by default
-# regroup=True is same as below
 result1 = model.transcribe('audio.mp3', regroup=False)
 (
     result1
     .split_by_punctuation([('.', ' '), '。', '?', '？', ',', '，'])
     .split_by_gap(.5)
     .merge_by_gap(.15, max_words=3)
     .split_by_punctuation([('.', ' '), '。', '?', '？'])
 )
-# result0 == result1
+result2 = model.transcribe('audio.mp3', regroup='sp=.* /。/?/？/,/，_sg=.5_mg=.15+3_sp=.* /。/?/？')
 ```
+Any regrouping algorithm can be expressed as a string. Please feel free share your strings [here](https://github.com/jianfch/stable-ts/discussions/162)
 #### Regrouping Methods
+- [regroup](https://github.com/jianfch/stable-ts/blob/7c6953526dce5d9058b23e8d0c223272bf808be7/stable_whisper/result.py#L808-L854)
 - [split_by_gap()](https://github.com/jianfch/stable-ts/blob/7c6953526dce5d9058b23e8d0c223272bf808be7/stable_whisper/result.py#L526-L543)
 - [split_by_punctuation()](https://github.com/jianfch/stable-ts/blob/7c6953526dce5d9058b23e8d0c223272bf808be7/stable_whisper/result.py#L579-L595)
 - [split_by_length()](https://github.com/jianfch/stable-ts/blob/7c6953526dce5d9058b23e8d0c223272bf808be7/stable_whisper/result.py#L637-L658)
 - [merge_by_gap()](https://github.com/jianfch/stable-ts/blob/7c6953526dce5d9058b23e8d0c223272bf808be7/stable_whisper/result.py#L547-L573)
 - [merge_by_punctuation()](https://github.com/jianfch/stable-ts/blob/7c6953526dce5d9058b23e8d0c223272bf808be7/stable_whisper/result.py#L599-L624)
 - [merge_all_segments()](https://github.com/jianfch/stable-ts/blob/7c6953526dce5d9058b23e8d0c223272bf808be7/stable_whisper/result.py#L630-L633)
 
@@ -166,15 +168,15 @@
 for match in matches:
   print(f'match: {match.text_match}\n'
         f'text: {match.text}\n'
         f'start: {match.start}\n'
         f'end: {match.end}\n')
 ```
 Parameters: 
-[find()](https://github.com/jianfch/stable-ts/blob/d30d0d1cfb5b17b4bf59c3fafcbbd21e37598ab9/stable_whisper/result.py#L768-L773)
+[find()](https://github.com/jianfch/stable-ts/blob/d30d0d1cfb5b17b4bf59c3fafcbbd21e37598ab9/stable_whisper/result.py#L898-L913)
 
 ### Boosting Performance
 * One of the methods that Stable-ts uses to increase timestamp accuracy 
 and reduce hallucinations is silence suppression, enabled with `suppress_silence=True` (default).
 This method essentially suppresses the timestamps where the audio is silent or contain no speech
 by suppressing the corresponding tokens during inference and also readjusting the timestamps after inference. 
 To figure out which parts of the audio track are silent or contain no speech, Stable-ts supports non-VAD and VAD methods.
```

### Comparing `stable-ts-2.6.2/README.md` & `stable-ts-2.6.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -108,33 +108,35 @@
 result = stable_whisper.WhisperResult('audio.json')
 result.to_srt_vtt('audio.srt')
 ```
 
 ### Regrouping Words
 Stable-ts has a preset for regrouping words into different segments with more natural boundaries. 
 This preset is enabled by `regroup=True` (default). 
-But there are other built-in [regrouping methods](#regrouping-methods) that allow you to customize the regrouping logic. 
+But there are other built-in [regrouping methods](#regrouping-methods) that allow you to customize the regrouping algorithm. 
 This preset is just a predefined combination of those methods.
 
 https://user-images.githubusercontent.com/28970749/226504985-3d087539-cfa4-46d1-8eb5-7083f235b429.mp4
 
 ```python
+# The following all functionally equivalent:
 result0 = model.transcribe('audio.mp3', regroup=True) # regroup is True by default
-# regroup=True is same as below
 result1 = model.transcribe('audio.mp3', regroup=False)
 (
     result1
     .split_by_punctuation([('.', ' '), '。', '?', '？', ',', '，'])
     .split_by_gap(.5)
     .merge_by_gap(.15, max_words=3)
     .split_by_punctuation([('.', ' '), '。', '?', '？'])
 )
-# result0 == result1
+result2 = model.transcribe('audio.mp3', regroup='sp=.* /。/?/？/,/，_sg=.5_mg=.15+3_sp=.* /。/?/？')
 ```
+Any regrouping algorithm can be expressed as a string. Please feel free share your strings [here](https://github.com/jianfch/stable-ts/discussions/162)
 #### Regrouping Methods
+- [regroup](https://github.com/jianfch/stable-ts/blob/7c6953526dce5d9058b23e8d0c223272bf808be7/stable_whisper/result.py#L808-L854)
 - [split_by_gap()](https://github.com/jianfch/stable-ts/blob/7c6953526dce5d9058b23e8d0c223272bf808be7/stable_whisper/result.py#L526-L543)
 - [split_by_punctuation()](https://github.com/jianfch/stable-ts/blob/7c6953526dce5d9058b23e8d0c223272bf808be7/stable_whisper/result.py#L579-L595)
 - [split_by_length()](https://github.com/jianfch/stable-ts/blob/7c6953526dce5d9058b23e8d0c223272bf808be7/stable_whisper/result.py#L637-L658)
 - [merge_by_gap()](https://github.com/jianfch/stable-ts/blob/7c6953526dce5d9058b23e8d0c223272bf808be7/stable_whisper/result.py#L547-L573)
 - [merge_by_punctuation()](https://github.com/jianfch/stable-ts/blob/7c6953526dce5d9058b23e8d0c223272bf808be7/stable_whisper/result.py#L599-L624)
 - [merge_all_segments()](https://github.com/jianfch/stable-ts/blob/7c6953526dce5d9058b23e8d0c223272bf808be7/stable_whisper/result.py#L630-L633)
 
@@ -155,15 +157,15 @@
 for match in matches:
   print(f'match: {match.text_match}\n'
         f'text: {match.text}\n'
         f'start: {match.start}\n'
         f'end: {match.end}\n')
 ```
 Parameters: 
-[find()](https://github.com/jianfch/stable-ts/blob/d30d0d1cfb5b17b4bf59c3fafcbbd21e37598ab9/stable_whisper/result.py#L768-L773)
+[find()](https://github.com/jianfch/stable-ts/blob/d30d0d1cfb5b17b4bf59c3fafcbbd21e37598ab9/stable_whisper/result.py#L898-L913)
 
 ### Boosting Performance
 * One of the methods that Stable-ts uses to increase timestamp accuracy 
 and reduce hallucinations is silence suppression, enabled with `suppress_silence=True` (default).
 This method essentially suppresses the timestamps where the audio is silent or contain no speech
 by suppressing the corresponding tokens during inference and also readjusting the timestamps after inference. 
 To figure out which parts of the audio track are silent or contain no speech, Stable-ts supports non-VAD and VAD methods.
```

### Comparing `stable-ts-2.6.2/setup.py` & `stable-ts-2.6.3/setup.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.6.2/stable_ts.egg-info/PKG-INFO` & `stable-ts-2.6.3/stable_ts.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stable-ts
-Version: 2.6.2
+Version: 2.6.3
 Summary: Modifies OpenAI's Whisper to produce more reliable timestamps.
 Home-page: https://github.com/jianfch/stable-ts
 Author: Jian
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -119,33 +119,35 @@
 result = stable_whisper.WhisperResult('audio.json')
 result.to_srt_vtt('audio.srt')
 ```
 
 ### Regrouping Words
 Stable-ts has a preset for regrouping words into different segments with more natural boundaries. 
 This preset is enabled by `regroup=True` (default). 
-But there are other built-in [regrouping methods](#regrouping-methods) that allow you to customize the regrouping logic. 
+But there are other built-in [regrouping methods](#regrouping-methods) that allow you to customize the regrouping algorithm. 
 This preset is just a predefined combination of those methods.
 
 https://user-images.githubusercontent.com/28970749/226504985-3d087539-cfa4-46d1-8eb5-7083f235b429.mp4
 
 ```python
+# The following all functionally equivalent:
 result0 = model.transcribe('audio.mp3', regroup=True) # regroup is True by default
-# regroup=True is same as below
 result1 = model.transcribe('audio.mp3', regroup=False)
 (
     result1
     .split_by_punctuation([('.', ' '), '。', '?', '？', ',', '，'])
     .split_by_gap(.5)
     .merge_by_gap(.15, max_words=3)
     .split_by_punctuation([('.', ' '), '。', '?', '？'])
 )
-# result0 == result1
+result2 = model.transcribe('audio.mp3', regroup='sp=.* /。/?/？/,/，_sg=.5_mg=.15+3_sp=.* /。/?/？')
 ```
+Any regrouping algorithm can be expressed as a string. Please feel free share your strings [here](https://github.com/jianfch/stable-ts/discussions/162)
 #### Regrouping Methods
+- [regroup](https://github.com/jianfch/stable-ts/blob/7c6953526dce5d9058b23e8d0c223272bf808be7/stable_whisper/result.py#L808-L854)
 - [split_by_gap()](https://github.com/jianfch/stable-ts/blob/7c6953526dce5d9058b23e8d0c223272bf808be7/stable_whisper/result.py#L526-L543)
 - [split_by_punctuation()](https://github.com/jianfch/stable-ts/blob/7c6953526dce5d9058b23e8d0c223272bf808be7/stable_whisper/result.py#L579-L595)
 - [split_by_length()](https://github.com/jianfch/stable-ts/blob/7c6953526dce5d9058b23e8d0c223272bf808be7/stable_whisper/result.py#L637-L658)
 - [merge_by_gap()](https://github.com/jianfch/stable-ts/blob/7c6953526dce5d9058b23e8d0c223272bf808be7/stable_whisper/result.py#L547-L573)
 - [merge_by_punctuation()](https://github.com/jianfch/stable-ts/blob/7c6953526dce5d9058b23e8d0c223272bf808be7/stable_whisper/result.py#L599-L624)
 - [merge_all_segments()](https://github.com/jianfch/stable-ts/blob/7c6953526dce5d9058b23e8d0c223272bf808be7/stable_whisper/result.py#L630-L633)
 
@@ -166,15 +168,15 @@
 for match in matches:
   print(f'match: {match.text_match}\n'
         f'text: {match.text}\n'
         f'start: {match.start}\n'
         f'end: {match.end}\n')
 ```
 Parameters: 
-[find()](https://github.com/jianfch/stable-ts/blob/d30d0d1cfb5b17b4bf59c3fafcbbd21e37598ab9/stable_whisper/result.py#L768-L773)
+[find()](https://github.com/jianfch/stable-ts/blob/d30d0d1cfb5b17b4bf59c3fafcbbd21e37598ab9/stable_whisper/result.py#L898-L913)
 
 ### Boosting Performance
 * One of the methods that Stable-ts uses to increase timestamp accuracy 
 and reduce hallucinations is silence suppression, enabled with `suppress_silence=True` (default).
 This method essentially suppresses the timestamps where the audio is silent or contain no speech
 by suppressing the corresponding tokens during inference and also readjusting the timestamps after inference. 
 To figure out which parts of the audio track are silent or contain no speech, Stable-ts supports non-VAD and VAD methods.
```

### Comparing `stable-ts-2.6.2/stable_ts.egg-info/SOURCES.txt` & `stable-ts-2.6.3/stable_ts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stable-ts-2.6.2/stable_whisper/audio.py` & `stable-ts-2.6.3/stable_whisper/audio.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.6.2/stable_whisper/decode.py` & `stable-ts-2.6.3/stable_whisper/decode.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.6.2/stable_whisper/enhancement.py` & `stable-ts-2.6.3/stable_whisper/enhancement.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.6.2/stable_whisper/quantization.py` & `stable-ts-2.6.3/stable_whisper/quantization.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.6.2/stable_whisper/result.py` & `stable-ts-2.6.3/stable_whisper/result.py`

 * *Files 3% similar despite different names*

```diff
@@ -733,15 +733,16 @@
             Whether to prevent future splits/merges from altering changes made by this method. (Default: False)
 
         """
         self._split_segments(lambda x: x.get_punctuation_indices(punctuation), lock=lock)
         return self
 
     def merge_by_punctuation(
-            self, punctuation: Union[List[str], List[Tuple[str, str]], str],
+            self,
+            punctuation: Union[List[str], List[Tuple[str, str]], str],
             max_words: int = None,
             max_chars: int = None,
             is_sum_max: bool = False,
             lock: bool = False
     ):
         """
 
@@ -799,18 +800,96 @@
 
         """
         if force_len:
             self.merge_all_segments()
         self._split_segments(lambda x: x.get_length_indices(max_chars=max_chars, max_words=max_words), lock=lock)
         return self
 
-    def regroup(self):
+    def regroup(self, regroup_algo: str = None, verbose: bool = False, only_show: bool = False):
         """
+
         Regroup (in-place) all words into segments with more natural boundaries without locking.
-        """
+
+        Parameters
+        ----------
+        regroup_algo: str
+            string for customizing the regrouping algorithm
+
+                Method keys:
+                    sg: split_by_gap
+                    sp: split_by_punctuation
+                    sl: split_by_length
+                    mg: merge_by_gap
+                    mp: merge_by_punctuation
+                    ms: merge_all_segment
+
+                Metacharacters:
+                    = separates a method key and its arguments (not used if no argument)
+                    _ separates method keys (after arguments if there are any)
+                    + separates arguments for a method key
+                    / separates an argument into list of strings
+                    * separates an item in list of strings into a nested list of strings
+
+                -arguments are parsed positionally
+                -if no argument is provided, the default ones will be used
+                -use 1 or 0 to represent True or False
+
+                Example 1:
+                    merge_by_gap(.2, 10, lock=True)
+                    mg=.2+10+++1
+                    Note: [lock] is the 5th argument hence the 2 missing arguments inbetween the three + before 1
+
+                Example 2:
+                    split_by_punctuation([('.', ' '), '。', '?', '？'], True)
+                    sp=.* /。/?/？+1
+
+                Example 3:
+                    merge_all_segments().split_by_gap(.5).merge_by_gap(.15, 3)
+                    ms_sg=.5_mg=.15+3
+
+        verbose: bool
+            whether to show all the methods and arguments parsed from [regroup_algo]
+        only_show: bool
+            show the all methods and arguments parsed from [regroup_algo] without running the methods
+
+        """
+        if isinstance(regroup_algo, str):
+            methods = dict(
+                sg=self.split_by_gap,
+                sp=self.split_by_punctuation,
+                sl=self.split_by_length,
+                mg=self.merge_by_gap,
+                mp=self.merge_by_punctuation,
+                ms=self.merge_all_segments
+            )
+
+            def _to_arg(x: str):
+                if len(x) == 0:
+                    return None
+                if '/' in x:
+                    return [a.split('*') if '*' in a else a for a in x.split('/')]
+                try:
+                    x = float(x) if '.' in x else int(x)
+                except ValueError:
+                    pass
+                finally:
+                    return x
+
+            for method in regroup_algo.split('_'):
+                method, args = method.split('=', maxsplit=1) if '=' in method else (method, '')
+                if method not in methods:
+                    raise NotImplementedError(f'{method} is not one of the available methods: {tuple(methods.keys())}')
+                args = [] if len(args) == 0 else list(map(_to_arg, args.split('+')))
+                if verbose or only_show:
+                    print(f'{methods[method].__name__}({", ".join(map(str, args))})')
+                if not only_show:
+                    methods[method](*args)
+
+            return self
+
         return (
             self
             .split_by_punctuation([('.', ' '), '。', '?', '？', ',', '，'])
             .split_by_gap(.5)
             .merge_by_gap(.3, max_words=3)
             .split_by_punctuation([('.', ' '), '。', '?', '？'])
         )
```

### Comparing `stable-ts-2.6.2/stable_whisper/stabilization.py` & `stable-ts-2.6.3/stable_whisper/stabilization.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.6.2/stable_whisper/text_output.py` & `stable-ts-2.6.3/stable_whisper/text_output.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.6.2/stable_whisper/timing.py` & `stable-ts-2.6.3/stable_whisper/timing.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.6.2/stable_whisper/video_output.py` & `stable-ts-2.6.3/stable_whisper/video_output.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.6.2/stable_whisper/whisper_word_level.py` & `stable-ts-2.6.3/stable_whisper/whisper_word_level.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         temperature: Union[float, Tuple[float, ...]] = (0.0, 0.2, 0.4, 0.6, 0.8, 1.0),
         compression_ratio_threshold: Optional[float] = 2.4,
         logprob_threshold: Optional[float] = -1.0,
         no_speech_threshold: Optional[float] = 0.6,
         condition_on_previous_text: bool = True,
         initial_prompt: Optional[str] = None,
         word_timestamps: bool = True,
-        regroup: bool = True,
+        regroup: Union[bool, str] = True,
         ts_num: int = 0,
         ts_noise: float = 0.1,
         suppress_silence: bool = True,
         suppress_word_ts: bool = True,
         q_levels: int = 20,
         k_size: int = 5,
         time_scale: float = None,
@@ -107,16 +107,17 @@
         to make it more likely to predict those word correctly.
 
     word_timestamps: bool
         Extract word-level timestamps using the cross-attention pattern and dynamic time warping,
         and include the timestamps for each word in each segment. (Default: True)
         Disabling this will prevent segments from splitting/merging properly.
 
-    regroup: bool
-        Regroup all words into segments with more natural boundaries.(Default: True)
+    regroup: Union[bool, str]
+        Whether to regroup all words into segments with more natural boundaries. (Default: True)
+        Specify string for customizing the regrouping algorithm.
         Ignored if [word_timestamps]=False.
 
     ts_num: int
         Number of extra timestamp inferences to perform then use average of these extra timestamps. (Default: 0).
 
     ts_noise: float
         Percentage of noise to add to audio_features to perform inferences for [ts_num]. (Default: 0.1)
@@ -603,15 +604,15 @@
 
     text = '' if tokenizer is None else tokenizer.decode(all_tokens[len(initial_prompt_tokens):])
     final_result = WhisperResult(dict(text=text,
                                       segments=all_segments,
                                       language=language,
                                       time_scale=time_scale))
     if word_timestamps and regroup:
-        final_result.regroup()
+        final_result.regroup(regroup)
 
     if time_scale is not None:
         final_result.rescale_time(1 / time_scale)
 
     if len(final_result.text) == 0:
         warnings.warn(f'Failed to {task} audio. Result contains no text. ')
 
@@ -743,16 +744,17 @@
                              "earlier than the first utterance")
 
     parser.add_argument("--word_timestamps", type=str2bool, default=True,
                         help="extract word-level timestamps using the cross-attention pattern and dynamic time warping,"
                              "and include the timestamps for each word in each segment;"
                              "disabling this will prevent segments from splitting/merging properly.")
 
-    parser.add_argument("--regroup", type=str2bool, default=True,
-                        help="regroup all words into segments with more natural boundaries;"
+    parser.add_argument("--regroup", type=str, default=True,
+                        help="whether to regroup all words into segments with more natural boundaries;"
+                             "specify string for customizing the regrouping algorithm"
                              "ignored if [word_timestamps]=False.")
 
     parser.add_argument('--ts_num', type=int, default=0,
                         help="number of extra inferences to perform to find the mean timestamps")
     parser.add_argument('--ts_noise', type=float, default=0.1,
                         help="percentage of noise to add to audio_features to perform inferences for [ts_num]")
 
@@ -900,14 +902,20 @@
     use_demucs = args.pop('demucs')
     demucs_outputs: List[Optional[str]] = args.pop("demucs_output")
     regroup = args.pop('regroup')
     max_chars = args.pop('max_chars')
     max_words = args.pop('max_words')
     reverse_text = args.pop('reverse_text')
 
+    if regroup:
+        try:
+            regroup = str2bool(regroup)
+        except ValueError:
+            pass
+
     if outputs:
         unsupported_formats = set(splitext(o)[-1].lower().strip('.') for o in outputs) - output_formats
         if len(unsupported_formats) != 0:
             raise NotImplementedError(f'{unsupported_formats} are not supported. Supported formats: {outputs}.')
 
     has_demucs_output = bool(demucs_outputs)
     if use_demucs and has_demucs_output and len(demucs_outputs) != len(inputs):
@@ -1074,15 +1082,15 @@
                 if model_loading_str:
                     print(f'Loaded {model_loading_str}  ')
             args['regroup'] = False
             result: WhisperResult = model.transcribe(input_audio, **args)
 
         if args.get('word_timestamps'):
             if regroup:
-                result.regroup()
+                result.regroup(regroup, verbose=args['verbose'] or debug)
             if max_chars or max_words:
                 result.split_by_length(max_chars=max_chars, max_words=max_words)
 
         if reverse_text:
             reverse_text = (args.get('prepend_punctuations'), args.get('append_punctuations'))
         make_parent(output_path)
         if is_json(output_path):
```

