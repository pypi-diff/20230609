# Comparing `tmp/ptyx_mcq-23.3.tar.gz` & `tmp/ptyx_mcq-23.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptyx_mcq-23.3.tar", max compression
+gzip compressed data, was "ptyx_mcq-23.4.tar", max compression
```

## Comparing `ptyx_mcq-23.3.tar` & `ptyx_mcq-23.4.tar`

### file list

```diff
@@ -1,48 +1,49 @@
--rw-r--r--   0        0        0     1808 2023-03-23 17:40:29.535683 ptyx_mcq-23.3/README.md
--rw-r--r--   0        0        0    18095 2022-06-29 17:25:23.274035 ptyx_mcq-23.3/ptyx_mcq/TODO.odt
--rw-r--r--   0        0        0     4977 2023-04-05 08:34:46.410607 ptyx_mcq-23.3/ptyx_mcq/__init__.py
--rwxr-xr-x   0        0        0      342 2023-03-04 15:17:13.547850 ptyx_mcq-23.3/ptyx_mcq/bin/scan
--rwxr-xr-x   0        0        0    11772 2023-04-04 14:07:28.932523 ptyx_mcq-23.3/ptyx_mcq/cli.py
--rw-r--r--   0        0        0    24338 2023-02-25 11:03:57.366686 ptyx_mcq-23.3/ptyx_mcq/doc/algo_detection_carres.odt
--rw-r--r--   0        0        0     1644 2022-06-29 17:25:23.306035 ptyx_mcq-23.3/ptyx_mcq/doc/exemple
--rw-r--r--   0        0        0    73081 2022-06-29 17:25:23.306035 ptyx_mcq-23.3/ptyx_mcq/doc/exemple_complet_syntaxe.pdf
--rw-r--r--   0        0        0    10495 2022-06-29 17:25:23.306035 ptyx_mcq-23.3/ptyx_mcq/doc/exemple_complet_syntaxe.tex
--rw-r--r--   0        0        0   241779 2022-06-29 17:25:23.306035 ptyx_mcq-23.3/ptyx_mcq/doc/profiling.png
--rw-r--r--   0        0        0    39227 2022-06-29 17:25:23.306035 ptyx_mcq-23.3/ptyx_mcq/doc/structure_QCM.svg
--rw-r--r--   0        0        0   531437 2023-03-07 21:06:59.000000 ptyx_mcq-23.3/ptyx_mcq/dump.profile
--rw-r--r--   0        0        0        0 2022-06-29 17:25:23.290035 ptyx_mcq-23.3/ptyx_mcq/make/__init__.py
--rw-r--r--   0        0        0    27478 2023-04-05 07:01:41.289244 ptyx_mcq-23.3/ptyx_mcq/make/extend_latex_generator.py
--rw-r--r--   0        0        0     9110 2023-04-02 20:55:13.248834 ptyx_mcq-23.3/ptyx_mcq/make/generate_ptyx_code.py
--rw-r--r--   0        0        0    16375 2023-03-05 21:51:32.428518 ptyx_mcq-23.3/ptyx_mcq/make/header.py
--rw-r--r--   0        0        0     4830 2023-04-04 08:47:51.837278 ptyx_mcq-23.3/ptyx_mcq/make/make.py
--rw-r--r--   0        0        0      307 2022-07-09 20:44:53.565792 ptyx_mcq-23.3/ptyx_mcq/parameters.py
--rw-r--r--   0        0        0        0 2022-07-08 16:36:52.243505 ptyx_mcq-23.3/ptyx_mcq/py.typed
--rw-r--r--   0        0        0        0 2022-06-29 17:25:23.306035 ptyx_mcq-23.3/ptyx_mcq/scan/__init__.py
--rw-r--r--   0        0        0     5964 2023-04-04 13:36:57.967586 ptyx_mcq-23.3/ptyx_mcq/scan/amend.py
--rw-r--r--   0        0        0      372 2023-03-13 07:53:49.962584 ptyx_mcq-23.3/ptyx_mcq/scan/color.py
--rw-r--r--   0        0        0    10823 2023-04-01 20:24:32.499387 ptyx_mcq-23.3/ptyx_mcq/scan/conflict_solver.py
--rw-r--r--   0        0        0    11146 2023-04-04 13:35:02.378259 ptyx_mcq-23.3/ptyx_mcq/scan/data_manager.py
--rw-r--r--   0        0        0     1771 2023-04-01 09:43:02.922713 ptyx_mcq-23.3/ptyx_mcq/scan/document_data.py
--rw-r--r--   0        0        0     2592 2023-03-04 15:22:24.432458 ptyx_mcq-23.3/ptyx_mcq/scan/paths_handler.py
--rw-r--r--   0        0        0     4069 2022-07-09 09:29:03.618479 ptyx_mcq-23.3/ptyx_mcq/scan/pdftools.py
--rw-r--r--   0        0        0    22117 2023-04-04 15:53:22.506660 ptyx_mcq-23.3/ptyx_mcq/scan/scan.py
--rw-r--r--   0        0        0    43085 2023-04-04 08:47:27.149000 ptyx_mcq-23.3/ptyx_mcq/scan/scan_pic.py
--rw-r--r--   0        0        0     4614 2023-03-09 21:43:04.310039 ptyx_mcq-23.3/ptyx_mcq/scan/scores.py
--rw-r--r--   0        0        0    11595 2023-03-13 07:53:49.978584 ptyx_mcq-23.3/ptyx_mcq/scan/square_detection.py
--rw-r--r--   0        0        0     2600 2023-03-13 07:53:49.978584 ptyx_mcq-23.3/ptyx_mcq/scan/tools.py
--rw-r--r--   0        0        0    11770 2023-03-13 07:53:49.990584 ptyx_mcq-23.3/ptyx_mcq/scan/visual_debugging.py
--rw-r--r--   0        0        0      106 2022-06-30 12:30:07.506267 ptyx_mcq-23.3/ptyx_mcq/templates/original/README.txt
--rw-r--r--   0        0        0     1455 2023-03-27 17:36:33.950580 ptyx_mcq-23.3/ptyx_mcq/templates/original/new.ptyx
--rw-r--r--   0        0        0     1081 2023-02-25 11:03:57.438687 ptyx_mcq-23.3/ptyx_mcq/templates/original/questions/question1.ex
--rw-r--r--   0        0        0      185 2022-06-29 17:25:23.310035 ptyx_mcq-23.3/ptyx_mcq/templates/original/questions/question2.ex
--rw-r--r--   0        0        0     1581 2023-03-14 20:28:42.000810 ptyx_mcq-23.3/ptyx_mcq/templates/original/questions/question3.ex
--rw-r--r--   0        0        0      951 2023-04-02 20:47:16.530766 ptyx_mcq-23.3/ptyx_mcq/templates/original/questions/question4.ex
--rw-r--r--   0        0        0      172 2022-06-30 17:29:40.726022 ptyx_mcq-23.3/ptyx_mcq/templates/original/scan/README.txt
--rw-r--r--   0        0        0        0 2022-07-08 16:36:52.299506 ptyx_mcq-23.3/ptyx_mcq/tools/__init__.py
--rw-r--r--   0        0        0    13649 2023-04-04 13:36:58.151588 ptyx_mcq-23.3/ptyx_mcq/tools/config_parser.py
--rw-r--r--   0        0        0     3359 2023-04-01 14:58:06.224097 ptyx_mcq-23.3/ptyx_mcq/tools/extend_literal_eval.py
--rw-r--r--   0        0        0     8021 2023-03-28 13:06:34.679264 ptyx_mcq-23.3/ptyx_mcq/tools/include_parser.py
--rw-r--r--   0        0        0     3694 2023-03-13 07:53:50.014585 ptyx_mcq-23.3/ptyx_mcq/tools/io_tools.py
--rw-r--r--   0        0        0     3704 2022-07-08 16:55:19.450575 ptyx_mcq-23.3/ptyx_mcq/tools/scriptlib.py
--rw-r--r--   0        0        0     1461 2023-04-04 15:40:18.062176 ptyx_mcq-23.3/pyproject.toml
--rw-r--r--   0        0        0     2738 1970-01-01 00:00:00.000000 ptyx_mcq-23.3/PKG-INFO
+-rw-r--r--   0        0        0     1808 2023-03-23 17:40:29.000000 ptyx_mcq-23.4/README.md
+-rw-r--r--   0        0        0    18095 2022-06-29 17:25:23.274035 ptyx_mcq-23.4/ptyx_mcq/TODO.odt
+-rw-r--r--   0        0        0     5283 2023-04-11 14:47:37.481049 ptyx_mcq-23.4/ptyx_mcq/__init__.py
+-rwxr-xr-x   0        0        0      342 2023-03-04 15:17:13.547850 ptyx_mcq-23.4/ptyx_mcq/bin/scan
+-rwxr-xr-x   0        0        0    13042 2023-06-08 20:21:01.158124 ptyx_mcq-23.4/ptyx_mcq/cli.py
+-rw-r--r--   0        0        0    24338 2023-02-25 11:03:57.366686 ptyx_mcq-23.4/ptyx_mcq/doc/algo_detection_carres.odt
+-rw-r--r--   0        0        0     1644 2022-06-29 17:25:23.306035 ptyx_mcq-23.4/ptyx_mcq/doc/exemple
+-rw-r--r--   0        0        0    73081 2022-06-29 17:25:23.306035 ptyx_mcq-23.4/ptyx_mcq/doc/exemple_complet_syntaxe.pdf
+-rw-r--r--   0        0        0    10495 2022-06-29 17:25:23.306035 ptyx_mcq-23.4/ptyx_mcq/doc/exemple_complet_syntaxe.tex
+-rw-r--r--   0        0        0   241779 2022-06-29 17:25:23.306035 ptyx_mcq-23.4/ptyx_mcq/doc/profiling.png
+-rw-r--r--   0        0        0    39227 2022-06-29 17:25:23.306035 ptyx_mcq-23.4/ptyx_mcq/doc/structure_QCM.svg
+-rw-r--r--   0        0        0   531437 2023-03-07 21:06:59.000000 ptyx_mcq-23.4/ptyx_mcq/dump.profile
+-rw-r--r--   0        0        0        0 2022-06-29 17:25:23.290035 ptyx_mcq-23.4/ptyx_mcq/make/__init__.py
+-rw-r--r--   0        0        0    27139 2023-04-11 21:26:45.646334 ptyx_mcq-23.4/ptyx_mcq/make/extend_latex_generator.py
+-rw-r--r--   0        0        0     9161 2023-06-08 21:27:42.452677 ptyx_mcq-23.4/ptyx_mcq/make/generate_ptyx_code.py
+-rw-r--r--   0        0        0    16375 2023-03-05 21:51:32.428518 ptyx_mcq-23.4/ptyx_mcq/make/header.py
+-rw-r--r--   0        0        0     4830 2023-04-04 08:47:51.837278 ptyx_mcq-23.4/ptyx_mcq/make/make.py
+-rw-r--r--   0        0        0      307 2022-07-09 20:44:53.565792 ptyx_mcq-23.4/ptyx_mcq/parameters.py
+-rw-r--r--   0        0        0        0 2022-07-08 16:36:52.243505 ptyx_mcq-23.4/ptyx_mcq/py.typed
+-rw-r--r--   0        0        0        0 2022-06-29 17:25:23.306035 ptyx_mcq-23.4/ptyx_mcq/scan/__init__.py
+-rw-r--r--   0        0        0     5964 2023-04-04 13:36:57.967586 ptyx_mcq-23.4/ptyx_mcq/scan/amend.py
+-rw-r--r--   0        0        0      372 2023-03-13 07:53:49.962584 ptyx_mcq-23.4/ptyx_mcq/scan/color.py
+-rw-r--r--   0        0        0    10823 2023-04-01 20:24:32.499387 ptyx_mcq-23.4/ptyx_mcq/scan/conflict_solver.py
+-rw-r--r--   0        0        0    11146 2023-04-11 21:16:58.851420 ptyx_mcq-23.4/ptyx_mcq/scan/data_manager.py
+-rw-r--r--   0        0        0     1771 2023-04-01 09:43:02.922713 ptyx_mcq-23.4/ptyx_mcq/scan/document_data.py
+-rw-r--r--   0        0        0     8169 2023-04-13 16:20:10.373383 ptyx_mcq-23.4/ptyx_mcq/scan/evaluation_strategies.py
+-rw-r--r--   0        0        0     2674 2023-04-11 20:15:40.763369 ptyx_mcq-23.4/ptyx_mcq/scan/paths_handler.py
+-rw-r--r--   0        0        0     4069 2022-07-09 09:29:03.618479 ptyx_mcq-23.4/ptyx_mcq/scan/pdftools.py
+-rw-r--r--   0        0        0    17855 2023-04-12 07:34:08.816654 ptyx_mcq-23.4/ptyx_mcq/scan/scan.py
+-rw-r--r--   0        0        0    42849 2023-04-12 06:53:48.365783 ptyx_mcq-23.4/ptyx_mcq/scan/scan_pic.py
+-rw-r--r--   0        0        0     7477 2023-05-07 07:06:30.918642 ptyx_mcq-23.4/ptyx_mcq/scan/scores_manager.py
+-rw-r--r--   0        0        0    11595 2023-03-13 07:53:49.978584 ptyx_mcq-23.4/ptyx_mcq/scan/square_detection.py
+-rw-r--r--   0        0        0     2600 2023-03-13 07:53:49.978584 ptyx_mcq-23.4/ptyx_mcq/scan/tools.py
+-rw-r--r--   0        0        0     7636 2023-04-07 20:17:29.873231 ptyx_mcq-23.4/ptyx_mcq/scan/visual_debugging.py
+-rw-r--r--   0        0        0      106 2022-06-30 12:30:07.506267 ptyx_mcq-23.4/ptyx_mcq/templates/original/README.txt
+-rw-r--r--   0        0        0     1662 2023-04-12 09:58:51.452538 ptyx_mcq-23.4/ptyx_mcq/templates/original/new.ptyx
+-rw-r--r--   0        0        0     1081 2023-02-25 11:03:57.438687 ptyx_mcq-23.4/ptyx_mcq/templates/original/questions/question1.ex
+-rw-r--r--   0        0        0      185 2022-06-29 17:25:23.310035 ptyx_mcq-23.4/ptyx_mcq/templates/original/questions/question2.ex
+-rw-r--r--   0        0        0     1581 2023-03-14 20:28:42.000810 ptyx_mcq-23.4/ptyx_mcq/templates/original/questions/question3.ex
+-rw-r--r--   0        0        0      953 2023-06-08 21:26:37.795757 ptyx_mcq-23.4/ptyx_mcq/templates/original/questions/question4.ex
+-rw-r--r--   0        0        0      172 2022-06-30 17:29:40.726022 ptyx_mcq-23.4/ptyx_mcq/templates/original/scan/README.txt
+-rw-r--r--   0        0        0        0 2022-07-08 16:36:52.299506 ptyx_mcq-23.4/ptyx_mcq/tools/__init__.py
+-rw-r--r--   0        0        0    13811 2023-04-11 21:15:07.210104 ptyx_mcq-23.4/ptyx_mcq/tools/config_parser.py
+-rw-r--r--   0        0        0     3359 2023-04-01 14:58:06.224097 ptyx_mcq-23.4/ptyx_mcq/tools/extend_literal_eval.py
+-rw-r--r--   0        0        0     9861 2023-04-11 14:46:49.280474 ptyx_mcq-23.4/ptyx_mcq/tools/include_parser.py
+-rw-r--r--   0        0        0     4046 2023-04-12 09:32:03.535874 ptyx_mcq-23.4/ptyx_mcq/tools/io_tools.py
+-rw-r--r--   0        0        0     3704 2022-07-08 16:55:19.450575 ptyx_mcq-23.4/ptyx_mcq/tools/scriptlib.py
+-rw-r--r--   0        0        0     1508 2023-04-12 07:32:28.000000 ptyx_mcq-23.4/pyproject.toml
+-rw-r--r--   0        0        0     2779 1970-01-01 00:00:00.000000 ptyx_mcq-23.4/PKG-INFO
```

### Comparing `ptyx_mcq-23.3/README.md` & `ptyx_mcq-23.4/README.md`

 * *Files identical despite different names*

### Comparing `ptyx_mcq-23.3/ptyx_mcq/TODO.odt` & `ptyx_mcq-23.4/ptyx_mcq/TODO.odt`

 * *Files identical despite different names*

### Comparing `ptyx_mcq-23.3/ptyx_mcq/__init__.py` & `ptyx_mcq-23.4/ptyx_mcq/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -140,15 +140,22 @@
     #     2:  [          <-- test n°2
     #         [2,3,4],   <-- 1st question: list of correct answers
     #         [0],       <-- 2nd question: list of correct answers
     #         [1,2],     ...
     #         ],
     #    }
 
