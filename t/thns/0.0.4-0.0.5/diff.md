# Comparing `tmp/thns-0.0.4.tar.gz` & `tmp/thns-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/thns-0.0.4.tar", last modified: Wed May 13 15:20:58 2020, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `thns-0.0.4.tar` & `thns-0.0.5.tar`

### file list

```diff
@@ -1,25 +1,8 @@
-drwxr-xr-x   0 gukroon   (1000) users      (100)        0 2020-05-13 15:20:58.000000 thns-0.0.4/
-drwxr-xr-x   0 gukroon   (1000) users      (100)        0 2020-05-13 15:20:58.000000 thns-0.0.4/old/
--rwx------   0 gukroon   (1000) users      (100)     5201 2020-05-10 11:48:08.000000 thns-0.0.4/old/thns.sh
--rw-r--r--   0 gukroon   (1000) users      (100)     1799 2020-05-10 11:46:44.000000 thns-0.0.4/.gitignore
--rw-r--r--   0 gukroon   (1000) users      (100)      168 2020-05-10 12:48:27.000000 thns-0.0.4/.gitlab-ci.yml
--rw-r--r--   0 gukroon   (1000) users      (100)     8648 2020-05-13 15:20:58.000000 thns-0.0.4/PKG-INFO
-drwxr-xr-x   0 gukroon   (1000) users      (100)        0 2020-05-13 15:20:58.000000 thns-0.0.4/example/
--rw-r--r--   0 gukroon   (1000) users      (100)  1052327 2020-05-09 16:35:10.000000 thns-0.0.4/example/example.jpg
--rw-r--r--   0 gukroon   (1000) users      (100)     1512 2020-05-09 16:36:39.000000 thns-0.0.4/LICENSE
-drwxr-xr-x   0 gukroon   (1000) users      (100)        0 2020-05-13 15:20:58.000000 thns-0.0.4/thns.egg-info/
--rw-r--r--   0 gukroon   (1000) users      (100)      307 2020-05-13 15:20:58.000000 thns-0.0.4/thns.egg-info/SOURCES.txt
--rw-r--r--   0 gukroon   (1000) users      (100)     8648 2020-05-13 15:20:58.000000 thns-0.0.4/thns.egg-info/PKG-INFO
--rw-r--r--   0 gukroon   (1000) users      (100)        1 2020-05-13 15:20:58.000000 thns-0.0.4/thns.egg-info/dependency_links.txt
--rw-r--r--   0 gukroon   (1000) users      (100)       45 2020-05-13 15:20:58.000000 thns-0.0.4/thns.egg-info/entry_points.txt
--rw-r--r--   0 gukroon   (1000) users      (100)        5 2020-05-13 15:20:58.000000 thns-0.0.4/thns.egg-info/top_level.txt
-drwxr-xr-x   0 gukroon   (1000) users      (100)        0 2020-05-13 15:20:58.000000 thns-0.0.4/init/
--rw-r--r--   0 gukroon   (1000) users      (100)      674 2020-05-10 14:56:46.000000 thns-0.0.4/init/thns.init
--rw-------   0 gukroon   (1000) users      (100)      391 2020-05-10 14:56:29.000000 thns-0.0.4/init/thns.service
--rw-r--r--   0 gukroon   (1000) users      (100)     1278 2020-05-13 15:17:38.000000 thns-0.0.4/setup.py
--rw-r--r--   0 gukroon   (1000) users      (100)      739 2020-05-13 15:17:26.000000 thns-0.0.4/CHANGELOG.md
-drwxr-xr-x   0 gukroon   (1000) users      (100)        0 2020-05-13 15:20:58.000000 thns-0.0.4/thns/
--rwxr-xr-x   0 gukroon   (1000) users      (100)     7820 2020-05-13 15:20:34.000000 thns-0.0.4/thns/__main__.py
--rw-r--r--   0 gukroon   (1000) users      (100)        0 2020-05-10 06:59:24.000000 thns-0.0.4/thns/__init__.py
--rw-r--r--   0 gukroon   (1000) users      (100)     6563 2020-05-13 15:16:10.000000 thns-0.0.4/README.md
--rw-r--r--   0 gukroon   (1000) users      (100)       38 2020-05-13 15:20:58.000000 thns-0.0.4/setup.cfg
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 thns-0.0.5/src/thns/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 thns-0.0.5/src/thns/__init__.py
+-rwxr-xr-x   0        0        0     7820 2020-02-02 00:00:00.000000 thns-0.0.5/src/thns/__main__.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 thns-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 thns-0.0.5/LICENSE
+-rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 thns-0.0.5/README.md
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 thns-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     7803 2020-02-02 00:00:00.000000 thns-0.0.5/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `thns-0.0.4/.gitignore` & `thns-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `thns-0.0.4/PKG-INFO` & `thns-0.0.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,170 +1,174 @@
 Metadata-Version: 2.1
 Name: thns
-Version: 0.0.4
+Version: 0.0.5
 Summary: Get Telegram notifications when requests are being made to your web server
-Home-page: https://gitlab.com/0bs1d1an/thns
-Author: Guido Kroon (@0bs1d1an)
-Author-email: gkroon@maelstrom.ninja
-License: UNKNOWN
 Project-URL: Bug Reports, https://gitlab.com/0bs1d1an/thns/issues
+Project-URL: Homepage, https://gitlab.com/0bs1d1an/thns
 Project-URL: Source, https://gitlab.com/0bs1d1an/thns/
-Description: [![pipeline status](https://gitlab.com/0bs1d1an/thns/badges/master/pipeline.svg)](https://gitlab.com/0bs1d1an/thns/commits/master)
-        
-        # Telegram HTTP notification script
-        
-        This script will notify you of any or selected HTTP requests made to your server, using the Telegram API.
-        It basically performs a `tail -F` on a specified web server access log file (only Nginx is supported for now).
-        Then for each new request it sends a Telegram message to your specified channel.
-        
-        ## Rationale
-        
-        During a red teaming operation I was tasked with writing a script similar to this one, as part of a phishing campaign we launched for our intial entry.
-        The goal of this script was to keep track of people that clicked on our link, downloaded our malicious payload, and submitted a form with their personal details.
-        We wanted to instantly know when such events happened, so that we could move on to the next flag using their compromised box.
-        I decided to make this script more general-purpose and further maintain it here. :-)
-        
-        ## Features
-        
-        - [X] Continuously read the access log, even when the log file is rotated;
-        - [X] Can only match specified requests (e.g. only /robots.txt, /wp-login.php);
-        - [X] Can add the user agent to the message;
-        - [X] Can ignore specified IPs (e.g. 127.0.0.1, ::1);
-        - [X] Can ignore specified HTTP status codes (e.g. 301, 302);
-        - [X] Can look up geo location of the requesting IP;
-        - [X] Can post the location on the map;
-        - [X] Can silently push Telegram messages.
-        
-        ## How to set it up
-        
-        TL;DR - basically 4 steps:
-        
-        1. Create your own Telegram bot;
-        1. Create a new (private) channel and add your bot to that channel;
-        1. Either hardcode your bot key, chat ID, and web server log file in this script, or use the script arguments;
-        1. Consider either editing and installing the systemd / OpenRC service script, or running the script in a `screen` session to run it in the background.
-        
-        Detailed explanation: 
-        
-        First, you will need to create your own [Telegram bot](https://core.telegram.org/bots), which is basically just an API key without any logic (unless you really want to create a [full fledged bot](https://python-telegram-bot.org/)).
-        Once you've created your bot using the [@BotFather](https://telegram.me/BotFather) it will also tell your the bot key (API key).
-        You can either hardcode the bot key in this script, or provide it as an argument (-k) when running this script.
-        
-        Second, create a Telegram (private) channel and write down the chat ID.
-        If you have trouble finding the chat ID, you can use [@username_to_id_bot](https://telegram.me/username_to_id_bot) and paste the invite link in there.
-        It will tell you the channel's chat ID, which you can also hardcode into the script if you want, or provide it as an argument (-c) when running this script.
-        Don't forget to also explicitely add the bot to the channel.
-        
-        Third, either hardcode the web server's access log file location as well, or provide it as an argument (-l) when running this script.
-        
-        Finally, run the script.
-        You could use the thns.service systemd script if you use systemd.
-        Edit the script and install it like described in the Install section below.
-        Or, you could also quickly run the script in a `screen` session to run it in the background so that you can leave your shell.
-        See the Example section for an example on how to do this.
-        Now you can safely logout and the script will remain in the background.
-        To attach again, login to your server again and run `screen -r thns`.
-        
-        ## Install
-        
-        Using Pip:
-        
-        ```
-        # python3 -m pip install thns
-        ```
-        
-        Or, using setup.py:
-        
-        ```
-        # python3 setup.py install
-        ```
-        
-        If you use systemd, you can also add the service script.
-        Edit the script with your own arguments and install it like so:
-        
-        ```
-        # cp thns.service /etc/systemd/system/
-        # systemctl daemon-reload
-        # systemctl enable --now thns.service
-        ```
-        
-        For OpenRC, edit the init script and then install it like so:
-        
-        ```
-        # cp thns.init /etc/init.d/
-        # rc-update add thns
-        # rc-service thns start
-        ```
-        
-        Installing the service script remains a manual step for now.
-        I don't know if there's any way to make this part of the pip package (please reach out to me if you know how to).
-        You could also reach out to your local OS package manager and ask them to make an OS package for this. ;-)
-        
-        ## Usage
-        
-        You can use thns in two ways:
-        
-        * When installed as a package, call the installed script: `thns --help`;
-        * When Git cloned, call the package directly from the root of the Git repository: `python -m thns --help`.
-        
-        ```
-        usage: thns [-h] [-c TELEGRAM_CHAT_ID] [-g] [-iI IGNORE_IPS [IGNORE_IPS ...]]
-                    [-iH IGNORE_HTTP_STATUS_CODES [IGNORE_HTTP_STATUS_CODES ...]]
-                    [-k TELEGRAM_BOT_KEY] [-l LOG_FILE] [-m]
-                    [-r MATCH_REQUESTS [MATCH_REQUESTS ...]] [-s] [-u]
-        
-        Get Telegram notifications when requests are being made to your web server
-        
-        optional arguments:
-          -h, --help            show this help message and exit
-          -c TELEGRAM_CHAT_ID, --chat-id TELEGRAM_CHAT_ID
-                                Specify the Telegram chat ID to post to.
-          -g, --geo             Include geographical information.
-          -iI IGNORE_IPS [IGNORE_IPS ...], --ignore-ips IGNORE_IPS [IGNORE_IPS ...]
-                                Ignore (multiple) IP addresses (e.g. 127.0.0.1 ::1).
-          -iH IGNORE_HTTP_STATUS_CODES [IGNORE_HTTP_STATUS_CODES ...], --ignore-http-status-codes IGNORE_HTTP_STATUS_CODES [IGNORE_HTTP_STATUS_CODES ...]
-                                Ignore (multiple) HTTP status codes (e.g. 301 302).
-          -k TELEGRAM_BOT_KEY, --bot-key TELEGRAM_BOT_KEY
-                                Specify the Telegram bot key.
-          -l LOG_FILE, --log-file LOG_FILE
-                                Specify the (Nginx) log file.
-          -m, --map             Post a map pointer.
-          -r MATCH_REQUESTS [MATCH_REQUESTS ...], --match-requests MATCH_REQUESTS [MATCH_REQUESTS ...]
-                                Match (multiple) specific HTTP requests (e.g. /
-                                /robots.txt).
-          -s, --silent          Send Telegram messages silently.
-          -u, --user-agent      Include the user agent string.
-        ```
-        
-        ## Example
-        
-        If you've edited and installed the systemd / OpenRC service script (see the Install section), you can start / stop it like any other service:
-        
-        ```
-        # systemcl start thnd.service  # systemd
-        # rc-service thns start        # OpenRC
-        ```
-        
-        You could also use `screen` to quickly run it in the background.
-        For example:
-        
-        ```
-        $ screen -S thns -d -m python3 -m thns -m -s -l /var/log/nginx/access.log -c "-1234567890123" -k "123456789:1234567890abcdefghijklmnopqrstuvwxyz" -iI 127.0.0.1 ::1
-        ```
-        
-        Then watch your Telegram channel fill:
-        
-        ![Example](example/example.jpg)
-        
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Author-email: "Guido Kroon (@0bs1d1an)" <gkroon@maelstrom.ninja>
+License-Expression: BSD-3-Clause
+License-File: LICENSE
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
-Classifier: Topic :: Security
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Topic :: Security
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+
+[![pipeline status](https://gitlab.com/0bs1d1an/thns/badges/master/pipeline.svg)](https://gitlab.com/0bs1d1an/thns/commits/master)
+
+# Telegram HTTP notification script
+
+This script will notify you of any or selected HTTP requests made to your server, using the Telegram API.
+It basically performs a `tail -F` on a specified web server access log file (only Nginx is supported for now).
+Then for each new request it sends a Telegram message to your specified channel.
+
+## Rationale
+
+During a red teaming operation I was tasked with writing a script similar to this one, as part of a phishing campaign we launched for our intial entry.
+The goal of this script was to keep track of people that clicked on our link, downloaded our malicious payload, and submitted a form with their personal details.
+We wanted to instantly know when such events happened, so that we could move on to the next flag using their compromised box.
+I decided to make this script more general-purpose and further maintain it here. :-)
+
+## Features
+
+- [X] Continuously read the access log, even when the log file is rotated;
+- [X] Can only match specified requests (e.g. only /robots.txt, /wp-login.php);
+- [X] Can add the user agent to the message;
+- [X] Can ignore specified IPs (e.g. 127.0.0.1, ::1);
+- [X] Can ignore specified HTTP status codes (e.g. 301, 302);
+- [X] Can look up geo location of the requesting IP;
+- [X] Can post the location on the map;
+- [X] Can silently push Telegram messages.
+
+## How to set it up
+
+TL;DR - basically 4 steps:
+
+1. Create your own Telegram bot;
+1. Create a new (private) channel and add your bot to that channel;
+1. Either hardcode your bot key, chat ID, and web server log file in this script, or use the script arguments;
+1. Consider either editing and installing the systemd / OpenRC service script, or running the script in a `screen` session to run it in the background.
+
+Detailed explanation: 
+
+First, you will need to create your own [Telegram bot](https://core.telegram.org/bots), which is basically just an API key without any logic (unless you really want to create a [full fledged bot](https://python-telegram-bot.org/)).
+Once you've created your bot using the [@BotFather](https://telegram.me/BotFather) it will also tell your the bot key (API key).
+You can either hardcode the bot key in this script, or provide it as an argument (-k) when running this script.
+
+Second, create a Telegram (private) channel and write down the chat ID.
+If you have trouble finding the chat ID, you can use [@username_to_id_bot](https://telegram.me/username_to_id_bot) and paste the invite link in there.
+It will tell you the channel's chat ID, which you can also hardcode into the script if you want, or provide it as an argument (-c) when running this script.
+Don't forget to also explicitely add the bot to the channel.
+
+Third, either hardcode the web server's access log file location as well, or provide it as an argument (-l) when running this script.
+
+Finally, run the script.
+You could use the thns.service systemd script if you use systemd.
+Edit the script and install it like described in the Install section below.
+Or, you could also quickly run the script in a `screen` session to run it in the background so that you can leave your shell.
+See the Example section for an example on how to do this.
+Now you can safely logout and the script will remain in the background.
+To attach again, login to your server again and run `screen -r thns`.
+
+## Install
+
+Using Pip:
+
+```
+# python3 -m pip install thns
+```
+
+Or, using setup.py:
+
+```
+# python3 setup.py install
+```
+
+If you use systemd, you can also add the service script.
+Edit the script with your own arguments and install it like so:
+
+```
+# cp thns.service /etc/systemd/system/
+# systemctl daemon-reload
+# systemctl enable --now thns.service
+```
+
+For OpenRC, edit the init script and then install it like so:
+
+```
+# cp thns.init /etc/init.d/
+# rc-update add thns
+# rc-service thns start
+```
+
+Installing the service script remains a manual step for now.
+I don't know if there's any way to make this part of the pip package (please reach out to me if you know how to).
+You could also reach out to your local OS package manager and ask them to make an OS package for this. ;-)
+
+## Usage
+
+You can use thns in two ways:
+
+* When installed as a package, call the installed script: `thns --help`;
+* When Git cloned, call the package directly from the root of the Git repository: `python -m thns --help`.
+
+```
+usage: thns [-h] [-c TELEGRAM_CHAT_ID] [-g] [-iI IGNORE_IPS [IGNORE_IPS ...]]
+            [-iH IGNORE_HTTP_STATUS_CODES [IGNORE_HTTP_STATUS_CODES ...]]
+            [-k TELEGRAM_BOT_KEY] [-l LOG_FILE] [-m]
+            [-r MATCH_REQUESTS [MATCH_REQUESTS ...]] [-s] [-u]
+
+Get Telegram notifications when requests are being made to your web server
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -c TELEGRAM_CHAT_ID, --chat-id TELEGRAM_CHAT_ID
+                        Specify the Telegram chat ID to post to.
+  -g, --geo             Include geographical information.
+  -iI IGNORE_IPS [IGNORE_IPS ...], --ignore-ips IGNORE_IPS [IGNORE_IPS ...]
+                        Ignore (multiple) IP addresses (e.g. 127.0.0.1 ::1).
+  -iH IGNORE_HTTP_STATUS_CODES [IGNORE_HTTP_STATUS_CODES ...], --ignore-http-status-codes IGNORE_HTTP_STATUS_CODES [IGNORE_HTTP_STATUS_CODES ...]
+                        Ignore (multiple) HTTP status codes (e.g. 301 302).
+  -k TELEGRAM_BOT_KEY, --bot-key TELEGRAM_BOT_KEY
+                        Specify the Telegram bot key.
+  -l LOG_FILE, --log-file LOG_FILE
+                        Specify the (Nginx) log file.
+  -m, --map             Post a map pointer.
+  -r MATCH_REQUESTS [MATCH_REQUESTS ...], --match-requests MATCH_REQUESTS [MATCH_REQUESTS ...]
+                        Match (multiple) specific HTTP requests (e.g. /
+                        /robots.txt).
+  -s, --silent          Send Telegram messages silently.
+  -u, --user-agent      Include the user agent string.
+```
+
+## Example
+
+If you've edited and installed the systemd / OpenRC service script (see the Install section), you can start / stop it like any other service:
+
+```
+# systemcl start thnd.service  # systemd
+# rc-service thns start        # OpenRC
+```
+
+You could also use `screen` to quickly run it in the background.
+For example:
+
+```
+$ screen -S thns -d -m python3 -m thns -m -s -l /var/log/nginx/access.log -c "-1234567890123" -k "123456789:1234567890abcdefghijklmnopqrstuvwxyz" -iI 127.0.0.1 ::1
+```
+
+Then watch your Telegram channel fill:
+
+![Example](example/example.jpg)
+
```

