# Comparing `tmp/patio-0.1.2.tar.gz` & `tmp/patio-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "patio-0.1.2.tar", max compression
+gzip compressed data, was "patio-0.1.3.tar", max compression
```

## Comparing `patio-0.1.2.tar` & `patio-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    13343 2023-06-08 10:57:28.341047 patio-0.1.2/README.md
--rw-r--r--   0        0        0      580 2023-06-08 10:47:29.273489 patio-0.1.2/patio/__init__.py
--rw-r--r--   0        0        0      294 2023-06-08 10:47:29.274047 patio-0.1.2/patio/broker/__init__.py
--rw-r--r--   0        0        0     1845 2023-06-08 10:47:29.274688 patio-0.1.2/patio/broker/abc.py
--rw-r--r--   0        0        0      542 2023-06-08 10:47:29.275407 patio-0.1.2/patio/broker/memory.py
--rw-r--r--   0        0        0     1684 2023-06-08 10:47:29.276506 patio-0.1.2/patio/broker/serializer.py
--rw-r--r--   0        0        0      151 2023-06-08 10:47:29.277259 patio-0.1.2/patio/broker/tcp/__init__.py
--rw-r--r--   0        0        0    13207 2023-06-08 10:47:29.277917 patio-0.1.2/patio/broker/tcp/broker.py
--rw-r--r--   0        0        0     2765 2023-06-08 10:47:29.278972 patio-0.1.2/patio/broker/tcp/protocol.py
--rw-r--r--   0        0        0      674 2023-06-08 10:47:29.279837 patio-0.1.2/patio/compat.py
--rw-r--r--   0        0        0      329 2023-06-08 10:47:29.280419 patio-0.1.2/patio/executor/__init__.py
--rw-r--r--   0        0        0     2176 2023-06-08 10:47:29.281010 patio-0.1.2/patio/executor/asyncronous.py
--rw-r--r--   0        0        0     2663 2023-06-08 10:47:29.281647 patio-0.1.2/patio/executor/base.py
--rw-r--r--   0        0        0      547 2023-06-08 10:47:29.282312 patio-0.1.2/patio/executor/null.py
--rw-r--r--   0        0        0     1277 2023-06-08 10:47:29.282966 patio-0.1.2/patio/executor/process_pool.py
--rw-r--r--   0        0        0     1308 2023-06-08 10:47:29.283510 patio-0.1.2/patio/executor/thread_pool.py
--rw-r--r--   0        0        0        0 2023-06-08 10:47:29.283734 patio-0.1.2/patio/py.typed
--rw-r--r--   0        0        0     8769 2023-06-08 10:47:29.285807 patio-0.1.2/patio/registry.py
--rw-r--r--   0        0        0     2299 2023-06-08 11:00:12.674462 patio-0.1.2/pyproject.toml
--rw-r--r--   0        0        0    14830 1970-01-01 00:00:00.000000 patio-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    13343 2023-06-09 06:38:24.251449 patio-0.1.3/README.md
+-rw-r--r--   0        0        0      580 2023-06-09 06:38:24.252956 patio-0.1.3/patio/__init__.py
+-rw-r--r--   0        0        0      294 2023-06-09 06:38:24.253102 patio-0.1.3/patio/broker/__init__.py
+-rw-r--r--   0        0        0     1845 2023-06-09 06:38:24.253194 patio-0.1.3/patio/broker/abc.py
+-rw-r--r--   0        0        0      542 2023-06-09 06:38:24.253274 patio-0.1.3/patio/broker/memory.py
+-rw-r--r--   0        0        0     1684 2023-06-09 06:38:24.253356 patio-0.1.3/patio/broker/serializer.py
+-rw-r--r--   0        0        0      151 2023-06-09 06:38:24.253494 patio-0.1.3/patio/broker/tcp/__init__.py
+-rw-r--r--   0        0        0    14402 2023-06-09 06:38:24.253713 patio-0.1.3/patio/broker/tcp/broker.py
+-rw-r--r--   0        0        0     2816 2023-06-09 06:38:24.253846 patio-0.1.3/patio/broker/tcp/protocol.py
+-rw-r--r--   0        0        0      674 2023-06-09 06:38:24.253948 patio-0.1.3/patio/compat.py
+-rw-r--r--   0        0        0      329 2023-06-09 06:38:24.254089 patio-0.1.3/patio/executor/__init__.py
+-rw-r--r--   0        0        0     2176 2023-06-09 06:38:24.254193 patio-0.1.3/patio/executor/asyncronous.py
+-rw-r--r--   0        0        0     2663 2023-06-09 06:38:24.254305 patio-0.1.3/patio/executor/base.py
+-rw-r--r--   0        0        0      625 2023-06-09 06:38:24.254448 patio-0.1.3/patio/executor/null.py
+-rw-r--r--   0        0        0     1277 2023-06-09 06:38:24.254562 patio-0.1.3/patio/executor/process_pool.py
+-rw-r--r--   0        0        0     1308 2023-06-09 06:38:24.254658 patio-0.1.3/patio/executor/thread_pool.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:38:24.254695 patio-0.1.3/patio/py.typed
+-rw-r--r--   0        0        0     8935 2023-06-09 06:38:24.254828 patio-0.1.3/patio/registry.py
+-rw-r--r--   0        0        0     2299 2023-06-09 06:38:24.255243 patio-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0    14580 1970-01-01 00:00:00.000000 patio-0.1.3/PKG-INFO
```

### Comparing `patio-0.1.2/README.md` & `patio-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `patio-0.1.2/patio/__init__.py` & `patio-0.1.3/patio/__init__.py`

 * *Files identical despite different names*

