# Comparing `tmp/py-miraie-ac-0.0.3.tar.gz` & `tmp/py-miraie-ac-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-miraie-ac-0.0.3.tar", last modified: Fri Jun  9 08:49:24 2023, max compression
+gzip compressed data, was "py-miraie-ac-0.0.4.tar", last modified: Fri Jun  9 13:05:30 2023, max compression
```

## Comparing `py-miraie-ac-0.0.3.tar` & `py-miraie-ac-0.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 08:49:24.643832 py-miraie-ac-0.0.3/
--rw-rw-rw-   0        0        0    35821 2023-06-09 07:50:41.000000 py-miraie-ac-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     1232 2023-06-09 08:49:24.644832 py-miraie-ac-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      625 2023-06-09 08:48:49.000000 py-miraie-ac-0.0.3/README.md
--rw-rw-rw-   0        0        0      108 2023-06-09 07:29:23.000000 py-miraie-ac-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0      744 2023-06-09 08:49:24.644832 py-miraie-ac-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-09 08:49:24.623774 py-miraie-ac-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-06-09 08:49:24.640832 py-miraie-ac-0.0.3/src/py-miraie-ac/
--rw-rw-rw-   0        0        0        0 2023-05-29 09:16:45.000000 py-miraie-ac-0.0.3/src/py-miraie-ac/__init__.py
--rw-rw-rw-   0        0        0     6036 2023-06-05 04:01:19.000000 py-miraie-ac-0.0.3/src/py-miraie-ac/api.py
--rw-rw-rw-   0        0        0     6210 2023-06-05 03:30:21.000000 py-miraie-ac-0.0.3/src/py-miraie-ac/broker.py
--rw-rw-rw-   0        0        0      421 2023-06-05 03:33:43.000000 py-miraie-ac-0.0.3/src/py-miraie-ac/constants.py
--rw-rw-rw-   0        0        0     4494 2023-06-05 04:00:59.000000 py-miraie-ac-0.0.3/src/py-miraie-ac/device.py
--rw-rw-rw-   0        0        0      846 2023-06-05 03:53:39.000000 py-miraie-ac-0.0.3/src/py-miraie-ac/deviceStatus.py
--rw-rw-rw-   0        0        0      917 2023-06-05 03:55:22.000000 py-miraie-ac-0.0.3/src/py-miraie-ac/enums.py
--rw-rw-rw-   0        0        0      121 2023-06-05 03:55:32.000000 py-miraie-ac-0.0.3/src/py-miraie-ac/exceptions.py
--rw-rw-rw-   0        0        0      470 2023-06-05 03:56:31.000000 py-miraie-ac-0.0.3/src/py-miraie-ac/home.py
--rw-rw-rw-   0        0        0      460 2023-06-05 03:57:35.000000 py-miraie-ac-0.0.3/src/py-miraie-ac/user.py
--rw-rw-rw-   0        0        0      236 2023-06-05 03:59:07.000000 py-miraie-ac-0.0.3/src/py-miraie-ac/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-09 08:49:24.643832 py-miraie-ac-0.0.3/src/py_miraie_ac.egg-info/
--rw-rw-rw-   0        0        0     1232 2023-06-09 08:49:24.000000 py-miraie-ac-0.0.3/src/py_miraie_ac.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      505 2023-06-09 08:49:24.000000 py-miraie-ac-0.0.3/src/py_miraie_ac.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 08:49:24.000000 py-miraie-ac-0.0.3/src/py_miraie_ac.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-06-09 08:49:24.000000 py-miraie-ac-0.0.3/src/py_miraie_ac.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 13:05:30.790069 py-miraie-ac-0.0.4/
+-rw-rw-rw-   0        0        0    35821 2023-06-09 07:50:41.000000 py-miraie-ac-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     1232 2023-06-09 13:05:30.790587 py-miraie-ac-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      625 2023-06-09 08:48:49.000000 py-miraie-ac-0.0.4/README.md
+-rw-rw-rw-   0        0        0      108 2023-06-09 07:29:23.000000 py-miraie-ac-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0      744 2023-06-09 13:05:30.791697 py-miraie-ac-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-09 13:05:30.527839 py-miraie-ac-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-06-09 13:05:30.784029 py-miraie-ac-0.0.4/src/py_miraie_ac/
+-rw-rw-rw-   0        0        0        0 2023-05-29 09:16:45.000000 py-miraie-ac-0.0.4/src/py_miraie_ac/__init__.py
+-rw-rw-rw-   0        0        0     6036 2023-06-05 04:01:19.000000 py-miraie-ac-0.0.4/src/py_miraie_ac/api.py
+-rw-rw-rw-   0        0        0     6210 2023-06-05 03:30:21.000000 py-miraie-ac-0.0.4/src/py_miraie_ac/broker.py
+-rw-rw-rw-   0        0        0      421 2023-06-05 03:33:43.000000 py-miraie-ac-0.0.4/src/py_miraie_ac/constants.py
+-rw-rw-rw-   0        0        0     4494 2023-06-05 04:00:59.000000 py-miraie-ac-0.0.4/src/py_miraie_ac/device.py
+-rw-rw-rw-   0        0        0      846 2023-06-05 03:53:39.000000 py-miraie-ac-0.0.4/src/py_miraie_ac/deviceStatus.py
+-rw-rw-rw-   0        0        0      917 2023-06-05 03:55:22.000000 py-miraie-ac-0.0.4/src/py_miraie_ac/enums.py
+-rw-rw-rw-   0        0        0      121 2023-06-05 03:55:32.000000 py-miraie-ac-0.0.4/src/py_miraie_ac/exceptions.py
+-rw-rw-rw-   0        0        0      470 2023-06-05 03:56:31.000000 py-miraie-ac-0.0.4/src/py_miraie_ac/home.py
+-rw-rw-rw-   0        0        0      460 2023-06-05 03:57:35.000000 py-miraie-ac-0.0.4/src/py_miraie_ac/user.py
+-rw-rw-rw-   0        0        0      236 2023-06-05 03:59:07.000000 py-miraie-ac-0.0.4/src/py_miraie_ac/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-09 13:05:30.788902 py-miraie-ac-0.0.4/src/py_miraie_ac.egg-info/
+-rw-rw-rw-   0        0        0     1232 2023-06-09 13:05:30.000000 py-miraie-ac-0.0.4/src/py_miraie_ac.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      505 2023-06-09 13:05:30.000000 py-miraie-ac-0.0.4/src/py_miraie_ac.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 13:05:30.000000 py-miraie-ac-0.0.4/src/py_miraie_ac.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-09 13:05:30.000000 py-miraie-ac-0.0.4/src/py_miraie_ac.egg-info/top_level.txt
```

### Comparing `py-miraie-ac-0.0.3/LICENSE` & `py-miraie-ac-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `py-miraie-ac-0.0.3/PKG-INFO` & `py-miraie-ac-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-miraie-ac
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package to control and read MirAIe Aircons by Panasonic
 Home-page: https://github.com/milothomas/py-miraie-ac
 Author: Milo Thomas
 Author-email: 20719501+milothomas@users.noreply.github.com
 Project-URL: Bug Tracker, https://github.com/milothomas/py-miraie-ac/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `py-miraie-ac-0.0.3/README.md` & `py-miraie-ac-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `py-miraie-ac-0.0.3/setup.cfg` & `py-miraie-ac-0.0.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 792d 6d69 7261 6965 2d61 630d   = py-miraie-ac.
-00000020: 0a76 6572 7369 6f6e 203d 2030 2e30 2e33  .version = 0.0.3
+00000020: 0a76 6572 7369 6f6e 203d 2030 2e30 2e34  .version = 0.0.4
 00000030: 0d0a 6175 7468 6f72 203d 204d 696c 6f20  ..author = Milo 
 00000040: 5468 6f6d 6173 0d0a 6175 7468 6f72 5f65  Thomas..author_e
 00000050: 6d61 696c 203d 2032 3037 3139 3530 312b  mail = 20719501+
 00000060: 6d69 6c6f 7468 6f6d 6173 4075 7365 7273  milothomas@users
 00000070: 2e6e 6f72 6570 6c79 2e67 6974 6875 622e  .noreply.github.
 00000080: 636f 6d0d 0a64 6573 6372 6970 7469 6f6e  com..description
 00000090: 203d 2041 2070 6163 6b61 6765 2074 6f20   = A package to
```

