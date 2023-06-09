# Comparing `tmp/watchserver-0.1.8.tar.gz` & `tmp/watchserver-0.1.9.tar.gz`

## Comparing `watchserver-0.1.8.tar` & `watchserver-0.1.9.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 watchserver-0.1.8/TODO.md
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 watchserver-0.1.8/requirements.txt
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 watchserver-0.1.8/.vscode/settings.json
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 watchserver-0.1.8/playground/test.py
--rw-r--r--   0        0        0     2254 2020-02-02 00:00:00.000000 watchserver-0.1.8/playground/pages/404.html
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 watchserver-0.1.8/playground/pages/index.html
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 watchserver-0.1.8/playground/pages/style.css
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 watchserver-0.1.8/playground/pages/account/index.html
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 watchserver-0.1.8/playground/pages/blog/index.html
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 watchserver-0.1.8/watchserver/__init__.py
--rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 watchserver-0.1.8/watchserver/__main__.py
--rw-r--r--   0        0        0     8775 2020-02-02 00:00:00.000000 watchserver-0.1.8/watchserver/live.py
--rw-r--r--   0        0        0     8896 2020-02-02 00:00:00.000000 watchserver-0.1.8/watchserver/server.py
--rw-r--r--   0        0        0     8729 2020-02-02 00:00:00.000000 watchserver-0.1.8/watchserver/util.py
--rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 watchserver-0.1.8/watchserver/watch.py
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 watchserver-0.1.8/.gitignore
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 watchserver-0.1.8/README.md
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 watchserver-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 watchserver-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 watchserver-0.1.9/Makefile
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 watchserver-0.1.9/TODO.md
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 watchserver-0.1.9/requirements.txt
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 watchserver-0.1.9/.vscode/settings.json
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 watchserver-0.1.9/playground/test.py
+-rw-r--r--   0        0        0     2254 2020-02-02 00:00:00.000000 watchserver-0.1.9/playground/pages/404.html
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 watchserver-0.1.9/playground/pages/index.html
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 watchserver-0.1.9/playground/pages/style.css
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 watchserver-0.1.9/playground/pages/account/index.html
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 watchserver-0.1.9/playground/pages/blog/index.html
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 watchserver-0.1.9/watchserver/__init__.py
+-rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 watchserver-0.1.9/watchserver/__main__.py
+-rw-r--r--   0        0        0     8808 2020-02-02 00:00:00.000000 watchserver-0.1.9/watchserver/live.py
+-rw-r--r--   0        0        0    10312 2020-02-02 00:00:00.000000 watchserver-0.1.9/watchserver/server.py
+-rw-r--r--   0        0        0     8729 2020-02-02 00:00:00.000000 watchserver-0.1.9/watchserver/util.py
+-rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 watchserver-0.1.9/watchserver/watch.py
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 watchserver-0.1.9/.gitignore
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 watchserver-0.1.9/README.md
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 watchserver-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 watchserver-0.1.9/PKG-INFO
```

### Comparing `watchserver-0.1.8/TODO.md` & `watchserver-0.1.9/TODO.md`

 * *Files identical despite different names*

### Comparing `watchserver-0.1.8/playground/pages/404.html` & `watchserver-0.1.9/playground/pages/404.html`

 * *Files identical despite different names*

### Comparing `watchserver-0.1.8/watchserver/__main__.py` & `watchserver-0.1.9/watchserver/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,36 +4,36 @@
 from time import sleep
 import click
 
 from watchserver import __version__, LiveServer
 
 HELP = {
     "root": "path where the server should attach",
-    "base": "base path where the server will find custom error files.",
+    "errors": "path where the server will find custom error files (ex. 404.html).",
     "serve": "port that the server will serve to",
     "watch": "list of paths to watch. Repeat the command for each entry to the list",
     "version": "Version of mophidian",
     "silent": "Surpress all logs from the server and file watcher",
-    "open": "Toggle on auto open. This will automatically open the base url in the browser.",
+    "open": "Toggle on auto open in browser.",
     "ignore": "list of ignore patterns to apply to file watcher. Repeat command for each entry",
 }
 
 
 @click.option("-r", "--root", default="", help=HELP["root"])
