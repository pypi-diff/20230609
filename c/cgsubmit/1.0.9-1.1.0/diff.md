# Comparing `tmp/cgsubmit-1.0.9.tar.gz` & `tmp/cgsubmit-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cgsubmit-1.0.9.tar", last modified: Thu Jun  8 22:03:56 2023, max compression
+gzip compressed data, was "cgsubmit-1.1.0.tar", last modified: Fri Jun  9 10:37:35 2023, max compression
```

## Comparing `cgsubmit-1.0.9.tar` & `cgsubmit-1.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:03:56.790213 cgsubmit-1.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-08 22:03:29.000000 cgsubmit-1.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-06-08 22:03:56.790213 cgsubmit-1.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-06-08 22:03:29.000000 cgsubmit-1.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:03:56.790213 cgsubmit-1.0.9/cgsubmit/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-08 22:03:29.000000 cgsubmit-1.0.9/cgsubmit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-06-08 22:03:29.000000 cgsubmit-1.0.9/cgsubmit/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:03:56.790213 cgsubmit-1.0.9/cgsubmit/api/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-08 22:03:29.000000 cgsubmit-1.0.9/cgsubmit/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-08 22:03:29.000000 cgsubmit-1.0.9/cgsubmit/api/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:03:56.790213 cgsubmit-1.0.9/cgsubmit/games/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-08 22:03:29.000000 cgsubmit-1.0.9/cgsubmit/games/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-06-08 22:03:29.000000 cgsubmit-1.0.9/cgsubmit/games/games.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:03:56.790213 cgsubmit-1.0.9/cgsubmit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-06-08 22:03:56.000000 cgsubmit-1.0.9/cgsubmit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-08 22:03:56.000000 cgsubmit-1.0.9/cgsubmit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 22:03:56.000000 cgsubmit-1.0.9/cgsubmit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-08 22:03:56.000000 cgsubmit-1.0.9/cgsubmit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-08 22:03:56.000000 cgsubmit-1.0.9/cgsubmit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-08 22:03:29.000000 cgsubmit-1.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 22:03:56.790213 cgsubmit-1.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-08 22:03:29.000000 cgsubmit-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:37:35.535842 cgsubmit-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-09 10:37:20.000000 cgsubmit-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-06-09 10:37:35.535842 cgsubmit-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-06-09 10:37:20.000000 cgsubmit-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:37:35.535842 cgsubmit-1.1.0/cgsubmit/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-09 10:37:20.000000 cgsubmit-1.1.0/cgsubmit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-06-09 10:37:20.000000 cgsubmit-1.1.0/cgsubmit/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:37:35.535842 cgsubmit-1.1.0/cgsubmit/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-09 10:37:20.000000 cgsubmit-1.1.0/cgsubmit/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-09 10:37:20.000000 cgsubmit-1.1.0/cgsubmit/api/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:37:35.535842 cgsubmit-1.1.0/cgsubmit/games/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-09 10:37:20.000000 cgsubmit-1.1.0/cgsubmit/games/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-06-09 10:37:20.000000 cgsubmit-1.1.0/cgsubmit/games/games.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:37:35.535842 cgsubmit-1.1.0/cgsubmit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-06-09 10:37:35.000000 cgsubmit-1.1.0/cgsubmit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-09 10:37:35.000000 cgsubmit-1.1.0/cgsubmit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 10:37:35.000000 cgsubmit-1.1.0/cgsubmit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-09 10:37:35.000000 cgsubmit-1.1.0/cgsubmit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-09 10:37:35.000000 cgsubmit-1.1.0/cgsubmit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-09 10:37:20.000000 cgsubmit-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 10:37:35.535842 cgsubmit-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-09 10:37:20.000000 cgsubmit-1.1.0/setup.py
```

### Comparing `cgsubmit-1.0.9/LICENSE` & `cgsubmit-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cgsubmit-1.0.9/PKG-INFO` & `cgsubmit-1.1.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cgsubmit
-Version: 1.0.9
+Version: 1.1.0
 Summary: Analyse your submit in codingame competitions.
 Home-page: https://github.com/FrequentlyMissedDeadlines/cgsubmit
 Author: FrequentlyMissedDeadlines
 Author-email: FrequentlyMissedDeadlines+cgsubmit@gmail.com
 Project-URL: Bug Reports, https://github.com/FrequentlyMissedDeadlines/cgsubmit/issues
 Project-URL: Source, https://github.com/FrequentlyMissedDeadlines/cgsubmit
 Classifier: Programming Language :: Python :: 3
