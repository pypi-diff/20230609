# Comparing `tmp/GeneralSQL-1.0.5.tar.gz` & `tmp/GeneralSQL-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GeneralSQL-1.0.5.tar", last modified: Thu Dec  8 05:46:10 2022, max compression
+gzip compressed data, was "GeneralSQL-1.0.6.tar", last modified: Fri Jun  9 12:01:14 2023, max compression
```

## Comparing `GeneralSQL-1.0.5.tar` & `GeneralSQL-1.0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 joker     (1000) joker     (1000)        0 2022-12-08 05:46:10.634922 GeneralSQL-1.0.5/
-drwxr-xr-x   0 joker     (1000) joker     (1000)        0 2022-12-08 05:46:10.634922 GeneralSQL-1.0.5/GeneralSQL/
--rw-r--r--   0 joker     (1000) joker     (1000)     2321 2022-11-05 22:52:08.000000 GeneralSQL-1.0.5/GeneralSQL/Error.py
-drwxr-xr-x   0 joker     (1000) joker     (1000)        0 2022-12-08 05:46:10.634922 GeneralSQL-1.0.5/GeneralSQL/Template/
--rw-r--r--   0 joker     (1000) joker     (1000)     1435 2022-11-05 22:52:08.000000 GeneralSQL-1.0.5/GeneralSQL/Template/__init__.py
--rw-r--r--   0 joker     (1000) joker     (1000)     3023 2022-11-05 22:52:08.000000 GeneralSQL-1.0.5/GeneralSQL/Template/base.py
--rw-r--r--   0 joker     (1000) joker     (1000)     2212 2022-12-08 05:41:37.000000 GeneralSQL-1.0.5/GeneralSQL/__init__.py
-drwxr-xr-x   0 joker     (1000) joker     (1000)        0 2022-12-08 05:46:10.634922 GeneralSQL-1.0.5/GeneralSQL/db/
--rw-r--r--   0 joker     (1000) joker     (1000)    14674 2022-12-08 05:41:13.000000 GeneralSQL-1.0.5/GeneralSQL/db/Jmysql.py
--rw-r--r--   0 joker     (1000) joker     (1000)       57 2022-11-05 22:52:08.000000 GeneralSQL-1.0.5/GeneralSQL/db/__init__.py
-drwxr-xr-x   0 joker     (1000) joker     (1000)        0 2022-12-08 05:46:10.634922 GeneralSQL-1.0.5/GeneralSQL.egg-info/
--rw-r--r--   0 joker     (1000) joker     (1000)     3487 2022-12-08 05:46:10.000000 GeneralSQL-1.0.5/GeneralSQL.egg-info/PKG-INFO
--rw-r--r--   0 joker     (1000) joker     (1000)      321 2022-12-08 05:46:10.000000 GeneralSQL-1.0.5/GeneralSQL.egg-info/SOURCES.txt
--rw-r--r--   0 joker     (1000) joker     (1000)        1 2022-12-08 05:46:10.000000 GeneralSQL-1.0.5/GeneralSQL.egg-info/dependency_links.txt
--rw-r--r--   0 joker     (1000) joker     (1000)       11 2022-12-08 05:46:10.000000 GeneralSQL-1.0.5/GeneralSQL.egg-info/top_level.txt
--rwxrwxrwx   0 joker     (1000) joker     (1000)    35149 2022-11-01 13:18:35.000000 GeneralSQL-1.0.5/LICENSE
--rw-r--r--   0 joker     (1000) joker     (1000)     3487 2022-12-08 05:46:10.634922 GeneralSQL-1.0.5/PKG-INFO
--rw-r--r--   0 joker     (1000) joker     (1000)     2967 2022-11-05 22:52:08.000000 GeneralSQL-1.0.5/README.md
--rwxrwxrwx   0 joker     (1000) joker     (1000)      510 2022-12-08 05:42:05.000000 GeneralSQL-1.0.5/pyproject.toml
--rw-r--r--   0 joker     (1000) joker     (1000)       38 2022-12-08 05:46:10.634922 GeneralSQL-1.0.5/setup.cfg
+drwxr-xr-x   0 joker     (1000) joker     (1000)        0 2023-06-09 12:01:14.561737 GeneralSQL-1.0.6/
+drwxr-xr-x   0 joker     (1000) joker     (1000)        0 2023-06-09 12:01:14.561737 GeneralSQL-1.0.6/GeneralSQL/
+-rw-r--r--   0 joker     (1000) joker     (1000)     2321 2022-12-18 15:36:05.000000 GeneralSQL-1.0.6/GeneralSQL/Error.py
+drwxr-xr-x   0 joker     (1000) joker     (1000)        0 2023-06-09 12:01:14.561737 GeneralSQL-1.0.6/GeneralSQL/Template/
+-rw-r--r--   0 joker     (1000) joker     (1000)     1431 2023-06-09 10:46:01.000000 GeneralSQL-1.0.6/GeneralSQL/Template/__init__.py
+-rw-r--r--   0 joker     (1000) joker     (1000)     3024 2023-06-09 10:45:33.000000 GeneralSQL-1.0.6/GeneralSQL/Template/base.py
+-rw-r--r--   0 joker     (1000) joker     (1000)     2155 2023-06-09 11:56:15.000000 GeneralSQL-1.0.6/GeneralSQL/__init__.py
+drwxr-xr-x   0 joker     (1000) joker     (1000)        0 2023-06-09 12:01:14.561737 GeneralSQL-1.0.6/GeneralSQL/db/
+-rw-r--r--   0 joker     (1000) joker     (1000)    14741 2023-06-09 11:16:08.000000 GeneralSQL-1.0.6/GeneralSQL/db/Jmysql.py
+-rw-r--r--   0 joker     (1000) joker     (1000)       57 2022-12-18 15:36:05.000000 GeneralSQL-1.0.6/GeneralSQL/db/__init__.py
+drwxr-xr-x   0 joker     (1000) joker     (1000)        0 2023-06-09 12:01:14.561737 GeneralSQL-1.0.6/GeneralSQL.egg-info/
+-rw-r--r--   0 joker     (1000) joker     (1000)      750 2023-06-09 12:01:14.000000 GeneralSQL-1.0.6/GeneralSQL.egg-info/PKG-INFO
+-rw-r--r--   0 joker     (1000) joker     (1000)      321 2023-06-09 12:01:14.000000 GeneralSQL-1.0.6/GeneralSQL.egg-info/SOURCES.txt
+-rw-r--r--   0 joker     (1000) joker     (1000)        1 2023-06-09 12:01:14.000000 GeneralSQL-1.0.6/GeneralSQL.egg-info/dependency_links.txt
+-rw-r--r--   0 joker     (1000) joker     (1000)       11 2023-06-09 12:01:14.000000 GeneralSQL-1.0.6/GeneralSQL.egg-info/top_level.txt
+-rwxr-xr-x   0 joker     (1000) joker     (1000)    35149 2022-12-18 15:40:21.000000 GeneralSQL-1.0.6/LICENSE
+-rw-r--r--   0 joker     (1000) joker     (1000)      750 2023-06-09 12:01:14.561737 GeneralSQL-1.0.6/PKG-INFO
+-rw-r--r--   0 joker     (1000) joker     (1000)      230 2022-12-18 16:34:16.000000 GeneralSQL-1.0.6/README.md
+-rwxr-xr-x   0 joker     (1000) joker     (1000)      510 2023-06-09 04:52:15.000000 GeneralSQL-1.0.6/pyproject.toml
+-rw-r--r--   0 joker     (1000) joker     (1000)       38 2023-06-09 12:01:14.561737 GeneralSQL-1.0.6/setup.cfg
```

### Comparing `GeneralSQL-1.0.5/GeneralSQL/Error.py` & `GeneralSQL-1.0.6/GeneralSQL/Error.py`

 * *Files identical despite different names*

### Comparing `GeneralSQL-1.0.5/GeneralSQL/Template/__init__.py` & `GeneralSQL-1.0.6/GeneralSQL/Template/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         JI.__init__(self)
         Sql.__init__(self)
         self.set_type('affairs')
         self.table = table
         self.data = data
 
     def data_decode(self): raise NotImplementedError
