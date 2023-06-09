# Comparing `tmp/thoughtful-2.0.2.tar.gz` & `tmp/thoughtful-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thoughtful-2.0.2.tar", max compression
+gzip compressed data, was "thoughtful-2.0.3.tar", max compression
```

## Comparing `thoughtful-2.0.2.tar` & `thoughtful-2.0.3.tar`

### file list

```diff
@@ -1,29 +1,31 @@
--rw-r--r--   0        0        0    11358 2023-06-08 16:34:10.616843 thoughtful-2.0.2/LICENSE
--rw-r--r--   0        0        0     2992 2023-06-08 16:34:10.616843 thoughtful-2.0.2/README.md
--rw-r--r--   0        0        0     1935 2023-06-08 16:34:10.620843 thoughtful-2.0.2/pyproject.toml
--rw-r--r--   0        0        0      222 2023-06-08 16:34:10.620843 thoughtful-2.0.2/thoughtful/__init__.py
--rw-r--r--   0        0        0       54 2023-06-08 16:34:10.620843 thoughtful-2.0.2/thoughtful/__version__.py
--rw-r--r--   0        0        0     1070 2023-06-08 16:34:10.620843 thoughtful-2.0.2/thoughtful/environment_variables.py
--rw-r--r--   0        0        0      143 2023-06-08 16:34:10.620843 thoughtful-2.0.2/thoughtful/supervisor/__init__.py
--rw-r--r--   0        0        0     4466 2023-06-08 16:34:10.620843 thoughtful-2.0.2/thoughtful/supervisor/default_instances.py
--rw-r--r--   0        0        0     8580 2023-06-08 16:34:10.620843 thoughtful-2.0.2/thoughtful/supervisor/main_context.py
--rw-r--r--   0        0        0    10567 2023-06-08 16:34:10.620843 thoughtful-2.0.2/thoughtful/supervisor/manifest.py
--rw-r--r--   0        0        0        0 2023-06-08 16:34:10.620843 thoughtful-2.0.2/thoughtful/supervisor/py.typed
--rw-r--r--   0        0        0        0 2023-06-08 16:34:10.620843 thoughtful-2.0.2/thoughtful/supervisor/reporting/__init__.py
--rw-r--r--   0        0        0     2872 2023-06-08 16:34:10.620843 thoughtful-2.0.2/thoughtful/supervisor/reporting/record.py
--rw-r--r--   0        0        0     1189 2023-06-08 16:34:10.620843 thoughtful-2.0.2/thoughtful/supervisor/reporting/record_report.py
--rw-r--r--   0        0        0     2066 2023-06-08 16:34:10.620843 thoughtful-2.0.2/thoughtful/supervisor/reporting/report.py
--rw-r--r--   0        0        0    10118 2023-06-08 16:34:10.620843 thoughtful-2.0.2/thoughtful/supervisor/reporting/report_builder.py
--rw-r--r--   0        0        0      660 2023-06-08 16:34:10.620843 thoughtful-2.0.2/thoughtful/supervisor/reporting/status.py
--rw-r--r--   0        0        0      876 2023-06-08 16:34:10.620843 thoughtful-2.0.2/thoughtful/supervisor/reporting/step_report.py
--rw-r--r--   0        0        0     1541 2023-06-08 16:34:10.620843 thoughtful-2.0.2/thoughtful/supervisor/reporting/timed_report.py
--rw-r--r--   0        0        0     1754 2023-06-08 16:34:10.620843 thoughtful-2.0.2/thoughtful/supervisor/reporting/timer.py
--rw-r--r--   0        0        0     7609 2023-06-08 16:34:10.620843 thoughtful-2.0.2/thoughtful/supervisor/step_context.py
--rw-r--r--   0        0        0     6531 2023-06-08 16:34:10.620843 thoughtful-2.0.2/thoughtful/supervisor/step_decorator_factory.py
--rw-r--r--   0        0        0        0 2023-06-08 16:34:10.620843 thoughtful-2.0.2/thoughtful/supervisor/streaming/__init__.py
--rw-r--r--   0        0        0      736 2023-06-08 16:34:10.620843 thoughtful-2.0.2/thoughtful/supervisor/streaming/action.py
--rw-r--r--   0        0        0     1347 2023-06-08 16:34:10.620843 thoughtful-2.0.2/thoughtful/supervisor/streaming/jwt_auth.py
--rw-r--r--   0        0        0     4164 2023-06-08 16:34:10.620843 thoughtful-2.0.2/thoughtful/supervisor/streaming/notifier.py
--rw-r--r--   0        0        0     3184 2023-06-08 16:34:10.620843 thoughtful-2.0.2/thoughtful/supervisor/streaming/payloads.py
--rw-r--r--   0        0        0     1352 2023-06-08 16:34:10.620843 thoughtful-2.0.2/thoughtful/supervisor/streaming/token.py
--rw-r--r--   0        0        0     4578 1970-01-01 00:00:00.000000 thoughtful-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-06-09 17:26:45.413957 thoughtful-2.0.3/LICENSE
+-rw-r--r--   0        0        0     2992 2023-06-09 17:26:45.413957 thoughtful-2.0.3/README.md
+-rw-r--r--   0        0        0     1935 2023-06-09 17:26:45.413957 thoughtful-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0      222 2023-06-09 17:26:45.417957 thoughtful-2.0.3/thoughtful/__init__.py
+-rw-r--r--   0        0        0       54 2023-06-09 17:26:45.417957 thoughtful-2.0.3/thoughtful/__version__.py
+-rw-r--r--   0        0        0     1070 2023-06-09 17:26:45.417957 thoughtful-2.0.3/thoughtful/environment_variables.py
+-rw-r--r--   0        0        0      143 2023-06-09 17:26:45.417957 thoughtful-2.0.3/thoughtful/supervisor/__init__.py
+-rw-r--r--   0        0        0     4816 2023-06-09 17:26:45.417957 thoughtful-2.0.3/thoughtful/supervisor/default_instances.py
+-rw-r--r--   0        0        0      922 2023-06-09 17:26:45.417957 thoughtful-2.0.3/thoughtful/supervisor/event_bus.py
+-rw-r--r--   0        0        0     8756 2023-06-09 17:26:45.417957 thoughtful-2.0.3/thoughtful/supervisor/main_context.py
+-rw-r--r--   0        0        0    10567 2023-06-09 17:26:45.417957 thoughtful-2.0.3/thoughtful/supervisor/manifest.py
+-rw-r--r--   0        0        0        0 2023-06-09 17:26:45.417957 thoughtful-2.0.3/thoughtful/supervisor/py.typed
+-rw-r--r--   0        0        0        0 2023-06-09 17:26:45.417957 thoughtful-2.0.3/thoughtful/supervisor/reporting/__init__.py
+-rw-r--r--   0        0        0     2872 2023-06-09 17:26:45.417957 thoughtful-2.0.3/thoughtful/supervisor/reporting/record.py
+-rw-r--r--   0        0        0     1189 2023-06-09 17:26:45.417957 thoughtful-2.0.3/thoughtful/supervisor/reporting/record_report.py
+-rw-r--r--   0        0        0     2066 2023-06-09 17:26:45.417957 thoughtful-2.0.3/thoughtful/supervisor/reporting/report.py
+-rw-r--r--   0        0        0    10118 2023-06-09 17:26:45.417957 thoughtful-2.0.3/thoughtful/supervisor/reporting/report_builder.py
+-rw-r--r--   0        0        0      660 2023-06-09 17:26:45.417957 thoughtful-2.0.3/thoughtful/supervisor/reporting/status.py
+-rw-r--r--   0        0        0      876 2023-06-09 17:26:45.417957 thoughtful-2.0.3/thoughtful/supervisor/reporting/step_report.py
+-rw-r--r--   0        0        0     1541 2023-06-09 17:26:45.417957 thoughtful-2.0.3/thoughtful/supervisor/reporting/timed_report.py
+-rw-r--r--   0        0        0     1754 2023-06-09 17:26:45.417957 thoughtful-2.0.3/thoughtful/supervisor/reporting/timer.py
+-rw-r--r--   0        0        0     7756 2023-06-09 17:26:45.417957 thoughtful-2.0.3/thoughtful/supervisor/step_context.py
+-rw-r--r--   0        0        0     6441 2023-06-09 17:26:45.417957 thoughtful-2.0.3/thoughtful/supervisor/step_decorator_factory.py
+-rw-r--r--   0        0        0        0 2023-06-09 17:26:45.417957 thoughtful-2.0.3/thoughtful/supervisor/streaming/__init__.py
+-rw-r--r--   0        0        0      736 2023-06-09 17:26:45.417957 thoughtful-2.0.3/thoughtful/supervisor/streaming/action.py
+-rw-r--r--   0        0        0     1347 2023-06-09 17:26:45.417957 thoughtful-2.0.3/thoughtful/supervisor/streaming/jwt_auth.py
+-rw-r--r--   0        0        0     4164 2023-06-09 17:26:45.417957 thoughtful-2.0.3/thoughtful/supervisor/streaming/notifier.py
+-rw-r--r--   0        0        0     3124 2023-06-09 17:26:45.417957 thoughtful-2.0.3/thoughtful/supervisor/streaming/payloads.py
+-rw-r--r--   0        0        0     4372 2023-06-09 17:26:45.417957 thoughtful-2.0.3/thoughtful/supervisor/streaming/streamer.py
+-rw-r--r--   0        0        0     1352 2023-06-09 17:26:45.417957 thoughtful-2.0.3/thoughtful/supervisor/streaming/token.py
+-rw-r--r--   0        0        0     4578 1970-01-01 00:00:00.000000 thoughtful-2.0.3/PKG-INFO
```

### Comparing `thoughtful-2.0.2/LICENSE` & `thoughtful-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.2/README.md` & `thoughtful-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.2/pyproject.toml` & `thoughtful-2.0.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "thoughtful"
-version = "2.0.2"
+version = "2.0.3"
 description = "Thoughtful is a python package by Thoughtful for helping manage automations with helpful packages like supervisor"
 authors = ["Thoughtful Automation <care@thoughtful.ai>"]
 license = "Apache-2.0"
 readme = 'README.md'
 homepage = "https://thoughtful.ai"
 repository = "https://github.com/thoughtful-automation/thoughtful"
 documentation = "https://thoughtful-supervisor.readthedocs-hosted.com/en/latest/index.html"
