# Comparing `tmp/aiodiskqueue-0.1.0b8.tar.gz` & `tmp/aiodiskqueue-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiodiskqueue-0.1.0b8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "aiodiskqueue-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aiodiskqueue-0.1.0b8.tar` & `aiodiskqueue-0.1.1.tar`

### file list

```diff
@@ -1,47 +1,13 @@
--rw-r--r--   0        0        0      227 2023-05-24 13:44:43.729148 aiodiskqueue-0.1.0b8/.coveragerc
--rw-r--r--   0        0        0      964 2023-05-24 14:34:49.657277 aiodiskqueue-0.1.0b8/.github/workflows/main.yml
--rw-r--r--   0        0        0      798 2023-05-28 19:18:15.116717 aiodiskqueue-0.1.0b8/.github/workflows/release.yml
--rw-r--r--   0        0        0      136 2023-06-01 19:01:40.059543 aiodiskqueue-0.1.0b8/.gitignore
--rw-r--r--   0        0        0      477 2023-05-17 22:01:56.296859 aiodiskqueue-0.1.0b8/.pre-commit-config.yaml
--rw-r--r--   0        0        0      142 2023-05-24 16:15:47.425496 aiodiskqueue-0.1.0b8/.readthedocs.yaml
--rw-r--r--   0        0        0     1080 2023-05-23 20:46:51.856056 aiodiskqueue-0.1.0b8/LICENSE
--rw-r--r--   0        0        0      121 2023-05-28 14:06:56.931356 aiodiskqueue-0.1.0b8/Makefile
--rw-r--r--   0        0        0     2899 2023-06-03 13:34:43.520022 aiodiskqueue-0.1.0b8/README.rst
--rw-r--r--   0        0        0      634 2023-05-24 14:44:01.590463 aiodiskqueue-0.1.0b8/docs/Makefile
--rw-r--r--   0        0        0       37 2023-05-24 17:17:07.835418 aiodiskqueue-0.1.0b8/docs/_static/custom.css
--rw-r--r--   0        0        0      267 2023-05-30 15:23:45.131006 aiodiskqueue-0.1.0b8/docs/api.rst
--rw-r--r--   0        0        0     1884 2023-05-28 18:08:22.925790 aiodiskqueue-0.1.0b8/docs/conf.py
--rw-r--r--   0        0        0      347 2023-05-24 15:23:38.770047 aiodiskqueue-0.1.0b8/docs/index.rst
--rw-r--r--   0        0        0      800 2023-05-24 14:44:01.594463 aiodiskqueue-0.1.0b8/docs/make.bat
--rw-r--r--   0        0        0        0 2023-05-24 11:55:33.417325 aiodiskqueue-0.1.0b8/examples/__init__.py
--rw-r--r--   0        0        0      210 2023-05-28 14:06:56.943355 aiodiskqueue-0.1.0b8/examples/basic_usage.py
--rw-r--r--   0        0        0      933 2023-05-28 14:06:56.943355 aiodiskqueue-0.1.0b8/examples/multiple_consumers.py
--rw-r--r--   0        0        0      879 2023-05-28 14:06:56.943355 aiodiskqueue-0.1.0b8/examples/single_consumer.py
--rw-r--r--   0        0        0        0 2023-06-01 19:01:40.059543 aiodiskqueue-0.1.0b8/measurements/__init__.py
--rw-r--r--   0        0        0    47249 2023-06-03 13:21:48.237118 aiodiskqueue-0.1.0b8/measurements/analysis.ipynb
--rw-r--r--   0        0        0      396 2023-06-03 12:47:40.471333 aiodiskqueue-0.1.0b8/measurements/config.toml
--rw-r--r--   0        0        0       17 2023-06-01 19:01:40.059543 aiodiskqueue-0.1.0b8/measurements/requirements.txt
--rw-r--r--   0        0        0     7041 2023-06-03 13:31:27.872382 aiodiskqueue-0.1.0b8/measurements/run.py
--rw-r--r--   0        0        0     1055 2023-06-02 22:08:23.472217 aiodiskqueue-0.1.0b8/pyproject.toml
--rw-r--r--   0        0        0      258 2023-06-03 12:38:59.334856 aiodiskqueue-0.1.0b8/src/aiodiskqueue/__init__.py
--rw-r--r--   0        0        0      230 2023-06-02 22:07:35.456683 aiodiskqueue-0.1.0b8/src/aiodiskqueue/engines/__init__.py
--rw-r--r--   0        0        0     1067 2023-06-03 13:31:27.656383 aiodiskqueue-0.1.0b8/src/aiodiskqueue/engines/base.py
--rw-r--r--   0        0        0     3473 2023-06-03 13:31:27.732383 aiodiskqueue-0.1.0b8/src/aiodiskqueue/engines/dbm.py
--rw-r--r--   0        0        0     3473 2023-06-03 13:31:27.768383 aiodiskqueue-0.1.0b8/src/aiodiskqueue/engines/simple.py
--rw-r--r--   0        0        0     2168 2023-06-03 13:31:27.824383 aiodiskqueue-0.1.0b8/src/aiodiskqueue/engines/sqlite.py
--rw-r--r--   0        0        0      268 2023-05-28 14:06:56.947355 aiodiskqueue-0.1.0b8/src/aiodiskqueue/exceptions.py
--rw-r--r--   0        0        0     7937 2023-06-03 13:31:27.696383 aiodiskqueue-0.1.0b8/src/aiodiskqueue/queues.py
--rw-r--r--   0        0        0      714 2023-05-28 18:34:37.954258 aiodiskqueue-0.1.0b8/src/aiodiskqueue/utils.py
--rw-r--r--   0        0        0        0 2023-05-24 11:07:45.426708 aiodiskqueue-0.1.0b8/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-06-01 19:01:40.071544 aiodiskqueue-0.1.0b8/tests/engines/__init__.py
--rw-r--r--   0        0        0     1791 2023-06-03 12:32:51.568346 aiodiskqueue-0.1.0b8/tests/engines/test_base.py
--rw-r--r--   0        0        0      635 2023-06-03 12:32:56.692325 aiodiskqueue-0.1.0b8/tests/engines/test_dbm.py
--rw-r--r--   0        0        0      714 2023-06-02 22:18:18.574682 aiodiskqueue-0.1.0b8/tests/engines/test_simple.py
--rw-r--r--   0        0        0      405 2023-06-02 22:10:58.483256 aiodiskqueue-0.1.0b8/tests/engines/test_sqlite.py
--rw-r--r--   0        0        0      527 2023-05-28 14:06:56.947355 aiodiskqueue-0.1.0b8/tests/factories.py
--rw-r--r--   0        0        0      356 2023-05-28 18:38:14.973455 aiodiskqueue-0.1.0b8/tests/helpers.py
--rw-r--r--   0        0        0     3510 2023-06-03 13:31:27.916382 aiodiskqueue-0.1.0b8/tests/test_integration.py
--rw-r--r--   0        0        0     8469 2023-06-02 22:33:56.531565 aiodiskqueue-0.1.0b8/tests/test_queues.py
--rw-r--r--   0        0        0      627 2023-05-28 17:55:30.938412 aiodiskqueue-0.1.0b8/tests/test_utils.py
--rw-r--r--   0        0        0      459 2023-06-02 22:24:25.114342 aiodiskqueue-0.1.0b8/tox.ini
--rw-r--r--   0        0        0     3863 1970-01-01 00:00:00.000000 aiodiskqueue-0.1.0b8/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-06-09 11:23:48.665306 aiodiskqueue-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2982 2023-06-09 11:23:48.665306 aiodiskqueue-0.1.1/README.rst
+-rw-r--r--   0        0        0     1053 2023-06-09 11:23:48.665306 aiodiskqueue-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      256 2023-06-09 11:23:48.665306 aiodiskqueue-0.1.1/src/aiodiskqueue/__init__.py
+-rw-r--r--   0        0        0      230 2023-06-09 11:23:48.665306 aiodiskqueue-0.1.1/src/aiodiskqueue/engines/__init__.py
+-rw-r--r--   0        0        0     1172 2023-06-09 11:23:48.665306 aiodiskqueue-0.1.1/src/aiodiskqueue/engines/base.py
+-rw-r--r--   0        0        0     3121 2023-06-09 11:23:48.665306 aiodiskqueue-0.1.1/src/aiodiskqueue/engines/dbm.py
+-rw-r--r--   0        0        0     3476 2023-06-09 11:23:48.665306 aiodiskqueue-0.1.1/src/aiodiskqueue/engines/simple.py
+-rw-r--r--   0        0        0     2166 2023-06-09 11:23:48.665306 aiodiskqueue-0.1.1/src/aiodiskqueue/engines/sqlite.py
+-rw-r--r--   0        0        0      268 2023-06-09 11:23:48.665306 aiodiskqueue-0.1.1/src/aiodiskqueue/exceptions.py
+-rw-r--r--   0        0        0     7934 2023-06-09 11:23:48.665306 aiodiskqueue-0.1.1/src/aiodiskqueue/queues.py
+-rw-r--r--   0        0        0      714 2023-06-09 11:23:48.665306 aiodiskqueue-0.1.1/src/aiodiskqueue/utils.py
+-rw-r--r--   0        0        0     3942 1970-01-01 00:00:00.000000 aiodiskqueue-0.1.1/PKG-INFO
```

