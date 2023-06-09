# Comparing `tmp/auto-obsidian-0.1.2.tar.gz` & `tmp/auto-obsidian-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto-obsidian-0.1.2.tar", last modified: Wed Jun  7 21:14:54 2023, max compression
+gzip compressed data, was "auto-obsidian-0.1.3.tar", last modified: Fri Jun  9 02:42:21 2023, max compression
```

## Comparing `auto-obsidian-0.1.2.tar` & `auto-obsidian-0.1.3.tar`

### file list

```diff
@@ -1,51 +1,52 @@
-drwxr-xr-x   0 iyevenko   (501) staff       (20)        0 2023-06-07 21:14:54.212304 auto-obsidian-0.1.2/
--rw-r--r--   0 iyevenko   (501) staff       (20)     2832 2023-06-07 21:14:54.211837 auto-obsidian-0.1.2/PKG-INFO
--rw-r--r--   0 iyevenko   (501) staff       (20)       10 2022-10-14 01:13:43.000000 auto-obsidian-0.1.2/README.md
-drwxr-xr-x   0 iyevenko   (501) staff       (20)        0 2023-06-07 21:14:54.198636 auto-obsidian-0.1.2/auto_obsidian.egg-info/
--rw-r--r--   0 iyevenko   (501) staff       (20)     2832 2023-06-07 21:14:54.000000 auto-obsidian-0.1.2/auto_obsidian.egg-info/PKG-INFO
--rw-r--r--   0 iyevenko   (501) staff       (20)     1170 2023-06-07 21:14:54.000000 auto-obsidian-0.1.2/auto_obsidian.egg-info/SOURCES.txt
--rw-r--r--   0 iyevenko   (501) staff       (20)        1 2023-06-07 21:14:54.000000 auto-obsidian-0.1.2/auto_obsidian.egg-info/dependency_links.txt
--rw-r--r--   0 iyevenko   (501) staff       (20)       50 2023-06-07 21:14:54.000000 auto-obsidian-0.1.2/auto_obsidian.egg-info/entry_points.txt
--rw-r--r--   0 iyevenko   (501) staff       (20)      239 2023-06-07 21:14:54.000000 auto-obsidian-0.1.2/auto_obsidian.egg-info/requires.txt
--rw-r--r--   0 iyevenko   (501) staff       (20)       10 2023-06-07 21:14:54.000000 auto-obsidian-0.1.2/auto_obsidian.egg-info/top_level.txt
-drwxr-xr-x   0 iyevenko   (501) staff       (20)        0 2023-06-07 21:14:54.202491 auto-obsidian-0.1.2/metalayer/
--rw-r--r--   0 iyevenko   (501) staff       (20)      628 2023-06-07 05:41:27.000000 auto-obsidian-0.1.2/metalayer/__init__.py
-drwxr-xr-x   0 iyevenko   (501) staff       (20)        0 2023-06-07 21:14:54.203485 auto-obsidian-0.1.2/metalayer/auto_obsidian/
--rw-r--r--   0 iyevenko   (501) staff       (20)        0 2023-05-26 22:54:04.000000 auto-obsidian-0.1.2/metalayer/auto_obsidian/__init__.py
--rw-r--r--   0 iyevenko   (501) staff       (20)     7626 2023-06-04 06:46:44.000000 auto-obsidian-0.1.2/metalayer/auto_obsidian/engine.py
--rw-r--r--   0 iyevenko   (501) staff       (20)     9717 2023-06-04 05:52:33.000000 auto-obsidian-0.1.2/metalayer/auto_obsidian/graph.py
--rw-r--r--   0 iyevenko   (501) staff       (20)     1623 2023-05-28 19:41:35.000000 auto-obsidian-0.1.2/metalayer/cache.py
-drwxr-xr-x   0 iyevenko   (501) staff       (20)        0 2023-06-07 21:14:54.206277 auto-obsidian-0.1.2/metalayer/chatgpt/
--rw-r--r--   0 iyevenko   (501) staff       (20)       46 2023-05-09 20:44:01.000000 auto-obsidian-0.1.2/metalayer/chatgpt/__init__.py
--rw-r--r--   0 iyevenko   (501) staff       (20)     3906 2023-05-17 22:51:51.000000 auto-obsidian-0.1.2/metalayer/chatgpt/activity_log.py
--rw-r--r--   0 iyevenko   (501) staff       (20)     2158 2023-06-07 05:59:19.000000 auto-obsidian-0.1.2/metalayer/chatgpt/chatgpt.py
--rw-r--r--   0 iyevenko   (501) staff       (20)      920 2023-05-10 23:11:25.000000 auto-obsidian-0.1.2/metalayer/chatgpt/info_extraction.py
--rw-r--r--   0 iyevenko   (501) staff       (20)     1095 2023-05-23 20:24:41.000000 auto-obsidian-0.1.2/metalayer/chatgpt/logger.py
--rw-r--r--   0 iyevenko   (501) staff       (20)      681 2023-05-10 20:30:01.000000 auto-obsidian-0.1.2/metalayer/chatgpt/ocr_filtering.py
-drwxr-xr-x   0 iyevenko   (501) staff       (20)        0 2023-06-07 21:14:54.196097 auto-obsidian-0.1.2/metalayer/chatgpt/prompts/
-drwxr-xr-x   0 iyevenko   (501) staff       (20)        0 2023-06-07 21:14:54.206790 auto-obsidian-0.1.2/metalayer/chatgpt/prompts/activity_log/
--rw-r--r--   0 iyevenko   (501) staff       (20)      332 2023-05-17 17:06:37.000000 auto-obsidian-0.1.2/metalayer/chatgpt/prompts/activity_log/user.txt
-drwxr-xr-x   0 iyevenko   (501) staff       (20)        0 2023-06-07 21:14:54.207913 auto-obsidian-0.1.2/metalayer/chatgpt/prompts/info_extraction/
--rw-r--r--   0 iyevenko   (501) staff       (20)      118 2023-05-10 23:43:20.000000 auto-obsidian-0.1.2/metalayer/chatgpt/prompts/info_extraction/system.txt
--rw-r--r--   0 iyevenko   (501) staff       (20)      373 2023-05-10 23:21:23.000000 auto-obsidian-0.1.2/metalayer/chatgpt/prompts/info_extraction/user.txt
-drwxr-xr-x   0 iyevenko   (501) staff       (20)        0 2023-06-07 21:14:54.208366 auto-obsidian-0.1.2/metalayer/chatgpt/prompts/ocr_filtering/
--rw-r--r--   0 iyevenko   (501) staff       (20)      407 2023-05-08 01:10:43.000000 auto-obsidian-0.1.2/metalayer/chatgpt/prompts/ocr_filtering/user.txt
--rw-r--r--   0 iyevenko   (501) staff       (20)     1537 2023-05-23 19:22:02.000000 auto-obsidian-0.1.2/metalayer/chatgpt/utils.py
--rw-r--r--   0 iyevenko   (501) staff       (20)     5951 2023-06-07 05:59:19.000000 auto-obsidian-0.1.2/metalayer/consumer.py
-drwxr-xr-x   0 iyevenko   (501) staff       (20)        0 2023-06-07 21:14:54.211236 auto-obsidian-0.1.2/metalayer/macos/
--rw-r--r--   0 iyevenko   (501) staff       (20)        0 2023-03-19 08:53:10.000000 auto-obsidian-0.1.2/metalayer/macos/__init__.py
--rw-r--r--   0 iyevenko   (501) staff       (20)      439 2023-03-19 09:22:07.000000 auto-obsidian-0.1.2/metalayer/macos/applescript.py
--rw-r--r--   0 iyevenko   (501) staff       (20)      919 2023-03-19 10:13:21.000000 auto-obsidian-0.1.2/metalayer/macos/battery.py
--rw-r--r--   0 iyevenko   (501) staff       (20)     7735 2023-06-06 04:44:47.000000 auto-obsidian-0.1.2/metalayer/macos/capture.py
--rw-r--r--   0 iyevenko   (501) staff       (20)     2695 2023-06-02 06:18:02.000000 auto-obsidian-0.1.2/metalayer/macos/ocr.py
--rw-r--r--   0 iyevenko   (501) staff       (20)      785 2023-03-19 09:22:07.000000 auto-obsidian-0.1.2/metalayer/macos/utils.py
--rw-r--r--   0 iyevenko   (501) staff       (20)     6091 2023-06-07 20:43:28.000000 auto-obsidian-0.1.2/metalayer/main.py
--rw-r--r--   0 iyevenko   (501) staff       (20)     5087 2023-05-27 17:07:22.000000 auto-obsidian-0.1.2/metalayer/obsidianize.py
--rw-r--r--   0 iyevenko   (501) staff       (20)     3520 2023-06-03 02:33:12.000000 auto-obsidian-0.1.2/metalayer/ocr.py
--rw-r--r--   0 iyevenko   (501) staff       (20)     5022 2023-06-03 04:44:47.000000 auto-obsidian-0.1.2/metalayer/ocr_heuristics.py
--rw-r--r--   0 iyevenko   (501) staff       (20)     3943 2023-05-10 18:36:00.000000 auto-obsidian-0.1.2/metalayer/producer.py
--rw-r--r--   0 iyevenko   (501) staff       (20)      936 2023-05-17 22:58:03.000000 auto-obsidian-0.1.2/metalayer/reindex.py
--rw-r--r--   0 iyevenko   (501) staff       (20)      793 2023-06-07 21:12:37.000000 auto-obsidian-0.1.2/metalayer/setup.py
--rw-r--r--   0 iyevenko   (501) staff       (20)      331 2023-05-13 16:54:14.000000 auto-obsidian-0.1.2/metalayer/system.py
--rw-r--r--   0 iyevenko   (501) staff       (20)     2240 2023-05-05 18:06:18.000000 auto-obsidian-0.1.2/metalayer/utils.py
--rw-r--r--   0 iyevenko   (501) staff       (20)       38 2023-06-07 21:14:54.212462 auto-obsidian-0.1.2/setup.cfg
+drwxr-xr-x   0 iyevenko   (501) staff       (20)        0 2023-06-09 02:42:21.798056 auto-obsidian-0.1.3/
+-rw-r--r--   0 iyevenko   (501) staff       (20)     2954 2023-06-09 02:42:21.797809 auto-obsidian-0.1.3/PKG-INFO
+-rw-r--r--   0 iyevenko   (501) staff       (20)       10 2022-10-14 01:13:43.000000 auto-obsidian-0.1.3/README.md
+drwxr-xr-x   0 iyevenko   (501) staff       (20)        0 2023-06-09 02:42:21.777667 auto-obsidian-0.1.3/auto_obsidian.egg-info/
+-rw-r--r--   0 iyevenko   (501) staff       (20)     2954 2023-06-09 02:42:21.000000 auto-obsidian-0.1.3/auto_obsidian.egg-info/PKG-INFO
+-rw-r--r--   0 iyevenko   (501) staff       (20)     1206 2023-06-09 02:42:21.000000 auto-obsidian-0.1.3/auto_obsidian.egg-info/SOURCES.txt
+-rw-r--r--   0 iyevenko   (501) staff       (20)        1 2023-06-09 02:42:21.000000 auto-obsidian-0.1.3/auto_obsidian.egg-info/dependency_links.txt
+-rw-r--r--   0 iyevenko   (501) staff       (20)       50 2023-06-09 02:42:21.000000 auto-obsidian-0.1.3/auto_obsidian.egg-info/entry_points.txt
+-rw-r--r--   0 iyevenko   (501) staff       (20)      239 2023-06-09 02:42:21.000000 auto-obsidian-0.1.3/auto_obsidian.egg-info/requires.txt
+-rw-r--r--   0 iyevenko   (501) staff       (20)       10 2023-06-09 02:42:21.000000 auto-obsidian-0.1.3/auto_obsidian.egg-info/top_level.txt
+drwxr-xr-x   0 iyevenko   (501) staff       (20)        0 2023-06-09 02:42:21.784150 auto-obsidian-0.1.3/metalayer/
+-rw-r--r--   0 iyevenko   (501) staff       (20)      628 2023-06-07 05:41:27.000000 auto-obsidian-0.1.3/metalayer/__init__.py
+drwxr-xr-x   0 iyevenko   (501) staff       (20)        0 2023-06-09 02:42:21.786075 auto-obsidian-0.1.3/metalayer/auto_obsidian/
+-rw-r--r--   0 iyevenko   (501) staff       (20)        0 2023-05-26 22:54:04.000000 auto-obsidian-0.1.3/metalayer/auto_obsidian/__init__.py
+-rw-r--r--   0 iyevenko   (501) staff       (20)     7618 2023-06-08 05:16:36.000000 auto-obsidian-0.1.3/metalayer/auto_obsidian/engine.py
+-rw-r--r--   0 iyevenko   (501) staff       (20)     9717 2023-06-04 05:52:33.000000 auto-obsidian-0.1.3/metalayer/auto_obsidian/graph.py
+-rw-r--r--   0 iyevenko   (501) staff       (20)     1623 2023-05-28 19:41:35.000000 auto-obsidian-0.1.3/metalayer/cache.py
+drwxr-xr-x   0 iyevenko   (501) staff       (20)        0 2023-06-09 02:42:21.791472 auto-obsidian-0.1.3/metalayer/chatgpt/
+-rw-r--r--   0 iyevenko   (501) staff       (20)      147 2023-06-08 03:22:22.000000 auto-obsidian-0.1.3/metalayer/chatgpt/__init__.py
+-rw-r--r--   0 iyevenko   (501) staff       (20)     3904 2023-06-08 05:16:36.000000 auto-obsidian-0.1.3/metalayer/chatgpt/activity_log.py
+-rw-r--r--   0 iyevenko   (501) staff       (20)     2186 2023-06-08 03:51:36.000000 auto-obsidian-0.1.3/metalayer/chatgpt/chatgpt.py
+-rw-r--r--   0 iyevenko   (501) staff       (20)     1417 2023-06-08 20:07:29.000000 auto-obsidian-0.1.3/metalayer/chatgpt/chatgpt_server.py
+-rw-r--r--   0 iyevenko   (501) staff       (20)      918 2023-06-08 05:16:36.000000 auto-obsidian-0.1.3/metalayer/chatgpt/info_extraction.py
+-rw-r--r--   0 iyevenko   (501) staff       (20)     1095 2023-05-23 20:24:41.000000 auto-obsidian-0.1.3/metalayer/chatgpt/logger.py
+-rw-r--r--   0 iyevenko   (501) staff       (20)      679 2023-06-08 05:16:36.000000 auto-obsidian-0.1.3/metalayer/chatgpt/ocr_filtering.py
+drwxr-xr-x   0 iyevenko   (501) staff       (20)        0 2023-06-09 02:42:21.774779 auto-obsidian-0.1.3/metalayer/chatgpt/prompts/
+drwxr-xr-x   0 iyevenko   (501) staff       (20)        0 2023-06-09 02:42:21.792094 auto-obsidian-0.1.3/metalayer/chatgpt/prompts/activity_log/
+-rw-r--r--   0 iyevenko   (501) staff       (20)      332 2023-05-17 17:06:37.000000 auto-obsidian-0.1.3/metalayer/chatgpt/prompts/activity_log/user.txt
+drwxr-xr-x   0 iyevenko   (501) staff       (20)        0 2023-06-09 02:42:21.793004 auto-obsidian-0.1.3/metalayer/chatgpt/prompts/info_extraction/
+-rw-r--r--   0 iyevenko   (501) staff       (20)      118 2023-05-10 23:43:20.000000 auto-obsidian-0.1.3/metalayer/chatgpt/prompts/info_extraction/system.txt
+-rw-r--r--   0 iyevenko   (501) staff       (20)      373 2023-05-10 23:21:23.000000 auto-obsidian-0.1.3/metalayer/chatgpt/prompts/info_extraction/user.txt
+drwxr-xr-x   0 iyevenko   (501) staff       (20)        0 2023-06-09 02:42:21.793619 auto-obsidian-0.1.3/metalayer/chatgpt/prompts/ocr_filtering/
+-rw-r--r--   0 iyevenko   (501) staff       (20)      407 2023-05-08 01:10:43.000000 auto-obsidian-0.1.3/metalayer/chatgpt/prompts/ocr_filtering/user.txt
+-rw-r--r--   0 iyevenko   (501) staff       (20)     1638 2023-06-08 05:16:36.000000 auto-obsidian-0.1.3/metalayer/chatgpt/utils.py
+-rw-r--r--   0 iyevenko   (501) staff       (20)     5951 2023-06-07 05:59:19.000000 auto-obsidian-0.1.3/metalayer/consumer.py
+drwxr-xr-x   0 iyevenko   (501) staff       (20)        0 2023-06-09 02:42:21.797055 auto-obsidian-0.1.3/metalayer/macos/
+-rw-r--r--   0 iyevenko   (501) staff       (20)        0 2023-03-19 08:53:10.000000 auto-obsidian-0.1.3/metalayer/macos/__init__.py
+-rw-r--r--   0 iyevenko   (501) staff       (20)      439 2023-03-19 09:22:07.000000 auto-obsidian-0.1.3/metalayer/macos/applescript.py
+-rw-r--r--   0 iyevenko   (501) staff       (20)      919 2023-03-19 10:13:21.000000 auto-obsidian-0.1.3/metalayer/macos/battery.py
+-rw-r--r--   0 iyevenko   (501) staff       (20)     7739 2023-06-08 22:44:56.000000 auto-obsidian-0.1.3/metalayer/macos/capture.py
+-rw-r--r--   0 iyevenko   (501) staff       (20)     2695 2023-06-02 06:18:02.000000 auto-obsidian-0.1.3/metalayer/macos/ocr.py
+-rw-r--r--   0 iyevenko   (501) staff       (20)      785 2023-03-19 09:22:07.000000 auto-obsidian-0.1.3/metalayer/macos/utils.py
+-rw-r--r--   0 iyevenko   (501) staff       (20)     8335 2023-06-09 02:41:51.000000 auto-obsidian-0.1.3/metalayer/main.py
+-rw-r--r--   0 iyevenko   (501) staff       (20)     5087 2023-05-27 17:07:22.000000 auto-obsidian-0.1.3/metalayer/obsidianize.py
+-rw-r--r--   0 iyevenko   (501) staff       (20)     3520 2023-06-03 02:33:12.000000 auto-obsidian-0.1.3/metalayer/ocr.py
+-rw-r--r--   0 iyevenko   (501) staff       (20)     5022 2023-06-03 04:44:47.000000 auto-obsidian-0.1.3/metalayer/ocr_heuristics.py
+-rw-r--r--   0 iyevenko   (501) staff       (20)     3943 2023-05-10 18:36:00.000000 auto-obsidian-0.1.3/metalayer/producer.py
+-rw-r--r--   0 iyevenko   (501) staff       (20)      936 2023-05-17 22:58:03.000000 auto-obsidian-0.1.3/metalayer/reindex.py
+-rw-r--r--   0 iyevenko   (501) staff       (20)      793 2023-06-09 02:30:10.000000 auto-obsidian-0.1.3/metalayer/setup.py
+-rw-r--r--   0 iyevenko   (501) staff       (20)      331 2023-05-13 16:54:14.000000 auto-obsidian-0.1.3/metalayer/system.py
+-rw-r--r--   0 iyevenko   (501) staff       (20)     2240 2023-05-05 18:06:18.000000 auto-obsidian-0.1.3/metalayer/utils.py
+-rw-r--r--   0 iyevenko   (501) staff       (20)       38 2023-06-09 02:42:21.798157 auto-obsidian-0.1.3/setup.cfg
```

### Comparing `auto-obsidian-0.1.2/PKG-INFO` & `auto-obsidian-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,62 +1,62 @@
 Metadata-Version: 2.1
 Name: auto-obsidian
