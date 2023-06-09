# Comparing `tmp/whisper_autosrt-0.1.1.tar.gz` & `tmp/whisper_autosrt-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whisper_autosrt-0.1.1.tar", last modified: Sun Jun  4 14:03:41 2023, max compression
+gzip compressed data, was "whisper_autosrt-0.1.2.tar", last modified: Fri Jun  9 01:38:23 2023, max compression
```

## Comparing `whisper_autosrt-0.1.1.tar` & `whisper_autosrt-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 14:03:40.998343 whisper_autosrt-0.1.1/
--rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 whisper_autosrt-0.1.1/LICENSE
--rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 whisper_autosrt-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1956 2023-06-04 14:03:40.999093 whisper_autosrt-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     4700 2023-05-27 16:57:41.000000 whisper_autosrt-0.1.1/README.md
--rw-rw-rw-   0        0        0      147 2023-06-04 14:03:41.001340 whisper_autosrt-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1642 2023-06-02 17:36:46.000000 whisper_autosrt-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-04 14:03:40.960876 whisper_autosrt-0.1.1/whisper_autosrt/
--rw-rw-rw-   0        0        0    82619 2023-06-04 12:34:43.000000 whisper_autosrt-0.1.1/whisper_autosrt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-04 14:03:40.996844 whisper_autosrt-0.1.1/whisper_autosrt.egg-info/
--rw-rw-rw-   0        0        0     1956 2023-06-04 14:03:40.000000 whisper_autosrt-0.1.1/whisper_autosrt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2023-06-04 14:03:40.000000 whisper_autosrt-0.1.1/whisper_autosrt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 14:03:40.000000 whisper_autosrt-0.1.1/whisper_autosrt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-06-04 14:03:40.000000 whisper_autosrt-0.1.1/whisper_autosrt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      119 2023-06-04 14:03:40.000000 whisper_autosrt-0.1.1/whisper_autosrt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-04 14:03:40.000000 whisper_autosrt-0.1.1/whisper_autosrt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 01:38:23.281040 whisper_autosrt-0.1.2/
+-rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 whisper_autosrt-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 whisper_autosrt-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1956 2023-06-09 01:38:23.281789 whisper_autosrt-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4700 2023-05-27 16:57:41.000000 whisper_autosrt-0.1.2/README.md
+-rw-rw-rw-   0        0        0      147 2023-06-09 01:38:23.284787 whisper_autosrt-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1642 2023-06-02 17:36:46.000000 whisper_autosrt-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 01:38:23.251074 whisper_autosrt-0.1.2/whisper_autosrt/
+-rw-rw-rw-   0        0        0   136062 2023-06-09 01:37:23.000000 whisper_autosrt-0.1.2/whisper_autosrt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 01:38:23.279541 whisper_autosrt-0.1.2/whisper_autosrt.egg-info/
+-rw-rw-rw-   0        0        0     1956 2023-06-09 01:38:23.000000 whisper_autosrt-0.1.2/whisper_autosrt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2023-06-09 01:38:23.000000 whisper_autosrt-0.1.2/whisper_autosrt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 01:38:23.000000 whisper_autosrt-0.1.2/whisper_autosrt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-06-09 01:38:23.000000 whisper_autosrt-0.1.2/whisper_autosrt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      119 2023-06-09 01:38:23.000000 whisper_autosrt-0.1.2/whisper_autosrt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-09 01:38:23.000000 whisper_autosrt-0.1.2/whisper_autosrt.egg-info/top_level.txt
```

### Comparing `whisper_autosrt-0.1.1/LICENSE` & `whisper_autosrt-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `whisper_autosrt-0.1.1/PKG-INFO` & `whisper_autosrt-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whisper_autosrt
-Version: 0.1.1
+Version: 0.1.2
 Summary: a command line utility for automatic speech recognition and subtitle generation
 Home-page: https://github.com/botbahlul/whisper_autosrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

### Comparing `whisper_autosrt-0.1.1/README.md` & `whisper_autosrt-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `whisper_autosrt-0.1.1/setup.py` & `whisper_autosrt-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `whisper_autosrt-0.1.1/whisper_autosrt.egg-info/PKG-INFO` & `whisper_autosrt-0.1.2/whisper_autosrt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whisper-autosrt
-Version: 0.1.1
+Version: 0.1.2
 Summary: a command line utility for automatic speech recognition and subtitle generation
 Home-page: https://github.com/botbahlul/whisper_autosrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

