# Comparing `tmp/libsnmp-3.0.0.tar.gz` & `tmp/libsnmp-3.0.1.tar.gz`

## Comparing `libsnmp-3.0.0.tar` & `libsnmp-3.0.1.tar`

### file list

```diff
@@ -1,44 +1,43 @@
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 libsnmp-3.0.0/COPYRIGHT
--rw-r--r--   0        0        0     2252 2020-02-02 00:00:00.000000 libsnmp-3.0.0/ChangeLog
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 libsnmp-3.0.0/INSTALL
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 libsnmp-3.0.0/MANIFEST
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 libsnmp-3.0.0/TODO
--rwxr-xr-x   0        0        0     1572 2020-02-02 00:00:00.000000 libsnmp-3.0.0/setup.py
--rwxr-xr-x   0        0        0     1622 2020-02-02 00:00:00.000000 libsnmp-3.0.0/snmpget-v1.py
--rwxr-xr-x   0        0        0     1622 2020-02-02 00:00:00.000000 libsnmp-3.0.0/snmpget-v2.py
--rwxr-xr-x   0        0        0     1774 2020-02-02 00:00:00.000000 libsnmp-3.0.0/snmpget.py
--rwxr-xr-x   0        0        0     1783 2020-02-02 00:00:00.000000 libsnmp-3.0.0/snmpset.py
--rwxr-xr-x   0        0        0     1853 2020-02-02 00:00:00.000000 libsnmp-3.0.0/snmpwalk.py
--rwxr-xr-x   0        0        0     1640 2020-02-02 00:00:00.000000 libsnmp-3.0.0/traplistener.py
--rwxr-xr-x   0        0        0     1399 2020-02-02 00:00:00.000000 libsnmp-3.0.0/trapsender.py
--rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 libsnmp-3.0.0/.github/workflows/python-app.yml
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 libsnmp-3.0.0/debian/changelog
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 libsnmp-3.0.0/debian/compat
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 libsnmp-3.0.0/debian/control
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 libsnmp-3.0.0/debian/copyright
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 libsnmp-3.0.0/debian/pyversions
--rwxr-xr-x   0        0        0     1963 2020-02-02 00:00:00.000000 libsnmp-3.0.0/debian/rules
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 libsnmp-3.0.0/lib/libsnmp/__init__.py
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 libsnmp-3.0.0/lib/libsnmp/asynrole.py
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 libsnmp-3.0.0/lib/libsnmp/debug.py
--rw-r--r--   0        0        0    27845 2020-02-02 00:00:00.000000 libsnmp-3.0.0/lib/libsnmp/rfc1155.py
--rw-r--r--   0        0        0     7742 2020-02-02 00:00:00.000000 libsnmp-3.0.0/lib/libsnmp/rfc1157.py
--rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 libsnmp-3.0.0/lib/libsnmp/rfc1902.py
--rw-r--r--   0        0        0     6688 2020-02-02 00:00:00.000000 libsnmp-3.0.0/lib/libsnmp/rfc1905.py
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 libsnmp-3.0.0/lib/libsnmp/role.py
--rw-r--r--   0        0        0    12662 2020-02-02 00:00:00.000000 libsnmp-3.0.0/lib/libsnmp/snmpmanager.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 libsnmp-3.0.0/lib/libsnmp/util.py
--rw-r--r--   0        0        0     9012 2020-02-02 00:00:00.000000 libsnmp-3.0.0/lib/libsnmp/v1.py
--rw-r--r--   0        0        0     7235 2020-02-02 00:00:00.000000 libsnmp-3.0.0/lib/libsnmp/v2.py
--rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 libsnmp-3.0.0/test/test_Messages.py
--rw-r--r--   0        0        0     2848 2020-02-02 00:00:00.000000 libsnmp-3.0.0/test/test_asynrole.py
--rw-r--r--   0        0        0     9855 2020-02-02 00:00:00.000000 libsnmp-3.0.0/test/test_encoder.py
--rw-r--r--   0        0        0     4421 2020-02-02 00:00:00.000000 libsnmp-3.0.0/test/test_rfc1155.py
--rw-r--r--   0        0        0     6559 2020-02-02 00:00:00.000000 libsnmp-3.0.0/test/test_rfc1157.py
--rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 libsnmp-3.0.0/test/test_snmpmanager.py
--rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 libsnmp-3.0.0/test/test_svt_encoder.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 libsnmp-3.0.0/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 libsnmp-3.0.0/LICENSE
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 libsnmp-3.0.0/README.md
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 libsnmp-3.0.0/pyproject.toml
--rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 libsnmp-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 libsnmp-3.0.1/COPYRIGHT
+-rw-r--r--   0        0        0     2252 2020-02-02 00:00:00.000000 libsnmp-3.0.1/ChangeLog
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 libsnmp-3.0.1/INSTALL
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 libsnmp-3.0.1/MANIFEST
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 libsnmp-3.0.1/TODO
+-rwxr-xr-x   0        0        0     1622 2020-02-02 00:00:00.000000 libsnmp-3.0.1/snmpget-v1.py
+-rwxr-xr-x   0        0        0     1622 2020-02-02 00:00:00.000000 libsnmp-3.0.1/snmpget-v2.py
+-rwxr-xr-x   0        0        0     1774 2020-02-02 00:00:00.000000 libsnmp-3.0.1/snmpget.py
+-rwxr-xr-x   0        0        0     1783 2020-02-02 00:00:00.000000 libsnmp-3.0.1/snmpset.py
+-rwxr-xr-x   0        0        0     1853 2020-02-02 00:00:00.000000 libsnmp-3.0.1/snmpwalk.py
+-rwxr-xr-x   0        0        0     1640 2020-02-02 00:00:00.000000 libsnmp-3.0.1/traplistener.py
+-rwxr-xr-x   0        0        0     1399 2020-02-02 00:00:00.000000 libsnmp-3.0.1/trapsender.py
+-rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 libsnmp-3.0.1/.github/workflows/python-app.yml
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 libsnmp-3.0.1/debian/changelog
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 libsnmp-3.0.1/debian/compat
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 libsnmp-3.0.1/debian/control
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 libsnmp-3.0.1/debian/copyright
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 libsnmp-3.0.1/debian/pyversions
+-rwxr-xr-x   0        0        0     1963 2020-02-02 00:00:00.000000 libsnmp-3.0.1/debian/rules
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 libsnmp-3.0.1/lib/libsnmp/__init__.py
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 libsnmp-3.0.1/lib/libsnmp/asynrole.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 libsnmp-3.0.1/lib/libsnmp/debug.py
+-rw-r--r--   0        0        0    27845 2020-02-02 00:00:00.000000 libsnmp-3.0.1/lib/libsnmp/rfc1155.py
+-rw-r--r--   0        0        0     7742 2020-02-02 00:00:00.000000 libsnmp-3.0.1/lib/libsnmp/rfc1157.py
+-rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 libsnmp-3.0.1/lib/libsnmp/rfc1902.py
+-rw-r--r--   0        0        0     6688 2020-02-02 00:00:00.000000 libsnmp-3.0.1/lib/libsnmp/rfc1905.py
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 libsnmp-3.0.1/lib/libsnmp/role.py
+-rw-r--r--   0        0        0    12662 2020-02-02 00:00:00.000000 libsnmp-3.0.1/lib/libsnmp/snmpmanager.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 libsnmp-3.0.1/lib/libsnmp/util.py
+-rw-r--r--   0        0        0     9012 2020-02-02 00:00:00.000000 libsnmp-3.0.1/lib/libsnmp/v1.py
+-rw-r--r--   0        0        0     7235 2020-02-02 00:00:00.000000 libsnmp-3.0.1/lib/libsnmp/v2.py
+-rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 libsnmp-3.0.1/test/test_Messages.py
+-rw-r--r--   0        0        0     2848 2020-02-02 00:00:00.000000 libsnmp-3.0.1/test/test_asynrole.py
+-rw-r--r--   0        0        0     9855 2020-02-02 00:00:00.000000 libsnmp-3.0.1/test/test_encoder.py
+-rw-r--r--   0        0        0     4421 2020-02-02 00:00:00.000000 libsnmp-3.0.1/test/test_rfc1155.py
+-rw-r--r--   0        0        0     6559 2020-02-02 00:00:00.000000 libsnmp-3.0.1/test/test_rfc1157.py
+-rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 libsnmp-3.0.1/test/test_snmpmanager.py
+-rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 libsnmp-3.0.1/test/test_svt_encoder.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 libsnmp-3.0.1/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 libsnmp-3.0.1/LICENSE
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 libsnmp-3.0.1/README.md
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 libsnmp-3.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 libsnmp-3.0.1/PKG-INFO
```

