# Comparing `tmp/troncos-4.0.0b8.tar.gz` & `tmp/troncos-4.0.0b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "troncos-4.0.0b8.tar", max compression
+gzip compressed data, was "troncos-4.0.0b9.tar", max compression
```

## Comparing `troncos-4.0.0b8.tar` & `troncos-4.0.0b9.tar`

### file list

```diff
@@ -1,36 +1,39 @@
--rw-r--r--   0        0        0     1077 2023-05-30 09:10:51.497222 troncos-4.0.0b8/LICENSE
--rw-r--r--   0        0        0     7753 2023-05-30 09:10:51.497222 troncos-4.0.0b8/README.md
--rw-r--r--   0        0        0     2389 2023-05-30 09:10:51.501222 troncos-4.0.0b8/pyproject.toml
--rw-r--r--   0        0        0      291 2023-05-30 09:10:51.501222 troncos-4.0.0b8/troncos/__init__.py
--rw-r--r--   0        0        0        0 2023-05-30 09:10:51.501222 troncos-4.0.0b8/troncos/contrib/__init__.py
--rw-r--r--   0        0        0        0 2023-05-30 09:10:51.501222 troncos-4.0.0b8/troncos/contrib/asgi/__init__.py
--rw-r--r--   0        0        0        0 2023-05-30 09:10:51.501222 troncos-4.0.0b8/troncos/contrib/asgi/logging/__init__.py
--rw-r--r--   0        0        0     5058 2023-05-30 09:10:51.501222 troncos-4.0.0b8/troncos/contrib/asgi/logging/middleware.py
--rw-r--r--   0        0        0        0 2023-05-30 09:10:51.501222 troncos-4.0.0b8/troncos/contrib/asgi/profiling/__init__.py
--rw-r--r--   0        0        0      576 2023-05-30 09:10:51.501222 troncos-4.0.0b8/troncos/contrib/asgi/profiling/app.py
--rw-r--r--   0        0        0        0 2023-05-30 09:10:51.501222 troncos-4.0.0b8/troncos/contrib/celery/__init__.py
--rw-r--r--   0        0        0        0 2023-05-30 09:10:51.501222 troncos-4.0.0b8/troncos/contrib/celery/logging/__init__.py
--rw-r--r--   0        0        0      949 2023-05-30 09:10:51.501222 troncos-4.0.0b8/troncos/contrib/celery/logging/signals.py
--rw-r--r--   0        0        0        0 2023-05-30 09:10:51.501222 troncos-4.0.0b8/troncos/contrib/django/__init__.py
--rw-r--r--   0        0        0        0 2023-05-30 09:10:51.501222 troncos-4.0.0b8/troncos/contrib/django/logging/__init__.py
--rw-r--r--   0        0        0     2334 2023-05-30 09:10:51.501222 troncos-4.0.0b8/troncos/contrib/django/logging/middleware.py
--rw-r--r--   0        0        0        0 2023-05-30 09:10:51.501222 troncos-4.0.0b8/troncos/contrib/django/profiling/__init__.py
--rw-r--r--   0        0        0      265 2023-05-30 09:10:51.501222 troncos-4.0.0b8/troncos/contrib/django/profiling/views.py
--rw-r--r--   0        0        0        0 2023-05-30 09:10:51.501222 troncos-4.0.0b8/troncos/contrib/starlette/__init__.py
--rw-r--r--   0        0        0        0 2023-05-30 09:10:51.501222 troncos-4.0.0b8/troncos/contrib/starlette/profiling/__init__.py
--rw-r--r--   0        0        0      291 2023-05-30 09:10:51.501222 troncos-4.0.0b8/troncos/contrib/starlette/profiling/views.py
--rw-r--r--   0        0        0     4053 2023-05-30 09:10:51.501222 troncos-4.0.0b8/troncos/contrib/structlog/__init__.py
--rw-r--r--   0        0        0      705 2023-05-30 09:10:51.501222 troncos-4.0.0b8/troncos/contrib/structlog/processors.py
--rw-r--r--   0        0        0        0 2023-05-30 09:10:51.501222 troncos-4.0.0b8/troncos/profiling/__init__.py
--rw-r--r--   0        0        0      192 2023-05-30 09:10:51.501222 troncos-4.0.0b8/troncos/profiling/auto.py
--rw-r--r--   0        0        0        0 2023-05-30 09:10:51.501222 troncos-4.0.0b8/troncos/profiling/bootstrap/__init__.py
--rw-r--r--   0        0        0      439 2023-05-30 09:10:51.501222 troncos-4.0.0b8/troncos/profiling/bootstrap/profile.py
--rw-r--r--   0        0        0      343 2023-05-30 09:10:51.501222 troncos-4.0.0b8/troncos/profiling/bootstrap/start.py
--rw-r--r--   0        0        0     1814 2023-05-30 09:10:51.501222 troncos-4.0.0b8/troncos/profiling/profiler.py
--rw-r--r--   0        0        0        0 2023-05-30 09:10:51.501222 troncos-4.0.0b8/troncos/py.typed
--rw-r--r--   0        0        0      690 2023-05-30 09:10:51.501222 troncos-4.0.0b8/troncos/tracing/__init__.py
--rw-r--r--   0        0        0       82 2023-05-30 09:10:51.501222 troncos-4.0.0b8/troncos/tracing/_enums.py
--rw-r--r--   0        0        0     2053 2023-05-30 09:10:51.501222 troncos-4.0.0b8/troncos/tracing/_otel.py
--rw-r--r--   0        0        0     4545 2023-05-30 09:10:51.501222 troncos-4.0.0b8/troncos/tracing/_span.py
--rw-r--r--   0        0        0     1884 2023-05-30 09:10:51.501222 troncos-4.0.0b8/troncos/tracing/_writer.py
--rw-r--r--   0        0        0     8744 1970-01-01 00:00:00.000000 troncos-4.0.0b8/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-06-02 06:54:10.106833 troncos-4.0.0b9/LICENSE
+-rw-r--r--   0        0        0     7753 2023-06-02 06:54:10.106833 troncos-4.0.0b9/README.md
+-rw-r--r--   0        0        0     2389 2023-06-02 06:54:10.106833 troncos-4.0.0b9/pyproject.toml
+-rw-r--r--   0        0        0      291 2023-06-02 06:54:10.106833 troncos-4.0.0b9/troncos/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-02 06:54:10.106833 troncos-4.0.0b9/troncos/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-02 06:54:10.106833 troncos-4.0.0b9/troncos/contrib/asgi/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-02 06:54:10.106833 troncos-4.0.0b9/troncos/contrib/asgi/logging/__init__.py
+-rw-r--r--   0        0        0     5297 2023-06-02 06:54:10.106833 troncos-4.0.0b9/troncos/contrib/asgi/logging/middleware.py
+-rw-r--r--   0        0        0        0 2023-06-02 06:54:10.106833 troncos-4.0.0b9/troncos/contrib/asgi/profiling/__init__.py
+-rw-r--r--   0        0        0      576 2023-06-02 06:54:10.106833 troncos-4.0.0b9/troncos/contrib/asgi/profiling/app.py
+-rw-r--r--   0        0        0        0 2023-06-02 06:54:10.106833 troncos-4.0.0b9/troncos/contrib/celery/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-02 06:54:10.110833 troncos-4.0.0b9/troncos/contrib/celery/logging/__init__.py
+-rw-r--r--   0        0        0      969 2023-06-02 06:54:10.110833 troncos-4.0.0b9/troncos/contrib/celery/logging/signals.py
+-rw-r--r--   0        0        0        0 2023-06-02 06:54:10.110833 troncos-4.0.0b9/troncos/contrib/django/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-02 06:54:10.110833 troncos-4.0.0b9/troncos/contrib/django/logging/__init__.py
+-rw-r--r--   0        0        0     2354 2023-06-02 06:54:10.110833 troncos-4.0.0b9/troncos/contrib/django/logging/middleware.py
+-rw-r--r--   0        0        0        0 2023-06-02 06:54:10.110833 troncos-4.0.0b9/troncos/contrib/django/profiling/__init__.py
+-rw-r--r--   0        0        0      259 2023-06-02 06:54:10.110833 troncos-4.0.0b9/troncos/contrib/django/profiling/views.py
+-rw-r--r--   0        0        0        0 2023-06-02 06:54:10.110833 troncos-4.0.0b9/troncos/contrib/logging/__init__.py
+-rw-r--r--   0        0        0     3455 2023-06-02 06:54:10.110833 troncos-4.0.0b9/troncos/contrib/logging/tools/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-02 06:54:10.110833 troncos-4.0.0b9/troncos/contrib/starlette/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-02 06:54:10.110833 troncos-4.0.0b9/troncos/contrib/starlette/profiling/__init__.py
+-rw-r--r--   0        0        0      291 2023-06-02 06:54:10.110833 troncos-4.0.0b9/troncos/contrib/starlette/profiling/views.py
+-rw-r--r--   0        0        0     4148 2023-06-02 06:54:10.110833 troncos-4.0.0b9/troncos/contrib/structlog/__init__.py
+-rw-r--r--   0        0        0      906 2023-06-02 06:54:10.110833 troncos-4.0.0b9/troncos/contrib/structlog/processors.py
+-rw-r--r--   0        0        0        0 2023-06-02 06:54:10.110833 troncos-4.0.0b9/troncos/profiling/__init__.py
+-rw-r--r--   0        0        0      192 2023-06-02 06:54:10.110833 troncos-4.0.0b9/troncos/profiling/auto.py
+-rw-r--r--   0        0        0        0 2023-06-02 06:54:10.110833 troncos-4.0.0b9/troncos/profiling/bootstrap/__init__.py
+-rw-r--r--   0        0        0      439 2023-06-02 06:54:10.110833 troncos-4.0.0b9/troncos/profiling/bootstrap/profile.py
+-rw-r--r--   0        0        0      343 2023-06-02 06:54:10.110833 troncos-4.0.0b9/troncos/profiling/bootstrap/start.py
+-rw-r--r--   0        0        0     1814 2023-06-02 06:54:10.110833 troncos-4.0.0b9/troncos/profiling/profiler.py
+-rw-r--r--   0        0        0        0 2023-06-02 06:54:10.110833 troncos-4.0.0b9/troncos/py.typed
+-rw-r--r--   0        0        0      690 2023-06-02 06:54:10.110833 troncos-4.0.0b9/troncos/tracing/__init__.py
+-rw-r--r--   0        0        0       82 2023-06-02 06:54:10.110833 troncos-4.0.0b9/troncos/tracing/_enums.py
+-rw-r--r--   0        0        0     2053 2023-06-02 06:54:10.110833 troncos-4.0.0b9/troncos/tracing/_otel.py
+-rw-r--r--   0        0        0     4545 2023-06-02 06:54:10.110833 troncos-4.0.0b9/troncos/tracing/_span.py
+-rw-r--r--   0        0        0     1884 2023-06-02 06:54:10.110833 troncos-4.0.0b9/troncos/tracing/_writer.py
+-rw-r--r--   0        0        0     7585 2023-06-02 06:54:10.110833 troncos-4.0.0b9/troncos/tracing/decorators.py
+-rw-r--r--   0        0        0     8744 1970-01-01 00:00:00.000000 troncos-4.0.0b9/PKG-INFO
```

### Comparing `troncos-4.0.0b8/LICENSE` & `troncos-4.0.0b9/LICENSE`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b8/README.md` & `troncos-4.0.0b9/README.md`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b8/pyproject.toml` & `troncos-4.0.0b9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "troncos"
-version = "4.0.0b8"
+version = "4.0.0b9"
 description = "Collection of Python logging, tracing and profiling tools"
 authors = [
     "Guðmundur Björn Birkisson <gudmundur.birkisson@oda.com>",
     "Karl Fredrik Haugland <karlfredrik.haugland@oda.com>",
     "Eirik Martiniussen Sylliaas <eirik.sylliaas@oda.com>",
 ]
 license = "MIT"
