# Comparing `tmp/orbit_database-0.99.91.tar.gz` & `tmp/orbit_database-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orbit_database-0.99.91.tar", max compression
+gzip compressed data, was "orbit_database-1.0.0.tar", max compression
```

## Comparing `orbit_database-0.99.91.tar` & `orbit_database-1.0.0.tar`

### file list

```diff
@@ -1,22 +1,24 @@
--rwxr-xr-x   0        0        0     1087 2023-04-19 17:27:34.642403 orbit_database-0.99.91/LICENSE
--rw-r--r--   0        0        0     3643 2023-04-20 12:26:13.473567 orbit_database-0.99.91/README.md
--rwxr-xr-x   0        0        0     1917 2023-04-20 11:57:07.111022 orbit_database-0.99.91/orbit_database/__init__.py
--rw-r--r--   0        0        0     5884 2023-04-20 12:12:44.156774 orbit_database-0.99.91/orbit_database/audit.py
--rwxr-xr-x   0        0        0     2473 2023-04-20 12:13:03.900306 orbit_database-0.99.91/orbit_database/bitmap.py
--rwxr-xr-x   0        0        0    10513 2023-04-20 12:13:14.200061 orbit_database-0.99.91/orbit_database/compression.py
--rwxr-xr-x   0        0        0     1880 2023-04-19 16:50:03.108978 orbit_database-0.99.91/orbit_database/cursor.py
--rwxr-xr-x   0        0        0    16046 2023-04-19 16:52:09.982122 orbit_database-0.99.91/orbit_database/database.py
--rwxr-xr-x   0        0        0     4817 2022-12-19 12:08:17.236425 orbit_database-0.99.91/orbit_database/decorators.py
--rwxr-xr-x   0        0        0    10060 2023-04-20 12:17:22.514168 orbit_database-0.99.91/orbit_database/doc.py
--rwxr-xr-x   0        0        0     1104 2021-03-29 14:51:15.628206 orbit_database-0.99.91/orbit_database/exceptions.py
--rwxr-xr-x   0        0        0     3322 2023-04-19 16:54:12.787363 orbit_database-0.99.91/orbit_database/filterresult.py
--rwxr-xr-x   0        0        0    10268 2023-04-19 16:54:12.787363 orbit_database-0.99.91/orbit_database/index.py
--rwxr-xr-x   0        0        0    13227 2023-04-20 12:18:37.912378 orbit_database-0.99.91/orbit_database/invertedwordindex.py
--rwxr-xr-x   0        0        0     2896 2023-04-19 16:54:12.787363 orbit_database-0.99.91/orbit_database/manager.py
--rwxr-xr-x   0        0        0    12179 2023-04-19 16:54:12.787363 orbit_database-0.99.91/orbit_database/metadata.py
--rwxr-xr-x   0        0        0     4432 2023-04-19 16:54:12.787363 orbit_database-0.99.91/orbit_database/objectid.py
--rwxr-xr-x   0        0        0     6867 2023-04-19 16:54:12.787363 orbit_database-0.99.91/orbit_database/serialiser.py
--rwxr-xr-x   0        0        0    42289 2023-04-20 12:13:54.815097 orbit_database-0.99.91/orbit_database/table.py
--rwxr-xr-x   0        0        0      387 2023-04-20 12:13:59.678982 orbit_database-0.99.91/orbit_database/types_.py
--rw-r--r--   0        0        0      817 2023-04-20 12:22:44.374529 orbit_database-0.99.91/pyproject.toml
--rw-r--r--   0        0        0     4124 1970-01-01 00:00:00.000000 orbit_database-0.99.91/PKG-INFO
+-rwxr-xr-x   0        0        0     1087 2023-06-09 10:34:34.878082 orbit_database-1.0.0/LICENSE
+-rw-r--r--   0        0        0     4506 2023-06-09 10:34:34.878082 orbit_database-1.0.0/README.md
+-rw-r--r--   0        0        0       46 2023-06-09 10:34:34.882082 orbit_database-1.0.0/orbit_database/README.md
+-rwxr-xr-x   0        0        0     1932 2023-06-09 10:34:34.882082 orbit_database-1.0.0/orbit_database/__init__.py
+-rw-r--r--   0        0        0     6369 2023-06-09 10:34:34.882082 orbit_database-1.0.0/orbit_database/audit.py
+-rwxr-xr-x   0        0        0     2473 2023-06-09 10:34:34.882082 orbit_database-1.0.0/orbit_database/bitmap.py
+-rw-r--r--   0        0        0     3542 2023-06-09 10:34:34.882082 orbit_database-1.0.0/orbit_database/catalog.py
+-rwxr-xr-x   0        0        0    10513 2023-06-09 10:34:34.882082 orbit_database-1.0.0/orbit_database/compression.py
+-rwxr-xr-x   0        0        0     1880 2023-06-09 10:34:34.882082 orbit_database-1.0.0/orbit_database/cursor.py
+-rwxr-xr-x   0        0        0    15912 2023-06-09 10:34:34.882082 orbit_database-1.0.0/orbit_database/database.py
+-rwxr-xr-x   0        0        0     5360 2023-06-09 10:34:34.882082 orbit_database-1.0.0/orbit_database/decorators.py
+-rwxr-xr-x   0        0        0    10044 2023-06-09 10:34:34.882082 orbit_database-1.0.0/orbit_database/doc.py
+-rwxr-xr-x   0        0        0     1104 2023-06-09 10:34:34.882082 orbit_database-1.0.0/orbit_database/exceptions.py
+-rwxr-xr-x   0        0        0     3322 2023-06-09 10:34:34.882082 orbit_database-1.0.0/orbit_database/filterresult.py
+-rwxr-xr-x   0        0        0    10506 2023-06-09 10:34:34.882082 orbit_database-1.0.0/orbit_database/index.py
+-rwxr-xr-x   0        0        0    15546 2023-06-09 10:34:34.882082 orbit_database-1.0.0/orbit_database/invertedwordindex.py
+-rwxr-xr-x   0        0        0     2924 2023-06-09 10:34:34.882082 orbit_database-1.0.0/orbit_database/manager.py
+-rwxr-xr-x   0        0        0    14240 2023-06-09 10:34:34.882082 orbit_database-1.0.0/orbit_database/metadata.py
+-rwxr-xr-x   0        0        0     4432 2023-06-09 10:34:34.882082 orbit_database-1.0.0/orbit_database/objectid.py
+-rwxr-xr-x   0        0        0     6864 2023-06-09 10:34:34.882082 orbit_database-1.0.0/orbit_database/serialiser.py
+-rwxr-xr-x   0        0        0    41987 2023-06-09 10:34:34.882082 orbit_database-1.0.0/orbit_database/table.py
+-rwxr-xr-x   0        0        0      387 2023-06-09 10:34:34.882082 orbit_database-1.0.0/orbit_database/types_.py
+-rw-r--r--   0        0        0     1570 2023-06-09 10:34:34.886081 orbit_database-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     5530 1970-01-01 00:00:00.000000 orbit_database-1.0.0/PKG-INFO
```

### Comparing `orbit_database-0.99.91/LICENSE` & `orbit_database-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `orbit_database-0.99.91/README.md` & `orbit_database-1.0.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,28 @@
-# Orbit Database
+# Orbit Database - Introduction
 
-This project is the NoSQL database that underpins the Orbit Framework. The interface is written in Python3 and uses LMDB as it's back-end key/value store. Please don't be put off by the <i>written in Python</i> statement, the database performs well and in many cases surpasses what you might expect from a dedicated database engine such as MariaDB or Postgres.
+#### Welcome to the Orbit Database repository and documentation. All project documentation is included within this repository and consists of markdown files and comments within the code. These are presented in real time by the "ZeroDocs" Orbit application which renders this content to HTML in real-time.
 
-<img style="height:350px" src="https://gitlab.com/madpenguin/orbit-database/-/raw/main/images/orbit_database.png" />
+This project is the NoSQL database that underpins the Orbit Framework. The interface is written in Python3 and uses LMDB as it's back-end key/value store. Please don't be put off by the <i>written in Python</i> statement, the database performs well and in many cases surpasses what you might expect from a dedicated database engine such as MariaDB or Postgres. The software architecture looks like this;
 
-### Primary design goals
+<table><tr><td><img style="height:350px" src="https://gitlab.com/madpenguin/orbit-database/-/raw/main/images/orbit_database.png" /></td><td>
+<h3 style="padding-left:1.4em">Primary design goals</h3>
 
 * Must perform well in a Python multi-processing environment
 * Must integrate well with Python based microservices
 * Must be easy to deploy in a cloud environment
 * Must be easily testable in a Python environment
 * Must offer the same basic functionality as mainstream database engines
 * Must facilitate efficient real-time triggers when data is changed
+* Must be easy to replicate in real time
+</td></tr></table>
 
 Although these goals are entirely subjective, when compared to Python applications using traditional SQL databases, in general these goals have arguably been surpassed. If you are looking for a fast primary database to use in a native non-Python environment, then look elsewhere. If you need a database system with more capacity for use outside of Python, then consider Orbit-Database as a cache / real-time buffer between your 'real' database and each user's screen. If all you need is a read-speed of a few hundred thousand records a second, and an ACID write speed of 20,000 per second, look no further!
 
-### Features
+### Database Features
 
 * Schemaless / NoSQL model, but with dynamic ORM system
 * Database interface effectively reads and writes Python objects
 * Secondary indexes can be created using any Python expression / function
 * Secondary indexes support primary and duplicate variants
 * The storage engine supports ACID Transactions
 * Locking system enables massively parallel writing over many processes
@@ -48,7 +51,20 @@
 from schema.People import PeopleCollection
 
 OrbitDatabase([PeopleCollection]).open('my_database')
 for result in PeopleCollection():
     person = result.doc
     print(f'Name={person._name} Age={person._age}')
 ```
