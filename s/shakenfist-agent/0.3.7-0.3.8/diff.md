# Comparing `tmp/shakenfist-agent-0.3.7.tar.gz` & `tmp/shakenfist-agent-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shakenfist-agent-0.3.7.tar", last modified: Wed May 31 09:12:07 2023, max compression
+gzip compressed data, was "shakenfist-agent-0.3.8.tar", last modified: Fri Jun  9 06:39:32 2023, max compression
```

## Comparing `shakenfist-agent-0.3.7.tar` & `shakenfist-agent-0.3.8.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-05-31 09:12:07.921237 shakenfist-agent-0.3.7/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      266 2023-03-06 10:11:43.000000 shakenfist-agent-0.3.7/.coveragerc
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-05-31 09:12:07.913236 shakenfist-agent-0.3.7/.github/
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-05-31 09:12:07.917236 shakenfist-agent-0.3.7/.github/workflows/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     1301 2023-03-06 10:11:43.000000 shakenfist-agent-0.3.7/.github/workflows/python-unit-tests.yml
--rw-rw-r--   0 parallels  (1000) parallels  (1000)       55 2022-03-31 06:16:40.000000 shakenfist-agent-0.3.7/.stestr.conf
--rw-rw-r--   0 parallels  (1000) parallels  (1000)       60 2023-05-31 09:12:07.000000 shakenfist-agent-0.3.7/AUTHORS
--rw-rw-r--   0 parallels  (1000) parallels  (1000)    11357 2022-03-16 08:23:02.000000 shakenfist-agent-0.3.7/LICENSE
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      907 2023-05-31 09:12:07.921237 shakenfist-agent-0.3.7/PKG-INFO
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      190 2022-03-16 08:23:02.000000 shakenfist-agent-0.3.7/README.md
--rwxrwxr-x   0 parallels  (1000) parallels  (1000)      857 2022-03-16 08:23:02.000000 shakenfist-agent-0.3.7/release.sh
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      249 2023-05-31 09:10:23.000000 shakenfist-agent-0.3.7/requirements.txt
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      729 2023-05-31 09:12:07.921237 shakenfist-agent-0.3.7/setup.cfg
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     1148 2022-03-16 08:23:02.000000 shakenfist-agent-0.3.7/setup.py
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-05-31 09:12:07.917236 shakenfist-agent-0.3.7/shakenfist_agent/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)        0 2022-03-16 08:23:02.000000 shakenfist-agent-0.3.7/shakenfist_agent/__init__.py
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-05-31 09:12:07.917236 shakenfist-agent-0.3.7/shakenfist_agent/commandline/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     8440 2023-05-31 09:10:23.000000 shakenfist-agent-0.3.7/shakenfist_agent/commandline/daemon.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      613 2022-08-07 23:05:27.000000 shakenfist-agent-0.3.7/shakenfist_agent/main.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     8638 2023-03-12 21:15:16.000000 shakenfist-agent-0.3.7/shakenfist_agent/protocol.py
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-05-31 09:12:07.917236 shakenfist-agent-0.3.7/shakenfist_agent/tests/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)        0 2022-03-31 06:16:40.000000 shakenfist-agent-0.3.7/shakenfist_agent/tests/__init__.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     4848 2023-03-08 21:01:13.000000 shakenfist-agent-0.3.7/shakenfist_agent/tests/test_daemon.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     3815 2023-03-06 10:12:52.000000 shakenfist-agent-0.3.7/shakenfist_agent/tests/test_protocol.py
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-05-31 09:12:07.917236 shakenfist-agent-0.3.7/shakenfist_agent.egg-info/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      907 2023-05-31 09:12:07.000000 shakenfist-agent-0.3.7/shakenfist_agent.egg-info/PKG-INFO
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      738 2023-05-31 09:12:07.000000 shakenfist-agent-0.3.7/shakenfist_agent.egg-info/SOURCES.txt
--rw-rw-r--   0 parallels  (1000) parallels  (1000)        1 2023-05-31 09:12:07.000000 shakenfist-agent-0.3.7/shakenfist_agent.egg-info/dependency_links.txt
--rw-rw-r--   0 parallels  (1000) parallels  (1000)       56 2023-05-31 09:12:07.000000 shakenfist-agent-0.3.7/shakenfist_agent.egg-info/entry_points.txt
--rw-rw-r--   0 parallels  (1000) parallels  (1000)        1 2023-05-31 09:12:07.000000 shakenfist-agent-0.3.7/shakenfist_agent.egg-info/not-zip-safe
--rw-rw-r--   0 parallels  (1000) parallels  (1000)       46 2023-05-31 09:12:07.000000 shakenfist-agent-0.3.7/shakenfist_agent.egg-info/pbr.json
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      101 2023-05-31 09:12:07.000000 shakenfist-agent-0.3.7/shakenfist_agent.egg-info/requires.txt
--rw-rw-r--   0 parallels  (1000) parallels  (1000)       17 2023-05-31 09:12:07.000000 shakenfist-agent-0.3.7/shakenfist_agent.egg-info/top_level.txt
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      164 2022-08-07 23:05:27.000000 shakenfist-agent-0.3.7/test-requirements.txt
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-05-31 09:12:07.917236 shakenfist-agent-0.3.7/tools/
--rwxrwxr-x   0 parallels  (1000) parallels  (1000)      573 2023-03-06 10:11:43.000000 shakenfist-agent-0.3.7/tools/flake8wrap.sh
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      867 2023-03-06 10:11:43.000000 shakenfist-agent-0.3.7/tox.ini
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-06-09 06:39:32.904024 shakenfist-agent-0.3.8/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      266 2023-03-06 10:11:43.000000 shakenfist-agent-0.3.8/.coveragerc
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-06-09 06:39:32.896024 shakenfist-agent-0.3.8/.github/
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-06-09 06:39:32.900024 shakenfist-agent-0.3.8/.github/workflows/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     1301 2023-03-06 10:11:43.000000 shakenfist-agent-0.3.8/.github/workflows/python-unit-tests.yml
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)       55 2022-03-31 06:16:40.000000 shakenfist-agent-0.3.8/.stestr.conf
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)       60 2023-06-09 06:39:32.000000 shakenfist-agent-0.3.8/AUTHORS
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)    11357 2022-03-16 08:23:02.000000 shakenfist-agent-0.3.8/LICENSE
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      907 2023-06-09 06:39:32.904024 shakenfist-agent-0.3.8/PKG-INFO
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      190 2022-03-16 08:23:02.000000 shakenfist-agent-0.3.8/README.md
+-rwxrwxr-x   0 parallels  (1000) parallels  (1000)      857 2022-03-16 08:23:02.000000 shakenfist-agent-0.3.8/release.sh
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      249 2023-05-31 09:10:23.000000 shakenfist-agent-0.3.8/requirements.txt
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      729 2023-06-09 06:39:32.904024 shakenfist-agent-0.3.8/setup.cfg
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     1148 2022-03-16 08:23:02.000000 shakenfist-agent-0.3.8/setup.py
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-06-09 06:39:32.900024 shakenfist-agent-0.3.8/shakenfist_agent/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)        0 2022-03-16 08:23:02.000000 shakenfist-agent-0.3.8/shakenfist_agent/__init__.py
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-06-09 06:39:32.904024 shakenfist-agent-0.3.8/shakenfist_agent/commandline/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     8562 2023-06-09 06:39:11.000000 shakenfist-agent-0.3.8/shakenfist_agent/commandline/daemon.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      613 2022-08-07 23:05:27.000000 shakenfist-agent-0.3.8/shakenfist_agent/main.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     8598 2023-06-09 06:39:11.000000 shakenfist-agent-0.3.8/shakenfist_agent/protocol.py
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-06-09 06:39:32.904024 shakenfist-agent-0.3.8/shakenfist_agent/tests/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)        0 2022-03-31 06:16:40.000000 shakenfist-agent-0.3.8/shakenfist_agent/tests/__init__.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     4848 2023-03-08 21:01:13.000000 shakenfist-agent-0.3.8/shakenfist_agent/tests/test_daemon.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     3815 2023-03-06 10:12:52.000000 shakenfist-agent-0.3.8/shakenfist_agent/tests/test_protocol.py
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-06-09 06:39:32.904024 shakenfist-agent-0.3.8/shakenfist_agent.egg-info/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      907 2023-06-09 06:39:32.000000 shakenfist-agent-0.3.8/shakenfist_agent.egg-info/PKG-INFO
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      738 2023-06-09 06:39:32.000000 shakenfist-agent-0.3.8/shakenfist_agent.egg-info/SOURCES.txt
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)        1 2023-06-09 06:39:32.000000 shakenfist-agent-0.3.8/shakenfist_agent.egg-info/dependency_links.txt
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)       56 2023-06-09 06:39:32.000000 shakenfist-agent-0.3.8/shakenfist_agent.egg-info/entry_points.txt
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)        1 2023-06-09 06:39:32.000000 shakenfist-agent-0.3.8/shakenfist_agent.egg-info/not-zip-safe
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)       46 2023-06-09 06:39:32.000000 shakenfist-agent-0.3.8/shakenfist_agent.egg-info/pbr.json
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      101 2023-06-09 06:39:32.000000 shakenfist-agent-0.3.8/shakenfist_agent.egg-info/requires.txt
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)       17 2023-06-09 06:39:32.000000 shakenfist-agent-0.3.8/shakenfist_agent.egg-info/top_level.txt
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      164 2022-08-07 23:05:27.000000 shakenfist-agent-0.3.8/test-requirements.txt
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-06-09 06:39:32.904024 shakenfist-agent-0.3.8/tools/
+-rwxrwxr-x   0 parallels  (1000) parallels  (1000)      573 2023-03-06 10:11:43.000000 shakenfist-agent-0.3.8/tools/flake8wrap.sh
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      867 2023-03-06 10:11:43.000000 shakenfist-agent-0.3.8/tox.ini
```

### Comparing `shakenfist-agent-0.3.7/.github/workflows/python-unit-tests.yml` & `shakenfist-agent-0.3.8/.github/workflows/python-unit-tests.yml`

 * *Files identical despite different names*

### Comparing `shakenfist-agent-0.3.7/LICENSE` & `shakenfist-agent-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `shakenfist-agent-0.3.7/PKG-INFO` & `shakenfist-agent-0.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shakenfist-agent
-Version: 0.3.7
+Version: 0.3.8
 Summary: An in-guest agent for instances running on Shaken Fist
 Home-page: https://madebymikal.com/shakenfist
 Author: Michael Still
 Author-email: mikal@stillhq.com
 License: Apache2
 Description: Python side channel agent for Shaken Fist
         =========================================
```

