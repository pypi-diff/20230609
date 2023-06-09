# Comparing `tmp/patio_redis-0.1.0.tar.gz` & `tmp/patio_redis-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "patio_redis-0.1.0.tar", max compression
+gzip compressed data, was "patio_redis-0.1.1.tar", max compression
```

## Comparing `patio_redis-0.1.0.tar` & `patio_redis-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      156 2023-06-08 15:21:48.297273 patio_redis-0.1.0/README.md
--rw-r--r--   0        0        0     7250 2023-06-08 15:21:48.300897 patio_redis-0.1.0/patio_redis.py
--rw-r--r--   0        0        0     2200 2023-06-08 15:21:48.302877 patio_redis-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1600 1970-01-01 00:00:00.000000 patio_redis-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2183 2023-06-09 08:18:01.152290 patio_redis-0.1.1/README.md
+-rw-r--r--   0        0        0     7250 2023-06-08 15:21:48.300897 patio_redis-0.1.1/patio_redis.py
+-rw-r--r--   0        0        0     2200 2023-06-09 07:04:57.454738 patio_redis-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3627 1970-01-01 00:00:00.000000 patio_redis-0.1.1/PKG-INFO
```

### Comparing `patio_redis-0.1.0/patio_redis.py` & `patio_redis-0.1.1/patio_redis.py`

 * *Files identical despite different names*

### Comparing `patio_redis-0.1.0/pyproject.toml` & `patio_redis-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "patio-redis"
-version = "0.1.0"
+version = "0.1.1"
 description = "Redis broker implementation for PATIO"
 authors = ["Dmitry Orlov <me@mosquito.su>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Framework :: AsyncIO",
```