### Comparing `aiodiskqueue-0.1.0b8/LICENSE` & `aiodiskqueue-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0b8/README.rst` & `aiodiskqueue-0.1.1/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,27 @@
+============
 aiodiskqueue
 ============
 
 Persistent queue for Python AsyncIO.
 
 |release| |python| |tests| |codecov| |docs| |pre-commit| |Code style: black|
 
 Description
 -----------
 
 This library provides a persistent FIFO queue for Python AsyncIO:
 
-- Queue content can persist a process restart
+- Queue content persist a process restart
 - Feature parity with Python's `asyncio.Queue <https://docs.python.org/3/library/asyncio-queue.html#queue>`_
 - Similar API to Python's `asyncio.Queue <https://docs.python.org/3/library/asyncio-queue.html#queue>`_
 - Sane logging
 - Type hints
 - Fully tested
-- Supports different storage engines
+- Supports different storage engines and can be extended with custom storage engines
 
 Usage
 -----
 
 Here is a basic example on how to use the queue:
 
 .. code:: python
@@ -56,30 +57,38 @@
 Storage Engines
 ---------------
 
 aiodiskqueue support different storage engines. The default engine is `DbmEngine`.
 
 We measured the throughput for a typical load scenario (5 producers, 1 consumer) with each storage engine:
 
