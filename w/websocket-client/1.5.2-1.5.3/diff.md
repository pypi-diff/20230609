# Comparing `tmp/websocket-client-1.5.2.tar.gz` & `tmp/websocket-client-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "websocket-client-1.5.2.tar", last modified: Sun May 21 19:29:25 2023, max compression
+gzip compressed data, was "websocket-client-1.5.3.tar", last modified: Fri Jun  9 09:33:59 2023, max compression
```

## Comparing `websocket-client-1.5.2.tar` & `websocket-client-1.5.3.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxr-x   0 drift3r   (1000) drift3r   (1000)        0 2023-05-21 19:29:25.776701 websocket-client-1.5.2/
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)    17075 2023-05-21 19:26:03.000000 websocket-client-1.5.2/ChangeLog
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)    11339 2023-02-04 17:51:20.000000 websocket-client-1.5.2/LICENSE
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)       81 2023-02-04 17:51:20.000000 websocket-client-1.5.2/MANIFEST.in
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     7350 2023-05-21 19:29:25.776701 websocket-client-1.5.2/PKG-INFO
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     5997 2023-02-04 17:51:20.000000 websocket-client-1.5.2/README.md
-drwxrwxr-x   0 drift3r   (1000) drift3r   (1000)        0 2023-05-21 19:29:25.772701 websocket-client-1.5.2/examples/
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)      344 2023-02-04 17:51:20.000000 websocket-client-1.5.2/examples/echo_client.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     1009 2023-02-04 17:51:20.000000 websocket-client-1.5.2/examples/echoapp_client.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)      351 2023-02-04 17:51:20.000000 websocket-client-1.5.2/examples/rel_client.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)       59 2023-05-21 19:29:25.776701 websocket-client-1.5.2/setup.cfg
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     2641 2023-05-21 19:21:24.000000 websocket-client-1.5.2/setup.py
-drwxrwxr-x   0 drift3r   (1000) drift3r   (1000)        0 2023-05-21 19:29:25.776701 websocket-client-1.5.2/websocket/
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)      801 2023-05-21 19:21:14.000000 websocket-client-1.5.2/websocket/__init__.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)    13619 2023-05-21 19:20:24.000000 websocket-client-1.5.2/websocket/_abnf.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)    20185 2023-05-21 19:20:24.000000 websocket-client-1.5.2/websocket/_app.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     2164 2023-05-21 19:20:24.000000 websocket-client-1.5.2/websocket/_cookiejar.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)    19872 2023-04-07 22:45:05.000000 websocket-client-1.5.2/websocket/_core.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     2106 2023-04-07 22:59:49.000000 websocket-client-1.5.2/websocket/_exceptions.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     6515 2023-04-07 22:48:16.000000 websocket-client-1.5.2/websocket/_handshake.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)    11806 2023-04-07 22:47:13.000000 websocket-client-1.5.2/websocket/_http.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     2220 2023-05-21 19:20:24.000000 websocket-client-1.5.2/websocket/_logging.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     4979 2023-05-21 19:20:24.000000 websocket-client-1.5.2/websocket/_socket.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     1122 2023-02-04 17:51:20.000000 websocket-client-1.5.2/websocket/_ssl_compat.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     4932 2023-05-21 19:20:24.000000 websocket-client-1.5.2/websocket/_url.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     3636 2023-05-21 19:20:24.000000 websocket-client-1.5.2/websocket/_utils.py
--rwxrwxr-x   0 drift3r   (1000) drift3r   (1000)     7120 2023-05-21 19:20:24.000000 websocket-client-1.5.2/websocket/_wsdump.py
-drwxrwxr-x   0 drift3r   (1000) drift3r   (1000)        0 2023-05-21 19:29:25.776701 websocket-client-1.5.2/websocket/tests/
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)        0 2023-02-04 17:51:20.000000 websocket-client-1.5.2/websocket/tests/__init__.py
-drwxrwxr-x   0 drift3r   (1000) drift3r   (1000)        0 2023-05-21 19:29:25.776701 websocket-client-1.5.2/websocket/tests/data/
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)      163 2023-02-04 17:51:20.000000 websocket-client-1.5.2/websocket/tests/data/header01.txt
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)      161 2023-02-04 17:51:20.000000 websocket-client-1.5.2/websocket/tests/data/header02.txt
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)      216 2023-02-04 17:51:20.000000 websocket-client-1.5.2/websocket/tests/data/header03.txt
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)      486 2023-05-21 19:20:24.000000 websocket-client-1.5.2/websocket/tests/echo-server.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     4175 2023-02-04 17:51:20.000000 websocket-client-1.5.2/websocket/tests/test_abnf.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)    12669 2023-02-04 17:51:20.000000 websocket-client-1.5.2/websocket/tests/test_app.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     4325 2023-02-04 17:51:20.000000 websocket-client-1.5.2/websocket/tests/test_cookiejar.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     9623 2023-02-04 17:51:20.000000 websocket-client-1.5.2/websocket/tests/test_http.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)    14589 2023-02-04 17:51:20.000000 websocket-client-1.5.2/websocket/tests/test_url.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)    18072 2023-02-04 17:51:20.000000 websocket-client-1.5.2/websocket/tests/test_websocket.py
-drwxrwxr-x   0 drift3r   (1000) drift3r   (1000)        0 2023-05-21 19:29:25.776701 websocket-client-1.5.2/websocket_client.egg-info/
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     7350 2023-05-21 19:29:25.000000 websocket-client-1.5.2/websocket_client.egg-info/PKG-INFO
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     1014 2023-05-21 19:29:25.000000 websocket-client-1.5.2/websocket_client.egg-info/SOURCES.txt
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)        1 2023-05-21 19:29:25.000000 websocket-client-1.5.2/websocket_client.egg-info/dependency_links.txt
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)       50 2023-05-21 19:29:25.000000 websocket-client-1.5.2/websocket_client.egg-info/entry_points.txt
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)       94 2023-05-21 19:29:25.000000 websocket-client-1.5.2/websocket_client.egg-info/requires.txt
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)       10 2023-05-21 19:29:25.000000 websocket-client-1.5.2/websocket_client.egg-info/top_level.txt
+drwxrwxr-x   0 drift3r   (1000) drift3r   (1000)        0 2023-06-09 09:33:59.804877 websocket-client-1.5.3/
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)    17264 2023-06-09 09:23:06.000000 websocket-client-1.5.3/ChangeLog
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)    11339 2023-02-04 17:51:20.000000 websocket-client-1.5.3/LICENSE
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)       81 2023-02-04 17:51:20.000000 websocket-client-1.5.3/MANIFEST.in
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     7350 2023-06-09 09:33:59.804877 websocket-client-1.5.3/PKG-INFO
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     5997 2023-02-04 17:51:20.000000 websocket-client-1.5.3/README.md
+drwxrwxr-x   0 drift3r   (1000) drift3r   (1000)        0 2023-06-09 09:33:59.796877 websocket-client-1.5.3/examples/
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)      344 2023-02-04 17:51:20.000000 websocket-client-1.5.3/examples/echo_client.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     1009 2023-02-04 17:51:20.000000 websocket-client-1.5.3/examples/echoapp_client.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)      351 2023-02-04 17:51:20.000000 websocket-client-1.5.3/examples/rel_client.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)       59 2023-06-09 09:33:59.804877 websocket-client-1.5.3/setup.cfg
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     2641 2023-06-09 09:20:50.000000 websocket-client-1.5.3/setup.py
+drwxrwxr-x   0 drift3r   (1000) drift3r   (1000)        0 2023-06-09 09:33:59.800877 websocket-client-1.5.3/websocket/
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)      801 2023-06-09 09:20:59.000000 websocket-client-1.5.3/websocket/__init__.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)    13619 2023-05-21 19:20:24.000000 websocket-client-1.5.3/websocket/_abnf.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)    20185 2023-05-21 19:20:24.000000 websocket-client-1.5.3/websocket/_app.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     2164 2023-05-21 19:20:24.000000 websocket-client-1.5.3/websocket/_cookiejar.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)    19872 2023-04-07 22:45:05.000000 websocket-client-1.5.3/websocket/_core.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     2106 2023-04-07 22:59:49.000000 websocket-client-1.5.3/websocket/_exceptions.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     6610 2023-06-09 09:14:52.000000 websocket-client-1.5.3/websocket/_handshake.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)    11806 2023-04-07 22:47:13.000000 websocket-client-1.5.3/websocket/_http.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     2220 2023-05-21 19:20:24.000000 websocket-client-1.5.3/websocket/_logging.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     4979 2023-05-21 19:20:24.000000 websocket-client-1.5.3/websocket/_socket.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     1122 2023-02-04 17:51:20.000000 websocket-client-1.5.3/websocket/_ssl_compat.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     4932 2023-05-21 19:20:24.000000 websocket-client-1.5.3/websocket/_url.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     3636 2023-05-21 19:20:24.000000 websocket-client-1.5.3/websocket/_utils.py
+-rwxrwxr-x   0 drift3r   (1000) drift3r   (1000)     7116 2023-06-09 09:20:10.000000 websocket-client-1.5.3/websocket/_wsdump.py
+drwxrwxr-x   0 drift3r   (1000) drift3r   (1000)        0 2023-06-09 09:33:59.800877 websocket-client-1.5.3/websocket/tests/
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)        0 2023-02-04 17:51:20.000000 websocket-client-1.5.3/websocket/tests/__init__.py
+drwxrwxr-x   0 drift3r   (1000) drift3r   (1000)        0 2023-06-09 09:33:59.800877 websocket-client-1.5.3/websocket/tests/data/
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)      163 2023-02-04 17:51:20.000000 websocket-client-1.5.3/websocket/tests/data/header01.txt
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)      161 2023-02-04 17:51:20.000000 websocket-client-1.5.3/websocket/tests/data/header02.txt
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)      216 2023-02-04 17:51:20.000000 websocket-client-1.5.3/websocket/tests/data/header03.txt
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)      486 2023-05-21 19:20:24.000000 websocket-client-1.5.3/websocket/tests/echo-server.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     4175 2023-02-04 17:51:20.000000 websocket-client-1.5.3/websocket/tests/test_abnf.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)    12669 2023-02-04 17:51:20.000000 websocket-client-1.5.3/websocket/tests/test_app.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     4325 2023-02-04 17:51:20.000000 websocket-client-1.5.3/websocket/tests/test_cookiejar.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     9623 2023-02-04 17:51:20.000000 websocket-client-1.5.3/websocket/tests/test_http.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)    14589 2023-02-04 17:51:20.000000 websocket-client-1.5.3/websocket/tests/test_url.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)    18072 2023-02-04 17:51:20.000000 websocket-client-1.5.3/websocket/tests/test_websocket.py
+drwxrwxr-x   0 drift3r   (1000) drift3r   (1000)        0 2023-06-09 09:33:59.804877 websocket-client-1.5.3/websocket_client.egg-info/
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     7350 2023-06-09 09:33:59.000000 websocket-client-1.5.3/websocket_client.egg-info/PKG-INFO
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     1014 2023-06-09 09:33:59.000000 websocket-client-1.5.3/websocket_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)        1 2023-06-09 09:33:59.000000 websocket-client-1.5.3/websocket_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)       50 2023-06-09 09:33:59.000000 websocket-client-1.5.3/websocket_client.egg-info/entry_points.txt
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)       94 2023-06-09 09:33:59.000000 websocket-client-1.5.3/websocket_client.egg-info/requires.txt
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)       10 2023-06-09 09:33:59.000000 websocket-client-1.5.3/websocket_client.egg-info/top_level.txt
```

### Comparing `websocket-client-1.5.2/ChangeLog` & `websocket-client-1.5.3/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 ChangeLog
 ============
 