### Comparing `libsnmp-3.0.0/COPYRIGHT` & `libsnmp-3.0.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `libsnmp-3.0.0/ChangeLog` & `libsnmp-3.0.1/ChangeLog`

 * *Files identical despite different names*

### Comparing `libsnmp-3.0.0/MANIFEST` & `libsnmp-3.0.1/MANIFEST`

 * *Files identical despite different names*

### Comparing `libsnmp-3.0.0/TODO` & `libsnmp-3.0.1/TODO`

 * *Files identical despite different names*

### Comparing `libsnmp-3.0.0/snmpget-v1.py` & `libsnmp-3.0.1/snmpget-v1.py`

 * *Files identical despite different names*

### Comparing `libsnmp-3.0.0/snmpget-v2.py` & `libsnmp-3.0.1/snmpget-v2.py`

 * *Files identical despite different names*

### Comparing `libsnmp-3.0.0/snmpget.py` & `libsnmp-3.0.1/snmpget.py`

 * *Files identical despite different names*

### Comparing `libsnmp-3.0.0/snmpset.py` & `libsnmp-3.0.1/snmpset.py`

 * *Files identical despite different names*

### Comparing `libsnmp-3.0.0/snmpwalk.py` & `libsnmp-3.0.1/snmpwalk.py`

 * *Files identical despite different names*

