# Comparing `tmp/serena-0.7.3.tar.gz` & `tmp/serena-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serena-0.7.3.tar", max compression
+gzip compressed data, was "serena-0.7.4.tar", max compression
```

## Comparing `serena-0.7.3.tar` & `serena-0.7.4.tar`

### file list

```diff
@@ -1,29 +1,35 @@
--rw-r--r--   0        0        0      138 2022-01-14 22:49:55.261592 serena-0.7.3/README.rst
--rw-r--r--   0        0        0     1714 2022-04-21 11:20:15.443765 serena-0.7.3/pyproject.toml
--rw-r--r--   0        0        0      633 2022-02-03 13:05:05.077281 serena-0.7.3/src/serena/__init__.py
--rw-r--r--   0        0        0    29250 2022-01-29 13:07:16.839481 serena-0.7.3/src/serena/channel.py
--rw-r--r--   0        0        0     9260 2022-01-22 02:04:05.144887 serena-0.7.3/src/serena/channel.py.orig
--rw-r--r--   0        0        0    29763 2022-01-29 12:45:46.552248 serena-0.7.3/src/serena/connection.py
--rw-r--r--   0        0        0     3747 2022-01-22 03:35:21.384552 serena-0.7.3/src/serena/enums.py
--rw-r--r--   0        0        0     3332 2022-01-14 23:26:48.593351 serena-0.7.3/src/serena/exc.py
--rw-r--r--   0        0        0      821 2022-01-13 01:12:24.144611 serena-0.7.3/src/serena/frame.py
--rw-r--r--   0        0        0     8028 2022-01-13 19:21:48.926033 serena-0.7.3/src/serena/frameparser.py
--rw-r--r--   0        0        0     3837 2022-01-13 22:45:55.155021 serena-0.7.3/src/serena/message.py
--rw-r--r--   0        0        0    15242 2022-04-21 11:13:32.414275 serena-0.7.3/src/serena/mixin.py
--rw-r--r--   0        0        0        0 2022-01-07 14:51:24.328484 serena-0.7.3/src/serena/payloads/__init__.py
--rw-r--r--   0        0        0      159 2022-01-10 00:39:28.045110 serena-0.7.3/src/serena/payloads/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2027 2022-01-13 22:11:18.560150 serena-0.7.3/src/serena/payloads/__pycache__/encoding.cpython-310.pyc
--rw-r--r--   0        0        0     3732 2022-01-22 23:33:14.685596 serena-0.7.3/src/serena/payloads/__pycache__/header.cpython-310.pyc
--rw-r--r--   0        0        0    20480 2022-01-22 23:33:14.645596 serena-0.7.3/src/serena/payloads/__pycache__/method.cpython-310.pyc
--rw-r--r--   0        0        0     2290 2022-01-13 22:11:13.740192 serena-0.7.3/src/serena/payloads/encoding.py
--rw-r--r--   0        0        0     4697 2022-02-03 13:05:05.113948 serena-0.7.3/src/serena/payloads/header.py
--rw-r--r--   0        0        0    28492 2022-01-22 23:31:38.223113 serena-0.7.3/src/serena/payloads/method.py
--rw-r--r--   0        0        0    16031 2022-04-21 11:19:37.554121 serena-0.7.3/src/serena/pool.py
--rw-r--r--   0        0        0        0 2021-12-30 01:14:06.764939 serena-0.7.3/src/serena/utils/__init__.py
--rw-r--r--   0        0        0      156 2022-01-10 00:39:28.081776 serena-0.7.3/src/serena/utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1699 2022-01-13 17:01:29.670197 serena-0.7.3/src/serena/utils/__pycache__/bitset.cpython-310.pyc
--rw-r--r--   0        0        0    13664 2022-01-13 17:00:36.967243 serena-0.7.3/src/serena/utils/__pycache__/buffer.cpython-310.pyc
--rw-r--r--   0        0        0     1038 2022-01-13 17:00:59.537081 serena-0.7.3/src/serena/utils/bitset.py
--rw-r--r--   0        0        0    12912 2022-01-13 17:00:34.043931 serena-0.7.3/src/serena/utils/buffer.py
--rw-r--r--   0        0        0     1213 2022-04-21 11:21:10.914826 serena-0.7.3/setup.py
--rw-r--r--   0        0        0     1288 2022-04-21 11:21:10.915080 serena-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0      138 2022-01-14 22:49:55.261592 serena-0.7.4/README.rst
+-rw-r--r--   0        0        0     1553 2023-06-09 20:08:48.322701 serena-0.7.4/pyproject.toml
+-rw-r--r--   0        0        0      633 2022-02-03 13:05:05.077281 serena-0.7.4/src/serena/__init__.py
+-rw-r--r--   0        0        0    29250 2022-01-29 13:07:16.839481 serena-0.7.4/src/serena/channel.py
+-rw-r--r--   0        0        0     9260 2022-01-22 02:04:05.144887 serena-0.7.4/src/serena/channel.py.orig
+-rw-r--r--   0        0        0    29763 2022-01-29 12:45:46.552248 serena-0.7.4/src/serena/connection.py
+-rw-r--r--   0        0        0     3747 2022-01-22 03:35:21.384552 serena-0.7.4/src/serena/enums.py
+-rw-r--r--   0        0        0     3332 2022-01-14 23:26:48.593351 serena-0.7.4/src/serena/exc.py
+-rw-r--r--   0        0        0      821 2022-01-13 01:12:24.144611 serena-0.7.4/src/serena/frame.py
+-rw-r--r--   0        0        0     8028 2022-01-13 19:21:48.926033 serena-0.7.4/src/serena/frameparser.py
+-rw-r--r--   0        0        0     3837 2022-01-13 22:45:55.155021 serena-0.7.4/src/serena/message.py
+-rw-r--r--   0        0        0    15242 2022-04-21 11:13:32.414275 serena-0.7.4/src/serena/mixin.py
+-rw-r--r--   0        0        0        0 2022-01-07 14:51:24.328484 serena-0.7.4/src/serena/payloads/__init__.py
+-rw-r--r--   0        0        0      159 2022-01-10 00:39:28.045110 serena-0.7.4/src/serena/payloads/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      175 2023-06-09 20:05:44.516873 serena-0.7.4/src/serena/payloads/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2027 2022-01-13 22:11:18.560150 serena-0.7.4/src/serena/payloads/__pycache__/encoding.cpython-310.pyc
+-rw-r--r--   0        0        0     3190 2023-06-09 20:05:44.543540 serena-0.7.4/src/serena/payloads/__pycache__/encoding.cpython-311.pyc
+-rw-r--r--   0        0        0     3732 2022-04-21 11:22:21.992583 serena-0.7.4/src/serena/payloads/__pycache__/header.cpython-310.pyc
+-rw-r--r--   0        0        0     6698 2023-06-09 20:05:44.586873 serena-0.7.4/src/serena/payloads/__pycache__/header.cpython-311.pyc
+-rw-r--r--   0        0        0    20480 2022-01-22 23:33:14.645596 serena-0.7.4/src/serena/payloads/__pycache__/method.cpython-310.pyc
+-rw-r--r--   0        0        0    40471 2023-06-09 20:05:44.523540 serena-0.7.4/src/serena/payloads/__pycache__/method.cpython-311.pyc
+-rw-r--r--   0        0        0     2290 2022-01-13 22:11:13.740192 serena-0.7.4/src/serena/payloads/encoding.py
+-rw-r--r--   0        0        0     4697 2022-02-03 13:05:05.113948 serena-0.7.4/src/serena/payloads/header.py
+-rw-r--r--   0        0        0    28492 2022-01-22 23:31:38.223113 serena-0.7.4/src/serena/payloads/method.py
+-rw-r--r--   0        0        0    16031 2022-04-21 11:19:37.554121 serena-0.7.4/src/serena/pool.py
+-rw-r--r--   0        0        0        0 2021-12-30 01:14:06.764939 serena-0.7.4/src/serena/utils/__init__.py
+-rw-r--r--   0        0        0      156 2022-01-10 00:39:28.081776 serena-0.7.4/src/serena/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      172 2023-06-09 20:05:44.543540 serena-0.7.4/src/serena/utils/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1699 2022-01-13 17:01:29.670197 serena-0.7.4/src/serena/utils/__pycache__/bitset.cpython-310.pyc
+-rw-r--r--   0        0        0     2609 2023-06-09 20:05:44.603540 serena-0.7.4/src/serena/utils/__pycache__/bitset.cpython-311.pyc
+-rw-r--r--   0        0        0    13664 2022-01-13 17:00:36.967243 serena-0.7.4/src/serena/utils/__pycache__/buffer.cpython-310.pyc
+-rw-r--r--   0        0        0    23020 2023-06-09 20:05:44.543540 serena-0.7.4/src/serena/utils/__pycache__/buffer.cpython-311.pyc
+-rw-r--r--   0        0        0     1038 2022-01-13 17:00:59.537081 serena-0.7.4/src/serena/utils/bitset.py
+-rw-r--r--   0        0        0    12912 2022-01-13 17:00:34.043931 serena-0.7.4/src/serena/utils/buffer.py
+-rw-r--r--   0        0        0      896 1970-01-01 00:00:00.000000 serena-0.7.4/PKG-INFO
```

### Comparing `serena-0.7.3/pyproject.toml` & `serena-0.7.4/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 [tool.poetry]
 name = "serena"