-    
+
     def format_sql(self): raise NotImplementedError
 
 class TUpdate(JU, Sql):
 
     def __init__(self, table, data:dict):
         JU.__init__(self)
         Sql.__init__(self)
```

### Comparing `GeneralSQL-1.0.5/GeneralSQL/Template/base.py` & `GeneralSQL-1.0.6/GeneralSQL/Template/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 
 
 class Sql:
     """Sql 数据类型
     """
 
     def __init__(self):
-        # type: query/affairs
+        # type: query/ affairs
         self.__type = None
         self.__value = None
 
     def get_sql(self):
         return self.__value
     
     def set_sql(self, v):
```

### Comparing `GeneralSQL-1.0.5/GeneralSQL/__init__.py` & `GeneralSQL-1.0.6/GeneralSQL/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import importlib
 import functools
 from . import db
 
-__version__ = '1.0.5'
+__version__ = '1.0.6'
 
 __cls__ = db.__all__
 
 
 def SeniorDB(t):
     if t in __cls__:
         __db = getattr(db, t).DB
@@ -45,17 +45,14 @@
             self.func = 'Select'
 
         def __run_class_func(func):
             @functools.wraps(func)
             def f(self, *args, **kwargs):
                 return getattr(getattr(pack, self.func), func.__name__)(self, *args, **kwargs)
             return f
