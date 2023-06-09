# Comparing `tmp/dfeed-0.0.7.tar.gz` & `tmp/dfeed-0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfeed-0.0.7.tar", last modified: Fri Jun  9 04:20:08 2023, max compression
+gzip compressed data, was "dfeed-0.0b1.tar", last modified: Tue Apr 11 17:49:32 2023, max compression
```

## Comparing `dfeed-0.0.7.tar` & `dfeed-0.0b1.tar`

### file list

```diff
@@ -1,28 +1,30 @@
-drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-06-09 04:20:08.966192 dfeed-0.0.7/
--rw-r--r--   0 anon      (1000) wheel      (998)    34946 2023-04-11 17:54:43.000000 dfeed-0.0.7/LICENSE
--rw-r--r--   0 anon      (1000) wheel      (998)      602 2023-06-09 04:20:08.966192 dfeed-0.0.7/PKG-INFO
--rw-r--r--   0 anon      (1000) wheel      (998)      292 2023-04-14 05:24:00.000000 dfeed-0.0.7/README.md
--rw-r--r--   0 anon      (1000) wheel      (998)      531 2023-06-09 04:19:40.000000 dfeed-0.0.7/pyproject.toml
--rw-r--r--   0 anon      (1000) wheel      (998)       38 2023-06-09 04:20:08.966192 dfeed-0.0.7/setup.cfg
-drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-06-09 04:20:08.962858 dfeed-0.0.7/src/
-drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-06-09 04:20:08.962858 dfeed-0.0.7/src/dfeed/
--rwxr-xr-x   0 anon      (1000) wheel      (998)       23 2022-09-22 02:48:23.000000 dfeed-0.0.7/src/dfeed/__init__.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)      994 2023-06-09 04:18:34.000000 dfeed-0.0.7/src/dfeed/__main__.py
--rw-r--r--   0 anon      (1000) wheel      (998)      705 2023-06-09 04:19:16.000000 dfeed-0.0.7/src/dfeed/args.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     1381 2023-06-09 04:19:16.000000 dfeed-0.0.7/src/dfeed/config.py
--rw-r--r--   0 anon      (1000) wheel      (998)     1907 2023-06-09 04:19:16.000000 dfeed-0.0.7/src/dfeed/list_feed.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)      200 2023-04-11 17:46:36.000000 dfeed-0.0.7/src/dfeed/media.py
--rw-r--r--   0 anon      (1000) wheel      (998)     1289 2023-04-13 22:59:40.000000 dfeed-0.0.7/src/dfeed/opener.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     3185 2023-06-09 01:09:31.000000 dfeed-0.0.7/src/dfeed/options.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     1114 2023-06-09 01:09:31.000000 dfeed-0.0.7/src/dfeed/prompts.py
--rw-r--r--   0 anon      (1000) wheel      (998)    11470 2023-06-09 04:19:16.000000 dfeed-0.0.7/src/dfeed/sfeed.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     2567 2023-06-09 01:09:31.000000 dfeed-0.0.7/src/dfeed/system.py
--rw-r--r--   0 anon      (1000) wheel      (998)     1930 2023-06-09 01:09:31.000000 dfeed-0.0.7/src/dfeed/user.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     4517 2023-04-13 18:56:57.000000 dfeed-0.0.7/src/dfeed/utils.py
-drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-06-09 04:20:08.966192 dfeed-0.0.7/src/dfeed.egg-info/
--rw-r--r--   0 anon      (1000) wheel      (998)      602 2023-06-09 04:20:08.000000 dfeed-0.0.7/src/dfeed.egg-info/PKG-INFO
--rw-r--r--   0 anon      (1000) wheel      (998)      494 2023-06-09 04:20:08.000000 dfeed-0.0.7/src/dfeed.egg-info/SOURCES.txt
--rw-r--r--   0 anon      (1000) wheel      (998)        1 2023-06-09 04:20:08.000000 dfeed-0.0.7/src/dfeed.egg-info/dependency_links.txt
--rw-r--r--   0 anon      (1000) wheel      (998)       46 2023-06-09 04:20:08.000000 dfeed-0.0.7/src/dfeed.egg-info/entry_points.txt
--rw-r--r--   0 anon      (1000) wheel      (998)       24 2023-06-09 04:20:08.000000 dfeed-0.0.7/src/dfeed.egg-info/requires.txt
--rw-r--r--   0 anon      (1000) wheel      (998)        6 2023-06-09 04:20:08.000000 dfeed-0.0.7/src/dfeed.egg-info/top_level.txt
+drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-11 17:49:32.033579 dfeed-0.0b1/
+-rw-r--r--   0 anon      (1000) wheel      (998)    34935 2023-04-11 17:49:00.000000 dfeed-0.0b1/LICENSE
+-rw-r--r--   0 anon      (1000) wheel      (998)      495 2023-04-11 17:49:32.033579 dfeed-0.0b1/PKG-INFO
+-rw-r--r--   0 anon      (1000) wheel      (998)      185 2023-04-11 07:21:35.000000 dfeed-0.0b1/README.md
+-rw-r--r--   0 anon      (1000) wheel      (998)      525 2023-04-11 17:46:18.000000 dfeed-0.0b1/pyproject.toml
+-rw-r--r--   0 anon      (1000) wheel      (998)       38 2023-04-11 17:49:32.033579 dfeed-0.0b1/setup.cfg
+drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-11 17:49:32.030245 dfeed-0.0b1/src/
+drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-11 17:49:32.033579 dfeed-0.0b1/src/dfeed/
+-rwxr-xr-x   0 anon      (1000) wheel      (998)       23 2022-09-22 02:48:23.000000 dfeed-0.0b1/src/dfeed/__init__.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)      962 2023-04-11 17:48:09.000000 dfeed-0.0b1/src/dfeed/__main__.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)      881 2023-04-11 07:28:03.000000 dfeed-0.0b1/src/dfeed/config.py
+-rw-r--r--   0 anon      (1000) wheel      (998)      275 2023-04-11 17:33:52.000000 dfeed-0.0b1/src/dfeed/list_feed.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)      200 2023-04-11 17:46:36.000000 dfeed-0.0b1/src/dfeed/media.py
+drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-11 17:49:32.033579 dfeed-0.0b1/src/dfeed/not_needed/
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     5287 2023-03-26 05:31:33.000000 dfeed-0.0b1/src/dfeed/not_needed/build.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     4113 2023-03-23 03:57:31.000000 dfeed-0.0b1/src/dfeed/not_needed/g_dl.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)      166 2022-09-22 02:48:23.000000 dfeed-0.0b1/src/dfeed/not_needed/initial_setup.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     1968 2023-03-26 06:41:39.000000 dfeed-0.0b1/src/dfeed/not_needed/search.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)      694 2023-04-11 07:24:52.000000 dfeed-0.0b1/src/dfeed/options.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     1190 2023-04-11 17:47:13.000000 dfeed-0.0b1/src/dfeed/prompts.py
+-rw-r--r--   0 anon      (1000) wheel      (998)      350 2023-04-11 17:41:04.000000 dfeed-0.0b1/src/dfeed/sfeed.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     1801 2023-04-11 17:32:45.000000 dfeed-0.0b1/src/dfeed/system.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     2026 2023-04-11 17:30:42.000000 dfeed-0.0b1/src/dfeed/utils.py
+drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-11 17:49:32.033579 dfeed-0.0b1/src/dfeed.egg-info/
+-rw-r--r--   0 anon      (1000) wheel      (998)      495 2023-04-11 17:49:32.000000 dfeed-0.0b1/src/dfeed.egg-info/PKG-INFO
+-rw-r--r--   0 anon      (1000) wheel      (998)      566 2023-04-11 17:49:32.000000 dfeed-0.0b1/src/dfeed.egg-info/SOURCES.txt
+-rw-r--r--   0 anon      (1000) wheel      (998)        1 2023-04-11 17:49:32.000000 dfeed-0.0b1/src/dfeed.egg-info/dependency_links.txt
+-rw-r--r--   0 anon      (1000) wheel      (998)       46 2023-04-11 17:49:32.000000 dfeed-0.0b1/src/dfeed.egg-info/entry_points.txt
+-rw-r--r--   0 anon      (1000) wheel      (998)       17 2023-04-11 17:49:32.000000 dfeed-0.0b1/src/dfeed.egg-info/requires.txt
+-rw-r--r--   0 anon      (1000) wheel      (998)        6 2023-04-11 17:49:32.000000 dfeed-0.0b1/src/dfeed.egg-info/top_level.txt
```

### Comparing `dfeed-0.0.7/LICENSE` & `dfeed-0.0b1/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -556,15 +556,15 @@
 everyone can redistribute and change under these terms.
 
 To do so, attach the following notices to the program. It is safest to attach
 them to the start of each source file to most effectively state the exclusion of
 warranty; and each file should have at least the “copyright” line and a pointer
 to where the full notice is found.
 
