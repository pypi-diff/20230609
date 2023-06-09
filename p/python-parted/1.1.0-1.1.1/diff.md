# Comparing `tmp/python_parted-1.1.0.tar.gz` & `tmp/python_parted-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_parted-1.1.0.tar", max compression
+gzip compressed data, was "python_parted-1.1.1.tar", max compression
```

## Comparing `python_parted-1.1.0.tar` & `python_parted-1.1.1.tar`

### file list

```diff
@@ -1,46 +1,47 @@
--rw-r--r--   0        0        0     1070 2023-05-02 15:06:52.033475 python_parted-1.1.0/LICENSE
--rw-r--r--   0        0        0      333 2023-06-06 22:30:13.288871 python_parted-1.1.0/README.md
--rw-r--r--   0        0        0    27877 2022-09-28 20:00:39.477913 python_parted-1.1.0/build.py
--rw-r--r--   0        0        0      672 2022-09-27 20:14:12.975319 python_parted-1.1.0/docs/Makefile
--rw-r--r--   0        0        0      804 2022-09-17 09:42:27.371559 python_parted-1.1.0/docs/make.bat
--rw-r--r--   0        0        0     1283 2022-09-27 20:19:01.809332 python_parted-1.1.0/docs/source/conf.py
--rw-r--r--   0        0        0      494 2022-09-17 21:22:29.390240 python_parted-1.1.0/docs/source/index.rst
--rw-r--r--   0        0        0      136 2022-09-17 18:05:18.932654 python_parted-1.1.0/docs/source/parted.alignment.rst
--rw-r--r--   0        0        0      139 2022-09-17 18:05:18.932654 python_parted-1.1.0/docs/source/parted.constraint.rst
--rw-r--r--   0        0        0      127 2022-09-17 18:05:18.932654 python_parted-1.1.0/docs/source/parted.device.rst
--rw-r--r--   0        0        0      121 2022-09-17 18:05:18.936654 python_parted-1.1.0/docs/source/parted.disk.rst
--rw-r--r--   0        0        0      139 2022-09-17 18:05:18.936654 python_parted-1.1.0/docs/source/parted.exceptions.rst
--rw-r--r--   0        0        0      124 2022-09-17 18:05:18.936654 python_parted-1.1.0/docs/source/parted.excpt.rst
--rw-r--r--   0        0        0      130 2022-09-17 18:05:18.940654 python_parted-1.1.0/docs/source/parted.filesys.rst
--rw-r--r--   0        0        0      121 2022-09-17 18:05:18.940654 python_parted-1.1.0/docs/source/parted.geom.rst
--rw-r--r--   0        0        0      336 2022-09-17 18:08:46.109657 python_parted-1.1.0/docs/source/parted.rst
--rw-r--r--   0        0        0      124 2022-09-17 18:05:18.940654 python_parted-1.1.0/docs/source/parted.timer.rst
--rw-r--r--   0        0        0      121 2022-09-17 18:05:18.944654 python_parted-1.1.0/docs/source/parted.util.rst
--rw-r--r--   0        0        0      155 2022-09-17 14:21:41.265355 python_parted-1.1.0/docs/source/usage.rst
--rw-r--r--   0        0        0     2668 2022-09-19 18:47:44.567750 python_parted-1.1.0/parted/__init__.py
--rw-r--r--   0        0        0    10023 2023-05-02 15:27:59.676306 python_parted-1.1.0/parted/alignment.py
--rw-r--r--   0        0        0    15841 2023-05-02 15:28:06.724366 python_parted-1.1.0/parted/constraint.py
--rw-r--r--   0        0        0    24591 2023-05-02 15:28:13.632425 python_parted-1.1.0/parted/device.py
--rw-r--r--   0        0        0    40881 2023-05-02 15:28:38.236635 python_parted-1.1.0/parted/disk.py
--rw-r--r--   0        0        0     2872 2023-05-02 15:28:45.476697 python_parted-1.1.0/parted/exceptions.py
--rw-r--r--   0        0        0     8853 2023-05-02 15:28:53.440765 python_parted-1.1.0/parted/excpt.py
--rw-r--r--   0        0        0     9082 2023-05-02 15:29:02.672844 python_parted-1.1.0/parted/filesys.py
--rw-r--r--   0        0        0    16132 2023-05-02 15:29:11.076916 python_parted-1.1.0/parted/geom.py
--rw-r--r--   0        0        0     7711 2023-05-02 15:29:21.297003 python_parted-1.1.0/parted/timer.py
--rw-r--r--   0        0        0     6615 2023-05-02 15:30:52.969789 python_parted-1.1.0/parted/util.py
--rw-r--r--   0        0        0     2204 2023-06-06 23:35:58.613661 python_parted-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     1680 2022-09-03 20:03:48.168386 python_parted-1.1.0/tests/__init__.py
--rw-r--r--   0        0        0    14445 2023-05-02 15:29:32.209097 python_parted-1.1.0/tests/test_alignment.py
--rw-r--r--   0        0        0    13330 2023-05-02 15:29:39.353158 python_parted-1.1.0/tests/test_constraint.py
--rw-r--r--   0        0        0    15065 2023-05-02 15:29:45.925214 python_parted-1.1.0/tests/test_device.py
--rw-r--r--   0        0        0    14004 2023-05-02 15:29:54.417287 python_parted-1.1.0/tests/test_disk.py
--rw-r--r--   0        0        0     1516 2023-05-02 15:30:00.637340 python_parted-1.1.0/tests/test_exception.py
--rw-r--r--   0        0        0     4016 2023-05-02 15:30:07.001395 python_parted-1.1.0/tests/test_filesys.py
--rw-r--r--   0        0        0     7659 2023-05-02 15:30:12.657443 python_parted-1.1.0/tests/test_geometry.py
--rw-r--r--   0        0        0    13914 2023-05-02 15:30:18.573494 python_parted-1.1.0/tests/test_partition.py
--rw-r--r--   0        0        0     1503 2023-05-02 15:30:24.701546 python_parted-1.1.0/tests/test_timer.py
--rw-r--r--   0        0        0     7327 2022-09-11 22:05:37.643649 python_parted-1.1.0/tests/util/__init__.py
--rw-r--r--   0        0        0    17842 2022-09-05 14:21:05.125147 python_parted-1.1.0/tests/util/gptdsk.py
--rw-r--r--   0        0        0    18087 2022-09-05 14:21:05.125147 python_parted-1.1.0/tests/util/msdosdsk.py
--rw-r--r--   0        0        0     2911 2023-05-02 15:30:50.137765 python_parted-1.1.0/tests/util/partedtest.py
--rw-r--r--   0        0        0     1234 1970-01-01 00:00:00.000000 python_parted-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-02 15:06:52.033475 python_parted-1.1.1/LICENSE
+-rw-r--r--   0        0        0      333 2023-06-06 22:30:13.288871 python_parted-1.1.1/README.md
+-rw-r--r--   0        0        0    27877 2022-09-28 20:00:39.477913 python_parted-1.1.1/build.py
+-rw-r--r--   0        0        0      672 2022-09-27 20:14:12.975319 python_parted-1.1.1/docs/Makefile
+-rw-r--r--   0        0        0      804 2022-09-17 09:42:27.371559 python_parted-1.1.1/docs/make.bat
+-rw-r--r--   0        0        0     1283 2022-09-27 20:19:01.809332 python_parted-1.1.1/docs/source/conf.py
+-rw-r--r--   0        0        0      494 2022-09-17 21:22:29.390240 python_parted-1.1.1/docs/source/index.rst
+-rw-r--r--   0        0        0      136 2022-09-17 18:05:18.932654 python_parted-1.1.1/docs/source/parted.alignment.rst
+-rw-r--r--   0        0        0      139 2022-09-17 18:05:18.932654 python_parted-1.1.1/docs/source/parted.constraint.rst
+-rw-r--r--   0        0        0      127 2022-09-17 18:05:18.932654 python_parted-1.1.1/docs/source/parted.device.rst
+-rw-r--r--   0        0        0      121 2022-09-17 18:05:18.936654 python_parted-1.1.1/docs/source/parted.disk.rst
+-rw-r--r--   0        0        0      139 2022-09-17 18:05:18.936654 python_parted-1.1.1/docs/source/parted.exceptions.rst
+-rw-r--r--   0        0        0      124 2022-09-17 18:05:18.936654 python_parted-1.1.1/docs/source/parted.excpt.rst
+-rw-r--r--   0        0        0      130 2022-09-17 18:05:18.940654 python_parted-1.1.1/docs/source/parted.filesys.rst
+-rw-r--r--   0        0        0      121 2022-09-17 18:05:18.940654 python_parted-1.1.1/docs/source/parted.geom.rst
+-rw-r--r--   0        0        0      336 2022-09-17 18:08:46.109657 python_parted-1.1.1/docs/source/parted.rst
+-rw-r--r--   0        0        0      124 2022-09-17 18:05:18.940654 python_parted-1.1.1/docs/source/parted.timer.rst
+-rw-r--r--   0        0        0      121 2022-09-17 18:05:18.944654 python_parted-1.1.1/docs/source/parted.util.rst
+-rw-r--r--   0        0        0      155 2022-09-17 14:21:41.265355 python_parted-1.1.1/docs/source/usage.rst
+-rw-r--r--   0        0        0     2668 2022-09-19 18:47:44.567750 python_parted-1.1.1/parted/__init__.py
+-rw-r--r--   0        0        0    10023 2023-05-02 15:27:59.676306 python_parted-1.1.1/parted/alignment.py
+-rw-r--r--   0        0        0    15841 2023-05-02 15:28:06.724366 python_parted-1.1.1/parted/constraint.py
+-rw-r--r--   0        0        0    24591 2023-05-02 15:28:13.632425 python_parted-1.1.1/parted/device.py
+-rw-r--r--   0        0        0    40881 2023-05-02 15:28:38.236635 python_parted-1.1.1/parted/disk.py
+-rw-r--r--   0        0        0     2872 2023-05-02 15:28:45.476697 python_parted-1.1.1/parted/exceptions.py
+-rw-r--r--   0        0        0     8853 2023-05-02 15:28:53.440765 python_parted-1.1.1/parted/excpt.py
+-rw-r--r--   0        0        0     9082 2023-05-02 15:29:02.672844 python_parted-1.1.1/parted/filesys.py
+-rw-r--r--   0        0        0    16132 2023-05-02 15:29:11.076916 python_parted-1.1.1/parted/geom.py
+-rw-r--r--   0        0        0        1 2023-06-09 13:42:53.449030 python_parted-1.1.1/parted/py.typed
+-rw-r--r--   0        0        0     7711 2023-05-02 15:29:21.297003 python_parted-1.1.1/parted/timer.py
+-rw-r--r--   0        0        0     6615 2023-05-02 15:30:52.969789 python_parted-1.1.1/parted/util.py
+-rw-r--r--   0        0        0     2238 2023-06-09 13:42:53.449030 python_parted-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1680 2022-09-03 20:03:48.168386 python_parted-1.1.1/tests/__init__.py
+-rw-r--r--   0        0        0    14445 2023-05-02 15:29:32.209097 python_parted-1.1.1/tests/test_alignment.py
+-rw-r--r--   0        0        0    13330 2023-05-02 15:29:39.353158 python_parted-1.1.1/tests/test_constraint.py
+-rw-r--r--   0        0        0    15065 2023-05-02 15:29:45.925214 python_parted-1.1.1/tests/test_device.py
+-rw-r--r--   0        0        0    14004 2023-05-02 15:29:54.417287 python_parted-1.1.1/tests/test_disk.py
+-rw-r--r--   0        0        0     1516 2023-05-02 15:30:00.637340 python_parted-1.1.1/tests/test_exception.py
+-rw-r--r--   0        0        0     4016 2023-05-02 15:30:07.001395 python_parted-1.1.1/tests/test_filesys.py
+-rw-r--r--   0        0        0     7659 2023-05-02 15:30:12.657443 python_parted-1.1.1/tests/test_geometry.py
+-rw-r--r--   0        0        0    13914 2023-05-02 15:30:18.573494 python_parted-1.1.1/tests/test_partition.py
+-rw-r--r--   0        0        0     1503 2023-05-02 15:30:24.701546 python_parted-1.1.1/tests/test_timer.py
+-rw-r--r--   0        0        0     7327 2022-09-11 22:05:37.643649 python_parted-1.1.1/tests/util/__init__.py
+-rw-r--r--   0        0        0    17842 2022-09-05 14:21:05.125147 python_parted-1.1.1/tests/util/gptdsk.py
+-rw-r--r--   0        0        0    18087 2022-09-05 14:21:05.125147 python_parted-1.1.1/tests/util/msdosdsk.py
+-rw-r--r--   0        0        0     2911 2023-05-02 15:30:50.137765 python_parted-1.1.1/tests/util/partedtest.py
+-rw-r--r--   0        0        0     1234 1970-01-01 00:00:00.000000 python_parted-1.1.1/PKG-INFO
```

### Comparing `python_parted-1.1.0/LICENSE` & `python_parted-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python_parted-1.1.0/build.py` & `python_parted-1.1.1/build.py`

 * *Files identical despite different names*

### Comparing `python_parted-1.1.0/docs/Makefile` & `python_parted-1.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `python_parted-1.1.0/docs/make.bat` & `python_parted-1.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `python_parted-1.1.0/docs/source/conf.py` & `python_parted-1.1.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `python_parted-1.1.0/parted/__init__.py` & `python_parted-1.1.1/parted/__init__.py`

 * *Files identical despite different names*

