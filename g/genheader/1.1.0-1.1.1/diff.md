# Comparing `tmp/genheader-1.1.0.tar.gz` & `tmp/genheader-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genheader-1.1.0.tar", last modified: Fri Jun  9 16:31:55 2023, max compression
+gzip compressed data, was "genheader-1.1.1.tar", last modified: Fri Jun  9 16:46:57 2023, max compression
```

## Comparing `genheader-1.1.0.tar` & `genheader-1.1.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 maplepy   (1000) maplepy   (1000)        0 2023-06-09 16:31:55.742474 genheader-1.1.0/
--rw-r--r--   0 maplepy   (1000) maplepy   (1000)     1211 2023-06-09 13:13:26.000000 genheader-1.1.0/LICENSE
--rw-r--r--   0 maplepy   (1000) maplepy   (1000)      986 2023-06-09 16:31:55.742474 genheader-1.1.0/PKG-INFO
--rw-r--r--   0 maplepy   (1000) maplepy   (1000)      491 2023-06-09 16:07:33.000000 genheader-1.1.0/README.md
--rw-r--r--   0 maplepy   (1000) maplepy   (1000)      103 2023-06-09 13:13:26.000000 genheader-1.1.0/pyproject.toml
--rw-r--r--   0 maplepy   (1000) maplepy   (1000)      675 2023-06-09 16:31:55.742474 genheader-1.1.0/setup.cfg
-drwxr-xr-x   0 maplepy   (1000) maplepy   (1000)        0 2023-06-09 16:31:55.739474 genheader-1.1.0/src/
-drwxr-xr-x   0 maplepy   (1000) maplepy   (1000)        0 2023-06-09 16:31:55.740474 genheader-1.1.0/src/genheader/
--rw-r--r--   0 maplepy   (1000) maplepy   (1000)      989 2023-06-09 16:29:58.000000 genheader-1.1.0/src/genheader/__init__.py
--rwxr-xr-x   0 maplepy   (1000) maplepy   (1000)       87 2023-06-09 16:20:28.000000 genheader-1.1.0/src/genheader/__main__.py
--rw-r--r--   0 maplepy   (1000) maplepy   (1000)      159 2023-06-09 16:25:35.000000 genheader-1.1.0/src/genheader/_version.py
-drwxr-xr-x   0 maplepy   (1000) maplepy   (1000)        0 2023-06-09 16:31:55.741474 genheader-1.1.0/src/genheader/injector/
--rw-r--r--   0 maplepy   (1000) maplepy   (1000)       39 2023-06-09 16:20:28.000000 genheader-1.1.0/src/genheader/injector/__init__.py
--rw-r--r--   0 maplepy   (1000) maplepy   (1000)     2862 2023-06-09 16:29:58.000000 genheader-1.1.0/src/genheader/injector/headers.py
-drwxr-xr-x   0 maplepy   (1000) maplepy   (1000)        0 2023-06-09 16:31:55.741474 genheader-1.1.0/src/genheader/proto/
--rw-r--r--   0 maplepy   (1000) maplepy   (1000)      115 2023-06-09 16:25:45.000000 genheader-1.1.0/src/genheader/proto/__init__.py
--rw-r--r--   0 maplepy   (1000) maplepy   (1000)     3624 2023-06-09 16:29:58.000000 genheader-1.1.0/src/genheader/proto/protos.py
--rw-r--r--   0 maplepy   (1000) maplepy   (1000)     3707 2023-06-09 16:29:58.000000 genheader-1.1.0/src/genheader/proto/sources.py
-drwxr-xr-x   0 maplepy   (1000) maplepy   (1000)        0 2023-06-09 16:31:55.742474 genheader-1.1.0/src/genheader/utils/
--rw-r--r--   0 maplepy   (1000) maplepy   (1000)      157 2023-06-09 16:20:28.000000 genheader-1.1.0/src/genheader/utils/__init__.py
--rw-r--r--   0 maplepy   (1000) maplepy   (1000)     1296 2023-06-09 16:29:58.000000 genheader-1.1.0/src/genheader/utils/arg_parsing.py
--rw-r--r--   0 maplepy   (1000) maplepy   (1000)      639 2023-06-09 16:20:28.000000 genheader-1.1.0/src/genheader/utils/colors.py
--rw-r--r--   0 maplepy   (1000) maplepy   (1000)      715 2023-06-09 16:20:28.000000 genheader-1.1.0/src/genheader/utils/regexrules.py
--rw-r--r--   0 maplepy   (1000) maplepy   (1000)      649 2023-06-09 16:29:58.000000 genheader-1.1.0/src/genheader/utils/utils.py
-drwxr-xr-x   0 maplepy   (1000) maplepy   (1000)        0 2023-06-09 16:31:55.740474 genheader-1.1.0/src/genheader.egg-info/
--rw-r--r--   0 maplepy   (1000) maplepy   (1000)      986 2023-06-09 16:31:55.000000 genheader-1.1.0/src/genheader.egg-info/PKG-INFO
--rw-r--r--   0 maplepy   (1000) maplepy   (1000)      649 2023-06-09 16:31:55.000000 genheader-1.1.0/src/genheader.egg-info/SOURCES.txt
--rw-r--r--   0 maplepy   (1000) maplepy   (1000)        1 2023-06-09 16:31:55.000000 genheader-1.1.0/src/genheader.egg-info/dependency_links.txt
--rw-r--r--   0 maplepy   (1000) maplepy   (1000)       45 2023-06-09 16:31:55.000000 genheader-1.1.0/src/genheader.egg-info/entry_points.txt
--rw-r--r--   0 maplepy   (1000) maplepy   (1000)       10 2023-06-09 16:31:55.000000 genheader-1.1.0/src/genheader.egg-info/top_level.txt
-drwxr-xr-x   0 maplepy   (1000) maplepy   (1000)        0 2023-06-09 16:31:55.742474 genheader-1.1.0/test/
--rw-r--r--   0 maplepy   (1000) maplepy   (1000)      349 2023-06-09 16:29:55.000000 genheader-1.1.0/test/test_proto.py
+drwxr-xr-x   0 maplepy   (1000) maplepy   (1000)        0 2023-06-09 16:46:57.399661 genheader-1.1.1/
+-rw-r--r--   0 maplepy   (1000) maplepy   (1000)     1211 2023-06-09 13:13:26.000000 genheader-1.1.1/LICENSE
+-rw-r--r--   0 maplepy   (1000) maplepy   (1000)      986 2023-06-09 16:46:57.399661 genheader-1.1.1/PKG-INFO
+-rw-r--r--   0 maplepy   (1000) maplepy   (1000)      491 2023-06-09 16:07:33.000000 genheader-1.1.1/README.md
+-rw-r--r--   0 maplepy   (1000) maplepy   (1000)      103 2023-06-09 13:13:26.000000 genheader-1.1.1/pyproject.toml
+-rw-r--r--   0 maplepy   (1000) maplepy   (1000)      675 2023-06-09 16:46:57.400661 genheader-1.1.1/setup.cfg
+drwxr-xr-x   0 maplepy   (1000) maplepy   (1000)        0 2023-06-09 16:46:57.396661 genheader-1.1.1/src/
+drwxr-xr-x   0 maplepy   (1000) maplepy   (1000)        0 2023-06-09 16:46:57.397661 genheader-1.1.1/src/genheader/
+-rw-r--r--   0 maplepy   (1000) maplepy   (1000)      989 2023-06-09 16:29:58.000000 genheader-1.1.1/src/genheader/__init__.py
+-rwxr-xr-x   0 maplepy   (1000) maplepy   (1000)       87 2023-06-09 16:20:28.000000 genheader-1.1.1/src/genheader/__main__.py
+-rw-r--r--   0 maplepy   (1000) maplepy   (1000)      159 2023-06-09 16:25:35.000000 genheader-1.1.1/src/genheader/_version.py
+drwxr-xr-x   0 maplepy   (1000) maplepy   (1000)        0 2023-06-09 16:46:57.398661 genheader-1.1.1/src/genheader/injector/
+-rw-r--r--   0 maplepy   (1000) maplepy   (1000)       39 2023-06-09 16:20:28.000000 genheader-1.1.1/src/genheader/injector/__init__.py
+-rw-r--r--   0 maplepy   (1000) maplepy   (1000)     2862 2023-06-09 16:29:58.000000 genheader-1.1.1/src/genheader/injector/headers.py
+drwxr-xr-x   0 maplepy   (1000) maplepy   (1000)        0 2023-06-09 16:46:57.398661 genheader-1.1.1/src/genheader/proto/
+-rw-r--r--   0 maplepy   (1000) maplepy   (1000)      115 2023-06-09 16:25:45.000000 genheader-1.1.1/src/genheader/proto/__init__.py
+-rw-r--r--   0 maplepy   (1000) maplepy   (1000)     3626 2023-06-09 16:46:36.000000 genheader-1.1.1/src/genheader/proto/protos.py
+-rw-r--r--   0 maplepy   (1000) maplepy   (1000)     3707 2023-06-09 16:29:58.000000 genheader-1.1.1/src/genheader/proto/sources.py
+drwxr-xr-x   0 maplepy   (1000) maplepy   (1000)        0 2023-06-09 16:46:57.399661 genheader-1.1.1/src/genheader/utils/
+-rw-r--r--   0 maplepy   (1000) maplepy   (1000)      157 2023-06-09 16:20:28.000000 genheader-1.1.1/src/genheader/utils/__init__.py
+-rw-r--r--   0 maplepy   (1000) maplepy   (1000)     1296 2023-06-09 16:29:58.000000 genheader-1.1.1/src/genheader/utils/arg_parsing.py
+-rw-r--r--   0 maplepy   (1000) maplepy   (1000)      639 2023-06-09 16:20:28.000000 genheader-1.1.1/src/genheader/utils/colors.py
+-rw-r--r--   0 maplepy   (1000) maplepy   (1000)      715 2023-06-09 16:20:28.000000 genheader-1.1.1/src/genheader/utils/regexrules.py
+-rw-r--r--   0 maplepy   (1000) maplepy   (1000)      649 2023-06-09 16:29:58.000000 genheader-1.1.1/src/genheader/utils/utils.py
+drwxr-xr-x   0 maplepy   (1000) maplepy   (1000)        0 2023-06-09 16:46:57.398661 genheader-1.1.1/src/genheader.egg-info/
+-rw-r--r--   0 maplepy   (1000) maplepy   (1000)      986 2023-06-09 16:46:57.000000 genheader-1.1.1/src/genheader.egg-info/PKG-INFO
+-rw-r--r--   0 maplepy   (1000) maplepy   (1000)      649 2023-06-09 16:46:57.000000 genheader-1.1.1/src/genheader.egg-info/SOURCES.txt
+-rw-r--r--   0 maplepy   (1000) maplepy   (1000)        1 2023-06-09 16:46:57.000000 genheader-1.1.1/src/genheader.egg-info/dependency_links.txt
+-rw-r--r--   0 maplepy   (1000) maplepy   (1000)       45 2023-06-09 16:46:57.000000 genheader-1.1.1/src/genheader.egg-info/entry_points.txt
+-rw-r--r--   0 maplepy   (1000) maplepy   (1000)       10 2023-06-09 16:46:57.000000 genheader-1.1.1/src/genheader.egg-info/top_level.txt
+drwxr-xr-x   0 maplepy   (1000) maplepy   (1000)        0 2023-06-09 16:46:57.399661 genheader-1.1.1/test/
+-rw-r--r--   0 maplepy   (1000) maplepy   (1000)      349 2023-06-09 16:29:55.000000 genheader-1.1.1/test/test_proto.py
```

### Comparing `genheader-1.1.0/LICENSE` & `genheader-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `genheader-1.1.0/PKG-INFO` & `genheader-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genheader
-Version: 1.1.0
+Version: 1.1.1
 Summary: A tool to inject prototypes into header from C files.
 Home-page: https://github.com/maplepy/genheader
 Author: maplepy
 Author-email: your-email@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `genheader-1.1.0/setup.cfg` & `genheader-1.1.1/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = genheader