-
-        @__run_class_func
-        def get_sql(self):...
         
         @__run_class_func
         def set_join(self, *args, **kwargs):...
 
         @__run_class_func
         def set_where(self, *args, **kwargs):...
```

### Comparing `GeneralSQL-1.0.5/GeneralSQL/db/Jmysql.py` & `GeneralSQL-1.0.6/GeneralSQL/db/Jmysql.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,29 +53,29 @@
             if symbol.upper() == 'IN':
                 if filter_data.get('not'):
                     symbol = 'NOT IN'
                 result = f"{field} {symbol} ({','.join([repr(str(i)) for i in val])})"
             elif symbol.upper() == 'LIKE':
                 if filter_data.get('not'):
                     symbol = 'NOT LIKE'
-                result = f"{field} {symbol} {str(val)}"
+                result = f"{field} {symbol} {repr(str(val))}"
             elif symbol.upper() == 'ISNULL':
                 symbol = 'IS NULL'
                 if filter_data.get('not'):
                     symbol = 'IS NOT NULL'
                 result = f'{field} {symbol}'
             elif symbol.upper() == 'BETWEEN':
                 if filter_data.get('not'):
                     symbol = 'NOT BETWEEN'
-                result = f"{field} {symbol} {val.get('start')} AND {val.get('end')}"
+                result = f'{field} {symbol} {repr(val.get("start"))} AND {repr(val.get("end"))}'
                 if filter_data.get('not'):
-                    symbol = 'NOT LIKE'
-                result = f'{field} {symbol} {str(val)}'
+                    symbol = 'NOT BETWEEN'
+                result = f'{field} {symbol} {repr(val.get("start"))} AND {repr(val.get("end"))}'
             else:
-                result = f'{field} {symbol} {val}'
+                result = f'{field} {symbol} {repr(val)}'
                 if filter_data.get('not'):
                     result = f'NOT {result}'
             # 关系
             if factor := filter_data.get('factor'):
                 if factor.upper() in ['AND', 'OR']:
                     result = f'{factor.upper()} {result}'
                 else:
@@ -228,52 +228,52 @@
             if isinstance(self.data, dict):
                 self.value = [f'`{k}` = {repr(v)}' for k, v in self.data.items()]
             else:
                 raise Error.ParamsError(400001)
         else:
             raise Error.UseError(200002)
 
-    def format_sql(self):
-        self.data_decode()
-        str_data = ','.join(self.value)
-        sql = f'{self.__base[0]} {self.table} {self.__base[1]} {str_data}'
-        if self.where:
-            sql = f'{sql} {self.where}'
-        self.set_sql(sql)
-
     def set_where(self, *filters):
         if len(filters) > 0:
             self.where = []
             for i in filters:
                 self.where.append(_filter_format(i))
             self.where = f'WHERE {" ".join(self.where)}'
         else:
             raise Error.ParamsError(400002)
 
+    def format_sql(self):
+        self.data_decode()
+        str_data = ','.join(self.value)
+        sql = f'{self.__base[0]} {self.table} {self.__base[1]} {str_data}'
+        if self.where:
+            sql = f'{sql} {self.where}'
+        self.set_sql(sql)
+
 class Delete(TDelete):
 
     def __init__(self, table):
         TDelete.__init__(self, table)
         self.__base = ['DELETE FROM']
 
-    def format_sql(self):
-        sql = f'{self.__base[0]} {self.table}'
-        if self.where:
-            sql = f'{sql} {self.where}'
-        self.set_sql(sql)
-
     def set_where(self, *filters):
         if len(filters) > 0:
             self.where = []
             for i in filters:
                 self.where.append(_filter_format(i))
             self.where = f'WHERE {" ".join(self.where)}'
         else:
             raise Error.ParamsError(400002)
 
+    def format_sql(self):
+        sql = f'{self.__base[0]} {self.table}'
+        if self.where:
+            sql = f'{sql} {self.where}'
+        self.set_sql(sql)
+
 class Select(TSelect):
 
     def __init__(self, **kwargs):
         TSelect.__init__(self, **kwargs)
         self.__base = ['SELECT', 'FROM']
         if kwargs.get('fields'):
             if isinstance(kwargs.get('fields'), (list, tuple, dict)):
@@ -283,15 +283,14 @@
 
     def set_fields(self, *fields):
         if len(fields) < 1:
             raise Error.ParamsError(400002)
         for i in fields:
             self.fields = _format_field(i)
 
-
     # 设置条件
     def set_where(self, *filters):
         if len(filters) > 0:
             self.where = []
             for i in filters:
                 self.where.append(_filter_format(i))
             self.where = f'WHERE {" ".join(self.where)}'
```

### Comparing `GeneralSQL-1.0.5/LICENSE` & `GeneralSQL-1.0.6/LICENSE`

 * *Files identical despite different names*

