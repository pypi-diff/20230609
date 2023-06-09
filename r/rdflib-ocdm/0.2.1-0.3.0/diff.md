# Comparing `tmp/rdflib_ocdm-0.2.1.tar.gz` & `tmp/rdflib_ocdm-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdflib_ocdm-0.2.1.tar", max compression
+gzip compressed data, was "rdflib_ocdm-0.3.0.tar", max compression
```

## Comparing `rdflib_ocdm-0.2.1.tar` & `rdflib_ocdm-0.3.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0      497 2023-06-05 16:08:39.917692 rdflib_ocdm-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      840 2023-04-20 10:05:30.759897 rdflib_ocdm-0.2.1/rdflib_ocdm/__init__.py
--rw-r--r--   0        0        0     6176 2023-04-19 10:29:03.161700 rdflib_ocdm-0.2.1/rdflib_ocdm/abstract_entity.py
--rw-r--r--   0        0        0      839 2023-04-14 08:27:27.373276 rdflib_ocdm-0.2.1/rdflib_ocdm/counter_handler/__init__.py
--rw-r--r--   0        0        0     2444 2023-04-14 08:14:45.294985 rdflib_ocdm-0.2.1/rdflib_ocdm/counter_handler/counter_handler.py
--rw-r--r--   0        0        0     5348 2023-06-05 21:03:43.220445 rdflib_ocdm-0.2.1/rdflib_ocdm/counter_handler/filesystem_counter_handler.py
--rw-r--r--   0        0        0     3119 2023-04-14 08:28:16.301132 rdflib_ocdm-0.2.1/rdflib_ocdm/counter_handler/in_memory_counter_handler.py
--rw-r--r--   0        0        0     3529 2023-06-05 21:22:26.205708 rdflib_ocdm-0.2.1/rdflib_ocdm/counter_handler/sqlite_counter_handler.py
--rw-r--r--   0        0        0     4612 2023-06-05 21:12:44.765077 rdflib_ocdm-0.2.1/rdflib_ocdm/ocdm_graph.py
--rw-r--r--   0        0        0      839 2023-04-14 08:14:45.296986 rdflib_ocdm-0.2.1/rdflib_ocdm/prov/__init__.py
--rw-r--r--   0        0        0     2906 2023-04-19 11:46:36.923513 rdflib_ocdm-0.2.1/rdflib_ocdm/prov/prov_entity.py
--rw-r--r--   0        0        0     7604 2023-06-05 21:16:39.230517 rdflib_ocdm-0.2.1/rdflib_ocdm/prov/provenance.py
--rw-r--r--   0        0        0    13514 2023-04-19 09:56:14.655005 rdflib_ocdm-0.2.1/rdflib_ocdm/prov/snapshot_entity.py
--rw-r--r--   0        0        0     4447 2023-04-19 11:43:30.274044 rdflib_ocdm-0.2.1/rdflib_ocdm/query_utils.py
--rw-r--r--   0        0        0     2259 2023-05-11 11:36:15.565333 rdflib_ocdm-0.2.1/rdflib_ocdm/reader.py
--rw-r--r--   0        0        0     4905 2023-04-19 10:53:30.709617 rdflib_ocdm-0.2.1/rdflib_ocdm/storer.py
--rw-r--r--   0        0        0     2570 2023-04-19 10:34:23.494049 rdflib_ocdm-0.2.1/rdflib_ocdm/support.py
--rw-r--r--   0        0        0      600 2023-04-20 10:52:06.623319 rdflib_ocdm-0.2.1/README.md
--rw-r--r--   0        0        0     1307 1970-01-01 00:00:00.000000 rdflib_ocdm-0.2.1/setup.py
--rw-r--r--   0        0        0     1212 1970-01-01 00:00:00.000000 rdflib_ocdm-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      515 2023-06-09 09:39:15.238291 rdflib_ocdm-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      840 2023-06-05 16:04:18.138485 rdflib_ocdm-0.3.0/rdflib_ocdm/__init__.py
+-rw-r--r--   0        0        0     6176 2023-06-05 16:04:18.139484 rdflib_ocdm-0.3.0/rdflib_ocdm/abstract_entity.py
+-rw-r--r--   0        0        0      839 2023-06-05 16:04:18.140484 rdflib_ocdm-0.3.0/rdflib_ocdm/counter_handler/__init__.py
+-rw-r--r--   0        0        0     2444 2023-06-05 16:04:18.142487 rdflib_ocdm-0.3.0/rdflib_ocdm/counter_handler/counter_handler.py
+-rw-r--r--   0        0        0     5348 2023-06-09 09:38:58.425496 rdflib_ocdm-0.3.0/rdflib_ocdm/counter_handler/filesystem_counter_handler.py
+-rw-r--r--   0        0        0     3119 2023-06-05 16:04:18.143488 rdflib_ocdm-0.3.0/rdflib_ocdm/counter_handler/in_memory_counter_handler.py
+-rw-r--r--   0        0        0     2026 2023-06-09 09:41:45.384683 rdflib_ocdm-0.3.0/rdflib_ocdm/counter_handler/redis_counter_handler.py
+-rw-r--r--   0        0        0     3529 2023-06-09 09:26:28.883672 rdflib_ocdm-0.3.0/rdflib_ocdm/counter_handler/sqlite_counter_handler.py
+-rw-r--r--   0        0        0     4612 2023-06-09 09:27:28.906520 rdflib_ocdm-0.3.0/rdflib_ocdm/ocdm_graph.py
+-rw-r--r--   0        0        0      839 2023-06-05 16:04:18.146489 rdflib_ocdm-0.3.0/rdflib_ocdm/prov/__init__.py
+-rw-r--r--   0        0        0     2906 2023-06-05 16:04:18.147772 rdflib_ocdm-0.3.0/rdflib_ocdm/prov/prov_entity.py
+-rw-r--r--   0        0        0     7604 2023-06-09 09:28:35.986054 rdflib_ocdm-0.3.0/rdflib_ocdm/prov/provenance.py
+-rw-r--r--   0        0        0    13514 2023-06-05 16:04:18.148774 rdflib_ocdm-0.3.0/rdflib_ocdm/prov/snapshot_entity.py
+-rw-r--r--   0        0        0     4447 2023-06-05 16:04:18.149774 rdflib_ocdm-0.3.0/rdflib_ocdm/query_utils.py
+-rw-r--r--   0        0        0     2259 2023-06-09 09:38:43.697466 rdflib_ocdm-0.3.0/rdflib_ocdm/reader.py
+-rw-r--r--   0        0        0     9000 2023-06-09 08:30:35.689725 rdflib_ocdm-0.3.0/rdflib_ocdm/storer.py
+-rw-r--r--   0        0        0     2570 2023-06-05 16:04:18.152780 rdflib_ocdm-0.3.0/rdflib_ocdm/support.py
+-rw-r--r--   0        0        0      600 2023-04-20 10:52:06.623319 rdflib_ocdm-0.3.0/README.md
+-rw-r--r--   0        0        0     1333 1970-01-01 00:00:00.000000 rdflib_ocdm-0.3.0/setup.py
+-rw-r--r--   0        0        0     1250 1970-01-01 00:00:00.000000 rdflib_ocdm-0.3.0/PKG-INFO
```

### Comparing `rdflib_ocdm-0.2.1/rdflib_ocdm/__init__.py` & `rdflib_ocdm-0.3.0/rdflib_ocdm/__init__.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.2.1/rdflib_ocdm/abstract_entity.py` & `rdflib_ocdm-0.3.0/rdflib_ocdm/abstract_entity.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.2.1/rdflib_ocdm/counter_handler/__init__.py` & `rdflib_ocdm-0.3.0/rdflib_ocdm/counter_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.2.1/rdflib_ocdm/counter_handler/counter_handler.py` & `rdflib_ocdm-0.3.0/rdflib_ocdm/counter_handler/counter_handler.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.2.1/rdflib_ocdm/counter_handler/filesystem_counter_handler.py` & `rdflib_ocdm-0.3.0/rdflib_ocdm/counter_handler/filesystem_counter_handler.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.2.1/rdflib_ocdm/counter_handler/in_memory_counter_handler.py` & `rdflib_ocdm-0.3.0/rdflib_ocdm/counter_handler/in_memory_counter_handler.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.2.1/rdflib_ocdm/counter_handler/sqlite_counter_handler.py` & `rdflib_ocdm-0.3.0/rdflib_ocdm/counter_handler/sqlite_counter_handler.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.2.1/rdflib_ocdm/ocdm_graph.py` & `rdflib_ocdm-0.3.0/rdflib_ocdm/ocdm_graph.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.2.1/rdflib_ocdm/prov/__init__.py` & `rdflib_ocdm-0.3.0/rdflib_ocdm/prov/__init__.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.2.1/rdflib_ocdm/prov/prov_entity.py` & `rdflib_ocdm-0.3.0/rdflib_ocdm/prov/prov_entity.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.2.1/rdflib_ocdm/prov/provenance.py` & `rdflib_ocdm-0.3.0/rdflib_ocdm/prov/provenance.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.2.1/rdflib_ocdm/prov/snapshot_entity.py` & `rdflib_ocdm-0.3.0/rdflib_ocdm/prov/snapshot_entity.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.2.1/rdflib_ocdm/query_utils.py` & `rdflib_ocdm-0.3.0/rdflib_ocdm/query_utils.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.2.1/rdflib_ocdm/reader.py` & `rdflib_ocdm-0.3.0/rdflib_ocdm/reader.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.2.1/rdflib_ocdm/support.py` & `rdflib_ocdm-0.3.0/rdflib_ocdm/support.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.2.1/README.md` & `rdflib_ocdm-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.2.1/setup.py` & `rdflib_ocdm-0.3.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,19 +4,22 @@
 packages = \
 ['rdflib_ocdm', 'rdflib_ocdm.counter_handler', 'rdflib_ocdm.prov']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['oc-ocdm>=7.1.7,<8.0.0', 'rdflib>=6.2.0,<7.0.0', 'sparqlwrapper>=2.0.0,<3.0.0']