@@ -41,15 +41,15 @@
 mkdocs = "^1.2.3"
 datamodel-code-generator = "^0.11.14"
 mkdocstrings = "^0.21.2"
 pytest = "^7.2.1"
 pytest-cov = "^2.12.1"
 pytest-watch = "^4.2.0"
 pytest-sugar = "^0.9.4"
-pytest-timeout = "^2.0.2"
+pytest-timeout = "^2.0.3"
 syrupy = "^1.5.0"
 yapf = "^0.31.0"
 pylint = "^2.11.1"
 pre-commit = "^2.21.0"
 devtools = "^0.8.0"
 isort = "^5.12.0"
 autoflake = "^1.7.8"
```

### Comparing `thoughtful-2.0.2/thoughtful/environment_variables.py` & `thoughtful-2.0.3/thoughtful/environment_variables.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.2/thoughtful/supervisor/default_instances.py` & `thoughtful-2.0.3/thoughtful/supervisor/default_instances.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,45 +14,33 @@
 """
 
 import logging
 import pathlib
 from typing import Union
 
 from thoughtful.environment_variables import EnvironmentVariables
+from thoughtful.supervisor.event_bus import EventBus
 from thoughtful.supervisor.main_context import MainContext
 from thoughtful.supervisor.manifest import Manifest
 from thoughtful.supervisor.reporting.report_builder import ReportBuilder
 from thoughtful.supervisor.step_context import StepContext
 from thoughtful.supervisor.step_decorator_factory import create_step_decorator
-from thoughtful.supervisor.streaming.notifier import Notifier
+from thoughtful.supervisor.streaming.streamer import Streamer
 
 logger = logging.getLogger(__name__)
 
-# Share a streaming callback variable, but we can't set it until a user
-# provides a JWT token.
-streamer = Notifier.from_encoded_tokens(
-    run_id=EnvironmentVariables().run_id,
-    callback_url=EnvironmentVariables().callback_url,
-    # The JWT token is set by the user later. If steamer is set to None,
-    # then the step decorators can't be updated to stream if streamer is
-    # changed to a new instance.
-    #
-    # See CX-2368 for the proper fix by lifting the streamer out of the contexts
-    access_token="",
-    refresh_token="",
-    refresh_url="",
-)
+shared_bus = EventBus()
 
 #: A shared ``ReportBuilder`` for steps and step contexts to add step reports
 #: to.
 report_builder = ReportBuilder()
 
 #: Use this decorator on your own functions to mark what workflow step each
 #: Python function is matched to.
-step = create_step_decorator(report_builder, streamer)
+step = create_step_decorator(report_builder=report_builder, event_bus=shared_bus)
 
 #: Use this function to mark a step as failed.
 #: This is just a shortcut for ``set_step_status(step_id, "failed")``.
 #: Exposes ``report_builder.fail_step``.
 fail_step = report_builder.fail_step
 
 #: Expose the report builder's ability to override a step's status as a
@@ -80,17 +68,17 @@
         A default `StepContext` that uses the root level `report_builder` and
         `recorder`.
 
         Args:
             *step_id: The list of integers that represent the step ID.
         """
         super().__init__(
-            report_builder,
-            step_id,
-            streaming_callback=streamer,
+            builder=report_builder,
+            step_id=step_id,
+            event_bus=shared_bus,
         )
 
 
 # noinspection PyPep8Naming
 class supervise(MainContext):
     """
     It's a context manager that provides a scope for the main context using the
@@ -116,11 +104,32 @@
                 be written to
         """
         super().__init__(
             report_builder=report_builder,
             manifest=manifest,
             output_dir=output_dir,
             upload_uri=EnvironmentVariables().s3_bucket_uri,
-            streaming_callback=streamer,
+            event_bus=shared_bus,
             *args,
             **kwargs,
         )