-version = "0.7.3"
+version = "0.7.4"
 description = "An AMQP 0-9-1 client using AnyIO."
 authors = ["Lura Skye <l@veriny.tf>"]
 license = "LGPL-3.0-or-later"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Operating System :: OS Independent",
     "Framework :: AnyIO",
 ]
 readme = "README.rst"
 
 [tool.poetry.dependencies]
-python = ">=3.8,<4.0"
-anyio = "^3.5.0"
-attrs = "^21.4.0"
-"backports.strenum" = { version = "^1.1.1;", python = "<3.11" }
-
-Sphinx = { version = "^4.3.2", optional = true }
-sphinx-rtd-theme = { version = "^1.0.0", optional = true }
-sphinx-inline-tabs = { version = "^2022.1.2-beta.11", optional = true }
-sphinxcontrib-trio = { version = "^1.1.2", optional = true }
-sphinx-autodoc-typehints = { version = "^1.15.2", optional = true }
-
-[tool.poetry.dev-dependencies]
-pytest = "^6.2.5"
-black = "^21.12b0"
-isort = "^5.10.1"
-trio = "^0.19.0"
-prettyprinter = "^0.18.0"
-pytest-cov = "^3.0.0"
+python = ">=3.10,<4.0"
+anyio = ">=3.6.2"
+attrs = ">=21.4.0"
+"backports.strenum" = { version = "^1.1.1",  python = "<3.11" }
+
+[tool.poetry.group.docs.dependencies]
+sphinx = "^6.1"
+sphinx-rtd-theme = "^1.2.2"
+sphinxcontrib-trio = "^1.1.2"
+sphinx-inline-tabs = "^2023.4.21"
+sphinx-autodoc-typehints = "^1.23.0"
+
+
+[tool.poetry.group.dev.dependencies]
+pytest = "^7.3.1"
+trio = "^0.22.0"
+isort = "^5.12.0"
+pytest-cov = "^4.1.0"
 
 [tool.poetry.extras]
 docs = ["Sphinx", "sphinxcontrib-trio", "sphinx-autodoc-typehints", "sphinx-rtd-theme",
     "sphinx-inline-tabs"]
 
 
 [tool.pytest.ini_options]