-     dfeed - dmenu + sfeed (works with fzf, and rofi too)
+     dfeed - a useful dmenu wrapper for sfeed.
      read.  Copyright (C) 2022 John Dovern
 
      This program is free software: you can redistribute it and/or modify it
      under the terms of the GNU General Public License as published by the Free
      Software Foundation, either version 3 of the License, or (at your option)
      any later version.
```

### Comparing `dfeed-0.0.7/pyproject.toml` & `dfeed-0.0b1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dfeed"
-version = "0.0.7"
+version = "0.0.b1"
 description = "dfeed - dmenu + sfeed (works with fzf, and rofi too)"
 readme = "README.md"
 license = { text = "GNU General Public License v3 (GPLv3)" }
 keywords = [ "mpv", "sfeed", "dmenu" ]
 dependencies = [
     "loadconf",
-    "promptx>=0.0.6"
+    "promptx"
 ]
 
 [project.optional-dependencies]
 
 [project.scripts]
 dfeed = "dfeed.__main__:main"
```

### Comparing `dfeed-0.0.7/src/dfeed/__main__.py` & `dfeed-0.0b1/src/dfeed/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 #!/usr/bin/env python3
 import shlex
 import sys
 
-from .args import Args
 from .config import get_user_settings
+from .sfeed import get_feeds
+
+# from .media import
 from .options import get_opts
