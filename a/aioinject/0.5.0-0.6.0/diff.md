# Comparing `tmp/aioinject-0.5.0.tar.gz` & `tmp/aioinject-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioinject-0.5.0.tar", last modified: Sun Mar 26 00:31:11 2023, max compression
+gzip compressed data, was "aioinject-0.6.0.tar", last modified: Fri Jun  9 04:36:37 2023, max compression
```

## Comparing `aioinject-0.5.0.tar` & `aioinject-0.6.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0      429 2023-03-26 00:30:33.719360 aioinject-0.5.0/aioinject/__init__.py
--rw-r--r--   0        0        0     2394 2023-02-19 11:03:05.196585 aioinject-0.5.0/aioinject/containers.py
--rw-r--r--   0        0        0     5965 2023-02-19 10:57:53.754032 aioinject-0.5.0/aioinject/context.py
--rw-r--r--   0        0        0     3198 2023-02-19 10:45:20.646472 aioinject-0.5.0/aioinject/decorators.py
--rw-r--r--   0        0        0        0 2022-06-21 12:45:09.224983 aioinject-0.5.0/aioinject/ext/__init__.py
--rw-r--r--   0        0        0     1142 2023-02-19 10:46:32.417782 aioinject-0.5.0/aioinject/ext/fastapi.py
--rw-r--r--   0        0        0      866 2023-03-25 23:51:07.879400 aioinject-0.5.0/aioinject/ext/strawberry.py
--rw-r--r--   0        0        0      154 2022-02-14 23:34:38.786956 aioinject-0.5.0/aioinject/markers.py
--rw-r--r--   0        0        0     5852 2023-02-19 10:37:32.040086 aioinject-0.5.0/aioinject/providers.py
--rw-r--r--   0        0        0     1063 2023-02-19 10:45:09.937041 aioinject-0.5.0/aioinject/utils.py
--rw-r--r--   0        0        0     1063 2022-02-10 14:33:31.888253 aioinject-0.5.0/LICENSE
--rw-r--r--   0        0        0     1966 2023-03-26 00:30:33.783358 aioinject-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     5266 2022-05-25 14:51:11.254512 aioinject-0.5.0/readme.md
--rw-r--r--   0        0        0        0 2022-02-10 14:33:31.896255 aioinject-0.5.0/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-02-19 10:38:23.524000 aioinject-0.5.0/tests/container/__init__.py
--rw-r--r--   0        0        0     2661 2023-02-19 10:35:54.333887 aioinject-0.5.0/tests/container/test_container.py
--rw-r--r--   0        0        0      489 2023-02-18 10:15:01.863109 aioinject-0.5.0/tests/container/test_override.py
--rw-r--r--   0        0        0        0 2022-02-14 23:35:15.649789 aioinject-0.5.0/tests/context/__init__.py
--rw-r--r--   0        0        0      500 2023-02-18 10:10:22.057657 aioinject-0.5.0/tests/context/conftest.py
--rw-r--r--   0        0        0     2022 2023-02-18 10:10:14.586441 aioinject-0.5.0/tests/context/test_context.py
--rw-r--r--   0        0        0     4254 2023-02-19 10:37:20.641899 aioinject-0.5.0/tests/context/test_context_managers.py
--rw-r--r--   0        0        0     2060 2023-02-18 11:02:03.522559 aioinject-0.5.0/tests/context/test_execute.py
--rw-r--r--   0        0        0        0 2023-02-19 10:38:23.524000 aioinject-0.5.0/tests/ext/__init__.py
--rw-r--r--   0        0        0        0 2023-02-19 10:38:23.524000 aioinject-0.5.0/tests/ext/strawberry/__init__.py
--rw-r--r--   0        0        0      818 2023-02-18 11:06:42.742442 aioinject-0.5.0/tests/ext/strawberry/test_inject_decorator.py
--rw-r--r--   0        0        0        0 2022-02-10 14:33:31.897254 aioinject-0.5.0/tests/providers/__init__.py
--rw-r--r--   0        0        0     4257 2023-02-19 10:29:06.577098 aioinject-0.5.0/tests/providers/test_callable.py
--rw-r--r--   0        0        0     1139 2023-02-18 11:02:25.628622 aioinject-0.5.0/tests/providers/test_object.py
--rw-r--r--   0        0        0      686 2023-02-18 09:50:26.751944 aioinject-0.5.0/tests/providers/test_singleton.py
--rw-r--r--   0        0        0     3845 2023-02-19 10:03:00.125198 aioinject-0.5.0/tests/test_inject.py
--rw-r--r--   0        0        0       39 2022-08-16 11:16:21.152175 aioinject-0.5.0/tests/utils/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2022-08-16 11:16:21.153175 aioinject-0.5.0/tests/utils/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      310 2022-08-16 11:16:21.152175 aioinject-0.5.0/tests/utils/.pytest_cache/README.md
--rw-r--r--   0        0        0       43 2022-08-16 11:16:21.153175 aioinject-0.5.0/tests/utils/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2022-08-16 11:16:21.154175 aioinject-0.5.0/tests/utils/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0        0 2023-02-19 10:38:23.524819 aioinject-0.5.0/tests/utils/__init__.py
--rw-r--r--   0        0        0     1502 2023-02-19 10:35:54.331885 aioinject-0.5.0/tests/utils/test_guess_impl.py
--rw-r--r--   0        0        0      520 2023-02-18 11:01:50.087958 aioinject-0.5.0/tests/utils/test_utils.py
--rw-r--r--   0        0        0     5443 1970-01-01 00:00:00.000000 aioinject-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      429 2023-06-09 04:36:24.553667 aioinject-0.6.0/aioinject/__init__.py
+-rw-r--r--   0        0        0     2701 2023-06-09 04:28:13.918025 aioinject-0.6.0/aioinject/containers.py
+-rw-r--r--   0        0        0     6734 2023-06-09 04:31:32.178144 aioinject-0.6.0/aioinject/context.py
+-rw-r--r--   0        0        0     3198 2023-02-19 10:45:20.646472 aioinject-0.6.0/aioinject/decorators.py
+-rw-r--r--   0        0        0        0 2022-06-21 12:45:09.224983 aioinject-0.6.0/aioinject/ext/__init__.py
+-rw-r--r--   0        0        0     1142 2023-02-19 10:46:32.417782 aioinject-0.6.0/aioinject/ext/fastapi.py
+-rw-r--r--   0        0        0      866 2023-03-25 23:51:07.879400 aioinject-0.6.0/aioinject/ext/strawberry.py
+-rw-r--r--   0        0        0      154 2022-02-14 23:34:38.786956 aioinject-0.6.0/aioinject/markers.py
+-rw-r--r--   0        0        0     5852 2023-02-19 10:37:32.040086 aioinject-0.6.0/aioinject/providers.py
+-rw-r--r--   0        0        0     1063 2023-02-19 10:45:09.937041 aioinject-0.6.0/aioinject/utils.py
+-rw-r--r--   0        0        0     1063 2022-02-10 14:33:31.888253 aioinject-0.6.0/LICENSE
+-rw-r--r--   0        0        0     1966 2023-06-09 04:36:24.617667 aioinject-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     5266 2022-05-25 14:51:11.254512 aioinject-0.6.0/readme.md
+-rw-r--r--   0        0        0        0 2022-02-10 14:33:31.896255 aioinject-0.6.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-19 10:38:23.524000 aioinject-0.6.0/tests/container/__init__.py
+-rw-r--r--   0        0        0     3271 2023-06-09 04:28:11.487983 aioinject-0.6.0/tests/container/test_container.py
+-rw-r--r--   0        0        0      489 2023-02-18 10:15:01.863109 aioinject-0.6.0/tests/container/test_override.py
+-rw-r--r--   0        0        0        0 2022-02-14 23:35:15.649789 aioinject-0.6.0/tests/context/__init__.py
+-rw-r--r--   0        0        0      500 2023-02-18 10:10:22.057657 aioinject-0.6.0/tests/context/conftest.py
+-rw-r--r--   0        0        0     2022 2023-02-18 10:10:14.586441 aioinject-0.6.0/tests/context/test_context.py
+-rw-r--r--   0        0        0     4256 2023-06-09 04:35:11.554281 aioinject-0.6.0/tests/context/test_context_managers.py
+-rw-r--r--   0        0        0     2060 2023-02-18 11:02:03.522559 aioinject-0.6.0/tests/context/test_execute.py
+-rw-r--r--   0        0        0        0 2023-02-19 10:38:23.524000 aioinject-0.6.0/tests/ext/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-19 10:38:23.524000 aioinject-0.6.0/tests/ext/strawberry/__init__.py
+-rw-r--r--   0        0        0      818 2023-02-18 11:06:42.742442 aioinject-0.6.0/tests/ext/strawberry/test_inject_decorator.py
+-rw-r--r--   0        0        0        0 2022-02-10 14:33:31.897254 aioinject-0.6.0/tests/providers/__init__.py
+-rw-r--r--   0        0        0     4257 2023-02-19 10:29:06.577098 aioinject-0.6.0/tests/providers/test_callable.py
+-rw-r--r--   0        0        0     1139 2023-02-18 11:02:25.628622 aioinject-0.6.0/tests/providers/test_object.py
+-rw-r--r--   0        0        0      686 2023-02-18 09:50:26.751944 aioinject-0.6.0/tests/providers/test_singleton.py
+-rw-r--r--   0        0        0     3845 2023-02-19 10:03:00.125198 aioinject-0.6.0/tests/test_inject.py
+-rw-r--r--   0        0        0       39 2022-08-16 11:16:21.152175 aioinject-0.6.0/tests/utils/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2022-08-16 11:16:21.153175 aioinject-0.6.0/tests/utils/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      310 2022-08-16 11:16:21.152175 aioinject-0.6.0/tests/utils/.pytest_cache/README.md
+-rw-r--r--   0        0        0       43 2022-08-16 11:16:21.153175 aioinject-0.6.0/tests/utils/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2022-08-16 11:16:21.154175 aioinject-0.6.0/tests/utils/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0        0 2023-02-19 10:38:23.524819 aioinject-0.6.0/tests/utils/__init__.py
+-rw-r--r--   0        0        0     1502 2023-02-19 10:35:54.331885 aioinject-0.6.0/tests/utils/test_guess_impl.py
+-rw-r--r--   0        0        0      520 2023-02-18 11:01:50.087958 aioinject-0.6.0/tests/utils/test_utils.py
+-rw-r--r--   0        0        0     5443 1970-01-01 00:00:00.000000 aioinject-0.6.0/PKG-INFO
```

### Comparing `aioinject-0.5.0/aioinject/containers.py` & `aioinject-0.6.0/aioinject/containers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import contextlib
 from collections import defaultdict
 from collections.abc import Generator
