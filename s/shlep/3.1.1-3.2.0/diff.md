# Comparing `tmp/shlep-3.1.1.tar.gz` & `tmp/shlep-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shlep-3.1.1.tar", last modified: Sat May 27 20:30:01 2023, max compression
+gzip compressed data, was "shlep-3.2.0.tar", last modified: Fri Jun  9 19:44:12 2023, max compression
```

## Comparing `shlep-3.1.1.tar` & `shlep-3.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11349 2023-05-21 19:33:44.704545 shlep-3.1.1/LICENSE
--rw-r--r--   0        0        0     2332 2023-05-27 20:10:45.441977 shlep-3.1.1/README.md
--rw-r--r--   0        0        0      454 2023-05-27 20:30:01.598827 shlep-3.1.1/pyproject.toml
--rw-r--r--   0        0        0       24 2023-05-27 20:10:45.436465 shlep-3.1.1/shlep/__init__.py
--rw-r--r--   0        0        0     3763 2023-05-27 20:29:44.925163 shlep-3.1.1/shlep/main.py
--rw-r--r--   0        0        0     2613 1970-01-01 00:00:00.000000 shlep-3.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11349 2023-05-21 19:33:44.704545 shlep-3.2.0/LICENSE
+-rw-r--r--   0        0        0     2332 2023-05-27 20:10:45.441977 shlep-3.2.0/README.md
+-rw-r--r--   0        0        0      454 2023-06-09 19:44:12.557191 shlep-3.2.0/pyproject.toml
+-rw-r--r--   0        0        0       24 2023-05-27 20:10:45.436465 shlep-3.2.0/shlep/__init__.py
+-rw-r--r--   0        0        0     4412 2023-06-09 19:42:51.131437 shlep-3.2.0/shlep/main.py
+-rw-r--r--   0        0        0     2613 1970-01-01 00:00:00.000000 shlep-3.2.0/PKG-INFO
```

### Comparing `shlep-3.1.1/LICENSE` & `shlep-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `shlep-3.1.1/README.md` & `shlep-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `shlep-3.1.1/shlep/main.py` & `shlep-3.2.0/shlep/main.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,44 +1,56 @@
 import argparse
+import fnmatch
 import json
 import logging
 import os
 from pathlib import Path
 
 from pathspec import PathSpec
 
 DEFAULT_EXCLUDED = [".git", ".idea"]
 
 logger = logging.getLogger(__name__)
 
 
-def _is_excluded(base: Path, path: Path, spec: PathSpec = None):
+def _is_excluded(base: Path, path: Path, spec: PathSpec = None, only_patterns=None):
+    path_relative_to_base = str(path.relative_to(base))
+
+    if only_patterns:
+        if any(path_relative_to_base == pattern for pattern in only_patterns):
+            return False
+        else:
+            return True
+
     if not spec:
         return True
-    return spec.match_file(str(path.relative_to(base)))
+
+    return spec.match_file(path_relative_to_base)
 
 
 def shlep(
     directory: Path | str,
     indent: int | None,
     additional_excludes: list[str],
     output_format: str,
     output_file: Path | str = None,
     quiet=False,
+    only_patterns=None,
 ) -> str:
     """
     Generate a file of all files in a directory.
 
     Args:
         directory: The directory to analyze.
         indent: The number of spaces to use for indentation in the output JSON.
         additional_excludes: Additional files or directories to exclude.
         output_format: The output format. Can be 'json', 'csv', or 'plaintext'. Default is 'json'.
         output_file: The output file to generate. If not specified, output is printed to stdout.
         quiet: don't print output to stdout
+        only_patterns: Only include files that match any of the specified patterns.
 
     Returns (str):
         output
     """
     files_list = []
     base = Path(directory).expanduser()
 
@@ -51,15 +63,15 @@
             "gitwildmatch",
             DEFAULT_EXCLUDED + additional_excludes,
         )
     else:
         spec = None
 
     for path in base.rglob("*"):
-        if path.is_file() and not _is_excluded(base, path, spec):
+        if path.is_file() and not _is_excluded(base, path, spec, only_patterns):
             try:
                 content = path.read_text()
             except UnicodeDecodeError:
                 logger.error(f"Could not read {path}")
             else:
                 files_list.append({"path": str(path), "content": content})
 
@@ -115,14 +127,28 @@
     parser.add_argument(
         "-f",
         "--format",
         choices=["json", "plaintext"],
         default="json",
         help="The output format. Can be 'json' or 'plaintext'. Default is 'json'.",
     )
+    parser.add_argument(
+        "-y",
+        "--only",
+        type=str,
+        action="append",
+        help="Only include files that match this pattern. Can be used multiple times.",
+    )
     args = parser.parse_args()
     excluded = args.exclude or []
-    shlep(args.directory, args.indent, excluded, args.format, args.output_file)
+    shlep(
+        args.directory,
+        args.indent,
+        excluded,
+        args.format,
+        args.output_file,
+        only_patterns=args.only,
+    )
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `shlep-3.1.1/PKG-INFO` & `shlep-3.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shlep
-Version: 3.1.1
+Version: 3.2.0
 Summary: gather directory contents into a single file
 Author-Email: Stephan Fitzpatrick <knowsuchagency@gmail.com>
 License: Apache-2.0
 Requires-Python: >=3.10
 Requires-Dist: pathspec>=0.11.1
 Description-Content-Type: text/markdown
```