-|chart|
-
-- `DbmEngine`: Consistent throughput at low and high volumes and about 3 x faster then Sqlite
-- `PickledList`: Very fast at low volumes, but does not scale well
-- `SqliteEngine`: Consistent throughput at low and high volumes. Relatively slow.
+.. image:: https://imgpile.com/images/9luzXk.png
+  :width: 800
+  :alt: Measurements
+
+* `DbmEngine`: Consistent throughput at low and high volumes and about 3 x faster then Sqlite
+* `PickledList`: Very fast at low volumes, but does not scale well
+* `SqliteEngine`: Consistent throughput at low and high volumes. Relatively slow.
 
 The scripts for running the measurements and generating this chart can be found in the measurements folder.
 
-.. |chart| image:: https://imgpile.com/images/9luzXk.png
+
 .. |release| image:: https://img.shields.io/pypi/v/aiodiskqueue?label=release
    :target: https://pypi.org/project/aiodiskqueue/
+
 .. |python| image:: https://img.shields.io/pypi/pyversions/aiodiskqueue
    :target: https://pypi.org/project/aiodiskqueue/
+
 .. |tests| image:: https://github.com/ErikKalkoken/aiodiskqueue/actions/workflows/main.yml/badge.svg
    :target: https://github.com/ErikKalkoken/aiodiskqueue/actions