+from contextlib import AsyncExitStack
 from typing import Any, TypeVar
 
 from .context import InjectionContext, SyncInjectionContext
 from .providers import Provider
 
 _T = TypeVar("_T")
 _Providers = dict[type[_T], list[Provider[_T]]]
 
 
 class Container:
     def __init__(self) -> None:
         self.providers: _Providers = defaultdict(list)
         self._overrides: _Providers = defaultdict(list)
+        self._exit_stack = AsyncExitStack()
 
     def register(
         self,
         provider: Provider[_T],
     ) -> None:
         if provider.type not in self.providers:
             self.providers[provider.type] = []
@@ -58,20 +60,29 @@
         provider = self._get_provider(self.providers, type_, impl)
         if provider is None:
             err_msg = f"Provider for type {type_.__qualname__} not found"
             raise ValueError(err_msg)
         return provider
 
     def context(self) -> InjectionContext:
-        return InjectionContext(container=self)
+        return InjectionContext(
+            container=self,
+            singleton_exit_stack=self._exit_stack,
+        )
 
     def sync_context(self) -> SyncInjectionContext:
-        return SyncInjectionContext(container=self)
+        return SyncInjectionContext(
+            container=self,
+            singleton_exit_stack=self._exit_stack,
+        )
 
     @contextlib.contextmanager
     def override(
         self,
         provider: Provider[_T],
     ) -> Generator[None, None, None]:
         self._overrides[provider.type].append(provider)
         yield
         self._overrides[provider.type].remove(provider)