-    text = IncludeParser(compiler.dir_path).parse(text)
+    try:
+        text = IncludeParser(compiler.dir_path).parse(text, strict=True)
+    except FileNotFoundError:
+        print_error(
+            "File not found when trying to resolve inclusions (see error message above).\n"
+            f"Hint: command `mcq update-include {getattr(compiler.file_path, 'name', 'FILENAME')}` "
+            "may fix it."
+        )
     additional_header_lines = autodetect_smallgraphlib(text)
 
     # Call extended_python extension.
     text = extended_python.main(text, compiler)
 
     code = generate_ptyx_code(text, additional_header_lines=additional_header_lines)
     assert isinstance(code, str)
```

### Comparing `ptyx_mcq-23.3/ptyx_mcq/cli.py` & `ptyx_mcq-23.4/ptyx_mcq/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,39 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 ptyx MCQ Command Line Interface
 
 @author: Nicolas Pourcelot
 """
-import re
+
 import shutil
 import sys
 from argparse import ArgumentParser
 from os import unlink
 from pathlib import Path
 from typing import Optional
 
 from platformdirs import PlatformDirs
 from ptyx.latex_generator import compiler
 
 from ptyx_mcq import IncludeParser
+from ptyx_mcq.scan.evaluation_strategies import EvaluationStrategies
 from .make.make import make, parse_ptyx_file
 from .scan.scan import scan
 from .tools.config_parser import Configuration
-from .tools.io_tools import print_success, print_error, get_file_or_sysexit
+from .tools.io_tools import (
+    print_success,
+    print_error,
+    get_file_or_sysexit,
+    ANSI_RESET,
+    ANSI_REVERSE_PURPLE,
+    ANSI_REVERSE_BLUE,
+    ANSI_BLUE,
+)
 
 
 def main(args: Optional[list] = None) -> None:
     """Main entry point, called whenever `mcq` command is executed."""
     parser = ArgumentParser(description="Generate and manage pdf MCQs.")
     subparsers = parser.add_subparsers()
     add_parser = subparsers.add_parser
@@ -138,14 +147,18 @@
         metavar="NAME",
         type=str,
         default="default",
         help="The template name must be a valid directory name.",
     )
     create_template_parser.set_defaults(func=create_template)
 
+    # create the parser for the "strategies" command
+    strategies_parser = add_parser("strategies", help="List available evaluation strategies.")
+    strategies_parser.set_defaults(func=strategies)
+
     parsed_args = parser.parse_args(args)
     try:
         # Launch the function corresponding to the given subcommand.
         kwargs = vars(parsed_args)
         func = kwargs.pop("func")
     except KeyError:
         # No subcommand passed.
@@ -173,40 +186,42 @@
         sys.exit(1)
 
     # Create the new MCQ.
     if path.exists():
         print_error(f"Path {path} already exists.")
         sys.exit(1)
     else:
+        print(f"Using template from '{template_path}'.")
         shutil.copytree(template_path, path)
         if include is not None:
             # No need to have a questions directory template,
             # since questions' files will be explicitly listed.
-            assert (path / "questions").is_dir()
-            shutil.rmtree(path / "questions")
+            shutil.rmtree(path / "questions", ignore_errors=True)
             # Edit the .ptyx file, to replace default code with the list of the questions' files.
-            ptyx_path = (path / "new.ptyx").resolve()
-            assert ptyx_path.is_file(), ptyx_path
-            with open(ptyx_path, encoding="utf8") as f:
-                content = f.read()
-            lines = [f"-- ROOT: {include.resolve()}"]
+            ptyx_path = get_file_or_sysexit(path, extension=".ptyx")
+            new_lines = [f"-- ROOT: {include.resolve()}"]
             for include_path in include.glob("**/*.ex"):
-                lines.append(f"-- {include_path.relative_to(include)}")
-            assert "-- questions/**/*.ex" in content
-            start = "<<<<<<<<<<<<<<<<<"
-            end = ">>>>>>>>>>>>>>>>>"
-            files_listing = "\n".join(lines)
-            content = re.sub(
-                f"{start}(.+){end}",
-                f"{start}\n{files_listing}\n{end}",
-                content,
-                flags=re.MULTILINE | re.DOTALL,
-            )
+                new_lines.append(f"-- {include_path.relative_to(include)}")
+            lines = []
+            with open(ptyx_path, encoding="utf8") as f:
+                include_section = False
+                for line in f:
+                    line = line.rstrip("\n")
+                    if line.startswith("<<<<"):
+                        include_section = True
+                        lines.append(line)
+                        lines.extend(new_lines)
+                    elif line.startswith(">>>>"):
+                        include_section = False
+                        lines.append(line)
+                    elif not include_section:
+                        lines.append(line)
+
             with open(ptyx_path, "w", encoding="utf8") as f:
-                f.write(content)
+                f.write("\n".join(lines) + "\n")
         print_success(f"A new MCQ was created at {path}.")
 
 
 def clear(path: Path) -> None:
     """Implement `mcq clear` command."""
     ptyxfile_path = get_file_or_sysexit(path, extension=".ptyx")
     filename = ptyxfile_path.name
@@ -279,14 +294,30 @@
     """Update the list of included files."""
     ptyxfile_path = get_file_or_sysexit(path, extension=".ptyx")
     root = ptyxfile_path.parent
     IncludeParser(root).update(ptyxfile_path)
     print_success("The list of included files was successfully updated.")
 
 
+def strategies() -> None:
+    """Display all evaluation modes with a description."""
+    strategies = EvaluationStrategies.get_all_strategies()
+    print(f"\n{ANSI_REVERSE_PURPLE}[ Available strategies ]{ANSI_RESET}")
+    print(", ".join(strategies))
+    print()
+    print(f"\n{ANSI_REVERSE_PURPLE}[ Details ]{ANSI_RESET}")
+    for name in strategies:
+        print(f"\n {ANSI_BLUE}╭───╴{ANSI_RESET}{ANSI_REVERSE_BLUE} {name} {ANSI_RESET} ")
+        print(f" {ANSI_BLUE}│{ANSI_RESET} ")
+        for line in getattr(EvaluationStrategies, name).__doc__.strip().split("\n"):
+            print(f" {ANSI_BLUE}│{ANSI_RESET} " + line.strip())
+        print(f" {ANSI_BLUE}│{ANSI_RESET} ")
+        print(f" {ANSI_BLUE}╰───╴{ANSI_RESET}")
+
+
 def create_template(name: str = "default") -> None:
     """Create default user template."""
     if name == "original":
         print_error(f"Name {name!r} is reserved, please choose another template name.")
         sys.exit(1)
     user_template = PlatformDirs().user_config_path / f"ptyx-mcq/templates/{name}"
     if user_template.is_dir():
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ptyx_mcq-23.3/ptyx_mcq/doc/algo_detection_carres.odt` & `ptyx_mcq-23.4/ptyx_mcq/doc/algo_detection_carres.odt`

 * *Files identical despite different names*

### Comparing `ptyx_mcq-23.3/ptyx_mcq/doc/exemple` & `ptyx_mcq-23.4/ptyx_mcq/doc/exemple`

 * *Files identical despite different names*

### Comparing `ptyx_mcq-23.3/ptyx_mcq/doc/exemple_complet_syntaxe.pdf` & `ptyx_mcq-23.4/ptyx_mcq/doc/exemple_complet_syntaxe.pdf`

 * *Files identical despite different names*

### Comparing `ptyx_mcq-23.3/ptyx_mcq/doc/exemple_complet_syntaxe.tex` & `ptyx_mcq-23.4/ptyx_mcq/doc/exemple_complet_syntaxe.tex`

 * *Files identical despite different names*

### Comparing `ptyx_mcq-23.3/ptyx_mcq/doc/profiling.png` & `ptyx_mcq-23.4/ptyx_mcq/doc/profiling.png`

 * *Files identical despite different names*

### Comparing `ptyx_mcq-23.3/ptyx_mcq/doc/structure_QCM.svg` & `ptyx_mcq-23.4/ptyx_mcq/doc/structure_QCM.svg`

 * *Files identical despite different names*

### Comparing `ptyx_mcq-23.3/ptyx_mcq/dump.profile` & `ptyx_mcq-23.4/ptyx_mcq/dump.profile`

 * *Files identical despite different names*

### Comparing `ptyx_mcq-23.3/ptyx_mcq/make/extend_latex_generator.py` & `ptyx_mcq-23.4/ptyx_mcq/make/extend_latex_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -227,25 +227,15 @@
         """Reset MCQ plugin cache.
 
         Some tags use cache, for code which don't change between two successive compilation.
         (Typically, this is used for (most of) the header)."""
         self.cache["mcq"] = {
             "header": None,
             "check_id_or_name": None,
-            "data": Configuration(
-                mode={"default": "some"},
-                weight={"default": 1},
-                correct={"default": 1},
-                incorrect={"default": 0},
-                skipped={"default": 0},
-                # -inf and inf would be sensible defaults for floor and ceil,
-                # but unfortunately they aren't supported by ast.literal_eval().
-                floor={"default": None},
-                ceil={"default": None},
-            ),
+            "data": Configuration(),
         }
 
     @property
     def mcq_cache(self) -> MCQCache:
         if "mcq" not in self.cache:
             self._mcq_reset_cache()
         return self.cache["mcq"]
@@ -649,14 +639,17 @@
                     self.mcq_data.id_format = data["id_format"]
                     self.mcq_data.students_ids = data["students_ids"]
                     code = student_id_table(*data["id_format"])
 
             if "sty" in config:
                 sty = config.pop("sty")
 
+            if "default_score" in config:
+                self.mcq_data.default_score = config.pop("default_score")
+
             # Config should be empty by now !
             for key in config:
                 if key == "scores":
                     right, wrong, skipped = config[key].split()
                     print_warning("Please update your ptyx file header:")
                     print(f"Replace `scores = {config[key]}` with:")
                     print(20 * "-")
```

### Comparing `ptyx_mcq-23.3/ptyx_mcq/make/generate_ptyx_code.py` & `ptyx_mcq-23.4/ptyx_mcq/make/generate_ptyx_code.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # from enum import Enum, unique
 #
 # @unique
 # class Levels(Enum):
 #     ROOT, QCM, SECTION, QUESTION, VERSION, ANSWERS_BLOCK, NEW_ANSWER = range(7)
-import re
 import sys
 from typing import Iterable
 
 from ptyx_mcq import print_error
 
 
 def generate_ptyx_code(text: str, additional_header_lines: Iterable[str] = ()) -> str:
@@ -175,26 +174,31 @@
 
         elif line.startswith("#ANSWERS_LIST"):
             # End question.
             # (Usually, questions are closed when seeing answers, i.e. lines
             # introduced by '-' or '+').
             code.append(line)
 
+        elif line.startswith("<->"):
+            # Examples:
+            # <->2cm
+            # <->.5
+            width = line[3:]
+            code.append(f"#{{ANSWER_WIDTH={width!r};}}")
+
         elif line.startswith("@"):
             raw = line.startswith("@@")
             # Examples:
-            # @{2cm}formatting_function
-            # @@{.5}\texttt{%s}
-            m = re.match("(?:{(.+)})?(.*)", line[(2 if raw else 1) :].strip())
-            assert m is not None
-            width, formatting = m.groups()
+            # @formatting_function
+            # @@\texttt{%s}
+            formatting = line[(2 if raw else 1) :].strip()
             if formatting == "":
                 formatting = "%s"
             # Declare function to be applied to all answers.
-            code.append(f"#{{RAW_CODE={raw};APPLY_TO_ANSWERS={formatting!r};ANSWER_WIDTH={width!r};}}")
+            code.append(f"#{{RAW_CODE={raw};APPLY_TO_ANSWERS={formatting!r};}}")
 
         elif line.startswith("- ") or line.startswith("+ ") or line.startswith("! "):
             # - incorrect answer
             # + correct answer
             # ! neutralized answer (neither really true nor false, this is useful when there was a problem
             # in an answer).
```

### Comparing `ptyx_mcq-23.3/ptyx_mcq/make/header.py` & `ptyx_mcq-23.4/ptyx_mcq/make/header.py`

 * *Files identical despite different names*

### Comparing `ptyx_mcq-23.3/ptyx_mcq/make/make.py` & `ptyx_mcq-23.4/ptyx_mcq/make/make.py`

 * *Files identical despite different names*

### Comparing `ptyx_mcq-23.3/ptyx_mcq/scan/amend.py` & `ptyx_mcq-23.4/ptyx_mcq/scan/amend.py`

 * *Files identical despite different names*

### Comparing `ptyx_mcq-23.3/ptyx_mcq/scan/conflict_solver.py` & `ptyx_mcq-23.4/ptyx_mcq/scan/conflict_solver.py`

 * *Files identical despite different names*

### Comparing `ptyx_mcq-23.3/ptyx_mcq/scan/data_manager.py` & `ptyx_mcq-23.4/ptyx_mcq/scan/data_manager.py`

 * *Files identical despite different names*

### Comparing `ptyx_mcq-23.3/ptyx_mcq/scan/document_data.py` & `ptyx_mcq-23.4/ptyx_mcq/scan/document_data.py`

 * *Files identical despite different names*

### Comparing `ptyx_mcq-23.3/ptyx_mcq/scan/paths_handler.py` & `ptyx_mcq-23.4/ptyx_mcq/scan/paths_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 
 
 @dataclass
 class FilesPaths:
     verified: Path
     skipped: Path
     more_infos: Path
-    scores: Path
+    csv_scores: Path
+    xlsx_scores: Path
     infos: Path
 
 
 @dataclass
 class DirsPaths:
     root: Path
     data: Path
@@ -67,15 +68,16 @@
             pdf=output_dir / "pdf",
             log=log,
         )
         self.files = FilesPaths(
             verified=cfg / "verified.txt",
             skipped=cfg / "skipped.txt",
             more_infos=cfg / "more_infos.csv",
-            scores=output_dir / "scores.csv",
+            csv_scores=output_dir / "scores.csv",
+            xlsx_scores=output_dir / "scores.xlsx",
             infos=output_dir / "infos.csv",
         )
         self.logfile_path = log / (strftime("%Y.%m.%d-%H.%M.%S") + ".log")
 
     def make_dirs(self, reset=False):
         """Make output directory structure. Is reset is `True`, remove all output directory content."""
         if reset and self.output_dir.is_dir():
```

### Comparing `ptyx_mcq-23.3/ptyx_mcq/scan/pdftools.py` & `ptyx_mcq-23.4/ptyx_mcq/scan/pdftools.py`

 * *Files identical despite different names*

### Comparing `ptyx_mcq-23.3/ptyx_mcq/scan/scan.py` & `ptyx_mcq-23.4/ptyx_mcq/scan/scan.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,32 @@
 #!/usr/bin/env python3
+import csv
+import subprocess
+import tempfile
+from math import inf
+from pathlib import Path
+from typing import Union, Literal, Optional
+
+from ptyx_mcq.scan.amend import amend_all
+from ptyx_mcq.scan.conflict_solver import ConflictSolver
+from ptyx_mcq.scan.data_manager import DataStorage
+from ptyx_mcq.scan.document_data import DocumentData, PicData, Page
+from ptyx_mcq.scan.pdftools import PIC_EXTS
+from ptyx_mcq.scan.scan_pic import (
+    scan_picture,
+    CalibrationError,
+)
+from ptyx_mcq.scan.scores_manager import ScoresManager
+from ptyx_mcq.tools.config_parser import (
+    StudentId,
+    StudentName,
+    DocumentId,
+)
+from ptyx_mcq.tools.io_tools import print_success, print_warning, ANSI_RESET, ANSI_GREEN
+
 
 # -----------------------------------------
 #                  Scan
 #     Extract info from digitized documents
 # -----------------------------------------
 #    PTYX
 #    Python LaTeX preprocessor
@@ -19,44 +43,14 @@
 #    GNU General Public License for more details.
 #
 #    You should have received a copy of the GNU General Public License
 #    along with this program; if not, write to the Free Software
 #    Foundation, Inc., 51 Franklin St, Fifth Floor, Boston, MA  02110-1301  USA
 
 
-import csv
-import subprocess
-import tempfile
-from math import inf
-from pathlib import Path
-from typing import Union, Literal, Optional
-
-from ptyx_mcq.scan import scores
-from ptyx_mcq.scan.amend import amend_all
-from ptyx_mcq.scan.conflict_solver import ConflictSolver
-from ptyx_mcq.scan.data_manager import DataStorage
-from ptyx_mcq.scan.document_data import DocumentData, PicData, Page
-from ptyx_mcq.scan.pdftools import PIC_EXTS
-from ptyx_mcq.scan.scan_pic import (
-    scan_picture,
-    ANSI_YELLOW,
-    ANSI_RESET,
-    ANSI_CYAN,
-    ANSI_GREEN,
-    ANSI_RED,
-    CalibrationError,
-)
-from ptyx_mcq.tools.config_parser import (
-    StudentId,
-    StudentName,
-    DocumentId,
-)
-from ptyx_mcq.tools.io_tools import print_success, print_warning
-
-
 # File `compilation.py` is in ../.., so we have to "hack" `sys.path` a bit.
 # script_path = dirname(abspath(sys._getframe().f_code.co_filename))
 # sys.path.insert(0, join(script_path, '../..'))
 # from ptyx.compilation import join_files, compile_latex
 
 # from ..make.header import answers_and_score
 
@@ -81,14 +75,15 @@
         # Set `already_seen` will contain all seen (ID, page) couples.
         # It is used to catch a hypothetical scanning problem:
         # we have to be sure that the same page on the same test is not seen
         # twice.
         self.already_seen: set[tuple[DocumentId, Page]] = set()
         self.warnings = False
         self.data_storage = DataStorage(Path(path), input_dir=input_dir, output_dir=output_dir)
+        self.scores_manager = ScoresManager(self)
 
     @property
     def config(self):
         return self.data_storage.config
 
     @property
     def data(self):
@@ -194,141 +189,42 @@
         if action == "l":
             # Remove first picture information.
             del self.data[doc_id]["pages"][p]
             self.data_storage.store_doc_data(firstpic.parent.name, doc_id, p)
 
         return action == "f"
 
-    def _calculate_scores(self) -> None:
-        cfg = self.config
-        default_mode = cfg.mode["default"]
-        default_weight = cfg.weight["default"]
-        default_correct = cfg.correct["default"]
-        default_incorrect = cfg.incorrect["default"]
-        default_skipped = cfg.skipped["default"]
-        default_floor = cfg.floor["default"]
-        default_ceil = cfg.ceil["default"]
-
-        for doc_id in self.data:
-            correct_ans = self.data_storage.correct_answers[doc_id]
-            neutralized_ans = self.data_storage.neutralized_answers[doc_id]
-            print(f'Test {doc_id} - {self.data[doc_id]["name"]}')
-            doc_data = self.data[doc_id]
-            for q in sorted(doc_data["answered"]):
-                answered = set(doc_data["answered"][q])
-                correct_ones = correct_ans[q]
-                neutralized_ones = neutralized_ans[q]
-                all_answers = {ans_num for ans_num, is_ok in cfg.ordering[doc_id]["answers"][q]}
-
-                # Neutralized answers must be removed from each set of answers.
-                # (Typically, neutralized answers are answers which were detected faulty during or after the
-                # examination).
-                answered -= neutralized_ones
-                correct_ones -= neutralized_ones
-                all_answers -= neutralized_ones
-
-                mode = cfg.mode.get(q, default_mode)
-
-                if mode == "skip":
-                    # Used mostly to skip bogus questions.
-                    print(f"Question {q} skipped...")
-                    continue
-
-                try:
-                    func = getattr(scores.ScoresStrategies, mode)
-                except AttributeError:
-                    raise AttributeError(f"Unknown evaluation mode: {mode!r}.")
-
-                ans_data = scores.AnswersData(checked=answered, correct=correct_ones, all=all_answers)
-                scores_data = scores.ScoreData(
-                    correct=float(cfg.correct.get(q, default_correct)),
-                    skipped=float(cfg.skipped.get(q, default_skipped)),
-                    incorrect=float(cfg.incorrect.get(q, default_incorrect)),
-                )
-                earn = func(ans_data, scores_data)
-
-                floor = cfg.floor.get(q, default_floor)
-                assert floor is None or isinstance(floor, (float, int))
-                if floor is not None and earn < floor:
-                    earn = floor
-                ceil = cfg.ceil.get(q, default_ceil)
-                assert ceil is None or isinstance(ceil, (float, int))
-                if ceil is not None and earn > ceil:
-                    earn = ceil
-
-                if earn == scores_data.correct:
-                    color = ANSI_GREEN
-                elif earn == scores_data.incorrect:
-                    color = ANSI_RED
-                else:
-                    color = ANSI_YELLOW
-                print(f"-  {color}Rating (Q{q}): {color}{earn:g}{ANSI_RESET}")
-                # Don't forget to include the weight of the question to calculate the global score.
-                earn *= float(cfg.weight.get(q, default_weight))
-                # Don't use weight for per question score, since it would make success rates
-                # harder to compare.
-                doc_data["score_per_question"][q] = earn
-                doc_data["score"] += earn
-
-    def generate_output(self) -> None:
-        """Generate CSV files with scores and annotated documents."""
-        max_score = self.config.max_score
-        # Generate CSV file with results.
-        # TODO: Add ability to change default score ("ABI" for now).
-        scores_: dict[str, float | str] = {name: "ABI" for name in self.config.students_ids.values()}
-        results: dict[str, float] = {doc_data["name"]: doc_data["score"] for doc_data in self.data.values()}
-        scores_.update(results)
-
-        def format_(num: float | str):
-            if isinstance(num, float):
-                num = round(num, 2)
-            return num
-
-        # ~ print(scores)
-        scores_path = self.data_storage.files.scores
-        print(f"{ANSI_CYAN}SCORES (/{max_score:g}):{ANSI_RESET}")
-        with open(scores_path, "w", newline="") as csvfile:
-            writerow = csv.writer(csvfile).writerow
-            writerow(("Name", "Score"))
-            for name in sorted(scores_):
-                score = scores_[name]
-                print(f" - {name}: {format_(score)}")
-                # TODO: Add ability to change the notation system.
-                if isinstance(score, float):
-                    score = score / max_score * 20
-                writerow([name, format_(score)])
-        if results:
-            mean = round(sum(results.values()) / len(results), 2)
-            print(f"{ANSI_YELLOW}Mean: {mean:g}/{max_score:g}{ANSI_RESET}")
-        else:
-            print("No score found !")
-        print(f'\nResults stored in "{scores_path}"\n')
+    def generate_report(self) -> None:
+        """Generate CSV files with some information concerning each student.
 
