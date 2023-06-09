# Comparing `tmp/pubpypack-harmony-bill-melvin-0.0.2.tar.gz` & `tmp/pubpypack-harmony-bill-melvin-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pubpypack-harmony-bill-melvin-0.0.2.tar", last modified: Thu Jun  8 13:00:37 2023, max compression
+gzip compressed data, was "pubpypack-harmony-bill-melvin-0.0.4.tar", last modified: Fri Jun  9 14:59:18 2023, max compression
```

## Comparing `pubpypack-harmony-bill-melvin-0.0.2.tar` & `pubpypack-harmony-bill-melvin-0.0.4.tar`

### file list

```diff
@@ -1,36 +1,25 @@
-drwxrwxr-x   0 bill      (1000) bill      (1000)        0 2023-06-08 13:00:37.133678 pubpypack-harmony-bill-melvin-0.0.2/
--rw-rw-r--   0 bill      (1000) bill      (1000)     1071 2023-04-06 23:40:32.000000 pubpypack-harmony-bill-melvin-0.0.2/LICENSE
--rw-rw-r--   0 bill      (1000) bill      (1000)       50 2023-04-09 12:50:08.000000 pubpypack-harmony-bill-melvin-0.0.2/MANIFEST.in
--rw-rw-r--   0 bill      (1000) bill      (1000)      618 2023-06-08 13:00:37.133678 pubpypack-harmony-bill-melvin-0.0.2/PKG-INFO
--rw-rw-r--   0 bill      (1000) bill      (1000)      189 2023-06-08 12:55:39.000000 pubpypack-harmony-bill-melvin-0.0.2/README.md
--rw-rw-r--   0 bill      (1000) bill      (1000)      167 2023-06-03 20:42:44.000000 pubpypack-harmony-bill-melvin-0.0.2/pyproject.toml
--rw-rw-r--   0 bill      (1000) bill      (1000)     1894 2023-06-08 13:00:37.137678 pubpypack-harmony-bill-melvin-0.0.2/setup.cfg
--rw-rw-r--   0 bill      (1000) bill      (1000)      145 2023-04-16 11:29:27.000000 pubpypack-harmony-bill-melvin-0.0.2/setup.py
-drwxrwxr-x   0 bill      (1000) bill      (1000)        0 2023-06-08 13:00:37.125678 pubpypack-harmony-bill-melvin-0.0.2/src/
--rw-r--r--   0 bill      (1000) bill      (1000)    53248 2023-05-07 17:33:39.000000 pubpypack-harmony-bill-melvin-0.0.2/src/.coverage
-drwxrwxr-x   0 bill      (1000) bill      (1000)        0 2023-06-08 13:00:37.129678 pubpypack-harmony-bill-melvin-0.0.2/src/first_python_package.egg-info/
--rw-rw-r--   0 bill      (1000) bill      (1000)      529 2023-06-03 20:28:31.000000 pubpypack-harmony-bill-melvin-0.0.2/src/first_python_package.egg-info/PKG-INFO
--rw-rw-r--   0 bill      (1000) bill      (1000)      660 2023-06-03 20:28:31.000000 pubpypack-harmony-bill-melvin-0.0.2/src/first_python_package.egg-info/SOURCES.txt
--rw-rw-r--   0 bill      (1000) bill      (1000)        1 2023-06-03 20:28:31.000000 pubpypack-harmony-bill-melvin-0.0.2/src/first_python_package.egg-info/dependency_links.txt
--rw-rw-r--   0 bill      (1000) bill      (1000)       48 2023-06-03 20:28:31.000000 pubpypack-harmony-bill-melvin-0.0.2/src/first_python_package.egg-info/entry_points.txt
--rw-rw-r--   0 bill      (1000) bill      (1000)       20 2023-06-03 20:28:31.000000 pubpypack-harmony-bill-melvin-0.0.2/src/first_python_package.egg-info/requires.txt
--rw-rw-r--   0 bill      (1000) bill      (1000)        7 2023-06-03 20:28:31.000000 pubpypack-harmony-bill-melvin-0.0.2/src/first_python_package.egg-info/top_level.txt
-drwxrwxr-x   0 bill      (1000) bill      (1000)        0 2023-06-08 13:00:37.129678 pubpypack-harmony-bill-melvin-0.0.2/src/imppkg/
--rw-rw-r--   0 bill      (1000) bill      (1000)        2 2023-04-09 12:26:04.000000 pubpypack-harmony-bill-melvin-0.0.2/src/imppkg/__init__.py
-drwxrwxr-x   0 bill      (1000) bill      (1000)        0 2023-06-08 13:00:37.129678 pubpypack-harmony-bill-melvin-0.0.2/src/imppkg/__pycache__/
--rw-rw-r--   0 bill      (1000) bill      (1000)      186 2023-05-13 00:28:43.000000 pubpypack-harmony-bill-melvin-0.0.2/src/imppkg/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 bill      (1000) bill      (1000)      769 2023-05-13 00:28:43.000000 pubpypack-harmony-bill-melvin-0.0.2/src/imppkg/__pycache__/harmony.cpython-310.pyc
--rw-rw-r--   0 bill      (1000) bill      (1000)       19 2023-04-09 12:45:01.000000 pubpypack-harmony-bill-melvin-0.0.2/src/imppkg/data.json
--rw-rw-r--   0 bill      (1000) bill      (1000)   146334 2023-04-25 13:38:37.000000 pubpypack-harmony-bill-melvin-0.0.2/src/imppkg/harmonic_mean.c
--rw-rw-r--   0 bill      (1000) bill      (1000)      252 2023-04-25 13:38:01.000000 pubpypack-harmony-bill-melvin-0.0.2/src/imppkg/harmonic_mean.pyx
--rw-rw-r--   0 bill      (1000) bill      (1000)      612 2023-06-02 20:07:19.000000 pubpypack-harmony-bill-melvin-0.0.2/src/imppkg/harmony.py
--rw-rw-r--   0 bill      (1000) bill      (1000)        2 2023-06-02 20:16:27.000000 pubpypack-harmony-bill-melvin-0.0.2/src/imppkg/py.typed
-drwxrwxr-x   0 bill      (1000) bill      (1000)        0 2023-06-08 13:00:37.133678 pubpypack-harmony-bill-melvin-0.0.2/src/pubpypack_harmony_bill_melvin.egg-info/
--rw-rw-r--   0 bill      (1000) bill      (1000)      618 2023-06-08 13:00:37.000000 pubpypack-harmony-bill-melvin-0.0.2/src/pubpypack_harmony_bill_melvin.egg-info/PKG-INFO
--rw-rw-r--   0 bill      (1000) bill      (1000)     1004 2023-06-08 13:00:37.000000 pubpypack-harmony-bill-melvin-0.0.2/src/pubpypack_harmony_bill_melvin.egg-info/SOURCES.txt
--rw-rw-r--   0 bill      (1000) bill      (1000)        1 2023-06-08 13:00:37.000000 pubpypack-harmony-bill-melvin-0.0.2/src/pubpypack_harmony_bill_melvin.egg-info/dependency_links.txt
--rw-rw-r--   0 bill      (1000) bill      (1000)       48 2023-06-08 13:00:37.000000 pubpypack-harmony-bill-melvin-0.0.2/src/pubpypack_harmony_bill_melvin.egg-info/entry_points.txt
--rw-rw-r--   0 bill      (1000) bill      (1000)       20 2023-06-08 13:00:37.000000 pubpypack-harmony-bill-melvin-0.0.2/src/pubpypack_harmony_bill_melvin.egg-info/requires.txt
--rw-rw-r--   0 bill      (1000) bill      (1000)        7 2023-06-08 13:00:37.000000 pubpypack-harmony-bill-melvin-0.0.2/src/pubpypack_harmony_bill_melvin.egg-info/top_level.txt
-drwxrwxr-x   0 bill      (1000) bill      (1000)        0 2023-06-08 13:00:37.133678 pubpypack-harmony-bill-melvin-0.0.2/test/
--rw-rw-r--   0 bill      (1000) bill      (1000)      471 2023-06-03 20:27:47.000000 pubpypack-harmony-bill-melvin-0.0.2/test/test_harmonic_mean.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:59:18.645728 pubpypack-harmony-bill-melvin-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-09 14:59:02.000000 pubpypack-harmony-bill-melvin-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-09 14:59:02.000000 pubpypack-harmony-bill-melvin-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-09 14:59:18.649728 pubpypack-harmony-bill-melvin-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-09 14:59:02.000000 pubpypack-harmony-bill-melvin-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-09 14:59:02.000000 pubpypack-harmony-bill-melvin-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-06-09 14:59:18.649728 pubpypack-harmony-bill-melvin-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-09 14:59:02.000000 pubpypack-harmony-bill-melvin-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:59:18.641728 pubpypack-harmony-bill-melvin-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:59:18.645728 pubpypack-harmony-bill-melvin-0.0.4/src/imppkg/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-09 14:59:02.000000 pubpypack-harmony-bill-melvin-0.0.4/src/imppkg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-09 14:59:02.000000 pubpypack-harmony-bill-melvin-0.0.4/src/imppkg/data.json
+-rw-r--r--   0 runner    (1001) docker     (123)   146537 2023-06-09 14:59:18.000000 pubpypack-harmony-bill-melvin-0.0.4/src/imppkg/harmonic_mean.c
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-09 14:59:02.000000 pubpypack-harmony-bill-melvin-0.0.4/src/imppkg/harmonic_mean.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-09 14:59:02.000000 pubpypack-harmony-bill-melvin-0.0.4/src/imppkg/harmony.py
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-09 14:59:02.000000 pubpypack-harmony-bill-melvin-0.0.4/src/imppkg/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:59:18.645728 pubpypack-harmony-bill-melvin-0.0.4/src/pubpypack_harmony_bill_melvin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-09 14:59:18.000000 pubpypack-harmony-bill-melvin-0.0.4/src/pubpypack_harmony_bill_melvin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-09 14:59:18.000000 pubpypack-harmony-bill-melvin-0.0.4/src/pubpypack_harmony_bill_melvin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 14:59:18.000000 pubpypack-harmony-bill-melvin-0.0.4/src/pubpypack_harmony_bill_melvin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-09 14:59:18.000000 pubpypack-harmony-bill-melvin-0.0.4/src/pubpypack_harmony_bill_melvin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-09 14:59:18.000000 pubpypack-harmony-bill-melvin-0.0.4/src/pubpypack_harmony_bill_melvin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-09 14:59:18.000000 pubpypack-harmony-bill-melvin-0.0.4/src/pubpypack_harmony_bill_melvin.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:59:18.645728 pubpypack-harmony-bill-melvin-0.0.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-09 14:59:02.000000 pubpypack-harmony-bill-melvin-0.0.4/test/test_harmonic_mean.py
```

### Comparing `pubpypack-harmony-bill-melvin-0.0.2/LICENSE` & `pubpypack-harmony-bill-melvin-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pubpypack-harmony-bill-melvin-0.0.2/PKG-INFO` & `pubpypack-harmony-bill-melvin-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pubpypack-harmony-bill-melvin
-Version: 0.0.2
+Version: 0.0.4
 Summary: Working the exercises in Publishing Python Packages by Dane Hillard
 Home-page: https://github.com/wmelvin/first-python-package
 Author: Bill Melvin
 Author-email: "Bill Melvin" <bill@billmelvin.com>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `pubpypack-harmony-bill-melvin-0.0.2/setup.cfg` & `pubpypack-harmony-bill-melvin-0.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pubpypack-harmony-bill-melvin
-version = 0.0.2
+version = 0.0.4
 url = https://github.com/wmelvin/first-python-package
 author = Bill Melvin
 author_email = "Bill Melvin" <bill@billmelvin.com>
 description = Working the exercises in Publishing Python Packages by Dane Hillard
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
```

