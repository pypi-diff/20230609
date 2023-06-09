# Comparing `tmp/FLOBOT-0.1.115.tar.gz` & `tmp/FLOBOT-0.1.116.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FLOBOT-0.1.115.tar", last modified: Thu Dec 22 13:55:43 2022, max compression
+gzip compressed data, was "FLOBOT-0.1.116.tar", last modified: Fri Jun  9 11:57:10 2023, max compression
```

## Comparing `FLOBOT-0.1.115.tar` & `FLOBOT-0.1.116.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2022-12-22 13:55:43.521206 FLOBOT-0.1.115/
-drwxrwxrwx   0        0        0        0 2022-12-22 13:55:43.302380 FLOBOT-0.1.115/FLOBOT/
--rw-rw-rw-   0        0        0    54302 2022-12-22 13:54:37.000000 FLOBOT-0.1.115/FLOBOT/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-22 13:55:43.483653 FLOBOT-0.1.115/FLOBOT.egg-info/
--rw-rw-rw-   0        0        0      277 2022-12-22 13:55:43.000000 FLOBOT-0.1.115/FLOBOT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      176 2022-12-22 13:55:43.000000 FLOBOT-0.1.115/FLOBOT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-22 13:55:43.000000 FLOBOT-0.1.115/FLOBOT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       93 2022-12-22 13:55:43.000000 FLOBOT-0.1.115/FLOBOT.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2022-12-22 13:55:43.000000 FLOBOT-0.1.115/FLOBOT.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      277 2022-12-22 13:55:43.489756 FLOBOT-0.1.115/PKG-INFO
--rw-rw-rw-   0        0        0       42 2022-12-22 13:55:43.521206 FLOBOT-0.1.115/setup.cfg
--rw-rw-rw-   0        0        0      590 2022-12-22 13:55:02.000000 FLOBOT-0.1.115/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 11:57:10.381962 FLOBOT-0.1.116/
+drwxrwxrwx   0        0        0        0 2023-06-09 11:57:10.131968 FLOBOT-0.1.116/FLOBOT/
+-rw-rw-rw-   0        0        0    54303 2023-06-09 11:55:59.000000 FLOBOT-0.1.116/FLOBOT/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 11:57:10.381962 FLOBOT-0.1.116/FLOBOT.egg-info/
+-rw-rw-rw-   0        0        0      277 2023-06-09 11:57:09.000000 FLOBOT-0.1.116/FLOBOT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      176 2023-06-09 11:57:10.000000 FLOBOT-0.1.116/FLOBOT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 11:57:09.000000 FLOBOT-0.1.116/FLOBOT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       93 2023-06-09 11:57:09.000000 FLOBOT-0.1.116/FLOBOT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-09 11:57:09.000000 FLOBOT-0.1.116/FLOBOT.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      277 2023-06-09 11:57:10.381962 FLOBOT-0.1.116/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-09 11:57:10.397552 FLOBOT-0.1.116/setup.cfg
+-rw-rw-rw-   0        0        0      590 2023-06-09 11:56:15.000000 FLOBOT-0.1.116/setup.py
```

### Comparing `FLOBOT-0.1.115/FLOBOT/__init__.py` & `FLOBOT-0.1.116/FLOBOT/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-try:
+atry:
     # System imports.
     from typing import Tuple, Any, Union, Optional
 
     import asyncio
     import sys
     import datetime
     import json
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-try: # System imports. from typing import Tuple, Any, Union, Optional import
+atry: # System imports. from typing import Tuple, Any, Union, Optional import
 asyncio import sys import datetime import json import functools import os
 import random as py_random import logging import uuid import json import
 subprocess # Third party imports. from fortnitepy.ext import commands from
 colorama import Fore, Back, Style, init init(autoreset=True) from functools
 import partial from datetime import timedelta import crayons try: import
 PirxcyPinger except: pass import fortnitepy import BenBotAsync import
 FortniteAPIAsync import sanic import aiohttp import uvloop import requests
```

### Comparing `FLOBOT-0.1.115/setup.py` & `FLOBOT-0.1.116/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
     
 setuptools.setup(
     name="FLOBOT",
-    version="0.1.115",
+    version="0.1.116",
     author="Sekkay",
     description="Lobby bot.",
     url="https://www.youtube.com",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