+        Used mainly for debugging.
+        """
         # Generate CSV file with ID and pictures names for all students.
         info_path = self.data_storage.files.infos
         info = [
             (
                 doc_data["name"],
                 doc_data["student_ID"],
                 doc_id,
                 doc_data["score"],
                 [doc_data["pages"][p].pic_path for p in doc_data["pages"]],
             )
             for doc_id, doc_data in self.data.items()
         ]
-        print(f"{ANSI_CYAN}SCORES (/{max_score:g}):{ANSI_RESET}")
+
         with open(info_path, "w", newline="") as csvfile:
             writerow = csv.writer(csvfile).writerow
             writerow(("Name", "Student ID", "Test ID", "Score", "Pictures"))
             for name, student_ID, doc_id, score, paths in sorted(info):
                 paths_as_str = ", ".join(str(pth) for pth in paths)
                 writerow([name, student_ID, f"#{doc_id}", score, paths_as_str])
         print(f'Infos stored in "{info_path}"\n')
+
+    def generate_amended_pdf(self) -> None:
         amend_all(self.data_storage)
-        print(f"\n{ANSI_GREEN}Success ! {ANSI_RESET}:)")
 
     def scan_picture(self, picture: Union[str, Path], manual_verification: bool = True) -> None:
         """This is used for debuging (it allows to test pages one by one)."""
         # f1-pic-003.jpg (page 25)
         # f12-pic-005.jpg
         # f12-pic-003.jpg
         # f12-pic-004.jpg
@@ -484,21 +380,31 @@
         self._test_integrity()
         print("Everything seems OK.")
 
         # ---------------------------
         # Calculate scores
         # ---------------------------
         # Calculate the score, taking care of the chosen mode.
-        self._calculate_scores()
-        print()
+        self.scores_manager.calculate_scores()
+        self.scores_manager.print_scores()
 
         # ---------------------------------------------------
         # Time to synthesize & store all those informations !
         # ---------------------------------------------------
-        self.generate_output()
+        self.scores_manager.generate_csv_file()
+        self.scores_manager.generate_xlsx_file()
+        cfg_ext = ".ptyx.mcq.config.json"
+        cfg_path = str(self.data_storage.paths.configfile)
+        assert cfg_path.endswith(cfg_ext)
+        xlsx_symlink = Path(cfg_path[: -len(cfg_ext)] + ".scores.xlsx")
+        xlsx_symlink.unlink(missing_ok=True)
+        xlsx_symlink.symlink_to(self.data_storage.files.xlsx_scores)
+        self.generate_report()
+        self.generate_amended_pdf()
+        print(f"\n{ANSI_GREEN}Success ! {ANSI_RESET}:)")
 
 
 def scan(
     path: Path,
     reset: bool = False,
     ask_for_name: bool = False,
     verify: Literal["auto", "always", "never"] = "auto",
```

### Comparing `ptyx_mcq-23.3/ptyx_mcq/scan/scan_pic.py` & `ptyx_mcq-23.4/ptyx_mcq/scan/scan_pic.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,27 +29,15 @@
     StudentIdFormat,
     OriginalQuestionNumber,
     OriginalAnswerNumber,
     DocumentId,
     StudentName,
     StudentId,
 )
-
-ANSI_RESET = "\u001B[0m"
-ANSI_BLACK = "\u001B[30m"
-ANSI_RED = "\u001B[31m"
-ANSI_GREEN = "\u001B[32m"
-ANSI_YELLOW = "\u001B[33m"
-ANSI_BLUE = "\u001B[34m"
-ANSI_PURPLE = "\u001B[35m"
-ANSI_CYAN = "\u001B[1;36m"
-ANSI_WHITE = "\u001B[37m"
-ANSI_GRAY = "\u001B[90m"
-ANSI_BOLD = "\u001B[1m"
-ANSI_REVERSE = "\u001B[45m"
+from ..tools.io_tools import ANSI_RESET, ANSI_YELLOW, ANSI_CYAN, ANSI_GRAY
 
 CORNERS = frozenset(("tl", "tr", "bl", "br"))
 CORNER_NAMES = {"tl": "top-left", "tr": "top-right", "bl": "bottom-left", "br": "bottom-right"}
 
 CornersPositions = dict[str, Pixel]
 
 # TODO: calibrate grayscale too.
```

### Comparing `ptyx_mcq-23.3/ptyx_mcq/scan/square_detection.py` & `ptyx_mcq-23.4/ptyx_mcq/scan/square_detection.py`

 * *Files identical despite different names*

### Comparing `ptyx_mcq-23.3/ptyx_mcq/scan/tools.py` & `ptyx_mcq-23.4/ptyx_mcq/scan/tools.py`

 * *Files identical despite different names*

### Comparing `ptyx_mcq-23.3/ptyx_mcq/scan/visual_debugging.py` & `ptyx_mcq-23.4/ptyx_mcq/scan/visual_debugging.py`

 * *Files 19% similar despite different names*

```diff
@@ -218,112 +218,7 @@
     - Left-dragging the picture with mouse inside feh removes blurring/anti-aliasing,
       making visual debugging a lot easier.
     """
     viewer = ArrayViewer(array)
     if from_ is not None:
         viewer.add_area(from_, to_, color=color, thickness=thickness, fill=fill)
     viewer.display(wait=wait)
