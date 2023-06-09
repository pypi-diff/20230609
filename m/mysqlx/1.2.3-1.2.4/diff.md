# Comparing `tmp/mysqlx-1.2.3.tar.gz` & `tmp/mysqlx-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mysqlx-1.2.3.tar", last modified: Thu Jun  8 15:09:45 2023, max compression
+gzip compressed data, was "dist\mysqlx-1.2.4.tar", last modified: Fri Jun  9 07:20:24 2023, max compression
```

## Comparing `mysqlx-1.2.3.tar` & `mysqlx-1.2.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 15:09:45.000000 mysqlx-1.2.3/
--rw-rw-rw-   0        0        0    11558 2021-11-30 10:47:21.000000 mysqlx-1.2.3/LICENSE
-drwxrwxrwx   0        0        0        0 2023-06-08 15:09:45.000000 mysqlx-1.2.3/mysqlx/
--rw-rw-rw-   0        0        0     5708 2023-06-08 15:08:36.000000 mysqlx-1.2.3/mysqlx/coder.py
--rw-rw-rw-   0        0        0     1433 2023-06-08 14:55:57.000000 mysqlx-1.2.3/mysqlx/coder.tpl
--rw-rw-rw-   0        0        0    10185 2023-06-07 12:34:06.000000 mysqlx-1.2.3/mysqlx/db.py
--rw-rw-rw-   0        0        0     3370 2023-06-06 00:29:56.000000 mysqlx-1.2.3/mysqlx/dbx.py
--rw-rw-rw-   0        0        0     5295 2023-06-06 23:27:22.000000 mysqlx-1.2.3/mysqlx/helper.py
--rw-rw-rw-   0        0        0    11033 2023-06-07 14:35:41.000000 mysqlx-1.2.3/mysqlx/orm.py
--rw-rw-rw-   0        0        0        0 2021-11-30 12:54:44.000000 mysqlx-1.2.3/mysqlx/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-08 15:09:45.000000 mysqlx-1.2.3/mysqlx.egg-info/
--rw-rw-rw-   0        0        0        1 2023-06-08 15:09:45.000000 mysqlx-1.2.3/mysqlx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-06 08:06:39.000000 mysqlx-1.2.3/mysqlx.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      404 2023-06-08 15:09:45.000000 mysqlx-1.2.3/mysqlx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       45 2023-06-08 15:09:45.000000 mysqlx-1.2.3/mysqlx.egg-info/requires.txt
--rw-rw-rw-   0        0        0      314 2023-06-08 15:09:45.000000 mysqlx-1.2.3/mysqlx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2023-06-08 15:09:45.000000 mysqlx-1.2.3/mysqlx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      404 2023-06-08 15:09:45.000000 mysqlx-1.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     2598 2023-06-06 12:09:45.000000 mysqlx-1.2.3/README.md
--rw-rw-rw-   0        0        0       42 2023-06-08 15:09:45.000000 mysqlx-1.2.3/setup.cfg
--rw-rw-rw-   0        0        0      816 2023-06-08 15:09:31.000000 mysqlx-1.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 07:20:24.000000 mysqlx-1.2.4/
+-rw-rw-rw-   0        0        0    11558 2021-11-30 10:47:21.000000 mysqlx-1.2.4/LICENSE
+drwxrwxrwx   0        0        0        0 2023-06-09 07:20:24.000000 mysqlx-1.2.4/mysqlx/
+-rw-rw-rw-   0        0        0     5989 2023-06-09 01:21:35.000000 mysqlx-1.2.4/mysqlx/coder.py
+-rw-rw-rw-   0        0        0     1589 2023-06-09 01:09:35.000000 mysqlx-1.2.4/mysqlx/coder.tpl
+-rw-rw-rw-   0        0        0    10185 2023-06-07 12:34:06.000000 mysqlx-1.2.4/mysqlx/db.py
+-rw-rw-rw-   0        0        0     3370 2023-06-06 00:29:56.000000 mysqlx-1.2.4/mysqlx/dbx.py
+-rw-rw-rw-   0        0        0     5295 2023-06-06 23:27:22.000000 mysqlx-1.2.4/mysqlx/helper.py
+-rw-rw-rw-   0        0        0    10862 2023-06-09 07:16:35.000000 mysqlx-1.2.4/mysqlx/orm.py
+-rw-rw-rw-   0        0        0        0 2021-11-30 12:54:44.000000 mysqlx-1.2.4/mysqlx/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 07:20:24.000000 mysqlx-1.2.4/mysqlx.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-06-09 07:20:24.000000 mysqlx-1.2.4/mysqlx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-06 08:06:39.000000 mysqlx-1.2.4/mysqlx.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      404 2023-06-09 07:20:24.000000 mysqlx-1.2.4/mysqlx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       45 2023-06-09 07:20:24.000000 mysqlx-1.2.4/mysqlx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      314 2023-06-09 07:20:24.000000 mysqlx-1.2.4/mysqlx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2023-06-09 07:20:24.000000 mysqlx-1.2.4/mysqlx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      404 2023-06-09 07:20:24.000000 mysqlx-1.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2598 2023-06-06 12:09:45.000000 mysqlx-1.2.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-09 07:20:24.000000 mysqlx-1.2.4/setup.cfg
+-rw-rw-rw-   0        0        0      816 2023-06-09 07:20:09.000000 mysqlx-1.2.4/setup.py
```

### Comparing `mysqlx-1.2.3/LICENSE` & `mysqlx-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mysqlx-1.2.3/mysqlx/coder.py` & `mysqlx-1.2.4/mysqlx/coder.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,22 +26,25 @@
 
     def generate_with_tables(self, tables: Union[str, Iterable[str]], path: str = None, common_cols=['create_by', 'create_time'],
                              attributes={'__pk__': 'id', '__update_by__': 'update_by', '__update_time__': 'update_time', '__del_flag__': 'del_flag'}):
         metas = None
         only_one_table = False
 
         columns = [v for v in attributes.values()]
