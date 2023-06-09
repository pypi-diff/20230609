# Comparing `tmp/muxtools-0.0.5.tar.gz` & `tmp/muxtools-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muxtools-0.0.5.tar", last modified: Mon Jun  5 18:42:28 2023, max compression
+gzip compressed data, was "muxtools-0.0.6.tar", last modified: Fri Jun  9 15:26:25 2023, max compression
```

## Comparing `muxtools-0.0.5.tar` & `muxtools-0.0.6.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 18:42:28.639931 muxtools-0.0.5/
--rw-rw-rw-   0        0        0    17098 2023-05-19 19:09:14.000000 muxtools-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     1115 2023-06-05 18:42:28.638931 muxtools-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      112 2023-05-27 13:25:07.000000 muxtools-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-05 18:42:28.604832 muxtools-0.0.5/muxtools/
--rw-rw-rw-   0        0        0      810 2023-05-31 22:50:01.000000 muxtools-0.0.5/muxtools/__init__.py
--rw-rw-rw-   0        0        0       72 2023-05-31 22:50:01.000000 muxtools-0.0.5/muxtools/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 18:42:28.623841 muxtools-0.0.5/muxtools/audio/
--rw-rw-rw-   0        0        0      190 2023-06-01 17:13:19.000000 muxtools-0.0.5/muxtools/audio/__init__.py
--rw-rw-rw-   0        0        0    11068 2023-06-03 01:30:34.000000 muxtools-0.0.5/muxtools/audio/audioutils.py
--rw-rw-rw-   0        0        0    14858 2023-06-04 10:23:26.000000 muxtools-0.0.5/muxtools/audio/encoders.py
--rw-rw-rw-   0        0        0    16812 2023-06-03 00:49:40.000000 muxtools-0.0.5/muxtools/audio/extractors.py
--rw-rw-rw-   0        0        0     9133 2023-06-03 01:36:04.000000 muxtools-0.0.5/muxtools/audio/memecoders.py
--rw-rw-rw-   0        0        0      962 2023-06-01 11:53:30.000000 muxtools-0.0.5/muxtools/audio/tools.py
--rw-rw-rw-   0        0        0     7680 2023-06-01 16:53:16.000000 muxtools-0.0.5/muxtools/cli.py
--rw-rw-rw-   0        0        0     3282 2023-06-02 21:32:44.000000 muxtools-0.0.5/muxtools/functions.py
--rw-rw-rw-   0        0        0     4589 2023-05-31 22:50:01.000000 muxtools-0.0.5/muxtools/main.py
-drwxrwxrwx   0        0        0        0 2023-06-05 18:42:28.624841 muxtools-0.0.5/muxtools/misc/
--rw-rw-rw-   0        0        0       51 2023-06-01 16:53:33.000000 muxtools-0.0.5/muxtools/misc/__init__.py
--rw-rw-rw-   0        0        0     7596 2023-06-04 11:54:07.000000 muxtools-0.0.5/muxtools/misc/chapters.py
-drwxrwxrwx   0        0        0        0 2023-06-05 18:42:28.628841 muxtools-0.0.5/muxtools/muxing/
--rw-rw-rw-   0        0        0      129 2023-05-31 22:50:01.000000 muxtools-0.0.5/muxtools/muxing/__init__.py
--rw-rw-rw-   0        0        0     4718 2023-06-04 21:27:11.000000 muxtools-0.0.5/muxtools/muxing/mux.py
--rw-rw-rw-   0        0        0     4403 2023-06-03 01:13:02.000000 muxtools-0.0.5/muxtools/muxing/muxfiles.py
--rw-rw-rw-   0        0        0     6371 2023-05-31 22:50:01.000000 muxtools-0.0.5/muxtools/muxing/tmdb.py
--rw-rw-rw-   0        0        0     6836 2023-06-04 10:19:37.000000 muxtools-0.0.5/muxtools/muxing/tracks.py
-drwxrwxrwx   0        0        0        0 2023-06-05 18:42:28.631842 muxtools-0.0.5/muxtools/subtitle/
--rw-rw-rw-   0        0        0      128 2023-05-31 22:50:01.000000 muxtools-0.0.5/muxtools/subtitle/__init__.py
--rw-rw-rw-   0        0        0     1621 2023-06-04 10:32:35.000000 muxtools-0.0.5/muxtools/subtitle/font.py
--rw-rw-rw-   0        0        0     3423 2023-06-01 16:53:30.000000 muxtools-0.0.5/muxtools/subtitle/styles.py
--rw-rw-rw-   0        0        0    20827 2023-06-04 13:49:24.000000 muxtools-0.0.5/muxtools/subtitle/sub.py
--rw-rw-rw-   0        0        0     1649 2023-06-01 16:53:30.000000 muxtools-0.0.5/muxtools/subtitle/subutils.py
-drwxrwxrwx   0        0        0        0 2023-06-05 18:42:28.637931 muxtools-0.0.5/muxtools/utils/
--rw-rw-rw-   0        0        0      242 2023-05-31 22:50:01.000000 muxtools-0.0.5/muxtools/utils/__init__.py
--rw-rw-rw-   0        0        0     3242 2023-05-31 22:50:01.000000 muxtools-0.0.5/muxtools/utils/convert.py
--rw-rw-rw-   0        0        0     4270 2023-06-03 00:34:39.000000 muxtools-0.0.5/muxtools/utils/download.py
--rw-rw-rw-   0        0        0     1468 2023-06-04 13:18:33.000000 muxtools-0.0.5/muxtools/utils/env.py
--rw-rw-rw-   0        0        0     5357 2023-05-31 22:50:01.000000 muxtools-0.0.5/muxtools/utils/files.py
--rw-rw-rw-   0        0        0     2426 2023-05-31 22:50:01.000000 muxtools-0.0.5/muxtools/utils/format.py
--rw-rw-rw-   0        0        0     1248 2023-05-31 22:50:01.000000 muxtools-0.0.5/muxtools/utils/glob.py
--rw-rw-rw-   0        0        0     1708 2023-06-01 16:53:30.000000 muxtools-0.0.5/muxtools/utils/log.py
--rw-rw-rw-   0        0        0     8153 2023-06-04 11:20:52.000000 muxtools-0.0.5/muxtools/utils/parsing.py
--rw-rw-rw-   0        0        0     3382 2023-06-02 23:57:08.000000 muxtools-0.0.5/muxtools/utils/types.py
-drwxrwxrwx   0        0        0        0 2023-06-05 18:42:28.619063 muxtools-0.0.5/muxtools.egg-info/
--rw-rw-rw-   0        0        0     1115 2023-06-05 18:42:28.000000 muxtools-0.0.5/muxtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1054 2023-06-05 18:42:28.000000 muxtools-0.0.5/muxtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 18:42:28.000000 muxtools-0.0.5/muxtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-06-05 18:42:28.000000 muxtools-0.0.5/muxtools.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      126 2023-06-05 18:42:28.000000 muxtools-0.0.5/muxtools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-05 18:42:28.000000 muxtools-0.0.5/muxtools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1335 2023-06-05 18:41:01.000000 muxtools-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-05 18:42:28.639931 muxtools-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-09 15:26:25.454151 muxtools-0.0.6/
+-rw-rw-rw-   0        0        0    17098 2023-05-19 19:09:14.000000 muxtools-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     1619 2023-06-09 15:26:25.453150 muxtools-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      616 2023-06-08 16:58:55.000000 muxtools-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-09 15:26:25.418472 muxtools-0.0.6/muxtools/
+-rw-rw-rw-   0        0        0      810 2023-05-31 22:50:01.000000 muxtools-0.0.6/muxtools/__init__.py
+-rw-rw-rw-   0        0        0       72 2023-05-31 22:50:01.000000 muxtools-0.0.6/muxtools/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 15:26:25.436677 muxtools-0.0.6/muxtools/audio/
+-rw-rw-rw-   0        0        0      190 2023-06-01 17:13:19.000000 muxtools-0.0.6/muxtools/audio/__init__.py
+-rw-rw-rw-   0        0        0    10057 2023-06-08 16:32:38.000000 muxtools-0.0.6/muxtools/audio/audioutils.py
+-rw-rw-rw-   0        0        0    14850 2023-06-05 21:23:22.000000 muxtools-0.0.6/muxtools/audio/encoders.py
+-rw-rw-rw-   0        0        0    16812 2023-06-03 00:49:40.000000 muxtools-0.0.6/muxtools/audio/extractors.py
+-rw-rw-rw-   0        0        0     9133 2023-06-03 01:36:04.000000 muxtools-0.0.6/muxtools/audio/memecoders.py
+-rw-rw-rw-   0        0        0      962 2023-06-01 11:53:30.000000 muxtools-0.0.6/muxtools/audio/tools.py
+-rw-rw-rw-   0        0        0     7680 2023-06-09 13:58:58.000000 muxtools-0.0.6/muxtools/cli.py
+-rw-rw-rw-   0        0        0     3282 2023-06-02 21:32:44.000000 muxtools-0.0.6/muxtools/functions.py
+-rw-rw-rw-   0        0        0     4589 2023-05-31 22:50:01.000000 muxtools-0.0.6/muxtools/main.py
+drwxrwxrwx   0        0        0        0 2023-06-09 15:26:25.437677 muxtools-0.0.6/muxtools/misc/
+-rw-rw-rw-   0        0        0       51 2023-06-01 16:53:33.000000 muxtools-0.0.6/muxtools/misc/__init__.py
+-rw-rw-rw-   0        0        0     7596 2023-06-04 11:54:07.000000 muxtools-0.0.6/muxtools/misc/chapters.py
+drwxrwxrwx   0        0        0        0 2023-06-09 15:26:25.441181 muxtools-0.0.6/muxtools/muxing/
+-rw-rw-rw-   0        0        0      129 2023-05-31 22:50:01.000000 muxtools-0.0.6/muxtools/muxing/__init__.py
+-rw-rw-rw-   0        0        0     4816 2023-06-06 22:31:04.000000 muxtools-0.0.6/muxtools/muxing/mux.py
+-rw-rw-rw-   0        0        0     4452 2023-06-05 21:11:08.000000 muxtools-0.0.6/muxtools/muxing/muxfiles.py
+-rw-rw-rw-   0        0        0     6371 2023-05-31 22:50:01.000000 muxtools-0.0.6/muxtools/muxing/tmdb.py
+-rw-rw-rw-   0        0        0     7136 2023-06-09 14:58:00.000000 muxtools-0.0.6/muxtools/muxing/tracks.py
+drwxrwxrwx   0        0        0        0 2023-06-09 15:26:25.444638 muxtools-0.0.6/muxtools/subtitle/
+-rw-rw-rw-   0        0        0      128 2023-05-31 22:50:01.000000 muxtools-0.0.6/muxtools/subtitle/__init__.py
+-rw-rw-rw-   0        0        0     2578 2023-06-07 23:13:50.000000 muxtools-0.0.6/muxtools/subtitle/font.py
+-rw-rw-rw-   0        0        0     3423 2023-06-01 16:53:30.000000 muxtools-0.0.6/muxtools/subtitle/styles.py
+-rw-rw-rw-   0        0        0    20827 2023-06-04 13:49:24.000000 muxtools-0.0.6/muxtools/subtitle/sub.py
+-rw-rw-rw-   0        0        0     1649 2023-06-01 16:53:30.000000 muxtools-0.0.6/muxtools/subtitle/subutils.py
+drwxrwxrwx   0        0        0        0 2023-06-09 15:26:25.453150 muxtools-0.0.6/muxtools/utils/
+-rw-rw-rw-   0        0        0      242 2023-05-31 22:50:01.000000 muxtools-0.0.6/muxtools/utils/__init__.py
+-rw-rw-rw-   0        0        0     3242 2023-05-31 22:50:01.000000 muxtools-0.0.6/muxtools/utils/convert.py
+-rw-rw-rw-   0        0        0     4270 2023-06-03 00:34:39.000000 muxtools-0.0.6/muxtools/utils/download.py
+-rw-rw-rw-   0        0        0     1468 2023-06-04 13:18:33.000000 muxtools-0.0.6/muxtools/utils/env.py
+-rw-rw-rw-   0        0        0     5383 2023-06-05 20:41:17.000000 muxtools-0.0.6/muxtools/utils/files.py
+-rw-rw-rw-   0        0        0     2426 2023-05-31 22:50:01.000000 muxtools-0.0.6/muxtools/utils/format.py
+-rw-rw-rw-   0        0        0     1248 2023-05-31 22:50:01.000000 muxtools-0.0.6/muxtools/utils/glob.py
+-rw-rw-rw-   0        0        0     1708 2023-06-01 16:53:30.000000 muxtools-0.0.6/muxtools/utils/log.py
+-rw-rw-rw-   0        0        0     8153 2023-06-04 11:20:52.000000 muxtools-0.0.6/muxtools/utils/parsing.py
+-rw-rw-rw-   0        0        0     3382 2023-06-02 23:57:08.000000 muxtools-0.0.6/muxtools/utils/types.py
+drwxrwxrwx   0        0        0        0 2023-06-09 15:26:25.431549 muxtools-0.0.6/muxtools.egg-info/
+-rw-rw-rw-   0        0        0     1619 2023-06-09 15:26:25.000000 muxtools-0.0.6/muxtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1054 2023-06-09 15:26:25.000000 muxtools-0.0.6/muxtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 15:26:25.000000 muxtools-0.0.6/muxtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-06-09 15:26:25.000000 muxtools-0.0.6/muxtools.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      126 2023-06-09 15:26:25.000000 muxtools-0.0.6/muxtools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-09 15:26:25.000000 muxtools-0.0.6/muxtools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1335 2023-06-09 15:25:29.000000 muxtools-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-09 15:26:25.454151 muxtools-0.0.6/setup.cfg
```

### Comparing `muxtools-0.0.5/LICENSE` & `muxtools-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.5/PKG-INFO` & `muxtools-0.0.6/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muxtools
-Version: 0.0.5
+Version: 0.0.6
 Summary: A library for various muxing and automation tools for anything and everything fansubbing related
 Author-email: Vodes <vodes.imp@gmail.com>
 License: MPL 2.0
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/muxtools
 Project-URL: Contact, https://discord.gg/qxTxVJGtst
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
@@ -20,7 +20,19 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # muxtools
 
 A library for various muxing and automation tools for anything and everything fansubbing related
