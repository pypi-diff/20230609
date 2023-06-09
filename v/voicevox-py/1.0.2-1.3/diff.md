# Comparing `tmp/voicevox.py-1.0.2.tar.gz` & `tmp/voicevox_py-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voicevox.py-1.0.2.tar", last modified: Thu Aug 25 08:26:04 2022, max compression
+gzip compressed data, was "voicevox_py-1.3.tar", max compression
```

## Comparing `voicevox.py-1.0.2.tar` & `voicevox_py-1.3.tar`

### file list

```diff
@@ -1,16 +1,5 @@
-drwxrwxrwx   0        0        0        0 2022-08-25 08:26:04.963681 voicevox.py-1.0.2/
--rw-rw-rw-   0        0        0     1084 2022-08-25 08:13:51.000000 voicevox.py-1.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0     1094 2022-08-25 08:26:04.962684 voicevox.py-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1268 2022-08-25 08:08:21.000000 voicevox.py-1.0.2/README.md
--rw-rw-rw-   0        0        0       42 2022-08-25 08:26:04.963681 voicevox.py-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1824 2022-08-25 08:26:01.000000 voicevox.py-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2022-08-25 08:26:04.953780 voicevox.py-1.0.2/voicevox/
--rw-rw-rw-   0        0        0       66 2022-08-25 06:00:03.000000 voicevox.py-1.0.2/voicevox/__init__.py
--rw-rw-rw-   0        0        0     1558 2022-08-25 06:08:21.000000 voicevox.py-1.0.2/voicevox/vboxclient.py
--rw-rw-rw-   0        0        0      575 2022-08-25 03:41:26.000000 voicevox.py-1.0.2/voicevox/webapi.py
-drwxrwxrwx   0        0        0        0 2022-08-25 08:26:04.961687 voicevox.py-1.0.2/voicevox.py.egg-info/
--rw-rw-rw-   0        0        0     1094 2022-08-25 08:26:04.000000 voicevox.py-1.0.2/voicevox.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      267 2022-08-25 08:26:04.000000 voicevox.py-1.0.2/voicevox.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-25 08:26:04.000000 voicevox.py-1.0.2/voicevox.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2022-08-25 08:26:04.000000 voicevox.py-1.0.2/voicevox.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-08-25 08:26:04.000000 voicevox.py-1.0.2/voicevox.py.egg-info/top_level.txt
+-rw-r--r--   0        0        0      364 2023-06-09 15:33:43.333667 voicevox_py-1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-09 15:34:25.115828 voicevox_py-1.3/README.md
+-rw-r--r--   0        0        0      134 2023-04-05 23:51:35.158012 voicevox_py-1.3/voicevox/__init__.py
+-rw-r--r--   0        0        0     1608 2023-04-06 03:53:05.794828 voicevox_py-1.3/voicevox/Synthesizer.py
+-rw-r--r--   0        0        0      439 1970-01-01 00:00:00.000000 voicevox_py-1.3/PKG-INFO
```

