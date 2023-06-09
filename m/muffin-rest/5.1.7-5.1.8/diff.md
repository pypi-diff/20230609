# Comparing `tmp/muffin_rest-5.1.7.tar.gz` & `tmp/muffin_rest-5.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muffin_rest-5.1.7.tar", max compression
+gzip compressed data, was "muffin_rest-5.1.8.tar", max compression
```

## Comparing `muffin_rest-5.1.7.tar` & `muffin_rest-5.1.8.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1082 2023-06-08 16:17:17.413749 muffin_rest-5.1.7/LICENSE
--rw-r--r--   0        0        0     2616 2023-06-08 16:17:17.413749 muffin_rest-5.1.7/README.rst
--rw-r--r--   0        0        0     1242 2023-06-08 16:17:17.413749 muffin_rest-5.1.7/muffin_rest/__init__.py
--rw-r--r--   0        0        0     3882 2023-06-08 16:17:17.413749 muffin_rest-5.1.7/muffin_rest/api.py
--rw-r--r--   0        0        0     1169 2023-06-08 16:17:17.413749 muffin_rest-5.1.7/muffin_rest/errors.py
--rw-r--r--   0        0        0     5164 2023-06-08 16:17:17.413749 muffin_rest-5.1.7/muffin_rest/filters.py
--rw-r--r--   0        0        0    10762 2023-06-08 16:17:17.413749 muffin_rest-5.1.7/muffin_rest/handler.py
--rw-r--r--   0        0        0     4805 2023-06-08 16:17:17.413749 muffin_rest-5.1.7/muffin_rest/mongo/__init__.py
--rw-r--r--   0        0        0      921 2023-06-08 16:17:17.413749 muffin_rest-5.1.7/muffin_rest/mongo/filters.py
--rw-r--r--   0        0        0     1205 2023-06-08 16:17:17.413749 muffin_rest-5.1.7/muffin_rest/mongo/schema.py
--rw-r--r--   0        0        0      870 2023-06-08 16:17:17.413749 muffin_rest-5.1.7/muffin_rest/mongo/sorting.py
--rw-r--r--   0        0        0      206 2023-06-08 16:17:17.413749 muffin_rest-5.1.7/muffin_rest/mongo/types.py
--rw-r--r--   0        0        0     3946 2023-06-08 16:17:17.413749 muffin_rest-5.1.7/muffin_rest/mongo/utils.py
--rw-r--r--   0        0        0     8770 2023-06-08 16:17:17.413749 muffin_rest-5.1.7/muffin_rest/openapi.py
--rw-r--r--   0        0        0     1927 2023-06-08 16:17:17.413749 muffin_rest-5.1.7/muffin_rest/options.py
--rw-r--r--   0        0        0      129 2023-06-08 16:17:17.413749 muffin_rest-5.1.7/muffin_rest/peewee/__init__.py
--rw-r--r--   0        0        0     2332 2023-06-08 16:17:17.413749 muffin_rest-5.1.7/muffin_rest/peewee/filters.py
--rw-r--r--   0        0        0     5378 2023-06-08 16:17:17.413749 muffin_rest-5.1.7/muffin_rest/peewee/handler.py
--rw-r--r--   0        0        0     1111 2023-06-08 16:17:17.413749 muffin_rest-5.1.7/muffin_rest/peewee/openapi.py
--rw-r--r--   0        0        0     1489 2023-06-08 16:17:17.413749 muffin_rest-5.1.7/muffin_rest/peewee/options.py
--rw-r--r--   0        0        0     1076 2023-06-08 16:17:17.413749 muffin_rest-5.1.7/muffin_rest/peewee/schemas.py
--rw-r--r--   0        0        0     1895 2023-06-08 16:17:17.413749 muffin_rest-5.1.7/muffin_rest/peewee/sorting.py
--rw-r--r--   0        0        0      155 2023-06-08 16:17:17.413749 muffin_rest-5.1.7/muffin_rest/peewee/types.py
--rw-r--r--   0        0        0      702 2023-06-08 16:17:17.413749 muffin_rest-5.1.7/muffin_rest/peewee/utils.py
--rw-r--r--   0        0        0        0 2023-06-08 16:17:17.413749 muffin_rest-5.1.7/muffin_rest/py.typed
--rw-r--r--   0        0        0      559 2023-06-08 16:17:17.413749 muffin_rest-5.1.7/muffin_rest/redoc.html
--rw-r--r--   0        0        0     2803 2023-06-08 16:17:17.413749 muffin_rest-5.1.7/muffin_rest/sorting.py
--rw-r--r--   0        0        0     6514 2023-06-08 16:17:17.413749 muffin_rest-5.1.7/muffin_rest/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     2460 2023-06-08 16:17:17.413749 muffin_rest-5.1.7/muffin_rest/sqlalchemy/filters.py
--rw-r--r--   0        0        0     1643 2023-06-08 16:17:17.413749 muffin_rest-5.1.7/muffin_rest/sqlalchemy/sorting.py
--rw-r--r--   0        0        0      204 2023-06-08 16:17:17.413749 muffin_rest-5.1.7/muffin_rest/sqlalchemy/types.py
--rw-r--r--   0        0        0     1736 2023-06-08 16:17:17.413749 muffin_rest-5.1.7/muffin_rest/swagger.html
--rw-r--r--   0        0        0      521 2023-06-08 16:17:17.413749 muffin_rest-5.1.7/muffin_rest/types.py
--rw-r--r--   0        0        0     2059 2023-06-08 16:17:17.413749 muffin_rest-5.1.7/muffin_rest/utils.py
--rw-r--r--   0        0        0     2826 2023-06-08 16:17:17.413749 muffin_rest-5.1.7/pyproject.toml
--rw-r--r--   0        0        0     4126 1970-01-01 00:00:00.000000 muffin_rest-5.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-06-09 07:45:32.141040 muffin_rest-5.1.8/LICENSE
+-rw-r--r--   0        0        0     2616 2023-06-09 07:45:32.141040 muffin_rest-5.1.8/README.rst
+-rw-r--r--   0        0        0     1242 2023-06-09 07:45:32.141040 muffin_rest-5.1.8/muffin_rest/__init__.py
+-rw-r--r--   0        0        0     3882 2023-06-09 07:45:32.141040 muffin_rest-5.1.8/muffin_rest/api.py
+-rw-r--r--   0        0        0     1169 2023-06-09 07:45:32.141040 muffin_rest-5.1.8/muffin_rest/errors.py
+-rw-r--r--   0        0        0     5164 2023-06-09 07:45:32.141040 muffin_rest-5.1.8/muffin_rest/filters.py
+-rw-r--r--   0        0        0    10762 2023-06-09 07:45:32.141040 muffin_rest-5.1.8/muffin_rest/handler.py
+-rw-r--r--   0        0        0     4805 2023-06-09 07:45:32.141040 muffin_rest-5.1.8/muffin_rest/mongo/__init__.py
+-rw-r--r--   0        0        0      921 2023-06-09 07:45:32.141040 muffin_rest-5.1.8/muffin_rest/mongo/filters.py
+-rw-r--r--   0        0        0     1205 2023-06-09 07:45:32.141040 muffin_rest-5.1.8/muffin_rest/mongo/schema.py
+-rw-r--r--   0        0        0      870 2023-06-09 07:45:32.141040 muffin_rest-5.1.8/muffin_rest/mongo/sorting.py
+-rw-r--r--   0        0        0      206 2023-06-09 07:45:32.141040 muffin_rest-5.1.8/muffin_rest/mongo/types.py
+-rw-r--r--   0        0        0     3946 2023-06-09 07:45:32.141040 muffin_rest-5.1.8/muffin_rest/mongo/utils.py
+-rw-r--r--   0        0        0     8770 2023-06-09 07:45:32.141040 muffin_rest-5.1.8/muffin_rest/openapi.py
+-rw-r--r--   0        0        0     1927 2023-06-09 07:45:32.141040 muffin_rest-5.1.8/muffin_rest/options.py
+-rw-r--r--   0        0        0      129 2023-06-09 07:45:32.145040 muffin_rest-5.1.8/muffin_rest/peewee/__init__.py
+-rw-r--r--   0        0        0     2332 2023-06-09 07:45:32.145040 muffin_rest-5.1.8/muffin_rest/peewee/filters.py
+-rw-r--r--   0        0        0     5378 2023-06-09 07:45:32.145040 muffin_rest-5.1.8/muffin_rest/peewee/handler.py
+-rw-r--r--   0        0        0     1111 2023-06-09 07:45:32.145040 muffin_rest-5.1.8/muffin_rest/peewee/openapi.py
+-rw-r--r--   0        0        0     1489 2023-06-09 07:45:32.145040 muffin_rest-5.1.8/muffin_rest/peewee/options.py
+-rw-r--r--   0        0        0     1215 2023-06-09 07:45:32.145040 muffin_rest-5.1.8/muffin_rest/peewee/schemas.py
+-rw-r--r--   0        0        0     1895 2023-06-09 07:45:32.145040 muffin_rest-5.1.8/muffin_rest/peewee/sorting.py
+-rw-r--r--   0        0        0      155 2023-06-09 07:45:32.145040 muffin_rest-5.1.8/muffin_rest/peewee/types.py
+-rw-r--r--   0        0        0      702 2023-06-09 07:45:32.145040 muffin_rest-5.1.8/muffin_rest/peewee/utils.py
+-rw-r--r--   0        0        0        0 2023-06-09 07:45:32.145040 muffin_rest-5.1.8/muffin_rest/py.typed
+-rw-r--r--   0        0        0      559 2023-06-09 07:45:32.145040 muffin_rest-5.1.8/muffin_rest/redoc.html
+-rw-r--r--   0        0        0     2803 2023-06-09 07:45:32.145040 muffin_rest-5.1.8/muffin_rest/sorting.py
+-rw-r--r--   0        0        0     6514 2023-06-09 07:45:32.145040 muffin_rest-5.1.8/muffin_rest/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     2460 2023-06-09 07:45:32.145040 muffin_rest-5.1.8/muffin_rest/sqlalchemy/filters.py
+-rw-r--r--   0        0        0     1643 2023-06-09 07:45:32.145040 muffin_rest-5.1.8/muffin_rest/sqlalchemy/sorting.py
+-rw-r--r--   0        0        0      204 2023-06-09 07:45:32.145040 muffin_rest-5.1.8/muffin_rest/sqlalchemy/types.py
+-rw-r--r--   0        0        0     1736 2023-06-09 07:45:32.145040 muffin_rest-5.1.8/muffin_rest/swagger.html
+-rw-r--r--   0        0        0      521 2023-06-09 07:45:32.145040 muffin_rest-5.1.8/muffin_rest/types.py
+-rw-r--r--   0        0        0     2059 2023-06-09 07:45:32.145040 muffin_rest-5.1.8/muffin_rest/utils.py
+-rw-r--r--   0        0        0     2826 2023-06-09 07:45:32.145040 muffin_rest-5.1.8/pyproject.toml
+-rw-r--r--   0        0        0     4126 1970-01-01 00:00:00.000000 muffin_rest-5.1.8/PKG-INFO
```

### Comparing `muffin_rest-5.1.7/LICENSE` & `muffin_rest-5.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.7/README.rst` & `muffin_rest-5.1.8/README.rst`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.7/muffin_rest/__init__.py` & `muffin_rest-5.1.8/muffin_rest/__init__.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.7/muffin_rest/api.py` & `muffin_rest-5.1.8/muffin_rest/api.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.7/muffin_rest/errors.py` & `muffin_rest-5.1.8/muffin_rest/errors.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.7/muffin_rest/filters.py` & `muffin_rest-5.1.8/muffin_rest/filters.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.7/muffin_rest/handler.py` & `muffin_rest-5.1.8/muffin_rest/handler.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.7/muffin_rest/mongo/__init__.py` & `muffin_rest-5.1.8/muffin_rest/mongo/__init__.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.7/muffin_rest/mongo/filters.py` & `muffin_rest-5.1.8/muffin_rest/mongo/filters.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.7/muffin_rest/mongo/schema.py` & `muffin_rest-5.1.8/muffin_rest/mongo/schema.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.7/muffin_rest/mongo/sorting.py` & `muffin_rest-5.1.8/muffin_rest/mongo/sorting.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.7/muffin_rest/mongo/utils.py` & `muffin_rest-5.1.8/muffin_rest/mongo/utils.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.7/muffin_rest/openapi.py` & `muffin_rest-5.1.8/muffin_rest/openapi.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.7/muffin_rest/options.py` & `muffin_rest-5.1.8/muffin_rest/options.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.7/muffin_rest/peewee/filters.py` & `muffin_rest-5.1.8/muffin_rest/peewee/filters.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.7/muffin_rest/peewee/handler.py` & `muffin_rest-5.1.8/muffin_rest/peewee/handler.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.7/muffin_rest/peewee/openapi.py` & `muffin_rest-5.1.8/muffin_rest/peewee/openapi.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.7/muffin_rest/peewee/options.py` & `muffin_rest-5.1.8/muffin_rest/peewee/options.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.7/muffin_rest/peewee/schemas.py` & `muffin_rest-5.1.8/muffin_rest/peewee/schemas.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,15 +13,18 @@
         self.choices_text = ", ".join([str(c.value) for c in enum])
         super().__init__(**kwargs)
 
     def _serialize(self, value, attr, obj, **kwargs):
         if value is None:
             return None
 
-        return value.value
+        try:
+            return value.value
+        except AttributeError:
+            raise ma.ValidationError(f"{obj}: {attr} value is invalid: {value}") from None
 
     def _deserialize(self, value, attr, data, **kwargs):
         try:
             return self.enum(value)
         except ValueError as error:
             raise self.make_error("unknown", choices=self.choices_text) from error
```

