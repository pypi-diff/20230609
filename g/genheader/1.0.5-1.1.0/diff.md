# Comparing `tmp/genheader-1.0.5.tar.gz` & `tmp/genheader-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genheader-1.0.5.tar", last modified: Fri Jun  9 15:54:44 2023, max compression
+gzip compressed data, was "genheader-1.1.0.tar", last modified: Fri Jun  9 16:31:55 2023, max compression
```

## Comparing `genheader-1.0.5.tar` & `genheader-1.1.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 maplepy   (1000) maplepy   (1000)        0 2023-06-09 15:54:44.009114 genheader-1.0.5/
--rw-r--r--   0 maplepy   (1000) maplepy   (1000)     1211 2023-06-09 13:13:26.000000 genheader-1.0.5/LICENSE
--rw-r--r--   0 maplepy   (1000) maplepy   (1000)      987 2023-06-09 15:54:44.009114 genheader-1.0.5/PKG-INFO
--rw-r--r--   0 maplepy   (1000) maplepy   (1000)      491 2023-06-09 15:53:09.000000 genheader-1.0.5/README.md
--rw-r--r--   0 maplepy   (1000) maplepy   (1000)      103 2023-06-09 13:13:26.000000 genheader-1.0.5/pyproject.toml
--rw-r--r--   0 maplepy   (1000) maplepy   (1000)      676 2023-06-09 15:54:44.010115 genheader-1.0.5/setup.cfg
-drwxr-xr-x   0 maplepy   (1000) maplepy   (1000)        0 2023-06-09 15:54:44.004114 genheader-1.0.5/src/
-drwxr-xr-x   0 maplepy   (1000) maplepy   (1000)        0 2023-06-09 15:54:44.006115 genheader-1.0.5/src/genheader/
--rw-r--r--   0 maplepy   (1000) maplepy   (1000)      974 2023-06-09 15:42:14.000000 genheader-1.0.5/src/genheader/__init__.py
--rwxr-xr-x   0 maplepy   (1000) maplepy   (1000)      974 2023-06-09 15:42:14.000000 genheader-1.0.5/src/genheader/__main__.py
--rw-r--r--   0 maplepy   (1000) maplepy   (1000)      149 2023-06-09 15:42:14.000000 genheader-1.0.5/src/genheader/_version.py
-drwxr-xr-x   0 maplepy   (1000) maplepy   (1000)        0 2023-06-09 15:54:44.007115 genheader-1.0.5/src/genheader/injector/
--rw-r--r--   0 maplepy   (1000) maplepy   (1000)       39 2023-06-09 14:24:09.000000 genheader-1.0.5/src/genheader/injector/__init__.py
--rw-r--r--   0 maplepy   (1000) maplepy   (1000)     2857 2023-06-09 15:42:14.000000 genheader-1.0.5/src/genheader/injector/headers.py
-drwxr-xr-x   0 maplepy   (1000) maplepy   (1000)        0 2023-06-09 15:54:44.008114 genheader-1.0.5/src/genheader/proto/
--rw-r--r--   0 maplepy   (1000) maplepy   (1000)      110 2023-06-09 15:42:14.000000 genheader-1.0.5/src/genheader/proto/__init__.py
--rw-r--r--   0 maplepy   (1000) maplepy   (1000)     3619 2023-06-09 15:42:14.000000 genheader-1.0.5/src/genheader/proto/protos.py
--rw-r--r--   0 maplepy   (1000) maplepy   (1000)     3697 2023-06-09 15:42:14.000000 genheader-1.0.5/src/genheader/proto/sources.py
-drwxr-xr-x   0 maplepy   (1000) maplepy   (1000)        0 2023-06-09 15:54:44.009114 genheader-1.0.5/src/genheader/utils/
--rw-r--r--   0 maplepy   (1000) maplepy   (1000)      157 2023-06-09 14:34:32.000000 genheader-1.0.5/src/genheader/utils/__init__.py
--rw-r--r--   0 maplepy   (1000) maplepy   (1000)     1262 2023-06-09 15:42:14.000000 genheader-1.0.5/src/genheader/utils/arg_parsing.py
--rw-r--r--   0 maplepy   (1000) maplepy   (1000)      639 2023-06-09 14:35:05.000000 genheader-1.0.5/src/genheader/utils/colors.py
--rw-r--r--   0 maplepy   (1000) maplepy   (1000)      715 2023-06-09 14:35:14.000000 genheader-1.0.5/src/genheader/utils/regexrules.py
--rw-r--r--   0 maplepy   (1000) maplepy   (1000)      644 2023-06-09 15:42:14.000000 genheader-1.0.5/src/genheader/utils/utils.py
-drwxr-xr-x   0 maplepy   (1000) maplepy   (1000)        0 2023-06-09 15:54:44.007115 genheader-1.0.5/src/genheader.egg-info/
--rw-r--r--   0 maplepy   (1000) maplepy   (1000)      987 2023-06-09 15:54:43.000000 genheader-1.0.5/src/genheader.egg-info/PKG-INFO
--rw-r--r--   0 maplepy   (1000) maplepy   (1000)      649 2023-06-09 15:54:44.000000 genheader-1.0.5/src/genheader.egg-info/SOURCES.txt
--rw-r--r--   0 maplepy   (1000) maplepy   (1000)        1 2023-06-09 15:54:43.000000 genheader-1.0.5/src/genheader.egg-info/dependency_links.txt
--rw-r--r--   0 maplepy   (1000) maplepy   (1000)       45 2023-06-09 15:54:43.000000 genheader-1.0.5/src/genheader.egg-info/entry_points.txt
--rw-r--r--   0 maplepy   (1000) maplepy   (1000)       10 2023-06-09 15:54:43.000000 genheader-1.0.5/src/genheader.egg-info/top_level.txt
-drwxr-xr-x   0 maplepy   (1000) maplepy   (1000)        0 2023-06-09 15:54:44.009114 genheader-1.0.5/test/
--rw-r--r--   0 maplepy   (1000) maplepy   (1000)      344 2023-06-09 15:42:14.000000 genheader-1.0.5/test/test_proto.py
+drwxr-xr-x   0 maplepy   (1000) maplepy   (1000)        0 2023-06-09 16:31:55.742474 genheader-1.1.0/
+-rw-r--r--   0 maplepy   (1000) maplepy   (1000)     1211 2023-06-09 13:13:26.000000 genheader-1.1.0/LICENSE
+-rw-r--r--   0 maplepy   (1000) maplepy   (1000)      986 2023-06-09 16:31:55.742474 genheader-1.1.0/PKG-INFO
+-rw-r--r--   0 maplepy   (1000) maplepy   (1000)      491 2023-06-09 16:07:33.000000 genheader-1.1.0/README.md
+-rw-r--r--   0 maplepy   (1000) maplepy   (1000)      103 2023-06-09 13:13:26.000000 genheader-1.1.0/pyproject.toml
+-rw-r--r--   0 maplepy   (1000) maplepy   (1000)      675 2023-06-09 16:31:55.742474 genheader-1.1.0/setup.cfg
+drwxr-xr-x   0 maplepy   (1000) maplepy   (1000)        0 2023-06-09 16:31:55.739474 genheader-1.1.0/src/
+drwxr-xr-x   0 maplepy   (1000) maplepy   (1000)        0 2023-06-09 16:31:55.740474 genheader-1.1.0/src/genheader/
+-rw-r--r--   0 maplepy   (1000) maplepy   (1000)      989 2023-06-09 16:29:58.000000 genheader-1.1.0/src/genheader/__init__.py
+-rwxr-xr-x   0 maplepy   (1000) maplepy   (1000)       87 2023-06-09 16:20:28.000000 genheader-1.1.0/src/genheader/__main__.py
+-rw-r--r--   0 maplepy   (1000) maplepy   (1000)      159 2023-06-09 16:25:35.000000 genheader-1.1.0/src/genheader/_version.py
+drwxr-xr-x   0 maplepy   (1000) maplepy   (1000)        0 2023-06-09 16:31:55.741474 genheader-1.1.0/src/genheader/injector/
+-rw-r--r--   0 maplepy   (1000) maplepy   (1000)       39 2023-06-09 16:20:28.000000 genheader-1.1.0/src/genheader/injector/__init__.py
+-rw-r--r--   0 maplepy   (1000) maplepy   (1000)     2862 2023-06-09 16:29:58.000000 genheader-1.1.0/src/genheader/injector/headers.py
+drwxr-xr-x   0 maplepy   (1000) maplepy   (1000)        0 2023-06-09 16:31:55.741474 genheader-1.1.0/src/genheader/proto/
+-rw-r--r--   0 maplepy   (1000) maplepy   (1000)      115 2023-06-09 16:25:45.000000 genheader-1.1.0/src/genheader/proto/__init__.py
+-rw-r--r--   0 maplepy   (1000) maplepy   (1000)     3624 2023-06-09 16:29:58.000000 genheader-1.1.0/src/genheader/proto/protos.py
+-rw-r--r--   0 maplepy   (1000) maplepy   (1000)     3707 2023-06-09 16:29:58.000000 genheader-1.1.0/src/genheader/proto/sources.py
+drwxr-xr-x   0 maplepy   (1000) maplepy   (1000)        0 2023-06-09 16:31:55.742474 genheader-1.1.0/src/genheader/utils/
+-rw-r--r--   0 maplepy   (1000) maplepy   (1000)      157 2023-06-09 16:20:28.000000 genheader-1.1.0/src/genheader/utils/__init__.py
+-rw-r--r--   0 maplepy   (1000) maplepy   (1000)     1296 2023-06-09 16:29:58.000000 genheader-1.1.0/src/genheader/utils/arg_parsing.py
+-rw-r--r--   0 maplepy   (1000) maplepy   (1000)      639 2023-06-09 16:20:28.000000 genheader-1.1.0/src/genheader/utils/colors.py
+-rw-r--r--   0 maplepy   (1000) maplepy   (1000)      715 2023-06-09 16:20:28.000000 genheader-1.1.0/src/genheader/utils/regexrules.py
+-rw-r--r--   0 maplepy   (1000) maplepy   (1000)      649 2023-06-09 16:29:58.000000 genheader-1.1.0/src/genheader/utils/utils.py
+drwxr-xr-x   0 maplepy   (1000) maplepy   (1000)        0 2023-06-09 16:31:55.740474 genheader-1.1.0/src/genheader.egg-info/
+-rw-r--r--   0 maplepy   (1000) maplepy   (1000)      986 2023-06-09 16:31:55.000000 genheader-1.1.0/src/genheader.egg-info/PKG-INFO
+-rw-r--r--   0 maplepy   (1000) maplepy   (1000)      649 2023-06-09 16:31:55.000000 genheader-1.1.0/src/genheader.egg-info/SOURCES.txt
+-rw-r--r--   0 maplepy   (1000) maplepy   (1000)        1 2023-06-09 16:31:55.000000 genheader-1.1.0/src/genheader.egg-info/dependency_links.txt
+-rw-r--r--   0 maplepy   (1000) maplepy   (1000)       45 2023-06-09 16:31:55.000000 genheader-1.1.0/src/genheader.egg-info/entry_points.txt
+-rw-r--r--   0 maplepy   (1000) maplepy   (1000)       10 2023-06-09 16:31:55.000000 genheader-1.1.0/src/genheader.egg-info/top_level.txt
+drwxr-xr-x   0 maplepy   (1000) maplepy   (1000)        0 2023-06-09 16:31:55.742474 genheader-1.1.0/test/
+-rw-r--r--   0 maplepy   (1000) maplepy   (1000)      349 2023-06-09 16:29:55.000000 genheader-1.1.0/test/test_proto.py
```

### Comparing `genheader-1.0.5/LICENSE` & `genheader-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `genheader-1.0.5/PKG-INFO` & `genheader-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: genheader
-Version: 1.0.5
+Version: 1.1.0
 Summary: A tool to inject prototypes into header from C files.
-Home-page: https://github.com/42-tronc/genheader
+Home-page: https://github.com/maplepy/genheader
 Author: maplepy
 Author-email: your-email@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.8.2
```

