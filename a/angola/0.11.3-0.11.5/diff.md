# Comparing `tmp/angola-0.11.3.tar.gz` & `tmp/angola-0.11.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "angola-0.11.3.tar", last modified: Wed Jun  7 07:05:25 2023, max compression
+gzip compressed data, was "angola-0.11.5.tar", last modified: Fri Jun  9 03:28:02 2023, max compression
```

## Comparing `angola-0.11.3.tar` & `angola-0.11.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-07 07:05:25.608914 angola-0.11.3/
--rw-r--r--   0 mardix     (501) staff       (20)     1084 2023-03-21 05:31:22.000000 angola-0.11.3/LICENSE
--rw-r--r--   0 mardix     (501) staff       (20)       26 2022-11-28 18:23:44.000000 angola-0.11.3/MANIFEST.in
--rw-r--r--   0 mardix     (501) staff       (20)     1257 2023-06-07 07:05:25.608986 angola-0.11.3/PKG-INFO
--rw-r--r--   0 mardix     (501) staff       (20)      877 2022-11-30 18:28:40.000000 angola-0.11.3/README.md
--rw-r--r--   0 mardix     (501) staff       (20)       79 2023-06-07 07:05:25.609221 angola-0.11.3/setup.cfg
--rw-r--r--   0 mardix     (501) staff       (20)      799 2023-06-07 07:05:15.000000 angola-0.11.3/setup.py
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-07 07:05:25.602844 angola-0.11.3/src/
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-07 07:05:25.606395 angola-0.11.3/src/angola/
--rw-r--r--   0 mardix     (501) staff       (20)      314 2023-04-30 19:58:20.000000 angola-0.11.3/src/angola/__init__.py
--rw-r--r--   0 mardix     (501) staff       (20)    48027 2023-05-30 03:49:44.000000 angola-0.11.3/src/angola/database.py
--rw-r--r--   0 mardix     (501) staff       (20)    12956 2023-06-03 04:28:39.000000 angola-0.11.3/src/angola/dict_mutator.py
--rw-r--r--   0 mardix     (501) staff       (20)    18847 2023-02-21 03:11:29.000000 angola-0.11.3/src/angola/dict_query.py
--rw-r--r--   0 mardix     (501) staff       (20)    17470 2023-06-03 04:30:01.000000 angola-0.11.3/src/angola/lib.py
--rw-r--r--   0 mardix     (501) staff       (20)    18970 2023-06-07 07:05:05.000000 angola-0.11.3/src/angola/lib_xql.py
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-07 07:05:25.607373 angola-0.11.3/src/angola.egg-info/
--rw-r--r--   0 mardix     (501) staff       (20)     1257 2023-06-07 07:05:25.000000 angola-0.11.3/src/angola.egg-info/PKG-INFO
--rw-r--r--   0 mardix     (501) staff       (20)      464 2023-06-07 07:05:25.000000 angola-0.11.3/src/angola.egg-info/SOURCES.txt
--rw-r--r--   0 mardix     (501) staff       (20)        1 2023-06-07 07:05:25.000000 angola-0.11.3/src/angola.egg-info/dependency_links.txt
--rw-r--r--   0 mardix     (501) staff       (20)       59 2023-06-07 07:05:25.000000 angola-0.11.3/src/angola.egg-info/requires.txt
--rw-r--r--   0 mardix     (501) staff       (20)        7 2023-06-07 07:05:25.000000 angola-0.11.3/src/angola.egg-info/top_level.txt
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-07 07:05:25.608815 angola-0.11.3/tests/
--rw-r--r--   0 mardix     (501) staff       (20)        0 2022-05-28 01:11:45.000000 angola-0.11.3/tests/test_cursor.py
--rw-r--r--   0 mardix     (501) staff       (20)      716 2022-11-28 18:20:13.000000 angola-0.11.3/tests/test_database.py
--rw-r--r--   0 mardix     (501) staff       (20)     1184 2022-11-28 18:20:13.000000 angola-0.11.3/tests/test_dict_mutator.py
--rw-r--r--   0 mardix     (501) staff       (20)     3301 2022-06-29 07:01:37.000000 angola-0.11.3/tests/test_lib.py
--rw-r--r--   0 mardix     (501) staff       (20)        0 2022-05-28 01:11:55.000000 angola-0.11.3/tests/test_query.py
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-09 03:28:02.081409 angola-0.11.5/
+-rw-r--r--   0 mardix     (501) staff       (20)     1084 2023-03-21 05:31:22.000000 angola-0.11.5/LICENSE
+-rw-r--r--   0 mardix     (501) staff       (20)       26 2022-11-28 18:23:44.000000 angola-0.11.5/MANIFEST.in
+-rw-r--r--   0 mardix     (501) staff       (20)     1318 2023-06-09 03:28:02.081477 angola-0.11.5/PKG-INFO
+-rw-r--r--   0 mardix     (501) staff       (20)      938 2023-06-09 03:27:48.000000 angola-0.11.5/README.md
+-rw-r--r--   0 mardix     (501) staff       (20)       79 2023-06-09 03:28:02.081732 angola-0.11.5/setup.cfg
+-rw-r--r--   0 mardix     (501) staff       (20)      799 2023-06-09 03:27:56.000000 angola-0.11.5/setup.py
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-09 03:28:02.075341 angola-0.11.5/src/
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-09 03:28:02.078556 angola-0.11.5/src/angola/
+-rw-r--r--   0 mardix     (501) staff       (20)      428 2023-06-09 03:27:14.000000 angola-0.11.5/src/angola/__init__.py
+-rw-r--r--   0 mardix     (501) staff       (20)    48677 2023-06-09 03:15:08.000000 angola-0.11.5/src/angola/database.py
+-rw-r--r--   0 mardix     (501) staff       (20)    12956 2023-06-03 04:28:39.000000 angola-0.11.5/src/angola/dict_mutator.py
+-rw-r--r--   0 mardix     (501) staff       (20)    18847 2023-02-21 03:11:29.000000 angola-0.11.5/src/angola/dict_query.py
+-rw-r--r--   0 mardix     (501) staff       (20)    17470 2023-06-03 04:30:01.000000 angola-0.11.5/src/angola/lib.py
+-rw-r--r--   0 mardix     (501) staff       (20)    19447 2023-06-09 03:27:14.000000 angola-0.11.5/src/angola/lib_xql.py
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-09 03:28:02.079561 angola-0.11.5/src/angola.egg-info/
+-rw-r--r--   0 mardix     (501) staff       (20)     1318 2023-06-09 03:28:02.000000 angola-0.11.5/src/angola.egg-info/PKG-INFO
+-rw-r--r--   0 mardix     (501) staff       (20)      464 2023-06-09 03:28:02.000000 angola-0.11.5/src/angola.egg-info/SOURCES.txt
+-rw-r--r--   0 mardix     (501) staff       (20)        1 2023-06-09 03:28:02.000000 angola-0.11.5/src/angola.egg-info/dependency_links.txt
+-rw-r--r--   0 mardix     (501) staff       (20)       59 2023-06-09 03:28:02.000000 angola-0.11.5/src/angola.egg-info/requires.txt
+-rw-r--r--   0 mardix     (501) staff       (20)        7 2023-06-09 03:28:02.000000 angola-0.11.5/src/angola.egg-info/top_level.txt
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-09 03:28:02.081285 angola-0.11.5/tests/
+-rw-r--r--   0 mardix     (501) staff       (20)        0 2022-05-28 01:11:45.000000 angola-0.11.5/tests/test_cursor.py
+-rw-r--r--   0 mardix     (501) staff       (20)      716 2022-11-28 18:20:13.000000 angola-0.11.5/tests/test_database.py
+-rw-r--r--   0 mardix     (501) staff       (20)     1184 2022-11-28 18:20:13.000000 angola-0.11.5/tests/test_dict_mutator.py
+-rw-r--r--   0 mardix     (501) staff       (20)     3301 2022-06-29 07:01:37.000000 angola-0.11.5/tests/test_lib.py
+-rw-r--r--   0 mardix     (501) staff       (20)        0 2022-05-28 01:11:55.000000 angola-0.11.5/tests/test_query.py
```

### Comparing `angola-0.11.3/LICENSE` & `angola-0.11.5/LICENSE`

 * *Files identical despite different names*

### Comparing `angola-0.11.3/PKG-INFO` & `angola-0.11.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: angola
-Version: 0.11.3
+Version: 0.11.5
 Summary: angola 
 Home-page: https://github.com/mardix/angola
 Author: Mardix
 Author-email: mardix@blackdevhub.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Database
