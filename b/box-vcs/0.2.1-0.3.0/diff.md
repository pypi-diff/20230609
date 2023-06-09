# Comparing `tmp/box-vcs-0.2.1.tar.gz` & `tmp/box-vcs-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "box-vcs-0.2.1.tar", last modified: Tue May 23 01:02:47 2023, max compression
+gzip compressed data, was "box-vcs-0.3.0.tar", last modified: Fri Jun  9 20:09:29 2023, max compression
```

## Comparing `box-vcs-0.2.1.tar` & `box-vcs-0.3.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxr-x   0 pysproxy  (1000) pysproxy  (1000)        0 2023-05-23 01:02:47.239831 box-vcs-0.2.1/
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)    18092 2023-05-21 21:52:01.000000 box-vcs-0.2.1/LICENSE
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     2639 2023-05-23 01:02:47.235831 box-vcs-0.2.1/PKG-INFO
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     1935 2023-05-23 00:35:25.000000 box-vcs-0.2.1/README.md
-drwxrwxr-x   0 pysproxy  (1000) pysproxy  (1000)        0 2023-05-23 01:02:47.215831 box-vcs-0.2.1/box/
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)      783 2023-05-23 01:00:30.000000 box-vcs-0.2.1/box/__init__.py
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     9430 2023-05-23 00:59:04.000000 box-vcs-0.2.1/box/__main__.py
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)      649 2023-05-21 21:52:01.000000 box-vcs-0.2.1/box/_config.py
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     9031 2023-05-21 21:52:01.000000 box-vcs-0.2.1/box/commit.py
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     1097 2023-05-21 21:52:01.000000 box-vcs-0.2.1/box/exceptions.py
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     2128 2023-05-22 23:40:23.000000 box-vcs-0.2.1/box/ignore.py
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     3508 2023-05-21 21:52:01.000000 box-vcs-0.2.1/box/tracker.py
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     2074 2023-05-21 21:52:01.000000 box-vcs-0.2.1/box/utils.py
-drwxrwxr-x   0 pysproxy  (1000) pysproxy  (1000)        0 2023-05-23 01:02:47.231831 box-vcs-0.2.1/box_vcs.egg-info/
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     2639 2023-05-23 01:02:47.000000 box-vcs-0.2.1/box_vcs.egg-info/PKG-INFO
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)      353 2023-05-23 01:02:47.000000 box-vcs-0.2.1/box_vcs.egg-info/SOURCES.txt
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)        1 2023-05-23 01:02:47.000000 box-vcs-0.2.1/box_vcs.egg-info/dependency_links.txt
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)       42 2023-05-23 01:02:47.000000 box-vcs-0.2.1/box_vcs.egg-info/entry_points.txt
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)       15 2023-05-23 01:02:47.000000 box-vcs-0.2.1/box_vcs.egg-info/requires.txt
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)        4 2023-05-23 01:02:47.000000 box-vcs-0.2.1/box_vcs.egg-info/top_level.txt
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)       38 2023-05-23 01:02:47.239831 box-vcs-0.2.1/setup.cfg
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     1083 2023-05-23 00:34:50.000000 box-vcs-0.2.1/setup.py
-drwxrwxr-x   0 pysproxy  (1000) pysproxy  (1000)        0 2023-05-23 01:02:47.235831 box-vcs-0.2.1/tests/
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     7205 2023-05-21 21:52:01.000000 box-vcs-0.2.1/tests/test_box.py
+drwxrwxr-x   0 pysproxy  (1000) pysproxy  (1000)        0 2023-06-09 20:09:29.498686 box-vcs-0.3.0/
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)    18092 2023-06-09 16:57:41.000000 box-vcs-0.3.0/LICENSE
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     2727 2023-06-09 20:09:29.498686 box-vcs-0.3.0/PKG-INFO
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     2021 2023-06-09 19:54:50.000000 box-vcs-0.3.0/README.md
+drwxrwxr-x   0 pysproxy  (1000) pysproxy  (1000)        0 2023-06-09 20:09:29.462686 box-vcs-0.3.0/box/
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)      783 2023-06-09 19:52:18.000000 box-vcs-0.3.0/box/__init__.py
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     9595 2023-06-09 19:36:25.000000 box-vcs-0.3.0/box/__main__.py
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)      649 2023-06-09 16:57:41.000000 box-vcs-0.3.0/box/_config.py
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     9031 2023-06-09 18:53:22.000000 box-vcs-0.3.0/box/commit.py
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     1097 2023-06-09 16:57:41.000000 box-vcs-0.3.0/box/exceptions.py
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     1431 2023-06-09 18:30:21.000000 box-vcs-0.3.0/box/filter.py
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     2183 2023-06-09 19:26:21.000000 box-vcs-0.3.0/box/ignore.py
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     3508 2023-06-09 19:05:17.000000 box-vcs-0.3.0/box/tracker.py
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     2074 2023-06-09 16:57:41.000000 box-vcs-0.3.0/box/utils.py
+drwxrwxr-x   0 pysproxy  (1000) pysproxy  (1000)        0 2023-06-09 20:09:29.486686 box-vcs-0.3.0/box_vcs.egg-info/
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     2727 2023-06-09 20:09:29.000000 box-vcs-0.3.0/box_vcs.egg-info/PKG-INFO
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)      367 2023-06-09 20:09:29.000000 box-vcs-0.3.0/box_vcs.egg-info/SOURCES.txt
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)        1 2023-06-09 20:09:29.000000 box-vcs-0.3.0/box_vcs.egg-info/dependency_links.txt
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)       42 2023-06-09 20:09:29.000000 box-vcs-0.3.0/box_vcs.egg-info/entry_points.txt
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)       15 2023-06-09 20:09:29.000000 box-vcs-0.3.0/box_vcs.egg-info/requires.txt
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)        4 2023-06-09 20:09:29.000000 box-vcs-0.3.0/box_vcs.egg-info/top_level.txt
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)       38 2023-06-09 20:09:29.498686 box-vcs-0.3.0/setup.cfg
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     1085 2023-06-09 20:08:45.000000 box-vcs-0.3.0/setup.py
+drwxrwxr-x   0 pysproxy  (1000) pysproxy  (1000)        0 2023-06-09 20:09:29.494686 box-vcs-0.3.0/tests/
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     7205 2023-06-09 19:02:59.000000 box-vcs-0.3.0/tests/test_box.py
```

### Comparing `box-vcs-0.2.1/LICENSE` & `box-vcs-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `box-vcs-0.2.1/PKG-INFO` & `box-vcs-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: box-vcs
-Version: 0.2.1
-Summary: Simple and fast file versioning with Box
+Version: 0.3.0
+Summary: Fast, easy-to-use file versioning with Box
 Home-page: https://github.com/firlast/box
 Author: Firlast
 Author-email: firlastinc@gmail.com
 License: GNU GPLv2
 Keywords: version,control,versioning,vcs
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,15 +15,16 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Version Control
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">Box</h1>
-<p align="center">Fast and simple file versioning</p>
+<p align="center">Fast, easy-to-use file versioning.</p>
+<p align="center">Make the most of version control written entirely in Python.</p>
 
 <p align="center">
     <a href="https://github.com/firlast/box/releases">
         <img alt="GitHub release (latest by date including pre-releases)" src="https://img.shields.io/github/v/release/firlast/box?include_prereleases">
     </a>
     <a href="https://github.com/firlast/box/blob/master/LICENSE" style="margin-right: 5px; margin-left: 5px">
         <img alt="PyPI - License" src="https://img.shields.io/pypi/l/box-vcs">
```