+
+
+if __name__ == "__main__":
+    from thoughtful.supervisor.event_bus import RunStatusChangeEvent
+    from thoughtful.supervisor.reporting.status import Status
+
+    _streamer = Streamer.from_encoded_tokens(
+        run_id=EnvironmentVariables().run_id,
+        callback_url=EnvironmentVariables().callback_url,
+        # The JWT token is set by the user later. If steamer is set to None,
+        # then the step decorators can't be updated to stream if streamer is
+        # changed to a new instance.
+        #
+        # See CX-2368 for the proper fix by lifting the streamer out of the contexts
+        access_token="",
+        refresh_token="",
+        refresh_url="",
+    )
+    shared_bus.subscribe(_streamer.handle_event)
+    test = RunStatusChangeEvent(status=Status.RUNNING)
+    shared_bus.emit(test)
```

### Comparing `thoughtful-2.0.2/thoughtful/supervisor/main_context.py` & `thoughtful-2.0.3/thoughtful/supervisor/main_context.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,18 +20,19 @@
 import pathlib
 from types import TracebackType
 from typing import Callable, Optional, Type, Union
 from urllib.parse import urlparse
 
 import boto3
 
+from thoughtful.supervisor.event_bus import ArtifactsUploadedEvent, EventBus
+from thoughtful.supervisor.event_bus import NewManifestEvent, RunStatusChangeEvent
 from thoughtful.supervisor.manifest import Manifest
 from thoughtful.supervisor.reporting.report_builder import ReportBuilder
 from thoughtful.supervisor.reporting.status import Status
