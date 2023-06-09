# Comparing `tmp/untypedscript-utsc-0.0.2.tar.gz` & `tmp/untypedscript-utsc-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "untypedscript-utsc-0.0.2.tar", last modified: Fri Jun  9 19:02:42 2023, max compression
+gzip compressed data, was "untypedscript-utsc-0.0.3.tar", last modified: Fri Jun  9 20:00:06 2023, max compression
```

## Comparing `untypedscript-utsc-0.0.2.tar` & `untypedscript-utsc-0.0.3.tar`

### file list

```diff
@@ -1,24 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 19:02:42.263016 untypedscript-utsc-0.0.2/
--rw-rw-rw-   0        0        0     1090 2023-06-09 18:03:17.000000 untypedscript-utsc-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     6567 2023-06-09 19:02:42.262026 untypedscript-utsc-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     4967 2023-06-07 01:23:46.000000 untypedscript-utsc-0.0.2/README.md
--rw-rw-rw-   0        0        0      705 2023-06-09 18:57:05.000000 untypedscript-utsc-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-09 19:02:42.263016 untypedscript-utsc-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-09 19:02:42.142551 untypedscript-utsc-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-06-09 19:02:42.208280 untypedscript-utsc-0.0.2/src/untypedscript_utsc.egg-info/
--rw-rw-rw-   0        0        0     6567 2023-06-09 19:02:42.000000 untypedscript-utsc-0.0.2/src/untypedscript_utsc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      503 2023-06-09 19:02:42.000000 untypedscript-utsc-0.0.2/src/untypedscript_utsc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 19:02:42.000000 untypedscript-utsc-0.0.2/src/untypedscript_utsc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-06-09 19:02:42.000000 untypedscript-utsc-0.0.2/src/untypedscript_utsc.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        5 2023-06-09 19:02:42.000000 untypedscript-utsc-0.0.2/src/untypedscript_utsc.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-09 19:02:42.258001 untypedscript-utsc-0.0.2/src/utsc/
--rw-rw-rw-   0        0        0     9308 2023-06-09 18:48:37.000000 untypedscript-utsc-0.0.2/src/utsc/__init__.py
--rw-rw-rw-   0        0        0      576 2023-02-24 02:16:29.000000 untypedscript-utsc-0.0.2/src/utsc/ast_cleaner.py
--rw-rw-rw-   0        0        0     2734 2023-06-09 18:44:30.000000 untypedscript-utsc-0.0.2/src/utsc/ast_preprocessor.py
--rw-rw-rw-   0        0        0     7217 2023-06-09 18:44:28.000000 untypedscript-utsc-0.0.2/src/utsc/code_lowerer.py
--rw-rw-rw-   0        0        0    36276 2023-06-09 18:44:23.000000 untypedscript-utsc-0.0.2/src/utsc/compiler.py
--rw-rw-rw-   0        0        0     2340 2023-06-04 23:42:15.000000 untypedscript-utsc-0.0.2/src/utsc/optimizer.py
--rw-rw-rw-   0        0        0     7829 2023-06-09 18:44:10.000000 untypedscript-utsc-0.0.2/src/utsc/sequential_lexer.py
--rw-rw-rw-   0        0        0     4789 2023-06-09 18:54:08.000000 untypedscript-utsc-0.0.2/src/utsc/utils.py
--rw-rw-rw-   0        0        0    39560 2023-06-09 18:44:01.000000 untypedscript-utsc-0.0.2/src/utsc/uts_parser.py
--rw-rw-rw-   0        0        0      161 2023-06-08 22:00:18.000000 untypedscript-utsc-0.0.2/src/utsc/utsc-config.json
+drwxrwxrwx   0        0        0        0 2023-06-09 20:00:06.469460 untypedscript-utsc-0.0.3/
+-rw-rw-rw-   0        0        0     1090 2023-06-09 18:03:17.000000 untypedscript-utsc-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     6567 2023-06-09 20:00:06.467034 untypedscript-utsc-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4967 2023-06-07 01:23:46.000000 untypedscript-utsc-0.0.3/README.md
+-rw-rw-rw-   0        0        0      710 2023-06-09 19:59:11.000000 untypedscript-utsc-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-09 20:00:06.470455 untypedscript-utsc-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-09 20:00:06.361741 untypedscript-utsc-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-06-09 20:00:06.399765 untypedscript-utsc-0.0.3/src/untypedscript_utsc.egg-info/
+-rw-rw-rw-   0        0        0     6567 2023-06-09 20:00:06.000000 untypedscript-utsc-0.0.3/src/untypedscript_utsc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      477 2023-06-09 20:00:06.000000 untypedscript-utsc-0.0.3/src/untypedscript_utsc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 20:00:06.000000 untypedscript-utsc-0.0.3/src/untypedscript_utsc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-06-09 20:00:06.000000 untypedscript-utsc-0.0.3/src/untypedscript_utsc.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-06-09 20:00:06.000000 untypedscript-utsc-0.0.3/src/untypedscript_utsc.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 20:00:06.461063 untypedscript-utsc-0.0.3/src/utsc/
+-rw-rw-rw-   0        0        0     9308 2023-06-09 18:48:37.000000 untypedscript-utsc-0.0.3/src/utsc/__init__.py
+-rw-rw-rw-   0        0        0      576 2023-02-24 02:16:29.000000 untypedscript-utsc-0.0.3/src/utsc/ast_cleaner.py
+-rw-rw-rw-   0        0        0     2734 2023-06-09 18:44:30.000000 untypedscript-utsc-0.0.3/src/utsc/ast_preprocessor.py
+-rw-rw-rw-   0        0        0     7217 2023-06-09 18:44:28.000000 untypedscript-utsc-0.0.3/src/utsc/code_lowerer.py
+-rw-rw-rw-   0        0        0    36276 2023-06-09 18:44:23.000000 untypedscript-utsc-0.0.3/src/utsc/compiler.py
+-rw-rw-rw-   0        0        0     2340 2023-06-04 23:42:15.000000 untypedscript-utsc-0.0.3/src/utsc/optimizer.py
+-rw-rw-rw-   0        0        0     7829 2023-06-09 18:44:10.000000 untypedscript-utsc-0.0.3/src/utsc/sequential_lexer.py
+-rw-rw-rw-   0        0        0     4817 2023-06-09 19:19:00.000000 untypedscript-utsc-0.0.3/src/utsc/utils.py
+-rw-rw-rw-   0        0        0    39560 2023-06-09 18:44:01.000000 untypedscript-utsc-0.0.3/src/utsc/uts_parser.py
```

### Comparing `untypedscript-utsc-0.0.2/LICENSE` & `untypedscript-utsc-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `untypedscript-utsc-0.0.2/PKG-INFO` & `untypedscript-utsc-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: untypedscript-utsc
-Version: 0.0.2
+Version: 0.0.3
 Summary: UntypedScript original implementation compiler
 Author-email: Carl Furtado <carlzfurtado@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Carl Furtado
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `untypedscript-utsc-0.0.2/README.md` & `untypedscript-utsc-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `untypedscript-utsc-0.0.2/pyproject.toml` & `untypedscript-utsc-0.0.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "untypedscript-utsc"
-version = "0.0.2"
+version = "0.0.3"
 description = "UntypedScript original implementation compiler"
 readme = "README.md"
 authors = [{ name = "Carl Furtado", email = "carlzfurtado@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = []
 keywords = []
 dependencies = []
@@ -19,8 +19,8 @@
 # Documentation = "https://webpy-framework.readthedocs.io/"
 
 [project.scripts]
 utsc = "utsc:main"
 utsc-configure = "utsc:configure"
 
 [tool.setuptools.package-data]
-utsc = ["utsc-config.json"]
+lib = ["*.uts", "libheapfunc.o"]
```