#### html2text {}

```diff
@@ -1,19 +1,20 @@
-Metadata-Version: 2.1 Name: box-vcs Version: 0.2.1 Summary: Simple and fast
+Metadata-Version: 2.1 Name: box-vcs Version: 0.3.0 Summary: Fast, easy-to-use
 file versioning with Box Home-page: https://github.com/firlast/box Author:
 Firlast Author-email: firlastinc@gmail.com License: GNU GPLv2 Keywords:
 version,control,versioning,vcs Classifier: License :: OSI Approved :: GNU
 General Public License v2 (GPLv2) Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Natural Language :: English Classifier: Operating System :: Unix Classifier:
 Programming Language :: Python :: 3 Classifier: Topic :: Software Development
 :: Version Control Requires-Python: >=3.7 Description-Content-Type: text/
 markdown License-File: LICENSE
                                ****** Box ******
-                        Fast and simple file versioning
+                      Fast, easy-to-use file versioning.
+         Make the most of version control written entirely in Python.
    [GitHub_release_(latest_by_date_including_pre-releases)] [PyPI_-_License]
 Box is an open-source version control system **written in Python** that allows
 users to manage changes to their projects efficiently and collaboratively. With
 Box, you can control the history of **changes made to files**, track issues and
 bugs, and collaborate with other developers in a safe and secure environment.
 With an **intuitive interface** and customizable features, Box is a complete
 solution for development teams looking for an affordable and easy-to-use
```