-from thoughtful.supervisor.streaming.notifier import Notifier
 
 logger = logging.getLogger(__name__)
 
 
 class MainContext:
     """
     Supervises an entire digital worker run and generates a work report
@@ -61,43 +62,45 @@
     """
 
     def __init__(
         self,
         report_builder: ReportBuilder,
         manifest: Union[Manifest, str, pathlib.Path],
         output_dir: Union[str, pathlib.Path],
+        event_bus: EventBus,
         upload_uri: Optional[str] = None,
         callback: Optional[Callable] = None,
-        streaming_callback: Optional[Notifier] = None,
     ):
         """
         Args:
             report_builder (ReportBuilder): A ReportBuilder object that will
                 receive the step reports and provide the run report.
                 messages and logs throughout the process execution.
             manifest (str, Path): A pathlike object that points to the manifest
                 file for the process.
             output_dir (str, Path): A pathlike object that points to the output
                 directory for the process. This will receive the run report and
                 output manifest.
+            event_bus (EventBus): This instance will send events, such as
+                a new manifest or a change in the run's status, to this bus.
             upload_uri (str, optional): A URI to upload the output files to.
             callback (callable, optional): a function that is invoked with three
                 parameters: the current context (as the `MainContext` instance)
                 and the `Report` generated from this digital worker's run.
         """
         self.report_builder = report_builder
         self.output_path = pathlib.Path(output_dir)
         self.upload_uri = upload_uri
 
         self.manifest_path = (
             manifest if isinstance(manifest, (str, pathlib.Path)) else None
         )
         self.manifest = self._parse_manifest(manifest)
         self.callback = callback