### Comparing `libsnmp-3.0.0/traplistener.py` & `libsnmp-3.0.1/traplistener.py`

 * *Files identical despite different names*

### Comparing `libsnmp-3.0.0/trapsender.py` & `libsnmp-3.0.1/trapsender.py`

 * *Files identical despite different names*

### Comparing `libsnmp-3.0.0/.github/workflows/python-app.yml` & `libsnmp-3.0.1/.github/workflows/python-app.yml`

 * *Files identical despite different names*

### Comparing `libsnmp-3.0.0/debian/changelog` & `libsnmp-3.0.1/debian/changelog`

 * *Files identical despite different names*

### Comparing `libsnmp-3.0.0/debian/control` & `libsnmp-3.0.1/debian/control`

 * *Files identical despite different names*

### Comparing `libsnmp-3.0.0/debian/copyright` & `libsnmp-3.0.1/debian/copyright`

 * *Files identical despite different names*

### Comparing `libsnmp-3.0.0/debian/rules` & `libsnmp-3.0.1/debian/rules`

 * *Files identical despite different names*

### Comparing `libsnmp-3.0.0/lib/libsnmp/asynrole.py` & `libsnmp-3.0.1/lib/libsnmp/asynrole.py`

 * *Files identical despite different names*

### Comparing `libsnmp-3.0.0/lib/libsnmp/debug.py` & `libsnmp-3.0.1/lib/libsnmp/debug.py`

 * *Files identical despite different names*

### Comparing `libsnmp-3.0.0/lib/libsnmp/rfc1155.py` & `libsnmp-3.0.1/lib/libsnmp/rfc1155.py`

 * *Files identical despite different names*

### Comparing `libsnmp-3.0.0/lib/libsnmp/rfc1157.py` & `libsnmp-3.0.1/lib/libsnmp/rfc1157.py`

 * *Files identical despite different names*

