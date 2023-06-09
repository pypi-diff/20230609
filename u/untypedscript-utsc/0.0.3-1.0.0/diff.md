# Comparing `tmp/untypedscript-utsc-0.0.3.tar.gz` & `tmp/untypedscript-utsc-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "untypedscript-utsc-0.0.3.tar", last modified: Fri Jun  9 20:00:06 2023, max compression
+gzip compressed data, was "untypedscript-utsc-1.0.0.tar", last modified: Fri Jun  9 20:33:38 2023, max compression
```

## Comparing `untypedscript-utsc-0.0.3.tar` & `untypedscript-utsc-1.0.0.tar`

### file list

```diff
@@ -1,23 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 20:00:06.469460 untypedscript-utsc-0.0.3/
--rw-rw-rw-   0        0        0     1090 2023-06-09 18:03:17.000000 untypedscript-utsc-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     6567 2023-06-09 20:00:06.467034 untypedscript-utsc-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     4967 2023-06-07 01:23:46.000000 untypedscript-utsc-0.0.3/README.md
--rw-rw-rw-   0        0        0      710 2023-06-09 19:59:11.000000 untypedscript-utsc-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-09 20:00:06.470455 untypedscript-utsc-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-09 20:00:06.361741 untypedscript-utsc-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-06-09 20:00:06.399765 untypedscript-utsc-0.0.3/src/untypedscript_utsc.egg-info/
--rw-rw-rw-   0        0        0     6567 2023-06-09 20:00:06.000000 untypedscript-utsc-0.0.3/src/untypedscript_utsc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      477 2023-06-09 20:00:06.000000 untypedscript-utsc-0.0.3/src/untypedscript_utsc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 20:00:06.000000 untypedscript-utsc-0.0.3/src/untypedscript_utsc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-06-09 20:00:06.000000 untypedscript-utsc-0.0.3/src/untypedscript_utsc.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-06-09 20:00:06.000000 untypedscript-utsc-0.0.3/src/untypedscript_utsc.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-09 20:00:06.461063 untypedscript-utsc-0.0.3/src/utsc/
--rw-rw-rw-   0        0        0     9308 2023-06-09 18:48:37.000000 untypedscript-utsc-0.0.3/src/utsc/__init__.py
--rw-rw-rw-   0        0        0      576 2023-02-24 02:16:29.000000 untypedscript-utsc-0.0.3/src/utsc/ast_cleaner.py
--rw-rw-rw-   0        0        0     2734 2023-06-09 18:44:30.000000 untypedscript-utsc-0.0.3/src/utsc/ast_preprocessor.py
--rw-rw-rw-   0        0        0     7217 2023-06-09 18:44:28.000000 untypedscript-utsc-0.0.3/src/utsc/code_lowerer.py
--rw-rw-rw-   0        0        0    36276 2023-06-09 18:44:23.000000 untypedscript-utsc-0.0.3/src/utsc/compiler.py
--rw-rw-rw-   0        0        0     2340 2023-06-04 23:42:15.000000 untypedscript-utsc-0.0.3/src/utsc/optimizer.py
--rw-rw-rw-   0        0        0     7829 2023-06-09 18:44:10.000000 untypedscript-utsc-0.0.3/src/utsc/sequential_lexer.py
--rw-rw-rw-   0        0        0     4817 2023-06-09 19:19:00.000000 untypedscript-utsc-0.0.3/src/utsc/utils.py
--rw-rw-rw-   0        0        0    39560 2023-06-09 18:44:01.000000 untypedscript-utsc-0.0.3/src/utsc/uts_parser.py
+drwxrwxrwx   0        0        0        0 2023-06-09 20:33:38.427480 untypedscript-utsc-1.0.0/
+-rw-rw-rw-   0        0        0     1090 2023-06-09 18:03:17.000000 untypedscript-utsc-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0       49 2023-06-09 20:08:40.000000 untypedscript-utsc-1.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     6644 2023-06-09 20:33:38.425475 untypedscript-utsc-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4967 2023-06-07 01:23:46.000000 untypedscript-utsc-1.0.0/README.md
+-rw-rw-rw-   0        0        0      648 2023-06-09 20:19:57.000000 untypedscript-utsc-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-09 20:33:38.427480 untypedscript-utsc-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-09 20:33:38.322118 untypedscript-utsc-1.0.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-09 20:33:38.354076 untypedscript-utsc-1.0.0/src/untypedscript_utsc.egg-info/
+-rw-rw-rw-   0        0        0     6644 2023-06-09 20:33:38.000000 untypedscript-utsc-1.0.0/src/untypedscript_utsc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      774 2023-06-09 20:33:38.000000 untypedscript-utsc-1.0.0/src/untypedscript_utsc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 20:33:38.000000 untypedscript-utsc-1.0.0/src/untypedscript_utsc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-06-09 20:33:38.000000 untypedscript-utsc-1.0.0/src/untypedscript_utsc.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       13 2023-06-09 20:33:38.000000 untypedscript-utsc-1.0.0/src/untypedscript_utsc.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 20:33:38.321110 untypedscript-utsc-1.0.0/src/uts-lib/
+drwxrwxrwx   0        0        0        0 2023-06-09 20:33:38.360422 untypedscript-utsc-1.0.0/src/uts-lib/typed/
+-rw-rw-rw-   0        0        0     2521 2023-06-04 21:46:35.000000 untypedscript-utsc-1.0.0/src/uts-lib/typed/io.uts
+-rw-rw-rw-   0        0        0      215 2023-05-01 19:54:36.000000 untypedscript-utsc-1.0.0/src/uts-lib/typed/typed-value.uts
+drwxrwxrwx   0        0        0        0 2023-06-09 20:33:38.369630 untypedscript-utsc-1.0.0/src/uts-lib/utils/
+-rw-rw-rw-   0        0        0      457 2023-04-26 20:34:59.000000 untypedscript-utsc-1.0.0/src/uts-lib/utils/math.uts
+-rw-rw-rw-   0        0        0     2225 2023-06-04 21:32:06.000000 untypedscript-utsc-1.0.0/src/uts-lib/utils/obj.uts
+-rw-rw-rw-   0        0        0      183 2023-04-10 00:56:50.000000 untypedscript-utsc-1.0.0/src/uts-lib/utils/uts-array.uts
+drwxrwxrwx   0        0        0        0 2023-06-09 20:33:38.378802 untypedscript-utsc-1.0.0/src/uts-lib/utils/win32/
+-rw-rw-rw-   0        0        0      812 2023-04-27 12:38:42.000000 untypedscript-utsc-1.0.0/src/uts-lib/utils/win32/async.uts
+-rw-rw-rw-   0        0        0     1629 2023-06-09 00:35:56.000000 untypedscript-utsc-1.0.0/src/uts-lib/utils/win32/heapfuncs-nouse.uts
+-rw-rw-rw-   0        0        0     2318 2023-06-09 00:39:22.000000 untypedscript-utsc-1.0.0/src/uts-lib/utils/win32/libheapfunc.o
+drwxrwxrwx   0        0        0        0 2023-06-09 20:33:38.385323 untypedscript-utsc-1.0.0/src/uts-lib/uts/
+-rw-rw-rw-   0        0        0       74 2023-06-04 16:59:55.000000 untypedscript-utsc-1.0.0/src/uts-lib/uts/info.uts
+drwxrwxrwx   0        0        0        0 2023-06-09 20:33:38.420454 untypedscript-utsc-1.0.0/src/utsc/
+-rw-rw-rw-   0        0        0     9311 2023-06-09 20:30:35.000000 untypedscript-utsc-1.0.0/src/utsc/__init__.py
+-rw-rw-rw-   0        0        0      576 2023-02-24 02:16:29.000000 untypedscript-utsc-1.0.0/src/utsc/ast_cleaner.py
+-rw-rw-rw-   0        0        0     2734 2023-06-09 18:44:30.000000 untypedscript-utsc-1.0.0/src/utsc/ast_preprocessor.py
+-rw-rw-rw-   0        0        0     7217 2023-06-09 18:44:28.000000 untypedscript-utsc-1.0.0/src/utsc/code_lowerer.py
+-rw-rw-rw-   0        0        0    36176 2023-06-09 20:31:27.000000 untypedscript-utsc-1.0.0/src/utsc/compiler.py
+-rw-rw-rw-   0        0        0     2340 2023-06-04 23:42:15.000000 untypedscript-utsc-1.0.0/src/utsc/optimizer.py
+-rw-rw-rw-   0        0        0     7829 2023-06-09 18:44:10.000000 untypedscript-utsc-1.0.0/src/utsc/sequential_lexer.py
+-rw-rw-rw-   0        0        0     4817 2023-06-09 19:19:00.000000 untypedscript-utsc-1.0.0/src/utsc/utils.py
+-rw-rw-rw-   0        0        0    39560 2023-06-09 18:44:01.000000 untypedscript-utsc-1.0.0/src/utsc/uts_parser.py
```

### Comparing `untypedscript-utsc-0.0.3/LICENSE` & `untypedscript-utsc-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `untypedscript-utsc-0.0.3/PKG-INFO` & `untypedscript-utsc-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: untypedscript-utsc
-Version: 0.0.3
+Version: 1.0.0
 Summary: UntypedScript original implementation compiler
 Author-email: Carl Furtado <carlzfurtado@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Carl Furtado
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -22,14 +22,15 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/User0332/UntypedScript
+Project-URL: Documentation, https://untypedscript.readthedocs.io/en/latest/
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # UntypedScript
 
 Project that branched off of the discontinued [PogScript](https://github.com/User0332/PogScript), with a considerably different JavaScript-like syntax. UntypedScript's goal is to become an easy-to-understand and easy-to-write language with speeds comparable to that of C or C++. Version `1.0.0` of the language will be published and available for download as soon as floats are introduced and error throwing is fixed (see the [todo list](#next-on-the-list-to-do)). The todo list is not necessarily based on an order of priority, although many low-priority tasks are near the end of the list.
```