### Comparing `untypedscript-utsc-0.0.2/src/untypedscript_utsc.egg-info/PKG-INFO` & `untypedscript-utsc-0.0.3/src/untypedscript_utsc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: untypedscript-utsc
-Version: 0.0.2
+Version: 0.0.3
 Summary: UntypedScript original implementation compiler
 Author-email: Carl Furtado <carlzfurtado@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Carl Furtado
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `untypedscript-utsc-0.0.2/src/utsc/__init__.py` & `untypedscript-utsc-0.0.3/src/utsc/__init__.py`

 * *Files identical despite different names*

### Comparing `untypedscript-utsc-0.0.2/src/utsc/ast_cleaner.py` & `untypedscript-utsc-0.0.3/src/utsc/ast_cleaner.py`

 * *Files identical despite different names*

### Comparing `untypedscript-utsc-0.0.2/src/utsc/ast_preprocessor.py` & `untypedscript-utsc-0.0.3/src/utsc/ast_preprocessor.py`

 * *Files identical despite different names*

### Comparing `untypedscript-utsc-0.0.2/src/utsc/code_lowerer.py` & `untypedscript-utsc-0.0.3/src/utsc/code_lowerer.py`

 * *Files identical despite different names*

### Comparing `untypedscript-utsc-0.0.2/src/utsc/compiler.py` & `untypedscript-utsc-0.0.3/src/utsc/compiler.py`

 * *Files identical despite different names*

### Comparing `untypedscript-utsc-0.0.2/src/utsc/optimizer.py` & `untypedscript-utsc-0.0.3/src/utsc/optimizer.py`

 * *Files identical despite different names*

### Comparing `untypedscript-utsc-0.0.2/src/utsc/sequential_lexer.py` & `untypedscript-utsc-0.0.3/src/utsc/sequential_lexer.py`

 * *Files identical despite different names*

### Comparing `untypedscript-utsc-0.0.2/src/utsc/utils.py` & `untypedscript-utsc-0.0.3/src/utsc/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,15 @@
 
 def checkfailure():
 	exit(1) if thrown else None
 #
 
 def import_config(fname: str) -> dict:
 	if not isfile(fname):
-		throw(f"Fatal Error UTSC 006: Config file {fname} does not exist!")
+		throw(f"Fatal Error UTSC 006: Config file {fname} does not exist (use utsc-configure to fix)!")
 		return
 		
 	with open(fname, 'r') as f:
 		try: conf = load(f)
 		except JSONDecodeError:
 			throw(f"Fatal Error UTSC 006: Config file {fname} is not valid JSON!")
 			return
```

### Comparing `untypedscript-utsc-0.0.2/src/utsc/uts_parser.py` & `untypedscript-utsc-0.0.3/src/utsc/uts_parser.py`

 * *Files identical despite different names*

