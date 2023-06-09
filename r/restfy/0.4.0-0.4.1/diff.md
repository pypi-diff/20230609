# Comparing `tmp/restfy-0.4.0.tar.gz` & `tmp/restfy-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "restfy-0.4.0.tar", max compression
+gzip compressed data, was "restfy-0.4.1.tar", max compression
```

## Comparing `restfy-0.4.0.tar` & `restfy-0.4.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1071 2023-05-04 09:49:25.883825 restfy-0.4.0/LICENSE
--rw-r--r--   0        0        0     4564 2023-05-31 10:31:39.962791 restfy-0.4.0/README.md
--rw-r--r--   0        0        0      514 2023-05-31 09:32:27.497218 restfy-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      309 2023-05-27 10:05:30.008092 restfy-0.4.0/restfy/__init__.py
--rw-r--r--   0        0        0     5863 2023-05-27 10:08:18.948024 restfy-0.4.0/restfy/application.py
--rw-r--r--   0        0        0        0 2023-05-27 10:08:18.940024 restfy-0.4.0/restfy/cors.py
--rw-r--r--   0        0        0      391 2023-05-04 09:49:25.883825 restfy-0.4.0/restfy/file.py
--rw-r--r--   0        0        0     2098 2023-05-27 10:14:12.191194 restfy-0.4.0/restfy/handler.py
--rw-r--r--   0        0        0     1189 2023-05-31 10:31:39.954791 restfy-0.4.0/restfy/http.py
--rw-r--r--   0        0        0      343 2023-05-27 10:05:30.012091 restfy-0.4.0/restfy/middleware.py
--rw-r--r--   0        0        0     4176 2023-05-27 11:38:52.551360 restfy-0.4.0/restfy/request.py
--rw-r--r--   0        0        0     3025 2023-05-23 11:15:26.608705 restfy-0.4.0/restfy/response.py
--rw-r--r--   0        0        0     5316 2023-05-27 10:05:30.004091 restfy-0.4.0/restfy/router.py
--rw-r--r--   0        0        0     1036 2023-05-27 10:35:29.074926 restfy-0.4.0/restfy/server.py
--rw-r--r--   0        0        0     1970 2023-05-24 11:35:36.204879 restfy-0.4.0/restfy/testing.py
--rw-r--r--   0        0        0      724 2023-05-04 09:49:25.883825 restfy-0.4.0/restfy/websocket.py
--rw-r--r--   0        0        0     5181 1970-01-01 00:00:00.000000 restfy-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-04 09:49:25.883825 restfy-0.4.1/LICENSE
+-rw-r--r--   0        0        0     7102 2023-06-06 11:13:09.887273 restfy-0.4.1/README.md
+-rw-r--r--   0        0        0      514 2023-06-02 11:10:42.205352 restfy-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      309 2023-05-27 10:05:30.008092 restfy-0.4.1/restfy/__init__.py
+-rw-r--r--   0        0        0     6108 2023-06-06 10:51:17.712068 restfy-0.4.1/restfy/application.py
+-rw-r--r--   0        0        0        0 2023-05-27 10:08:18.940024 restfy-0.4.1/restfy/cors.py
+-rw-r--r--   0        0        0      391 2023-05-04 09:49:25.883825 restfy-0.4.1/restfy/file.py
+-rw-r--r--   0        0        0     2097 2023-06-07 10:55:51.640929 restfy-0.4.1/restfy/handler.py
+-rw-r--r--   0        0        0     1350 2023-06-04 10:04:17.432950 restfy-0.4.1/restfy/http.py
+-rw-r--r--   0        0        0      390 2023-06-06 10:39:48.788325 restfy-0.4.1/restfy/middleware.py
+-rw-r--r--   0        0        0     4496 2023-06-03 10:25:18.890505 restfy-0.4.1/restfy/request.py
+-rw-r--r--   0        0        0     3043 2023-06-03 11:12:59.606686 restfy-0.4.1/restfy/response.py
+-rw-r--r--   0        0        0     5932 2023-06-07 17:55:57.915395 restfy-0.4.1/restfy/router.py
+-rw-r--r--   0        0        0     1036 2023-05-27 10:35:29.074926 restfy-0.4.1/restfy/server.py
+-rw-r--r--   0        0        0     2597 2023-06-03 09:55:26.663987 restfy-0.4.1/restfy/testing.py
+-rw-r--r--   0        0        0      724 2023-05-04 09:49:25.883825 restfy-0.4.1/restfy/websocket.py
+-rw-r--r--   0        0        0     7719 1970-01-01 00:00:00.000000 restfy-0.4.1/PKG-INFO
```

### Comparing `restfy-0.4.0/LICENSE` & `restfy-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `restfy-0.4.0/pyproject.toml` & `restfy-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "restfy"
-version = "0.4.0"
+version = "0.4.1"
 description = "A small rest framework"
 authors = ["Manasses Lima <manasseslima@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/manasseslima/restfy"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-bike = "^0.3.1"
+bike = "^0.3.2"
 httplus = "^0.1.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest-asyncio = "^0.21.0"
 pytest = "^7.3.1"
 mkdocs-material = "^9.1.14"
```