### Comparing `box-vcs-0.2.1/README.md` & `box-vcs-0.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 <h1 align="center">Box</h1>
-<p align="center">Fast and simple file versioning</p>
+<p align="center">Fast, easy-to-use file versioning.</p>
+<p align="center">Make the most of version control written entirely in Python.</p>
 
 <p align="center">
     <a href="https://github.com/firlast/box/releases">
         <img alt="GitHub release (latest by date including pre-releases)" src="https://img.shields.io/github/v/release/firlast/box?include_prereleases">
     </a>
     <a href="https://github.com/firlast/box/blob/master/LICENSE" style="margin-right: 5px; margin-left: 5px">
         <img alt="PyPI - License" src="https://img.shields.io/pypi/l/box-vcs">
```

#### html2text {}

```diff
@@ -1,9 +1,10 @@
                                ****** Box ******
-                        Fast and simple file versioning
+                      Fast, easy-to-use file versioning.
+         Make the most of version control written entirely in Python.
    [GitHub_release_(latest_by_date_including_pre-releases)] [PyPI_-_License]
 Box is an open-source version control system **written in Python** that allows
 users to manage changes to their projects efficiently and collaboratively. With
 Box, you can control the history of **changes made to files**, track issues and
 bugs, and collaborate with other developers in a safe and secure environment.
 With an **intuitive interface** and customizable features, Box is a complete
 solution for development teams looking for an affordable and easy-to-use
```

### Comparing `box-vcs-0.2.1/box/__init__.py` & `box-vcs-0.3.0/box/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along
 # with this program; if not, write to the Free Software Foundation, Inc.,
 # 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 
-__version__ = '0.2.1'
+__version__ = '0.3.0'
```

### Comparing `box-vcs-0.2.1/box/__main__.py` & `box-vcs-0.3.0/box/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,21 +18,22 @@
 import sys
 import time
 from os import path, makedirs
 from typing import Union
 
 from argeasy import ArgEasy
 
-from .__init__ import __version__
-from .tracker import Tracker
-from .commit import Commit
-from .ignore import get_non_ignored
 from . import _config
 from . import exceptions
 from . import utils
+from .tracker import Tracker
+from .commit import Commit
+from .filter import Filter
+from .__init__ import __version__
+from .ignore import get_non_ignored
 
 REPO_PATH = '.box'
 OBJECTS_PATH = path.join(REPO_PATH, 'objects')
 
 tracker = Tracker()
 commit = Commit()
 
@@ -142,29 +143,23 @@
         print(f'Commit #\033[4m{commit_id[:7]}\033[m "{message}"')
         print(f'\033[33m{len(files)} files committed in {time.time() - time_s:.3f}s\033[m')
     except exceptions.NoFilesToCommitError:
         print('\033[1;31mNo files changed to commit\033[m')
         print('\033[33mYou can only commit changed and tracked files\033[m')
 
 