-from .sfeed import get_feed_files
 from .system import open_process
-from .user import User
 from .utils import cprint
-from .list_feed import show_list
 
 
 __license__ = "GPL-v3.0"
 __program__ = "dfeed"
 
 
-def process_opts():
+def process_opts(user, args):
     """
     Opts handler for main
     """
-    return show_list()
+    if args.list:
+        return get_feeds(user, args)
+    else:
+        return 1
 
 
 def main():
     """
     Command line application to integrate dmenu into sfeed
     """
     # Set and get command line args
     args = get_opts(__program__)
 
     # Creates a UserSettings object. This will be used by various function
     # to access file paths, settings, filters, and command line args
     user, args = get_user_settings(program=__program__, args=args)
 
-    User.define_user(user)
-    Args.define_args(args)
     # Execute the appropriate function based on command line options
-    return process_opts()
+    return process_opts(user, args=args)
 
 
 if __name__ == "__main__":
     sys.exit(main())
```

### Comparing `dfeed-0.0.7/src/dfeed/prompts.py` & `dfeed-0.0b1/src/dfeed/prompts.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 #!/usr/bin/env python3
 from promptx import PromptX
-from typing import List
-
-from .user import User
+from .utils import cprint
 
 
 class InvalidCmdPrompt(Exception):
     """Exception raised when user has invalid command prompt"""
 
     def __init__(self, error, message="ERROR: prompt_cmd not recognized"):
         self.error = error
@@ -25,21 +23,28 @@
         self.message = message
 
     def __str__(self):
         return f"{self.prefix}{self.message}{self.error}"
 
 
 def user_choice(
-    options: List[str],
-    prompt: str,
+    options,
+    user,
+    prompt,
 ):
     """
     Give user a prompt to choose from a list of options.  Uses dmenu, fzf, or
     rofi
     """
-    p = PromptX(prompt_cmd=User.settings_str("prompt_cmd"))
+    cmd = user.settings["prompt_cmd"]
+    cmd_args = user.settings["prompt_args"]
+    p = PromptX(prompt_cmd=cmd)
+    if cmd == "dmenu" and cmd_args == "":
+        cmd_args = "-l 20 -i"
+
     choice = p.ask(
         options=options,
         prompt=prompt,
-        additional_args=User.settings_str("prompt_args"),
+        additional_args=cmd_args,
     )
+
     return choice
```