### Comparing `thns-0.0.4/LICENSE` & `thns-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `thns-0.0.4/setup.py` & `thns-0.0.5/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,47 @@
-import setuptools
+[build-system]
+requires = ["hatchling"]
+build-backend = "hatchling.build"
 
-with open("README.md", "r") as fh:
-    long_description = fh.read()
+[project]
+name = "thns"
+dynamic = ["version"]
+description = "Get Telegram notifications when requests are being made to your web server"
+readme = "README.md"
+license = "BSD-3-Clause"
+requires-python = ">=3.6"
+authors = [
+  { name = "Guido Kroon (@0bs1d1an)", email = "gkroon@maelstrom.ninja" },
+]
+classifiers = [
+  "Development Status :: 4 - Beta",
+  "Programming Language :: Python",
+  "Programming Language :: Python :: 3.6",
+  "Programming Language :: Python :: 3.7",
+  "Programming Language :: Python :: 3.8",
+  "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: Implementation :: CPython",
+  "Programming Language :: Python :: Implementation :: PyPy",
+  "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
+  "Intended Audience :: Information Technology",
+  "Intended Audience :: System Administrators",
+  "Topic :: Security",
+]
+dependencies = []
 
-setuptools.setup(
-    name="thns",
-    version="0.0.4",
-    author="Guido Kroon (@0bs1d1an)",
-    author_email="gkroon@maelstrom.ninja",
-    description="Get Telegram notifications when requests are being made to " +
-            "your web server",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url="https://gitlab.com/0bs1d1an/thns",
-    packages=setuptools.find_packages(),
-    classifiers=[
-        'Development Status :: 3 - Alpha',
-        'Intended Audience :: Information Technology',
-        'Intended Audience :: System Administrators',
-        'Topic :: Security',
-        "License :: OSI Approved :: BSD License",
-        "Operating System :: OS Independent",
-        "Programming Language :: Python :: 3",
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-    ],
-    python_requires='>=3.6',
-    install_requires=[],
-    entry_points={
-        'console_scripts': [
-            'thns=thns.__main__:main',
-        ],
-    },
-    project_urls={  # Optional
-        'Bug Reports': 'https://gitlab.com/0bs1d1an/thns/issues',
-        'Source': 'https://gitlab.com/0bs1d1an/thns/',
-    },
-)
+[project.scripts]
+thns = "thns.__main__:main"
+
+[project.urls]
+"Bug Reports" = "https://gitlab.com/0bs1d1an/thns/issues"
+Homepage = "https://gitlab.com/0bs1d1an/thns"
+Source = "https://gitlab.com/0bs1d1an/thns/"
+
+[tool.hatch.version]
+path = "src/thns/__about__.py"
+
+[tool.hatch.build.targets.sdist]
+include = [
+    "/src/thns",
+]
```

### Comparing `thns-0.0.4/thns/__main__.py` & `thns-0.0.5/src/thns/__main__.py`

 * *Files identical despite different names*

### Comparing `thns-0.0.4/README.md` & `thns-0.0.5/README.md`

 * *Files identical despite different names*

