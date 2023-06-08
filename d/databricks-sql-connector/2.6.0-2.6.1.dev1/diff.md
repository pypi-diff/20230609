# Comparing `tmp/databricks_sql_connector-2.6.0.tar.gz` & `tmp/databricks_sql_connector-2.6.1.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databricks_sql_connector-2.6.0.tar", max compression
+gzip compressed data, was "databricks_sql_connector-2.6.1.dev1.tar", max compression
```

## Comparing `databricks_sql_connector-2.6.0.tar` & `databricks_sql_connector-2.6.1.dev1.tar`

### file list

```diff
@@ -1,30 +1,32 @@
--rw-r--r--   0        0        0     4320 2023-06-07 22:24:49.881864 databricks_sql_connector-2.6.0/CHANGELOG.md
--rw-r--r--   0        0        0    11346 2023-06-07 22:24:49.881864 databricks_sql_connector-2.6.0/LICENSE
--rw-r--r--   0        0        0     2723 2023-06-07 22:24:49.881864 databricks_sql_connector-2.6.0/README.md
--rw-r--r--   0        0        0     1417 2023-06-07 22:25:18.463320 databricks_sql_connector-2.6.0/pyproject.toml
--rw-r--r--   0        0        0      295 2023-06-07 22:24:49.881864 databricks_sql_connector-2.6.0/src/databricks/__init__.py
--rw-r--r--   0        0        0     1269 2023-06-07 22:24:49.881864 databricks_sql_connector-2.6.0/src/databricks/sql/__init__.py
--rw-r--r--   0        0        0        0 2023-06-07 22:24:49.881864 databricks_sql_connector-2.6.0/src/databricks/sql/auth/__init__.py
--rw-r--r--   0        0        0     3894 2023-06-07 22:24:49.881864 databricks_sql_connector-2.6.0/src/databricks/sql/auth/auth.py
--rw-r--r--   0        0        0     5493 2023-06-07 22:24:49.881864 databricks_sql_connector-2.6.0/src/databricks/sql/auth/authenticators.py
--rw-r--r--   0        0        0     9717 2023-06-07 22:24:49.881864 databricks_sql_connector-2.6.0/src/databricks/sql/auth/oauth.py
--rw-r--r--   0        0        0     1201 2023-06-07 22:24:49.881864 databricks_sql_connector-2.6.0/src/databricks/sql/auth/oauth_http_handler.py
--rw-r--r--   0        0        0     5900 2023-06-07 22:24:49.881864 databricks_sql_connector-2.6.0/src/databricks/sql/auth/thrift_http_client.py
--rw-r--r--   0        0        0    36862 2023-06-07 22:24:49.881864 databricks_sql_connector-2.6.0/src/databricks/sql/client.py
--rw-r--r--   0        0        0     2423 2023-06-07 22:24:49.881864 databricks_sql_connector-2.6.0/src/databricks/sql/exc.py
--rw-r--r--   0        0        0        0 2023-06-07 22:24:49.881864 databricks_sql_connector-2.6.0/src/databricks/sql/experimental/__init__.py
--rw-r--r--   0        0        0     2236 2023-06-07 22:24:49.881864 databricks_sql_connector-2.6.0/src/databricks/sql/experimental/oauth_persistence.py
--rwxr-xr-x   0        0        0     8062 2023-06-07 22:24:49.881864 databricks_sql_connector-2.6.0/src/databricks/sql/thrift_api/TCLIService/TCLIService-remote
--rw-r--r--   0        0        0   136849 2023-06-07 22:24:49.881864 databricks_sql_connector-2.6.0/src/databricks/sql/thrift_api/TCLIService/TCLIService.py
--rw-r--r--   0        0        0       49 2023-06-07 22:24:49.881864 databricks_sql_connector-2.6.0/src/databricks/sql/thrift_api/TCLIService/__init__.py
--rw-r--r--   0        0        0     1307 2023-06-07 22:24:49.881864 databricks_sql_connector-2.6.0/src/databricks/sql/thrift_api/TCLIService/constants.py
--rw-r--r--   0        0        0  2077276 2023-06-07 22:24:49.889865 databricks_sql_connector-2.6.0/src/databricks/sql/thrift_api/TCLIService/ttypes.py
--rw-r--r--   0        0        0        0 2023-06-07 22:24:49.889865 databricks_sql_connector-2.6.0/src/databricks/sql/thrift_api/__init__.py
--rw-r--r--   0        0        0    41308 2023-06-07 22:24:49.889865 databricks_sql_connector-2.6.0/src/databricks/sql/thrift_backend.py
--rw-r--r--   0        0        0     6771 2023-06-07 22:24:49.889865 databricks_sql_connector-2.6.0/src/databricks/sql/types.py
--rw-r--r--   0        0        0     6646 2023-06-07 22:24:49.889865 databricks_sql_connector-2.6.0/src/databricks/sql/utils.py
--rw-r--r--   0        0        0       60 2023-06-07 22:24:49.889865 databricks_sql_connector-2.6.0/src/databricks/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     9761 2023-06-07 22:24:49.889865 databricks_sql_connector-2.6.0/src/databricks/sqlalchemy/dialect/__init__.py
--rw-r--r--   0        0        0      494 2023-06-07 22:24:49.889865 databricks_sql_connector-2.6.0/src/databricks/sqlalchemy/dialect/base.py
--rw-r--r--   0        0        0      792 2023-06-07 22:24:49.889865 databricks_sql_connector-2.6.0/src/databricks/sqlalchemy/dialect/compiler.py
--rw-r--r--   0        0        0     4107 1970-01-01 00:00:00.000000 databricks_sql_connector-2.6.0/PKG-INFO
+-rw-r--r--   0        0        0     4392 2023-06-08 21:31:02.291524 databricks_sql_connector-2.6.1.dev1/CHANGELOG.md
+-rw-r--r--   0        0        0    11346 2022-07-01 15:51:10.712635 databricks_sql_connector-2.6.1.dev1/LICENSE
+-rw-r--r--   0        0        0     2723 2023-04-14 18:34:59.049677 databricks_sql_connector-2.6.1.dev1/README.md
+-rw-r--r--   0        0        0     1422 2023-06-08 21:30:06.565778 databricks_sql_connector-2.6.1.dev1/pyproject.toml
+-rw-r--r--   0        0        0      295 2023-04-14 18:34:59.055358 databricks_sql_connector-2.6.1.dev1/src/databricks/__init__.py
+-rw-r--r--   0        0        0     1274 2023-06-08 21:30:14.033060 databricks_sql_connector-2.6.1.dev1/src/databricks/sql/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-03 16:24:58.334788 databricks_sql_connector-2.6.1.dev1/src/databricks/sql/auth/__init__.py
+-rw-r--r--   0        0        0     3894 2023-04-14 18:35:15.931583 databricks_sql_connector-2.6.1.dev1/src/databricks/sql/auth/auth.py
+-rw-r--r--   0        0        0     5493 2023-04-14 18:35:15.932289 databricks_sql_connector-2.6.1.dev1/src/databricks/sql/auth/authenticators.py
+-rw-r--r--   0        0        0     9717 2023-05-15 19:51:43.874759 databricks_sql_connector-2.6.1.dev1/src/databricks/sql/auth/oauth.py
+-rw-r--r--   0        0        0     1201 2022-10-03 16:24:58.337383 databricks_sql_connector-2.6.1.dev1/src/databricks/sql/auth/oauth_http_handler.py
+-rw-r--r--   0        0        0     5949 2023-06-08 21:27:39.900632 databricks_sql_connector-2.6.1.dev1/src/databricks/sql/auth/thrift_http_client.py
+-rw-r--r--   0        0        0     7398 2023-06-06 18:22:07.351264 databricks_sql_connector-2.6.1.dev1/src/databricks/sql/auth/thrift_http_client_base.py
+-rw-r--r--   0        0        0    36862 2023-04-14 18:34:59.057965 databricks_sql_connector-2.6.1.dev1/src/databricks/sql/client.py
+-rw-r--r--   0        0        0     2423 2023-04-15 04:06:26.706720 databricks_sql_connector-2.6.1.dev1/src/databricks/sql/exc.py
+-rw-r--r--   0        0        0        0 2022-10-03 16:24:58.338569 databricks_sql_connector-2.6.1.dev1/src/databricks/sql/experimental/__init__.py
+-rw-r--r--   0        0        0     2236 2022-10-03 16:24:58.339078 databricks_sql_connector-2.6.1.dev1/src/databricks/sql/experimental/oauth_persistence.py
+-rwxr-xr-x   0        0        0     8062 2023-02-17 22:37:09.888185 databricks_sql_connector-2.6.1.dev1/src/databricks/sql/thrift_api/TCLIService/TCLIService-remote
+-rw-r--r--   0        0        0   136849 2023-02-17 22:37:09.888959 databricks_sql_connector-2.6.1.dev1/src/databricks/sql/thrift_api/TCLIService/TCLIService.py
+-rw-r--r--   0        0        0       49 2022-10-27 13:27:23.168192 databricks_sql_connector-2.6.1.dev1/src/databricks/sql/thrift_api/TCLIService/__init__.py
+-rw-r--r--   0        0        0     1307 2023-02-17 22:37:09.889536 databricks_sql_connector-2.6.1.dev1/src/databricks/sql/thrift_api/TCLIService/constants.py
+-rw-r--r--   0        0        0  2077276 2023-02-17 22:37:09.894769 databricks_sql_connector-2.6.1.dev1/src/databricks/sql/thrift_api/TCLIService/ttypes.py
+-rw-r--r--   0        0        0        0 2022-07-01 15:51:10.721377 databricks_sql_connector-2.6.1.dev1/src/databricks/sql/thrift_api/__init__.py
+-rw-r--r--   0        0        0    41308 2023-06-07 22:14:21.044846 databricks_sql_connector-2.6.1.dev1/src/databricks/sql/thrift_backend.py
+-rw-r--r--   0        0        0     6771 2022-07-01 15:51:10.722149 databricks_sql_connector-2.6.1.dev1/src/databricks/sql/types.py
+-rw-r--r--   0        0        0     6646 2023-04-14 18:34:59.058795 databricks_sql_connector-2.6.1.dev1/src/databricks/sql/utils.py
+-rw-r--r--   0        0        0       60 2023-04-14 18:34:59.059517 databricks_sql_connector-2.6.1.dev1/src/databricks/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     9761 2023-05-24 19:08:38.516515 databricks_sql_connector-2.6.1.dev1/src/databricks/sqlalchemy/dialect/__init__.py
+-rw-r--r--   0        0        0      494 2023-04-14 18:34:59.061408 databricks_sql_connector-2.6.1.dev1/src/databricks/sqlalchemy/dialect/base.py
+-rw-r--r--   0        0        0      792 2023-05-24 19:03:23.969272 databricks_sql_connector-2.6.1.dev1/src/databricks/sqlalchemy/dialect/compiler.py
+-rw-r--r--   0        0        0     4377 1970-01-01 00:00:00.000000 databricks_sql_connector-2.6.1.dev1/setup.py
+-rw-r--r--   0        0        0     4108 1970-01-01 00:00:00.000000 databricks_sql_connector-2.6.1.dev1/PKG-INFO
```

### Comparing `databricks_sql_connector-2.6.0/CHANGELOG.md` & `databricks_sql_connector-2.6.1.dev1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # Release History
 
 ## 2.6.x (Unreleased)
 