-
-
-# # noinspection PyDefaultArgument
-# def color2debug(
-#     array: ndarray = None,
-#     from_: FloatPosition = None,
-#     to_: FloatPosition = None,
-#     color: RGB = Color.red,
-#     display: bool = True,
-#     thickness: int = 2,
-#     fill=False,
-#     _d={},
-#     wait=True,
-# ):
-#     """Display picture with a red (by default) rectangle for debugging.
-#     The annotated picture can be displayed immediately (default), or the annotation can be memorized,
-#     if `display` is set to `False`.
-#     It allows to display several annotations at once.
-#
-#     Launch this function without argument to clear all previous stored annotations.
-#
-#     Parameters:
-#     `array` is an array containing the image data (image must be gray mode,
-#     each pixel represented by a float from 0 (black) to 1 (white)).
-#     `from_` represent one corner of the red rectangle.
-#     `to_` represent opposite corner of the red rectangle.
-#     `color` is given as a RGB tuple ([0-255], [0-255], [0-255]).
-#     `fill` (True|False) indicates if the rectangle should be filled.
-#
-#     Usage: color2debug((0,0), (200,10), color=(255, 0, 255))
-#
-#     If you need to display `n` rectangles, call `color2debug()` with
-#     `display=False` for the first `n-1` rectangles, and then with
-#     `display=True` for the last rectangle.
-#
-#     `_d` is used internally to store values between two runs, if display=False.
-#
-#     NOTA:
-#     - `feh` must be installed.
-#       On Ubuntu/Debian: sudo apt-get install feh
-#     - Left-dragging the picture with mouse inside feh removes blurring/anti-aliasing,
-#       making visual debugging a lot easier.
-#     """
-#     if array is None:
-#         _d.clear()
-#         return
-#     ID = id(array)
-#     if ID not in _d:
-#         # Load image only if not loaded previously.
-#         # .astype(int8) will make more arrays representable.
-#         _d[ID] = Image.fromarray((255 * array).astype(int8)).convert("RGB")
-#     rgb = _d[ID]
-#     height, width = array.shape
-#     if from_ is not None:
-#         if to_ is None:
-#             to_ = from_
-#         i1, j1 = from_
-#         i2, j2 = to_
-#         if i2 is None:
-#             i2 = height - 1
-#         if j2 is None:
-#             j2 = width - 1
-#         pix = rgb.load()
-#         imin, imax = int(min(i1, i2)), int(max(i1, i2))
-#         jmin, jmax = int(min(j1, j2)), int(max(j1, j2))
-#
-#         def set_pix(i: int, j: int, color: RGB) -> None:
-#             """Set safely pixel color (if `i` or `j` is incorrect, do nothing)."""
-#             if 0 <= i < height and 0 <= j < width:
-#                 pix[j, i] = color
-#
-#         if fill:
-#             for i in range(imin, imax + 1):
-#                 for j in range(jmin, jmax + 1):
-#                     set_pix(i, j, color)
-#         else:
-#             # left and right sides of rectangle
-#             for i in range(imin, imax + 1):
-#                 for j in range(jmin, jmin + thickness):
-#                     set_pix(i, j, color)
-#                 for j in range(jmax + 1 - thickness, jmax + 1):
-#                     set_pix(i, j, color)
-#             # top and bottom sides of rectangle
-#             for j in range(jmin, jmax + 1):
-#                 for i in range(imin, imin + thickness):
-#                     set_pix(i, j, color)
-#                 for i in range(imax + 1 - thickness, imax + 1):
-#                     set_pix(i, j, color)
-#
-#     if display:
-#         del _d[ID]
-#         if subprocess.call(["which", "feh"]) != 0:
-#             raise RuntimeError(
-#                 "The `feh` command is not found, please " "install it (`sudo apt install feh` on Ubuntu)."
-#             )
-#         with tempfile.TemporaryDirectory() as tmpdirname:
-#             path = join(tmpdirname, "test.png")
-#             rgb.save(path)
-#             process: subprocess.CompletedProcess | subprocess.Popen
-#             if wait:
-#                 process = subprocess.run(["feh", "-F", path])
-#             else:
-#                 process = subprocess.Popen(["feh", "-F", path], stdin=subprocess.DEVNULL)
-#             input("-- pause --\n")
-#             return process
```

### Comparing `ptyx_mcq-23.3/ptyx_mcq/templates/original/new.ptyx` & `ptyx_mcq-23.4/ptyx_mcq/templates/original/new.ptyx`

 * *Files 17% similar despite different names*

```diff
@@ -13,21 +13,25 @@
 incorrect = 0 
 # Score when the question was left unanswered (usually null)
 skipped = 0
 # Minimal score for a question
 # floor = 0
 # Maximal score for a question
 # ceil = 1