```

### Comparing `serena-0.7.3/src/serena/__init__.py` & `serena-0.7.4/src/serena/__init__.py`

 * *Files identical despite different names*

### Comparing `serena-0.7.3/src/serena/channel.py` & `serena-0.7.4/src/serena/channel.py`

 * *Files identical despite different names*

### Comparing `serena-0.7.3/src/serena/channel.py.orig` & `serena-0.7.4/src/serena/channel.py.orig`

 * *Files identical despite different names*

### Comparing `serena-0.7.3/src/serena/connection.py` & `serena-0.7.4/src/serena/connection.py`

 * *Files identical despite different names*

### Comparing `serena-0.7.3/src/serena/enums.py` & `serena-0.7.4/src/serena/enums.py`

 * *Files identical despite different names*

### Comparing `serena-0.7.3/src/serena/exc.py` & `serena-0.7.4/src/serena/exc.py`

 * *Files identical despite different names*

### Comparing `serena-0.7.3/src/serena/frame.py` & `serena-0.7.4/src/serena/frame.py`

 * *Files identical despite different names*

### Comparing `serena-0.7.3/src/serena/frameparser.py` & `serena-0.7.4/src/serena/frameparser.py`

 * *Files identical despite different names*

### Comparing `serena-0.7.3/src/serena/message.py` & `serena-0.7.4/src/serena/message.py`

 * *Files identical despite different names*

### Comparing `serena-0.7.3/src/serena/mixin.py` & `serena-0.7.4/src/serena/mixin.py`

 * *Files identical despite different names*

### Comparing `serena-0.7.3/src/serena/payloads/__pycache__/encoding.cpython-310.pyc` & `serena-0.7.4/src/serena/payloads/__pycache__/encoding.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `serena-0.7.3/src/serena/payloads/__pycache__/header.cpython-310.pyc` & `serena-0.7.4/src/serena/payloads/__pycache__/header.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Jan 22 23:31:42 2022 UTC, .py size: 4697 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 de93 ec61 5912 0000  o..........aY...
+00000000: 6f0d 0d0a 0000 0000 01d3 fb61 5912 0000  o..........aY...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0173 e200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6403 6c03 6d04 5a04 6d05 5a05  Z.d.d.l.m.Z.m.Z.
 00000050: 6d06 5a06 6d07 5a07 0100 6400 6402 6c08  m.Z.m.Z...d.d.l.
 00000060: 5a08 6400 6404 6c09 6d0a 5a0a 6d0b 5a0b  Z.d.d.l.m.Z.m.Z.
 00000070: 0100 6400 6405 6c0c 6d0d 5a0d 6d0e 5a0e  ..d.d.l.m.Z.m.Z.
```