-@click.option("-b", "--base", default="", help=HELP["base"])
+@click.option("-e", "--errors", default="", help=HELP["errors"])
 @click.option("-p", "--port", default=3031, help=HELP["serve"])
 @click.option("-w", "--watch", multiple=True, default=[], help=HELP["watch"])
 @click.option("-i", "--ignore", multiple=True, default=[], help=HELP["ignore"])
 @click.option("-v", "--version", flag_value=True, default=False, help=HELP["version"])
 @click.option("-o", "--open", flag_value=True, default=False, help=HELP["open"])
 @click.option("-s", "--silent", flag_value=True, default=False, help=HELP["silent"])
 @click.command(name="serve")
 def serve(
     root: str = "",
-    base: str = "",
+    errors: str = "",
     port: int = 3031,
     watch: list[str] = [],
     ignore: list[str] = [],
     version: bool = False,
     silent: bool = False,
     open: bool = False,
 ):
@@ -46,15 +46,15 @@
         click.echo(f"Livereload v{__version__}")
         exit()
 
     liveserver = LiveServer(
         watch,
         ignore_list=ignore,
         root=root,
-        base=base,
+        errors=errors,
         port=port,
         suppress=silent,
         auto_open="" if open else None
     )
 
     try:
         print(f"Started serving at http://localhost:{port}/")