+
+## Todo List (features)
+
+* Deploy new indexing on OC + test - running - wip
+* Write V2 conversion routine - wip
+
+* Implement rename table in shell
+* Implement rename index in shell
+
+
+* Freelist management and compression for full-text indexcies
+* Resting encryption for specific fields and raw blobs and words
+* Better form of JSON for reading fields without deserialisation
```

### Comparing `orbit_database-0.99.91/orbit_database/__init__.py` & `orbit_database-1.0.0/orbit_database/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 #####################################################################################
 #
 #  Copyright (c) 2020 - Mad Penguin Consulting Ltd
 #
 #####################################################################################
 
-__version__ = '0.9.91'
+__version__ = '1.0.0'
 
 from orbit_database.manager import Manager
 from orbit_database.database import Database
 from orbit_database.table import Table
 from orbit_database.filterresult import FilterResult, MatchResult
 from orbit_database.index import Index
 from orbit_database.doc import Doc, JournalType
 from orbit_database.compression import CompressionType
 from orbit_database.objectid import ObjectId
 from orbit_database.audit import AuditEntry
-from orbit_database.decorators import transparent_resize, WriteTransaction, ReadTransaction
+from orbit_database.decorators import WriteTransaction, ReadTransaction, wrap_writer, wrap_reader
 from orbit_database.serialiser import Serialiser, SerialiserType
 from orbit_database.exceptions import IndexAlreadyExists, FailedToWriteMetadata, DocumentAlreadyExists, FailedToWriteData, \
     DocumentDoesntExist, InvalidKeySpecifier, NoSuchIndex, NotDuplicateIndex, NoSuchTable, \
     DuplicateKey, IndexWriteError, TableNotOpen, TrainingDataExists, InvalidSerialiser, InvalidId
 from orbit_database.bitmap import Bitmap
 from orbit_database.invertedwordindex import InvertedWordIndex, Lexicon
 
@@ -31,15 +31,16 @@
     Table,
     Index,
     Doc,
     CompressionType,
     ObjectId,
     FilterResult,
     MatchResult,
-    transparent_resize,
+    wrap_reader,
+    wrap_writer,
     WriteTransaction,
     ReadTransaction,
     JournalType,
     Serialiser,
     SerialiserType,
     IndexAlreadyExists,
     FailedToWriteMetadata,
```

### Comparing `orbit_database-0.99.91/orbit_database/audit.py` & `orbit_database-1.0.0/orbit_database/audit.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from threading import Thread
 from orbit_database.doc import Doc
 from orbit_database.serialiser import SerialiserType
 from struct import pack, unpack
 from time import sleep
 from getpass import getuser
 import asyncio
+import hashlib
 
 try:
     from loguru import logger as log
 except Exception:
     import logging as log
 
 
@@ -42,25 +43,36 @@
         self._semaphore = None
         self._handlers = {}
         self._finished = False
         self._auditing = False
         self._tasks = []
 
     def open(self, auditing=False):
-        doc = self._database.meta.fetch_key(self.UUID_KEY)
-        if doc:
-            self._uuid = doc._uuid
-        else:
-            self._uuid = f'{getuser()}_{self._database._name}'
-            self._database.meta.store_key(self.UUID_KEY, Doc({'uuid': self._uuid}))
-        self._table = self._database.table(f'__audit_table__')
+        # doc = self._database.meta.fetch_key(self.UUID_KEY)
+        # if doc:
+        #     self._uuid = doc._uuid
+        # else:
+        #     self._uuid = f'{getuser()}_{self._database._name}'
+        #     self._database.meta.store_key(self.UUID_KEY, Doc({'uuid': self._uuid}))
+        #
+        #   Needs to be unique based on path + user ... metadata is an overcomplication
+        #
+        hObj = hashlib.new('sha1')
+        hObj.update(str(self._database._path).encode())
+        self._uuid = hObj.hexdigest()
+        if self._database.index_version == 1:
+            audit_table_name = '__audit_table__'
+        elif self._database.index_version == 2:
+            audit_table_name = '@@audit_table@@'
+
+        self._table = self._database.table(audit_table_name)
         try:
             self._semaphore = Semaphore(f'/{self._uuid}', flags=O_CREAT)
-        except ExistentialError as e:                   # pragma: no cover
-            raise Exception(f'audit error: {str(e)}')   # pragma: no cover
+        except (ExistentialError, ValueError) as e:                   # pragma: no cover
+            raise Exception(f'audit error: {str(e)} // {self._uuid}')   # pragma: no cover
         self._auditing = auditing                   
         if auditing:
             self._finished = False
             self._thread = Thread(target=self.callback, args=(asyncio.get_event_loop(),), daemon=True)
             self._thread.start()
         return self
```

### Comparing `orbit_database-0.99.91/orbit_database/bitmap.py` & `orbit_database-1.0.0/orbit_database/bitmap.py`

 * *Files identical despite different names*

### Comparing `orbit_database-0.99.91/orbit_database/compression.py` & `orbit_database-1.0.0/orbit_database/compression.py`

 * *Files identical despite different names*

### Comparing `orbit_database-0.99.91/orbit_database/cursor.py` & `orbit_database-1.0.0/orbit_database/cursor.py`

 * *Files identical despite different names*

### Comparing `orbit_database-0.99.91/orbit_database/database.py` & `orbit_database-1.0.0/orbit_database/database.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,30 +2,31 @@
 #
 #  Copyright (c) 2020 - Mad Penguin Consulting Ltd
 #
 #####################################################################################
 from __future__ import annotations
 from pathlib import Path
 from collections import UserDict
-from lmdb import Environment, Transaction as TXN, MapResizedError
+from lmdb import Environment, Transaction as TXN, MapResizedError, NotFoundError
 from typing import Optional, Generator, Dict, Callable, ClassVar, Tuple
 from orbit_database.doc import Doc
 from orbit_database.table import Table
 from orbit_database.audit import Auditor
 from orbit_database.serialiser import SerialiserType
 from orbit_database.compression import CompressionType
 from orbit_database.decorators import wrap_reader_yield, wrap_reader, WriteTransaction, transparent_resize
 from orbit_database.exceptions import NoSuchTable
 from orbit_database.types_ import Config
 from orbit_database.metadata import MetaData
+from orbit_database.catalog import Catalog, CatalogEntry
 
 try:
     from loguru import logger as log
 except Exception:  # pragma: no cover
-    from logging import log  # pragma: no cover
+    import logging as log  # pragma: no cover
 
 
 class Database(UserDict):
     """
     The Database object models the top-level container for a collection of tables and indexes, each Database
     object maps to an LMDB database object. When you open a database there are a variety of low-level (LMDB)
     database settings that can be applied, it's worth understanding what some of them do as when you come to
@@ -111,14 +112,18 @@
         
     def reset (self):
         self.meta = None
         self.auto_resize = False
         self._conf = dict(self.CONFIG)
         self._auditor = None
         self._auditing = None
+        # self._index_version = 1
+        # self._catalog = None
+        self._path = None
+        self._cat = None
         self._db = None
         self.env = None
         self.data = {}
 
     def __getitem__(self, name: str) -> Table:
         """
         Shortcut to self.table
@@ -147,15 +152,14 @@
               cls: Optional[Doc]=Doc,
               defer: Callable=False) -> Table:
         """
         Returns the table associated with the supplied name
 
         table_name - the name of the table to recover
         """
