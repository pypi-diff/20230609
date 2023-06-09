# Comparing `tmp/ovos-microphone-plugin-files-0.0.0a1.tar.gz` & `tmp/ovos-microphone-plugin-files-0.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-microphone-plugin-files-0.0.0a1.tar", last modified: Fri Jun  9 21:54:18 2023, max compression
+gzip compressed data, was "ovos-microphone-plugin-files-0.0.0a2.tar", last modified: Fri Jun  9 21:57:26 2023, max compression
```

## Comparing `ovos-microphone-plugin-files-0.0.0a1.tar` & `ovos-microphone-plugin-files-0.0.0a2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 21:54:18.179891 ovos-microphone-plugin-files-0.0.0a1/
--rw-r--r--   0 runner    (1001) docker     (123)    11431 2023-06-09 21:54:10.000000 ovos-microphone-plugin-files-0.0.0a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-09 21:54:10.000000 ovos-microphone-plugin-files-0.0.0a1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-09 21:54:18.179891 ovos-microphone-plugin-files-0.0.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-09 21:54:10.000000 ovos-microphone-plugin-files-0.0.0a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 21:54:18.175891 ovos-microphone-plugin-files-0.0.0a1/ovos_microphone_plugin_files/
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-06-09 21:54:10.000000 ovos-microphone-plugin-files-0.0.0a1/ovos_microphone_plugin_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-09 21:54:13.000000 ovos-microphone-plugin-files-0.0.0a1/ovos_microphone_plugin_files/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 21:54:18.179891 ovos-microphone-plugin-files-0.0.0a1/ovos_microphone_plugin_files.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-09 21:54:17.000000 ovos-microphone-plugin-files-0.0.0a1/ovos_microphone_plugin_files.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-09 21:54:18.000000 ovos-microphone-plugin-files-0.0.0a1/ovos_microphone_plugin_files.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 21:54:17.000000 ovos-microphone-plugin-files-0.0.0a1/ovos_microphone_plugin_files.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-09 21:54:17.000000 ovos-microphone-plugin-files-0.0.0a1/ovos_microphone_plugin_files.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-09 21:54:17.000000 ovos-microphone-plugin-files-0.0.0a1/ovos_microphone_plugin_files.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-09 21:54:17.000000 ovos-microphone-plugin-files-0.0.0a1/ovos_microphone_plugin_files.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 21:54:17.000000 ovos-microphone-plugin-files-0.0.0a1/ovos_microphone_plugin_files.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 21:54:18.179891 ovos-microphone-plugin-files-0.0.0a1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3130 2023-06-09 21:54:10.000000 ovos-microphone-plugin-files-0.0.0a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 21:57:26.333835 ovos-microphone-plugin-files-0.0.0a2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11431 2023-06-09 21:57:18.000000 ovos-microphone-plugin-files-0.0.0a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-09 21:57:18.000000 ovos-microphone-plugin-files-0.0.0a2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-09 21:57:26.333835 ovos-microphone-plugin-files-0.0.0a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-09 21:57:18.000000 ovos-microphone-plugin-files-0.0.0a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 21:57:26.333835 ovos-microphone-plugin-files-0.0.0a2/ovos_microphone_plugin_files/
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-06-09 21:57:18.000000 ovos-microphone-plugin-files-0.0.0a2/ovos_microphone_plugin_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-09 21:57:21.000000 ovos-microphone-plugin-files-0.0.0a2/ovos_microphone_plugin_files/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 21:57:26.333835 ovos-microphone-plugin-files-0.0.0a2/ovos_microphone_plugin_files.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-09 21:57:25.000000 ovos-microphone-plugin-files-0.0.0a2/ovos_microphone_plugin_files.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-09 21:57:26.000000 ovos-microphone-plugin-files-0.0.0a2/ovos_microphone_plugin_files.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 21:57:25.000000 ovos-microphone-plugin-files-0.0.0a2/ovos_microphone_plugin_files.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-09 21:57:25.000000 ovos-microphone-plugin-files-0.0.0a2/ovos_microphone_plugin_files.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-09 21:57:25.000000 ovos-microphone-plugin-files-0.0.0a2/ovos_microphone_plugin_files.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-09 21:57:25.000000 ovos-microphone-plugin-files-0.0.0a2/ovos_microphone_plugin_files.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 21:57:25.000000 ovos-microphone-plugin-files-0.0.0a2/ovos_microphone_plugin_files.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 21:57:26.333835 ovos-microphone-plugin-files-0.0.0a2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3130 2023-06-09 21:57:18.000000 ovos-microphone-plugin-files-0.0.0a2/setup.py
```

### Comparing `ovos-microphone-plugin-files-0.0.0a1/LICENSE` & `ovos-microphone-plugin-files-0.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `ovos-microphone-plugin-files-0.0.0a1/PKG-INFO` & `ovos-microphone-plugin-files-0.0.0a2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-microphone-plugin-files
-Version: 0.0.0a1
+Version: 0.0.0a2
 Summary: A files microphone implementation for OVOS
 Home-page: https://github.com/OpenVoiceOS/ovos-microphone-plugin-files
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Description: UNKNOWN
 Keywords: ovos plugin listener microphone files
```