-        common_cols.reverse()
-        for i in range(0, 2):
-            columns.insert(1, common_cols[i])
-
-        # 去重
-        base_columns = list(set(columns))
-        # 保持原有顺序
-        base_columns.sort(key=columns.index)
+        if common_cols:
+            common_cols.reverse()
+            for i in range(0, len(common_cols)):
+                columns.insert(1, common_cols[i])
+
+            # 去重
+            base_columns = list(set(columns))
+            # 保持原有顺序
+            base_columns.sort(key=columns.index)
+        else:
+            base_columns = columns
 
         if isinstance(tables, str):
             if self.comma1 in tables:
                 tables = tables.split(self.comma1)
             elif self.comma2 in tables:
                 tables = tables.split(self.comma2)
             else:
@@ -87,22 +90,26 @@
         for col in columns:
             if col['COLUMN_KEY'] == 'PRI':
                 pk = col['COLUMN_NAME']
 
             if col['COLUMN_NAME'] in base_columns:
                 super_columns.append(col)
 
-            if col['DATA_TYPE'] in ('tinyint', 'bigint'):
+            if col['DATA_TYPE'] in ('int', 'tinyint', 'bigint'):
                 col['DATA_TYPE'] = 'int'
-            elif col['DATA_TYPE'] == 'double':
+            elif col['DATA_TYPE'] in ('float', 'double'):
                 col['DATA_TYPE'] = 'float'
             elif col['DATA_TYPE'] == 'decimal':
                 col['DATA_TYPE'] = 'Decimal'
             elif col['DATA_TYPE'] in ('char', 'varchar', 'text'):
                 col['DATA_TYPE'] = 'str'
