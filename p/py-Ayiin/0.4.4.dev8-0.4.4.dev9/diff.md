# Comparing `tmp/py-Ayiin-0.4.4.dev8.tar.gz` & `tmp/py-Ayiin-0.4.4.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-Ayiin-0.4.4.dev8.tar", last modified: Fri Jun  9 04:13:52 2023, max compression
+gzip compressed data, was "py-Ayiin-0.4.4.dev9.tar", last modified: Fri Jun  9 04:36:50 2023, max compression
```

## Comparing `py-Ayiin-0.4.4.dev8.tar` & `py-Ayiin-0.4.4.dev9.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:13:52.084660 py-Ayiin-0.4.4.dev8/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-09 04:13:52.084660 py-Ayiin-0.4.4.dev8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:13:52.064660 py-Ayiin-0.4.4.dev8/pyAyiin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:13:52.064660 py-Ayiin-0.4.4.dev8/pyAyiin/Clients/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/Clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12525 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/Clients/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/Clients/pytgcalls.py
--rw-r--r--   0 runner    (1001) docker     (123)    38643 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/Clients/startup.py
--rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/assistant.py
--rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:13:52.068660 py-Ayiin-0.4.4.dev8/pyAyiin/dB/
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/dB/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/dB/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/dB/_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/dB/absen.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/dB/admins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/dB/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/dB/blacklistfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/dB/blacklistgcast.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/dB/blacklistuser.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/dB/gban.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/dB/langs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/dB/logdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/dB/pmpermit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/dB/premium.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/dB/start.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/dB/sudo.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/dB/variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/dB/videocalls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/dB/welcome.py
--rw-r--r--   0 runner    (1001) docker     (123)    33254 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:13:52.072660 py-Ayiin-0.4.4.dev8/pyAyiin/methods/
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10094 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/methods/_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/methods/_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/methods/changer.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/methods/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/methods/func.py
--rw-r--r--   0 runner    (1001) docker     (123)     6278 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/methods/funcb.py
--rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/methods/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/methods/hosting.py
--rw-r--r--   0 runner    (1001) docker     (123)     7027 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/methods/inlinebot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/methods/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/methods/thumbnail.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:13:52.076660 py-Ayiin-0.4.4.dev8/pyAyiin/pyrogram/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/pyrogram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/pyrogram/_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13157 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/pyrogram/func.py
--rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/pyrogram/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/pyrogram/pastebin.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/pyrogram/sections.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/pyrogram/toolbot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/pyrogram/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:13:52.080660 py-Ayiin-0.4.4.dev8/pyAyiin/resources/
--rw-r--r--   0 runner    (1001) docker     (123)   281001 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/resources/Logo Ayiin.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    31343 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/resources/Youtube.jpeg
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39497 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/resources/ayiin_music.jpg
--rw-r--r--   0 runner    (1001) docker     (123)  1808670 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/resources/ayiin_ubot.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    60539 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/resources/ayiin_userbot.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/resources/blank.png
--rw-r--r--   0 runner    (1001) docker     (123)    56364 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/resources/default.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   141612 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/resources/font.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   128248 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/resources/font2.ttf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:13:52.080660 py-Ayiin-0.4.4.dev8/pyAyiin/telethon/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/telethon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:13:52.080660 py-Ayiin-0.4.4.dev8/pyAyiin/telethon/ayiin/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/telethon/ayiin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/telethon/ayiin/_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/telethon/ayiin/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/telethon/ayiin/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    17263 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/pyAyiin/xd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:13:52.080660 py-Ayiin-0.4.4.dev8/py_Ayiin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-09 04:13:51.000000 py-Ayiin-0.4.4.dev8/py_Ayiin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-06-09 04:13:52.000000 py-Ayiin-0.4.4.dev8/py_Ayiin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 04:13:51.000000 py-Ayiin-0.4.4.dev8/py_Ayiin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-09 04:13:51.000000 py-Ayiin-0.4.4.dev8/py_Ayiin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-09 04:13:51.000000 py-Ayiin-0.4.4.dev8/py_Ayiin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 04:13:52.084660 py-Ayiin-0.4.4.dev8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-09 04:13:39.000000 py-Ayiin-0.4.4.dev8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:36:50.532514 py-Ayiin-0.4.4.dev9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-09 04:36:41.000000 py-Ayiin-0.4.4.dev9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-09 04:36:41.000000 py-Ayiin-0.4.4.dev9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-09 04:36:41.000000 py-Ayiin-0.4.4.dev9/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-09 04:36:50.532514 py-Ayiin-0.4.4.dev9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-06-09 04:36:41.000000 py-Ayiin-0.4.4.dev9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:36:50.524514 py-Ayiin-0.4.4.dev9/pyAyiin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:36:50.524514 py-Ayiin-0.4.4.dev9/pyAyiin/Clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-09 04:36:41.000000 py-Ayiin-0.4.4.dev9/pyAyiin/Clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12525 2023-06-09 04:36:41.000000 py-Ayiin-0.4.4.dev9/pyAyiin/Clients/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-06-09 04:36:41.000000 py-Ayiin-0.4.4.dev9/pyAyiin/Clients/pytgcalls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38643 2023-06-09 04:36:41.000000 py-Ayiin-0.4.4.dev9/pyAyiin/Clients/startup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-06-09 04:36:41.000000 py-Ayiin-0.4.4.dev9/pyAyiin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-09 04:36:41.000000 py-Ayiin-0.4.4.dev9/pyAyiin/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-06-09 04:36:41.000000 py-Ayiin-0.4.4.dev9/pyAyiin/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-06-09 04:36:41.000000 py-Ayiin-0.4.4.dev9/pyAyiin/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:36:50.528514 py-Ayiin-0.4.4.dev9/pyAyiin/dB/
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-06-09 04:36:41.000000 py-Ayiin-0.4.4.dev9/pyAyiin/dB/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-09 04:36:41.000000 py-Ayiin-0.4.4.dev9/pyAyiin/dB/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 04:36:41.000000 py-Ayiin-0.4.4.dev9/pyAyiin/dB/_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-09 04:36:41.000000 py-Ayiin-0.4.4.dev9/pyAyiin/dB/absen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-09 04:36:41.000000 py-Ayiin-0.4.4.dev9/pyAyiin/dB/admins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-06-09 04:36:41.000000 py-Ayiin-0.4.4.dev9/pyAyiin/dB/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-09 04:36:41.000000 py-Ayiin-0.4.4.dev9/pyAyiin/dB/blacklistfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-09 04:36:41.000000 py-Ayiin-0.4.4.dev9/pyAyiin/dB/blacklistgcast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-09 04:36:41.000000 py-Ayiin-0.4.4.dev9/pyAyiin/dB/blacklistuser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-09 04:36:41.000000 py-Ayiin-0.4.4.dev9/pyAyiin/dB/gban.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-09 04:36:41.000000 py-Ayiin-0.4.4.dev9/pyAyiin/dB/langs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-09 04:36:41.000000 py-Ayiin-0.4.4.dev9/pyAyiin/dB/logdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-06-09 04:36:41.000000 py-Ayiin-0.4.4.dev9/pyAyiin/dB/pmpermit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-09 04:36:41.000000 py-Ayiin-0.4.4.dev9/pyAyiin/dB/premium.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-09 04:36:41.000000 py-Ayiin-0.4.4.dev9/pyAyiin/dB/start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-09 04:36:41.000000 py-Ayiin-0.4.4.dev9/pyAyiin/dB/sudo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-09 04:36:41.000000 py-Ayiin-0.4.4.dev9/pyAyiin/dB/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-09 04:36:41.000000 py-Ayiin-0.4.4.dev9/pyAyiin/dB/videocalls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-09 04:36:41.000000 py-Ayiin-0.4.4.dev9/pyAyiin/dB/welcome.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33254 2023-06-09 04:36:41.000000 py-Ayiin-0.4.4.dev9/pyAyiin/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-09 04:36:41.000000 py-Ayiin-0.4.4.dev9/pyAyiin/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:36:50.528514 py-Ayiin-0.4.4.dev9/pyAyiin/methods/
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-09 04:36:41.000000 py-Ayiin-0.4.4.dev9/pyAyiin/methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10094 2023-06-09 04:36:41.000000 py-Ayiin-0.4.4.dev9/pyAyiin/methods/_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-06-09 04:36:41.000000 py-Ayiin-0.4.4.dev9/pyAyiin/methods/_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-06-09 04:36:41.000000 py-Ayiin-0.4.4.dev9/pyAyiin/methods/changer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-09 04:36:41.000000 py-Ayiin-0.4.4.dev9/pyAyiin/methods/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-06-09 04:36:41.000000 py-Ayiin-0.4.4.dev9/pyAyiin/methods/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6173 2023-06-09 04:36:41.000000 py-Ayiin-0.4.4.dev9/pyAyiin/methods/funcb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-06-09 04:36:41.000000 py-Ayiin-0.4.4.dev9/pyAyiin/methods/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-09 04:36:41.000000 py-Ayiin-0.4.4.dev9/pyAyiin/methods/hosting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7155 2023-06-09 04:36:41.000000 py-Ayiin-0.4.4.dev9/pyAyiin/methods/inlinebot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-06-09 04:36:41.000000 py-Ayiin-0.4.4.dev9/pyAyiin/methods/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-06-09 04:36:41.000000 py-Ayiin-0.4.4.dev9/pyAyiin/methods/thumbnail.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:36:50.528514 py-Ayiin-0.4.4.dev9/pyAyiin/pyrogram/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-09 04:36:41.000000 py-Ayiin-0.4.4.dev9/pyAyiin/pyrogram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-06-09 04:36:41.000000 py-Ayiin-0.4.4.dev9/pyAyiin/pyrogram/_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13157 2023-06-09 04:36:41.000000 py-Ayiin-0.4.4.dev9/pyAyiin/pyrogram/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-06-09 04:36:41.000000 py-Ayiin-0.4.4.dev9/pyAyiin/pyrogram/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-09 04:36:41.000000 py-Ayiin-0.4.4.dev9/pyAyiin/pyrogram/pastebin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-09 04:36:41.000000 py-Ayiin-0.4.4.dev9/pyAyiin/pyrogram/sections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-06-09 04:36:41.000000 py-Ayiin-0.4.4.dev9/pyAyiin/pyrogram/toolbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-06-09 04:36:41.000000 py-Ayiin-0.4.4.dev9/pyAyiin/pyrogram/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:36:50.532514 py-Ayiin-0.4.4.dev9/pyAyiin/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)   281001 2023-06-09 04:36:41.000000 py-Ayiin-0.4.4.dev9/pyAyiin/resources/Logo Ayiin.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    31343 2023-06-09 04:36:41.000000 py-Ayiin-0.4.4.dev9/pyAyiin/resources/Youtube.jpeg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 04:36:41.000000 py-Ayiin-0.4.4.dev9/pyAyiin/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39497 2023-06-09 04:36:41.000000 py-Ayiin-0.4.4.dev9/pyAyiin/resources/ayiin_music.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)  1808670 2023-06-09 04:36:41.000000 py-Ayiin-0.4.4.dev9/pyAyiin/resources/ayiin_ubot.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    60539 2023-06-09 04:36:41.000000 py-Ayiin-0.4.4.dev9/pyAyiin/resources/ayiin_userbot.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-09 04:36:41.000000 py-Ayiin-0.4.4.dev9/pyAyiin/resources/blank.png
+-rw-r--r--   0 runner    (1001) docker     (123)    56364 2023-06-09 04:36:41.000000 py-Ayiin-0.4.4.dev9/pyAyiin/resources/default.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   141612 2023-06-09 04:36:41.000000 py-Ayiin-0.4.4.dev9/pyAyiin/resources/font.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   128248 2023-06-09 04:36:41.000000 py-Ayiin-0.4.4.dev9/pyAyiin/resources/font2.ttf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:36:50.532514 py-Ayiin-0.4.4.dev9/pyAyiin/telethon/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-09 04:36:41.000000 py-Ayiin-0.4.4.dev9/pyAyiin/telethon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:36:50.532514 py-Ayiin-0.4.4.dev9/pyAyiin/telethon/ayiin/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-09 04:36:41.000000 py-Ayiin-0.4.4.dev9/pyAyiin/telethon/ayiin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-09 04:36:41.000000 py-Ayiin-0.4.4.dev9/pyAyiin/telethon/ayiin/_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-06-09 04:36:41.000000 py-Ayiin-0.4.4.dev9/pyAyiin/telethon/ayiin/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-06-09 04:36:41.000000 py-Ayiin-0.4.4.dev9/pyAyiin/telethon/ayiin/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17263 2023-06-09 04:36:41.000000 py-Ayiin-0.4.4.dev9/pyAyiin/xd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:36:50.532514 py-Ayiin-0.4.4.dev9/py_Ayiin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-09 04:36:50.000000 py-Ayiin-0.4.4.dev9/py_Ayiin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-06-09 04:36:50.000000 py-Ayiin-0.4.4.dev9/py_Ayiin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 04:36:50.000000 py-Ayiin-0.4.4.dev9/py_Ayiin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-09 04:36:50.000000 py-Ayiin-0.4.4.dev9/py_Ayiin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-09 04:36:50.000000 py-Ayiin-0.4.4.dev9/py_Ayiin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-09 04:36:41.000000 py-Ayiin-0.4.4.dev9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 04:36:50.532514 py-Ayiin-0.4.4.dev9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-09 04:36:41.000000 py-Ayiin-0.4.4.dev9/setup.py
```

### Comparing `py-Ayiin-0.4.4.dev8/LICENSE` & `py-Ayiin-0.4.4.dev9/LICENSE`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev8/NOTICE` & `py-Ayiin-0.4.4.dev9/NOTICE`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev8/PKG-INFO` & `py-Ayiin-0.4.4.dev9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-Ayiin
-Version: 0.4.4.dev8
+Version: 0.4.4.dev9
 Summary: A Secure and Powerful Python-Telethon Based and Python-Pyrogram Based Library For Your Userbot Module.
 Home-page: https://github.com/AyiinXd/AyiinXd
 Author: AyiinXd
 Author-email: ayingaming98@gmail.com
 License: GNU General Public License v3.0 (GPL-3.0)
 Project-URL: Bug Tracker, https://github.com/AyiinXd/AyiinXd/issues
 Project-URL: Source Code, https://github.com/AyiinXd/AyiinXd