@@ -14,14 +14,22 @@
 
 # Angola
 
 **Angola**
 
 ## API
 
+- `db` 
+- `xql_to_aql`
+- `parse_dict_mutations`
+- `gen_xid`
+- `Collection` 
+- `CollectionItem`
+- `CollectionActiveRecordMixin`
+- 
 ## Connection
 
 ```
 import angola
 
 #--- connect
 db = angola.db(hosts="http://host:8529", username="root", password:str)
@@ -36,23 +44,19 @@
 coll.insert({k:v,...}, _key='awesome')
 
 
 ```
 
 ### Query 
 
-### @@CURRDATE
-
-`@@CURRDATE($format=None, $dateshifter=None) `
-
 
 
 ```
   {
-    "_modified_at": "@@CURRDATE() +2Days"
+    "_modified_at:$datetime": "+2hh"
   }
 ```
 
 Format:
 
 ```
 YYYY: Year
```

### Comparing `angola-0.11.3/setup.py` & `angola-0.11.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 
 def long_description():
     with open('README.md', 'r') as file:
         return file.read()
 
-VERSION = "0.11.3"
+VERSION = "0.11.5"
 setuptools.setup(
     name='angola',
     version=VERSION,
     author='Mardix',
     author_email='mardix@blackdevhub.io',
     description='angola ',
     long_description=long_description(),
```

### Comparing `angola-0.11.3/src/angola/database.py` & `angola-0.11.5/src/angola/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -734,15 +734,15 @@
         if self.dbname:
             self.db = self.client.db(name=self.dbname, username=self.username, password=self.password)
 
     @property
     def aql(self):
         return self.db.aql
 
-    def _prefix_collection_name(self, collection_name:str) -> str:
+    def prefix_collection_name(self, collection_name:str) -> str:
         if self._collection_prefix:
             if isinstance(self._collection_prefix, str):
                 collection_name = "%s%s" % (self._collection_prefix, collection_name)
             elif callable(self._collection_prefix):
                 collection_name = self._collection_prefix(collection_name)
         return collection_name
 
@@ -801,24 +801,24 @@
 
         Params:
             collection_name:str - the collection name 
 
         Returns:
             bool
         """
-        collection_name = self._prefix_collection_name(collection_name)
+        collection_name = self.prefix_collection_name(collection_name)
         return self.db.has_collection(collection_name)
 
     def create_collection(self, collection_name:str, indexes:list=[]) -> bool:
         """
         Create a collection if not exists
         Returns: bool
         """
         if not self.has_collection(collection_name):
-            collection_name = self._prefix_collection_name(collection_name)
+            collection_name = self.prefix_collection_name(collection_name)
             col = self.db.create_collection(collection_name)
 
             _indexes = DEFAULT_INDEXES
             if not indexes and self.default_indexes:
                 _indexes = [*self.default_indexes, *_indexes]
 
             for index in _indexes:
@@ -838,31 +838,31 @@
             auto_create:bool - To auto create the collection if doesn't exist
 
         Return: Collection
 
         """
 
         if self.has_collection(collection_name):
-            collection_name = self._prefix_collection_name(collection_name)
+            collection_name = self.prefix_collection_name(collection_name)
             col = self.db.collection(collection_name)
         elif auto_create is True:
             self.create_collection(collection_name=collection_name, indexes=indexes)
-            collection_name = self._prefix_collection_name(collection_name)
+            collection_name = self.prefix_collection_name(collection_name)
             col = self.db.collection(collection_name)
         else:
             raise CollectionNotFoundError()
 
         return Collection(db=self, collection=col, immut_keys=immut_keys, custom_ops=self._custom_ops, item_class=item_class)
 
     def select_edge_collection(self, collection_name:str):
         if self.db.has_collection(collection_name):
-            collection_name = self._prefix_collection_name(collection_name)
+            collection_name = self.prefix_collection_name(collection_name)
             return self.db.collection(collection_name)
         else:
-            collection_name = self._prefix_collection_name(collection_name)
+            collection_name = self.prefix_collection_name(collection_name)
             return self.db.create_collection(name=collection_name, edge=True)
 
     def get_item(self, path:str) -> CollectionItem:
         """
         To get an item via path.
 
         - Item Path: [COLLECTION_NAME/KEY] -> articles/1234568
@@ -885,19 +885,19 @@
         paths = path.split("/")
         len_paths = len(paths)
         if len_paths < 2 or len_paths > 4:
             raise InvalidItemPathError()
 
         try:
             if len_paths == 2: # item -> [coll/key]
-                return self.select_collection(self._prefix_collection_name(paths[0])).get(paths[1])
+                return self.select_collection(self.prefix_collection_name(paths[0])).get(paths[1])
             elif len_paths == 3: # item's subcolelction -> [coll/key/subcoll]
-                return self.select_collection(self._prefix_collection_name(paths[0])).get(paths[1]).select_subcollection(paths[2])
+                return self.select_collection(self.prefix_collection_name(paths[0])).get(paths[1]).select_subcollection(paths[2])
             elif len_paths == 4: # item's subcollection items -> [coll/key/subcoll/subkey]
-                return self.select_collection(self._prefix_collection_name(paths[0]))\
+                return self.select_collection(self.prefix_collection_name(paths[0]))\
                     .get(paths[1])\
                     .select_subcollection(paths[2])\
                     .get(paths[3])
         except Exception as e:
             return None
 
     def execute_aql(self, query:str, bind_vars:dict={}, *a, **kw):
@@ -906,83 +906,95 @@
         Params:
             query:str - the AQL to execute 
             bind_vars: dict - the variables to pass in the query
         Return aql cursor
         """
         return self.aql.execute(query=query, bind_vars=bind_vars, *a, **kw)
 
-    def query(self, xql:lib_xql.XQLDEFINITION, data:dict={}, kvmap:dict={}, parser=None, data_mapper=None) -> _QueryResultIterator:
+    def query(self, xql:lib_xql.XQLDEFINITION, data:dict={}, parser=None, data_mapper=None) -> _QueryResultIterator:
         """
         XQL query  a collection based on filters
 
         It will return the cursor:ArangoCursor and a pagination for the current state
         
         Params:
             xql:lib_xql.XQLDEFINITION
             data:dict
-            kvmap:dict
             data_mapper:function - a callback function
         Returns
             _QueryResultIterator
         """
 
-        aql, bind_vars, pager = self._build_query(xql=xql, data=data, kvmap=kvmap, parser=parser)
+        aql, bind_vars, pager = self.build_query(xql=xql, data=data, parser=parser)
         cursor = self.execute_aql(aql, bind_vars=bind_vars, count=True, full_count=True)            
         return _QueryResultIterator(cursor=cursor, pager=pager, data_mapper=data_mapper)
 
-    def _build_query(self, xql:lib_xql.XQLDEFINITION, data:dict={}, kvmap:dict={}, parser=None):
+    def build_query(self, xql:lib_xql.XQLDEFINITION, data:dict={}, parser=None):
         """
         Build a query from XQL
 
         Return tuple:
             - aql:str
             - bind_vars:dict
             - pagination:tuple 
                 -> tuple(page, per_page)
         """        
         xql = lib_xql.prepare_xql(xql)
-        # replace the kvmap
-        xql["FILTERS"] = lib.dict_find_replace(xql["FILTERS"], kvmap)
 
         # pagination
         if "page" in data:
             xql["PAGE"] = data.get("page") or 1
             del data["page"]
         if "limit" in data:
             xql["LIMIT"] = data.get("limit") or 10
             del data["limit"]
 
         _per_page, _, _page = lib_xql.xql_take_skip_page(xql=xql, max_limit=self.query_max_limit)
         aql, bind_vars = lib_xql.xql_to_aql(xql, vars=data, parser=parser, max_limit=self.query_max_limit)
         bind_vars.update(data)
         return aql, bind_vars, (_page, _per_page)
 
+    def return_count(self, xql:lib_xql.XQLDEFINITION, data:dict={}) -> int:
+        """
+        From a query, it returns the count 
+
+        Params:
+            xql:lib_xql.XQLDEFINITION
+            data:dict
+        Returns
+            Interger
+        """
+        xql["RETURN_COUNT"] = True
+        aql, bind_vars, pager = self.build_query(xql=xql, data=data)
+        cursor = self.execute_aql(aql, bind_vars=bind_vars, count=True, full_count=True) 
+        return cursor.batch()[0] if cursor.count() else 0
+
     def collections(self) -> list:
         """
         All collections in the db
 
         Returns:
             list
         """
         return self.db.collections()
     
     def rename_collection(self, collection_name:str, new_name:str):
         """
         Rename collection
         """
         if self.has(collection_name) and not self.has(new_name):
-            collection_name = self._prefix_collection_name(collection_name)
-            new_name = self._prefix_collection_name(new_name)
+            collection_name = self.prefix_collection_name(collection_name)
+            new_name = self.prefix_collection_name(new_name)
             coll = self.select(collection_name)
             coll.rename(new_name)
             return self.select(new_name)
     
     def drop_collection(self, collection_name:str):
         if self.has_collection(collection_name):
-            collection_name = self._prefix_collection_name(collection_name)
+            collection_name = self.prefix_collection_name(collection_name)
             self.db.delete_collection(collection_name)
 
     def add_index(self, collection_name, data:dict):
         """
         Args:
             - collection, the collection name
             - data: dict of 
@@ -991,27 +1003,27 @@
                         "fields": [] # list of fields
                         "unique": False # bool - Whether the index is unique
                         "sparse": False # bool,
                         "name": "" # str - Optional name for the index
                         "inBackground": False # bool - Do not hold the collection lock
                     }
         """
-        collection_name = self._prefix_collection_name(collection_name)
+        collection_name = self.prefix_collection_name(collection_name)
         col = self.db.collection(collection_name)
         col._add_index(data)
       
     def delete_index(self, collection_name:str, id):
         """
         Delete Index
 
         Args:
             - collection, the collection name
             - id: the index id
         """
-        collection_name = self._prefix_collection_name(collection_name)
+        collection_name = self.prefix_collection_name(collection_name)
         col = self.db.collection(collection_name)
         col.delete_index(id, ignore_missing=True)
 
     def link_edges(self, from_item:"CollectionItem", to_item:"CollectionItem", data:dict={}, edge_collection_name:str=None):
         """
         GRAPH
         Link edges of 2 collections from:to
@@ -1052,15 +1064,15 @@
 
     def unlink_edges(self, from_item:"CollectionItem", to_item:"CollectionItem"):
         pass
 
     def _load_item(self, data:dict) -> "CollectionItem":
         if "_id" in data:
             collection_name, _key = data.get("_id").split("/")
-            collection_name = self._prefix_collection_name(collection_name)
+            collection_name = self.prefix_collection_name(collection_name)
             col = self.db.collection(collection_name)
             return Collection(db=self, collection=col, custom_ops=self._custom_ops).item(data)
         else:
             raise Exception("INVALID_ITEM__MUST_HAVE_ID")
 
     def traverse(self, from_item:"CollectionItem", collection:"Collection", relations:list("Collection")=None, direction="outbound", filters={}):
         """
@@ -1316,14 +1328,28 @@
             if "JOIN" in _xql:
                 read_only = True
 
 
         def data_mapper(item): return self.item(item, read_only=read_only)
         return self.db.query(_xql, data_mapper=data_mapper)
 
+    def return_count(self, filters:dict={}) -> int:
+        """
+        Return the total count of documents from query
+
+        Returns
+            Int
+        """
+        
+        _xql = {
+            "FROM": self.collection_name, 
+            "FILTERS": filters
+        }
+        return self.db.return_count(xql=_xql)
+
     def find_one(self, filters:dict, sort=None):
         """
         Retrieve one item based on the criteria
 
         Returns
             CollectionItem
         """
```

### Comparing `angola-0.11.3/src/angola/dict_mutator.py` & `angola-0.11.5/src/angola/dict_mutator.py`

 * *Files identical despite different names*

### Comparing `angola-0.11.3/src/angola/dict_query.py` & `angola-0.11.5/src/angola/dict_query.py`

 * *Files identical despite different names*

### Comparing `angola-0.11.3/src/angola/lib.py` & `angola-0.11.5/src/angola/lib.py`

 * *Files identical despite different names*

### Comparing `angola-0.11.3/src/angola/lib_xql.py` & `angola-0.11.5/src/angola/lib_xql.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,27 +23,30 @@
         :param PAGE: int = help calculate the skip by using a page number. 
         :param JOIN: list[XQL]
         :param RETURN_COUNT: bool =  Will return a count of all matched documents
         :param RETURN: str = string representation
         :param MERGE: str = on JOIN, to merge the data.
             ie: MERGE: "{__profile: profile}" 
             Can be done manually with RETURN MERGE(doc, {data})
+        :param RETURN_PARTIAL_QUERY: bool 
+            To return the query without final the return. By this can help with SELECT to INSERT
 
     """
     FROM: str = None
     ALIAS: str = None
     FILTERS: dict = {}
     SORT: list = []
     OFFSET: int = 0
     LIMIT: int = 10
     PAGE: int = 1
     JOIN: list = []
     RETURN_COUNT: str = None
     RETURN: str = None
     MERGE: str = None
+    RETURN_PARTIAL_QUERY: bool = False
 
 
 # -----------------------------------------------------------------------------
 # === MACROS ------------------------------------------------------------------
 
 def _re_match(pattern, value) -> re:
     return re.match(pattern, value, flags=re.IGNORECASE)
@@ -364,24 +367,25 @@
     # TODO
     return ""
 
 
 def prepare_xql(xql: dict) -> dict:
     _defaults = {
         "FROM": None,
-        "ALIAS": "root__",
+        "ALIAS": "doc",
         "FILTERS": {},
         "SORT": None,
         "OFFSET": None,
         "RETURN_COUNT": False,
         "LIMIT": 10,
         "PAGE": 1,
         "JOIN": [],
         "RETURN": None,
         "RETURN_WITH": None,
+        "RETURN_PARTIAL_QUERY": False,
         **xql
     }
     r = {k.upper(): v for k, v in _defaults.items()}
     if r["RETURN"] is None:
         r["RETURN"] = r["ALIAS"]
     return r
 
@@ -436,19 +440,20 @@
         ALIAS: str = alias
         FILTERS: dict = filters
         SORT: list/str = sort 
         OFFSET: int = the offset of the limit, default=0
         LIMIT: int = the limit of result, default=10
         PAGE: int = help calculate the offset by using a page number. 
         JOIN: list[XQL]
-        RETURN_COUNT: str =  To count all the document, and return the value. Alias to `COLLECT WITH COUNT INTO`
         RETURN: str = string representation
         MERGE: str = on JOIN, to merge the data.
             ie: MERGE: "{__profile: profile}" 
             Can be done manually with RETURN MERGE(doc, {data})
+        RETURN_COUNT: str =  To count all the document, and return the value. Alias to `COLLECT WITH COUNT INTO`
+        RETURN_PARTIAL_QUERY: bool - To return the query without final the return. By this can help with SELECT to INSERT
 
         # TODO
         - WHEN: ? = a conditional to evaluate before running
         - FILTER_WHEN: add additional filters when a condition is true
 
     === 
     schema example:
@@ -515,36 +520,38 @@
             ],
             "RETURN": "MERGE(post, {__account: loco})"
     """
 
     xql = prepare_xql(xql)
 
     if not xql.get("ALIAS"):
-        xql["ALIAS"] = "root__"
+        xql["ALIAS"] = "doc"
 
-    ALIAS = xql.get("ALIAS") or "root__"
+    ALIAS = xql.get("ALIAS") or "doc"
 
     if parser:
         xql = parser(xql)
 
     COLLECTION = xql.get("FROM")
     FILTERS = xql.get("FILTERS") or {}
     SORTS = xql.get("SORT")
     OFFSET = xql.get("OFFSET")
     LIMIT = xql.get("LIMIT") or 10
     PAGE = xql.get("PAGE") or 1
     JOINS = xql.get("JOIN") or []
-    RETURN_COUNT = xql.get("RETURN_COUNT")
     COLLECTS = xql.get("COLLECT") or []
     RETURN = xql.get("RETURN") or ALIAS
 
+    RETURN_COUNT = xql.get("RETURN_COUNT")
+    RETURN_PARTIAL_QUERY = xql.get("RETURN_PARTIAL_QUERY")
+
     # work with take/skip
     if OFFSET is None:
         page = PAGE or 1
-        per_page = max_limit if per_page > max_limit else LIMIT
+        per_page = max_limit if LIMIT > max_limit else LIMIT
         OFFSET = lib.calc_pagination_offset(page=page, per_page=per_page)
         LIMIT = per_page
     if LIMIT > max_limit:
         LIMIT = max_limit
 
 
     # unique num to give each field to prevent name collision
@@ -566,15 +573,18 @@
     # Query
     query = "FOR {alias} IN @@collection_{num_} ".format(alias=ALIAS, num_=num_)
     query += aql_filter
     query += subquery
     query += aql_collects
     query += " LIMIT @offset_%s, @limit_%s " % (num_, num_)
     query += aql_sorting
-    query += "RETURN UNSET_RECURSIVE(%s, ['_id', '_rev', '_old_rev'])" % RETURN
+ 
+    # partial query doesn't have the final return
+    if not RETURN_PARTIAL_QUERY:
+        query += "RETURN UNSET_RECURSIVE(%s, ['_id', '_rev', '_old_rev'])" % RETURN
 
     if RETURN_COUNT:
         query = "RETURN LENGTH(%s)" % query
 
     bind_vars.update({
         **filter_vars,
         "offset_%s" % num_: OFFSET,
```

### Comparing `angola-0.11.3/src/angola.egg-info/PKG-INFO` & `angola-0.11.5/src/angola.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: angola
-Version: 0.11.3
+Version: 0.11.5
 Summary: angola 
 Home-page: https://github.com/mardix/angola
 Author: Mardix
 Author-email: mardix@blackdevhub.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Database
@@ -14,14 +14,22 @@
 
 # Angola
 
 **Angola**
 
 ## API
 
+- `db` 
+- `xql_to_aql`
+- `parse_dict_mutations`
+- `gen_xid`
+- `Collection` 
+- `CollectionItem`
+- `CollectionActiveRecordMixin`
+- 
 ## Connection
 
 ```
 import angola
 
 #--- connect
 db = angola.db(hosts="http://host:8529", username="root", password:str)
@@ -36,23 +44,19 @@
 coll.insert({k:v,...}, _key='awesome')
 
 
 ```
 
 ### Query 
 
-### @@CURRDATE
-
-`@@CURRDATE($format=None, $dateshifter=None) `
-
 
 
 ```
   {
-    "_modified_at": "@@CURRDATE() +2Days"
+    "_modified_at:$datetime": "+2hh"
   }
 ```
 
 Format:
 
 ```
 YYYY: Year
```

### Comparing `angola-0.11.3/tests/test_database.py` & `angola-0.11.5/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `angola-0.11.3/tests/test_dict_mutator.py` & `angola-0.11.5/tests/test_dict_mutator.py`

 * *Files identical despite different names*

### Comparing `angola-0.11.3/tests/test_lib.py` & `angola-0.11.5/tests/test_lib.py`

 * *Files identical despite different names*