+
+    async def aclose(self) -> None:
+        await self._exit_stack.aclose()
```

### Comparing `aioinject-0.5.0/aioinject/context.py` & `aioinject-0.6.0/aioinject/context.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,108 +1,135 @@
 from __future__ import annotations
 
 import contextlib
 import contextvars
 import inspect
 import typing
 from collections.abc import Callable, Coroutine, Iterable
+from contextlib import AsyncExitStack, ExitStack
 from contextvars import ContextVar
 from types import TracebackType
-from typing import TYPE_CHECKING, Any, Protocol, TypeVar, Union
+from typing import TYPE_CHECKING, Any, Generic, Protocol, TypeVar, Union
 
-from .providers import Dependency
+from .providers import Dependency, Provider, Singleton
 
 if TYPE_CHECKING:
     from .containers import Container
 
 _T = TypeVar("_T")
 
 _AnyCtx = Union["InjectionContext", "SyncInjectionContext"]
 context_var: ContextVar[_AnyCtx] = ContextVar("aioinject_context")
 
 container_var: ContextVar[Container] = ContextVar("aioinject_container")
 
-
 TypeAndImpl = tuple[type[_T], _T | None]
+TExitStack = TypeVar("TExitStack")
 
 
 class DiCache(Protocol):
     def __setitem__(self, key: TypeAndImpl[_T], value: _T) -> None:
-        ...
+        ...  # pragma: no cover
 
     def __getitem__(self, item: TypeAndImpl[_T]) -> _T:
-        ...
+        ...  # pragma: no cover
 
     def __contains__(self, item: TypeAndImpl) -> bool:
-        ...
+        ...  # pragma: no cover
 
 
-class _BaseInjectionContext:
+class _BaseInjectionContext(Generic[TExitStack]):
     _token: contextvars.Token | None
+    _exit_stack_type: type[TExitStack]
 
-    def __init__(self, container: Container) -> None:
+    def __init__(
+        self,
+        container: Container,
+        singleton_exit_stack: AsyncExitStack,
+    ) -> None:
         self.container = container
+        self.singleton_exit_stack = singleton_exit_stack
+        self.exit_stack = self._exit_stack_type()
         self.cache: DiCache = {}
         self._token = None
 
+    def __class_getitem__(
+        cls,
+        item: type[TExitStack],
+    ) -> _BaseInjectionContext[TExitStack]:
+        return type(  # type: ignore[return-value]
+            f"_BaseInjectionContext[{item.__class__.__name__}]",
+            (cls,),
+            {"_exit_stack_type": item},
+        )
+
+    def _get_exit_stack(
+        self,
+        provider: Provider,
+    ) -> TExitStack | AsyncExitStack:
+        if isinstance(provider, Singleton):
+            return self.singleton_exit_stack
+        return self.exit_stack
 
-class InjectionContext(_BaseInjectionContext):
-    def __init__(self, container: Container) -> None:
-        super().__init__(container=container)
-        self.exit_stack = contextlib.AsyncExitStack()
 
+class InjectionContext(_BaseInjectionContext[AsyncExitStack]):
     async def resolve(
         self,
         type_: type[_T],
         impl: Any | None = None,
         *,
         use_cache: bool = True,
     ) -> _T:
         if use_cache and (type_, impl) in self.cache:
             return self.cache[type_, impl]
+
         provider = self.container.get_provider(type_, impl)
         dependencies = {
             dep.name: await self.resolve(
                 type_=dep.type_,
                 impl=dep.implementation,
                 use_cache=dep.use_cache,
             )
             for dep in provider.dependencies
         }
 
         resolved = await provider.provide(**dependencies)
+        stack = self._get_exit_stack(provider=provider)
+
         if isinstance(resolved, contextlib.ContextDecorator):
