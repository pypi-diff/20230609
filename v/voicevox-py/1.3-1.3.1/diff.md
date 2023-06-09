# Comparing `tmp/voicevox_py-1.3.tar.gz` & `tmp/voicevox_py-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voicevox_py-1.3.tar", max compression
+gzip compressed data, was "voicevox_py-1.3.1.tar", max compression
```

## Comparing `voicevox_py-1.3.tar` & `voicevox_py-1.3.1.tar`

### file list

```diff
@@ -1,5 +1,9 @@
--rw-r--r--   0        0        0      364 2023-06-09 15:33:43.333667 voicevox_py-1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-09 15:34:25.115828 voicevox_py-1.3/README.md
--rw-r--r--   0        0        0      134 2023-04-05 23:51:35.158012 voicevox_py-1.3/voicevox/__init__.py
--rw-r--r--   0        0        0     1608 2023-04-06 03:53:05.794828 voicevox_py-1.3/voicevox/Synthesizer.py
--rw-r--r--   0        0        0      439 1970-01-01 00:00:00.000000 voicevox_py-1.3/PKG-INFO
+-rw-r--r--   0        0        0      362 2023-06-09 15:49:05.847933 voicevox_py-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-09 15:34:25.115828 voicevox_py-1.3.1/README.md
+-rw-r--r--   0        0        0       97 2023-06-09 15:41:58.756477 voicevox_py-1.3.1/src/coeiroink/__init__.py
+-rw-r--r--   0        0        0     1608 2023-04-06 03:52:46.459529 voicevox_py-1.3.1/src/coeiroink/Synthesizer.py
+-rw-r--r--   0        0        0       97 2023-06-09 15:41:53.725853 voicevox_py-1.3.1/src/sharevox/__init__.py
+-rw-r--r--   0        0        0     1608 2023-04-06 04:56:43.817186 voicevox_py-1.3.1/src/sharevox/Synthesizer.py
+-rw-r--r--   0        0        0       97 2023-06-09 15:41:37.676793 voicevox_py-1.3.1/src/voicevox/__init__.py
+-rw-r--r--   0        0        0     1608 2023-04-06 03:53:05.794828 voicevox_py-1.3.1/src/voicevox/Synthesizer.py
+-rw-r--r--   0        0        0      441 1970-01-01 00:00:00.000000 voicevox_py-1.3.1/PKG-INFO
```

### Comparing `voicevox_py-1.3/voicevox/Synthesizer.py` & `voicevox_py-1.3.1/src/voicevox/Synthesizer.py`

 * *Files identical despite different names*