+
 .. |codecov| image:: https://codecov.io/gh/ErikKalkoken/aiodiskqueue/branch/main/graph/badge.svg?token=V43h7hl1Te
    :target: https://codecov.io/gh/ErikKalkoken/aiodiskqueue
+
 .. |docs| image:: https://readthedocs.org/projects/aiodiskqueue/badge/?version=latest
    :target: https://aiodiskqueue.readthedocs.io/en/latest/?badge=latest
+
 .. |pre-commit| image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
    :target: https://github.com/pre-commit/pre-commit
+
 .. |Code style: black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
```

### Comparing `aiodiskqueue-0.1.0b8/pyproject.toml` & `aiodiskqueue-0.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dynamic = ["version", "description"]
 requires-python = ">=3.8"
 dependencies = [
-    "aiodbm>=0.2.0a1",
+    "aiodbm>=0.4.0",
 
 ]
 
 [project.optional-dependencies]
 aiofiles = [
     "aiofiles>=23.1.0",
 ]
```

### Comparing `aiodiskqueue-0.1.0b8/src/aiodiskqueue/engines/dbm.py` & `aiodiskqueue-0.1.1/src/aiodiskqueue/engines/dbm.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,102 +1,96 @@
-"""Engines for storing the queues on disk."""
+"""Engines for storing the queues with DBM."""
 
 import dbm
 import logging
 import pickle
 from pathlib import Path
 from typing import Any, List, Optional, Union
 
-try:
-    import aiodbm
-except ImportError:
-    has_aiodbm = False
-else:
-    has_aiodbm = True
+import aiodbm
 
-from .base import _FifoStorageEngine
+from .base import FifoStorageEngine
 
 logger = logging.getLogger("aiodiskqueue")
 
-if has_aiodbm:
 
-    class DbmEngine(_FifoStorageEngine):
-        """A queue storage engine using DBM."""
+class DbmEngine(FifoStorageEngine):
+    """A queue storage engine using DBM."""
 
-        def __init__(self, data_path: Path) -> None:
-            super().__init__(data_path)
-            self._data_path_2 = str(data_path.absolute())
-
-        HEAD_ID_KEY = "head_id"
-        TAIL_ID_KEY = "tail_id"
-
-        async def initialize(self):
-            async with aiodbm.open(self._data_path_2, "c") as db:
-                await db.set("dummy", "test")
-                await db.delete("dummy")
-
-        async def fetch_all(self) -> List[Any]:
-            try:
-                async with aiodbm.open(self._data_path_2, "r") as db:
-                    head_id = await self._get_obj(db, self.HEAD_ID_KEY)
-                    tail_id = await self._get_obj(db, self.TAIL_ID_KEY)
-                    if not head_id or not tail_id:
-                        return []
-
-                    items = []
-                    for item_id in range(head_id, tail_id + 1):
-                        item_key = self._make_item_key(item_id)
-                        item = await self._get_obj(db, item_key)
-                        items.append(item)
-            except dbm.error:
-                items = []
-
-            return items
-
-        async def add_item(self, item: Any):
-            async with aiodbm.open(self._data_path_2, "w") as db:
-                tail_id = await self._get_obj(db, self.TAIL_ID_KEY)
-                if tail_id:
-                    item_id = tail_id + 1
-                    is_first = False
-                else:
-                    item_id = 1
-                    is_first = True
-
-                await self._set_obj(db, self._make_item_key(item_id), item)
-                await self._set_obj(db, self.TAIL_ID_KEY, item_id)
-
-                if is_first:
-                    await self._set_obj(db, self.HEAD_ID_KEY, item_id)
-
-        async def remove_item(self):
-            async with aiodbm.open(self._data_path_2, "w") as db:
-                head_id = await self._get_obj(db, self.HEAD_ID_KEY)
-                tail_id = await self._get_obj(db, self.TAIL_ID_KEY)
+    def __init__(self, data_path: Path) -> None:
+        super().__init__(data_path)
+        self._data_path_2 = str(data_path.absolute())
+
+    _HEAD_ID_KEY = "head_id"
+    _TAIL_ID_KEY = "tail_id"
+
+    async def initialize(self):
+        async with aiodbm.open(self._data_path_2, "c") as db:
+            await db.set("dummy", "test")
+            await db.delete("dummy")
+
+    async def fetch_all(self) -> List[Any]:
+        try:
+            async with aiodbm.open(self._data_path_2, "r") as db:
+                head_id = await self._get_obj(db, self._HEAD_ID_KEY)
+                tail_id = await self._get_obj(db, self._TAIL_ID_KEY)
                 if not head_id or not tail_id:
