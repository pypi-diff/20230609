# Comparing `tmp/vsmuxtools-0.0.5.tar.gz` & `tmp/vsmuxtools-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vsmuxtools-0.0.5.tar", last modified: Mon Jun  5 19:50:46 2023, max compression
+gzip compressed data, was "vsmuxtools-0.0.6.tar", last modified: Fri Jun  9 15:27:01 2023, max compression
```

## Comparing `vsmuxtools-0.0.5.tar` & `vsmuxtools-0.0.6.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 19:50:46.089028 vsmuxtools-0.0.5/
--rw-rw-rw-   0        0        0    17098 2023-05-27 19:14:49.000000 vsmuxtools-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      994 2023-06-05 19:50:46.089028 vsmuxtools-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       78 2023-05-27 19:14:49.000000 vsmuxtools-0.0.5/README.md
--rw-rw-rw-   0        0        0     1078 2023-06-05 18:41:57.000000 vsmuxtools-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-05 19:50:46.089028 vsmuxtools-0.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-05 19:50:46.069854 vsmuxtools-0.0.5/vsmuxtools/
--rw-rw-rw-   0        0        0      266 2023-06-04 11:09:34.000000 vsmuxtools-0.0.5/vsmuxtools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 19:50:46.083755 vsmuxtools-0.0.5/vsmuxtools/extension/
--rw-rw-rw-   0        0        0       80 2023-05-30 18:54:48.000000 vsmuxtools-0.0.5/vsmuxtools/extension/__init__.py
--rw-rw-rw-   0        0        0     2717 2023-05-31 21:39:04.000000 vsmuxtools-0.0.5/vsmuxtools/extension/audio.py
--rw-rw-rw-   0        0        0     1477 2023-06-04 11:42:52.000000 vsmuxtools-0.0.5/vsmuxtools/extension/chapters.py
-drwxrwxrwx   0        0        0        0 2023-06-05 19:50:46.085755 vsmuxtools-0.0.5/vsmuxtools/utils/
--rw-rw-rw-   0        0        0       84 2023-05-30 16:15:03.000000 vsmuxtools-0.0.5/vsmuxtools/utils/__init__.py
--rw-rw-rw-   0        0        0     7943 2023-06-04 12:11:30.000000 vsmuxtools-0.0.5/vsmuxtools/utils/src.py
--rw-rw-rw-   0        0        0      186 2023-05-30 16:15:19.000000 vsmuxtools-0.0.5/vsmuxtools/utils/types.py
-drwxrwxrwx   0        0        0        0 2023-06-05 19:50:46.088028 vsmuxtools-0.0.5/vsmuxtools/video/
--rw-rw-rw-   0        0        0       97 2023-05-30 16:12:00.000000 vsmuxtools-0.0.5/vsmuxtools/video/__init__.py
--rw-rw-rw-   0        0        0    14785 2023-05-31 22:17:09.000000 vsmuxtools-0.0.5/vsmuxtools/video/encoders.py
--rw-rw-rw-   0        0        0     3075 2023-05-31 08:35:11.000000 vsmuxtools-0.0.5/vsmuxtools/video/resumable.py
--rw-rw-rw-   0        0        0    10096 2023-06-05 18:38:29.000000 vsmuxtools-0.0.5/vsmuxtools/video/settings.py
-drwxrwxrwx   0        0        0        0 2023-06-05 19:50:46.081754 vsmuxtools-0.0.5/vsmuxtools.egg-info/
--rw-rw-rw-   0        0        0      994 2023-06-05 19:50:46.000000 vsmuxtools-0.0.5/vsmuxtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      516 2023-06-05 19:50:46.000000 vsmuxtools-0.0.5/vsmuxtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 19:50:46.000000 vsmuxtools-0.0.5/vsmuxtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-06-05 19:50:46.000000 vsmuxtools-0.0.5/vsmuxtools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-05 19:50:46.000000 vsmuxtools-0.0.5/vsmuxtools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 15:27:01.312384 vsmuxtools-0.0.6/
+-rw-rw-rw-   0        0        0    17098 2023-05-27 19:14:49.000000 vsmuxtools-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     1417 2023-06-09 15:27:01.312384 vsmuxtools-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      501 2023-06-08 16:59:28.000000 vsmuxtools-0.0.6/README.md
+-rw-rw-rw-   0        0        0     1100 2023-06-09 15:25:44.000000 vsmuxtools-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-09 15:27:01.312384 vsmuxtools-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-09 15:27:01.292511 vsmuxtools-0.0.6/vsmuxtools/
+-rw-rw-rw-   0        0        0      266 2023-06-04 11:09:34.000000 vsmuxtools-0.0.6/vsmuxtools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 15:27:01.306646 vsmuxtools-0.0.6/vsmuxtools/extension/
+-rw-rw-rw-   0        0        0       80 2023-05-30 18:54:48.000000 vsmuxtools-0.0.6/vsmuxtools/extension/__init__.py
+-rw-rw-rw-   0        0        0     3910 2023-06-05 21:05:59.000000 vsmuxtools-0.0.6/vsmuxtools/extension/audio.py
+-rw-rw-rw-   0        0        0     1477 2023-06-04 11:42:52.000000 vsmuxtools-0.0.6/vsmuxtools/extension/chapters.py
+drwxrwxrwx   0        0        0        0 2023-06-09 15:27:01.308646 vsmuxtools-0.0.6/vsmuxtools/utils/
+-rw-rw-rw-   0        0        0      127 2023-06-05 20:25:49.000000 vsmuxtools-0.0.6/vsmuxtools/utils/__init__.py
+-rw-rw-rw-   0        0        0     5909 2023-06-05 20:52:26.000000 vsmuxtools-0.0.6/vsmuxtools/utils/audio.py
+-rw-rw-rw-   0        0        0     8125 2023-06-05 20:47:48.000000 vsmuxtools-0.0.6/vsmuxtools/utils/src.py
+-rw-rw-rw-   0        0        0      186 2023-05-30 16:15:19.000000 vsmuxtools-0.0.6/vsmuxtools/utils/types.py
+drwxrwxrwx   0        0        0        0 2023-06-09 15:27:01.311159 vsmuxtools-0.0.6/vsmuxtools/video/
+-rw-rw-rw-   0        0        0       97 2023-05-30 16:12:00.000000 vsmuxtools-0.0.6/vsmuxtools/video/__init__.py
+-rw-rw-rw-   0        0        0    14785 2023-05-31 22:17:09.000000 vsmuxtools-0.0.6/vsmuxtools/video/encoders.py
+-rw-rw-rw-   0        0        0     3075 2023-05-31 08:35:11.000000 vsmuxtools-0.0.6/vsmuxtools/video/resumable.py
+-rw-rw-rw-   0        0        0    10096 2023-06-05 18:38:29.000000 vsmuxtools-0.0.6/vsmuxtools/video/settings.py
+drwxrwxrwx   0        0        0        0 2023-06-09 15:27:01.304645 vsmuxtools-0.0.6/vsmuxtools.egg-info/
+-rw-rw-rw-   0        0        0     1417 2023-06-09 15:27:01.000000 vsmuxtools-0.0.6/vsmuxtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      542 2023-06-09 15:27:01.000000 vsmuxtools-0.0.6/vsmuxtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 15:27:01.000000 vsmuxtools-0.0.6/vsmuxtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-06-09 15:27:01.000000 vsmuxtools-0.0.6/vsmuxtools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-09 15:27:01.000000 vsmuxtools-0.0.6/vsmuxtools.egg-info/top_level.txt
```

### Comparing `vsmuxtools-0.0.5/LICENSE` & `vsmuxtools-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `vsmuxtools-0.0.5/PKG-INFO` & `vsmuxtools-0.0.6/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsmuxtools
-Version: 0.0.5
+Version: 0.0.6
 Summary: The extension to muxtools with vapoursynth and encoding stuff
 Author-email: Vodes <vodes.imp@gmail.com>
 License: MPL 2.0
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-muxtools
 Project-URL: Contact, https://discord.gg/qxTxVJGtst
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
@@ -17,8 +17,21 @@
 Classifier: Topic :: Multimedia :: Video :: Conversion
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # vs-muxtools
+
 The extension to muxtools with vapoursynth and encoding stuff
+
+## How do I use this?
+
+You might wanna check out the [wiki](https://github.com/Irrational-Encoding-Wizardry/vs-muxtools/wiki).
+
+## Installation
+
+Git is always the most updated one obviously but I can't guarantee that everything is in a working state.
+
+You can also grab the latest stable ish versions from pip.
+
+[![PyPI version](https://badge.fury.io/py/vsmuxtools.svg)](https://badge.fury.io/py/vsmuxtools)
```