### Comparing `muffin_rest-5.1.7/muffin_rest/peewee/sorting.py` & `muffin_rest-5.1.8/muffin_rest/peewee/sorting.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.7/muffin_rest/peewee/utils.py` & `muffin_rest-5.1.8/muffin_rest/peewee/utils.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.7/muffin_rest/redoc.html` & `muffin_rest-5.1.8/muffin_rest/redoc.html`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.7/muffin_rest/sorting.py` & `muffin_rest-5.1.8/muffin_rest/sorting.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.7/muffin_rest/sqlalchemy/__init__.py` & `muffin_rest-5.1.8/muffin_rest/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.7/muffin_rest/sqlalchemy/filters.py` & `muffin_rest-5.1.8/muffin_rest/sqlalchemy/filters.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.7/muffin_rest/sqlalchemy/sorting.py` & `muffin_rest-5.1.8/muffin_rest/sqlalchemy/sorting.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.7/muffin_rest/swagger.html` & `muffin_rest-5.1.8/muffin_rest/swagger.html`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.7/muffin_rest/types.py` & `muffin_rest-5.1.8/muffin_rest/types.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.7/muffin_rest/utils.py` & `muffin_rest-5.1.8/muffin_rest/utils.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.7/pyproject.toml` & `muffin_rest-5.1.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "muffin-rest"
-version = "5.1.7"
+version = "5.1.8"
 description = "The package provides enhanced support for writing REST APIs with Muffin framework"
 readme = "README.rst"
 homepage = "https://github.com/klen/muffin-rest"
 repository = "https://github.com/klen/muffin-rest"
 authors = ["Kirill Klenov <horneds@gmail.com>"]
 license = "MIT"
 keywords = ["rest", "api", "muffin", "asgi", "asyncio", "trio"]
```

### Comparing `muffin_rest-5.1.7/PKG-INFO` & `muffin_rest-5.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muffin-rest
-Version: 5.1.7
+Version: 5.1.8
 Summary: The package provides enhanced support for writing REST APIs with Muffin framework
 Home-page: https://github.com/klen/muffin-rest
 License: MIT
 Keywords: rest,api,muffin,asgi,asyncio,trio
 Author: Kirill Klenov
 Author-email: horneds@gmail.com
 Requires-Python: >=3.8,<4.0
```