### Comparing `python_parted-1.1.0/parted/alignment.py` & `python_parted-1.1.1/parted/alignment.py`

 * *Files identical despite different names*

### Comparing `python_parted-1.1.0/parted/constraint.py` & `python_parted-1.1.1/parted/constraint.py`

 * *Files identical despite different names*

### Comparing `python_parted-1.1.0/parted/device.py` & `python_parted-1.1.1/parted/device.py`

 * *Files identical despite different names*

### Comparing `python_parted-1.1.0/parted/disk.py` & `python_parted-1.1.1/parted/disk.py`

 * *Files identical despite different names*

### Comparing `python_parted-1.1.0/parted/exceptions.py` & `python_parted-1.1.1/parted/exceptions.py`

 * *Files identical despite different names*

### Comparing `python_parted-1.1.0/parted/excpt.py` & `python_parted-1.1.1/parted/excpt.py`

 * *Files identical despite different names*

### Comparing `python_parted-1.1.0/parted/filesys.py` & `python_parted-1.1.1/parted/filesys.py`

 * *Files identical despite different names*

### Comparing `python_parted-1.1.0/parted/geom.py` & `python_parted-1.1.1/parted/geom.py`

 * *Files identical despite different names*

### Comparing `python_parted-1.1.0/parted/timer.py` & `python_parted-1.1.1/parted/timer.py`

 * *Files identical despite different names*

