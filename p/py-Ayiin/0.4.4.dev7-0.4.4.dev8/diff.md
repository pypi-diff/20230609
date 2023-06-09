# Comparing `tmp/py-Ayiin-0.4.4.dev7.tar.gz` & `tmp/py-Ayiin-0.4.4.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-Ayiin-0.4.4.dev7.tar", last modified: Thu Jun  8 15:48:46 2023, max compression
+gzip compressed data, was "py-Ayiin-0.4.4.dev8.tar", last modified: Fri Jun  9 04:13:52 2023, max compression
```

## Comparing `py-Ayiin-0.4.4.dev7.tar` & `py-Ayiin-0.4.4.dev8.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:48:46.851807 py-Ayiin-0.4.4.dev7/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-08 15:48:35.000000 py-Ayiin-0.4.4.dev7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-08 15:48:35.000000 py-Ayiin-0.4.4.dev7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-08 15:48:35.000000 py-Ayiin-0.4.4.dev7/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-08 15:48:46.851807 py-Ayiin-0.4.4.dev7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-06-08 15:48:35.000000 py-Ayiin-0.4.4.dev7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:48:46.843807 py-Ayiin-0.4.4.dev7/pyAyiin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:48:46.843807 py-Ayiin-0.4.4.dev7/pyAyiin/Clients/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-08 15:48:35.000000 py-Ayiin-0.4.4.dev7/pyAyiin/Clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12525 2023-06-08 15:48:35.000000 py-Ayiin-0.4.4.dev7/pyAyiin/Clients/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-06-08 15:48:35.000000 py-Ayiin-0.4.4.dev7/pyAyiin/Clients/pytgcalls.py
--rw-r--r--   0 runner    (1001) docker     (123)    38643 2023-06-08 15:48:35.000000 py-Ayiin-0.4.4.dev7/pyAyiin/Clients/startup.py
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-08 15:48:35.000000 py-Ayiin-0.4.4.dev7/pyAyiin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-08 15:48:35.000000 py-Ayiin-0.4.4.dev7/pyAyiin/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-06-08 15:48:35.000000 py-Ayiin-0.4.4.dev7/pyAyiin/assistant.py
--rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-06-08 15:48:35.000000 py-Ayiin-0.4.4.dev7/pyAyiin/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:48:46.847807 py-Ayiin-0.4.4.dev7/pyAyiin/dB/
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-06-08 15:48:35.000000 py-Ayiin-0.4.4.dev7/pyAyiin/dB/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-08 15:48:35.000000 py-Ayiin-0.4.4.dev7/pyAyiin/dB/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:48:35.000000 py-Ayiin-0.4.4.dev7/pyAyiin/dB/_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-08 15:48:35.000000 py-Ayiin-0.4.4.dev7/pyAyiin/dB/absen.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-08 15:48:35.000000 py-Ayiin-0.4.4.dev7/pyAyiin/dB/admins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-06-08 15:48:35.000000 py-Ayiin-0.4.4.dev7/pyAyiin/dB/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-08 15:48:35.000000 py-Ayiin-0.4.4.dev7/pyAyiin/dB/blacklistfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-08 15:48:35.000000 py-Ayiin-0.4.4.dev7/pyAyiin/dB/blacklistgcast.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-08 15:48:35.000000 py-Ayiin-0.4.4.dev7/pyAyiin/dB/blacklistuser.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-08 15:48:35.000000 py-Ayiin-0.4.4.dev7/pyAyiin/dB/gban.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-08 15:48:35.000000 py-Ayiin-0.4.4.dev7/pyAyiin/dB/langs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-08 15:48:35.000000 py-Ayiin-0.4.4.dev7/pyAyiin/dB/logdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-06-08 15:48:35.000000 py-Ayiin-0.4.4.dev7/pyAyiin/dB/pmpermit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-08 15:48:35.000000 py-Ayiin-0.4.4.dev7/pyAyiin/dB/premium.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-08 15:48:35.000000 py-Ayiin-0.4.4.dev7/pyAyiin/dB/start.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-08 15:48:35.000000 py-Ayiin-0.4.4.dev7/pyAyiin/dB/sudo.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-08 15:48:35.000000 py-Ayiin-0.4.4.dev7/pyAyiin/dB/variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-08 15:48:35.000000 py-Ayiin-0.4.4.dev7/pyAyiin/dB/videocalls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-08 15:48:35.000000 py-Ayiin-0.4.4.dev7/pyAyiin/dB/welcome.py
--rw-r--r--   0 runner    (1001) docker     (123)    33254 2023-06-08 15:48:35.000000 py-Ayiin-0.4.4.dev7/pyAyiin/decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-08 15:48:35.000000 py-Ayiin-0.4.4.dev7/pyAyiin/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:48:46.847807 py-Ayiin-0.4.4.dev7/pyAyiin/methods/
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-08 15:48:35.000000 py-Ayiin-0.4.4.dev7/pyAyiin/methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10094 2023-06-08 15:48:35.000000 py-Ayiin-0.4.4.dev7/pyAyiin/methods/_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-06-08 15:48:35.000000 py-Ayiin-0.4.4.dev7/pyAyiin/methods/_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-06-08 15:48:35.000000 py-Ayiin-0.4.4.dev7/pyAyiin/methods/changer.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-08 15:48:35.000000 py-Ayiin-0.4.4.dev7/pyAyiin/methods/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-06-08 15:48:35.000000 py-Ayiin-0.4.4.dev7/pyAyiin/methods/func.py
--rw-r--r--   0 runner    (1001) docker     (123)     6278 2023-06-08 15:48:35.000000 py-Ayiin-0.4.4.dev7/pyAyiin/methods/funcb.py
--rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-06-08 15:48:35.000000 py-Ayiin-0.4.4.dev7/pyAyiin/methods/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-08 15:48:35.000000 py-Ayiin-0.4.4.dev7/pyAyiin/methods/hosting.py
--rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-06-08 15:48:35.000000 py-Ayiin-0.4.4.dev7/pyAyiin/methods/inlinebot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-06-08 15:48:35.000000 py-Ayiin-0.4.4.dev7/pyAyiin/methods/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-06-08 15:48:35.000000 py-Ayiin-0.4.4.dev7/pyAyiin/methods/thumbnail.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:48:46.847807 py-Ayiin-0.4.4.dev7/pyAyiin/pyrogram/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-08 15:48:35.000000 py-Ayiin-0.4.4.dev7/pyAyiin/pyrogram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-06-08 15:48:35.000000 py-Ayiin-0.4.4.dev7/pyAyiin/pyrogram/_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13157 2023-06-08 15:48:35.000000 py-Ayiin-0.4.4.dev7/pyAyiin/pyrogram/func.py
--rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-06-08 15:48:35.000000 py-Ayiin-0.4.4.dev7/pyAyiin/pyrogram/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-08 15:48:35.000000 py-Ayiin-0.4.4.dev7/pyAyiin/pyrogram/pastebin.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-08 15:48:35.000000 py-Ayiin-0.4.4.dev7/pyAyiin/pyrogram/sections.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-06-08 15:48:35.000000 py-Ayiin-0.4.4.dev7/pyAyiin/pyrogram/toolbot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-06-08 15:48:35.000000 py-Ayiin-0.4.4.dev7/pyAyiin/pyrogram/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:48:46.851807 py-Ayiin-0.4.4.dev7/pyAyiin/resources/
--rw-r--r--   0 runner    (1001) docker     (123)   281001 2023-06-08 15:48:35.000000 py-Ayiin-0.4.4.dev7/pyAyiin/resources/Logo Ayiin.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    31343 2023-06-08 15:48:35.000000 py-Ayiin-0.4.4.dev7/pyAyiin/resources/Youtube.jpeg
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:48:35.000000 py-Ayiin-0.4.4.dev7/pyAyiin/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39497 2023-06-08 15:48:35.000000 py-Ayiin-0.4.4.dev7/pyAyiin/resources/ayiin_music.jpg
--rw-r--r--   0 runner    (1001) docker     (123)  1808670 2023-06-08 15:48:35.000000 py-Ayiin-0.4.4.dev7/pyAyiin/resources/ayiin_ubot.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    60539 2023-06-08 15:48:35.000000 py-Ayiin-0.4.4.dev7/pyAyiin/resources/ayiin_userbot.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-08 15:48:35.000000 py-Ayiin-0.4.4.dev7/pyAyiin/resources/blank.png
--rw-r--r--   0 runner    (1001) docker     (123)    56364 2023-06-08 15:48:35.000000 py-Ayiin-0.4.4.dev7/pyAyiin/resources/default.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   141612 2023-06-08 15:48:35.000000 py-Ayiin-0.4.4.dev7/pyAyiin/resources/font.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   128248 2023-06-08 15:48:35.000000 py-Ayiin-0.4.4.dev7/pyAyiin/resources/font2.ttf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:48:46.851807 py-Ayiin-0.4.4.dev7/pyAyiin/telethon/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-08 15:48:35.000000 py-Ayiin-0.4.4.dev7/pyAyiin/telethon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:48:46.851807 py-Ayiin-0.4.4.dev7/pyAyiin/telethon/ayiin/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-08 15:48:35.000000 py-Ayiin-0.4.4.dev7/pyAyiin/telethon/ayiin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-08 15:48:35.000000 py-Ayiin-0.4.4.dev7/pyAyiin/telethon/ayiin/_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-06-08 15:48:35.000000 py-Ayiin-0.4.4.dev7/pyAyiin/telethon/ayiin/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-06-08 15:48:35.000000 py-Ayiin-0.4.4.dev7/pyAyiin/telethon/ayiin/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    17263 2023-06-08 15:48:35.000000 py-Ayiin-0.4.4.dev7/pyAyiin/xd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:48:46.851807 py-Ayiin-0.4.4.dev7/py_Ayiin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-08 15:48:46.000000 py-Ayiin-0.4.4.dev7/py_Ayiin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-06-08 15:48:46.000000 py-Ayiin-0.4.4.dev7/py_Ayiin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 15:48:46.000000 py-Ayiin-0.4.4.dev7/py_Ayiin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-08 15:48:46.000000 py-Ayiin-0.4.4.dev7/py_Ayiin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-08 15:48:46.000000 py-Ayiin-0.4.4.dev7/py_Ayiin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-08 15:48:35.000000 py-Ayiin-0.4.4.dev7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 15:48:46.851807 py-Ayiin-0.4.4.dev7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-08 15:48:35.000000 py-Ayiin-0.4.4.dev7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:13:52.084660 py-Ayiin-0.4.4.dev8/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-09 04:13:52.084660 py-Ayiin-0.4.4.dev8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:13:52.064660 py-Ayiin-0.4.4.dev8/pyAyiin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:13:52.064660 py-Ayiin-0.4.4.dev8/pyAyiin/Clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/Clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12525 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/Clients/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/Clients/pytgcalls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38643 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/Clients/startup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:13:52.068660 py-Ayiin-0.4.4.dev8/pyAyiin/dB/
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/dB/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/dB/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/dB/_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/dB/absen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/dB/admins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/dB/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/dB/blacklistfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/dB/blacklistgcast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/dB/blacklistuser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/dB/gban.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/dB/langs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/dB/logdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/dB/pmpermit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/dB/premium.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/dB/start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/dB/sudo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/dB/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/dB/videocalls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/dB/welcome.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33254 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:13:52.072660 py-Ayiin-0.4.4.dev8/pyAyiin/methods/
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10094 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/methods/_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/methods/_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/methods/changer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/methods/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/methods/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6278 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/methods/funcb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/methods/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/methods/hosting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7027 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/methods/inlinebot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/methods/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/methods/thumbnail.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:13:52.076660 py-Ayiin-0.4.4.dev8/pyAyiin/pyrogram/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/pyrogram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/pyrogram/_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13157 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/pyrogram/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/pyrogram/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/pyrogram/pastebin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/pyrogram/sections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/pyrogram/toolbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/pyrogram/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:13:52.080660 py-Ayiin-0.4.4.dev8/pyAyiin/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)   281001 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/resources/Logo Ayiin.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    31343 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/resources/Youtube.jpeg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39497 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/resources/ayiin_music.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)  1808670 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/resources/ayiin_ubot.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    60539 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/resources/ayiin_userbot.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/resources/blank.png
+-rw-r--r--   0 runner    (1001) docker     (123)    56364 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/resources/default.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   141612 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/resources/font.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   128248 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/resources/font2.ttf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:13:52.080660 py-Ayiin-0.4.4.dev8/pyAyiin/telethon/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/telethon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:13:52.080660 py-Ayiin-0.4.4.dev8/pyAyiin/telethon/ayiin/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/telethon/ayiin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/telethon/ayiin/_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/telethon/ayiin/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/telethon/ayiin/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17263 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/xd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:13:52.080660 py-Ayiin-0.4.4.dev8/py_Ayiin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-09 04:13:51.000000 py-Ayiin-0.4.4.dev8/py_Ayiin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-06-09 04:13:52.000000 py-Ayiin-0.4.4.dev8/py_Ayiin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 04:13:51.000000 py-Ayiin-0.4.4.dev8/py_Ayiin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-09 04:13:51.000000 py-Ayiin-0.4.4.dev8/py_Ayiin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-09 04:13:51.000000 py-Ayiin-0.4.4.dev8/py_Ayiin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 04:13:52.084660 py-Ayiin-0.4.4.dev8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/setup.py
```

### Comparing `py-Ayiin-0.4.4.dev7/LICENSE` & `py-Ayiin-0.4.4.dev8/LICENSE`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev7/NOTICE` & `py-Ayiin-0.4.4.dev8/NOTICE`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev7/PKG-INFO` & `py-Ayiin-0.4.4.dev8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-Ayiin
-Version: 0.4.4.dev7
+Version: 0.4.4.dev8
 Summary: A Secure and Powerful Python-Telethon Based and Python-Pyrogram Based Library For Your Userbot Module.
 Home-page: https://github.com/AyiinXd/AyiinXd
 Author: AyiinXd
 Author-email: ayingaming98@gmail.com
 License: GNU General Public License v3.0 (GPL-3.0)
 Project-URL: Bug Tracker, https://github.com/AyiinXd/AyiinXd/issues
 Project-URL: Source Code, https://github.com/AyiinXd/AyiinXd