+- Fix: http.client would raise a BadStatusLine exception in some cases
+
 ## 2.6.0 (2023-06-07)
 
 - Add support for HTTP 1.1 connections (connection pools)
 - Add a default socket timeout for thrift RPCs
 
 ## 2.5.2 (2023-05-08)
```

### Comparing `databricks_sql_connector-2.6.0/LICENSE` & `databricks_sql_connector-2.6.1.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.6.0/README.md` & `databricks_sql_connector-2.6.1.dev1/README.md`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.6.0/pyproject.toml` & `databricks_sql_connector-2.6.1.dev1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "databricks-sql-connector"
-version = "2.6.0"
+version = "2.6.1.dev1"
 description = "Databricks SQL Connector for Python"
 authors = ["Databricks <databricks-sql-connector-maintainers@databricks.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "databricks", from = "src"}]
 include = ["CHANGELOG.md"]
```

### Comparing `databricks_sql_connector-2.6.0/src/databricks/sql/__init__.py` & `databricks_sql_connector-2.6.1.dev1/src/databricks/sql/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 NUMBER = DBAPITypeObject(
     "boolean", "tinyint", "smallint", "int", "bigint", "float", "double", "decimal"
 )
 DATETIME = DBAPITypeObject("timestamp")
 DATE = DBAPITypeObject("date")
 ROWID = DBAPITypeObject()
 