### Comparing `untypedscript-utsc-0.0.3/README.md` & `untypedscript-utsc-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `untypedscript-utsc-0.0.3/pyproject.toml` & `untypedscript-utsc-1.0.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "untypedscript-utsc"
-version = "0.0.3"
+version = "1.0.0"
 description = "UntypedScript original implementation compiler"
 readme = "README.md"
 authors = [{ name = "Carl Furtado", email = "carlzfurtado@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = []
 keywords = []
 dependencies = []
 requires-python = ">= 3.9"
 
 [project.urls]
 Homepage = "https://github.com/User0332/UntypedScript"
-# Documentation = "https://webpy-framework.readthedocs.io/"
+Documentation = "https://untypedscript.readthedocs.io/en/latest/"
 
 [project.scripts]
 utsc = "utsc:main"
-utsc-configure = "utsc:configure"
-
-[tool.setuptools.package-data]
-lib = ["*.uts", "libheapfunc.o"]
+utsc-configure = "utsc:configure"
```

### Comparing `untypedscript-utsc-0.0.3/src/untypedscript_utsc.egg-info/PKG-INFO` & `untypedscript-utsc-1.0.0/src/untypedscript_utsc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: untypedscript-utsc
-Version: 0.0.3
+Version: 1.0.0
 Summary: UntypedScript original implementation compiler
 Author-email: Carl Furtado <carlzfurtado@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Carl Furtado
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -22,14 +22,15 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/User0332/UntypedScript
+Project-URL: Documentation, https://untypedscript.readthedocs.io/en/latest/
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # UntypedScript
 
 Project that branched off of the discontinued [PogScript](https://github.com/User0332/PogScript), with a considerably different JavaScript-like syntax. UntypedScript's goal is to become an easy-to-understand and easy-to-write language with speeds comparable to that of C or C++. Version `1.0.0` of the language will be published and available for download as soon as floats are introduced and error throwing is fixed (see the [todo list](#next-on-the-list-to-do)). The todo list is not necessarily based on an order of priority, although many low-priority tasks are near the end of the list.
```

### Comparing `untypedscript-utsc-0.0.3/src/utsc/__init__.py` & `untypedscript-utsc-1.0.0/src/utsc/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 )
 
 # OTHER UTILITY MODULES
 from json import (
 	dumps, dump
 )
 
+from importlib import import_module
+
 
 #SYSTEM MODULES
 from subprocess import (
 	call as subprocess_call
 )
 
 from os import (
@@ -48,18 +50,17 @@
 from sys import (
 	exit,
 	argv,
 	platform as sys_platform
 )
 
 
-#Indepenedent Environment Constants
-COMPILER_EXE_PATH = dirname(argv[0]).replace('\\', '/')
-#
-
+COMPILER_EXE_PATH: str = dirname(
+	import_module("utsc").__file__
+).replace('\\', '/')
 
 def main():
 	argparser = ArgParser(description="PogScript Compiler", prog = "pogc2")
 	
 	argparser.add_argument("-d", "--dump", type=str, help="show AST, tokens, disassembly, unprocessed or ALL (unprocessed is not included in ALL)")
 	argparser.add_argument("-s", "--suppresswarnings", help="suppress all warnings", action="store_true", default=False)
 	argparser.add_argument("filename", nargs='?', default='', type=str, help='Source file')
@@ -101,19 +102,17 @@
 
 	try:
 		with open(file, 'r') as f:
 			code = f.read()
 	except OSError:
 		throw("Fatal Error UTSC 003: Either the specified source file could not be found, or permission was denied.")
 
-	#Dependent Constants
 	INPUT_FILE_PATH = dirname(file).replace("\\", "/")
 	if INPUT_FILE_PATH == '':
 		INPUT_FILE_PATH = "./"
-	#
 
 	chdir(INPUT_FILE_PATH)
 
 	basesource = ".".join(basename(file).split(".")[:-1])
 
 	if args.out == None:
 		out = basesource+".o"
```

### Comparing `untypedscript-utsc-0.0.3/src/utsc/ast_cleaner.py` & `untypedscript-utsc-1.0.0/src/utsc/ast_cleaner.py`

 * *Files identical despite different names*

### Comparing `untypedscript-utsc-0.0.3/src/utsc/ast_preprocessor.py` & `untypedscript-utsc-1.0.0/src/utsc/ast_preprocessor.py`

 * *Files identical despite different names*

### Comparing `untypedscript-utsc-0.0.3/src/utsc/code_lowerer.py` & `untypedscript-utsc-1.0.0/src/utsc/code_lowerer.py`

 * *Files identical despite different names*

### Comparing `untypedscript-utsc-0.0.3/src/utsc/compiler.py` & `untypedscript-utsc-1.0.0/src/utsc/compiler.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 		self.symbols = SymbolTable(code)
 		self.evaluator = SyntaxTreePreproccesor(ast)
 		self.source = code
 		self.structs: dict[str, list[str]] = structs
 		self.used_counters: list[int] = []
 		self.hidden_cached: int = None
 		self.optimize = optimize
-		self.compiler_path = compiler_path+'/..' if compiler_path.endswith("src") else compiler_path # this will point to the src folder, we want it to point to root proj directory
+		self.compiler_path = compiler_path+'/..'
 		self.file_path = file_path
 		self.filename = filename
 		self.link_with: list[str] = []
 		self.exports: list[str] = []
 		self.imported_modinfo: dict[str, dict[str, Union[list[str], dict]]] = {}
 		self.names_from: dict[str, str] = {}
 		self.in_namespace: list[str] = []
@@ -188,17 +188,17 @@
 		module = node["module"]
 
 		self.imported_names.extend(names)
 
 		uts_mod = normpath(f"{self.file_path}/{module}.uts")
 		modinfo = normpath(f"{module}.modinfo")
 		asm_mod = normpath(f"{self.file_path}/{module}.asm")
-		lib_uts_mod = normpath(f"{self.compiler_path}/lib/{module}.uts")
-		lib_modinfo = normpath(f"{self.compiler_path}/lib/{module}.modinfo")
-		lib_obj_mod = normpath(f"{self.compiler_path}/lib/{module}.o")
+		lib_uts_mod = normpath(f"{self.compiler_path}/uts-lib/{module}.uts")
+		lib_modinfo = normpath(f"{self.compiler_path}/uts-lib/{module}.modinfo")
+		lib_obj_mod = normpath(f"{self.compiler_path}/uts-lib/{module}.o")
 		obj_mod = normpath(f"{self.file_path}/{module}.o")
 
 		if (not isfile(uts_mod) and isfile(lib_uts_mod)):
 			uts_mod = lib_uts_mod
 			modinfo = lib_modinfo
 			obj_mod = lib_obj_mod
 
@@ -285,17 +285,17 @@
 	def import_ns(self, node: dict):
 		ns_names: list[str] = node["names"]
 		module: module = node["module"]
 		idx: int = node["index"]
 
 		uts_mod = normpath(f"{self.file_path}/{module}.uts")
 		modinfo = normpath(f"{module}.modinfo")
-		lib_uts_mod = normpath(f"{self.compiler_path}/lib/{module}.uts")
-		lib_modinfo = normpath(f"{self.compiler_path}/lib/{module}.modinfo")
-		lib_obj_mod = normpath(f"{self.compiler_path}/lib/{module}.o")
+		lib_uts_mod = normpath(f"{self.compiler_path}/uts-lib/{module}.uts")
+		lib_modinfo = normpath(f"{self.compiler_path}/uts-lib/{module}.modinfo")
+		lib_obj_mod = normpath(f"{self.compiler_path}/uts-lib/{module}.o")
 		obj_mod = normpath(f"{self.file_path}/{module}.o")
 
 		if not isfile(uts_mod):
 			uts_mod = lib_uts_mod
 			modinfo = lib_modinfo
 			obj_mod = lib_obj_mod
 
@@ -372,16 +372,16 @@
 	def import_struct(self, node: dict):
 		struct_names: list[str] = node["names"]
 		module: module = node["module"]
 		idx: int = node["index"]
 
 		uts_mod = normpath(f"{self.file_path}/{module}.uts")
 		struct_mod = normpath(f"{self.file_path}/{module}.structs")
-		lib_uts_mod = normpath(f"{self.compiler_path}/lib/{module}.uts")
-		lib_struct_mod = normpath(f"{self.compiler_path}/lib/{module}.structs")
+		lib_uts_mod = normpath(f"{self.compiler_path}/uts-lib/{module}.uts")
+		lib_struct_mod = normpath(f"{self.compiler_path}/uts-lib/{module}.structs")
 
 
 		if not isfile(uts_mod):
 			uts_mod = lib_uts_mod
 			struct_mod = lib_struct_mod
 
 		if sys_platform == "win32":
```

### Comparing `untypedscript-utsc-0.0.3/src/utsc/optimizer.py` & `untypedscript-utsc-1.0.0/src/utsc/optimizer.py`

 * *Files identical despite different names*

### Comparing `untypedscript-utsc-0.0.3/src/utsc/sequential_lexer.py` & `untypedscript-utsc-1.0.0/src/utsc/sequential_lexer.py`

 * *Files identical despite different names*

### Comparing `untypedscript-utsc-0.0.3/src/utsc/utils.py` & `untypedscript-utsc-1.0.0/src/utsc/utils.py`

 * *Files identical despite different names*

### Comparing `untypedscript-utsc-0.0.3/src/utsc/uts_parser.py` & `untypedscript-utsc-1.0.0/src/utsc/uts_parser.py`

 * *Files identical despite different names*

