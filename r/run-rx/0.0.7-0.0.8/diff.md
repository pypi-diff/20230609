# Comparing `tmp/run_rx-0.0.7.tar.gz` & `tmp/run_rx-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "run_rx-0.0.7.tar", max compression
+gzip compressed data, was "run_rx-0.0.8.tar", max compression
```

## Comparing `run_rx-0.0.7.tar` & `run_rx-0.0.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1069 2023-05-16 20:24:41.276898 run_rx-0.0.7/LICENSE.txt
--rw-r--r--   0        0        0     1679 2023-05-19 14:53:21.015913 run_rx-0.0.7/README.md
--rw-r--r--   0        0        0      313 2023-06-01 23:35:09.526681 run_rx-0.0.7/install/.rxignore
--rw-r--r--   0        0        0      274 2023-06-04 16:34:29.656668 run_rx-0.0.7/install/README.md
--rw-r--r--   0        0        0       98 2023-05-16 20:24:41.277933 run_rx-0.0.7/install/python-cpu
--rw-r--r--   0        0        0       98 2023-06-06 18:01:13.521487 run_rx-0.0.7/install/python-gpu
--rw-r--r--   0        0        0      736 2023-06-07 13:36:28.564487 run_rx-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      300 2023-05-16 20:24:41.279362 run_rx-0.0.7/rx/__main__.py
--rw-r--r--   0        0        0     2850 2023-06-06 23:31:04.918753 run_rx-0.0.7/rx/client/commands/exec.py
--rw-r--r--   0        0        0     1284 2023-06-06 19:06:15.414502 run_rx-0.0.7/rx/client/commands/init.py
--rw-r--r--   0        0        0     2109 2023-06-04 16:41:38.419103 run_rx-0.0.7/rx/client/configuration/config_base.py
--rw-r--r--   0        0        0     7016 2023-06-07 13:36:36.440622 run_rx-0.0.7/rx/client/configuration/local.py
--rw-r--r--   0        0        0      641 2023-06-06 18:04:41.546820 run_rx-0.0.7/rx/client/configuration/remote.py
--rw-r--r--   0        0        0      256 2023-05-16 20:24:41.281715 run_rx-0.0.7/rx/client/grpc_helper.py
--rw-r--r--   0        0        0     9694 2023-05-16 20:24:41.282187 run_rx-0.0.7/rx/client/login.py
--rw-r--r--   0        0        0     2029 2023-05-16 20:24:41.282556 run_rx-0.0.7/rx/client/menu.py
--rw-r--r--   0        0        0     1092 2023-05-16 20:24:41.282728 run_rx-0.0.7/rx/client/output_handler.py
--rw-r--r--   0        0        0     3306 2023-06-06 18:01:13.524830 run_rx-0.0.7/rx/client/rsync.py
--rw-r--r--   0        0        0     4668 2023-06-07 12:43:18.155388 run_rx-0.0.7/rx/client/trex_client.py
--rw-r--r--   0        0        0     1603 2023-05-16 20:24:41.283538 run_rx-0.0.7/rx/client/user.py
--rw-r--r--   0        0        0     5565 2023-06-07 13:22:07.723770 run_rx-0.0.7/rx/client/worker_client.py
--rw-r--r--   0        0        0     6391 2023-06-06 22:54:37.232578 run_rx-0.0.7/rx/proto/rx_pb2.py
--rw-r--r--   0        0        0     8466 2023-06-06 22:54:37.232746 run_rx-0.0.7/rx/proto/rx_pb2.pyi
--rw-r--r--   0        0        0    12622 2023-06-06 22:54:37.233305 run_rx-0.0.7/rx/proto/rx_pb2_grpc.py
--rw-r--r--   0        0        0     2597 1970-01-01 00:00:00.000000 run_rx-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-16 20:24:41.276898 run_rx-0.0.8/LICENSE.txt
+-rw-r--r--   0        0        0     1679 2023-05-19 14:53:21.015913 run_rx-0.0.8/README.md
+-rw-r--r--   0        0        0      313 2023-06-01 23:35:09.526681 run_rx-0.0.8/install/.rxignore
+-rw-r--r--   0        0        0      274 2023-06-04 16:34:29.656668 run_rx-0.0.8/install/README.md
+-rw-r--r--   0        0        0       98 2023-05-16 20:24:41.277933 run_rx-0.0.8/install/python-cpu
+-rw-r--r--   0        0        0       98 2023-06-06 18:01:13.521487 run_rx-0.0.8/install/python-gpu
+-rw-r--r--   0        0        0      736 2023-06-09 02:26:40.439644 run_rx-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      300 2023-05-16 20:24:41.279362 run_rx-0.0.8/rx/__main__.py
+-rw-r--r--   0        0        0     2850 2023-06-06 23:31:04.918753 run_rx-0.0.8/rx/client/commands/exec.py
+-rw-r--r--   0        0        0     3782 2023-06-09 01:08:03.971935 run_rx-0.0.8/rx/client/commands/init.py
+-rw-r--r--   0        0        0     2109 2023-06-04 16:41:38.419103 run_rx-0.0.8/rx/client/configuration/config_base.py
+-rw-r--r--   0        0        0     7016 2023-06-09 02:26:51.137891 run_rx-0.0.8/rx/client/configuration/local.py
+-rw-r--r--   0        0        0      641 2023-06-06 18:04:41.546820 run_rx-0.0.8/rx/client/configuration/remote.py
+-rw-r--r--   0        0        0      256 2023-05-16 20:24:41.281715 run_rx-0.0.8/rx/client/grpc_helper.py
+-rw-r--r--   0        0        0     9852 2023-06-09 00:46:28.253468 run_rx-0.0.8/rx/client/login.py
+-rw-r--r--   0        0        0     2251 2023-06-09 01:11:45.554956 run_rx-0.0.8/rx/client/menu.py
+-rw-r--r--   0        0        0     1092 2023-05-16 20:24:41.282728 run_rx-0.0.8/rx/client/output_handler.py
+-rw-r--r--   0        0        0     3306 2023-06-06 18:01:13.524830 run_rx-0.0.8/rx/client/rsync.py
+-rw-r--r--   0        0        0     4668 2023-06-08 21:15:48.685289 run_rx-0.0.8/rx/client/trex_client.py
+-rw-r--r--   0        0        0     1603 2023-05-16 20:24:41.283538 run_rx-0.0.8/rx/client/user.py
+-rw-r--r--   0        0        0     5565 2023-06-07 13:22:07.723770 run_rx-0.0.8/rx/client/worker_client.py
+-rw-r--r--   0        0        0     6391 2023-06-06 22:54:37.232578 run_rx-0.0.8/rx/proto/rx_pb2.py
+-rw-r--r--   0        0        0     8466 2023-06-06 22:54:37.232746 run_rx-0.0.8/rx/proto/rx_pb2.pyi
+-rw-r--r--   0        0        0    12622 2023-06-06 22:54:37.233305 run_rx-0.0.8/rx/proto/rx_pb2_grpc.py
+-rw-r--r--   0        0        0     2597 1970-01-01 00:00:00.000000 run_rx-0.0.8/PKG-INFO
```

### Comparing `run_rx-0.0.7/LICENSE.txt` & `run_rx-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `run_rx-0.0.7/README.md` & `run_rx-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `run_rx-0.0.7/pyproject.toml` & `run_rx-0.0.8/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "run-rx"
-version = "0.0.7"
+version = "0.0.8"
 description = "A tool to simplify remote execution"
 authors = ["Kris Chodorow <k.chodorow@gmail.com>"]
 license = "LICENSE.txt"
 readme = "README.md"
 homepage = "https://www.run-rx.com"
 repository = "https://github.com/run-rx/rx"
 packages = [
```

### Comparing `run_rx-0.0.7/rx/client/commands/exec.py` & `run_rx-0.0.8/rx/client/commands/exec.py`

 * *Files identical despite different names*

### Comparing `run_rx-0.0.7/rx/client/configuration/config_base.py` & `run_rx-0.0.8/rx/client/configuration/config_base.py`

 * *Files identical despite different names*

### Comparing `run_rx-0.0.7/rx/client/configuration/local.py` & `run_rx-0.0.8/rx/client/configuration/local.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from absl import flags
 from absl import logging
 import sty
 
 from rx.client.configuration import config_base
 from rx.proto import rx_pb2
 
-VERSION = '0.0.7'
+VERSION = '0.0.8'
 
 IGNORE = pathlib.Path('.rxignore')
 
 _REMOTE = flags.DEFINE_string(
   'remote', None,
   'The path to the remote configuration file to use (see .rx/README.md).')
 _RSYNC_PATH = flags.DEFINE_string('rsync_path', None, 'Path to rsync binary')
```

### Comparing `run_rx-0.0.7/rx/client/configuration/remote.py` & `run_rx-0.0.8/rx/client/configuration/remote.py`

 * *Files identical despite different names*

### Comparing `run_rx-0.0.7/rx/client/login.py` & `run_rx-0.0.8/rx/client/login.py`

 * *Files 2% similar despite different names*

```diff
@@ -273,14 +273,20 @@
 
 
 def decode_id_token(b64: str) -> Dict[str, Any]:
   """The id_token field is a base64 encoded, .-delimited string."""
   return jwt.decode(b64, options={'verify_signature': False})
 
 
+def needs_login(rxroot: pathlib.Path) -> bool:
+  return not (
+    _get_access_token_file(rxroot).exists() and
+    _get_refresh_token_file(rxroot).exists())
+
+
 def _get_access_token_file(rxroot: pathlib.Path) -> pathlib.Path:
   return config_base.get_config_dir(rxroot) / 'user/access-token'
 
 
 def _get_refresh_token_file(rxroot: pathlib.Path) -> pathlib.Path:
   return config_base.get_config_dir(rxroot) / 'user/.refresh-token'
```

### Comparing `run_rx-0.0.7/rx/client/menu.py` & `run_rx-0.0.8/rx/client/menu.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,20 +7,26 @@
 2. Validate the response. If validation fails, go back to 1.
 """
 
 import pathlib
 from typing import Any, Callable, List, Optional
 
 
-def bool_prompt(prompt: str) -> bool:
-  response = input(f'{prompt} (y/n): ')
+def bool_prompt(prompt: str, default_opt: str = '') -> bool:
+  y = 'Y' if default_opt == 'y' else 'y'
+  n = 'N' if default_opt == 'n' else 'n'
+  response = input(f'{prompt} ({y}/{n}): ')
+  if not response:
+    response = default_opt
+  response = response.lower()
   if response == 'y':
     return True
   elif response == 'n':
     return False
+  print('Please choose "y" or "n".')
   return bool_prompt(prompt)
 
 
 def numbered_options_prompt(
     prompt: str, options: List[Any], default: int = 0) -> int:
   """Prompt with a numbered list of options."""
```

### Comparing `run_rx-0.0.7/rx/client/output_handler.py` & `run_rx-0.0.8/rx/client/output_handler.py`

 * *Files identical despite different names*

### Comparing `run_rx-0.0.7/rx/client/rsync.py` & `run_rx-0.0.8/rx/client/rsync.py`

 * *Files identical despite different names*

### Comparing `run_rx-0.0.7/rx/client/trex_client.py` & `run_rx-0.0.8/rx/client/trex_client.py`

 * *Files identical despite different names*

### Comparing `run_rx-0.0.7/rx/client/user.py` & `run_rx-0.0.8/rx/client/user.py`

 * *Files identical despite different names*

### Comparing `run_rx-0.0.7/rx/client/worker_client.py` & `run_rx-0.0.8/rx/client/worker_client.py`

 * *Files identical despite different names*

### Comparing `run_rx-0.0.7/rx/proto/rx_pb2.py` & `run_rx-0.0.8/rx/proto/rx_pb2.py`

 * *Files identical despite different names*

### Comparing `run_rx-0.0.7/rx/proto/rx_pb2.pyi` & `run_rx-0.0.8/rx/proto/rx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `run_rx-0.0.7/rx/proto/rx_pb2_grpc.py` & `run_rx-0.0.8/rx/proto/rx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `run_rx-0.0.7/PKG-INFO` & `run_rx-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: run-rx
-Version: 0.0.7
+Version: 0.0.8
 Summary: A tool to simplify remote execution
 Home-page: https://www.run-rx.com
 License: LICENSE.txt
 Author: Kris Chodorow
 Author-email: k.chodorow@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
```

