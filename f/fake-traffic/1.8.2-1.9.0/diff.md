# Comparing `tmp/fake_traffic-1.8.2.tar.gz` & `tmp/fake_traffic-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fake_traffic-1.8.2.tar", last modified: Thu Nov 24 14:47:21 2022, max compression
+gzip compressed data, was "fake_traffic-1.9.0.tar", last modified: Fri Jun  9 18:13:22 2023, max compression
```

## Comparing `fake_traffic-1.8.2.tar` & `fake_traffic-1.9.0.tar`

### file list

```diff
@@ -1,14 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 14:47:21.165329 fake_traffic-1.8.2/
--rw-r--r--   0 runner    (1001) docker     (122)     1063 2022-11-24 14:47:02.000000 fake_traffic-1.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     5442 2022-11-24 14:47:21.165329 fake_traffic-1.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4433 2022-11-24 14:47:02.000000 fake_traffic-1.8.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 14:47:21.165329 fake_traffic-1.8.2/fake_traffic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     5442 2022-11-24 14:47:21.000000 fake_traffic-1.8.2/fake_traffic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      256 2022-11-24 14:47:21.000000 fake_traffic-1.8.2/fake_traffic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-24 14:47:21.000000 fake_traffic-1.8.2/fake_traffic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-24 14:47:21.000000 fake_traffic-1.8.2/fake_traffic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       97 2022-11-24 14:47:21.000000 fake_traffic-1.8.2/fake_traffic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2022-11-24 14:47:21.000000 fake_traffic-1.8.2/fake_traffic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     7876 2022-11-24 14:47:02.000000 fake_traffic-1.8.2/fake_traffic.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-24 14:47:21.165329 fake_traffic-1.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1515 2022-11-24 14:47:02.000000 fake_traffic-1.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:13:22.242478 fake_traffic-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-09 18:13:02.000000 fake_traffic-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-06-09 18:13:22.242478 fake_traffic-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-06-09 18:13:02.000000 fake_traffic-1.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:13:22.242478 fake_traffic-1.9.0/fake_traffic/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-09 18:13:02.000000 fake_traffic-1.9.0/fake_traffic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-06-09 18:13:02.000000 fake_traffic-1.9.0/fake_traffic/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8784 2023-06-09 18:13:02.000000 fake_traffic-1.9.0/fake_traffic/fake_traffic.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-09 18:13:02.000000 fake_traffic-1.9.0/fake_traffic/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:13:22.242478 fake_traffic-1.9.0/fake_traffic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-06-09 18:13:22.000000 fake_traffic-1.9.0/fake_traffic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-09 18:13:22.000000 fake_traffic-1.9.0/fake_traffic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 18:13:22.000000 fake_traffic-1.9.0/fake_traffic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-09 18:13:22.000000 fake_traffic-1.9.0/fake_traffic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-09 18:13:22.000000 fake_traffic-1.9.0/fake_traffic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-09 18:13:22.000000 fake_traffic-1.9.0/fake_traffic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-09 18:13:02.000000 fake_traffic-1.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 18:13:22.242478 fake_traffic-1.9.0/setup.cfg
```

### Comparing `fake_traffic-1.8.2/LICENSE` & `fake_traffic-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fake_traffic-1.8.2/PKG-INFO` & `fake_traffic-1.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: fake_traffic
-Version: 1.8.2
-Summary: Imitating an Internet user by mimicking popular web traffic
-Home-page: https://github.com/deedy5/fake_traffic
+Version: 1.9.0
+Summary: Imitating an Internet user by mimicking popular web traffic.
 Author: deedy5
-Author-email: 
-License: MIT
+License: MIT License
+Project-URL: Homepage, https://github.com/deedy5/duckduckgo_search
+Keywords: python,traffic generator
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Python >= 3.6](https://img.shields.io/badge/python->=3.6-red.svg)](https://www.python.org/downloads/) [![](https://badgen.net/github/release/deedy5/fake_traffic)](https://github.com/deedy5/fake_traffic/releases) [![](https://badge.fury.io/py/fake-traffic.svg)](https://pypi.org/project/fake-traffic) 
 # fake_traffic
 Imitating an Internet user by mimicking popular web traffic (internet traffic generator).
 
@@ -43,21 +42,25 @@
 ---
 ### Install
 
 ```python3
 pip install -U fake_traffic
 ```
 ---
-### Dependencies (are installed automatically)
+### CLI version
 ```python3
-lxml
-requests
-google_trends
-duckduckgo_search
-google_searching
+fake_traffic -h
+```
+CLI examples:
+```python3
+# user located in Turkey, who speaks Kurdish and is interested in hot stories
+fake_traffic -c tr -l ku-tr -ca h -d
+# user located in Brazil, who speaks Portuguese and is interested in sports
+fake_traffic -c br -l pt-br -ca s -d
+
 ```
 ---
 ### Simple usage
 ```python3
 from fake_traffic import fake_traffic
 
 fake_traffic(country='US', language='en-US")
```

### Comparing `fake_traffic-1.8.2/README.md` & `fake_traffic-1.9.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -18,21 +18,25 @@
 ---
 ### Install
 
 ```python3
 pip install -U fake_traffic
 ```
 ---
-### Dependencies (are installed automatically)
+### CLI version
 ```python3
-lxml
-requests
-google_trends
-duckduckgo_search
-google_searching
+fake_traffic -h
+```
+CLI examples:
+```python3
+# user located in Turkey, who speaks Kurdish and is interested in hot stories
+fake_traffic -c tr -l ku-tr -ca h -d
+# user located in Brazil, who speaks Portuguese and is interested in sports
+fake_traffic -c br -l pt-br -ca s -d
+
 ```
 ---
 ### Simple usage
 ```python3
 from fake_traffic import fake_traffic
 
 fake_traffic(country='US', language='en-US")
```

### Comparing `fake_traffic-1.8.2/fake_traffic.egg-info/PKG-INFO` & `fake_traffic-1.9.0/fake_traffic.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: fake-traffic
-Version: 1.8.2
-Summary: Imitating an Internet user by mimicking popular web traffic
-Home-page: https://github.com/deedy5/fake_traffic
+Version: 1.9.0
+Summary: Imitating an Internet user by mimicking popular web traffic.
 Author: deedy5
-Author-email: 
-License: MIT
+License: MIT License
+Project-URL: Homepage, https://github.com/deedy5/duckduckgo_search
+Keywords: python,traffic generator
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Python >= 3.6](https://img.shields.io/badge/python->=3.6-red.svg)](https://www.python.org/downloads/) [![](https://badgen.net/github/release/deedy5/fake_traffic)](https://github.com/deedy5/fake_traffic/releases) [![](https://badge.fury.io/py/fake-traffic.svg)](https://pypi.org/project/fake-traffic) 
 # fake_traffic
 Imitating an Internet user by mimicking popular web traffic (internet traffic generator).
 
@@ -43,21 +42,25 @@
 ---
 ### Install
 
 ```python3
 pip install -U fake_traffic
 ```
 ---
-### Dependencies (are installed automatically)
+### CLI version
 ```python3
-lxml
-requests
-google_trends
-duckduckgo_search
-google_searching
+fake_traffic -h
+```
+CLI examples:
+```python3
+# user located in Turkey, who speaks Kurdish and is interested in hot stories
+fake_traffic -c tr -l ku-tr -ca h -d
+# user located in Brazil, who speaks Portuguese and is interested in sports
+fake_traffic -c br -l pt-br -ca s -d
+
 ```
 ---
 ### Simple usage
 ```python3
 from fake_traffic import fake_traffic
 
 fake_traffic(country='US', language='en-US")
```