### Comparing `restfy-0.4.0/restfy/application.py` & `restfy-0.4.1/restfy/application.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,19 @@
 
     def add_route(self, path, handle, method='GET'):
         self.router.add_route(path, handle, method)
 
     def register_router(self, path, router):
         self.router.register_router(path, router)
 
-    async def handler(self, reader: asyncio.streams.StreamReader, writer: asyncio.streams.StreamWriter):
+    async def handler(
+            self,
+            reader: asyncio.streams.StreamReader,
+            writer: asyncio.streams.StreamWriter
+    ):
         start = datetime.datetime.now()
         ini = time.time()
         data = await reader.readline()
         (method, url, version) = data.decode().replace('\n', '').split(' ')
         request = self.generate_request(url=url, method=method, version=version)
         try:
             while True:
@@ -43,60 +47,65 @@
                 header = line.decode()
                 if header == '\r\n':
                     break
                 header = header.replace('\r\n', '')
                 splt = header.split(':', maxsplit=1)
                 request.add_header(key=splt[0].strip(), value=splt[1].strip())
             if request.length:
-                size = request.length
+                length = request.length
+                size = length if length <= 1000 else 1000
                 content = b''
                 while True:
                     content += await reader.read(size)
-                    size = request.length - len(content)
-                    if size == 0:
+                    length -= size
+                    if length == 0:
                         break
+                    size = length if length <= 1000 else 1000
                 request.body = content
             if request.preflight:
                 response = Response(status=204)
                 response.headers.update(self.cors.get_response_headers())
             else:
                 response = await self.execute_handler(request=request)
         except Exception as e:
             response = Response({'message': 'Internal Server Error', 'detail': str(e)}, status=500)
         block = response.render()
         writer.write(block)
         await writer.drain()
         writer.close()
+        await writer.wait_closed()
         diff = time.time() - ini
         self.print_request(start, method, url, response, diff)
 
-    async def execute_handler(self, request):
+    async def execute_handler(self, request: Request):
         if route := self.router.match(request.url, request.method):
             response = await self.execute_middlewares(route, request)
             if request.origin:
                 response.headers.update(self.cors.get_response_headers())
             if route.is_websocket:
                 prepare_websocket(request=request, response=response)
         else:
             response = Response(status=404)
         return response
 
-    def generate_request(self, url: str, method: str, version: str):
+    def generate_request(
+            self,
+            url: str,
+            method: str,
+            version: str
+    ) -> Request:
         request = Request(method=method, version=version)
         request.app = self
-        if '?' in url:
-            (path, query) = url.split('?')
-        else:
-            path = url
-            query = ''
-        args = self.extract_arguments(query=query)
+        splt = url.split('?')
+        path, query = splt[0], splt[1] if len(splt) > 1 else ''
         request.url = path
         request.query = query
-        request.args = args
+        args = self.extract_arguments(query=query)
         request.query_args = args
+        request.params = {**args}
         return request
 
     def extract_arguments(self, query):
         ret = {}
         if query:
             pairs = query.split('&')
             for pair in pairs:
@@ -112,15 +121,15 @@
         if self.middlewares:
             self.middlewares[-1].next = route
             response = await self.middlewares[0].exec(request)
         else:
             response = await route.exec(request)
         return response
 
-    def register_middleware(self, middleware):
+    def register_middleware(self, middleware: type[Middleware]):
         instance = middleware()
         if self.middlewares:
             self.middlewares[-1].next = instance
         self.middlewares.append(instance)
 
     def get(self, path):
         return self.router.get(path)
```

### Comparing `restfy-0.4.0/restfy/handler.py` & `restfy-0.4.1/restfy/handler.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from .response import Response
 
 
 class Handler:
     def __init__(self, func: callable):
         self.func: callable = func
         self.func_name: str = func.__name__
+        self.variable_name: str = ''
         self.parameters: dict = {}
         self.request_parameter: str = ''
         self.payload_parameter: str = ''
         self.payload_model = None
         self.return_type: type | None = None
         params = func.__annotations__
         for name, param in params.items():
