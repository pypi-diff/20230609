# Comparing `tmp/crocodile-8.40.tar.gz` & `tmp/crocodile-9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crocodile-8.40.tar", last modified: Wed Jan 11 20:56:25 2023, max compression
+gzip compressed data, was "crocodile-9.0.tar", last modified: Fri Jan 13 00:38:31 2023, max compression
```

## Comparing `crocodile-8.40.tar` & `crocodile-9.0.tar`

### file list

```diff
@@ -1,46 +1,54 @@
-drwxrwxrwx   0        0        0        0 2023-01-11 20:56:25.604603 crocodile-8.40/
--rw-rw-rw-   0        0        0      156 2022-12-26 10:51:14.000000 crocodile-8.40/MANIFEST.in
--rw-rw-rw-   0        0        0     7850 2023-01-11 20:56:25.604603 crocodile-8.40/PKG-INFO
--rw-rw-rw-   0        0        0     7243 2022-12-26 10:51:14.000000 crocodile-8.40/README.md
--rw-rw-rw-   0        0        0    11556 2022-12-26 10:51:14.000000 crocodile-8.40/license.txt
-drwxrwxrwx   0        0        0        0 2023-01-11 20:56:25.401614 crocodile-8.40/myresources/
-drwxrwxrwx   0        0        0        0 2023-01-11 20:56:25.525859 crocodile-8.40/myresources/crocodile/
--rw-rw-rw-   0        0        0      434 2023-01-11 20:56:10.000000 crocodile-8.40/myresources/crocodile/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-11 20:56:25.407634 crocodile-8.40/myresources/crocodile/cluster/
-drwxrwxrwx   0        0        0        0 2023-01-11 20:56:25.573931 crocodile-8.40/myresources/crocodile/cluster/__pycache__/
--rw-rw-rw-   0        0        0      161 2022-12-26 11:33:08.000000 crocodile-8.40/myresources/crocodile/cluster/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     4519 2023-01-10 07:14:53.000000 crocodile-8.40/myresources/crocodile/cluster/__pycache__/data_transfer.cpython-39.pyc
--rw-rw-rw-   0        0        0     6145 2023-01-02 09:12:18.000000 crocodile-8.40/myresources/crocodile/cluster/__pycache__/distribute.cpython-39.pyc
--rw-rw-rw-   0        0        0     1964 2023-01-04 09:23:20.000000 crocodile-8.40/myresources/crocodile/cluster/__pycache__/meta_handling.cpython-39.pyc
--rw-rw-rw-   0        0        0    10044 2023-01-10 07:13:30.000000 crocodile-8.40/myresources/crocodile/cluster/__pycache__/remote_machine.cpython-39.pyc
--rw-rw-rw-   0        0        0     1406 2023-01-04 09:47:01.000000 crocodile-8.40/myresources/crocodile/cluster/__pycache__/trial_file.cpython-39.pyc
-drwxrwxrwx   0        0        0        0 2023-01-11 20:56:25.407634 crocodile-8.40/myresources/crocodile/comms/
-drwxrwxrwx   0        0        0        0 2023-01-11 20:56:25.590682 crocodile-8.40/myresources/crocodile/comms/__pycache__/
--rw-rw-rw-   0        0        0      396 2022-12-29 04:22:01.000000 crocodile-8.40/myresources/crocodile/comms/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0      875 2022-12-29 04:22:01.000000 crocodile-8.40/myresources/crocodile/comms/__pycache__/helper_funcs.cpython-39.pyc
--rw-rw-rw-   0        0        0    24760 2023-01-09 04:47:52.000000 crocodile-8.40/myresources/crocodile/core.py
--rw-rw-rw-   0        0        0     2093 2023-01-07 21:29:02.000000 crocodile-8.40/myresources/crocodile/croshell.py
--rw-rw-rw-   0        0        0     6017 2022-12-30 00:56:40.000000 crocodile-8.40/myresources/crocodile/database.py
--rw-rw-rw-   0        0        0    42342 2023-01-04 10:12:36.000000 crocodile-8.40/myresources/crocodile/deeplearning.py
--rw-rw-rw-   0        0        0    10151 2022-12-26 10:51:14.000000 crocodile-8.40/myresources/crocodile/deeplearning_torch.py
--rw-rw-rw-   0        0        0    11194 2023-01-01 03:41:45.000000 crocodile-8.40/myresources/crocodile/environment.py
--rw-rw-rw-   0        0        0    48732 2023-01-08 22:54:30.000000 crocodile-8.40/myresources/crocodile/file_management.py
--rw-rw-rw-   0        0        0    39143 2022-12-26 10:51:14.000000 crocodile-8.40/myresources/crocodile/matplotlib_management.py
--rw-rw-rw-   0        0        0    39895 2023-01-11 20:47:27.000000 crocodile-8.40/myresources/crocodile/meta.py
-drwxrwxrwx   0        0        0        0 2023-01-11 20:56:25.410033 crocodile-8.40/myresources/crocodile/msc/
-drwxrwxrwx   0        0        0        0 2023-01-11 20:56:25.595590 crocodile-8.40/myresources/crocodile/msc/__pycache__/
--rw-rw-rw-   0        0        0      175 2023-01-11 08:58:35.000000 crocodile-8.40/myresources/crocodile/msc/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0      157 2022-12-26 10:51:21.000000 crocodile-8.40/myresources/crocodile/msc/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0    13761 2023-01-11 08:58:35.000000 crocodile-8.40/myresources/crocodile/msc/__pycache__/odds.cpython-311.pyc
--rw-rw-rw-   0        0        0     7111 2022-12-27 04:25:39.000000 crocodile-8.40/myresources/crocodile/msc/__pycache__/odds.cpython-39.pyc
--rw-rw-rw-   0        0        0     2403 2022-12-26 10:51:14.000000 crocodile-8.40/myresources/crocodile/plotly_management.py
--rw-rw-rw-   0        0        0     4593 2023-01-11 20:51:32.000000 crocodile-8.40/myresources/crocodile/run.py
--rw-rw-rw-   0        0        0     2031 2022-12-26 10:51:14.000000 crocodile-8.40/myresources/crocodile/toolbox.py
-drwxrwxrwx   0        0        0        0 2023-01-11 20:56:25.557261 crocodile-8.40/myresources/crocodile.egg-info/
--rw-rw-rw-   0        0        0     7850 2023-01-11 20:56:25.000000 crocodile-8.40/myresources/crocodile.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1540 2023-01-11 20:56:25.000000 crocodile-8.40/myresources/crocodile.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-11 20:56:25.000000 crocodile-8.40/myresources/crocodile.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      122 2023-01-11 20:56:25.000000 crocodile-8.40/myresources/crocodile.egg-info/requires.txt
--rw-rw-rw-   0        0        0       76 2023-01-11 20:56:25.000000 crocodile-8.40/myresources/crocodile.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-01-11 20:56:25.606118 crocodile-8.40/setup.cfg
--rw-rw-rw-   0        0        0     2988 2022-12-26 10:51:14.000000 crocodile-8.40/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 00:38:31.260007 crocodile-9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-01-13 00:38:21.000000 crocodile-9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7727 2023-01-13 00:38:31.260007 crocodile-9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7143 2023-01-13 00:38:21.000000 crocodile-9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 00:38:31.256007 crocodile-9.0/myresources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 00:38:31.256007 crocodile-9.0/myresources/crocodile/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-01-13 00:38:21.000000 crocodile-9.0/myresources/crocodile/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 00:38:31.256007 crocodile-9.0/myresources/crocodile/art/
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-01-13 00:38:21.000000 crocodile-9.0/myresources/crocodile/art/croco_caliography_2
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-01-13 00:38:21.000000 crocodile-9.0/myresources/crocodile/art/fat_croco
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-01-13 00:38:21.000000 crocodile-9.0/myresources/crocodile/art/halfwit_croco
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-01-13 00:38:21.000000 crocodile-9.0/myresources/crocodile/art/happy_croco
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-01-13 00:38:21.000000 crocodile-9.0/myresources/crocodile/art/water_croco
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 00:38:31.260007 crocodile-9.0/myresources/crocodile/cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-13 00:38:21.000000 crocodile-9.0/myresources/crocodile/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-01-13 00:38:21.000000 crocodile-9.0/myresources/crocodile/cluster/data_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-01-13 00:38:21.000000 crocodile-9.0/myresources/crocodile/cluster/distribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-01-13 00:38:21.000000 crocodile-9.0/myresources/crocodile/cluster/meta_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16622 2023-01-13 00:38:21.000000 crocodile-9.0/myresources/crocodile/cluster/remote_machine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-01-13 00:38:21.000000 crocodile-9.0/myresources/crocodile/cluster/script_execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-01-13 00:38:21.000000 crocodile-9.0/myresources/crocodile/cluster/script_notify_upon_completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-01-13 00:38:21.000000 crocodile-9.0/myresources/crocodile/cluster/trial_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 00:38:31.260007 crocodile-9.0/myresources/crocodile/comms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-13 00:38:21.000000 crocodile-9.0/myresources/crocodile/comms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12635 2023-01-13 00:38:21.000000 crocodile-9.0/myresources/crocodile/comms/gdrive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-01-13 00:38:21.000000 crocodile-9.0/myresources/crocodile/comms/helper_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-01-13 00:38:21.000000 crocodile-9.0/myresources/crocodile/comms/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6358 2023-01-13 00:38:21.000000 crocodile-9.0/myresources/crocodile/comms/onedrive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24791 2023-01-13 00:38:21.000000 crocodile-9.0/myresources/crocodile/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-01-13 00:38:21.000000 crocodile-9.0/myresources/crocodile/croshell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-01-13 00:38:21.000000 crocodile-9.0/myresources/crocodile/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41572 2023-01-13 00:38:21.000000 crocodile-9.0/myresources/crocodile/deeplearning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9889 2023-01-13 00:38:21.000000 crocodile-9.0/myresources/crocodile/deeplearning_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10983 2023-01-13 00:38:21.000000 crocodile-9.0/myresources/crocodile/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48331 2023-01-13 00:38:21.000000 crocodile-9.0/myresources/crocodile/file_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38698 2023-01-13 00:38:21.000000 crocodile-9.0/myresources/crocodile/matplotlib_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39620 2023-01-13 00:38:21.000000 crocodile-9.0/myresources/crocodile/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 00:38:31.260007 crocodile-9.0/myresources/crocodile/msc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-13 00:38:21.000000 crocodile-9.0/myresources/crocodile/msc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-01-13 00:38:21.000000 crocodile-9.0/myresources/crocodile/msc/ascii_art.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-01-13 00:38:21.000000 crocodile-9.0/myresources/crocodile/msc/dl_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-01-13 00:38:21.000000 crocodile-9.0/myresources/crocodile/msc/numerical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-01-13 00:38:21.000000 crocodile-9.0/myresources/crocodile/msc/odds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-01-13 00:38:21.000000 crocodile-9.0/myresources/crocodile/plotly_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-01-13 00:38:21.000000 crocodile-9.0/myresources/crocodile/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-01-13 00:38:21.000000 crocodile-9.0/myresources/crocodile/toolbox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 00:38:31.260007 crocodile-9.0/myresources/crocodile.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7727 2023-01-13 00:38:31.000000 crocodile-9.0/myresources/crocodile.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-01-13 00:38:31.000000 crocodile-9.0/myresources/crocodile.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-13 00:38:31.000000 crocodile-9.0/myresources/crocodile.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-01-13 00:38:31.000000 crocodile-9.0/myresources/crocodile.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-01-13 00:38:31.000000 crocodile-9.0/myresources/crocodile.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-13 00:38:31.260007 crocodile-9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-01-13 00:38:21.000000 crocodile-9.0/setup.py
```

### Comparing `crocodile-8.40/PKG-INFO` & `crocodile-9.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,116 +1,118 @@
-Metadata-Version: 2.1
-Name: crocodile
-Version: 8.40
-Summary: Making Python even more convenient by extending list and dict and pathlib and more.
-Home-page: https://github.com/thisismygitrepo/crocodile
-Author: Alex Al-Saffar
-Author-email: programmer@usa.com
-License: Apache 2.0
-Project-URL: Bug Tracker, https://github.com/thisismygitrepo/crocodile/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: license.txt
-
-
-# Welcome to crocodile
-
-Crocodile is a library aiming at facilitating the use of Python in scripting, thus, offering an alternative to `PowerShell` & `Bash` which have absurdly complex commands that are nothing but jumble of ad-hoc developments piled over decades to save some programmers a key stroke or two. This heritage poses huge burden on the people coming into the computer science field. A full rant bashing those shells by `Brian Will` [is here](<https://www.youtube.com/watch?v=L9v4Mg8wi4U`>).
-
-The core rationale is:
-* No one has the time to listen to hours long tutorials on how powerful and versatile `ls` or `grep` are, let alone keeping the random syntax in mind (unless used on daily basis). 
-* Python shell on the other hand, offers benign syntax and eminent readibility but it comes at the rather hefty cost of terseness, or the lack of it. For example, to make up for just `ls`, you need to import some libraries and it will eventually set you back a couple of lines of code. That's not acceptable for the simple task of listing directory contents, let alone a task of compressing a directory.
-* Crocodile comes here to make Python terser and friendlier by offering functionality for everyday use, like **file management, SSH, enviroment variables management, etc**. In essence, croshell to IPython is what IPython to Python shell is; that is, the basic Python shell that can only do arithmetic is turbo-boosted making it perfect for everyday errands.
-* The library, if used in coding, will fill your life with one-liners, take your code to artistic level of brevity and readability while simultaneously being more productive by typing less boilerplate lines of code that are needless to say.
-
-The name `crocodile` signifies the use of brute force in its implementation. The focus is on ease of use, as oppoesd to beating the existing shells in speed.
-Mind you, speed is not an issue in 99% of everyday chores.
-`Crocodile` designed carefully to be loved, learning curve cound't be flattened further.
-
-This package extends many native Python classes to equip you with an uneasy-to-tame power. The major classes extended are:
-
- * `pathlib.Path` is  extended to `P`
-      * Forget about importing all the **archaic** Python libraries `os`, `glob`, `shutil`, `sys`, `zipfile` etc. `P` makes the path an object, not a lame string. `P` objects are incredibly powerful for parsing paths, *no* more than one line of code is required to do **any** operation. Take a squint at this:
-      ```
-   path = P("dataset/type1/meta/images/file3.ext")
-     >> path[0]  # allows indexing! makes sense, hah?
-      P("dataset")
-     >> path[-1]  # nifty!
-      P("file3.ext")
-     >> path[2:-1]  # even slicing!
-      P("meta/images/file3.ext")
-   ```
- * `list` is  extended to `List`
-   * Forget that `for` loops exist, because with this class, `for` loops are implicitly used to apply a function to all items.
-     Inevitably while programming, one will encounter objects of the same type and you will be struggling to get a tough grab on them.  `List` is a powerful structure that put at your disposal a grip, so tough, that the objects you have at hand start behaving like one object. Behaviour is ala-JavaScript implementation of ``forEach`` method of Arrays.
-
- * `dict` is  extended to `Struct`.
-     * Combines the power of dot notation like classes and key access like dictionaries.
-
- * Additionally, the package provides many other new classes, e.g. `Read` and `Save`. Together with `P`, they provide comprehensive support for file management. Life cannot get easier with those. Every class inherits attributes that allow saving and loading in one line.
-
-   
-Furthermore, those classes are inextricably connected. For example, globbing a path `P` object returns a `List` object. You can move back and forth between `List` and `Struct` and `DataFrame` with one method, and so on.
-
-* Deep Learning Modules.
-  * A paradigm that facilitates working with deep learning models that is based on a tri-partite scheme:
-    * HyperParameters: facilitated through `HParams` class.
-    * Data: facilitated though `DataReader` class.
-    * `BaseModel` is a frontend for both `TensorFlow` & `Pytorch` backends. The wrapper worked in tandem.
-  * The aforementioned classes cooperate together to offer sealmess workflow during creation, training, and saving models.
-
-
-# Install
-In the commandline:
-`pip install crocodile`.
-
-Being a thin extension on top of almost pure Python, you need to worry **not** about your venv, the package is not aggressive in requirements, it installs itself peacefully, never interfere with your other packages. If you do not have `numpy`, `matplotlib` and `pandas`, it simply throws `ImportError` at runtime, that's it.
-
-[comment]: # (The package is not fussy about versions either. It can though at runtime, install packages on the fly, e.g. `dill` and `tqdm` which are very lightweight libraries.)
-
-# Install Croshell Terminal
-For `Windows` machines, run the following in elevated `PowerShell`:
-```ps1
-Invoke-WebRequest https://github.com/thisismygitrepo/machineconfig/src/machineconfig/setup_windows/croshell.ps1 | Invoke-Expression
-```
-
-# Getting Started
-That's as easy as taking candy from a baby; whenever you start a Python file, preface it with following in order to unleash the library:
-
-```
-import crocodile.toolbox as tb
-```
-
-
-# A Taste of Power
-EX1: Get a list of `.exe` available in terminal.
-
-     P.env().Path.search('*.exe').reduce(lambda x, y: x+y).print()
-
-EX2: Suppose you want to know how many lines of code in your repository. The procedure is to glob all `.py` files recursively, read string code, split each one of them by lines, count the lines, add up everything from all strings of code.
-
-
-To achieve this, all you need is an eminently readable one-liner.
-```
-tb.P.cwd().search("*.py", r=True).read_text().split('\n').apply(len).to_numpy().sum()
-```
-
-How does this make perfect sense?
-* `search` returns `List` of `P` path objects
-* `read_text` is a `P` method, but it is being run against `List` object. Behind the scenes, **responsible black magic** fails to find such a method in `List` and realizes it is a method of items inside the list, so it runs it against them and thus read all files and containerize them in another `List` object and returns it.
-* A similar story applies to `split` which is a method of strings in Python.
-* Next, `apply` is a method of `List`. Sure enough, it lives up to its apt name and applies the passed function `len` to all items in the list and returns another `List` object that contains the results.
-* `.to_numpy()` converts `List` to `numpy` array, then `.sum` is a method of `numpy`, which gives the final result.
-
-Methods naming convention like `apply` and `to_numpy` are inspired from the popular `pandas` library, resulting in almost non-existing learning curve.
-
-# Friendly interactive tutorial.
-Please refer to [Here](<https://github.com/thisismygitrepo/crocodile/blob/master/tutorial.ipynb>) on the main git repo.
-
-# Full docs:
-Click [Here](<https://crocodile.readthedocs.io/en/latest/>)
-
-# Author
-Alex Al-Saffar. [email](mailto:programmer@usa.com)
+Metadata-Version: 2.1
+Name: crocodile
+Version: 9.0
+Summary: Making Python even more convenient by extending list and dict and pathlib and more.
+Home-page: https://github.com/thisismygitrepo/crocodile
+Author: Alex Al-Saffar
+Author-email: programmer@usa.com
+License: Apache 2.0
+Project-URL: Bug Tracker, https://github.com/thisismygitrepo/crocodile/issues
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
+
+# Welcome to crocodile
+
+Crocodile is a library aiming at facilitating the use of Python in scripting, thus, offering an alternative to `PowerShell` & `Bash` which have absurdly complex commands that are nothing but jumble of ad-hoc developments piled over decades to save some programmers a key stroke or two. This heritage poses huge burden on the people coming into the computer science field. A full rant bashing those shells by `Brian Will` [is here](<https://www.youtube.com/watch?v=L9v4Mg8wi4U`>).
+
+The core rationale is:
+* No one has the time to listen to hours long tutorials on how powerful and versatile `ls` or `grep` are, let alone keeping the random syntax in mind (unless used on daily basis). 
+* Python shell on the other hand, offers benign syntax and eminent readibility but it comes at the rather hefty cost of terseness, or the lack of it. For example, to make up for just `ls`, you need to import some libraries and it will eventually set you back a couple of lines of code. That's not acceptable for the simple task of listing directory contents, let alone a task of compressing a directory.
+* Crocodile comes here to make Python terser and friendlier by offering functionality for everyday use, like **file management, SSH, enviroment variables management, etc**. In essence, croshell to IPython is what IPython to Python shell is; that is, the basic Python shell that can only do arithmetic is turbo-boosted making it perfect for everyday errands.
+* The library, if used in coding, will fill your life with one-liners, take your code to artistic level of brevity and readability while simultaneously being more productive by typing less boilerplate lines of code that are needless to say.
+
+The name `crocodile` signifies the use of brute force in its implementation. The focus is on ease of use, as oppoesd to beating the existing shells in speed.
+Mind you, speed is not an issue in 99% of everyday chores.
+`Crocodile` designed carefully to be loved, learning curve cound't be flattened further.
+
+This package extends many native Python classes to equip you with an uneasy-to-tame power. The major classes extended are:
+
+ * `pathlib.Path` is  extended to `P`
+      * Forget about importing all the **archaic** Python libraries `os`, `glob`, `shutil`, `sys`, `zipfile` etc. `P` makes the path an object, not a lame string. `P` objects are incredibly powerful for parsing paths, *no* more than one line of code is required to do **any** operation. Take a squint at this:
+      ```
+   path = P("dataset/type1/meta/images/file3.ext")
+     >> path[0]  # allows indexing! makes sense, hah?
+      P("dataset")
+     >> path[-1]  # nifty!
+      P("file3.ext")
+     >> path[2:-1]  # even slicing!
+      P("meta/images/file3.ext")
+   ```
+ * `list` is  extended to `List`
+   * Forget that `for` loops exist, because with this class, `for` loops are implicitly used to apply a function to all items.
+     Inevitably while programming, one will encounter objects of the same type and you will be struggling to get a tough grab on them.  `List` is a powerful structure that put at your disposal a grip, so tough, that the objects you have at hand start behaving like one object. Behaviour is ala-JavaScript implementation of ``forEach`` method of Arrays.
+
+ * `dict` is  extended to `Struct`.
+     * Combines the power of dot notation like classes and key access like dictionaries.
+
+ * Additionally, the package provides many other new classes, e.g. `Read` and `Save`. Together with `P`, they provide comprehensive support for file management. Life cannot get easier with those. Every class inherits attributes that allow saving and loading in one line.
+
+   
+Furthermore, those classes are inextricably connected. For example, globbing a path `P` object returns a `List` object. You can move back and forth between `List` and `Struct` and `DataFrame` with one method, and so on.
+
+* Deep Learning Modules.
+  * A paradigm that facilitates working with deep learning models that is based on a tri-partite scheme:
+    * HyperParameters: facilitated through `HParams` class.
+    * Data: facilitated though `DataReader` class.
+    * `BaseModel` is a frontend for both `TensorFlow` & `Pytorch` backends. The wrapper worked in tandem.
+  * The aforementioned classes cooperate together to offer sealmess workflow during creation, training, and saving models.
+
+
+# Install
+In the commandline:
+`pip install crocodile`.
+
+Being a thin extension on top of almost pure Python, you need to worry **not** about your venv, the package is not aggressive in requirements, it installs itself peacefully, never interfere with your other packages. If you do not have `numpy`, `matplotlib` and `pandas`, it simply throws `ImportError` at runtime, that's it.
+
+[comment]: # (The package is not fussy about versions either. It can though at runtime, install packages on the fly, e.g. `dill` and `tqdm` which are very lightweight libraries.)
+
+# Install Croshell Terminal
+For `Windows` machines, run the following in elevated `PowerShell`:
+```ps1
+Invoke-WebRequest https://github.com/thisismygitrepo/machineconfig/src/machineconfig/setup_windows/croshell.ps1 | Invoke-Expression
+```
+
+# Getting Started
+That's as easy as taking candy from a baby; whenever you start a Python file, preface it with following in order to unleash the library:
+
+```
+import crocodile.toolbox as tb
+```
+
+
+# A Taste of Power
+EX1: Get a list of `.exe` available in terminal.
+
+     P.env().Path.search('*.exe').reduce(lambda x, y: x+y).print()
+
+EX2: Suppose you want to know how many lines of code in your repository. The procedure is to glob all `.py` files recursively, read string code, split each one of them by lines, count the lines, add up everything from all strings of code.
+
+
+To achieve this, all you need is an eminently readable one-liner.
+```
+tb.P.cwd().search("*.py", r=True).read_text().split('\n').apply(len).to_numpy().sum()
+```
+
+How does this make perfect sense?
+* `search` returns `List` of `P` path objects
+* `read_text` is a `P` method, but it is being run against `List` object. Behind the scenes, **responsible black magic** fails to find such a method in `List` and realizes it is a method of items inside the list, so it runs it against them and thus read all files and containerize them in another `List` object and returns it.
+* A similar story applies to `split` which is a method of strings in Python.
+* Next, `apply` is a method of `List`. Sure enough, it lives up to its apt name and applies the passed function `len` to all items in the list and returns another `List` object that contains the results.
+* `.to_numpy()` converts `List` to `numpy` array, then `.sum` is a method of `numpy`, which gives the final result.
+
+Methods naming convention like `apply` and `to_numpy` are inspired from the popular `pandas` library, resulting in almost non-existing learning curve.
+
+# Friendly interactive tutorial.
+Please refer to [Here](<https://github.com/thisismygitrepo/crocodile/blob/master/tutorial.ipynb>) on the main git repo.
+
+# Full docs:
+Click [Here](<https://crocodile.readthedocs.io/en/latest/>)
+
+# Author
+Alex Al-Saffar. [email](mailto:programmer@usa.com)
+
+
```

### Comparing `crocodile-8.40/README.md` & `crocodile-9.0/README.md`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,100 +1,100 @@
-
-# Welcome to crocodile
-
-Crocodile is a library aiming at facilitating the use of Python in scripting, thus, offering an alternative to `PowerShell` & `Bash` which have absurdly complex commands that are nothing but jumble of ad-hoc developments piled over decades to save some programmers a key stroke or two. This heritage poses huge burden on the people coming into the computer science field. A full rant bashing those shells by `Brian Will` [is here](<https://www.youtube.com/watch?v=L9v4Mg8wi4U`>).
-
-The core rationale is:
-* No one has the time to listen to hours long tutorials on how powerful and versatile `ls` or `grep` are, let alone keeping the random syntax in mind (unless used on daily basis). 
-* Python shell on the other hand, offers benign syntax and eminent readibility but it comes at the rather hefty cost of terseness, or the lack of it. For example, to make up for just `ls`, you need to import some libraries and it will eventually set you back a couple of lines of code. That's not acceptable for the simple task of listing directory contents, let alone a task of compressing a directory.
-* Crocodile comes here to make Python terser and friendlier by offering functionality for everyday use, like **file management, SSH, enviroment variables management, etc**. In essence, croshell to IPython is what IPython to Python shell is; that is, the basic Python shell that can only do arithmetic is turbo-boosted making it perfect for everyday errands.
-* The library, if used in coding, will fill your life with one-liners, take your code to artistic level of brevity and readability while simultaneously being more productive by typing less boilerplate lines of code that are needless to say.
-
-The name `crocodile` signifies the use of brute force in its implementation. The focus is on ease of use, as oppoesd to beating the existing shells in speed.
-Mind you, speed is not an issue in 99% of everyday chores.
-`Crocodile` designed carefully to be loved, learning curve cound't be flattened further.
-
-This package extends many native Python classes to equip you with an uneasy-to-tame power. The major classes extended are:
-
- * `pathlib.Path` is  extended to `P`
-      * Forget about importing all the **archaic** Python libraries `os`, `glob`, `shutil`, `sys`, `zipfile` etc. `P` makes the path an object, not a lame string. `P` objects are incredibly powerful for parsing paths, *no* more than one line of code is required to do **any** operation. Take a squint at this:
-      ```
-   path = P("dataset/type1/meta/images/file3.ext")
-     >> path[0]  # allows indexing! makes sense, hah?
-      P("dataset")
-     >> path[-1]  # nifty!
-      P("file3.ext")
-     >> path[2:-1]  # even slicing!
-      P("meta/images/file3.ext")
-   ```
- * `list` is  extended to `List`
-   * Forget that `for` loops exist, because with this class, `for` loops are implicitly used to apply a function to all items.
-     Inevitably while programming, one will encounter objects of the same type and you will be struggling to get a tough grab on them.  `List` is a powerful structure that put at your disposal a grip, so tough, that the objects you have at hand start behaving like one object. Behaviour is ala-JavaScript implementation of ``forEach`` method of Arrays.
-
- * `dict` is  extended to `Struct`.
-     * Combines the power of dot notation like classes and key access like dictionaries.
-
- * Additionally, the package provides many other new classes, e.g. `Read` and `Save`. Together with `P`, they provide comprehensive support for file management. Life cannot get easier with those. Every class inherits attributes that allow saving and loading in one line.
-
-   
-Furthermore, those classes are inextricably connected. For example, globbing a path `P` object returns a `List` object. You can move back and forth between `List` and `Struct` and `DataFrame` with one method, and so on.
-
-* Deep Learning Modules.
-  * A paradigm that facilitates working with deep learning models that is based on a tri-partite scheme:
-    * HyperParameters: facilitated through `HParams` class.
-    * Data: facilitated though `DataReader` class.
-    * `BaseModel` is a frontend for both `TensorFlow` & `Pytorch` backends. The wrapper worked in tandem.
-  * The aforementioned classes cooperate together to offer sealmess workflow during creation, training, and saving models.
-
-
-# Install
-In the commandline:
-`pip install crocodile`.
-
-Being a thin extension on top of almost pure Python, you need to worry **not** about your venv, the package is not aggressive in requirements, it installs itself peacefully, never interfere with your other packages. If you do not have `numpy`, `matplotlib` and `pandas`, it simply throws `ImportError` at runtime, that's it.
-
-[comment]: # (The package is not fussy about versions either. It can though at runtime, install packages on the fly, e.g. `dill` and `tqdm` which are very lightweight libraries.)
-
-# Install Croshell Terminal
-For `Windows` machines, run the following in elevated `PowerShell`:
-```ps1
-Invoke-WebRequest https://github.com/thisismygitrepo/machineconfig/src/machineconfig/setup_windows/croshell.ps1 | Invoke-Expression
-```
-
-# Getting Started
-That's as easy as taking candy from a baby; whenever you start a Python file, preface it with following in order to unleash the library:
-
-```
-import crocodile.toolbox as tb
-```
-
-
-# A Taste of Power
-EX1: Get a list of `.exe` available in terminal.
-
-     P.env().Path.search('*.exe').reduce(lambda x, y: x+y).print()
-
-EX2: Suppose you want to know how many lines of code in your repository. The procedure is to glob all `.py` files recursively, read string code, split each one of them by lines, count the lines, add up everything from all strings of code.
-
-
-To achieve this, all you need is an eminently readable one-liner.
-```
-tb.P.cwd().search("*.py", r=True).read_text().split('\n').apply(len).to_numpy().sum()
-```
-
-How does this make perfect sense?
-* `search` returns `List` of `P` path objects
-* `read_text` is a `P` method, but it is being run against `List` object. Behind the scenes, **responsible black magic** fails to find such a method in `List` and realizes it is a method of items inside the list, so it runs it against them and thus read all files and containerize them in another `List` object and returns it.
-* A similar story applies to `split` which is a method of strings in Python.
-* Next, `apply` is a method of `List`. Sure enough, it lives up to its apt name and applies the passed function `len` to all items in the list and returns another `List` object that contains the results.
-* `.to_numpy()` converts `List` to `numpy` array, then `.sum` is a method of `numpy`, which gives the final result.
-
-Methods naming convention like `apply` and `to_numpy` are inspired from the popular `pandas` library, resulting in almost non-existing learning curve.
-
-# Friendly interactive tutorial.
-Please refer to [Here](<https://github.com/thisismygitrepo/crocodile/blob/master/tutorial.ipynb>) on the main git repo.
-
-# Full docs:
-Click [Here](<https://crocodile.readthedocs.io/en/latest/>)
-
-# Author
-Alex Al-Saffar. [email](mailto:programmer@usa.com)
+
+# Welcome to crocodile
+
+Crocodile is a library aiming at facilitating the use of Python in scripting, thus, offering an alternative to `PowerShell` & `Bash` which have absurdly complex commands that are nothing but jumble of ad-hoc developments piled over decades to save some programmers a key stroke or two. This heritage poses huge burden on the people coming into the computer science field. A full rant bashing those shells by `Brian Will` [is here](<https://www.youtube.com/watch?v=L9v4Mg8wi4U`>).
+
+The core rationale is:
+* No one has the time to listen to hours long tutorials on how powerful and versatile `ls` or `grep` are, let alone keeping the random syntax in mind (unless used on daily basis). 
+* Python shell on the other hand, offers benign syntax and eminent readibility but it comes at the rather hefty cost of terseness, or the lack of it. For example, to make up for just `ls`, you need to import some libraries and it will eventually set you back a couple of lines of code. That's not acceptable for the simple task of listing directory contents, let alone a task of compressing a directory.
+* Crocodile comes here to make Python terser and friendlier by offering functionality for everyday use, like **file management, SSH, enviroment variables management, etc**. In essence, croshell to IPython is what IPython to Python shell is; that is, the basic Python shell that can only do arithmetic is turbo-boosted making it perfect for everyday errands.
+* The library, if used in coding, will fill your life with one-liners, take your code to artistic level of brevity and readability while simultaneously being more productive by typing less boilerplate lines of code that are needless to say.
+
+The name `crocodile` signifies the use of brute force in its implementation. The focus is on ease of use, as oppoesd to beating the existing shells in speed.
+Mind you, speed is not an issue in 99% of everyday chores.
+`Crocodile` designed carefully to be loved, learning curve cound't be flattened further.
+
+This package extends many native Python classes to equip you with an uneasy-to-tame power. The major classes extended are:
+
+ * `pathlib.Path` is  extended to `P`
+      * Forget about importing all the **archaic** Python libraries `os`, `glob`, `shutil`, `sys`, `zipfile` etc. `P` makes the path an object, not a lame string. `P` objects are incredibly powerful for parsing paths, *no* more than one line of code is required to do **any** operation. Take a squint at this:
+      ```
+   path = P("dataset/type1/meta/images/file3.ext")
+     >> path[0]  # allows indexing! makes sense, hah?
+      P("dataset")
+     >> path[-1]  # nifty!
+      P("file3.ext")
+     >> path[2:-1]  # even slicing!
+      P("meta/images/file3.ext")
+   ```
+ * `list` is  extended to `List`
+   * Forget that `for` loops exist, because with this class, `for` loops are implicitly used to apply a function to all items.
+     Inevitably while programming, one will encounter objects of the same type and you will be struggling to get a tough grab on them.  `List` is a powerful structure that put at your disposal a grip, so tough, that the objects you have at hand start behaving like one object. Behaviour is ala-JavaScript implementation of ``forEach`` method of Arrays.
+
+ * `dict` is  extended to `Struct`.
+     * Combines the power of dot notation like classes and key access like dictionaries.
+
+ * Additionally, the package provides many other new classes, e.g. `Read` and `Save`. Together with `P`, they provide comprehensive support for file management. Life cannot get easier with those. Every class inherits attributes that allow saving and loading in one line.
+
+   
+Furthermore, those classes are inextricably connected. For example, globbing a path `P` object returns a `List` object. You can move back and forth between `List` and `Struct` and `DataFrame` with one method, and so on.
+
+* Deep Learning Modules.
+  * A paradigm that facilitates working with deep learning models that is based on a tri-partite scheme:
+    * HyperParameters: facilitated through `HParams` class.
+    * Data: facilitated though `DataReader` class.
+    * `BaseModel` is a frontend for both `TensorFlow` & `Pytorch` backends. The wrapper worked in tandem.
+  * The aforementioned classes cooperate together to offer sealmess workflow during creation, training, and saving models.
+
+
+# Install
+In the commandline:
+`pip install crocodile`.
+
+Being a thin extension on top of almost pure Python, you need to worry **not** about your venv, the package is not aggressive in requirements, it installs itself peacefully, never interfere with your other packages. If you do not have `numpy`, `matplotlib` and `pandas`, it simply throws `ImportError` at runtime, that's it.
+
+[comment]: # (The package is not fussy about versions either. It can though at runtime, install packages on the fly, e.g. `dill` and `tqdm` which are very lightweight libraries.)
+
+# Install Croshell Terminal
+For `Windows` machines, run the following in elevated `PowerShell`:
+```ps1
+Invoke-WebRequest https://github.com/thisismygitrepo/machineconfig/src/machineconfig/setup_windows/croshell.ps1 | Invoke-Expression
+```
+
+# Getting Started
+That's as easy as taking candy from a baby; whenever you start a Python file, preface it with following in order to unleash the library:
+
+```
+import crocodile.toolbox as tb
+```
+
+
+# A Taste of Power
+EX1: Get a list of `.exe` available in terminal.
+
+     P.env().Path.search('*.exe').reduce(lambda x, y: x+y).print()
+
+EX2: Suppose you want to know how many lines of code in your repository. The procedure is to glob all `.py` files recursively, read string code, split each one of them by lines, count the lines, add up everything from all strings of code.
+
+
+To achieve this, all you need is an eminently readable one-liner.
+```
+tb.P.cwd().search("*.py", r=True).read_text().split('\n').apply(len).to_numpy().sum()
+```
+
+How does this make perfect sense?
+* `search` returns `List` of `P` path objects
+* `read_text` is a `P` method, but it is being run against `List` object. Behind the scenes, **responsible black magic** fails to find such a method in `List` and realizes it is a method of items inside the list, so it runs it against them and thus read all files and containerize them in another `List` object and returns it.
+* A similar story applies to `split` which is a method of strings in Python.
+* Next, `apply` is a method of `List`. Sure enough, it lives up to its apt name and applies the passed function `len` to all items in the list and returns another `List` object that contains the results.
+* `.to_numpy()` converts `List` to `numpy` array, then `.sum` is a method of `numpy`, which gives the final result.
+
+Methods naming convention like `apply` and `to_numpy` are inspired from the popular `pandas` library, resulting in almost non-existing learning curve.
+
+# Friendly interactive tutorial.
+Please refer to [Here](<https://github.com/thisismygitrepo/crocodile/blob/master/tutorial.ipynb>) on the main git repo.
+
+# Full docs:
+Click [Here](<https://crocodile.readthedocs.io/en/latest/>)
+
+# Author
+Alex Al-Saffar. [email](mailto:programmer@usa.com)
```

### Comparing `crocodile-8.40/myresources/crocodile/core.py` & `crocodile-9.0/myresources/crocodile/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,223 +1,224 @@
-
-"""
-"""
-
-from pathlib import Path
-
-
-# ============================== Accessories ============================================
-def validate_name(astring: str, replace='_') -> str: return __import__("re").sub(r'[^-a-zA-Z0-9_.()]+', replace, str(astring))
-def timestamp(fmt=None, name=None): return ((name + '_') if name is not None else '') + __import__("datetime").datetime.now().strftime(fmt or '%Y-%m-%d-%I-%M-%S-%p-%f')  # isoformat is not compatible with file naming convention, fmt here is.
-def str2timedelta(shift):  # Converts a human readable string like '1m' or '1d' to a timedate object. In essence, its gives a `2m` short for `pd.timedelta(minutes=2)`"""
-    key, val = {"s": "seconds", "m": "minutes", "h": "hours", "d": "days", "w": "weeks", "M": "months", "y": "years"}[shift[-1]], eval(shift[:-1])
-    key, val = ("days", val * 30) if key == "months" else (("weeks", val * 52) if key == "years" else (key, val)); return __import__("datetime").timedelta(**{key: val})
-def randstr(length=10, lower=True, upper=True, digits=True, punctuation=False, safe=False) -> str:
-    if safe: return __import__("secrets").token_urlsafe(length)  # interannly, it uses: random.SystemRandom or os.urandom which is hardware-based, not pseudo
-    string = __import__("string"); return ''.join(__import__("random").choices((string.ascii_lowercase if lower else "") + (string.ascii_uppercase if upper else "") + (string.digits if digits else "") + (string.punctuation if punctuation else ""), k=length))
-def install_n_import(package, name=None, **kwargs):  # sometimes package name is different from import, e.g. skimage.
-    try: return __import__(package, **kwargs)
-    except ImportError: __import__("subprocess").check_call([__import__("sys").executable, "-m", "pip", "install", name or package]); return __import__(package, **kwargs)
-def get_env(): import crocodile.environment as env; return env
-
-
-def save_decorator(ext=""):  # apply default paths, add extension to path, print the saved file path
-    def decorator(func):
-        def wrapper(obj, path: str = None, verbose=True, add_suffix=True, desc="", class_name="", **kwargs):
-            if path is None: path = Path.home().joinpath("tmp_results/tmp_files").joinpath(randstr()); print(f"tb.core: Warning: Path not passed to {func}. A default path has been chosen: {path.absolute().as_uri()}") if verbose else None
-            if add_suffix:
-                [(print(f"tb.core: Warning: suffix `{a_suffix}` is added to path passed {path}") if verbose else None) for a_suffix in [ext, class_name] if a_suffix not in str(path)]
-                path = str(path).replace(ext, "").replace(class_name, "") + class_name + ext; path = Path(path).expanduser().resolve(); path.parent.mkdir(parents=True, exist_ok=True)
-            func(path=path, obj=obj, **kwargs); print(f"SAVED {desc or path.name} {obj.__class__.__name__}: {f(repr(obj), justify=0, limit=50)}  @ `{path.absolute().as_uri()}`. Size = {path.stat().st_size / 1024**2:0.2f} MB") if verbose else None  # |  Directory: `{path.parent.absolute().as_uri()}`
-            return path
-        return wrapper
-    return decorator
-
-
-@save_decorator(".json")
-def json(obj, path=None, indent=None, **kwargs): return Path(path).write_text(__import__("json").dumps(obj, indent=indent, default=lambda x: x.__dict__, **kwargs))
-@save_decorator(".yml")
-def yaml(obj, path, **kwargs):
-    with open(Path(path), 'w') as file: __import__("yaml").dump(obj, file, **kwargs)
-@save_decorator(".toml")
-def toml(obj: dict, path): return Path(path).write_text(install_n_import("toml").dumps(obj))
-@save_decorator(".ini")
-def ini(obj: dict, path, **kwargs):
-    conf = install_n_import("configparser").ConfigParser(); conf.read_dict(obj)
-    with open(path, 'w') as configfile: conf.write(configfile, **kwargs)
-@save_decorator(".csv")
-def csv(obj, path=None): return obj.to_frame('dtypes').reset_index().to_csv(path + ".dtypes")
-@save_decorator(".npy")
-def npy(obj, path, **kwargs): return __import__('numpy').save(path, obj, **kwargs)
-@save_decorator(".mat")
-def mat(mdict, path=None, **kwargs): [mdict.__setitem(key, []) for key, value in mdict.items() if value is None]; from scipy.io import savemat; savemat(str(path), mdict, **kwargs)  # Avoid using mat as it lacks perfect restoration: * `None` type is not accepted. Scalars are conveteed to [1 x 1] arrays.
-@save_decorator(".pkl")
-def vanilla_pickle(obj, path, **kwargs): return Path(path).write_bytes(__import__("pickle").dumps(obj, **kwargs))
-@save_decorator(".pkl")
-def pickle(obj=None, path=None, r=False, **kwargs): return Path(path).write_bytes(__import__("dill").dumps(obj, recurse=r, **kwargs))  # In IPyconsole of Pycharm, this works only if object is of a an imported class. Don't use with objects defined at main.
-def pickles(obj, r=False, **kwargs): return __import__("dill").dumps(obj, r=r, **kwargs)
-class Save: json = json; yaml = yaml; toml = toml; ini = ini; csv = csv; npy = npy; mat = mat; vanilla_pickle = vanilla_pickle; pickle = pickle; pickles = pickles
-
-
-# ====================================== Object Management ====================================
-class Base(object):
-    def __init__(self, *args, **kwargs): _ = args, kwargs
-    def __getstate__(self): return self.__dict__.copy()
-    def __setstate__(self, state): self.__dict__.update(state)
-    def __deepcopy__(self, *args, **kwargs): obj = self.__class__(*args, **kwargs); obj.__dict__.update(__import__("copy").deepcopy(self.__dict__)); return obj
-    def __copy__(self, *args, **kwargs): obj = self.__class__(*args, **kwargs); obj.__dict__.update(self.__dict__.copy()); return obj
-    def eval(self, string_, func=False, other=False): return string_ if type(string_) is not str else eval((("lambda x, y: " if other else "lambda x:") if not str(string_).startswith("lambda") and func else "") + string_ + (self if False else ''))
-    def exec(self, expr: str) -> 'Base': exec(expr); return self  # exec returns None.
-    def save(self, path=None, add_suffix=True, save_code=False, verbose=True, data_only=True, desc=""):
-        saved_file = Save.pickle(obj=self.__getstate__() if data_only else self, path=path, verbose=verbose, add_suffix=add_suffix, class_name="." + self.__class__.__name__ + (".dat" if data_only else ""), desc=desc or (f"Data of {self.__class__}" if data_only else desc))
-        self.save_code(path=saved_file.parent.joinpath(saved_file.name + "_saved_code.py")) if save_code else None; return self
-    @classmethod
-    def from_saved_data(cls, path, *args, **kwargs): obj = cls(*args, **kwargs); obj.__setstate__(dict(__import__("dill").loads(Path(path).read_bytes()))); return obj
-    def save_code(self, path):
-        if hasattr(module := __import__("inspect").getmodule(self), "__file__"): file = Path(module.__file__)
-        else: raise FileNotFoundError(f"Attempted to save code from a script running in interactive session! module should be imported instead.")
-        Path(path).expanduser().write_text(file.read_text()); return Path(path) if type(path) is str else path  # path could be tb.P, better than Path
-    def get_attributes(self, remove_base_attrs=True, return_objects=False, fields=True, methods=True):
-        attrs = List(dir(self)).filter(lambda x: '__' not in x and not x.startswith('_')).remove(values=Base().get_attributes(remove_base_attrs=False)if remove_base_attrs else []); import inspect
-        attrs = attrs.filter(lambda x: (inspect.ismethod(getattr(self, x)) if not fields else True) and ((not inspect.ismethod(getattr(self, x))) if not methods else True))  # logic (questionable): anything that is not a method is a field
-        return List([getattr(self, x) for x in attrs]) if return_objects else List(attrs)
-    @staticmethod
-    def print(self, dtype=False, attrs=False, **kwargs): return Struct(self.__dict__).update(attrs=self.get_attributes() if attrs else None).print(dtype=dtype, **kwargs)
-    @staticmethod
-    def get_state(obj, repr_func=lambda x: x, exclude=None) -> dict: return repr_func(obj) if not any([hasattr(obj, "__getstate__"), hasattr(obj, "__dict__")]) else (tmp if type(tmp := obj.__getstate__() if hasattr(obj, "__getstate__") else obj.__dict__) is not dict else Struct(tmp).filter(lambda k, v: k not in (exclude or [])).apply2values(lambda k, v: Base.get_state(v, exclude=exclude, repr_func=repr_func)).__dict__)
-    def viz_composition_heirarchy(self, depth=3, obj=None, filt=None):
-        install_n_import("objgraph").show_refs([self] if obj is None else [obj], max_depth=depth, filename=str(filename := Path(__import__("tempfile").gettempdir()).joinpath("graph_viz_" + randstr() + ".png")), filter=filt)
-        __import__("os").startfile(str(filename.absolute())) if __import__("sys").platform == "win32" else None; return filename
-
-
-class List(Base):  # Inheriting from Base gives save method.  # Use this class to keep items of the same type."""
-    def __init__(self, obj_list=None): super().__init__(); self.list = list(obj_list) if obj_list is not None else []
-    def save_items(self, directory, names=None, saver=None): [(saver or Save.pickle)(path=directory / name, obj=item) for name, item in zip(names or range(len(self)), self.list)]
-    def __repr__(self): return f"List [{len(self.list)} elements]. First Item: " + f"{get_repr(self.list[0], justify=0, limit=100)}" if len(self.list) > 0 else f"An Empty List []"
-    def print(self, sep='\n', styler=repr, return_str=False, **kwargs): res = sep.join([f"{idx:2}- {styler(item)}" for idx, item in enumerate(self.list)]); print(res) if not return_str else None; return res if return_str else None
-    def __deepcopy__(self): return List([__import__("copy").deepcopy(i) for i in self.list])
-    def __bool__(self): return bool(self.list)
-    def __contains__(self, key): return key in self.list
-    def __copy__(self) -> 'List': return List(self.list.copy())
-    def __getstate__(self): return self.list
-    def __setstate__(self, state): self.list = state
-    def __len__(self): return len(self.list)
-    def __iter__(self): return iter(self.list)
-    def __array__(self): import numpy as np; return np.array(self.list)  # compatibility with numpy
-    len = property(lambda self: self.list.__len__())
-    # ================= call methods =====================================
-    def __getattr__(self, name) -> 'List': return List(getattr(i, name) for i in self.list)  # fallback position when __getattribute__ mechanism fails.
-    def __call__(self, *args, **kwargs) -> 'List': return List(i(*args, **kwargs) for i in self.list)
-    # ======================== Access Methods ==========================================
-    def __setitem__(self, key, value): self.list[key] = value
-    def sample(self, size=1, replace=False, p=None) -> 'List': return self[list(__import__("numpy").random.choice(len(self), size, replace=replace, p=p))]
-    def split(self, every=1, to=None) -> 'List': every = every if to is None else __import__("math").ceil(len(self) / to); return List([(self[ix:ix+every] if ix+every < len(self) else self[ix:len(self)]) for ix in range(0, len(self), every)])
-    def filter(self, func, which=lambda idx, x: x) -> 'List': self.eval(func, func=True); return List([which(idx, x) for idx, x in enumerate(self.list) if func(x)])
-    # ======================= Modify Methods ===============================
-    def reduce(self, func=lambda x, y: x+y, default=None) -> 'List': args = (self.eval(func, func=True, other=True), self.list) + ((default,) if default is not None else ()); return __import__("functools").reduce(*args)
-    def append(self, item) -> 'List': self.list.append(item); return self
-    def __add__(self, other) -> 'List': return List(self.list + list(other))  # implement coersion
-    def __radd__(self, other) -> 'List': return List(list(other) + self.list)
-    def __iadd__(self, other) -> 'List': self.list = self.list + list(other); return self  # inplace add.
-    def sort(self, key=None, reverse=False) -> 'List': self.list.sort(key=key, reverse=reverse); return self
-    def sorted(self, *args, **kwargs) -> 'List': return List(sorted(self.list, *args, **kwargs))
-    def insert(self, __index: int, __object): self.list.insert(__index, __object); return self
-    def modify(self, expr: str, other=None) -> 'List': [exec(expr) for idx, x in enumerate(self.list)] if other is None else [exec(expr) for idx, (x, y) in enumerate(zip(self.list, other))]; return self
-    def remove(self, value=None, values=None, strict=True) -> 'List': [self.list.remove(a_val) for a_val in ((values or []) + ([value] if value else [])) if strict or value in self.list]; return self
-    def to_series(self): return __import__("pandas").Series(self.list)
-    def to_list(self) -> list: return self.list
-    def to_numpy(self, **kwargs): import numpy as np; return np.array(self.list, **kwargs)
-    np = property(lambda self: self.to_numpy())
-    def to_struct(self, key_val=None) -> 'Struct': return Struct.from_keys_values_pairs(self.apply(self.eval(key_val, func=True) if key_val else lambda x: (str(x), x)))
-    def __getitem__(self, key: str or list or slice):
-        if type(key) is list: return List(self[item] for item in key)  # to allow fancy indexing like List[1, 5, 6]
-        elif type(key) is str: return List(item[key] for item in self.list)  # access keys like dictionaries.
-        return self.list[key] if type(key) is not slice else List(self.list[key])  # must be an integer or slice: behaves similarly to Numpy A[1] vs A[1:2]
-    def apply(self, func, *args, other=None, filt=lambda x: True, jobs=None, prefer=[None, 'processes', 'threads'][0], depth=1, verbose=False, desc=None, **kwargs) -> 'List':
-        if depth > 1: self.apply(lambda x: x.apply(func, *args, other=other, jobs=jobs, depth=depth-1, **kwargs)); func = self.eval(func, func=True, other=bool(other))
-        iterator = (self.list if not verbose else install_n_import("tqdm").tqdm(self.list, desc=desc)) if other is None else (zip(self.list, other) if not verbose else install_n_import("tqdm").tqdm(zip(self.list, other), desc=desc))
-        if jobs: from joblib import Parallel, delayed; return List(Parallel(n_jobs=jobs, prefer=prefer)(delayed(func)(x, *args, **kwargs) for x in iterator)) if other is None else List(Parallel(n_jobs=jobs, prefer=prefer)(delayed(func)(x, y) for x, y in iterator))
-        return List([func(x, *args, **kwargs) for x in iterator if filt(x)]) if other is None else List([func(x, y) for x, y in iterator])
-    def to_dataframe(self, names=None, minimal=False, obj_included=True):
-        df = __import__("pandas").DataFrame(columns=(['object'] if obj_included or names else []) + list(self.list[0].__dict__.keys()))
-        if minimal: return df
-        for i, obj in enumerate(self.list):  # Populate the dataframe:
-            if obj_included or names: df.loc[i] = ([obj] if names is None else [names[i]]) + list(self.list[i].__dict__.values())
-            else: df.loc[i] = list(self.list[i].__dict__.values())
-        return df
-
-
-class Struct(Base):  # inheriting from dict gives `get` method, should give `__contains__` but not working. # Inheriting from Base gives `save` method.
-    """Use this class to keep bits and sundry items. Combines the power of dot notation in classes with strings in dictionaries to provide Pandas-like experience"""
-    def __init__(self, dictionary=None, **kwargs):
-        if dictionary is None or type(dictionary) is dict: final_dict = dict() if dictionary is None else dictionary
-        else: final_dict = (dict(dictionary) if dictionary.__class__.__name__ == "mappingproxy" else dictionary.__dict__)
-        final_dict.update(kwargs); super(Struct, self).__init__(); self.__dict__ = final_dict
-    @staticmethod
-    def recursive_struct(mydict) -> 'Struct': struct = Struct(mydict); [struct.__setitem__(key, Struct.recursive_struct(val) if type(val) is dict else val) for key, val in struct.items()]; return struct
-    @staticmethod
-    def recursive_dict(struct) -> 'Struct': [struct.__dict__.__setitem__(key, Struct.recursive_dict(val) if type(val) is Struct else val) for key, val in struct.__dict__.items()]; return struct.__dict__
-    def save_json(self, path=None, indent=None): return Save.json(obj=self.__dict__, path=path, indent=indent)
-    from_keys_values = classmethod(lambda cls, k, v: cls(dict(zip(k, v))))
-    from_keys_values_pairs = classmethod(lambda cls, my_list: cls({k: v for k, v in my_list}))
-    @classmethod
-    def from_names(cls, names, default_=None) -> 'Struct': return cls.from_keys_values(k=names, v=default_ or [None] * len(names))  # Mimick NamedTuple and defaultdict
-    def spawn_from_values(self, values) -> 'Struct': return self.from_keys_values(self.keys(), self.eval(values, func=False))
-    def spawn_from_keys(self, keys) -> 'Struct': return self.from_keys_values(self.eval(keys, func=False), self.values())
-    def to_default(self, default=lambda: None): tmp2 = __import__("collections").defaultdict(default); tmp2.update(self.__dict__); self.__dict__ = tmp2; return self
-    def __str__(self, sep="\n"): return config(self.__dict__, sep=sep)
-    def __getattr__(self, item) -> 'Struct':
-        try: return self.__dict__[item]
-        except KeyError: raise AttributeError(f'{type(self).__name__!r} object has no attribute {item!r}')  # this works better with the linter. replacing Key error with Attribute error makes class work nicely with hasattr() by returning False.
-    clean_view = property(lambda self: type("TempClass", (object,), self.__dict__))
-    def __repr__(self, limit=150): return "Struct: " + Display.get_repr(self.keys().list.__repr__(), limit=limit, justify=0)
-    def __getitem__(self, item): return self.__dict__[item]  # thus, gives both dot notation and string access to elements.
-    def __setitem__(self, key, value): self.__dict__[key] = value
-    def __bool__(self): return bool(self.__dict__)
-    def __contains__(self, key): return key in self.__dict__
-    def __len__(self): return len(self.keys())
-    def __getstate__(self): return self.__dict__  # serialization
-    def __setstate__(self, state): self.__dict__ = state
-    def __iter__(self): return iter(self.__dict__.items())
-    def __delitem__(self, key): del self.__dict__[key]
-    def copy(self) -> 'Struct': return Struct(self.__dict__.copy())
-    def to_dataframe(self, *args, **kwargs): return __import__("pandas").DataFrame(self.__dict__, *args, **kwargs)
-    def keys(self, verbose=False) -> 'List': return List(list(self.__dict__.keys())) if not verbose else install_n_import("tqdm").tqdm(self.__dict__.keys())
-    def values(self, verbose=False) -> 'List': return List(list(self.__dict__.values())) if not verbose else install_n_import("tqdm").tqdm(self.__dict__.values())
-    def items(self, verbose=False, desc="") -> 'List': return List(self.__dict__.items()) if not verbose else install_n_import("tqdm").tqdm(self.__dict__.items(), desc=desc)
-    def get(self, key=None, default=None, strict=False, keys=None) -> 'List': return List([self.__dict__.get(key, default) if not strict else self[key] for key in (keys if keys is not None else [])]) if keys is not None else (self.__dict__.get(key, default) if not strict else self[key])
-    def apply2keys(self, kv_func, verbose=False, desc="") -> 'Struct': return Struct({kv_func(key, val): val for key, val in self.items(verbose=verbose, desc=desc)})
-    def apply2values(self, kv_func, verbose=False, desc="") -> 'Struct': [self.__setitem__(key, kv_func(key, val)) for key, val in self.items(verbose=verbose, desc=desc)]; return self
-    def apply(self, kv_func) -> 'List': return self.items().apply(lambda item: kv_func(item[0], item[1]))
-    def filter(self, kv_func=None) -> 'Struct': return Struct({key: self[key] for key, val in self.items() if kv_func(key, val)})
-    def inverse(self) -> 'Struct': return Struct({v: k for k, v in self.__dict__.items()})
-    def update(self, *args, **kwargs) -> 'Struct': self.__dict__.update(Struct(*args, **kwargs).__dict__); return self
-    def delete(self, key=None, keys=None, kv_func=None) -> 'Struct': [self.__dict__.__delitem__(key) for key in ([key] if key else [] + (keys if keys is not None else []))]; [self.__dict__.__delitem__(k) for k, v in self.items() if kv_func(k, v)] if kv_func is not None else None; return self
-    def _pandas_repr(self, justify, return_str=False, limit=30): res = __import__("pandas").DataFrame(__import__("numpy").array([self.keys(), self.values().apply(lambda x: str(type(x)).split("'")[1]), self.values().apply(lambda x: get_repr(x, justify=justify, limit=limit).replace("\n", " "))]).T, columns=["key", "dtype", "details"]); return res if not return_str else str(res)
-    def print(self, dtype=True, return_str=False, justify=30, as_config=False, as_yaml=False, limit=50, **kwargs):
-        res = f"Empty Struct." if not bool(self) else ((__import__("yaml").dump(self.__dict__) if as_yaml else config(self.__dict__, justify=justify, **kwargs)) if as_yaml or as_config else self._pandas_repr(justify=justify, return_str=False, limit=limit).drop(columns=[] if dtype else ["dtype"]))
-        print(res) if not return_str else None; return str(res) if return_str else self
-    @staticmethod
-    def concat_values(*dicts, orient='list') -> 'Struct': return Struct(__import__("pandas").concat(List(dicts).apply(lambda x: Struct(x).to_dataframe())).to_dict(orient=orient))
-    def plot(self, use_plt=True, title='', xlabel='', ylabel='', **kwargs):
-        if not use_plt: fig = __import__("crocodile.plotly_management").px.line(self.__dict__); fig.show(); return fig
-        else: artist = __import__("crocodile").matplotlib_management.Artist(figname='Structure Plot', **kwargs); artist.plot_dict(self.__dict__, title=title, xlabel=xlabel, ylabel=ylabel); return artist
-
-def set_pandas_display(rows=1000, columns=1000, width=5000, colwidth=40) -> None: import pandas as pd; pd.set_option('display.max_colwidth', colwidth); pd.set_option('display.max_columns', columns); pd.set_option('display.width', width); pd.set_option('display.max_rows', rows)
-def set_pandas_auto_width(): __import__("pandas").set_option('width', 0)  # this way, pandas is told to detect window length and act appropriately.  For fixed width host windows, this is recommended to avoid chaos due to line-wrapping.
-def set_numpy_display(precision=3, linewidth=250, suppress=True, floatmode='fixed', **kwargs) -> None: __import__("numpy").set_printoptions(precision=precision, suppress=suppress, linewidth=linewidth, floatmode=floatmode, **kwargs)
-def config(mydict, sep="\n", justify=15, quotes=False): return sep.join([f"{key:>{justify}} = {repr(val) if quotes else val}" for key, val in mydict.items()])
-def f(str_, limit=float('inf'), justify=50, direc="<") -> str: return f"{(str_[:limit - 4] + '... ' if len(str_) > limit else str_):{direc}{justify}}"
-def eng(): __import__("pandas").set_eng_float_format(accuracy=3, use_eng_prefix=True); __import__("pandas").options.float_format = '{:, .5f}'.format; __import__("pandas").set_option('precision', 7)  # __import__("pandas").set_printoptions(formatter={'float': '{: 0.3f}'.format})
-def outline(array, name="Array", printit=True): str_ = f"{name}. Shape={array.shape}. Dtype={array.dtype}"; print(str_) if printit else None; return str_
-def get_repr(data, justify=15, limit=float('inf'), direc="<") -> str:
-    if (dtype := data.__class__.__name__) in {'list', 'str'}: str_ = data if dtype == 'str' else f"list. length = {len(data)}. " + ("1st item type: " + str(type(data[0])).split("'")[1]) if len(data) > 0 else " "
-    elif dtype in {"DataFrame", "Series"}: str_ = f"Pandas DF: shape = {data.shape}, dtype = {data.dtypes}." if dtype == 'DataFrame' else f"Pandas Series: Length = {len(data)}, Keys = {get_repr(data.keys().to_list())}."
-    else: str_ = f"shape = {data.shape}, dtype = {data.dtype}." if dtype == 'ndarray' else repr(data)
-    return f(str_.replace("\n", ", "), justify=justify, limit=limit, direc=direc)
-def print_string_list(mylist, char_per_row=125, sep=" ", style=str, _counter=0):
-    for item in mylist: print("") if (_counter + len(style(item))) // char_per_row > 0 else print(style(item), end=sep); _counter = len(style(item)) if (_counter + len(style(item))) // char_per_row > 0 else _counter + len(style(item))
-class Display: set_pandas_display = set_pandas_display; set_pandas_auto_width = set_pandas_auto_width; set_numpy_display = set_numpy_display; config = config; f = f; eng = eng; outline = outline; get_repr = get_repr; print_string_list = print_string_list  # or D = type('D', (object, ), dict(set_pandas_display
-
-
-if __name__ == '__main__':
-    pass
+
+"""
+"""
+
+from pathlib import Path
+
+
+# ============================== Accessories ============================================
+def validate_name(astring: str, replace='_') -> str: return __import__("re").sub(r'[^-a-zA-Z0-9_.()]+', replace, str(astring))
+def timestamp(fmt=None, name=None): return ((name + '_') if name is not None else '') + __import__("datetime").datetime.now().strftime(fmt or '%Y-%m-%d-%I-%M-%S-%p-%f')  # isoformat is not compatible with file naming convention, fmt here is.
+def str2timedelta(shift):  # Converts a human readable string like '1m' or '1d' to a timedate object. In essence, its gives a `2m` short for `pd.timedelta(minutes=2)`"""
+    key, val = {"s": "seconds", "m": "minutes", "h": "hours", "d": "days", "w": "weeks", "M": "months", "y": "years"}[shift[-1]], eval(shift[:-1])
+    key, val = ("days", val * 30) if key == "months" else (("weeks", val * 52) if key == "years" else (key, val)); return __import__("datetime").timedelta(**{key: val})
+def randstr(length=10, lower=True, upper=True, digits=True, punctuation=False, safe=False) -> str:
+    if safe: return __import__("secrets").token_urlsafe(length)  # interannly, it uses: random.SystemRandom or os.urandom which is hardware-based, not pseudo
+    string = __import__("string"); return ''.join(__import__("random").choices((string.ascii_lowercase if lower else "") + (string.ascii_uppercase if upper else "") + (string.digits if digits else "") + (string.punctuation if punctuation else ""), k=length))
+def install_n_import(package, name=None, **kwargs):  # sometimes package name is different from import, e.g. skimage.
+    try: return __import__(package, **kwargs)
+    except ImportError: __import__("subprocess").check_call([__import__("sys").executable, "-m", "pip", "install", name or package]); return __import__(package, **kwargs)
+def get_env(): import crocodile.environment as env; return env
+
+
+def save_decorator(ext=""):  # apply default paths, add extension to path, print the saved file path
+    def decorator(func):
+        def wrapper(obj, path: str = None, verbose=True, add_suffix=True, desc="", class_name="", **kwargs):
+            if path is None: path = Path.home().joinpath("tmp_results/tmp_files").joinpath(randstr()); print(f"tb.core: Warning: Path not passed to {func}. A default path has been chosen: {path.absolute().as_uri()}") if verbose else None
+            if add_suffix:
+                [(print(f"tb.core: Warning: suffix `{a_suffix}` is added to path passed {path}") if verbose else None) for a_suffix in [ext, class_name] if a_suffix not in str(path)]
+                path = str(path).replace(ext, "").replace(class_name, "") + class_name + ext; path = Path(path).expanduser().resolve(); path.parent.mkdir(parents=True, exist_ok=True)
+            func(path=path, obj=obj, **kwargs); print(f"SAVED {desc or path.name} {obj.__class__.__name__}: {f(repr(obj), justify=0, limit=50)}  @ `{path.absolute().as_uri()}`. Size = {path.stat().st_size / 1024**2:0.2f} MB") if verbose else None  # |  Directory: `{path.parent.absolute().as_uri()}`
+            return path
+        return wrapper
+    return decorator
+
+
+@save_decorator(".json")
+def json(obj, path=None, indent=None, **kwargs): return Path(path).write_text(__import__("json").dumps(obj, indent=indent, default=lambda x: x.__dict__, **kwargs))
+@save_decorator(".yml")
+def yaml(obj, path, **kwargs):
+    with open(Path(path), 'w') as file: __import__("yaml").dump(obj, file, **kwargs)
+@save_decorator(".toml")
+def toml(obj: dict, path): return Path(path).write_text(install_n_import("toml").dumps(obj))
+@save_decorator(".ini")
+def ini(obj: dict, path, **kwargs):
+    conf = install_n_import("configparser").ConfigParser(); conf.read_dict(obj)
+    with open(path, 'w') as configfile: conf.write(configfile, **kwargs)
+@save_decorator(".csv")
+def csv(obj, path=None): return obj.to_frame('dtypes').reset_index().to_csv(path + ".dtypes")
+@save_decorator(".npy")
+def npy(obj, path, **kwargs): return __import__('numpy').save(path, obj, **kwargs)
+@save_decorator(".mat")
+def mat(mdict, path=None, **kwargs): [mdict.__setitem(key, []) for key, value in mdict.items() if value is None]; from scipy.io import savemat; savemat(str(path), mdict, **kwargs)  # Avoid using mat as it lacks perfect restoration: * `None` type is not accepted. Scalars are conveteed to [1 x 1] arrays.
+@save_decorator(".pkl")
+def vanilla_pickle(obj, path, **kwargs): return Path(path).write_bytes(__import__("pickle").dumps(obj, **kwargs))
+@save_decorator(".pkl")
+def pickle(obj=None, path=None, r=False, **kwargs): return Path(path).write_bytes(__import__("dill").dumps(obj, recurse=r, **kwargs))  # In IPyconsole of Pycharm, this works only if object is of a an imported class. Don't use with objects defined at main.
+def pickles(obj, r=False, **kwargs): return __import__("dill").dumps(obj, r=r, **kwargs)
+class Save: json = json; yaml = yaml; toml = toml; ini = ini; csv = csv; npy = npy; mat = mat; vanilla_pickle = vanilla_pickle; pickle = pickle; pickles = pickles
+
+
+# ====================================== Object Management ====================================
+class Base(object):
+    def __init__(self, *args, **kwargs): _ = args, kwargs
+    def __getstate__(self): return self.__dict__.copy()
+    def __setstate__(self, state): self.__dict__.update(state)
+    def __deepcopy__(self, *args, **kwargs): obj = self.__class__(*args, **kwargs); obj.__dict__.update(__import__("copy").deepcopy(self.__dict__)); return obj
+    def __copy__(self, *args, **kwargs): obj = self.__class__(*args, **kwargs); obj.__dict__.update(self.__dict__.copy()); return obj
+    def eval(self, string_, func=False, other=False): return string_ if type(string_) is not str else eval((("lambda x, y: " if other else "lambda x:") if not str(string_).startswith("lambda") and func else "") + string_ + (self if False else ''))
+    def exec(self, expr: str) -> 'Base': exec(expr); return self  # exec returns None.
+    def save(self, path=None, add_suffix=True, save_code=False, verbose=True, data_only=True, desc=""):  # + (".dat" if data_only else "")
+        saved_file = Save.pickle(obj=self.__getstate__() if data_only else self, path=path, verbose=verbose, add_suffix=add_suffix, class_name="." + self.__class__.__name__, desc=desc or (f"Data of {self.__class__}" if data_only else desc))
+        self.save_code(path=saved_file.parent.joinpath(saved_file.name + "_saved_code.py")) if save_code else None; return self
+    @classmethod
+    def from_saved_data(cls, path, *args, **kwargs): obj = cls(*args, **kwargs); obj.__setstate__(dict(__import__("dill").loads(Path(path).read_bytes()))); return obj
+    def save_code(self, path):
+        if hasattr(module := __import__("inspect").getmodule(self), "__file__"): file = Path(module.__file__)
+        else: raise FileNotFoundError(f"Attempted to save code from a script running in interactive session! module should be imported instead.")
+        Path(path).expanduser().write_text(file.read_text()); return Path(path) if type(path) is str else path  # path could be tb.P, better than Path
+    def get_attributes(self, remove_base_attrs=True, return_objects=False, fields=True, methods=True):
+        attrs = List(dir(self)).filter(lambda x: '__' not in x and not x.startswith('_')).remove(values=Base().get_attributes(remove_base_attrs=False)if remove_base_attrs else []); import inspect
+        attrs = attrs.filter(lambda x: (inspect.ismethod(getattr(self, x)) if not fields else True) and ((not inspect.ismethod(getattr(self, x))) if not methods else True))  # logic (questionable): anything that is not a method is a field
+        return List([getattr(self, x) for x in attrs]) if return_objects else List(attrs)
+    @staticmethod
+    def print(self, dtype=False, attrs=False, **kwargs): return Struct(self.__dict__).update(attrs=self.get_attributes() if attrs else None).print(dtype=dtype, **kwargs)
+    @staticmethod
+    def get_state(obj, repr_func=lambda x: x, exclude=None) -> dict: return repr_func(obj) if not any([hasattr(obj, "__getstate__"), hasattr(obj, "__dict__")]) else (tmp if type(tmp := obj.__getstate__() if hasattr(obj, "__getstate__") else obj.__dict__) is not dict else Struct(tmp).filter(lambda k, v: k not in (exclude or [])).apply2values(lambda k, v: Base.get_state(v, exclude=exclude, repr_func=repr_func)).__dict__)
+    def viz_composition_heirarchy(self, depth=3, obj=None, filt=None):
+        install_n_import("objgraph").show_refs([self] if obj is None else [obj], max_depth=depth, filename=str(filename := Path(__import__("tempfile").gettempdir()).joinpath("graph_viz_" + randstr() + ".png")), filter=filt)
+        __import__("os").startfile(str(filename.absolute())) if __import__("sys").platform == "win32" else None; return filename
+
+
+class List(Base):  # Inheriting from Base gives save method.  # Use this class to keep items of the same type."""
+    def __init__(self, obj_list=None): super().__init__(); self.list = list(obj_list) if obj_list is not None else []
+    def save_items(self, directory, names=None, saver=None): [(saver or Save.pickle)(path=directory / name, obj=item) for name, item in zip(names or range(len(self)), self.list)]
+    def __repr__(self): return f"List [{len(self.list)} elements]. First Item: " + f"{get_repr(self.list[0], justify=0, limit=100)}" if len(self.list) > 0 else f"An Empty List []"
+    def print(self, sep='\n', styler=repr, return_str=False, **kwargs): res = sep.join([f"{idx:2}- {styler(item)}" for idx, item in enumerate(self.list)]); print(res) if not return_str else None; return res if return_str else None
+    def __deepcopy__(self): return List([__import__("copy").deepcopy(i) for i in self.list])
+    def __bool__(self): return bool(self.list)
+    def __contains__(self, key): return key in self.list
+    def __copy__(self) -> 'List': return List(self.list.copy())
+    def __getstate__(self): return self.list
+    def __setstate__(self, state): self.list = state
+    def __len__(self): return len(self.list)
+    def __iter__(self): return iter(self.list)
+    def __array__(self): import numpy as np; return np.array(self.list)  # compatibility with numpy
+    len = property(lambda self: self.list.__len__())
+    # ================= call methods =====================================
+    def __getattr__(self, name) -> 'List': return List(getattr(i, name) for i in self.list)  # fallback position when __getattribute__ mechanism fails.
+    def __call__(self, *args, **kwargs) -> 'List': return List(i(*args, **kwargs) for i in self.list)
+    # ======================== Access Methods ==========================================
+    def __setitem__(self, key, value): self.list[key] = value
+    def sample(self, size=1, replace=False, p=None) -> 'List': return self[list(__import__("numpy").random.choice(len(self), size, replace=replace, p=p))]
+    def split(self, every=1, to=None) -> 'List': every = every if to is None else __import__("math").ceil(len(self) / to); return List([(self[ix:ix+every] if ix+every < len(self) else self[ix:len(self)]) for ix in range(0, len(self), every)])
+    def filter(self, func, which=lambda idx, x: x) -> 'List': self.eval(func, func=True); return List([which(idx, x) for idx, x in enumerate(self.list) if func(x)])
+    # ======================= Modify Methods ===============================
+    def reduce(self, func=lambda x, y: x+y, default=None) -> 'List': args = (self.eval(func, func=True, other=True), self.list) + ((default,) if default is not None else ()); return __import__("functools").reduce(*args)
+    def append(self, item) -> 'List': self.list.append(item); return self
+    def __add__(self, other) -> 'List': return List(self.list + list(other))  # implement coersion
+    def __radd__(self, other) -> 'List': return List(list(other) + self.list)
+    def __iadd__(self, other) -> 'List': self.list = self.list + list(other); return self  # inplace add.
+    def sort(self, key=None, reverse=False) -> 'List': self.list.sort(key=key, reverse=reverse); return self
+    def sorted(self, *args, **kwargs) -> 'List': return List(sorted(self.list, *args, **kwargs))
+    def insert(self, __index: int, __object): self.list.insert(__index, __object); return self
+    def modify(self, expr: str, other=None) -> 'List': [exec(expr) for idx, x in enumerate(self.list)] if other is None else [exec(expr) for idx, (x, y) in enumerate(zip(self.list, other))]; return self
+    def remove(self, value=None, values=None, strict=True) -> 'List': [self.list.remove(a_val) for a_val in ((values or []) + ([value] if value else [])) if strict or value in self.list]; return self
+    def to_series(self): return __import__("pandas").Series(self.list)
+    def to_list(self) -> list: return self.list
+    def to_numpy(self, **kwargs): import numpy as np; return np.array(self.list, **kwargs)
+    np = property(lambda self: self.to_numpy())
+    def to_struct(self, key_val=None) -> 'Struct': return Struct.from_keys_values_pairs(self.apply(self.eval(key_val, func=True) if key_val else lambda x: (str(x), x)))
+    def __getitem__(self, key: str or list or slice):
+        if type(key) is list: return List(self[item] for item in key)  # to allow fancy indexing like List[1, 5, 6]
+        elif type(key) is str: return List(item[key] for item in self.list)  # access keys like dictionaries.
+        return self.list[key] if type(key) is not slice else List(self.list[key])  # must be an integer or slice: behaves similarly to Numpy A[1] vs A[1:2]
+    def apply(self, func, *args, other=None, filt=lambda x: True, jobs=None, prefer=[None, 'processes', 'threads'][0], depth=1, verbose=False, desc=None, **kwargs) -> 'List':
+        if depth > 1: self.apply(lambda x: x.apply(func, *args, other=other, jobs=jobs, depth=depth-1, **kwargs)); func = self.eval(func, func=True, other=bool(other))
+        iterator = (self.list if not verbose else install_n_import("tqdm").tqdm(self.list, desc=desc)) if other is None else (zip(self.list, other) if not verbose else install_n_import("tqdm").tqdm(zip(self.list, other), desc=desc))
+        if jobs: from joblib import Parallel, delayed; return List(Parallel(n_jobs=jobs, prefer=prefer)(delayed(func)(x, *args, **kwargs) for x in iterator)) if other is None else List(Parallel(n_jobs=jobs, prefer=prefer)(delayed(func)(x, y) for x, y in iterator))
+        return List([func(x, *args, **kwargs) for x in iterator if filt(x)]) if other is None else List([func(x, y) for x, y in iterator])
+    def to_dataframe(self, names=None, minimal=False, obj_included=True):
+        df = __import__("pandas").DataFrame(columns=(['object'] if obj_included or names else []) + list(self.list[0].__dict__.keys()))
+        if minimal: return df
+        for i, obj in enumerate(self.list):  # Populate the dataframe:
+            if obj_included or names: df.loc[i] = ([obj] if names is None else [names[i]]) + list(self.list[i].__dict__.values())
+            else: df.loc[i] = list(self.list[i].__dict__.values())
+        return df
+
+
+class Struct(Base):  # inheriting from dict gives `get` method, should give `__contains__` but not working. # Inheriting from Base gives `save` method.
+    """Use this class to keep bits and sundry items. Combines the power of dot notation in classes with strings in dictionaries to provide Pandas-like experience"""
+    def __init__(self, dictionary=None, **kwargs):
+        if dictionary is None or type(dictionary) is dict: final_dict = dict() if dictionary is None else dictionary
+        else: final_dict = (dict(dictionary) if dictionary.__class__.__name__ == "mappingproxy" else dictionary.__dict__)
+        final_dict.update(kwargs); super(Struct, self).__init__(); self.__dict__ = final_dict
+    @staticmethod
+    def recursive_struct(mydict) -> 'Struct': struct = Struct(mydict); [struct.__setitem__(key, Struct.recursive_struct(val) if type(val) is dict else val) for key, val in struct.items()]; return struct
+    @staticmethod
+    def recursive_dict(struct) -> 'Struct': [struct.__dict__.__setitem__(key, Struct.recursive_dict(val) if type(val) is Struct else val) for key, val in struct.__dict__.items()]; return struct.__dict__
+    def save_json(self, path=None, indent=None): return Save.json(obj=self.__dict__, path=path, indent=indent)
+    from_keys_values = classmethod(lambda cls, k, v: cls(dict(zip(k, v))))
+    from_keys_values_pairs = classmethod(lambda cls, my_list: cls({k: v for k, v in my_list}))
+    @classmethod
+    def from_names(cls, names, default_=None) -> 'Struct': return cls.from_keys_values(k=names, v=default_ or [None] * len(names))  # Mimick NamedTuple and defaultdict
+    def spawn_from_values(self, values) -> 'Struct': return self.from_keys_values(self.keys(), self.eval(values, func=False))
+    def spawn_from_keys(self, keys) -> 'Struct': return self.from_keys_values(self.eval(keys, func=False), self.values())
+    def to_default(self, default=lambda: None): tmp2 = __import__("collections").defaultdict(default); tmp2.update(self.__dict__); self.__dict__ = tmp2; return self
+    def __str__(self, sep="\n"): return config(self.__dict__, sep=sep)
+    def __getattr__(self, item) -> 'Struct':
+        try: return self.__dict__[item]
+        except KeyError: raise AttributeError(f'{type(self).__name__!r} object has no attribute {item!r}')  # this works better with the linter. replacing Key error with Attribute error makes class work nicely with hasattr() by returning False.
+    clean_view = property(lambda self: type("TempClass", (object,), self.__dict__))
+    def __repr__(self, limit=150): return "Struct: " + Display.get_repr(self.keys().list.__repr__(), limit=limit, justify=0)
+    def __getitem__(self, item): return self.__dict__[item]  # thus, gives both dot notation and string access to elements.
+    def __setitem__(self, key, value): self.__dict__[key] = value
+    def __bool__(self): return bool(self.__dict__)
+    def __contains__(self, key): return key in self.__dict__
+    def __len__(self): return len(self.keys())
+    def __getstate__(self): return self.__dict__  # serialization
+    def __setstate__(self, state): self.__dict__ = state
+    def __iter__(self): return iter(self.__dict__.items())
+    def __delitem__(self, key): del self.__dict__[key]
+    def copy(self) -> 'Struct': return Struct(self.__dict__.copy())
+    def to_dataframe(self, *args, **kwargs): return __import__("pandas").DataFrame(self.__dict__, *args, **kwargs)
+    def keys(self, verbose=False) -> 'List': return List(list(self.__dict__.keys())) if not verbose else install_n_import("tqdm").tqdm(self.__dict__.keys())
+    def values(self, verbose=False) -> 'List': return List(list(self.__dict__.values())) if not verbose else install_n_import("tqdm").tqdm(self.__dict__.values())
+    def items(self, verbose=False, desc="") -> 'List': return List(self.__dict__.items()) if not verbose else install_n_import("tqdm").tqdm(self.__dict__.items(), desc=desc)
+    def get(self, key=None, default=None, strict=False, keys=None) -> 'List': return List([self.__dict__.get(key, default) if not strict else self[key] for key in (keys if keys is not None else [])]) if keys is not None else (self.__dict__.get(key, default) if not strict else self[key])
+    def apply2keys(self, kv_func, verbose=False, desc="") -> 'Struct': return Struct({kv_func(key, val): val for key, val in self.items(verbose=verbose, desc=desc)})
+    def apply2values(self, kv_func, verbose=False, desc="") -> 'Struct': [self.__setitem__(key, kv_func(key, val)) for key, val in self.items(verbose=verbose, desc=desc)]; return self
+    def apply(self, kv_func) -> 'List': return self.items().apply(lambda item: kv_func(item[0], item[1]))
+    def filter(self, kv_func=None) -> 'Struct': return Struct({key: self[key] for key, val in self.items() if kv_func(key, val)})
+    def inverse(self) -> 'Struct': return Struct({v: k for k, v in self.__dict__.items()})
+    def update(self, *args, **kwargs) -> 'Struct': self.__dict__.update(Struct(*args, **kwargs).__dict__); return self
+    def delete(self, key=None, keys=None, kv_func=None) -> 'Struct': [self.__dict__.__delitem__(key) for key in ([key] if key else [] + (keys if keys is not None else []))]; [self.__dict__.__delitem__(k) for k, v in self.items() if kv_func(k, v)] if kv_func is not None else None; return self
+    def _pandas_repr(self, justify, return_str=False, limit=30): res = __import__("pandas").DataFrame(__import__("numpy").array([self.keys(), self.values().apply(lambda x: str(type(x)).split("'")[1]), self.values().apply(lambda x: get_repr(x, justify=justify, limit=limit).replace("\n", " "))]).T, columns=["key", "dtype", "details"]); return res if not return_str else str(res)
+    def print(self, dtype=True, return_str=False, justify=30, as_config=False, as_yaml=False, limit=50, title="", **kwargs):
+        if as_config and not return_str: install_n_import("rich").inspect(self, value=False, title=title, docs=False, sort=False); return self
+        res = f"Empty Struct." if not bool(self) else ((__import__("yaml").dump(self.__dict__) if as_yaml else config(self.__dict__, justify=justify, **kwargs)) if as_yaml or as_config else self._pandas_repr(justify=justify, return_str=False, limit=limit).drop(columns=[] if dtype else ["dtype"]))
+        (install_n_import("rich").print(res.to_markdown()) if "DataFrame" in res.__class__.__name__ else print(res)) if not return_str else None; return str(res) if return_str else self
+    @staticmethod
+    def concat_values(*dicts, orient='list') -> 'Struct': return Struct(__import__("pandas").concat(List(dicts).apply(lambda x: Struct(x).to_dataframe())).to_dict(orient=orient))
+    def plot(self, use_plt=True, title='', xlabel='', ylabel='', **kwargs):
+        if not use_plt: fig = __import__("crocodile.plotly_management").px.line(self.__dict__); fig.show(); return fig
+        else: artist = __import__("crocodile").matplotlib_management.Artist(figname='Structure Plot', **kwargs); artist.plot_dict(self.__dict__, title=title, xlabel=xlabel, ylabel=ylabel); return artist
+
+def set_pandas_display(rows=1000, columns=1000, width=5000, colwidth=40) -> None: import pandas as pd; pd.set_option('display.max_colwidth', colwidth); pd.set_option('display.max_columns', columns); pd.set_option('display.width', width); pd.set_option('display.max_rows', rows)
+def set_pandas_auto_width(): __import__("pandas").set_option('width', 0)  # this way, pandas is told to detect window length and act appropriately.  For fixed width host windows, this is recommended to avoid chaos due to line-wrapping.
+def set_numpy_display(precision=3, linewidth=250, suppress=True, floatmode='fixed', **kwargs) -> None: __import__("numpy").set_printoptions(precision=precision, suppress=suppress, linewidth=linewidth, floatmode=floatmode, **kwargs)
+def config(mydict, sep="\n", justify=15, quotes=False): return sep.join([f"{key:>{justify}} = {repr(val) if quotes else val}" for key, val in mydict.items()])
+def f(str_, limit=float('inf'), justify=50, direc="<") -> str: return f"{(str_[:limit - 4] + '... ' if len(str_) > limit else str_):{direc}{justify}}"
+def eng(): __import__("pandas").set_eng_float_format(accuracy=3, use_eng_prefix=True); __import__("pandas").options.float_format = '{:, .5f}'.format; __import__("pandas").set_option('precision', 7)  # __import__("pandas").set_printoptions(formatter={'float': '{: 0.3f}'.format})
+def outline(array, name="Array", printit=True): str_ = f"{name}. Shape={array.shape}. Dtype={array.dtype}"; print(str_) if printit else None; return str_
+def get_repr(data, justify=15, limit=float('inf'), direc="<") -> str:
+    if (dtype := data.__class__.__name__) in {'list', 'str'}: str_ = data if dtype == 'str' else f"list. length = {len(data)}. " + ("1st item type: " + str(type(data[0])).split("'")[1]) if len(data) > 0 else " "
+    elif dtype in {"DataFrame", "Series"}: str_ = f"Pandas DF: shape = {data.shape}, dtype = {data.dtypes}." if dtype == 'DataFrame' else f"Pandas Series: Length = {len(data)}, Keys = {get_repr(data.keys().to_list())}."
+    else: str_ = f"shape = {data.shape}, dtype = {data.dtype}." if dtype == 'ndarray' else repr(data)
+    return f(str_.replace("\n", ", "), justify=justify, limit=limit, direc=direc)
+def print_string_list(mylist, char_per_row=125, sep=" ", style=str, _counter=0):
+    for item in mylist: print("") if (_counter + len(style(item))) // char_per_row > 0 else print(style(item), end=sep); _counter = len(style(item)) if (_counter + len(style(item))) // char_per_row > 0 else _counter + len(style(item))
+class Display: set_pandas_display = set_pandas_display; set_pandas_auto_width = set_pandas_auto_width; set_numpy_display = set_numpy_display; config = config; f = f; eng = eng; outline = outline; get_repr = get_repr; print_string_list = print_string_list  # or D = type('D', (object, ), dict(set_pandas_display
+
+
+if __name__ == '__main__':
+    pass
```

### Comparing `crocodile-8.40/myresources/crocodile/croshell.py` & `crocodile-9.0/myresources/crocodile/croshell.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,64 +1,64 @@
-
-
-"""Crocodile Shell
-"""
-
-import argparse
-import os
-import random
-from rich import pretty, inspect, progress, traceback, print
-from rich.text import Text
-from rich.console import Console
-
-from crocodile.core import *
-from crocodile.file_management import *
-from crocodile.meta import *
-# import crocodile.environment as env
-from crocodile.matplotlib_management import *
-import crocodile.toolbox as tb
-import numpy as np
-import pandas as pd
-import platform
-
-
-console = Console()
-pretty.install()
-
-_ = f"Python {platform.python_version()} in VE `{os.getenv('VIRTUAL_ENV')}` On {platform.system()}."
-_ = Text(_); _.stylize("bold blue")
-console.rule(_, style="bold red", align="center")
-# link to tutorial or github
-_ = Text(f"Crocodile Shell")
-_.stylize("#93e6c7 on #093006")
-print(_, __import__('crocodile').__version__)
-print("Made with 🐍 | Built with ❤️")
-
-tb.D.set_numpy_display()
-tb.D.set_pandas_display()
-D = Display; L = List; E = Experimental; S = Struct
-
-__ = P(__file__).parent.joinpath("art").search().sample(size=1)[0]
-if platform.system() == "Windows": print(__.read_text())
-else:
-    try:
-        surprise = random.choice([True, True, True, True, False])  # classic art (True) or boxes (False)
-        if surprise:
-            from crocodile.msc.ascii_art import get_art
-            artlib = random.choice(['boxes', 'cowsay'])
-            get_art("crocodile", calliagraphy=None, artlib=artlib, file=(__ := P.tmpfile("croco_art", folder="tmp_arts")), verbose=False)
-        os.system(f"cat {__} | /usr/games/lolcat")  # full path since lolcat might not be in PATH.
-    except: print(__.read_text())
-print("\n\n")
-
-
-def build_parser():
-    parser = argparse.ArgumentParser(description="Generic Parser to launch a script in a separate window.")
-    parser.add_argument("--cmd", "-c", dest="cmd", help="Python command.", default="")
-    args = parser.parse_args()
-    # tb.Struct(args.__dict__).print(as_config=True)
-    print(args.cmd)
-    exec(args.cmd, globals())
-
-
-if __name__ == "__main__":
-    build_parser()
+
+
+"""Crocodile Shell
+"""
+
+import argparse
+import os
+import random
+from rich import pretty, inspect, progress, traceback, print
+from rich.text import Text
+from rich.console import Console
+
+from crocodile.core import *
+from crocodile.file_management import *
+from crocodile.meta import *
+# import crocodile.environment as env
+from crocodile.matplotlib_management import *
+import crocodile.toolbox as tb
+import numpy as np
+import pandas as pd
+import platform
+
+
+console = Console()
+pretty.install()
+
+_ = f"Python {platform.python_version()} in VE `{os.getenv('VIRTUAL_ENV')}` On {platform.system()}."
+_ = Text(_); _.stylize("bold blue")
+console.rule(_, style="bold red", align="center")
+# link to tutorial or github
+_ = Text(f"Crocodile Shell")
+_.stylize("#93e6c7 on #093006")
+print(_, __import__('crocodile').__version__)
+print("Made with 🐍 | Built with ❤️")
+
+tb.D.set_numpy_display()
+tb.D.set_pandas_display()
+D = Display; L = List; E = Experimental; S = Struct
+
+__ = P(__file__).parent.joinpath("art").search().sample(size=1)[0]
+if platform.system() == "Windows": print(__.read_text())
+else:
+    try:
+        surprise = random.choice([True, True, True, True, False])  # classic art (True) or boxes (False)
+        if surprise:
+            from crocodile.msc.ascii_art import get_art
+            artlib = random.choice(['boxes', 'cowsay'])
+            get_art("crocodile", calliagraphy=None, artlib=artlib, file=(__ := P.tmpfile("croco_art", folder="tmp_arts")), verbose=False)
+        os.system(f"cat {__} | /usr/games/lolcat")  # full path since lolcat might not be in PATH.
+    except: print(__.read_text())
+print("\n\n")
+
+
+def build_parser():
+    parser = argparse.ArgumentParser(description="Generic Parser to launch a script in a separate window.")
+    parser.add_argument("--cmd", "-c", dest="cmd", help="Python command.", default="")
+    args = parser.parse_args()
+    # tb.Struct(args.__dict__).print(as_config=True)
+    print(args.cmd)
+    exec(args.cmd, globals())
+
+
+if __name__ == "__main__":
+    build_parser()
```

### Comparing `crocodile-8.40/myresources/crocodile/deeplearning.py` & `crocodile-9.0/myresources/crocodile/deeplearning.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,770 +1,770 @@
-
-import crocodile.toolbox as tb
-from crocodile.matplotlib_management import ImShow, FigureSave
-import numpy as np
-import pandas as pd
-from abc import ABC
-from typing import Generic, TypeVar
-import enum
-from tqdm import tqdm
-import copy
-
-
-# %% ========================== DeepLearning Accessories =================================
-
-BM = TypeVar("BM", bound="BaseModel")
-DR = TypeVar("DR", bound="DataReader")
-HPM = TypeVar("HPM", bound="HyperParam")
-
-
-class Device(enum.Enum):
-    gpu0 = 'gpu0'
-    gpu1 = 'gpu1'
-    cpu = 'cpu'
-    two_gpus = '2gpus'
-    auto = 'auto'
-
-
-class HyperParam(tb.Struct):
-    """Use this class to organize model hyperparameters:
-    * one place to control everything: a control panel.
-    * When doing multiple experiments, one command in console reminds you of settings used in that run (hp.__dict__).
-    * Ease of saving settings of experiments! and also replicating it later.
-    """
-    subpath = tb.P('metadata/hyper_param')  # location within model directory where this will be saved.
-
-    def __init__(self, **kwargs):
-        super().__init__(
-            # ==================== Enviroment =========================
-            name='default_model_name_' + tb.randstr(),
-            root=tb.P.tmp(folder="tmp_models"),
-            pkg_name='tensorflow',
-            device_name=Device.gpu0,
-            # ===================== Data ==============================
-            seed=234,
-            shuffle=True,
-            precision='float32',
-            # ===================== Model =============================
-            # depth = 3
-            # ===================== Training ==========================
-            test_split=0.2,  # test split
-            learning_rate=0.0005,
-            batch_size=32,
-            epochs=30,
-        )
-        self._configured = False
-        self.device_name = None
-        self.save_type = ["data", "obj", "both"][-1]
-        self.update(**kwargs)
-
-    def save(self, **kwargs):
-        self.save_dir.joinpath(self.subpath / 'hparams.txt').create(parents_only=True).write_text(str(self))
-        if self.save_type in {"data", "both"}: super(HyperParam, self).save(path=self.save_dir.joinpath(self.subpath / "hparams.HyperParam.dat.pkl"), add_suffix=False, data_only=True, desc="")
-        # if self.save_type in {"obj", "both"}: super(HyperParam, self).save(path=self.save_dir.joinpath(self.subpath / "hparams.HyperParam.pkl"), add_suffix=False, data_only=False, desc="")
-
-    @classmethod
-    def from_saved_data(cls, path, *args, **kwargs): return super(HyperParam, cls).from_saved_data(tb.P(path) / cls.subpath / "hparams.HyperParam.dat.pkl", *args, **kwargs)
-    def __repr__(self, **kwargs): return "HParams Object with specs:\n" + tb.Struct(self.__dict__).print(as_config=True, return_str=True)
-    @property
-    def pkg(self): return __import__("tensorflow") if self.pkg_name == "tensorflow" else (__import__("torch") if self.pkg_name == "torch" else ValueError(f"pkg_name must be either `tensorflow` or `torch`"))
-    @property
-    def save_dir(self) -> tb.P: return (tb.P(self.root) / self.name).create()
-
-    @property
-    def device(self):
-        handle = self.pkg
-        if handle.__name__ == 'tensorflow':
-            """
-            To disable gpu, here's one way: # before importing tensorflow do this:
-            if device == 'cpu':
-                os.environ["CUDA_VISIBLE_DEVICES"] = "-1"
-            handle.device(device)  # used as context, every tensor constructed and every computation takes place therein
-            For more manual control, use .cpu() and .gpu('0') .gpu('1') attributes.
-            """
-            devices = handle.config.experimental.list_physical_devices('CPU')
-            devices += handle.config.experimental.list_physical_devices('GPU')
-            device_dict = dict(zip(['cpu', 'gpu0', 'gpu1'], devices))
-            if self.device_name is Device.auto: chosen_device = Device.gpu0 if len(devices) > 1 else Device.cpu
-            else: chosen_device = self.device_name
-            device_str = chosen_device.value if 1 > 0 else "haha"
-            if device_str not in device_dict.keys():
-                print(f"This machine has no such a device to be chosen! ({device_str})\n" * 10)
-                device_str = "cpu"  # Revert to cpu, keep going, instead of throwing an error.
-            try:
-                device = device_dict[device_str]
-                return device
-            except KeyError:  # 2gpus not a key in the dict.
-                assert len(handle.config.experimental.get_visible_devices()) > 2
-                mirrored_strategy = handle.distribute.MirroredStrategy()
-                return mirrored_strategy
-
-        elif handle.__name__ == 'torch':
-            device = self.device_name
-            if device is Device.auto: return handle.device('cuda:0') if handle.cuda.is_available() else handle.device('cpu')
-            elif device is Device.cpu: return handle.device('cpu')
-            elif device is Device.gpu0:
-                assert handle.cuda.device_count() > 0, f"GPU {device} not available"
-                return handle.device('cuda:0')
-            elif device is Device.gpu1:
-                assert handle.cuda.device_count() > 1, f"GPU {device} not available"
-                return handle.device('cuda:1')
-            # How to run Torch model on 2 GPUs ?
-        else: raise NotImplementedError(f"I don't know how to configure devices for this package {handle}")
-
-    def config_device(self):
-        """
-        """
-        handle = self.pkg
-        device_str = self.device_name.value
-        device = self.device
-        if handle.__name__ == 'torch': return None
-        try:
-            # Now we want only one device to be seen:
-            if device_str in ['gpu0', 'gpu1']:
-                limit_memory = True
-                if limit_memory:  # memory growth can only be limited for GPU devices.
-                    handle.config.experimental.set_memory_growth(device, True)
-                handle.config.experimental.set_visible_devices(device, 'GPU')  # will only see this device
-                # logical_gpus = handle.config.experimental.list_logical_devices('GPU')
-                # now, logical gpu is created only for visible device
-                # print(len(devices), "Physical devices,", len(logical_gpus), "Logical GPU")
-            else:  # for cpu devices, we want no gpu to be seen:
-                handle.config.experimental.set_visible_devices([], 'GPU')  # will only see this device
-                # logical_gpus = handle.config.experimental.list_logical_devices('GPU')
-                # now, logical gpu is created only for visible device
-                # print(len(devices), "Physical devices,", len(logical_gpus), "Logical GPU")
-        except AssertionError as e:
-            print(e)
-            print(f"Trying again with auto-device {Device.auto}")
-            self.device_name = Device.auto
-            self.config_device()
-        except ValueError: print("Cannot set memory growth on non-GPU devices")
-        except RuntimeError as e:
-            print(e)
-            print(f"Device already configured, skipping ... ")
-
-
-class DataReader(tb.Base):
-    subpath = tb.P("metadata/data_reader")
-    """This class holds the dataset for training and testing. However, it also holds meta data for preprocessing
-    and postprocessing. The latter is essential at inference time_produced, but the former need not to be saved. As such,
-    at save time_produced, this class only remember the attributes inside `.specs` `Struct`. Thus, whenever encountering
-    such type of data, make sure to keep them inside that `Struct`. Lastly, for convenience purpose, the class has
-    implemented a fallback `getattr` method that allows accessing those attributes from the class data_only, without the 
-    need to reference `.dataspects`.
-    """
-    def __init__(self, hp: Generic[HPM] = None, specs=None, split=None, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.hp = hp
-        self.split = split
-        self.plotter = None
-        # attributes to be saved.
-        self.specs = specs if specs else tb.Struct()
-        self.ip_strings = None  # e.g.: ["x1", "x2"]
-        self.op_strings = None  # e.g.: ["y1", "y2"]
-        self.other_strings = None  # e.g.: indices or names
-
-        # dataframes
-        self.scaler = None
-        self.imputer = None
-        self.cols_ordinal = None
-        self.cols_onehot = None
-        self.cols_numerical = None
-        self.encoder_onehot = None
-        self.encoder_ordinal = None
-
-    def save(self, path=None, *args, **kwargs):
-        base = (tb.P(path) if path is not None else self.hp.save_dir).joinpath(self.subpath).create()
-        if self.hp.save_type in {"data", "both"}: super(DataReader, self).save(path=base / "data_reader.DataReader.dat.pkl", add_suffix=False, data_only=True)
-        # if self.hp.save_type in {"obj", "both"}: super(DataReader, self).save(path=base / "data_reader.DataReader.pkl", add_suffix=False, data_only=False)
-
-    @classmethod
-    def from_saved_data(cls, path, *args, **kwargs): return super(DataReader, cls).from_saved_data(tb.P(path) / cls.subpath / "data_reader.DataReader.dat.pkl", *args, **kwargs)
-    def __getstate__(self):
-        items = ["specs", "scaler", "imputer", "ip_strings", "op_strings", "other_strings", "cols_numerical", "cols_ordinal", "cols_onehot", "encoder_onehot", "encoder_ordinal"]
-        return dict(zip(items, [getattr(self, item) for item in items]))
-    def __setstate__(self, state): return self.__dict__.update(state)
-    def __repr__(self): return f"DataReader Object with these keys: \n" + tb.Struct(self.__dict__).print(as_config=False, return_str=True)
-
-    def split_the_data(self, *args, ip_strings=None, op_strings=None, others_string=None, **kwargs):
-        from sklearn.model_selection import train_test_split
-        result = train_test_split(*args, test_size=self.hp.test_split, shuffle=self.hp.shuffle, random_state=self.hp.seed, **kwargs)
-        self.split = tb.Struct(train_loader=None, test_loader=None)
-        if ip_strings is None:
-            ip_strings = [f"x_{i}" for i in range(len(args)-1)]
-            if len(ip_strings) == 1: ip_strings = ["x"]
-        self.ip_strings = ip_strings
-        if op_strings is None: op_strings = ["y"]
-        self.op_strings = op_strings
-        if others_string is None: others_string = []
-        self.other_strings = others_string
-        strings = ip_strings + op_strings + others_string
-        self.specs.ip_shapes = []  # useful info for instantiating models.
-        self.specs.op_shapes = []
-        self.specs.other_shapes = []
-
-        for an_arg, key in zip(args, strings):
-            a_shape = an_arg.iloc[0].shape if type(an_arg) in {pd.DataFrame, pd.Series} else np.array(an_arg[0]).shape
-            if key in ip_strings: self.specs.ip_shapes.append(a_shape)
-            elif key in op_strings: self.specs.op_shapes.append(a_shape)
-            elif key in others_string: self.specs.other_shapes.append(a_shape)
-        self.split.update({astring + '_train': result[ii * 2] for ii, astring in enumerate(strings)})
-        self.split.update({astring + '_test': result[ii * 2 + 1] for ii, astring in enumerate(strings)})
-        print(f"================== Training Data Split ===========================")
-        self.split.print()
-
-    def get_data_strings(self, which_data="ip", which_split="train"):
-        strings = {"op": self.op_strings, "ip": self.ip_strings, "others": self.other_strings}[which_data]
-        keys_ip = [item + f"_{which_split}" for item in strings]
-        return keys_ip
-
-    def sample_dataset(self, aslice=None, indices=None, use_slice=False, split="test", size=None):
-        assert self.split is not None, f"No dataset is loaded to DataReader, .split attribute is empty. Consider using `.load_training_data()` method."
-        keys_ip = self.get_data_strings(which_data="ip", which_split=split)
-        keys_op = self.get_data_strings(which_data="op", which_split=split)
-        keys_others = self.get_data_strings(which_data="others", which_split=split)
-        ds_size = len(self.split[keys_ip[0]])
-        select_size = size or self.hp.batch_size
-        start_idx = np.random.choice(ds_size - select_size)
-
-        if indices is not None: selection = indices
-        elif aslice is not None: selection = aslice
-        elif use_slice: selection = slice(start_idx, start_idx + select_size)  # ragged tensors don't support indexing, this can be handy in that case.
-        else: selection = np.random.choice(ds_size, size=select_size, replace=False)
-
-        x, y, others = [], [], []
-        for idx, key in zip([0] * len(keys_ip) + [1] * len(keys_op) + [2] * len(keys_others), keys_ip + keys_op + keys_others):
-            tmp = self.split[key]
-            item = tmp.iloc[selection] if type(tmp) in {pd.DataFrame, pd.Series} else tmp[selection]
-            if idx == 0: x.append(item)
-            elif idx == 1: y.append(item)
-            else: others.append(item)
-        x = x[0] if len(self.ip_strings) == 1 else x
-        y = y[0] if len(self.op_strings) == 1 else y
-        others = others[0] if len(self.other_strings) == 1 else others
-        if len(others) == 0:
-            # others = np.arange(len(x if len(self.ip_strings) == 1 else x[0]))
-            if type(selection) is slice:
-                others = np.arange(*selection.indices(10000000000000))
-            else:
-                others = selection
-        return x, y, others
-
-    def get_random_inputs_outputs(self, ip_shapes=None, op_shapes=None):
-        if ip_shapes is None: ip_shapes = self.specs.ip_shapes
-        if op_shapes is None: op_shapes = self.specs.op_shapes
-        dtype = self.hp.precision if hasattr(self.hp, "precision") else "float32"
-        x = [np.random.randn(*((self.hp.batch_size,) + ip_shape)).astype(dtype) for ip_shape in ip_shapes]
-        y = [np.random.randn(*((self.hp.batch_size,) + op_shape)).astype(dtype) for op_shape in op_shapes]
-        x = x[0] if len(self.ip_strings) == 1 else x
-        y = y[0] if len(self.op_strings) == 1 else y
-        return x, y
-
-    def profile_dataframe(self, df, file=None, silent=False, suffix="", explorative=True):
-        profile_report = tb.install_n_import("pandas_profiling").ProfileReport
-        # from import ProfileReport  # also try pandasgui  # import statement is kept inside the function due to collission with matplotlib
-        file = file or self.hp.save_dir.joinpath(self.subpath, f"pandas_profile_report_{suffix}.html").create(parents_only=True)
-        profile_report(df, title="Pandas Profiling Report", explorative=explorative).to_file(file, silent=silent)
-        return file
-    def open_dataframe_profile(self): self.hp.save_dir.joinpath(self.subpath, "pandas_profile_report.html")()
-
-    def encode(self, df: pd.DataFrame) -> pd.DataFrame:
-        """Converts the dataframe to numerical format. Missing values are encoded as `pd.NA`, otherwise, encoders will fail to handle them."""
-        df[self.cols_ordinal] = self.encoder_ordinal.transform(df[self.cols_ordinal])
-        tmp = self.encoder_onehot.transform(df[self.cols_onehot])
-        df.drop(columns=self.cols_onehot, inplace=True)
-        df[self.encoder_onehot.get_feature_names_out()] = tmp
-        df[self.cols_numerical] = df[self.cols_numerical].to_numpy().astype(self.hp.precision)
-        return df
-
-    def impute_standardize(self, df: pd.DataFrame) -> pd.DataFrame:
-        df.fillna(np.nan, inplace=True)  # SKlearn Imputer only works with Numpy's np.nan, as opposed to Pandas' pd.NA
-        columns = df.columns
-        df = self.imputer.transform(df)
-        df = self.scaler.transform(pd.DataFrame(df, columns=columns))
-        return pd.DataFrame(df, columns=columns)
-
-    def preprocess(self, *args, **kwargs): _ = args, kwargs, self; return args[0]  # acts like identity.
-    def postprocess(self, *args, **kwargs): _ = args, kwargs, self; return args[0]  # acts like identity
-
-    def standardize(self):
-        assert self.split is not None, "Load up the data first before you standardize it."
-        from sklearn.preprocessing import StandardScaler
-        self.scaler = StandardScaler()
-        self.split.x_train = self.scaler.fit_transform(self.split.x_train)
-        self.split.x_test = self.scaler.transform(self.split.x_test)
-
-    def image_viz(self, pred, gt=None, names=None, **kwargs):
-        """
-        Assumes numpy inputs
-        """
-        if gt is None: self.plotter = ImShow(pred, labels=None, sup_titles=names, origin='lower', **kwargs)
-        else: self.plotter = ImShow(pred, gt, labels=['Reconstruction', 'Ground Truth'], sup_titles=names, origin='lower', **kwargs)
-
-    def viz(self, *args, **kwargs):
-        """Implement here how you would visualize a batch of input and ouput pair. Assume Numpy arguments rather than tensors."""
-        _ = self, args, kwargs
-        return None
-
-
-class BaseModel(ABC):
-    """My basic model. It implements the following methods:
-
-    * :func:`BaseModel.preprocess` This should convert to tensors as appropriate for the model.
-    * :func:`BaseModel.postprocess` This method should convert back to numpy arrays.
-    * :func:`BaseModel.infer` This method expects processed input and only forwards through the model
-    * :func:`BaseModel.predict` expects a processed input, uese infer and does postprocessing.
-    * :func:`BaseModel.predict_from_s` reads, preprocess, then uses predict method.
-    * :func:`BseModel.evaluate` Expects processed input and internally calls infer and postprocess methods.
-
-    Functionally or Sequentually built models are much more powerful than Subclassed models. They are faster, have more features, can be plotted, serialized, correspond to computational graphs etc.
-    """
-    # @abstractmethod
-    def __init__(self, hp: Generic[HPM] = None, data: Generic[BM] = None, model=None, compiler=None, history=None):
-        self.hp = hp  # should be populated upon instantiation.
-        self.model = model  # should be populated upon instantiation.
-        self.data = data  # should be populated upon instantiation.
-        self.compiler = compiler  # Struct with .losses, .metrics and .optimizer.
-        self.history = tb.List() if history is None else history  # should be populated in fit method, or loaded up.
-        self.plotter = FigureSave.NullAuto
-        self.fig = None
-        self.kwargs = None
-        self.tmp = None
-
-    def compile(self, loss=None, optimizer=None, metrics=None, compile_model=True, **kwargs):
-        """ Updates compiler attributes. This acts like a setter.
-        .. note:: * this method is as good as setting attributes of `compiler` directly in case of PyTorch.
-                  * In case of TF, this is not the case as TF requires actual futher different
-                    compilation before changes take effect.
-        Remember:
-        * Must be run prior to fit method.
-        * Can be run only after defining model attribute.
-        """
-        pkg = self.hp.pkg
-        if self.hp.pkg_name == 'tensorflow':
-            if loss is None: loss = pkg.keras.losses.MeanSquaredError()
-            if optimizer is None: optimizer = pkg.keras.optimizers.Adam(self.hp.learning_rate)
-            if metrics is None: metrics = []  # [pkg.keras.metrics.MeanSquaredError()]
-        elif self.hp.pkg_name == 'torch':
-            if loss is None: loss = pkg.nn.MSELoss()
-            if optimizer is None: optimizer = pkg.optim.Adam(self.model.parameters(), lr=self.hp.learning_rate)
-            if metrics is None: metrics = []  # [tmp.MeanSquareError()]
-        # Create a new compiler object
-        self.compiler = tb.Struct(loss=loss, optimizer=optimizer, metrics=metrics, **kwargs)
-        # in both cases: pass the specs to the compiler if we have TF framework
-        if self.hp.pkg.__name__ == "tensorflow" and compile_model: self.model.compile(**self.compiler.__dict__)
-
-    def fit(self, viz=True, val_sample_weights=None, **kwargs):
-        x_train = self.data.split.get(keys=self.data.get_data_strings(which_data="ip", which_split="train")).list
-        y_train = self.data.split.get(keys=self.data.get_data_strings(which_data="op", which_split="train")).list
-        x_test = self.data.split.get(keys=self.data.get_data_strings(which_data="ip", which_split="test")).list
-        y_test = self.data.split.get(keys=self.data.get_data_strings(which_data="op", which_split="test")).list
-        x_test = x_test[0] if len(x_test) == 1 else x_test
-        y_test = y_test[0] if len(y_test) == 1 else y_test
-        default_settings = tb.Struct(x=x_train[0] if len(x_train) == 1 else x_train,
-                                     y=y_train[0] if len(y_train) == 1 else y_train,
-                                     validation_data=(x_test, y_test) if val_sample_weights is None else (x_test, y_test, val_sample_weights),
-                                     batch_size=self.hp.batch_size, epochs=self.hp.epochs, verbose=1, shuffle=self.hp.shuffle, callbacks=[])
-        default_settings.update(kwargs)
-        hist = self.model.fit(**default_settings.__dict__)
-        self.history.append(tb.Struct(copy.deepcopy(hist.history)))  # it is paramount to copy, cause source can change.
-        if viz:
-            artist = self.plot_loss()
-            artist.fig.savefig(self.hp.save_dir.joinpath(f"metadata/loss_curve.png").append(index=True).create(parents_only=True))
-        return self
-
-    def switch_to_sgd(self, epochs=10):
-        print(f'Switching the optimizer to SGD. Loss is fixed to {self.compiler.loss}'.center(100, '*'))
-        if self.hp.pkg.__name__ == 'tensorflow': new_optimizer = self.hp.pkg.keras.optimizers.SGD(lr=self.hp.learning_rate * 0.5)
-        else: new_optimizer = self.hp.pkg.optim.SGD(self.model.parameters(), lr=self.hp.learning_rate * 0.5)
-        self.compiler.optimizer = new_optimizer
-        return self.fit(epochs=epochs)
-
-    def switch_to_l1(self, epochs=10):
-        if self.hp.pkg.__name__ == 'tensorflow':
-            self.model.reset_metrics()
-        print(f'Switching the loss to l1. Optimizer is fixed to {self.compiler.optimizer}'.center(100, '*'))
-        if self.hp.pkg.__name__ == 'tensorflow':
-            new_loss = self.hp.pkg.keras.losses.MeanAbsoluteError()
-        else:
-            import crocodile.deeplearning_torch as tmp
-            new_loss = tmp.MeanAbsoluteError()
-        self.compiler.loss = new_loss
-        return self.fit(epochs=epochs)
-
-    def preprocess(self, *args, **kwargs):
-        """Converts an object to a numerical form consumable by the NN."""
-        return self.data.preprocess(*args, **kwargs)
-
-    def postprocess(self, *args, **kwargs): return self.data.postprocess(*args, **kwargs)
-    def __call__(self, *args, **kwargs): return self.model(*args, **kwargs)
-    def viz(self, *args, **kwargs): return self.data.viz(*args, **kwargs)
-    def save_model(self, directory): self.model.save(directory)  # In TF: send only path dir. Save path is saved_model.pb
-    def save_weights(self, directory): self.model.save_weights(directory.joinpath(self.model.name))  # TF: last part of path is file path.
-    @staticmethod
-    def load_model(directory): __import__("tensorflow").keras.models.load_model(directory)  # path to directory. file saved_model.pb is read auto.
-    def load_weights(self, directory): self.model.load_weights(directory.glob('*.data*').__next__().__str__().split('.data')[0])  # requires path to file path.
-    def summary(self):
-        from contextlib import redirect_stdout
-        path = self.hp.save_dir.joinpath("metadata/model_summary.txt").create(parents_only=True)
-        with open(str(path), 'w') as f:
-            with redirect_stdout(f): self.model.summary()
-        return self.model.summary()
-    def config(self): [print(layer.get_config(), "\n==============================") for layer in self.model.layers]; return None
-    def plot_loss(self, *args, **kwargs): return tb.Struct.concat_values(*self.history).plot(*args, title="Loss Curve",
-                                                                                             xlabel="epochs",
-                                                                                             ylabel=self.compiler.loss.name if hasattr(self.compiler.loss, "name") else self.compiler.loss.__name__,
-                                                                                             **kwargs)
-
-    def infer(self, x):
-        """ This method assumes numpy input, datatype-wise and is also preprocessed.
-        NN is put in eval mode.
-        :param x:
-        :return: prediction as numpy
-        """
-        return self.model.predict(x)  # Keras automatically handles special layers, can accept dataframes, and always returns numpy.
-
-    def predict(self, x, **kwargs):
-        """This method assumes preprocessed input. Returns postprocessed output. It is useful at evaluation time with preprocessed test set."""
-        return self.postprocess(self.infer(x), **kwargs)
-
-    def deduce(self, obj, viz=True, **kwargs):
-        """Assumes that contents of the object are in the form of a batch."""
-        preprocessed = self.preprocess(obj, **kwargs)
-        prediction = self.infer(preprocessed)
-        postprocessed = self.postprocess(prediction, **kwargs)
-        result = tb.Struct(input=obj, preprocessed=preprocessed, prediction=prediction, postprocessed=postprocessed)
-        if viz: self.viz(postprocessed, **kwargs)
-        return result
-
-    def evaluate(self, x_test=None, y_test=None, names_test=None, aslice=None, indices=None, use_slice=False, size=None, split="test", viz=True, **kwargs):
-        if x_test is None and y_test is None and names_test is None:
-            x_test, y_test, names_test = self.data.sample_dataset(aslice=aslice, indices=indices, use_slice=use_slice, split=split, size=size)
-        elif names_test is None: names_test = np.arange(len(x_test))
-        # ==========================================================================
-        y_pred = self.infer(x_test)
-        loss_df = self.get_metrics_evaluations(y_pred, y_test)
-        if loss_df is not None:
-            if len(self.data.other_strings) == 1: loss_df[self.data.other_strings[0]] = names_test
-            else:
-                for val, name in zip(names_test, self.data.other_strings): loss_df[name] = val
-        y_pred_pp = self.postprocess(y_pred, per_instance_kwargs=dict(name=names_test), legend="Prediction", **kwargs)
-        y_true_pp = self.postprocess(y_test, per_instance_kwargs=dict(name=names_test), legend="Ground Truth", **kwargs)
-        results = tb.Struct(x=x_test, y_pred=y_pred, y_pred_pp=y_pred_pp, y_true=y_test, y_true_pp=y_true_pp, names=names_test, loss_df=loss_df, )
-        if viz:
-            loss_name = results.loss_df.columns.to_list()[0]  # first loss path
-            loss_label = results.loss_df[loss_name].apply(lambda x: f"{loss_name} = {x}").to_list()
-            names = [f"{aname}. Case: {anindex}" for aname, anindex in zip(loss_label, names_test)]
-            self.fig = self.viz(y_pred_pp, y_true_pp, names=names, **kwargs)
-        return results
-
-    def get_metrics_evaluations(self, prediction, groun_truth) -> pd.DataFrame or None:
-        if self.compiler is None: return None
-        metrics = tb.L([self.compiler.loss]) + self.compiler.metrics
-        loss_dict = dict()
-        for a_metric in metrics:
-            if hasattr(a_metric, "name"): name = a_metric.name
-            elif hasattr(a_metric, "__name__"): name = a_metric.__name__
-            else: name = "unknown_loss_name"
-            # try:  # EAFP vs LBYL: both are duck-typing styles as they ask for what object can do (whether by introspection or trial) as opposed to checking its type.
-            #     path = a_metric.path  # works for subclasses Metrics
-            # except AttributeError: path = a_metric.__name__  # works for functions.
-            loss_dict[name] = []
-            for a_prediction, a_y_test in zip(prediction, groun_truth):
-                if hasattr(a_metric, "reset_states"): a_metric.reset_states()
-                loss = a_metric(y_pred=a_prediction[None], y_true=a_y_test[None])
-                loss_dict[name].append(np.array(loss).item())
-        return pd.DataFrame(loss_dict)
-
-    def save_class(self, weights_only=True, version='0', **kwargs):
-        """Simply saves everything:
-        1. Hparams
-        2. Data specs
-        3. Model architecture or weights depending on the following argument.
-        :param version: Model version, up to the user.
-        :param weights_only: self-explanatory
-        :return:
-        """
-        self.hp.save()  # goes into the meta path.
-        self.data.save()  # goes into the meta path.
-        tb.Save.pickle(obj=self.history, path=self.hp.save_dir / 'metadata/history.pkl', verbose=True, desc="Training History")  # goes into the meta path.
-        try: tb.Experimental.generate_readme(self.hp.save_dir, obj=self.__class__, **kwargs)
-        except Exception as ex: print(ex)  # often fails because model is defined in main during experiments.
-        save_dir = self.hp.save_dir.joinpath(f'{"weights" if weights_only else "model"}_save_v{version}').create()  # model save goes into data path.
-        if weights_only: self.save_weights(save_dir)
-        else: self.save_model(save_dir)
-        print(f'SAVED Model Class @ {self.hp.save_dir.as_uri()}')
-        return self.hp.save_dir
-
-    @classmethod
-    def from_class_weights(cls, path, hparam_class=None, data_class=None, device_name=None, verbose=True):
-        path = tb.P(path)
-        if hparam_class is not None: hp_obj = hparam_class.from_saved_data(path)
-        else: hp_obj = (path / HyperParam.subpath + "hparams.HyperParam.pkl").readit()
-        if device_name: hp_obj.device_name = device_name
-        if data_class is not None: d_obj = data_class.from_saved_data(path, hp=hp_obj)
-        else: d_obj = (path / DataReader.subpath / "data_reader.DataReader.pkl").readit()
-        if hp_obj.root != path.parent: hp_obj.root, hp_obj.name = path.parent, path.name  # if user moved the file to somewhere else, this will help alighment with new directory in case a modified version is to be saved.
-        d_obj.hp = hp_obj
-        model_obj = cls(hp_obj, d_obj)
-        model_obj.load_weights(path.search('*_save_*')[0])
-        model_obj.history = (path / "metadata/history.pkl").readit(notfound=tb.L())
-        print(f"LOADED {model_obj.__class__}: {model_obj.hp.name}") if verbose else None
-        return model_obj
-
-    @classmethod
-    def from_class_model(cls, path):
-        path = tb.P(path)
-        data_obj = DataReader.from_saved_data(path)
-        hp_obj = HyperParam.from_saved_data(path)
-        model_obj = cls.load_model(path.search('*_save_*')[0])  # static method.
-        wrapper_class = cls(hp_obj, data_obj, model_obj)
-        return wrapper_class
-
-    def plot_model(self, dpi=150, **kwargs):  # alternative viz via tf2onnx then Netron.
-        import tensorflow as tf
-        path = self.hp.save_dir / 'model_plot.png'
-        tf.keras.utils.plot_model(self.model, to_file=path, show_shapes=True, show_layer_names=True, show_layer_activations=True, show_dtype=True, expand_nested=True, dpi=dpi, **kwargs)
-        print(f"Successfully plotted the model @ {path.as_uri()}")
-        return path
-
-    def build(self, sample_dataset=False, ip_shapes=None, ip=None, verbose=True):
-        """ Building has two main uses.
-        * Useful to baptize the model, especially when its layers are built lazily. Although this will eventually happen as the first batch goes in. This is a must before showing the summary of the model.
-        * Doing sanity check about shapes when designing model.
-        * Sanity check about values and ranges when random normal input is fed.
-        :param sample_dataset:
-        :param ip_shapes:
-        :param ip:
-        :param verbose:
-        :return:
-        """
-        keys_ip = self.data.get_data_strings(which_data="ip", which_split="test")
-        keys_op = self.data.get_data_strings(which_data="op", which_split="test")
-
-        if ip is None:
-            if sample_dataset: ip, _, _ = self.data.sample_dataset()
-            else: ip, _ = self.data.get_random_inputs_outputs(ip_shapes=ip_shapes)
-        op = self.model(inputs=ip)
-        ops = [op] if len(keys_op) == 1 else op
-        ips = [ip] if len(keys_ip) == 1 else ip
-        if verbose:
-            print("\n")
-            print("Build Test".center(50, '-'))
-            print(f"Input shapes:")
-            tb.Struct.from_keys_values(keys_ip, tb.L(ips).apply(lambda x: x.shape)).print(as_config=True)
-            print(f"Output shape:")
-            tb.Struct.from_keys_values(keys_op, tb.L(ops).apply(lambda x: x.shape)).print(as_config=True)
-            print("\n\nStats on output data for random normal input:")
-            try:
-                res = []
-                for item_str, item_val in zip(keys_ip + keys_op, list(ips) + list(ops)):
-                    a_df = pd.DataFrame(np.array(item_val).flatten()).describe().rename(columns={0: item_str})
-                    res.append(a_df)
-                print(pd.concat(res, axis=1))
-            except Exception as ex:
-                print(f"Could not do stats on outputs and inputs. Error: {ex}")
-            print("Build Test Finished".center(50, '-'))
-            print("\n")
-
-
-class Ensemble(tb.Base):
-    def __init__(self, hp_class: Generic[HPM] = None, data_class: Generic[DR] = None, model_class: Generic[BM] = None, size=10, *args, **kwargs):
-        """
-        :param model_class: Either a class for constructing saved_models or list of saved_models already cosntructed.
-          * In either case, the following methods should be implemented:
-          __init__, load, load_weights, save, save_weights, predict, fit
-          Model constructor should takes everything it needs from self.hp and self.data only.
-          Otherwise, you must pass a list of already constructed saved_models.
-        :param size: size of ensemble
-        """
-        super().__init__(*args, **kwargs)
-        self.__dict__.update(kwargs)
-        self.size = size
-        self.hp_class = hp_class
-        self.data_class = data_class
-        self.model_class = model_class
-        self.models = tb.List()
-        self.data = None  # one data object for all models (so that it can fit in the memory)
-        if hp_class and data_class and model_class:
-            # only generate the dataset once and attach it to the ensemble to be reused by models.
-            self.data = self.data_class(hp_class(), load_trianing_data=True)
-            print("Creating Models".center(100, "="))
-            for i in tqdm(range(size)):
-                hp = self.hp_class()
-                hp.name = str(hp.name) + f'__model__{i}'
-                datacopy = copy.copy(self.data)  # shallow copy
-                datacopy.hp = hp
-                self.models.append(model_class(hp, datacopy))
-        self.performance = None
-
-    @classmethod
-    def from_saved_models(cls, parent_dir, model_class):
-        obj = cls(model_class=model_class, path=parent_dir, size=len(tb.P(parent_dir).search('*__model__*')))
-        obj.models = tb.P(parent_dir).search('*__model__*').apply(model_class.from_class_model)
-        return obj
-
-    @classmethod
-    def from_saved_weights(cls, parent_dir, model_class):
-        obj = cls(model_class=model_class, path=parent_dir, size=len(tb.P(parent_dir).search('*__model__*')))
-        obj.models = tb.P(parent_dir).search('*__model__*').apply(model_class.from_class_weights)
-        return obj
-
-    def fit(self, shuffle_train_test=True, save=True, **kwargs):
-        self.performance = tb.L()
-        for i in range(self.size):
-            print('\n\n', f" Training Model {i} ".center(100, "*"), '\n\n')
-            if shuffle_train_test:
-                self.models[i].hp.seed = np.random.randint(0, 1000)
-                self.data.split_the_data()  # shuffle data (shared among models)
-            self.models[i].fit(**kwargs)
-            self.performance.append(self.models[i].evaluate(idx=slice(0, -1), viz=False))
-            if save:
-                self.models[i].save_class()
-                self.performance.save(self.hp_class.save_dir / "performance.List.pkl")
-        print("\n\n", f" Finished fitting the ensemble ".center(100, ">"), "\n")
-
-    def clear_memory(self): pass  # t.cuda.empty_cache()
-
-
-class Losses:
-    @staticmethod
-    def get_log_square_loss_class():
-        import tensorflow as tf
-
-        class LogSquareLoss(tf.keras.losses.Loss):
-            def __init__(self, *args, **kwargs):
-                super().__init__(*args, **kwargs)
-                self.name = "LogSquareLoss"
-
-            def call(self, y_true, y_pred):
-                _ = self
-                factor = (20 / tf.math.log(tf.convert_to_tensor(10.0, dtype=y_pred.dtype)))
-                return factor * tf.math.log(tf.reduce_mean((y_true - y_pred)**2))
-        return LogSquareLoss
-
-    @staticmethod
-    def get_mean_max_error(tf):
-        """
-        For Tensorflow
-        """
-        class MeanMaxError(tf.keras.metrics.Metric):
-            def __init__(self, name='MeanMaximumError', **kwargs):
-                super(MeanMaxError, self).__init__(name=name, **kwargs)
-                self.mme = self.add_weight(name='mme', initializer='zeros')
-                self.__name__ = name
-
-            def update_state(self, y_true, y_pred, sample_weight=None): self.mme.assign(tf.reduce_mean(tf.reduce_max(sample_weight or 1.0 * tf.abs(y_pred - y_true), axis=1)))
-            def result(self): return self.mme
-            def reset_states(self): self.mme.assign(0.0)
-        return MeanMaxError
-
-
-class HPTuning:
-    def __init__(self):
-        # ================== Tuning ===============
-        from tensorboard.plugins.hparams import api as hpt
-        self.hpt = hpt
-        import tensorflow as tf
-        self.pkg = tf
-        self.dir = None
-        self.params = tb.List()
-        self.acc_metric = None
-        self.metrics = None
-
-    @staticmethod
-    def help():
-        """Steps of use: subclass this and do the following:
-        * Set directory attribute.
-        * set params
-        * set accuracy metric
-        * generate writer.
-        * implement run method.
-        * run loop method.
-        * in the command line, run `tensorboard --logdir <self.dir>`
-        """
-        pass
-
-    def run(self, param_dict):
-        _, _ = self, param_dict
-        # should return a result that you want to maximize
-        return _
-
-    def gen_writer(self):
-        import tensorflow as tf
-        with tf.summary.create_file_writer(str(self.dir)).as_default():
-            self.hpt.hparams_config(
-                hparams=self.params,
-                metrics=self.metrics)
-
-    def loop(self):
-        import itertools
-        counter = -1
-        tmp = self.params.list[0].domain.values
-        for combination in itertools.product(*[tmp]):
-            counter += 1
-            param_dict = dict(zip(self.params.list, combination))
-            with self.pkg.summary.create_file_writer(str(self.dir / f"run_{counter}")).as_default():
-                self.hpt.hparams(param_dict)  # record the values used in this trial
-                accuracy = self.run(param_dict)
-                self.pkg.summary.scalar(self.acc_metric, accuracy, step=1)
-
-    def optimize(self): self.gen_writer(); self.loop()
-
-
-class KerasOptimizer:
-    def __init__(self, d):
-        self.data = d
-        self.tuner = None
-
-    def __call__(self, ktp): pass
-
-    def tune(self):
-        kt = tb.core.install_n_import("kerastuner")
-        self.tuner = kt.Hyperband(self, objective='loss', max_epochs=10, factor=3, directory=tb.P.tmp('my_dir'), project_name='intro_to_kt')
-
-
-def batcher(func_type='function'):
-    if func_type == 'method':
-        def batch(func):
-            # from functools import wraps
-            # @wraps(func)
-            def wrapper(self, x, *args, per_instance_kwargs=None, **kwargs):
-                output = []
-                for counter, item in enumerate(x):
-                    mykwargs = {key: value[counter] for key, value in per_instance_kwargs.items()} if per_instance_kwargs is not None else {}
-                    output.append(func(self, item, *args, **mykwargs, **kwargs))
-                return np.array(output)
-            return wrapper
-        return batch
-    elif func_type == 'class': raise NotImplementedError
-    elif func_type == 'function':
-        class Batch(object):
-            def __init__(self, func): self.func = func
-            def __call__(self, x, **kwargs): return np.array([self.func(item, **kwargs) for item in x])
-        return Batch
-
-
-def batcherv2(func_type='function', order=1):
-    if func_type == 'method':
-        def batch(func):
-            # from functools import wraps
-            # @wraps(func)
-            def wrapper(self, *args, **kwargs): return np.array([func(self, *items, *args[order:], **kwargs) for items in zip(*args[:order])])
-            return wrapper
-        return batch
-    elif func_type == 'class': raise NotImplementedError
-    elif func_type == 'function':
-        class Batch(object):
-            def __int__(self, func): self.func = func
-            def __call__(self, *args, **kwargs): return np.array([self.func(self, *items, *args[order:], **kwargs) for items in zip(*args[:order])])
-        return Batch
-
-
-def get_template():
-    tb.install_n_import("clipboard").copy(tb.P(__file__).parent.joinpath("msc/dl_template.py").read_text(encoding="utf-8"))
-    print("Copied to clipboard")
-
-
-if __name__ == '__main__':
-    pass
+
+import crocodile.toolbox as tb
+from crocodile.matplotlib_management import ImShow, FigureSave
+import numpy as np
+import pandas as pd
+from abc import ABC
+from typing import Generic, TypeVar
+import enum
+from tqdm import tqdm
+import copy
+
+
+# %% ========================== DeepLearning Accessories =================================
+
+BM = TypeVar("BM", bound="BaseModel")
+DR = TypeVar("DR", bound="DataReader")
+HPM = TypeVar("HPM", bound="HyperParam")
+
+
+class Device(enum.Enum):
+    gpu0 = 'gpu0'
+    gpu1 = 'gpu1'
+    cpu = 'cpu'
+    two_gpus = '2gpus'
+    auto = 'auto'
+
+
+class HyperParam(tb.Struct):
+    """Use this class to organize model hyperparameters:
+    * one place to control everything: a control panel.
+    * When doing multiple experiments, one command in console reminds you of settings used in that run (hp.__dict__).
+    * Ease of saving settings of experiments! and also replicating it later.
+    """
+    subpath = tb.P('metadata/hyper_param')  # location within model directory where this will be saved.
+
+    def __init__(self, **kwargs):
+        super().__init__(
+            # ==================== Enviroment =========================
+            name='default_model_name_' + tb.randstr(),
+            root=tb.P.tmp(folder="tmp_models"),
+            pkg_name='tensorflow',
+            device_name=Device.gpu0,
+            # ===================== Data ==============================
+            seed=234,
+            shuffle=True,
+            precision='float32',
+            # ===================== Model =============================
+            # depth = 3
+            # ===================== Training ==========================
+            test_split=0.2,  # test split
+            learning_rate=0.0005,
+            batch_size=32,
+            epochs=30,
+        )
+        self._configured = False
+        self.device_name = None
+        self.save_type = ["data", "obj", "both"][-1]
+        self.update(**kwargs)
+
+    def save(self, **kwargs):
+        self.save_dir.joinpath(self.subpath / 'hparams.txt').create(parents_only=True).write_text(str(self))
+        if self.save_type in {"data", "both"}: super(HyperParam, self).save(path=self.save_dir.joinpath(self.subpath / "hparams.HyperParam.dat.pkl"), add_suffix=False, data_only=True, desc="")
+        # if self.save_type in {"obj", "both"}: super(HyperParam, self).save(path=self.save_dir.joinpath(self.subpath / "hparams.HyperParam.pkl"), add_suffix=False, data_only=False, desc="")
+
+    @classmethod
+    def from_saved_data(cls, path, *args, **kwargs): return super(HyperParam, cls).from_saved_data(tb.P(path) / cls.subpath / "hparams.HyperParam.dat.pkl", *args, **kwargs)
+    def __repr__(self, **kwargs): return "HParams Object with specs:\n" + tb.Struct(self.__dict__).print(as_config=True, return_str=True)
+    @property
+    def pkg(self): return __import__("tensorflow") if self.pkg_name == "tensorflow" else (__import__("torch") if self.pkg_name == "torch" else ValueError(f"pkg_name must be either `tensorflow` or `torch`"))
+    @property
+    def save_dir(self) -> tb.P: return (tb.P(self.root) / self.name).create()
+
+    @property
+    def device(self):
+        handle = self.pkg
+        if handle.__name__ == 'tensorflow':
+            """
+            To disable gpu, here's one way: # before importing tensorflow do this:
+            if device == 'cpu':
+                os.environ["CUDA_VISIBLE_DEVICES"] = "-1"
+            handle.device(device)  # used as context, every tensor constructed and every computation takes place therein
+            For more manual control, use .cpu() and .gpu('0') .gpu('1') attributes.
+            """
+            devices = handle.config.experimental.list_physical_devices('CPU')
+            devices += handle.config.experimental.list_physical_devices('GPU')
+            device_dict = dict(zip(['cpu', 'gpu0', 'gpu1'], devices))
+            if self.device_name is Device.auto: chosen_device = Device.gpu0 if len(devices) > 1 else Device.cpu
+            else: chosen_device = self.device_name
+            device_str = chosen_device.value if 1 > 0 else "haha"
+            if device_str not in device_dict.keys():
+                print(f"This machine has no such a device to be chosen! ({device_str})\n" * 10)
+                device_str = "cpu"  # Revert to cpu, keep going, instead of throwing an error.
+            try:
+                device = device_dict[device_str]
+                return device
+            except KeyError:  # 2gpus not a key in the dict.
+                assert len(handle.config.experimental.get_visible_devices()) > 2
+                mirrored_strategy = handle.distribute.MirroredStrategy()
+                return mirrored_strategy
+
+        elif handle.__name__ == 'torch':
+            device = self.device_name
+            if device is Device.auto: return handle.device('cuda:0') if handle.cuda.is_available() else handle.device('cpu')
+            elif device is Device.cpu: return handle.device('cpu')
+            elif device is Device.gpu0:
+                assert handle.cuda.device_count() > 0, f"GPU {device} not available"
+                return handle.device('cuda:0')
+            elif device is Device.gpu1:
+                assert handle.cuda.device_count() > 1, f"GPU {device} not available"
+                return handle.device('cuda:1')
+            # How to run Torch model on 2 GPUs ?
+        else: raise NotImplementedError(f"I don't know how to configure devices for this package {handle}")
+
+    def config_device(self):
+        """
+        """
+        handle = self.pkg
+        device_str = self.device_name.value
+        device = self.device
+        if handle.__name__ == 'torch': return None
+        try:
+            # Now we want only one device to be seen:
+            if device_str in ['gpu0', 'gpu1']:
+                limit_memory = True
+                if limit_memory:  # memory growth can only be limited for GPU devices.
+                    handle.config.experimental.set_memory_growth(device, True)
+                handle.config.experimental.set_visible_devices(device, 'GPU')  # will only see this device
+                # logical_gpus = handle.config.experimental.list_logical_devices('GPU')
+                # now, logical gpu is created only for visible device
+                # print(len(devices), "Physical devices,", len(logical_gpus), "Logical GPU")
+            else:  # for cpu devices, we want no gpu to be seen:
+                handle.config.experimental.set_visible_devices([], 'GPU')  # will only see this device
+                # logical_gpus = handle.config.experimental.list_logical_devices('GPU')
+                # now, logical gpu is created only for visible device
+                # print(len(devices), "Physical devices,", len(logical_gpus), "Logical GPU")
+        except AssertionError as e:
+            print(e)
+            print(f"Trying again with auto-device {Device.auto}")
+            self.device_name = Device.auto
+            self.config_device()
+        except ValueError: print("Cannot set memory growth on non-GPU devices")
+        except RuntimeError as e:
+            print(e)
+            print(f"Device already configured, skipping ... ")
+
+
+class DataReader(tb.Base):
+    subpath = tb.P("metadata/data_reader")
+    """This class holds the dataset for training and testing. However, it also holds meta data for preprocessing
+    and postprocessing. The latter is essential at inference time_produced, but the former need not to be saved. As such,
+    at save time_produced, this class only remember the attributes inside `.specs` `Struct`. Thus, whenever encountering
+    such type of data, make sure to keep them inside that `Struct`. Lastly, for convenience purpose, the class has
+    implemented a fallback `getattr` method that allows accessing those attributes from the class data_only, without the 
+    need to reference `.dataspects`.
+    """
+    def __init__(self, hp: Generic[HPM] = None, specs=None, split=None, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.hp = hp
+        self.split = split
+        self.plotter = None
+        # attributes to be saved.
+        self.specs = specs if specs else tb.Struct()
+        self.ip_strings = None  # e.g.: ["x1", "x2"]
+        self.op_strings = None  # e.g.: ["y1", "y2"]
+        self.other_strings = None  # e.g.: indices or names
+
+        # dataframes
+        self.scaler = None
+        self.imputer = None
+        self.cols_ordinal = None
+        self.cols_onehot = None
+        self.cols_numerical = None
+        self.encoder_onehot = None
+        self.encoder_ordinal = None
+
+    def save(self, path=None, *args, **kwargs):
+        base = (tb.P(path) if path is not None else self.hp.save_dir).joinpath(self.subpath).create()
+        if self.hp.save_type in {"data", "both"}: super(DataReader, self).save(path=base / "data_reader.DataReader.dat.pkl", add_suffix=False, data_only=True)
+        # if self.hp.save_type in {"obj", "both"}: super(DataReader, self).save(path=base / "data_reader.DataReader.pkl", add_suffix=False, data_only=False)
+
+    @classmethod
+    def from_saved_data(cls, path, *args, **kwargs): return super(DataReader, cls).from_saved_data(tb.P(path) / cls.subpath / "data_reader.DataReader.dat.pkl", *args, **kwargs)
+    def __getstate__(self):
+        items = ["specs", "scaler", "imputer", "ip_strings", "op_strings", "other_strings", "cols_numerical", "cols_ordinal", "cols_onehot", "encoder_onehot", "encoder_ordinal"]
+        return dict(zip(items, [getattr(self, item) for item in items]))
+    def __setstate__(self, state): return self.__dict__.update(state)
+    def __repr__(self): return f"DataReader Object with these keys: \n" + tb.Struct(self.__dict__).print(as_config=False, return_str=True)
+
+    def split_the_data(self, *args, ip_strings=None, op_strings=None, others_string=None, **kwargs):
+        from sklearn.model_selection import train_test_split
+        result = train_test_split(*args, test_size=self.hp.test_split, shuffle=self.hp.shuffle, random_state=self.hp.seed, **kwargs)
+        self.split = tb.Struct(train_loader=None, test_loader=None)
+        if ip_strings is None:
+            ip_strings = [f"x_{i}" for i in range(len(args)-1)]
+            if len(ip_strings) == 1: ip_strings = ["x"]
+        self.ip_strings = ip_strings
+        if op_strings is None: op_strings = ["y"]
+        self.op_strings = op_strings
+        if others_string is None: others_string = []
+        self.other_strings = others_string
+        strings = ip_strings + op_strings + others_string
+        self.specs.ip_shapes = []  # useful info for instantiating models.
+        self.specs.op_shapes = []
+        self.specs.other_shapes = []
+
+        for an_arg, key in zip(args, strings):
+            a_shape = an_arg.iloc[0].shape if type(an_arg) in {pd.DataFrame, pd.Series} else np.array(an_arg[0]).shape
+            if key in ip_strings: self.specs.ip_shapes.append(a_shape)
+            elif key in op_strings: self.specs.op_shapes.append(a_shape)
+            elif key in others_string: self.specs.other_shapes.append(a_shape)
+        self.split.update({astring + '_train': result[ii * 2] for ii, astring in enumerate(strings)})
+        self.split.update({astring + '_test': result[ii * 2 + 1] for ii, astring in enumerate(strings)})
+        print(f"================== Training Data Split ===========================")
+        self.split.print()
+
+    def get_data_strings(self, which_data="ip", which_split="train"):
+        strings = {"op": self.op_strings, "ip": self.ip_strings, "others": self.other_strings}[which_data]
+        keys_ip = [item + f"_{which_split}" for item in strings]
+        return keys_ip
+
+    def sample_dataset(self, aslice=None, indices=None, use_slice=False, split="test", size=None):
+        assert self.split is not None, f"No dataset is loaded to DataReader, .split attribute is empty. Consider using `.load_training_data()` method."
+        keys_ip = self.get_data_strings(which_data="ip", which_split=split)
+        keys_op = self.get_data_strings(which_data="op", which_split=split)
+        keys_others = self.get_data_strings(which_data="others", which_split=split)
+        ds_size = len(self.split[keys_ip[0]])
+        select_size = size or self.hp.batch_size
+        start_idx = np.random.choice(ds_size - select_size)
+
+        if indices is not None: selection = indices
+        elif aslice is not None: selection = aslice
+        elif use_slice: selection = slice(start_idx, start_idx + select_size)  # ragged tensors don't support indexing, this can be handy in that case.
+        else: selection = np.random.choice(ds_size, size=select_size, replace=False)
+
+        x, y, others = [], [], []
+        for idx, key in zip([0] * len(keys_ip) + [1] * len(keys_op) + [2] * len(keys_others), keys_ip + keys_op + keys_others):
+            tmp = self.split[key]
+            item = tmp.iloc[selection] if type(tmp) in {pd.DataFrame, pd.Series} else tmp[selection]
+            if idx == 0: x.append(item)
+            elif idx == 1: y.append(item)
+            else: others.append(item)
+        x = x[0] if len(self.ip_strings) == 1 else x
+        y = y[0] if len(self.op_strings) == 1 else y
+        others = others[0] if len(self.other_strings) == 1 else others
+        if len(others) == 0:
+            # others = np.arange(len(x if len(self.ip_strings) == 1 else x[0]))
+            if type(selection) is slice:
+                others = np.arange(*selection.indices(10000000000000))
+            else:
+                others = selection
+        return x, y, others
+
+    def get_random_inputs_outputs(self, ip_shapes=None, op_shapes=None):
+        if ip_shapes is None: ip_shapes = self.specs.ip_shapes
+        if op_shapes is None: op_shapes = self.specs.op_shapes
+        dtype = self.hp.precision if hasattr(self.hp, "precision") else "float32"
+        x = [np.random.randn(*((self.hp.batch_size,) + ip_shape)).astype(dtype) for ip_shape in ip_shapes]
+        y = [np.random.randn(*((self.hp.batch_size,) + op_shape)).astype(dtype) for op_shape in op_shapes]
+        x = x[0] if len(self.ip_strings) == 1 else x
+        y = y[0] if len(self.op_strings) == 1 else y
+        return x, y
+
+    def profile_dataframe(self, df, file=None, silent=False, suffix="", explorative=True):
+        profile_report = tb.install_n_import("pandas_profiling").ProfileReport
+        # from import ProfileReport  # also try pandasgui  # import statement is kept inside the function due to collission with matplotlib
+        file = file or self.hp.save_dir.joinpath(self.subpath, f"pandas_profile_report_{suffix}.html").create(parents_only=True)
+        profile_report(df, title="Pandas Profiling Report", explorative=explorative).to_file(file, silent=silent)
+        return file
+    def open_dataframe_profile(self): self.hp.save_dir.joinpath(self.subpath, "pandas_profile_report.html")()
+
+    def encode(self, df: pd.DataFrame) -> pd.DataFrame:
+        """Converts the dataframe to numerical format. Missing values are encoded as `pd.NA`, otherwise, encoders will fail to handle them."""
+        df[self.cols_ordinal] = self.encoder_ordinal.transform(df[self.cols_ordinal])
+        tmp = self.encoder_onehot.transform(df[self.cols_onehot])
+        df.drop(columns=self.cols_onehot, inplace=True)
+        df[self.encoder_onehot.get_feature_names_out()] = tmp
+        df[self.cols_numerical] = df[self.cols_numerical].to_numpy().astype(self.hp.precision)
+        return df
+
+    def impute_standardize(self, df: pd.DataFrame) -> pd.DataFrame:
+        df.fillna(np.nan, inplace=True)  # SKlearn Imputer only works with Numpy's np.nan, as opposed to Pandas' pd.NA
+        columns = df.columns
+        df = self.imputer.transform(df)
+        df = self.scaler.transform(pd.DataFrame(df, columns=columns))
+        return pd.DataFrame(df, columns=columns)
+
+    def preprocess(self, *args, **kwargs): _ = args, kwargs, self; return args[0]  # acts like identity.
+    def postprocess(self, *args, **kwargs): _ = args, kwargs, self; return args[0]  # acts like identity
+
+    def standardize(self):
+        assert self.split is not None, "Load up the data first before you standardize it."
+        from sklearn.preprocessing import StandardScaler
+        self.scaler = StandardScaler()
+        self.split.x_train = self.scaler.fit_transform(self.split.x_train)
+        self.split.x_test = self.scaler.transform(self.split.x_test)
+
+    def image_viz(self, pred, gt=None, names=None, **kwargs):
+        """
+        Assumes numpy inputs
+        """
+        if gt is None: self.plotter = ImShow(pred, labels=None, sup_titles=names, origin='lower', **kwargs)
+        else: self.plotter = ImShow(pred, gt, labels=['Reconstruction', 'Ground Truth'], sup_titles=names, origin='lower', **kwargs)
+
+    def viz(self, *args, **kwargs):
+        """Implement here how you would visualize a batch of input and ouput pair. Assume Numpy arguments rather than tensors."""
+        _ = self, args, kwargs
+        return None
+
+
+class BaseModel(ABC):
+    """My basic model. It implements the following methods:
+
+    * :func:`BaseModel.preprocess` This should convert to tensors as appropriate for the model.
+    * :func:`BaseModel.postprocess` This method should convert back to numpy arrays.
+    * :func:`BaseModel.infer` This method expects processed input and only forwards through the model
+    * :func:`BaseModel.predict` expects a processed input, uese infer and does postprocessing.
+    * :func:`BaseModel.predict_from_s` reads, preprocess, then uses predict method.
+    * :func:`BseModel.evaluate` Expects processed input and internally calls infer and postprocess methods.
+
+    Functionally or Sequentually built models are much more powerful than Subclassed models. They are faster, have more features, can be plotted, serialized, correspond to computational graphs etc.
+    """
+    # @abstractmethod
+    def __init__(self, hp: Generic[HPM] = None, data: Generic[BM] = None, model=None, compiler=None, history=None):
+        self.hp = hp  # should be populated upon instantiation.
+        self.model = model  # should be populated upon instantiation.
+        self.data = data  # should be populated upon instantiation.
+        self.compiler = compiler  # Struct with .losses, .metrics and .optimizer.
+        self.history = tb.List() if history is None else history  # should be populated in fit method, or loaded up.
+        self.plotter = FigureSave.NullAuto
+        self.fig = None
+        self.kwargs = None
+        self.tmp = None
+
+    def compile(self, loss=None, optimizer=None, metrics=None, compile_model=True, **kwargs):
+        """ Updates compiler attributes. This acts like a setter.
+        .. note:: * this method is as good as setting attributes of `compiler` directly in case of PyTorch.
+                  * In case of TF, this is not the case as TF requires actual futher different
+                    compilation before changes take effect.
+        Remember:
+        * Must be run prior to fit method.
+        * Can be run only after defining model attribute.
+        """
+        pkg = self.hp.pkg
+        if self.hp.pkg_name == 'tensorflow':
+            if loss is None: loss = pkg.keras.losses.MeanSquaredError()
+            if optimizer is None: optimizer = pkg.keras.optimizers.Adam(self.hp.learning_rate)
+            if metrics is None: metrics = []  # [pkg.keras.metrics.MeanSquaredError()]
+        elif self.hp.pkg_name == 'torch':
+            if loss is None: loss = pkg.nn.MSELoss()
+            if optimizer is None: optimizer = pkg.optim.Adam(self.model.parameters(), lr=self.hp.learning_rate)
+            if metrics is None: metrics = []  # [tmp.MeanSquareError()]
+        # Create a new compiler object
+        self.compiler = tb.Struct(loss=loss, optimizer=optimizer, metrics=metrics, **kwargs)
+        # in both cases: pass the specs to the compiler if we have TF framework
+        if self.hp.pkg.__name__ == "tensorflow" and compile_model: self.model.compile(**self.compiler.__dict__)
+
+    def fit(self, viz=True, val_sample_weights=None, **kwargs):
+        x_train = self.data.split.get(keys=self.data.get_data_strings(which_data="ip", which_split="train")).list
+        y_train = self.data.split.get(keys=self.data.get_data_strings(which_data="op", which_split="train")).list
+        x_test = self.data.split.get(keys=self.data.get_data_strings(which_data="ip", which_split="test")).list
+        y_test = self.data.split.get(keys=self.data.get_data_strings(which_data="op", which_split="test")).list
+        x_test = x_test[0] if len(x_test) == 1 else x_test
+        y_test = y_test[0] if len(y_test) == 1 else y_test
+        default_settings = tb.Struct(x=x_train[0] if len(x_train) == 1 else x_train,
+                                     y=y_train[0] if len(y_train) == 1 else y_train,
+                                     validation_data=(x_test, y_test) if val_sample_weights is None else (x_test, y_test, val_sample_weights),
+                                     batch_size=self.hp.batch_size, epochs=self.hp.epochs, verbose=1, shuffle=self.hp.shuffle, callbacks=[])
+        default_settings.update(kwargs)
+        hist = self.model.fit(**default_settings.__dict__)
+        self.history.append(tb.Struct(copy.deepcopy(hist.history)))  # it is paramount to copy, cause source can change.
+        if viz:
+            artist = self.plot_loss()
+            artist.fig.savefig(self.hp.save_dir.joinpath(f"metadata/loss_curve.png").append(index=True).create(parents_only=True))
+        return self
+
+    def switch_to_sgd(self, epochs=10):
+        print(f'Switching the optimizer to SGD. Loss is fixed to {self.compiler.loss}'.center(100, '*'))
+        if self.hp.pkg.__name__ == 'tensorflow': new_optimizer = self.hp.pkg.keras.optimizers.SGD(lr=self.hp.learning_rate * 0.5)
+        else: new_optimizer = self.hp.pkg.optim.SGD(self.model.parameters(), lr=self.hp.learning_rate * 0.5)
+        self.compiler.optimizer = new_optimizer
+        return self.fit(epochs=epochs)
+
+    def switch_to_l1(self, epochs=10):
+        if self.hp.pkg.__name__ == 'tensorflow':
+            self.model.reset_metrics()
+        print(f'Switching the loss to l1. Optimizer is fixed to {self.compiler.optimizer}'.center(100, '*'))
+        if self.hp.pkg.__name__ == 'tensorflow':
+            new_loss = self.hp.pkg.keras.losses.MeanAbsoluteError()
+        else:
+            import crocodile.deeplearning_torch as tmp
+            new_loss = tmp.MeanAbsoluteError()
+        self.compiler.loss = new_loss
+        return self.fit(epochs=epochs)
+
+    def preprocess(self, *args, **kwargs):
+        """Converts an object to a numerical form consumable by the NN."""
+        return self.data.preprocess(*args, **kwargs)
+
+    def postprocess(self, *args, **kwargs): return self.data.postprocess(*args, **kwargs)
+    def __call__(self, *args, **kwargs): return self.model(*args, **kwargs)
+    def viz(self, *args, **kwargs): return self.data.viz(*args, **kwargs)
+    def save_model(self, directory): self.model.save(directory)  # In TF: send only path dir. Save path is saved_model.pb
+    def save_weights(self, directory): self.model.save_weights(directory.joinpath(self.model.name))  # TF: last part of path is file path.
+    @staticmethod
+    def load_model(directory): __import__("tensorflow").keras.models.load_model(directory)  # path to directory. file saved_model.pb is read auto.
+    def load_weights(self, directory): self.model.load_weights(directory.glob('*.data*').__next__().__str__().split('.data')[0])  # requires path to file path.
+    def summary(self):
+        from contextlib import redirect_stdout
+        path = self.hp.save_dir.joinpath("metadata/model_summary.txt").create(parents_only=True)
+        with open(str(path), 'w') as f:
+            with redirect_stdout(f): self.model.summary()
+        return self.model.summary()
+    def config(self): [print(layer.get_config(), "\n==============================") for layer in self.model.layers]; return None
+    def plot_loss(self, *args, **kwargs): return tb.Struct.concat_values(*self.history).plot(*args, title="Loss Curve",
+                                                                                             xlabel="epochs",
+                                                                                             ylabel=self.compiler.loss.name if hasattr(self.compiler.loss, "name") else self.compiler.loss.__name__,
+                                                                                             **kwargs)
+
+    def infer(self, x):
+        """ This method assumes numpy input, datatype-wise and is also preprocessed.
+        NN is put in eval mode.
+        :param x:
+        :return: prediction as numpy
+        """
+        return self.model.predict(x)  # Keras automatically handles special layers, can accept dataframes, and always returns numpy.
+
+    def predict(self, x, **kwargs):
+        """This method assumes preprocessed input. Returns postprocessed output. It is useful at evaluation time with preprocessed test set."""
+        return self.postprocess(self.infer(x), **kwargs)
+
+    def deduce(self, obj, viz=True, **kwargs):
+        """Assumes that contents of the object are in the form of a batch."""
+        preprocessed = self.preprocess(obj, **kwargs)
+        prediction = self.infer(preprocessed)
+        postprocessed = self.postprocess(prediction, **kwargs)
+        result = tb.Struct(input=obj, preprocessed=preprocessed, prediction=prediction, postprocessed=postprocessed)
+        if viz: self.viz(postprocessed, **kwargs)
+        return result
+
+    def evaluate(self, x_test=None, y_test=None, names_test=None, aslice=None, indices=None, use_slice=False, size=None, split="test", viz=True, **kwargs):
+        if x_test is None and y_test is None and names_test is None:
+            x_test, y_test, names_test = self.data.sample_dataset(aslice=aslice, indices=indices, use_slice=use_slice, split=split, size=size)
+        elif names_test is None: names_test = np.arange(len(x_test))
+        # ==========================================================================
+        y_pred = self.infer(x_test)
+        loss_df = self.get_metrics_evaluations(y_pred, y_test)
+        if loss_df is not None:
+            if len(self.data.other_strings) == 1: loss_df[self.data.other_strings[0]] = names_test
+            else:
+                for val, name in zip(names_test, self.data.other_strings): loss_df[name] = val
+        y_pred_pp = self.postprocess(y_pred, per_instance_kwargs=dict(name=names_test), legend="Prediction", **kwargs)
+        y_true_pp = self.postprocess(y_test, per_instance_kwargs=dict(name=names_test), legend="Ground Truth", **kwargs)
+        results = tb.Struct(x=x_test, y_pred=y_pred, y_pred_pp=y_pred_pp, y_true=y_test, y_true_pp=y_true_pp, names=names_test, loss_df=loss_df, )
+        if viz:
+            loss_name = results.loss_df.columns.to_list()[0]  # first loss path
+            loss_label = results.loss_df[loss_name].apply(lambda x: f"{loss_name} = {x}").to_list()
+            names = [f"{aname}. Case: {anindex}" for aname, anindex in zip(loss_label, names_test)]
+            self.fig = self.viz(y_pred_pp, y_true_pp, names=names, **kwargs)
+        return results
+
+    def get_metrics_evaluations(self, prediction, groun_truth) -> pd.DataFrame or None:
+        if self.compiler is None: return None
+        metrics = tb.L([self.compiler.loss]) + self.compiler.metrics
+        loss_dict = dict()
+        for a_metric in metrics:
+            if hasattr(a_metric, "name"): name = a_metric.name
+            elif hasattr(a_metric, "__name__"): name = a_metric.__name__
+            else: name = "unknown_loss_name"
+            # try:  # EAFP vs LBYL: both are duck-typing styles as they ask for what object can do (whether by introspection or trial) as opposed to checking its type.
+            #     path = a_metric.path  # works for subclasses Metrics
+            # except AttributeError: path = a_metric.__name__  # works for functions.
+            loss_dict[name] = []
+            for a_prediction, a_y_test in zip(prediction, groun_truth):
+                if hasattr(a_metric, "reset_states"): a_metric.reset_states()
+                loss = a_metric(y_pred=a_prediction[None], y_true=a_y_test[None])
+                loss_dict[name].append(np.array(loss).item())
+        return pd.DataFrame(loss_dict)
+
+    def save_class(self, weights_only=True, version='0', **kwargs):
+        """Simply saves everything:
+        1. Hparams
+        2. Data specs
+        3. Model architecture or weights depending on the following argument.
+        :param version: Model version, up to the user.
+        :param weights_only: self-explanatory
+        :return:
+        """
+        self.hp.save()  # goes into the meta path.
+        self.data.save()  # goes into the meta path.
+        tb.Save.pickle(obj=self.history, path=self.hp.save_dir / 'metadata/history.pkl', verbose=True, desc="Training History")  # goes into the meta path.
+        try: tb.Experimental.generate_readme(self.hp.save_dir, obj=self.__class__, **kwargs)
+        except Exception as ex: print(ex)  # often fails because model is defined in main during experiments.
+        save_dir = self.hp.save_dir.joinpath(f'{"weights" if weights_only else "model"}_save_v{version}').create()  # model save goes into data path.
+        if weights_only: self.save_weights(save_dir)
+        else: self.save_model(save_dir)
+        print(f'SAVED Model Class @ {self.hp.save_dir.as_uri()}')
+        return self.hp.save_dir
+
+    @classmethod
+    def from_class_weights(cls, path, hparam_class=None, data_class=None, device_name=None, verbose=True):
+        path = tb.P(path)
+        if hparam_class is not None: hp_obj = hparam_class.from_saved_data(path)
+        else: hp_obj = (path / HyperParam.subpath + "hparams.HyperParam.pkl").readit()
+        if device_name: hp_obj.device_name = device_name
+        if data_class is not None: d_obj = data_class.from_saved_data(path, hp=hp_obj)
+        else: d_obj = (path / DataReader.subpath / "data_reader.DataReader.pkl").readit()
+        if hp_obj.root != path.parent: hp_obj.root, hp_obj.name = path.parent, path.name  # if user moved the file to somewhere else, this will help alighment with new directory in case a modified version is to be saved.
+        d_obj.hp = hp_obj
+        model_obj = cls(hp_obj, d_obj)
+        model_obj.load_weights(path.search('*_save_*')[0])
+        model_obj.history = (path / "metadata/history.pkl").readit(notfound=tb.L())
+        print(f"LOADED {model_obj.__class__}: {model_obj.hp.name}") if verbose else None
+        return model_obj
+
+    @classmethod
+    def from_class_model(cls, path):
+        path = tb.P(path)
+        data_obj = DataReader.from_saved_data(path)
+        hp_obj = HyperParam.from_saved_data(path)
+        model_obj = cls.load_model(path.search('*_save_*')[0])  # static method.
+        wrapper_class = cls(hp_obj, data_obj, model_obj)
+        return wrapper_class
+
+    def plot_model(self, dpi=150, **kwargs):  # alternative viz via tf2onnx then Netron.
+        import tensorflow as tf
+        path = self.hp.save_dir / 'model_plot.png'
+        tf.keras.utils.plot_model(self.model, to_file=path, show_shapes=True, show_layer_names=True, show_layer_activations=True, show_dtype=True, expand_nested=True, dpi=dpi, **kwargs)
+        print(f"Successfully plotted the model @ {path.as_uri()}")
+        return path
+
+    def build(self, sample_dataset=False, ip_shapes=None, ip=None, verbose=True):
+        """ Building has two main uses.
+        * Useful to baptize the model, especially when its layers are built lazily. Although this will eventually happen as the first batch goes in. This is a must before showing the summary of the model.
+        * Doing sanity check about shapes when designing model.
+        * Sanity check about values and ranges when random normal input is fed.
+        :param sample_dataset:
+        :param ip_shapes:
+        :param ip:
+        :param verbose:
+        :return:
+        """
+        keys_ip = self.data.get_data_strings(which_data="ip", which_split="test")
+        keys_op = self.data.get_data_strings(which_data="op", which_split="test")
+
+        if ip is None:
+            if sample_dataset: ip, _, _ = self.data.sample_dataset()
+            else: ip, _ = self.data.get_random_inputs_outputs(ip_shapes=ip_shapes)
+        op = self.model(inputs=ip)
+        ops = [op] if len(keys_op) == 1 else op
+        ips = [ip] if len(keys_ip) == 1 else ip
+        if verbose:
+            print("\n")
+            print("Build Test".center(50, '-'))
+            print(f"Input shapes:")
+            tb.Struct.from_keys_values(keys_ip, tb.L(ips).apply(lambda x: x.shape)).print(as_config=True)
+            print(f"Output shape:")
+            tb.Struct.from_keys_values(keys_op, tb.L(ops).apply(lambda x: x.shape)).print(as_config=True)
+            print("\n\nStats on output data for random normal input:")
+            try:
+                res = []
+                for item_str, item_val in zip(keys_ip + keys_op, list(ips) + list(ops)):
+                    a_df = pd.DataFrame(np.array(item_val).flatten()).describe().rename(columns={0: item_str})
+                    res.append(a_df)
+                print(pd.concat(res, axis=1))
+            except Exception as ex:
+                print(f"Could not do stats on outputs and inputs. Error: {ex}")
+            print("Build Test Finished".center(50, '-'))
+            print("\n")
+
+
+class Ensemble(tb.Base):
+    def __init__(self, hp_class: Generic[HPM] = None, data_class: Generic[DR] = None, model_class: Generic[BM] = None, size=10, *args, **kwargs):
+        """
+        :param model_class: Either a class for constructing saved_models or list of saved_models already cosntructed.
+          * In either case, the following methods should be implemented:
+          __init__, load, load_weights, save, save_weights, predict, fit
+          Model constructor should takes everything it needs from self.hp and self.data only.
+          Otherwise, you must pass a list of already constructed saved_models.
+        :param size: size of ensemble
+        """
+        super().__init__(*args, **kwargs)
+        self.__dict__.update(kwargs)
+        self.size = size
+        self.hp_class = hp_class
+        self.data_class = data_class
+        self.model_class = model_class
+        self.models = tb.List()
+        self.data = None  # one data object for all models (so that it can fit in the memory)
+        if hp_class and data_class and model_class:
+            # only generate the dataset once and attach it to the ensemble to be reused by models.
+            self.data = self.data_class(hp_class(), load_trianing_data=True)
+            print("Creating Models".center(100, "="))
+            for i in tqdm(range(size)):
+                hp = self.hp_class()
+                hp.name = str(hp.name) + f'__model__{i}'
+                datacopy = copy.copy(self.data)  # shallow copy
+                datacopy.hp = hp
+                self.models.append(model_class(hp, datacopy))
+        self.performance = None
+
+    @classmethod
+    def from_saved_models(cls, parent_dir, model_class):
+        obj = cls(model_class=model_class, path=parent_dir, size=len(tb.P(parent_dir).search('*__model__*')))
+        obj.models = tb.P(parent_dir).search('*__model__*').apply(model_class.from_class_model)
+        return obj
+
+    @classmethod
+    def from_saved_weights(cls, parent_dir, model_class):
+        obj = cls(model_class=model_class, path=parent_dir, size=len(tb.P(parent_dir).search('*__model__*')))
+        obj.models = tb.P(parent_dir).search('*__model__*').apply(model_class.from_class_weights)
+        return obj
+
+    def fit(self, shuffle_train_test=True, save=True, **kwargs):
+        self.performance = tb.L()
+        for i in range(self.size):
+            print('\n\n', f" Training Model {i} ".center(100, "*"), '\n\n')
+            if shuffle_train_test:
+                self.models[i].hp.seed = np.random.randint(0, 1000)
+                self.data.split_the_data()  # shuffle data (shared among models)
+            self.models[i].fit(**kwargs)
+            self.performance.append(self.models[i].evaluate(idx=slice(0, -1), viz=False))
+            if save:
+                self.models[i].save_class()
+                self.performance.save(self.hp_class.save_dir / "performance.List.pkl")
+        print("\n\n", f" Finished fitting the ensemble ".center(100, ">"), "\n")
+
+    def clear_memory(self): pass  # t.cuda.empty_cache()
+
+
+class Losses:
+    @staticmethod
+    def get_log_square_loss_class():
+        import tensorflow as tf
+
+        class LogSquareLoss(tf.keras.losses.Loss):
+            def __init__(self, *args, **kwargs):
+                super().__init__(*args, **kwargs)
+                self.name = "LogSquareLoss"
+
+            def call(self, y_true, y_pred):
+                _ = self
+                factor = (20 / tf.math.log(tf.convert_to_tensor(10.0, dtype=y_pred.dtype)))
+                return factor * tf.math.log(tf.reduce_mean((y_true - y_pred)**2))
+        return LogSquareLoss
+
+    @staticmethod
+    def get_mean_max_error(tf):
+        """
+        For Tensorflow
+        """
+        class MeanMaxError(tf.keras.metrics.Metric):
+            def __init__(self, name='MeanMaximumError', **kwargs):
+                super(MeanMaxError, self).__init__(name=name, **kwargs)
+                self.mme = self.add_weight(name='mme', initializer='zeros')
+                self.__name__ = name
+
+            def update_state(self, y_true, y_pred, sample_weight=None): self.mme.assign(tf.reduce_mean(tf.reduce_max(sample_weight or 1.0 * tf.abs(y_pred - y_true), axis=1)))
+            def result(self): return self.mme
+            def reset_states(self): self.mme.assign(0.0)
+        return MeanMaxError
+
+
+class HPTuning:
+    def __init__(self):
+        # ================== Tuning ===============
+        from tensorboard.plugins.hparams import api as hpt
+        self.hpt = hpt
+        import tensorflow as tf
+        self.pkg = tf
+        self.dir = None
+        self.params = tb.List()
+        self.acc_metric = None
+        self.metrics = None
+
+    @staticmethod
+    def help():
+        """Steps of use: subclass this and do the following:
+        * Set directory attribute.
+        * set params
+        * set accuracy metric
+        * generate writer.
+        * implement run method.
+        * run loop method.
+        * in the command line, run `tensorboard --logdir <self.dir>`
+        """
+        pass
+
+    def run(self, param_dict):
+        _, _ = self, param_dict
+        # should return a result that you want to maximize
+        return _
+
+    def gen_writer(self):
+        import tensorflow as tf
+        with tf.summary.create_file_writer(str(self.dir)).as_default():
+            self.hpt.hparams_config(
+                hparams=self.params,
+                metrics=self.metrics)
+
+    def loop(self):
+        import itertools
+        counter = -1
+        tmp = self.params.list[0].domain.values
+        for combination in itertools.product(*[tmp]):
+            counter += 1
+            param_dict = dict(zip(self.params.list, combination))
+            with self.pkg.summary.create_file_writer(str(self.dir / f"run_{counter}")).as_default():
+                self.hpt.hparams(param_dict)  # record the values used in this trial
+                accuracy = self.run(param_dict)
+                self.pkg.summary.scalar(self.acc_metric, accuracy, step=1)
+
+    def optimize(self): self.gen_writer(); self.loop()
+
+
+class KerasOptimizer:
+    def __init__(self, d):
+        self.data = d
+        self.tuner = None
+
+    def __call__(self, ktp): pass
+
+    def tune(self):
+        kt = tb.core.install_n_import("kerastuner")
+        self.tuner = kt.Hyperband(self, objective='loss', max_epochs=10, factor=3, directory=tb.P.tmp('my_dir'), project_name='intro_to_kt')
+
+
+def batcher(func_type='function'):
+    if func_type == 'method':
+        def batch(func):
+            # from functools import wraps
+            # @wraps(func)
+            def wrapper(self, x, *args, per_instance_kwargs=None, **kwargs):
+                output = []
+                for counter, item in enumerate(x):
+                    mykwargs = {key: value[counter] for key, value in per_instance_kwargs.items()} if per_instance_kwargs is not None else {}
+                    output.append(func(self, item, *args, **mykwargs, **kwargs))
+                return np.array(output)
+            return wrapper
+        return batch
+    elif func_type == 'class': raise NotImplementedError
+    elif func_type == 'function':
+        class Batch(object):
+            def __init__(self, func): self.func = func
+            def __call__(self, x, **kwargs): return np.array([self.func(item, **kwargs) for item in x])
+        return Batch
+
+
+def batcherv2(func_type='function', order=1):
+    if func_type == 'method':
+        def batch(func):
+            # from functools import wraps
+            # @wraps(func)
+            def wrapper(self, *args, **kwargs): return np.array([func(self, *items, *args[order:], **kwargs) for items in zip(*args[:order])])
+            return wrapper
+        return batch
+    elif func_type == 'class': raise NotImplementedError
+    elif func_type == 'function':
+        class Batch(object):
+            def __int__(self, func): self.func = func
+            def __call__(self, *args, **kwargs): return np.array([self.func(self, *items, *args[order:], **kwargs) for items in zip(*args[:order])])
+        return Batch
+
+
+def get_template():
+    tb.install_n_import("clipboard").copy(tb.P(__file__).parent.joinpath("msc/dl_template.py").read_text(encoding="utf-8"))
+    print("Copied to clipboard")
+
+
+if __name__ == '__main__':
+    pass
```

### Comparing `crocodile-8.40/myresources/crocodile/environment.py` & `crocodile-9.0/myresources/crocodile/environment.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,211 +1,211 @@
-
-import crocodile.toolbox as tb
-import platform
-import getpass
-import os
-import sys
-
-P = tb.P
-L = tb.L
-
-system = platform.system()  # Linux or Windows
-myhome = tb.P(f"myhome/{platform.system().lower()}")
-
-OS = os.getenv("OS")  # Windows_NT
-sep = ";" if system == "Windows" else ":"  # PATH separator, this is special for PATH object, not to be confused with P.sep (normal paths), usually / or \
-# env = tb.Struct(dict(os.environ)).clean_view
-exe = P(sys.executable)
-
-tm = tb.Terminal()
-
-# ============================== Common Paths ============================
-
-LocalAppData = P(tmp) if (tmp := os.getenv("LOCALAPPDATA")) else None  # C:\Users\username\AppData\Local
-AppData = P(tmp) if (tmp := os.getenv("APPDATA")) else None  # C:\Users\username\AppData\Roaming
-WindowsApps = LocalAppData.joinpath(r"Microsoft\WindowsApps") if AppData else None  # this path is already in PATH. Thus, useful to add symlinks and shortcuts to apps that one would like to be in the PATH.
-
-ProgramData = P(tmp) if (tmp := os.getenv("PROGRAMDATA")) else None  # C:\ProgramData
-ProgramFiles = P(tmp) if (tmp := os.getenv("ProgramFiles")) else None  # C:\Program Files
-ProgramW6432 = P(tmp) if (tmp := os.getenv("ProgramW6432")) else None  # C:\Program Files
-ProgramFilesX86 = P(tmp) if (tmp := os.getenv("ProgramFiles(x86)")) else None  # C:\Program Files (x86)
-
-CommonProgramFiles = P(tmp) if (tmp := os.getenv("CommonProgramFiles")) else None  # C:\Program Files\Common Files
-CommonProgramW6432 = P(tmp) if (tmp := os.getenv("CommonProgramW6432")) else None  # C:\Program Files\Common Files
-CommonProgramFilesX86 = P(tmp) if (tmp := os.getenv("CommonProgramFiles(x86)")) else None  # C:\Program Files (x86)\Common Files
-
-Tmp = P(tmp) if (tmp := os.getenv("TMP")) else None  # C:\Users\usernrame\AppData\Local\Temp
-Temp = Tmp
-
-Path = L(os.getenv("PATH").split(sep)).apply(P)
-PSPath = L(tmp.split(sep)).apply(P) if (tmp := os.getenv("PSModulePath")) else None
-
-HostName          = platform.node()  # e.g. "MY-SURFACE", os.getenv("COMPUTERNAME") only works for windows.
-UserName          = getpass.getuser()  # e.g: username, os.getenv("USERNAME") only works for windows.
-UserDomain        = os.getenv("USERDOMAIN")  # e.g. HAD OR MY-SURFACE
-UserDomainRoaming = P(tmp) if (tmp := os.getenv("USERDOMAIN_ROAMINGPROFILE")) else None  # e.g. SURFACE
-LogonServer       = os.getenv("LOGONSERVER")  # e.g. "\\MY-SURFACE"
-# UserProfile       = P(tmp) if (tmp := os.getenv("USERPROFILE")) else None  # e.g C:\Users\username
-# HomePath          = P(tmp) if (tmp := os.getenv("HOMEPATH")) else None  # e.g. C:\Users\username
-Public            = P(tmp) if (tmp := os.getenv("PUBLIC")) else None  # C:\Users\Public
-
-WSL_FROM_WIN = P(r"\\wsl.localhost\Ubuntu-22.04\home")  # P(rf"\\wsl$\Ubuntu\home")  # see localappdata/canonical
-WIN_FROM_WSL = P(rf"/mnt/c/Users")
-
-
-OneDriveConsumer = P(tmp) if (tmp := os.getenv("OneDriveConsumer")) else None
-OneDriveCommercial = P(tmp) if (tmp := os.getenv("OneDriveCommercial")) else None
-OneDrive = P(tmp) if (tmp := os.getenv("OneDrive")) else None
-if system == "Windows":
-    tmp1 = LocalAppData.joinpath("Microsoft/OneDrive/OneDrive.exe")
-    tmp2 = P(r"C:/Program Files/Microsoft OneDrive/OneDrive.exe")
-    OneDriveExe = tmp1 if tmp1.exists() else tmp2
-else: OneDriveExe = None
-
-
-DotFiles = P.home().joinpath("dotfiles")
-
-# ============================== Networking ==============================
-
-
-def get_addresses():
-    netifaces = tb.install_n_import("netifaces")
-    subnet_mask = netifaces.ifaddresses(netifaces.gateways()['default'][netifaces.AF_INET][1])[netifaces.AF_INET][0]['netmask']
-    default_gateway = netifaces.gateways()['default'][netifaces.AF_INET][0]
-    import uuid
-    mac = uuid.getnode()
-    mac_address = ":".join(("%012X" % mac)[i:i + 2] for i in range(0, 12, 2))
-    # elif hex_format: return hex(mac)
-    # else: return mac
-    import socket
-    local_ip_v4 = socket.gethostbyname(socket.gethostname() + ".local")  # without .local, in linux machines, '/etc/hosts' file content, you have an IP address mapping with '127.0.1.1' to your hostname
-    return dict(subnet_mask=subnet_mask, mac_address=mac_address, local_ip_v4=local_ip_v4, default_gateway=default_gateway, public_ip_v4=P('https://api.ipify.org').download(memory=True).text)
-
-
-# ============================== System Variables ==============================
-
-
-class ShellVar(object):
-    @staticmethod
-    def set(key, val, run=False, shell="powershell"):
-        if system == "Windows":
-            res = f"set {key} {val}"
-            return res if not run else tm.run(res, shell=shell)
-        elif system == "Linux":
-            res = f"{key} = {val}"
-            return res if not run else tm.run(res, shell="bash")
-
-    @staticmethod
-    def get(key, run=False):
-        result = f"${key}"  # works in powershell and bash
-        return result if run is False else tm.run(result, shell="powershell")
-    # in windows cmd `%key%`
-
-
-class EnvVar:
-    @staticmethod
-    def set(key, val, temp=False, run=False):
-        if system == "Windows":
-            if temp is False:
-                res = f"setx {key} {val}"  # WARNING: setx limits val to 1024 characters # in case the variable included ";" separated paths, this limit can be exceeded.
-                return res if not run else tm.run(res, shell="powershell")
-            else: raise NotImplementedError
-        elif system == "Linux": return f"export {key} = {val}"  # this is shell command. in csh: `setenv key val`
-        else: raise NotImplementedError
-
-    @staticmethod
-    def get(key, run=False):
-        result = f"${key}"  # works in powershell and bash
-        return result if run is False else tm.run(result, shell="powershell")
-
-    # in windows cmd `%key%`
-    @staticmethod
-    def delete(key, temp=True, scope=["User", "system"][0], run=False):
-        if system == "Windows":
-            if temp:
-                result = fr"Remove-Item Env:\{key}"  # temporary removal (session)
-                return result if run is False else tm.run(result, shell="powershell")
-            else:
-                result = fr'[Environment]::SetEnvironmentVariable("{key}",$null,"{scope}")'
-                return result if run is False else tm.run(result, shell="powershell")
-        else:
-            raise NotImplementedError
-
-
-class PathVar:
-    @staticmethod
-    def append_temporarily(dirs, kind="append", run=False):
-        dirs_ = []
-        for path in dirs:
-            path = tb.P(path).collapseuser(strict=False)
-            path = path.as_posix() if system == "Linux" else str(path)
-            if path in Path: print(f"Path passed `{path}` is already in PATH, skipping the appending.")
-            else: dirs_.append(path)
-        dirs = dirs_
-        if len(dirs) == 0: return ""
-
-        if system == "Windows":
-            """Source: https://docs.microsoft.com/en-us/powershell/module/microsoft.powershell.core/about/about_environment_variables?view=powershell-7.2"""
-            if kind == "append": command = fr'$env:Path += ";{sep.join(dirs)}"'  # Append to the Path variable in the current window:
-            elif kind == "prefix": command = fr'$env:Path = "{sep.join(dirs)};" + $env:Path'  # Prefix the Path variable in the current window:
-            elif kind == "replace": command = fr'$env:Path = "{sep.join(dirs)}"'  # Replace the Path variable in the current window (use with caution!):
-            else: raise KeyError
-            return command if run is False else tm.run(command, shell="powershell")
-        elif system == "Linux": result = f'export PATH="{sep.join(dirs)}:$PATH"'
-        else: raise ValueError
-        return result if run is False else tm.run(result, shell="powershell")
-
-    @staticmethod
-    def append_permanently(path, scope=["User", "system"][0], run=False):
-        if system == "Windows":
-            # AVOID THIS AND OPT TO SAVE IT IN $profile.
-            tmp_path = tb.P.tmpfile(suffix=".path_backup")
-            if tb.P(path) in Path:
-                print(f"Path passed `{path}` is already in PATH, skipping the appending.")
-                return None
-            backup = fr'$env:PATH >> {tmp_path}; '
-            command = fr'[Environment]::SetEnvironmentVariable("Path", $env:PATH + ";{path}", "{scope}")'
-            result = backup + command
-            return result if run is False else tm.run(result, shell="powershell").print()
-        else: tb.P.home().joinpath(".bashrc").append_text(f"export PATH='{path}:$PATH'")
-
-    @staticmethod
-    def set_permanetly(path, scope=["User", "system"][0], run=False):
-        """This is useful if path is manipulated with a text editor or Python string manipulation (not recommended programmatically even if original is backed up) and set the final value.
-        On a windows machine, system and user variables are kept separately. env:Path returns the combination of both, starting from system then user.
-        To see impact of change, you will need to restart the process from which the shell started. This is probably windows explorer.
-        This can be achieved by suspending the process, alternatively you need to logoff and on.
-        This is because enviroment variables are inherited from parent process, and so long explorere is not updated, restarting the shell would not help."""
-        tmpfile = tb.P.tmpfile(suffix=".path_backup")
-        print(f"Saving original path to {tmpfile}")
-        backup = fr'$env:PATH >> {tmpfile}; '
-        result = backup + fr'[Environment]::SetEnvironmentVariable("Path", "{path}", "{scope}")'
-        return result if run is False else tm.run(result, shell="powershell")
-
-    @staticmethod
-    def load_fresh_path(run=False):
-        if system == "Windows":
-            result = fr'[System.Environment]::GetEnvironmentVariable("Path","Machine") + ";" + [System.Environment]::GetEnvironmentVariable("Path","User")'
-            return result if run is False else tm.run(result, shell="powershell")
-
-
-# ============================== Shells =========================================
-
-
-def get_shell_profiles(shell):
-    # following this: https://docs.microsoft.com/en-us/powershell/module/microsoft.powershell.core/about/about_profiles?view=powershell-7.2
-    # https://devblogs.microsoft.com/scripting/understanding-the-six-powershell-profiles/
-    # Dynmaically obtained:
-    return tb.Struct(
-        CurrentUserCurrentHost=tm.run("$PROFILE.CurrentUserCurrentHost", shell=shell).op2path(),
-        CurrentUserAllHosts=tm.run("$PROFILE.CurrentUserAllHosts", shell=shell).op2path(),
-        AllUsersCurrentHost=tm.run("$PROFILE.AllUsersCurrentHost", shell=shell).op2path(),
-        AllUsersAllHosts=tm.run("$PROFILE.AllUsersAllHosts", shell=shell).op2path(),
-    )
-
-
-def construct_path(path_list): return tb.L(__import__("pd").unique(path_list)).reduce(lambda x, y: str(x) + sep + str(y))
-def get_path_defined_files(string_="*.exe"): res = Path.search(string_).reduce(lambda x, y: x + y); res.print(); return res
-
-
-if __name__ == '__main__':
-    pass
+
+import crocodile.toolbox as tb
+import platform
+import getpass
+import os
+import sys
+
+P = tb.P
+L = tb.L
+
+system = platform.system()  # Linux or Windows
+myhome = tb.P(f"myhome/{platform.system().lower()}")
+
+OS = os.getenv("OS")  # Windows_NT
+sep = ";" if system == "Windows" else ":"  # PATH separator, this is special for PATH object, not to be confused with P.sep (normal paths), usually / or \
+# env = tb.Struct(dict(os.environ)).clean_view
+exe = P(sys.executable)
+
+tm = tb.Terminal()
+
+# ============================== Common Paths ============================
+
+LocalAppData = P(tmp) if (tmp := os.getenv("LOCALAPPDATA")) else None  # C:\Users\username\AppData\Local
+AppData = P(tmp) if (tmp := os.getenv("APPDATA")) else None  # C:\Users\username\AppData\Roaming
+WindowsApps = LocalAppData.joinpath(r"Microsoft\WindowsApps") if AppData else None  # this path is already in PATH. Thus, useful to add symlinks and shortcuts to apps that one would like to be in the PATH.
+
+ProgramData = P(tmp) if (tmp := os.getenv("PROGRAMDATA")) else None  # C:\ProgramData
+ProgramFiles = P(tmp) if (tmp := os.getenv("ProgramFiles")) else None  # C:\Program Files
+ProgramW6432 = P(tmp) if (tmp := os.getenv("ProgramW6432")) else None  # C:\Program Files
+ProgramFilesX86 = P(tmp) if (tmp := os.getenv("ProgramFiles(x86)")) else None  # C:\Program Files (x86)
+
+CommonProgramFiles = P(tmp) if (tmp := os.getenv("CommonProgramFiles")) else None  # C:\Program Files\Common Files
+CommonProgramW6432 = P(tmp) if (tmp := os.getenv("CommonProgramW6432")) else None  # C:\Program Files\Common Files
+CommonProgramFilesX86 = P(tmp) if (tmp := os.getenv("CommonProgramFiles(x86)")) else None  # C:\Program Files (x86)\Common Files
+
+Tmp = P(tmp) if (tmp := os.getenv("TMP")) else None  # C:\Users\usernrame\AppData\Local\Temp
+Temp = Tmp
+
+Path = L(os.getenv("PATH").split(sep)).apply(P)
+PSPath = L(tmp.split(sep)).apply(P) if (tmp := os.getenv("PSModulePath")) else None
+
+HostName          = platform.node()  # e.g. "MY-SURFACE", os.getenv("COMPUTERNAME") only works for windows.
+UserName          = getpass.getuser()  # e.g: username, os.getenv("USERNAME") only works for windows.
+UserDomain        = os.getenv("USERDOMAIN")  # e.g. HAD OR MY-SURFACE
+UserDomainRoaming = P(tmp) if (tmp := os.getenv("USERDOMAIN_ROAMINGPROFILE")) else None  # e.g. SURFACE
+LogonServer       = os.getenv("LOGONSERVER")  # e.g. "\\MY-SURFACE"
+# UserProfile       = P(tmp) if (tmp := os.getenv("USERPROFILE")) else None  # e.g C:\Users\username
+# HomePath          = P(tmp) if (tmp := os.getenv("HOMEPATH")) else None  # e.g. C:\Users\username
+Public            = P(tmp) if (tmp := os.getenv("PUBLIC")) else None  # C:\Users\Public
+
+WSL_FROM_WIN = P(r"\\wsl.localhost\Ubuntu-22.04\home")  # P(rf"\\wsl$\Ubuntu\home")  # see localappdata/canonical
+WIN_FROM_WSL = P(rf"/mnt/c/Users")
+
+
+OneDriveConsumer = P(tmp) if (tmp := os.getenv("OneDriveConsumer")) else None
+OneDriveCommercial = P(tmp) if (tmp := os.getenv("OneDriveCommercial")) else None
+OneDrive = P(tmp) if (tmp := os.getenv("OneDrive")) else None
+if system == "Windows":
+    tmp1 = LocalAppData.joinpath("Microsoft/OneDrive/OneDrive.exe")
+    tmp2 = P(r"C:/Program Files/Microsoft OneDrive/OneDrive.exe")
+    OneDriveExe = tmp1 if tmp1.exists() else tmp2
+else: OneDriveExe = None
+
+
+DotFiles = P.home().joinpath("dotfiles")
+
+# ============================== Networking ==============================
+
+
+def get_addresses():
+    netifaces = tb.install_n_import("netifaces")
+    subnet_mask = netifaces.ifaddresses(netifaces.gateways()['default'][netifaces.AF_INET][1])[netifaces.AF_INET][0]['netmask']
+    default_gateway = netifaces.gateways()['default'][netifaces.AF_INET][0]
+    import uuid
+    mac = uuid.getnode()
+    mac_address = ":".join(("%012X" % mac)[i:i + 2] for i in range(0, 12, 2))
+    # elif hex_format: return hex(mac)
+    # else: return mac
+    import socket
+    local_ip_v4 = socket.gethostbyname(socket.gethostname() + ".local")  # without .local, in linux machines, '/etc/hosts' file content, you have an IP address mapping with '127.0.1.1' to your hostname
+    return dict(subnet_mask=subnet_mask, mac_address=mac_address, local_ip_v4=local_ip_v4, default_gateway=default_gateway, public_ip_v4=P('https://api.ipify.org').download(memory=True).text)
+
+
+# ============================== System Variables ==============================
+
+
+class ShellVar(object):
+    @staticmethod
+    def set(key, val, run=False, shell="powershell"):
+        if system == "Windows":
+            res = f"set {key} {val}"
+            return res if not run else tm.run(res, shell=shell)
+        elif system == "Linux":
+            res = f"{key} = {val}"
+            return res if not run else tm.run(res, shell="bash")
+
+    @staticmethod
+    def get(key, run=False):
+        result = f"${key}"  # works in powershell and bash
+        return result if run is False else tm.run(result, shell="powershell")
+    # in windows cmd `%key%`
+
+
+class EnvVar:
+    @staticmethod
+    def set(key, val, temp=False, run=False):
+        if system == "Windows":
+            if temp is False:
+                res = f"setx {key} {val}"  # WARNING: setx limits val to 1024 characters # in case the variable included ";" separated paths, this limit can be exceeded.
+                return res if not run else tm.run(res, shell="powershell")
+            else: raise NotImplementedError
+        elif system == "Linux": return f"export {key} = {val}"  # this is shell command. in csh: `setenv key val`
+        else: raise NotImplementedError
+
+    @staticmethod
+    def get(key, run=False):
+        result = f"${key}"  # works in powershell and bash
+        return result if run is False else tm.run(result, shell="powershell")
+
+    # in windows cmd `%key%`
+    @staticmethod
+    def delete(key, temp=True, scope=["User", "system"][0], run=False):
+        if system == "Windows":
+            if temp:
+                result = fr"Remove-Item Env:\{key}"  # temporary removal (session)
+                return result if run is False else tm.run(result, shell="powershell")
+            else:
+                result = fr'[Environment]::SetEnvironmentVariable("{key}",$null,"{scope}")'
+                return result if run is False else tm.run(result, shell="powershell")
+        else:
+            raise NotImplementedError
+
+
+class PathVar:
+    @staticmethod
+    def append_temporarily(dirs, kind="append", run=False):
+        dirs_ = []
+        for path in dirs:
+            path = tb.P(path).collapseuser(strict=False)
+            path = path.as_posix() if system == "Linux" else str(path)
+            if path in Path: print(f"Path passed `{path}` is already in PATH, skipping the appending.")
+            else: dirs_.append(path)
+        dirs = dirs_
+        if len(dirs) == 0: return ""
+
+        if system == "Windows":
+            """Source: https://docs.microsoft.com/en-us/powershell/module/microsoft.powershell.core/about/about_environment_variables?view=powershell-7.2"""
+            if kind == "append": command = fr'$env:Path += ";{sep.join(dirs)}"'  # Append to the Path variable in the current window:
+            elif kind == "prefix": command = fr'$env:Path = "{sep.join(dirs)};" + $env:Path'  # Prefix the Path variable in the current window:
+            elif kind == "replace": command = fr'$env:Path = "{sep.join(dirs)}"'  # Replace the Path variable in the current window (use with caution!):
+            else: raise KeyError
+            return command if run is False else tm.run(command, shell="powershell")
+        elif system == "Linux": result = f'export PATH="{sep.join(dirs)}:$PATH"'
+        else: raise ValueError
+        return result if run is False else tm.run(result, shell="powershell")
+
+    @staticmethod
+    def append_permanently(path, scope=["User", "system"][0], run=False):
+        if system == "Windows":
+            # AVOID THIS AND OPT TO SAVE IT IN $profile.
+            tmp_path = tb.P.tmpfile(suffix=".path_backup")
+            if tb.P(path) in Path:
+                print(f"Path passed `{path}` is already in PATH, skipping the appending.")
+                return None
+            backup = fr'$env:PATH >> {tmp_path}; '
+            command = fr'[Environment]::SetEnvironmentVariable("Path", $env:PATH + ";{path}", "{scope}")'
+            result = backup + command
+            return result if run is False else tm.run(result, shell="powershell").print()
+        else: tb.P.home().joinpath(".bashrc").append_text(f"export PATH='{path}:$PATH'")
+
+    @staticmethod
+    def set_permanetly(path, scope=["User", "system"][0], run=False):
+        """This is useful if path is manipulated with a text editor or Python string manipulation (not recommended programmatically even if original is backed up) and set the final value.
+        On a windows machine, system and user variables are kept separately. env:Path returns the combination of both, starting from system then user.
+        To see impact of change, you will need to restart the process from which the shell started. This is probably windows explorer.
+        This can be achieved by suspending the process, alternatively you need to logoff and on.
+        This is because enviroment variables are inherited from parent process, and so long explorere is not updated, restarting the shell would not help."""
+        tmpfile = tb.P.tmpfile(suffix=".path_backup")
+        print(f"Saving original path to {tmpfile}")
+        backup = fr'$env:PATH >> {tmpfile}; '
+        result = backup + fr'[Environment]::SetEnvironmentVariable("Path", "{path}", "{scope}")'
+        return result if run is False else tm.run(result, shell="powershell")
+
+    @staticmethod
+    def load_fresh_path(run=False):
+        if system == "Windows":
+            result = fr'[System.Environment]::GetEnvironmentVariable("Path","Machine") + ";" + [System.Environment]::GetEnvironmentVariable("Path","User")'
+            return result if run is False else tm.run(result, shell="powershell")
+
+
+# ============================== Shells =========================================
+
+
+def get_shell_profiles(shell):
+    # following this: https://docs.microsoft.com/en-us/powershell/module/microsoft.powershell.core/about/about_profiles?view=powershell-7.2
+    # https://devblogs.microsoft.com/scripting/understanding-the-six-powershell-profiles/
+    # Dynmaically obtained:
+    return tb.Struct(
+        CurrentUserCurrentHost=tm.run("$PROFILE.CurrentUserCurrentHost", shell=shell).op2path(),
+        CurrentUserAllHosts=tm.run("$PROFILE.CurrentUserAllHosts", shell=shell).op2path(),
+        AllUsersCurrentHost=tm.run("$PROFILE.AllUsersCurrentHost", shell=shell).op2path(),
+        AllUsersAllHosts=tm.run("$PROFILE.AllUsersAllHosts", shell=shell).op2path(),
+    )
+
+
+def construct_path(path_list): return tb.L(__import__("pd").unique(path_list)).reduce(lambda x, y: str(x) + sep + str(y))
+def get_path_defined_files(string_="*.exe"): res = Path.search(string_).reduce(lambda x, y: x + y); res.print(); return res
+
+
+if __name__ == '__main__':
+    pass
```

### Comparing `crocodile-8.40/myresources/crocodile/file_management.py` & `crocodile-9.0/myresources/crocodile/file_management.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,400 +1,400 @@
-
-from crocodile.core import Struct, List, timestamp, randstr, validate_name, str2timedelta, Save, Path, get_env, install_n_import
-from datetime import datetime
-
-# %% =============================== Security ================================================
-def obscure(msg: bytes) -> bytes: return __import__("base64").urlsafe_b64encode(__import__("zlib").compress(msg, 9))
-def unobscure(obscured: bytes) -> bytes: return __import__("zlib").decompress(__import__("base64").urlsafe_b64decode(obscured))
-def pwd2key(password: str, salt=None, iterations=None) -> bytes:  # Derive a secret key from a given password and salt"""
-    if salt is None: m = __import__("hashlib").sha256(); m.update(password.encode("utf-8")); return __import__("base64").urlsafe_b64encode(m.digest())  # make url-safe bytes required by Ferent.
-    from cryptography.hazmat.primitives import hashes; from cryptography.hazmat.primitives.kdf.pbkdf2 import PBKDF2HMAC
-    return __import__("base64").urlsafe_b64encode(PBKDF2HMAC(algorithm=hashes.SHA256(), length=32, salt=salt, iterations=iterations, backend=None).derive(password.encode()))
-def encrypt(msg: bytes, key=None, pwd: str = None, salted=True, iteration: int = None, gen_key=False) -> bytes:
-    salt = None  # silence the linter.
-    if pwd is not None:  # generate it from password
-        assert (key is None) and (type(pwd) is str), f"You can either pass key or pwd, or none of them, but not both."
-        salt, iteration = (__import__('secrets').token_bytes(16), iteration or __import__('secrets').randbelow(1_000_000)) if salted else (None, None); key = pwd2key(pwd, salt, iteration)
-    elif key is None:
-        if gen_key: key = __import__("cryptography.fernet").__dict__["fernet"].Fernet.generate_key(); P.home().joinpath('dotfiles/creds/data/encrypted_files_key.bytes').write_bytes(key)
-        else:
-            try: key = P.home().joinpath("dotfiles/creds/data/encrypted_files_key.bytes").read_bytes()  # read from file
-            except FileNotFoundError as err: print("\n"*3, "~"*50, f"""Consider Loading up your dotfiles or pass `gen_key=True` to make and save one.""", "~"*50, "\n"*3); raise FileNotFoundError(err)
-    elif type(key) in {str, P, Path}: key = P(key).read_bytes()  # a path to a key file was passed, read it:
-    elif type(key) is bytes: pass  # key passed explicitly
-    else: raise TypeError(f"Key must be either a path, bytes object or None.")
-    code = __import__("cryptography.fernet").__dict__["fernet"].Fernet(key).encrypt(msg)
-    return __import__("base64").urlsafe_b64encode(b'%b%b%b' % (salt, iteration.to_bytes(4, 'big'), __import__("base64").urlsafe_b64decode(code))) if pwd is not None and salted is True else code
-def decrypt(token: bytes, key=None, pwd: str = None, salted=True) -> bytes:
-    if pwd is not None:
-        assert key is None, f"You can either pass key or pwd, or none of them, but not both."
-        if salted:
-            decoded = __import__("base64").urlsafe_b64decode(token); salt, iterations, token = decoded[:16], decoded[16:20], __import__("base64").urlsafe_b64encode(decoded[20:])
-            key = pwd2key(pwd, salt, int.from_bytes(iterations, 'big'))
-        else: key = pwd2key(pwd)  # trailing `;` prevents IPython from caching the result.
-    if type(key) is bytes: pass  # passsed explicitly
-    elif key is None: key = P("~/dotfiles/creds/data/encrypted_files_key.bytes").expanduser().read_bytes()  # read from file
-    elif type(key) in {str, P, Path}: key = P(key).read_bytes()  # passed a path to a file containing kwy
-    else: raise TypeError(f"Key must be either str, P, Path, bytes or None. Recieved: {type(key)}")
-    return __import__("cryptography.fernet").__dict__["fernet"].Fernet(key).decrypt(token)
-def unlock(drive="D:", pwd=None, auto_unlock=False):
-    return __import__("crocodile").meta.Terminal().run(f"""$SecureString = ConvertTo-SecureString "{pwd or P.home().joinpath("dotfiles/creds/data/bitlocker_pwd").read_text()}" -AsPlainText -Force; Unlock-BitLocker -MountPoint "{drive}" -Password $SecureString; """ + (f'Enable-BitLockerAutoUnlock -MountPoint "{drive}"' if auto_unlock else ''), shell="pwsh")
-
-# %% =================================== File ============================================
-def read(path, **kwargs):
-    suffix = Path(path).suffix[1:]
-    try: return getattr(Read, suffix)(str(path), **kwargs)
-    except AttributeError as err:
-        if "type object 'Read' has no attribute" not in str(err): raise AttributeError(err)
-        if suffix in ('eps', 'jpg', 'jpeg', 'pdf', 'pgf', 'png', 'ps', 'raw', 'rgba', 'svg', 'svgz', 'tif', 'tiff'): return __import__("matplotlib").pyplot.imread(path, **kwargs)  # from: plt.gcf().canvas.get_supported_filetypes().keys():
-        raise AttributeError(f"Unknown file type. failed to recognize the suffix `{suffix}`. According to libmagic1, the file seems to be: {install_n_import('magic', 'python-magic').from_file(path)}")
-def json(path, r=False, **kwargs):
-    try: mydict = __import__("json").loads(P(path).read_text(), **kwargs)
-    except Exception: mydict = install_n_import("pyjson5").loads(P(path).read_text(), **kwargs)  # file has C-style comments.
-    return Struct.recursive_struct(mydict) if r else Struct(mydict)
-def yaml(path, r=False):
-    with open(str(path), "r") as file: mydict = __import__("yaml").load(file, Loader=__import__("yaml").FullLoader)
-    return Struct(mydict) if not r else Struct.recursive_struct(mydict)
-def ini(path): import configparser; res = configparser.ConfigParser(); res.read(str(path)); return res
-def toml(path): return __import__("tomli").loads(P(path).read_text())
-def npy(path, **kwargs): data = (np := __import__("numpy")).load(str(path), allow_pickle=True, **kwargs); data = data.item() if data.dtype == np.object else data; return Struct(data) if type(data) is dict else data
-def mat(path, remove_meta=False, **kwargs): res = Struct(__import__("scipy.io").__dict__["io"].loadmat(path, **kwargs)); List(res.keys()).filter("x.startswith('__')").apply(lambda x: res.__delattr__(x)) if remove_meta else None; return res
-def csv(path, **kwargs): return __import__("pandas").read_csv(path, **kwargs)
-def py(path, init_globals=None, run_name=None): return Struct(__import__("runpy").run_path(path, init_globals=init_globals, run_name=run_name))
-def pickles(bytes_obj): return __import__("dill").loads(bytes_obj)  # handles imports automatically provided that saved object was from an imported class (not in defined in __main__)
-def pickle(path, **kwargs): obj = __import__("dill").loads(P(path).read_bytes(), **kwargs); return Struct(obj) if type(obj) is dict else obj
-def pkl(*args, **kwargs): return pickle(*args, **kwargs)
-class Read: read = read; mat = mat; json = json; yaml = yaml; ini = ini; npy = npy; csv = csv; pkl = pkl; py = py; pickle = pickle; toml = toml; txt = lambda path, encoding=None: P(path).read_text(encoding=encoding)
-
-
-def modify_text(txt_raw, txt_search, txt_alt, replace_line=True, notfound_append=False, prepend=False):
-    lines, bingo = txt_raw.split("\n"), False
-    if not replace_line:  # no need for line splitting
-        if txt_search in txt_raw: return txt_raw.replace(txt_search, txt_alt)
-        return txt_raw + "\n" +  txt_alt if notfound_append else txt_raw
-    for idx, line in enumerate(lines):
-        if txt_search in line:
-            lines[idx], bingo = txt_alt if type(txt_alt) is str else txt_alt(line), True
-    if bingo is False and notfound_append is True: (lines.insert(0, txt_alt) if prepend else lines.append(txt_alt))  # txt not found, add it anyway.
-    return "\n".join(lines)
-
-
-class P(type(Path()), Path):
-    # ============= Path management ==================
-    """ The default behaviour of methods acting on underlying disk object is to perform the action and return a new path referring to the mutated object in disk drive.
-    However, there is a flag `orig` that makes the function return orignal path object `self` as opposed to the new one pointing to new object.
-    Additionally, the fate of the original object can be decided by a flag `inplace` which means `replace` it defaults to False and in essence, it deletes the original underlying object.
-    This can be seen in `zip` and `encrypt` but not in `copy`, `move`, `retitle` because the fate of original file is dictated already.
-    Furthermore, those methods are accompanied with print statement explaining what happened to the object."""
-    def delete(self, sure=False, verbose=True) -> 'P':  # slf = self.expanduser().resolve() don't resolve symlinks.
-        if not sure: print(f"Did NOT DELETE because user is not sure. file: {repr(self)}.") if verbose else None; return self
-        if not self.exists(): self.unlink(missing_ok=True); print(f"Could NOT DELETE nonexisting file {repr(self)}. ") if verbose else None; return self  # broken symlinks exhibit funny existence behaviour, catch them here.
-        self.unlink(missing_ok=True) if self.is_file() or self.is_symlink() else __import__("shutil").rmtree(self, ignore_errors=False); print(f"DELETED {repr(self)}.") if verbose else None; return self
-    def send2trash(self, verbose=True) -> 'P':
-        if self.exists(): install_n_import("send2trash").send2trash(self.resolve().str); print(f"TRASHED {repr(self)}") if verbose else None  # do not expand user symlinks.
-        elif verbose: print(f"Could NOT trash {self}"); return self
-    def move(self, folder=None, name=None, path=None, rel2it=False, overwrite=False, verbose=True, parents=True, content=False) -> 'P':
-        path = self._resolve_path(folder=folder, name=name, path=path, default_name=self.absolute().name, rel2it=rel2it)
-        path.parent.create(parents=True, exist_ok=True) if parents else None; slf = self.expanduser().resolve()
-        if content:
-            assert self.is_dir(), NotADirectoryError(f"When `content` flag is set to True, path must be a directory. It is not: `{repr(self)}`")
-            self.search("*").apply(lambda x: x.move(folder=path.parent, content=False, overwrite=overwrite)); return path  # contents live within this directory.
-        if overwrite: tmp_path = slf.rename(path.parent.absolute() / randstr()); path.delete(sure=True, verbose=verbose); tmp_path.rename(path)  # works if moving a path up and parent has same name
-        else: slf.rename(path)  # self._return(res=path, inplace=True, operation='rename', orig=False, verbose=verbose, strict=True, msg='')
-        print(f"MOVED {repr(self)} ==> {repr(path)}`") if verbose else None; return path
-    def copy(self, folder=None, name=None, path=None, content=False, verbose=True, append=None, overwrite=False, orig=False) -> 'P':  # tested %100  # TODO: replace `content` flag with ability to interpret "*" in resolve method.
-        dest = self._resolve_path(folder=folder, name=name, path=path, default_name=self.name, rel2it=False)
-        dest, slf = dest.expanduser().resolve().create(parents_only=True), self.expanduser().resolve()
-        dest = self.append(append if append is not None else f"_copy_{randstr()}") if dest == slf else dest
-        dest.delete(sure=True) if not content and overwrite and dest.exists() else None
-        if not content and not overwrite and dest.exists(): raise FileExistsError(f"Destination already exists: {repr(dest)}")
-        if slf.is_file(): __import__("shutil").copy(str(slf), str(dest)); print(f"COPIED {repr(slf)} ==> {repr(dest)}") if verbose else None
-        elif slf.is_dir(): dest = dest.parent if content else dest; __import__("distutils.dir_util").__dict__["dir_util"].copy_tree(str(slf), str(dest)); print(f"COPIED {'Content of ' if False else ''} {repr(slf)} ==> {repr(dest)}") if verbose else None
-        else: print(f"Could NOT COPY. Not a file nor a path: {repr(slf)}.")
-        return dest if not orig else self
-    # ======================================= File Editing / Reading ===================================
-    def readit(self, reader=None, strict=True, notfound=None, verbose=False, **kwargs) -> 'P':
-        if not (slf := self.expanduser().resolve()).exists():
-            if strict: raise FileNotFoundError(f"`{slf}` is no where to be found!")
-            else: (print(f"tb.P.readit warning: FileNotFoundError, skipping reading of file `{self}") if verbose else None); return notfound
-        if verbose: print(f"Reading {slf.name} ({slf.size()} MB) ...")
-        filename = slf.unzip(folder=slf.tmp(folder="tmp_unzipped"), verbose=verbose) if '.zip' in str(slf) else slf
-        try: return Read.read(filename, **kwargs) if reader is None else reader(str(filename), **kwargs)
-        except IOError: raise IOError
-    def start(self, opener=None):
-        if str(self).startswith("http") or str(self).startswith("www"): __import__("webbrowser").open(str(self)); return self
-        if __import__("sys").platform == "win32":  # double quotes fail with cmd. # __import__("os").startfile(filename)  # works for files and folders alike, but if opener is given, e.g. opener="start"
-            __import__("subprocess").Popen(f"powershell start '{self.expanduser().resolve().str}'" if opener is None else rf'powershell {opener} \'{self}\''); return self  # fails for folders. Start must be passed, but is not defined.
-        elif __import__("sys").platform == 'linux': __import__("subprocess").call(["xdg-open", self.expanduser().resolve().str]); return self  # works for files and folders alike
-        else:  __import__("subprocess").call(["open", self.expanduser().resolve().str]); return self  # works for files and folders alike  # mac
-    def __call__(self, *args, **kwargs) -> 'P': self.start(*args, **kwargs); return self
-    def append_text(self, appendix) -> 'P': self.write_text(self.read_text() + appendix); return self
-    def cache_from(self, source_func, expire="1w", save=Save.pickle, reader=Read.read, **kwargs): return Cache(source_func=source_func, path=self, expire=expire, save=save, reader=reader, **kwargs)
-    def modify_text(self, txt_search, txt_alt, replace_line=False, notfound_append=False, prepend=False, encoding=None):
-        if not self.exists(): self.create(parents_only=True).write_text(txt_search)
-        return self.write_text(modify_text(txt_raw=self.read_text(encoding=encoding), txt_search=txt_search, txt_alt=txt_alt, replace_line=replace_line, notfound_append=notfound_append, prepend=prepend), encoding=encoding)
-    def download(self, directory=None, name=None, memory=False, allow_redirects=True, params=None) -> 'P':
-        response = __import__("requests").get(self.as_url_str(), allow_redirects=allow_redirects, params=params)  # Alternative: from urllib import request; request.urlopen(url).read().decode('utf-8').
-        return response if memory else (P.home().joinpath("Downloads") if directory is None else P(directory)).joinpath(validate_name(name or self.name)).create(parents_only=True).write_bytes(response.content)  # r.contents is bytes encoded as per docs of requests.
-    def _return(self, res, inlieu=False, inplace=False, operation=None, overwrite=False, orig=False, verbose=False, strict=True, msg="", __delayed_msg__="") -> 'P':
-        if inlieu: self._str = str(res)
-        if inplace:
-            assert self.exists(), f"`inplace` flag is only relevant if the path exists. It doesn't {self}"
-            if operation == "rename":
-                if overwrite and res.exists(): res.delete(sure=True, verbose=verbose)
-                if not overwrite and res.exists():
-                    if strict: raise FileExistsError(f"File {res} already exists.")
-                    else: print(f"SKIPPED RENAMING {repr(self)} ==> {repr(res)} because FileExistsError and scrict=False policy.") if verbose else None; return self if orig else res
-                self.rename(res); msg = msg or f"RENAMED {repr(self)} ==> {repr(res)}"
-            elif operation == "delete": self.delete(sure=True, verbose=False);  __delayed_msg__ = f"DELETED {repr(self)}."
-        print(msg) if verbose and msg != "" else None; print(__delayed_msg__) if verbose and __delayed_msg__ != "" else None; return self if orig else res
-    # ================================ Path Object management ===========================================
-    """ Distinction between Path object and the underlying file on disk that the path may refer to. Two distinct flags are used:
-        `inplace`: the operation on the path object will affect the underlying file on disk if this flag is raised, otherwise the method will only alter the string.
-        `inliue`: the method acts on the path object itself instead of creating a new one if this flag is raised.
-        `orig`: whether the method returns the original path object or a new one."""
-    def prepend(self, prefix, suffix=None, verbose=True, **kwargs): return self._return(self.parent.joinpath(prefix + self.trunk + (suffix or ''.join(('bruh'+self).suffixes))), operation="rename", verbose=verbose, **kwargs)  # Path('.ssh').suffix fails, 'bruh' fixes it.
-    def append(self, name='', index=False, suffix=None, verbose=True, **kwargs): return self.append(name=f'_{len(self.parent.search(f"*{self.stem}*"))}', index=False, verbose=verbose, suffix=suffix, **kwargs) if index else self._return(self.parent.joinpath(self.trunk + (name or "_" + timestamp()) + (suffix or ''.join(('bruh'+self).suffixes))), operation="rename", verbose=verbose, **kwargs)
-    def with_trunk(self, name, verbose=True, **kwargs): return self._return(self.parent.joinpath(name + "".join(self.suffixes)), operation="rename", verbose=verbose, **kwargs)  # Complementary to `with_stem` and `with_suffix`
-    def with_name(self, name, verbose=True, **kwargs): assert type(name) is str, "name must be a string."; return self._return(self.parent / name, verbose=verbose, operation="rename", **kwargs)
-    def switch(self, key: str, val: str, verbose=True, **kwargs): return self._return(P(str(self).replace(key, val)), operation="rename", verbose=verbose, **kwargs)  # Like string replce method, but `replace` is an already defined method."""
-    def switch_by_index(self, idx: int, val: str, verbose=True, **kwargs): return self._return(P(*[val if index == idx else value for index, value in enumerate(self.parts)]), operation="rename", verbose=verbose, **kwargs)
-    # ============================= attributes of object ======================================
-    trunk = property(lambda self: self.name.split('.')[0])  # """ useful if you have multiple dots in file path where `.stem` fails."""
-    len = property(lambda self: self.__len__()); items = property(lambda self: List(self.parts)); str = property(lambda self: str(self))  # or self._str
-    def __len__(self): return len(self.parts)
-    def __contains__(self, item): return P(item).as_posix() in self.as_posix()
-    def __iter__(self): return self.parts.__iter__()
-    def __deepcopy__(self) -> 'P': return P(str(self))
-    def __getstate__(self) -> str: return str(self)
-    def __setstate__(self, state): self._str = str(state)
-    def __add__(self, other) -> 'P': return self.parent.joinpath(self.name + str(other))  # used append and prepend if the addition wanted to be before suffix.
-    def __radd__(self, other) -> 'P': return self.parent.joinpath(str(other) + self.name)  # other + P and `other` doesn't know how to make this addition.
-    def __sub__(self, other) -> 'P': res = P(str(self).replace(str(other), "")); return (res[1:] if str(res[0]) in {"\\", "/"} else res) if len(res) else res  # paths starting with "/" are problematic. e.g ~ / "/path" doesn't work.
-    def rel2cwd(self, inlieu=False) -> 'P': return self._return(P(self.expanduser().absolute().relative_to(Path.cwd())), inlieu)
-    def rel2home(self, inlieu=False) -> 'P': return self._return(P(self.expanduser().absolute().relative_to(Path.home())), inlieu)  # very similat to collapseuser but without "~" being added so its consistent with rel2cwd.
-    def collapseuser(self, strict=True):
-        if strict: assert P.home() in self.expanduser().absolute().resolve(), ValueError(f"`{P.home()}` is not in the subpath of `{self}`")
-        return self if "~" in self else self._return(P("~") / (self.expanduser().absolute().resolve(strict=strict) - P.home()))    # opposite of `expanduser` resolve is crucial to fix Windows cases insensitivty problem.
-    def __getitem__(self, slici): return P(*[self[item] for item in slici]) if type(slici) is list else (P(*self.parts[slici]) if type(slici) is slice else P(self.parts[slici]))  # it is an integer
-    def __setitem__(self, key: str or int or slice, value: str or Path):
-        fullparts, new = list(self.parts), list(P(value).parts)
-        if type(key) is str: idx = fullparts.index(key); fullparts.remove(key); fullparts = fullparts[:idx] + new + fullparts[idx + 1:]
-        elif type(key) is int: fullparts = fullparts[:key] + new + fullparts[key + 1:]
-        elif type(key) is slice: fullparts = fullparts[:(0 if key.start is None else key.start)] + new + fullparts[(len(fullparts) if key.stop is None else key.stop):]
-        self._str = str(P(*fullparts))  # similar attributes: # self._parts # self._pparts # self._cparts # self._cached_cparts
-    def split(self, at: str = None, index: int = None, sep=[-1, 0, 1][-1], strict=True):
-        if index is None and (at is not None):  # at is provided  # ====================================   Splitting
-            if not strict:  # behaves like split method of string
-                one, two = (items := str(self).split(sep=str(at)))[0], items[1]; one, two = P(one[:-1]) if one.endswith("/") else P(one), P(two[1:]) if two.startswith("/") else P(two)
-            else:  # "strict": # raises an error if exact match is not found.
-                index = self.parts.index(str(at)); one, two = self[0:index], self[index + 1:]  # both one and two do not include the split item.
-        elif index is not None and (at is None):  # index is provided
-            one, two = self[:index], P(*self.parts[index + 1:]); at = self[index]  # this is needed below.
-        else: raise ValueError("Either `index` or `at` can be provided. Both are not allowed simulatanesouly.")
-        if sep == 0: return one, two  # neither of the portions get the sperator appended to it. # ================================  appending `at` to one of the portions
-        elif sep == 1: return one, at / two   # append it to right portion
-        elif sep == -1: return one / at, two  # append it to left portion.
-        else: raise ValueError(f"`sep` should take a value from the set [-1, 0, 1] but got {sep}")
-    def __repr__(self):  # this is useful only for the console
-        if self.is_symlink():
-            try: target = self.resolve()  # broken symolinks are funny, and almost always fail `resolve` method.
-            except Exception: target = "BROKEN LINK " + str(self)  # avoid infinite recursions for broken links.
-            return "P: Symlink '" + str(self) + "' ==> " + repr(str(target) if target == self else target)
-        elif self.is_absolute(): return "P: " + self._type() + " '" + self.clickable() + "'" + (" | " + self.time(which="c").isoformat()[:-7].replace("T", "  ") if self.exists() else "") + (f" | {self.size()} Mb" if self.is_file() else "")
-        elif "http" in str(self): return "P: URL " + self.as_url_str()
-        else: return "P: Relative " + "'" + str(self) + "'"  # not much can be said about a relative path.
-    # def __str__(self): return self.as_url_str() if "http" in self else self._str
-    def size(self, units='mb'):  # ===================================== File Specs ==========================================================================================
-        total_size = self.stat().st_size if self.is_file() else sum([item.stat().st_size for item in self.rglob("*") if item.is_file()])
-        return round(total_size / dict(zip(List(['b', 'kb', 'mb', 'gb']).eval("self+self.swapcase()"), 2 * [1024 ** item for item in range(4)]))[units], 1)
-    def time(self, which=["m", "c", "a"][0], **kwargs): return datetime.fromtimestamp({"m": self.stat().st_mtime, "a": self.stat().st_atime, "c": self.stat().st_ctime}[which], **kwargs)  # m last mofidication of content, i.e. the time it was created. c last status change (its inode is changed, permissions, path, but not content) a: last access
-    def stats(self): return Struct(size=self.size(), content_mod_time=self.time(which="m"), attr_mod_time=self.time(which="c"), last_access_time=self.time(which="a"), group_id_owner=self.stat().st_gid, user_id_owner=self.stat().st_uid)
-    # ================================ String Nature management ====================================
-    def _type(self): return ("File" if self.is_file() else ("Dir" if self.is_dir() else "NotExist")) if self.absolute() else "Relative"
-    def clickable(self, inlieu=False) -> 'P': return self._return(self.expanduser().resolve().as_uri(), inlieu)
-    def as_url_str(self, inlieu=False) -> 'P': return self._return(self.as_posix().replace("https:/", "https://").replace("http:/", "http://"), inlieu)
-    def as_url_obj(self, inlieu=False) -> 'P': return self._return(install_n_import("urllib3").connection_from_url(self), inlieu)
-    def as_unix(self, inlieu=False) -> 'P': return self._return(P(str(self).replace('\\', '/').replace('//', '/')), inlieu)
-    def as_zip_path(self): res = self.expanduser().resolve(); return __import__("zipfile").Path(res)  # .str.split(".zip") tmp=res[1]+(".zip" if len(res) > 2 else ""); root=res[0]+".zip", at=P(tmp).as_posix())  # TODO
-    def get_num(self, astring=None): int("".join(filter(str.isdigit, str(astring or self.stem))))
-    def validate_name(self, replace='_'): validate_name(self.trunk, replace=replace)
-    # ========================== override =======================================
-    def write_text(self, data: str, **kwargs) -> 'P': super(P, self).write_text(data, **kwargs); return self
-    def read_text(self, encoding=None, lines=False, printit=False) -> str: res = super(P, self).read_text(encoding=encoding) if not lines else List(super(P, self).read_text(encoding=encoding).splitlines()); print(res) if printit else None; return res
-    def write_bytes(self, data: bytes) -> 'P':
-        res = super(P, self).write_bytes(data)
-        if res == 0: raise RuntimeError(f"Could not save file on disk.")
-        return self
-    def touch(self, mode: int = 0o666, parents=True, exist_ok: bool = ...) -> 'P': self.parent.create(parents=parents) if parents else None; super(P, self).touch(mode=mode, exist_ok=exist_ok); return self
-    def symlink_from(self, src_folder=None, src_file=None, verbose=False, overwrite=False):
-        assert self.expanduser().exists(), "self must exist if this method is used."
-        if src_file is not None: assert src_folder is None, "You can only pass source or source_dir, not both."; result = P(src_file).expanduser().absolute()
-        else: result = P(src_folder or P.cwd()).expanduser().absolute() / self.name
-        return result.symlink_to(self, verbose=verbose, overwrite=overwrite)
-    def symlink_to(self, target=None, verbose=True, overwrite=False, orig=False):
-        self.parent.create(); assert (target := P(target).expanduser().resolve()).exists(), f"Target path `{target}` doesn't exist. This will create a broken link."
-        if overwrite and (self.is_symlink() or self.exists()): self.delete(sure=True, verbose=verbose)
-        if __import__("platform").system() == "Windows" and not (tm := __import__("crocodile").meta.Terminal).is_user_admin():  # you cannot create symlink without priviliages.
-            tm.run_as_admin(file=__import__("sys").executable, params=f" -c \"from pathlib import Path; Path(r'{self.expanduser()}').symlink_to(r'{str(target)}')\"", wait=2)
-        else: super(P, self.expanduser()).symlink_to(str(target))
-        return self._return(P(target), inlieu=False, inplace=False, orig=orig, verbose=verbose, msg=f"LINKED {repr(self)}")
-    def resolve(self, strict=False):
-        try: return super(P, self).resolve(strict=strict)
-        except OSError: return self
-    # ======================================== Folder management =======================================
-    def search(self, pattern='*', r=False, files=True, folders=True, compressed=False, dotfiles=False, filters: list = None, not_in: list = None, exts=None, win_order=False) -> List:
-        filters = (filters or []) + ([lambda x: all([str(notin) not in str(x) for notin in not_in])] if not_in is not None else []) + ([lambda x: any([ext in x.name for ext in exts])] if exts is not None else [])
-        if ".zip" in (slf := self.expanduser().resolve()) and compressed:  # the root (self) is itself a zip archive (as opposed to some search results are zip archives)
-            root = slf.as_zip_path(); raw = List(root.iterdir()) if not r else List(__import__("zipfile").ZipFile(str(slf)).namelist()).apply(lambda x: root.joinpath(x))
-            return raw.filter(lambda zip_path: __import__("fnmatch").fnmatch(zip_path.at, pattern)).filter(lambda x: (folders or x.is_file()) and (files or x.is_dir()))  # .apply(lambda x: P(str(x)))
-        elif dotfiles: raw = slf.glob(pattern) if not r else self.rglob(pattern)
-        else: raw = __import__("glob").glob(str(slf / "**" / pattern), recursive=r) if r else __import__("glob").glob(str(slf.joinpath(pattern)))  # glob ignroes dot and hidden files
-        if ".zip" not in slf and compressed: raw += List([P(comp_file).search(pattern=pattern, r=r, files=files, folders=folders, compressed=True, dotfiles=dotfiles, filters=filters, not_in=not_in, win_order=win_order) for comp_file in self.search("*.zip", r=r)]).reduce().list
-        processed = List([P(item) for item in raw if (lambda item_: all([item_.is_dir() if not files else True, item_.is_file() if not folders else True] + [afilter(item_) for afilter in filters]))(P(item))])
-        return processed if not win_order else processed.sort(key=lambda x: [int(k) if k.isdigit() else k for k in __import__("re").split('([0-9]+)', x.stem)])
-    def tree(self, *args, **kwargs): return __import__("crocodile.msc.odds").msc.odds.__dict__['tree'](self, *args, **kwargs)
-    # def find(self, *args, r=True, compressed=True, **kwargs) -> 'P':  # short for the method ``search`` then pick first item from results. useful for superflous directories or zip archives containing a single file."""
-    #     if compressed is False and self.is_file(): return self
-    #     if len(results := self.search(*args, r=r, compressed=compressed, **kwargs)) > 0: return results[0].unzip() if ".zip" in str(results[0]) else results[0]
-    browse = property(lambda self: self.search("*").to_struct(key_val=lambda x: ("qq_" + validate_name(x), x)).clean_view)
-    def create(self, parents=True, exist_ok=True, parents_only=False) -> 'P': self.parent.mkdir(parents=parents, exist_ok=exist_ok) if parents_only else self.mkdir(parents=parents, exist_ok=exist_ok); return self
-    def chdir(self) -> 'P': __import__("os").chdir(str(self.expanduser())); return self
-    def listdir(self) -> List: return List(__import__("os").listdir(self.expanduser().resolve())).apply(P)
-    tempdir = staticmethod(lambda: P(__import__("tempfile").mktemp()))
-    temp = staticmethod(lambda: P(__import__("tempfile").gettempdir()))
-    tmpdir = staticmethod(lambda prefix="": P.tmp(folder=rf"tmp_dirs/{prefix + ('_' if prefix != '' else '') + randstr()}"))
-    tmpfile = staticmethod(lambda name=None, suffix="", folder=None, tstamp=False: P.tmp(file=(name or randstr()) + "_" + randstr() + (("_" + timestamp()) if tstamp else "") + suffix, folder=folder or "tmp_files"))
-    tmp = staticmethod(lambda folder=None, file=None, root="~/tmp_results": P(root).expanduser().create().joinpath(folder or "").joinpath(file or "").create(parents_only=True if file else False))
-    # ====================================== Compression & Encryption ===========================================
-    def zip(self, path=None, folder=None, name=None, arcname=None, inplace=False, verbose=True, content=False, orig=False, use_7z=False, pwd=None, **kwargs) -> 'P':
-        path, slf = self._resolve_path(folder, name, path, self.name).expanduser().resolve(), self.expanduser().resolve()
-        if use_7z: path = seven_zip(path=slf, op_path=path, pwd=pwd)
-        else:
-            if (arcname := P(arcname or slf.name)).name != slf.name: arcname /= slf.name  # arcname has to start from somewhere and end with filename
-            if slf.is_file(): path = Compression.zip_file(ip_path=slf, op_path=path + f".zip" if path.suffix != ".zip" else path, arcname=arcname, **kwargs)
-            else:
-                root_dir, base_dir = (slf, ".") if content else (slf.split(at=str(arcname[0]))[0], arcname)
-                path = Compression.compress_folder(root_dir=root_dir, op_path=path, base_dir=base_dir, fmt='zip', **kwargs)
-        return self._return(path, inlieu=False, inplace=inplace, operation="delete", orig=orig, verbose=verbose, msg=f"ZIPPED {repr(slf)} ==>  {repr(path)}")
-    def unzip(self, folder=None, fname=None, verbose=True, content=False, inplace=False, overwrite=False, merge=True, orig=False, pwd=None, **kwargs) -> 'P':
-        slf = zipfile = self.expanduser().resolve()
-        if any(ztype in slf.parent for ztype in (".zip", ".7z")):  # path include a zip archive in the middle.
-            if (ztype := [item for item in (".zip", ".7z", "") if item in str(slf)][0]) == "": return slf
-            zipfile, fname = slf.split(at=List(slf.parts).filter(lambda x: ztype in x)[0], sep=-1)
-        folder = (zipfile.parent / zipfile.stem) if folder is None else P(folder).expanduser().absolute().resolve().joinpath(zipfile.stem)
-        folder = folder if not content else folder.parent
-        if slf.suffix == ".7z": P(folder).delete(sure=True) if overwrite else None; result = un_seven_zip(path=slf, op_dir=folder, pwd=pwd)
-        else:
-            if overwrite:
-                if not content: P(folder).joinpath(fname or "").delete(sure=True, verbose=True)  # deletes a specific file / folder that has the same name as the zip file without extension.
-                else: List([x for x in __import__("zipfile").ZipFile(self.str).namelist() if "/" not in x or (len(x.split('/')) == 2 and x.endswith("/"))]).apply(lambda item: P(folder).joinpath(fname or "", item.replace("/", "")).delete(sure=True, verbose=True))
-            result = Compression.unzip(zipfile, folder, None if fname is None else P(fname).as_posix(), **kwargs)
-        return self._return(result, inlieu=False, inplace=inplace, operation="delete", orig=orig, verbose=verbose, msg=f"UNZIPPED {repr(zipfile)} ==> {repr(result)}")
-    def tar(self, path=None, name=None, folder=None, inplace=False, orig=False, verbose=True) -> 'P': Compression.tar(self.expanduser().resolve(), op_path := self._resolve_path(folder, name, path, self.name + ".tar").expanduser().resolve()); return self._return(op_path, inlieu=False, inplace=inplace, operation="delete", orig=orig, verbose=verbose, msg=f"TARRED {repr(self)} ==>  {repr(op_path)}")
-    def untar(self, folder=None, path=None, name=None, inplace=False, orig=False, verbose=True) -> 'P': Compression.untar(self.expanduser().resolve(), op_path := self._resolve_path(folder, name, path, self.name.replace(".tar", "")).expanduser().resolve()); return self._return(op_path, inlieu=False, inplace=inplace, operation="delete", orig=orig, verbose=verbose, msg=f"UNTARRED {repr(self)} ==>  {repr(op_path)}")
-    def gz(self, path=None, folder=None, name=None, inplace=False, orig=False, verbose=True) -> 'P': Compression.gz(self.expanduser().resolve(), op_path := self._resolve_path(folder, name, path, self.name + ".gz").expanduser().resolve()); return self._return(op_path, inlieu=False, inplace=inplace, operation="delete", orig=orig, verbose=verbose, msg=f"GZED {repr(self)} ==>  {repr(op_path)}")
-    def ungz(self, folder=None, name=None, path=None, inplace=False, orig=False, verbose=True) -> 'P': Compression.ungz(self.expanduser().resolve(), op_path := self._resolve_path(folder, name, path, self.name.replace(".gz", "")).expanduser().resolve()); return self._return(op_path, inlieu=False, inplace=inplace, operation="delete", orig=orig, verbose=verbose, msg=f"UNGZED {repr(self)} ==>  {repr(op_path)}")
-    def xz(self, path=None, name=None, folder=None, inplace=False, orig=False, verbose=True) -> 'P': Compression.xz(self.expanduser().resolve(), op_path := self._resolve_path(folder, name, path, self.name + ".xz").expanduser().resolve()); return self._return(op_path, inlieu=False, inplace=inplace, operation="delete", orig=orig, verbose=verbose, msg=f"XZED {repr(self)} ==>  {repr(op_path)}")
-    def unxz(self, folder=None, name=None, path=None, inplace=False, orig=False, verbose=True) -> 'P': Compression.unxz(self.expanduser().resolve(), op_path := self._resolve_path(folder, name, path, self.name.replace(".xz", "")).expanduser().resolve()); return self._return(op_path, inlieu=False, inplace=inplace, operation="delete", orig=orig, verbose=verbose, msg=f"UNXZED {repr(self)} ==>  {repr(op_path)}")
-    def tar_gz(self, folder=None, name=None, path=None, inplace=False, orig=False, verbose=True) -> 'P': return self.tar(inplace=inplace).gz(folder=folder, name=name, path=path, inplace=True, orig=orig, verbose=verbose)
-    def ungz_untar(self, folder=None, name=None, path=None, inplace=False, verbose=True, orig=False) -> 'P': return self.ungz(inplace=inplace).untar(folder=folder, name=name, path=path, inplace=True, orig=orig, verbose=verbose)
-    def tar_xz(self, folder=None, name=None, path=None, inplace=False, verbose=True, orig=False) -> 'P': return self.tar(inplace=inplace).xz(folder=folder, name=name, path=path, inplace=True, orig=orig, verbose=verbose)
-    def unxz_untar(self, folder=None, name=None, path=None, inplace=False,  verbose=True, orig=False) -> 'P': return self.unxz(inplace=inplace).untar(folder=folder, name=name, path=path, inplace=True, orig=orig, verbose=verbose)
-    def decompress(self, folder=None, name=None, path=None, inplace=False,  verbose=True, orig=False) -> 'P': raise NotImplementedError("Not implemented yet.")
-    def encrypt(self, key=None, pwd=None, folder=None, name=None, path=None, verbose=True, suffix=".enc", inplace=False, orig=False) -> 'P':  # see: https://stackoverflow.com/questions/42568262/how-to-encrypt-text-with-a-password-in-python & https://stackoverflow.com/questions/2490334/simple-way-to-encode-a-string-according-to-a-password"""
-        slf = self.expanduser().resolve(); path = self._resolve_path(folder, name, path, slf.name+suffix)
-        assert slf.is_file(), f"Cannot encrypt a directory. You might want to try `zip_n_encrypt`. {self}"; path.write_bytes(encrypt(msg=slf.read_bytes(), key=key, pwd=pwd))
-        return self._return(path, inlieu=False, inplace=inplace, operation="delete", orig=orig, verbose=verbose, msg=f"ENCRYPTED: {repr(slf)} ==> {repr(path)}.")
-    def decrypt(self, key=None, pwd=None, path=None, folder=None, name=None, verbose=True, suffix=".enc", **kwargs) -> 'P':
-        slf = self.expanduser().resolve(); path = self._resolve_path(folder, name, path, slf.name.replace(suffix, "") if suffix in slf.name else "decrypted_" + slf.name).write_bytes(decrypt(slf.read_bytes(), key=key, pwd=pwd))
-        return self._return(path, operation="delete", verbose=verbose, msg=f"DECRYPTED: {repr(slf)} ==> {repr(path)}.", **kwargs)
-    def zip_n_encrypt(self, key=None, pwd=None, inplace=False, verbose=True, orig=False, content=False) -> 'P': return self.zip(inplace=inplace, verbose=verbose, content=content).encrypt(key=key, pwd=pwd, verbose=verbose, inplace=True) if not orig else self
-    def decrypt_n_unzip(self, key=None, pwd=None, inplace=False, verbose=True, orig=False) -> 'P': return self.decrypt(key=key, pwd=pwd, verbose=verbose, inplace=inplace).unzip(folder=None, inplace=True, content=False) if not orig else self
-    def _resolve_path(self, folder, name, path, default_name, rel2it=False) -> 'P':  # From all arguments, figure out what is the final path.
-        """:param rel2it: `folder` or `path` are relative to `self` as opposed to cwd. This is used when resolving '../dir'"""
-        if path is not None:
-            path = P(self.joinpath(path).resolve() if rel2it else path).expanduser().resolve()
-            assert folder is None and name is None, f"If `path` is passed, `folder` and `name` cannot be passed."; assert not path.is_dir(), f"`path` passed is a directory! it must not be that. If this is meant, pass it with `folder` kwarg. `{path}`"
-            return path
-        name, folder = (default_name if name is None else str(name)), (self.parent if folder is None else folder)  # good for edge cases of path with single part.  # means same directory, just different name
-        return P(self.joinpath(folder).resolve() if rel2it else folder).expanduser().resolve() / name
-    def checksum(self, kind=["md5", "sha256"][1]): import hashlib; myhash = {"md5": hashlib.md5, "sha256": hashlib.sha256}[kind](); myhash.update(self.read_bytes()); return myhash.hexdigest()
-    get_env = staticmethod(lambda: get_env())
-    def transfer_sh(self) -> 'P': return P(__import__("requests").put(f"https://transfer.sh/{self.expanduser().name}", self.expanduser().absolute().read_bytes()).text)
-
-
-def compress_folder(root_dir, op_path, base_dir, fmt='zip', **kwargs):  # shutil works with folders nicely (recursion is done interally) # directory to be archived: root_dir\base_dir, unless base_dir is passed as absolute path. # when archive opened; base_dir will be found."""
-    assert fmt in {"zip", "tar", "gztar", "bztar", "xztar"}  # .zip is added automatically by library, hence we'd like to avoid repeating it if user sent it.
-    return P(__import__('shutil').make_archive(base_name=str(op_path)[:-4] if str(op_path).endswith(".zip") else str(op_path), format=fmt, root_dir=str(root_dir), base_dir=str(base_dir), **kwargs))  # returned path possible have added extension.
-def zip_file(ip_path, op_path, arcname=None, password=None, mode="w", **kwargs):
-    """arcname determines the directory of the file being archived inside the archive. Defaults to same as original directory except for drive.
-    When changed, it should still include the file path in its end. If arcname = filename without any path, then, it will be in the root of the archive."""
-    import zipfile
-    with zipfile.ZipFile(str(op_path), mode=mode) as jungle_zip:
-        jungle_zip.setpassword(pwd=password) if password is not None else None
-        jungle_zip.write(filename=str(ip_path), arcname=str(arcname) if arcname is not None else None, compress_type=zipfile.ZIP_DEFLATED, **kwargs)
-    return P(op_path)
-def unzip(ip_path, op_path=None, fname=None, password=None, memory=False, **kwargs):
-    with __import__("zipfile").ZipFile(str(ip_path), 'r') as zipObj:
-        if memory: return Struct({name: zipObj.read(name) for name in zipObj.namelist()}) if fname is None else zipObj.read(fname)
-        if fname is None: zipObj.extractall(op_path, pwd=password, **kwargs); return P(op_path)
-        else: zipObj.extract(member=str(fname), path=str(op_path), pwd=password); return P(op_path) / fname
-def seven_zip(path: P, op_path: P, pwd=None, mode='w'):  # benefits over regular zip and encrypt: can handle very large files with low memory footprint
-    op_path = op_path + '.7z' if not op_path.suffix == '.7z' else op_path
-    if (env := get_env()).system == "Windows":
-        env.tm.run('winget install --name "7-zip" --Id "7zip.7zip" --source winget', shell="powershell") if not (program := env.ProgramFiles.joinpath("7-Zip/7z.exe")).exists() else None
-        res = env.tm.run(f"&'{program}' a '{op_path}' '{path}' {f'-p{pwd}' if pwd is not None else ''}", shell="powershell"); assert res.is_successful, res.print(); return op_path
-    elif env.system == "Linux":  # python variant is much slower than 7-zip, and consumes more memroy, see py7zr project on github.
-        op_path = op_path + '.7z' if not op_path.suffix == '.7z' else op_path; py7zr = install_n_import("py7zr")
-        with py7zr.SevenZipFile(op_path, mode, password=pwd) as archive: archive.writeall(path)
-        return op_path
-def un_seven_zip(path, op_dir, overwrite=False, pwd=None):  # TODO: use py7zr instead of two implementations for linux and windows.
-    if (env := get_env()).system == "Windows":
-        env.tm.run('winget install --name "7-zip" --Id "7zip.7zip" --source winget', shell="powershell") if not (program := env.ProgramFiles.joinpath("7-Zip/7z.exe")).exists() else None
-        res = env.tm.run(f"&'{program}' x",  f"'{path}'",  f"-o'{op_dir}'", f"-p{pwd}" if pwd is not None else '', shell="powershell"); assert res.is_successful, res.print(); return op_dir
-    else: raise NotImplementedError("7z not implemented for Linux")
-def gz(file, op_path):  # see this on what to use: https://stackoverflow.com/questions/10540935/what-is-the-difference-between-tar-and-zip
-    with open(file, 'rb') as f_in:
-        with __import__("gzip").open(op_path, 'wb') as f_out:  __import__("shutil").copyfileobj(f_in, f_out)
-    return P(op_path)
-def ungz(self, op_path=None):
-    with __import__("gzip").open(str(self), 'r') as f_in, open(op_path, 'wb') as f_out: __import__("shutil").copyfileobj(f_in, f_out)
-    return P(op_path)
-def xz(self, op_path):
-    with __import__("lzma").open(op_path, "w") as f: f.write(self)
-def unxz(ip_path, op_path):
-    with __import__("lzma").open(ip_path) as file: P(op_path).write_bytes(file.read())
-def tar(self, op_path):
-    with __import__("tarfile").open(op_path, "w:gz") as tar_: tar_.add(str(self), arcname=__import__("os").path.basename(str(self)))
-    return P(op_path)
-def untar(self, op_path, fname=None, mode='r', **kwargs):
-    with __import__("tarfile").open(str(self), mode) as file:
-        if fname is None: file.extractall(path=op_path, **kwargs)  # extract all files in the archive
-        else: file.extract(fname, **kwargs)
-    return P(op_path)
-class Compression: compress_folder = compress_folder; zip_file = zip_file; unzip = unzip; gz = gz; ungz = ungz; tar = tar; untar = untar; xz = xz; unxz = unxz  # Provides consistent behaviour across all methods
-
-
-class Cache:  # This class helps to accelrate access to latest data coming from expensive function. The class has two flavours, memory-based and disk-based variants."""
-    def __init__(self, source_func, expire="1m", logger=None, path=None, save=Save.pickle, reader=Read.read):
-        self.cache = None  # fridge content
-        self.source_func = source_func  # function which when called returns a fresh object to be frozen.
-        self.path = P(path) if path else None  # if path is passed, it will function as disk-based flavour.
-        self.time_produced, self.save, self.reader, self.logger, self.expire = None, save, reader, logger, expire
-    age = property(lambda self: datetime.now() - self.time_produced if self.path is None else datetime.now() - self.path.stats().content_mod_time)
-    def __setstate__(self, state): self.__dict__.update(state); self.path = P.home() / self.path if self.path is not None else self.path
-    def __getstate__(self): state = self.__dict__.copy(); state["path"] = self.path.rel2home() if self.path is not None else state["path"]; return state  # With this implementation, instances can be pickled and loaded up in different machine and still works.
-    def __call__(self, fresh=False):
-        if self.path is None:  # Memory Cache
-            if self.cache is None or fresh is True or self.age > str2timedelta(self.expire): self.cache, self.time_produced = self.source_func(), datetime.now(); self.logger.debug(f"Updating / Saving data from {self.source_func}") if self.logger else None
-            elif self.logger: self.logger.debug(f"Using cached values. Lag = {self.age}.")
-        elif fresh or not self.path.exists() or self.age > str2timedelta(self.expire):  # disk fridge
-            if self.logger: self.logger.debug(f"Updating & Saving {self.path} ...")
-            self.cache = self.source_func(); self.save(obj=self.cache, path=self.path)  # fresh order, never existed or exists but expired.
-        elif self.age < str2timedelta(self.expire) and self.cache is None: self.cache = self.reader(self.path)  # this implementation favours reading over pulling fresh at instantiation.  # exists and not expired. else # use the one in memory self.cache
-        return self.cache
-
-
-if __name__ == '__main__':
-    # print('hi from file_managements')
-    pass
+
+from crocodile.core import Struct, List, timestamp, randstr, validate_name, str2timedelta, Save, Path, get_env, install_n_import
+from datetime import datetime
+
+# %% =============================== Security ================================================
+def obscure(msg: bytes) -> bytes: return __import__("base64").urlsafe_b64encode(__import__("zlib").compress(msg, 9))
+def unobscure(obscured: bytes) -> bytes: return __import__("zlib").decompress(__import__("base64").urlsafe_b64decode(obscured))
+def pwd2key(password: str, salt=None, iterations=None) -> bytes:  # Derive a secret key from a given password and salt"""
+    if salt is None: m = __import__("hashlib").sha256(); m.update(password.encode("utf-8")); return __import__("base64").urlsafe_b64encode(m.digest())  # make url-safe bytes required by Ferent.
+    from cryptography.hazmat.primitives import hashes; from cryptography.hazmat.primitives.kdf.pbkdf2 import PBKDF2HMAC
+    return __import__("base64").urlsafe_b64encode(PBKDF2HMAC(algorithm=hashes.SHA256(), length=32, salt=salt, iterations=iterations, backend=None).derive(password.encode()))
+def encrypt(msg: bytes, key=None, pwd: str = None, salted=True, iteration: int = None, gen_key=False) -> bytes:
+    salt = None  # silence the linter.
+    if pwd is not None:  # generate it from password
+        assert (key is None) and (type(pwd) is str), f"You can either pass key or pwd, or none of them, but not both."
+        salt, iteration = (__import__('secrets').token_bytes(16), iteration or __import__('secrets').randbelow(1_000_000)) if salted else (None, None); key = pwd2key(pwd, salt, iteration)
+    elif key is None:
+        if gen_key: key = __import__("cryptography.fernet").__dict__["fernet"].Fernet.generate_key(); P.home().joinpath('dotfiles/creds/data/encrypted_files_key.bytes').write_bytes(key)
+        else:
+            try: key = P.home().joinpath("dotfiles/creds/data/encrypted_files_key.bytes").read_bytes()  # read from file
+            except FileNotFoundError as err: print("\n"*3, "~"*50, f"""Consider Loading up your dotfiles or pass `gen_key=True` to make and save one.""", "~"*50, "\n"*3); raise FileNotFoundError(err)
+    elif type(key) in {str, P, Path}: key = P(key).read_bytes()  # a path to a key file was passed, read it:
+    elif type(key) is bytes: pass  # key passed explicitly
+    else: raise TypeError(f"Key must be either a path, bytes object or None.")
+    code = __import__("cryptography.fernet").__dict__["fernet"].Fernet(key).encrypt(msg)
+    return __import__("base64").urlsafe_b64encode(b'%b%b%b' % (salt, iteration.to_bytes(4, 'big'), __import__("base64").urlsafe_b64decode(code))) if pwd is not None and salted is True else code
+def decrypt(token: bytes, key=None, pwd: str = None, salted=True) -> bytes:
+    if pwd is not None:
+        assert key is None, f"You can either pass key or pwd, or none of them, but not both."
+        if salted:
+            decoded = __import__("base64").urlsafe_b64decode(token); salt, iterations, token = decoded[:16], decoded[16:20], __import__("base64").urlsafe_b64encode(decoded[20:])
+            key = pwd2key(pwd, salt, int.from_bytes(iterations, 'big'))
+        else: key = pwd2key(pwd)  # trailing `;` prevents IPython from caching the result.
+    if type(key) is bytes: pass  # passsed explicitly
+    elif key is None: key = P("~/dotfiles/creds/data/encrypted_files_key.bytes").expanduser().read_bytes()  # read from file
+    elif type(key) in {str, P, Path}: key = P(key).read_bytes()  # passed a path to a file containing kwy
+    else: raise TypeError(f"Key must be either str, P, Path, bytes or None. Recieved: {type(key)}")
+    return __import__("cryptography.fernet").__dict__["fernet"].Fernet(key).decrypt(token)
+def unlock(drive="D:", pwd=None, auto_unlock=False):
+    return __import__("crocodile").meta.Terminal().run(f"""$SecureString = ConvertTo-SecureString "{pwd or P.home().joinpath("dotfiles/creds/data/bitlocker_pwd").read_text()}" -AsPlainText -Force; Unlock-BitLocker -MountPoint "{drive}" -Password $SecureString; """ + (f'Enable-BitLockerAutoUnlock -MountPoint "{drive}"' if auto_unlock else ''), shell="pwsh")
+
+# %% =================================== File ============================================
+def read(path, **kwargs):
+    suffix = Path(path).suffix[1:]
+    try: return getattr(Read, suffix)(str(path), **kwargs)
+    except AttributeError as err:
+        if "type object 'Read' has no attribute" not in str(err): raise AttributeError(err)
+        if suffix in ('eps', 'jpg', 'jpeg', 'pdf', 'pgf', 'png', 'ps', 'raw', 'rgba', 'svg', 'svgz', 'tif', 'tiff'): return __import__("matplotlib").pyplot.imread(path, **kwargs)  # from: plt.gcf().canvas.get_supported_filetypes().keys():
+        raise AttributeError(f"Unknown file type. failed to recognize the suffix `{suffix}`. According to libmagic1, the file seems to be: {install_n_import('magic', 'python-magic').from_file(path)}")
+def json(path, r=False, **kwargs):
+    try: mydict = __import__("json").loads(P(path).read_text(), **kwargs)
+    except Exception: mydict = install_n_import("pyjson5").loads(P(path).read_text(), **kwargs)  # file has C-style comments.
+    return Struct.recursive_struct(mydict) if r else Struct(mydict)
+def yaml(path, r=False):
+    with open(str(path), "r") as file: mydict = __import__("yaml").load(file, Loader=__import__("yaml").FullLoader)
+    return Struct(mydict) if not r else Struct.recursive_struct(mydict)
+def ini(path): import configparser; res = configparser.ConfigParser(); res.read(str(path)); return res
+def toml(path): return __import__("tomli").loads(P(path).read_text())
+def npy(path, **kwargs): data = (np := __import__("numpy")).load(str(path), allow_pickle=True, **kwargs); data = data.item() if data.dtype == np.object else data; return Struct(data) if type(data) is dict else data
+def mat(path, remove_meta=False, **kwargs): res = Struct(__import__("scipy.io").__dict__["io"].loadmat(path, **kwargs)); List(res.keys()).filter("x.startswith('__')").apply(lambda x: res.__delattr__(x)) if remove_meta else None; return res
+def csv(path, **kwargs): return __import__("pandas").read_csv(path, **kwargs)
+def py(path, init_globals=None, run_name=None): return Struct(__import__("runpy").run_path(path, init_globals=init_globals, run_name=run_name))
+def pickles(bytes_obj): return __import__("dill").loads(bytes_obj)  # handles imports automatically provided that saved object was from an imported class (not in defined in __main__)
+def pickle(path, **kwargs): obj = __import__("dill").loads(P(path).read_bytes(), **kwargs); return Struct(obj) if type(obj) is dict else obj
+def pkl(*args, **kwargs): return pickle(*args, **kwargs)
+class Read: read = read; mat = mat; json = json; yaml = yaml; ini = ini; npy = npy; csv = csv; pkl = pkl; py = py; pickle = pickle; toml = toml; txt = lambda path, encoding=None: P(path).read_text(encoding=encoding)
+
+
+def modify_text(txt_raw, txt_search, txt_alt, replace_line=True, notfound_append=False, prepend=False):
+    lines, bingo = txt_raw.split("\n"), False
+    if not replace_line:  # no need for line splitting
+        if txt_search in txt_raw: return txt_raw.replace(txt_search, txt_alt)
+        return txt_raw + "\n" + txt_alt if notfound_append else txt_raw
+    for idx, line in enumerate(lines):
+        if txt_search in line:
+            lines[idx], bingo = txt_alt if type(txt_alt) is str else txt_alt(line), True
+    if bingo is False and notfound_append is True: (lines.insert(0, txt_alt) if prepend else lines.append(txt_alt))  # txt not found, add it anyway.
+    return "\n".join(lines)
+
+
+class P(type(Path()), Path):
+    # ============= Path management ==================
+    """ The default behaviour of methods acting on underlying disk object is to perform the action and return a new path referring to the mutated object in disk drive.
+    However, there is a flag `orig` that makes the function return orignal path object `self` as opposed to the new one pointing to new object.
+    Additionally, the fate of the original object can be decided by a flag `inplace` which means `replace` it defaults to False and in essence, it deletes the original underlying object.
+    This can be seen in `zip` and `encrypt` but not in `copy`, `move`, `retitle` because the fate of original file is dictated already.
+    Furthermore, those methods are accompanied with print statement explaining what happened to the object."""
+    def delete(self, sure=False, verbose=True) -> 'P':  # slf = self.expanduser().resolve() don't resolve symlinks.
+        if not sure: print(f"Did NOT DELETE because user is not sure. file: {repr(self)}.") if verbose else None; return self
+        if not self.exists(): self.unlink(missing_ok=True); print(f"Could NOT DELETE nonexisting file {repr(self)}. ") if verbose else None; return self  # broken symlinks exhibit funny existence behaviour, catch them here.
+        self.unlink(missing_ok=True) if self.is_file() or self.is_symlink() else __import__("shutil").rmtree(self, ignore_errors=False); print(f"DELETED {repr(self)}.") if verbose else None; return self
+    def send2trash(self, verbose=True) -> 'P':
+        if self.exists(): install_n_import("send2trash").send2trash(self.resolve().str); print(f"TRASHED {repr(self)}") if verbose else None  # do not expand user symlinks.
+        elif verbose: print(f"Could NOT trash {self}"); return self
+    def move(self, folder=None, name=None, path=None, rel2it=False, overwrite=False, verbose=True, parents=True, content=False) -> 'P':
+        path = self._resolve_path(folder=folder, name=name, path=path, default_name=self.absolute().name, rel2it=rel2it)
+        path.parent.create(parents=True, exist_ok=True) if parents else None; slf = self.expanduser().resolve()
+        if content:
+            assert self.is_dir(), NotADirectoryError(f"When `content` flag is set to True, path must be a directory. It is not: `{repr(self)}`")
+            self.search("*").apply(lambda x: x.move(folder=path.parent, content=False, overwrite=overwrite)); return path  # contents live within this directory.
+        if overwrite: tmp_path = slf.rename(path.parent.absolute() / randstr()); path.delete(sure=True, verbose=verbose); tmp_path.rename(path)  # works if moving a path up and parent has same name
+        else: slf.rename(path)  # self._return(res=path, inplace=True, operation='rename', orig=False, verbose=verbose, strict=True, msg='')
+        print(f"MOVED {repr(self)} ==> {repr(path)}`") if verbose else None; return path
+    def copy(self, folder=None, name=None, path=None, content=False, verbose=True, append=None, overwrite=False, orig=False) -> 'P':  # tested %100  # TODO: replace `content` flag with ability to interpret "*" in resolve method.
+        dest = self._resolve_path(folder=folder, name=name, path=path, default_name=self.name, rel2it=False)
+        dest, slf = dest.expanduser().resolve().create(parents_only=True), self.expanduser().resolve()
+        dest = self.append(append if append is not None else f"_copy_{randstr()}") if dest == slf else dest
+        dest.delete(sure=True) if not content and overwrite and dest.exists() else None
+        if not content and not overwrite and dest.exists(): raise FileExistsError(f"Destination already exists: {repr(dest)}")
+        if slf.is_file(): __import__("shutil").copy(str(slf), str(dest)); print(f"COPIED {repr(slf)} ==> {repr(dest)}") if verbose else None
+        elif slf.is_dir(): dest = dest.parent if content else dest; __import__("distutils.dir_util").__dict__["dir_util"].copy_tree(str(slf), str(dest)); print(f"COPIED {'Content of ' if False else ''} {repr(slf)} ==> {repr(dest)}") if verbose else None
+        else: print(f"Could NOT COPY. Not a file nor a path: {repr(slf)}.")
+        return dest if not orig else self
+    # ======================================= File Editing / Reading ===================================
+    def readit(self, reader=None, strict=True, notfound=None, verbose=False, **kwargs) -> 'P':
+        if not (slf := self.expanduser().resolve()).exists():
+            if strict: raise FileNotFoundError(f"`{slf}` is no where to be found!")
+            else: (print(f"tb.P.readit warning: FileNotFoundError, skipping reading of file `{self}") if verbose else None); return notfound
+        if verbose: print(f"Reading {slf.name} ({slf.size()} MB) ...")
+        filename = slf.unzip(folder=slf.tmp(folder="tmp_unzipped"), verbose=verbose) if '.zip' in str(slf) else slf
+        try: return Read.read(filename, **kwargs) if reader is None else reader(str(filename), **kwargs)
+        except IOError: raise IOError
+    def start(self, opener=None):
+        if str(self).startswith("http") or str(self).startswith("www"): __import__("webbrowser").open(str(self)); return self
+        if __import__("sys").platform == "win32":  # double quotes fail with cmd. # __import__("os").startfile(filename)  # works for files and folders alike, but if opener is given, e.g. opener="start"
+            __import__("subprocess").Popen(f"powershell start '{self.expanduser().resolve().str}'" if opener is None else rf'powershell {opener} \'{self}\''); return self  # fails for folders. Start must be passed, but is not defined.
+        elif __import__("sys").platform == 'linux': __import__("subprocess").call(["xdg-open", self.expanduser().resolve().str]); return self  # works for files and folders alike
+        else:  __import__("subprocess").call(["open", self.expanduser().resolve().str]); return self  # works for files and folders alike  # mac
+    def __call__(self, *args, **kwargs) -> 'P': self.start(*args, **kwargs); return self
+    def append_text(self, appendix) -> 'P': self.write_text(self.read_text() + appendix); return self
+    def cache_from(self, source_func, expire="1w", save=Save.pickle, reader=Read.read, **kwargs): return Cache(source_func=source_func, path=self, expire=expire, save=save, reader=reader, **kwargs)
+    def modify_text(self, txt_search, txt_alt, replace_line=False, notfound_append=False, prepend=False, encoding=None):
+        if not self.exists(): self.create(parents_only=True).write_text(txt_search)
+        return self.write_text(modify_text(txt_raw=self.read_text(encoding=encoding), txt_search=txt_search, txt_alt=txt_alt, replace_line=replace_line, notfound_append=notfound_append, prepend=prepend), encoding=encoding)
+    def download(self, directory=None, name=None, memory=False, allow_redirects=True, params=None) -> 'P':
+        response = __import__("requests").get(self.as_url_str(), allow_redirects=allow_redirects, params=params)  # Alternative: from urllib import request; request.urlopen(url).read().decode('utf-8').
+        return response if memory else (P.home().joinpath("Downloads") if directory is None else P(directory)).joinpath(validate_name(name or self.name)).create(parents_only=True).write_bytes(response.content)  # r.contents is bytes encoded as per docs of requests.
+    def _return(self, res, inlieu=False, inplace=False, operation=None, overwrite=False, orig=False, verbose=False, strict=True, msg="", __delayed_msg__="") -> 'P':
+        if inlieu: self._str = str(res)
+        if inplace:
+            assert self.exists(), f"`inplace` flag is only relevant if the path exists. It doesn't {self}"
+            if operation == "rename":
+                if overwrite and res.exists(): res.delete(sure=True, verbose=verbose)
+                if not overwrite and res.exists():
+                    if strict: raise FileExistsError(f"File {res} already exists.")
+                    else: print(f"SKIPPED RENAMING {repr(self)} ==> {repr(res)} because FileExistsError and scrict=False policy.") if verbose else None; return self if orig else res
+                self.rename(res); msg = msg or f"RENAMED {repr(self)} ==> {repr(res)}"
+            elif operation == "delete": self.delete(sure=True, verbose=False);  __delayed_msg__ = f"DELETED {repr(self)}."
+        print(msg) if verbose and msg != "" else None; print(__delayed_msg__) if verbose and __delayed_msg__ != "" else None; return self if orig else res
+    # ================================ Path Object management ===========================================
+    """ Distinction between Path object and the underlying file on disk that the path may refer to. Two distinct flags are used:
+        `inplace`: the operation on the path object will affect the underlying file on disk if this flag is raised, otherwise the method will only alter the string.
+        `inliue`: the method acts on the path object itself instead of creating a new one if this flag is raised.
+        `orig`: whether the method returns the original path object or a new one."""
+    def prepend(self, prefix, suffix=None, verbose=True, **kwargs): return self._return(self.parent.joinpath(prefix + self.trunk + (suffix or ''.join(('bruh'+self).suffixes))), operation="rename", verbose=verbose, **kwargs)  # Path('.ssh').suffix fails, 'bruh' fixes it.
+    def append(self, name='', index=False, suffix=None, verbose=True, **kwargs): return self.append(name=f'_{len(self.parent.search(f"*{self.stem}*"))}', index=False, verbose=verbose, suffix=suffix, **kwargs) if index else self._return(self.parent.joinpath(self.trunk + (name or "_" + timestamp()) + (suffix or ''.join(('bruh'+self).suffixes))), operation="rename", verbose=verbose, **kwargs)
+    def with_trunk(self, name, verbose=True, **kwargs): return self._return(self.parent.joinpath(name + "".join(self.suffixes)), operation="rename", verbose=verbose, **kwargs)  # Complementary to `with_stem` and `with_suffix`
+    def with_name(self, name, verbose=True, **kwargs): assert type(name) is str, "name must be a string."; return self._return(self.parent / name, verbose=verbose, operation="rename", **kwargs)
+    def switch(self, key: str, val: str, verbose=True, **kwargs): return self._return(P(str(self).replace(key, val)), operation="rename", verbose=verbose, **kwargs)  # Like string replce method, but `replace` is an already defined method."""
+    def switch_by_index(self, idx: int, val: str, verbose=True, **kwargs): return self._return(P(*[val if index == idx else value for index, value in enumerate(self.parts)]), operation="rename", verbose=verbose, **kwargs)
+    # ============================= attributes of object ======================================
+    trunk = property(lambda self: self.name.split('.')[0])  # """ useful if you have multiple dots in file path where `.stem` fails."""
+    len = property(lambda self: self.__len__()); items = property(lambda self: List(self.parts)); str = property(lambda self: str(self))  # or self._str
+    def __len__(self): return len(self.parts)
+    def __contains__(self, item): return P(item).as_posix() in self.as_posix()
+    def __iter__(self): return self.parts.__iter__()
+    def __deepcopy__(self) -> 'P': return P(str(self))
+    def __getstate__(self) -> str: return str(self)
+    def __setstate__(self, state): self._str = str(state)
+    def __add__(self, other) -> 'P': return self.parent.joinpath(self.name + str(other))  # used append and prepend if the addition wanted to be before suffix.
+    def __radd__(self, other) -> 'P': return self.parent.joinpath(str(other) + self.name)  # other + P and `other` doesn't know how to make this addition.
+    def __sub__(self, other) -> 'P': res = P(str(self).replace(str(other), "")); return (res[1:] if str(res[0]) in {"\\", "/"} else res) if len(res) else res  # paths starting with "/" are problematic. e.g ~ / "/path" doesn't work.
+    def rel2cwd(self, inlieu=False) -> 'P': return self._return(P(self.expanduser().absolute().relative_to(Path.cwd())), inlieu)
+    def rel2home(self, inlieu=False) -> 'P': return self._return(P(self.expanduser().absolute().relative_to(Path.home())), inlieu)  # very similat to collapseuser but without "~" being added so its consistent with rel2cwd.
+    def collapseuser(self, strict=True):
+        if strict: assert P.home() in self.expanduser().absolute().resolve(), ValueError(f"`{P.home()}` is not in the subpath of `{self}`")
+        return self if "~" in self else self._return(P("~") / (self.expanduser().absolute().resolve(strict=strict) - P.home()))    # opposite of `expanduser` resolve is crucial to fix Windows cases insensitivty problem.
+    def __getitem__(self, slici): return P(*[self[item] for item in slici]) if type(slici) is list else (P(*self.parts[slici]) if type(slici) is slice else P(self.parts[slici]))  # it is an integer
+    def __setitem__(self, key: str or int or slice, value: str or Path):
+        fullparts, new = list(self.parts), list(P(value).parts)
+        if type(key) is str: idx = fullparts.index(key); fullparts.remove(key); fullparts = fullparts[:idx] + new + fullparts[idx + 1:]
+        elif type(key) is int: fullparts = fullparts[:key] + new + fullparts[key + 1:]
+        elif type(key) is slice: fullparts = fullparts[:(0 if key.start is None else key.start)] + new + fullparts[(len(fullparts) if key.stop is None else key.stop):]
+        self._str = str(P(*fullparts))  # similar attributes: # self._parts # self._pparts # self._cparts # self._cached_cparts
+    def split(self, at: str = None, index: int = None, sep=[-1, 0, 1][-1], strict=True):
+        if index is None and (at is not None):  # at is provided  # ====================================   Splitting
+            if not strict:  # behaves like split method of string
+                one, two = (items := str(self).split(sep=str(at)))[0], items[1]; one, two = P(one[:-1]) if one.endswith("/") else P(one), P(two[1:]) if two.startswith("/") else P(two)
+            else:  # "strict": # raises an error if exact match is not found.
+                index = self.parts.index(str(at)); one, two = self[0:index], self[index + 1:]  # both one and two do not include the split item.
+        elif index is not None and (at is None):  # index is provided
+            one, two = self[:index], P(*self.parts[index + 1:]); at = self[index]  # this is needed below.
+        else: raise ValueError("Either `index` or `at` can be provided. Both are not allowed simulatanesouly.")
+        if sep == 0: return one, two  # neither of the portions get the sperator appended to it. # ================================  appending `at` to one of the portions
+        elif sep == 1: return one, at / two   # append it to right portion
+        elif sep == -1: return one / at, two  # append it to left portion.
+        else: raise ValueError(f"`sep` should take a value from the set [-1, 0, 1] but got {sep}")
+    def __repr__(self):  # this is useful only for the console
+        if self.is_symlink():
+            try: target = self.resolve()  # broken symolinks are funny, and almost always fail `resolve` method.
+            except Exception: target = "BROKEN LINK " + str(self)  # avoid infinite recursions for broken links.
+            return "P: Symlink '" + str(self) + "' ==> " + repr(str(target) if target == self else target)
+        elif self.is_absolute(): return "P: " + self._type() + " '" + self.clickable() + "'" + (" | " + self.time(which="c").isoformat()[:-7].replace("T", "  ") if self.exists() else "") + (f" | {self.size()} Mb" if self.is_file() else "")
+        elif "http" in str(self): return "P: URL " + self.as_url_str()
+        else: return "P: Relative " + "'" + str(self) + "'"  # not much can be said about a relative path.
+    # def __str__(self): return self.as_url_str() if "http" in self else self._str
+    def size(self, units='mb'):  # ===================================== File Specs ==========================================================================================
+        total_size = self.stat().st_size if self.is_file() else sum([item.stat().st_size for item in self.rglob("*") if item.is_file()])
+        return round(total_size / dict(zip(List(['b', 'kb', 'mb', 'gb']).eval("self+self.swapcase()"), 2 * [1024 ** item for item in range(4)]))[units], 1)
+    def time(self, which=["m", "c", "a"][0], **kwargs): return datetime.fromtimestamp({"m": self.stat().st_mtime, "a": self.stat().st_atime, "c": self.stat().st_ctime}[which], **kwargs)  # m last mofidication of content, i.e. the time it was created. c last status change (its inode is changed, permissions, path, but not content) a: last access
+    def stats(self): return Struct(size=self.size(), content_mod_time=self.time(which="m"), attr_mod_time=self.time(which="c"), last_access_time=self.time(which="a"), group_id_owner=self.stat().st_gid, user_id_owner=self.stat().st_uid)
+    # ================================ String Nature management ====================================
+    def _type(self): return ("File" if self.is_file() else ("Dir" if self.is_dir() else "NotExist")) if self.absolute() else "Relative"
+    def clickable(self, inlieu=False) -> 'P': return self._return(self.expanduser().resolve().as_uri(), inlieu)
+    def as_url_str(self, inlieu=False) -> 'P': return self._return(self.as_posix().replace("https:/", "https://").replace("http:/", "http://"), inlieu)
+    def as_url_obj(self, inlieu=False) -> 'P': return self._return(install_n_import("urllib3").connection_from_url(self), inlieu)
+    def as_unix(self, inlieu=False) -> 'P': return self._return(P(str(self).replace('\\', '/').replace('//', '/')), inlieu)
+    def as_zip_path(self): res = self.expanduser().resolve(); return __import__("zipfile").Path(res)  # .str.split(".zip") tmp=res[1]+(".zip" if len(res) > 2 else ""); root=res[0]+".zip", at=P(tmp).as_posix())  # TODO
+    def get_num(self, astring=None): int("".join(filter(str.isdigit, str(astring or self.stem))))
+    def validate_name(self, replace='_'): validate_name(self.trunk, replace=replace)
+    # ========================== override =======================================
+    def write_text(self, data: str, **kwargs) -> 'P': super(P, self).write_text(data, **kwargs); return self
+    def read_text(self, encoding=None, lines=False, printit=False) -> str: res = super(P, self).read_text(encoding=encoding) if not lines else List(super(P, self).read_text(encoding=encoding).splitlines()); print(res) if printit else None; return res
+    def write_bytes(self, data: bytes) -> 'P':
+        res = super(P, self).write_bytes(data)
+        if res == 0: raise RuntimeError(f"Could not save file on disk.")
+        return self
+    def touch(self, mode: int = 0o666, parents=True, exist_ok: bool = ...) -> 'P': self.parent.create(parents=parents) if parents else None; super(P, self).touch(mode=mode, exist_ok=exist_ok); return self
+    def symlink_from(self, src_folder=None, src_file=None, verbose=False, overwrite=False):
+        assert self.expanduser().exists(), "self must exist if this method is used."
+        if src_file is not None: assert src_folder is None, "You can only pass source or source_dir, not both."; result = P(src_file).expanduser().absolute()
+        else: result = P(src_folder or P.cwd()).expanduser().absolute() / self.name
+        return result.symlink_to(self, verbose=verbose, overwrite=overwrite)
+    def symlink_to(self, target=None, verbose=True, overwrite=False, orig=False):
+        self.parent.create(); assert (target := P(target).expanduser().resolve()).exists(), f"Target path `{target}` doesn't exist. This will create a broken link."
+        if overwrite and (self.is_symlink() or self.exists()): self.delete(sure=True, verbose=verbose)
+        if __import__("platform").system() == "Windows" and not (tm := __import__("crocodile").meta.Terminal).is_user_admin():  # you cannot create symlink without priviliages.
+            tm.run_as_admin(file=__import__("sys").executable, params=f" -c \"from pathlib import Path; Path(r'{self.expanduser()}').symlink_to(r'{str(target)}')\"", wait=2)
+        else: super(P, self.expanduser()).symlink_to(str(target))
+        return self._return(P(target), inlieu=False, inplace=False, orig=orig, verbose=verbose, msg=f"LINKED {repr(self)}")
+    def resolve(self, strict=False):
+        try: return super(P, self).resolve(strict=strict)
+        except OSError: return self
+    # ======================================== Folder management =======================================
+    def search(self, pattern='*', r=False, files=True, folders=True, compressed=False, dotfiles=False, filters: list = None, not_in: list = None, exts=None, win_order=False) -> List:
+        filters = (filters or []) + ([lambda x: all([str(notin) not in str(x) for notin in not_in])] if not_in is not None else []) + ([lambda x: any([ext in x.name for ext in exts])] if exts is not None else [])
+        if ".zip" in (slf := self.expanduser().resolve()) and compressed:  # the root (self) is itself a zip archive (as opposed to some search results are zip archives)
+            root = slf.as_zip_path(); raw = List(root.iterdir()) if not r else List(__import__("zipfile").ZipFile(str(slf)).namelist()).apply(lambda x: root.joinpath(x))
+            return raw.filter(lambda zip_path: __import__("fnmatch").fnmatch(zip_path.at, pattern)).filter(lambda x: (folders or x.is_file()) and (files or x.is_dir()))  # .apply(lambda x: P(str(x)))
+        elif dotfiles: raw = slf.glob(pattern) if not r else self.rglob(pattern)
+        else: raw = __import__("glob").glob(str(slf / "**" / pattern), recursive=r) if r else __import__("glob").glob(str(slf.joinpath(pattern)))  # glob ignroes dot and hidden files
+        if ".zip" not in slf and compressed: raw += List([P(comp_file).search(pattern=pattern, r=r, files=files, folders=folders, compressed=True, dotfiles=dotfiles, filters=filters, not_in=not_in, win_order=win_order) for comp_file in self.search("*.zip", r=r)]).reduce().list
+        processed = List([P(item) for item in raw if (lambda item_: all([item_.is_dir() if not files else True, item_.is_file() if not folders else True] + [afilter(item_) for afilter in filters]))(P(item))])
+        return processed if not win_order else processed.sort(key=lambda x: [int(k) if k.isdigit() else k for k in __import__("re").split('([0-9]+)', x.stem)])
+    def tree(self, *args, **kwargs): return __import__("crocodile.msc.odds").msc.odds.__dict__['tree'](self, *args, **kwargs)
+    # def find(self, *args, r=True, compressed=True, **kwargs) -> 'P':  # short for the method ``search`` then pick first item from results. useful for superflous directories or zip archives containing a single file."""
+    #     if compressed is False and self.is_file(): return self
+    #     if len(results := self.search(*args, r=r, compressed=compressed, **kwargs)) > 0: return results[0].unzip() if ".zip" in str(results[0]) else results[0]
+    browse = property(lambda self: self.search("*").to_struct(key_val=lambda x: ("qq_" + validate_name(x), x)).clean_view)
+    def create(self, parents=True, exist_ok=True, parents_only=False) -> 'P': self.parent.mkdir(parents=parents, exist_ok=exist_ok) if parents_only else self.mkdir(parents=parents, exist_ok=exist_ok); return self
+    def chdir(self) -> 'P': __import__("os").chdir(str(self.expanduser())); return self
+    def listdir(self) -> List: return List(__import__("os").listdir(self.expanduser().resolve())).apply(P)
+    tempdir = staticmethod(lambda: P(__import__("tempfile").mktemp()))
+    temp = staticmethod(lambda: P(__import__("tempfile").gettempdir()))
+    tmpdir = staticmethod(lambda prefix="": P.tmp(folder=rf"tmp_dirs/{prefix + ('_' if prefix != '' else '') + randstr()}"))
+    tmpfile = staticmethod(lambda name=None, suffix="", folder=None, tstamp=False: P.tmp(file=(name or randstr()) + "_" + randstr() + (("_" + timestamp()) if tstamp else "") + suffix, folder=folder or "tmp_files"))
+    tmp = staticmethod(lambda folder=None, file=None, root="~/tmp_results": P(root).expanduser().create().joinpath(folder or "").joinpath(file or "").create(parents_only=True if file else False))
+    # ====================================== Compression & Encryption ===========================================
+    def zip(self, path=None, folder=None, name=None, arcname=None, inplace=False, verbose=True, content=False, orig=False, use_7z=False, pwd=None, **kwargs) -> 'P':
+        path, slf = self._resolve_path(folder, name, path, self.name).expanduser().resolve(), self.expanduser().resolve()
+        if use_7z: path = seven_zip(path=slf, op_path=path, pwd=pwd)
+        else:
+            if (arcname := P(arcname or slf.name)).name != slf.name: arcname /= slf.name  # arcname has to start from somewhere and end with filename
+            if slf.is_file(): path = Compression.zip_file(ip_path=slf, op_path=path + f".zip" if path.suffix != ".zip" else path, arcname=arcname, **kwargs)
+            else:
+                root_dir, base_dir = (slf, ".") if content else (slf.split(at=str(arcname[0]))[0], arcname)
+                path = Compression.compress_folder(root_dir=root_dir, op_path=path, base_dir=base_dir, fmt='zip', **kwargs)
+        return self._return(path, inlieu=False, inplace=inplace, operation="delete", orig=orig, verbose=verbose, msg=f"ZIPPED {repr(slf)} ==>  {repr(path)}")
+    def unzip(self, folder=None, fname=None, verbose=True, content=False, inplace=False, overwrite=False, merge=True, orig=False, pwd=None, **kwargs) -> 'P':
+        slf = zipfile = self.expanduser().resolve()
+        if any(ztype in slf.parent for ztype in (".zip", ".7z")):  # path include a zip archive in the middle.
+            if (ztype := [item for item in (".zip", ".7z", "") if item in str(slf)][0]) == "": return slf
+            zipfile, fname = slf.split(at=List(slf.parts).filter(lambda x: ztype in x)[0], sep=-1)
+        folder = (zipfile.parent / zipfile.stem) if folder is None else P(folder).expanduser().absolute().resolve().joinpath(zipfile.stem)
+        folder = folder if not content else folder.parent
+        if slf.suffix == ".7z": P(folder).delete(sure=True) if overwrite else None; result = un_seven_zip(path=slf, op_dir=folder, pwd=pwd)
+        else:
+            if overwrite:
+                if not content: P(folder).joinpath(fname or "").delete(sure=True, verbose=True)  # deletes a specific file / folder that has the same name as the zip file without extension.
+                else: List([x for x in __import__("zipfile").ZipFile(self.str).namelist() if "/" not in x or (len(x.split('/')) == 2 and x.endswith("/"))]).apply(lambda item: P(folder).joinpath(fname or "", item.replace("/", "")).delete(sure=True, verbose=True))
+            result = Compression.unzip(zipfile, folder, None if fname is None else P(fname).as_posix(), **kwargs)
+        return self._return(result, inlieu=False, inplace=inplace, operation="delete", orig=orig, verbose=verbose, msg=f"UNZIPPED {repr(zipfile)} ==> {repr(result)}")
+    def tar(self, path=None, name=None, folder=None, inplace=False, orig=False, verbose=True) -> 'P': Compression.tar(self.expanduser().resolve(), op_path := self._resolve_path(folder, name, path, self.name + ".tar").expanduser().resolve()); return self._return(op_path, inlieu=False, inplace=inplace, operation="delete", orig=orig, verbose=verbose, msg=f"TARRED {repr(self)} ==>  {repr(op_path)}")
+    def untar(self, folder=None, path=None, name=None, inplace=False, orig=False, verbose=True) -> 'P': Compression.untar(self.expanduser().resolve(), op_path := self._resolve_path(folder, name, path, self.name.replace(".tar", "")).expanduser().resolve()); return self._return(op_path, inlieu=False, inplace=inplace, operation="delete", orig=orig, verbose=verbose, msg=f"UNTARRED {repr(self)} ==>  {repr(op_path)}")
+    def gz(self, path=None, folder=None, name=None, inplace=False, orig=False, verbose=True) -> 'P': Compression.gz(self.expanduser().resolve(), op_path := self._resolve_path(folder, name, path, self.name + ".gz").expanduser().resolve()); return self._return(op_path, inlieu=False, inplace=inplace, operation="delete", orig=orig, verbose=verbose, msg=f"GZED {repr(self)} ==>  {repr(op_path)}")
+    def ungz(self, folder=None, name=None, path=None, inplace=False, orig=False, verbose=True) -> 'P': Compression.ungz(self.expanduser().resolve(), op_path := self._resolve_path(folder, name, path, self.name.replace(".gz", "")).expanduser().resolve()); return self._return(op_path, inlieu=False, inplace=inplace, operation="delete", orig=orig, verbose=verbose, msg=f"UNGZED {repr(self)} ==>  {repr(op_path)}")
+    def xz(self, path=None, name=None, folder=None, inplace=False, orig=False, verbose=True) -> 'P': Compression.xz(self.expanduser().resolve(), op_path := self._resolve_path(folder, name, path, self.name + ".xz").expanduser().resolve()); return self._return(op_path, inlieu=False, inplace=inplace, operation="delete", orig=orig, verbose=verbose, msg=f"XZED {repr(self)} ==>  {repr(op_path)}")
+    def unxz(self, folder=None, name=None, path=None, inplace=False, orig=False, verbose=True) -> 'P': Compression.unxz(self.expanduser().resolve(), op_path := self._resolve_path(folder, name, path, self.name.replace(".xz", "")).expanduser().resolve()); return self._return(op_path, inlieu=False, inplace=inplace, operation="delete", orig=orig, verbose=verbose, msg=f"UNXZED {repr(self)} ==>  {repr(op_path)}")
+    def tar_gz(self, folder=None, name=None, path=None, inplace=False, orig=False, verbose=True) -> 'P': return self.tar(inplace=inplace).gz(folder=folder, name=name, path=path, inplace=True, orig=orig, verbose=verbose)
+    def ungz_untar(self, folder=None, name=None, path=None, inplace=False, verbose=True, orig=False) -> 'P': return self.ungz(inplace=inplace).untar(folder=folder, name=name, path=path, inplace=True, orig=orig, verbose=verbose)
+    def tar_xz(self, folder=None, name=None, path=None, inplace=False, verbose=True, orig=False) -> 'P': return self.tar(inplace=inplace).xz(folder=folder, name=name, path=path, inplace=True, orig=orig, verbose=verbose)
+    def unxz_untar(self, folder=None, name=None, path=None, inplace=False,  verbose=True, orig=False) -> 'P': return self.unxz(inplace=inplace).untar(folder=folder, name=name, path=path, inplace=True, orig=orig, verbose=verbose)
+    def decompress(self, folder=None, name=None, path=None, inplace=False,  verbose=True, orig=False) -> 'P': raise NotImplementedError("Not implemented yet.")
+    def encrypt(self, key=None, pwd=None, folder=None, name=None, path=None, verbose=True, suffix=".enc", inplace=False, orig=False) -> 'P':  # see: https://stackoverflow.com/questions/42568262/how-to-encrypt-text-with-a-password-in-python & https://stackoverflow.com/questions/2490334/simple-way-to-encode-a-string-according-to-a-password"""
+        slf = self.expanduser().resolve(); path = self._resolve_path(folder, name, path, slf.name+suffix)
+        assert slf.is_file(), f"Cannot encrypt a directory. You might want to try `zip_n_encrypt`. {self}"; path.write_bytes(encrypt(msg=slf.read_bytes(), key=key, pwd=pwd))
+        return self._return(path, inlieu=False, inplace=inplace, operation="delete", orig=orig, verbose=verbose, msg=f"ENCRYPTED: {repr(slf)} ==> {repr(path)}.")
+    def decrypt(self, key=None, pwd=None, path=None, folder=None, name=None, verbose=True, suffix=".enc", **kwargs) -> 'P':
+        slf = self.expanduser().resolve(); path = self._resolve_path(folder, name, path, slf.name.replace(suffix, "") if suffix in slf.name else "decrypted_" + slf.name).write_bytes(decrypt(slf.read_bytes(), key=key, pwd=pwd))
+        return self._return(path, operation="delete", verbose=verbose, msg=f"DECRYPTED: {repr(slf)} ==> {repr(path)}.", **kwargs)
+    def zip_n_encrypt(self, key=None, pwd=None, inplace=False, verbose=True, orig=False, content=False) -> 'P': return self.zip(inplace=inplace, verbose=verbose, content=content).encrypt(key=key, pwd=pwd, verbose=verbose, inplace=True) if not orig else self
+    def decrypt_n_unzip(self, key=None, pwd=None, inplace=False, verbose=True, orig=False) -> 'P': return self.decrypt(key=key, pwd=pwd, verbose=verbose, inplace=inplace).unzip(folder=None, inplace=True, content=False) if not orig else self
+    def _resolve_path(self, folder, name, path, default_name, rel2it=False) -> 'P':  # From all arguments, figure out what is the final path.
+        """:param rel2it: `folder` or `path` are relative to `self` as opposed to cwd. This is used when resolving '../dir'"""
+        if path is not None:
+            path = P(self.joinpath(path).resolve() if rel2it else path).expanduser().resolve()
+            assert folder is None and name is None, f"If `path` is passed, `folder` and `name` cannot be passed."; assert not path.is_dir(), f"`path` passed is a directory! it must not be that. If this is meant, pass it with `folder` kwarg. `{path}`"
+            return path
+        name, folder = (default_name if name is None else str(name)), (self.parent if folder is None else folder)  # good for edge cases of path with single part.  # means same directory, just different name
+        return P(self.joinpath(folder).resolve() if rel2it else folder).expanduser().resolve() / name
+    def checksum(self, kind=["md5", "sha256"][1]): import hashlib; myhash = {"md5": hashlib.md5, "sha256": hashlib.sha256}[kind](); myhash.update(self.read_bytes()); return myhash.hexdigest()
+    get_env = staticmethod(lambda: get_env())
+    def transfer_sh(self) -> 'P': return P(__import__("requests").put(f"https://transfer.sh/{self.expanduser().name}", self.expanduser().absolute().read_bytes()).text)
+
+
+def compress_folder(root_dir, op_path, base_dir, fmt='zip', **kwargs):  # shutil works with folders nicely (recursion is done interally) # directory to be archived: root_dir\base_dir, unless base_dir is passed as absolute path. # when archive opened; base_dir will be found."""
+    assert fmt in {"zip", "tar", "gztar", "bztar", "xztar"}  # .zip is added automatically by library, hence we'd like to avoid repeating it if user sent it.
+    return P(__import__('shutil').make_archive(base_name=str(op_path)[:-4] if str(op_path).endswith(".zip") else str(op_path), format=fmt, root_dir=str(root_dir), base_dir=str(base_dir), **kwargs))  # returned path possible have added extension.
+def zip_file(ip_path, op_path, arcname=None, password=None, mode="w", **kwargs):
+    """arcname determines the directory of the file being archived inside the archive. Defaults to same as original directory except for drive.
+    When changed, it should still include the file path in its end. If arcname = filename without any path, then, it will be in the root of the archive."""
+    import zipfile
+    with zipfile.ZipFile(str(op_path), mode=mode) as jungle_zip:
+        jungle_zip.setpassword(pwd=password) if password is not None else None
+        jungle_zip.write(filename=str(ip_path), arcname=str(arcname) if arcname is not None else None, compress_type=zipfile.ZIP_DEFLATED, **kwargs)
+    return P(op_path)
+def unzip(ip_path, op_path=None, fname=None, password=None, memory=False, **kwargs):
+    with __import__("zipfile").ZipFile(str(ip_path), 'r') as zipObj:
+        if memory: return Struct({name: zipObj.read(name) for name in zipObj.namelist()}) if fname is None else zipObj.read(fname)
+        if fname is None: zipObj.extractall(op_path, pwd=password, **kwargs); return P(op_path)
+        else: zipObj.extract(member=str(fname), path=str(op_path), pwd=password); return P(op_path) / fname
+def seven_zip(path: P, op_path: P, pwd=None, mode='w'):  # benefits over regular zip and encrypt: can handle very large files with low memory footprint
+    op_path = op_path + '.7z' if not op_path.suffix == '.7z' else op_path
+    if (env := get_env()).system == "Windows":
+        env.tm.run('winget install --name "7-zip" --Id "7zip.7zip" --source winget', shell="powershell") if not (program := env.ProgramFiles.joinpath("7-Zip/7z.exe")).exists() else None
+        res = env.tm.run(f"&'{program}' a '{op_path}' '{path}' {f'-p{pwd}' if pwd is not None else ''}", shell="powershell"); assert res.is_successful, res.print(); return op_path
+    elif env.system == "Linux":  # python variant is much slower than 7-zip, and consumes more memroy, see py7zr project on github.
+        op_path = op_path + '.7z' if not op_path.suffix == '.7z' else op_path; py7zr = install_n_import("py7zr")
+        with py7zr.SevenZipFile(op_path, mode, password=pwd) as archive: archive.writeall(path)
+        return op_path
+def un_seven_zip(path, op_dir, overwrite=False, pwd=None):  # TODO: use py7zr instead of two implementations for linux and windows.
+    if (env := get_env()).system == "Windows":
+        env.tm.run('winget install --name "7-zip" --Id "7zip.7zip" --source winget', shell="powershell") if not (program := env.ProgramFiles.joinpath("7-Zip/7z.exe")).exists() else None
+        res = env.tm.run(f"&'{program}' x",  f"'{path}'",  f"-o'{op_dir}'", f"-p{pwd}" if pwd is not None else '', shell="powershell"); assert res.is_successful, res.print(); return op_dir
+    else: raise NotImplementedError("7z not implemented for Linux")
+def gz(file, op_path):  # see this on what to use: https://stackoverflow.com/questions/10540935/what-is-the-difference-between-tar-and-zip
+    with open(file, 'rb') as f_in:
+        with __import__("gzip").open(op_path, 'wb') as f_out:  __import__("shutil").copyfileobj(f_in, f_out)
+    return P(op_path)
+def ungz(self, op_path=None):
+    with __import__("gzip").open(str(self), 'r') as f_in, open(op_path, 'wb') as f_out: __import__("shutil").copyfileobj(f_in, f_out)
+    return P(op_path)
+def xz(self, op_path):
+    with __import__("lzma").open(op_path, "w") as f: f.write(self)
+def unxz(ip_path, op_path):
+    with __import__("lzma").open(ip_path) as file: P(op_path).write_bytes(file.read())
+def tar(self, op_path):
+    with __import__("tarfile").open(op_path, "w:gz") as tar_: tar_.add(str(self), arcname=__import__("os").path.basename(str(self)))
+    return P(op_path)
+def untar(self, op_path, fname=None, mode='r', **kwargs):
+    with __import__("tarfile").open(str(self), mode) as file:
+        if fname is None: file.extractall(path=op_path, **kwargs)  # extract all files in the archive
+        else: file.extract(fname, **kwargs)
+    return P(op_path)
+class Compression: compress_folder = compress_folder; zip_file = zip_file; unzip = unzip; gz = gz; ungz = ungz; tar = tar; untar = untar; xz = xz; unxz = unxz  # Provides consistent behaviour across all methods
+
+
+class Cache:  # This class helps to accelrate access to latest data coming from expensive function. The class has two flavours, memory-based and disk-based variants."""
+    def __init__(self, source_func, expire="1m", logger=None, path=None, save=Save.pickle, reader=Read.read):
+        self.cache = None  # fridge content
+        self.source_func = source_func  # function which when called returns a fresh object to be frozen.
+        self.path = P(path) if path else None  # if path is passed, it will function as disk-based flavour.
+        self.time_produced, self.save, self.reader, self.logger, self.expire = None, save, reader, logger, expire
+    age = property(lambda self: datetime.now() - self.time_produced if self.path is None else datetime.now() - self.path.stats().content_mod_time)
+    def __setstate__(self, state): self.__dict__.update(state); self.path = P.home() / self.path if self.path is not None else self.path
+    def __getstate__(self): state = self.__dict__.copy(); state["path"] = self.path.rel2home() if self.path is not None else state["path"]; return state  # With this implementation, instances can be pickled and loaded up in different machine and still works.
+    def __call__(self, fresh=False):
+        if self.path is None:  # Memory Cache
+            if self.cache is None or fresh is True or self.age > str2timedelta(self.expire): self.cache, self.time_produced = self.source_func(), datetime.now(); self.logger.debug(f"Updating / Saving data from {self.source_func}") if self.logger else None
+            elif self.logger: self.logger.debug(f"Using cached values. Lag = {self.age}.")
+        elif fresh or not self.path.exists() or self.age > str2timedelta(self.expire):  # disk fridge
+            if self.logger: self.logger.debug(f"Updating & Saving {self.path} ...")
+            self.cache = self.source_func(); self.save(obj=self.cache, path=self.path)  # fresh order, never existed or exists but expired.
+        elif self.age < str2timedelta(self.expire) and self.cache is None: self.cache = self.reader(self.path)  # this implementation favours reading over pulling fresh at instantiation.  # exists and not expired. else # use the one in memory self.cache
+        return self.cache
+
+
+if __name__ == '__main__':
+    # print('hi from file_managements')
+    pass
```

### Comparing `crocodile-8.40/myresources/crocodile/matplotlib_management.py` & `crocodile-9.0/myresources/crocodile/matplotlib_management.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,445 +1,445 @@
-
-
-from crocodile.core import List, timestamp, Save, install_n_import, validate_name
-from crocodile.file_management import P
-from crocodile.meta import Terminal
-
-import matplotlib.pyplot as plt
-from crocodile.msc.odds import Cycle
-from matplotlib import widgets
-import matplotlib.colors as mcolors
-from matplotlib import animation
-import enum
-import subprocess
-import platform
-import pandas as pd
-import numpy as np
-
-
-"""TODO: add implementation https://github.com/gustavovelascoh/plot_update
-"""
-
-
-class FigurePolicy(enum.Enum):
-    close_create_new = 'Close the previous figure that has the same figname and create a new fresh one'
-    add_new = 'Create a new figure with same path but with added suffix'
-    same = 'Grab the figure of the same path'
-
-
-def assert_requirements():
-    try: subprocess.check_output(['where.exe' if platform.system() == 'Windows' else 'which', 'magick'])
-    except (FileNotFoundError, subprocess.CalledProcessError):
-        # P(r"https://www.gyan.dev/ffmpeg/builds/ffmpeg-git-full.7z").download().unzip().search()[0].rename("ffmpeg").move(r"C://")  # P("C:\\ffmpeg\\bin")  # add to PATH
-        print("Installinng image magick")
-        if __import__("platform").system() == "Windows":
-            Terminal().run("winget install ImageMagick.ImageMagick", shell="powershell")  # gives ffmpeg as well
-            print("You might need to restart your machine before PATH change impact takes place.")
-        else: raise NotImplementedError
-
-
-class FigureSave:
-    class GenericSave:
-        stream = ['clear', 'accumulate', 'update'][0]
-        def __init__(self, save_dir=None, save_name=None, watch_figs: list or None = None, max_calls=2000, delay=100, **kwargs):
-            """How to control what to be saved: you can either pass the figures to be tracked at init time, pass them dynamically at add time, or, add method will capture every figure and axis"""
-            self.watch_figs = watch_figs if watch_figs is None else ([plt.figure(num=afig) for afig in watch_figs] if type(watch_figs[0]) is str else watch_figs)
-            self.save_name, self.save_dir = timestamp(name=save_name), save_dir or P.tmpdir(prefix="tmp_fig_save")
-            self.kwargs, self.counter, self.delay, self.max = kwargs, 0, delay, max_calls
-        def add(self, fignames=None, names=None, **kwargs):  # generic method used at runtime, never changed.
-            print(f"Saver added frame number {self.counter}", end='\r')
-            self.counter += 1; plt.pause(self.delay * 0.001); print('Turning off IO') if self.counter > self.max else None; plt.ioff()
-            self.watch_figs = [plt.figure(figname) for figname in fignames] if fignames else ([plt.figure(k) for k in plt.get_figlabels()] if self.watch_figs is None else self.watch_figs)  # path sent explicitly, # None exist ==> add all else # they exist already.
-            if names is None: names = [timestamp(name=a_figure.get_label()) for a_figure in self.watch_figs]  # individual save path, useful for PNG.
-            for afig, aname in zip(self.watch_figs, names): self._save(afig, aname, **kwargs)
-        def _save(self, *args, **kwargs): pass  # called by generic method `add`, to be implemented when subclassing.
-    class Null(GenericSave):  # serves as a filler.
-        def __init__(self, *args, **kwargs): super().__init__(*args, **kwargs); self.fname = self.save_dir
-        def finish(self): print(f"Nothing saved by {self}"); return self.fname
-    class PDF(GenericSave):  # For pdf, you just need any stream [update, clear, accumalate], preferabbly the fastest."""
-        def __init__(self, *args, **kwargs):
-            super().__init__(*args, **kwargs)
-            from matplotlib.backends.backend_pdf import PdfPages
-            self.fname = self.save_dir.joinpath(self.save_name + ('.pdf' if '.pdf' not in str(self.save_name) else '')); self.pp = PdfPages(self.fname)
-        def _save(self, a_fig, a_name, bbox_inches='tight', pad_inches=0.3, **kwargs): self.pp.savefig(a_fig, bbox_inches=bbox_inches, pad_inches=pad_inches, **kwargs)
-        def finish(self): print(f"Saving results ..."); self.pp.close(); print(f"SAVED PDF @", P(self.fname).absolute().as_uri()); return self
-    class PNG(GenericSave):
-        def __init__(self, *args, **kwargs): super().__init__(*args, **kwargs); self.fname = self.save_dir = self.save_dir.joinpath(self.save_name)
-        def _save(self, afigure, aname, dpi=150, **kwargs):  afigure.savefig(self.save_dir.joinpath(validate_name(aname)).create(parents_only=True), bbox_inches='tight', pad_inches=0.3, dpi=dpi, **kwargs)
-        def finish(self): print(f"SAVED PNGs @", P(self.fname).absolute().as_uri()); return self
-    class GIF(GenericSave):  # NOT RECOMMENDED, used GIFFileBased instead.
-        """This class uses ArtistAnimation: works on lines and images list attached to figure axes and Doesn't work on axes, unless you add large number of them. As such, titles are not incorporated etc (limitation).
-        Requirements: same axis must persist (If you clear the axis, nothing will be saved), only new objects are drawn inside it. Additionally, the objects drawn must not be removed, or updated, instead they should pile up in axis.
-        # usually it is smoother when adding animate=True to plot or imshow commands for GIF purpose
-        Works for images only. Add more .imshow to the same axis, and that's it. imshow will conver up previous images. For lines, it will superimpose it and will look ugly.
-        The class will automatically detect new lines by their "neo" labels and add them then hide them for the next round.
-        """
-        def __init__(self, interval=100, **kwargs):
-            super().__init__(**kwargs); from collections import defaultdict
-            self.container, self.interval, self.fname = defaultdict(lambda: []), interval, None  # determined at finish time.
-        def _save(self, afigure, aname, cla=False, **kwargs):
-            fig_list, subcontainer = self.container[afigure.get_label()], []
-            for item in FigureManager.findobj(afigure, 'neo'): item.set_label('processed'); item.set_visible(False); subcontainer += [item]
-            fig_list.append(subcontainer)  # if you want the method coupled with cla being used in main, then it add_line is required for axes.
-        def finish(self):
-            print("Saving the GIF ....")
-            for idx, a_fig in enumerate(self.watch_figs):
-                if ims := self.container[a_fig.get_label()]:
-                    self.fname = self.save_dir.joinpath(f'{a_fig.get_label()}_{self.save_name}.gif')
-                    ani = animation.ArtistAnimation(a_fig, ims, interval=self.interval, blit=True, repeat_delay=1000)
-                    # noinspection PyTypeChecker
-                    ani.save(self.fname, writer=animation.PillowWriter(fps=4))  # if you don't specify the writer, it goes to ffmpeg by default then try others if that is not available, resulting in behaviours that is not consistent across machines.
-                    print(f"SAVED GIF @", P(self.fname).absolute().as_uri())
-                else: print(f"Nothing to be saved by GIF writer."); return self.fname
-    class GIFFileBased(GenericSave):
-        def __init__(self, fps=4, dpi=100, bitrate=1800, _type='GIFFileBased', **kwargs):
-            super().__init__(**kwargs); assert_requirements()
-            if _type == 'GIFPipeBased': writer, extension = animation.ImageMagickFileWriter, '.gif'  # internally calls: matplotlib._get_executable_info("magick")
-            elif _type == "GIFFileBased": writer, extension = animation.ImageMagickWriter, '.gif'
-            elif _type == 'MPEGFileBased': writer, extension = animation.FFMpegFileWriter, '.mp4'
-            elif _type == 'MPEGPipeBased': writer, extension = animation.FFMpegWriter, '.mp4'
-            else: raise ValueError("Unknown writer.")
-            self.writer = writer(fps=fps, metadata=dict(artist='Alex Al-Saffar'), bitrate=bitrate)
-            self.fname = self.save_dir.joinpath(self.save_name + extension)
-            assert self.watch_figs, "No figure was sent during instantiation of saver, therefore the writer cannot be setup. Did you mean to use an autosaver?"
-            self.writer.setup(fig=self.watch_figs[0], outfile=str(self.fname), dpi=dpi)
-        def _save(self, afig, aname, **kwargs): self.writer.grab_frame(**kwargs)
-        def finish(self): print('Saving results ...'); self.writer.finish(); print(f"SAVED GIF @", P(self.fname).absolute().as_uri()); return self
-    class GIFPipeBased(GIFFileBased):
-        def __init__(self, *args, **kwargs): super().__init__(*args, _type=self.__class__.__name__, **kwargs)
-    class MPEGFileBased(GIFFileBased):
-        def __init__(self, *args, **kwargs): super().__init__(*args, _type=self.__class__.__name__, **kwargs)
-    class MPEGPipeBased(GIFFileBased):
-        def __init__(self, *args, **kwargs): super().__init__(*args, _type=self.__class__.__name__, **kwargs)
-    class GenericAuto(GenericSave):
-        """Parses the data internally, hence requires artist with animate method implemetend. Artist needs to have .fig attribute."""
-        save_type = 'auto'
-        def __init__(self, plotter_class, data, names_list=None, **kwargs):
-            super().__init__(**kwargs); self.saver, self.plotter = None, None; assert_requirements()
-            self.plotter_class, self.data, self.names_list, self.kwargs = plotter_class, data, names_list, kwargs
-        def animate(self):
-            self.plotter = self.plotter_class(**self.kwargs); plt.pause(0.5)  # give time for figures to show up before updating them
-            for idx, datum in __import__("tqdm").tqdm(enumerate(self.data)): self.plotter.animate(datum); self.saver.add(names=[self.names_list[idx] if self.names_list is not None else str(idx)])
-            self.saver.finish()
-    class GIFAuto(GenericAuto):
-        def __init__(self, plotter_class, data, interval=500, extension='gif', fps=4, metadata=None, **kwargs):
-            super().__init__(plotter_class, data, **kwargs)
-            writer = animation.PillowWriter(fps=fps) if extension == '.mp4' else animation.FFMpegWriter(fps=fps, metadata=metadata, bitrate=2500)
-            self.plotter = self.plotter_class(**kwargs); plt.pause(self.delay * 0.001)  # give time for figures to show up before updating them
-            # noinspection PyTypeChecker
-            self.ani = animation.FuncAnimation(fig=self.plotter.fig, func=self.plotter.animate, frames=(i for i in zip(*self.data)), interval=interval, repeat_delay=1500, fargs=None, cache_frame_data=True, save_count=10000)
-            self.fname = self.save_dir.joinpath(self.save_name + f".{extension}")
-            self.ani.save(filename=self.fname, writer=writer); print(f"SAVED GIF @ ", P(self.fname).absolute().as_uri())
-    class PDFAuto(GenericAuto):
-        def __init__(self, **kwargs): super().__init__(**kwargs); self.saver = FigureSave.PDF(**kwargs); self.animate()
-    class PNGAuto(GenericAuto):
-        def __init__(self, **kwargs): super().__init__(**kwargs); self.saver = FigureSave.PNG(**kwargs); self.save_dir = self.saver.save_dir; self.animate(); self.fname = self.saver.fname
-    class NullAuto(GenericAuto):
-        def __init__(self, **kwargs): super().__init__(**kwargs); self.saver = FigureSave.Null(**kwargs); self.fname = self.saver.fname; self.animate()
-    class GIFFileBasedAuto(GenericAuto):
-        def __init__(self, plotter_class, data, fps=4, dpi=150, bitrate=2500, _type='GIFFileBasedAuto', **kwargs):
-            super().__init__(**kwargs)
-            if _type == 'GIFPipeBasedAuto': writer = animation.ImageMagickFileWriter; extension = '.gif'
-            elif _type == 'MPEGFileBasedAuto': writer = animation.FFMpegFileWriter; extension = '.mp4'
-            elif _type == 'MPEGPipeBasedAuto': writer = animation.FFMpegWriter; extension = '.mp4'
-            else: raise ValueError("Unknown writer.")
-            self.saver = writer(fps=fps, metadata=dict(artist='Alex Al-Saffar'), bitrate=bitrate)
-            self.fname = self.save_dir.joinpath(self.save_name + extension)
-            self.data = lambda: (i for i in zip(*data)); self.plotter = plotter_class(*[piece[0] for piece in data], **kwargs); plt.pause(0.5); from tqdm import tqdm
-            with self.saver.saving(fig=self.plotter.fig, outfile=self.fname, dpi=dpi):
-                for datum in tqdm(self.data()): self.plotter.animate(datum); self.saver.grab_frame(); plt.pause(self.delay * 0.001)
-            print(f"SAVED GIF successfully @ {self.fname}")
-    class GIFPipeBasedAuto(GIFFileBasedAuto):
-        def __init__(self, *args, **kwargs): super().__init__(*args, _type=self.__class__.__name__, **kwargs)
-    class MPEGFileBasedAuto(GIFFileBasedAuto):
-        def __init__(self, *args, **kwargs): super().__init__(*args, _type=self.__class__.__name__, **kwargs)
-    class MPEGPipeBasedAuto(GIFFileBasedAuto):
-        def __init__(self, *args, **kwargs): super().__init__(*args, _type=self.__class__.__name__, **kwargs)
-
-
-class FigureManager:  # use as base class for Artist & Viewers to give it free animation powers.
-    def __init__(self, info_loc=None, figpolicy=FigurePolicy.same):
-        self.figpolicy = figpolicy
-        self.fig = self.ax = self.event = None
-        self.cmaps, self.colors, self.mcolors, self.facecolor = Cycle(plt.colormaps()), Cycle(plt.rcParams['axes.prop_cycle'].by_key()['color']), list(mcolors.CSS4_COLORS.keys()), Cycle(list(mcolors.CSS4_COLORS.values()))
-        self.cmaps.set_value('viridis')
-        self.idx_cycle = Cycle([]); self.pause = None  # animation
-        self.help_menu = {'_-=+[{]}\\': {'help': "Adjust Vmin Vmax. Shift + key applies change to all axes \\ toggles auto-brightness ", 'func': self.adjust_brightness},
-                          "/": {'help': 'Show/Hide info text', 'func': self.text_info},
-                          "h": {'help': 'Show/Hide help menu', 'func': self.show_help},
-                          "tyTY": {'help': 'Change color map', 'func': self.change_cmap},
-                          '<>': {'help': 'Change figure face color', 'func': self.change_facecolor},
-                          "v": {'help': 'Show/Hide pixel values (Toggle)', 'func': self.show_pix_val},
-                          'P': {'help': 'Pause/Proceed (Toggle)', 'func': self.pause_func},
-                          'r': {'help': 'Replay', 'func': self.replay},
-                          '1': {'help': 'Previous Image', 'func': self.previous}, '2': {'help': 'Next Image', 'func': self.next},
-                          'S': {'help': 'Save Object', 'func': self.save},
-                          'c': {'help': 'Show/Hide cursor', 'func': self.show_cursor},
-                          'aA': {'help': 'Show/Hide ticks and their labels', 'func': self.show_ticks},
-                          'alt+a': {'help': 'Show/Hide annotations', 'func': self.toggle_annotate}}  # IMPORTANT: add the 'alt/ctrl+key' versions of key after the key in the dictionary above, not before, otherwise the naked key version will statisfy the condition `is key in this`? in the parser.
-        self.auto_brightness, self.pix_vals = False, False; self.boundaries_flag, self.annot_flag = True, False
-        self.info_loc = [0.8, 0.01] if info_loc is None else info_loc
-        self.message, self.message_obj, self.cursor = '', None, None
-    def show_help(self, event):
-        default_plt = {"q ": {'help': "Quit Figure."},
-                       "Ll": {'help': "change x/y scale to log and back to linear (toggle)"},
-                       "Gg": {'help': "Turn on and off x and y grid respectively."},
-                       "s ": {'help': "Save Figure"},
-                       "f ": {'help': "Toggle Full screen"},
-                       "p ": {'help': "Select / Deselect Pan"}}
-        if "Keyboard shortcuts" in plt.get_figlabels(): plt.close("Keyboard shortcuts"); _ = event  # toggle
-        else:
-            fig = plt.figure(num="Keyboard shortcuts")
-            for i, key in enumerate(self.help_menu.keys()): fig.text(0.1, 1 - 0.05 * (i + 1), f"{key:30s} {self.help_menu[key]['help']}")
-            print(pd.DataFrame([[val['help'], key] for key, val in self.help_menu.items()], columns=['Action', 'Key']), "\nDefault plt Keys:\n")
-            print(pd.DataFrame([[val['help'], key] for key, val in default_plt.items()], columns=['Action', 'Key']))
-    # =============== EVENT METHODS ====================================
-    def animate(self): pass  # a method of the artist child class that is inheriting from this class to define behaviour when user press next or previous buttons.
-    def connect(self): self.fig.canvas.mpl_connect('key_press_event', self.process_key); return self
-    def process_key(self, event):
-        self.event = event  # useful for debugging.
-        for key in self.help_menu.keys():
-            if event.key in key: self.help_menu[key]['func'](event); self.update_info_text(self.message); break
-        if event.key != 'q': event.canvas.figure.canvas.draw()  # for smooth quit without throwing errors  # don't update if you want to quit.
-    def toggle_annotate(self, event):
-        self.annot_flag = not self.annot_flag
-        if event.inaxes and event.inaxes.images: event.inaxes.images[0].set_picker(True); self.message = f"Annotation flag is toggled to {self.annot_flag}"
-    def annotate(self, event, axis=None, data=None):
-        self.event = event; e = event.mouseevent; ax = e.inaxes if axis is None else axis
-        if not ax: return None
-        if not hasattr(ax, 'annot_obj'): ax.annot_obj = ax.annotate("", xy=(0, 0), xytext=(-30, 30), textcoords="offset points", arrowprops=dict(arrowstyle="->", color="w", connectionstyle="arc3"),
-                                                                    va="bottom", ha="left", fontsize=10, bbox=dict(boxstyle="round", fc="w"), )
-        else: ax.annot_obj.set_visible(self.annot_flag)
-        x, y = int(np.round(e.xdata)), int(np.round(e.ydata))
-        z = e.inaxes.images[0].get_array()[y, x] if data is None else data[y, x]
-        ax.annot_obj.set_text(f'x:{x}\ny:{y}\nvalue:{z:.3f}'); ax.annot_obj.xy = (x, y); self.fig.canvas.draw_idle()
-    def save(self, event): _ = event; Save.pickle(path=P.tmpfile(name="figure_manager"), obj=self)
-    def replay(self, event): _ = event; self.pause = False; self.idx_cycle.set_index(0); self.message = 'Replaying'; self.animate()
-    def pause_func(self, event): _ = event; self.pause = not self.pause; self.message = f'Pause flag is set to {self.pause}'; self.animate()
-    def previous(self, event): _ = event; self.idx_cycle.previous(); self.message = f'Previous {self.idx_cycle}'; self.animate()
-    def next(self, event): _ = event; self.idx_cycle.next(); self.message = f'Next {self.idx_cycle}'; self.animate()
-    def text_info(self, event): _ = event; self.message = ''
-    def change_facecolor(self, event): self.fig.set_facecolor(self.facecolor.next() if event.key == '>' else self.facecolor.previous()); self.message = f"Figure facecolor was set to {self.mcolors[self.facecolor.get_index()]}"
-    def adjust_brightness(self, event):
-        ax, message = event.inaxes, "None"
-        if ax is None or not ax.images: return None
-        if event.key == '\\':
-            self.auto_brightness = not self.auto_brightness; message = f"Auto-brightness flag is toggled to {self.auto_brightness}"
-            if self.auto_brightness: im = self.ax.images[0]; im.norm.autoscale(im.get_array())  # changes to all ims take place in animate as in ImShow and Nifti methods animate.
-        vmin, vmax = ax.images[0].get_clim()
-        if event.key in '-_': message = 'increase vmin'; vmin += 1
-        elif event.key in '[{': message = 'decrease vmin'; vmin -= 1
-        elif event.key in '=+': message = 'increase vmax'; vmax += 1
-        elif event.key in ']}': message = 'decrease vmax'; vmax -= 1
-        self.message = message + '  ' + str(round(vmin, 1)) + '  ' + str(round(vmax, 1))
-        if event.key in '_+}{': [ax.images[0].set_clim((vmin, vmax)) for ax in self.fig.axes if ax.images]
-        else: ax.images[0].set_clim((vmin, vmax)) if ax.images else None
-    def change_cmap(self, event):
-        if ax := event.inaxes is not None:
-            cmap = self.cmaps.next() if event.key in 'tT' else self.cmaps.previous()
-            [[im.set_cmap(cmap) for im in ax.images] for ax in self.fig.axe] if event.key in 'TY'else [im.set_cmap(cmap) for im in ax.images]
-            self.message = f"Color map changed to {ax.images[0].cmap.name}"
-    def show_pix_val(self, event):
-        if (ax := event.inaxes) is not None:
-            self.pix_vals = not self.pix_vals; self.message = f"Pixel values flag set to {self.pix_vals}"
-            if self.pix_vals: self.show_pixels_values(ax)
-            else:
-                while len(ax.texts) > 0: [text.remove() for text in ax.texts]
-    def show_cursor(self, event):
-        if not (ax := event.inaxes): return None  # don't do this if c was pressed outside an axis.
-        if hasattr(ax, 'cursor_'):  # is this the first time?
-            if ax.cursor_ is None: ax.cursor_ = widgets.Cursor(ax=ax, vertOn=True, horizOn=True, color='red', lw=1.0)
-            else: ax.cursor_ = None  # toggle the cursor.
-            self.message = f'Cursor flag set to {bool(ax.cursor_)}'
-        else: ax.cursor_ = None; self.show_cursor(event)  # first call
-    def show_ticks(self, event):
-        self.boundaries_flag = not self.boundaries_flag
-        if event.key == 'a' and (axis := event.inaxes): self.toggle_ticks(axis); self.message = f"Boundaries flag set to {self.boundaries_flag} in {axis}"
-        else: [self.toggle_ticks(ax) for ax in self.ax]
-    # ====================== class methods ===============================
-    def get_fig(self, figname='', suffix=None, **kwargs): return FigureManager.get_fig_static(self.figpolicy, figname, suffix, **kwargs)
-    def update_info_text(self, message): self.message_obj.remove() if self.message_obj else None; self.message_obj = self.fig.text(*self.info_loc, message, fontsize=8)
-    def maximize_fig(self): _ = self; plt.get_current_fig_manager().full_screen_toggle()  # TODO not working appropriately ImShow.test() # The command required is backend-dependent and also OS dependent. Doesn't work if figure is not shown yet.
-    def clear_axes(self): [ax.cla() for ax in self.ax]
-    def transperent_fig(self): self.fig.canvas.manager.window.attributes("-transparentcolor", "white")
-    def close(self): plt.close(self.fig)
-    # ====================== axis helpers ========================
-    @staticmethod
-    def grid(ax, factor=5, x_or_y='both', color='gray', alpha1=0.5, alpha2=0.25):
-        if type(ax) in {list, List, np.ndarray}: [FigureManager.grid(an_ax, factor=factor, x_or_y=x_or_y, color=color, alpha1=alpha1, alpha2=alpha2) for an_ax in ax]  # Turning on major grid for both axes.
-        ax.grid(which='major', axis='x', color='gray', linewidth=0.5, alpha=alpha1); ax.grid(which='major', axis='y', color='gray', linewidth=0.5, alpha=alpha1)
-        if x_or_y in {'both', 'x'}: xt = ax.get_xticks(); ax.xaxis.set_minor_locator(plt.MultipleLocator((xt[1] - xt[0]) / factor)); ax.grid(which='minor', axis='x', color=color, linewidth=0.5, alpha=alpha2)
-        if x_or_y in {'both', 'y'}: yt = ax.get_yticks(); ax.yaxis.set_minor_locator(plt.MultipleLocator((yt[1] - yt[0]) / factor)); ax.grid(which='minor', axis='y', color=color, linewidth=0.5, alpha=alpha2)
-    @staticmethod
-    def set_ax_size(ax, w, h, units='inches'):
-        l, r, t, b, _ = ax.figure.subplotpars.left, ax.figure.subplotpars.right, ax.figure.subplotpars.top, ax.figure.subplotpars.bottom, units
-        ax.figure.set_size_inches(float(w) / (r - l), float(h) / (t - b))
-    @staticmethod
-    def get_ax_size(ax, units="inches"):
-        w, h = ax.figure.get_size_inches() if units == "inches" else ax.figure.get_size_pixels()
-        width, height = ax.figure.subplotpars.right - ax.figure.subplotpars.left, ax.figure.subplotpars.top - ax.figure.subplotpars.bottom
-        return w * width, h * height
-    @staticmethod
-    def toggle_ticks(an_ax, state=None): [line.set_visible(not line.get_visible() if state is None else state) for line in an_ax.get_yticklines() + an_ax.get_xticklines() + an_ax.get_xticklabels() + an_ax.get_yticklabels()]
-    @staticmethod
-    def set_ax_to_real_life_size(ax, inch_per_unit=1 / 25.4): FigureManager.set_ax_size(ax, (ax.get_xlim()[1] - ax.get_xlim()[0]) * inch_per_unit, (ax.get_ylim()[1] - ax.get_ylim()[0]) * inch_per_unit)
-    @staticmethod
-    def show_pixels_values(ax):
-        xmin, xmax = ax.get_xlim(); ymin, ymax = ax.get_ylim()
-        if ymin > ymax: ymin, ymax = ymax, ymin  # default imshow settings
-        [ax.text(i, j, np.round(label).__int__(), ha='center', va='center', size=8) for (j, i), label in np.ndenumerate(ax.images[0].get_array()) if (xmin < i < xmax) and (ymin < j < ymax)]
-    # ============================ matplotlib setup ==============================
-    @staticmethod
-    def get_nrows_ncols(num_plots, nrows=None, ncols=None):
-        if not nrows and not ncols:
-            nrows, ncols = int(np.floor(np.sqrt(num_plots))), int(np.ceil(np.sqrt(num_plots)))
-            while nrows * ncols < num_plots: ncols += 1
-        elif not ncols and nrows: ncols = int(np.ceil(num_plots / nrows))
-        elif not nrows and ncols: nrows = int(np.ceil(num_plots / ncols))
-        return nrows, ncols
-    @staticmethod
-    def findobj(figname, obj_name): return (plt.figure(num=figname) if type(figname) is str else figname).findobj(lambda x: x.get_label() == obj_name)
-    @staticmethod
-    def get_fig_static(figpolicy, figname='', suffix=None, **kwargs):
-        exist = True if figname in plt.get_figlabels() else False
-        if figpolicy is FigurePolicy.same: return plt.figure(num=figname, **kwargs)
-        elif figpolicy is FigurePolicy.add_new: return plt.figure(num=(timestamp(name=figname) if suffix is None else figname + suffix) if exist else figname, **kwargs)
-        elif figpolicy is FigurePolicy.close_create_new: plt.close(figname) if exist else None; return plt.figure(num=figname, **kwargs)
-    @staticmethod
-    def try_figure_size():
-        fig, ax = plt.subplots()
-        y = np.sin(x := np.arange(0, 100, 0.01)) * 100
-        ax.plot(x, y); ax.axis("square"); ax.set_xlim(0, 100); ax.set_ylim(-100, 100)
-        FigureManager.set_ax_to_real_life_size(ax); fig.savefig(P.tmp() / "trial.png", dpi=250)
-    @staticmethod
-    def write(txt, name="text", size=8, **kwargs):
-        FigureManager.maximize_fig(fig := plt.figure(figsize=(11.69, 8.27), num=name))
-        fig.clf(); fig.text(0.5, 0.5, txt, transform=fig.transFigure, size=size, ha="center", va='center', **kwargs); return fig
-    @staticmethod
-    def activate_latex(size=20):
-        plt.rc('xtick', labelsize=size); plt.rc('ytick', labelsize=size)
-        plt.rc('axes', titlesize=size); plt.rc('legend', fontsize=size / 1.5)  # rc('text', usetex=True)
-        plt.rcParams['text.usetex'] = True; plt.rc('font', **{'family': 'serif', 'serif': ['Computer Modern']})
-    @staticmethod
-    def set_linestyles_and_markers_and_colors(test=False):
-        from cycler import cycler; from matplotlib import lines
-        markers = list(lines.lineMarkers.keys())[:-4]  # ignore the None
-        linestyles = (list(lines.lineStyles.keys())[:-3] * 10)[:len(markers)]
-        colors = (plt.rcParams['axes.prop_cycle'].by_key()['color'] * 10)[:len(markers)]
-        default_cycler = (cycler(linestyle=linestyles) + cycler(marker=markers) + cycler(color=colors))
-        plt.rc('axes', prop_cycle=default_cycler)
-        if test: [plt.plot(aq + idx * 2) for idx, aq in enumerate(np.random.randn(10, 10))]
-
-
-class VisibilityViewer(FigureManager):  # This is used for browsing purpose, as opposed to saving.
-    artist = ['internal', 'external'][1]  # How is the data visualized? You need artist. The artist can either be internal, as in ImShow or passed externally (especially non image data)
-    parser = ['internal', 'external'][1]  # Data parsing: internal for loop to go through all the dataset passed. # Allows manual control over parsing. external for loop. It should have add method. # Manual control only takes place after the external loop is over. #TODO parallelize this.
-    stream = ['clear', 'accumulate', 'update'][1]  # Streaming (Refresh mechanism): * Clear the axis. (slowest, but easy on memory) * accumulate, using visibility to hide previous axes. (Fastest but memory intensive)  * The artist has an update method. (best)
-    """ This class works on hiding axes shown on a plot, so that a new plot can be drawn. Once the entire loop is finished, you can browse through the plots with the keyboard Animation linked to `animate`"""
-    def __init__(self, fig):  # Downside: slow if number of axes, lines, texts, etc. are too large. In that case, it is better to avoid this viewer and plot on the fly during animation.
-        super().__init__(); self.objs_repo = []  # list of lists of axes and texts.
-        self.fig = fig; self.connect(); self.idx_cycle = Cycle([])
-    def add(self, objs): self.idx_cycle.expand(); self.objs_repo.append(objs); [obj.set_visible(False) for obj in (self.objs_repo[-2] if len(self.objs_repo) > 1 else [])]; print(f"VViewer added plot number {self.idx_cycle.get_index()}", end='\r')
-    def animate(self): [ax.set_visible(False) for ax in self.objs_repo[self.idx_cycle.prev_index]]; [ax.set_visible(True) for ax in self.objs_repo[self.idx_cycle.get_index()]]; self.fig.canvas.draw()
-
-
-class Artist(FigureManager):  # This object knows how to draw a figure from curve-type data.
-    def __init__(self, ax=None, figname='Graph', title='', label='curve', style='seaborn', figpolicy=FigurePolicy.add_new, figsize=(14, 8)):
-        super().__init__(figpolicy=figpolicy)
-        self.style, self.title = style, title; self.line = self.cursor = self.check_b = None
-        if ax is None:  # create a figure
-            with plt.style.context(style=self.style): self.fig = self.get_fig(figname, figsize=figsize); self.ax = self.fig.subplots()
-        else: self.ax = ax; self.fig = ax.figure  # use the passed axis
-        self.visibility_ax, self.txt, self.label = [0.01, 0.05, 0.2, 0.15], [], label
-    def plot(self, *args, legends=None, title=None, **kwargs): self.line = self.ax.plot(*args, **kwargs); self.ax.legend(legends or []); self.ax.set_title(title) if title is not None else None; self.ax.grid('on')
-    def plot_dict(self, adict, title='', xlabel='', ylabel=''): [self.plot(val, label=key) for key, val in adict.items()]; self.ax.legend(); self.ax.set_title(title); self.ax.set_xlabel(xlabel); self.ax.set_ylabel(ylabel); return self
-    def plot_twin(self, c1, c2, x=None, l1='', l2='', ax=None): ax = ax or self.ax; twin_ax = ax.twinx(); line1 = ax.plot(x or range(len(c1)), c1, color="blue", label=l1)[0]; line2 = twin_ax.plot(c2, color="red", label=l2)[0]; twin_ax.legend([line1, line2], [l1, l2]); ax.set_ylabel(l1); twin_ax.set_ylabel(l2); plt.show()
-    def suptitle(self, title): self.txt = [self.fig.text(0.5, 0.98, title, ha='center', va='center', size=9)]
-    def clear(self): self.fig.clf()  # objects that use this class will demand that the artist expose this method, in addition to .plot()
-    def axes(self): return [self.ax]  # objects that use this class will demand that the artist expose this method, in addition to .plot()
-    def visibility(self):
-        from matplotlib.widgets import CheckButtons; self.fig.subplots_adjust(left=0.3); self.visibility_ax[-1] = 0.05 * len(self.ax.lines)
-        rax = self.fig.add_axes(self.visibility_ax)
-        labels, visibility = [str(line.get_label()) for line in self.ax.lines], [line.get_visible() for line in self.ax.lines]
-        self.check_b = CheckButtons(rax, labels, visibility)
-        def func(label): index = labels.index(label); self.ax.lines[index].set_visible(not self.ax.lines[index].get_visible()); self.fig.canvas.draw()
-        self.check_b.on_clicked(func)
-    @staticmethod
-    def styler(plot_gen):
-        for astyle in plt.style.available:
-            with plt.style.context(style=astyle): plot_gen(); plt.title(astyle); plt.pause(1); plt.cla()
-
-
-class VisibilityViewerAuto(VisibilityViewer):
-    artist = ['internal', 'external'][1]
-    parser = ['internal', 'external'][0]
-    stream = ['clear', 'accumulate', 'update'][0:2]
-    def __init__(self, data=None, artist=None, stream='clear', save_type=FigureSave.Null, save_dir=None, save_name=None, delay=1,
-                 titles=None, legends=None, x_labels=None, pause=True, **kwargs):
-        """data: tensor of form  NumInputsForAnimation x ArgsPerPlot (to be unstarred) x Input (possible points x signals)
-        stream: ensure that behaviour of artist is consistent with stream. When `cccumulate`, artist should create new axes whenever plot is called."""
-        self.data = data; self.artist = artist or Artist()
-        self.legends = [f"Plot {i}" for i in range(len(self.data))] if legends is None else legends; self.titles = titles if titles is not None else np.arange(len(self.data))
-        super().__init__(fig=self.artist.fig); _ = kwargs
-        self.saver = save_type(watch_figs=[self.artist.fig], save_dir=save_dir, save_name=save_name, delay=delay, fps=1000 / delay)
-        self.index_max, self.pause, self.stream, self.lables = len(self.data), pause, stream, x_labels
-    test = staticmethod(lambda: VisibilityViewerAuto(data=np.random.randn(10, 1, 10, 3)))
-    def animate(self):
-        for i in range(0, self.index_max):
-            self.artist.plot(*self.data[i], title=self.titles[i], legends=self.legends)  # replot the new data point on a new axis.
-            super().add(self.artist.axes()) if self.stream == 'accumulate' else self.artist.clear()
-            self.saver.add()
-            if self.pause: break
-            else: self.idx_cycle.set_index(i)
-        return self.saver.finish()  # arrived at last image and not in manual mode
-
-
-class ImShow(FigureManager):
-    artist = ['internal', 'external'][0]
-    parser = ['internal', 'external'][0]
-    stream = ['clear', 'accumulate', 'update'][2]
-    def __init__(self, img_tensor, sup_titles=None, sub_labels=None, save_type=FigureSave.Null, save_name=None, save_dir=None, save_kwargs=None,
-                 subplots_adjust=None, gridspec=None, tight=True, info_loc=None, nrows=None, ncols=None, ax=None,
-                 figsize=None, figname='im_show', auto_brightness=True, delay=200, pause=False, **kwargs):
-        """
-        :param img_tensor: size N x M x W x H [x C]  # M used spatially, N for animation.
-        :param sup_titles: Titles for frames (N)
-        :param sub_labels: M x N. If shape sent is M
-        """
-        n, m = len(img_tensor), len(img_tensor[0]); self.m, self.n = m, n; super(ImShow, self).__init__(info_loc=info_loc)
-        nrows, ncols = self.get_nrows_ncols(m, nrows, ncols)
-        self.img_tensor, self.sub_labels, self.sup_titles = img_tensor, sub_labels if sub_labels is not None else [[f"{i}-{j}" for j in range(m)] for i in range(n)], sup_titles if sup_titles is not None else np.arange(n)
-        self.pause, self.kwargs, self.delay, self.auto_brightness = pause, kwargs, delay, auto_brightness
-        self.fname = self.event = None; self.ims = []  # container for images.
-        self.cmaps = Cycle(plt.colormaps()); self.cmaps.set_value('viridis')
-        if ax is None:
-            self.fig = self.get_fig(figname=figname, figsize=(14, 9) if figsize is None else figsize, facecolor='white'); self.maximize_fig() if figsize is None else None
-            if gridspec is not None: gs = self.fig.add_gridspec(gridspec[0]); self.ax = [self.fig.add_subplot(gs[ags[0], ags[1]]) for ags in gs[1:]]
-            else: self.ax = self.fig.subplots(nrows=nrows, ncols=ncols)
-        else: self.ax = ax; self.fig = ax[0].figure if type(ax) is list else ax.figure
-        self.connect(); self.fig.canvas.mpl_connect("pick_event", self.annotate)
-        self.fig.tight_layout() if tight else None; self.fig.subplots_adjust(**subplots_adjust) if subplots_adjust is not None else None
-        self.saver = save_type(watch_figs=[self.fig], save_dir=save_dir, save_name=save_name, delay=delay, fps=1000 / delay, **({} if save_kwargs is None else save_kwargs))
-        self.ax = [self.ax] if nrows == 1 and ncols == 1 else self.ax.ravel()  # make a list out of it or # make a 1D  list out of a 2D array.
-        [self.toggle_ticks(an_ax, state=False) for an_ax in self.ax]; self.idx_cycle = Cycle(max_idx=len(self.img_tensor))  # self.animate()
-    def animate(self):
-        for i in range(self.idx_cycle.get_index(), self.n):
-            for j, (an_image, a_label, an_ax) in enumerate(zip(self.img_tensor[i], self.sub_labels[i], self.ax)):  # with zipping, the shortest of the three, will stop the loop.
-                if i == 0 and self.ims.__len__() < self.m: self.ims.append(an_ax.imshow(an_image, animated=True, **self.kwargs))
-                else: self.ims[j].set_data(an_image)
-                if self.auto_brightness: self.ims[j].norm.autoscale(an_image)
-                an_ax.set_xlabel(f'{a_label}')
-            self.fig.suptitle(self.sup_titles[i], fontsize=8); self.saver.add(names=[self.sup_titles[i]])
-            if self.pause: break
-            else: self.idx_cycle.set_index(i)
-        if self.idx_cycle.get_index() == self.n - 1 and not self.pause: self.fname = self.saver.finish()  # arrived at last image and not in manual mode
-    @staticmethod
-    def try_cmaps(im, nrows=3, ncols=7, **kwargs): _ = ImShow(*np.array_split([plt.get_cmap(style)(im) for style in plt.colormaps()], nrows * ncols), nrows=nrows, ncols=ncols, sub_labels=np.array_split(plt.colormaps(), nrows * ncols), **kwargs); return [plt.get_cmap(style)(im) for style in plt.colormaps()]
-    def annotate(self, event, axis=None, data=None): [super().annotate(event, axis=ax, data=ax.images[0].get_array()) for ax in self.ax]
-    from_img_paths = staticmethod(lambda paths, **kwargs: ImShow(List(paths).apply(plt.imread), sub_labels=List(paths).apply(lambda x: P(x).stem), **kwargs))
-    from_complex = staticmethod(lambda data, pause=True, **kwargs: ImShow(data.real, data.imag, np.angle(data), abs(data), labels=['Real Part', 'Imaginary Part', 'Angle in Radians', 'Absolute Value'], pause=pause, **kwargs))
-    test = staticmethod(lambda: ImShow(np.random.rand(12, 10, 80, 120, 3)))  # https://ai.googleblog.com/2019/08/turbo-improved-rainbow-colormap-for.html # https://gist.github.com/mikhailov-work/ee72ba4191942acecc03fe6da94fc73f
-    resize = staticmethod(lambda path, m, n: plt.imsave(path, install_n_import(package="skimage", name="scikit-image").transform.resize(plt.imread(path), (m, n), anti_aliasing=True)))
-
-
-if __name__ == '__main__':
-    pass
+
+
+from crocodile.core import List, timestamp, Save, install_n_import, validate_name
+from crocodile.file_management import P
+from crocodile.meta import Terminal
+
+import matplotlib.pyplot as plt
+from crocodile.msc.odds import Cycle
+from matplotlib import widgets
+import matplotlib.colors as mcolors
+from matplotlib import animation
+import enum
+import subprocess
+import platform
+import pandas as pd
+import numpy as np
+
+
+"""TODO: add implementation https://github.com/gustavovelascoh/plot_update
+"""
+
+
+class FigurePolicy(enum.Enum):
+    close_create_new = 'Close the previous figure that has the same figname and create a new fresh one'
+    add_new = 'Create a new figure with same path but with added suffix'
+    same = 'Grab the figure of the same path'
+
+
+def assert_requirements():
+    try: subprocess.check_output(['where.exe' if platform.system() == 'Windows' else 'which', 'magick'])
+    except (FileNotFoundError, subprocess.CalledProcessError):
+        # P(r"https://www.gyan.dev/ffmpeg/builds/ffmpeg-git-full.7z").download().unzip().search()[0].rename("ffmpeg").move(r"C://")  # P("C:\\ffmpeg\\bin")  # add to PATH
+        print("Installinng image magick")
+        if __import__("platform").system() == "Windows":
+            Terminal().run("winget install ImageMagick.ImageMagick", shell="powershell")  # gives ffmpeg as well
+            print("You might need to restart your machine before PATH change impact takes place.")
+        else: raise NotImplementedError
+
+
+class FigureSave:
+    class GenericSave:
+        stream = ['clear', 'accumulate', 'update'][0]
+        def __init__(self, save_dir=None, save_name=None, watch_figs: list or None = None, max_calls=2000, delay=100, **kwargs):
+            """How to control what to be saved: you can either pass the figures to be tracked at init time, pass them dynamically at add time, or, add method will capture every figure and axis"""
+            self.watch_figs = watch_figs if watch_figs is None else ([plt.figure(num=afig) for afig in watch_figs] if type(watch_figs[0]) is str else watch_figs)
+            self.save_name, self.save_dir = timestamp(name=save_name), save_dir or P.tmpdir(prefix="tmp_fig_save")
+            self.kwargs, self.counter, self.delay, self.max = kwargs, 0, delay, max_calls
+        def add(self, fignames=None, names=None, **kwargs):  # generic method used at runtime, never changed.
+            print(f"Saver added frame number {self.counter}", end='\r')
+            self.counter += 1; plt.pause(self.delay * 0.001); print('Turning off IO') if self.counter > self.max else None; plt.ioff()
+            self.watch_figs = [plt.figure(figname) for figname in fignames] if fignames else ([plt.figure(k) for k in plt.get_figlabels()] if self.watch_figs is None else self.watch_figs)  # path sent explicitly, # None exist ==> add all else # they exist already.
+            if names is None: names = [timestamp(name=a_figure.get_label()) for a_figure in self.watch_figs]  # individual save path, useful for PNG.
+            for afig, aname in zip(self.watch_figs, names): self._save(afig, aname, **kwargs)
+        def _save(self, *args, **kwargs): pass  # called by generic method `add`, to be implemented when subclassing.
+    class Null(GenericSave):  # serves as a filler.
+        def __init__(self, *args, **kwargs): super().__init__(*args, **kwargs); self.fname = self.save_dir
+        def finish(self): print(f"Nothing saved by {self}"); return self.fname
+    class PDF(GenericSave):  # For pdf, you just need any stream [update, clear, accumalate], preferabbly the fastest."""
+        def __init__(self, *args, **kwargs):
+            super().__init__(*args, **kwargs)
+            from matplotlib.backends.backend_pdf import PdfPages
+            self.fname = self.save_dir.joinpath(self.save_name + ('.pdf' if '.pdf' not in str(self.save_name) else '')); self.pp = PdfPages(self.fname)
+        def _save(self, a_fig, a_name, bbox_inches='tight', pad_inches=0.3, **kwargs): self.pp.savefig(a_fig, bbox_inches=bbox_inches, pad_inches=pad_inches, **kwargs)
+        def finish(self): print(f"Saving results ..."); self.pp.close(); print(f"SAVED PDF @", P(self.fname).absolute().as_uri()); return self
+    class PNG(GenericSave):
+        def __init__(self, *args, **kwargs): super().__init__(*args, **kwargs); self.fname = self.save_dir = self.save_dir.joinpath(self.save_name)
+        def _save(self, afigure, aname, dpi=150, **kwargs):  afigure.savefig(self.save_dir.joinpath(validate_name(aname)).create(parents_only=True), bbox_inches='tight', pad_inches=0.3, dpi=dpi, **kwargs)
+        def finish(self): print(f"SAVED PNGs @", P(self.fname).absolute().as_uri()); return self
+    class GIF(GenericSave):  # NOT RECOMMENDED, used GIFFileBased instead.
+        """This class uses ArtistAnimation: works on lines and images list attached to figure axes and Doesn't work on axes, unless you add large number of them. As such, titles are not incorporated etc (limitation).
+        Requirements: same axis must persist (If you clear the axis, nothing will be saved), only new objects are drawn inside it. Additionally, the objects drawn must not be removed, or updated, instead they should pile up in axis.
+        # usually it is smoother when adding animate=True to plot or imshow commands for GIF purpose
+        Works for images only. Add more .imshow to the same axis, and that's it. imshow will conver up previous images. For lines, it will superimpose it and will look ugly.
+        The class will automatically detect new lines by their "neo" labels and add them then hide them for the next round.
+        """
+        def __init__(self, interval=100, **kwargs):
+            super().__init__(**kwargs); from collections import defaultdict
+            self.container, self.interval, self.fname = defaultdict(lambda: []), interval, None  # determined at finish time.
+        def _save(self, afigure, aname, cla=False, **kwargs):
+            fig_list, subcontainer = self.container[afigure.get_label()], []
+            for item in FigureManager.findobj(afigure, 'neo'): item.set_label('processed'); item.set_visible(False); subcontainer += [item]
+            fig_list.append(subcontainer)  # if you want the method coupled with cla being used in main, then it add_line is required for axes.
+        def finish(self):
+            print("Saving the GIF ....")
+            for idx, a_fig in enumerate(self.watch_figs):
+                if ims := self.container[a_fig.get_label()]:
+                    self.fname = self.save_dir.joinpath(f'{a_fig.get_label()}_{self.save_name}.gif')
+                    ani = animation.ArtistAnimation(a_fig, ims, interval=self.interval, blit=True, repeat_delay=1000)
+                    # noinspection PyTypeChecker
+                    ani.save(self.fname, writer=animation.PillowWriter(fps=4))  # if you don't specify the writer, it goes to ffmpeg by default then try others if that is not available, resulting in behaviours that is not consistent across machines.
+                    print(f"SAVED GIF @", P(self.fname).absolute().as_uri())
+                else: print(f"Nothing to be saved by GIF writer."); return self.fname
+    class GIFFileBased(GenericSave):
+        def __init__(self, fps=4, dpi=100, bitrate=1800, _type='GIFFileBased', **kwargs):
+            super().__init__(**kwargs); assert_requirements()
+            if _type == 'GIFPipeBased': writer, extension = animation.ImageMagickFileWriter, '.gif'  # internally calls: matplotlib._get_executable_info("magick")
+            elif _type == "GIFFileBased": writer, extension = animation.ImageMagickWriter, '.gif'
+            elif _type == 'MPEGFileBased': writer, extension = animation.FFMpegFileWriter, '.mp4'
+            elif _type == 'MPEGPipeBased': writer, extension = animation.FFMpegWriter, '.mp4'
+            else: raise ValueError("Unknown writer.")
+            self.writer = writer(fps=fps, metadata=dict(artist='Alex Al-Saffar'), bitrate=bitrate)
+            self.fname = self.save_dir.joinpath(self.save_name + extension)
+            assert self.watch_figs, "No figure was sent during instantiation of saver, therefore the writer cannot be setup. Did you mean to use an autosaver?"
+            self.writer.setup(fig=self.watch_figs[0], outfile=str(self.fname), dpi=dpi)
+        def _save(self, afig, aname, **kwargs): self.writer.grab_frame(**kwargs)
+        def finish(self): print('Saving results ...'); self.writer.finish(); print(f"SAVED GIF @", P(self.fname).absolute().as_uri()); return self
+    class GIFPipeBased(GIFFileBased):
+        def __init__(self, *args, **kwargs): super().__init__(*args, _type=self.__class__.__name__, **kwargs)
+    class MPEGFileBased(GIFFileBased):
+        def __init__(self, *args, **kwargs): super().__init__(*args, _type=self.__class__.__name__, **kwargs)
+    class MPEGPipeBased(GIFFileBased):
+        def __init__(self, *args, **kwargs): super().__init__(*args, _type=self.__class__.__name__, **kwargs)
+    class GenericAuto(GenericSave):
+        """Parses the data internally, hence requires artist with animate method implemetend. Artist needs to have .fig attribute."""
+        save_type = 'auto'
+        def __init__(self, plotter_class, data, names_list=None, **kwargs):
+            super().__init__(**kwargs); self.saver, self.plotter = None, None; assert_requirements()
+            self.plotter_class, self.data, self.names_list, self.kwargs = plotter_class, data, names_list, kwargs
+        def animate(self):
+            self.plotter = self.plotter_class(**self.kwargs); plt.pause(0.5)  # give time for figures to show up before updating them
+            for idx, datum in __import__("tqdm").tqdm(enumerate(self.data)): self.plotter.animate(datum); self.saver.add(names=[self.names_list[idx] if self.names_list is not None else str(idx)])
+            self.saver.finish()
+    class GIFAuto(GenericAuto):
+        def __init__(self, plotter_class, data, interval=500, extension='gif', fps=4, metadata=None, **kwargs):
+            super().__init__(plotter_class, data, **kwargs)
+            writer = animation.PillowWriter(fps=fps) if extension == '.mp4' else animation.FFMpegWriter(fps=fps, metadata=metadata, bitrate=2500)
+            self.plotter = self.plotter_class(**kwargs); plt.pause(self.delay * 0.001)  # give time for figures to show up before updating them
+            # noinspection PyTypeChecker
+            self.ani = animation.FuncAnimation(fig=self.plotter.fig, func=self.plotter.animate, frames=(i for i in zip(*self.data)), interval=interval, repeat_delay=1500, fargs=None, cache_frame_data=True, save_count=10000)
+            self.fname = self.save_dir.joinpath(self.save_name + f".{extension}")
+            self.ani.save(filename=self.fname, writer=writer); print(f"SAVED GIF @ ", P(self.fname).absolute().as_uri())
+    class PDFAuto(GenericAuto):
+        def __init__(self, **kwargs): super().__init__(**kwargs); self.saver = FigureSave.PDF(**kwargs); self.animate()
+    class PNGAuto(GenericAuto):
+        def __init__(self, **kwargs): super().__init__(**kwargs); self.saver = FigureSave.PNG(**kwargs); self.save_dir = self.saver.save_dir; self.animate(); self.fname = self.saver.fname
+    class NullAuto(GenericAuto):
+        def __init__(self, **kwargs): super().__init__(**kwargs); self.saver = FigureSave.Null(**kwargs); self.fname = self.saver.fname; self.animate()
+    class GIFFileBasedAuto(GenericAuto):
+        def __init__(self, plotter_class, data, fps=4, dpi=150, bitrate=2500, _type='GIFFileBasedAuto', **kwargs):
+            super().__init__(**kwargs)
+            if _type == 'GIFPipeBasedAuto': writer = animation.ImageMagickFileWriter; extension = '.gif'
+            elif _type == 'MPEGFileBasedAuto': writer = animation.FFMpegFileWriter; extension = '.mp4'
+            elif _type == 'MPEGPipeBasedAuto': writer = animation.FFMpegWriter; extension = '.mp4'
+            else: raise ValueError("Unknown writer.")
+            self.saver = writer(fps=fps, metadata=dict(artist='Alex Al-Saffar'), bitrate=bitrate)
+            self.fname = self.save_dir.joinpath(self.save_name + extension)
+            self.data = lambda: (i for i in zip(*data)); self.plotter = plotter_class(*[piece[0] for piece in data], **kwargs); plt.pause(0.5); from tqdm import tqdm
+            with self.saver.saving(fig=self.plotter.fig, outfile=self.fname, dpi=dpi):
+                for datum in tqdm(self.data()): self.plotter.animate(datum); self.saver.grab_frame(); plt.pause(self.delay * 0.001)
+            print(f"SAVED GIF successfully @ {self.fname}")
+    class GIFPipeBasedAuto(GIFFileBasedAuto):
+        def __init__(self, *args, **kwargs): super().__init__(*args, _type=self.__class__.__name__, **kwargs)
+    class MPEGFileBasedAuto(GIFFileBasedAuto):
+        def __init__(self, *args, **kwargs): super().__init__(*args, _type=self.__class__.__name__, **kwargs)
+    class MPEGPipeBasedAuto(GIFFileBasedAuto):
+        def __init__(self, *args, **kwargs): super().__init__(*args, _type=self.__class__.__name__, **kwargs)
+
+
+class FigureManager:  # use as base class for Artist & Viewers to give it free animation powers.
+    def __init__(self, info_loc=None, figpolicy=FigurePolicy.same):
+        self.figpolicy = figpolicy
+        self.fig = self.ax = self.event = None
+        self.cmaps, self.colors, self.mcolors, self.facecolor = Cycle(plt.colormaps()), Cycle(plt.rcParams['axes.prop_cycle'].by_key()['color']), list(mcolors.CSS4_COLORS.keys()), Cycle(list(mcolors.CSS4_COLORS.values()))
+        self.cmaps.set_value('viridis')
+        self.idx_cycle = Cycle([]); self.pause = None  # animation
+        self.help_menu = {'_-=+[{]}\\': {'help': "Adjust Vmin Vmax. Shift + key applies change to all axes \\ toggles auto-brightness ", 'func': self.adjust_brightness},
+                          "/": {'help': 'Show/Hide info text', 'func': self.text_info},
+                          "h": {'help': 'Show/Hide help menu', 'func': self.show_help},
+                          "tyTY": {'help': 'Change color map', 'func': self.change_cmap},
+                          '<>': {'help': 'Change figure face color', 'func': self.change_facecolor},
+                          "v": {'help': 'Show/Hide pixel values (Toggle)', 'func': self.show_pix_val},
+                          'P': {'help': 'Pause/Proceed (Toggle)', 'func': self.pause_func},
+                          'r': {'help': 'Replay', 'func': self.replay},
+                          '1': {'help': 'Previous Image', 'func': self.previous}, '2': {'help': 'Next Image', 'func': self.next},
+                          'S': {'help': 'Save Object', 'func': self.save},
+                          'c': {'help': 'Show/Hide cursor', 'func': self.show_cursor},
+                          'aA': {'help': 'Show/Hide ticks and their labels', 'func': self.show_ticks},
+                          'alt+a': {'help': 'Show/Hide annotations', 'func': self.toggle_annotate}}  # IMPORTANT: add the 'alt/ctrl+key' versions of key after the key in the dictionary above, not before, otherwise the naked key version will statisfy the condition `is key in this`? in the parser.
+        self.auto_brightness, self.pix_vals = False, False; self.boundaries_flag, self.annot_flag = True, False
+        self.info_loc = [0.8, 0.01] if info_loc is None else info_loc
+        self.message, self.message_obj, self.cursor = '', None, None
+    def show_help(self, event):
+        default_plt = {"q ": {'help': "Quit Figure."},
+                       "Ll": {'help': "change x/y scale to log and back to linear (toggle)"},
+                       "Gg": {'help': "Turn on and off x and y grid respectively."},
+                       "s ": {'help': "Save Figure"},
+                       "f ": {'help': "Toggle Full screen"},
+                       "p ": {'help': "Select / Deselect Pan"}}
+        if "Keyboard shortcuts" in plt.get_figlabels(): plt.close("Keyboard shortcuts"); _ = event  # toggle
+        else:
+            fig = plt.figure(num="Keyboard shortcuts")
+            for i, key in enumerate(self.help_menu.keys()): fig.text(0.1, 1 - 0.05 * (i + 1), f"{key:30s} {self.help_menu[key]['help']}")
+            print(pd.DataFrame([[val['help'], key] for key, val in self.help_menu.items()], columns=['Action', 'Key']), "\nDefault plt Keys:\n")
+            print(pd.DataFrame([[val['help'], key] for key, val in default_plt.items()], columns=['Action', 'Key']))
+    # =============== EVENT METHODS ====================================
+    def animate(self): pass  # a method of the artist child class that is inheriting from this class to define behaviour when user press next or previous buttons.
+    def connect(self): self.fig.canvas.mpl_connect('key_press_event', self.process_key); return self
+    def process_key(self, event):
+        self.event = event  # useful for debugging.
+        for key in self.help_menu.keys():
+            if event.key in key: self.help_menu[key]['func'](event); self.update_info_text(self.message); break
+        if event.key != 'q': event.canvas.figure.canvas.draw()  # for smooth quit without throwing errors  # don't update if you want to quit.
+    def toggle_annotate(self, event):
+        self.annot_flag = not self.annot_flag
+        if event.inaxes and event.inaxes.images: event.inaxes.images[0].set_picker(True); self.message = f"Annotation flag is toggled to {self.annot_flag}"
+    def annotate(self, event, axis=None, data=None):
+        self.event = event; e = event.mouseevent; ax = e.inaxes if axis is None else axis
+        if not ax: return None
+        if not hasattr(ax, 'annot_obj'): ax.annot_obj = ax.annotate("", xy=(0, 0), xytext=(-30, 30), textcoords="offset points", arrowprops=dict(arrowstyle="->", color="w", connectionstyle="arc3"),
+                                                                    va="bottom", ha="left", fontsize=10, bbox=dict(boxstyle="round", fc="w"), )
+        else: ax.annot_obj.set_visible(self.annot_flag)
+        x, y = int(np.round(e.xdata)), int(np.round(e.ydata))
+        z = e.inaxes.images[0].get_array()[y, x] if data is None else data[y, x]
+        ax.annot_obj.set_text(f'x:{x}\ny:{y}\nvalue:{z:.3f}'); ax.annot_obj.xy = (x, y); self.fig.canvas.draw_idle()
+    def save(self, event): _ = event; Save.pickle(path=P.tmpfile(name="figure_manager"), obj=self)
+    def replay(self, event): _ = event; self.pause = False; self.idx_cycle.set_index(0); self.message = 'Replaying'; self.animate()
+    def pause_func(self, event): _ = event; self.pause = not self.pause; self.message = f'Pause flag is set to {self.pause}'; self.animate()
+    def previous(self, event): _ = event; self.idx_cycle.previous(); self.message = f'Previous {self.idx_cycle}'; self.animate()
+    def next(self, event): _ = event; self.idx_cycle.next(); self.message = f'Next {self.idx_cycle}'; self.animate()
+    def text_info(self, event): _ = event; self.message = ''
+    def change_facecolor(self, event): self.fig.set_facecolor(self.facecolor.next() if event.key == '>' else self.facecolor.previous()); self.message = f"Figure facecolor was set to {self.mcolors[self.facecolor.get_index()]}"
+    def adjust_brightness(self, event):
+        ax, message = event.inaxes, "None"
+        if ax is None or not ax.images: return None
+        if event.key == '\\':
+            self.auto_brightness = not self.auto_brightness; message = f"Auto-brightness flag is toggled to {self.auto_brightness}"
+            if self.auto_brightness: im = self.ax.images[0]; im.norm.autoscale(im.get_array())  # changes to all ims take place in animate as in ImShow and Nifti methods animate.
+        vmin, vmax = ax.images[0].get_clim()
+        if event.key in '-_': message = 'increase vmin'; vmin += 1
+        elif event.key in '[{': message = 'decrease vmin'; vmin -= 1
+        elif event.key in '=+': message = 'increase vmax'; vmax += 1
+        elif event.key in ']}': message = 'decrease vmax'; vmax -= 1
+        self.message = message + '  ' + str(round(vmin, 1)) + '  ' + str(round(vmax, 1))
+        if event.key in '_+}{': [ax.images[0].set_clim((vmin, vmax)) for ax in self.fig.axes if ax.images]
+        else: ax.images[0].set_clim((vmin, vmax)) if ax.images else None
+    def change_cmap(self, event):
+        if ax := event.inaxes is not None:
+            cmap = self.cmaps.next() if event.key in 'tT' else self.cmaps.previous()
+            [[im.set_cmap(cmap) for im in ax.images] for ax in self.fig.axe] if event.key in 'TY'else [im.set_cmap(cmap) for im in ax.images]
+            self.message = f"Color map changed to {ax.images[0].cmap.name}"
+    def show_pix_val(self, event):
+        if (ax := event.inaxes) is not None:
+            self.pix_vals = not self.pix_vals; self.message = f"Pixel values flag set to {self.pix_vals}"
+            if self.pix_vals: self.show_pixels_values(ax)
+            else:
+                while len(ax.texts) > 0: [text.remove() for text in ax.texts]
+    def show_cursor(self, event):
+        if not (ax := event.inaxes): return None  # don't do this if c was pressed outside an axis.
+        if hasattr(ax, 'cursor_'):  # is this the first time?
+            if ax.cursor_ is None: ax.cursor_ = widgets.Cursor(ax=ax, vertOn=True, horizOn=True, color='red', lw=1.0)
+            else: ax.cursor_ = None  # toggle the cursor.
+            self.message = f'Cursor flag set to {bool(ax.cursor_)}'
+        else: ax.cursor_ = None; self.show_cursor(event)  # first call
+    def show_ticks(self, event):
+        self.boundaries_flag = not self.boundaries_flag
+        if event.key == 'a' and (axis := event.inaxes): self.toggle_ticks(axis); self.message = f"Boundaries flag set to {self.boundaries_flag} in {axis}"
+        else: [self.toggle_ticks(ax) for ax in self.ax]
+    # ====================== class methods ===============================
+    def get_fig(self, figname='', suffix=None, **kwargs): return FigureManager.get_fig_static(self.figpolicy, figname, suffix, **kwargs)
+    def update_info_text(self, message): self.message_obj.remove() if self.message_obj else None; self.message_obj = self.fig.text(*self.info_loc, message, fontsize=8)
+    def maximize_fig(self): _ = self; plt.get_current_fig_manager().full_screen_toggle()  # TODO not working appropriately ImShow.test() # The command required is backend-dependent and also OS dependent. Doesn't work if figure is not shown yet.
+    def clear_axes(self): [ax.cla() for ax in self.ax]
+    def transperent_fig(self): self.fig.canvas.manager.window.attributes("-transparentcolor", "white")
+    def close(self): plt.close(self.fig)
+    # ====================== axis helpers ========================
+    @staticmethod
+    def grid(ax, factor=5, x_or_y='both', color='gray', alpha1=0.5, alpha2=0.25):
+        if type(ax) in {list, List, np.ndarray}: [FigureManager.grid(an_ax, factor=factor, x_or_y=x_or_y, color=color, alpha1=alpha1, alpha2=alpha2) for an_ax in ax]  # Turning on major grid for both axes.
+        ax.grid(which='major', axis='x', color='gray', linewidth=0.5, alpha=alpha1); ax.grid(which='major', axis='y', color='gray', linewidth=0.5, alpha=alpha1)
+        if x_or_y in {'both', 'x'}: xt = ax.get_xticks(); ax.xaxis.set_minor_locator(plt.MultipleLocator((xt[1] - xt[0]) / factor)); ax.grid(which='minor', axis='x', color=color, linewidth=0.5, alpha=alpha2)
+        if x_or_y in {'both', 'y'}: yt = ax.get_yticks(); ax.yaxis.set_minor_locator(plt.MultipleLocator((yt[1] - yt[0]) / factor)); ax.grid(which='minor', axis='y', color=color, linewidth=0.5, alpha=alpha2)
+    @staticmethod
+    def set_ax_size(ax, w, h, units='inches'):
+        l, r, t, b, _ = ax.figure.subplotpars.left, ax.figure.subplotpars.right, ax.figure.subplotpars.top, ax.figure.subplotpars.bottom, units
+        ax.figure.set_size_inches(float(w) / (r - l), float(h) / (t - b))
+    @staticmethod
+    def get_ax_size(ax, units="inches"):
+        w, h = ax.figure.get_size_inches() if units == "inches" else ax.figure.get_size_pixels()
+        width, height = ax.figure.subplotpars.right - ax.figure.subplotpars.left, ax.figure.subplotpars.top - ax.figure.subplotpars.bottom
+        return w * width, h * height
+    @staticmethod
+    def toggle_ticks(an_ax, state=None): [line.set_visible(not line.get_visible() if state is None else state) for line in an_ax.get_yticklines() + an_ax.get_xticklines() + an_ax.get_xticklabels() + an_ax.get_yticklabels()]
+    @staticmethod
+    def set_ax_to_real_life_size(ax, inch_per_unit=1 / 25.4): FigureManager.set_ax_size(ax, (ax.get_xlim()[1] - ax.get_xlim()[0]) * inch_per_unit, (ax.get_ylim()[1] - ax.get_ylim()[0]) * inch_per_unit)
+    @staticmethod
+    def show_pixels_values(ax):
+        xmin, xmax = ax.get_xlim(); ymin, ymax = ax.get_ylim()
+        if ymin > ymax: ymin, ymax = ymax, ymin  # default imshow settings
+        [ax.text(i, j, np.round(label).__int__(), ha='center', va='center', size=8) for (j, i), label in np.ndenumerate(ax.images[0].get_array()) if (xmin < i < xmax) and (ymin < j < ymax)]
+    # ============================ matplotlib setup ==============================
+    @staticmethod
+    def get_nrows_ncols(num_plots, nrows=None, ncols=None):
+        if not nrows and not ncols:
+            nrows, ncols = int(np.floor(np.sqrt(num_plots))), int(np.ceil(np.sqrt(num_plots)))
+            while nrows * ncols < num_plots: ncols += 1
+        elif not ncols and nrows: ncols = int(np.ceil(num_plots / nrows))
+        elif not nrows and ncols: nrows = int(np.ceil(num_plots / ncols))
+        return nrows, ncols
+    @staticmethod
+    def findobj(figname, obj_name): return (plt.figure(num=figname) if type(figname) is str else figname).findobj(lambda x: x.get_label() == obj_name)
+    @staticmethod
+    def get_fig_static(figpolicy, figname='', suffix=None, **kwargs):
+        exist = True if figname in plt.get_figlabels() else False
+        if figpolicy is FigurePolicy.same: return plt.figure(num=figname, **kwargs)
+        elif figpolicy is FigurePolicy.add_new: return plt.figure(num=(timestamp(name=figname) if suffix is None else figname + suffix) if exist else figname, **kwargs)
+        elif figpolicy is FigurePolicy.close_create_new: plt.close(figname) if exist else None; return plt.figure(num=figname, **kwargs)
+    @staticmethod
+    def try_figure_size():
+        fig, ax = plt.subplots()
+        y = np.sin(x := np.arange(0, 100, 0.01)) * 100
+        ax.plot(x, y); ax.axis("square"); ax.set_xlim(0, 100); ax.set_ylim(-100, 100)
+        FigureManager.set_ax_to_real_life_size(ax); fig.savefig(P.tmp() / "trial.png", dpi=250)
+    @staticmethod
+    def write(txt, name="text", size=8, **kwargs):
+        FigureManager.maximize_fig(fig := plt.figure(figsize=(11.69, 8.27), num=name))
+        fig.clf(); fig.text(0.5, 0.5, txt, transform=fig.transFigure, size=size, ha="center", va='center', **kwargs); return fig
+    @staticmethod
+    def activate_latex(size=20):
+        plt.rc('xtick', labelsize=size); plt.rc('ytick', labelsize=size)
+        plt.rc('axes', titlesize=size); plt.rc('legend', fontsize=size / 1.5)  # rc('text', usetex=True)
+        plt.rcParams['text.usetex'] = True; plt.rc('font', **{'family': 'serif', 'serif': ['Computer Modern']})
+    @staticmethod
+    def set_linestyles_and_markers_and_colors(test=False):
+        from cycler import cycler; from matplotlib import lines
+        markers = list(lines.lineMarkers.keys())[:-4]  # ignore the None
+        linestyles = (list(lines.lineStyles.keys())[:-3] * 10)[:len(markers)]
+        colors = (plt.rcParams['axes.prop_cycle'].by_key()['color'] * 10)[:len(markers)]
+        default_cycler = (cycler(linestyle=linestyles) + cycler(marker=markers) + cycler(color=colors))
+        plt.rc('axes', prop_cycle=default_cycler)
+        if test: [plt.plot(aq + idx * 2) for idx, aq in enumerate(np.random.randn(10, 10))]
+
+
+class VisibilityViewer(FigureManager):  # This is used for browsing purpose, as opposed to saving.
+    artist = ['internal', 'external'][1]  # How is the data visualized? You need artist. The artist can either be internal, as in ImShow or passed externally (especially non image data)
+    parser = ['internal', 'external'][1]  # Data parsing: internal for loop to go through all the dataset passed. # Allows manual control over parsing. external for loop. It should have add method. # Manual control only takes place after the external loop is over. #TODO parallelize this.
+    stream = ['clear', 'accumulate', 'update'][1]  # Streaming (Refresh mechanism): * Clear the axis. (slowest, but easy on memory) * accumulate, using visibility to hide previous axes. (Fastest but memory intensive)  * The artist has an update method. (best)
+    """ This class works on hiding axes shown on a plot, so that a new plot can be drawn. Once the entire loop is finished, you can browse through the plots with the keyboard Animation linked to `animate`"""
+    def __init__(self, fig):  # Downside: slow if number of axes, lines, texts, etc. are too large. In that case, it is better to avoid this viewer and plot on the fly during animation.
+        super().__init__(); self.objs_repo = []  # list of lists of axes and texts.
+        self.fig = fig; self.connect(); self.idx_cycle = Cycle([])
+    def add(self, objs): self.idx_cycle.expand(); self.objs_repo.append(objs); [obj.set_visible(False) for obj in (self.objs_repo[-2] if len(self.objs_repo) > 1 else [])]; print(f"VViewer added plot number {self.idx_cycle.get_index()}", end='\r')
+    def animate(self): [ax.set_visible(False) for ax in self.objs_repo[self.idx_cycle.prev_index]]; [ax.set_visible(True) for ax in self.objs_repo[self.idx_cycle.get_index()]]; self.fig.canvas.draw()
+
+
+class Artist(FigureManager):  # This object knows how to draw a figure from curve-type data.
+    def __init__(self, ax=None, figname='Graph', title='', label='curve', style='seaborn', figpolicy=FigurePolicy.add_new, figsize=(14, 8)):
+        super().__init__(figpolicy=figpolicy)
+        self.style, self.title = style, title; self.line = self.cursor = self.check_b = None
+        if ax is None:  # create a figure
+            with plt.style.context(style=self.style): self.fig = self.get_fig(figname, figsize=figsize); self.ax = self.fig.subplots()
+        else: self.ax = ax; self.fig = ax.figure  # use the passed axis
+        self.visibility_ax, self.txt, self.label = [0.01, 0.05, 0.2, 0.15], [], label
+    def plot(self, *args, legends=None, title=None, **kwargs): self.line = self.ax.plot(*args, **kwargs); self.ax.legend(legends or []); self.ax.set_title(title) if title is not None else None; self.ax.grid('on')
+    def plot_dict(self, adict, title='', xlabel='', ylabel=''): [self.plot(val, label=key) for key, val in adict.items()]; self.ax.legend(); self.ax.set_title(title); self.ax.set_xlabel(xlabel); self.ax.set_ylabel(ylabel); return self
+    def plot_twin(self, c1, c2, x=None, l1='', l2='', ax=None): ax = ax or self.ax; twin_ax = ax.twinx(); line1 = ax.plot(x or range(len(c1)), c1, color="blue", label=l1)[0]; line2 = twin_ax.plot(c2, color="red", label=l2)[0]; twin_ax.legend([line1, line2], [l1, l2]); ax.set_ylabel(l1); twin_ax.set_ylabel(l2); plt.show()
+    def suptitle(self, title): self.txt = [self.fig.text(0.5, 0.98, title, ha='center', va='center', size=9)]
+    def clear(self): self.fig.clf()  # objects that use this class will demand that the artist expose this method, in addition to .plot()
+    def axes(self): return [self.ax]  # objects that use this class will demand that the artist expose this method, in addition to .plot()
+    def visibility(self):
+        from matplotlib.widgets import CheckButtons; self.fig.subplots_adjust(left=0.3); self.visibility_ax[-1] = 0.05 * len(self.ax.lines)
+        rax = self.fig.add_axes(self.visibility_ax)
+        labels, visibility = [str(line.get_label()) for line in self.ax.lines], [line.get_visible() for line in self.ax.lines]
+        self.check_b = CheckButtons(rax, labels, visibility)
+        def func(label): index = labels.index(label); self.ax.lines[index].set_visible(not self.ax.lines[index].get_visible()); self.fig.canvas.draw()
+        self.check_b.on_clicked(func)
+    @staticmethod
+    def styler(plot_gen):
+        for astyle in plt.style.available:
+            with plt.style.context(style=astyle): plot_gen(); plt.title(astyle); plt.pause(1); plt.cla()
+
+
+class VisibilityViewerAuto(VisibilityViewer):
+    artist = ['internal', 'external'][1]
+    parser = ['internal', 'external'][0]
+    stream = ['clear', 'accumulate', 'update'][0:2]
+    def __init__(self, data=None, artist=None, stream='clear', save_type=FigureSave.Null, save_dir=None, save_name=None, delay=1,
+                 titles=None, legends=None, x_labels=None, pause=True, **kwargs):
+        """data: tensor of form  NumInputsForAnimation x ArgsPerPlot (to be unstarred) x Input (possible points x signals)
+        stream: ensure that behaviour of artist is consistent with stream. When `cccumulate`, artist should create new axes whenever plot is called."""
+        self.data = data; self.artist = artist or Artist()
+        self.legends = [f"Plot {i}" for i in range(len(self.data))] if legends is None else legends; self.titles = titles if titles is not None else np.arange(len(self.data))
+        super().__init__(fig=self.artist.fig); _ = kwargs
+        self.saver = save_type(watch_figs=[self.artist.fig], save_dir=save_dir, save_name=save_name, delay=delay, fps=1000 / delay)
+        self.index_max, self.pause, self.stream, self.lables = len(self.data), pause, stream, x_labels
+    test = staticmethod(lambda: VisibilityViewerAuto(data=np.random.randn(10, 1, 10, 3)))
+    def animate(self):
+        for i in range(0, self.index_max):
+            self.artist.plot(*self.data[i], title=self.titles[i], legends=self.legends)  # replot the new data point on a new axis.
+            super().add(self.artist.axes()) if self.stream == 'accumulate' else self.artist.clear()
+            self.saver.add()
+            if self.pause: break
+            else: self.idx_cycle.set_index(i)
+        return self.saver.finish()  # arrived at last image and not in manual mode
+
+
+class ImShow(FigureManager):
+    artist = ['internal', 'external'][0]
+    parser = ['internal', 'external'][0]
+    stream = ['clear', 'accumulate', 'update'][2]
+    def __init__(self, img_tensor, sup_titles=None, sub_labels=None, save_type=FigureSave.Null, save_name=None, save_dir=None, save_kwargs=None,
+                 subplots_adjust=None, gridspec=None, tight=True, info_loc=None, nrows=None, ncols=None, ax=None,
+                 figsize=None, figname='im_show', auto_brightness=True, delay=200, pause=False, **kwargs):
+        """
+        :param img_tensor: size N x M x W x H [x C]  # M used spatially, N for animation.
+        :param sup_titles: Titles for frames (N)
+        :param sub_labels: M x N. If shape sent is M
+        """
+        n, m = len(img_tensor), len(img_tensor[0]); self.m, self.n = m, n; super(ImShow, self).__init__(info_loc=info_loc)
+        nrows, ncols = self.get_nrows_ncols(m, nrows, ncols)
+        self.img_tensor, self.sub_labels, self.sup_titles = img_tensor, sub_labels if sub_labels is not None else [[f"{i}-{j}" for j in range(m)] for i in range(n)], sup_titles if sup_titles is not None else np.arange(n)
+        self.pause, self.kwargs, self.delay, self.auto_brightness = pause, kwargs, delay, auto_brightness
+        self.fname = self.event = None; self.ims = []  # container for images.
+        self.cmaps = Cycle(plt.colormaps()); self.cmaps.set_value('viridis')
+        if ax is None:
+            self.fig = self.get_fig(figname=figname, figsize=(14, 9) if figsize is None else figsize, facecolor='white'); self.maximize_fig() if figsize is None else None
+            if gridspec is not None: gs = self.fig.add_gridspec(gridspec[0]); self.ax = [self.fig.add_subplot(gs[ags[0], ags[1]]) for ags in gs[1:]]
+            else: self.ax = self.fig.subplots(nrows=nrows, ncols=ncols)
+        else: self.ax = ax; self.fig = ax[0].figure if type(ax) is list else ax.figure
+        self.connect(); self.fig.canvas.mpl_connect("pick_event", self.annotate)
+        self.fig.tight_layout() if tight else None; self.fig.subplots_adjust(**subplots_adjust) if subplots_adjust is not None else None
+        self.saver = save_type(watch_figs=[self.fig], save_dir=save_dir, save_name=save_name, delay=delay, fps=1000 / delay, **({} if save_kwargs is None else save_kwargs))
+        self.ax = [self.ax] if nrows == 1 and ncols == 1 else self.ax.ravel()  # make a list out of it or # make a 1D  list out of a 2D array.
+        [self.toggle_ticks(an_ax, state=False) for an_ax in self.ax]; self.idx_cycle = Cycle(max_idx=len(self.img_tensor))  # self.animate()
+    def animate(self):
+        for i in range(self.idx_cycle.get_index(), self.n):
+            for j, (an_image, a_label, an_ax) in enumerate(zip(self.img_tensor[i], self.sub_labels[i], self.ax)):  # with zipping, the shortest of the three, will stop the loop.
+                if i == 0 and self.ims.__len__() < self.m: self.ims.append(an_ax.imshow(an_image, animated=True, **self.kwargs))
+                else: self.ims[j].set_data(an_image)
+                if self.auto_brightness: self.ims[j].norm.autoscale(an_image)
+                an_ax.set_xlabel(f'{a_label}')
+            self.fig.suptitle(self.sup_titles[i], fontsize=8); self.saver.add(names=[self.sup_titles[i]])
+            if self.pause: break
+            else: self.idx_cycle.set_index(i)
+        if self.idx_cycle.get_index() == self.n - 1 and not self.pause: self.fname = self.saver.finish()  # arrived at last image and not in manual mode
+    @staticmethod
+    def try_cmaps(im, nrows=3, ncols=7, **kwargs): _ = ImShow(*np.array_split([plt.get_cmap(style)(im) for style in plt.colormaps()], nrows * ncols), nrows=nrows, ncols=ncols, sub_labels=np.array_split(plt.colormaps(), nrows * ncols), **kwargs); return [plt.get_cmap(style)(im) for style in plt.colormaps()]
+    def annotate(self, event, axis=None, data=None): [super().annotate(event, axis=ax, data=ax.images[0].get_array()) for ax in self.ax]
+    from_img_paths = staticmethod(lambda paths, **kwargs: ImShow(List(paths).apply(plt.imread), sub_labels=List(paths).apply(lambda x: P(x).stem), **kwargs))
+    from_complex = staticmethod(lambda data, pause=True, **kwargs: ImShow(data.real, data.imag, np.angle(data), abs(data), labels=['Real Part', 'Imaginary Part', 'Angle in Radians', 'Absolute Value'], pause=pause, **kwargs))
+    test = staticmethod(lambda: ImShow(np.random.rand(12, 10, 80, 120, 3)))  # https://ai.googleblog.com/2019/08/turbo-improved-rainbow-colormap-for.html # https://gist.github.com/mikhailov-work/ee72ba4191942acecc03fe6da94fc73f
+    resize = staticmethod(lambda path, m, n: plt.imsave(path, install_n_import(package="skimage", name="scikit-image").transform.resize(plt.imread(path), (m, n), anti_aliasing=True)))
+
+
+if __name__ == '__main__':
+    pass
```

### Comparing `crocodile-8.40/myresources/crocodile/meta.py` & `crocodile-9.0/myresources/crocodile/meta.py`

 * *Ordering differences only*

 * *Files 5% similar despite different names*

```diff
@@ -1,275 +1,275 @@
-
-from crocodile.core import timestamp, randstr, str2timedelta, Save, install_n_import, List, Struct
-from crocodile.file_management import P, datetime
-import time
-import logging
-import subprocess
-import sys
-
-
-class Null:
-    def __init__(self, return_='self'): self.return_ = return_
-    def __getattr__(self, item) -> 'Null': _ = item; return self if self.return_ == 'self' else self.return_
-    def __getitem__(self, item) -> 'Null': _ = item; return self if self.return_ == 'self' else self.return_
-    def __call__(self, *args, **kwargs) -> 'Null': return self if self.return_ == 'self' else self.return_
-    def __len__(self): return 0
-    def __bool__(self): return False
-    def __contains__(self, item): _ = self, item; return False
-    def __iter__(self): return iter([self])
-
-
-class Log(logging.Logger):  #
-    def __init__(self, dialect=["colorlog", "logging", "coloredlogs"][0], name=None, file: bool = False, file_path=None, stream=True, fmt=None, sep=" | ",
-                 s_level=logging.DEBUG, f_level=logging.DEBUG, l_level=logging.DEBUG, verbose=False, log_colors=None):
-        super().__init__(name := randstr() if name is None and not print(f"Logger name not passed. It is recommended to pass a name indicating the owner.") else name, level=l_level)  # logs everything, finer level of control is given to its handlers
-        print(f"Logger `{name}` from `{dialect}` is instantiated with level {l_level}."); self.file_path = file_path  # proper update to this value by self.add_filehandler()
-        if dialect == "colorlog": module = install_n_import("colorlog"); processed_fmt = module.ColoredFormatter(fmt or (rf"%(log_color)s" + Log.get_format(sep)), datefmt="%d %H:%M:%S", log_colors=log_colors or {'DEBUG': 'bold_cyan', 'INFO': 'green', 'WARNING': 'yellow', 'ERROR': 'thin_red', 'CRITICAL': 'fg_bold_red,bg_black', })  # see here for format: https://pypi.org/project/colorlog/
-        else: module = logging; processed_fmt = logging.Formatter(fmt or Log.get_format(sep, datefmt="%d %H:%M:%S"))
-        self.add_filehandler(file_path=file_path, fmt=processed_fmt, f_level=f_level) if file or file_path else None; self.add_streamhandler(s_level, fmt=processed_fmt, module=module) if stream else None
-        self.specs = dict(dialect=dialect, name=self.name, file=file, file_path=self.file_path, stream=bool(self.get_shandler()), fmt=fmt, sep=sep, s_level=s_level, f_level=f_level, l_level=l_level, verbose=verbose, log_colors=log_colors)  # # this way of creating relative path makes transferrable across machines.
-    def get_shandler(self): return List(handler for handler in self.handlers if "StreamHandler" in str(handler))
-    def get_fhandler(self): return List(handler for handler in self.handlers if "FileHandler" in str(handler))
-    def set_level(self, level, which=["logger", "stream", "file", "all"][0]): self.setLevel(level) if which in {"logger", "all"} else None; self.get_shandler().setLevel(level) if which in {"stream", "all"} else None; self.get_fhandler().setLevel(level) if which in {"file", "all"} else None
-    def __reduce_ex__(self, protocol): _ = protocol; return self.__class__, tuple(self.specs.values())  # reduce_ex is enchanced reduce. Its lower than getstate and setstate. It uses init method to create an instance.
-    def __repr__(self): return "".join([f"Logger {self.name} (level {self.level}) with handlers: \n"] + [repr(h) + f"" + "\n" for h in self.handlers])
-    get_format = staticmethod(lambda sep=' | ': f"%(asctime)s{sep}%(name)s{sep}%(module)s{sep}%(funcName)s{sep}%(levelname)s(%(levelno)s){sep}%(message)s{sep}")  # Reference: https://docs.python.org/3/library/logging.html#logrecord-attributes logging.BASIC_FORMAT
-    def manual_degug(self, path): _ = self; sys.stdout = open(path, 'w'); sys.stdout.close(); print(f"Finished ... have a look @ \n {path}")  # all print statements will write to this file.
-    @staticmethod
-    def get_coloredlogs(name=None, file=False, file_path=None, stream=True, fmt=None, sep=" | ", s_level=logging.DEBUG, f_level=logging.DEBUG, l_level=logging.DEBUG, verbose=False):
-        level_styles = {'spam': {'color': 'green', 'faint': True}, 'debug': {'color': 'white'}, 'verbose': {'color': 'blue'}, 'info': {'color': "green"}, 'notice': {'color': 'magenta'}, 'warning': {'color': 'yellow'}, 'success': {'color': 'green', 'bold': True},
-                        'error': {'color': 'red', "faint": True, "underline": True}, 'critical': {'color': 'red', 'bold': True, "inverse": False}}  # https://coloredlogs.readthedocs.io/en/latest/api.html#available-text-styles-and-colors
-        field_styles = {'asctime': {'color': 'green'}, 'hostname': {'color': 'magenta'}, 'levelname': {'color': 'black', 'bold': True}, 'path': {'color': 'blue'}, 'programname': {'color': 'cyan'}, 'username': {'color': 'yellow'}}
-        if verbose: logger = install_n_import("verboselogs").VerboseLogger(name=name); logger.setLevel(l_level)  # https://github.com/xolox/python-verboselogs # verboselogs.install()  # hooks into logging module.
-        else: logger = Log(name=name, dialect="logging", l_level=l_level, file=file, f_level=f_level, file_path=file_path, fmt=fmt or Log.get_format(sep), stream=stream, s_level=s_level)  # new step, not tested:
-        install_n_import("coloredlogs").install(logger=logger, name="lol_different_name", level=logging.NOTSET, level_styles=level_styles, field_styles=field_styles, fmt=fmt or Log.get_format(sep), isatty=True, milliseconds=True); return logger
-    def add_streamhandler(self, s_level=logging.DEBUG, fmt=None, module=logging, name="myStreamHandler"):
-        shandler = module.StreamHandler(); shandler.setLevel(level=s_level); shandler.setFormatter(fmt=fmt); shandler.set_name(name); self.addHandler(shandler); print(f"    Level {s_level} stream handler for Logger `{self.name}` is created.")
-    def add_filehandler(self, file_path=None, fmt=None, f_level=logging.DEBUG, mode="a", name="myFileHandler"):
-        fhandler = logging.FileHandler(filename := (P.tmpfile(name="logger_" + self.name, suffix=".log", folder="tmp_loggers") if file_path is None else P(file_path).expanduser()), mode=mode)
-        fhandler.setFormatter(fmt=fmt); fhandler.setLevel(level=f_level); fhandler.set_name(name); self.addHandler(fhandler); self.file_path = filename.collapseuser(); print(f"    Level {f_level} file handler for Logger `{self.name}` is created @ " + P(filename).clickable())
-    def test(self): List([self.debug, self.info, self.warning, self.error, self.critical]).apply(lambda func: func(f"this is a {func.__name__} message")); [self.log(msg=f"This is a message of level {level}", level=level) for level in range(0, 60, 5)]
-    def get_history(self, lines=200, to_html=False): logs = "\n".join(self.file_path.expanduser().absolute().read_text().split("\n")[-lines:]); return install_n_import("ansi2html").Ansi2HTMLConverter().convert(logs) if to_html else logs
-
-
-class Terminal:
-    class Response:
-        @staticmethod
-        def from_completed_process(cp: subprocess.CompletedProcess): (resp := Terminal.Response(cmd=cp.args)).output.update(dict(stdout=cp.stdout, stderr=cp.stderr, returncode=cp.returncode)); return resp
-        def __init__(self, stdin=None, stdout=None, stderr=None, cmd=None, desc=""): self.std, self.output, self.input, self.desc = dict(stdin=stdin, stdout=stdout, stderr=stderr), dict(stdin="", stdout="", stderr="", returncode=None), cmd, desc  # input command
-        def __call__(self, *args, **kwargs): return self.op.rstrip() if type(self.op) is str else None
-        op = property(lambda self: self.output["stdout"])
-        ip = property(lambda self: self.output["stdin"])
-        err = property(lambda self: self.output["stderr"])
-        returncode = property(lambda self: self.output["returncode"])
-        def op2path(self, strict_returncode=True, strict_err=False) -> P or None:
-            return P(self.op.rstrip()) if self.is_successful(strict_returcode=strict_returncode, strict_err=strict_err) else None
-        def op_if_successfull_or_default(self, strict_returcode=True, strict_err=False, default=None): return self.op if self.is_successful(strict_returcode=strict_returcode, strict_err=strict_err) else default
-        def is_successful(self, strict_returcode=True, strict_err=False): return ((self.output["returncode"] in {0, None}) if strict_returcode else True) and (self.err == "" if strict_err else True)
-        def capture(self): [self.output.__setitem__(key, val.read().decode().rstrip()) for key, val in self.std.items() if val is not None and val.readable()]; return self
-        def print(self, desc="TERMINAL CMD", capture=True):
-            self.capture() if capture else None; install_n_import("rich"); from rich import console; con = console.Console(); from rich.panel import Panel; from rich.text import Text  # from rich.syntax import Syntax; syntax = Syntax(my_code, "python", theme="monokai", line_numbers=True)
-            tmp1 = Text("Input Command:\n"); tmp1.stylize("u bold blue"); tmp2 = Text("\nTerminal Response:\n"); tmp2.stylize("u bold blue")
-            txt = tmp1 + Text(str(self.input), style="white") + tmp2 + Text("\n".join([f"{f' {idx} - {key} '}".center(40, "-") + f"\n{val}" for idx, (key, val) in enumerate(self.output.items())]), style="white")
-            con.print(Panel(txt, title=self.desc, subtitle=desc, width=150, style="bold cyan on black")); return self
-    def __init__(self, stdout=subprocess.PIPE, stderr=subprocess.PIPE, stdin=subprocess.PIPE, elevated=False):
-        self.available_consoles, self.machine = ["cmd", "Command Prompt", "wt", "powershell", "wsl", "ubuntu", "pwsh"], __import__("platform").system()
-        self.elevated, self.stdout, self.stderr, self.stdin = elevated, stdout, stderr, stdin
-    def set_std_system(self): self.stdout = sys.stdout; self.stderr = sys.stderr; self.stdin = sys.stdin
-    def set_std_pipe(self): self.stdout = subprocess.PIPE; self.stderr = subprocess.PIPE; self.stdin = subprocess.PIPE
-    def set_std_null(self): self.stdout, self.stderr, self.stdin = subprocess.DEVNULL, subprocess.DEVNULL, subprocess.DEVNULL  # Equivalent to `echo 'foo' &> /dev/null`
-    def run(self, *cmds, shell=None, check=False, ip=None):  # Runs SYSTEM commands like subprocess.run
-        """Blocking operation. Thus, if you start a shell via this method, it will run in the main and won't stop until you exit manually IF stdin is set to sys.stdin, otherwise it will run and close quickly. Other combinations of stdin, stdout can lead to funny behaviour like no output but accept input or opposite.
-        * This method is short for: res = subprocess.run("powershell command", capture_output=True, shell=True, text=True) and unlike os.system(cmd), subprocess.run(cmd) gives much more control over the output and input.
-        * `shell=True` loads up the profile of the shell called so more specific commands can be run. Importantly, on Windows, the `start` command becomes availalbe and new windows can be launched.
-        * `capture_output` prevents the stdout to redirect to the stdout of the script automatically, instead it will be stored in the Response object returned. # `capture_output=True` same as `stdout=subprocess.PIPE, stderr=subprocess.PIPE`"""
-        my_list = list(cmds)  # `subprocess.Popen` (process open) is the most general command. Used here to create asynchronous job. `subprocess.run` is a thin wrapper around Popen that makes it wait until it finishes the task. `suprocess.call` is an archaic command for pre-Python-3.5.
-        if self.machine == "Windows" and shell in {"powershell", "pwsh"}: my_list = [shell, "-Command"] + my_list  # alternatively, one can run "cmd"
-        if self.elevated is False or self.is_user_admin(): resp = subprocess.run(my_list, stderr=self.stderr, stdin=self.stdin, stdout=self.stdout, text=True, shell=True, check=check, input=ip)
-        else: resp = __import__("ctypes").windll.shell32.ShellExecuteW(None, "runas", sys.executable, " ".join(sys.argv), None, 1)
-        return self.Response.from_completed_process(resp)
-    @staticmethod
-    def is_user_admin() -> bool:  # adopted from: https://stackoverflow.com/questions/19672352/how-to-run-script-with-elevated-privilege-on-windows"""
-        if __import__('os').name == 'nt':
-            try: return __import__("ctypes").windll.shell32.IsUserAnAdmin()
-            except: import traceback; traceback.print_exc(); print("Admin check failed, assuming not an admin."); return False
-        else: return __import__('os').getuid() == 0  # Check for root on Posix
-    @staticmethod
-    def run_as_admin(file, params, wait=False): proce_info = install_n_import("win32com", fromlist=["shell.shell.ShellExecuteEx"]).shell.shell.ShellExecuteEx(lpVerb='runas', lpFile=file, lpParameters=params); time.sleep(wait) if wait is not False and wait is not True else None; return proce_info
-    def run_async(self, *cmds, new_window=True, shell=None, terminal=None):  # Runs SYSTEM commands like subprocess.Popen
-        """Opens a new terminal, and let it run asynchronously. Maintaining an ongoing conversation with another process is very hard. It is adviseable to run all
-        commands in one go without interaction with an ongoing channel. Use this only for the purpose of producing a different window and humanly interact with it. Reference: https://stackoverflow.com/questions/54060274/dynamic-communication-between-main-and-subprocess-in-python & https://www.youtube.com/watch?v=IynV6Y80vws and https://www.oreilly.com/library/view/windows-powershell-cookbook/9781449359195/ch01.html"""
-        if terminal is None: terminal = ""  # this means that cmd is the default console. alternative is "wt"
-        if shell is None: shell = "" if self.machine == "Windows" else ""  # other options are "powershell" and "cmd". # if terminal is wt, then it will pick powershell by default anyway.
-        new_window = "start" if new_window is True else ""  # start is alias for Start-Process which launches a new window.  adding `start` to the begining of the command results in launching a new console that will not inherit from the console python was launched from e.g. conda
-        extra, my_list = ("-Command" if shell in {"powershell", "pwsh"} else ""), list(cmds)
-        if self.machine == "Windows": my_list = [new_window, terminal, shell, extra] + my_list  # having a list is equivalent to: start "ipython -i file.py". Thus, arguments of ipython go to ipython, not start.
-        print("Meta.Terminal.run_async: Subprocess command: ", my_list := [item for item in my_list if item != ""])
-        return subprocess.Popen(my_list, stdin=subprocess.PIPE, shell=True)  # stdout=self.stdout, stderr=self.stderr, stdin=self.stdin. # returns Popen object, not so useful for communcation with an opened terminal
-    @staticmethod
-    def run_py(script, wdir=None, interactive=True, ipython=True, shell=None, delete=False, terminal="", new_window=True, header=True):  # async run, since sync run is meaningless.
-        script = ((Terminal.get_header(wdir=wdir) if header else "") + script) + ("\ntb.DisplayData.set_pandas_auto_width()\n" if terminal in {"wt", "powershell", "pwsh"} else "")
-        file = P.tmpfile(name="tmp_python_script", suffix=".py", folder="tmp_scripts").write_text(f"""print(r'''{script}''')""" + "\n" + script); print(f"Script to be executed asyncronously: ", file.absolute().as_uri())
-        Terminal().run_async(f"{'ipython' if ipython else 'python'}", f"{'-i' if interactive else ''}", f"{file}", terminal=terminal, shell=shell, new_window=new_window)  # python will use the same dir as the one from console this method is called.
-        _ = delete  # we need to ensure that async process finished reading before deleteing: file.delete(sure=delete, verbose=False)
-    pickle_to_new_session = staticmethod(lambda obj, cmd="": Terminal.run_py(f"""path = tb.P(r'{Save.pickle(obj=obj, path=P.tmpfile(tstamp=False, suffix=".pkl"), verbose=False)}')\n obj = path.readit()\npath.delete(sure=True, verbose=False)\n {cmd}"""))
-    @staticmethod
-    def import_to_new_session(func=None, cmd="", header=True, interactive=True, ipython=True, **kwargs):
-        load_kwargs_string = f"""loaded_kwargs = tb.P(r'{Save.pickle(obj=kwargs, path=P.tmpfile(tstamp=False, suffix=".pkl"), verbose=False)}').readit()\nloaded_kwargs.print()\nobj(**loaded_kwargs)""" if kwargs is not {} else ""
-        if callable(func) and func.__name__ != func.__qualname__:  # it is a method of a class, must be instantiated first.
-            module = P(sys.modules['__main__'].__file__).rel2cwd().stem if (module := func.__module__) == "__main__" else module
-            load_func_string = f"import {module} as m\ninst=m.{func.__qualname__.split('.')[0]}()\nobj = inst.{func.__name__}" + f"\n{cmd}\n{load_kwargs_string}\n"
-        elif callable(func) and hasattr(func, "__code__"):  # it is a standalone function...
-            module = P(func.__code__.co_filename)  # module = func.__module__  # fails if the function comes from main as it returns __main__.
-            load_func_string = f"tb.sys.path.insert(0, r'{module.parent}')\nimport {module.stem} as m\nobj=m.{func.__name__}" + f"\n{cmd}\n{load_kwargs_string}\n"
-        else: load_func_string = f"""obj = tb.P(r'{Save.pickle(obj=func, path=P.tmpfile(tstamp=False, suffix=".pkl"), verbose=False)}').readit()"""
-        return Terminal.run_py(load_func_string, header=header, interactive=interactive, ipython=ipython)  # Terminal().run_async("python", "-c", load_func_string + f"\n{cmd}\n{load_kwargs_string}\n")
-    @staticmethod
-    def replicate_session(cmd=""): __import__("dill").dump_session(file := P.tmpfile(suffix=".pkl"), main=sys.modules[__name__]); Terminal().run_py(script=f"""path = tb.P(r'{file}')\nimport dill\nsess= dill.load_session(str(path))\npath.delete(sure=True, verbose=False)\n{cmd}""")
-    @staticmethod
-    def get_header(wdir=None): return f"""\n# >> Code prepended\nimport crocodile.toolbox as tb""" + (f"""\ntb.sys.path.insert(0, r'{wdir}')""" if wdir is not None else '') + f"""\n# >> End of header, start of script passed\n"""
-
-
-class SSH:  # inferior alternative: https://github.com/fabric/fabric
-    def __init__(self, username=None, hostname=None, host=None, tmate_sess=None, sshkey=None, pwd=None, port=22, ve="ve", compress=False):  # https://stackoverflow.com/questions/51027192/execute-command-script-using-different-shell-in-ssh-paramiko
-        username, self.host, self.tmate_sess, self.compress, self.pwd, self.ve = username or __import__("getpass").getuser(), None, tmate_sess, compress, pwd, ve  # Defaults: (1) use localhost if nothing provided.
-        if "@" not in username and hostname is None:  # then, username is probably a Host profile
-            try:
-                config = __import__("paramiko.config").config.SSHConfig.from_path(P.home().joinpath(".ssh/config").str); config_dict = config.lookup(host or username)
-                self.hostname, self.username, self.host, port, sshkey = config_dict["hostname"], config_dict["user"], host or username, config_dict.get("port", port), tmp[0] if type(tmp := config_dict.get("identityfile", sshkey)) is list else tmp
-                if sshkey is not None: sshkey = tmp[0] if type(tmp := config.lookup("*").get("identityfile", sshkey)) is list else tmp
-            except (FileNotFoundError, KeyError): self.hostname, self.username = __import__("platform").node(), username
-        else: self.username, self.hostname = username.split("@") if "@" in username else (username, hostname)
-        self.hostname, self.port = self.hostname.split(":") if ":" in self.hostname else (self.hostname, port); self.port = int(self.port)
-        self.sshkey = str(P(sshkey).expanduser().absolute()) if sshkey is not None else None  # no need to pass sshkey if it was configured properly already
-        self.ssh = (paramiko := __import__("paramiko")).SSHClient(); self.ssh.load_system_host_keys(); self.ssh.set_missing_host_key_policy(paramiko.AutoAddPolicy())
-        install_n_import("rich").inspect(Struct(hostname=self.hostname, username=self.username, password="***", port=self.port, key_filename=self.sshkey), value=False, title="SSHing To", docs=False, sort=False)
-        self.ssh.connect(hostname=self.hostname, username=self.username, password=self.pwd, port=self.port, key_filename=self.sshkey, compress=self.compress)
-        try: self.sftp = self.ssh.open_sftp()
-        except Exception as err: self.sftp = None; print(f"WARNING: could not open SFTP connection to {hostname}. No data transfer is possible. Erorr faced: `{err}`")
-        def view_bar(slf, a, b): slf.total = int(b); slf.update(int(a - slf.n))  # update pbar with increment
-        self.tqdm_wrap = type('TqdmWrap', (install_n_import("tqdm").tqdm,), {'view_bar': view_bar})
-        self._local_distro, self._remote_distro, self._remote_machine, self.terminal_responses, self.platform = None, None, None, [], __import__("platform")
-        self.remote_env_cmd = rf"""~/venvs/{self.ve}/Scripts/Activate.ps1""" if self.get_remote_machine() == "Windows" else rf"""source ~/venvs/{self.ve}/bin/activate"""
-        self.local_env_cmd = rf"""~/venvs/{self.ve}/Scripts/Activate.ps1""" if self.platform.system() == "Windows" else rf"""source ~/venvs/{self.ve}/bin/activate"""  # works for both cmd and pwsh
-    def __getstate__(self): return {attr: self.__getattribute__(attr) for attr in ["username", "hostname", "host", "tmate_sess", "port", "sshkey", "compress", "pwd", "ve"]}
-    def __setstate__(self, state): self.__init__(**state)
-    def get_remote_machine(self): self._remote_machine = ("Windows" if (self.run("$env:OS", verbose=False, desc="Testing OS").capture().op == "Windows_NT" or self.run("echo %OS%", verbose=False, desc="Testing OS").capture().op == "Windows_NT") else "Linux") if self._remote_machine is None else self._remote_machine; return self._remote_machine  # echo %OS% TODO: uname on linux
-    def get_local_distro(self): self._local_distro = install_n_import("distro").name(pretty=True) if self._local_distro is None else self._local_distro; return self._local_distro
-    def get_remote_distro(self): self._remote_distro = self.run_py("print(tb.install_n_import('distro').name(pretty=True))", verbose=False).capture().op_if_successfull_or_default(default="") if self._remote_distro is None else self._remote_distro; return self._remote_distro
-    def restart_computer(self): self.run("Restart-Computer -Force" if self.get_remote_machine() == "Windows" else "sudo reboot")
-    def send_ssh_key(self): self.copy_from_here("~/.ssh/id_rsa.pub"); assert self.get_remote_machine() == "Windows"; self.run(P(install_n_import("machineconfig").scripts.windows.__path__.__dict__["_path"][0]).joinpath("openssh_server_add_sshkey.ps1").read_text())
-    def copy_env_var(self, name): assert self.get_remote_machine() == "Linux"; return self.run(f"{name} = {__import__('os').environ[name]}; export {name}")
-    def get_repr(self, which="remote", add_machine=False): return (f"{self.username}@{self.hostname}:{self.port}" + (f" [{self.get_remote_machine()}][{self.get_remote_distro()}]" if add_machine else "")) if which == "remote" else f"{__import__('getpass').getuser()}@{self.platform.node()}" + (f" [{self.platform.system()}][{self.get_local_distro()}]" if add_machine else "")
-    def __repr__(self): return f"local {self.get_repr('local', add_machine=True)} >>> SSH TO >>> remote {self.get_repr('remote', add_machine=True)}"
-    def run_locally(self, command): print(f"Executing Locally @ {self.platform.node()}:\n{command}"); return Terminal.Response(__import__('os').system(command))
-    def get_ssh_conn_str(self, cmd=""): return f"ssh" + (f" -i {self.sshkey}" if self.sshkey else "") + (f' -t {cmd} ' if cmd != '' else ' ') + self.get_repr('remote').replace(':', ' -p ')
-    def open_console(self, cmd='', new_window=True, terminal=None): Terminal().run_async(*self.get_ssh_conn_str().split(" "), cmd, new_window=new_window, terminal=terminal)
-    def run(self, cmd, verbose=True, desc="", strict_err=False, strict_returncode=False, env_prefix=False) -> Terminal.Response:  # most central method.
-        cmd = (self.remote_env_cmd + "; " + cmd) if env_prefix else cmd; res = Terminal.Response(stdin=(raw := self.ssh.exec_command(cmd))[0], stdout=raw[1], stderr=raw[2], cmd=cmd, desc=desc)
-        if strict_err or strict_returncode: assert res.is_successful(strict_err=strict_err, strict_returcode=strict_returncode), res.print()
-        res.print() if verbose else None; self.terminal_responses.append(res); return res
-    def run_py(self, cmd, desc="", return_obj=False, verbose=True, strict_err=False, strict_returncode=False):
-        assert '"' not in cmd, f'Avoid using `"` in your command. I dont know how to handle this when passing is as command to python in pwsh command.'
-        if not return_obj: return self.run(f"""{self.remote_env_cmd}; python -c "{Terminal.get_header(wdir=None)}{cmd}\n""" + '"', desc=desc or f"run_py on {self.get_repr('remote')}", verbose=verbose, strict_err=strict_err, strict_returncode=strict_returncode)
-        else: assert "obj=" in cmd, f"The command sent to run_py must have `obj=` statement if return_obj is set to True"; source_file = self.run_py(f"""{cmd}\npath = tb.Save.pickle(obj=obj, path=tb.P.tmpfile(suffix='.pkl'))\nprint(path)""", desc=desc, verbose=verbose, strict_err=True, strict_returncode=True).op.split('\n')[-1]; return self.copy_to_here(source=source_file, target=P.tmpfile(suffix='.pkl')).readit()
-    def copy_from_here(self, source, target=None, z=False, r=False, overwrite=False) -> P or List[P]:
-        if not z and (source := P(source).expanduser()).is_dir(): return source.search("*", folders=False, r=True).apply(lambda file: self.copy_from_here(source=file, target=target)) if r is True else print(f"tb.Meta.SSH Error: source is a directory! either set r=True for recursive sending or raise zip_first flag.")
-        if z: print(f"ZIPPING ..."); source = P(source).expanduser().zip(content=True)  # .append(f"_{randstr()}", inplace=True)  # eventually, unzip will raise content flag, so this name doesn't matter.
-        if target is None: target = P(source).collapseuser(); assert target.is_relative_to("~"), f"If target is not specified, source must be relative to home."
-        remotepath = self.run_py(f"path=tb.P(r'{P(target).as_posix()}').expanduser()\n{'path.delete(sure=True)' if overwrite else ''}\nprint(path.parent.create())", desc=f"Creating Target directory `{P(target).parent.as_posix()}` @ {self.get_repr('remote')}").op or ''; remotepath = P(remotepath.split("\n")[-1]).joinpath(P(target).name)
-        print(f"SENDING `{repr(P(source))}` ==> `{remotepath.as_posix()}`")
-        with self.tqdm_wrap(ascii=True, unit='b', unit_scale=True) as pbar: self.sftp.put(localpath=P(source).expanduser(), remotepath=remotepath.as_posix(), callback=pbar.view_bar)
-        if z: resp = self.run_py(f"""tb.P(r'{remotepath.as_posix()}').expanduser().unzip(content=False, inplace=True, overwrite={overwrite})""", desc=f"UNZIPPING {remotepath.as_posix()}"); source.delete(sure=True); return resp
-    def copy_to_here(self, source, target=None, zip_first=False, r=False) -> P:
-        if not zip_first and self.run_py(f"print(tb.P(r'{source}').expanduser().is_dir())", desc="Check if source is a dir", verbose=True, strict_returncode=True, strict_err=True).op.split("\n")[-1] == 'True':
-            return self.run_py(f"obj=tb.P(r'{source}').search(folders=False, r=True).collapseuser()", desc="Searching for files in source", return_obj=True).apply(lambda file: self.copy_to_here(source=file.as_posix(), target=P(target).joinpath(P(file).relative_to(source)) if target else None, r=False)) if r else print(f"source is a directory! either set r=True for recursive sending or raise zip_first flag.")
-        if zip_first: source = self.run_py(f"print(tb.P(r'{source}').expanduser().zip(inplace=False, verbose=False))", desc=f"Zipping source file").op2path(strict_returncode=True, strict_err=True)
-        if target is None: target = self.run_py(f"print(tb.P(r'{P(source).as_posix()}').collapseuser())", desc=f"Finding default target via relative source path", strict_returncode=True, strict_err=True).op2path(); assert target.is_relative_to("~"), f"If target is not specified, source must be relative to home."
-        target = P(target).expanduser().create(parents_only=True); target += '.zip' if zip_first and '.zip' not in target.suffix else ''
-        source = self.run_py(f"print(tb.P(r'{source}').expanduser())", desc=f"# Resolving source path address by expanding user", strict_returncode=True, strict_err=True).op2path() if "~" in str(source) else P(source); print(f"RECEVING `{source}` ==> `{target}`")
-        with self.tqdm_wrap(ascii=True, unit='b', unit_scale=True) as pbar: self.sftp.get(remotepath=source.as_posix(), localpath=target.as_posix(), callback=pbar.view_bar)
-        if zip_first: target = target.unzip(inplace=True, content=True); self.run_py(f"tb.P(r'{source}').delete(sure=True)", desc="Cleaning temp files", strict_returncode=True, strict_err=True)
-        return target
-    def print_summary(self):   # ip=rsp.ip, op=rsp.op
-        install_n_import("tabulate"); df = __import__("pandas").DataFrame.from_records(List(self.terminal_responses).apply(lambda rsp: dict(desc=rsp.desc, err=rsp.err, returncode=rsp.returncode))); print("\nSummary of operations performed:"); print(df.to_markdown())
-        print("\nAll operations completed successfully.\n") if ((df['returncode'].to_list()[2:] == [None] * (len(df) - 2)) and (df['err'].to_list()[2:] == [''] * (len(df) - 2))) else print("\nSome operations failed. \n"); return df
-
-
-class Scheduler:
-    def __init__(self, routine=None, wait: str = "2m", other_routine=None, other_ratio: int = 10, max_cycles=float("inf"), exception_handler=None, logger: Log = None, sess_stats=None):
-        self.routine = (lambda sched: None) if routine is None else routine  # main routine to be repeated every `wait` time period
-        self.other_routine = (lambda sched: None) if other_routine is None else other_routine  # routine to be repeated every `other` time period
-        self.wait, self.other_ratio = str2timedelta(wait).total_seconds(), other_ratio  # wait period between routine cycles.
-        self.logger, self.exception_handler = logger if logger is not None else Log(name="SchedLogger_" + randstr(length=2)), exception_handler
-        self.sess_start_time, self.records, self.cycle, self.max_cycles, self.sess_stats = None, List([]), 0, max_cycles, sess_stats or (lambda sched: {})
-    def run(self, max_cycles=None, until="2050-01-01"):
-        self.max_cycles, self.cycle, self.sess_start_time = max_cycles or self.max_cycles, 0, datetime.now()
-        while datetime.now() < datetime.fromisoformat(until) and self.cycle < self.max_cycles:  # 1- Time before Ops, and Opening Message
-            time1 = datetime.now(); self.logger.warning(f"Starting Cycle {str(self.cycle).zfill(5)}. Total Run Time = {str(datetime.now() - self.sess_start_time)}. UTC {datetime.utcnow().strftime('%d %H:%M:%S')}")
-            try: self.routine(sched=self)
-            except BaseException as ex: self._handle_exceptions(ex=ex, during="routine")  # 2- Perform logic
-            if self.cycle % self.other_ratio == 0:
-                try: self.other_routine(sched=self)
-                except BaseException as ex: self._handle_exceptions(ex=ex, during="occasional")  # 3- Optional logic every while
-            time_left = int(self.wait - (datetime.now() - time1).total_seconds())  # 4- Conclude Message
-            self.cycle += 1; self.logger.warning(f"Finishing Cycle {str(self.cycle - 1).zfill(5)}. Sleeping for {self.wait}s ({time_left}s left)\n" + "-" * 100)
-            try: time.sleep(time_left if time_left > 0 else 0.1)  # # 5- Sleep. consider replacing by Asyncio.sleep
-            except KeyboardInterrupt as ex: self._handle_exceptions(ex, during="sleep")  # that's probably the only kind of exception that can rise during sleep.
-        else: self.record_session_end(reason=f"Reached maximum number of cycles ({self.max_cycles})" if self.cycle >= self.max_cycles else f"Reached due stop time ({until})"); return self
-    def get_records_df(self): return __import__("pandas").DataFrame.from_records(self.records, columns=["start", "finish", "duration", "cycles", "termination reason", "logfile"] + list(self.sess_stats(sched=self).keys()))
-    def record_session_end(self, reason="Not passed to function."):
-        self.records.append([self.sess_start_time, end_time := datetime.now(), duration := end_time-self.sess_start_time, self.cycle, reason, self.logger.file_path] + list((sess_stats := self.sess_stats(sched=self)).values()))
-        summ = {"start time": f"{str(self.sess_start_time)}", "finish time": f"{str(end_time)}.", "duration": f"{str(duration)} | wait time {self.wait}s", "cycles ran": f"{self.cycle} | Lifetime cycles = {self.get_records_df()['cycles'].sum()}", f"termination reason": reason, "logfile": self.logger.file_path}
-        self.logger.critical(f"\n--> Scheduler has finished running a session. \n" + Struct(summ).update(sess_stats).print(as_config=True, return_str=True, quotes=False) + "\n" + "-" * 100); self.logger.critical(f"\n--> Logger history.\n" + str(self.get_records_df())); return self
-    def _handle_exceptions(self, ex, during):
-        if self.exception_handler is not None: self.exception_handler(ex, during=during, sched=self)  # user decides on handling and continue, terminate, save checkpoint, etc.  # Use signal library.
-        else: self.record_session_end(reason=f"during {during}, " + str(ex)); self.logger.exception(ex); raise ex
-
-
-def try_this(func, return_=None, raise_=None, run=None, handle=None, verbose=False, **kwargs):
-    try: return func()
-    except BaseException as ex:  # or Exception
-        if verbose: print(ex)
-        if raise_ is not None: raise raise_
-        if handle is not None: return handle(ex, **kwargs)
-        return run() if run is not None else return_
-def show_globals(scope, **kwargs): return Struct(scope).filter(lambda k, v: "__" not in k and not k.startswith("_") and k not in {"In", "Out", "get_ipython", "quit", "exit", "sys"}).print(**kwargs)
-def monkey_patch(class_inst, func): setattr(class_inst.__class__, func.__name__, func)
-def capture_locals(func, scope, args=None, self: str = None, update_scope=True): res = dict(); exec(extract_code(func, args=args, self=self, include_args=True, verbose=False), scope, res); scope.update(res) if update_scope else None; return Struct(res)
-def generate_readme(path, obj=None, desc=None, save_source_code=True, verbose=True):  # Generates a readme file to contextualize any binary files by mentioning module, class, method or function used to generate the data"""
-    text, obj_path, path = "# Description\n" + (desc if desc is not None else '') + (separator := "\n" + "-" * 50 + "\n\n"), P(__import__('inspect').getfile(obj)) if obj is not None else None, P(path)
-    text += (f"# Source code file generated me was located here: \n`{obj_path.collapseuser().as_posix()}`\n" + separator) if obj is not None else ""
-    try:
-        repo = install_n_import("git", "gitpython").Repo(obj_path.parent, search_parent_directories=True)
-        text += f"# Last Commit\n{repo.git.execute('git log -1')}{separator}# Remote Repo\n{repo.git.execute('git remote -v')}{separator}"
-        text += f"# link to files: \n{repo.remote().url.replace('.git', '')}/tree/{repo.active_branch.commit.hexsha}/{Experimental.try_this(lambda: obj_path.relative_to(repo.working_dir).as_posix(), return_='')}{separator}"
-    except: text += f"Could not read git repository @ `{obj_path.parent}`.\n"
-    text += (f"\n\n# Code to reproduce results\n\n```python\n" + __import__("inspect").getsource(obj) + "\n```" + separator) if obj is not None else ""
-    readmepath = (path / f"README.md" if path.is_dir() else (path.with_name(path.trunk + "_README.md") if path.is_file() else path)).write_text(text, encoding="utf-8"); print(f"SAVED {readmepath.name} @ {readmepath.absolute().as_uri()}") if verbose else None
-    if save_source_code: P((obj.__code__.co_filename if hasattr(obj, "__code__") else None) or __import__("inspect").getmodule(obj).__file__).zip(path=readmepath.with_name(P(readmepath).trunk + "_source_code.zip"), verbose=False); print("SAVED source code @ " + readmepath.with_name("source_code.zip").absolute().as_uri()); return readmepath
-def load_from_source_code(directory, obj=None, delete=False):
-    P(directory).find("source_code*", r=True).unzip(tmpdir := P.tmp() / timestamp(name="tmp_sourcecode"))
-    sys.path.insert(0, str(tmpdir)); sourcefile = __import__(tmpdir.find("*").stem); tmpdir.delete(sure=delete, verbose=False)
-    return getattr(sourcefile, obj) if obj is not None else sourcefile
-def extract_code(func, code: str = None, include_args=True, verbose=True, copy2clipboard=False, **kwargs):  # TODO: how to handle decorated functions.  add support for lambda functions.  ==> use dill for powerfull inspection"""
-    import inspect; import textwrap  # assumptions: first line could be @classmethod or @staticmethod. second line could be def(...). Then function body must come in subsequent lines, otherwise ignored.
-    raw = inspect.getsourcelines(func)[0]; lines = textwrap.dedent("".join(raw[1 + (1 if raw[0].lstrip().startswith("@") else 0):])).split("\n")
-    code_string = '\n'.join([aline if not textwrap.dedent(aline).startswith("return ") else aline.replace("return ", "return_ = ") for aline in lines])  # remove return statements if there else keep line as is.
-    title, args_header, injection_header, body_header, suffix = ((f"\n# " + f"{item} {func.__name__}".center(50, "=") + "\n") for item in ["CODE EXTRACTED FROM", "ARGS KWARGS OF", "INJECTED CODE INTO", "BODY OF", "BODY END OF"])
-    code_string = title + ((args_header + extract_arguments(func, **kwargs)) if include_args else '') + ((injection_header + code) if code is not None else '') + body_header + code_string + suffix  # added later so it has more overwrite authority.
-    install_n_import("clipboard").copy(code_string) if copy2clipboard else None; print(code_string) if verbose else None; return code_string  # ready to be run with exec()
-def extract_arguments(func, copy2clipboard=False, **kwargs):
-    ak = Struct(dict((inspect := __import__("inspect")).signature(func).parameters)).values()  # ignores self for methods automatically but also ignores args and kwargs.
-    res = Struct.from_keys_values(ak.name, ak.default).update(kwargs).print(as_config=True, return_str=True, justify=0, quotes=True).replace("<class 'inspect._empty'>", "None").replace("= '", "= rf'")
-    ak = inspect.getfullargspec(func); res = res + (f"{ak.varargs} = (,)\n" if ak.varargs else '') + (f"{ak.varkw} = " + "{}\n" if ak.varkw else '')  # add args = () and kwargs = {}
-    install_n_import("clipboard").copy(res) if copy2clipboard else None; return res
-def run_cell(pointer, module=sys.modules[__name__]):
-    for cell in P(module.__file__).read_text().split("#%%"):
-        if pointer in cell.split('\n')[0]: break  # bingo
-    else: raise KeyError(f"The pointer `{pointer}` was not found in the module `{module}`")
-    print(cell); install_n_import("clipboard").copy(cell); return cell
-class Experimental: try_this = try_this; show_globals = show_globals; monkey_patch = monkey_patch; capture_locals = capture_locals; generate_readme = generate_readme; load_from_source_code = load_from_source_code; extract_code = extract_code; extract_arguments = extract_arguments; run_cell = run_cell  # Debugging and Meta programming tools"""
-
-
-if __name__ == '__main__':
-    pass
+
+from crocodile.core import timestamp, randstr, str2timedelta, Save, install_n_import, List, Struct
+from crocodile.file_management import P, datetime
+import time
+import logging
+import subprocess
+import sys
+
+
+class Null:
+    def __init__(self, return_='self'): self.return_ = return_
+    def __getattr__(self, item) -> 'Null': _ = item; return self if self.return_ == 'self' else self.return_
+    def __getitem__(self, item) -> 'Null': _ = item; return self if self.return_ == 'self' else self.return_
+    def __call__(self, *args, **kwargs) -> 'Null': return self if self.return_ == 'self' else self.return_
+    def __len__(self): return 0
+    def __bool__(self): return False
+    def __contains__(self, item): _ = self, item; return False
+    def __iter__(self): return iter([self])
+
+
+class Log(logging.Logger):  #
+    def __init__(self, dialect=["colorlog", "logging", "coloredlogs"][0], name=None, file: bool = False, file_path=None, stream=True, fmt=None, sep=" | ",
+                 s_level=logging.DEBUG, f_level=logging.DEBUG, l_level=logging.DEBUG, verbose=False, log_colors=None):
+        super().__init__(name := randstr() if name is None and not print(f"Logger name not passed. It is recommended to pass a name indicating the owner.") else name, level=l_level)  # logs everything, finer level of control is given to its handlers
+        print(f"Logger `{name}` from `{dialect}` is instantiated with level {l_level}."); self.file_path = file_path  # proper update to this value by self.add_filehandler()
+        if dialect == "colorlog": module = install_n_import("colorlog"); processed_fmt = module.ColoredFormatter(fmt or (rf"%(log_color)s" + Log.get_format(sep)), datefmt="%d %H:%M:%S", log_colors=log_colors or {'DEBUG': 'bold_cyan', 'INFO': 'green', 'WARNING': 'yellow', 'ERROR': 'thin_red', 'CRITICAL': 'fg_bold_red,bg_black', })  # see here for format: https://pypi.org/project/colorlog/
+        else: module = logging; processed_fmt = logging.Formatter(fmt or Log.get_format(sep, datefmt="%d %H:%M:%S"))
+        self.add_filehandler(file_path=file_path, fmt=processed_fmt, f_level=f_level) if file or file_path else None; self.add_streamhandler(s_level, fmt=processed_fmt, module=module) if stream else None
+        self.specs = dict(dialect=dialect, name=self.name, file=file, file_path=self.file_path, stream=bool(self.get_shandler()), fmt=fmt, sep=sep, s_level=s_level, f_level=f_level, l_level=l_level, verbose=verbose, log_colors=log_colors)  # # this way of creating relative path makes transferrable across machines.
+    def get_shandler(self): return List(handler for handler in self.handlers if "StreamHandler" in str(handler))
+    def get_fhandler(self): return List(handler for handler in self.handlers if "FileHandler" in str(handler))
+    def set_level(self, level, which=["logger", "stream", "file", "all"][0]): self.setLevel(level) if which in {"logger", "all"} else None; self.get_shandler().setLevel(level) if which in {"stream", "all"} else None; self.get_fhandler().setLevel(level) if which in {"file", "all"} else None
+    def __reduce_ex__(self, protocol): _ = protocol; return self.__class__, tuple(self.specs.values())  # reduce_ex is enchanced reduce. Its lower than getstate and setstate. It uses init method to create an instance.
+    def __repr__(self): return "".join([f"Logger {self.name} (level {self.level}) with handlers: \n"] + [repr(h) + f"" + "\n" for h in self.handlers])
+    get_format = staticmethod(lambda sep=' | ': f"%(asctime)s{sep}%(name)s{sep}%(module)s{sep}%(funcName)s{sep}%(levelname)s(%(levelno)s){sep}%(message)s{sep}")  # Reference: https://docs.python.org/3/library/logging.html#logrecord-attributes logging.BASIC_FORMAT
+    def manual_degug(self, path): _ = self; sys.stdout = open(path, 'w'); sys.stdout.close(); print(f"Finished ... have a look @ \n {path}")  # all print statements will write to this file.
+    @staticmethod
+    def get_coloredlogs(name=None, file=False, file_path=None, stream=True, fmt=None, sep=" | ", s_level=logging.DEBUG, f_level=logging.DEBUG, l_level=logging.DEBUG, verbose=False):
+        level_styles = {'spam': {'color': 'green', 'faint': True}, 'debug': {'color': 'white'}, 'verbose': {'color': 'blue'}, 'info': {'color': "green"}, 'notice': {'color': 'magenta'}, 'warning': {'color': 'yellow'}, 'success': {'color': 'green', 'bold': True},
+                        'error': {'color': 'red', "faint": True, "underline": True}, 'critical': {'color': 'red', 'bold': True, "inverse": False}}  # https://coloredlogs.readthedocs.io/en/latest/api.html#available-text-styles-and-colors
+        field_styles = {'asctime': {'color': 'green'}, 'hostname': {'color': 'magenta'}, 'levelname': {'color': 'black', 'bold': True}, 'path': {'color': 'blue'}, 'programname': {'color': 'cyan'}, 'username': {'color': 'yellow'}}
+        if verbose: logger = install_n_import("verboselogs").VerboseLogger(name=name); logger.setLevel(l_level)  # https://github.com/xolox/python-verboselogs # verboselogs.install()  # hooks into logging module.
+        else: logger = Log(name=name, dialect="logging", l_level=l_level, file=file, f_level=f_level, file_path=file_path, fmt=fmt or Log.get_format(sep), stream=stream, s_level=s_level)  # new step, not tested:
+        install_n_import("coloredlogs").install(logger=logger, name="lol_different_name", level=logging.NOTSET, level_styles=level_styles, field_styles=field_styles, fmt=fmt or Log.get_format(sep), isatty=True, milliseconds=True); return logger
+    def add_streamhandler(self, s_level=logging.DEBUG, fmt=None, module=logging, name="myStreamHandler"):
+        shandler = module.StreamHandler(); shandler.setLevel(level=s_level); shandler.setFormatter(fmt=fmt); shandler.set_name(name); self.addHandler(shandler); print(f"    Level {s_level} stream handler for Logger `{self.name}` is created.")
+    def add_filehandler(self, file_path=None, fmt=None, f_level=logging.DEBUG, mode="a", name="myFileHandler"):
+        fhandler = logging.FileHandler(filename := (P.tmpfile(name="logger_" + self.name, suffix=".log", folder="tmp_loggers") if file_path is None else P(file_path).expanduser()), mode=mode)
+        fhandler.setFormatter(fmt=fmt); fhandler.setLevel(level=f_level); fhandler.set_name(name); self.addHandler(fhandler); self.file_path = filename.collapseuser(); print(f"    Level {f_level} file handler for Logger `{self.name}` is created @ " + P(filename).clickable())
+    def test(self): List([self.debug, self.info, self.warning, self.error, self.critical]).apply(lambda func: func(f"this is a {func.__name__} message")); [self.log(msg=f"This is a message of level {level}", level=level) for level in range(0, 60, 5)]
+    def get_history(self, lines=200, to_html=False): logs = "\n".join(self.file_path.expanduser().absolute().read_text().split("\n")[-lines:]); return install_n_import("ansi2html").Ansi2HTMLConverter().convert(logs) if to_html else logs
+
+
+class Terminal:
+    class Response:
+        @staticmethod
+        def from_completed_process(cp: subprocess.CompletedProcess): (resp := Terminal.Response(cmd=cp.args)).output.update(dict(stdout=cp.stdout, stderr=cp.stderr, returncode=cp.returncode)); return resp
+        def __init__(self, stdin=None, stdout=None, stderr=None, cmd=None, desc=""): self.std, self.output, self.input, self.desc = dict(stdin=stdin, stdout=stdout, stderr=stderr), dict(stdin="", stdout="", stderr="", returncode=None), cmd, desc  # input command
+        def __call__(self, *args, **kwargs): return self.op.rstrip() if type(self.op) is str else None
+        op = property(lambda self: self.output["stdout"])
+        ip = property(lambda self: self.output["stdin"])
+        err = property(lambda self: self.output["stderr"])
+        returncode = property(lambda self: self.output["returncode"])
+        def op2path(self, strict_returncode=True, strict_err=False) -> P or None:
+            return P(self.op.rstrip()) if self.is_successful(strict_returcode=strict_returncode, strict_err=strict_err) else None
+        def op_if_successfull_or_default(self, strict_returcode=True, strict_err=False, default=None): return self.op if self.is_successful(strict_returcode=strict_returcode, strict_err=strict_err) else default
+        def is_successful(self, strict_returcode=True, strict_err=False): return ((self.output["returncode"] in {0, None}) if strict_returcode else True) and (self.err == "" if strict_err else True)
+        def capture(self): [self.output.__setitem__(key, val.read().decode().rstrip()) for key, val in self.std.items() if val is not None and val.readable()]; return self
+        def print(self, desc="TERMINAL CMD", capture=True):
+            self.capture() if capture else None; install_n_import("rich"); from rich import console; con = console.Console(); from rich.panel import Panel; from rich.text import Text  # from rich.syntax import Syntax; syntax = Syntax(my_code, "python", theme="monokai", line_numbers=True)
+            tmp1 = Text("Input Command:\n"); tmp1.stylize("u bold blue"); tmp2 = Text("\nTerminal Response:\n"); tmp2.stylize("u bold blue")
+            txt = tmp1 + Text(str(self.input), style="white") + tmp2 + Text("\n".join([f"{f' {idx} - {key} '}".center(40, "-") + f"\n{val}" for idx, (key, val) in enumerate(self.output.items())]), style="white")
+            con.print(Panel(txt, title=self.desc, subtitle=desc, width=150, style="bold cyan on black")); return self
+    def __init__(self, stdout=subprocess.PIPE, stderr=subprocess.PIPE, stdin=subprocess.PIPE, elevated=False):
+        self.available_consoles, self.machine = ["cmd", "Command Prompt", "wt", "powershell", "wsl", "ubuntu", "pwsh"], __import__("platform").system()
+        self.elevated, self.stdout, self.stderr, self.stdin = elevated, stdout, stderr, stdin
+    def set_std_system(self): self.stdout = sys.stdout; self.stderr = sys.stderr; self.stdin = sys.stdin
+    def set_std_pipe(self): self.stdout = subprocess.PIPE; self.stderr = subprocess.PIPE; self.stdin = subprocess.PIPE
+    def set_std_null(self): self.stdout, self.stderr, self.stdin = subprocess.DEVNULL, subprocess.DEVNULL, subprocess.DEVNULL  # Equivalent to `echo 'foo' &> /dev/null`
+    def run(self, *cmds, shell=None, check=False, ip=None):  # Runs SYSTEM commands like subprocess.run
+        """Blocking operation. Thus, if you start a shell via this method, it will run in the main and won't stop until you exit manually IF stdin is set to sys.stdin, otherwise it will run and close quickly. Other combinations of stdin, stdout can lead to funny behaviour like no output but accept input or opposite.
+        * This method is short for: res = subprocess.run("powershell command", capture_output=True, shell=True, text=True) and unlike os.system(cmd), subprocess.run(cmd) gives much more control over the output and input.
+        * `shell=True` loads up the profile of the shell called so more specific commands can be run. Importantly, on Windows, the `start` command becomes availalbe and new windows can be launched.
+        * `capture_output` prevents the stdout to redirect to the stdout of the script automatically, instead it will be stored in the Response object returned. # `capture_output=True` same as `stdout=subprocess.PIPE, stderr=subprocess.PIPE`"""
+        my_list = list(cmds)  # `subprocess.Popen` (process open) is the most general command. Used here to create asynchronous job. `subprocess.run` is a thin wrapper around Popen that makes it wait until it finishes the task. `suprocess.call` is an archaic command for pre-Python-3.5.
+        if self.machine == "Windows" and shell in {"powershell", "pwsh"}: my_list = [shell, "-Command"] + my_list  # alternatively, one can run "cmd"
+        if self.elevated is False or self.is_user_admin(): resp = subprocess.run(my_list, stderr=self.stderr, stdin=self.stdin, stdout=self.stdout, text=True, shell=True, check=check, input=ip)
+        else: resp = __import__("ctypes").windll.shell32.ShellExecuteW(None, "runas", sys.executable, " ".join(sys.argv), None, 1)
+        return self.Response.from_completed_process(resp)
+    @staticmethod
+    def is_user_admin() -> bool:  # adopted from: https://stackoverflow.com/questions/19672352/how-to-run-script-with-elevated-privilege-on-windows"""
+        if __import__('os').name == 'nt':
+            try: return __import__("ctypes").windll.shell32.IsUserAnAdmin()
+            except: import traceback; traceback.print_exc(); print("Admin check failed, assuming not an admin."); return False
+        else: return __import__('os').getuid() == 0  # Check for root on Posix
+    @staticmethod
+    def run_as_admin(file, params, wait=False): proce_info = install_n_import("win32com", fromlist=["shell.shell.ShellExecuteEx"]).shell.shell.ShellExecuteEx(lpVerb='runas', lpFile=file, lpParameters=params); time.sleep(wait) if wait is not False and wait is not True else None; return proce_info
+    def run_async(self, *cmds, new_window=True, shell=None, terminal=None):  # Runs SYSTEM commands like subprocess.Popen
+        """Opens a new terminal, and let it run asynchronously. Maintaining an ongoing conversation with another process is very hard. It is adviseable to run all
+        commands in one go without interaction with an ongoing channel. Use this only for the purpose of producing a different window and humanly interact with it. Reference: https://stackoverflow.com/questions/54060274/dynamic-communication-between-main-and-subprocess-in-python & https://www.youtube.com/watch?v=IynV6Y80vws and https://www.oreilly.com/library/view/windows-powershell-cookbook/9781449359195/ch01.html"""
+        if terminal is None: terminal = ""  # this means that cmd is the default console. alternative is "wt"
+        if shell is None: shell = "" if self.machine == "Windows" else ""  # other options are "powershell" and "cmd". # if terminal is wt, then it will pick powershell by default anyway.
+        new_window = "start" if new_window is True else ""  # start is alias for Start-Process which launches a new window.  adding `start` to the begining of the command results in launching a new console that will not inherit from the console python was launched from e.g. conda
+        extra, my_list = ("-Command" if shell in {"powershell", "pwsh"} else ""), list(cmds)
+        if self.machine == "Windows": my_list = [new_window, terminal, shell, extra] + my_list  # having a list is equivalent to: start "ipython -i file.py". Thus, arguments of ipython go to ipython, not start.
+        print("Meta.Terminal.run_async: Subprocess command: ", my_list := [item for item in my_list if item != ""])
+        return subprocess.Popen(my_list, stdin=subprocess.PIPE, shell=True)  # stdout=self.stdout, stderr=self.stderr, stdin=self.stdin. # returns Popen object, not so useful for communcation with an opened terminal
+    @staticmethod
+    def run_py(script, wdir=None, interactive=True, ipython=True, shell=None, delete=False, terminal="", new_window=True, header=True):  # async run, since sync run is meaningless.
+        script = ((Terminal.get_header(wdir=wdir) if header else "") + script) + ("\ntb.DisplayData.set_pandas_auto_width()\n" if terminal in {"wt", "powershell", "pwsh"} else "")
+        file = P.tmpfile(name="tmp_python_script", suffix=".py", folder="tmp_scripts").write_text(f"""print(r'''{script}''')""" + "\n" + script); print(f"Script to be executed asyncronously: ", file.absolute().as_uri())
+        Terminal().run_async(f"{'ipython' if ipython else 'python'}", f"{'-i' if interactive else ''}", f"{file}", terminal=terminal, shell=shell, new_window=new_window)  # python will use the same dir as the one from console this method is called.
+        _ = delete  # we need to ensure that async process finished reading before deleteing: file.delete(sure=delete, verbose=False)
+    pickle_to_new_session = staticmethod(lambda obj, cmd="": Terminal.run_py(f"""path = tb.P(r'{Save.pickle(obj=obj, path=P.tmpfile(tstamp=False, suffix=".pkl"), verbose=False)}')\n obj = path.readit()\npath.delete(sure=True, verbose=False)\n {cmd}"""))
+    @staticmethod
+    def import_to_new_session(func=None, cmd="", header=True, interactive=True, ipython=True, **kwargs):
+        load_kwargs_string = f"""loaded_kwargs = tb.P(r'{Save.pickle(obj=kwargs, path=P.tmpfile(tstamp=False, suffix=".pkl"), verbose=False)}').readit()\nloaded_kwargs.print()\nobj(**loaded_kwargs)""" if kwargs is not {} else ""
+        if callable(func) and func.__name__ != func.__qualname__:  # it is a method of a class, must be instantiated first.
+            module = P(sys.modules['__main__'].__file__).rel2cwd().stem if (module := func.__module__) == "__main__" else module
+            load_func_string = f"import {module} as m\ninst=m.{func.__qualname__.split('.')[0]}()\nobj = inst.{func.__name__}" + f"\n{cmd}\n{load_kwargs_string}\n"
+        elif callable(func) and hasattr(func, "__code__"):  # it is a standalone function...
+            module = P(func.__code__.co_filename)  # module = func.__module__  # fails if the function comes from main as it returns __main__.
+            load_func_string = f"tb.sys.path.insert(0, r'{module.parent}')\nimport {module.stem} as m\nobj=m.{func.__name__}" + f"\n{cmd}\n{load_kwargs_string}\n"
+        else: load_func_string = f"""obj = tb.P(r'{Save.pickle(obj=func, path=P.tmpfile(tstamp=False, suffix=".pkl"), verbose=False)}').readit()"""
+        return Terminal.run_py(load_func_string, header=header, interactive=interactive, ipython=ipython)  # Terminal().run_async("python", "-c", load_func_string + f"\n{cmd}\n{load_kwargs_string}\n")
+    @staticmethod
+    def replicate_session(cmd=""): __import__("dill").dump_session(file := P.tmpfile(suffix=".pkl"), main=sys.modules[__name__]); Terminal().run_py(script=f"""path = tb.P(r'{file}')\nimport dill\nsess= dill.load_session(str(path))\npath.delete(sure=True, verbose=False)\n{cmd}""")
+    @staticmethod
+    def get_header(wdir=None): return f"""\n# >> Code prepended\nimport crocodile.toolbox as tb""" + (f"""\ntb.sys.path.insert(0, r'{wdir}')""" if wdir is not None else '') + f"""\n# >> End of header, start of script passed\n"""
+
+
+class SSH:  # inferior alternative: https://github.com/fabric/fabric
+    def __init__(self, username=None, hostname=None, host=None, tmate_sess=None, sshkey=None, pwd=None, port=22, ve="ve", compress=False):  # https://stackoverflow.com/questions/51027192/execute-command-script-using-different-shell-in-ssh-paramiko
+        username, self.host, self.tmate_sess, self.compress, self.pwd, self.ve = username or __import__("getpass").getuser(), None, tmate_sess, compress, pwd, ve  # Defaults: (1) use localhost if nothing provided.
+        if "@" not in username and hostname is None:  # then, username is probably a Host profile
+            try:
+                config = __import__("paramiko.config").config.SSHConfig.from_path(P.home().joinpath(".ssh/config").str); config_dict = config.lookup(host or username)
+                self.hostname, self.username, self.host, port, sshkey = config_dict["hostname"], config_dict["user"], host or username, config_dict.get("port", port), tmp[0] if type(tmp := config_dict.get("identityfile", sshkey)) is list else tmp
+                if sshkey is not None: sshkey = tmp[0] if type(tmp := config.lookup("*").get("identityfile", sshkey)) is list else tmp
+            except (FileNotFoundError, KeyError): self.hostname, self.username = __import__("platform").node(), username
+        else: self.username, self.hostname = username.split("@") if "@" in username else (username, hostname)
+        self.hostname, self.port = self.hostname.split(":") if ":" in self.hostname else (self.hostname, port); self.port = int(self.port)
+        self.sshkey = str(P(sshkey).expanduser().absolute()) if sshkey is not None else None  # no need to pass sshkey if it was configured properly already
+        self.ssh = (paramiko := __import__("paramiko")).SSHClient(); self.ssh.load_system_host_keys(); self.ssh.set_missing_host_key_policy(paramiko.AutoAddPolicy())
+        install_n_import("rich").inspect(Struct(hostname=self.hostname, username=self.username, password="***", port=self.port, key_filename=self.sshkey), value=False, title="SSHing To", docs=False, sort=False)
+        self.ssh.connect(hostname=self.hostname, username=self.username, password=self.pwd, port=self.port, key_filename=self.sshkey, compress=self.compress)
+        try: self.sftp = self.ssh.open_sftp()
+        except Exception as err: self.sftp = None; print(f"WARNING: could not open SFTP connection to {hostname}. No data transfer is possible. Erorr faced: `{err}`")
+        def view_bar(slf, a, b): slf.total = int(b); slf.update(int(a - slf.n))  # update pbar with increment
+        self.tqdm_wrap = type('TqdmWrap', (install_n_import("tqdm").tqdm,), {'view_bar': view_bar})
+        self._local_distro, self._remote_distro, self._remote_machine, self.terminal_responses, self.platform = None, None, None, [], __import__("platform")
+        self.remote_env_cmd = rf"""~/venvs/{self.ve}/Scripts/Activate.ps1""" if self.get_remote_machine() == "Windows" else rf"""source ~/venvs/{self.ve}/bin/activate"""
+        self.local_env_cmd = rf"""~/venvs/{self.ve}/Scripts/Activate.ps1""" if self.platform.system() == "Windows" else rf"""source ~/venvs/{self.ve}/bin/activate"""  # works for both cmd and pwsh
+    def __getstate__(self): return {attr: self.__getattribute__(attr) for attr in ["username", "hostname", "host", "tmate_sess", "port", "sshkey", "compress", "pwd", "ve"]}
+    def __setstate__(self, state): self.__init__(**state)
+    def get_remote_machine(self): self._remote_machine = ("Windows" if (self.run("$env:OS", verbose=False, desc="Testing OS").capture().op == "Windows_NT" or self.run("echo %OS%", verbose=False, desc="Testing OS").capture().op == "Windows_NT") else "Linux") if self._remote_machine is None else self._remote_machine; return self._remote_machine  # echo %OS% TODO: uname on linux
+    def get_local_distro(self): self._local_distro = install_n_import("distro").name(pretty=True) if self._local_distro is None else self._local_distro; return self._local_distro
+    def get_remote_distro(self): self._remote_distro = self.run_py("print(tb.install_n_import('distro').name(pretty=True))", verbose=False).capture().op_if_successfull_or_default(default="") if self._remote_distro is None else self._remote_distro; return self._remote_distro
+    def restart_computer(self): self.run("Restart-Computer -Force" if self.get_remote_machine() == "Windows" else "sudo reboot")
+    def send_ssh_key(self): self.copy_from_here("~/.ssh/id_rsa.pub"); assert self.get_remote_machine() == "Windows"; self.run(P(install_n_import("machineconfig").scripts.windows.__path__.__dict__["_path"][0]).joinpath("openssh_server_add_sshkey.ps1").read_text())
+    def copy_env_var(self, name): assert self.get_remote_machine() == "Linux"; return self.run(f"{name} = {__import__('os').environ[name]}; export {name}")
+    def get_repr(self, which="remote", add_machine=False): return (f"{self.username}@{self.hostname}:{self.port}" + (f" [{self.get_remote_machine()}][{self.get_remote_distro()}]" if add_machine else "")) if which == "remote" else f"{__import__('getpass').getuser()}@{self.platform.node()}" + (f" [{self.platform.system()}][{self.get_local_distro()}]" if add_machine else "")
+    def __repr__(self): return f"local {self.get_repr('local', add_machine=True)} >>> SSH TO >>> remote {self.get_repr('remote', add_machine=True)}"
+    def run_locally(self, command): print(f"Executing Locally @ {self.platform.node()}:\n{command}"); return Terminal.Response(__import__('os').system(command))
+    def get_ssh_conn_str(self, cmd=""): return f"ssh" + (f" -i {self.sshkey}" if self.sshkey else "") + (f' -t {cmd} ' if cmd != '' else ' ') + self.get_repr('remote').replace(':', ' -p ')
+    def open_console(self, cmd='', new_window=True, terminal=None): Terminal().run_async(*self.get_ssh_conn_str().split(" "), cmd, new_window=new_window, terminal=terminal)
+    def run(self, cmd, verbose=True, desc="", strict_err=False, strict_returncode=False, env_prefix=False) -> Terminal.Response:  # most central method.
+        cmd = (self.remote_env_cmd + "; " + cmd) if env_prefix else cmd; res = Terminal.Response(stdin=(raw := self.ssh.exec_command(cmd))[0], stdout=raw[1], stderr=raw[2], cmd=cmd, desc=desc)
+        if strict_err or strict_returncode: assert res.is_successful(strict_err=strict_err, strict_returcode=strict_returncode), res.print()
+        res.print() if verbose else None; self.terminal_responses.append(res); return res
+    def run_py(self, cmd, desc="", return_obj=False, verbose=True, strict_err=False, strict_returncode=False):
+        assert '"' not in cmd, f'Avoid using `"` in your command. I dont know how to handle this when passing is as command to python in pwsh command.'
+        if not return_obj: return self.run(f"""{self.remote_env_cmd}; python -c "{Terminal.get_header(wdir=None)}{cmd}\n""" + '"', desc=desc or f"run_py on {self.get_repr('remote')}", verbose=verbose, strict_err=strict_err, strict_returncode=strict_returncode)
+        else: assert "obj=" in cmd, f"The command sent to run_py must have `obj=` statement if return_obj is set to True"; source_file = self.run_py(f"""{cmd}\npath = tb.Save.pickle(obj=obj, path=tb.P.tmpfile(suffix='.pkl'))\nprint(path)""", desc=desc, verbose=verbose, strict_err=True, strict_returncode=True).op.split('\n')[-1]; return self.copy_to_here(source=source_file, target=P.tmpfile(suffix='.pkl')).readit()
+    def copy_from_here(self, source, target=None, z=False, r=False, overwrite=False) -> P or List[P]:
+        if not z and (source := P(source).expanduser()).is_dir(): return source.search("*", folders=False, r=True).apply(lambda file: self.copy_from_here(source=file, target=target)) if r is True else print(f"tb.Meta.SSH Error: source is a directory! either set r=True for recursive sending or raise zip_first flag.")
+        if z: print(f"ZIPPING ..."); source = P(source).expanduser().zip(content=True)  # .append(f"_{randstr()}", inplace=True)  # eventually, unzip will raise content flag, so this name doesn't matter.
+        if target is None: target = P(source).collapseuser(); assert target.is_relative_to("~"), f"If target is not specified, source must be relative to home."
+        remotepath = self.run_py(f"path=tb.P(r'{P(target).as_posix()}').expanduser()\n{'path.delete(sure=True)' if overwrite else ''}\nprint(path.parent.create())", desc=f"Creating Target directory `{P(target).parent.as_posix()}` @ {self.get_repr('remote')}").op or ''; remotepath = P(remotepath.split("\n")[-1]).joinpath(P(target).name)
+        print(f"SENDING `{repr(P(source))}` ==> `{remotepath.as_posix()}`")
+        with self.tqdm_wrap(ascii=True, unit='b', unit_scale=True) as pbar: self.sftp.put(localpath=P(source).expanduser(), remotepath=remotepath.as_posix(), callback=pbar.view_bar)
+        if z: resp = self.run_py(f"""tb.P(r'{remotepath.as_posix()}').expanduser().unzip(content=False, inplace=True, overwrite={overwrite})""", desc=f"UNZIPPING {remotepath.as_posix()}"); source.delete(sure=True); return resp
+    def copy_to_here(self, source, target=None, zip_first=False, r=False) -> P:
+        if not zip_first and self.run_py(f"print(tb.P(r'{source}').expanduser().is_dir())", desc="Check if source is a dir", verbose=True, strict_returncode=True, strict_err=True).op.split("\n")[-1] == 'True':
+            return self.run_py(f"obj=tb.P(r'{source}').search(folders=False, r=True).collapseuser()", desc="Searching for files in source", return_obj=True).apply(lambda file: self.copy_to_here(source=file.as_posix(), target=P(target).joinpath(P(file).relative_to(source)) if target else None, r=False)) if r else print(f"source is a directory! either set r=True for recursive sending or raise zip_first flag.")
+        if zip_first: source = self.run_py(f"print(tb.P(r'{source}').expanduser().zip(inplace=False, verbose=False))", desc=f"Zipping source file").op2path(strict_returncode=True, strict_err=True)
+        if target is None: target = self.run_py(f"print(tb.P(r'{P(source).as_posix()}').collapseuser())", desc=f"Finding default target via relative source path", strict_returncode=True, strict_err=True).op2path(); assert target.is_relative_to("~"), f"If target is not specified, source must be relative to home."
+        target = P(target).expanduser().create(parents_only=True); target += '.zip' if zip_first and '.zip' not in target.suffix else ''
+        source = self.run_py(f"print(tb.P(r'{source}').expanduser())", desc=f"# Resolving source path address by expanding user", strict_returncode=True, strict_err=True).op2path() if "~" in str(source) else P(source); print(f"RECEVING `{source}` ==> `{target}`")
+        with self.tqdm_wrap(ascii=True, unit='b', unit_scale=True) as pbar: self.sftp.get(remotepath=source.as_posix(), localpath=target.as_posix(), callback=pbar.view_bar)
+        if zip_first: target = target.unzip(inplace=True, content=True); self.run_py(f"tb.P(r'{source}').delete(sure=True)", desc="Cleaning temp files", strict_returncode=True, strict_err=True)
+        return target
+    def print_summary(self):   # ip=rsp.ip, op=rsp.op
+        install_n_import("tabulate"); df = __import__("pandas").DataFrame.from_records(List(self.terminal_responses).apply(lambda rsp: dict(desc=rsp.desc, err=rsp.err, returncode=rsp.returncode))); print("\nSummary of operations performed:"); print(df.to_markdown())
+        print("\nAll operations completed successfully.\n") if ((df['returncode'].to_list()[2:] == [None] * (len(df) - 2)) and (df['err'].to_list()[2:] == [''] * (len(df) - 2))) else print("\nSome operations failed. \n"); return df
+
+
+class Scheduler:
+    def __init__(self, routine=None, wait: str = "2m", other_routine=None, other_ratio: int = 10, max_cycles=float("inf"), exception_handler=None, logger: Log = None, sess_stats=None):
+        self.routine = (lambda sched: None) if routine is None else routine  # main routine to be repeated every `wait` time period
+        self.other_routine = (lambda sched: None) if other_routine is None else other_routine  # routine to be repeated every `other` time period
+        self.wait, self.other_ratio = str2timedelta(wait).total_seconds(), other_ratio  # wait period between routine cycles.
+        self.logger, self.exception_handler = logger if logger is not None else Log(name="SchedLogger_" + randstr(length=2)), exception_handler
+        self.sess_start_time, self.records, self.cycle, self.max_cycles, self.sess_stats = None, List([]), 0, max_cycles, sess_stats or (lambda sched: {})
+    def run(self, max_cycles=None, until="2050-01-01"):
+        self.max_cycles, self.cycle, self.sess_start_time = max_cycles or self.max_cycles, 0, datetime.now()
+        while datetime.now() < datetime.fromisoformat(until) and self.cycle < self.max_cycles:  # 1- Time before Ops, and Opening Message
+            time1 = datetime.now(); self.logger.warning(f"Starting Cycle {str(self.cycle).zfill(5)}. Total Run Time = {str(datetime.now() - self.sess_start_time)}. UTC {datetime.utcnow().strftime('%d %H:%M:%S')}")
+            try: self.routine(sched=self)
+            except BaseException as ex: self._handle_exceptions(ex=ex, during="routine")  # 2- Perform logic
+            if self.cycle % self.other_ratio == 0:
+                try: self.other_routine(sched=self)
+                except BaseException as ex: self._handle_exceptions(ex=ex, during="occasional")  # 3- Optional logic every while
+            time_left = int(self.wait - (datetime.now() - time1).total_seconds())  # 4- Conclude Message
+            self.cycle += 1; self.logger.warning(f"Finishing Cycle {str(self.cycle - 1).zfill(5)}. Sleeping for {self.wait}s ({time_left}s left)\n" + "-" * 100)
+            try: time.sleep(time_left if time_left > 0 else 0.1)  # # 5- Sleep. consider replacing by Asyncio.sleep
+            except KeyboardInterrupt as ex: self._handle_exceptions(ex, during="sleep")  # that's probably the only kind of exception that can rise during sleep.
+        else: self.record_session_end(reason=f"Reached maximum number of cycles ({self.max_cycles})" if self.cycle >= self.max_cycles else f"Reached due stop time ({until})"); return self
+    def get_records_df(self): return __import__("pandas").DataFrame.from_records(self.records, columns=["start", "finish", "duration", "cycles", "termination reason", "logfile"] + list(self.sess_stats(sched=self).keys()))
+    def record_session_end(self, reason="Not passed to function."):
+        self.records.append([self.sess_start_time, end_time := datetime.now(), duration := end_time-self.sess_start_time, self.cycle, reason, self.logger.file_path] + list((sess_stats := self.sess_stats(sched=self)).values()))
+        summ = {"start time": f"{str(self.sess_start_time)}", "finish time": f"{str(end_time)}.", "duration": f"{str(duration)} | wait time {self.wait}s", "cycles ran": f"{self.cycle} | Lifetime cycles = {self.get_records_df()['cycles'].sum()}", f"termination reason": reason, "logfile": self.logger.file_path}
+        self.logger.critical(f"\n--> Scheduler has finished running a session. \n" + Struct(summ).update(sess_stats).print(as_config=True, return_str=True, quotes=False) + "\n" + "-" * 100); self.logger.critical(f"\n--> Logger history.\n" + str(self.get_records_df())); return self
+    def _handle_exceptions(self, ex, during):
+        if self.exception_handler is not None: self.exception_handler(ex, during=during, sched=self)  # user decides on handling and continue, terminate, save checkpoint, etc.  # Use signal library.
+        else: self.record_session_end(reason=f"during {during}, " + str(ex)); self.logger.exception(ex); raise ex
+
+
+def try_this(func, return_=None, raise_=None, run=None, handle=None, verbose=False, **kwargs):
+    try: return func()
+    except BaseException as ex:  # or Exception
+        if verbose: print(ex)
+        if raise_ is not None: raise raise_
+        if handle is not None: return handle(ex, **kwargs)
+        return run() if run is not None else return_
+def show_globals(scope, **kwargs): return Struct(scope).filter(lambda k, v: "__" not in k and not k.startswith("_") and k not in {"In", "Out", "get_ipython", "quit", "exit", "sys"}).print(**kwargs)
+def monkey_patch(class_inst, func): setattr(class_inst.__class__, func.__name__, func)
+def capture_locals(func, scope, args=None, self: str = None, update_scope=True): res = dict(); exec(extract_code(func, args=args, self=self, include_args=True, verbose=False), scope, res); scope.update(res) if update_scope else None; return Struct(res)
+def generate_readme(path, obj=None, desc=None, save_source_code=True, verbose=True):  # Generates a readme file to contextualize any binary files by mentioning module, class, method or function used to generate the data"""
+    text, obj_path, path = "# Description\n" + (desc if desc is not None else '') + (separator := "\n" + "-" * 50 + "\n\n"), P(__import__('inspect').getfile(obj)) if obj is not None else None, P(path)
+    text += (f"# Source code file generated me was located here: \n`{obj_path.collapseuser().as_posix()}`\n" + separator) if obj is not None else ""
+    try:
+        repo = install_n_import("git", "gitpython").Repo(obj_path.parent, search_parent_directories=True)
+        text += f"# Last Commit\n{repo.git.execute('git log -1')}{separator}# Remote Repo\n{repo.git.execute('git remote -v')}{separator}"
+        text += f"# link to files: \n{repo.remote().url.replace('.git', '')}/tree/{repo.active_branch.commit.hexsha}/{Experimental.try_this(lambda: obj_path.relative_to(repo.working_dir).as_posix(), return_='')}{separator}"
+    except: text += f"Could not read git repository @ `{obj_path.parent}`.\n"
+    text += (f"\n\n# Code to reproduce results\n\n```python\n" + __import__("inspect").getsource(obj) + "\n```" + separator) if obj is not None else ""
+    readmepath = (path / f"README.md" if path.is_dir() else (path.with_name(path.trunk + "_README.md") if path.is_file() else path)).write_text(text, encoding="utf-8"); print(f"SAVED {readmepath.name} @ {readmepath.absolute().as_uri()}") if verbose else None
+    if save_source_code: P((obj.__code__.co_filename if hasattr(obj, "__code__") else None) or __import__("inspect").getmodule(obj).__file__).zip(path=readmepath.with_name(P(readmepath).trunk + "_source_code.zip"), verbose=False); print("SAVED source code @ " + readmepath.with_name("source_code.zip").absolute().as_uri()); return readmepath
+def load_from_source_code(directory, obj=None, delete=False):
+    P(directory).find("source_code*", r=True).unzip(tmpdir := P.tmp() / timestamp(name="tmp_sourcecode"))
+    sys.path.insert(0, str(tmpdir)); sourcefile = __import__(tmpdir.find("*").stem); tmpdir.delete(sure=delete, verbose=False)
+    return getattr(sourcefile, obj) if obj is not None else sourcefile
+def extract_code(func, code: str = None, include_args=True, verbose=True, copy2clipboard=False, **kwargs):  # TODO: how to handle decorated functions.  add support for lambda functions.  ==> use dill for powerfull inspection"""
+    import inspect; import textwrap  # assumptions: first line could be @classmethod or @staticmethod. second line could be def(...). Then function body must come in subsequent lines, otherwise ignored.
+    raw = inspect.getsourcelines(func)[0]; lines = textwrap.dedent("".join(raw[1 + (1 if raw[0].lstrip().startswith("@") else 0):])).split("\n")
+    code_string = '\n'.join([aline if not textwrap.dedent(aline).startswith("return ") else aline.replace("return ", "return_ = ") for aline in lines])  # remove return statements if there else keep line as is.
+    title, args_header, injection_header, body_header, suffix = ((f"\n# " + f"{item} {func.__name__}".center(50, "=") + "\n") for item in ["CODE EXTRACTED FROM", "ARGS KWARGS OF", "INJECTED CODE INTO", "BODY OF", "BODY END OF"])
+    code_string = title + ((args_header + extract_arguments(func, **kwargs)) if include_args else '') + ((injection_header + code) if code is not None else '') + body_header + code_string + suffix  # added later so it has more overwrite authority.
+    install_n_import("clipboard").copy(code_string) if copy2clipboard else None; print(code_string) if verbose else None; return code_string  # ready to be run with exec()
+def extract_arguments(func, copy2clipboard=False, **kwargs):
+    ak = Struct(dict((inspect := __import__("inspect")).signature(func).parameters)).values()  # ignores self for methods automatically but also ignores args and kwargs.
+    res = Struct.from_keys_values(ak.name, ak.default).update(kwargs).print(as_config=True, return_str=True, justify=0, quotes=True).replace("<class 'inspect._empty'>", "None").replace("= '", "= rf'")
+    ak = inspect.getfullargspec(func); res = res + (f"{ak.varargs} = (,)\n" if ak.varargs else '') + (f"{ak.varkw} = " + "{}\n" if ak.varkw else '')  # add args = () and kwargs = {}
+    install_n_import("clipboard").copy(res) if copy2clipboard else None; return res
+def run_cell(pointer, module=sys.modules[__name__]):
+    for cell in P(module.__file__).read_text().split("#%%"):
+        if pointer in cell.split('\n')[0]: break  # bingo
+    else: raise KeyError(f"The pointer `{pointer}` was not found in the module `{module}`")
+    print(cell); install_n_import("clipboard").copy(cell); return cell
+class Experimental: try_this = try_this; show_globals = show_globals; monkey_patch = monkey_patch; capture_locals = capture_locals; generate_readme = generate_readme; load_from_source_code = load_from_source_code; extract_code = extract_code; extract_arguments = extract_arguments; run_cell = run_cell  # Debugging and Meta programming tools"""
+
+
+if __name__ == '__main__':
+    pass
```

### Comparing `crocodile-8.40/myresources/crocodile/plotly_management.py` & `crocodile-9.0/myresources/crocodile/plotly_management.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,64 +1,64 @@
-
-import crocodile.toolbox as tb
-# import pandas as pd
-
-import plotly.graph_objects as go
-import plotly.express as px
-from plotly.subplots import make_subplots
-import plotly.io as pio
-
-import dash
-from dash import Input, Output, State, callback_context as ctx
-from dash import dcc
-from dash import html
-import dash_daq as daq
-
-from types import SimpleNamespace
-import sys
-
-pio.renderers.default = "browser"
-tm = tb.Terminal()
-_ = Input, Output, State, dcc, html, daq
-_ = go, px, make_subplots
-
-
-CONFIG = SimpleNamespace(displayModeBar=True,  # always visible.
-                         staticPlot=False,
-                         scrollZoom=False,
-                         doubleClick="reset",
-                         showTips=True,
-                         toImageButtonOptions={
-                             'format': 'png',  # one of png, svg, jpeg, webp
-                             'filename': 'custom_image',
-                             'height': 1500,  # None means use currently rendered size.
-                             'width': 1500,
-                             'scale': 1  # Multiply title/legend/axis/canvas sizes by this factor
-                         },
-                         modeBarButtonsToAdd=['drawline',
-                                              'drawopenpath',
-                                              'drawclosedpath',
-                                              'drawcircle',
-                                              'drawrect',
-                                              'eraseshape']
-                         )
-
-
-class App:
-    @staticmethod
-    def run(app, debug=False, random_port=True):
-        host = "127.0.0.1"
-        port = tb.randstr(lower=False, upper=False, length=4) if random_port else "8050"  # Random ports prevent multile programs from crashing into each other.
-        # pynoinspection HTTP
-        tb.P(rf'http://{host}:{port}/')()
-        app.run_server(debug=debug, port=port)  # , processes=2, threaded=False)
-
-    @staticmethod
-    def get_app(name=""): return dash.Dash(name=name+tb.randstr(), external_stylesheets=[r'https://codepen.io/chriddyp/pen/bWLwgP.css'])
-
-    @staticmethod
-    def run_async_decorator(func):  # Decorate functions with this to make them run_command asynchornously."""
-        raise NotImplementedError
-
-
-if __name__ == '__main__':
-    pass
+
+import crocodile.toolbox as tb
+# import pandas as pd
+
+import plotly.graph_objects as go
+import plotly.express as px
+from plotly.subplots import make_subplots
+import plotly.io as pio
+
+import dash
+from dash import Input, Output, State, callback_context as ctx
+from dash import dcc
+from dash import html
+import dash_daq as daq
+
+from types import SimpleNamespace
+import sys
+
+pio.renderers.default = "browser"
+tm = tb.Terminal()
+_ = Input, Output, State, dcc, html, daq
+_ = go, px, make_subplots
+
+
+CONFIG = SimpleNamespace(displayModeBar=True,  # always visible.
+                         staticPlot=False,
+                         scrollZoom=False,
+                         doubleClick="reset",
+                         showTips=True,
+                         toImageButtonOptions={
+                             'format': 'png',  # one of png, svg, jpeg, webp
+                             'filename': 'custom_image',
+                             'height': 1500,  # None means use currently rendered size.
+                             'width': 1500,
+                             'scale': 1  # Multiply title/legend/axis/canvas sizes by this factor
+                         },
+                         modeBarButtonsToAdd=['drawline',
+                                              'drawopenpath',
+                                              'drawclosedpath',
+                                              'drawcircle',
+                                              'drawrect',
+                                              'eraseshape']
+                         )
+
+
+class App:
+    @staticmethod
+    def run(app, debug=False, random_port=True):
+        host = "127.0.0.1"
+        port = tb.randstr(lower=False, upper=False, length=4) if random_port else "8050"  # Random ports prevent multile programs from crashing into each other.
+        # pynoinspection HTTP
+        tb.P(rf'http://{host}:{port}/')()
+        app.run_server(debug=debug, port=port)  # , processes=2, threaded=False)
+
+    @staticmethod
+    def get_app(name=""): return dash.Dash(name=name+tb.randstr(), external_stylesheets=[r'https://codepen.io/chriddyp/pen/bWLwgP.css'])
+
+    @staticmethod
+    def run_async_decorator(func):  # Decorate functions with this to make them run_command asynchornously."""
+        raise NotImplementedError
+
+
+if __name__ == '__main__':
+    pass
```

### Comparing `crocodile-8.40/myresources/crocodile/run.py` & `crocodile-9.0/myresources/crocodile/run.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,90 +1,90 @@
-
-"""
-Argument Parsing:
-* Script level.
-    * This is system dependent and is hard in bash.
-    * It remains a necessity because at system level one can dictate the enviroment, the interpretor, etc.
-* Python level:
-    * system agnostic.
-    * Benign syntax, but predetermines to a great extent what is being executed (which python, enviroment).
-* python library `fire`:
-    * this is good for passing arguments to specfic python functions from commandline without writing specific argparsing for those functions.
-
-The best approach is to use python and fire to pass process args of script and:
-   * return a string to the script file to execute it.
-   * or, execute it via terminal from within python.
-
-Choices made by default:
-* ipython over python
-* interactive is the default
-* importing the file to be run (as opposed to running it as main) is the default. The advantage of running it as an imported module is having reference to the file from which classes came. This is vital for pickling.
-
-"""
-
-# import crocodile.toolbox as tb
-import argparse
-import subprocess
-import platform
-from pathlib import Path
-
-
-def build_parser():
-    parser = argparse.ArgumentParser(description="Generic Parser to launch crocodile shell.")
-
-    # POSITIONAL ARGUMENT (UNNAMED)
-    # if dest is not specified, then, it has same path as keyword, e.g. "--dest"
-    # parser.add_argument("--file", "-f", dest="file", help="Python file path.", default="")
-
-    # A FLAG:
-    parser.add_argument("--module", '-m', help="Flag tells to run the file as main.", action="store_true", default=False)  # default is running as main, unless indicated by --module flag.
-    parser.add_argument("--newWindow", "-w", help="Flag for running in new window.", action="store_true", default=False)
-    parser.add_argument("--nonInteratctive", "-N", help="Specify a non-interactive session.", action="store_true", default=False)
-    parser.add_argument("--python", "-p", help="Use python over IPython.", action="store_true", default=False)
-
-    # OPTIONAL KEYWORD
-    parser.add_argument("--file", "-f", dest="file", help="Python file path.", default="")
-    parser.add_argument("--func", "-F", dest="func", help=f"function to be run after import", default="")
-    parser.add_argument("--cmd", "-c", dest="cmd", help="Python command.", default="")
-    parser.add_argument("--read", "-r", dest="read", help="Read file", default="")
-    parser.add_argument("--terminal", "-t", dest="terminal",  help=f"Flag to specify which terminal to be used. Default console host.", default="")  # can choose `wt`
-    parser.add_argument("--shell", "-S", dest="shell", help=f"Flag to specify which terminal to be used. Default CMD.", default="")
-
-    args = parser.parse_args()
-    # print(f"Crocodile.run: args of the firing command = {args.__dict__}")
-
-    # ==================================================================================
-    # flags processing
-    interactivity = '' if args.nonInteratctive else '-i'
-    interpreter = 'python' if args.python else 'ipython'
-
-    if args.file != "":
-        file = Path(args.file).expanduser().absolute()
-        if not args.module: res = f"{interpreter} {interactivity} {file}"
-        else:  # run as a module (i.e. import it)
-            script = fr"""
-from {file} import *
-args.cmd"""
-            if args.func != "": script += f"tb.E.capture_locals({args.func}, globals())"
-            res = f"{interpreter} {interactivity} {script}"
-    elif args.cmd != "":
-        # res = f""" python -c "from crocodile.toolbox import *; import crocodile.environment as env; {args.cmd}" """
-        import textwrap
-        code = f"from crocodile.toolbox import *\n{textwrap.dedent(args.cmd)}"
-        # print(code)
-        exec(code)
-        return None
-    elif args.read != "":
-        c = f"""p = P(r\'{str(args.read).lstrip()}\').absolute(); dat = tb.E.try_this(lambda: p.readit(), verbose=True) """
-        res = f"""ipython --no-banner -i -m crocodile.croshell -- -c "{c}" """
-    else:
-        res = f"{interpreter} {interactivity} --no-banner -m crocodile.croshell"  # --term-title croshell
-        # Clear-Host;
-        # # --autocall 1 in order to enable shell-like behaviour: e.g.: P x is interpreted as P(x)
-
-    # print(res)
-    if platform.system() == "Windows": return subprocess.run([f"powershell", "-Command", res], shell=True, capture_output=False, text=True)
-    else: return subprocess.run([res], shell=True, capture_output=False, text=True)
-
-
-if __name__ == "__main__":
-    build_parser()
+
+"""
+Argument Parsing:
+* Script level.
+    * This is system dependent and is hard in bash.
+    * It remains a necessity because at system level one can dictate the enviroment, the interpretor, etc.
+* Python level:
+    * system agnostic.
+    * Benign syntax, but predetermines to a great extent what is being executed (which python, enviroment).
+* python library `fire`:
+    * this is good for passing arguments to specfic python functions from commandline without writing specific argparsing for those functions.
+
+The best approach is to use python and fire to pass process args of script and:
+   * return a string to the script file to execute it.
+   * or, execute it via terminal from within python.
+
+Choices made by default:
+* ipython over python
+* interactive is the default
+* importing the file to be run (as opposed to running it as main) is the default. The advantage of running it as an imported module is having reference to the file from which classes came. This is vital for pickling.
+
+"""
+
+# import crocodile.toolbox as tb
+import argparse
+import subprocess
+import platform
+from pathlib import Path
+
+
+def build_parser():
+    parser = argparse.ArgumentParser(description="Generic Parser to launch crocodile shell.")
+
+    # POSITIONAL ARGUMENT (UNNAMED)
+    # if dest is not specified, then, it has same path as keyword, e.g. "--dest"
+    # parser.add_argument("--file", "-f", dest="file", help="Python file path.", default="")
+
+    # A FLAG:
+    parser.add_argument("--module", '-m', help="Flag tells to run the file as main.", action="store_true", default=False)  # default is running as main, unless indicated by --module flag.
+    parser.add_argument("--newWindow", "-w", help="Flag for running in new window.", action="store_true", default=False)
+    parser.add_argument("--nonInteratctive", "-N", help="Specify a non-interactive session.", action="store_true", default=False)
+    parser.add_argument("--python", "-p", help="Use python over IPython.", action="store_true", default=False)
+
+    # OPTIONAL KEYWORD
+    parser.add_argument("--file", "-f", dest="file", help="Python file path.", default="")
+    parser.add_argument("--func", "-F", dest="func", help=f"function to be run after import", default="")
+    parser.add_argument("--cmd", "-c", dest="cmd", help="Python command.", default="")
+    parser.add_argument("--read", "-r", dest="read", help="Read file", default="")
+    parser.add_argument("--terminal", "-t", dest="terminal",  help=f"Flag to specify which terminal to be used. Default console host.", default="")  # can choose `wt`
+    parser.add_argument("--shell", "-S", dest="shell", help=f"Flag to specify which terminal to be used. Default CMD.", default="")
+
+    args = parser.parse_args()
+    # print(f"Crocodile.run: args of the firing command = {args.__dict__}")
+
+    # ==================================================================================
+    # flags processing
+    interactivity = '' if args.nonInteratctive else '-i'
+    interpreter = 'python' if args.python else 'ipython'
+
+    if args.file != "":
+        file = Path(args.file).expanduser().absolute()
+        if not args.module: res = f"{interpreter} {interactivity} {file}"
+        else:  # run as a module (i.e. import it)
+            script = fr"""
+from {file} import *
+args.cmd"""
+            if args.func != "": script += f"tb.E.capture_locals({args.func}, globals())"
+            res = f"{interpreter} {interactivity} {script}"
+    elif args.cmd != "":
+        # res = f""" python -c "from crocodile.toolbox import *; import crocodile.environment as env; {args.cmd}" """
+        import textwrap
+        code = f"from crocodile.toolbox import *\n{textwrap.dedent(args.cmd)}"
+        # print(code)
+        exec(code)
+        return None
+    elif args.read != "":
+        c = f"""p = P(r\'{str(args.read).lstrip()}\').absolute(); dat = tb.E.try_this(lambda: p.readit(), verbose=True) """
+        res = f"""ipython --no-banner -i -m crocodile.croshell -- -c "{c}" """
+    else:
+        res = f"{interpreter} {interactivity} --no-banner -m crocodile.croshell"  # --term-title croshell
+        # Clear-Host;
+        # # --autocall 1 in order to enable shell-like behaviour: e.g.: P x is interpreted as P(x)
+
+    # print(res)
+    if platform.system() == "Windows": return subprocess.run([f"powershell", "-Command", res], shell=True, capture_output=False, text=True)
+    else: return subprocess.run([res], shell=True, capture_output=False, text=True)
+
+
+if __name__ == "__main__":
+    build_parser()
```

### Comparing `crocodile-8.40/myresources/crocodile/toolbox.py` & `crocodile-9.0/myresources/crocodile/toolbox.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,53 +1,53 @@
-
-"""
-A collection of classes extending the functionality of Python's builtins.
-author: Alex Al-Saffar
-email: programmer@usa.com
-
-This is `export file` where one can dictate what will be exposed with toolbox
-"""
-
-from crocodile import core
-from crocodile import meta
-from crocodile import file_management as _fm
-# from crocodile import run
-
-# CORE =====================================
-str2timedelta, timestamp, randstr, validate_name, install_n_import, get_env = core.str2timedelta, core.timestamp, core.randstr, core.validate_name, core.install_n_import, core.get_env
-Base, Struct, Display, Save, List = core.Base, core.Struct, core.Display, core.Save, core.List
-# File Management ==========================
-P, Read, Compression, Cache, encrypt, decrypt, modify_text = _fm.P, _fm.Read, _fm.Compression, _fm.Cache, _fm.encrypt, _fm.decrypt, _fm.modify_text
-# META =====================================
-Experimental, Terminal, Log, Null, Scheduler, SSH = meta.Experimental, meta.Terminal, meta.Log, meta.Null, meta.Scheduler, meta.SSH
-
-Path = P
-L = List
-S = Struct
-D = Display
-T = Terminal
-E = Experimental
-tmp = P.tmp
-
-_ = Base, timestamp, Save, Terminal, List, Struct, Display, P, Read, Compression, Experimental
-# from crocodile.core import datetime, dt, os, sys, string, random, np, copy, dill
-logging, subprocess, sys, time = meta.logging, meta.subprocess, meta.sys, meta.time
-datetime = _fm.datetime
-
-
-# _ = False
-# if _:
-#     from crocodile import matplotlib_management as _pm
-#     from crocodile.matplotlib_management import plt, enum, FigureManager
-#
-#     Artist, FigurePolicy, ImShow, FigureSave = _pm.Artist, _pm.FigurePolicy, _pm.ImShow, _pm.FigureSave
-#     VisibilityViewer, VisibilityViewerAuto = _pm.VisibilityViewer, _pm.VisibilityViewerAuto
-#
-#     _ = plt, enum, FigureManager, FigurePolicy, ImShow, FigureSave, VisibilityViewer, VisibilityViewerAuto, Artist
-#
-#     import pandas as pd
-#     _ = pd
-
-
-if __name__ == '__main__':
-    # get_parser()
-    pass
+
+"""
+A collection of classes extending the functionality of Python's builtins.
+author: Alex Al-Saffar
+email: programmer@usa.com
+
+This is `export file` where one can dictate what will be exposed with toolbox
+"""
+
+from crocodile import core
+from crocodile import meta
+from crocodile import file_management as _fm
+# from crocodile import run
+
+# CORE =====================================
+str2timedelta, timestamp, randstr, validate_name, install_n_import, get_env = core.str2timedelta, core.timestamp, core.randstr, core.validate_name, core.install_n_import, core.get_env
+Base, Struct, Display, Save, List = core.Base, core.Struct, core.Display, core.Save, core.List
+# File Management ==========================
+P, Read, Compression, Cache, encrypt, decrypt, modify_text = _fm.P, _fm.Read, _fm.Compression, _fm.Cache, _fm.encrypt, _fm.decrypt, _fm.modify_text
+# META =====================================
+Experimental, Terminal, Log, Null, Scheduler, SSH = meta.Experimental, meta.Terminal, meta.Log, meta.Null, meta.Scheduler, meta.SSH
+
+Path = P
+L = List
+S = Struct
+D = Display
+T = Terminal
+E = Experimental
+tmp = P.tmp
+
+_ = Base, timestamp, Save, Terminal, List, Struct, Display, P, Read, Compression, Experimental
+# from crocodile.core import datetime, dt, os, sys, string, random, np, copy, dill
+logging, subprocess, sys, time = meta.logging, meta.subprocess, meta.sys, meta.time
+datetime = _fm.datetime
+
+
+# _ = False
+# if _:
+#     from crocodile import matplotlib_management as _pm
+#     from crocodile.matplotlib_management import plt, enum, FigureManager
+#
+#     Artist, FigurePolicy, ImShow, FigureSave = _pm.Artist, _pm.FigurePolicy, _pm.ImShow, _pm.FigureSave
+#     VisibilityViewer, VisibilityViewerAuto = _pm.VisibilityViewer, _pm.VisibilityViewerAuto
+#
+#     _ = plt, enum, FigureManager, FigurePolicy, ImShow, FigureSave, VisibilityViewer, VisibilityViewerAuto, Artist
+#
+#     import pandas as pd
+#     _ = pd
+
+
+if __name__ == '__main__':
+    # get_parser()
+    pass
```

### Comparing `crocodile-8.40/myresources/crocodile.egg-info/PKG-INFO` & `crocodile-9.0/myresources/crocodile.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,116 +1,118 @@
-Metadata-Version: 2.1
-Name: crocodile
-Version: 8.40
-Summary: Making Python even more convenient by extending list and dict and pathlib and more.
-Home-page: https://github.com/thisismygitrepo/crocodile
-Author: Alex Al-Saffar
-Author-email: programmer@usa.com
-License: Apache 2.0
-Project-URL: Bug Tracker, https://github.com/thisismygitrepo/crocodile/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: license.txt
-
-
-# Welcome to crocodile
-
-Crocodile is a library aiming at facilitating the use of Python in scripting, thus, offering an alternative to `PowerShell` & `Bash` which have absurdly complex commands that are nothing but jumble of ad-hoc developments piled over decades to save some programmers a key stroke or two. This heritage poses huge burden on the people coming into the computer science field. A full rant bashing those shells by `Brian Will` [is here](<https://www.youtube.com/watch?v=L9v4Mg8wi4U`>).
-
-The core rationale is:
-* No one has the time to listen to hours long tutorials on how powerful and versatile `ls` or `grep` are, let alone keeping the random syntax in mind (unless used on daily basis). 
-* Python shell on the other hand, offers benign syntax and eminent readibility but it comes at the rather hefty cost of terseness, or the lack of it. For example, to make up for just `ls`, you need to import some libraries and it will eventually set you back a couple of lines of code. That's not acceptable for the simple task of listing directory contents, let alone a task of compressing a directory.
-* Crocodile comes here to make Python terser and friendlier by offering functionality for everyday use, like **file management, SSH, enviroment variables management, etc**. In essence, croshell to IPython is what IPython to Python shell is; that is, the basic Python shell that can only do arithmetic is turbo-boosted making it perfect for everyday errands.
-* The library, if used in coding, will fill your life with one-liners, take your code to artistic level of brevity and readability while simultaneously being more productive by typing less boilerplate lines of code that are needless to say.
-
-The name `crocodile` signifies the use of brute force in its implementation. The focus is on ease of use, as oppoesd to beating the existing shells in speed.
-Mind you, speed is not an issue in 99% of everyday chores.
-`Crocodile` designed carefully to be loved, learning curve cound't be flattened further.
-
-This package extends many native Python classes to equip you with an uneasy-to-tame power. The major classes extended are:
-
- * `pathlib.Path` is  extended to `P`
-      * Forget about importing all the **archaic** Python libraries `os`, `glob`, `shutil`, `sys`, `zipfile` etc. `P` makes the path an object, not a lame string. `P` objects are incredibly powerful for parsing paths, *no* more than one line of code is required to do **any** operation. Take a squint at this:
-      ```
-   path = P("dataset/type1/meta/images/file3.ext")
-     >> path[0]  # allows indexing! makes sense, hah?
-      P("dataset")
-     >> path[-1]  # nifty!
-      P("file3.ext")
-     >> path[2:-1]  # even slicing!
-      P("meta/images/file3.ext")
-   ```
- * `list` is  extended to `List`
-   * Forget that `for` loops exist, because with this class, `for` loops are implicitly used to apply a function to all items.
-     Inevitably while programming, one will encounter objects of the same type and you will be struggling to get a tough grab on them.  `List` is a powerful structure that put at your disposal a grip, so tough, that the objects you have at hand start behaving like one object. Behaviour is ala-JavaScript implementation of ``forEach`` method of Arrays.
-
- * `dict` is  extended to `Struct`.
-     * Combines the power of dot notation like classes and key access like dictionaries.
-
- * Additionally, the package provides many other new classes, e.g. `Read` and `Save`. Together with `P`, they provide comprehensive support for file management. Life cannot get easier with those. Every class inherits attributes that allow saving and loading in one line.
-
-   
-Furthermore, those classes are inextricably connected. For example, globbing a path `P` object returns a `List` object. You can move back and forth between `List` and `Struct` and `DataFrame` with one method, and so on.
-
-* Deep Learning Modules.
-  * A paradigm that facilitates working with deep learning models that is based on a tri-partite scheme:
-    * HyperParameters: facilitated through `HParams` class.
-    * Data: facilitated though `DataReader` class.
-    * `BaseModel` is a frontend for both `TensorFlow` & `Pytorch` backends. The wrapper worked in tandem.
-  * The aforementioned classes cooperate together to offer sealmess workflow during creation, training, and saving models.
-
-
-# Install
-In the commandline:
-`pip install crocodile`.
-
-Being a thin extension on top of almost pure Python, you need to worry **not** about your venv, the package is not aggressive in requirements, it installs itself peacefully, never interfere with your other packages. If you do not have `numpy`, `matplotlib` and `pandas`, it simply throws `ImportError` at runtime, that's it.
-
-[comment]: # (The package is not fussy about versions either. It can though at runtime, install packages on the fly, e.g. `dill` and `tqdm` which are very lightweight libraries.)
-
-# Install Croshell Terminal
-For `Windows` machines, run the following in elevated `PowerShell`:
-```ps1
-Invoke-WebRequest https://github.com/thisismygitrepo/machineconfig/src/machineconfig/setup_windows/croshell.ps1 | Invoke-Expression
-```
-
-# Getting Started
-That's as easy as taking candy from a baby; whenever you start a Python file, preface it with following in order to unleash the library:
-
-```
-import crocodile.toolbox as tb
-```
-
-
-# A Taste of Power
-EX1: Get a list of `.exe` available in terminal.
-
-     P.env().Path.search('*.exe').reduce(lambda x, y: x+y).print()
-
-EX2: Suppose you want to know how many lines of code in your repository. The procedure is to glob all `.py` files recursively, read string code, split each one of them by lines, count the lines, add up everything from all strings of code.
-
-
-To achieve this, all you need is an eminently readable one-liner.
-```
-tb.P.cwd().search("*.py", r=True).read_text().split('\n').apply(len).to_numpy().sum()
-```
-
-How does this make perfect sense?
-* `search` returns `List` of `P` path objects
-* `read_text` is a `P` method, but it is being run against `List` object. Behind the scenes, **responsible black magic** fails to find such a method in `List` and realizes it is a method of items inside the list, so it runs it against them and thus read all files and containerize them in another `List` object and returns it.
-* A similar story applies to `split` which is a method of strings in Python.
-* Next, `apply` is a method of `List`. Sure enough, it lives up to its apt name and applies the passed function `len` to all items in the list and returns another `List` object that contains the results.
-* `.to_numpy()` converts `List` to `numpy` array, then `.sum` is a method of `numpy`, which gives the final result.
-
-Methods naming convention like `apply` and `to_numpy` are inspired from the popular `pandas` library, resulting in almost non-existing learning curve.
-
-# Friendly interactive tutorial.
-Please refer to [Here](<https://github.com/thisismygitrepo/crocodile/blob/master/tutorial.ipynb>) on the main git repo.
-
-# Full docs:
-Click [Here](<https://crocodile.readthedocs.io/en/latest/>)
-
-# Author
-Alex Al-Saffar. [email](mailto:programmer@usa.com)
+Metadata-Version: 2.1
+Name: crocodile
+Version: 9.0
+Summary: Making Python even more convenient by extending list and dict and pathlib and more.
+Home-page: https://github.com/thisismygitrepo/crocodile
+Author: Alex Al-Saffar
+Author-email: programmer@usa.com
+License: Apache 2.0
+Project-URL: Bug Tracker, https://github.com/thisismygitrepo/crocodile/issues
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
+
+# Welcome to crocodile
+
+Crocodile is a library aiming at facilitating the use of Python in scripting, thus, offering an alternative to `PowerShell` & `Bash` which have absurdly complex commands that are nothing but jumble of ad-hoc developments piled over decades to save some programmers a key stroke or two. This heritage poses huge burden on the people coming into the computer science field. A full rant bashing those shells by `Brian Will` [is here](<https://www.youtube.com/watch?v=L9v4Mg8wi4U`>).
+
+The core rationale is:
+* No one has the time to listen to hours long tutorials on how powerful and versatile `ls` or `grep` are, let alone keeping the random syntax in mind (unless used on daily basis). 
+* Python shell on the other hand, offers benign syntax and eminent readibility but it comes at the rather hefty cost of terseness, or the lack of it. For example, to make up for just `ls`, you need to import some libraries and it will eventually set you back a couple of lines of code. That's not acceptable for the simple task of listing directory contents, let alone a task of compressing a directory.
+* Crocodile comes here to make Python terser and friendlier by offering functionality for everyday use, like **file management, SSH, enviroment variables management, etc**. In essence, croshell to IPython is what IPython to Python shell is; that is, the basic Python shell that can only do arithmetic is turbo-boosted making it perfect for everyday errands.
+* The library, if used in coding, will fill your life with one-liners, take your code to artistic level of brevity and readability while simultaneously being more productive by typing less boilerplate lines of code that are needless to say.
+
+The name `crocodile` signifies the use of brute force in its implementation. The focus is on ease of use, as oppoesd to beating the existing shells in speed.
+Mind you, speed is not an issue in 99% of everyday chores.
+`Crocodile` designed carefully to be loved, learning curve cound't be flattened further.
+
+This package extends many native Python classes to equip you with an uneasy-to-tame power. The major classes extended are:
+
+ * `pathlib.Path` is  extended to `P`
+      * Forget about importing all the **archaic** Python libraries `os`, `glob`, `shutil`, `sys`, `zipfile` etc. `P` makes the path an object, not a lame string. `P` objects are incredibly powerful for parsing paths, *no* more than one line of code is required to do **any** operation. Take a squint at this:
+      ```
+   path = P("dataset/type1/meta/images/file3.ext")
+     >> path[0]  # allows indexing! makes sense, hah?
+      P("dataset")
+     >> path[-1]  # nifty!
+      P("file3.ext")
+     >> path[2:-1]  # even slicing!
+      P("meta/images/file3.ext")
+   ```
+ * `list` is  extended to `List`
+   * Forget that `for` loops exist, because with this class, `for` loops are implicitly used to apply a function to all items.
+     Inevitably while programming, one will encounter objects of the same type and you will be struggling to get a tough grab on them.  `List` is a powerful structure that put at your disposal a grip, so tough, that the objects you have at hand start behaving like one object. Behaviour is ala-JavaScript implementation of ``forEach`` method of Arrays.
+
+ * `dict` is  extended to `Struct`.
+     * Combines the power of dot notation like classes and key access like dictionaries.
+
+ * Additionally, the package provides many other new classes, e.g. `Read` and `Save`. Together with `P`, they provide comprehensive support for file management. Life cannot get easier with those. Every class inherits attributes that allow saving and loading in one line.
+
+   
+Furthermore, those classes are inextricably connected. For example, globbing a path `P` object returns a `List` object. You can move back and forth between `List` and `Struct` and `DataFrame` with one method, and so on.
+
+* Deep Learning Modules.
+  * A paradigm that facilitates working with deep learning models that is based on a tri-partite scheme:
+    * HyperParameters: facilitated through `HParams` class.
+    * Data: facilitated though `DataReader` class.
+    * `BaseModel` is a frontend for both `TensorFlow` & `Pytorch` backends. The wrapper worked in tandem.
+  * The aforementioned classes cooperate together to offer sealmess workflow during creation, training, and saving models.
+
+
+# Install
+In the commandline:
+`pip install crocodile`.
+
+Being a thin extension on top of almost pure Python, you need to worry **not** about your venv, the package is not aggressive in requirements, it installs itself peacefully, never interfere with your other packages. If you do not have `numpy`, `matplotlib` and `pandas`, it simply throws `ImportError` at runtime, that's it.
+
+[comment]: # (The package is not fussy about versions either. It can though at runtime, install packages on the fly, e.g. `dill` and `tqdm` which are very lightweight libraries.)
+
+# Install Croshell Terminal
+For `Windows` machines, run the following in elevated `PowerShell`:
+```ps1
+Invoke-WebRequest https://github.com/thisismygitrepo/machineconfig/src/machineconfig/setup_windows/croshell.ps1 | Invoke-Expression
+```
+
+# Getting Started
+That's as easy as taking candy from a baby; whenever you start a Python file, preface it with following in order to unleash the library:
+
+```
+import crocodile.toolbox as tb
+```
+
+
+# A Taste of Power
+EX1: Get a list of `.exe` available in terminal.
+
+     P.env().Path.search('*.exe').reduce(lambda x, y: x+y).print()
+
+EX2: Suppose you want to know how many lines of code in your repository. The procedure is to glob all `.py` files recursively, read string code, split each one of them by lines, count the lines, add up everything from all strings of code.
+
+
+To achieve this, all you need is an eminently readable one-liner.
+```
+tb.P.cwd().search("*.py", r=True).read_text().split('\n').apply(len).to_numpy().sum()
+```
+
+How does this make perfect sense?
+* `search` returns `List` of `P` path objects
+* `read_text` is a `P` method, but it is being run against `List` object. Behind the scenes, **responsible black magic** fails to find such a method in `List` and realizes it is a method of items inside the list, so it runs it against them and thus read all files and containerize them in another `List` object and returns it.
+* A similar story applies to `split` which is a method of strings in Python.
+* Next, `apply` is a method of `List`. Sure enough, it lives up to its apt name and applies the passed function `len` to all items in the list and returns another `List` object that contains the results.
+* `.to_numpy()` converts `List` to `numpy` array, then `.sum` is a method of `numpy`, which gives the final result.
+
+Methods naming convention like `apply` and `to_numpy` are inspired from the popular `pandas` library, resulting in almost non-existing learning curve.
+
+# Friendly interactive tutorial.
+Please refer to [Here](<https://github.com/thisismygitrepo/crocodile/blob/master/tutorial.ipynb>) on the main git repo.
+
+# Full docs:
+Click [Here](<https://crocodile.readthedocs.io/en/latest/>)
+
+# Author
+Alex Al-Saffar. [email](mailto:programmer@usa.com)
+
+
```