### Comparing `vsmuxtools-0.0.5/pyproject.toml` & `vsmuxtools-0.0.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 
 [project]
 name = "vsmuxtools"
-version = "0.0.5"
+version = "0.0.6"
 description = "The extension to muxtools with vapoursynth and encoding stuff"
 authors = [
     { name="Vodes", email="vodes.imp@gmail.com" }
 ]
 dependencies = [
     "vapoursynth>=60",
     "vstools>=1.6.2",
-    "muxtools>=0.0.5",
+    "numpy>=1.24.3",
+    "muxtools>=0.0.6",
 ]
 classifiers = [
     "Natural Language :: English",
     "Intended Audience :: Developers",
     "Intended Audience :: End Users/Desktop",
     "Programming Language :: Python :: 3.10",
     "Operating System :: OS Independent",
```

### Comparing `vsmuxtools-0.0.5/vsmuxtools/extension/chapters.py` & `vsmuxtools-0.0.6/vsmuxtools/extension/chapters.py`

 * *Files identical despite different names*

### Comparing `vsmuxtools-0.0.5/vsmuxtools/utils/src.py` & `vsmuxtools-0.0.6/vsmuxtools/utils/src.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,25 @@
 import shutil as sh
 from pathlib import Path
 from typing import Callable
 from fractions import Fraction
 from vstools import vs, core, initialize_clip, copy_signature
-from muxtools import Trim, PathLike, parse_m2ts_path, ensure_path_exists, warn, info, get_workdir, get_temp_workdir, clean_temp_files
+from muxtools import (
+    Trim,
+    PathLike,
+    parse_m2ts_path,
+    ensure_path_exists,
+    warn,
+    info,
+    get_workdir,
+    get_temp_workdir,
+    clean_temp_files,
+    get_absolute_track,
+    TrackType,
+)
 
 
 __all__ = ["src_file", "SRC_FILE", "FileInfo", "src", "frames_to_samples", "f2s"]
 
 
 class src_file:
     file: PathLike
@@ -86,15 +98,18 @@
 
     def get_audio(self, track: int = 0, **kwargs) -> vs.AudioNode:
         """
         Indexes the specified audio track from the input file.
         """
         args = dict(exact=True)
         args.update(**kwargs)
-        return core.bs.AudioSource(str(self.file.resolve()), track, **args)
+
+        absolute = get_absolute_track(self.file, track, TrackType.AUDIO)
+
+        return core.bs.AudioSource(str(self.file.resolve()), absolute.track_id, **args)
 
     def get_audio_trimmed(self, track: int = 0, **kwargs) -> vs.AudioNode:
         """
         Gets the indexed audio track with the trim specified in the src_file.
         """
         node = self.get_audio(track, **kwargs)
         if self.trim:
```

### Comparing `vsmuxtools-0.0.5/vsmuxtools/video/encoders.py` & `vsmuxtools-0.0.6/vsmuxtools/video/encoders.py`

 * *Files identical despite different names*

### Comparing `vsmuxtools-0.0.5/vsmuxtools/video/resumable.py` & `vsmuxtools-0.0.6/vsmuxtools/video/resumable.py`

 * *Files identical despite different names*

### Comparing `vsmuxtools-0.0.5/vsmuxtools/video/settings.py` & `vsmuxtools-0.0.6/vsmuxtools/video/settings.py`

 * *Files identical despite different names*

### Comparing `vsmuxtools-0.0.5/vsmuxtools.egg-info/PKG-INFO` & `vsmuxtools-0.0.6/vsmuxtools.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsmuxtools
-Version: 0.0.5
+Version: 0.0.6
 Summary: The extension to muxtools with vapoursynth and encoding stuff
 Author-email: Vodes <vodes.imp@gmail.com>
 License: MPL 2.0
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-muxtools
 Project-URL: Contact, https://discord.gg/qxTxVJGtst
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
@@ -17,8 +17,21 @@
 Classifier: Topic :: Multimedia :: Video :: Conversion
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # vs-muxtools
+
 The extension to muxtools with vapoursynth and encoding stuff
+
+## How do I use this?
+
+You might wanna check out the [wiki](https://github.com/Irrational-Encoding-Wizardry/vs-muxtools/wiki).
+
+## Installation
+
+Git is always the most updated one obviously but I can't guarantee that everything is in a working state.
+
+You can also grab the latest stable ish versions from pip.
+
+[![PyPI version](https://badge.fury.io/py/vsmuxtools.svg)](https://badge.fury.io/py/vsmuxtools)
```

### Comparing `vsmuxtools-0.0.5/vsmuxtools.egg-info/SOURCES.txt` & `vsmuxtools-0.0.6/vsmuxtools.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -7,13 +7,14 @@
 vsmuxtools.egg-info/dependency_links.txt
 vsmuxtools.egg-info/requires.txt
 vsmuxtools.egg-info/top_level.txt
 vsmuxtools/extension/__init__.py
 vsmuxtools/extension/audio.py
 vsmuxtools/extension/chapters.py
 vsmuxtools/utils/__init__.py
+vsmuxtools/utils/audio.py
 vsmuxtools/utils/src.py
 vsmuxtools/utils/types.py
 vsmuxtools/video/__init__.py
 vsmuxtools/video/encoders.py
 vsmuxtools/video/resumable.py
 vsmuxtools/video/settings.py
```