-        self.streaming_callback = streaming_callback
+        self.event_bus = event_bus
 
     @staticmethod
     def _parse_manifest(
         manifest: Union[Manifest, str, pathlib.Path]
     ) -> Optional[Manifest]:
         if isinstance(manifest, Manifest):
             return manifest
@@ -113,16 +116,20 @@
         """
         Logic for when this context is first started. Attempts to load the
         manifest and returns itself as the context.
 
         Returns:
             MainContext: This instance.
         """
-        if self.manifest and self.streaming_callback:
-            self.streaming_callback.post_manifest(self.manifest)
+        if self.manifest:
+            self.event_bus.emit(
+                NewManifestEvent(
+                    manifest=self.manifest,
+                )
+            )
         self._stream_run_status_change(Status.RUNNING)
 
         return self
 
     def set_run_status(self, status: Union[Status, str]) -> None:
         """
         Sets the run status of the process. This is the final status of the
@@ -187,16 +194,15 @@
         # this context sees the exception (if any)
         return False
 
     def _stream_run_status_change(self, status: Status) -> None:
         """
         Post a status change to the stream callback if it exists.
         """
-        if self.streaming_callback:
-            self.streaming_callback.post_status_change(status)
+        self.event_bus.emit(RunStatusChangeEvent(status=status))
 
     def _upload_output_files_to_s3(self, upload_uri: str) -> None:
         """
         It uploads all files in the output directory to S3. It requires the
         environment variable `SUPERVISOR_ARTIFACT_UPLOAD_URI` to be set with
         the S3 URI to upload the files to.
 
@@ -211,17 +217,15 @@
         for file in self.output_path.glob("*"):
             try:
                 if file.is_file():
                     obj = f"{path}/{file.name}" if path else file.name
                     s3_client.upload_file(str(file), bucket, obj)
             except Exception:
                 logger.exception(f"Failed to upload {file} to S3")
-
-        if self.streaming_callback:
-            self.streaming_callback.post_artifacts_uploaded(output_uri=upload_uri)
+        self.event_bus.emit(ArtifactsUploadedEvent(output_uri=upload_uri))
 
     def _safe_report_path(self, file_prefix: str) -> pathlib.Path:
         """
         A ``pathlib.Path`` instance that points to a new work report writable
         location that is safe across all OSes.
 
         Returns:
```

### Comparing `thoughtful-2.0.2/thoughtful/supervisor/manifest.py` & `thoughtful-2.0.3/thoughtful/supervisor/manifest.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.2/thoughtful/supervisor/reporting/record.py` & `thoughtful-2.0.3/thoughtful/supervisor/reporting/record.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.2/thoughtful/supervisor/reporting/record_report.py` & `thoughtful-2.0.3/thoughtful/supervisor/reporting/record_report.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.2/thoughtful/supervisor/reporting/report.py` & `thoughtful-2.0.3/thoughtful/supervisor/reporting/report.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.2/thoughtful/supervisor/reporting/report_builder.py` & `thoughtful-2.0.3/thoughtful/supervisor/reporting/report_builder.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.2/thoughtful/supervisor/reporting/status.py` & `thoughtful-2.0.3/thoughtful/supervisor/reporting/status.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.2/thoughtful/supervisor/reporting/step_report.py` & `thoughtful-2.0.3/thoughtful/supervisor/reporting/step_report.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.2/thoughtful/supervisor/reporting/timed_report.py` & `thoughtful-2.0.3/thoughtful/supervisor/reporting/timed_report.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.2/thoughtful/supervisor/reporting/timer.py` & `thoughtful-2.0.3/thoughtful/supervisor/reporting/timer.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.2/thoughtful/supervisor/step_context.py` & `thoughtful-2.0.3/thoughtful/supervisor/step_context.py`

 * *Files 19% similar despite different names*

```diff
@@ -36,47 +36,46 @@
 """
 
 from __future__ import annotations
 
 from types import TracebackType
 from typing import Optional, Type, Union
 