### Comparing `shakenfist-agent-0.3.7/release.sh` & `shakenfist-agent-0.3.8/release.sh`

 * *Files identical despite different names*

### Comparing `shakenfist-agent-0.3.7/setup.cfg` & `shakenfist-agent-0.3.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `shakenfist-agent-0.3.7/setup.py` & `shakenfist-agent-0.3.8/setup.py`

 * *Files identical despite different names*

### Comparing `shakenfist-agent-0.3.7/shakenfist_agent/commandline/daemon.py` & `shakenfist-agent-0.3.8/shakenfist_agent/commandline/daemon.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,15 @@
             'result': facts
         })
 
     def put_file_response(self, packet):
         path = packet['path']
         if path not in self.incomplete_file_puts:
             self.incomplete_file_puts[path] = {}
-            self.imcomplete_file_puts[path]['flo'] = open(path, 'wb')
+            self.incomplete_file_puts[path]['flo'] = open(path, 'wb')
 
         if 'chunk' not in packet:
             # A metadata packet
             self.incomplete_file_puts[path].update(packet['stat_result'])
             return
 
         if packet['chunk'] is None:
@@ -123,22 +123,26 @@
                  symbolicmode.symbolic_to_numeric_permissions(packet['mode']))
         self.send_packet({
             'command': 'chmod-response',
             'path': packet['path']
         })
 
     def chown(self, packet):