### Comparing `ovos-microphone-plugin-files-0.0.0a1/ovos_microphone_plugin_files/__init__.py` & `ovos-microphone-plugin-files-0.0.0a2/ovos_microphone_plugin_files/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from dataclasses import dataclass, field
 from queue import Queue
 from typing import Optional
 from os.path import expanduser
 import speech_recognition as sr
 from ovos_plugin_manager.templates.microphone import Microphone
 from ovos_utils.file_utils import FileWatcher
+from ovos_utils.log import LOG
 
 
 @dataclass
 class FilesMicrophone(Microphone):
     files_folder: str = expanduser("~/file_microphone")
     current_file: str = ""
     autodelete: bool = True
@@ -42,23 +43,25 @@
         with sr.AudioFile(wave_file_path) as source:
             audio = r.record(source)
         return audio
 
     def on_new_file(self, path):
         self.current_file = path
 
-        audio = self.read_wave_file(path)
-        full_chunk = audio.frame_data
-        while len(full_chunk) >= self.chunk_size:
-            self._queue.put_nowait(full_chunk[: self.chunk_size])
-            full_chunk = full_chunk[self.chunk_size:]
-
+        try:
+            audio = self.read_wave_file(path)
+            full_chunk = audio.frame_data
+            while len(full_chunk) >= self.chunk_size:
+                self._queue.put_nowait(full_chunk[: self.chunk_size])
+                full_chunk = full_chunk[self.chunk_size:]
+            if self.autodelete:
+                os.remove(path)
+        except:
+            LOG.exception(f"failed to process file: {path}")
         self.current_file = ""
-        if self.autodelete:
-            os.remove(path)
 
     def start(self):
         assert self._watcher is None, "Already started"
         self._watcher = FileWatcher(self.files_folder,
                                     callback=self.on_new_file)
         self._is_running = True
```

### Comparing `ovos-microphone-plugin-files-0.0.0a1/ovos_microphone_plugin_files.egg-info/PKG-INFO` & `ovos-microphone-plugin-files-0.0.0a2/ovos_microphone_plugin_files.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-microphone-plugin-files
-Version: 0.0.0a1
+Version: 0.0.0a2
 Summary: A files microphone implementation for OVOS
 Home-page: https://github.com/OpenVoiceOS/ovos-microphone-plugin-files
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Description: UNKNOWN
 Keywords: ovos plugin listener microphone files
```

### Comparing `ovos-microphone-plugin-files-0.0.0a1/setup.py` & `ovos-microphone-plugin-files-0.0.0a2/setup.py`

 * *Files identical despite different names*