```

### Comparing `py-Ayiin-0.4.4.dev7/README.md` & `py-Ayiin-0.4.4.dev8/README.md`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev7/pyAyiin/Clients/__init__.py` & `py-Ayiin-0.4.4.dev8/pyAyiin/Clients/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev7/pyAyiin/Clients/client.py` & `py-Ayiin-0.4.4.dev8/pyAyiin/Clients/client.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev7/pyAyiin/Clients/pytgcalls.py` & `py-Ayiin-0.4.4.dev8/pyAyiin/Clients/pytgcalls.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev7/pyAyiin/Clients/startup.py` & `py-Ayiin-0.4.4.dev8/pyAyiin/Clients/startup.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev7/pyAyiin/__init__.py` & `py-Ayiin-0.4.4.dev8/pyAyiin/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,16 +48,17 @@
 
 
 logs = logging.getLogger(__name__)
 
 
 __copyright__ = "Copyright (C) 2022-present AyiinXd <https://github.com/AyiinXd>"
 __license__ = "GNU General Public License v3.0 (GPL-3.0)"
-__version__ = "0.4.4.dev07"
+__version__ = "0.4.4.dev08"
 ayiin_ver = "0.1.1"
+prem_version = "0.1"
 
 
 DEVS = [
     607067484, # Ayiin
     997461844, #Ayang_Ayiin
     2130526178, # Alfa
 ]
```