+['oc-ocdm>=7.1.7,<8.0.0',
+ 'rdflib>=6.2.0,<7.0.0',
+ 'redis>=4.5.5,<5.0.0',
+ 'sparqlwrapper>=2.0.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'rdflib-ocdm',
-    'version': '0.2.1',
+    'version': '0.3.0',
     'description': '',
     'long_description': '[<img src="https://img.shields.io/badge/powered%20by-OpenCitations-%239931FC?labelColor=2D22DE" />](http://opencitations.net)\n[![Run tests](https://github.com/opencitations/rdflib-ocdm/actions/workflows/run_tests.yml/badge.svg)](https://github.com/opencitations/rdflib-ocdm/actions/workflows/run_tests.yml)\n![Coverage](https://raw.githubusercontent.com/opencitations/rdflib-ocdm/main/test/coverage/coverage.svg)\n![PyPI](https://img.shields.io/pypi/pyversions/rdflib-ocdm)\n![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/opencitations/rdflib-ocdm)\n\n# rdflib-ocdm\n',
     'author': 'arcangelo7',
     'author_email': 'arcangelomas@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `rdflib_ocdm-0.2.1/PKG-INFO` & `rdflib_ocdm-0.3.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: rdflib-ocdm
-Version: 0.2.1
+Version: 0.3.0
 Summary: 
 License: ISC
 Author: arcangelo7
 Author-email: arcangelomas@gmail.com
 Requires-Python: >=3.7.4,<4.0.0
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: oc-ocdm (>=7.1.7,<8.0.0)
 Requires-Dist: rdflib (>=6.2.0,<7.0.0)
+Requires-Dist: redis (>=4.5.5,<5.0.0)
 Requires-Dist: sparqlwrapper (>=2.0.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 [<img src="https://img.shields.io/badge/powered%20by-OpenCitations-%239931FC?labelColor=2D22DE" />](http://opencitations.net)
 [![Run tests](https://github.com/opencitations/rdflib-ocdm/actions/workflows/run_tests.yml/badge.svg)](https://github.com/opencitations/rdflib-ocdm/actions/workflows/run_tests.yml)
 ![Coverage](https://raw.githubusercontent.com/opencitations/rdflib-ocdm/main/test/coverage/coverage.svg)
 ![PyPI](https://img.shields.io/pypi/pyversions/rdflib-ocdm)
```