-                    raise ValueError("Nothing to remove from an empty database")
-                item_key = self._make_item_key(head_id)
-                await db.delete(item_key)
-
-                if head_id != tail_id:
-                    # there are items left
-                    await self._set_obj(db, self.HEAD_ID_KEY, head_id + 1)
-                else:
-                    # was last item
-                    await db.delete(self.HEAD_ID_KEY)
-                    await db.delete(self.TAIL_ID_KEY)
-
-        @staticmethod
-        def _make_item_key(item_id: int) -> str:
-            return f"item-{item_id}"
-
-        @staticmethod
-        async def _get_obj(db, key: Union[str, bytes]) -> Optional[Any]:
-            data = await db.get(key)
-            if not data:
-                return None
-            return pickle.loads(data)
-
-        @staticmethod
-        async def _set_obj(db, key: Union[str, bytes], item: Any):
-            data = pickle.dumps(item)
-            await db.set(key, data)
+                    return []
+
+                items = []
+                for item_id in range(head_id, tail_id + 1):
+                    item_key = self._make_item_key(item_id)
+                    item = await self._get_obj(db, item_key)
+                    items.append(item)
+        except dbm.error:
+            items = []
+
+        return items
+
+    async def add_item(self, item: Any):
+        async with aiodbm.open(self._data_path_2, "w") as db:
+            tail_id = await self._get_obj(db, self._TAIL_ID_KEY)
+            if tail_id:
+                item_id = tail_id + 1
+                is_first = False
+            else:
+                item_id = 1
+                is_first = True
+
+            await self._set_obj(db, self._make_item_key(item_id), item)
+            await self._set_obj(db, self._TAIL_ID_KEY, item_id)
+
+            if is_first:
+                await self._set_obj(db, self._HEAD_ID_KEY, item_id)
+
+    async def remove_item(self):
+        async with aiodbm.open(self._data_path_2, "w") as db:
+            head_id = await self._get_obj(db, self._HEAD_ID_KEY)
+            tail_id = await self._get_obj(db, self._TAIL_ID_KEY)
+            if not head_id or not tail_id:
+                raise ValueError("Nothing to remove from an empty database")
+            item_key = self._make_item_key(head_id)
+            await db.delete(item_key)
+
+            if head_id != tail_id:
+                # there are items left
+                await self._set_obj(db, self._HEAD_ID_KEY, head_id + 1)
+            else:
+                # was last item
+                await db.delete(self._HEAD_ID_KEY)
+                await db.delete(self._TAIL_ID_KEY)
+
+    @staticmethod
+    def _make_item_key(item_id: int) -> str:
+        return f"item-{item_id}"
+
+    @staticmethod
+    async def _get_obj(db, key: Union[str, bytes]) -> Optional[Any]:
+        data = await db.get(key)
+        if not data:
+            return None
+        return pickle.loads(data)
+
+    @staticmethod
+    async def _set_obj(db, key: Union[str, bytes], item: Any):
+        data = pickle.dumps(item)
+        await db.set(key, data)
```

### Comparing `aiodiskqueue-0.1.0b8/src/aiodiskqueue/engines/simple.py` & `aiodiskqueue-0.1.1/src/aiodiskqueue/engines/simple.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-"""Engines for storing the queues on disk."""
+"""Engines for storing the queues in flat files."""
 
 import io
 import logging
 import pickle
 from typing import Any, List
 
 import aiofiles
 import aiofiles.os
 
