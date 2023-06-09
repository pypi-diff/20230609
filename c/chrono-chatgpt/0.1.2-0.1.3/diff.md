# Comparing `tmp/chrono_chatgpt-0.1.2.tar.gz` & `tmp/chrono_chatgpt-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chrono_chatgpt-0.1.2.tar", last modified: Fri Jun  9 13:44:06 2023, max compression
+gzip compressed data, was "chrono_chatgpt-0.1.3.tar", last modified: Fri Jun  9 13:52:23 2023, max compression
```

## Comparing `chrono_chatgpt-0.1.2.tar` & `chrono_chatgpt-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 13:44:06.047090 chrono_chatgpt-0.1.2/
--rw-rw-rw-   0        0        0      228 2023-06-09 13:44:06.047090 chrono_chatgpt-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-06-09 06:11:46.000000 chrono_chatgpt-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-09 13:44:06.041090 chrono_chatgpt-0.1.2/chrono_chatgpt.egg-info/
--rw-rw-rw-   0        0        0      228 2023-06-09 13:44:05.000000 chrono_chatgpt-0.1.2/chrono_chatgpt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      277 2023-06-09 13:44:05.000000 chrono_chatgpt-0.1.2/chrono_chatgpt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 13:44:05.000000 chrono_chatgpt-0.1.2/chrono_chatgpt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-06-09 13:44:05.000000 chrono_chatgpt-0.1.2/chrono_chatgpt.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-09 13:44:06.046090 chrono_chatgpt-0.1.2/core/
--rw-rw-rw-   0        0        0        0 2023-03-24 04:29:09.000000 chrono_chatgpt-0.1.2/core/__init__.py
--rw-rw-rw-   0        0        0      419 2023-03-24 21:07:32.000000 chrono_chatgpt-0.1.2/core/bot_initializer.py
--rw-rw-rw-   0        0        0     3760 2023-06-09 05:46:47.000000 chrono_chatgpt-0.1.2/core/chatbot_core.py
--rw-rw-rw-   0        0        0     3319 2023-03-24 21:07:27.000000 chrono_chatgpt-0.1.2/core/internet_module.py
--rw-rw-rw-   0        0        0        0 2023-06-09 06:42:11.000000 chrono_chatgpt-0.1.2/core/version0.1.1.py
--rw-rw-rw-   0        0        0       42 2023-06-09 13:44:06.047090 chrono_chatgpt-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      506 2023-06-09 13:43:57.000000 chrono_chatgpt-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 13:52:23.835944 chrono_chatgpt-0.1.3/
+-rw-rw-rw-   0        0        0      228 2023-06-09 13:52:23.834945 chrono_chatgpt-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-06-09 06:11:46.000000 chrono_chatgpt-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-09 13:52:23.833943 chrono_chatgpt-0.1.3/chrono_chatgpt.egg-info/
+-rw-rw-rw-   0        0        0      228 2023-06-09 13:52:23.000000 chrono_chatgpt-0.1.3/chrono_chatgpt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      170 2023-06-09 13:52:23.000000 chrono_chatgpt-0.1.3/chrono_chatgpt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 13:52:23.000000 chrono_chatgpt-0.1.3/chrono_chatgpt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 13:52:23.000000 chrono_chatgpt-0.1.3/chrono_chatgpt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-09 13:52:23.835944 chrono_chatgpt-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      506 2023-06-09 13:51:59.000000 chrono_chatgpt-0.1.3/setup.py
```