@@ -20,32 +21,30 @@
                 self.payload_parameter = name
                 self.payload_model = param
             elif name == 'return':
                 self.return_type = param
             else:
                 self.parameters[name] = param
 
-    async def execute(self, properties, request):
+    async def execute(self, request: Request):
         args = {}
         for key, kind in self.parameters.items():
-            value = properties.get(key)
-            if not value:
-                value = request.args.pop(key, '')
+            value = request.vars.pop(key, None) or request.params.pop(key, None)
             if not value:
                 continue
             if kind in [int, float, bool]:
                 try:
                     value = kind(value)
                 except Exception as e:
                     raise Exception(f'Error try cast value "{value}" {key} {kind}: {e}')
             args[key] = value
         if self.request_parameter:
             args[self.request_parameter] = request
         if self.payload_parameter:
-            instance = self.payload_model(**request.body)
+            instance = self.payload_model(**request.data)
             args[self.payload_parameter] = instance
         try:
             ret = await self.func(**args)
             if isinstance(ret, tuple):
                 ret = Response(ret[0], ret[1])
             elif isinstance(ret, (dict, list, str, int, float, bool)):
                 ret = Response(ret)
```

### Comparing `restfy-0.4.0/restfy/request.py` & `restfy-0.4.1/restfy/request.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 import json
+import mimetypes
 from restfy.file import File
 
 
+mime_types = {
+    'multipart/form-data': 'form-data',
+    'application/x-www-form-urlencoded': 'x-www-form-urlencoded',
+    **{v: k[1:] for k, v in mimetypes.types_map.items()},
+}
+
+
 class AccessControl:
     allow_origin = '*'
     expose_headers = []
     max_age = 0.0
     allow_credentials = False
     allow_methods = []
     allow_headers = []
@@ -44,57 +52,62 @@
         self.request_method = ''
         self.request_headers = ''
         self.preflight = False
         self.multipart = False
         self.boundary = ''
         self.data = {}
         self.query_args: dict = {}
+        self.params: dict = {}
         self.path_args: dict = {}
+        self.vars: dict = {}
 
     def add_header(self, key, value):
         self.headers[key] = value
         if key == 'Content-Type':
             if 'multipart/form-data' in value:
                 self.multipart = True
                 (content, boundary) = value.split(';')
                 self.type = content.strip()
                 self.boundary = boundary.replace('boundary=', '').strip()
             else:
-                self.type = value
+                self.type = mime_types.get(value, 'plain')
         elif key == 'Content-Length':
             self.length = int(value)
         elif key == 'Origin':
             self.origin = value
             self.preflight = True if self.method == 'OPTIONS' else False
         elif key == 'Access-Control-Request-Method':
             self.request_method = value
         elif key == 'Access-Control-Request-Headers':
             self.request_headers = value
 
     def dict(self):
+        return self.decode_data()
+
+    def decode_data(self):
         if self.body:
-            if self.type == 'application/json':
+            if self.type == 'json':
                 return json.loads(self.body)
-            elif self.type == 'multipart/form-data':
+            elif self.type == 'form-data':
                 return self._process_form_data()
-            elif self.type == 'application/x-www-form-urlencoded':
+            elif self.type == 'x-www-form-urlencoded':
                 return self._url_decoded_data()
         return {}
 
     def args(self):
         args = {}
         if self.query:
             pairs = self.query.split('&')
             for pair in pairs:
                 (key, value) = pair.split('=')
                 args[key] = value
         return args
 
     def prepare_data(self):
-        self.data = self.dict()
+        self.data = self.decode_data()
 
     def _process_form_data(self):
         data = {}
         parts = self.body.split(f'--{self.boundary}'.encode())
         for part in parts:
             if not part or part == b'--\r\n':
                 continue
```

### Comparing `restfy-0.4.0/restfy/response.py` & `restfy-0.4.1/restfy/response.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,37 +45,37 @@
         return o
 
 
 class Response:
     def __init__(
             self,
             data: Any = None,
-            *,
             status: int = 200,
+            *,
             content_type: str = '',
             headers: dict = None
     ):
         self.version = 'HTTP/1.1'
         self.status = status
         self.data = data if status != 204 else None
         self.headers = {}
         self.content_type = content_type
         self._prepare_headers(headers)
         self.content = b''
         self.text = ''
 
-    def render(self):
+    def render(self) -> bytes:
         title = status_title.get(self.status, 'STATUS WITHOUT TITLE')
         headers = '\r\n'.join([f"{k}:{v}" for k, v in self.headers.items()])
         body = self.data
         content = f'{self.version} {self.status} {title}\r\n{headers}\r\n\r\n'
         if body:
             content = f'{content}{body}'
             self.content = body.encode()