### Comparing `py-Ayiin-0.4.4.dev7/pyAyiin/__main__.py` & `py-Ayiin-0.4.4.dev8/pyAyiin/__main__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev7/pyAyiin/assistant.py` & `py-Ayiin-0.4.4.dev8/pyAyiin/assistant.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev7/pyAyiin/config.py` & `py-Ayiin-0.4.4.dev8/pyAyiin/config.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev7/pyAyiin/dB/__init__.py` & `py-Ayiin-0.4.4.dev8/pyAyiin/dB/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev7/pyAyiin/dB/absen.py` & `py-Ayiin-0.4.4.dev8/pyAyiin/dB/absen.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev7/pyAyiin/dB/admins.py` & `py-Ayiin-0.4.4.dev8/pyAyiin/dB/admins.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev7/pyAyiin/dB/auth.py` & `py-Ayiin-0.4.4.dev8/pyAyiin/dB/auth.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev7/pyAyiin/dB/blacklistfilter.py` & `py-Ayiin-0.4.4.dev8/pyAyiin/dB/blacklistfilter.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev7/pyAyiin/dB/blacklistgcast.py` & `py-Ayiin-0.4.4.dev8/pyAyiin/dB/blacklistgcast.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev7/pyAyiin/dB/blacklistuser.py` & `py-Ayiin-0.4.4.dev8/pyAyiin/dB/blacklistuser.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev7/pyAyiin/dB/gban.py` & `py-Ayiin-0.4.4.dev8/pyAyiin/dB/gban.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev7/pyAyiin/dB/langs.py` & `py-Ayiin-0.4.4.dev8/pyAyiin/dB/langs.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev7/pyAyiin/dB/logdb.py` & `py-Ayiin-0.4.4.dev8/pyAyiin/dB/logdb.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev7/pyAyiin/dB/pmpermit.py` & `py-Ayiin-0.4.4.dev8/pyAyiin/dB/pmpermit.py`

 * *Files 21% similar despite different names*