-        # log.debug(f'table [{table_name}] auditing={auditing}')
         if table_name not in self.data:
             cls.table = self.data[table_name] = Table(self, table_name, cls)
         if not defer:
             cls.table = self.data[table_name]
             if not self.data[table_name].isopen:
                 self.data[table_name].open(
                     codec=codec,
@@ -168,15 +172,15 @@
         return self.data[table_name]
 
     @property
     def isopen(self) -> bool:
         """
         Return True is the database is currently open
         """
-        return hasattr(self, '_db') and self._db
+        return True if hasattr(self, '_db') and self._db else False
 
     @property
     def map_size(self) -> int:
         """
         Return the currently mapped database size
         """
         return self.env.info()['map_size']
@@ -190,19 +194,15 @@
 
         txn - an optional transaction to wrap this operation
         """
         transaction = txn if isinstance(txn, TXN) else txn.txn
         total_bytes = 0
         results = {}
         for name in self.tables(all=True, txn=transaction):
-            close = name not in self.data
             used = self.table(name).storage_used()
-            # if close:
-            #     self.table(name).close()
-            #     del self.data[name]
             total_bytes += used
             results[name] = used
         return total_bytes, results
 
     @property
     def storage_allocated(self):
         """
@@ -217,23 +217,37 @@
     def tables(self, all: bool=False, txn: Optional[TXN]=None) -> Generator[str, None, None]:
         """
         Generate a list of tables available in this database
 
         all - if True also show hidden / structural tables
         txn - an optional transaction
         """
-        transaction = txn if isinstance(txn, TXN) else txn.txn
-        with transaction.cursor(self._db) as cursor:
-            while cursor.next():
-                try:
-                    name = cursor.key().decode()
-                except UnicodeDecodeError:
-                    continue
-                if (name[0] not in ['_', '~']) or all:
-                    yield name
+        if self.index_version == 1:
+            transaction = txn if isinstance(txn, TXN) else txn.txn
+            with transaction.cursor(self._db) as cursor:
+                while cursor.next():
+                    try:
+                        name = cursor.key().decode()
+                    except UnicodeDecodeError:
+                        continue
+                    if (name[0] not in ['_', '~', '@']) or all:
+                        yield name
+        elif self.index_version == 2:
+            if all:
+                transaction = txn if isinstance(txn, TXN) else txn.txn
+                with transaction.cursor(self._db) as cursor:
+                    while cursor.next():
+                        try:
+                            name = cursor.key().decode()
+                        except UnicodeDecodeError:
+                            continue
+                        if name.startswith('@@'):
+                            yield name
+            for result in self.table('@@catalog@@').filter():
+                yield result.oid.decode()
 
     def sync(self, force: bool=True) -> None:
         """
         Force a database sync
 
         force - if True make the flush synchronous
         """
@@ -241,14 +255,18 @@
 
     # @property
     # def name(self):
     #     """Return the unique name (uuid) of this database for replication"""
     #     return self.replication.uuid
 
     @property
+    def index_version (self) -> int:
+        return self._cat.version if self._cat else 0
+
+    @property
     def write_transaction(self) -> TXN:
         """Return a write-transaction for this database"""
         return WriteTransaction(self)
 
     @property
     def read_transaction(self) -> TXN:
         """
@@ -265,29 +283,24 @@
         Adjust the database configuration
         Return a reference to the current database instance
         """
         if not config:
             config = {}
         else:
             config = dict(config)
-
-        # if 'replication' in config:
-        #     self.replication.enabled = config.get('replication', False)
-        # else:
-        #     self.replication.enabled = config.get('journal', False)
-            
         if 'auditing' in config:
             self._auditing = config.get('auditing')
             del config['auditing']
             
         self.auto_resize = config.get('auto_resize', False)
 
-        for param in ['replication', 'journal', 'auto_resize', 'defer_fulltext', 'reindex', 'auditing']:
+        for param in ['replication', 'journal', 'auto_resize', 'defer_fulltext', 'reindex', 'auditing', 'version']:
             # log.debug(f'Setting: flag_{param} = {config.get(param, False)}')
-            setattr(self, f'flag_{param}', config.get(param, False))
+            if param in config:
+                setattr(self, f'flag_{param}', config.get(param, False))
             if param in config:
                 del config[param]
 
         self._conf = dict(self._conf, **config)
         return self
 
     def open(self, path: str, name: str=None) -> Database:
@@ -296,78 +309,55 @@
 
         path - the location of the database files
 
         Returns a reference to the Database object
         """
         if self.isopen:
             return self
-        # mapsize = self._conf.get('map_size', 0)
-        # if mapsize < 32768:
-        #     self._conf['map_size'] = 32768  # pragma: no cover
         self._path = path
         self._name = name
         self.env = Environment(path, **self._conf)
-
-        @transparent_resize
-        def openup(db, txn=None):
-            self._db = self.env.open_db()
+        self._cat = Catalog(getattr(self, 'flag_version', None))
+        self._db = self.env.open_db()
+        with TXN(env=self.env, write=True) as txn:
+            self._cat.open(self, txn=txn)
             self.meta = MetaData(self).open(txn=txn)
-            # self.replication.open(txn=txn)
-
-        openup(self)
-        # log.error(f"OPEN AUDIT: {self._auditing}")
         self._auditor = Auditor(self).open(self._auditing)
         return
 
     def close(self) -> None:
         """Close this database if it is open"""
-        # log.warning(f'Close: {self._auditor}')
         if self._auditor:
-            # log.error('1')
             self._auditor.close()
             self._auditor = None
-            # log.error('2')
-        
         if self.isopen:
             try:
-                # log.error('3')
                 for table_name in list(self.tables()):
-                    # log.error('4')
                     if table_name in self.data:
                         if self.data[table_name].isopen:
-                            # log.warning(f'Close: {table_name}')
                             self.data[table_name].close()
             except Exception as e:
                 log.warning(f'unable to close all tables: {str(e)}')
                 log.exception(e)
-        # if hasattr(self, 'replication'):
-        # log.warning("all closed")
-        #     self.replication.close()
         if hasattr(self, 'env') and self.env:
             self.env.close()
-        # log.warning("env closed")
         self.reset()
-        # self._conf = dict(self.CONFIG)
-        # self.replication = Replication(self)
-        # self.meta = None
-        # self._db = None
-        # self.env = None
-        # self.data = {}
 
     def reopen(self) -> None:
         """
         Reopen a database and all of it's tables
 
         After calling set_mapsize to resize the database, individual database handles
         are potentially invalidated, hence the save option is to reopen everything.
         """
         @transparent_resize
         def openup(db, txn=None):
             self._db = self.env.open_db()
-            self.meta.reopen(txn=txn)
+            if self.meta:
+                self.meta.reopen(txn=txn)
 
         # self.open(self._path)
         openup(self)
         for table_name, table in self.data.items():
             table.reopen()
 
     def drop(self, name: str, txn: Optional[TXN]=None) -> None:
```

### Comparing `orbit_database-0.99.91/orbit_database/decorators.py` & `orbit_database-1.0.0/orbit_database/decorators.py`

 * *Files 7% similar despite different names*

```diff
@@ -112,15 +112,15 @@
                 del kwargs['txn']
             while True:
                 try:
                     with Transaction(env=args[0].env) as txn:
                         yield from func(*args, **kwargs, txn=txn)
                         return
                 except MapResizedError:
-                    args[0].env.set_mapsize(0)                         # pragma: no cover
+                    args[0].env.set_mapsize(0) # pragma: no cover
     return wrapped
 
 
 def wrap_reader(func: Callable) -> Callable:
     @functools.wraps(func)
     def wrapped(*args, **kwargs) -> Any:
         if kwargs.get('txn'):
@@ -129,9 +129,29 @@
             if 'txn' in kwargs:
                 del kwargs['txn']
             while True:
                 try:
                     with Transaction(env=args[0].env) as txn:
                         return func(*args, **kwargs, txn=txn)
                 except MapResizedError:
-                    args[0].env.set_mapsize(0)                         # pragma: no cover
+                    args[0].env.set_mapsize(0) # pragma: no cover
     return wrapped
+
+
+def wrap_writer(func: Callable) -> Callable:
+    @functools.wraps(func)
+    def wrapped(*args, **kwargs) -> Any:
+        if kwargs.get('txn'):
+            return func(*args, **kwargs)
+        else:
+            if 'txn' in kwargs:
+                del kwargs['txn']
+            while True:
+                try:
+                    with WriteTransaction(getattr(args[0], '_database', args[0])) as txn:
+                        return func(*args, **kwargs, txn=txn)
+                except MapResizedError:
+                    args[0].env.set_mapsize(0) # pragma: no cover
+    return wrapped
+
+
+
```

### Comparing `orbit_database-0.99.91/orbit_database/doc.py` & `orbit_database-1.0.0/orbit_database/doc.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 #####################################################################################
 from __future__ import annotations
 from enum import Enum
 from typing import TYPE_CHECKING, Any, Optional, KeysView, ItemsView, ValuesView, Dict, List
 from lmdb import Transaction as TXN
 from struct import pack, unpack
 from orbit_database.objectid import ObjectId
+
 try:
     from loguru import logger as log
 except ModuleNotFoundError:
     import logging as log
-    log.info("OK")
 
 if TYPE_CHECKING:
     from .table import Table  # pragma: no cover
 
 
 class JournalType(Enum):
     """
@@ -300,7 +300,9 @@
     def doc_with_id(self) -> Dict[str, Any]:
         """
         Return the new buffer as a dictionary, i.e. the old + updates
         """
         if isinstance(self.dat, dict) and isinstance(self.upd, dict):
             return dict(self.dat, **self.upd, _id=self.key)
         return self.upd or self.dat
+
+
```

### Comparing `orbit_database-0.99.91/orbit_database/exceptions.py` & `orbit_database-1.0.0/orbit_database/exceptions.py`

 * *Files identical despite different names*

### Comparing `orbit_database-0.99.91/orbit_database/filterresult.py` & `orbit_database-1.0.0/orbit_database/filterresult.py`

 * *Files identical despite different names*

### Comparing `orbit_database-0.99.91/orbit_database/index.py` & `orbit_database-1.0.0/orbit_database/index.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 if TYPE_CHECKING:
     from .table import Table  # pragma: no cover
 
 try:
     from loguru import logger as log
 except Exception:  # pragma: no cover
-    from logging import log  # pragma: no cover
+    import logging as log  # pragma: no cover
 
 
 class Index(InvertedWordIndex):
     """
     The Index class models individual indexes of which a table may have zero or more. There
     are two crucial parameters supplied when setting up an index and are passed via "conf".
 
@@ -45,39 +45,46 @@
         """
         self._table = table
         self._conf = dict(conf)
         self.env = table.env
         self.name = name
         self._db = None
         self._writer = None
+        self._lower = False
         self.func = func = self._conf.get('func')
 
         if func:
             if func[:4] == 'def ':
                 self._func = self.anonymous_full(func)
             else:
                 if self._conf.get('lower'):
+                    self._lower = True
                     skel = '(r): return "{}".format(**r).lower().encode()'
                 else:
                     skel = '(r): return "{}".format(**r).encode()'
                 self._func = self.anonymous(skel.format(self._conf.get('func')))
         self.duplicates = self._conf.get('dupsort', False)
         self._conf.pop('func', None)
         self._conf.pop('lower', None)
         super().__init__()
 
+    @property
+    def metadata (self):
+        return dict(self._conf, **{'func': self.func})
+
     def open(self, txn: TXN) -> None:
         """
         Open the index and make it available to the table
 
         txn = an optional transaction
         """
+        if self._iwx:
+            return super().open(txn)
         options = dict(self._conf, **{'key': self._conf['key'].encode()})
         self._db = self.env.open_db(**options, txn=txn)
-        super().open(txn)
 
     @wrap_reader
     def records(self, txn: Optional[TXN]=None) -> int:
         """
         Return the number of records in this index
 
         txn - an optional transaction
@@ -96,15 +103,15 @@
         old_doc - the previous version of the record
         new_doc - the new version of the record
         txn - an optional transaction
         """
         if not super().save(old_doc, new_doc, txn):
             try:
                 old_key = self._func(old_doc.doc)
-            except (KeyError, TypeError):  # pragma: no cover
+            except (AttributeError, KeyError, TypeError):  # pragma: no cover
                 old_key = []  # pragma: no cover
             try:
                 new_key = self._func(new_doc.doc)
             except (AttributeError, KeyError, TypeError):
                 new_key = []
                 # log.error(f'bad key, index={self.name} table={self._table.name} / {e} / {new_doc.doc}')
                 # log.error(f'old={old_key} new={new_key}')
@@ -172,14 +179,15 @@
                             if not self.duplicates:
                                 # log.error(f'duplicate on table={self._table.name} index={self.name} key={keys}')
                                 raise DuplicateKey(f'trying to add key "{key}"')
                     except BadValsizeError:
                         log.error(f'key error: {keys} / {self.name}')
                         raise
 
+
     def put_cursor(self, cursor: Cursor, txn: TXN) -> None:
         """
         Put a new index entry based on a Cursor rather than a Doc object. This is here
         mainly to make "reindex" more elegant / readable.
 
         cursor - an LMDB Cursor object
         txn - an optional transaction
@@ -217,27 +225,27 @@
     def empty(self, txn: TXN) -> None:
         """
         Remove all entries from this index
 
         txn - an optional transaction
         """
         transaction = txn if isinstance(txn, TXN) else txn.txn
-        super().empty(transaction)
-        transaction.drop(self._db, delete=False)
+        if not super().empty(transaction):
+            transaction.drop(self._db, delete=False)
 
     def drop(self, txn: TXN) -> None:
         """
         Remove all entries from this index and then remove the index
 
         txn - an optional transaction
         """
         transaction = txn if isinstance(txn, TXN) else txn.txn
-        super().drop(transaction)
-        transaction.drop(self._db, delete=True)
-        self._table._meta.remove_index(self._table.name, self.name, txn=txn)
+        if not super().drop(transaction):
+            transaction.drop(self._db, delete=True)
+            self._table._meta.remove_index(self._table.name, self.name, txn=txn)
 
     def map_key(self, doc: Doc) -> str:
         """
         Return the key derived from the supplied record for this particular index
 
         doc - the record from which we want to derive a key
         """
```

### Comparing `orbit_database-0.99.91/orbit_database/invertedwordindex.py` & `orbit_database-1.0.0/orbit_database/invertedwordindex.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,18 +8,19 @@
 #   a. Lookup by word (inverted index)
 #   b. Lookup by document (forward index)
 #
 #   (a) Will use raw LMDB duplicate indexes, whereas (b) will be a sparse bitmap index
 #
 from collections import Counter
 from struct import pack, unpack
-from lmdb import Transaction, Cursor
+from lmdb import Transaction, Cursor, BadValsizeError
 from typing import List
 from orbit_database.doc import Doc
 from orbit_database.bitmap import Bitmap
+from orbit_database.decorators import wrap_writer
 from ujson import loads, dumps
 from functools import wraps
 from time import time
 from os import times
 
 try:
     from loguru import logger as log
@@ -40,23 +41,43 @@
         """
         config = getattr(self, '_conf', config or {})
         self._iwx = config.get('iwx')
         self._iwx_cache = None
         for token in dict(config):
             if token in self.REMOVE_TOKENS:
                 del config[token]
+        self._lexicon = None
+        self._docindx = None
+        self._docrindx = None
+        self._bitmap = None
+        self._words = None
+        self._map = None
 
     def open(self, txn: Transaction) -> None:
         if self._iwx:
-            self._lexicon = self.env.open_db(key=self.iwx_path('lexicon'), txn=txn)
-            self._docindx = self.env.open_db(key=self.iwx_path('docindx'), txn=txn)
-            self._docrindx = self.env.open_db(key=self.iwx_path('docrindx'), txn=txn)
-            self._bitmap = self.env.open_db(key=self.iwx_path('bitmap'), txn=txn)
-            self._words = self.env.open_db(key=self.iwx_path('words'), txn=txn)
+            if not hasattr(self, 'name') or self._table._database.index_version == 1:
+                self._lexicon = self.env.open_db(key=self.iwx_path('lexicon'), txn=txn)
+                self._docindx = self.env.open_db(key=self.iwx_path('docindx'), txn=txn)
+                self._docrindx = self.env.open_db(key=self.iwx_path('docrindx'), txn=txn)
+                self._bitmap = self.env.open_db(key=self.iwx_path('bitmap'), txn=txn)
+                self._words = self.env.open_db(key=self.iwx_path('words'), txn=txn)
+            else:
+                index_name = self.name
+                table_name = self._table.name
+                catalog = self._table._database._cat
+                conf = catalog.get_metadata(table_name, index_name, txn=txn)
+                self._lexicon = self.env.open_db(conf['lexicon'].encode(), txn=txn)
+                self._docindx = self.env.open_db(conf['docindx'].encode(), txn=txn)
+                self._docrindx = self.env.open_db(conf['docrindx'].encode(), txn=txn)
+                self._bitmap = self.env.open_db(conf['bitmap'].encode(), txn=txn)
+                self._words = self.env.open_db(conf['words'].encode(), txn=txn)
+
             self._map = Bitmap(self._bitmap)
+            return True
+        return False
 
     def empty(self, txn: Transaction) -> None:
         if not self._iwx:
             return False
         return self.iwx_empty(txn, False)
 
     def drop(self, txn: Transaction) -> None:
@@ -103,101 +124,107 @@
     def write(self, oid: str, words: List[dict], txn: Transaction):
         transaction = txn if isinstance(txn, Transaction) else txn.txn
         if not words:
             lexicon = Lexicon(self).from_oid(oid, transaction=transaction)
         else:
             lexicon = Lexicon(self).from_words(oid, words, transaction=transaction)
         lexicon.update_words(transaction=transaction)
+        if words:
+            txn.put(oid, dumps(words).encode(), db=self._words)
 
     def iwx_counts(self, txn: Transaction):
+        txn = txn if isinstance(txn, Transaction) else txn.txn
         return {
-            'lexicon': txn.stat(self._lexicon).get('entries', 0),
-            'docindx': txn.stat(self._docindx).get('entries', 0),
-            'docrindex': txn.stat(self._docrindx).get('entries', 0),
-            'bitmap': txn.stat(self._bitmap).get('entries', 0),
-            'words': txn.stat(self._words).get('entries', 0)
+            'lexicon':  txn.stat(self._lexicon).get('entries', 0),
+            'docindx':  txn.stat(self._docindx).get('entries', 0),
+            'docrindx': txn.stat(self._docrindx).get('entries', 0),
+            'bitmap':   txn.stat(self._bitmap).get('entries', 0),
+            'words':    txn.stat(self._words).get('entries', 0)
         }
 
+    def iwx_empty_words(self, txn: Transaction, delete=False) -> None:
+        if self._iwx:
+            txn = txn if isinstance(txn, Transaction) else txn.txn
+            txn.drop(self._words, delete=False)
+            return True
+        return False
+
     def iwx_empty(self, txn: Transaction, delete=False) -> None:
         if self._iwx:
+            txn = txn if isinstance(txn, Transaction) else txn.txn
             txn.drop(self._lexicon, delete=delete)
+            txn.drop(self._bitmap, delete=delete)
             txn.drop(self._docindx, delete=delete)
             txn.drop(self._docrindx, delete=delete)
-            txn.drop(self._bitmap, delete=delete)
+            return True
         return False
 
     def iwx_path(self, name: str) -> str:
         """
         Produce the path for a supplementary table
         """
         if hasattr(self, '_table'):
             return f'_{self._table.name}={self.name}={name}'.encode()
         else:
             return f'_pytest=pytest={name}'.encode()
 
     def iwx_oids(self, txn: Transaction):
         return txn.stat(self._docindx).get('entries', 0)
 
-    # def lookup_word(self, word: str, txn: Transaction):
-    #     if len(word) > self.MAX_WORD_SIZE:
-    #         return None
-    #     item = txn.get(word, db=self._lexicon)
-    #     if item:
-    #         return unpack('>LL', item)[0]
-    #     stat = txn.stat(db=self._lexicon)
-    #     indx = stat['entries'] + 1
-    #     try:
-    #         txn.put(word, pack('>LL', indx, 0), db=self._lexicon)
-    #         return indx
-    #     except Exception as e:
-    #         log.error(e)
-    #         return None
-
     def resolve_idoc(self, idoc, txn):
         key = pack('>L', idoc)
         doc = txn.get(key, db=self._docrindx)
         if not doc:
             return None
         return doc
 
-    # def lookup_document(self, oid, txn: Transaction):
-    #     item = txn.get(oid, db=self._docindx)
-    #     if item:
-    #         return unpack('>L', item)[0]
-    #     stat = txn.stat(db=self._docindx)
-    #     indx = stat['entries'] + 1
-    #     try:
-    #         txn.put(oid, pack('>L', indx), db=self._docindx)
-    #         txn.put(pack('>L', indx), oid, db=self._docrindx)
-    #         return indx
-    #     except Exception as e:
-    #         log.error(e)
-    #         return None
-
     def iwx_get_words(self, oid):
         with self.env.begin(db=self._words) as txn:
             raw = txn.get(oid, db=self._words)
             return loads(raw) if raw else []
 
     def iwx_put_words(self, oid, words):
         with self.env.begin(db=self._words, write=True) as txn:
-            txn.put(oid, dumps(words).encode(), db=self._words)
+            try:
+                txn.put(oid, dumps(words).encode(), db=self._words)
+            except BadValsizeError:
+                log.error(f'issue with key or words, key={oid} words={words}')
+                log.error('record not indexed!!')
 
- 
     def iwx_space(self, stat, suffix='B'):
         num = stat['psize'] * (stat['leaf_pages'] + stat['branch_pages'] + stat['overflow_pages'] + 2)
         for unit in ['','Ki','Mi','Gi','Ti','Pi','Ei','Zi']:
             if abs(num) < 1024.0:
                 return "%3.1f%s%s" % (num, unit, suffix)
             num /= 1024.0
         return "%.1f%s%s" % (num, 'Yi', suffix)
 
     def iwx_stat_format(self, name, stat):
         return f'{name:10} records={stat["entries"]:10} size={self.iwx_space(stat):>10}'
 
+    def iwx_analysis(self, txn: Transaction):
+        txn = txn if isinstance(txn, Transaction) else txn.txn
+        return {
+            'lexicon':  self.iwx_space(txn.stat(self._lexicon)),
+            'docindx':  self.iwx_space(txn.stat(self._docindx)),
+            'docrindx': self.iwx_space(txn.stat(self._docrindx)),
+            'bitmap':   self.iwx_space(txn.stat(self._bitmap)),
+            'words':    self.iwx_space(txn.stat(self._words))
+        }
+
+    def dump_words (self):
+        count = 0
+        with self.env.begin(db=self._words) as txn:
+            cursor = txn.cursor()
+            while cursor.next():
+                print(cursor.key(), cursor.value())
+                count += 1
+                if count == 5:
+                    break
+
     def dump(self, debug=False):
         lexicon = []
         if debug:
             print('Lexicon')
             print(f'+----------------------+----------+----------+')
             print(f'| Word                 |    Index |     Freq |')
             print(f'+----------------------+----------+----------+')
@@ -208,14 +235,37 @@
                 index, count = unpack('>LL', cursor.value())
                 lexicon.append([key, count])
                 if debug:
                     print(f'| {key.strip():20} | {index:8} | {count:8} |')
         if debug:
             print(f'+----------------------+----------+----------+')
 
+        # print('Index')
+        # print(f'+------------------------------+----------+')
+        # print(f'| Doc Id                       |    Index |')
+        # print(f'+------------------------------+----------+')
+        # with self.env.begin(db=self._docindx) as txn:
+        #     cursor = txn.cursor()
+        #     while cursor.next():
+        #         key = cursor.key().decode()
+        #         index = unpack('>L', cursor.value())[0]
+        #         print(f'| {key.strip():20} | {index:8} |')
+        # print(f'+------------------------------+----------+')
+
+        # print('RIndex')
+        # print(f'+----------+------------------------------+')
+        # print(f'| Index    | Doc Id                       |')
+        # print(f'+----------+------------------------------+')
+        # with self.env.begin(db=self._docrindx) as txn:
+        #     cursor = txn.cursor()
+        #     while cursor.next():
+        #         key = unpack('>L', cursor.key())[0]
+        #         index = cursor.value().decode()
+        #         print(f'| {key:8} | {index:20} |')
+        # print(f'+----------+-----------------------------+')
         return {'lexicon': lexicon}
 
     def iwx_lexicon(self, terms, max, txn=None):
         """Recover a list of matches from the Lexicon based on 'term'"""
         words = []
         if not len(terms):
             return []
@@ -329,28 +379,23 @@
             return document_index
         except Exception as e:
             log.error(e)
             return None
 
     def update_words(self, transaction):
         document_index = self.lookup_document(self._oid, transaction)
-        # words = Counter(self._words)
         for word in self._words:
             if word:
                 word_index = self.lookup_word(word.encode(), transaction)
                 if not word_index:
-                    log.debug(f'word index fail for {word}')
                     continue
                 word_index, count = unpack('>LL', transaction.get(word.encode(), db=self._table_lexicon))
                 transaction.put(word.encode(), pack('>LL', word_index, count + self._words[word]), db=self._table_lexicon)
                 self._map.update(word_index, document_index, True, transaction=transaction)
             
     def delete(self, transaction):
         transaction.delete(self._oid, db=self._table_words)
         document_index = self.lookup_document(self._oid, transaction=transaction)
-        transaction.delete(self._oid, db=self._table_index)
-        transaction.delete(pack(">L", document_index), db=self._table_rindex)
-        # words = Counter(self._words)
         for word in self._words:
             word_index, count = unpack('>LL', transaction.get(word.encode(), db=self._table_lexicon))
             transaction.put(word.encode(), pack('>LL', word_index, count - self._words[word]), db=self._table_lexicon)
             self._map.update(word_index, document_index, False, transaction=transaction)
```

### Comparing `orbit_database-0.99.91/orbit_database/manager.py` & `orbit_database-1.0.0/orbit_database/manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from typing import Optional
 from orbit_database.database import Database
 from orbit_database.types_ import Config
 
 try:
     from loguru import logger as log
 except Exception:  # pragma: no cover
-    from logging import log  # pragma: no cover
+    import logging as log  # pragma: no cover
 
 
 class Manager(UserDict):
     """
     Manager is a dictionary like object the holds references to all the databases currently
     registered with the running instance. If you only ever reference one database then
     technically you can skip this object and just use the Database object.
@@ -64,22 +64,23 @@
         config - a dictionary containing configuration specifics for this database
 
         Returns a reference to an open Database
         """
         # log.debug(f'database auditing={auditing}')
         if name in self.data:
             database = self.data[name]
-            if not database.isopen:
-                database.open(database._path)
-            return database
+            if database.isopen:
+                return database
         if name and not path:
             path = name
             name = None
             if path in self._paths:
-                return self._paths[path]
+                database = self._paths[path]
+                if database.isopen:
+                    return database
         database = Database()
         database.configure(config)
         if not name:
             name = path
         database.open(path, name=name)
         self.data[name] = database
         self._paths[path] = database
```

### Comparing `orbit_database-0.99.91/orbit_database/metadata.py` & `orbit_database-1.0.0/orbit_database/metadata.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,18 @@
 from __future__ import annotations
 from struct import pack, unpack
 from typing import TYPE_CHECKING, Tuple, Generator
 from lmdb import Transaction as TXN
 from orbit_database.doc import Doc
 from orbit_database.decorators import wrap_reader_yield, wrap_reader, transparent_resize, WriteTransaction
 
+try:
+    from loguru import logger as log
+except Exception:  # pragma: no cover
+    import logging as log  # pragma: no cover
 
 if TYPE_CHECKING:
     from .database import Database  # pragma: no cover
 
 
 class MetaData:
     """
@@ -46,16 +50,22 @@
     def open(self, txn: TXN=None):
         """
         Open the __metadata__ table and make it available for IO
         """
         if self._table:
             return self  # pragma: no cover
 
+        if self._database.index_version == 1:
+            metadata_name = '__metadata__'
+        elif self._database.index_version == 2:
+            metadata_name = '@@metadata@@'
+        else:
+            raise Exception(f'no index version: {self._database.index_version}')
         transaction = txn if isinstance(txn, TXN) else txn.txn
-        self._table = self._database.table('__metadata__', txn=transaction)
+        self._table = self._database.table(metadata_name, txn=transaction)
         return self
 
     def reopen(self, txn: TXN=None):
         """
         Re-Open the __metadata__ table and make it available for IO
         """
         self._table.reopen(txn=txn)
@@ -280,7 +290,39 @@
         Remove a key, used to remove database specific information.
 
         key - the key of the information to remove
         txn - a write transaction to wrap the operation
         """
         transaction = txn if isinstance(txn, TXN) else txn.txn
         transaction.delete(key.encode(), db=self._table._db)
+
+    # def migrateIndecies (self, txn: TXN=None):
+    #     version = self.fetch_int('index_version', txn=txn)
+    #     if not version:
+    #         log.warning('Upgrading indecies to version # 1')
+    #         rename = []
+    #         transaction = txn if isinstance(txn, TXN) else txn.txn
+    #         with transaction.cursor(self._database._db) as cursor:
+    #             while cursor.next():
+    #                 try:
+    #                     table_name = cursor.key().decode()
+    #                 except UnicodeDecodeError:
+    #                     continue
+    #                 if (table_name[0] not in ['_', '~']):
+    #                     index_key = f'_{table_name}_'
+    #                     offset = len(index_key)
+    #                     with transaction.cursor(db=self._database._db) as sub:
+    #                         sub.set_range(index_key.encode())
+    #                         name = sub.key().decode()
+    #                         while name.startswith(index_key):
+    #                             rename.append((name, f'_{table_name}|{name[offset:]}'))
+    #                             if not sub.next():
+    #                                 break
+    #                             name = sub.key().decode()
+    #         for entry in rename:
+    #             log.warning(f'Rename: {entry[0]} => {entry[1]}')
+    #             with transaction.cursor(db=self._database._db) as cursor:
+    #                 cursor.get(entry[1].encode())
+    #                 cursor.delete(entry[1].encode())
+                    
+    #                 # cursor.replace(entry[1].encode(), cursor.value())
+    #                 break
```

### Comparing `orbit_database-0.99.91/orbit_database/objectid.py` & `orbit_database-1.0.0/orbit_database/objectid.py`

 * *Files identical despite different names*

### Comparing `orbit_database-0.99.91/orbit_database/serialiser.py` & `orbit_database-1.0.0/orbit_database/serialiser.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,16 +14,15 @@
 from json import loads, dumps
 from orbit_database.doc import Doc
 from orbit_database.exceptions import InvalidSerialiser
 
 try:
     from loguru import logger as log
 except Exception:  # pragma: no cover
-    from logging import log  # pragma: no cover
-
+    import logging as log  # pragma: no cover
 
 try:
     import ujson
 except Exception:   # pragma: no cover
     pass            # pragma: no cover
 
 try:
```

### Comparing `orbit_database-0.99.91/orbit_database/table.py` & `orbit_database-1.0.0/orbit_database/table.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,24 +12,25 @@
 from orbit_database.index import Index
 from orbit_database.doc import Doc, JournalType
 from orbit_database.compression import Compression, CompressionType
 from orbit_database.serialiser import Serialiser, SerialiserType
 from orbit_database.cursor import Cursor
 from orbit_database.objectid import ObjectId
 from orbit_database.filterresult import FilterResult, MatchResult
-from orbit_database.decorators import wrap_reader, wrap_reader_yield, WriteTransaction, ReadTransaction, transparent_resize
+from orbit_database.decorators import wrap_reader, wrap_reader_yield, WriteTransaction, wrap_writer
 from orbit_database.exceptions import IndexAlreadyExists, DocumentDoesntExist, InvalidKeySpecifier, NoSuchIndex
 from orbit_database.types_ import Config, OID, OIDS
 from pathlib import Path
 from operator import gt as greater, lt as less
+from json import load, dump
 
 try:
     from loguru import logger as log
 except Exception:  # pragma: no cover
-    from logging import log  # pragma: no cover
+    import logging as log  # pragma: no cover
 
 
 ZERO = 0
 
 
 if TYPE_CHECKING:
     from .database import Database  # pragma: no cover
@@ -64,14 +65,15 @@
         name - the name of the table to reference
         """
         self.name = name
         self.env = database.env
         self._database = database
         self._cls = cls
         self._db = None
+        self._oid = None
         self._meta = database.meta
         UserDict.__init__(self)
         Compression.__init__(self)
 
     def __setitem__(self, name: str, conf: Config) -> None:
         """
         Create an entry for an index with the specified name
@@ -87,32 +89,44 @@
         """
         Generate a string representation of this object, by default we include the
         table name and the table status, i.e. whether it is open or not.
         """
         return f'<{__name__}.Table instance> name="{self.name}" status={"open" if self.isopen else "closed"}'
 
     @property
+    def oid (self) -> ObjectId:
+        return self._oid
+
+    @property
     def isopen(self) -> bool:
         """
         Return True if this table is open
         """
         return False if self._db is None else True
 
     @wrap_reader
     def records(self, txn: Optional[TXN]=None) -> int:
         """
         Return the number of records in this table
 
         txn - an transaction to wrap the operation
         """
         transaction = txn if isinstance(txn, TXN) else txn.txn
-        # log.error(f'DB={self._db.flags()} Path={self.env.path()}')
-        # log.error(self.name)
         return transaction.stat(self._db).get('entries', 0)
 
+    @wrap_reader
+    def stat(self, txn: Optional[TXN]=None) -> int:
+        """
+        Get the stat() buffer for this table
+
+        txn - an transaction to wrap the operation
+        """
+        transaction = txn if isinstance(txn, TXN) else txn.txn
+        return transaction.stat(self._db)
+
     @property
     def read_transaction(self) -> TXN:
         """
         Use with "with" to begin a Read-Only transaction
         """
         # return ReadTransaction(self._database)
 
@@ -133,15 +147,15 @@
         Return the amount of storage space used by data contained within this table
 
         txn - optional transaction to wrap this operation
         """
         stat = txn.stat(self._db)
         return stat['psize'] * (stat['leaf_pages'] + stat['branch_pages'] + stat['overflow_pages'] + 2)
 
-    @transparent_resize
+    @wrap_writer
     def open(
             self,
             compression_type: Optional[CompressionType]=CompressionType.NONE,
             compression_level: Optional[int]=None,
             codec: SerialiserType=SerialiserType.NONE,
             integerkey: int=False,
             compress_existing: bool=False,
@@ -164,83 +178,106 @@
         transaction = txn if isinstance(txn, TXN) else txn.txn
         create = False
         self._compression_type = compression_type
         self._compression_level = compression_level
         self._codec = codec
         self.integerkey = integerkey
         self._auditing = auditing
+
+        if not self.name.startswith('@@') and self._database.index_version == 2:
+            self._oid = name = self._database._cat.get_table_id(self.name, txn)
+        else:
+            self._oid = self.name
+
         try:
             self._db = self.env.open_db(
-                self.name.encode() if isinstance(self.name, str) else self.name,
+                # self.name.encode() if isinstance(self.name, str) else self.name,
+                self._oid.encode(),
                 create=False,
                 integerkey=integerkey,
                 txn=transaction)
         except NotFoundError:
             create = True
             self._db = self.env.open_db(
-                self.name.encode(),
+                # self.name.encode(),
+                self._oid.encode(),
                 integerkey=integerkey,
                 txn=transaction)
         except IncompatibleError as e:
-            log.error(f'{self.name}:: {str(e)}')
+            log.error(f'{self.name} => {self._oid}:: {str(e)}')
             return self
 
         try:
             Serialiser.__init__(self, codec, txn=transaction)
             if not self._meta:
                 return self
             for index_name in self.indexes(txn=transaction):
                 if index_name in self.data:
                     # means the index is open so we're doing a 're-open'
                     self.data[index_name].open(txn=transaction)  # pragma: no cover
                 else:
-                    doc = self._meta.fetch_index(self.name, index_name, txn=transaction)
-                    if not doc['conf']:
-                        break  # pragma: no cover
-                    self.__setitem__(index_name, doc['conf'])
+                    if self._database.index_version == 1:
+                        doc = self._meta.fetch_index(self.name, index_name, txn=transaction)
+                        if not doc['conf']:
+                            break  # pragma: no cover
+                        self.__setitem__(index_name, doc['conf'])
+                    else:
+                        # log.success(f'get meta: {self.name}/{index_name} => {self._database._cat.get_metadata(self.name, index_name)}')
+                        self.__setitem__(index_name, self._database._cat.get_metadata(self.name, index_name))
+                    
                     self.data[index_name].open(txn=transaction)
             if compression_type and compression_type != CompressionType.NONE:
                 do_compress = self.compression_select(compression_type, compression_level, txn=transaction)
                 Compression.open(self, txn=transaction)
                 if compress_existing and do_compress and self.records(txn=transaction):
                     self.compress_existing_data(txn=transaction)
             else:
                 Compression.open(self, txn=transaction)
-
-            # if create and self.replicated(txn):
-            #     doc = Doc({
-            #         'compression_type': compression_type.value,
-            #         'compression_level': compression_level,
-            #         'codec': codec.value
-            #     })
-            #     txn.journal.append(doc.journal_entry(JournalType.CREATE, self.name))
             if auditing:
                 self._database._auditor.watch(self.name, callback)
             
         except Exception:
             try:
                 self.close()  # pragma: no cover
             except Exception:  # pragma: no cover
                 pass
             raise
 
         return self
 
+    @wrap_writer
+    def droptable(self, txn: Optional[TXN|WriteTransaction]=None) -> None:
+        """
+        Drop the current table, this will empty the table, remove all the indexes,
+        remote the table itself, and remove all associated metadat.
+
+        txn - a write transaction to wrap this operation
+        """
+        transaction = txn if isinstance(txn, TXN) else txn.txn
+        for index_name in self.data:
+            self.data[index_name].drop(txn=txn)
+
+        transaction.drop(self._db, True)
+        self._database._cat.drop(self.name, txn)
+        # if self._database.index_version == 2:
+        #     self._database._catalog.delete(self.name, txn=txn)
+        self._meta.remove(self.name, txn=txn)
+
     def close(self) -> None:
         """
         Close a table by essentially losing all references to it
         """
         # log.error(f'close table: {self.name}')
         # if self._database._auditor:
         #     self._database._auditor.close()
         self._db = None
         self.data.clear()
         Compression.close(self)
 
-    @transparent_resize
+    @wrap_writer
     def reopen(
         self,
         auditing: bool=False,
         callback: Callable=None,
         txn: Optional[TXN|WriteTransaction]=None) -> None:
         """
         ReOpen a table, used following a change to the map size. Everything should be the
@@ -253,56 +290,45 @@
             self._compression_level,
             self._codec,
             self.integerkey,
             auditing = auditing,
             callback = callback,
             txn=txn)
 