### Comparing `serena-0.7.3/src/serena/payloads/__pycache__/method.cpython-310.pyc` & `serena-0.7.4/src/serena/payloads/__pycache__/method.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `serena-0.7.3/src/serena/payloads/encoding.py` & `serena-0.7.4/src/serena/payloads/encoding.py`

 * *Files identical despite different names*

### Comparing `serena-0.7.3/src/serena/payloads/header.py` & `serena-0.7.4/src/serena/payloads/header.py`

 * *Files identical despite different names*

### Comparing `serena-0.7.3/src/serena/payloads/method.py` & `serena-0.7.4/src/serena/payloads/method.py`

 * *Files identical despite different names*

### Comparing `serena-0.7.3/src/serena/pool.py` & `serena-0.7.4/src/serena/pool.py`

 * *Files identical despite different names*

### Comparing `serena-0.7.3/src/serena/utils/__pycache__/bitset.cpython-310.pyc` & `serena-0.7.4/src/serena/utils/__pycache__/bitset.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `serena-0.7.3/src/serena/utils/__pycache__/buffer.cpython-310.pyc` & `serena-0.7.4/src/serena/utils/__pycache__/buffer.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `serena-0.7.3/src/serena/utils/bitset.py` & `serena-0.7.4/src/serena/utils/bitset.py`

 * *Files identical despite different names*

### Comparing `serena-0.7.3/src/serena/utils/buffer.py` & `serena-0.7.4/src/serena/utils/buffer.py`

 * *Files identical despite different names*

### Comparing `serena-0.7.3/PKG-INFO` & `serena-0.7.4/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,32 +1,26 @@
 Metadata-Version: 2.1
 Name: serena
-Version: 0.7.3
+Version: 0.7.4
 Summary: An AMQP 0-9-1 client using AnyIO.
 License: LGPL-3.0-or-later
 Author: Lura Skye
 Author-email: l@veriny.tf
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AnyIO
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: docs
-Requires-Dist: Sphinx (>=4.3.2,<5.0.0); extra == "docs"
-Requires-Dist: anyio (>=3.5.0,<4.0.0)
-Requires-Dist: attrs (>=21.4.0,<22.0.0)
-Requires-Dist: backports.strenum; python_version < "3.11"
-Requires-Dist: sphinx-autodoc-typehints (>=1.15.2,<2.0.0); extra == "docs"
-Requires-Dist: sphinx-inline-tabs (>=2022.1.2-beta.11,<2023.0.0); extra == "docs"
-Requires-Dist: sphinx-rtd-theme (>=1.0.0,<2.0.0); extra == "docs"
-Requires-Dist: sphinxcontrib-trio (>=1.1.2,<2.0.0); extra == "docs"
+Requires-Dist: anyio (>=3.6.2)
+Requires-Dist: attrs (>=21.4.0)
+Requires-Dist: backports.strenum (>=1.1.1,<2.0.0) ; python_version < "3.11"
 Description-Content-Type: text/x-rst
 
 Serena
 ======
 
 *Serena* is a pure-Python, structually concurrent AMQP 0-9-1 client.
```