### Comparing `python_parted-1.1.0/parted/util.py` & `python_parted-1.1.1/parted/util.py`

 * *Files identical despite different names*

### Comparing `python_parted-1.1.0/pyproject.toml` & `python_parted-1.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 [tool.poetry]
 name = "python-parted"
-version = "1.1.0"
+version = "1.1.1"
 license = "MIT"
 readme = "README.md"
 description = "Python interface to access the parted library"
 authors = ["Adolfo Gómez García <dkmaster@dkmon.com>"]
 packages = [
     {include = "parted"},
+    {include = "parted/py.typed"}
 ]
 include = [
     {path = "build.py", format="sdist" },
     {path = 'README.md', format="sdist"},
     {path = 'LICENSE', format="sdist"},
     {path = 'tests', format="sdist"},
     {path = 'docs/source', format="sdist"},
```

### Comparing `python_parted-1.1.0/tests/__init__.py` & `python_parted-1.1.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `python_parted-1.1.0/tests/test_alignment.py` & `python_parted-1.1.1/tests/test_alignment.py`

 * *Files identical despite different names*

### Comparing `python_parted-1.1.0/tests/test_constraint.py` & `python_parted-1.1.1/tests/test_constraint.py`

 * *Files identical despite different names*

### Comparing `python_parted-1.1.0/tests/test_device.py` & `python_parted-1.1.1/tests/test_device.py`

 * *Files identical despite different names*

### Comparing `python_parted-1.1.0/tests/test_disk.py` & `python_parted-1.1.1/tests/test_disk.py`

 * *Files identical despite different names*

### Comparing `python_parted-1.1.0/tests/test_exception.py` & `python_parted-1.1.1/tests/test_exception.py`

 * *Files identical despite different names*

### Comparing `python_parted-1.1.0/tests/test_filesys.py` & `python_parted-1.1.1/tests/test_filesys.py`

 * *Files identical despite different names*

### Comparing `python_parted-1.1.0/tests/test_geometry.py` & `python_parted-1.1.1/tests/test_geometry.py`

 * *Files identical despite different names*

### Comparing `python_parted-1.1.0/tests/test_partition.py` & `python_parted-1.1.1/tests/test_partition.py`

 * *Files identical despite different names*

### Comparing `python_parted-1.1.0/tests/test_timer.py` & `python_parted-1.1.1/tests/test_timer.py`

 * *Files identical despite different names*

### Comparing `python_parted-1.1.0/tests/util/__init__.py` & `python_parted-1.1.1/tests/util/__init__.py`

 * *Files identical despite different names*

### Comparing `python_parted-1.1.0/tests/util/gptdsk.py` & `python_parted-1.1.1/tests/util/gptdsk.py`

 * *Files identical despite different names*

### Comparing `python_parted-1.1.0/tests/util/msdosdsk.py` & `python_parted-1.1.1/tests/util/msdosdsk.py`

 * *Files identical despite different names*

### Comparing `python_parted-1.1.0/tests/util/partedtest.py` & `python_parted-1.1.1/tests/util/partedtest.py`

 * *Files identical despite different names*

### Comparing `python_parted-1.1.0/PKG-INFO` & `python_parted-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-parted
-Version: 1.1.0
+Version: 1.1.1
 Summary: Python interface to access the parted library
 Home-page: https://github.com/dkmstr/python-parted
 License: MIT
 Author: Adolfo Gómez García
 Author-email: dkmaster@dkmon.com
 Requires-Python: >=3.8.0
 Classifier: Development Status :: 4 - Beta
```