-        shutil.chown(packet['path'], user=packet.get('user'), group=packet.get('group'))
+        shutil.chown(packet.get('path'), user=packet.get('user'), group=packet.get('group'))
         self.send_packet({
             'command': 'chown-response',
             'path': packet['path']
         })
 
     def get_file(self, packet):
-        self._send_file('get-file', packet.get('path'))
+        path = packet.get('path')
+        error = self._path_is_a_file('get-file', path)
+        if error:
+            return
+        self._send_file('get-file', path, path)
 
     def watch_file(self, packet):
         path = packet.get('path')
         if not self._path_is_a_file('watch-file', path):
             return
 
         flo = open(path, 'rb')
```

### Comparing `shakenfist-agent-0.3.7/shakenfist_agent/main.py` & `shakenfist-agent-0.3.8/shakenfist_agent/main.py`

 * *Files identical despite different names*

### Comparing `shakenfist-agent-0.3.7/shakenfist_agent/protocol.py` & `shakenfist-agent-0.3.8/shakenfist_agent/protocol.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,15 +179,15 @@
 
     def send_pong(self, packet):
         self.send_packet({
             'command': 'pong',
             'unique': packet['unique']
         })
 
-    def _path_is_a_file(self, command, path, send_error_packets=True):
+    def _path_is_a_file(self, command, path):
         if not path:
             self.send_packet({
                 'command': '%s-response' % command,
                 'result': False,
                 'message': 'path is not set'
             })
             return 'path is not set'
