# Comparing `tmp/chrono_chatgpt-0.1.4.tar.gz` & `tmp/chrono_chatgpt-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chrono_chatgpt-0.1.4.tar", last modified: Fri Jun  9 13:57:31 2023, max compression
+gzip compressed data, was "chrono_chatgpt-0.2.tar", last modified: Fri Jun  9 16:09:07 2023, max compression
```

## Comparing `chrono_chatgpt-0.1.4.tar` & `chrono_chatgpt-0.2.tar`

### file list

```diff
@@ -1,10 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 13:57:31.157984 chrono_chatgpt-0.1.4/
--rw-rw-rw-   0        0        0      228 2023-06-09 13:57:31.156983 chrono_chatgpt-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-06-09 06:11:46.000000 chrono_chatgpt-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-09 13:57:31.155984 chrono_chatgpt-0.1.4/chrono_chatgpt.egg-info/
--rw-rw-rw-   0        0        0      228 2023-06-09 13:57:30.000000 chrono_chatgpt-0.1.4/chrono_chatgpt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      170 2023-06-09 13:57:31.000000 chrono_chatgpt-0.1.4/chrono_chatgpt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 13:57:30.000000 chrono_chatgpt-0.1.4/chrono_chatgpt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 13:57:30.000000 chrono_chatgpt-0.1.4/chrono_chatgpt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-09 13:57:31.157984 chrono_chatgpt-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      506 2023-06-09 13:57:28.000000 chrono_chatgpt-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 16:09:07.873323 chrono_chatgpt-0.2/
+-rw-rw-rw-   0        0        0      226 2023-06-09 16:09:07.873323 chrono_chatgpt-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-06-09 06:11:46.000000 chrono_chatgpt-0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-09 16:09:07.858323 chrono_chatgpt-0.2/chrono_chatgpt/
+-rw-rw-rw-   0        0        0        0 2023-03-24 04:29:09.000000 chrono_chatgpt-0.2/chrono_chatgpt/__init__.py
+-rw-rw-rw-   0        0        0      419 2023-03-24 21:07:32.000000 chrono_chatgpt-0.2/chrono_chatgpt/bot_initializer.py
+-rw-rw-rw-   0        0        0     4094 2023-06-09 16:05:40.000000 chrono_chatgpt-0.2/chrono_chatgpt/chatbot_core.py
+-rw-rw-rw-   0        0        0     3319 2023-03-24 21:07:27.000000 chrono_chatgpt-0.2/chrono_chatgpt/internet_module.py
+-rw-rw-rw-   0        0        0        0 2023-06-09 06:42:11.000000 chrono_chatgpt-0.2/chrono_chatgpt/version0.1.1.py
+drwxrwxrwx   0        0        0        0 2023-06-09 16:09:07.871326 chrono_chatgpt-0.2/chrono_chatgpt.egg-info/
+-rw-rw-rw-   0        0        0      226 2023-06-09 16:09:07.000000 chrono_chatgpt-0.2/chrono_chatgpt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      327 2023-06-09 16:09:07.000000 chrono_chatgpt-0.2/chrono_chatgpt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 16:09:07.000000 chrono_chatgpt-0.2/chrono_chatgpt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-06-09 16:09:07.000000 chrono_chatgpt-0.2/chrono_chatgpt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-09 16:09:07.873323 chrono_chatgpt-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      504 2023-06-09 16:07:22.000000 chrono_chatgpt-0.2/setup.py
```