-        return content
+        return content.encode()
 
     def parser(self, model: Any = None):
         res = json.loads(self.data)
         if model:
             res = model(**res)
         return res
```

### Comparing `restfy-0.4.0/restfy/router.py` & `restfy-0.4.1/restfy/router.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,45 +14,52 @@
         self.prepare_data: bool = prepare_data
         self.is_websocket = websocket
 
     def __repr__(self):
         return f'{self.__class__}: {self.name}'
 
     def add_node(self, path, handle, method='GET', websocket=False):
+        handler = Handler(handle)
         node = path.pop(0)
         if websocket:
             method = 'GET'
         if node.startswith('{'):
+            name = node[1:-1]
             if self.variable:
+                handler.variable_name = name
                 route = self.variable
             else:
                 route = Route(websocket=websocket)
                 route.is_variable = True
-                route.name = node[1:-1]
+                route.name = name
                 self.variable = route
         else:
             route = self.routes.get(node, Route(websocket=websocket))
             route.name = node
             self.routes[node] = route
         if path:
             route.add_node(path=path, handle=handle, method=method, websocket=websocket)
         else:
-            route.add_handler(handle, method)
+            # handlers = route.handlers if route.is_variable else self.handlers
+            route.handlers[method] = handler
+            # handlers[method] = handler
+            ...
 
     def add_handler(self, func, method: str):
         handler = Handler(func)
         self.handlers[method] = handler
 
     async def exec(self, request: Request):
         handler = self.handlers[request.method]
         if self.prepare_data and request.app.prepare_request_data:
             request.prepare_data()
         for key, value in self.properties.items():
             request.path_args[key] = value
-        return await handler.execute(self.properties, request)
+            request.vars[key] = value
+        return await handler.execute(request)
 
 
 class Router(Route):
     def __init__(self, base_url=''):
         super().__init__()
         self.base_url = base_url
 
@@ -80,14 +87,23 @@
         else:
             routes = self.routes
             while True:
                 node = nodes.pop(0)
                 if len(nodes) == 0:
                     routes[node] = router
                     break
+                elif node.startswith('{'):
+                    if self.variable:
+                        route = self.variable
+                    else:
+                        route = Route()
+                        route.is_variable = True
+                        route.name = node[1:-1]
+                        self.variable = route
+                        routes = route.routes
                 else:
                     if node in routes:
                         if routes[node].routes:
                             routes = routes[node].routes
                         else:
                             routes = routes[node].variable
                     else:
@@ -107,17 +123,16 @@
             route = routes.get(node, None)
             if not route:
                 if variable:
                     route = variable
                     args[route.name] = node
                 else:
                     break
-            else:
-                routes = route.routes
-                variable = route.variable
+            routes = route.routes
+            variable = route.variable
         if route:
             if method in route.handlers:
                 route.properties = args
             else:
                 route = None
         return route
```

### Comparing `restfy-0.4.0/restfy/server.py` & `restfy-0.4.1/restfy/server.py`

 * *Files identical despite different names*

### Comparing `restfy-0.4.0/restfy/testing.py` & `restfy-0.4.1/restfy/testing.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,37 @@
-from .application import Application, Response, Request
+import json
+from .application import Application, Response
 
 
 class Client:
     def __init__(self, app: Application):
         self.app = app
 
     async def request(
             self,
             method: str,
             url: str,
             data: ... = None,
             headers: dict = None
     ) -> Response:
-        req = Request(method=method)
-        req.url = url
-        req.app = self.app
-        req.headers = headers or {}
-        req.body = data or b''
+        headers = headers or {}
+        req = self.app.generate_request(url=url, method=method, version='http/1.1')
+        for k, v in headers.items():
+            req.add_header(k, v)
+        content_type = req.headers.get('Content-Type', '')
+        if not content_type:
+            if isinstance(data, bytes):
+                raise Exception(f'A content type need to be set on headers')
+            req.body = json.dumps(data).encode()
+            req.add_header('Content-Type', 'application/json')
+            req.add_header('Content-Length', len(req.body))
+        else:
+            if content_type == 'application/json' and not isinstance(data, bytes):
+                req.body = json.dumps(data).encode()
+                req.add_header('Content-Length', len(req.body))
         res = await self.app.execute_handler(req)
         res.render()
         return res
 
     async def get(
             self,
             url: str,
```

### Comparing `restfy-0.4.0/restfy/websocket.py` & `restfy-0.4.1/restfy/websocket.py`

 * *Files identical despite different names*