+from thoughtful.supervisor.event_bus import EventBus, StepReportChangeEvent
 from thoughtful.supervisor.reporting.report_builder import ReportBuilder
 from thoughtful.supervisor.reporting.report_builder import StepReportBuilder
 from thoughtful.supervisor.reporting.status import Status
 from thoughtful.supervisor.reporting.timer import Timer
-from thoughtful.supervisor.streaming.notifier import Notifier
 
 
 class StepContext:
     """
     A context manager for a step that is running inside another step.
     This is an alternative to ``@step`` decorator when you don't want
     to write an entire function for a step.
     """
 
     def __init__(
         self,
         builder: ReportBuilder,
         step_id: Union[str, int],
-        streaming_callback: Optional[Notifier] = None,
+        event_bus: EventBus,
     ):
         """
         Args:
-            builder: Where the step report will be written.
-            *step_id: The step id of this step, ie `"1.1"`
-            streaming_callback (StreamingCallback, optional): If set, streams
-                the status of work report steps to that callback handler.
-                Defaults to `None`.
+            builder (ReportBuilder): Where the step report will be written.
+            step_id (str): The step id of this step, ie `"1.1"`
+            event_bus (EventBus): The decorator will emit events, such as when
+                a step report has been created or updated, to this bus.
         """
         self.step_id = str(step_id)
         self.report_builder = builder
         self.timer = Timer()
         self._status_override: Optional[Status] = None
-        self.streaming_callback = streaming_callback
+        self.event_bus = event_bus
         self.step_report_builder: StepReportBuilder
 
     def __enter__(self):
         """
         Logic for when this context is first started.
 
         Returns:
@@ -85,17 +84,18 @@
         start_time = self.timer.start()
         self.step_report_builder = StepReportBuilder(
             step_id=self.step_id,
             start_time=start_time,
             status=Status.RUNNING,
         )
 
-        if self.streaming_callback:
-            for report in self.step_report_builder.to_reports():
-                self.streaming_callback.post_step_update(report)
+        for report in self.step_report_builder.to_reports():
+            new_event = StepReportChangeEvent(step_report=report)
+            self.event_bus.emit(new_event)
+
         return self
 
     def __exit__(
         self,
         exc_type: Optional[Type[BaseException]],
         exc_val: Optional[BaseException],
         exc_tb: Optional[TracebackType],
@@ -115,18 +115,17 @@
         else:
             step_status = Status.FAILED if exc_type else Status.SUCCEEDED
 
         # Update step report with finished step details
         self.step_report_builder.end_time = timed_info.end
         self.step_report_builder.status = step_status
 
-        # Stream reports if requested
-        if self.streaming_callback:
-            for report in self.step_report_builder.to_reports():
-                self.streaming_callback.post_step_update(report)
+        for report in self.step_report_builder.to_reports():
+            new_event = StepReportChangeEvent(step_report=report)
+            self.event_bus.emit(new_event)
 
         self.report_builder.step_report_builders.append(self.step_report_builder)
 
         # Return False so that any exceptions inside this context
         # are still raised after this function ends
         return False
 
@@ -190,14 +189,17 @@
     ) -> None:
         """
         Override a step context's record to be in the status of ``status``
 
         Args:
             status (str, Status): The status to set the record to
             record_id (str): The ID of the record