### Comparing `patio-0.1.2/patio/broker/abc.py` & `patio-0.1.3/patio/broker/abc.py`

 * *Files identical despite different names*

### Comparing `patio-0.1.2/patio/broker/memory.py` & `patio-0.1.3/patio/broker/memory.py`

 * *Files identical despite different names*

### Comparing `patio-0.1.2/patio/broker/serializer.py` & `patio-0.1.3/patio/broker/serializer.py`

 * *Files identical despite different names*

### Comparing `patio-0.1.2/patio/broker/tcp/broker.py` & `patio-0.1.3/patio/broker/tcp/broker.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 import asyncio
 import logging
 import pickle
 import ssl
 import uuid
 from abc import ABC, abstractmethod
-from collections import deque
+from collections import defaultdict, deque
 from dataclasses import dataclass
 from functools import cached_property
 from types import MappingProxyType
 from typing import (
-    Any, Callable, Coroutine, Deque, Dict, Mapping, Optional, Set, Tuple,
-    TypeVar, Union, final,
+    Any, Callable, Coroutine, DefaultDict, Deque, Dict, Iterable, List, Mapping,
+    Optional, Set, Tuple, TypeVar, Union, final,
 )
 
 from patio.broker import AbstractBroker, TimeoutType
 from patio.broker.serializer import (
     AbstractSerializer, RestrictedPickleSerializer,
 )
 from patio.broker.tcp.protocol import Header, PacketTypes, Protocol
@@ -44,15 +44,14 @@
 
 
 class PacketHandler(ABC):
     reader: asyncio.StreamReader
     writer: asyncio.StreamWriter
     protocol: Protocol
     executor: AbstractExecutor
-    registry: Registry
 
     def __init__(
         self,
         reader: asyncio.StreamReader,
         writer: asyncio.StreamWriter,
         executor: AbstractExecutor,
         protocol: Protocol,
@@ -68,14 +67,15 @@
 
         self.__method_map: Mapping[
             PacketTypes, Callable[[RPCEvent], Coroutine[Any, Any, Any]],
         ] = MappingProxyType({
             PacketTypes.REQUEST: self.handle_request,
             PacketTypes.RESPONSE: self.handle_response,
             PacketTypes.ERROR: self.handle_error,
+            PacketTypes.DISCOVER_REQUEST: self.handle_discover_request,
         })
 
     @cached_property
     def loop(self) -> asyncio.AbstractEventLoop:
         return asyncio.get_running_loop()
 
     async def get_event(self) -> RPCEvent:
@@ -127,28 +127,50 @@
             payload = self.protocol.serializer.unpack(event.payload)
         except (ValueError, pickle.UnpicklingError) as e:
             future.set_exception(e)
             return
 
         future.set_exception(payload)
 
+    async def handle_discover_request(self, event: RPCEvent) -> None:
+        self.writer.write(
+            self.protocol.pack(
+                list(self.executor.registry),
+                PacketTypes.DISCOVER_RESPONSE,
+                serial=event.header.serial,
+            ),
+        )
+
     async def step(self) -> None:
         event = await self.get_event()
         method = self.__method_map[event.header.type]
         await method(event)
 
     async def make_request(self, request: CallRequest) -> Any:
         serial = self.protocol.get_serial()
         future = self.loop.create_future()
         self.__results[serial] = future
         self.writer.write(
             self.protocol.pack(request, PacketTypes.REQUEST, serial=serial),
         )
         return await future
 
+    async def discover(self) -> List[str]:
+        self.writer.write(
+            self.protocol.pack(None, PacketTypes.DISCOVER_REQUEST),
+        )
+        while True:
+            event: RPCEvent = await self.get_event()
+
+            if event.header.type == PacketTypes.DISCOVER_REQUEST:
+                await self.handle_discover_request(event)
+                continue
+
+            return self.protocol.serializer.unpack(event.payload)
+
     @abstractmethod
     async def authorize(self) -> bool:
         raise NotImplementedError
 
     async def close(self) -> None:
         if not self.writer.can_write_eof():
             return
@@ -234,40 +256,45 @@
         ssl_context: Optional[ssl.SSLContext] = None,
         reconnect_timeout: TimeoutType = 1,
         serializer: AbstractSerializer = RestrictedPickleSerializer()
     ):
         self.protocol = Protocol(key=key, serializer=serializer)
         self.reconnect_timeout = reconnect_timeout
         self._ssl_context: Optional[ssl.SSLContext] = ssl_context