```

### Comparing `troncos-4.0.0b8/troncos/contrib/asgi/logging/middleware.py` & `troncos-4.0.0b9/troncos/contrib/asgi/logging/middleware.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import time
 from typing import Any, Awaitable, Callable, Iterator, Mapping, MutableMapping
 
+import ddtrace
 from ipware import IpWare
 
 try:
     from structlog import get_logger
 except ImportError:
     raise RuntimeError(
         "Structlog must be installed to use the asgi logging middleware."
@@ -88,17 +89,17 @@
 
     def __init__(
         self,
         app: Any,
         logger_name: str | None = None,
     ) -> None:
         self._app = app
-        ln = logger_name or "asgi"
-        self._access = get_logger(f"troncos.{ln}.access")
-        self._error = get_logger(f"troncos.{ln}.error")
+        ln = logger_name or "troncos.asgi"
+        self._access = get_logger(f"{ln}.access")
+        self._error = get_logger(f"{ln}.error")
 
     async def __call__(
         self,
         scope: dict[str, Any],
         receive: Callable[[Any], Any],
         send: Callable[[dict[str, Any]], Awaitable[Any]],
     ) -> Any:
@@ -117,45 +118,43 @@
         http_version = scope.get("http_version")
         status = [0]
         start_time = time.perf_counter()
 
         async def wrapped_send(message: dict[str, Any]) -> None:
             if "status" in message:
                 status[0] = message.get("status", 0)
-
             await send(message)
 
-            # "more_body" is used if there is still data to send. Log the request
-            # when "http.response.body" has no more data left to send in the response.
-            if message.get("type") == "http.response.body" and not message.get(
-                "more_body", False
-            ):
-                extra = {
-                    "http_client_addr": str(client_ip) if client_ip else "NO_IP",
-                    "http_method": method,
-                    "http_path": path,
-                    "http_version": http_version,
-                    "http_status_code": status[0],
-                    "duration": time.perf_counter() - start_time,
-                }
-                self._access.info(
-                    "",
-                    **extra,
-                )
+        log_fn = self._access.info
+        extra = {}
+
+        # Earlier implementations of this middleware logged calls in the 'wrapped_send'
+        # function above, and made it the responsibility of the trace injection log
+        # processor to add the trace/span id to the log entry. The problem is that the
+        # ASGI TraceMiddleware defined in ddtrace, sometimes ends the span during the
+        # 'send(message)' call, and so the trace injection processor would not see the
+        # trace context, and therefore not log the trace/span id.
+        #
+        # To ensure that the trace information is always logged, we simply inject that
+        # information in here, and by doing so we do not have to care about the
+        # internals of the ASGI TraceMiddleware in ddtrace.
+        if dd_context := ddtrace.tracer.current_trace_context():
+            extra["trace_id"] = f"{dd_context.trace_id:x}"
+            extra["span_id"] = f"{dd_context.span_id:x}"
 
         try:
             return await self._app(scope, receive, wrapped_send)
         except Exception as e:
-            extra = {
-                "http_client_addr": str(client_ip) if client_ip else "NO_IP",
-                "http_method": method,
-                "http_path": path,
-                "http_version": http_version,
-                "http_status_code": 500,
-                "duration": time.perf_counter() - start_time,
-            }
-
-            self._error.exception(
-                "",
+            status[0] = 500
+            log_fn = self._error.exception
+            raise e
+        finally:
+            log_fn(
+                "ASGI HTTP response",
+                http_client_addr=str(client_ip) if client_ip else "NO_IP",
+                http_method=method,
+                http_path=path,
+                http_version=http_version,
+                http_status_code=status[0],
+                duration=time.perf_counter() - start_time,
                 **extra,
             )
-            raise e
```

### Comparing `troncos-4.0.0b8/troncos/contrib/asgi/profiling/app.py` & `troncos-4.0.0b9/troncos/contrib/asgi/profiling/app.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b8/troncos/contrib/celery/logging/signals.py` & `troncos-4.0.0b9/troncos/contrib/celery/logging/signals.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,8 +28,8 @@
     started_time = getattr(task, "__troncos_start_time", None)
 
     extra = {}
 
     if started_time:
         extra["duration"] = time.perf_counter() - started_time
 
-    logger.info("", task=task.name, state=kwargs["state"], **extra)
+    logger.info("Celery task post-run", task=task.name, state=kwargs["state"], **extra)
```

### Comparing `troncos-4.0.0b8/troncos/contrib/django/logging/middleware.py` & `troncos-4.0.0b9/troncos/contrib/django/logging/middleware.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         *, response: HttpResponse, request_data: dict[str, Any], start_time: float
     ) -> None:
         http_status_code = response.status_code
 
         logger_method = access.info if http_status_code < 500 else error.error
 
         logger_method(
-            "",
+            "Django HTTP response",
             http_status_code=http_status_code,
             duration=time.perf_counter() - start_time,
             **request_data,
         )
 
     if iscoroutinefunction(get_response):
```

### Comparing `troncos-4.0.0b8/troncos/contrib/structlog/__init__.py` & `troncos-4.0.0b9/troncos/contrib/structlog/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import logging
 import logging.config
 
 import structlog
 
-from troncos.contrib.structlog.processors import trace_injection_processor
+from troncos.contrib.structlog.processors import (
+    LogfmtRenderer,
+    trace_injection_processor,
+)
 
 try:
     from structlog_sentry import SentryProcessor
 except ImportError:
     SentryProcessor = None
 
 shared_processors: list[structlog.types.Processor] = [
@@ -45,14 +48,16 @@
 
     processor: structlog.types.Processor
 
     if format == "text":
         processor = structlog.dev.ConsoleRenderer(colors=True)
     elif format == "json":
         processor = structlog.processors.JSONRenderer()
+    elif format == "logfmt":
+        processor = LogfmtRenderer()
     else:
         raise RuntimeError(f"Invalid log format {format}")
 
     if configure_logging:
         config = {
             "version": 1,
             "disable_existing_loggers": True,
```

### Comparing `troncos-4.0.0b8/troncos/contrib/structlog/processors.py` & `troncos-4.0.0b9/troncos/contrib/structlog/processors.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 from ddtrace import tracer
+from structlog.processors import LogfmtRenderer as LogFmt
 from structlog.types import EventDict, WrappedLogger
 
 
 def trace_injection_processor(
     _logger: WrappedLogger, _log_method: str, event_dict: EventDict
 ) -> EventDict:
     """
     Simple logging processor that adds a trace_id to the log record if available.
     """
 
-    # Try to get context from log record
-    dd_context = event_dict.pop("dd_context", None)
-
     # Try to get context from tracer
-    if not dd_context:
-        dd_context = tracer.current_trace_context()
+    dd_context = tracer.current_trace_context()
 
     # Add context to log record if exists
     if dd_context:
         event_dict["trace_id"] = f"{dd_context.trace_id:x}"
         event_dict["span_id"] = f"{dd_context.span_id:x}"
 
     return event_dict
+
+
+class LogfmtRenderer(LogFmt):
+    """
+    A structlog Logfmt renderer that does not produce new lines
+    """
+
+    def __call__(self, _: WrappedLogger, __: str, event_dict: EventDict) -> str:
+        return super().__call__(_, __, event_dict).replace("\n", " ")
```

### Comparing `troncos-4.0.0b8/troncos/profiling/profiler.py` & `troncos-4.0.0b9/troncos/profiling/profiler.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b8/troncos/tracing/__init__.py` & `troncos-4.0.0b9/troncos/tracing/__init__.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b8/troncos/tracing/_otel.py` & `troncos-4.0.0b9/troncos/tracing/_otel.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b8/troncos/tracing/_span.py` & `troncos-4.0.0b9/troncos/tracing/_span.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b8/troncos/tracing/_writer.py` & `troncos-4.0.0b9/troncos/tracing/_writer.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b8/PKG-INFO` & `troncos-4.0.0b9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: troncos
-Version: 4.0.0b8
+Version: 4.0.0b9
 Summary: Collection of Python logging, tracing and profiling tools
 Home-page: https://github.com/kolonialno/troncos
 License: MIT
 Keywords: logs,traces,opentelemetry
 Author: Guðmundur Björn Birkisson
 Author-email: gudmundur.birkisson@oda.com
 Requires-Python: >=3.10,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: troncos Version: 4.0.0b8 Summary: Collection of
+Metadata-Version: 2.1 Name: troncos Version: 4.0.0b9 Summary: Collection of
 Python logging, tracing and profiling tools Home-page: https://github.com/
 kolonialno/troncos License: MIT Keywords: logs,traces,opentelemetry Author:
 GuÃ°mundur BjÃ¶rn Birkisson Author-email: gudmundur.birkisson@oda.com Requires-
 Python: >=3.10,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: grpc Requires-Dist: ddtrace (==1.13.3) Requires-Dist:
```

