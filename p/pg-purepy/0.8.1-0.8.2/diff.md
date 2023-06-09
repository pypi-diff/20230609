# Comparing `tmp/pg-purepy-0.8.1.tar.gz` & `tmp/pg_purepy-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pg-purepy-0.8.1.tar", max compression
+gzip compressed data, was "pg_purepy-0.8.2.tar", max compression
```

## Comparing `pg-purepy-0.8.1.tar` & `pg_purepy-0.8.2.tar`

### file list

```diff
@@ -1,39 +1,47 @@
--rw-r--r--   0        0        0      423 2021-07-04 22:53:41.121324 pg-purepy-0.8.1/README.rst
--rw-r--r--   0        0        0     1617 2022-04-20 23:15:37.547744 pg-purepy-0.8.1/pyproject.toml
--rw-r--r--   0        0        0      733 2022-03-22 12:12:13.790523 pg-purepy-0.8.1/src/pg_purepy/__init__.py
--rw-r--r--   0        0        0    20260 2022-03-22 12:12:05.497249 pg-purepy-0.8.1/src/pg_purepy/connection.py
--rw-r--r--   0        0        0     2986 2021-10-27 01:45:23.945806 pg-purepy-0.8.1/src/pg_purepy/conversion/__init__.py
--rw-r--r--   0        0        0     2981 2022-02-19 03:55:52.860474 pg-purepy-0.8.1/src/pg_purepy/conversion/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2985 2021-10-27 01:54:19.898864 pg-purepy-0.8.1/src/pg_purepy/conversion/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     2332 2022-02-19 03:55:52.897140 pg-purepy-0.8.1/src/pg_purepy/conversion/__pycache__/_parse_hstore.cpython-310.pyc
--rw-r--r--   0        0        0     2314 2021-10-27 11:58:23.491037 pg-purepy-0.8.1/src/pg_purepy/conversion/__pycache__/_parse_hstore.cpython-39.pyc
--rw-r--r--   0        0        0     2165 2022-02-19 03:55:52.863807 pg-purepy-0.8.1/src/pg_purepy/conversion/__pycache__/abc.cpython-310.pyc
--rw-r--r--   0        0        0     2119 2021-07-14 19:52:47.209081 pg-purepy-0.8.1/src/pg_purepy/conversion/__pycache__/abc.cpython-39.pyc
--rw-r--r--   0        0        0     1071 2022-02-19 03:55:52.870473 pg-purepy-0.8.1/src/pg_purepy/conversion/__pycache__/array_parse.cpython-310.pyc
--rw-r--r--   0        0        0     1073 2021-10-27 01:54:19.905530 pg-purepy-0.8.1/src/pg_purepy/conversion/__pycache__/array_parse.cpython-39.pyc
--rw-r--r--   0        0        0     2121 2022-02-19 03:55:52.870473 pg-purepy-0.8.1/src/pg_purepy/conversion/__pycache__/arrays.cpython-310.pyc
--rw-r--r--   0        0        0     2103 2021-07-14 19:52:47.219080 pg-purepy-0.8.1/src/pg_purepy/conversion/__pycache__/arrays.cpython-39.pyc
--rw-r--r--   0        0        0     3071 2022-02-19 03:55:52.870473 pg-purepy-0.8.1/src/pg_purepy/conversion/__pycache__/basics.cpython-310.pyc
--rw-r--r--   0        0        0     3044 2021-07-14 17:40:29.727817 pg-purepy-0.8.1/src/pg_purepy/conversion/__pycache__/basics.cpython-39.pyc
--rw-r--r--   0        0        0     3329 2022-02-19 03:55:52.873807 pg-purepy-0.8.1/src/pg_purepy/conversion/__pycache__/dt.cpython-310.pyc
--rw-r--r--   0        0        0     3248 2021-07-14 19:52:47.219080 pg-purepy-0.8.1/src/pg_purepy/conversion/__pycache__/dt.cpython-39.pyc
--rw-r--r--   0        0        0     2181 2022-02-19 03:55:52.893807 pg-purepy-0.8.1/src/pg_purepy/conversion/__pycache__/enums.cpython-310.pyc
--rw-r--r--   0        0        0     2107 2021-07-14 02:31:07.635634 pg-purepy-0.8.1/src/pg_purepy/conversion/__pycache__/enums.cpython-39.pyc
--rw-r--r--   0        0        0     1742 2022-02-19 03:55:52.893807 pg-purepy-0.8.1/src/pg_purepy/conversion/__pycache__/hstore.cpython-310.pyc
--rw-r--r--   0        0        0     1676 2021-10-27 01:54:19.925530 pg-purepy-0.8.1/src/pg_purepy/conversion/__pycache__/hstore.cpython-39.pyc
--rw-r--r--   0        0        0     3622 2021-10-27 02:02:24.193406 pg-purepy-0.8.1/src/pg_purepy/conversion/_parse_hstore.py
--rw-r--r--   0        0        0     1567 2021-07-14 19:42:37.122921 pg-purepy-0.8.1/src/pg_purepy/conversion/abc.py
--rw-r--r--   0        0        0     3038 2021-10-27 01:41:42.214344 pg-purepy-0.8.1/src/pg_purepy/conversion/array_parse.py
--rw-r--r--   0        0        0     1429 2021-07-14 19:52:43.762461 pg-purepy-0.8.1/src/pg_purepy/conversion/arrays.py
--rw-r--r--   0        0        0     1871 2021-07-14 16:18:43.130899 pg-purepy-0.8.1/src/pg_purepy/conversion/basics.py
--rw-r--r--   0        0        0     3388 2021-07-14 19:24:00.107881 pg-purepy-0.8.1/src/pg_purepy/conversion/dt.py
--rw-r--r--   0        0        0     1930 2021-07-14 01:56:00.928320 pg-purepy-0.8.1/src/pg_purepy/conversion/enums.py
--rw-r--r--   0        0        0     1084 2021-10-27 01:53:13.272387 pg-purepy-0.8.1/src/pg_purepy/conversion/hstore.py
--rw-r--r--   0        0        0     4753 2021-07-03 00:30:47.252046 pg-purepy-0.8.1/src/pg_purepy/dbapi.py
--rw-r--r--   0        0        0     1290 2021-07-14 01:07:18.445621 pg-purepy-0.8.1/src/pg_purepy/exc.py
--rw-r--r--   0        0        0    11074 2022-02-19 05:30:55.714863 pg-purepy-0.8.1/src/pg_purepy/messages.py
--rw-r--r--   0        0        0    14358 2022-04-20 23:01:13.939549 pg-purepy-0.8.1/src/pg_purepy/pool.py
--rw-r--r--   0        0        0    45859 2022-02-19 05:30:40.501695 pg-purepy-0.8.1/src/pg_purepy/protocol.py
--rw-r--r--   0        0        0     2199 2022-02-19 04:37:01.003832 pg-purepy-0.8.1/src/pg_purepy/util.py
--rw-r--r--   0        0        0     1601 2022-04-20 23:16:05.478836 pg-purepy-0.8.1/setup.py
--rw-r--r--   0        0        0     1764 2022-04-20 23:16:05.479129 pg-purepy-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0      423 2021-07-04 22:53:41.121324 pg_purepy-0.8.2/README.rst
+-rw-r--r--   0        0        0     1436 2023-06-09 03:12:23.047525 pg_purepy-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0      733 2022-03-22 12:12:13.790523 pg_purepy-0.8.2/src/pg_purepy/__init__.py
+-rw-r--r--   0        0        0    20260 2022-03-22 12:12:05.497249 pg_purepy-0.8.2/src/pg_purepy/connection.py
+-rw-r--r--   0        0        0     2986 2021-10-27 01:45:23.945806 pg_purepy-0.8.2/src/pg_purepy/conversion/__init__.py
+-rw-r--r--   0        0        0     2981 2022-02-19 03:55:52.860474 pg_purepy-0.8.2/src/pg_purepy/conversion/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     4862 2023-06-09 02:41:09.098525 pg_purepy-0.8.2/src/pg_purepy/conversion/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2985 2021-10-27 01:54:19.898864 pg_purepy-0.8.2/src/pg_purepy/conversion/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     2332 2022-02-19 03:55:52.897140 pg_purepy-0.8.2/src/pg_purepy/conversion/__pycache__/_parse_hstore.cpython-310.pyc
+-rw-r--r--   0        0        0     3797 2023-06-09 02:41:09.125192 pg_purepy-0.8.2/src/pg_purepy/conversion/__pycache__/_parse_hstore.cpython-311.pyc
+-rw-r--r--   0        0        0     2314 2021-10-27 11:58:23.491037 pg_purepy-0.8.2/src/pg_purepy/conversion/__pycache__/_parse_hstore.cpython-39.pyc
+-rw-r--r--   0        0        0     2165 2022-02-19 03:55:52.863807 pg_purepy-0.8.2/src/pg_purepy/conversion/__pycache__/abc.cpython-310.pyc
+-rw-r--r--   0        0        0     2722 2023-06-09 02:41:09.098525 pg_purepy-0.8.2/src/pg_purepy/conversion/__pycache__/abc.cpython-311.pyc
+-rw-r--r--   0        0        0     2119 2021-07-14 19:52:47.209081 pg_purepy-0.8.2/src/pg_purepy/conversion/__pycache__/abc.cpython-39.pyc
+-rw-r--r--   0        0        0     1071 2022-02-19 03:55:52.870473 pg_purepy-0.8.2/src/pg_purepy/conversion/__pycache__/array_parse.cpython-310.pyc
+-rw-r--r--   0        0        0     2225 2023-06-09 02:41:09.105192 pg_purepy-0.8.2/src/pg_purepy/conversion/__pycache__/array_parse.cpython-311.pyc
+-rw-r--r--   0        0        0     1073 2021-10-27 01:54:19.905530 pg_purepy-0.8.2/src/pg_purepy/conversion/__pycache__/array_parse.cpython-39.pyc
+-rw-r--r--   0        0        0     2121 2022-02-19 03:55:52.870473 pg_purepy-0.8.2/src/pg_purepy/conversion/__pycache__/arrays.cpython-310.pyc
+-rw-r--r--   0        0        0     2975 2023-06-09 02:41:09.105192 pg_purepy-0.8.2/src/pg_purepy/conversion/__pycache__/arrays.cpython-311.pyc
+-rw-r--r--   0        0        0     2103 2021-07-14 19:52:47.219080 pg_purepy-0.8.2/src/pg_purepy/conversion/__pycache__/arrays.cpython-39.pyc
+-rw-r--r--   0        0        0     3071 2022-02-19 03:55:52.870473 pg_purepy-0.8.2/src/pg_purepy/conversion/__pycache__/basics.cpython-310.pyc
+-rw-r--r--   0        0        0     4172 2023-06-09 02:41:09.105192 pg_purepy-0.8.2/src/pg_purepy/conversion/__pycache__/basics.cpython-311.pyc
+-rw-r--r--   0        0        0     3044 2021-07-14 17:40:29.727817 pg_purepy-0.8.2/src/pg_purepy/conversion/__pycache__/basics.cpython-39.pyc
+-rw-r--r--   0        0        0     3329 2022-02-19 03:55:52.873807 pg_purepy-0.8.2/src/pg_purepy/conversion/__pycache__/dt.cpython-310.pyc
+-rw-r--r--   0        0        0     4704 2023-06-09 02:41:09.105192 pg_purepy-0.8.2/src/pg_purepy/conversion/__pycache__/dt.cpython-311.pyc
+-rw-r--r--   0        0        0     3248 2021-07-14 19:52:47.219080 pg_purepy-0.8.2/src/pg_purepy/conversion/__pycache__/dt.cpython-39.pyc
+-rw-r--r--   0        0        0     2181 2022-02-19 03:55:52.893807 pg_purepy-0.8.2/src/pg_purepy/conversion/__pycache__/enums.cpython-310.pyc
+-rw-r--r--   0        0        0     2874 2023-06-09 02:41:09.121858 pg_purepy-0.8.2/src/pg_purepy/conversion/__pycache__/enums.cpython-311.pyc
+-rw-r--r--   0        0        0     2107 2021-07-14 02:31:07.635634 pg_purepy-0.8.2/src/pg_purepy/conversion/__pycache__/enums.cpython-39.pyc
+-rw-r--r--   0        0        0     1742 2022-02-19 03:55:52.893807 pg_purepy-0.8.2/src/pg_purepy/conversion/__pycache__/hstore.cpython-310.pyc
+-rw-r--r--   0        0        0     2283 2023-06-09 02:41:09.125192 pg_purepy-0.8.2/src/pg_purepy/conversion/__pycache__/hstore.cpython-311.pyc
+-rw-r--r--   0        0        0     1676 2021-10-27 01:54:19.925530 pg_purepy-0.8.2/src/pg_purepy/conversion/__pycache__/hstore.cpython-39.pyc
+-rw-r--r--   0        0        0     3622 2021-10-27 02:02:24.193406 pg_purepy-0.8.2/src/pg_purepy/conversion/_parse_hstore.py
+-rw-r--r--   0        0        0     1567 2021-07-14 19:42:37.122921 pg_purepy-0.8.2/src/pg_purepy/conversion/abc.py
+-rw-r--r--   0        0        0     3038 2021-10-27 01:41:42.214344 pg_purepy-0.8.2/src/pg_purepy/conversion/array_parse.py
+-rw-r--r--   0        0        0     1429 2021-07-14 19:52:43.762461 pg_purepy-0.8.2/src/pg_purepy/conversion/arrays.py
+-rw-r--r--   0        0        0     1871 2021-07-14 16:18:43.130899 pg_purepy-0.8.2/src/pg_purepy/conversion/basics.py
+-rw-r--r--   0        0        0     3388 2021-07-14 19:24:00.107881 pg_purepy-0.8.2/src/pg_purepy/conversion/dt.py
+-rw-r--r--   0        0        0     1930 2021-07-14 01:56:00.928320 pg_purepy-0.8.2/src/pg_purepy/conversion/enums.py
+-rw-r--r--   0        0        0     1084 2021-10-27 01:53:13.272387 pg_purepy-0.8.2/src/pg_purepy/conversion/hstore.py
+-rw-r--r--   0        0        0     4753 2021-07-03 00:30:47.252046 pg_purepy-0.8.2/src/pg_purepy/dbapi.py
+-rw-r--r--   0        0        0     1290 2021-07-14 01:07:18.445621 pg_purepy-0.8.2/src/pg_purepy/exc.py
+-rw-r--r--   0        0        0    11074 2022-02-19 05:30:55.714863 pg_purepy-0.8.2/src/pg_purepy/messages.py
+-rw-r--r--   0        0        0    14358 2022-04-20 23:01:13.939549 pg_purepy-0.8.2/src/pg_purepy/pool.py
+-rw-r--r--   0        0        0    45859 2022-02-19 05:30:40.501695 pg_purepy-0.8.2/src/pg_purepy/protocol.py
+-rw-r--r--   0        0        0     2199 2022-02-19 04:37:01.003832 pg_purepy-0.8.2/src/pg_purepy/util.py
+-rw-r--r--   0        0        0     1296 1970-01-01 00:00:00.000000 pg_purepy-0.8.2/PKG-INFO
```

### Comparing `pg-purepy-0.8.1/src/pg_purepy/__init__.py` & `pg_purepy-0.8.2/src/pg_purepy/__init__.py`

 * *Files identical despite different names*

### Comparing `pg-purepy-0.8.1/src/pg_purepy/connection.py` & `pg_purepy-0.8.2/src/pg_purepy/connection.py`

 * *Files identical despite different names*

### Comparing `pg-purepy-0.8.1/src/pg_purepy/conversion/__init__.py` & `pg_purepy-0.8.2/src/pg_purepy/conversion/__init__.py`

 * *Files identical despite different names*

### Comparing `pg-purepy-0.8.1/src/pg_purepy/conversion/__pycache__/__init__.cpython-310.pyc` & `pg_purepy-0.8.2/src/pg_purepy/conversion/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pg-purepy-0.8.1/src/pg_purepy/conversion/__pycache__/__init__.cpython-39.pyc` & `pg_purepy-0.8.2/src/pg_purepy/conversion/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pg-purepy-0.8.1/src/pg_purepy/conversion/__pycache__/_parse_hstore.cpython-310.pyc` & `pg_purepy-0.8.2/src/pg_purepy/conversion/__pycache__/_parse_hstore.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pg-purepy-0.8.1/src/pg_purepy/conversion/__pycache__/_parse_hstore.cpython-39.pyc` & `pg_purepy-0.8.2/src/pg_purepy/conversion/__pycache__/_parse_hstore.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pg-purepy-0.8.1/src/pg_purepy/conversion/__pycache__/abc.cpython-310.pyc` & `pg_purepy-0.8.2/src/pg_purepy/conversion/__pycache__/abc.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pg-purepy-0.8.1/src/pg_purepy/conversion/__pycache__/abc.cpython-39.pyc` & `pg_purepy-0.8.2/src/pg_purepy/conversion/__pycache__/abc.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pg-purepy-0.8.1/src/pg_purepy/conversion/__pycache__/array_parse.cpython-310.pyc` & `pg_purepy-0.8.2/src/pg_purepy/conversion/__pycache__/array_parse.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pg-purepy-0.8.1/src/pg_purepy/conversion/__pycache__/array_parse.cpython-39.pyc` & `pg_purepy-0.8.2/src/pg_purepy/conversion/__pycache__/array_parse.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pg-purepy-0.8.1/src/pg_purepy/conversion/__pycache__/arrays.cpython-310.pyc` & `pg_purepy-0.8.2/src/pg_purepy/conversion/__pycache__/arrays.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pg-purepy-0.8.1/src/pg_purepy/conversion/__pycache__/arrays.cpython-39.pyc` & `pg_purepy-0.8.2/src/pg_purepy/conversion/__pycache__/arrays.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pg-purepy-0.8.1/src/pg_purepy/conversion/__pycache__/basics.cpython-310.pyc` & `pg_purepy-0.8.2/src/pg_purepy/conversion/__pycache__/basics.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pg-purepy-0.8.1/src/pg_purepy/conversion/__pycache__/basics.cpython-39.pyc` & `pg_purepy-0.8.2/src/pg_purepy/conversion/__pycache__/basics.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pg-purepy-0.8.1/src/pg_purepy/conversion/__pycache__/dt.cpython-310.pyc` & `pg_purepy-0.8.2/src/pg_purepy/conversion/__pycache__/dt.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pg-purepy-0.8.1/src/pg_purepy/conversion/__pycache__/dt.cpython-39.pyc` & `pg_purepy-0.8.2/src/pg_purepy/conversion/__pycache__/dt.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pg-purepy-0.8.1/src/pg_purepy/conversion/__pycache__/enums.cpython-310.pyc` & `pg_purepy-0.8.2/src/pg_purepy/conversion/__pycache__/enums.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pg-purepy-0.8.1/src/pg_purepy/conversion/__pycache__/enums.cpython-39.pyc` & `pg_purepy-0.8.2/src/pg_purepy/conversion/__pycache__/enums.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pg-purepy-0.8.1/src/pg_purepy/conversion/__pycache__/hstore.cpython-310.pyc` & `pg_purepy-0.8.2/src/pg_purepy/conversion/__pycache__/hstore.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pg-purepy-0.8.1/src/pg_purepy/conversion/__pycache__/hstore.cpython-39.pyc` & `pg_purepy-0.8.2/src/pg_purepy/conversion/__pycache__/hstore.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pg-purepy-0.8.1/src/pg_purepy/conversion/_parse_hstore.py` & `pg_purepy-0.8.2/src/pg_purepy/conversion/_parse_hstore.py`

 * *Files identical despite different names*

### Comparing `pg-purepy-0.8.1/src/pg_purepy/conversion/abc.py` & `pg_purepy-0.8.2/src/pg_purepy/conversion/abc.py`

 * *Files identical despite different names*

### Comparing `pg-purepy-0.8.1/src/pg_purepy/conversion/array_parse.py` & `pg_purepy-0.8.2/src/pg_purepy/conversion/array_parse.py`

 * *Files identical despite different names*

### Comparing `pg-purepy-0.8.1/src/pg_purepy/conversion/arrays.py` & `pg_purepy-0.8.2/src/pg_purepy/conversion/arrays.py`

 * *Files identical despite different names*

### Comparing `pg-purepy-0.8.1/src/pg_purepy/conversion/basics.py` & `pg_purepy-0.8.2/src/pg_purepy/conversion/basics.py`

 * *Files identical despite different names*

### Comparing `pg-purepy-0.8.1/src/pg_purepy/conversion/dt.py` & `pg_purepy-0.8.2/src/pg_purepy/conversion/dt.py`

 * *Files identical despite different names*

### Comparing `pg-purepy-0.8.1/src/pg_purepy/conversion/enums.py` & `pg_purepy-0.8.2/src/pg_purepy/conversion/enums.py`

 * *Files identical despite different names*

### Comparing `pg-purepy-0.8.1/src/pg_purepy/conversion/hstore.py` & `pg_purepy-0.8.2/src/pg_purepy/conversion/hstore.py`

 * *Files identical despite different names*

### Comparing `pg-purepy-0.8.1/src/pg_purepy/dbapi.py` & `pg_purepy-0.8.2/src/pg_purepy/dbapi.py`

 * *Files identical despite different names*

### Comparing `pg-purepy-0.8.1/src/pg_purepy/exc.py` & `pg_purepy-0.8.2/src/pg_purepy/exc.py`

 * *Files identical despite different names*

### Comparing `pg-purepy-0.8.1/src/pg_purepy/messages.py` & `pg_purepy-0.8.2/src/pg_purepy/messages.py`

 * *Files identical despite different names*

### Comparing `pg-purepy-0.8.1/src/pg_purepy/pool.py` & `pg_purepy-0.8.2/src/pg_purepy/pool.py`

 * *Files identical despite different names*

### Comparing `pg-purepy-0.8.1/src/pg_purepy/protocol.py` & `pg_purepy-0.8.2/src/pg_purepy/protocol.py`

 * *Files identical despite different names*

### Comparing `pg-purepy-0.8.1/src/pg_purepy/util.py` & `pg_purepy-0.8.2/src/pg_purepy/util.py`

 * *Files identical despite different names*

### Comparing `pg-purepy-0.8.1/PKG-INFO` & `pg_purepy-0.8.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,29 @@
 Metadata-Version: 2.1
 Name: pg-purepy
