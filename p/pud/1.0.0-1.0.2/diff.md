# Comparing `tmp/pud-1.0.0-py3-none-any.whl.zip` & `tmp/pud-1.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 6363 bytes, number of entries: 12
+Zip file size: 6374 bytes, number of entries: 12
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-07 14:07 pud/__init__.py
--rw-rw-rw-  2.0 fat      100 b- defN 23-Jun-09 12:33 pud/__main__.py
+-rw-rw-rw-  2.0 fat      100 b- defN 23-Jun-09 12:58 pud/__main__.py
 -rw-rw-rw-  2.0 fat     8009 b- defN 23-Jun-09 11:22 pud/app.py
 -rw-rw-rw-  2.0 fat      779 b- defN 23-Jun-09 08:33 pud/entity.py
 -rw-rw-rw-  2.0 fat      285 b- defN 23-Jun-08 15:03 pud/main.py
--rw-rw-rw-  2.0 fat      545 b- defN 23-Jun-08 14:59 pud/options.py
--rw-rw-rw-  2.0 fat     1070 b- defN 23-Jun-09 12:34 pud-1.0.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      973 b- defN 23-Jun-09 12:34 pud-1.0.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-09 12:34 pud-1.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       39 b- defN 23-Jun-09 12:34 pud-1.0.0.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        4 b- defN 23-Jun-09 12:34 pud-1.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      868 b- defN 23-Jun-09 12:34 pud-1.0.0.dist-info/RECORD
-12 files, 12764 bytes uncompressed, 4923 bytes compressed:  61.4%
+-rw-rw-rw-  2.0 fat      545 b- defN 23-Jun-09 12:58 pud/options.py
+-rw-rw-rw-  2.0 fat     1070 b- defN 23-Jun-09 13:02 pud-1.0.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      997 b- defN 23-Jun-09 13:02 pud-1.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-09 13:02 pud-1.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       39 b- defN 23-Jun-09 13:02 pud-1.0.2.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        4 b- defN 23-Jun-09 13:02 pud-1.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      868 b- defN 23-Jun-09 13:02 pud-1.0.2.dist-info/RECORD
+12 files, 12788 bytes uncompressed, 4934 bytes compressed:  61.4%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: pud/main.py
 Comment: 
 
 Filename: pud/options.py
 Comment: 
 
-Filename: pud-1.0.0.dist-info/LICENSE
+Filename: pud-1.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: pud-1.0.0.dist-info/METADATA
+Filename: pud-1.0.2.dist-info/METADATA
 Comment: 
 
-Filename: pud-1.0.0.dist-info/WHEEL
+Filename: pud-1.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: pud-1.0.0.dist-info/entry_points.txt
+Filename: pud-1.0.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: pud-1.0.0.dist-info/top_level.txt
+Filename: pud-1.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: pud-1.0.0.dist-info/RECORD
+Filename: pud-1.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pud/__main__.py

```diff
@@ -1,7 +1,7 @@
-# For using python -m pod
+# For using python -m pud
 
 from pud.main import main
 
 
 if __name__ == "__main__":
     main()
```

## pud/options.py

```diff
@@ -1,14 +1,14 @@
 import argparse
 from typing import Sequence
 
 
 def get_args(argv: Sequence[str]):
     parser = argparse.ArgumentParser(
-        prog="pod",
+        prog="pud",
         allow_abbrev=False
     )
 
     parser.add_argument(
         "--cursor",
         default="=>",
         help="The cursor to use."
```

## Comparing `pud-1.0.0.dist-info/LICENSE` & `pud-1.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pud-1.0.0.dist-info/METADATA` & `pud-1.0.2.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,49 +1,48 @@
 Metadata-Version: 2.1
 Name: pud
-Version: 1.0.0
+Version: 1.0.2
 Summary: A command-line tool for navigating directories.
-Home-page: https://github.com/Jedddy/pod
+Home-page: https://github.com/Jedddy/pud
 Author: Jedddy
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: windows-curses (==2.3.1)
+Requires-Dist: windows-curses (==2.3.1) ; sys_platform == "win32"
 
 
-Pod
+Pud
 ===
-Pod is a mini command-line tool to navigate directories.
+Pud is a mini command-line tool to navigate directories.
 
 Installation
 ===
 ```
-git clone https://github.com/Jedddy/pod.git
+git clone https://github.com/Jedddy/pud.git
 
 python setup.py install
 ```
 
 Usage
 ===
 ```
-pod [arguments]
-
+pud [arguments]
 ```
 
 Options
 ===
 Currently there are 2 options:
 - cursor: The cursor you want to use.
     ```
-    pod --cursor=">>>"
+    pud --cursor=">>>"
     ```
 - no-keep-state: Whether not to keep the state of your cursor after entering/leaving a directory
     ```
-    pod --no-keep-state
+    pud --no-keep-state
     ```
```

