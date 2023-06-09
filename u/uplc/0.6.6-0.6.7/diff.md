# Comparing `tmp/uplc-0.6.6.tar.gz` & `tmp/uplc-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uplc-0.6.6.tar", max compression
+gzip compressed data, was "uplc-0.6.7.tar", max compression
```

## Comparing `uplc-0.6.6.tar` & `uplc-0.6.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1077 2023-05-08 19:03:17.159501 uplc-0.6.6/LICENSE.txt
--rw-r--r--   0        0        0     2218 2023-05-08 19:03:17.159501 uplc-0.6.6/README.md
--rw-r--r--   0        0        0     1347 2023-05-08 19:03:17.223501 uplc-0.6.6/pyproject.toml
--rw-r--r--   0        0        0      506 2023-05-08 19:03:17.223501 uplc-0.6.6/uplc/__init__.py
--rw-r--r--   0        0        0     4935 2023-05-08 19:03:17.227501 uplc-0.6.6/uplc/__main__.py
--rw-r--r--   0        0        0    28865 2023-05-08 19:03:17.227501 uplc-0.6.6/uplc/ast.py
--rw-r--r--   0        0        0     9066 2023-05-08 19:03:17.227501 uplc-0.6.6/uplc/flat_decoder.py
--rw-r--r--   0        0        0    10052 2023-05-08 19:03:17.227501 uplc-0.6.6/uplc/flat_encoder.py
--rw-r--r--   0        0        0     1202 2023-05-08 19:03:17.227501 uplc-0.6.6/uplc/lexer.py
--rw-r--r--   0        0        0     3357 2023-05-08 19:03:17.227501 uplc-0.6.6/uplc/machine.py
--rw-r--r--   0        0        0        0 2023-05-08 19:03:17.227501 uplc-0.6.6/uplc/optimizer/__init__.py
--rw-r--r--   0        0        0      630 2023-05-08 19:03:17.227501 uplc-0.6.6/uplc/optimizer/pre_evaluation.py
--rw-r--r--   0        0        0    10960 2023-05-08 19:03:17.227501 uplc-0.6.6/uplc/parser.py
--rw-r--r--   0        0        0        0 2023-05-08 19:03:17.227501 uplc-0.6.6/uplc/tests/__init__.py
--rw-r--r--   0        0        0     3391 2023-05-08 19:03:17.227501 uplc-0.6.6/uplc/tests/test_acceptance.py
--rw-r--r--   0        0        0    14584 2023-05-08 19:03:17.227501 uplc-0.6.6/uplc/tests/test_hypothesis.py
--rw-r--r--   0        0        0   211128 2023-05-08 19:03:17.227501 uplc-0.6.6/uplc/tests/test_misc.py
--rw-r--r--   0        0        0     1998 2023-05-08 19:03:17.227501 uplc-0.6.6/uplc/tools.py
--rw-r--r--   0        0        0        0 2023-05-08 19:03:17.227501 uplc-0.6.6/uplc/transformer/__init__.py
--rw-r--r--   0        0        0      784 2023-05-08 19:03:17.227501 uplc-0.6.6/uplc/transformer/debrujin_variables.py
--rw-r--r--   0        0        0      938 2023-05-08 19:03:17.227501 uplc-0.6.6/uplc/transformer/undebrujin_variables.py
--rw-r--r--   0        0        0     1947 2023-05-08 19:03:17.227501 uplc-0.6.6/uplc/transformer/unique_variables.py
--rw-r--r--   0        0        0     3009 2023-05-08 19:03:17.227501 uplc-0.6.6/uplc/util.py
--rw-r--r--   0        0        0     3559 1970-01-01 00:00:00.000000 uplc-0.6.6/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-06-09 09:38:12.221613 uplc-0.6.7/LICENSE.txt
+-rw-r--r--   0        0        0     2218 2023-06-09 09:38:12.221613 uplc-0.6.7/README.md
+-rw-r--r--   0        0        0     1347 2023-06-09 09:38:12.289612 uplc-0.6.7/pyproject.toml
+-rw-r--r--   0        0        0      506 2023-06-09 09:38:12.289612 uplc-0.6.7/uplc/__init__.py
+-rw-r--r--   0        0        0     5177 2023-06-09 09:38:12.289612 uplc-0.6.7/uplc/__main__.py
+-rw-r--r--   0        0        0    28865 2023-06-09 09:38:12.289612 uplc-0.6.7/uplc/ast.py
+-rw-r--r--   0        0        0     9066 2023-06-09 09:38:12.289612 uplc-0.6.7/uplc/flat_decoder.py
+-rw-r--r--   0        0        0    10052 2023-06-09 09:38:12.289612 uplc-0.6.7/uplc/flat_encoder.py
+-rw-r--r--   0        0        0     1202 2023-06-09 09:38:12.289612 uplc-0.6.7/uplc/lexer.py
+-rw-r--r--   0        0        0     3357 2023-06-09 09:38:12.289612 uplc-0.6.7/uplc/machine.py
+-rw-r--r--   0        0        0        0 2023-06-09 09:38:12.289612 uplc-0.6.7/uplc/optimizer/__init__.py
+-rw-r--r--   0        0        0      630 2023-06-09 09:38:12.289612 uplc-0.6.7/uplc/optimizer/pre_evaluation.py
+-rw-r--r--   0        0        0    10960 2023-06-09 09:38:12.289612 uplc-0.6.7/uplc/parser.py
+-rw-r--r--   0        0        0        0 2023-06-09 09:38:12.289612 uplc-0.6.7/uplc/tests/__init__.py
+-rw-r--r--   0        0        0     3391 2023-06-09 09:38:12.289612 uplc-0.6.7/uplc/tests/test_acceptance.py
+-rw-r--r--   0        0        0    14584 2023-06-09 09:38:12.289612 uplc-0.6.7/uplc/tests/test_hypothesis.py
+-rw-r--r--   0        0        0   211128 2023-06-09 09:38:12.293612 uplc-0.6.7/uplc/tests/test_misc.py
+-rw-r--r--   0        0        0     1998 2023-06-09 09:38:12.293612 uplc-0.6.7/uplc/tools.py
+-rw-r--r--   0        0        0        0 2023-06-09 09:38:12.293612 uplc-0.6.7/uplc/transformer/__init__.py
+-rw-r--r--   0        0        0      784 2023-06-09 09:38:12.293612 uplc-0.6.7/uplc/transformer/debrujin_variables.py
+-rw-r--r--   0        0        0      938 2023-06-09 09:38:12.293612 uplc-0.6.7/uplc/transformer/undebrujin_variables.py
+-rw-r--r--   0        0        0     1947 2023-06-09 09:38:12.293612 uplc-0.6.7/uplc/transformer/unique_variables.py
+-rw-r--r--   0        0        0     3009 2023-06-09 09:38:12.293612 uplc-0.6.7/uplc/util.py
+-rw-r--r--   0        0        0     3357 1970-01-01 00:00:00.000000 uplc-0.6.7/PKG-INFO
```

### Comparing `uplc-0.6.6/LICENSE.txt` & `uplc-0.6.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `uplc-0.6.6/README.md` & `uplc-0.6.7/README.md`

 * *Files identical despite different names*