-Version: 0.8.1
+Version: 0.8.2
 Summary: A pure-Python anyio-based PostgreSQL adapter.
 License: LGPL-3.0-or-later
 Author: Lura Skye
 Author-email: l@veriny.tf
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Database
 Classifier: Topic :: Database :: Front-Ends
 Provides-Extra: docs
-Requires-Dist: Sphinx (>=3.0,<4.0); extra == "docs"
-Requires-Dist: anyio (>=3.5.0,<4.0.0)
-Requires-Dist: arrow (>=1.2.2,<2.0.0)
-Requires-Dist: async_generator (>=1.10,<2.0); python_version < "3.10"
-Requires-Dist: attrs (>=21.4.0,<22.0.0)
+Requires-Dist: anyio (==3.6.2)
+Requires-Dist: arrow (>=1.2.3,<2.0.0)
+Requires-Dist: attrs (>=23.1.0,<24.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
-Requires-Dist: scramp (>=1.4.1,<2.0.0)
-Requires-Dist: sphinx-autodoc-typehints (>=1.12.0,<2.0.0); extra == "docs"
-Requires-Dist: sphinx-inline-tabs (>=2021.4.11-beta.9,<2022.0.0); extra == "docs"
-Requires-Dist: sphinx-rtd-theme (>=0.5.2,<0.6.0); extra == "docs"
-Requires-Dist: sphinxcontrib-trio (>=1.1.2,<2.0.0); extra == "docs"
+Requires-Dist: scramp (>=1.4.4,<2.0.0)
 Description-Content-Type: text/x-rst
 
 pg-purepy
 =========
 
 .. image:: https://img.shields.io/pypi/pyversions/pg-purepy?style=flat-square
     :alt: PyPI - Python Version
```