```

### Comparing `py-Ayiin-0.4.4.dev8/README.md` & `py-Ayiin-0.4.4.dev9/README.md`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev8/pyAyiin/Clients/__init__.py` & `py-Ayiin-0.4.4.dev9/pyAyiin/Clients/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev8/pyAyiin/Clients/client.py` & `py-Ayiin-0.4.4.dev9/pyAyiin/Clients/client.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev8/pyAyiin/Clients/pytgcalls.py` & `py-Ayiin-0.4.4.dev9/pyAyiin/Clients/pytgcalls.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev8/pyAyiin/Clients/startup.py` & `py-Ayiin-0.4.4.dev9/pyAyiin/Clients/startup.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev8/pyAyiin/__init__.py` & `py-Ayiin-0.4.4.dev9/pyAyiin/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
 
 logs = logging.getLogger(__name__)
 
 
 __copyright__ = "Copyright (C) 2022-present AyiinXd <https://github.com/AyiinXd>"
 __license__ = "GNU General Public License v3.0 (GPL-3.0)"
-__version__ = "0.4.4.dev08"
+__version__ = "0.4.4.dev09"
 ayiin_ver = "0.1.1"
 prem_version = "0.1"
 
 
 DEVS = [
     607067484, # Ayiin
     997461844, #Ayang_Ayiin
```

