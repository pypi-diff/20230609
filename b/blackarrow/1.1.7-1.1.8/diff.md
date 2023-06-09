# Comparing `tmp/blackarrow-1.1.7.tar.gz` & `tmp/blackarrow-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blackarrow-1.1.7.tar", max compression
+gzip compressed data, was "blackarrow-1.1.8.tar", max compression
```

## Comparing `blackarrow-1.1.7.tar` & `blackarrow-1.1.8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1076 2023-05-24 04:30:00.135084 blackarrow-1.1.7/LICENSE.txt
--rw-r--r--   0        0        0     3222 2023-05-24 04:30:00.135084 blackarrow-1.1.7/README.md
--rw-r--r--   0        0        0     2853 2023-06-09 15:48:19.942829 blackarrow-1.1.7/blackarrow/__init__.py
--rwxr-xr-x   0        0        0     8228 2023-06-09 15:48:29.782830 blackarrow-1.1.7/blackarrow/blackarrow.py
--rw-r--r--   0        0        0        0 2023-05-24 04:30:00.135084 blackarrow-1.1.7/blackarrow/test/__init__.py
--rw-r--r--   0        0        0     1114 2023-05-24 04:30:00.135084 blackarrow-1.1.7/blackarrow/test/test_indexing.py
--rw-r--r--   0        0        0     1069 2023-06-09 15:49:22.042829 blackarrow-1.1.7/pyproject.toml
--rw-r--r--   0        0        0      104 2023-05-24 04:30:00.135084 blackarrow-1.1.7/sample/tester.txt
--rw-r--r--   0        0        0      104 2023-05-24 04:30:00.135084 blackarrow-1.1.7/sample/tester2.txt
--rw-r--r--   0        0        0     4141 1970-01-01 00:00:00.000000 blackarrow-1.1.7/setup.py
--rw-r--r--   0        0        0     4415 1970-01-01 00:00:00.000000 blackarrow-1.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-05-24 04:30:00.135084 blackarrow-1.1.8/LICENSE.txt
+-rw-r--r--   0        0        0     3222 2023-05-24 04:30:00.135084 blackarrow-1.1.8/README.md
+-rw-r--r--   0        0        0     2866 2023-06-09 15:50:33.042829 blackarrow-1.1.8/blackarrow/__init__.py
+-rwxr-xr-x   0        0        0     8241 2023-06-09 15:50:52.362829 blackarrow-1.1.8/blackarrow/blackarrow.py
+-rw-r--r--   0        0        0        0 2023-05-24 04:30:00.135084 blackarrow-1.1.8/blackarrow/test/__init__.py
+-rw-r--r--   0        0        0     1114 2023-05-24 04:30:00.135084 blackarrow-1.1.8/blackarrow/test/test_indexing.py
+-rw-r--r--   0        0        0     1069 2023-06-09 15:51:00.692829 blackarrow-1.1.8/pyproject.toml
+-rw-r--r--   0        0        0      104 2023-05-24 04:30:00.135084 blackarrow-1.1.8/sample/tester.txt
+-rw-r--r--   0        0        0      104 2023-05-24 04:30:00.135084 blackarrow-1.1.8/sample/tester2.txt
+-rw-r--r--   0        0        0     4141 1970-01-01 00:00:00.000000 blackarrow-1.1.8/setup.py
+-rw-r--r--   0        0        0     4415 1970-01-01 00:00:00.000000 blackarrow-1.1.8/PKG-INFO
```

### Comparing `blackarrow-1.1.7/LICENSE.txt` & `blackarrow-1.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blackarrow-1.1.7/README.md` & `blackarrow-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `blackarrow-1.1.7/blackarrow/__init__.py` & `blackarrow-1.1.8/blackarrow/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     processes, final_queue = ba.start_search(args)
     try:
         # This doesn't work as it is hanging on that queue for memory safety
         # print_process.join()  # Wait main thread until printer is done
 
         # need to instead listen to that queue and treat it as poison - like the others
         while True:
-            poison = final_queue.get(block=True)
+            poison = final_queue.get(block=True, timeout=500)
             if poison == 'EXIT':
                 break
 
     except (KeyboardInterrupt, EOFError):  # kill all on ctrl+c/d
         [p.terminate() for p in processes]
```

### Comparing `blackarrow-1.1.7/blackarrow/blackarrow.py` & `blackarrow-1.1.8/blackarrow/blackarrow.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,15 +185,15 @@
 ) -> None:
     file_count = 0
     found_count = 0
     exit_count = 0
     line_count = 0
     file_list = []
     while True:
-        statement = output.get(block=True)
+        statement = output.get(block=True, timeout=360)
         if statement[0][:4] == "EXIT":
             exit_count += 1
             line_count += statement[1]
             file_count += statement[2]
             found_count += statement[3]
 
             if DEVMODE:
```

### Comparing `blackarrow-1.1.7/blackarrow/test/test_indexing.py` & `blackarrow-1.1.8/blackarrow/test/test_indexing.py`

 * *Files identical despite different names*

### Comparing `blackarrow-1.1.7/pyproject.toml` & `blackarrow-1.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "blackarrow"
-version = "1.1.7"
+version = "1.1.8"
 description = "A fast keyword searcher"
 authors = ["Zoe Farmer <zoe@dataleek.io>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/TheDataLeek/black-arrow"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
```

### Comparing `blackarrow-1.1.7/setup.py` & `blackarrow-1.1.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['fabulous>=0.4.0,<0.5.0', 'faster-fifo>=1.4.5,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['ba = blackarrow:main', 'blackarrow = blackarrow:main']}
 
 setup_kwargs = {
     'name': 'blackarrow',
-    'version': '1.1.7',
+    'version': '1.1.8',
     'description': 'A fast keyword searcher',
     'long_description': '"Universal" Text Finder\n=======================\n\n[![Test Status](https://travis-ci.org/TheDataLeek/black-arrow.svg?branch=master)](https://travis-ci.org/TheDataLeek/black-arrow)\n[![Coverage Status](https://coveralls.io/repos/github/TheDataLeek/black-arrow/badge.svg?branch=master)](https://coveralls.io/github/TheDataLeek/black-arrow?branch=master)\n\nIt\'s basically just grep in python... Nothing fancy, just an easy extensible way\nto find things....\n\nYeah, I know, it\'s "reinventing the wheel" but ehhh, this is easier to extend to\ncover any and all weird cases without having to memorize a bunch of obscure\ncombinations of bash commands.\n\nThat out of the way, let\'s talk about what this *actually does*...\n\n## Quick Overview\n\nEssentially Black Arrow (or `ba` for short) is a way to search through every line in every file and\nfind matching keyword *or* regular expressions. It uses smart case, so if the search term is all\nlowercase it defaults to case-insensitive (mostly for ease of use).\n\n![png](./img/demo.png)\n\nYou can also supply it with regular expressions and it handles them natively.\n\n![png](./img/demo2.png)\n\nOther features include -\n\n* excluding certain files or paths,\n* replacing any matches that have been found,\n* specifying the max depth to search (good for large directory structures),\n* "pipe" mode for unix piping,\n* open the files in the `$EDITOR` for manual parsing. \n\n## Installation\n\n```\n┬─[zoe@fillory:~/Dropbox/Projects/black-arrow]─[09:22:12 PM]\n╰─>$ pip install --user blackarrow\n```\n\n## Black-Arrow Script\n\n```bash\n┬─[zoe@fillory:~/Dropbox/Projects/black-arrow]─[09:33:40 PM]\n╰─>$ ./black-arrow/blackarrow.py -h\nusage: ba [-h] [-d DIRECTORIES [DIRECTORIES ...]] [-i IGNORE [IGNORE ...]]\n          [-f FILENAME [FILENAME ...]] [-w WORKERS] [-p] [-e] [-l]\n          [-r REPLACE] [-D DEPTH] [--dev]\n          R\n\npositional arguments:\n  R                     Search term (regular expression)\n\noptional arguments:\n  -h, --help            show this help message and exit\n  -d DIRECTORIES [DIRECTORIES ...], --directories DIRECTORIES [DIRECTORIES ...]\n                        Director(y|ies) to run against\n  -i IGNORE [IGNORE ...], --ignore IGNORE [IGNORE ...]\n                        Things to ignore (regular expressions)\n  -f FILENAME [FILENAME ...], --filename FILENAME [FILENAME ...]\n                        Filename search term(s)\n  -w WORKERS, --workers WORKERS\n                        Number of workers to use (default numcores, with\n                        fallback 6 unless set)\n  -p, --pipe            Run in "pipe" mode with brief output\n  -e, --edit            Edit the files?\n  -l, --lower           Check strict lower case?\n  -r REPLACE, --replace REPLACE\n                        Replace text found in place with supplied\n  -D DEPTH, --depth DEPTH\n                        Directory depth to search in\n  --dev                 Run in development mode (NO OUTPUT)\n```\n\n#### The Name\n\n*"Arrow! Black arrow! I have saved you to the last. You have never failed me and\nI have always recovered you. I had you from my father and he from of old. If\never you came from the forges of the true king under the Mountain, go now and\nspeed well!"*\n\n― J.R.R. Tolkien, The Hobbit\n',
     'author': 'Zoe Farmer',
     'author_email': 'zoe@dataleek.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/TheDataLeek/black-arrow',
```

### Comparing `blackarrow-1.1.7/PKG-INFO` & `blackarrow-1.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blackarrow
-Version: 1.1.7
+Version: 1.1.8
 Summary: A fast keyword searcher
 Home-page: https://github.com/TheDataLeek/black-arrow
 License: MIT
 Keywords: development,searching,text,find,replace
 Author: Zoe Farmer
 Author-email: zoe@dataleek.io
 Requires-Python: >=3.6.2,<4.0.0
```