```diff
@@ -64,42 +64,70 @@
     doc = {"user_id": user_id, "pmpermit_message": text}
     await pmpermitdb.update_one(
         {"user_id": user_id},
         {"$set": doc},
         upsert=True)
 
 
+async def get_message_pmermit(user_id: int):
+    x = await pmpermitdb.find_one({"user_id": user_id})
+    if not x:
+        return MSG_PERMIT
+    return x["pmpermit_message"]
+
+
 async def limit_pmpermit(user_id: int, limit):
     doc = {"user_id": user_id, "limit": limit}
     await pmpermitdb.update_one(
       {"user_id": user_id},
       {"$set": doc},
       upsert=True)
 
 
+async def get_limit_pmermit(user_id: int):
+    x = await pmpermitdb.find_one({"user_id": user_id})
+    if not x:
+        return LIMIT
+    return x["limit"]
+
+
 async def block_message_pmpermit(user_id: int, text: str):
     doc = {"user_id": user_id, "block_message": text}
     await pmpermitdb.update_one(
       {"user_id": user_id},
       {"$set": doc},
       upsert=True)
 
 
+async def get_block_pmermit(user_id: int):
+    x = await pmpermitdb.find_one({"user_id": user_id})
+    if not x:
+        return BLOCK_MSG
+    return x["block_message"]
+
+
 async def media_pmpermit(user_id: int, url: str):
     doc = {"user_id": user_id, "media_message": url}
     await pmpermitdb.update_one(
       {"user_id": user_id},
       {"$set": doc},
       upsert=True)
 
 
+async def get_media_pmermit(user_id: int):
+    x = await pmpermitdb.find_one({"user_id": user_id})
+    if not x:
+        return None
+    return x["media_message"]
+
+
 async def all_pmpermit(user_id: int):
     result = await pmpermitdb.find_one({"user_id": user_id})
-    if not result:
-        return MSG_PERMIT, None, LIMIT
+    #if not result:
+    #    return MSG_PERMIT, None, LIMIT
     permit = result["pmpermit"]
     pm_message = result.get("pmpermit_message") if result.get("pmpermit_message") is not None else MSG_PERMIT
     media_message = result.get("media_message") 
     limit = result.get("limit") if result.get("limit") is not None else LIMIT
     return pm_message, media_message, limit
```