-__version__ = "2.6.0"
+__version__ = "2.6.1.dev1"
 USER_AGENT_NAME = "PyDatabricksSqlConnector"
 
 # These two functions are pyhive legacy
 Date = datetime.date
 Timestamp = datetime.datetime
```

### Comparing `databricks_sql_connector-2.6.0/src/databricks/sql/auth/auth.py` & `databricks_sql_connector-2.6.1.dev1/src/databricks/sql/auth/auth.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.6.0/src/databricks/sql/auth/authenticators.py` & `databricks_sql_connector-2.6.1.dev1/src/databricks/sql/auth/authenticators.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.6.0/src/databricks/sql/auth/oauth.py` & `databricks_sql_connector-2.6.1.dev1/src/databricks/sql/auth/oauth.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.6.0/src/databricks/sql/auth/oauth_http_handler.py` & `databricks_sql_connector-2.6.1.dev1/src/databricks/sql/auth/oauth_http_handler.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.6.0/src/databricks/sql/auth/thrift_http_client.py` & `databricks_sql_connector-2.6.1.dev1/src/databricks/sql/auth/thrift_http_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,14 +111,15 @@
             self.__pool = proxy_manager.connection_from_host(
                 self.host, self.port, pool_kwargs=_pool_kwargs
             )
         else:
             self.__pool = pool_class(self.host, self.port, **_pool_kwargs)
 
     def close(self):