### Comparing `genheader-1.0.5/setup.cfg` & `genheader-1.1.0/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [metadata]
 name = genheader
-version = 1.0.5
+version = 1.1.0
 author = maplepy
 author_email = your-email@example.com
 description = A tool to inject prototypes into header from C files.
 long_description = file: README.md
 long_description_content_type = text/markdown
-url = https://github.com/42-tronc/genheader
+url = https://github.com/maplepy/genheader
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Development Status :: 3 - Alpha
 
 [options]
```

### Comparing `genheader-1.0.5/src/genheader/__init__.py` & `genheader-1.1.0/src/genheader/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from argparse import Namespace
 from pathlib import Path
 from sys import argv, stderr
 
-from hgen.injector import insert_prototypes
-from hgen.proto import get_prototypes
-from hgen.utils import create_parser, visualize
+from genheader.injector import insert_prototypes
+from genheader.proto import get_prototypes
+from genheader.utils import create_parser, visualize
 
 
 def update_header_prototypes(args: Namespace):
     prototypes: list[str] = []
 
     dest_path = args.includes
```

### Comparing `genheader-1.0.5/src/genheader/injector/headers.py` & `genheader-1.1.0/src/genheader/injector/headers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from pathlib import Path
 
-from hgen.utils import RegexRules, cstr, get_lines_from
+from genheader.utils import RegexRules, cstr, get_lines_from
 
 
 def get_flag_span(lines: "list[str]") -> "tuple[int, int]":
     """
     Find the beginning and end line indices of the function flag header.
 
     Args:
```

### Comparing `genheader-1.0.5/src/genheader/proto/protos.py` & `genheader-1.1.0/src/genheader/proto/protos.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 
 import re
 from dataclasses import dataclass, field
 from functools import cached_property
 from pathlib import Path
 
-from hgen.utils import RegexRules, cstr, get_lines_from
+from genheader.utils import RegexRules, cstr, get_lines_from
 from termcolor import cprint
 
 # _NAME_HEADER = "/*\n** < {filename} > */"
 _NAME_HEADER = "// {filename}"
 _COLOR_HEADER = "magenta"
 _COLOR_TYPE = "red"
 _COLOR_VAR = "blue"
```

### Comparing `genheader-1.0.5/src/genheader/proto/sources.py` & `genheader-1.1.0/src/genheader/proto/sources.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 
 from itertools import chain
 from pathlib import Path
 
-from hgen.proto import Protos
-from hgen.utils import TAB, cprint, cstr
+from genheader.proto import Protos
+from genheader.utils import TAB, cprint, cstr
 
 
 def _crawl_prototypes(src_path: Path) -> "list[Protos]":
     def crawl_file(src: Path):
         status, res = "green", ""
         try:
             target = Protos(src)
```

### Comparing `genheader-1.0.5/src/genheader/utils/arg_parsing.py` & `genheader-1.1.0/src/genheader/utils/arg_parsing.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from argparse import ArgumentParser
 from pathlib import Path
 
-from hgen._version import __version__
+from genheader._version import __version__
 
 from .utils import cstr
 
 
 def create_parser():
-    prog = "hgen"
+    prog = "genheader"
     parser = ArgumentParser(
         prog=prog,
         usage=f"{prog} [-hv] [-r] -I header.h [path ...]",
-        description=cstr("green", "HGEN: Header prototype GENerator"),
+        description=cstr("green", "genheader: Header prototype Generator (fixed by maplepy)"),
     )
     parser.add_argument(
         "-I",
         "--includes",
         type=Path,
         default=Path(".") / "includes",
         required=True,
```

### Comparing `genheader-1.0.5/src/genheader/utils/colors.py` & `genheader-1.1.0/src/genheader/utils/colors.py`

 * *Files identical despite different names*

### Comparing `genheader-1.0.5/src/genheader/utils/regexrules.py` & `genheader-1.1.0/src/genheader/utils/regexrules.py`

 * *Files identical despite different names*

### Comparing `genheader-1.0.5/src/genheader/utils/utils.py` & `genheader-1.1.0/src/genheader/utils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 
 from pathlib import Path
 
-from hgen.utils.colors import cstr
+from genheader.utils.colors import cstr
 
 TAB = "\t"
 
 
 # Function to read lines from a file
 def get_lines_from(file: Path) -> "list[str]":
     return file.read_text().splitlines(keepends=False)
```

### Comparing `genheader-1.0.5/src/genheader.egg-info/PKG-INFO` & `genheader-1.1.0/src/genheader.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: genheader
-Version: 1.0.5
+Version: 1.1.0
 Summary: A tool to inject prototypes into header from C files.
-Home-page: https://github.com/42-tronc/genheader
+Home-page: https://github.com/maplepy/genheader
 Author: maplepy
 Author-email: your-email@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.8.2
```

### Comparing `genheader-1.0.5/src/genheader.egg-info/SOURCES.txt` & `genheader-1.1.0/src/genheader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