### Comparing `py-Ayiin-0.4.4.dev7/pyAyiin/dB/premium.py` & `py-Ayiin-0.4.4.dev8/pyAyiin/dB/premium.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev7/pyAyiin/dB/start.py` & `py-Ayiin-0.4.4.dev8/pyAyiin/dB/start.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev7/pyAyiin/dB/sudo.py` & `py-Ayiin-0.4.4.dev8/pyAyiin/dB/sudo.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev7/pyAyiin/dB/variable.py` & `py-Ayiin-0.4.4.dev8/pyAyiin/dB/variable.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev7/pyAyiin/dB/videocalls.py` & `py-Ayiin-0.4.4.dev8/pyAyiin/dB/videocalls.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev7/pyAyiin/dB/welcome.py` & `py-Ayiin-0.4.4.dev8/pyAyiin/dB/welcome.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev7/pyAyiin/decorator.py` & `py-Ayiin-0.4.4.dev8/pyAyiin/decorator.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev7/pyAyiin/exceptions.py` & `py-Ayiin-0.4.4.dev8/pyAyiin/exceptions.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev7/pyAyiin/methods/__init__.py` & `py-Ayiin-0.4.4.dev8/pyAyiin/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev7/pyAyiin/methods/_database.py` & `py-Ayiin-0.4.4.dev8/pyAyiin/methods/_database.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev7/pyAyiin/methods/_misc.py` & `py-Ayiin-0.4.4.dev8/pyAyiin/methods/_misc.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev7/pyAyiin/methods/changer.py` & `py-Ayiin-0.4.4.dev8/pyAyiin/methods/changer.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev7/pyAyiin/methods/converter.py` & `py-Ayiin-0.4.4.dev8/pyAyiin/methods/converter.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev7/pyAyiin/methods/func.py` & `py-Ayiin-0.4.4.dev8/pyAyiin/methods/func.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev7/pyAyiin/methods/funcb.py` & `py-Ayiin-0.4.4.dev8/pyAyiin/methods/funcb.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev7/pyAyiin/methods/helpers.py` & `py-Ayiin-0.4.4.dev8/pyAyiin/methods/helpers.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev7/pyAyiin/methods/hosting.py` & `py-Ayiin-0.4.4.dev8/pyAyiin/methods/hosting.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev7/pyAyiin/methods/inlinebot.py` & `py-Ayiin-0.4.4.dev8/pyAyiin/methods/inlinebot.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 from ..config import Var
 from ..pyrogram.toolbot import ToolBot
 
 
 class InlineBot(Var, ToolBot):
     async def inline_pmpermit(self, user_id, ids):