-    @transparent_resize
-    def droptable(self, txn: Optional[TXN|WriteTransaction]=None) -> None:
-        """
-        Drop the current table, this will empty the table, remove all the indexes,
-        remote the table itself, and remove all associated metadat.
-
-        txn - a write transaction to wrap this operation
-        """
-        transaction = txn if isinstance(txn, TXN) else txn.txn
-        for index_name in self.data:
-            self.data[index_name].drop(txn=txn)
-        transaction.drop(self._db, True)
-
-        # if self.replicated(txn):
-        #     doc = Doc({
-        #         'delete': True
-        #     })
-        #     txn.journal.append(doc.journal_entry(JournalType.REMOVE, self.name))
-
-        self._meta.remove(self.name, txn=txn)
-
     @wrap_reader_yield
     def indexes(self, txn: Optional[TXN]=None) -> Generator[str, None, None]:
         """
         Generate a list if indexs (names) available for this table
 
         txn - an optional transaction
         """
+        if self.name.startswith('@@'):
+            return []
         transaction = txn if isinstance(txn, TXN) else txn.txn
-        metadata = self._database.table('__metadata__', txn=transaction)
-        index_key = Index.index_path(self.name, '')
-        offset = len(index_key)
-        with transaction.cursor(db=metadata._db) as cursor:
-            cursor.set_range(index_key.encode())
-            name = cursor.key().decode()
-            while name.startswith(index_key):
-                yield name[offset:]
-                if not cursor.next():
-                    break  # pragma: no cover
+        if self._database.index_version == 1:
+            metadata = self._database.table('__metadata__', txn=transaction)
+            index_key = Index.index_path(self.name, '')
+            offset = len(index_key)
+            with transaction.cursor(db=metadata._db) as cursor:
+                cursor.set_range(index_key.encode())
                 name = cursor.key().decode()