### Comparing `pubpypack-harmony-bill-melvin-0.0.2/src/imppkg/harmonic_mean.c` & `pubpypack-harmony-bill-melvin-0.0.4/src/imppkg/harmonic_mean.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.34 */
+/* Generated by Cython 0.29.35 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "name": "imppkg.harmonic_mean",
         "sources": [
             "./src/imppkg/harmonic_mean.pyx"
@@ -17,16 +17,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_34"
-#define CYTHON_HEX_VERSION 0x001D22F0
+#define CYTHON_ABI "0_29_35"
+#define CYTHON_HEX_VERSION 0x001D23F0
 #define CYTHON_FUTURE_DIVISION 0
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -86,16 +86,20 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
@@ -3052,15 +3056,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -3248,15 +3252,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
```

### Comparing `pubpypack-harmony-bill-melvin-0.0.2/src/imppkg/harmony.py` & `pubpypack-harmony-bill-melvin-0.0.4/src/imppkg/harmony.py`

 * *Files identical despite different names*

### Comparing `pubpypack-harmony-bill-melvin-0.0.2/src/pubpypack_harmony_bill_melvin.egg-info/PKG-INFO` & `pubpypack-harmony-bill-melvin-0.0.4/src/pubpypack_harmony_bill_melvin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pubpypack-harmony-bill-melvin
-Version: 0.0.2
+Version: 0.0.4
 Summary: Working the exercises in Publishing Python Packages by Dane Hillard
 Home-page: https://github.com/wmelvin/first-python-package
 Author: Bill Melvin
 Author-email: "Bill Melvin" <bill@billmelvin.com>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