-            resolved = self.exit_stack.enter_context(resolved)  # type: ignore[arg-type]
+            resolved = stack.enter_context(resolved)  # type: ignore[arg-type]
 
         if isinstance(resolved, contextlib.AsyncContextDecorator):
-            resolved = await self.exit_stack.enter_async_context(resolved)  # type: ignore[arg-type]
+            resolved = await stack.enter_async_context(
+                resolved,  # type: ignore[arg-type]
+            )
 
         if use_cache:
             self.cache[type_, impl] = resolved
         return resolved
 
     @typing.overload
     async def execute(
         self,
         function: Callable[..., Coroutine[Any, Any, _T]],
         dependencies: Iterable[Dependency],
         *args: Any,
         **kwargs: Any,
     ) -> _T:
-        ...
+        ...  # pragma: no cover
 
     @typing.overload
     async def execute(
         self,
         function: Callable[..., _T],
         dependencies: Iterable[Dependency],
         *args: Any,
         **kwargs: Any,
     ) -> _T:
-        ...
+        ...  # pragma: no cover
 
     async def execute(
         self,
         function: Callable[..., Coroutine[Any, Any, _T] | _T],
         dependencies: Iterable[Dependency],
         *args: Any,
         **kwargs: Any,
@@ -130,19 +157,15 @@
         exc_val: BaseException | None,
         exc_tb: TracebackType | None,
     ) -> None:
         context_var.reset(self._token)  # type: ignore[arg-type]
         await self.exit_stack.__aexit__(exc_type, exc_val, exc_tb)
 
 
-class SyncInjectionContext(_BaseInjectionContext):
-    def __init__(self, container: Container) -> None:
-        super().__init__(container=container)
-        self.exit_stack = contextlib.ExitStack()
-
+class SyncInjectionContext(_BaseInjectionContext[ExitStack]):
     def resolve(
         self,
         type_: type[_T],
         impl: Any | None = None,
         *,
         use_cache: bool = True,
     ) -> _T:
```

### Comparing `aioinject-0.5.0/aioinject/decorators.py` & `aioinject-0.6.0/aioinject/decorators.py`

 * *Files identical despite different names*

### Comparing `aioinject-0.5.0/aioinject/ext/fastapi.py` & `aioinject-0.6.0/aioinject/ext/fastapi.py`

 * *Files identical despite different names*

### Comparing `aioinject-0.5.0/aioinject/ext/strawberry.py` & `aioinject-0.6.0/aioinject/ext/strawberry.py`

 * *Files identical despite different names*

### Comparing `aioinject-0.5.0/aioinject/providers.py` & `aioinject-0.6.0/aioinject/providers.py`

 * *Files identical despite different names*

### Comparing `aioinject-0.5.0/aioinject/utils.py` & `aioinject-0.6.0/aioinject/utils.py`

 * *Files identical despite different names*

### Comparing `aioinject-0.5.0/LICENSE` & `aioinject-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aioinject-0.5.0/pyproject.toml` & `aioinject-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 composite = [
     "coverage run",
     "coverage report",
 ]
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.5.0"
+version = "0.6.0"
 version_files = [
     "aioinject/__init__.py",
     "pyproject.toml:version",
 ]
 
 [tool.coverage.run]
 source = [
@@ -108,15 +108,15 @@
 ]
 staticmethod-decorators = [
     "staticmethod",
 ]
 
 [project]
 name = "aioinject"
-version = "0.5.0"
+version = "0.6.0"
 description = ""
 authors = [
     { name = "Doctor", email = "thirvondukr@gmail.com" },
 ]
 dependencies = []
 requires-python = ">=3.10"
 readme = "readme.md"
```

### Comparing `aioinject-0.5.0/readme.md` & `aioinject-0.6.0/readme.md`

 * *Files identical despite different names*

### Comparing `aioinject-0.5.0/tests/container/test_container.py` & `aioinject-0.6.0/tests/container/test_container.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,13 @@
+import contextlib
+from collections.abc import AsyncIterator
+
 import pytest
 