+                while name.startswith(index_key):
+                    yield name[offset:]
+                    if not cursor.next():
+                        break  # pragma: no cover
+                    name = cursor.key().decode()
+        elif self._database.index_version == 2:
+            for name in self._database._cat.indexes(self.name, transaction):
+                yield name
+            # catalog = self._database._catalog.get(self.name, txn=transaction)
+            # for name in catalog._indexes or []:
+            #     yield name
+
 
-    @transparent_resize
+    @wrap_writer
     def ensure(
             self,
             index_name: str,
             func: str=None,
             duplicates: bool=False,
             force: bool=False,
             lower: bool=False,
@@ -351,100 +377,85 @@
         print('--')
         [print(person.doc) for person in people.find('by_age_fs')]
         print('--')
         [print(person.doc) for person in people.find('by_age_func')]
         ```
         """
         transaction = txn if isinstance(txn, TXN) else txn.txn
-        old_conf = self._meta.fetch_index(self.name, index_name, txn=transaction)
+        if self._database.index_version == 2 and iwx:
+            if index_name not in self.data or force:
+                if index_name in self.data:
+                    self.drop(index_name, txn=transaction)
+
+                catalog = self._database._cat.ensure(self.name, index_name, iwx, transaction)
+                conf = catalog._indexes[index_name]
+                self.__setitem__(index_name, conf)
+                self.data[index_name].open(txn=transaction)
+            return self.data[index_name]
+        #
+        #   Abstract get old conf
+        #   Abstract store_index
+        #
+
+        if self._database.index_version == 1:
+            old_conf = self._meta.fetch_index(self.name, index_name, txn=transaction)
+            if not old_conf._conf:
+                old_conf = {'key': Index.index_path(self.name, index_name)}
+            else:
+                old_conf = old_conf._conf
+        else:
+            old_conf = self._database._cat.get_metadata(self.name, index_name)
+            if not old_conf:
+                old_conf = { 'key': str(ObjectId()) }
+
         new_conf = {
-            'key': Index.index_path(self.name, index_name),
+            'key': old_conf['key'],
             'dupsort': duplicates,
             'create': True,
             'func': func,
             'iwx': iwx,
             'lower': lower
         }
-        # if force:
-        #     log.error(f'Force was set on: {self.name} / {index_name}')
-        force = old_conf._conf != new_conf or force
-        # if old_conf._conf != new_conf and old_conf.doc:
-        #     log.error(f'Index mismatch on: {self.name} / {index_name} / {old_conf.doc}')
+        force = old_conf != new_conf or force
         if index_name not in self.data or force:
             if index_name in self.data:
                 self.drop(index_name, txn=transaction)
             self.__setitem__(index_name, new_conf)
             self.data[index_name].open(txn=transaction)
             if force:
-                self._meta.store_index(self.name, index_name, Doc({'conf': new_conf}), txn=transaction)
+                if self._database.index_version == 1:
+                    self._meta.store_index(self.name, index_name, Doc({'conf': new_conf}), txn=transaction)
+                else:
+                    self._database._cat.store_index(self.name, index_name, new_conf, txn=transaction)
                 self.reindex(index_name, progress=progress, txn=transaction)
         self.data[index_name].reindexed = force
         return self.data[index_name]
 
-        # if force and index_name in self.data:
-        #     self.drop(index_name, txn=transaction)
-        # if index_name in self.data:
-        #     return self.data[index_name]
-        # if iwx:
-        #     duplicates = True
-        # old_conf = self._meta.fetch_index(self.name, index_name, txn=transaction)
-        # index_path = Index.index_path(self.name, index_name)
-        # conf = {
-        #     'key': index_path,
-        #     'dupsort': duplicates,
-        #     'create': True,
-        #     'func': func,
-        #     'iwx': iwx,
-        #     'lower': lower
-        # }
-        # self.__setitem__(index_name, conf)
-        # self.data[index_name].open(txn=transaction)
-        # if conf != old_conf:
-        #     if self.replicated(txn):
-        #         doc = Doc({
-        #             'index_name': index_name,
-        #             'func': func,
-        #             'duplicates': duplicates,
-        #             'force': force,
-        #             'iwx': iwx,
-        #             'lower': lower
-        #         })
-        #         txn.journal.append(doc.journal_entry(JournalType.ENSURE, self.name))
-        #     self._meta.store_index(self.name, index_name, Doc({'conf': conf}), txn=transaction)
-        # if not self.data[index_name]._iwx:
-        #     self.reindex(index_name, progress=progress, txn=transaction)
-        # return self.data[index_name]
-
-    # def replicated(self, txn):
-    #     """Return True if the current transaction is going to be marked for replication"""
-    #     return isinstance(txn, WriteTransaction) and self._database.replication.enabled and self.name[0] != '_'
-
-    @transparent_resize
+    @wrap_writer
     def reindex(self, index_name: str, progress: Optional[Callable]=None, txn: Optional[TXN]=None) -> None:
         """
         Reindex the named index, assuming the index exists. The index is first emptied
         and then each record is reindexed, for a large table this can take some time
         and will lock the database while in progress.
 
         index_name - the name of the index to reindex
         txn - a write transaction to wrap the operation
         """
+        # log.warning(f'Running reindex for {index_name} in {self.name}')
         if index_name not in self.data:
             raise NoSuchIndex
-        # if self.data[index_name]._iwx:
-        #     raise Exception('unable to re-index inverted word indecies')
         transaction = txn if isinstance(txn, TXN) else txn.txn
         self.data[index_name].empty(txn=transaction)
         with transaction.cursor(self._db) as cursor:
             while cursor.next():
                 if progress:
                     progress.update(1)  # pragma: no cover
                 self.data[index_name].put_cursor(cursor, txn=transaction)
 
-    @transparent_resize
+    @wrap_writer
     def append(self, doc: Doc, txn: Optional[TXN|WriteTransaction]=None) -> Doc:
         """
         Append a new record to this table
 
         doc - the data to append
         txn - an optional transaction object
         """
@@ -456,23 +467,21 @@
                         oid = 0
                     else:
                         oid = unpack('=Q', cursor.key())[0] + 1
                     doc.oid = pack('=Q', oid)
             else:
                 doc.oid = str(ObjectId()).encode()
         transaction.put(doc.oid, self._compressor(doc), db=self._db)
-        # if self.replicated(txn):
-        #     txn.journal.append(doc.journal_entry(JournalType.APPEND, self.name))
         if self._auditing:
             self._database._auditor.append(self, doc, txn)
         for index_name in self.data:
             self.data[index_name].put(doc, txn=transaction)
         return doc
 
-    @transparent_resize
+    @wrap_writer
     def save(self, doc: Doc, txn: Optional[TXN, WriteTransaction]=None) -> None:
         """
         Update the current record in the table
 
         doc - the record to update
         txn - an optional transaction
         """
@@ -482,18 +491,14 @@
         old_doc = Doc(None, doc.oid).get(self, txn=transaction)
         if self._auditing:
             if old_doc:
                 self._database._auditor.save(self, old_doc, txn)
             else:
                 log.error(f'Audit: no old document for oid: {doc.oid}')
         transaction.put(doc.oid, self._compressor(doc), db=self._db)
-
-        # if self.replicated(txn):
-        #     txn.journal.append(doc.journal_entry(JournalType.UPDATE, self.name))
-
         for index_name in self.data:
             self.data[index_name].save(old_doc, doc, txn=transaction)
 
 
     @wrap_reader_yield
     def find(
             self,
@@ -543,15 +548,15 @@
         try:
             transaction = txn if isinstance(txn, TXN) else txn.txn
             return Doc(None, pack('=Q', oid) if self.integerkey else oid).get(self, txn=transaction)
         except Exception as e:  # pragma: no cover
             log.exception(e)  # pragma: no cover
             log.error(f'key was: {oid}')  # pragma: no cover
 
-    @transparent_resize
+    @wrap_writer
     def delete(self, keyspec: Union[OID, OIDS, Doc], txn: Optional[TXN]=None) -> None:
         """
         Delete one or more records from the database based on a key specification that
         should reference one or more records by primary key.
 
         keyspec - we accept either a key, a list of keys or a Doc, keys may be str or bytes
         txn - an optional transaction
@@ -583,15 +588,15 @@
                     self._database._auditor.delete(self, doc, txn)
 
                 for index_name in self.data:
                     self.data[index_name].delete(doc, txn=transaction)
             else:
                 log.error(f'unable to delete key: "{key}" from table "{self.name}"')  # pragma: no cover
 
-    @transparent_resize
+    @wrap_writer
     def empty(self, txn: Optional[TXN|WriteTransaction]=None) -> None:
         """
         Remove all data from the current table leaving the indexing structure in-tact
 
         txn - an optional transaction
         """
         transaction = txn if isinstance(txn, TXN) else txn.txn
@@ -602,32 +607,30 @@
         #         'delete': False
         #     })
         #     txn.journal.append(doc.journal_entry(JournalType.REMOVE, self.name))
 
         for index_name in self.data:
             self.data[index_name].empty(txn=transaction)
 
-    @transparent_resize
+    @wrap_writer
     def drop(self, index_name: str, txn: Optional[TXN, WriteTransaction]=None) -> None:
         """
         Drop an index from the current table
 
         index_name - the name of the index to drop
         txn - an optional transaction
         """
         if index_name not in self.data:
             raise NoSuchIndex(index_name)
 
         transaction = txn if isinstance(txn, TXN) else txn.txn
         index = self.data[index_name]
         del self.data[index_name]
         index.drop(txn=transaction)
-
-        # if self.replicated(txn):
-        #     txn.journal.append(Doc({'index': index_name}).journal_entry(JournalType.DROPIX, self.name))
+        self._database._cat.drop_index(self.name, index_name, txn)
 
     @wrap_reader_yield
     def tail(self, key: Optional[OID]=None, txn: Optional[TXN]=None) -> Generator[Doc, None, None]:
         """
         Generates a sequence of records starting from the key after the primary key supplied. If no
         key is supplied, all records are returned, if a misssing key is supplied, no records are
         returned. Typically use this against the last-seen key to access new keys since the last
@@ -870,40 +873,32 @@
         context - a paging context to determine where to start tge next page (see comments)
         page_size - maximum number of records to return
         inclusive - if set to True, include the keys at each end, i.e. use <=|=> rather than <|>
         suppress_duplicates - no duplicate keys, return only unique key values and ignore duplicates
         reverse - navigate the index in reverse order
         txn - an optional transaction
         """
-        # log.error(f"Lower0> {lower} ({lower.doc if lower else ''})")
-        # log.error(f"Upper0> {upper} ({upper.doc if upper else ''})")
-
-
         transaction = txn if isinstance(txn, TXN) else txn.txn
         if index_name is not None:
             if index_name not in self.data:
                 raise NoSuchIndex()
             index = self.data[index_name]
             db = index._db
-            # log.warning(f">>> {index} {index.map_key(lower)}")
             lower_keys = index.map_key(lower) if lower else [None]
             upper_keys = index.map_key(upper) if upper else [None]
             if not isinstance(lower_keys, list):
                 lower_keys = [lower_keys]
             if not isinstance(upper_keys, list):
                 upper_keys = [upper_keys]
         else:
             db = self._db
             index = None
             lower_keys = [None] if lower is None else [lower.oid]
             upper_keys = [None] if upper is None else [upper.oid]
 
-        # log.error(f"Lower1> {lower_keys}")
-        # log.error(f"Upper1> {upper_keys}")
-
         with transaction.cursor(db) as cursor:
             next_record = cursor.next_nodup if suppress_duplicates else cursor.next
             prev_record = cursor.prev_nodup if suppress_duplicates else cursor.prev
             if reverse:
                 prev_record, next_record = next_record, prev_record
                 lower_keys, upper_keys = upper_keys, lower_keys
                 first = cursor.last
@@ -1003,23 +998,28 @@
     def unwatch(self, callback: Callable=None, txn: Optional[TXN|WriteTransaction]=None) -> None:
         self._database._auditor.unwatch(self.name, callback)
 
     def export_to_file (self, filename, force=False):
         path = Path(filename)
         if path.exists() and not force:
             raise FileExistsError
-        with open(filename, 'wb') as io:
+        with open(filename, 'w') as io:
+            count = 0
+            io.write('{\n')
             for result in self.filter():
-                io.write(self.serialise(result.doc.doc_with_id) + b'\n')
+                if count: io.write(',\n')
+                io.write('  "' + result.doc.key + '": ')
+                dump(result.doc.doc, io)
+                count += 1
+            io.write('\n}\n')
+        return count
 
     def import_from_file (self, filename):
         path = Path(filename)
         if not path.exists():
             raise FileNotFoundError
-        with open(filename, 'rb') as io:
-            while True:
-                line = io.readline()
-                if not line:
-                    break
-                dic = self.deserialise(line)
-                oid = dic.pop('_id')
-                self.append(Doc(dic, oid=oid))
+        with open(filename, 'r') as io:
+            data = load(io)
+            for key in data:
+                doc = Doc(dict(data[key], **{'key': key}))
+                self.append(doc)
+        return len(data)
```