```

### Comparing `watchserver-0.1.8/watchserver/live.py` & `watchserver-0.1.9/watchserver/live.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,15 +109,15 @@
     """
 
     def __init__(
         self,
         watch: list[str] | None = None,
         ignore_list: list[str] | None = None,
         root: str = "",
-        base: str = "",
+        errors: str = "",
         auto_open: str|None = None,
         host: str = LOCALHOST[0],
         port: int = SERVER_PORT,
         suppress: bool = False,
         live_callback: LiveCallback = LiveCallback(),
     ) -> None:
         self.root = root
@@ -129,15 +129,15 @@
 
         self.server_thread = LiveServerThread(
             self.host,
             self.port,
             daemon=True,
             reloads=self.reloads,
             directory=root,
-            base=base
+            errors=errors
         )
 
         if suppress:
             self.server_thread.suppress()
 
         # Setup function that sends the file_path to a callback and ensures
         # that it either returns a bool or defaults to False
@@ -155,15 +155,15 @@
         )
         self.watchdog = Observer()
 
         # Add recursive watch directories to watchdog
         if watch is not None:
             if len(watch) == 0:
                 if not suppress:
-                    print(f"Watching path {ServerPath(root).posix()!r}")
+                    print(f"Watching path {ServerPath(root).posix()!r}\n")
                 self.watchdog.schedule(
                     event_handler,
                     ServerPath(root).platform(),
                     recursive=True
                 )
             else:
                 if not suppress:
@@ -174,14 +174,15 @@
                         if not suppress:
                             print(f"  - {path!r}")
                         self.watchdog.schedule(
                             event_handler,
                             path.posix(),
                             recursive=True
                         )
+                print()
 
     def suppress(self):
         """Surpress all logs from the server."""
         self.server_thread.suppress()
 
     def logging(self):
         """Enable all logs from the server."""
```

### Comparing `watchserver-0.1.8/watchserver/server.py` & `watchserver-0.1.9/watchserver/server.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 from __future__ import annotations
 
 from http import HTTPStatus
 from http.server import ThreadingHTTPServer, SimpleHTTPRequestHandler
 from typing import Any, BinaryIO
 from queue import Queue
+from traceback import print_exc
 import urllib
+import time
 import io
+import sys
 
 from threading import Thread
 from re import match
 import os
 
 from .util import ServerPath, PORT_RANGE, livereload_script, translate_path, LOCALHOST
 
@@ -24,19 +27,19 @@
     def __init__(
         self,
         host: str = "localhost",
         port=PORT_RANGE[0],
         *args,
         reloads: Queue[ServerPath],
         directory: str = "",
-        base: str = "",
+        errors: str = "",
         **kwargs,
     ):
         super(LiveServerThread, self).__init__(*args, **kwargs)
-        self.server = Server(reloads, directory, base, host=host, port=port)
+        self.server = Server(reloads, directory, errors, host=host, port=port)
 
     def suppress(self):
         """Surpress all logs from the server."""
         self.server.logging = False
 
     def logging(self):
         """Enable all logs from the server."""
@@ -96,23 +99,48 @@
     def no_cache_headers(self):
         self.send_header("Cache-Control", "no-cache, no-store, must-revalidate")
         self.send_header("Pragma", "no-cache")
         self.send_header("Expires", "0")
 
     def log_error(self, format: str, *args: Any) -> None:
         if self.server.logging:
-            return super().log_error(format, *args)
+            print("\x1b[1m[\x1b[31mERROR\x1b[39m]\x1b[0m", " ".join(args))
+            # return super().log_error(format, *args)
 
-    def log_message(self, format: str, *args: Any) -> None:
+    def get_time(self):
+        _, _, _, hh, mm, ss, _, _, _ = time.localtime(time.time())
+        return "%02d:%02d:%02d" % (hh, mm, ss)
+
+    def log_message(self, message: str, *args) -> None:
         if self.server.logging:
-            return super().log_message(format, *args)
+            if len(args) > 0:
+                message = message % args
+
+            sys.stderr.write(f"[{self.get_time()}] {message}\n")
+
+    def format_code(self, code: str|int) -> str:
+        code = int(code)
+        if code >= 100 and code <= 199:
+            return f"\x1b[34m{code}\x1b[39m"
+        if code >= 200 and code <= 299:
+            return f"\x1b[32m{code}\x1b[39m"
+        if code >= 300 and code <= 399:
+            return f"\x1b[35m{code}\x1b[39m"
+        if code >= 400 and code <= 499:
+            return f"\x1b[31m{code}\x1b[39m"
+        if code >= 500 and code <= 599:
+            return f"\x1b[33m{code}\x1b[39m"
+        return str(code)
 
     def log_request(self, code: int | str = "-", size: int | str = "-") -> None:
         if "/livereload/" not in self.requestline and self.server.logging:
-            return super().log_request(code, size)
+            if isinstance(code, HTTPStatus):
+                code = code.value
+            r_type, r_path = self.requestline.split()[:2]
+            self.log_message(f'({self.format_code(code)}) {r_type} {r_path!r}')
 
     def send_head(self, live_reload: str, request_path: str) -> io.BytesIO | BinaryIO | None:
         path = self.translate_path(self.path)
         f = None
         if ServerPath(path).isdir():
             parts = urllib.parse.urlsplit(request_path)
             if not parts.path.endswith('/'):
@@ -164,67 +192,73 @@
 
     def lr_script(self) -> str:
         """Construct the live reload script html element based on the current path."""
         return livereload_script.substitute(path=translate_path(self.server.root, self.path))
 
     def do_GET(self) -> None:
         live_reload = match(r"/?livereload/(?P<path>.*)", self.path)
-        if live_reload is not None:
-            file_path = translate_path(self.server.root, live_reload.group("path"))
-            self.send_response(200)
-            self.end_headers()
+        try:
+            if live_reload is not None:
+                file_path = translate_path(self.server.root, live_reload.group("path"))
+                self.send_response(200)
+                self.end_headers()
 
-            code = 0
-            try:
-                while self.server.reloads.qsize() != 0:
-                    reload = self.server.reloads.get(timeout=5)
-                    if match(f"^{reload.regex()}$", file_path) is not None:
-                        code = 1
-                    self.server.reloads.task_done()
-            except Exception:
-                pass
-            self.wfile.write(bytes(f"{code}", "utf-8"))
-        else:
-            # Same as super().do_GET() except a live reload script is injected
-            request_path = str(self.path)
-            self.path = ServerPath(self.server.root, self.path).posix()
-            live_reload = self.lr_script()
-            file = self.send_head(live_reload, request_path)
-            if file:
-                try: 
-                    if self.path.endswith((".html", ".htm")) or not ServerPath(self.path).lstrip().isfile():
-                        data = file.read() + bytes(live_reload, "utf-8")
-                        self.wfile.write(data)
-                    else:
-                        self.copyfile(file, self.wfile)
-                finally:
-                   file.close()
+                code = 0
+                try:
+                    while self.server.reloads.qsize() != 0:
+                        reload = self.server.reloads.get(timeout=5)
+                        if match(f"^{reload.regex()}$", file_path) is not None:
+                            code = 1
+                        self.server.reloads.task_done()
+                except Exception:
+                    pass
+                self.wfile.write(bytes(f"{code}", "utf-8"))
+            else:
+                # Same as super().do_GET() except a live reload script is injected
+                request_path = str(self.path)
+                self.path = ServerPath(self.server.root, self.path).posix()
+                live_reload = self.lr_script()
+                file = self.send_head(live_reload, request_path)
+                if file:
+                    try:
+                        if (
+                            self.path.endswith((".html", ".htm"))
+                            or not ServerPath(self.path).lstrip().isfile()
+                        ):
+                            data = file.read() + bytes(live_reload, "utf-8")
+                            self.wfile.write(data)
+                        else:
+                            self.copyfile(file, self.wfile)
+                    finally:
+                        file.close()
+        except Exception as exc:
+            print_exc()
+            print("\x1b[1m[\x1b[31mERROR\x1b[39m]\x1b[0m", exc)
 
 
 class Server(ThreadingHTTPServer):
     """Threaded live reload server."""
 
     def __init__(
         self,
         reloads: Queue[ServerPath],
         root: str,
-        base: str,
+        errors: str,
         *,
         host: str = "localhost",
         port=PORT_RANGE[0],
     ):
-
         super().__init__((host, port), ServiceHandler)
         self.host = host
         self.port = port
         self.is_active = False
         self.full_url = f"http://{host}:{port}/"
         self.reloads = reloads
         self.root = root
-        self.epath = base
+        self.epath = errors
         self.logging = True
 
     def serve_forever(self, poll_interval: float = 0.5) -> None:
         self.is_active = True
         return super().serve_forever(poll_interval)
 
     def shutdown(self) -> None:
```

### Comparing `watchserver-0.1.8/watchserver/util.py` & `watchserver-0.1.9/watchserver/util.py`

 * *Files identical despite different names*

### Comparing `watchserver-0.1.8/watchserver/watch.py` & `watchserver-0.1.9/watchserver/watch.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,29 +72,29 @@
         super().__init__()
 
     @debounce(WAIT)
     def on_any_event(self, event: FileSystemEvent):
         pass
 
     @debounce(WAIT)
-    def on_modified(self, event: DirModifiedEvent | FileModifiedEvent):
+    def on_modified(self, event):
         src_path = ServerPath(event.src_path).posix()
         if isinstance(event, FileModifiedEvent) and all(
             match(ignore.regex(), src_path) is None for ignore in self._ignore
         ):
             self._update(src_path)
 
     @debounce(WAIT)
     def on_created(self, event):
         src_path = ServerPath(event.src_path).posix()
-        if isinstance(event, FileModifiedEvent) and all(
+        if isinstance(event, FileCreatedEvent) and all(
             match(ignore.regex(), src_path) is None for ignore in self._ignore
         ):
             self._create(src_path)
 
     @debounce(WAIT)
     def on_deleted(self, event):
         src_path = ServerPath(event.src_path).posix()
-        if isinstance(event, FileModifiedEvent) and all(
+        if isinstance(event, FileDeletedEvent) and all(
             match(ignore.regex(), src_path) is None for ignore in self._ignore
         ):
-            self._update(src_path)
+            self._remove(src_path)
```

### Comparing `watchserver-0.1.8/README.md` & `watchserver-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `watchserver-0.1.8/pyproject.toml` & `watchserver-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "watchserver"
-version = "0.1.8"
+version = "0.1.9"
 authors = [
     { name="Tired Fox", email="zboehm104@gmail.com"}
 ]
 description="Python live reload server"
 readme = "README.md"
 license = "MIT"
 requires-python = ">=3.7"
```

### Comparing `watchserver-0.1.8/PKG-INFO` & `watchserver-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watchserver
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python live reload server
 Project-URL: Homepage, https://github.com/Tired-Fox/watchserver
 Project-URL: Documentation, https://tired-fox.github.io/watchserver
 Author-email: Tired Fox <zboehm104@gmail.com>
 License-Expression: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