+        self.__resp and self.__resp.drain_conn()
         self.__resp and self.__resp.release_conn()
         self.__resp = None
 
     def read(self, sz):
         return self.__resp.read(sz)
 
     def isOpen(self):
```

### Comparing `databricks_sql_connector-2.6.0/src/databricks/sql/client.py` & `databricks_sql_connector-2.6.1.dev1/src/databricks/sql/client.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.6.0/src/databricks/sql/exc.py` & `databricks_sql_connector-2.6.1.dev1/src/databricks/sql/exc.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.6.0/src/databricks/sql/experimental/oauth_persistence.py` & `databricks_sql_connector-2.6.1.dev1/src/databricks/sql/experimental/oauth_persistence.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.6.0/src/databricks/sql/thrift_api/TCLIService/TCLIService-remote` & `databricks_sql_connector-2.6.1.dev1/src/databricks/sql/thrift_api/TCLIService/TCLIService-remote`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.6.0/src/databricks/sql/thrift_api/TCLIService/TCLIService.py` & `databricks_sql_connector-2.6.1.dev1/src/databricks/sql/thrift_api/TCLIService/TCLIService.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.6.0/src/databricks/sql/thrift_api/TCLIService/constants.py` & `databricks_sql_connector-2.6.1.dev1/src/databricks/sql/thrift_api/TCLIService/constants.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.6.0/src/databricks/sql/thrift_api/TCLIService/ttypes.py` & `databricks_sql_connector-2.6.1.dev1/src/databricks/sql/thrift_api/TCLIService/ttypes.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.6.0/src/databricks/sql/thrift_backend.py` & `databricks_sql_connector-2.6.1.dev1/src/databricks/sql/thrift_backend.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.6.0/src/databricks/sql/types.py` & `databricks_sql_connector-2.6.1.dev1/src/databricks/sql/types.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.6.0/src/databricks/sql/utils.py` & `databricks_sql_connector-2.6.1.dev1/src/databricks/sql/utils.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.6.0/src/databricks/sqlalchemy/dialect/__init__.py` & `databricks_sql_connector-2.6.1.dev1/src/databricks/sqlalchemy/dialect/__init__.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.6.0/src/databricks/sqlalchemy/dialect/compiler.py` & `databricks_sql_connector-2.6.1.dev1/src/databricks/sqlalchemy/dialect/compiler.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.6.0/PKG-INFO` & `databricks_sql_connector-2.6.1.dev1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: databricks-sql-connector
-Version: 2.6.0
+Version: 2.6.1.dev1
 Summary: Databricks SQL Connector for Python
 License: Apache-2.0
 Author: Databricks
 Author-email: databricks-sql-connector-maintainers@databricks.com
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: alembic (>=1.0.11,<2.0.0)
 Requires-Dist: lz4 (>=4.0.2,<5.0.0)
-Requires-Dist: numpy (>=1.16.6) ; python_version >= "3.7" and python_version < "3.11"
-Requires-Dist: numpy (>=1.23.4) ; python_version >= "3.11"
+Requires-Dist: numpy (>=1.16.6); python_version >= "3.7" and python_version < "3.11"
+Requires-Dist: numpy (>=1.23.4); python_version >= "3.11"
 Requires-Dist: oauthlib (>=3.1.0,<4.0.0)
 Requires-Dist: openpyxl (>=3.0.10,<4.0.0)
 Requires-Dist: pandas (>=1.2.5,<2.0.0)
-Requires-Dist: pyarrow (>=10.0.1) ; python_version >= "3.11"
-Requires-Dist: pyarrow (>=6.0.0) ; python_version >= "3.7" and python_version < "3.11"
+Requires-Dist: pyarrow (>=10.0.1); python_version >= "3.11"
+Requires-Dist: pyarrow (>=6.0.0); python_version >= "3.7" and python_version < "3.11"
 Requires-Dist: requests (>=2.18.1,<3.0.0)
 Requires-Dist: sqlalchemy (>=1.3.24,<2.0.0)
 Requires-Dist: thrift (>=0.16.0,<0.17.0)
 Project-URL: Bug Tracker, https://github.com/databricks/databricks-sql-python/issues
 Project-URL: Homepage, https://github.com/databricks/databricks-sql-python
 Description-Content-Type: text/markdown
```