### Comparing `py-Ayiin-0.4.4.dev8/pyAyiin/__main__.py` & `py-Ayiin-0.4.4.dev9/pyAyiin/__main__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev8/pyAyiin/assistant.py` & `py-Ayiin-0.4.4.dev9/pyAyiin/assistant.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev8/pyAyiin/config.py` & `py-Ayiin-0.4.4.dev9/pyAyiin/config.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev8/pyAyiin/dB/__init__.py` & `py-Ayiin-0.4.4.dev9/pyAyiin/dB/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev8/pyAyiin/dB/absen.py` & `py-Ayiin-0.4.4.dev9/pyAyiin/dB/absen.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev8/pyAyiin/dB/admins.py` & `py-Ayiin-0.4.4.dev9/pyAyiin/dB/admins.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev8/pyAyiin/dB/auth.py` & `py-Ayiin-0.4.4.dev9/pyAyiin/dB/auth.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev8/pyAyiin/dB/blacklistfilter.py` & `py-Ayiin-0.4.4.dev9/pyAyiin/dB/blacklistfilter.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev8/pyAyiin/dB/blacklistgcast.py` & `py-Ayiin-0.4.4.dev9/pyAyiin/dB/blacklistgcast.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev8/pyAyiin/dB/blacklistuser.py` & `py-Ayiin-0.4.4.dev9/pyAyiin/dB/blacklistuser.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev8/pyAyiin/dB/gban.py` & `py-Ayiin-0.4.4.dev9/pyAyiin/dB/gban.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev8/pyAyiin/dB/langs.py` & `py-Ayiin-0.4.4.dev9/pyAyiin/dB/langs.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev8/pyAyiin/dB/logdb.py` & `py-Ayiin-0.4.4.dev9/pyAyiin/dB/logdb.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev8/pyAyiin/dB/pmpermit.py` & `py-Ayiin-0.4.4.dev9/pyAyiin/dB/pmpermit.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev8/pyAyiin/dB/premium.py` & `py-Ayiin-0.4.4.dev9/pyAyiin/dB/premium.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev8/pyAyiin/dB/start.py` & `py-Ayiin-0.4.4.dev9/pyAyiin/dB/start.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev8/pyAyiin/dB/sudo.py` & `py-Ayiin-0.4.4.dev9/pyAyiin/dB/sudo.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev8/pyAyiin/dB/variable.py` & `py-Ayiin-0.4.4.dev9/pyAyiin/dB/variable.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev8/pyAyiin/dB/videocalls.py` & `py-Ayiin-0.4.4.dev9/pyAyiin/dB/videocalls.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev8/pyAyiin/dB/welcome.py` & `py-Ayiin-0.4.4.dev9/pyAyiin/dB/welcome.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev8/pyAyiin/decorator.py` & `py-Ayiin-0.4.4.dev9/pyAyiin/decorator.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev8/pyAyiin/exceptions.py` & `py-Ayiin-0.4.4.dev9/pyAyiin/exceptions.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev8/pyAyiin/methods/__init__.py` & `py-Ayiin-0.4.4.dev9/pyAyiin/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev8/pyAyiin/methods/_database.py` & `py-Ayiin-0.4.4.dev9/pyAyiin/methods/_database.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev8/pyAyiin/methods/_misc.py` & `py-Ayiin-0.4.4.dev9/pyAyiin/methods/_misc.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev8/pyAyiin/methods/changer.py` & `py-Ayiin-0.4.4.dev9/pyAyiin/methods/changer.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev8/pyAyiin/methods/converter.py` & `py-Ayiin-0.4.4.dev9/pyAyiin/methods/converter.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev8/pyAyiin/methods/func.py` & `py-Ayiin-0.4.4.dev9/pyAyiin/methods/func.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev8/pyAyiin/methods/funcb.py` & `py-Ayiin-0.4.4.dev9/pyAyiin/methods/funcb.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,35 +27,33 @@
 
 class FuncBot(object):
     async def approve_pmpermit(
         self,
         cb,
         user_ids,
         chat_id,
-        OLD_MSG,
     ):
         from ..dB.pmpermit import approve_pmpermit, is_pmpermit_approved
 
         
         if isinstance(cb, CallbackQuery):
             if await is_pmpermit_approved(user_ids, chat_id):
                 await cb.answer("Pengguna Ini Sudah Ada Di Database.", show_alert=True)
                 return