-        self.__handlers: Deque[PacketHandler] = deque()
+        self.__handlers: DefaultDict[str, Deque[PacketHandler]] = (
+            defaultdict(deque)
+        )
         self.__rotate_lock = asyncio.Lock()
 
         super().__init__(executor=executor)
 
-    async def _get_handler(self) -> PacketHandler:
+    async def _get_handler(self, method: str) -> PacketHandler:
         handler: PacketHandler
 
         async with self.__rotate_lock:
-            while not self.__handlers:
+            while method not in self.__handlers:
                 log.warning(
                     "No active connections, retrying after %.3f seconds.",
                     self.reconnect_timeout,
                 )
                 await asyncio.sleep(self.reconnect_timeout)
-
-            handler = self.__handlers.popleft()
-            self.__handlers.append(handler)
+            handler = self.__handlers[method].popleft()
+            self.__handlers[method].append(handler)
         return handler
 
-    async def _add_handler(self, handler: PacketHandler) -> None:
-        self.__handlers.append(handler)
+    async def _add_handler(
+        self, handler: PacketHandler, methods: Iterable[str],
+    ) -> None:
+        for method in methods:
+            self.__handlers[method].append(handler)
 
     async def _remove_handler(self, handler: PacketHandler) -> None:
         async with self.__rotate_lock:
-            self.__handlers.remove(handler)
+            for handlers in self.__handlers.values():
+                handlers.remove(handler)
 
     async def call(
         self,
         func: Union[str, TaskFunctionType],
         *args: Any,
         timeout: Optional[TimeoutType] = None,
         **kwargs: Any,
@@ -275,19 +302,19 @@
         if not isinstance(func, str):
             raise TypeError("Only strings supports")
 
         request = CallRequest(
             func=func, args=args, kwargs=kwargs, timeout=timeout,
         )
 
-        async def go() -> Any:
-            handler = await self._get_handler()
+        async def go(name: str) -> Any:
+            handler = await self._get_handler(name)
             return await handler.make_request(request)
 
-        return await asyncio.wait_for(go(), timeout=timeout)
+        return await asyncio.wait_for(go(func), timeout=timeout)
 
 
 DEFAULT_PORT = 15383
 
 
 @final
 class TCPServerBroker(TCPBrokerBase):
@@ -313,15 +340,17 @@
             executor=self.executor, protocol=self.protocol,
         )
 
         async def handle() -> None:
             if not await handler.authorize():
                 raise RuntimeError("Unauthorized")
 
-            await self._add_handler(handler)
+            methods = await handler.discover()
+
+            await self._add_handler(handler, methods or ())
 
             try:
                 await handler.start_processing()
             finally:
                 await self._remove_handler(handler)
 
         await self.create_task(handle())
@@ -368,17 +397,17 @@
                     handler = ClientPacketHandler(
                         reader=reader, writer=writer,
                         executor=self.executor, protocol=self.protocol,
                     )
                     if not await handler.authorize():
                         raise RuntimeError("Unauthorized")
 
