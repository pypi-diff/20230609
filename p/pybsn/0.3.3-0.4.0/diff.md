# Comparing `tmp/pybsn-0.3.3.tar.gz` & `tmp/pybsn-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybsn-0.3.3.tar", last modified: Mon Feb  8 19:24:16 2021, max compression
+gzip compressed data, was "pybsn-0.4.0.tar", last modified: Fri Jun  9 10:07:54 2023, max compression
```

## Comparing `pybsn-0.3.3.tar` & `pybsn-0.4.0.tar`

### file list

```diff
@@ -1,19 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-08 19:24:16.891733 pybsn-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (121)      354 2021-02-08 19:24:16.891733 pybsn-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6592 2021-02-08 19:24:06.000000 pybsn-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-08 19:24:16.891733 pybsn-0.3.3/bin/
--rwxr-xr-x   0 runner    (1001) docker     (121)     5731 2021-02-08 19:24:06.000000 pybsn-0.3.3/bin/pybsn-repl
--rwxr-xr-x   0 runner    (1001) docker     (121)     4352 2021-02-08 19:24:06.000000 pybsn-0.3.3/bin/pybsn-schema
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-08 19:24:16.891733 pybsn-0.3.3/pybsn/
--rw-r--r--   0 runner    (1001) docker     (121)    17417 2021-02-08 19:24:06.000000 pybsn-0.3.3/pybsn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-08 19:24:16.891733 pybsn-0.3.3/pybsn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      354 2021-02-08 19:24:16.000000 pybsn-0.3.3/pybsn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      266 2021-02-08 19:24:16.000000 pybsn-0.3.3/pybsn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-02-08 19:24:16.000000 pybsn-0.3.3/pybsn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-02-08 19:24:16.000000 pybsn-0.3.3/pybsn.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       46 2021-02-08 19:24:16.000000 pybsn-0.3.3/pybsn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2021-02-08 19:24:16.000000 pybsn-0.3.3/pybsn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-02-08 19:24:16.891733 pybsn-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      658 2021-02-08 19:24:06.000000 pybsn-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-08 19:24:16.891733 pybsn-0.3.3/test/
--rw-r--r--   0 runner    (1001) docker     (121)     8976 2021-02-08 19:24:06.000000 pybsn-0.3.3/test/test_bigdb_client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:07:54.706987 pybsn-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1715 2023-06-09 10:07:42.000000 pybsn-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      337 2023-06-09 10:07:54.706987 pybsn-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6366 2023-06-09 10:07:42.000000 pybsn-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:07:54.702987 pybsn-0.4.0/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5625 2023-06-09 10:07:42.000000 pybsn-0.4.0/bin/pybsn-repl
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4288 2023-06-09 10:07:42.000000 pybsn-0.4.0/bin/pybsn-schema
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:07:54.702987 pybsn-0.4.0/pybsn/
+-rw-r--r--   0 runner    (1001) docker     (122)    26495 2023-06-09 10:07:42.000000 pybsn-0.4.0/pybsn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:07:54.702987 pybsn-0.4.0/pybsn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      337 2023-06-09 10:07:54.000000 pybsn-0.4.0/pybsn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      399 2023-06-09 10:07:54.000000 pybsn-0.4.0/pybsn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-09 10:07:54.000000 pybsn-0.4.0/pybsn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-09 10:07:54.000000 pybsn-0.4.0/pybsn.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2023-06-09 10:07:54.000000 pybsn-0.4.0/pybsn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-06-09 10:07:54.000000 pybsn-0.4.0/pybsn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-09 10:07:54.706987 pybsn-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      658 2023-06-09 10:07:42.000000 pybsn-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:07:54.706987 pybsn-0.4.0/test/
+-rw-r--r--   0 runner    (1001) docker     (122)    13307 2023-06-09 10:07:42.000000 pybsn-0.4.0/test/test_bigdb_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6964 2023-06-09 10:07:42.000000 pybsn-0.4.0/test/test_node.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15152 2023-06-09 10:07:42.000000 pybsn-0.4.0/test/test_timeout_bigdbclient.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2976 2023-06-09 10:07:42.000000 pybsn-0.4.0/test/test_timeout_bigdbclient_integration.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4464 2023-06-09 10:07:42.000000 pybsn-0.4.0/test/test_timeout_connect.py
```

### Comparing `pybsn-0.3.3/README.md` & `pybsn-0.4.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,57 +1,58 @@
 # pybsn
 pybsn is a python interface to [Big Switch Network](http://bigswitch.com) products
 
-[![Build Status](https://travis-ci.org/bigswitch/pybsn.svg)](https://travis-ci.org/bigswitch/pybsn)
 [![PyPI version](https://badge.fury.io/py/pybsn.svg)](https://pypi.python.org/pypi/pybsn/)
 
 ## Installation
 
+pybsn supports Python versions 3.6 to 3.11. pybsn with Python 3.6
+support has been deprecated, and may be removed in the
+next release.
+
+
 ```bash
-pip install pybsn
-# ... or ...
 pip3 install pybsn
 ```
-pybsn is compatible with python 2.7+ and python 3.
+As of version 0.4.0, pybsn is only compatible with python 3.6 or newer.
 
 ---
 ## PyBSN Repl - Interactive Shell
 
-`pybsn-repl` is a powerful, interactive shell for the REST API. It is based on and requires python3 and ipython 7.0. (**Note**: The pybsn library works with python 2.7 and python 3, the repl program requires python 3!)
+`pybsn-repl` is a powerful, interactive shell for the REST API. It is based on and requires python3.5 or newer and ipython 7.9 or newer.
 
 ### Installing Python3 on Mac
 
-[Homebrew](https://brew.sh/) is a recommended option to install python3 on mac
+[Homebrew](https://brew.sh/) is a recommended option to install python3 on mac.
 
 After you install homebrew, install python3 with
 
 ```
 brew install python
 ```
 
 ### Installing IPython 7
 ```bash
 pip3 install ipython
 ```
-* Note: make sure you use the `pip` module associated with `python3`. Often, it is available as `pip3`; otherwise you may want to try `python3 -m pip install ...` instead.
 
 ### Running pybsn-repl
 ```bash
 ./bin/pybsn-repl -H <controller_host> -u <user> -p <passwd>
 ```
-**Note:** `pybsn-repl` requires `pybsn` to be available; you can either install it from `pip` (see above); or use it directly from the source by prefixing the
+**Note:** `pybsn-repl` requires `pybsn` to be available; you can either install it from `pip3` (see above); or use it directly from the source by prefixing the
 command with `PYTHONPATH=<dir>`, e.g.,
 
 ```bash
 ~/dev/pybsn $ PYTHONPATH=. ./bin/pybsn-repl -H <controller_host> -u <user> -p <passwd>
 ```
 
 ### Using pybsn-repl
 
-PyBSN-reply presents an IPython shell to interact with the REST API.
+PyBSN-repl presents an IPython shell to interact with the REST API.
 
 It accepts any python expressions, and exposes the following variables as primary
 entry points:
 * `ctrl`: BigDbClient instance
 * `root`: ctrl.root - a reference to the root node.
 
 #### Node Hierarchy
@@ -109,19 +110,19 @@
 
 * call HTTP methods on the node to mutate data:
    * `node.post(data)` - inserts data at the node
    * `node.put(data)` - replaces the node entirely with the new data
    * `node.patch(data)` - selectively updates the node with the given data, leaving unspecified values untouched
    * `node.delete()` - delete the node
 
-In these examples, `data` is a JSON serializable object, often a dictionary. Node that the dictionary keys must be in schema format at present (i.e., with hyphens, `some-long-property` not `some_long_property`).
+In these examples, `data` is a JSON serializable object, often a dictionary. Note that the dictionary keys must be in schema format at present (i.e., with hyphens, `some-long-property` not `some_long_property`).
 
 * call `node.rpc(input_data)` to make an RPC call to the RPC specified in the node.
 
-`input_data` is a JSON serializable object, often a dictionary. Node that the dictionary keys must be in schema format at present (i.e., with hyphens, `some-long-property` not `some_long_property`).
+`input_data` is a JSON serializable object, often a dictionary. Note that the dictionary keys must be in schema format at present (i.e., with hyphens, `some-long-property` not `some_long_property`).
 
 The output/result of the RPC returned as a dictionary.
 
 
 #### More Examples:
 
 ```python
```

### Comparing `pybsn-0.3.3/bin/pybsn-repl` & `pybsn-0.4.0/bin/pybsn-repl`

 * *Files 5% similar despite different names*

```diff
@@ -15,25 +15,22 @@
 
     # Get info for all switches
     root.core.switch()
 
     # Get info for a specific switch
     root.core.switch.match(name="leaf0a").get()
 """
-from __future__ import print_function
-
 import pybsn
 import argparse
 import logging
 import textwrap
 import re
 import os
 from traitlets.config.loader import Config
 from IPython.terminal.ipapp import TerminalIPythonApp
-from IPython.core.inputtransformer import StatelessInputTransformer
 from IPython.core.magic import Magics, magics_class, line_magic
 
 
 def env_var(value):
     if value not in os.environ:
         raise argparse.ArgumentTypeError("'%s' is not an environment variable" % value)
     return os.environ[value]
@@ -56,32 +53,35 @@
 logging.getLogger("pybsn").setLevel(logging.DEBUG if args.verbose > 1 else logging.INFO)
 
 if args.token:
     ctrl = pybsn.connect(host=args.host, token=args.token, login=False)
 else:
     ctrl = pybsn.connect(host=args.host, username=args.user, password=args.password)
 
+
 def line_transform(lines):
     def convert(line):
         if line.endswith('#'):
             return "show_schema(%s)" % line[:-1]
         else:
             return line
 
-    return [ convert(l.strip()) + "\n" for l in lines ]
+    return [convert(li.strip()) + "\n" for li in lines]
+
 
 @magics_class
 class BsnMagics(Magics):
     @line_magic
     def help(self, s):
         print(__doc__.strip())
 
+
 def show_schema(root, max_depth=1, verbose=True):
     def pretty_type(node):
-        if not 'typeSchemaNode' in node:
+        if 'typeSchemaNode' not in node:
             return node['leafType'].lower()
 
         t = node['typeSchemaNode']
 
         if t['leafType'] == 'ENUMERATION':
             names = [x for x in t['typeValidator'] if x['type'] == 'ENUMERATION_VALIDATOR'][0]['names']
             return "enum { %s }" % ', '.join(names)
@@ -126,32 +126,33 @@
         elif node['nodeType'] == 'LEAF':
             output(name, ":", pretty_type(node), config, description)
         elif node['nodeType'] == 'LEAF_LIST':
             output(name, ":", "list of", pretty_type(node['leafSchemaNode']), config, description)
         elif node['nodeType'] == 'RPC':
             output(name, "(rpc)", description)
             if max_depth is not None and depth < max_depth:
-                for name, item in ( ("in", "inputSchemaNode"), ("out", "outputSchemaNode")):
+                for name, item in (("in", "inputSchemaNode"), ("out", "outputSchemaNode")):
                     if item in node:
                         traverse(node[item], depth+1, name, max_depth=None)
                     else:
                         output(name, "(NONE)", depth=depth+1)
         else:
             assert False, "unknown node type %s" % node['nodeType']
 
     traverse(root.schema(), name=root._path, max_depth=max_depth)
 
+
 config = Config()
 config.TerminalInteractiveShell.banner1 = "pybsn REPL - Run %help for help"
 config.TerminalInteractiveShell.confirm_exit = False
 
 user_ns = dict(ctrl=ctrl, root=ctrl.root, show_schema=show_schema)
 
 app = TerminalIPythonApp(config=config)
 app.interact = not args.command
-app.initialize(argv = [])
+app.initialize(argv=[])
 app.shell.push(user_ns, interactive=False)
 app.shell.input_transformers_cleanup.append(line_transform)
 app.shell.register_magics(BsnMagics(app.shell))
 if args.command:
     app.shell.run_cell(args.command)
 app.start()
```

### Comparing `pybsn-0.3.3/bin/pybsn-schema` & `pybsn-0.4.0/bin/pybsn-schema`

 * *Files 4% similar despite different names*

```diff
@@ -11,16 +11,14 @@
 By default this will display the entire schema. To navigate the schema more
 easily, you'll want to use the 'path' and '--max-depth' options. For example:
 
     pybsn-schema -H $HOSTNAME -d 2 -v controller.core.switch
 
 This shows 2 levels of schema starting from the path "controller.core.switch".
 """
-from __future__ import print_function
-
 import pybsn
 import argparse
 import json
 import textwrap
 import re
 
 
@@ -36,15 +34,15 @@
 parser.add_argument("--raw", action="store_true", help="Print raw JSON")
 parser.add_argument("--verbose", "-v", action="store_true", help="Include descriptions in the output")
 
 args = parser.parse_args()
 
 
 def pretty_type(node):
-    if not 'typeSchemaNode' in node:
+    if 'typeSchemaNode' not in node:
         return node['leafType'].lower()
 
     t = node['typeSchemaNode']
 
     if t['leafType'] == 'ENUMERATION':
         names = list([x for x in t['typeValidator'] if x['type'] == 'ENUMERATION_VALIDATOR'][0]['names'].keys())
         if not args.verbose and len(names) > 4:
@@ -52,14 +50,15 @@
         return "enum { %s }" % ', '.join(names)
     elif t['leafType'] == 'UNION':
         names = [x['name'] for x in t['typeSchemaNodes']]
         return "union { %s }" % ', '.join(names)
     else:
         return t['leafType'].lower()
 
+
 def traverse(node, depth=0, name="root"):
     def output(*s, **kw):
         d = kw.get("depth", depth)
         print(" " * (d * 2) + ' '.join(s))
 
     if args.max_depth is not None and depth > args.max_depth:
         return
@@ -90,29 +89,30 @@
         traverse(node['listElementSchemaNode'], depth, name)
     elif node['nodeType'] == 'LEAF':
         output(name, ":", pretty_type(node), config, description)
     elif node['nodeType'] == 'LEAF_LIST':
         output(name, ":", "list of", pretty_type(node['leafSchemaNode']), config, description)
     elif node['nodeType'] == 'RPC':
         output(name, description, "(RPC)")
-        for name, item in ( ("in", "inputSchemaNode"), ("out", "outputSchemaNode")):
+        for name, item in (("in", "inputSchemaNode"), ("out", "outputSchemaNode")):
             if item in node:
                 traverse(node[item], depth+1, name)
             else:
                 output(name, "(NONE)", depth=depth+1)
     else:
         assert False, "unknown node type %s" % node['nodeType']
 
+
 path = args.path.replace('.', '/').replace('_', '-')
 
 
 if args.json_file:
     with open(args.json_file) as file_:
         schema = json.load(file_)
 else:
     bcf = pybsn.connect(args.host, args.user, args.password)
     schema = bcf.schema(path)
 
 if args.raw:
-    print(json.dumps(schema, indent=4, cls=pybcf.BCFJSONEncoder))
+    print(json.dumps(schema, indent=4))
 else:
     traverse(schema, name=path)
```

### Comparing `pybsn-0.3.3/setup.py` & `pybsn-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 
 setup(name='pybsn',
-    version='0.3.3',
+    version='0.4.0',
     description="pybsn is a python interface to Big Switch Networks' products",
     url='https://github.com/floodlight/pybsn',
     author='Andreas Wundsam, Andre Kutzleb, Jason Parraga, Rich Lane',
     author_email='Andreas.Wundsam@arista.com, Andre.Kutzleb@arista.com',
     license='ECLIPSE',
     packages=['pybsn'],
     zip_safe=False,
```

### Comparing `pybsn-0.3.3/test/test_bigdb_client.py` & `pybsn-0.4.0/test/test_bigdb_client.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import json
 import os
 import logging
 import re
 import unittest
-
+from unittest.mock import patch
 import requests
 
 import pybsn
 import responses
 
 my_dir = os.path.dirname(__file__)
 
 
-class TestBigDbClient(unittest.TestCase):
+class TestBigDBClient(unittest.TestCase):
     def setUp(self):
         self.client = pybsn.connect("http://127.0.0.1:8080")
 
     def _login_cb(self, req):
         self.assertEqual(json.loads(req.body), {'user': 'admin', 'password': 'somepassword'})
         headers = {
             "Set-Cookie": "session_cookie=v_8yOI7FI-WKr-5QU6nxoJkVtAu5rKI-; Path=/api/;"
@@ -180,21 +180,114 @@
 
         with pybsn.connect("http://127.0.0.1:8080") as client:
             client.session.cookies.set_cookie(
                 requests.cookies.create_cookie(name="session_cookie", value="value"))
             client.get("controller/core/healthy")
 
     @responses.activate
+    def test_get(self):
+        responses.add(responses.GET, "http://127.0.0.1:8080/api/v1/data/controller/test",
+                      json={'state': "ok" }, status=200)
+        result = self.client.get(path="controller/test")
+        self.assertEqual(result, {'state':"ok"})
+
+    @responses.activate
+    def test_get_with_param(self):
+        responses.add(responses.GET, "http://127.0.0.1:8080/api/v1/data/controller/test?state-type=global-config",
+                      json={'state': "ok" }, status=200)
+        result = self.client.get(path="controller/test", params={'state-type': 'global-config'})
+        self.assertEqual(result, {'state':"ok"})
+
+    @responses.activate
+    def _mutate_test(self, response_type, method_name, add_params=False):
+        def _cb(req):
+            self.assertEqual(json.loads(req.body), {"foo": "bar"})
+            return (204, {}, None)
+
+        expected_url = "http://127.0.0.1:8080/api/v1/data/controller/test"
+        path = "controller/test"
+
+        if add_params:
+            expected_url += "?state-type=global-config"
+
+        responses.add_callback(response_type, expected_url, callback=_cb)
+        method = getattr(self.client, method_name)
+        if add_params:
+            method(path="controller/test", data={"foo": "bar"}, params={'state-type': 'global-config'})
+        else:
+            method(path="controller/test", data={"foo": "bar"})
+
+    def test_mutations(self):
+        self._mutate_test(response_type=responses.POST, method_name="post", add_params=False)
+        self._mutate_test(response_type=responses.POST, method_name="post", add_params=True)
+        self._mutate_test(response_type=responses.PUT, method_name="put", add_params=False)
+        self._mutate_test(response_type=responses.PUT, method_name="put", add_params=True)
+        self._mutate_test(response_type=responses.PATCH, method_name="patch", add_params=False)
+        self._mutate_test(response_type=responses.PATCH, method_name="patch", add_params=True)
+
+    @responses.activate
+    def test_delete(self):
+        responses.add(responses.DELETE, "http://127.0.0.1:8080/api/v1/data/controller/test",
+                      status=204)
+        self.client.delete(path="controller/test")
+
+    @responses.activate
+    def test_delete_with_param(self):
+        responses.add(responses.DELETE, "http://127.0.0.1:8080/api/v1/data/controller/test?state-type=global-config",
+                    status=204)
+        self.client.delete(path="controller/test", params={'state-type': 'global-config'})
+
+    @responses.activate
     def test_rpc(self):
         responses.add(responses.POST, "http://127.0.0.1:8080/api/v1/rpc/controller/rpc",
                       json={'id': 1234}, status=200)
         result = self.client.rpc(path="controller/rpc",
                                  data={"description": "desc"})
         self.assertEqual(result, {'id': 1234})
 
     @responses.activate
+    def test_rpc_async_accepted(self):
+        responses.add(responses.POST, "http://127.0.0.1:8080/api/v1/rpc/controller/rpc",
+                      status=202)
+        result = self.client.rpc(path="controller/rpc",
+                                 data={"description": "desc"},
+                                 params={'initiate-async': 'asyncId'})
+        self.assertEqual(result, None)
+
+    @responses.activate
     def test_no_response(self):
         responses.add(responses.POST, "http://127.0.0.1:8080/api/v1/rpc/controller/rpc",
                       status=204)
         result = self.client.rpc(path="controller/rpc",
                                  data={"description": "desc"})
         self.assertIsNone(result)
+
+    @responses.activate
+    def test_schema(self):
+        responses.add(responses.GET, "http://127.0.0.1:8080/api/v1/schema/",
+                      json={'state': "ok" }, status=200)
+        result = self.client.schema()
+        self.assertEqual(result, {'state':"ok"})
+
+    @responses.activate
+    def test_schema_with_path(self):
+        responses.add(responses.GET, "http://127.0.0.1:8080/api/v1/schema/foo",
+                      json={'state': "ok" }, status=200)
+        result = self.client.schema(path="foo")
+        self.assertEqual(result, {'state':"ok"})
+
+    @responses.activate
+    def test_schema_failed(self):
+        responses.add(responses.GET, "http://127.0.0.1:8080/api/v1/schema/",
+                      json={'state': "ok" }, status=404)
+        with self.assertRaises(requests.exceptions.HTTPError):
+            self.client.schema()
+
+    @responses.activate
+    def test_schema_logged(self):
+        with patch.object(logging.Logger, 'isEnabledFor') as mock_is_enabled:
+            mock_is_enabled.return_value = True
+            with patch.object(logging.Logger, "debug") as mock_debug:
+                responses.add(responses.GET, "http://127.0.0.1:8080/api/v1/schema/",
+                      json={'state': "ok" }, status=200)
+                self.client.schema()
+                mock_debug.assert_called()
```

