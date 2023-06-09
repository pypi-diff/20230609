# Comparing `tmp/hello_jupyter_proxy-0.1.tar.gz` & `tmp/hello_jupyter_proxy-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hello_jupyter_proxy-0.1.tar", last modified: Mon Feb 14 13:40:59 2022, max compression
+gzip compressed data, was "hello_jupyter_proxy-0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `hello_jupyter_proxy-0.1.tar` & `hello_jupyter_proxy-0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        7 2022-02-14 11:05:15.721639 hello_jupyter_proxy-0.1/.gitignore
--rw-r--r--   0        0        0     1081 2022-02-14 10:59:03.642550 hello_jupyter_proxy-0.1/LICENSE
--rw-r--r--   0        0        0     2042 2022-02-14 12:14:30.463705 hello_jupyter_proxy-0.1/README.rst
--rw-r--r--   0        0        0     1971 2022-02-14 12:09:23.232504 hello_jupyter_proxy-0.1/hello_jupyter_proxy.py
--rw-r--r--   0        0        0      549 2022-02-14 12:13:49.333540 hello_jupyter_proxy-0.1/pyproject.toml
--rw-r--r--   0        0        0     2416 1970-01-01 00:00:00.000000 hello_jupyter_proxy-0.1/PKG-INFO
+-rw-r--r--   0        0        0        7 2022-02-14 11:05:15.721639 hello_jupyter_proxy-0.2/.gitignore
+-rw-r--r--   0        0        0     1081 2022-02-14 10:59:03.642550 hello_jupyter_proxy-0.2/LICENSE
+-rw-r--r--   0        0        0     2042 2022-02-14 12:14:30.463705 hello_jupyter_proxy-0.2/README.rst
+-rw-r--r--   0        0        0     3308 2023-06-09 09:58:16.022316 hello_jupyter_proxy-0.2/hello_jupyter_proxy.py
+-rw-r--r--   0        0        0      594 2023-06-08 16:17:48.195332 hello_jupyter_proxy-0.2/pyproject.toml
+-rw-r--r--   0        0        0     2422 1970-01-01 00:00:00.000000 hello_jupyter_proxy-0.2/PKG-INFO
```

### Comparing `hello_jupyter_proxy-0.1/LICENSE` & `hello_jupyter_proxy-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hello_jupyter_proxy-0.1/README.rst` & `hello_jupyter_proxy-0.2/README.rst`

 * *Files identical despite different names*

### Comparing `hello_jupyter_proxy-0.1/hello_jupyter_proxy.py` & `hello_jupyter_proxy-0.2/hello_jupyter_proxy.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,56 @@
 """A minimal example server to run with jupyter-server-proxy
 """
 import argparse
+import socket
 import sys
 from copy import copy
+from pathlib import Path
 from http.server import BaseHTTPRequestHandler, HTTPServer
 
-__version__ = '0.1'
+__version__ = '0.2'
 
 # This is the entry point for jupyter-server-proxy . The packaging metadata
 # tells it about this function. For details, see:
 # https://jupyter-server-proxy.readthedocs.io/en/latest/server-process.html
 def setup_hello():
+    # Using a Unix socket prevents other users on a multi-user system from accessing
+    # our server. The alternative is a TCP socket ('-p', '{port}').
     return {
-        'command': [sys.executable, '-m', 'hello_jupyter_proxy', '{port}']
+        'command': [sys.executable, '-m', 'hello_jupyter_proxy', '-u', '{unix_socket}'],
+        'unix_socket': True,
     }
 
 # Define a web application to proxy.
 # You would normally do this with a web framework like tornado or Flask, or run
 # something else outside of Python.
 # This example uses Python's low-level http.server, to minimise dependencies.
 class RequestHandler(BaseHTTPRequestHandler):
     def do_GET(self):
