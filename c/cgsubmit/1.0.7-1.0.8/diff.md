# Comparing `tmp/cgsubmit-1.0.7.tar.gz` & `tmp/cgsubmit-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cgsubmit-1.0.7.tar", last modified: Thu Jun  8 19:07:10 2023, max compression
+gzip compressed data, was "cgsubmit-1.0.8.tar", last modified: Thu Jun  8 19:18:43 2023, max compression
```

## Comparing `cgsubmit-1.0.7.tar` & `cgsubmit-1.0.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:07:10.588092 cgsubmit-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-08 19:06:54.000000 cgsubmit-1.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-06-08 19:07:10.588092 cgsubmit-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-06-08 19:06:54.000000 cgsubmit-1.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:07:10.584092 cgsubmit-1.0.7/cgsubmit/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-08 19:06:54.000000 cgsubmit-1.0.7/cgsubmit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-06-08 19:06:54.000000 cgsubmit-1.0.7/cgsubmit/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:07:10.584092 cgsubmit-1.0.7/cgsubmit/api/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-08 19:06:54.000000 cgsubmit-1.0.7/cgsubmit/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-08 19:06:54.000000 cgsubmit-1.0.7/cgsubmit/api/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:07:10.588092 cgsubmit-1.0.7/cgsubmit/games/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-08 19:06:54.000000 cgsubmit-1.0.7/cgsubmit/games/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-06-08 19:06:54.000000 cgsubmit-1.0.7/cgsubmit/games/games.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:07:10.584092 cgsubmit-1.0.7/cgsubmit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-06-08 19:07:10.000000 cgsubmit-1.0.7/cgsubmit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-08 19:07:10.000000 cgsubmit-1.0.7/cgsubmit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 19:07:10.000000 cgsubmit-1.0.7/cgsubmit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-08 19:07:10.000000 cgsubmit-1.0.7/cgsubmit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-08 19:07:10.000000 cgsubmit-1.0.7/cgsubmit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-08 19:06:54.000000 cgsubmit-1.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 19:07:10.588092 cgsubmit-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-08 19:06:54.000000 cgsubmit-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:18:43.319032 cgsubmit-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-08 19:18:27.000000 cgsubmit-1.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-06-08 19:18:43.319032 cgsubmit-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-06-08 19:18:27.000000 cgsubmit-1.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:18:43.319032 cgsubmit-1.0.8/cgsubmit/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-08 19:18:27.000000 cgsubmit-1.0.8/cgsubmit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-06-08 19:18:27.000000 cgsubmit-1.0.8/cgsubmit/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:18:43.319032 cgsubmit-1.0.8/cgsubmit/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-08 19:18:27.000000 cgsubmit-1.0.8/cgsubmit/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-08 19:18:27.000000 cgsubmit-1.0.8/cgsubmit/api/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:18:43.319032 cgsubmit-1.0.8/cgsubmit/games/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-08 19:18:27.000000 cgsubmit-1.0.8/cgsubmit/games/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-06-08 19:18:27.000000 cgsubmit-1.0.8/cgsubmit/games/games.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:18:43.319032 cgsubmit-1.0.8/cgsubmit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-06-08 19:18:43.000000 cgsubmit-1.0.8/cgsubmit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-08 19:18:43.000000 cgsubmit-1.0.8/cgsubmit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 19:18:43.000000 cgsubmit-1.0.8/cgsubmit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-08 19:18:43.000000 cgsubmit-1.0.8/cgsubmit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-08 19:18:43.000000 cgsubmit-1.0.8/cgsubmit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-08 19:18:27.000000 cgsubmit-1.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 19:18:43.319032 cgsubmit-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-08 19:18:27.000000 cgsubmit-1.0.8/setup.py
```

### Comparing `cgsubmit-1.0.7/LICENSE` & `cgsubmit-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `cgsubmit-1.0.7/PKG-INFO` & `cgsubmit-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cgsubmit
-Version: 1.0.7
+Version: 1.0.8
 Summary: Analyse your submit in codingame competitions.
 Home-page: https://github.com/FrequentlyMissedDeadlines/cgsubmit
 Author: FrequentlyMissedDeadlines
 Author-email: FrequentlyMissedDeadlines+cgsubmit@gmail.com
 Project-URL: Bug Reports, https://github.com/FrequentlyMissedDeadlines/cgsubmit/issues
 Project-URL: Source, https://github.com/FrequentlyMissedDeadlines/cgsubmit
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cgsubmit-1.0.7/README.md` & `cgsubmit-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `cgsubmit-1.0.7/cgsubmit/__main__.py` & `cgsubmit-1.0.8/cgsubmit/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,11 +33,11 @@
 
         print()
         for game in lost_games:
             print('➤ Lost game #{2} https://www.codingame.com/replay/{0} by {1} points'.format(game['gameId'], abs(game['scores'][0] - game['scores'][1]), games.number_by_id[game['gameId']]))
 
         
     except Exception as exception:
-        print(exception)
+        print(str(exception))
 
 if __name__ == '__main__':
 	main()
```

### Comparing `cgsubmit-1.0.7/cgsubmit/api/api.py` & `cgsubmit-1.0.8/cgsubmit/api/api.py`

 * *Files identical despite different names*

### Comparing `cgsubmit-1.0.7/cgsubmit/games/games.py` & `cgsubmit-1.0.8/cgsubmit/games/games.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
         for i in range(len(games)):
             number_by_id[games[i]['gameId']] = len(games) - i
         
         return number_by_id
     
     def get_win_and_lost(self, games, pseudo):
-        wins = [a for a in games if (a['players'][0]['nickname'] == pseudo and a['players'][0]['position'] == 0) or \
-                (len(a['players']) > 1 and a['players'][1]['nickname'] == pseudo and a['players'][1]['position'] == 0)]
+        wins = [a for a in games if ('nickname' in a['players'][0] and a['players'][0]['nickname'] == pseudo and a['players'][0]['position'] == 0) or \
+                (len(a['players']) > 1 and 'nickname' in a['players'][1] and a['players'][1]['nickname'] == pseudo and a['players'][1]['position'] == 0)]
         losts = [a['gameId'] for a in games if a not in wins]
         return (wins, losts)
     
     def get_timeouts(self, lost_games):
         self.timeouts = [a for a in lost_games if a['scores'][0] == -1 or a['scores'][1] == -1]
         return self.timeouts
```

### Comparing `cgsubmit-1.0.7/cgsubmit.egg-info/PKG-INFO` & `cgsubmit-1.0.8/cgsubmit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cgsubmit
-Version: 1.0.7
+Version: 1.0.8
 Summary: Analyse your submit in codingame competitions.
 Home-page: https://github.com/FrequentlyMissedDeadlines/cgsubmit
 Author: FrequentlyMissedDeadlines
 Author-email: FrequentlyMissedDeadlines+cgsubmit@gmail.com
 Project-URL: Bug Reports, https://github.com/FrequentlyMissedDeadlines/cgsubmit/issues
 Project-URL: Source, https://github.com/FrequentlyMissedDeadlines/cgsubmit
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cgsubmit-1.0.7/setup.py` & `cgsubmit-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 README_MD = open(join(dirname(abspath(__file__)), "README.md")).read()
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
     name="cgsubmit",
-    version="1.0.7",
+    version="1.0.8",
     packages=find_namespace_packages(include=['cgsubmit', 'cgsubmit.*'], exclude=['*.tests*']),
     description="Analyse your submit in codingame competitions.",
     long_description=README_MD,
     long_description_content_type="text/markdown",
     url="https://github.com/FrequentlyMissedDeadlines/cgsubmit",
     author="FrequentlyMissedDeadlines",
     author_email="FrequentlyMissedDeadlines+cgsubmit@gmail.com",
```