-from .base import _FifoStorageEngine
+from .base import FifoStorageEngine
 
 logger = logging.getLogger("aiodiskqueue")
 
 
-class PickledList(_FifoStorageEngine):
+class PickledList(FifoStorageEngine):
     """This engine stores items as one singular pickled list of items."""
 
     async def initialize(self):
         await self._save_all_items([])
 
     async def fetch_all(self) -> List[Any]:
         try:
@@ -50,15 +50,15 @@
 
     async def _save_all_items(self, items: List[Any]):
         async with aiofiles.open(self._data_path, "wb", buffering=0) as file:
             await file.write(pickle.dumps(items))
         logger.debug("Wrote queue with %d items: %s", len(items), self._data_path)
 
 
-class PickleSequence(_FifoStorageEngine):
+class PickleSequence(FifoStorageEngine):
     """This engine stores items as a sequence of single pickles."""
 
     async def initialize(self):
         await self._save_all_items([])
 
     async def fetch_all(self) -> List[Any]:
         try:
```

### Comparing `aiodiskqueue-0.1.0b8/src/aiodiskqueue/engines/sqlite.py` & `aiodiskqueue-0.1.1/src/aiodiskqueue/engines/sqlite.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 try:
     import aiosqlite
 except ImportError:
     has_aiosqlite = False
 else:
     has_aiosqlite = True
 
-from .base import _FifoStorageEngine
+from .base import FifoStorageEngine
 
 logger = logging.getLogger("aiodiskqueue")
 
 if has_aiosqlite:
 