+            await cb.answer()
             await approve_pmpermit(user_ids, chat_id)
             await cb.edit_message_text("Pesan Anda Diterima Tod")
-            if str(chat_id) in OLD_MSG:
-                await OLD_MSG[str(chat_id)].delete()
+            await cb.message.delete()
         elif isinstance(cb, Message):
             if await is_pmpermit_approved(user_ids, chat_id):
                 await cb.edit("Pengguna Ini Sudah Ada Di Database.", show_alert=True)
                 return
             await approve_pmpermit(user_ids, chat_id)
             await cb.edit("Pesan Anda Diterima Tod")
-            if str(chat_id) in OLD_MSG:
-                await OLD_MSG[str(chat_id)].delete()
+            await cb.delete()
         
     async def disapprove_pmpermit(
         self,
         cb,
         user_ids,
         chat_id,
     ):
```

### Comparing `py-Ayiin-0.4.4.dev8/pyAyiin/methods/helpers.py` & `py-Ayiin-0.4.4.dev9/pyAyiin/methods/helpers.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev8/pyAyiin/methods/hosting.py` & `py-Ayiin-0.4.4.dev9/pyAyiin/methods/hosting.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev8/pyAyiin/methods/inlinebot.py` & `py-Ayiin-0.4.4.dev9/pyAyiin/methods/inlinebot.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,19 +31,19 @@
     async def inline_pmpermit(self, user_id, ids):
         from pyAyiin.dB.pmpermit import all_pmpermit, get_media_pmermit, get_message_pmermit
         
         button = [
             [
                 InlineKeyboardButton(
                     text='• Approve •',
-                    callback_data=f'terima_{ids}',
+                    callback_data=f'terima_{user_id}xd{ids}',
                 ),
                 InlineKeyboardButton(
                     text='• Disapprove •',
-                    callback_data=f'tolak_{ids}',
+                    callback_data=f'tolak_{user_id}xd{ids}',
                 ),
             ],
             [
                 InlineKeyboardButton(
                     text='• Close •',
                     callback_data=f'close',
                 ),
@@ -137,21 +137,22 @@
                             ),
                         input_message_content=InputTextMessageContent(output),
                     )
                 )
             ]
         return results
     