+
+## How do I use this?
+
+You might wanna check out the [wiki](https://github.com/Irrational-Encoding-Wizardry/vs-muxtools/wiki) in the [vs-muxtools](https://github.com/Irrational-Encoding-Wizardry/vs-muxtools) repo.
+
+## Installation
+
+Git is always the most updated one obviously but I can't guarantee that everything is in a working state.
+
+You can also grab the latest stable ish versions from pip.
+
+[![PyPI version](https://badge.fury.io/py/muxtools.svg)](https://badge.fury.io/py/muxtools)
```

### Comparing `muxtools-0.0.5/muxtools/__init__.py` & `muxtools-0.0.6/muxtools/__init__.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.5/muxtools/audio/audioutils.py` & `muxtools-0.0.6/muxtools/audio/audioutils.py`

 * *Files 6% similar despite different names*

```diff
@@ -83,47 +83,14 @@
 
     if valid_type == ValidInputType.FLAC:
         return get_flac(input)
     else:
         return get_pcm(input)
 
 
-def compare_trims(trim: Trim, trim2: Trim):
-    if trim[0] is None and trim2[0] is not None:
-        return -1
-    elif trim[0] is not None and trim2[0] is None:
-        return 1
-    else:
-        if trim[0] is None and trim2[0] is None:
-            return trim[1] - trim2[1]
-        else:
-            return trim[0] - trim2[0]
-
-
-def clean_trims(trims: list[Trim]):
-    sorted_trims = sorted(trims, key=cmp_to_key(compare_trims))
-
-    final_trims = []
-    for start, end in sorted_trims:
-        if final_trims:
-            prev_start, prev_end = final_trims[-1]
-            if start is None and prev_end is not None:
-                continue
-            elif prev_end is not None and prev_end >= start:
-                final_trims[-1] = (prev_start, max(prev_end, end))
-            elif prev_end is None and end is None:
-                continue
-            else:
-                final_trims.append((start, end))
-        elif start is not None or end is not None:
-            final_trims.append((start, end))
-
-    return final_trims
-
-
 def sanitize_trims(
     trims: Trim | list[Trim], total_frames: int = 0, uses_frames: bool = True, allow_negative_start: bool = False, caller: any = None
 ) -> list[Trim]:
     caller = caller if caller else sanitize_trims
     if not isinstance(trims, (list, tuple)):
         raise error("Trims must be a list of 2-tuples (or just one 2-tuple)", caller)
     if not isinstance(trims, list):
@@ -135,30 +102,34 @@
             raise error(f"The trim {trim} needs 2 elements", caller)
         for i in trim:
             if not isinstance(i, (int, type(None))):
                 raise error(f"The trim {trim} must have 2 ints or None's", caller)
         if trim[-1] == 0:
             raise error("Slices cannot end with 0, if attempting to use an empty slice, use `None`", caller)
 
-        if trim[0] and trim[0] < 0 and not allow_negative_start:
+        if trim[0] and trim[0] < 0 and not allow_negative_start and index == 0:
             raise error("The first part of a trim cannot be negative.", caller)
 
-        if trim[1] and uses_frames:
-            if total_frames and trim[1] > total_frames:
-                warn(f"The trim {trim} extends the frame number that was passed. Will be set to max frame.", caller, 5)
-                trims[index] = (trim[0], total_frames - 1)
-            if trim[1] < 0:
-                if not total_frames:
-                    raise error("A trim cannot be negative if you're not passing the total frame number.", caller)
-                new_val = total_frames + trim[1]
-                trims[index] = (trim[0], new_val)
-                if new_val < 0:
-                    raise error(f"The negative number of the trim {trim} is out of bounds.", caller)
+        has_negative = (trim[1] is not None and trim[1] < 0) or (trim[0] is not None and trim[0] < 0)
+        if not uses_frames and has_negative:
+            raise error(f"If you use milliseconds to trim you cannot use negative values.")
+
+        if not total_frames and has_negative:
+            raise error(f"If you want to use negative trims you gotta pass a total frame number.")
+
+        if trim[1] is not None and trim[1] < 0:
+            trim = (trim[0], total_frames + trim[1])
+            trims[index] = trim
+
+        if trim[0] is not None and trim[0] < 0:
+            if allow_negative_start and index == 0:
+                continue
+            trims[index] = (total_frames + trim[0], trim[1])
 
-    return clean_trims(trims)
+    return trims
 
 
 # Of course these are not all of the formats possible but those are the most common from what I know.
 # fmt: off
 formats = [
     # Lossy
     AudioFormat("AC-3",         "ac3",      "A_AC3"),
```

### Comparing `muxtools-0.0.5/muxtools/audio/encoders.py` & `muxtools-0.0.6/muxtools/audio/encoders.py`

 * *Files 0% similar despite different names*

```diff
@@ -197,15 +197,15 @@
                     self.bitrate = 320
             debug(f"Encoding '{input.file.stem}' to Opus ({self.bitrate} kbps) using opusenc...", self)
         else:
             debug(f"Encoding '{input.file.stem}' to Opus using opusenc...", self)
 
         output = make_output(input.file, "opus", "opusenc", self.output)
         source = ensure_valid_in(
-            input, dither=self.dither, dither_type=self.dither_type, caller=self, valid_type=ValidInputType.AIFF_OR_FLAC, supports_pipe=True
+            input, dither=self.dither, dither_type=self.dither_type, caller=self, valid_type=ValidInputType.FLAC, supports_pipe=True
         )
 
         args = [exe, "--vbr" if self.vbr else "--cvbr", "--bitrate", str(self.bitrate)]
         if self.append:
             args.extend(splitcommand(self.append))
         args.append(str(source.file.resolve()) if isinstance(source, AudioFile) else "-")
         args.append(str(output))
```

### Comparing `muxtools-0.0.5/muxtools/audio/extractors.py` & `muxtools-0.0.6/muxtools/audio/extractors.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.5/muxtools/audio/memecoders.py` & `muxtools-0.0.6/muxtools/audio/memecoders.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.5/muxtools/audio/tools.py` & `muxtools-0.0.6/muxtools/audio/tools.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.5/muxtools/cli.py` & `muxtools-0.0.6/muxtools/cli.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.5/muxtools/functions.py` & `muxtools-0.0.6/muxtools/functions.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.5/muxtools/main.py` & `muxtools-0.0.6/muxtools/main.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.5/muxtools/misc/chapters.py` & `muxtools-0.0.6/muxtools/misc/chapters.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.5/muxtools/muxing/mux.py` & `muxtools-0.0.6/muxtools/muxing/mux.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,16 @@
     filename = re.sub(re.escape(R"$ep$"), episode, filename)
     filename = re.sub(re.escape(R"$crc32$"), "#crc32#", filename)
 
     mkvtitle = re.sub(re.escape(R"$show$"), show_name, mkv_title_naming)
     mkvtitle = re.sub(re.escape(R"$ep$"), episode, mkvtitle)
 
     try:
+        if " " in episode:
+            episode = str(episode).split(" ")[0]
         epint = int(episode)
     except:
         if tmdb and not tmdb.movie:
             warn(f"{episode} is not a valid integer! TMDB will be skipped.", "Mux", 3)
             tmdb = None
     if tmdb:
         debug("Fetching tmdb metadata...", "Mux")
@@ -85,15 +87,15 @@
                 warn("It's strongly recommended to pass tracks to ensure naming and tagging instead of MuxingFiles directly!", "Mux", 1)
             track = track.to_track()
             args.extend(splitcommand(track.mkvmerge_args()))
             continue
         elif isinstance(track, Chapters):
             args.extend(["--chapters", track.to_file()])
             continue
-        elif isinstance(track, PathLike) or isinstance(track, GlobSearch):
+        elif isinstance(track, Path) or isinstance(track, str) or isinstance(track, GlobSearch):
             # Failsave for if someone passes Chapters().to_file() or a txt/xml file
             track = ensure_path_exists(track, "Mux")
             if track.suffix.lower() in [".txt", ".xml"]:
                 args.extend(["--chapters", track.resolve()])
                 continue
 
         raise error("Only _track, MuxingFiles or Chapters types are supported as muxing input!", "Mux")
```

### Comparing `muxtools-0.0.5/muxtools/muxing/muxfiles.py` & `muxtools-0.0.6/muxtools/muxing/muxfiles.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,10 +117,12 @@
         else:
             raise error("Failed to mux AudioFile to mka.", self)
 
     @staticmethod
     def from_file(pathIn: PathLike, caller: any):
         from ..utils.log import warn
 
-        warn("It's strongly recommended to explicitly extract tracks first!", caller, 1)
         file = ensure_path_exists(pathIn, caller)
+        if file.suffix.lower() != ".wav":
+            warn("It's strongly recommended to explicitly extract tracks first!", caller, 1)
+
         return AudioFile(file, 0, file)
```

### Comparing `muxtools-0.0.5/muxtools/muxing/tmdb.py` & `muxtools-0.0.6/muxtools/muxing/tmdb.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.5/muxtools/muxing/tracks.py` & `muxtools-0.0.6/muxtools/muxing/tracks.py`

 * *Files 6% similar despite different names*

```diff
@@ -137,50 +137,58 @@
         file: PathLike | GlobSearch,
         video: int | list[int] | None = -1,
         audio: int | list[int] | None = -1,
         subtitles: int | list[int] | None = -1,
         keep_attachments: bool = True,
         mkvmerge_args: str = "--no-global-tags",
     ) -> None:
-        args = mkvmerge_args
+        args = ""
         if video is None:
             args += " -D"
         elif video != -1:
             if isinstance(video, list):
+                lv = []
                 for num in video:
                     abso = get_absolute_tracknum(file, num, TrackType.VIDEO)
-                    args += f" -d {abso}"
+                    lv.append(abso)
+                args += f" -d {','.join(str(i) for i in lv)}"
             else:
                 abso = get_absolute_tracknum(file, video, TrackType.VIDEO)
                 args += f" -d {abso}"
 
         if audio is None:
             args += " -A"
         elif audio != -1:
             if isinstance(audio, list):
+                la = []
                 for num in audio:
                     abso = get_absolute_tracknum(file, num, TrackType.AUDIO)
-                    args += f" -a {abso}"
+                    la.append(abso)
+                args += f" -a {','.join(str(i) for i in la)}"
             else:
                 abso = get_absolute_tracknum(file, audio, TrackType.AUDIO)
                 args += f" -a {abso}"
 
         if subtitles is None:
             args += " -S"
         elif subtitles != -1:
             if isinstance(subtitles, list):
-                for num in audio:
+                ls = []
+                for num in subtitles:
                     abso = get_absolute_tracknum(file, num, TrackType.SUB)
-                    args += f" -s {abso}"
+                    ls.append(abso)
+                args += f" -s {','.join(str(i) for i in ls)}"
             else:
                 abso = get_absolute_tracknum(file, subtitles, TrackType.SUB)
                 args += f" -s {abso}"
 
         if not keep_attachments:
             args += " -M"
+
+        args = f" {args.strip()} {mkvmerge_args.strip()}"
         super().__init__(file, TrackType.MKV, args, "", False, False, 0)
 
 
 VT = VideoTrack
 AT = AudioTrack
 ST = SubTrack
 MkvTrack = Premux
```

### Comparing `muxtools-0.0.5/muxtools/subtitle/styles.py` & `muxtools-0.0.6/muxtools/subtitle/styles.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.5/muxtools/subtitle/sub.py` & `muxtools-0.0.6/muxtools/subtitle/sub.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.5/muxtools/subtitle/subutils.py` & `muxtools-0.0.6/muxtools/subtitle/subutils.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.5/muxtools/utils/convert.py` & `muxtools-0.0.6/muxtools/utils/convert.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.5/muxtools/utils/download.py` & `muxtools-0.0.6/muxtools/utils/download.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.5/muxtools/utils/env.py` & `muxtools-0.0.6/muxtools/utils/env.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.5/muxtools/utils/files.py` & `muxtools-0.0.6/muxtools/utils/files.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 __all__ = [
     "ensure_path",
     "uniquify_path",
     "get_crc32",
     "make_output",
     "ensure_path_exists",
     "clean_temp_files",
+    "get_absolute_track",
 ]
 
 
 def ensure_path(pathIn: PathLike, caller: any) -> Path:
     """
     Utility function for other functions to make sure a path was passed to them.
```

### Comparing `muxtools-0.0.5/muxtools/utils/format.py` & `muxtools-0.0.6/muxtools/utils/format.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.5/muxtools/utils/glob.py` & `muxtools-0.0.6/muxtools/utils/glob.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.5/muxtools/utils/log.py` & `muxtools-0.0.6/muxtools/utils/log.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.5/muxtools/utils/parsing.py` & `muxtools-0.0.6/muxtools/utils/parsing.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.5/muxtools/utils/types.py` & `muxtools-0.0.6/muxtools/utils/types.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.5/muxtools.egg-info/PKG-INFO` & `muxtools-0.0.6/muxtools.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muxtools
-Version: 0.0.5
+Version: 0.0.6
 Summary: A library for various muxing and automation tools for anything and everything fansubbing related
 Author-email: Vodes <vodes.imp@gmail.com>
 License: MPL 2.0
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/muxtools
 Project-URL: Contact, https://discord.gg/qxTxVJGtst
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
@@ -20,7 +20,19 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # muxtools
 
 A library for various muxing and automation tools for anything and everything fansubbing related
+
+## How do I use this?
+
+You might wanna check out the [wiki](https://github.com/Irrational-Encoding-Wizardry/vs-muxtools/wiki) in the [vs-muxtools](https://github.com/Irrational-Encoding-Wizardry/vs-muxtools) repo.
+
+## Installation
+
+Git is always the most updated one obviously but I can't guarantee that everything is in a working state.
+
+You can also grab the latest stable ish versions from pip.
+
+[![PyPI version](https://badge.fury.io/py/muxtools.svg)](https://badge.fury.io/py/muxtools)
```

### Comparing `muxtools-0.0.5/muxtools.egg-info/SOURCES.txt` & `muxtools-0.0.6/muxtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.5/pyproject.toml` & `muxtools-0.0.6/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [project]
 name = "muxtools"
-version = "0.0.5"
+version = "0.0.6"
 description = "A library for various muxing and automation tools for anything and everything fansubbing related"
 authors = [
     { name="Vodes", email="vodes.imp@gmail.com" }
 ]
 dependencies = [
     "requests>=2.31.0",
     "fontcollector>=2.1.0",
```