### Comparing `libsnmp-3.0.0/lib/libsnmp/rfc1902.py` & `libsnmp-3.0.1/lib/libsnmp/rfc1902.py`

 * *Files identical despite different names*

### Comparing `libsnmp-3.0.0/lib/libsnmp/rfc1905.py` & `libsnmp-3.0.1/lib/libsnmp/rfc1905.py`

 * *Files identical despite different names*

### Comparing `libsnmp-3.0.0/lib/libsnmp/role.py` & `libsnmp-3.0.1/lib/libsnmp/role.py`

 * *Files identical despite different names*

### Comparing `libsnmp-3.0.0/lib/libsnmp/snmpmanager.py` & `libsnmp-3.0.1/lib/libsnmp/snmpmanager.py`

 * *Files identical despite different names*

### Comparing `libsnmp-3.0.0/lib/libsnmp/util.py` & `libsnmp-3.0.1/lib/libsnmp/util.py`

 * *Files identical despite different names*

### Comparing `libsnmp-3.0.0/lib/libsnmp/v1.py` & `libsnmp-3.0.1/lib/libsnmp/v1.py`

 * *Files identical despite different names*

### Comparing `libsnmp-3.0.0/lib/libsnmp/v2.py` & `libsnmp-3.0.1/lib/libsnmp/v2.py`

 * *Files identical despite different names*

### Comparing `libsnmp-3.0.0/test/test_Messages.py` & `libsnmp-3.0.1/test/test_Messages.py`

 * *Files identical despite different names*

### Comparing `libsnmp-3.0.0/test/test_asynrole.py` & `libsnmp-3.0.1/test/test_asynrole.py`

 * *Files identical despite different names*

### Comparing `libsnmp-3.0.0/test/test_encoder.py` & `libsnmp-3.0.1/test/test_encoder.py`

 * *Files identical despite different names*

### Comparing `libsnmp-3.0.0/test/test_rfc1155.py` & `libsnmp-3.0.1/test/test_rfc1155.py`

 * *Files identical despite different names*

### Comparing `libsnmp-3.0.0/test/test_rfc1157.py` & `libsnmp-3.0.1/test/test_rfc1157.py`

 * *Files identical despite different names*

### Comparing `libsnmp-3.0.0/test/test_snmpmanager.py` & `libsnmp-3.0.1/test/test_snmpmanager.py`

 * *Files identical despite different names*

### Comparing `libsnmp-3.0.0/test/test_svt_encoder.py` & `libsnmp-3.0.1/test/test_svt_encoder.py`

 * *Files identical despite different names*

### Comparing `libsnmp-3.0.0/LICENSE` & `libsnmp-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `libsnmp-3.0.0/README.md` & `libsnmp-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `libsnmp-3.0.0/pyproject.toml` & `libsnmp-3.0.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "libsnmp"
-version = "3.0.0"
+version = "3.0.1"
 description = "A pure Python implementation of the Simple Network Management Protocol"
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.0"
 keywords = ["SNMP", "library"]
 authors = [ 
     {name = "Justin Warren"}, {email = "daedalus@eigenmagic.com"}
@@ -27,11 +27,14 @@
 documentation = "https://github.com/jpwarren/libsnmp"
 repository = "https://github.com/jpwarren/libsnmp"
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
+[tool.hatch.build.targets.wheel]
+packages = ['lib/libsnmp']
+
 [tool.pytest.ini_options]
 addopts = [
     "--import-mode=importlib",
 ]
```

### Comparing `libsnmp-3.0.0/PKG-INFO` & `libsnmp-3.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libsnmp
-Version: 3.0.0
+Version: 3.0.1
 Summary: A pure Python implementation of the Simple Network Management Protocol
 Project-URL: homepage, https://github.com/jpwarren/libsnmp
 Project-URL: documentation, https://github.com/jpwarren/libsnmp
 Project-URL: repository, https://github.com/jpwarren/libsnmp
 Author: Justin Warren
 Author-email: daedalus@eigenmagic.com
 License: Copyright (c) 2003 Justin Warren <daedalus@eigenmagic.com>
```