### Comparing `py-miraie-ac-0.0.3/src/py-miraie-ac/api.py` & `py-miraie-ac-0.0.4/src/py_miraie_ac/api.py`

 * *Files identical despite different names*

### Comparing `py-miraie-ac-0.0.3/src/py-miraie-ac/broker.py` & `py-miraie-ac-0.0.4/src/py_miraie_ac/broker.py`

 * *Files identical despite different names*

### Comparing `py-miraie-ac-0.0.3/src/py-miraie-ac/device.py` & `py-miraie-ac-0.0.4/src/py_miraie_ac/device.py`

 * *Files identical despite different names*

### Comparing `py-miraie-ac-0.0.3/src/py-miraie-ac/deviceStatus.py` & `py-miraie-ac-0.0.4/src/py_miraie_ac/deviceStatus.py`

 * *Files identical despite different names*

### Comparing `py-miraie-ac-0.0.3/src/py-miraie-ac/enums.py` & `py-miraie-ac-0.0.4/src/py_miraie_ac/enums.py`

 * *Files identical despite different names*

### Comparing `py-miraie-ac-0.0.3/src/py_miraie_ac.egg-info/PKG-INFO` & `py-miraie-ac-0.0.4/src/py_miraie_ac.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-miraie-ac
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package to control and read MirAIe Aircons by Panasonic
 Home-page: https://github.com/milothomas/py-miraie-ac
 Author: Milo Thomas
 Author-email: 20719501+milothomas@users.noreply.github.com
 Project-URL: Bug Tracker, https://github.com/milothomas/py-miraie-ac/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

