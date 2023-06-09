# Comparing `tmp/manytasks-2.1.tar.gz` & `tmp/manytasks-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manytasks-2.1.tar", last modified: Mon Apr 24 10:18:52 2023, max compression
+gzip compressed data, was "manytasks-2.2.tar", last modified: Fri Jun  9 13:00:05 2023, max compression
```

## Comparing `manytasks-2.1.tar` & `manytasks-2.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 admin      (502) staff       (20)        0 2023-04-24 10:18:52.343328 manytasks-2.1/
--rw-r--r--   0 admin      (502) staff       (20)     4716 2023-04-24 10:18:52.342670 manytasks-2.1/PKG-INFO
--rw-r--r--   0 admin      (502) staff       (20)     4406 2023-04-24 10:18:06.000000 manytasks-2.1/README.md
-drwxr-xr-x   0 admin      (502) staff       (20)        0 2023-04-24 10:18:52.333900 manytasks-2.1/manytasks/
--rw-r--r--   0 admin      (502) staff       (20)        0 2021-10-01 08:51:25.000000 manytasks-2.1/manytasks/__init__.py
--rw-r--r--   0 admin      (502) staff       (20)      550 2022-07-12 12:41:21.000000 manytasks-2.1/manytasks/cuda_manager.py
--rw-r--r--   0 admin      (502) staff       (20)     4914 2023-04-24 10:18:06.000000 manytasks-2.1/manytasks/defs.py
--rw-r--r--   0 admin      (502) staff       (20)     8321 2022-12-21 16:04:37.000000 manytasks-2.1/manytasks/entry.py
--rw-r--r--   0 admin      (502) staff       (20)     3897 2022-05-09 13:45:49.000000 manytasks-2.1/manytasks/log_extractor.py
--rw-r--r--   0 admin      (502) staff       (20)     5249 2023-04-24 10:18:06.000000 manytasks-2.1/manytasks/task_runner.py
--rw-r--r--   0 admin      (502) staff       (20)     7448 2023-04-24 10:18:06.000000 manytasks-2.1/manytasks/taskpool_loader.py
--rw-r--r--   0 admin      (502) staff       (20)     3668 2023-04-24 10:18:06.000000 manytasks-2.1/manytasks/util.py
-drwxr-xr-x   0 admin      (502) staff       (20)        0 2023-04-24 10:18:52.340008 manytasks-2.1/manytasks.egg-info/
--rw-r--r--   0 admin      (502) staff       (20)     4716 2023-04-24 10:18:51.000000 manytasks-2.1/manytasks.egg-info/PKG-INFO
--rw-r--r--   0 admin      (502) staff       (20)      434 2023-04-24 10:18:52.000000 manytasks-2.1/manytasks.egg-info/SOURCES.txt
--rw-r--r--   0 admin      (502) staff       (20)        1 2023-04-24 10:18:51.000000 manytasks-2.1/manytasks.egg-info/dependency_links.txt
--rw-r--r--   0 admin      (502) staff       (20)       51 2023-04-24 10:18:51.000000 manytasks-2.1/manytasks.egg-info/entry_points.txt
--rw-r--r--   0 admin      (502) staff       (20)        1 2022-07-03 02:41:06.000000 manytasks-2.1/manytasks.egg-info/not-zip-safe
--rw-r--r--   0 admin      (502) staff       (20)       39 2023-04-24 10:18:52.000000 manytasks-2.1/manytasks.egg-info/requires.txt
--rw-r--r--   0 admin      (502) staff       (20)       10 2023-04-24 10:18:52.000000 manytasks-2.1/manytasks.egg-info/top_level.txt
--rw-r--r--   0 admin      (502) staff       (20)       38 2023-04-24 10:18:52.343678 manytasks-2.1/setup.cfg
--rw-r--r--   0 admin      (502) staff       (20)      844 2023-04-24 10:18:06.000000 manytasks-2.1/setup.py
+drwxr-xr-x   0 admin      (502) staff       (20)        0 2023-06-09 13:00:05.266114 manytasks-2.2/
+-rw-r--r--   0 admin      (502) staff       (20)     5047 2023-06-09 13:00:05.265687 manytasks-2.2/PKG-INFO
+-rw-r--r--   0 admin      (502) staff       (20)     4737 2023-06-07 06:11:51.000000 manytasks-2.2/README.md
+drwxr-xr-x   0 admin      (502) staff       (20)        0 2023-06-09 13:00:05.255393 manytasks-2.2/manytasks/
+-rw-r--r--   0 admin      (502) staff       (20)        0 2021-10-01 08:51:25.000000 manytasks-2.2/manytasks/__init__.py
+-rw-r--r--   0 admin      (502) staff       (20)      550 2022-07-12 12:41:21.000000 manytasks-2.2/manytasks/cuda_manager.py
+-rw-r--r--   0 admin      (502) staff       (20)     4914 2023-04-24 10:18:06.000000 manytasks-2.2/manytasks/defs.py
+-rw-r--r--   0 admin      (502) staff       (20)     8321 2022-12-21 16:04:37.000000 manytasks-2.2/manytasks/entry.py
+-rw-r--r--   0 admin      (502) staff       (20)     3897 2022-05-09 13:45:49.000000 manytasks-2.2/manytasks/log_extractor.py
+-rw-r--r--   0 admin      (502) staff       (20)     5249 2023-04-24 10:18:06.000000 manytasks-2.2/manytasks/task_runner.py
+-rw-r--r--   0 admin      (502) staff       (20)     8172 2023-06-07 06:10:50.000000 manytasks-2.2/manytasks/taskpool_loader.py
+-rw-r--r--   0 admin      (502) staff       (20)     3668 2023-04-24 10:18:06.000000 manytasks-2.2/manytasks/util.py
+drwxr-xr-x   0 admin      (502) staff       (20)        0 2023-06-09 13:00:05.264768 manytasks-2.2/manytasks.egg-info/
+-rw-r--r--   0 admin      (502) staff       (20)     5047 2023-06-09 13:00:04.000000 manytasks-2.2/manytasks.egg-info/PKG-INFO
+-rw-r--r--   0 admin      (502) staff       (20)      434 2023-06-09 13:00:04.000000 manytasks-2.2/manytasks.egg-info/SOURCES.txt
+-rw-r--r--   0 admin      (502) staff       (20)        1 2023-06-09 13:00:04.000000 manytasks-2.2/manytasks.egg-info/dependency_links.txt
+-rw-r--r--   0 admin      (502) staff       (20)       51 2023-06-09 13:00:04.000000 manytasks-2.2/manytasks.egg-info/entry_points.txt
+-rw-r--r--   0 admin      (502) staff       (20)        1 2022-07-03 02:41:06.000000 manytasks-2.2/manytasks.egg-info/not-zip-safe
+-rw-r--r--   0 admin      (502) staff       (20)       39 2023-06-09 13:00:04.000000 manytasks-2.2/manytasks.egg-info/requires.txt
+-rw-r--r--   0 admin      (502) staff       (20)       10 2023-06-09 13:00:04.000000 manytasks-2.2/manytasks.egg-info/top_level.txt
+-rw-r--r--   0 admin      (502) staff       (20)       38 2023-06-09 13:00:05.266285 manytasks-2.2/setup.cfg
+-rw-r--r--   0 admin      (502) staff       (20)      844 2023-06-07 05:45:54.000000 manytasks-2.2/setup.py
```

### Comparing `manytasks-2.1/PKG-INFO` & `manytasks-2.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manytasks
-Version: 2.1
+Version: 2.2
 Summary: A tool for deploying many tasks automatically.
 Home-page: https://github.com/dugu9sword/manytasks
 Author: dugu9sword
 Author-email: dugu9sword@163.com
 License: WTFPL Licence
 Keywords: manytasks
 Platform: any