-version = 1.1.0
+version = 1.1.1
 author = maplepy
 author_email = your-email@example.com
 description = A tool to inject prototypes into header from C files.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/maplepy/genheader
 classifiers =
```

### Comparing `genheader-1.1.0/src/genheader/__init__.py` & `genheader-1.1.1/src/genheader/__init__.py`

 * *Files identical despite different names*

### Comparing `genheader-1.1.0/src/genheader/injector/headers.py` & `genheader-1.1.1/src/genheader/injector/headers.py`

 * *Files identical despite different names*

### Comparing `genheader-1.1.0/src/genheader/proto/protos.py` & `genheader-1.1.1/src/genheader/proto/protos.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
                     else:
                         collected += inparam.lstrip("\t")
             for inside_code in lines:
                 if inside_code == "}":
                     break
 
             self.prototypes.append(f"{collected};")
-            print(f"Prototype found: {collected}")
+            # print(f"Prototype found: {collected}")
 
     def __len__(self) -> int:
         """Return the number of function prototypes."""
         return len(self.prototypes)
 
     def __repr__(self) -> str:
         """Return a string representation of Protos object."""
```

### Comparing `genheader-1.1.0/src/genheader/proto/sources.py` & `genheader-1.1.1/src/genheader/proto/sources.py`

 * *Files identical despite different names*

### Comparing `genheader-1.1.0/src/genheader/utils/arg_parsing.py` & `genheader-1.1.1/src/genheader/utils/arg_parsing.py`

 * *Files identical despite different names*

### Comparing `genheader-1.1.0/src/genheader/utils/colors.py` & `genheader-1.1.1/src/genheader/utils/colors.py`

 * *Files identical despite different names*

### Comparing `genheader-1.1.0/src/genheader/utils/regexrules.py` & `genheader-1.1.1/src/genheader/utils/regexrules.py`

 * *Files identical despite different names*

### Comparing `genheader-1.1.0/src/genheader/utils/utils.py` & `genheader-1.1.1/src/genheader/utils/utils.py`

 * *Files identical despite different names*

### Comparing `genheader-1.1.0/src/genheader.egg-info/PKG-INFO` & `genheader-1.1.1/src/genheader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genheader
-Version: 1.1.0
+Version: 1.1.1
 Summary: A tool to inject prototypes into header from C files.
 Home-page: https://github.com/maplepy/genheader
 Author: maplepy
 Author-email: your-email@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `genheader-1.1.0/src/genheader.egg-info/SOURCES.txt` & `genheader-1.1.1/src/genheader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