+            elif col['DATA_TYPE'] in ('date', 'datetime'):
+                pass
+            else:
+                col['DATA_TYPE'] = 'None'
 
         if pk is None:
             return table
 
         class_name = self._get_class_name(table)
         return {
             'pk': pk,
```

### Comparing `mysqlx-1.2.3/mysqlx/coder.tpl` & `mysqlx-1.2.4/mysqlx/coder.tpl`

 * *Files 11% similar despite different names*

```diff
@@ -13,12 +13,12 @@
         self.{{item.COLUMN_NAME}} = {{item.COLUMN_NAME}} {% endfor %}
 
 {% for meta in metas %}
 class {{meta.class_name}}(BaseModel):{% if meta.pk != __pk__ %}
     __pk__ = '{{meta.pk}}'{% endif %}
     __table__ = '{{meta.table}}'
 
-    def __init__(self,{% for item in meta.columns %}{% if loop.last %} {{item.COLUMN_NAME}}: {{item.DATA_TYPE}} = None{% else %} {{item.COLUMN_NAME}}: {{item.DATA_TYPE}} = None,{% endif %}{% endfor %}):
+    def __init__(self,{% for item in meta.columns %}{% if loop.last %}{% if item.DATA_TYPE=='None' %} {{item.COLUMN_NAME}}=None{% else %} {{item.COLUMN_NAME}}: {{item.DATA_TYPE}} = None{% endif %}{% else %}{% if item.DATA_TYPE=='None' %} {{item.COLUMN_NAME}}=None{% else %} {{item.COLUMN_NAME}}: {{item.DATA_TYPE}} = None{% endif %},{% endif %}{% endfor %}):
         super().__init__({% for item in meta.super_columns %}{% if loop.first %}{{item.COLUMN_NAME}}={{item.COLUMN_NAME}}{% else %}, {{item.COLUMN_NAME}}={{item.COLUMN_NAME}}{% endif %}{% endfor %}) {% for item in meta.self_columns %}
         self.{{item.COLUMN_NAME}} = {{item.COLUMN_NAME}} {% endfor %}
 
 {% endfor %}
```

### Comparing `mysqlx-1.2.3/mysqlx/db.py` & `mysqlx-1.2.4/mysqlx/db.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.2.3/mysqlx/dbx.py` & `mysqlx-1.2.4/mysqlx/dbx.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.2.3/mysqlx/helper.py` & `mysqlx-1.2.4/mysqlx/helper.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.2.3/mysqlx/orm.py` & `mysqlx-1.2.4/mysqlx/orm.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,30 +5,46 @@
 SYMBOLS = ['=', '>', '<']
 BETWEEN, LIKE, IN = 'between', 'like', 'in'
 
 
 def _get_condition_arg(k, v):
     if not isinstance(v, str):
         return "`%s`=?" % k, v
+
     v_lower = v.lower()
     if any([symbol in SYMBOLS for symbol in v_lower]):
         return "`%s`%s" % (k, v), None
     elif BETWEEN in v_lower or LIKE in v_lower or IN in v_lower:
         return "`%s` %s" % (k, v), None
     else:
         return "`%s`=?" % k, v
 
 
-def _get_where_args(**kwargs):
+def _get_where_arg_limit(**kwargs):
+    where, args, limit = '', [], 0
+    if 'limit' in kwargs:
+        limit = kwargs.get('limit')
+        del kwargs['limit']
+
     if kwargs:
         conditions, args = zip(*[_get_condition_arg(k, v) for k, v in kwargs.items()])
         args = [arg for arg in args if arg is not None]
         where = 'WHERE %s' % ' and '.join(conditions)
-        return where, args
-    return '', []
+
+    return where, args, limit
+
+
+def _split_ids(ids: Iterable[int], batch_size):
+    ids_size = len(ids)
+    mod = ids_size % batch_size
+    n = ids_size // batch_size
+    if mod != 0:
+        n += 1
+
+    return [ids[i:i + batch_size] for i in range(0, ids_size, batch_size)]
 
 
 class Model:
     def __str__(self):
         kv = {k: v for k, v in self.__dict__.items() if not k.startswith("__")}
         return str(kv)
 
@@ -53,46 +69,39 @@
         pk, table = self._get_pk_and_table()
         kv = {k: v for k, v in self.__dict__.items() if v is not None}
         if pk not in kv:
             raise KeyError("Not primary key.")
 
         update_kv = {k: v for k, v in kv.items() if k != pk}
         if update_kv:
-            cols, args = zip(*update_kv.items())
-            args = [*args, kv[pk]]
-            update_time_col = self._get_update_time_col()
-            if update_time_col is None or update_time_col in update_kv:
-                sql = 'UPDATE `%s` SET %s WHERE `%s`=? limit 1' % (table, ','.join(['`%s`=?' % col for col in cols]), pk)
-            else:
-                sql = 'UPDATE `%s` SET %s, %s=CURRENT_TIMESTAMP WHERE `%s`=? limit 1' % (table, ','.join(['`%s`=?' % col for col in cols]), update_time_col, pk)
-            db.do_execute(sql, *args)
+            self.update_by_id(kv[pk], **update_kv)
 
     def load(self):
-        pk, table = self._get_pk_and_table()
+        pk = self._get_pk()
         kv = self.__dict__
         _id = kv.get(pk)
         if _id is not None:
             cols, _ = zip(*kv.items())
-            sql = 'SELECT %s FROM `%s` WHERE `%s`=? limit 1' % (','.join(['`%s`' % col for col in cols]), table, pk)
-            self.__dict__.update(db.do_select_one(sql, _id))
+            where = 'WHERE `%s`=?' % pk
+            sql = self._select_sql(where, 1, *cols)
+            self.__dict__.update(db.do_select_one(sql, _id, 1))
             return self
         else:
             raise KeyError("Not primary key.")
 
     def delete(self):
-        pk, table = self._get_pk_and_table()
+        pk = self._get_pk()
         _id = self.__dict__.get(pk)
         if _id is None:
             raise KeyError("Not primary key.")
 
-        sql = 'DELETE FROM `%s` WHERE `%s`=? limit 1' % (table, pk)
-        return db.do_execute(sql, _id)
+        return self.delete_by_id(_id)
 
     def logic_delete(self, update_by: int = None):
-        pk, table = self._get_pk_and_table()
+        pk = self._get_pk()
         _id = self.__dict__.get(pk)
         if _id is None:
             raise KeyError("Not primary key.")
 
         return self.logic_delete_by_id(_id, update_by)
 
     @classmethod
@@ -121,152 +130,163 @@
         return [cls._dict2obj(d) for d in cls.select_by_ids(ids, *selection)]
 
     @classmethod
     def select_by_id(cls, id: int, *selection):
         """
         Return one row(dict) or None if no result.
         """
-        pk, table = cls._get_pk_and_table()
-        if len(selection) == 0:
-            sql = 'SELECT * FROM `%s` WHERE `%s`=? limit 1' % (table, pk)
-        else:
-            sql = 'SELECT %s FROM `%s` WHERE `%s`=? limit 1' % (','.join(['`%s`' % col for col in selection]), table, pk)
-        return db.do_select_one(sql, id)
+        pk = cls._get_pk()
+        where = 'WHERE `%s`=?' % pk
+        sql = cls._select_sql(where, 1, *selection)
+        return db.do_select_one(sql, id, 1)
 
     @classmethod
     def select_by_ids(cls, ids: Iterable[int], *selection):
         """
         Return list(dict) or empty list if no result.
         """
         ids_size = len(ids)
         assert ids_size > 0, 'ids must not be empty.'
-        pk, table = cls._get_pk_and_table()
+
+        pk = cls._get_pk()
         ids_str = ','.join(list(map(str, ids)))
-        if len(selection) == 0:
-            sql = 'SELECT * FROM `%s` WHERE `%s` in (%s) limit %d' % (table, pk, ids_str, ids_size)
-        else:
-            sql = 'SELECT %s FROM `%s` WHERE `%s` in (%s) limit %d' % (','.join(['`%s`' % col for col in selection]), table, pk, ids_str, ids_size)
-        return db.do_select(sql)
+        where = 'WHERE `%s` in (%s)' % (pk, ids_str)
+        sql = cls._select_sql(where, ids_size, *selection)
+        return db.do_select(sql, ids_size)
 
     @classmethod
     def update_by_id(cls, id: int, **kwargs):
         assert kwargs, 'Must set update kv'
-        pk, table = cls._get_pk_and_table()
+        pk = cls._get_pk()
+        where = '`%s`=?' % pk
         cols, args = zip(*kwargs.items())
-        args = [*args, id]
-        update_time_col = cls._get_update_time_col()
-        if update_time_col is None or update_time_col in kwargs:
-            sql = 'UPDATE `%s` SET %s WHERE `%s`=? limit 1' % (table, ','.join(['`%s`=?' % col for col in cols]), pk)
-        else:
-            sql = 'UPDATE `%s` SET %s, `%s`=CURRENT_TIMESTAMP WHERE `%s`=? limit 1' % (table, ','.join(['`%s`=?' % col for col in cols]), update_time_col, pk)
-        db.do_execute(sql, *args)
+        sql = cls._update_sql(where, *cols)
+        return db.do_execute(sql, *args, id, 1)
 
     @classmethod
     def delete_by_id(cls, id: int):
         pk, table = cls._get_pk_and_table()
-        sql = 'DELETE FROM `%s` WHERE `%s`=? limit 1' % (table, pk)
-        return db.do_execute(sql, id)
+        sql = 'DELETE FROM `%s` WHERE `%s`=? limit ?' % (table, pk)
+        return db.do_execute(sql, id, 1)
 
     @classmethod
-    def delete_by_ids(cls, ids: Iterable[int]):
+    def delete_by_ids(cls, ids: Iterable[int], batch_size=128):
         ids_size = len(ids)
         assert ids_size > 0, 'ids must not be empty.'
+
+        if ids_size == 1:
+            return cls.delete_by_id(ids[0])
+
+        if ids_size <= batch_size:
+            return cls._delete_by_ids(ids)
+        else:
+            split_ids = _split_ids(ids, batch_size)
+            with db.transaction():
+                results = [cls._delete_by_ids(ids) for ids in split_ids]
+            return sum(results)
+
+    @classmethod
+    def _delete_by_ids(cls, ids: Iterable[int]):
         pk, table = cls._get_pk_and_table()
-        sql = 'DELETE FROM `%s` WHERE `%s` in (%s) limit %d' % (table, pk, ','.join(list(map(str, ids))), ids_size)
-        return db.do_execute(sql)
+        sql = 'DELETE FROM `%s` WHERE `%s` in (%s) limit ?' % (table, pk, ','.join(list(map(str, ids))))
+        return db.do_execute(sql, len(ids))
 
     @classmethod
     def logic_delete_by_id(cls, id: int, update_by: int = None):
         pk, table = cls._get_pk_and_table()
         del_flag_col = cls._get_del_flag_col()
         update_by_col = cls._get_update_by_col()
-        update_time_col = cls._get_update_time_col()
 
-        if update_by is None or update_by_col is None:
-            if update_time_col:
-                sql = 'UPDATE `%s` SET `%s`=?, `%s`=CURRENT_TIMESTAMP WHERE `%s`=? limit 1' % (table, del_flag_col, update_time_col, pk)
-            else:
-                sql = 'UPDATE `%s` SET `%s`=? WHERE `%s`=? limit 1' % (table, del_flag_col, pk)
-            return db.do_execute(sql, 1, id)
+        where = '`%s`=?' % pk
+        limit = 1
+        if update_by is not None and update_by_col is not None:
+            sql = cls._update_sql(where, del_flag_col, update_by_col)
+            return db.do_execute(sql, 1, update_by, id, limit)
         else:
-            if update_time_col:
-                sql = 'UPDATE `%s` SET `%s`=?, `%s`=?, `%s`=CURRENT_TIMESTAMP WHERE `%s`=? limit 1' % (table, del_flag_col, update_by_col, update_time_col, pk)
-            else:
-                sql = 'UPDATE `%s` SET `%s`=?, `%s`=? WHERE `%s`=? limit 1' % (table, del_flag_col, update_by_col, pk)
-            return db.do_execute(sql, 1, update_by, id)
+            sql = cls._update_sql(where, del_flag_col)
+            return db.do_execute(sql, 1, id, limit)
 
     @classmethod
-    def logic_delete_by_ids(cls, ids: Iterable[int], update_by: int = None):
+    def logic_delete_by_ids(cls, ids: Iterable[int], update_by: int = None, batch_size=128):
         ids_size = len(ids)
         assert ids_size > 0, 'ids must not be empty.'
 
-        pk, table = cls._get_pk_and_table()
-        ids_str = ','.join(list(map(str, ids)))
+        if ids_size == 1:
+            return cls.logic_delete_by_id(ids[0], update_by)
+
+        if ids_size <= batch_size:
+            return cls._logic_delete_by_ids(ids, update_by)
+        else:
+            split_ids = _split_ids(ids, batch_size)
+            with db.transaction():
+                results = [cls._logic_delete_by_ids(ids, update_by) for ids in split_ids]
+            return sum(results)
+
+    @classmethod
+    def _logic_delete_by_ids(cls, ids: Iterable[int], update_by: int = None):
+        ids_size = len(ids)
+        pk = cls._get_pk()
         del_flag_col = cls._get_del_flag_col()
         update_by_col = cls._get_update_by_col()
-        update_time_col = cls._get_update_time_col()
 
-        if update_by is None or update_by_col is None:
-            if update_time_col:
-                sql = 'UPDATE `%s` SET `%s`=?, `%s`=CURRENT_TIMESTAMP WHERE `%s` in (%s) limit %d' % (table, del_flag_col, update_time_col, pk, ids_str, ids_size)
-            else:
-                sql = 'UPDATE `%s` SET `%s`=?, WHERE `%s` in (%s) limit %d' % (table, del_flag_col, pk, ids_str, ids_size)
-            return db.execute(sql, 1)
+        ids_str = ','.join(list(map(str, ids)))
+        where = '`%s` in (%s)' % (pk, ids_str)
+        if update_by is not None and update_by_col is not None:
+            sql = cls._update_sql(where, del_flag_col, update_by_col)
+            return db.do_execute(sql, 1, update_by, ids_size)
         else:
-            if update_time_col:
-                sql = 'UPDATE `%s` SET `%s`=?, `%s`=?, `%s`=CURRENT_TIMESTAMP WHERE `%s` in (%s) limit %d' % (table, del_flag_col, update_by_col, update_time_col, pk, ids_str, ids_size)
-            else:
-                sql = 'UPDATE `%s` SET `%s`=?, `%s`=?, WHERE `%s` in (%s) limit %d' % (table, del_flag_col, update_by_col, pk, ids_str, ids_size)
-            return db.do_execute(sql, 1, update_by)
+            sql = cls._update_sql(where, del_flag_col)
+            return db.do_execute(sql, 1, ids_size)
+
+    @classmethod
+    def count(cls, **kwargs):
+        where, args, _ = _get_where_arg_limit(**kwargs)
+        selection = 'count(1)'
+        limit = 1
+        sql = cls._select_sql(where, limit, selection)
+        return db.do_get(sql, *args, limit)
 
     @classmethod
     def find(cls, *selection, **kwargs):
         """
         Return list(object) or empty list if no result.
         """
-        pk, table = cls._get_pk_and_table()
         return [cls._dict2obj(d) for d in cls.select(*selection, **kwargs)]
 
     @classmethod
     def select(cls, *selection, **kwargs):
         """
         Return list(dict) or empty list if no result.
         """
-        where, args = '', []
-        if kwargs:
-            limit = kwargs.get('limit')
-            if limit:
-                del kwargs['limit']
-            where, args = _get_where_args(**kwargs)
-        else:
+        where, args, limit = _get_where_arg_limit(**kwargs)
+        if not limit:
             limit = 1000
 
-        limit_str = 'limit %d' % limit if limit else ''
-        pk, table = cls._get_pk_and_table()
-        if len(selection) == 0:
-            sql = 'SELECT * FROM `%s` %s %s' % (table, where, limit_str)
-        else:
-            sql = 'SELECT %s FROM `%s` %s %s' % (','.join(['`%s`' % col for col in selection]), table, where, limit_str)
-        return db.do_select(sql, *args)
+        sql = cls._select_sql(where, limit, *selection)
+        return db.do_select(sql, *args, limit) if limit else db.do_select(sql, *args)
 
     @classmethod
-    def _get_pk_and_table(cls):
+    def _get_pk(cls):
         assert hasattr(cls, PK), "%s not set attribute '%s'" % (cls.__name__, PK)
-        return cls.__pk__, cls._get_table()
+        return cls.__pk__
 
     @classmethod
     def _get_table(cls):
         assert hasattr(cls, TABLE), "%s not set attribute '%s'" % (cls.__name__, TABLE)
         return cls.__table__
 
     @classmethod
+    def _get_pk_and_table(cls):
+        return cls._get_pk(), cls._get_table()
+
+    @classmethod
     def _dict2obj(cls, dictionary):
         m = Model()
-        m.__dict__.update(dictionary)
         m.__class__ = cls
+        cls.__init__(m, **dictionary)
         return m
 
     @classmethod
     def _get_update_by_col(cls):
         if hasattr(cls, UPDATE_BY):
             return cls.__update_by__
         return None
@@ -277,7 +297,31 @@
             return cls.__update_time__
         return None
 
     @classmethod
     def _get_del_flag_col(cls):
         assert hasattr(cls, DEL_FLAG), "%s not set attribute '%s'" % (cls.__name__, DEL_FLAG)
         return cls.__del_flag__
+
+    @classmethod
+    def _select_sql(cls, where, limit, *selection):
+        table = cls._get_table()
+        if len(selection) == 0:
+            selection = '*'
+        else:
+            selection = ','.join(['%s' % col if '(' in col else '`%s`' % col for col in selection])
+
+        if limit:
+            return 'SELECT %s FROM `%s` %s limit ?' % (selection, table, where)
+        else:
+            return 'SELECT %s FROM `%s` %s' % (selection, table, where)
+
+    @classmethod
+    def _update_sql(cls, where, *update_cols):
+        table = cls._get_table()
+        update_cols = ','.join(['`%s`=?' % col for col in update_cols])
+        update_time_col = cls._get_update_time_col()
+        if update_time_col is not None and update_time_col not in update_cols:
+            update_cols = '%s, %s' % (update_cols, '`%s`=CURRENT_TIMESTAMP' % update_time_col)
+
+        return 'UPDATE `%s` SET %s WHERE %s limit ?' % (table, update_cols, where)
+
```

### Comparing `mysqlx-1.2.3/README.md` & `mysqlx-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `mysqlx-1.2.3/setup.py` & `mysqlx-1.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     packages=find_packages(),
     description="mysqlx is a simple python sql executor for MySQL like iBatis.",
     long_description_content_type='text/markdown',
     install_requires=[
         'Jinja2>=3.0.3',
         'mysql-connector-python>=8.0.20',
     ],
-    version='1.2.3',
+    version='1.2.4',
     url='https://gitee.com/summry/mysqlx',
     author='summry',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'MySQL', 'iBatis', 'MyBatis', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.txt', '*.tpl'],
```

