# Comparing `tmp/stable-ts-2.6.3.tar.gz` & `tmp/stable-ts-2.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stable-ts-2.6.3.tar", last modified: Fri Jun  9 01:27:22 2023, max compression
+gzip compressed data, was "stable-ts-2.6.4.tar", last modified: Fri Jun  9 16:54:09 2023, max compression
```

## Comparing `stable-ts-2.6.3.tar` & `stable-ts-2.6.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 01:27:22.452035 stable-ts-2.6.3/
--rw-rw-rw-   0        0        0     1082 2022-11-20 18:10:26.000000 stable-ts-2.6.3/LICENSE
--rw-rw-rw-   0        0        0    11608 2023-06-09 01:27:22.452035 stable-ts-2.6.3/PKG-INFO
--rw-rw-rw-   0        0        0    11312 2023-06-09 01:22:48.000000 stable-ts-2.6.3/README.md
--rw-rw-rw-   0        0        0       42 2023-06-09 01:27:22.452035 stable-ts-2.6.3/setup.cfg
--rw-rw-rw-   0        0        0     1100 2023-03-25 19:12:43.000000 stable-ts-2.6.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-09 01:27:22.385313 stable-ts-2.6.3/stable_ts.egg-info/
--rw-rw-rw-   0        0        0    11608 2023-06-09 01:27:22.000000 stable-ts-2.6.3/stable_ts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      597 2023-06-09 01:27:22.000000 stable-ts-2.6.3/stable_ts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 01:27:22.000000 stable-ts-2.6.3/stable_ts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2023-06-09 01:27:22.000000 stable-ts-2.6.3/stable_ts.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      110 2023-06-09 01:27:22.000000 stable-ts-2.6.3/stable_ts.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-09 01:27:22.000000 stable-ts-2.6.3/stable_ts.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-09 01:27:22.449412 stable-ts-2.6.3/stable_whisper/
--rw-rw-rw-   0        0        0      200 2023-03-17 04:40:26.000000 stable-ts-2.6.3/stable_whisper/__init__.py
--rw-rw-rw-   0        0        0       44 2023-02-15 00:11:21.000000 stable-ts-2.6.3/stable_whisper/__main__.py
--rw-rw-rw-   0        0        0       23 2023-06-09 00:03:52.000000 stable-ts-2.6.3/stable_whisper/_version.py
--rw-rw-rw-   0        0        0     7619 2023-04-28 17:05:35.000000 stable-ts-2.6.3/stable_whisper/audio.py
--rw-rw-rw-   0        0        0     4373 2023-04-24 04:50:11.000000 stable-ts-2.6.3/stable_whisper/decode.py
--rw-rw-rw-   0        0        0    15934 2023-04-28 16:52:08.000000 stable-ts-2.6.3/stable_whisper/enhancement.py
--rw-rw-rw-   0        0        0     1645 2023-05-03 19:33:54.000000 stable-ts-2.6.3/stable_whisper/quantization.py
--rw-rw-rw-   0        0        0    40573 2023-06-09 01:03:20.000000 stable-ts-2.6.3/stable_whisper/result.py
--rw-rw-rw-   0        0        0    13540 2023-05-09 17:04:10.000000 stable-ts-2.6.3/stable_whisper/stabilization.py
--rw-rw-rw-   0        0        0    20528 2023-05-08 02:53:22.000000 stable-ts-2.6.3/stable_whisper/text_output.py
--rw-rw-rw-   0        0        0    10370 2023-04-24 04:57:46.000000 stable-ts-2.6.3/stable_whisper/timing.py
--rw-rw-rw-   0        0        0     2265 2023-03-17 01:46:33.000000 stable-ts-2.6.3/stable_whisper/video_output.py
--rw-rw-rw-   0        0        0    53432 2023-06-09 00:02:50.000000 stable-ts-2.6.3/stable_whisper/whisper_word_level.py
+drwxrwxrwx   0        0        0        0 2023-06-09 16:54:09.808747 stable-ts-2.6.4/
+-rw-rw-rw-   0        0        0     1082 2022-11-20 18:10:26.000000 stable-ts-2.6.4/LICENSE
+-rw-rw-rw-   0        0        0    11608 2023-06-09 16:54:09.807744 stable-ts-2.6.4/PKG-INFO
+-rw-rw-rw-   0        0        0    11312 2023-06-09 01:22:48.000000 stable-ts-2.6.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-09 16:54:09.808747 stable-ts-2.6.4/setup.cfg
+-rw-rw-rw-   0        0        0     1100 2023-03-25 19:12:43.000000 stable-ts-2.6.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 16:54:09.749234 stable-ts-2.6.4/stable_ts.egg-info/
+-rw-rw-rw-   0        0        0    11608 2023-06-09 16:54:09.000000 stable-ts-2.6.4/stable_ts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      597 2023-06-09 16:54:09.000000 stable-ts-2.6.4/stable_ts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 16:54:09.000000 stable-ts-2.6.4/stable_ts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2023-06-09 16:54:09.000000 stable-ts-2.6.4/stable_ts.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      110 2023-06-09 16:54:09.000000 stable-ts-2.6.4/stable_ts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-09 16:54:09.000000 stable-ts-2.6.4/stable_ts.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 16:54:09.805738 stable-ts-2.6.4/stable_whisper/
+-rw-rw-rw-   0        0        0      200 2023-03-17 04:40:26.000000 stable-ts-2.6.4/stable_whisper/__init__.py
+-rw-rw-rw-   0        0        0       44 2023-02-15 00:11:21.000000 stable-ts-2.6.4/stable_whisper/__main__.py
+-rw-rw-rw-   0        0        0       23 2023-06-09 16:50:46.000000 stable-ts-2.6.4/stable_whisper/_version.py
+-rw-rw-rw-   0        0        0     7619 2023-04-28 17:05:35.000000 stable-ts-2.6.4/stable_whisper/audio.py
+-rw-rw-rw-   0        0        0     4373 2023-04-24 04:50:11.000000 stable-ts-2.6.4/stable_whisper/decode.py
+-rw-rw-rw-   0        0        0    15934 2023-04-28 16:52:08.000000 stable-ts-2.6.4/stable_whisper/enhancement.py
+-rw-rw-rw-   0        0        0     1645 2023-05-03 19:33:54.000000 stable-ts-2.6.4/stable_whisper/quantization.py
+-rw-rw-rw-   0        0        0    40573 2023-06-09 01:03:20.000000 stable-ts-2.6.4/stable_whisper/result.py
+-rw-rw-rw-   0        0        0    13540 2023-05-09 17:04:10.000000 stable-ts-2.6.4/stable_whisper/stabilization.py
+-rw-rw-rw-   0        0        0    20528 2023-05-08 02:53:22.000000 stable-ts-2.6.4/stable_whisper/text_output.py
+-rw-rw-rw-   0        0        0    10370 2023-04-24 04:57:46.000000 stable-ts-2.6.4/stable_whisper/timing.py
+-rw-rw-rw-   0        0        0     2265 2023-03-17 01:46:33.000000 stable-ts-2.6.4/stable_whisper/video_output.py
+-rw-rw-rw-   0        0        0    53434 2023-06-09 16:49:15.000000 stable-ts-2.6.4/stable_whisper/whisper_word_level.py
```

### Comparing `stable-ts-2.6.3/LICENSE` & `stable-ts-2.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `stable-ts-2.6.3/PKG-INFO` & `stable-ts-2.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stable-ts
-Version: 2.6.3
+Version: 2.6.4
 Summary: Modifies OpenAI's Whisper to produce more reliable timestamps.
 Home-page: https://github.com/jianfch/stable-ts
 Author: Jian
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `stable-ts-2.6.3/README.md` & `stable-ts-2.6.4/README.md`

 * *Files identical despite different names*

### Comparing `stable-ts-2.6.3/setup.py` & `stable-ts-2.6.4/setup.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.6.3/stable_ts.egg-info/PKG-INFO` & `stable-ts-2.6.4/stable_ts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stable-ts
-Version: 2.6.3
+Version: 2.6.4
 Summary: Modifies OpenAI's Whisper to produce more reliable timestamps.
 Home-page: https://github.com/jianfch/stable-ts
 Author: Jian
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `stable-ts-2.6.3/stable_ts.egg-info/SOURCES.txt` & `stable-ts-2.6.4/stable_ts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stable-ts-2.6.3/stable_whisper/audio.py` & `stable-ts-2.6.4/stable_whisper/audio.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.6.3/stable_whisper/decode.py` & `stable-ts-2.6.4/stable_whisper/decode.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.6.3/stable_whisper/enhancement.py` & `stable-ts-2.6.4/stable_whisper/enhancement.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.6.3/stable_whisper/quantization.py` & `stable-ts-2.6.4/stable_whisper/quantization.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.6.3/stable_whisper/result.py` & `stable-ts-2.6.4/stable_whisper/result.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.6.3/stable_whisper/stabilization.py` & `stable-ts-2.6.4/stable_whisper/stabilization.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.6.3/stable_whisper/text_output.py` & `stable-ts-2.6.4/stable_whisper/text_output.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.6.3/stable_whisper/timing.py` & `stable-ts-2.6.4/stable_whisper/timing.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.6.3/stable_whisper/video_output.py` & `stable-ts-2.6.4/stable_whisper/video_output.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.6.3/stable_whisper/whisper_word_level.py` & `stable-ts-2.6.4/stable_whisper/whisper_word_level.py`

 * *Files 0% similar despite different names*

```diff
@@ -744,15 +744,15 @@
                              "earlier than the first utterance")
 
     parser.add_argument("--word_timestamps", type=str2bool, default=True,
                         help="extract word-level timestamps using the cross-attention pattern and dynamic time warping,"
                              "and include the timestamps for each word in each segment;"
                              "disabling this will prevent segments from splitting/merging properly.")
 
-    parser.add_argument("--regroup", type=str, default=True,
+    parser.add_argument("--regroup", type=str, default="True",
                         help="whether to regroup all words into segments with more natural boundaries;"
                              "specify string for customizing the regrouping algorithm"
                              "ignored if [word_timestamps]=False.")
 
     parser.add_argument('--ts_num', type=int, default=0,
                         help="number of extra inferences to perform to find the mean timestamps")
     parser.add_argument('--ts_noise', type=float, default=0.1,
```