@@ -39,14 +39,18 @@
 ![](https://raw.githubusercontent.com/FrequentlyMissedDeadlines/cgsubmit/main/Doc/output.png)
 ![](https://raw.githubusercontent.com/FrequentlyMissedDeadlines/cgsubmit/main/Doc/Codingame.PNG)
 
 ## Installation
 ```
 pip install cgsubmit
 ```
+or to update to the latest version:
+```
+pip install cgsubmit -U
+```
 
 ## Usage
 ### Getting your test session handle
 This token is linked to your session and game you are playing.
 To retrieve it:
 
 1. open the IDE of the game you are playing in your browser (for example [https://www.codingame.com/ide/puzzle/spring-challenge-2023-ants](https://www.codingame.com/ide/puzzle/spring-challenge-2023-ants))
@@ -55,13 +59,29 @@
 
 ### Run
 
 ```
 python -m cgsubmit -t your-test-session-handle
 ```
 
+or for a most advanced usage use `-h` option to get the description of all parameters:
+
+```
+python -m cgsubmit -h
+usage: cgsubmit [-h] -t TOKEN [--noreplay]
+
+Analyse your submit in codingame competitions.
+
+options:
+  -h, --help            show this help message and exit
+  -t TOKEN, --testsessionhandle TOKEN
+                        The test session handle. If you don't know how to get it, look at the doc: https://github.com/FrequentlyMissedDeadlines/cgsubmit
+  --noreplay            Remove replay URLs.
+```
+
 ### Known issues
 
 If you are using git bash to run the command you might see this kind of error: ```'charmap' codec can't encode character '\u274c' in position 0: character maps to <undefined>```
 
 You must go to the settings and set the encoding to UTF-8:
+
 ![](https://raw.githubusercontent.com/FrequentlyMissedDeadlines/cgsubmit/main/Doc/utf8.PNG)
```

### Comparing `cgsubmit-1.0.9/README.md` & `cgsubmit-1.1.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -15,14 +15,18 @@
 ![](https://raw.githubusercontent.com/FrequentlyMissedDeadlines/cgsubmit/main/Doc/output.png)
 ![](https://raw.githubusercontent.com/FrequentlyMissedDeadlines/cgsubmit/main/Doc/Codingame.PNG)
 
 ## Installation
 ```
 pip install cgsubmit
 ```
+or to update to the latest version:
+```
+pip install cgsubmit -U
+```
 
 ## Usage
 ### Getting your test session handle
 This token is linked to your session and game you are playing.
 To retrieve it:
 
 1. open the IDE of the game you are playing in your browser (for example [https://www.codingame.com/ide/puzzle/spring-challenge-2023-ants](https://www.codingame.com/ide/puzzle/spring-challenge-2023-ants))
@@ -31,13 +35,29 @@
 
 ### Run
 
 ```
 python -m cgsubmit -t your-test-session-handle
 ```
 
+or for a most advanced usage use `-h` option to get the description of all parameters:
+
+```
+python -m cgsubmit -h
+usage: cgsubmit [-h] -t TOKEN [--noreplay]
+
+Analyse your submit in codingame competitions.
+
+options:
+  -h, --help            show this help message and exit
+  -t TOKEN, --testsessionhandle TOKEN
+                        The test session handle. If you don't know how to get it, look at the doc: https://github.com/FrequentlyMissedDeadlines/cgsubmit
+  --noreplay            Remove replay URLs.
+```
+
 ### Known issues
 
 If you are using git bash to run the command you might see this kind of error: ```'charmap' codec can't encode character '\u274c' in position 0: character maps to <undefined>```
 
 You must go to the settings and set the encoding to UTF-8:
+
 ![](https://raw.githubusercontent.com/FrequentlyMissedDeadlines/cgsubmit/main/Doc/utf8.PNG)
```

### Comparing `cgsubmit-1.0.9/cgsubmit/__main__.py` & `cgsubmit-1.1.0/cgsubmit/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 
 import argparse
 from cgsubmit.api import *
 from cgsubmit.games import *
 import sys
 
 def main():
-    parser = argparse.ArgumentParser(description='Analyse your submit in codingame competitions.')
-    parser.add_argument('-t', '--testsessionhandle', required=True, help='The test session handle. If you don\'t know how to get it, look at the doc: https://github.com/FrequentlyMissedDeadlines/cgsubmit')
-   
+    parser = argparse.ArgumentParser(description='Analyse your submit in codingame competitions.', prog='cgsubmit')
+    parser.add_argument('-t', '--testsessionhandle', metavar='TOKEN', required=True, help='The test session handle. If you don\'t know how to get it, look at the doc: https://github.com/FrequentlyMissedDeadlines/cgsubmit')
+    parser.add_argument('--noreplay', required=False, help='Remove replay URLs.', action='store_true')
+
     args = parser.parse_args()
     sys.stdout.reconfigure(encoding='utf-8')
 
     try:
         api = Api(args.testsessionhandle)
         battles = api.get_all_battles()
         games = Games(battles)
@@ -23,23 +24,28 @@
         print('Total win and draw: {0}'.format(len(games.win)))
         print('Total lose: {0}'.format(len(games.lost)))
         print()
 
         if len(timeouts) > 0:
             print('❌Total timeouts {0}'.format(len(timeouts)))
             for timeout in timeouts:
-                print('⌛Timeout in game #{1} https://www.codingame.com/replay/{0}'.format(timeout['gameId'], games.number_by_id[timeout['gameId']]))
+                if args.noreplay:
+                    print('⌛Timeout in game #{0}'.format(games.number_by_id[timeout['gameId']]))
+                else:
+                    print('⌛Timeout in game #{1} https://www.codingame.com/replay/{0}'.format(timeout['gameId'], games.number_by_id[timeout['gameId']]))
         else:
             print('✅ No timeouts detected')
 
         lost_games.sort(key=lambda a: abs(a['scores'][0] - a['scores'][1]), reverse=True)
 
         print()
         for game in lost_games:
-            print('➤ Lost game #{2} https://www.codingame.com/replay/{0} by {1} points'.format(game['gameId'], abs(game['scores'][0] - game['scores'][1]), games.number_by_id[game['gameId']]))
-
+            if args.noreplay:
+                print('➤ Lost game #{1} by {0} points'.format(abs(game['scores'][0] - game['scores'][1]), games.number_by_id[game['gameId']]))
+            else:
+                print('➤ Lost game #{2} https://www.codingame.com/replay/{0} by {1} points'.format(game['gameId'], abs(game['scores'][0] - game['scores'][1]), games.number_by_id[game['gameId']])) 
         
     except Exception as exception:
         print(str(exception))
 
 if __name__ == '__main__':
 	main()
```

### Comparing `cgsubmit-1.0.9/cgsubmit/api/api.py` & `cgsubmit-1.1.0/cgsubmit/api/api.py`

 * *Files identical despite different names*

### Comparing `cgsubmit-1.0.9/cgsubmit/games/games.py` & `cgsubmit-1.1.0/cgsubmit/games/games.py`

 * *Files identical despite different names*

### Comparing `cgsubmit-1.0.9/cgsubmit.egg-info/PKG-INFO` & `cgsubmit-1.1.0/cgsubmit.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cgsubmit
-Version: 1.0.9
+Version: 1.1.0
 Summary: Analyse your submit in codingame competitions.
 Home-page: https://github.com/FrequentlyMissedDeadlines/cgsubmit
 Author: FrequentlyMissedDeadlines
 Author-email: FrequentlyMissedDeadlines+cgsubmit@gmail.com
 Project-URL: Bug Reports, https://github.com/FrequentlyMissedDeadlines/cgsubmit/issues
 Project-URL: Source, https://github.com/FrequentlyMissedDeadlines/cgsubmit
 Classifier: Programming Language :: Python :: 3
@@ -39,14 +39,18 @@
 ![](https://raw.githubusercontent.com/FrequentlyMissedDeadlines/cgsubmit/main/Doc/output.png)
 ![](https://raw.githubusercontent.com/FrequentlyMissedDeadlines/cgsubmit/main/Doc/Codingame.PNG)
 
 ## Installation
 ```
 pip install cgsubmit
 ```
+or to update to the latest version:
+```
+pip install cgsubmit -U
+```
 
 ## Usage
 ### Getting your test session handle
 This token is linked to your session and game you are playing.
 To retrieve it:
 
 1. open the IDE of the game you are playing in your browser (for example [https://www.codingame.com/ide/puzzle/spring-challenge-2023-ants](https://www.codingame.com/ide/puzzle/spring-challenge-2023-ants))
@@ -55,13 +59,29 @@
 
 ### Run
 
 ```
 python -m cgsubmit -t your-test-session-handle
 ```
 
+or for a most advanced usage use `-h` option to get the description of all parameters:
+
+```
+python -m cgsubmit -h
+usage: cgsubmit [-h] -t TOKEN [--noreplay]
+
+Analyse your submit in codingame competitions.
+
+options:
+  -h, --help            show this help message and exit
+  -t TOKEN, --testsessionhandle TOKEN
+                        The test session handle. If you don't know how to get it, look at the doc: https://github.com/FrequentlyMissedDeadlines/cgsubmit
+  --noreplay            Remove replay URLs.
+```
+
 ### Known issues
 
 If you are using git bash to run the command you might see this kind of error: ```'charmap' codec can't encode character '\u274c' in position 0: character maps to <undefined>```
 
 You must go to the settings and set the encoding to UTF-8:
+
 ![](https://raw.githubusercontent.com/FrequentlyMissedDeadlines/cgsubmit/main/Doc/utf8.PNG)
```

### Comparing `cgsubmit-1.0.9/setup.py` & `cgsubmit-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 README_MD = open(join(dirname(abspath(__file__)), "README.md")).read()
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
     name="cgsubmit",
-    version="1.0.9",
+    version="1.1.0",
     packages=find_namespace_packages(include=['cgsubmit', 'cgsubmit.*'], exclude=['*.tests*']),
     description="Analyse your submit in codingame competitions.",
     long_description=README_MD,
     long_description_content_type="text/markdown",
     url="https://github.com/FrequentlyMissedDeadlines/cgsubmit",
     author="FrequentlyMissedDeadlines",
     author_email="FrequentlyMissedDeadlines+cgsubmit@gmail.com",
```

