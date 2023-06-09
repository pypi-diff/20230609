# Comparing `tmp/patio_rabbitmq-0.1.0.tar.gz` & `tmp/patio_rabbitmq-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "patio_rabbitmq-0.1.0.tar", max compression
+gzip compressed data, was "patio_rabbitmq-0.1.1.tar", max compression
```

## Comparing `patio_rabbitmq-0.1.0.tar` & `patio_rabbitmq-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     1408 2023-06-08 15:07:15.006551 patio_rabbitmq-0.1.0/README.md
--rw-r--r--   0        0        0     2158 2023-06-08 15:07:15.040124 patio_rabbitmq-0.1.0/patio_rabbitmq.py
--rw-r--r--   0        0        0     2193 2023-06-08 15:07:15.042371 patio_rabbitmq-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2862 1970-01-01 00:00:00.000000 patio_rabbitmq-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2155 2023-06-09 07:06:46.800976 patio_rabbitmq-0.1.1/README.md
+-rw-r--r--   0        0        0     2158 2023-06-08 15:07:15.040124 patio_rabbitmq-0.1.1/patio_rabbitmq.py
+-rw-r--r--   0        0        0     2193 2023-06-09 08:18:12.209035 patio_rabbitmq-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3609 1970-01-01 00:00:00.000000 patio_rabbitmq-0.1.1/PKG-INFO
```

### Comparing `patio_rabbitmq-0.1.0/patio_rabbitmq.py` & `patio_rabbitmq-0.1.1/patio_rabbitmq.py`

 * *Files identical despite different names*

### Comparing `patio_rabbitmq-0.1.0/pyproject.toml` & `patio_rabbitmq-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 
 name = "patio-rabbitmq"
-version = "0.1.0"
+version = "0.1.1"
 description = "RabbitMQ broker implementation for PATIO"
 authors = ["Dmitry Orlov <me@mosquito.su>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Framework :: AsyncIO",
```

### Comparing `patio_rabbitmq-0.1.0/PKG-INFO` & `patio_rabbitmq-0.1.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: patio-rabbitmq
-Version: 0.1.0
+Version: 0.1.1
 Summary: RabbitMQ broker implementation for PATIO
 License: MIT
 Author: Dmitry Orlov
 Author-email: me@mosquito.su
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AsyncIO
@@ -30,14 +30,16 @@
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Dist: aio-pika (>=9.0.7,<10.0.0)
 Requires-Dist: patio
 Description-Content-Type: text/markdown
 
+[![PyPI - License](https://img.shields.io/pypi/l/patio-rabbitmq)](https://pypi.org/project/patio-rabbitmq) [![Wheel](https://img.shields.io/pypi/wheel/patio-rabbitmq)](https://pypi.org/project/patio-rabbitmq) [![Mypy](http://www.mypy-lang.org/static/mypy_badge.svg)]() [![PyPI](https://img.shields.io/pypi/v/patio-rabbitmq)](https://pypi.org/project/patio-rabbitmq) [![PyPI](https://img.shields.io/pypi/pyversions/patio-rabbitmq)](https://pypi.org/project/patio-rabbitmq) [![Coverage Status](https://coveralls.io/repos/github/patio-python/patio-rabbitmq/badge.svg?branch=master)](https://coveralls.io/github/patio-python/patio-rabbitmq?branch=master) ![tox](https://github.com/patio-python/patio-rabbitmq/workflows/tests/badge.svg?branch=master)
+
 PATIO Rabbitmq
 ==============
 
 PATIO is an acronym for **P**ython **A**synchronous **T**ask for Async**IO**.
 
 This package provides RabbitMQ broker implementation.
```