### Comparing `uplc-0.6.6/pyproject.toml` & `uplc-0.6.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "uplc"
-version = "0.6.6"
+version = "0.6.7"
 description = "Python implementation of untyped plutus language core"
 authors = ["nielstron <n.muendler@web.de>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/opshin/uplc"
 keywords = ["python", "language", "programming-language", "compiler", "validator", "smart-contracts", "cardano"]
 classifiers=[
```

### Comparing `uplc-0.6.6/uplc/__main__.py` & `uplc-0.6.7/uplc/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -59,15 +59,22 @@
     )
     a.add_argument(
         "args",
         nargs="*",
         default=[],
         help="Input parameters for the function, in case the command is eval.",
     )
+    a.add_argument(
+        "--recursion-limit",
+        default=sys.getrecursionlimit(),
+        help="Modify the recursion limit (necessary for larger UPLC programs)",
+        type=int,
+    )
     args = a.parse_args()
+    sys.setrecursionlimit(args.recursion_limit)
     command = Command(args.command)
     input_file = pathlib.Path(args.input_file) if args.input_file != "-" else sys.stdin
     with open(input_file, "r") as f:
         source_code = f.read()
 
     if args.from_cbor:
         code = unflatten(bytes.fromhex(source_code))
```

### Comparing `uplc-0.6.6/uplc/ast.py` & `uplc-0.6.7/uplc/ast.py`

 * *Files identical despite different names*

### Comparing `uplc-0.6.6/uplc/flat_decoder.py` & `uplc-0.6.7/uplc/flat_decoder.py`

 * *Files identical despite different names*

### Comparing `uplc-0.6.6/uplc/flat_encoder.py` & `uplc-0.6.7/uplc/flat_encoder.py`

 * *Files identical despite different names*

### Comparing `uplc-0.6.6/uplc/lexer.py` & `uplc-0.6.7/uplc/lexer.py`

 * *Files identical despite different names*

### Comparing `uplc-0.6.6/uplc/machine.py` & `uplc-0.6.7/uplc/machine.py`

 * *Files identical despite different names*

### Comparing `uplc-0.6.6/uplc/optimizer/pre_evaluation.py` & `uplc-0.6.7/uplc/optimizer/pre_evaluation.py`

 * *Files identical despite different names*

### Comparing `uplc-0.6.6/uplc/parser.py` & `uplc-0.6.7/uplc/parser.py`

 * *Files identical despite different names*

### Comparing `uplc-0.6.6/uplc/tests/test_acceptance.py` & `uplc-0.6.7/uplc/tests/test_acceptance.py`

 * *Files identical despite different names*

### Comparing `uplc-0.6.6/uplc/tests/test_hypothesis.py` & `uplc-0.6.7/uplc/tests/test_hypothesis.py`

 * *Files identical despite different names*

### Comparing `uplc-0.6.6/uplc/tests/test_misc.py` & `uplc-0.6.7/uplc/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `uplc-0.6.6/uplc/tools.py` & `uplc-0.6.7/uplc/tools.py`

 * *Files identical despite different names*

### Comparing `uplc-0.6.6/uplc/transformer/debrujin_variables.py` & `uplc-0.6.7/uplc/transformer/debrujin_variables.py`

 * *Files identical despite different names*

### Comparing `uplc-0.6.6/uplc/transformer/undebrujin_variables.py` & `uplc-0.6.7/uplc/transformer/undebrujin_variables.py`

 * *Files identical despite different names*

### Comparing `uplc-0.6.6/uplc/transformer/unique_variables.py` & `uplc-0.6.7/uplc/transformer/unique_variables.py`

 * *Files identical despite different names*

### Comparing `uplc-0.6.6/uplc/util.py` & `uplc-0.6.7/uplc/util.py`

 * *Files identical despite different names*

### Comparing `uplc-0.6.6/PKG-INFO` & `uplc-0.6.7/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uplc
-Version: 0.6.6
+Version: 0.6.7
 Summary: Python implementation of untyped plutus language core
 Home-page: https://github.com/opshin/uplc
 License: MIT
 Keywords: python,language,programming-language,compiler,validator,smart-contracts,cardano
 Author: nielstron
 Author-email: n.muendler@web.de
 Requires-Python: >=3.8,<3.12
@@ -12,18 +12,14 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Assemblers
 Requires-Dist: cbor2 (>=5.4.6,<6.0.0)
 Requires-Dist: frozendict (>=2.3.8,<3.0.0)
 Requires-Dist: frozenlist (>=1.3.3,<2.0.0)
 Requires-Dist: pycardano (>=0.9.0,<0.10.0)
 Requires-Dist: python-secp256k1-cardano (>=0.2.3,<0.3.0)
 Requires-Dist: rply (>=0.7.8,<0.8.0)
```