-from aioinject import providers
+from aioinject import Singleton, providers
 from aioinject.containers import Container
 from aioinject.context import InjectionContext
 
 
 class _AbstractService:
     pass
 
@@ -88,7 +91,30 @@
 def test_missing_provider() -> None:
     container = Container()
     with pytest.raises(ValueError) as exc_info:  # noqa: PT011
         assert container.get_provider(_ServiceA)
 
     msg = f"Provider for type {_ServiceA.__qualname__} not found"
     assert str(exc_info.value) == msg
+
+
+@pytest.mark.anyio
+async def test_should_close_singletons() -> None:
+    shutdown = False
+
+    @contextlib.asynccontextmanager
+    async def dependency() -> AsyncIterator[int]:
+        nonlocal shutdown
+
+        yield 42
+        shutdown = True
+
+    provider = Singleton(dependency)
+
+    container = Container()
+    container.register(provider)
+    async with container.context() as ctx:
+        assert await ctx.resolve(int) == 42  # noqa: PLR2004
+    assert shutdown is False
+
+    await container.aclose()
+    assert shutdown is True
```

### Comparing `aioinject-0.5.0/tests/context/test_context.py` & `aioinject-0.6.0/tests/context/test_context.py`

 * *Files identical despite different names*

### Comparing `aioinject-0.5.0/tests/context/test_context_managers.py` & `aioinject-0.6.0/tests/context/test_context_managers.py`

 * *Files 4% similar despite different names*

```diff
@@ -120,27 +120,30 @@
     instance.mock.open.assert_not_called()
     instance.mock.close.assert_not_called()
 
 
 def test_sync_context_manager_should_receive_exception() -> None:
     mock = MagicMock()
 
+    class TestError(Exception):
+        pass
+
     @contextlib.contextmanager
     def get_session() -> Iterator[_Session]:
         try:
             yield _Session()
-        except Exception:  # noqa: BLE001
+        except TestError:
             mock.exception_happened()
 
     container = Container()
     container.register(Callable(get_session))
 
     with (  # noqa: PT012
-        pytest.raises(Exception),  # noqa: PT011
+        pytest.raises(TestError),
         container.sync_context() as ctx,
     ):
         session = ctx.resolve(_Session)
         assert isinstance(session, _Session)
         mock.exception_happened.assert_not_called()
-        raise Exception  # noqa: TRY002
+        raise TestError
 
     mock.exception_happened.asssert_called_once()
```

### Comparing `aioinject-0.5.0/tests/context/test_execute.py` & `aioinject-0.6.0/tests/context/test_execute.py`

 * *Files identical despite different names*

### Comparing `aioinject-0.5.0/tests/ext/strawberry/test_inject_decorator.py` & `aioinject-0.6.0/tests/ext/strawberry/test_inject_decorator.py`

 * *Files identical despite different names*

### Comparing `aioinject-0.5.0/tests/providers/test_callable.py` & `aioinject-0.6.0/tests/providers/test_callable.py`

 * *Files identical despite different names*

### Comparing `aioinject-0.5.0/tests/providers/test_object.py` & `aioinject-0.6.0/tests/providers/test_object.py`

 * *Files identical despite different names*

### Comparing `aioinject-0.5.0/tests/providers/test_singleton.py` & `aioinject-0.6.0/tests/providers/test_singleton.py`

 * *Files identical despite different names*

### Comparing `aioinject-0.5.0/tests/test_inject.py` & `aioinject-0.6.0/tests/test_inject.py`

 * *Files identical despite different names*

### Comparing `aioinject-0.5.0/tests/utils/test_guess_impl.py` & `aioinject-0.6.0/tests/utils/test_guess_impl.py`

 * *Files identical despite different names*

### Comparing `aioinject-0.5.0/tests/utils/test_utils.py` & `aioinject-0.6.0/tests/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `aioinject-0.5.0/PKG-INFO` & `aioinject-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioinject
-Version: 0.5.0
+Version: 0.6.0
 License: MIT
 Author-email: Doctor <thirvondukr@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 Async-first dependency injection library based on python type hints
```