+- 1.5.3
+  - Add logic to avoid error in the case where content-length header does not exist, bug introduced in 1.5.2 (#911)
+  - Fix wsdump.py script typing, bug introduced in 1.5.2 (#914)
+
 - 1.5.2
   - Add typehints (#908)
   - Fix pytype errors (#906)
   - Fix args passed to logging function (#898)
   - Standardize PEP 3101 formatting (c6a445f)
   - Add more verbose exception for unsuccessful handshake for #900 (f85ae1f)
```

### Comparing `websocket-client-1.5.2/LICENSE` & `websocket-client-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `websocket-client-1.5.2/PKG-INFO` & `websocket-client-1.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: websocket-client
-Version: 1.5.2
+Version: 1.5.3
 Summary: WebSocket client for Python with low level API options
 Home-page: https://github.com/websocket-client/websocket-client.git
 Download-URL: https://github.com/websocket-client/websocket-client/releases
 Author: liris
 Author-email: liris.pp@gmail.com
 License: Apache-2.0
 Project-URL: Documentation, https://websocket-client.readthedocs.io/
```

### Comparing `websocket-client-1.5.2/README.md` & `websocket-client-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `websocket-client-1.5.2/examples/echoapp_client.py` & `websocket-client-1.5.3/examples/echoapp_client.py`

 * *Files identical despite different names*

### Comparing `websocket-client-1.5.2/setup.py` & `websocket-client-1.5.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-VERSION = "1.5.2"
+VERSION = "1.5.3"
 
 install_requires = []
 tests_require = []
 
 setup(
     name="websocket-client",
     version=VERSION,
```

### Comparing `websocket-client-1.5.2/websocket/__init__.py` & `websocket-client-1.5.3/websocket/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,8 +19,8 @@
 from ._abnf import *
 from ._app import WebSocketApp, setReconnect
 from ._core import *
 from ._exceptions import *
 from ._logging import *
 from ._socket import *
 
-__version__ = "1.5.2"
+__version__ = "1.5.3"
```

### Comparing `websocket-client-1.5.2/websocket/_abnf.py` & `websocket-client-1.5.3/websocket/_abnf.py`

 * *Files identical despite different names*

### Comparing `websocket-client-1.5.2/websocket/_app.py` & `websocket-client-1.5.3/websocket/_app.py`

 * *Files identical despite different names*

### Comparing `websocket-client-1.5.2/websocket/_cookiejar.py` & `websocket-client-1.5.3/websocket/_cookiejar.py`

 * *Files identical despite different names*

### Comparing `websocket-client-1.5.2/websocket/_core.py` & `websocket-client-1.5.3/websocket/_core.py`

 * *Files identical despite different names*

### Comparing `websocket-client-1.5.2/websocket/_exceptions.py` & `websocket-client-1.5.3/websocket/_exceptions.py`

 * *Files identical despite different names*

### Comparing `websocket-client-1.5.2/websocket/_handshake.py` & `websocket-client-1.5.3/websocket/_handshake.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,24 +131,26 @@
     client_cookie = options.get("cookie", None)
 
     cookie = "; ".join(filter(None, [server_cookie, client_cookie]))
 
     if cookie:
         headers.append("Cookie: {cookie}".format(cookie=cookie))
 
-    headers.append("")
-    headers.append("")
-
+    headers.extend(("", ""))
     return headers, key
 
 
 def _get_resp_headers(sock, success_statuses=SUCCESS_STATUSES):
     status, resp_headers, status_message = read_headers(sock)
     if status not in success_statuses:
-        response_body = sock.recv(int(resp_headers['content-length']))  # read the body of the HTTP error message response and include it in the exception
+        content_len = resp_headers.get('content-length')
+        if content_len:
+            response_body = sock.recv(int(content_len))  # read the body of the HTTP error message response and include it in the exception
+        else:
+            response_body = None
         raise WebSocketBadStatusException("Handshake status {status} {message} -+-+- {headers} -+-+- {body}".format(status=status, message=status_message, headers=resp_headers, body=response_body), status, status_message, resp_headers, response_body)
     return status, resp_headers
 
 
 _HEADERS_TO_CHECK = {
     "upgrade": "websocket",
     "connection": "upgrade",
```

### Comparing `websocket-client-1.5.2/websocket/_http.py` & `websocket-client-1.5.3/websocket/_http.py`

 * *Files identical despite different names*

### Comparing `websocket-client-1.5.2/websocket/_logging.py` & `websocket-client-1.5.3/websocket/_logging.py`

 * *Files identical despite different names*

### Comparing `websocket-client-1.5.2/websocket/_socket.py` & `websocket-client-1.5.3/websocket/_socket.py`

 * *Files identical despite different names*

### Comparing `websocket-client-1.5.2/websocket/_ssl_compat.py` & `websocket-client-1.5.3/websocket/_ssl_compat.py`

 * *Files identical despite different names*

### Comparing `websocket-client-1.5.2/websocket/_url.py` & `websocket-client-1.5.3/websocket/_url.py`

 * *Files identical despite different names*

### Comparing `websocket-client-1.5.2/websocket/_utils.py` & `websocket-client-1.5.3/websocket/_utils.py`

 * *Files identical despite different names*

### Comparing `websocket-client-1.5.2/websocket/_wsdump.py` & `websocket-client-1.5.3/websocket/_wsdump.py`

 * *Files 3% similar despite different names*

```diff
@@ -150,26 +150,26 @@
     ws = websocket.create_connection(args.url, sslopt=opts, **options)
     if args.raw:
         console = NonInteractive()
     else:
         console = InteractiveConsole()
         print("Press Ctrl+C to quit")
 
-    def recv() -> tuple(int, str):
+    def recv() -> tuple[int, str]:
         try:
             frame = ws.recv_frame()
         except websocket.WebSocketException:
-            return websocket.ABNF.OPCODE_CLOSE, None
+            return websocket.ABNF.OPCODE_CLOSE, ""
         if not frame:
             raise websocket.WebSocketException("Not a valid frame {frame}".format(frame=frame))
         elif frame.opcode in OPCODE_DATA:
             return frame.opcode, frame.data
         elif frame.opcode == websocket.ABNF.OPCODE_CLOSE:
             ws.send_close()
-            return frame.opcode, None
+            return frame.opcode, ""
         elif frame.opcode == websocket.ABNF.OPCODE_PING:
             ws.pong(frame.data)
             return frame.opcode, frame.data
 
         return frame.opcode, frame.data
 
     def recv_ws() -> None:
```

### Comparing `websocket-client-1.5.2/websocket/tests/test_abnf.py` & `websocket-client-1.5.3/websocket/tests/test_abnf.py`

 * *Files identical despite different names*

### Comparing `websocket-client-1.5.2/websocket/tests/test_app.py` & `websocket-client-1.5.3/websocket/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `websocket-client-1.5.2/websocket/tests/test_cookiejar.py` & `websocket-client-1.5.3/websocket/tests/test_cookiejar.py`

 * *Files identical despite different names*

### Comparing `websocket-client-1.5.2/websocket/tests/test_http.py` & `websocket-client-1.5.3/websocket/tests/test_http.py`

 * *Files identical despite different names*

### Comparing `websocket-client-1.5.2/websocket/tests/test_url.py` & `websocket-client-1.5.3/websocket/tests/test_url.py`

 * *Files identical despite different names*

### Comparing `websocket-client-1.5.2/websocket/tests/test_websocket.py` & `websocket-client-1.5.3/websocket/tests/test_websocket.py`

 * *Files identical despite different names*

### Comparing `websocket-client-1.5.2/websocket_client.egg-info/PKG-INFO` & `websocket-client-1.5.3/websocket_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: websocket-client
-Version: 1.5.2
+Version: 1.5.3
 Summary: WebSocket client for Python with low level API options
 Home-page: https://github.com/websocket-client/websocket-client.git
 Download-URL: https://github.com/websocket-client/websocket-client/releases
 Author: liris
 Author-email: liris.pp@gmail.com
 License: Apache-2.0
 Project-URL: Documentation, https://websocket-client.readthedocs.io/
```

### Comparing `websocket-client-1.5.2/websocket_client.egg-info/SOURCES.txt` & `websocket-client-1.5.3/websocket_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

