# Comparing `tmp/py-miraie-ac-0.0.6.tar.gz` & `tmp/py-miraie-ac-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-miraie-ac-0.0.6.tar", last modified: Fri Jun  9 13:29:51 2023, max compression
+gzip compressed data, was "py-miraie-ac-0.0.8.tar", last modified: Fri Jun  9 16:12:51 2023, max compression
```

## Comparing `py-miraie-ac-0.0.6.tar` & `py-miraie-ac-0.0.8.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 13:29:51.643589 py-miraie-ac-0.0.6/
--rw-rw-rw-   0        0        0    35821 2023-06-09 07:50:41.000000 py-miraie-ac-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     1232 2023-06-09 13:29:51.643589 py-miraie-ac-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      625 2023-06-09 08:48:49.000000 py-miraie-ac-0.0.6/README.md
--rw-rw-rw-   0        0        0      108 2023-06-09 07:29:23.000000 py-miraie-ac-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0      744 2023-06-09 13:29:51.645592 py-miraie-ac-0.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-09 13:29:51.621510 py-miraie-ac-0.0.6/src/
-drwxrwxrwx   0        0        0        0 2023-06-09 13:29:51.638594 py-miraie-ac-0.0.6/src/py_miraie_ac/
--rw-rw-rw-   0        0        0      403 2023-06-09 13:16:33.000000 py-miraie-ac-0.0.6/src/py_miraie_ac/__init__.py
--rw-rw-rw-   0        0        0     6172 2023-06-09 13:28:16.000000 py-miraie-ac-0.0.6/src/py_miraie_ac/api.py
--rw-rw-rw-   0        0        0     6221 2023-06-09 13:28:36.000000 py-miraie-ac-0.0.6/src/py_miraie_ac/broker.py
--rw-rw-rw-   0        0        0      421 2023-06-05 03:33:43.000000 py-miraie-ac-0.0.6/src/py_miraie_ac/constants.py
--rw-rw-rw-   0        0        0     4542 2023-06-09 13:28:51.000000 py-miraie-ac-0.0.6/src/py_miraie_ac/device.py
--rw-rw-rw-   0        0        0      857 2023-06-09 13:29:04.000000 py-miraie-ac-0.0.6/src/py_miraie_ac/deviceStatus.py
--rw-rw-rw-   0        0        0      917 2023-06-05 03:55:22.000000 py-miraie-ac-0.0.6/src/py_miraie_ac/enums.py
--rw-rw-rw-   0        0        0      121 2023-06-05 03:55:32.000000 py-miraie-ac-0.0.6/src/py_miraie_ac/exceptions.py
--rw-rw-rw-   0        0        0      483 2023-06-09 13:29:18.000000 py-miraie-ac-0.0.6/src/py_miraie_ac/home.py
--rw-rw-rw-   0        0        0      460 2023-06-05 03:57:35.000000 py-miraie-ac-0.0.6/src/py_miraie_ac/user.py
--rw-rw-rw-   0        0        0      236 2023-06-09 13:29:27.000000 py-miraie-ac-0.0.6/src/py_miraie_ac/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-09 13:29:51.643589 py-miraie-ac-0.0.6/src/py_miraie_ac.egg-info/
--rw-rw-rw-   0        0        0     1232 2023-06-09 13:29:51.000000 py-miraie-ac-0.0.6/src/py_miraie_ac.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      505 2023-06-09 13:29:51.000000 py-miraie-ac-0.0.6/src/py_miraie_ac.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 13:29:51.000000 py-miraie-ac-0.0.6/src/py_miraie_ac.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-06-09 13:29:51.000000 py-miraie-ac-0.0.6/src/py_miraie_ac.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 16:12:51.501058 py-miraie-ac-0.0.8/
+-rw-rw-rw-   0        0        0    35821 2023-06-09 07:50:41.000000 py-miraie-ac-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     1232 2023-06-09 16:12:51.512073 py-miraie-ac-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      625 2023-06-09 08:48:49.000000 py-miraie-ac-0.0.8/README.md
+-rw-rw-rw-   0        0        0      104 2023-06-09 16:09:32.000000 py-miraie-ac-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0      801 2023-06-09 16:12:51.512073 py-miraie-ac-0.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-09 16:12:51.394343 py-miraie-ac-0.0.8/src/
+drwxrwxrwx   0        0        0        0 2023-06-09 16:12:51.411850 py-miraie-ac-0.0.8/src/py_miraie_ac/
+-rw-rw-rw-   0        0        0      403 2023-06-09 13:16:33.000000 py-miraie-ac-0.0.8/src/py_miraie_ac/__init__.py
+-rw-rw-rw-   0        0        0     6172 2023-06-09 13:28:16.000000 py-miraie-ac-0.0.8/src/py_miraie_ac/api.py
+-rw-rw-rw-   0        0        0     6221 2023-06-09 13:28:36.000000 py-miraie-ac-0.0.8/src/py_miraie_ac/broker.py
+-rw-rw-rw-   0        0        0      421 2023-06-05 03:33:43.000000 py-miraie-ac-0.0.8/src/py_miraie_ac/constants.py
+-rw-rw-rw-   0        0        0     4542 2023-06-09 13:28:51.000000 py-miraie-ac-0.0.8/src/py_miraie_ac/device.py
+-rw-rw-rw-   0        0        0      857 2023-06-09 13:29:04.000000 py-miraie-ac-0.0.8/src/py_miraie_ac/deviceStatus.py
+-rw-rw-rw-   0        0        0      917 2023-06-05 03:55:22.000000 py-miraie-ac-0.0.8/src/py_miraie_ac/enums.py
+-rw-rw-rw-   0        0        0      121 2023-06-05 03:55:32.000000 py-miraie-ac-0.0.8/src/py_miraie_ac/exceptions.py
+-rw-rw-rw-   0        0        0      483 2023-06-09 13:29:18.000000 py-miraie-ac-0.0.8/src/py_miraie_ac/home.py
+-rw-rw-rw-   0        0        0      460 2023-06-05 03:57:35.000000 py-miraie-ac-0.0.8/src/py_miraie_ac/user.py
+-rw-rw-rw-   0        0        0      236 2023-06-09 13:29:27.000000 py-miraie-ac-0.0.8/src/py_miraie_ac/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-09 16:12:51.501058 py-miraie-ac-0.0.8/src/py_miraie_ac.egg-info/
+-rw-rw-rw-   0        0        0     1232 2023-06-09 16:12:51.000000 py-miraie-ac-0.0.8/src/py_miraie_ac.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      544 2023-06-09 16:12:51.000000 py-miraie-ac-0.0.8/src/py_miraie_ac.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 16:12:51.000000 py-miraie-ac-0.0.8/src/py_miraie_ac.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-06-09 16:12:51.000000 py-miraie-ac-0.0.8/src/py_miraie_ac.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-09 16:12:51.000000 py-miraie-ac-0.0.8/src/py_miraie_ac.egg-info/top_level.txt
```

### Comparing `py-miraie-ac-0.0.6/LICENSE` & `py-miraie-ac-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `py-miraie-ac-0.0.6/PKG-INFO` & `py-miraie-ac-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-miraie-ac
-Version: 0.0.6
+Version: 0.0.8
 Summary: A package to control and read MirAIe Aircons by Panasonic
 Home-page: https://github.com/milothomas/py-miraie-ac
 Author: Milo Thomas
 Author-email: 20719501+milothomas@users.noreply.github.com
 Project-URL: Bug Tracker, https://github.com/milothomas/py-miraie-ac/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `py-miraie-ac-0.0.6/README.md` & `py-miraie-ac-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `py-miraie-ac-0.0.6/setup.cfg` & `py-miraie-ac-0.0.8/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 792d 6d69 7261 6965 2d61 630d   = py-miraie-ac.
-00000020: 0a76 6572 7369 6f6e 203d 2030 2e30 2e36  .version = 0.0.6
+00000020: 0a76 6572 7369 6f6e 203d 2030 2e30 2e38  .version = 0.0.8
 00000030: 0d0a 6175 7468 6f72 203d 204d 696c 6f20  ..author = Milo 
 00000040: 5468 6f6d 6173 0d0a 6175 7468 6f72 5f65  Thomas..author_e
 00000050: 6d61 696c 203d 2032 3037 3139 3530 312b  mail = 20719501+
 00000060: 6d69 6c6f 7468 6f6d 6173 4075 7365 7273  milothomas@users
 00000070: 2e6e 6f72 6570 6c79 2e67 6974 6875 622e  .noreply.github.
 00000080: 636f 6d0d 0a64 6573 6372 6970 7469 6f6e  com..description
 00000090: 203d 2041 2070 6163 6b61 6765 2074 6f20   = A package to 
@@ -35,13 +35,17 @@
 00000220: 4f70 6572 6174 696e 6720 5379 7374 656d  Operating System
 00000230: 203a 3a20 4f53 2049 6e64 6570 656e 6465   :: OS Independe
 00000240: 6e74 0d0a 0d0a 5b6f 7074 696f 6e73 5d0d  nt....[options].
 00000250: 0a70 6163 6b61 6765 5f64 6972 203d 200d  .package_dir = .
 00000260: 0a09 3d20 7372 630d 0a70 6163 6b61 6765  ..= src..package
 00000270: 7320 3d20 6669 6e64 3a0d 0a70 7974 686f  s = find:..pytho
 00000280: 6e5f 7265 7175 6972 6573 203d 203e 3d33  n_requires = >=3
-00000290: 2e36 0d0a 0d0a 5b6f 7074 696f 6e73 2e70  .6....[options.p
-000002a0: 6163 6b61 6765 732e 6669 6e64 5d0d 0a77  ackages.find]..w
-000002b0: 6865 7265 203d 2073 7263 0d0a 0d0a 5b65  here = src....[e
-000002c0: 6767 5f69 6e66 6f5d 0d0a 7461 675f 6275  gg_info]..tag_bu
-000002d0: 696c 6420 3d20 0d0a 7461 675f 6461 7465  ild = ..tag_date
-000002e0: 203d 2030 0d0a 0d0a                       = 0....
+00000290: 2e36 0d0a 696e 7374 616c 6c5f 7265 7175  .6..install_requ
+000002a0: 6972 6573 203d 200d 0a09 6169 6f68 7474  ires = ...aiohtt
+000002b0: 703d 3d33 2e38 2e34 0d0a 0970 6168 6f5f  p==3.8.4...paho_
+000002c0: 6d71 7474 3d3d 312e 362e 310d 0a0d 0a5b  mqtt==1.6.1....[
+000002d0: 6f70 7469 6f6e 732e 7061 636b 6167 6573  options.packages
+000002e0: 2e66 696e 645d 0d0a 7768 6572 6520 3d20  .find]..where = 
+000002f0: 7372 630d 0a0d 0a5b 6567 675f 696e 666f  src....[egg_info
+00000300: 5d0d 0a74 6167 5f62 7569 6c64 203d 200d  ]..tag_build = .
+00000310: 0a74 6167 5f64 6174 6520 3d20 300d 0a0d  .tag_date = 0...
+00000320: 0a                                       .
```