-    async def inline_alive(self, output, cb):
+    async def inline_alive(self, output):
         from pyAyiin.dB.variable import get_var
         
         alive_pic = await get_var('ALIVE_PIC')
         buttons = [
             [
-                InlineKeyboardButton("•• Help ••", callback_data=cb),
+                InlineKeyboardButton("•• Group ••", url='https://t.me/AyiinChats'),
+                InlineKeyboardButton("•• Channel ••", url='https://t.me/AyiinChannel'),
             ]
         ]
         endsw = (".mp4", ".gif")
         if alive_pic is not None: # Jika database alive tidak kosong
             if alive_pic.endswith(endsw): # jika format video atau gif
                 results = [
                     (
```

### Comparing `py-Ayiin-0.4.4.dev8/pyAyiin/methods/queue.py` & `py-Ayiin-0.4.4.dev9/pyAyiin/methods/queue.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev8/pyAyiin/methods/thumbnail.py` & `py-Ayiin-0.4.4.dev9/pyAyiin/methods/thumbnail.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev8/pyAyiin/pyrogram/__init__.py` & `py-Ayiin-0.4.4.dev9/pyAyiin/pyrogram/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev8/pyAyiin/pyrogram/_wrappers.py` & `py-Ayiin-0.4.4.dev9/pyAyiin/pyrogram/_wrappers.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev8/pyAyiin/pyrogram/func.py` & `py-Ayiin-0.4.4.dev9/pyAyiin/pyrogram/func.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev8/pyAyiin/pyrogram/misc.py` & `py-Ayiin-0.4.4.dev9/pyAyiin/pyrogram/misc.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev8/pyAyiin/pyrogram/pastebin.py` & `py-Ayiin-0.4.4.dev9/pyAyiin/pyrogram/pastebin.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev8/pyAyiin/pyrogram/sections.py` & `py-Ayiin-0.4.4.dev9/pyAyiin/pyrogram/sections.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev8/pyAyiin/pyrogram/toolbot.py` & `py-Ayiin-0.4.4.dev9/pyAyiin/pyrogram/toolbot.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev8/pyAyiin/pyrogram/tools.py` & `py-Ayiin-0.4.4.dev9/pyAyiin/pyrogram/tools.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev8/pyAyiin/resources/Logo Ayiin.jpg` & `py-Ayiin-0.4.4.dev9/pyAyiin/resources/Logo Ayiin.jpg`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev8/pyAyiin/resources/Youtube.jpeg` & `py-Ayiin-0.4.4.dev9/pyAyiin/resources/Youtube.jpeg`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev8/pyAyiin/resources/ayiin_music.jpg` & `py-Ayiin-0.4.4.dev9/pyAyiin/resources/ayiin_music.jpg`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev8/pyAyiin/resources/ayiin_ubot.jpg` & `py-Ayiin-0.4.4.dev9/pyAyiin/resources/ayiin_ubot.jpg`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev8/pyAyiin/resources/ayiin_userbot.jpg` & `py-Ayiin-0.4.4.dev9/pyAyiin/resources/ayiin_userbot.jpg`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev8/pyAyiin/resources/blank.png` & `py-Ayiin-0.4.4.dev9/pyAyiin/resources/blank.png`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev8/pyAyiin/resources/default.ttf` & `py-Ayiin-0.4.4.dev9/pyAyiin/resources/default.ttf`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev8/pyAyiin/resources/font.ttf` & `py-Ayiin-0.4.4.dev9/pyAyiin/resources/font.ttf`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev8/pyAyiin/resources/font2.ttf` & `py-Ayiin-0.4.4.dev9/pyAyiin/resources/font2.ttf`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev8/pyAyiin/telethon/ayiin/_wrappers.py` & `py-Ayiin-0.4.4.dev9/pyAyiin/telethon/ayiin/_wrappers.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev8/pyAyiin/telethon/ayiin/events.py` & `py-Ayiin-0.4.4.dev9/pyAyiin/telethon/ayiin/events.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev8/pyAyiin/telethon/ayiin/misc.py` & `py-Ayiin-0.4.4.dev9/pyAyiin/telethon/ayiin/misc.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev8/pyAyiin/xd.py` & `py-Ayiin-0.4.4.dev9/pyAyiin/xd.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev8/py_Ayiin.egg-info/PKG-INFO` & `py-Ayiin-0.4.4.dev9/py_Ayiin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-Ayiin
-Version: 0.4.4.dev8
+Version: 0.4.4.dev9
 Summary: A Secure and Powerful Python-Telethon Based and Python-Pyrogram Based Library For Your Userbot Module.
 Home-page: https://github.com/AyiinXd/AyiinXd
 Author: AyiinXd
 Author-email: ayingaming98@gmail.com
 License: GNU General Public License v3.0 (GPL-3.0)
 Project-URL: Bug Tracker, https://github.com/AyiinXd/AyiinXd/issues
 Project-URL: Source Code, https://github.com/AyiinXd/AyiinXd
```

### Comparing `py-Ayiin-0.4.4.dev8/py_Ayiin.egg-info/SOURCES.txt` & `py-Ayiin-0.4.4.dev9/py_Ayiin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev8/setup.py` & `py-Ayiin-0.4.4.dev9/setup.py`

 * *Files identical despite different names*