-        self.send_response(200)
-        self.end_headers()
-        self.wfile.write(TEMPLATE.format(
-            path=self.path, headers=self._headers_hide_cookie()
-        ).encode('utf-8'))
+        server_addr = self.server.server_address
+        if isinstance(server_addr, tuple):
+            server_addr = "{}:{}".format(*server_addr)
+
+        try:
+            self.send_response(200)
+            self.end_headers()
+            self.wfile.write(TEMPLATE.format(
+                path=self.path, headers=self._headers_hide_cookie(),
+                server_address=server_addr,
+            ).encode('utf-8'))
+        except BrokenPipeError:
+            # Connection closed without the client reading the whole response.
+            # Not a problem for the server.
+            pass
+
+    def address_string(self):
+        # Overridden to fix logging when serving on Unix socket
+        if isinstance(self.client_address, str):
+            return self.client_address  # Unix sock
+        return super().address_string()
 
     def _headers_hide_cookie(self):
         # Not sure if there's any security risk in showing the Cookie value,
         # but better safe than sorry. You can inspect cookie values in the
         # browser.
         res = copy(self.headers)
         if 'Cookie' in self.headers:
@@ -45,23 +66,34 @@
 <title>Hello Jupyter-server-proxy</title>
 </head>
 <body>
 <h1>Hello Jupyter-server-proxy</h1>
 <p>Request path is <code>{path}</code></p>
 <p>Headers:</p>
 <pre>{headers}</pre>
+<p>Server is listening (behind the proxy) on <code>{server_address}</code>.</p>
 </body>
 </html>
 """
 
+class HTTPUnixServer(HTTPServer):
+    address_family = socket.AF_UNIX
+
 def main():
     ap = argparse.ArgumentParser()
-    ap.add_argument('port', type=int)
+    ap.add_argument('-p', '--port')
+    ap.add_argument('-u', '--unix-socket')
     args = ap.parse_args()
 
-    # 127.0.0.1 = localhost: only accept connections from the same machine
-    httpd = HTTPServer(('127.0.0.1', args.port), RequestHandler)
+    if args.unix_socket:
+        print("Unix server at", repr(args.unix_socket))
+        Path(args.unix_socket).unlink(missing_ok=True)
+        httpd = HTTPUnixServer(args.unix_socket, RequestHandler)
+    else:
+        # 127.0.0.1 = localhost: only accept connections from the same machine
+        print("TCP server on port", int(args.port))
+        httpd = HTTPServer(('127.0.0.1', int(args.port)), RequestHandler)
     print("Launching example HTTP server")
     httpd.serve_forever()
 
 if __name__ == '__main__':
     main()
```

### Comparing `hello_jupyter_proxy-0.1/pyproject.toml` & `hello_jupyter_proxy-0.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "hello_jupyter_proxy"
 authors = [{name = "Thomas Kluyver", email = "thomas@kluyver.me.uk"}]
 readme = "README.rst"
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: MIT License"]
-dependencies = ["jupyter-server-proxy"]
+dependencies = ["jupyter-server-proxy >=4.0"]  # v4 required for Unix socket support
 dynamic = ["version", "description"]
 
 [project.urls]
 Home = "https://github.com/takluyver/hello_jupyter_proxy"
 
 [project.entry-points.jupyter_serverproxy_servers]
 hello = "hello_jupyter_proxy:setup_hello"
```

### Comparing `hello_jupyter_proxy-0.1/PKG-INFO` & `hello_jupyter_proxy-0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: hello_jupyter_proxy
-Version: 0.1
+Version: 0.2
 Summary: A minimal example server to run with jupyter-server-proxy
 Author-email: Thomas Kluyver <thomas@kluyver.me.uk>
 Description-Content-Type: text/x-rst
 Classifier: License :: OSI Approved :: MIT License
-Requires-Dist: jupyter-server-proxy
+Requires-Dist: jupyter-server-proxy >=4.0
 Project-URL: Home, https://github.com/takluyver/hello_jupyter_proxy
 
 Jupyter Server Proxy Demo
 =========================
 
 This is a demo package showing how to run a web app through
 `Jupyter Server Proxy <https://jupyter-server-proxy.readthedocs.io/en/latest/>`_.
```