-    class SqliteEngine(_FifoStorageEngine):
+    class SqliteEngine(FifoStorageEngine):
         """A queue storage engine using Sqlite."""
 
         async def initialize(self):
             async with aiosqlite.connect(self._data_path, isolation_level=None) as db:
                 await db.execute(
                     """
                     CREATE TABLE IF NOT EXISTS queue (item BLOB);
```

### Comparing `aiodiskqueue-0.1.0b8/src/aiodiskqueue/queues.py` & `aiodiskqueue-0.1.1/src/aiodiskqueue/queues.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Core implementation of a persistent AsyncIO queue."""
 
 import asyncio
 import logging
 from pathlib import Path
 from typing import Any, Union
 
-from aiodiskqueue.engines.base import _FifoStorageEngine
+from aiodiskqueue.engines.base import FifoStorageEngine
 from aiodiskqueue.engines.dbm import DbmEngine
 from aiodiskqueue.exceptions import QueueEmpty, QueueFull
 from aiodiskqueue.utils import NoDirectInstantiation
 
 logger = logging.getLogger("aiodiskqueue")
 
 
@@ -25,15 +25,15 @@
     """
 
     def __init__(
         self,
         data_path: Path,
         maxsize: int,
         queue: list,
-        storage_engine: _FifoStorageEngine,
+        storage_engine: FifoStorageEngine,
     ) -> None:
         """Direct instantiation would break the persistance feature
         and has therefore been disabled.
 
         :meta private:
         """
         self._data_path = Path(data_path)
@@ -204,15 +204,15 @@
         data_path = Path(data_path)
         if data_path.suffix == ".bak":
             raise ValueError("Invalid file name: .bak suffix is reserved for backups")
 
         if not cls_storage_engine:
             cls_storage_engine = DbmEngine
         else:
-            if not issubclass(cls_storage_engine, _FifoStorageEngine):
+            if not issubclass(cls_storage_engine, FifoStorageEngine):
                 raise TypeError("Invalid storage engine")
         storage_engine = cls_storage_engine(data_path)
         queue = await storage_engine.fetch_all()
         if not queue:
             await storage_engine.initialize()  # ensuring early we can write
         else:
             logger.info(
```

### Comparing `aiodiskqueue-0.1.0b8/src/aiodiskqueue/utils.py` & `aiodiskqueue-0.1.1/src/aiodiskqueue/utils.py`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0b8/PKG-INFO` & `aiodiskqueue-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,49 +1,50 @@
 Metadata-Version: 2.1
 Name: aiodiskqueue
-Version: 0.1.0b8
+Version: 0.1.1
 Summary: Persistent queue for Python AsyncIO.
 Author-email: Erik Kalkoken <kalkoken87@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: aiodbm>=0.2.0a1
+Requires-Dist: aiodbm>=0.4.0
 Requires-Dist: aiofiles>=23.1.0 ; extra == "aiofiles"
 Requires-Dist: aiosqlite>=0.19.0 ; extra == "aiosqlite"
 Project-URL: Documentation, https://aiodiskqueue.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/ErikKalkoken/aiodiskqueue
 Project-URL: Tracker, https://github.com/ErikKalkoken/aiodiskqueue/issues
 Provides-Extra: aiofiles
 Provides-Extra: aiosqlite
 
+============
 aiodiskqueue
 ============
 
 Persistent queue for Python AsyncIO.
 
 |release| |python| |tests| |codecov| |docs| |pre-commit| |Code style: black|
 
 Description
 -----------
 
 This library provides a persistent FIFO queue for Python AsyncIO:
 
-- Queue content can persist a process restart
+- Queue content persist a process restart
 - Feature parity with Python's `asyncio.Queue <https://docs.python.org/3/library/asyncio-queue.html#queue>`_
 - Similar API to Python's `asyncio.Queue <https://docs.python.org/3/library/asyncio-queue.html#queue>`_
 - Sane logging
 - Type hints
 - Fully tested
-- Supports different storage engines
+- Supports different storage engines and can be extended with custom storage engines
 
 Usage
 -----
 
 Here is a basic example on how to use the queue:
 
 .. code:: python
@@ -79,31 +80,39 @@
 Storage Engines
 ---------------
 
 aiodiskqueue support different storage engines. The default engine is `DbmEngine`.
 
 We measured the throughput for a typical load scenario (5 producers, 1 consumer) with each storage engine:
 
-|chart|
-
-- `DbmEngine`: Consistent throughput at low and high volumes and about 3 x faster then Sqlite
-- `PickledList`: Very fast at low volumes, but does not scale well
-- `SqliteEngine`: Consistent throughput at low and high volumes. Relatively slow.
+.. image:: https://imgpile.com/images/9luzXk.png
+  :width: 800
+  :alt: Measurements
+
+* `DbmEngine`: Consistent throughput at low and high volumes and about 3 x faster then Sqlite
+* `PickledList`: Very fast at low volumes, but does not scale well
+* `SqliteEngine`: Consistent throughput at low and high volumes. Relatively slow.
 
 The scripts for running the measurements and generating this chart can be found in the measurements folder.
 
-.. |chart| image:: https://imgpile.com/images/9luzXk.png
+
 .. |release| image:: https://img.shields.io/pypi/v/aiodiskqueue?label=release
    :target: https://pypi.org/project/aiodiskqueue/
+
 .. |python| image:: https://img.shields.io/pypi/pyversions/aiodiskqueue
    :target: https://pypi.org/project/aiodiskqueue/
+
 .. |tests| image:: https://github.com/ErikKalkoken/aiodiskqueue/actions/workflows/main.yml/badge.svg
    :target: https://github.com/ErikKalkoken/aiodiskqueue/actions
+
 .. |codecov| image:: https://codecov.io/gh/ErikKalkoken/aiodiskqueue/branch/main/graph/badge.svg?token=V43h7hl1Te
    :target: https://codecov.io/gh/ErikKalkoken/aiodiskqueue
+
 .. |docs| image:: https://readthedocs.org/projects/aiodiskqueue/badge/?version=latest
    :target: https://aiodiskqueue.readthedocs.io/en/latest/?badge=latest
+
 .. |pre-commit| image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
    :target: https://github.com/pre-commit/pre-commit
+
 .. |Code style: black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
```