@@ -105,14 +105,17 @@
 The syntax sugar makes the enumeration of arguments more easier.
 
 | Type                     | Example Input                | Example Output                             |
 | ------------------------ | ---------------------------- | ------------------------------------------ |
 | **list**                 | `$<1:6>`                     | `[1, 2, 3, 4, 5]`                          |
 | **list** (with step)     | `$<1:6:2>`                   | `[1, 3, 5]`                                |
 | **list** (with zero-pad) | `$<1:6:2;3>`                | `[001, 003, 005]`                          |
+| **files**                | `$<files:/home/*.py>`       | `[/home/foo.py, /home/bar.py, ...]`                     |
+| **files** (without path) | `$<files:/home/*.py;nameonly>`  | `[foo.py, bar.py, ...]`                     |
+| **lines**                | `$<lines:urls.txt>`         | `[baidu.com, google.com, ...]`              |
 | **set**          | `$<a\|b\|c>`               | `[a, b, c]`                                |
 | **composition** | `x_$<1:3;3>.txt` | `[x_001.txt, x_002.txt]` |
 | **composition** (more) | `logs/$<a\|b>.$<1:3>`         | `[logs/a.1, logs/a.2, logs/b.1, logs/b.2]` |
```

### Comparing `manytasks-2.1/README.md` & `manytasks-2.2/manytasks.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: manytasks
+Version: 2.2
+Summary: A tool for deploying many tasks automatically.
+Home-page: https://github.com/dugu9sword/manytasks
+Author: dugu9sword
+Author-email: dugu9sword@163.com
+License: WTFPL Licence
+Keywords: manytasks
+Platform: any
+Description-Content-Type: text/markdown
+
 # Manytasks
 
 A lightweight tool for deploying many tasks automatically, without any modification to your code.
 
 - [Manytasks](#manytasks)
   - [Installation](#installation)
   - [Quick Example](#quick-example)
@@ -93,14 +105,17 @@
 The syntax sugar makes the enumeration of arguments more easier.
 
 | Type                     | Example Input                | Example Output                             |
 | ------------------------ | ---------------------------- | ------------------------------------------ |
 | **list**                 | `$<1:6>`                     | `[1, 2, 3, 4, 5]`                          |
 | **list** (with step)     | `$<1:6:2>`                   | `[1, 3, 5]`                                |
 | **list** (with zero-pad) | `$<1:6:2;3>`                | `[001, 003, 005]`                          |
+| **files**                | `$<files:/home/*.py>`       | `[/home/foo.py, /home/bar.py, ...]`                     |
+| **files** (without path) | `$<files:/home/*.py;nameonly>`  | `[foo.py, bar.py, ...]`                     |
+| **lines**                | `$<lines:urls.txt>`         | `[baidu.com, google.com, ...]`              |
 | **set**          | `$<a\|b\|c>`               | `[a, b, c]`                                |
 | **composition** | `x_$<1:3;3>.txt` | `[x_001.txt, x_002.txt]` |
 | **composition** (more) | `logs/$<a\|b>.$<1:3>`         | `[logs/a.1, logs/a.2, logs/b.1, logs/b.2]` |
 
 
 
 
@@ -124,7 +139,9 @@
 ## Analysis
 
 See `Analysis.md`.
 
 ## History
 
 See `History.md`.
+
+
```

### Comparing `manytasks-2.1/manytasks/cuda_manager.py` & `manytasks-2.2/manytasks/cuda_manager.py`

 * *Files identical despite different names*

### Comparing `manytasks-2.1/manytasks/defs.py` & `manytasks-2.2/manytasks/defs.py`

 * *Files identical despite different names*

### Comparing `manytasks-2.1/manytasks/entry.py` & `manytasks-2.2/manytasks/entry.py`

 * *Files identical despite different names*

### Comparing `manytasks-2.1/manytasks/log_extractor.py` & `manytasks-2.2/manytasks/log_extractor.py`

 * *Files identical despite different names*

### Comparing `manytasks-2.1/manytasks/task_runner.py` & `manytasks-2.2/manytasks/task_runner.py`

 * *Files identical despite different names*

### Comparing `manytasks-2.1/manytasks/taskpool_loader.py` & `manytasks-2.2/manytasks/taskpool_loader.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import itertools
 import re
+import os
+import glob
 from typing import List, Tuple
 from collections import defaultdict
 
 import jstyleson
 
 from manytasks.defs import Arg, Reserved, Task, TaskPool
 
@@ -99,15 +101,15 @@
             # Case I
             #   $<?>
             if enum_repr.strip() == "$<?>":
                 enum_list = [Reserved.ON, Reserved.OFF]
                 break
 
             # Case II
-            #   $<start:end:[step]:[zfill]>
+            #   $<start:end:[step];[zfill]>
             found = re.search(r"^(-?\d+)(:-?\d+)(:-?\d+)?(;\d+)?$", enum_repr[2:-1])
             if found:
                 start = int(found.group(1))
                 end = int(found.group(2)[1:])
                 step = int(found.group(3)[1:]) if found.group(3) else None
                 zero_num = int(found.group(4)[1:]) if found.group(4) else None
                 if step:
@@ -123,15 +125,31 @@
             # Case III
             #   $<a|b|c|d>
             found = re.search(r"^([^|]+\|)+[^|]+$", enum_repr[2:-1])
             if found:
                 enum_list = enum_repr[2:-1].split("|")
                 break
 
-            break
+            # Case IV
+            #   $<files:manytasks/*.py>
+            found = re.search(r"^files:([^;]*)(;nameonly)?$", enum_repr[2:-1])
+            if found:
+                enum_list = glob.glob(found.group(1))
+                if found.group(2) is not None:
+                    enum_list = [os.path.basename(ele) for ele in enum_list]
+                break
+
+            # Case V
+            #   $<lines:lines.txt>
+            found = re.search(r"^lines:(.*)$", enum_repr[2:-1])
+            if found:
+                enum_list = open(found.group(1)).readlines()
+                enum_list = [ele.strip() for ele in enum_list]
+                enum_list = [ele for ele in enum_list if ele != ""]
+                break
 
         string = string[:enum_start] + f"#ENUM<{enum_idx}>" + string[enum_end:]
         enum_lists.append(enum_list)
         enum_idx += 1
         
     # Step 2. expand the string to list
     if enum_idx == 0:
```

### Comparing `manytasks-2.1/manytasks/util.py` & `manytasks-2.2/manytasks/util.py`

 * *Files identical despite different names*

### Comparing `manytasks-2.1/manytasks.egg-info/PKG-INFO` & `manytasks-2.2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: manytasks
-Version: 2.1
-Summary: A tool for deploying many tasks automatically.
-Home-page: https://github.com/dugu9sword/manytasks
-Author: dugu9sword
-Author-email: dugu9sword@163.com
-License: WTFPL Licence
-Keywords: manytasks
-Platform: any
-Description-Content-Type: text/markdown
-
 # Manytasks
 
 A lightweight tool for deploying many tasks automatically, without any modification to your code.
 
 - [Manytasks](#manytasks)
   - [Installation](#installation)
   - [Quick Example](#quick-example)
@@ -105,14 +93,17 @@
 The syntax sugar makes the enumeration of arguments more easier.
 
 | Type                     | Example Input                | Example Output                             |
 | ------------------------ | ---------------------------- | ------------------------------------------ |
 | **list**                 | `$<1:6>`                     | `[1, 2, 3, 4, 5]`                          |
 | **list** (with step)     | `$<1:6:2>`                   | `[1, 3, 5]`                                |
 | **list** (with zero-pad) | `$<1:6:2;3>`                | `[001, 003, 005]`                          |
+| **files**                | `$<files:/home/*.py>`       | `[/home/foo.py, /home/bar.py, ...]`                     |
+| **files** (without path) | `$<files:/home/*.py;nameonly>`  | `[foo.py, bar.py, ...]`                     |
+| **lines**                | `$<lines:urls.txt>`         | `[baidu.com, google.com, ...]`              |
 | **set**          | `$<a\|b\|c>`               | `[a, b, c]`                                |
 | **composition** | `x_$<1:3;3>.txt` | `[x_001.txt, x_002.txt]` |
 | **composition** (more) | `logs/$<a\|b>.$<1:3>`         | `[logs/a.1, logs/a.2, logs/b.1, logs/b.2]` |
 
 
 
 
@@ -136,9 +127,7 @@
 ## Analysis
 
 See `Analysis.md`.
 
 ## History
 
 See `History.md`.
-
-
```

### Comparing `manytasks-2.1/setup.py` & `manytasks-2.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="manytasks",
-    version="2.1",
+    version="2.2",
     keywords=["manytasks", ],
     description="A tool for deploying many tasks automatically.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     license="WTFPL Licence",
 
     url="https://github.com/dugu9sword/manytasks",
```