-def _log(filter_by_name: str = None, filter_by_email: str = None) -> None:
-    commits = commit.get_commits()
-    filtered_commits = []
+def _log(by_name: str = None, by_email: str = None, by_date: str = None) -> None:
+    _filter = Filter()
 
-    for cid, cdata in reversed(commits.items()):    
-        if filter_by_name:
-            if cdata['author'] == filter_by_name:
-                filtered_commits.append((cid, cdata))
-        elif filter_by_email:
-            if cdata['author_email'] == filter_by_email:
-                filtered_commits.append((cid, cdata))
-        else:
-            filtered_commits.append((cid, cdata))
+    commits = commit.get_commits()
+    commits = reversed(commits.items())
+    filtered_commits = _filter.filter(dict(commits), by_name=by_name,
+                                      by_email=by_email, by_date=by_date)
 
-    for cid, cdata in filtered_commits:
+    for cid, cdata in filtered_commits.items():
         author_email = cdata['author_email']
         files = len(cdata['objects'])
         message = cdata['message']
         author = cdata['author']
         date = cdata['date']
 
         print(f'{files} file(s) in \033[34;4m{cid[:7]}\033[m by {author} <{author_email}> '
@@ -225,14 +220,15 @@
     parser.add_flag('-am', 'Commit all changed files add insert a message')
     parser.add_flag('-m', 'A short message to commit')
 
     parser.add_flag('--name', 'Set author name')
     parser.add_flag('--email', 'Set author email')
 
     parser.add_flag('--filter-by-name', 'Filter log commit by author name')
+    parser.add_flag('--filter-by-date', 'Filter log commit by commit date')
     parser.add_flag('--filter-by-email', 'Filter log commit by author email')
 
     args = parser.parse()
 
     if not path.isdir(OBJECTS_PATH) and not any((args.init, args.config)):
         print('\033[1;31mRepository not found\033[m')
         print('\033[33mCreate a repository with "init" command\033[m')
@@ -244,17 +240,20 @@
         if args.a:
             _add('*')
         else:
             _add(args.add)
     elif args.status:
         _status()
     elif args.log:
-        _log(args.filter_by_name, args.filter_by_email)
+        _log(args.filter_by_name, args.filter_by_email, args.filter_by_date)
     elif args.commit is not None:
-        if args.am:
+        if args.am and len(args.commit) > 0:
+            print(f'\033[1;31mThe "commit" command must not contain arguments when "-am" is present.\033[m')
+            print('\033[33mUse "commit <filename> -m" or "commit -am"\033[m')
+        elif args.am:
             _commit('*', args.am)
         else:
             _commit(args.commit, args.m)
     elif args.diff:
         _diff()
     elif args.integrity:
         _integrity()
```

### Comparing `box-vcs-0.2.1/box/_config.py` & `box-vcs-0.3.0/box/_config.py`

 * *Files identical despite different names*

### Comparing `box-vcs-0.2.1/box/commit.py` & `box-vcs-0.3.0/box/commit.py`

 * *Files identical despite different names*

### Comparing `box-vcs-0.2.1/box/exceptions.py` & `box-vcs-0.3.0/box/exceptions.py`

 * *Files identical despite different names*

### Comparing `box-vcs-0.2.1/box/ignore.py` & `box-vcs-0.3.0/box/ignore.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     try:
         with open('.ignore', 'r') as ignore_file:
             filelist = ignore_file.readlines()
     except FileNotFoundError:
         ignored = []
     else:
         filelist = [file.replace('\n', '') for file in filelist]
+        filelist = [file for file in filelist if file]
         ignored = list(map(_filter_filelist, filelist))
 
     ignored.append('.box')
     return ignored
 
 
 def get_non_ignored() -> list:
```

### Comparing `box-vcs-0.2.1/box/tracker.py` & `box-vcs-0.3.0/box/tracker.py`

 * *Files identical despite different names*

### Comparing `box-vcs-0.2.1/box/utils.py` & `box-vcs-0.3.0/box/utils.py`

 * *Files identical despite different names*

### Comparing `box-vcs-0.2.1/box_vcs.egg-info/PKG-INFO` & `box-vcs-0.3.0/box_vcs.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: box-vcs
-Version: 0.2.1
-Summary: Simple and fast file versioning with Box
+Version: 0.3.0
+Summary: Fast, easy-to-use file versioning with Box
 Home-page: https://github.com/firlast/box
 Author: Firlast
 Author-email: firlastinc@gmail.com
 License: GNU GPLv2
 Keywords: version,control,versioning,vcs
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,15 +15,16 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Version Control
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">Box</h1>
-<p align="center">Fast and simple file versioning</p>
+<p align="center">Fast, easy-to-use file versioning.</p>
+<p align="center">Make the most of version control written entirely in Python.</p>
 
 <p align="center">
     <a href="https://github.com/firlast/box/releases">
         <img alt="GitHub release (latest by date including pre-releases)" src="https://img.shields.io/github/v/release/firlast/box?include_prereleases">
     </a>
     <a href="https://github.com/firlast/box/blob/master/LICENSE" style="margin-right: 5px; margin-left: 5px">
         <img alt="PyPI - License" src="https://img.shields.io/pypi/l/box-vcs">
```

#### html2text {}

```diff
@@ -1,19 +1,20 @@
-Metadata-Version: 2.1 Name: box-vcs Version: 0.2.1 Summary: Simple and fast
+Metadata-Version: 2.1 Name: box-vcs Version: 0.3.0 Summary: Fast, easy-to-use
 file versioning with Box Home-page: https://github.com/firlast/box Author:
 Firlast Author-email: firlastinc@gmail.com License: GNU GPLv2 Keywords:
 version,control,versioning,vcs Classifier: License :: OSI Approved :: GNU
 General Public License v2 (GPLv2) Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Natural Language :: English Classifier: Operating System :: Unix Classifier:
 Programming Language :: Python :: 3 Classifier: Topic :: Software Development
 :: Version Control Requires-Python: >=3.7 Description-Content-Type: text/
 markdown License-File: LICENSE
                                ****** Box ******
-                        Fast and simple file versioning
+                      Fast, easy-to-use file versioning.
+         Make the most of version control written entirely in Python.
    [GitHub_release_(latest_by_date_including_pre-releases)] [PyPI_-_License]
 Box is an open-source version control system **written in Python** that allows
 users to manage changes to their projects efficiently and collaboratively. With
 Box, you can control the history of **changes made to files**, track issues and
 bugs, and collaborate with other developers in a safe and secure environment.
 With an **intuitive interface** and customizable features, Box is a complete
 solution for development teams looking for an affordable and easy-to-use
```

### Comparing `box-vcs-0.2.1/setup.py` & `box-vcs-0.3.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 with open('README.md') as file:
     readme = file.read()
 
 setup(
     author='Firlast',
     author_email='firlastinc@gmail.com',
     name='box-vcs',
-    description='Simple and fast file versioning with Box',
+    description='Fast, easy-to-use file versioning with Box',
     version=__version__,
     packages=['box'],
     url='https://github.com/firlast/box',
     long_description=readme,
     long_description_content_type='text/markdown',
     license='GNU GPLv2',
     python_requires='>=3.7',
-    install_requires=['argeasy==3.0.0'],
+    install_requires=['argeasy==3.1.0'],
     entry_points={
         'console_scripts': [
             'box = box.__main__:main'
         ]
     },
     keywords=['version', 'control', 'versioning', 'vcs'],
     classifiers=[
```

### Comparing `box-vcs-0.2.1/tests/test_box.py` & `box-vcs-0.3.0/tests/test_box.py`

 * *Files identical despite different names*