+                    methods = await handler.discover()
                     on_connected.set()
-                    await self._add_handler(handler)
-
+                    await self._add_handler(handler, methods or ())
                     await handler.start_processing()
                 except asyncio.CancelledError:
                     if not writer.is_closing():
                         writer.close()
                         await writer.wait_closed()
                     raise
```

### Comparing `patio-0.1.2/patio/broker/tcp/protocol.py` & `patio-0.1.3/patio/broker/tcp/protocol.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 
 @unique
 class PacketTypes(IntEnum):
     AUTH_DIGEST = 0
     AUTH_REQUEST = 1
     AUTH_RESPONSE = 2
     AUTH_OK = 3
+    DISCOVER_REQUEST = 5
+    DISCOVER_RESPONSE = 6
     REQUEST = 10
     RESPONSE = 20
     ERROR = 30
 
 
 @dataclass
 class Header:
```

### Comparing `patio-0.1.2/patio/compat.py` & `patio-0.1.3/patio/compat.py`

 * *Files identical despite different names*

### Comparing `patio-0.1.2/patio/executor/asyncronous.py` & `patio-0.1.3/patio/executor/asyncronous.py`

 * *Files identical despite different names*

### Comparing `patio-0.1.2/patio/executor/base.py` & `patio-0.1.3/patio/executor/base.py`

 * *Files identical despite different names*

### Comparing `patio-0.1.2/patio/executor/null.py` & `patio-0.1.3/patio/executor/null.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,23 @@
+import copy
 from typing import Any, Awaitable, Callable
 
 from patio.executor.base import AbstractExecutor
 from patio.registry import T
 
 
 class NullExecutor(AbstractExecutor):
     """
     Doesn't execute anything, serves as a stub to explicitly forbid calls
     to this registry.
     """
 
     async def setup(self) -> None:
-        pass
+        self.registry = copy.copy(self.registry)
+        self.registry.clear()
 
     def submit(
         self, func: Callable[..., T], *args: Any, **kwargs: Any
     ) -> Awaitable[T]:
         raise RuntimeError("Null executor can't execute anything")
 
     async def shutdown(self) -> None:
```

### Comparing `patio-0.1.2/patio/executor/process_pool.py` & `patio-0.1.3/patio/executor/process_pool.py`

 * *Files identical despite different names*

### Comparing `patio-0.1.2/patio/executor/thread_pool.py` & `patio-0.1.3/patio/executor/thread_pool.py`

 * *Files identical despite different names*

### Comparing `patio-0.1.2/patio/registry.py` & `patio-0.1.3/patio/registry.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 from types import MappingProxyType
 from typing import (
     Any, Awaitable, Callable, DefaultDict, Dict, Generic, ItemsView, Iterator,
     KeysView, MutableMapping, Optional, Set, Tuple, TypeVar, Union, ValuesView,
     overload,
 )
 
+from patio.compat import Self
+
 
 T = TypeVar("T")
 
 AsyncTaskFunctionType = Callable[..., Awaitable[T]]
 SyncTaskFunctionType = Callable[..., T]
 TaskFunctionType = Union[AsyncTaskFunctionType, SyncTaskFunctionType]
 
@@ -297,14 +299,19 @@
         self.__locked = state["locked"]
         self.__store = {}
         self.__reverse_store = defaultdict(set)
 
         for name, func in state["store"].items():
             self[name] = func
 
+    def __copy__(self) -> Self:
+        clone = self.__class__()
+        clone.__setstate__(self.__getstate__())
+        return clone
+
 
 __all__ = (
     "AsyncTaskFunctionType",
     "Registry",
     "SyncTaskFunctionType",
     "T",
     "TaskFunctionType",
```

### Comparing `patio-0.1.2/pyproject.toml` & `patio-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "patio"
-version = "0.1.2"
+version = "0.1.3"
 description = "Python Asynchronous Task for AsyncIO"
 authors = ["Dmitry Orlov <me@mosquito.su>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/patio-python/patio/"
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `patio-0.1.2/PKG-INFO` & `patio-0.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: patio
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python Asynchronous Task for AsyncIO
 Home-page: https://github.com/patio-python/patio/
 License: MIT
 Author: Dmitry Orlov
 Author-email: me@mosquito.su
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -16,19 +16,14 @@
 Classifier: Natural Language :: Russian
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Dist: typing_extensions ; python_version < "3.11"
```