### Comparing `py-miraie-ac-0.0.6/src/py_miraie_ac/api.py` & `py-miraie-ac-0.0.8/src/py_miraie_ac/api.py`

 * *Files identical despite different names*

### Comparing `py-miraie-ac-0.0.6/src/py_miraie_ac/broker.py` & `py-miraie-ac-0.0.8/src/py_miraie_ac/broker.py`

 * *Files identical despite different names*

### Comparing `py-miraie-ac-0.0.6/src/py_miraie_ac/device.py` & `py-miraie-ac-0.0.8/src/py_miraie_ac/device.py`

 * *Files identical despite different names*

### Comparing `py-miraie-ac-0.0.6/src/py_miraie_ac/deviceStatus.py` & `py-miraie-ac-0.0.8/src/py_miraie_ac/deviceStatus.py`

 * *Files identical despite different names*

### Comparing `py-miraie-ac-0.0.6/src/py_miraie_ac/enums.py` & `py-miraie-ac-0.0.8/src/py_miraie_ac/enums.py`

 * *Files identical despite different names*

### Comparing `py-miraie-ac-0.0.6/src/py_miraie_ac.egg-info/PKG-INFO` & `py-miraie-ac-0.0.8/src/py_miraie_ac.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-miraie-ac
-Version: 0.0.6
+Version: 0.0.8
 Summary: A package to control and read MirAIe Aircons by Panasonic
 Home-page: https://github.com/milothomas/py-miraie-ac
 Author: Milo Thomas
 Author-email: 20719501+milothomas@users.noreply.github.com
 Project-URL: Bug Tracker, https://github.com/milothomas/py-miraie-ac/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