@@ -208,54 +208,50 @@
                 'path': path,
                 'message': 'path is not a file'
             })
             return 'path is not a file'
 
         return None
 
-    def _send_file(self, command, path):
-        error = self._path_is_a_file(command, path)
-        if error:
-            return
-
-        st = os.stat(path, follow_symlinks=True)
+    def _send_file(self, command, source_path, destination_path):
+        st = os.stat(source_path, follow_symlinks=True)
         self.send_packet({
             'command': '%s-response' % command,
             'result': True,
-            'path': path,
+            'path': destination_path,
             'stat_result': {
                 'mode': st.st_mode,
                 'size': st.st_size,
                 'uid': st.st_uid,
                 'gid': st.st_gid,
                 'atime': st.st_atime,
                 'mtime': st.st_mtime,
                 'ctime': st.st_ctime
             }
         })
 
         offset = 0
-        with open(path, 'rb') as f:
+        with open(source_path, 'rb') as f:
             d = f.read(1024)
             while d:
                 self.send_packet({
                     'command': '%s-response' % command,
                     'result': True,
-                    'path': path,
+                    'path': destination_path,
                     'offset': offset,
                     'encoding': 'base64',
                     'chunk': base64.b64encode(d).decode('utf-8')
                 })
                 offset += len(d)
                 d = f.read(1024)
 
             self.send_packet({
                 'command': '%s-response' % command,
                 'result': True,
-                'path': path,
+                'path': destination_path,
                 'offset': offset,
                 'encoding': 'base64',
                 'chunk': None
             })
 
 
 class SocketAgent(Agent):
```

### Comparing `shakenfist-agent-0.3.7/shakenfist_agent/tests/test_daemon.py` & `shakenfist-agent-0.3.8/shakenfist_agent/tests/test_daemon.py`

 * *Files identical despite different names*

### Comparing `shakenfist-agent-0.3.7/shakenfist_agent/tests/test_protocol.py` & `shakenfist-agent-0.3.8/shakenfist_agent/tests/test_protocol.py`

 * *Files identical despite different names*

### Comparing `shakenfist-agent-0.3.7/shakenfist_agent.egg-info/PKG-INFO` & `shakenfist-agent-0.3.8/shakenfist_agent.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shakenfist-agent
-Version: 0.3.7
+Version: 0.3.8
 Summary: An in-guest agent for instances running on Shaken Fist
 Home-page: https://madebymikal.com/shakenfist
 Author: Michael Still
 Author-email: mikal@stillhq.com
 License: Apache2
 Description: Python side channel agent for Shaken Fist
         =========================================
```

### Comparing `shakenfist-agent-0.3.7/shakenfist_agent.egg-info/SOURCES.txt` & `shakenfist-agent-0.3.8/shakenfist_agent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shakenfist-agent-0.3.7/tools/flake8wrap.sh` & `shakenfist-agent-0.3.8/tools/flake8wrap.sh`

 * *Files identical despite different names*

### Comparing `shakenfist-agent-0.3.7/tox.ini` & `shakenfist-agent-0.3.8/tox.ini`

 * *Files identical despite different names*