+            message (str, optional): A short message to attach to the record
+            metadata (dict, optional): A dictionary of metadata to attach to the
+                record. These should be short, tag-like values.
 
         .. code-block:: python
 
             with step_scope("1.1") as s:
                 ...  # do some stuff
                 s.set_record_status("warning", "record01")
```

### Comparing `thoughtful-2.0.2/thoughtful/supervisor/step_decorator_factory.py` & `thoughtful-2.0.3/thoughtful/supervisor/step_decorator_factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,47 +53,43 @@
     num_list = [1, 2, 3, 4, 5]
     num_list = times_two(num_list)
     set_step_status("1.1", "warning")
 """
 
 from __future__ import annotations
 
-import contextlib
 import functools
-import json
-import logging
 from typing import Any, Callable, Dict, List, Optional, Union
 
+from thoughtful.supervisor.event_bus import EventBus, StepReportChangeEvent
 from thoughtful.supervisor.reporting.report_builder import ReportBuilder
 from thoughtful.supervisor.reporting.report_builder import StepReportBuilder
 from thoughtful.supervisor.reporting.status import Status
 from thoughtful.supervisor.reporting.timer import Timer
-from thoughtful.supervisor.streaming.notifier import Notifier
 
 
 def create_step_decorator(
     report_builder: ReportBuilder,
-    streaming_callback: Optional[Notifier] = None,
+    event_bus: EventBus,
 ) -> Callable:
     """
     A step decorator generator that as input receives a ``ReportBuilder``
     object and a ``Recorder`` object. The returned decorator will use these
     objects to record the execution of the decorated function.
 
     Note that the return type here is `Any`, because proper type hinting
     for decorators is not yet obvious. PEP 612 specifies a way to type
     hint decorators starting in 3.10, but this project supports >= 3.7. See
     more here: https://stackoverflow.com/a/68290080/2597913.
 
     Args:
         report_builder (ReportBuilder): The report builder to use to record
             the execution of the decorated function.
-        streaming_callback (StreamingCallback, optional): If set, streams
-            the status of work report steps to that callback handler.
-            Defaults to `None`.
+        event_bus (EventBus): The decorator will emit events, such as when
+            a step report has been created or updated, to this bus.
 
     Returns:
         Any: A decorator to attach to functions.
     """
 
     # The decorator to be returned as the property
     # This handles the inputs to the decorator itself
@@ -120,15 +116,15 @@
             # args and kwargs arguments
             @functools.wraps(fn)
             def wrapper(*fn_args, **fn_kwargs):
                 return _run_wrapped_func(
                     fn,
                     str(step_id),
                     report_builder,
-                    streaming_callback,
+                    event_bus,
                     *fn_args,
                     **fn_kwargs,
                 )
 
             return wrapper
 
         return inner_decorator
@@ -136,15 +132,15 @@
     return returned_decorator
 
 
 def _run_wrapped_func(
     fn: Callable,
     step_id: str,
     report_builder: ReportBuilder,
-    streaming_callback: Notifier,
+    event_bus: EventBus,
     *fn_args: Optional[Any],
     **fn_kwargs: Optional[Any],
 ) -> Any:
     """
     Runs `fn` with the given args `args` and `kwargs`, times how long it
     takes to run, and records the execution of this function under `step_id`
     in the work report.
@@ -171,17 +167,17 @@
     this_steps_report_builder = StepReportBuilder(
         step_id=step_id,
         start_time=func_timer.start_time,
         end_time=None,
         status=Status.RUNNING,
     )
 
-    if streaming_callback:
-        for report in this_steps_report_builder.to_reports():
-            streaming_callback.post_step_update(report)
+    for report in this_steps_report_builder.to_reports():
+        new_event = StepReportChangeEvent(step_report=report)
+        event_bus.emit(new_event)
 
     """Run the step"""
     try:
         fn_result = fn(*fn_args, **fn_kwargs)
         final_status = Status.SUCCEEDED
     except Exception as ex:
         fn_result = None
@@ -190,17 +186,17 @@
     timer_result = func_timer.end()
 
     # Finish the report
     this_steps_report_builder.end_time = timer_result.end
     this_steps_report_builder.status = final_status
     report_builder.step_report_builders.append(this_steps_report_builder)
 