-Version: 0.1.2
+Version: 0.1.3
 Summary: A layer on top of your OS that understands what you're doing
 Author: Ivan Yevenko
 Author-email: iyevenko@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Metalayer
 
 When you install this package, you will get a command line tool called `metalayer`.
 
-## Prerequisites
-
-### Permissions
-For each of the following pages in the settings app, you need to check the box next to Terminal or add Terminal.
-- System Preferences > Privacy & Security > Screen Recording
-- System Preferences > Privacy & Security > Accessibility
-- System Preferences > Privacy & Security > Input Monitoring
-
-If you're using chrome, you also need to enable apple events since metalayer uses those to get the 
-title of the active tab and other metadata. 
-To do this, open chrome then click View > Developer > Allow JavaScript from Apple Events.
-
-### OpenAI API key
-You need to get an OpenAI API key with credits to use the metalayer. Sign up [here](https://platform.openai.com).
-Once you have a key, run the following command to set it:
-```bash
-metalayer set-api-key <your-key>
-```
-
-### Initializing your knowledge repo
 To initialize your knowledge repo, run the following command, which will walk you through the process:
 ```bash
 metalayer init
 ```
 
-## Running the metalayer
 When you've initialized the knowledge repo, run the following command:
 ```bash
 metalayer run
 ```
 
 This will start recording your screen(s) and printing a bunch of stuff.
 Once you start looking at stuff related to the folders you created, files should start appearing in those folders.
 After a few minutes, open up your Knowledge Repo folder up in Obsidian to explore the notes!
 
+To stop the metalayer. Type `q` + `enter` in the terminal window where you ran `metalayer run`.
+This stops the program gracefully, but if you need to hard-stop just type `^C` (`control` + `c`).
+
+## Manual Set-up (Optional)
 
-### Manual Set-up
+This section is OPTIONAL. Ignore unless you want/need to set up the metalayer manually.
+
+### Permissions
+For each of the following pages in the settings app, you need to check the box next to Terminal or add Terminal.
+- System Preferences > Privacy & Security > Screen Recording
+- System Preferences > Privacy & Security > Accessibility
+- System Preferences > Privacy & Security > Input Monitoring
+
+If you're using chrome, you also need to enable apple events since metalayer uses those to get the
+title of the active tab and other metadata.
+To do this, open chrome then click View > Developer > Allow JavaScript from Apple Events.
+
+### Setting up your knowledge repo
 The tutorial in `metalayer init` will walk you through this, but in case you want to do it yourself this heres how:
 
 Before you start recording your screen and saving auto-generated markdown notes to a folder,
-you need to first create the folder. I call mine Knowledge Repo.
+you need to first create the folder. I call mine Knowledge Repo. To set your folder as the obsidian vault root, run:
+
+```bash
+metalayer set-vault-dir <path-to-your-folder>
+```
+
 Then, create a subfolder for each topic you want to record notes for.
 NOTE: for each subfolder, you need to create a file called `_desciption.md`,
 which should have a 1-3 sentence description of what you want to be indexed into that folder.
 A more specific description will make filtering quality better. Here's an example from my repo:
 ```
 Knowledge Repo
 ├── Control Theory
```

### Comparing `auto-obsidian-0.1.2/auto_obsidian.egg-info/PKG-INFO` & `auto-obsidian-0.1.3/auto_obsidian.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,62 +1,62 @@
 Metadata-Version: 2.1
 Name: auto-obsidian
-Version: 0.1.2
+Version: 0.1.3
 Summary: A layer on top of your OS that understands what you're doing
 Author: Ivan Yevenko
 Author-email: iyevenko@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Metalayer
 
 When you install this package, you will get a command line tool called `metalayer`.
 
-## Prerequisites
-
-### Permissions
-For each of the following pages in the settings app, you need to check the box next to Terminal or add Terminal.
-- System Preferences > Privacy & Security > Screen Recording
-- System Preferences > Privacy & Security > Accessibility
-- System Preferences > Privacy & Security > Input Monitoring
-
-If you're using chrome, you also need to enable apple events since metalayer uses those to get the 
-title of the active tab and other metadata. 
-To do this, open chrome then click View > Developer > Allow JavaScript from Apple Events.
-
-### OpenAI API key
-You need to get an OpenAI API key with credits to use the metalayer. Sign up [here](https://platform.openai.com).
-Once you have a key, run the following command to set it:
-```bash
-metalayer set-api-key <your-key>
-```
-
-### Initializing your knowledge repo
 To initialize your knowledge repo, run the following command, which will walk you through the process:
 ```bash
 metalayer init
 ```
 
-## Running the metalayer
 When you've initialized the knowledge repo, run the following command:
 ```bash
 metalayer run
 ```
 
 This will start recording your screen(s) and printing a bunch of stuff.
 Once you start looking at stuff related to the folders you created, files should start appearing in those folders.
 After a few minutes, open up your Knowledge Repo folder up in Obsidian to explore the notes!
 
+To stop the metalayer. Type `q` + `enter` in the terminal window where you ran `metalayer run`.
+This stops the program gracefully, but if you need to hard-stop just type `^C` (`control` + `c`).
+
+## Manual Set-up (Optional)
 
-### Manual Set-up
+This section is OPTIONAL. Ignore unless you want/need to set up the metalayer manually.
+
+### Permissions
+For each of the following pages in the settings app, you need to check the box next to Terminal or add Terminal.
+- System Preferences > Privacy & Security > Screen Recording
+- System Preferences > Privacy & Security > Accessibility
+- System Preferences > Privacy & Security > Input Monitoring
+
+If you're using chrome, you also need to enable apple events since metalayer uses those to get the
+title of the active tab and other metadata.
+To do this, open chrome then click View > Developer > Allow JavaScript from Apple Events.
+
+### Setting up your knowledge repo
 The tutorial in `metalayer init` will walk you through this, but in case you want to do it yourself this heres how:
 
 Before you start recording your screen and saving auto-generated markdown notes to a folder,
-you need to first create the folder. I call mine Knowledge Repo.
+you need to first create the folder. I call mine Knowledge Repo. To set your folder as the obsidian vault root, run:
+
+```bash
+metalayer set-vault-dir <path-to-your-folder>
+```
+
 Then, create a subfolder for each topic you want to record notes for.
 NOTE: for each subfolder, you need to create a file called `_desciption.md`,
 which should have a 1-3 sentence description of what you want to be indexed into that folder.
 A more specific description will make filtering quality better. Here's an example from my repo:
 ```
 Knowledge Repo
 ├── Control Theory
```

### Comparing `auto-obsidian-0.1.2/auto_obsidian.egg-info/SOURCES.txt` & `auto-obsidian-0.1.3/auto_obsidian.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 metalayer/utils.py
 metalayer/auto_obsidian/__init__.py
 metalayer/auto_obsidian/engine.py
 metalayer/auto_obsidian/graph.py
 metalayer/chatgpt/__init__.py
 metalayer/chatgpt/activity_log.py
 metalayer/chatgpt/chatgpt.py
+metalayer/chatgpt/chatgpt_server.py
 metalayer/chatgpt/info_extraction.py
 metalayer/chatgpt/logger.py
 metalayer/chatgpt/ocr_filtering.py
 metalayer/chatgpt/utils.py
 metalayer/chatgpt/prompts/activity_log/user.txt
 metalayer/chatgpt/prompts/info_extraction/system.txt
 metalayer/chatgpt/prompts/info_extraction/user.txt
```

### Comparing `auto-obsidian-0.1.2/metalayer/__init__.py` & `auto-obsidian-0.1.3/metalayer/__init__.py`

 * *Files identical despite different names*

### Comparing `auto-obsidian-0.1.2/metalayer/auto_obsidian/engine.py` & `auto-obsidian-0.1.3/metalayer/auto_obsidian/engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import re
 from metalayer.chatgpt import complete_async
-from metalayer.chatgpt.utils import fill_messages, retry_on_rate_limit
+from metalayer.chatgpt.utils import fill_messages, retry_on_exception
 
 
 choose_node_prompt = """\
 \"""
 Application: {0}
 Window Title: {1}
 Summary:
@@ -17,15 +17,15 @@
 Based on the given information, which folder would be the best fit for the user's activity? \
 Please choose from the following options or suggest a new one by selecting the "New folder option":
 
 {5}
 
 Respond with only the number of your answer\
 """
-@retry_on_rate_limit(retries=3)
+@retry_on_exception(retries=3)
 async def choose_node(parent_node, app, title, summary, activity, info):
     if len(parent_node.children) == 0 or parent_node.content is not None:
         return None
     options = parent_node.list_children() + f'\n{len(parent_node.children)+1}. New folder'
     messages = fill_messages(None, choose_node_prompt, app, title, summary, activity, info, options)
     response = await complete_async(messages, temperature=0, stop=['.', ' ', '\n'])
     # find first integer in response
@@ -45,15 +45,15 @@
 
 \"""
 {1}
 \"""
 
 Merge the above two markdown files into one. Use markdown format! Use headings and lists when necessary.\
 """
-@retry_on_rate_limit(retries=3)
+@retry_on_exception(retries=3)
 async def merge_nodes(node1, node2):
     messages = fill_messages(None, merge_node_prompt, node1.content, node2.content)
     response = await complete_async(messages, temperature=0)
     merged_content = response.strip('"')
     merged_node = node1.copy()
     merged_node.content = merged_content
     return merged_node
@@ -77,15 +77,15 @@
 Write the relevant information on my screen in a markdown note, using headings and lists when necessary. \
 This should be an independent note that can be placed in the above folder.
 
 VERY IMPORTANT: DO NOT mention open tabs, bookmarks, files, folders, buttons, or any other system elements \
 from the user's screen. DO NOT acknowledge the existence of a user or their screen. \
 If you include this information you fail the task.\
 """
-@retry_on_rate_limit(retries=3)
+@retry_on_exception(retries=3)
 async def create_node(node, ocr_lines, app, title):
     messages = fill_messages(create_node_system_prompt, create_node_prompt, ocr_lines, app, title, str(node.parent))
     response = await complete_async(messages, temperature=0)
     node.content = response.strip('"')
     return node
 
 
@@ -95,15 +95,15 @@
 \"""
 Given the markdown note above, determine which of the following folders the note should be added to:
 
 {1}
 
 Choose one of the numbered options by only responding with a number.\
 """
-@retry_on_rate_limit(retries=3)
+@retry_on_exception(retries=3)
 async def choose_node_to_update(node):
     parent_node = node.parent
     N = len(parent_node.children)
     options = parent_node.list_children()
     options += f'\n{N+1}. New folder in the {parent_node.get_path()} directory'
     options += f'\n{N+2}. Does not belong in this directory'
 
@@ -126,15 +126,15 @@
 {0}
 \"""
 
 Give the above markdown note a name and a 1-3 sentence description. \
 The name should only include alphanumeric characters and spaces. Format your response like:
 Name | Description\
 """
-@retry_on_rate_limit(retries=3)
+@retry_on_exception(retries=3)
 async def add_name_and_description(node, ignore_name=False, ignore_description=False):
     messages = fill_messages(None, name_and_description_prompt, node.content)
     response = await complete_async(messages, temperature=0)
     name, description, *_ = response.strip('"').split('|')
     name = name.strip()
     description = description.strip()
     if not ignore_name:
@@ -148,15 +148,15 @@
 \"""
 {0}
 \"""
 I need to move some information from this note into a new one. Can you choose a range of headings that could be moved into an independent. Respond with one range of heading indices to remove formatted like this:
 
 [a-b]\
 """
-@retry_on_rate_limit(retries=3)
+@retry_on_exception(retries=3)
 async def split_node(node):
     # Number the headings
     content = node.content
     lines = []
     heading_inds = []
     for i, line in enumerate(content.split('\n')):
         if line.startswith('#'):
@@ -206,15 +206,15 @@
         match = re.search('[a-zA-Z]', line)
         if match is None:
             continue
         i = match.start()
         lines.append(line[i:])
     return '\n'.join(lines)
 
-@retry_on_rate_limit(retries=3)
+@retry_on_exception(retries=3)
 async def make_folders(node):
     subfolders= [f'{child.name} - {child.description}' for child in node.children if child.content is None]
     if len(subfolders) == 0:
         subfolders = ['NONE - directory is empty']
     else:
         subfolders = '\n'.join(subfolders)
```

### Comparing `auto-obsidian-0.1.2/metalayer/auto_obsidian/graph.py` & `auto-obsidian-0.1.3/metalayer/auto_obsidian/graph.py`

 * *Files identical despite different names*

### Comparing `auto-obsidian-0.1.2/metalayer/cache.py` & `auto-obsidian-0.1.3/metalayer/cache.py`

 * *Files identical despite different names*

### Comparing `auto-obsidian-0.1.2/metalayer/chatgpt/activity_log.py` & `auto-obsidian-0.1.3/metalayer/chatgpt/activity_log.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import asyncio
 
 from metalayer.chatgpt import complete, complete_async
-from metalayer.chatgpt.utils import load_prompts, fill_messages, retry_on_rate_limit
+from metalayer.chatgpt.utils import load_prompts, fill_messages, retry_on_exception
 
 
 system_prompt, user_prompt = load_prompts('activity_log')
 
 completion_params = {
     'temperature': 0
 }
@@ -23,15 +23,15 @@
     return {
         'summary': summary,
         'activity': activity,
         'info': info
     }
 
 
-@retry_on_rate_limit(retries=5, initial_wait_time=1)
+@retry_on_exception(retries=5, initial_wait_time=1)
 async def log_activity_async(text):
     messages = fill_messages(system_prompt, user_prompt, text)
     raw_output = await complete_async(messages, **completion_params)
     summary, activity, info, *_ = raw_output.split('\n\n')
 
     summary = summary.split(':')[-1].strip()
     activity = activity.split(':')[-1].strip()
```

### Comparing `auto-obsidian-0.1.2/metalayer/chatgpt/chatgpt.py` & `auto-obsidian-0.1.3/metalayer/chatgpt/chatgpt.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 import asyncio
 import os
 import time
+
 import openai
 
 from metalayer import config
+from metalayer.chatgpt.utils import get_response_text
 from metalayer.chatgpt.logger import log_result, log_result_async
 
-
 openai.api_key = os.getenv("OPENAI_API_KEY")
 if openai.api_key is None:
     openai.api_key = config.get('openai_api_key')
+if openai.api_key is None:
+    raise Exception('No OpenAI API key found in environment or config file')
+
 
 @log_result
 def complete(messages, model='gpt-3.5-turbo', **completion_kwargs):
     response = openai.ChatCompletion.create(model=model, messages=messages, **completion_kwargs)
-    text = response.choices[0].message.content
-    return text.encode("ascii", errors="ignore").decode()
+    return get_response_text(response)
+
 
 @log_result_async
 async def complete_async(messages, model='gpt-3.5-turbo', **completion_kwargs):
     response = await openai.ChatCompletion.acreate(model=model, messages=messages, **completion_kwargs)
-    text = response.choices[0].message.content
-    return text.encode("ascii", errors="ignore").decode()
+    return get_response_text(response)
 
 
 def example():
     messages = [
         {'role': 'system', 'content': "You're a chatbot that makes edgy jokes at the request of the user."},
         {'role': 'user', 'content': "Write me a poem by Alex Jones about frogs."},
     ]
```

### Comparing `auto-obsidian-0.1.2/metalayer/chatgpt/info_extraction.py` & `auto-obsidian-0.1.3/metalayer/chatgpt/info_extraction.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from metalayer.chatgpt import complete, complete_async
-from metalayer.chatgpt.utils import load_prompts, fill_messages, retry_on_rate_limit
+from metalayer.chatgpt.utils import load_prompts, fill_messages, retry_on_exception
 
 
 system_prompt, user_prompt = load_prompts('info_extraction')
 
 completion_params = {
     'temperature': 0,
     'presence_penalty': 0.5,
@@ -15,14 +15,14 @@
     messages = fill_messages(system_prompt, user_prompt, text)
     extracted = complete(messages, **completion_params)
     if extracted.startswith('- '):
         extracted = extracted[2:].replace('\n- ', '\n')
     return extracted
 
 
-@retry_on_rate_limit(retries=5, initial_wait_time=1)
+@retry_on_exception(retries=5, initial_wait_time=1)
 async def extract_info_async(text):
     messages = fill_messages(system_prompt, user_prompt, text)
     extracted = await complete_async(messages, **completion_params)
     if extracted.startswith('- '):
         extracted = extracted[2:].replace('\n- ', '\n')
     return extracted
```

### Comparing `auto-obsidian-0.1.2/metalayer/chatgpt/logger.py` & `auto-obsidian-0.1.3/metalayer/chatgpt/logger.py`

 * *Files identical despite different names*

### Comparing `auto-obsidian-0.1.2/metalayer/chatgpt/utils.py` & `auto-obsidian-0.1.3/metalayer/chatgpt/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,24 +25,29 @@
         messages.append({'role': 'system', 'content': system_prompt})
     if user_prompt:
         if len(args) > 0:
             user_prompt = user_prompt.format(*args)
         messages.append({'role': 'user', 'content': user_prompt})
     return messages
 
+
+def get_response_text(response):
+    text = response.choices[0].message.content
+    return text.encode("ascii", errors="ignore").decode()
+
+
 import asyncio
-from openai.error import OpenAIError
-def retry_on_rate_limit(retries=5, initial_wait_time=1):
+def retry_on_exception(retries=5, initial_wait_time=1):
     def decorator(func):
         async def wrapper(*args, **kwargs):
             wait_time = initial_wait_time
             for attempt in range(retries):
                 try:
                     return await func(*args, **kwargs)
-                except OpenAIError as e:
+                except Exception as e:
                     if attempt == retries - 1:
                         raise e
                     print(e)
                     await asyncio.sleep(wait_time)
                     wait_time *= 2
         return wrapper
     return decorator
```

### Comparing `auto-obsidian-0.1.2/metalayer/consumer.py` & `auto-obsidian-0.1.3/metalayer/consumer.py`

 * *Files identical despite different names*

### Comparing `auto-obsidian-0.1.2/metalayer/macos/battery.py` & `auto-obsidian-0.1.3/metalayer/macos/battery.py`

 * *Files identical despite different names*

### Comparing `auto-obsidian-0.1.2/metalayer/macos/capture.py` & `auto-obsidian-0.1.3/metalayer/macos/capture.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
 def check_window_valid(w, display_bounds, seen_bboxes):
     if WHITELIST and w['kCGWindowOwnerName'] not in WHITELIST:
         return False
 
     if BLACKLIST and w['kCGWindowOwnerName'] in BLACKLIST:
         return False
 
-    if WINDOW_BLACKLIST and w['kCGWindowName'] in WINDOW_BLACKLIST:
+    if WINDOW_BLACKLIST and w.get('kCGWindowName') in WINDOW_BLACKLIST:
         return False
 
     if w['kCGWindowAlpha'] != 1 or w['kCGWindowLayer'] != 0:
         return False
 
     # Window is not too small
     bounds = w['kCGWindowBounds']
```

### Comparing `auto-obsidian-0.1.2/metalayer/macos/ocr.py` & `auto-obsidian-0.1.3/metalayer/macos/ocr.py`

 * *Files identical despite different names*

### Comparing `auto-obsidian-0.1.2/metalayer/macos/utils.py` & `auto-obsidian-0.1.3/metalayer/macos/utils.py`

 * *Files identical despite different names*

### Comparing `auto-obsidian-0.1.2/metalayer/main.py` & `auto-obsidian-0.1.3/metalayer/main.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import argparse
 import json
 import os
 import sys
 from multiprocessing import Queue
 from threading import Thread, Timer
 
+import Quartz.CoreGraphics as cg
+from AppKit import NSWorkspace, NSURL
+
 sys.path.append('../')
 from metalayer import config, CONFIG_PATH
 from metalayer.consumer import CaptureConsumer
 from metalayer.producer import CaptureProducer
 
 
 def main():
@@ -81,22 +84,63 @@
  d8"'    `"8b  88          d8"'    `"8b   88      "8b  88           
 d8'            88         d8'        `8b  88      ,8P  88           
 88             88         88          88  88aaaaaa8P'  88aaaaa      
 88      88888  88         88          88  88""\""\""8b,  88""\"""
 Y8,        88  88         Y8,        ,8P  88      `8b  88
  Y8a.    .a88  88          Y8a.    .a8P   88      a8P  88
   `"Y88888P"   88888888888  `"Y8888Y"'    88888888P"   88888888888
+  K N O W L E D G E   S O L U T I O N S   I N C O R P O R A T E D
 
 """
     print(globe_string)
 
-    vault_dir = os.path.join(os.path.expanduser('~'), 'Knowledge Repo')
+    print('Before you begin, we need you to enable some permissions.')
+    print("You should get some pop-ups asking you to enable settings in your privacy tab.")
+    print("Once you enable the settings, quit and restart Terminal, then rerun metalayer init")
+    print("Press ENTER to continue.")
+    input()
+
+    capture_enabled = cg.CGRequestScreenCaptureAccess()
+    if not capture_enabled:
+        print('Screen Capture not enabled for Terminal. If you did not get a pop-up, please enable manually\n'
+              'in System Preferences > Security & Privacy > Privacy > Screen Recording')
+        print('Press ENTER once you have enabled screen recording. Choose to restart "later".')
+        input()
+
+    listen_enabled = cg.CGRequestListenEventAccess()
+    if not listen_enabled:
+        print('Input Monitoring not enabled for Terminal. If you did not get a pop-up, please enable manually\n'
+              'in System Preferences > Security & Privacy > Privacy > Input Monitoring')
+        print('Press ENTER once you have enabled input monitoring. Choose to restart "later".')
+        input()
+
+    post_enabled = cg.CGRequestPostEventAccess()
+    if not post_enabled:
+        print('Accessibility not enabled for Terminal. If you did not get a pop-up, please enable manually\n'
+              'in System Preferences > Security & Privacy > Privacy > Accessibility')
+        print('Press ENTER once you have enabled accessibility. Choose to restart "later".')
+        input()
+
+
+    print("If you're using Google Chrome, you'll need to grant Terminal Automation access to \nGoogle Chrome.")
+    print('Press ENTER to open Automation settings')
+    print("Press ENTER once you have checked the Google Chrome box under Terminal.")
+    url = "x-apple.systempreferences:com.apple.preference.security?Privacy_Automation"
+    shared_workspace = NSWorkspace.sharedWorkspace()
+    shared_workspace.openURL_(NSURL.URLWithString_(url))
+    input()
+
+    if not all([capture_enabled, listen_enabled, post_enabled]):
+        print("Once you've enabled all permissions, quit and restart Terminal")
+        return
+
+    vault_dir = os.path.join(os.path.expanduser('~'), 'Knowledge-Repo')
     vault_dir = config.get('vault_dir', vault_dir)
 
-    print('Welcome to the metalayer. Your knowledge repo will live in:\n')
+    print('\nWelcome to the metalayer. Your knowledge repo will live in:\n')
     print(vault_dir)
     print("\nIf you'd like to change this, you can run the following command:")
     print('\nmetalayer set-vault-dir <path>\n')
     print("Now let's create some folders to filter what goes into your repo\n")
 
     for _ in range(5):
         print("Enter a topic you'd like to index in your knowledge repo:")
```

### Comparing `auto-obsidian-0.1.2/metalayer/obsidianize.py` & `auto-obsidian-0.1.3/metalayer/obsidianize.py`

 * *Files identical despite different names*

### Comparing `auto-obsidian-0.1.2/metalayer/ocr.py` & `auto-obsidian-0.1.3/metalayer/ocr.py`

 * *Files identical despite different names*

### Comparing `auto-obsidian-0.1.2/metalayer/ocr_heuristics.py` & `auto-obsidian-0.1.3/metalayer/ocr_heuristics.py`

 * *Files identical despite different names*

### Comparing `auto-obsidian-0.1.2/metalayer/producer.py` & `auto-obsidian-0.1.3/metalayer/producer.py`

 * *Files identical despite different names*

### Comparing `auto-obsidian-0.1.2/metalayer/reindex.py` & `auto-obsidian-0.1.3/metalayer/reindex.py`

 * *Files identical despite different names*

### Comparing `auto-obsidian-0.1.2/metalayer/setup.py` & `auto-obsidian-0.1.3/metalayer/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description = f.read()
 
 with open('metalayer/requirements.txt', 'r') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='auto-obsidian',
-    version='0.1.2',
+    version='0.1.3',
     packages=find_packages(),
     package_data={'metalayer.chatgpt': ['prompts/*/*.txt']},
     description="A layer on top of your OS that understands what you're doing",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Ivan Yevenko',
     author_email='iyevenko@gmail.com',
```

### Comparing `auto-obsidian-0.1.2/metalayer/utils.py` & `auto-obsidian-0.1.3/metalayer/utils.py`

 * *Files identical despite different names*