-        from pyAyiin.dB.pmpermit import all_pmpermit
+        from pyAyiin.dB.pmpermit import all_pmpermit, get_media_pmermit, get_message_pmermit
         
         button = [
             [
                 InlineKeyboardButton(
                     text='• Approve •',
                     callback_data=f'terima_{ids}',
                 ),
@@ -45,17 +45,18 @@
             [
                 InlineKeyboardButton(
                     text='• Close •',
                     callback_data=f'close',
                 ),
             ]
         ]
-        pm_message, media_message, limit = await all_pmpermit(user_id)
+        media_message = await get_media_pmermit(user_id)
+        pm_message = await get_message_pmermit(user_id)
         endsw = (".mp4", ".gif")
-        if media_message: # Jika database HELP_PIC tidak kosong
+        if media_message is not None: # Jika database HELP_PIC tidak kosong
             if media_message.endswith(endsw): # jika format video atau gif 
                 pm_results = [
                     (
                         InlineQueryResultVideo(
                             video_url=media_message,
                             thumb_url=media_message,
                             title="PmPermit",
```

### Comparing `py-Ayiin-0.4.4.dev7/pyAyiin/methods/queue.py` & `py-Ayiin-0.4.4.dev8/pyAyiin/methods/queue.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev7/pyAyiin/methods/thumbnail.py` & `py-Ayiin-0.4.4.dev8/pyAyiin/methods/thumbnail.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev7/pyAyiin/pyrogram/__init__.py` & `py-Ayiin-0.4.4.dev8/pyAyiin/pyrogram/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev7/pyAyiin/pyrogram/_wrappers.py` & `py-Ayiin-0.4.4.dev8/pyAyiin/pyrogram/_wrappers.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev7/pyAyiin/pyrogram/func.py` & `py-Ayiin-0.4.4.dev8/pyAyiin/pyrogram/func.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev7/pyAyiin/pyrogram/misc.py` & `py-Ayiin-0.4.4.dev8/pyAyiin/pyrogram/misc.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev7/pyAyiin/pyrogram/pastebin.py` & `py-Ayiin-0.4.4.dev8/pyAyiin/pyrogram/pastebin.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev7/pyAyiin/pyrogram/sections.py` & `py-Ayiin-0.4.4.dev8/pyAyiin/pyrogram/sections.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev7/pyAyiin/pyrogram/toolbot.py` & `py-Ayiin-0.4.4.dev8/pyAyiin/pyrogram/toolbot.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev7/pyAyiin/pyrogram/tools.py` & `py-Ayiin-0.4.4.dev8/pyAyiin/pyrogram/tools.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev7/pyAyiin/resources/Logo Ayiin.jpg` & `py-Ayiin-0.4.4.dev8/pyAyiin/resources/Logo Ayiin.jpg`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev7/pyAyiin/resources/Youtube.jpeg` & `py-Ayiin-0.4.4.dev8/pyAyiin/resources/Youtube.jpeg`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev7/pyAyiin/resources/ayiin_music.jpg` & `py-Ayiin-0.4.4.dev8/pyAyiin/resources/ayiin_music.jpg`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev7/pyAyiin/resources/ayiin_ubot.jpg` & `py-Ayiin-0.4.4.dev8/pyAyiin/resources/ayiin_ubot.jpg`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev7/pyAyiin/resources/ayiin_userbot.jpg` & `py-Ayiin-0.4.4.dev8/pyAyiin/resources/ayiin_userbot.jpg`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev7/pyAyiin/resources/blank.png` & `py-Ayiin-0.4.4.dev8/pyAyiin/resources/blank.png`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev7/pyAyiin/resources/default.ttf` & `py-Ayiin-0.4.4.dev8/pyAyiin/resources/default.ttf`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev7/pyAyiin/resources/font.ttf` & `py-Ayiin-0.4.4.dev8/pyAyiin/resources/font.ttf`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev7/pyAyiin/resources/font2.ttf` & `py-Ayiin-0.4.4.dev8/pyAyiin/resources/font2.ttf`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev7/pyAyiin/telethon/ayiin/_wrappers.py` & `py-Ayiin-0.4.4.dev8/pyAyiin/telethon/ayiin/_wrappers.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev7/pyAyiin/telethon/ayiin/events.py` & `py-Ayiin-0.4.4.dev8/pyAyiin/telethon/ayiin/events.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev7/pyAyiin/telethon/ayiin/misc.py` & `py-Ayiin-0.4.4.dev8/pyAyiin/telethon/ayiin/misc.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev7/pyAyiin/xd.py` & `py-Ayiin-0.4.4.dev8/pyAyiin/xd.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev7/py_Ayiin.egg-info/PKG-INFO` & `py-Ayiin-0.4.4.dev8/py_Ayiin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-Ayiin
-Version: 0.4.4.dev7
+Version: 0.4.4.dev8
 Summary: A Secure and Powerful Python-Telethon Based and Python-Pyrogram Based Library For Your Userbot Module.
 Home-page: https://github.com/AyiinXd/AyiinXd
 Author: AyiinXd
 Author-email: ayingaming98@gmail.com
 License: GNU General Public License v3.0 (GPL-3.0)
 Project-URL: Bug Tracker, https://github.com/AyiinXd/AyiinXd/issues
 Project-URL: Source Code, https://github.com/AyiinXd/AyiinXd
```

### Comparing `py-Ayiin-0.4.4.dev7/py_Ayiin.egg-info/SOURCES.txt` & `py-Ayiin-0.4.4.dev8/py_Ayiin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev7/setup.py` & `py-Ayiin-0.4.4.dev8/setup.py`

 * *Files identical despite different names*