-    if streaming_callback:
-        for report in this_steps_report_builder.to_reports():
-            streaming_callback.post_step_update(report)
+    for report in this_steps_report_builder.to_reports():
+        new_event = StepReportChangeEvent(step_report=report)
+        event_bus.emit(new_event)
 
     """Passthrough the step's return value or raised exception"""
     # If the step failed and raised an exception, raise that instead
     # of returning None
     if caught_exception:
         raise caught_exception
```

### Comparing `thoughtful-2.0.2/thoughtful/supervisor/streaming/action.py` & `thoughtful-2.0.3/thoughtful/supervisor/streaming/action.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.2/thoughtful/supervisor/streaming/jwt_auth.py` & `thoughtful-2.0.3/thoughtful/supervisor/streaming/jwt_auth.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.2/thoughtful/supervisor/streaming/notifier.py` & `thoughtful-2.0.3/thoughtful/supervisor/streaming/notifier.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.2/thoughtful/supervisor/streaming/payloads.py` & `thoughtful-2.0.3/thoughtful/supervisor/streaming/payloads.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from thoughtful.supervisor.manifest import Manifest
 from thoughtful.supervisor.reporting.status import Status
 from thoughtful.supervisor.reporting.step_report import StepReport
 from thoughtful.supervisor.streaming.action import Action
 
 
 @dataclass
-class StreamingPayload:
+class Payload:
     """
     Base payload format for all streaming messages.
     """
 
     run_id: str
     action: Action
     client: str = "supervisor"
@@ -30,45 +30,45 @@
             "action": self.action.value,
             "payload": {
                 "timestamp": datetime.datetime.now(datetime.timezone.utc).isoformat()
             },
         }
 
 
-class StepReportStreamingPayload(StreamingPayload):
+class StepReportPayload(Payload):
     """
     Payload for sending a step report action.
     """
 
     def __init__(self, step_report: StepReport, run_id: str):
         super().__init__(run_id=run_id, action=Action.STEP_REPORT)
         self.step_report = step_report
 
     def __json__(self) -> dict:
         _json = super().__json__()
         _json["payload"]["step_report"] = self.step_report.__json__()
         return _json
 
 
-class BotManifestStreamingPayload(StreamingPayload):
+class BotManifestPayload(Payload):
     """
     Payload for sending the manifest.
     """
 
     def __init__(self, manifest: Manifest, run_id: str):
         self.manifest = manifest
         super().__init__(run_id=run_id, action=Action.BOT_MANIFEST)
 
     def __json__(self) -> dict:
         _json = super().__json__()
         _json["payload"]["bot_manifest"] = self.manifest.__json__()
         return _json
 
 
-class ArtifactsUploadedPayload(StreamingPayload):
+class ArtifactsUploadedPayload(Payload):
     """
     Payload for notifying the stream consumer that artifacts have been uploaded
     to S3.
     """
 
     def __init__(self, run_id: str, output_artifacts_uri: str):
         self.output_artifacts_uri = output_artifacts_uri
@@ -76,15 +76,15 @@
 
     def __json__(self) -> dict:
         _json = super().__json__()
         _json["payload"]["output_artifacts_uri"] = self.output_artifacts_uri
         return _json
 
 
-class StatusChangePayload(StreamingPayload):
+class RunStatusChangePayload(Payload):
     """
     Payload for notifying the stream consumer that a bot's status has changed
     """
 
     def __init__(self, run_id: str, status: Status):
         self.status = status
         super().__init__(run_id, action=Action.STATUS_CHANGE)
```

### Comparing `thoughtful-2.0.2/thoughtful/supervisor/streaming/token.py` & `thoughtful-2.0.3/thoughtful/supervisor/streaming/token.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.2/PKG-INFO` & `thoughtful-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thoughtful
-Version: 2.0.2
+Version: 2.0.3
 Summary: Thoughtful is a python package by Thoughtful for helping manage automations with helpful packages like supervisor
 Home-page: https://thoughtful.ai
 License: Apache-2.0
 Keywords: rpa,robot-framework,robocorp,automation
 Author: Thoughtful Automation
 Author-email: care@thoughtful.ai
 Requires-Python: >=3.8,<3.12
```