-# Mode must be `all`, `some`, `proportional`, `partial_answers_linear` or `partial_answers_quadratic`
-mode=all
+# The full list of the evaluation strategies and their description can be obtained
+# using command `mcq strategies`.
+# Available modes include `all`, `some`, `proportional`, `partial_answers` or `correct_minus_incorrect`.
+mode = all
 # Uncomment and edit the following line to load students ID.
 # This must be a comma separated CSV file with at least 2 columns.
 # Students identifiers must be in the 1st column (without any header).
-# ids=~/listings/INE_2021.csv
-id format=8 digits
+# ids = ~/listings/INE_2021.csv
+id format = 8 digits
+# Value displayed for missing students (empty by default):
+# default score = ABI
 ---------------------------
 # You may include here raw LaTeX code (definition of new LaTeX commands for example).
 # It will be appended to the LaTeX preamble. Example:
 # \usetikzlibrary{arrows.meta}
 
 ===========================
```

### Comparing `ptyx_mcq-23.3/ptyx_mcq/templates/original/questions/question1.ex` & `ptyx_mcq-23.4/ptyx_mcq/templates/original/questions/question1.ex`

 * *Files identical despite different names*

### Comparing `ptyx_mcq-23.3/ptyx_mcq/templates/original/questions/question3.ex` & `ptyx_mcq-23.4/ptyx_mcq/templates/original/questions/question3.ex`

 * *Files identical despite different names*

### Comparing `ptyx_mcq-23.3/ptyx_mcq/templates/original/questions/question4.ex` & `ptyx_mcq-23.4/ptyx_mcq/templates/original/questions/question4.ex`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 # If `@@` is used the line before an answer, the following answers will be displayed in verbatim mode:
 # a fixed-width font is used, spaces are kept intact and latex special characters like `{` or `$`
 # are escaped.
 # By default, if the answer is on several lines, it is supposed to use the full page width.
 # The width can be manually reduced using `{6cm}`, or `{.5}` which stands for ``{.5\linewidth}`.
 # Combining verbatim mode and reduced width is useful to display code:
 
-@@{.45}
+<->.45
+@@
 + public double getNorm() {
 	int i, sum = 0;
 	for (i=0; i<counts.length; i++) {
 		sum += counts[i]*counts[i]; }
 	return Math.sqrt(sum); }
 
 - public double getNorm() {
```

### Comparing `ptyx_mcq-23.3/ptyx_mcq/tools/config_parser.py` & `ptyx_mcq-23.4/ptyx_mcq/tools/config_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,22 +59,25 @@
 # "boxes": {},  # {NUM: {'tag': 'p4, (23.456, 34.667)', ...}, ...}
 # "id_format": None,
 
 
 # TODO: improve typing precision
 @dataclass(kw_only=True, slots=True)
 class Configuration:
-    mode: dict[QuestionNumberOrDefault, str]  # = field(default_factory=lambda: {"default": "some"})
-    correct: dict[QuestionNumberOrDefault, float]  # = field(default_factory=lambda: {"default": 1})
-    incorrect: dict[QuestionNumberOrDefault, float]  # = field(default_factory=lambda: {"default": 0})
-    skipped: dict[QuestionNumberOrDefault, float]  # = field(default_factory=lambda: {"default": 0})
-    weight: dict[QuestionNumberOrDefault, float]  # = field(default_factory=lambda: {"default": 0})
-    floor: dict[QuestionNumberOrDefault, float | None]  # = field(default_factory=lambda: {"default": None})
-    ceil: dict[QuestionNumberOrDefault, float | None]  # = field(default_factory=dict)
+    mode: dict[QuestionNumberOrDefault, str] = field(default_factory=lambda: {"default": "all"})
+    correct: dict[QuestionNumberOrDefault, float] = field(default_factory=lambda: {"default": 1})
+    incorrect: dict[QuestionNumberOrDefault, float] = field(default_factory=lambda: {"default": 0})
+    skipped: dict[QuestionNumberOrDefault, float] = field(default_factory=lambda: {"default": 0})
+    weight: dict[QuestionNumberOrDefault, float] = field(default_factory=lambda: {"default": 1})
+    # -inf and inf would be sensible defaults for floor and ceil,
+    # but unfortunately they aren't supported by ast.literal_eval().
+    floor: dict[QuestionNumberOrDefault, float | None] = field(default_factory=lambda: {"default": None})
+    ceil: dict[QuestionNumberOrDefault, float | None] = field(default_factory=lambda: {"default": None})
     id_format: StudentIdFormat | None = None
+    default_score: str = ""
     students_ids: dict[StudentId, StudentName] = field(default_factory=dict)
     students_list: list[StudentName] = field(default_factory=list)
     ordering: dict[DocumentId, OrderingConfiguration] = field(default_factory=dict)
     # ordering: {NUM: {'questions': [2,1,3...],
     #                  'answers': {1: [(2, True), (1, False), (3, True)...], ...}}, ...}
     boxes: dict[DocumentId, dict[int, dict[str, tuple[float, float]]]] = field(default_factory=dict)
     # boxes: {NUM: {'tag': 'p4, (23.456, 34.667)', ...}, ...}
```

### Comparing `ptyx_mcq-23.3/ptyx_mcq/tools/extend_literal_eval.py` & `ptyx_mcq-23.4/ptyx_mcq/tools/extend_literal_eval.py`

 * *Files identical despite different names*

### Comparing `ptyx_mcq-23.3/ptyx_mcq/tools/include_parser.py` & `ptyx_mcq-23.4/ptyx_mcq/tools/include_parser.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import re
 from enum import auto, Enum
+from functools import partial
 from pathlib import Path
 from typing import Match
 
-from ptyx_mcq.tools.io_tools import print_info, print_warning
+from ptyx_mcq.tools.io_tools import print_info, print_warning, print_error
 
 
 class IncludeStatus(Enum):
     OK = auto()
     DISABLED = auto()
     NOT_FOUND = auto()
     AUTOMATICALLY_ADDED = auto()
@@ -44,58 +45,74 @@
 
     # Store all include paths.
     # Format: {ROOT folder: {relative path: include enabled (True)|disabled (False)|invalid (None)}}
     includes: dict[str, dict[str, IncludeStatus]]
     _root: Path
 
     def __init__(self, default_path: Path):
+        """Path `default_path` should be the parent directory of the ptyx file."""
         self.default_path = default_path
         self._reset()
 
     def _reset(self):
         self._root = self.default_path
+        self._last_status = IncludeStatus.OK
         self.includes = {}
 
-    def _parse_include(self, match: Match) -> str:
+    def _parse_include(self, match: Match, strict: bool) -> str:
         include_enabled = match.group(0)[0] != "!"
+        if match.group(0)[0] == "#":
+            # Special `#--` comments are used to indicate include status.
+            # (Currently, this only used to mark that an include was automatically added.)
+            try:
+                self._last_status = IncludeStatus[match.group(1).strip().rstrip(":")]
+            except KeyError:
+                print_warning(f"Invalid line: {match.group(0)}")
+            return ""
+        status = self._last_status
+        self._last_status = IncludeStatus.OK
         pattern = match.group(1).strip()
         if pattern.startswith("ROOT:"):
             if include_enabled:
                 path = Path(pattern[5:].strip()).expanduser()
                 if not path.is_absolute():
                     path = (self.default_path / path).resolve()
-                print_info(f"Directory for files inclusion changed to '{path}'.")
+                print_info(f"Directory for files inclusion set to '{path}'.")
                 if not path.is_dir():
                     raise FileNotFoundError(
                         f"Directory '{path}' not found.\n"
                         f'HINT: Change "-- {pattern}" line in your ptyx file.'
                     )
                 self._root = path
-            return "\n"
+            return ""
         else:
             includes = self.includes.setdefault(str(self._root), {})
             if include_enabled:
                 file_found = False
                 contents = []
                 for path in sorted(self._root.glob(pattern)):
                     if path.is_file():
                         file_found = True
-                        contents.append(self._include_file(path))
+                        contents.append(self._include_file(path).strip())
                 if file_found:
                     # Include enabled
-                    includes[str(pattern)] = IncludeStatus.OK
+                    includes[str(pattern)] = status
                 else:
                     # Invalid include
                     includes[str(pattern)] = IncludeStatus.NOT_FOUND
-                    print_warning(f"No file corresponding to {pattern!r} in '{self._root}'!")
+                    if strict:
+                        print_error(message := f"No file corresponding to {pattern!r} in '{self._root}'!")
+                        raise FileNotFoundError(message)
+                    else:
+                        print_warning(f"No file corresponding to {pattern!r} in '{self._root}'!")
                 return "\n\n" + "\n\n".join(contents) + "\n\n"
             else:
                 # Include disabled
                 includes[str(pattern)] = IncludeStatus.DISABLED
-                return "\n"
+                return ""
 
     def _include_file(self, path: Path) -> str:
         lines: list[str] = []
         with open(path) as file:
             file_content = file.read().strip()
             # Remove comments
             file_content = re.sub("( # .+)|(^# .+\n)", "", file_content, flags=re.MULTILINE)
@@ -111,18 +128,24 @@
                     or line.startswith("OR ")
                     or line.rstrip() in ("*", ">", "OR")
                 ):
                     prettified_path = path.parent / f"\u001b[36m{path.name.replace('#', '##')}\u001b[0m"
                     lines.append(f'#PRINT{{\u001b[36mIMPORTING\u001b[0m "{prettified_path}"}}')
         return "\n".join(lines)
 
-    def parse(self, text: str) -> str:
-        """"""
+    def parse(self, code: str, strict: bool = False) -> str:
+        """Parse all include directives and include the corresponding files into the code.
+
+        By default, if a path or a pattern don't match any file, a warning is raised,
+        but the parsing will go on.
+        However, if `strict` is set to `True`, a `FileNotFoundError` is raised in that case.
+        """
         self._reset()
-        return re.sub(r"^!?-- (.+)$", self._parse_include, text, flags=re.MULTILINE)
+        _parse = partial(self._parse_include, strict=strict)
+        return re.sub(r"^[#!]?-- (.+)$", _parse, code, flags=re.MULTILINE)
 
     def update(self, ptyxfile_path: Path):
         """Track all the `.ex` files and update pTyX file to include all the `.ex` files found.
 
         The `.ex` files are searched:
             - in the same directory as the `.pTyX` file
             - in any directory manually added via a `-- ROOT: /my/path` directive.
@@ -158,28 +181,37 @@
                     already_indexed.add(ex_file_path)
                     ex_file = str(ex_file_path.relative_to(directory_path))
                     new_includes[directory][ex_file] = IncludeStatus.AUTOMATICALLY_ADDED
         self.includes = new_includes
         self._rewrite_file(ptyxfile_path, new_includes)
 
     def _rewrite_file(self, ptyxfile_path: Path, includes: dict[str, dict[str, IncludeStatus]]):
+        new_file_added = False
         lines = []
         with open(ptyxfile_path, encoding="utf8") as f:
             for line in f:
                 if line.startswith(">>>"):  # `>>>` marks the end of the MCQ
                     # Insert all include directives just before the end of the MCQ.
                     for folder, paths in includes.items():
-                        lines.append(f"\n-- ROOT: {folder}")
-                        for path, status in paths.items():
+                        folder_path = Path(folder)
+                        if folder_path.is_relative_to(self.default_path):
+                            folder = str(folder_path.relative_to(self.default_path))
+                        lines.append(f"-- ROOT: {folder}")
+                        for path, status in sorted(paths.items()):
                             match status:
                                 case IncludeStatus.OK:
                                     lines.append(f"-- {path}")
                                 case IncludeStatus.DISABLED:
                                     lines.append(f"!-- {path}")
                                 case IncludeStatus.NOT_FOUND:
-                                    lines.append(f"# Invalid path:\n!-- {path}")
+                                    lines.append(f"#-- NOT_FOUND:\n!-- {path}")
+                                    print_warning(f"Invalid file path removed: '{path}'.")
                                 case IncludeStatus.AUTOMATICALLY_ADDED:
-                                    lines.append(f"# New path detected:\n-- {path}")
-                if not re.match(r"!?-- ", line):
+                                    lines.append(f"#-- AUTOMATICALLY_ADDED:\n-- {path}")
+                                    print_info(f"New file added: '{path}'.")
+                                    new_file_added = True
+                if not re.match(r"[#!]?-- ", line):
                     lines.append(line.rstrip())
+        if not new_file_added:
+            print_info("No new file found.")
         with open(ptyxfile_path, "w", encoding="utf8") as f:
-            f.write("\n".join(lines))
+            f.write("\n".join(lines) + "\n")
```

### Comparing `ptyx_mcq-23.3/ptyx_mcq/tools/io_tools.py` & `ptyx_mcq-23.4/ptyx_mcq/tools/io_tools.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,26 @@
 import sys
 import traceback
 from pathlib import Path
 
+ANSI_RESET = "\u001B[0m"
+ANSI_BLACK = "\u001B[30m"
+ANSI_RED = "\u001B[31m"
+ANSI_GREEN = "\u001B[32m"
+ANSI_YELLOW = "\u001B[33m"
+ANSI_BLUE = "\u001B[34m"
+ANSI_PURPLE = "\u001B[35m"
+ANSI_CYAN = "\u001B[1;36m"
+ANSI_WHITE = "\u001B[37m"
+ANSI_GRAY = "\u001B[90m"
+ANSI_BOLD = "\u001B[1m"
+ANSI_REVERSE_PURPLE = "\u001B[45m"
+ANSI_REVERSE_BLUE = "\u001B[44m"
+
+
 shell_colors = {
     "red": 1,
     "green": 2,
     "yellow": 3,
     "blue": 4,
 }
```

### Comparing `ptyx_mcq-23.3/ptyx_mcq/tools/scriptlib.py` & `ptyx_mcq-23.4/ptyx_mcq/tools/scriptlib.py`

 * *Files identical despite different names*

### Comparing `ptyx_mcq-23.3/pyproject.toml` & `ptyx_mcq-23.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ptyx-mcq"
-version = "23.3"
+version = "23.4"
 description = "pTyX is a python precompiler for LaTeX."
 authors = ["Nicolas Pourcelot <nicolas.pourcelot@gmail.com>"]
 repository = "https://github.com/wxgeo/ptyx"
 license = "GPL-3.0-or-later"
 readme = "README.md"
 keywords = ["python", "tikz", "latex", "pdf", "exam", "mcq", "student"]
 
@@ -13,26 +13,28 @@
 numpy = "^1.23.0"
 Pillow = "^9.2"
 sympy = "^1.10.1"
 pdf2image = "^1.16.0"
 ptyx = "^23.2"
 smallgraphlib = "^0.6.3"
 platformdirs = "^3.2.0"
+openpyxl = "^3.1.2"
 
 
 [tool.poetry.dev-dependencies]
+types-openpyxl = "^3.1.0.3"
 types-Pillow = "^9.0.20"
 pytest = "^7"
 mypy = "^1.0"
 flake8 = "^6"
-black = "^22.1.0"
+black = "^23.3.0"
 tox = "^4.1.2"
 sphinx-autodoc-typehints = "^1.18.3"
 sphinx-rtd-theme = "^1.0.0"#
-myst-parser = "^0.18.0"
+myst-parser = "^1.0.0"
 ptyx = {path = "../ptyx", develop = true}
 
 [tool.poetry.scripts]
 mcq = 'ptyx_mcq.cli:main'
 
 [tool.poetry.plugins."ptyx.extensions"]
 mcq = "ptyx_mcq"
```

### Comparing `ptyx_mcq-23.3/PKG-INFO` & `ptyx_mcq-23.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: ptyx-mcq
-Version: 23.3
+Version: 23.4
 Summary: pTyX is a python precompiler for LaTeX.
 Home-page: https://github.com/wxgeo/ptyx
 License: GPL-3.0-or-later
 Keywords: python,tikz,latex,pdf,exam,mcq,student
 Author: Nicolas Pourcelot
 Author-email: nicolas.pourcelot@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Pillow (>=9.2,<10.0)
 Requires-Dist: numpy (>=1.23.0,<2.0.0)
+Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
 Requires-Dist: pdf2image (>=1.16.0,<2.0.0)
 Requires-Dist: platformdirs (>=3.2.0,<4.0.0)
 Requires-Dist: ptyx (>=23.2,<24.0)
 Requires-Dist: smallgraphlib (>=0.6.3,<0.7.0)
 Requires-Dist: sympy (>=1.10.1,<2.0.0)
 Project-URL: Repository, https://github.com/wxgeo/ptyx
 Description-Content-Type: text/markdown
```

