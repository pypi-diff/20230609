# Comparing `tmp/turbo-tunnel-0.9.1.tar.gz` & `tmp/turbo-tunnel-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turbo-tunnel-0.9.1.tar", last modified: Mon Sep  6 23:48:36 2021, max compression
+gzip compressed data, was "turbo-tunnel-0.9.2.tar", last modified: Sat Sep 18 15:45:03 2021, max compression
```

## Comparing `turbo-tunnel-0.9.1.tar` & `turbo-tunnel-0.9.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-06 23:48:36.152757 turbo-tunnel-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (121)       13 2021-09-06 23:48:26.000000 turbo-tunnel-0.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     8030 2021-09-06 23:48:36.152757 turbo-tunnel-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5746 2021-09-06 23:48:26.000000 turbo-tunnel-0.9.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       10 2021-09-06 23:48:26.000000 turbo-tunnel-0.9.1/extra_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       75 2021-09-06 23:48:26.000000 turbo-tunnel-0.9.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-09-06 23:48:36.152757 turbo-tunnel-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1885 2021-09-06 23:48:26.000000 turbo-tunnel-0.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-06 23:48:36.148757 turbo-tunnel-0.9.1/turbo_tunnel/
--rw-r--r--   0 runner    (1001) docker     (121)      368 2021-09-06 23:48:26.000000 turbo-tunnel-0.9.1/turbo_tunnel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4305 2021-09-06 23:48:26.000000 turbo-tunnel-0.9.1/turbo_tunnel/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)      191 2021-09-06 23:48:26.000000 turbo-tunnel-0.9.1/turbo_tunnel/auth.py
--rw-r--r--   0 runner    (1001) docker     (121)     6758 2021-09-06 23:48:26.000000 turbo-tunnel-0.9.1/turbo_tunnel/chain.py
--rw-r--r--   0 runner    (1001) docker     (121)     6558 2021-09-06 23:48:26.000000 turbo-tunnel-0.9.1/turbo_tunnel/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)    15678 2021-09-06 23:48:26.000000 turbo-tunnel-0.9.1/turbo_tunnel/https.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-06 23:48:36.152757 turbo-tunnel-0.9.1/turbo_tunnel/plugins/
--rw-r--r--   0 runner    (1001) docker     (121)      550 2021-09-06 23:48:26.000000 turbo-tunnel-0.9.1/turbo_tunnel/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9370 2021-09-06 23:48:26.000000 turbo-tunnel-0.9.1/turbo_tunnel/plugins/terminal.py
--rw-r--r--   0 runner    (1001) docker     (121)     1440 2021-09-06 23:48:26.000000 turbo-tunnel-0.9.1/turbo_tunnel/registry.py
--rw-r--r--   0 runner    (1001) docker     (121)      623 2021-09-06 23:48:26.000000 turbo-tunnel-0.9.1/turbo_tunnel/route.py
--rw-r--r--   0 runner    (1001) docker     (121)     8868 2021-09-06 23:48:26.000000 turbo-tunnel-0.9.1/turbo_tunnel/server.py
--rw-r--r--   0 runner    (1001) docker     (121)     5178 2021-09-06 23:48:26.000000 turbo-tunnel-0.9.1/turbo_tunnel/socks.py
--rw-r--r--   0 runner    (1001) docker     (121)    18079 2021-09-06 23:48:26.000000 turbo-tunnel-0.9.1/turbo_tunnel/ssh.py
--rw-r--r--   0 runner    (1001) docker     (121)    18831 2021-09-06 23:48:26.000000 turbo-tunnel-0.9.1/turbo_tunnel/tunnel.py
--rw-r--r--   0 runner    (1001) docker     (121)    11037 2021-09-06 23:48:26.000000 turbo-tunnel-0.9.1/turbo_tunnel/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    11967 2021-09-06 23:48:26.000000 turbo-tunnel-0.9.1/turbo_tunnel/websocket.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-06 23:48:36.152757 turbo-tunnel-0.9.1/turbo_tunnel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8030 2021-09-06 23:48:35.000000 turbo-tunnel-0.9.1/turbo_tunnel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      673 2021-09-06 23:48:36.000000 turbo-tunnel-0.9.1/turbo_tunnel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-06 23:48:35.000000 turbo-tunnel-0.9.1/turbo_tunnel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       61 2021-09-06 23:48:35.000000 turbo-tunnel-0.9.1/turbo_tunnel.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       92 2021-09-06 23:48:35.000000 turbo-tunnel-0.9.1/turbo_tunnel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2021-09-06 23:48:35.000000 turbo-tunnel-0.9.1/turbo_tunnel.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-18 15:45:03.658047 turbo-tunnel-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2021-09-18 15:44:54.000000 turbo-tunnel-0.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     6539 2021-09-18 15:45:03.658047 turbo-tunnel-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     5746 2021-09-18 15:44:54.000000 turbo-tunnel-0.9.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       10 2021-09-18 15:44:54.000000 turbo-tunnel-0.9.2/extra_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       75 2021-09-18 15:44:54.000000 turbo-tunnel-0.9.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-09-18 15:45:03.658047 turbo-tunnel-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1885 2021-09-18 15:44:54.000000 turbo-tunnel-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-18 15:45:03.654047 turbo-tunnel-0.9.2/turbo_tunnel/
+-rw-r--r--   0 runner    (1001) docker     (121)      368 2021-09-18 15:44:54.000000 turbo-tunnel-0.9.2/turbo_tunnel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4305 2021-09-18 15:44:54.000000 turbo-tunnel-0.9.2/turbo_tunnel/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      191 2021-09-18 15:44:54.000000 turbo-tunnel-0.9.2/turbo_tunnel/auth.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6758 2021-09-18 15:44:54.000000 turbo-tunnel-0.9.2/turbo_tunnel/chain.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6558 2021-09-18 15:44:54.000000 turbo-tunnel-0.9.2/turbo_tunnel/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15678 2021-09-18 15:44:54.000000 turbo-tunnel-0.9.2/turbo_tunnel/https.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-18 15:45:03.658047 turbo-tunnel-0.9.2/turbo_tunnel/plugins/
+-rw-r--r--   0 runner    (1001) docker     (121)      550 2021-09-18 15:44:54.000000 turbo-tunnel-0.9.2/turbo_tunnel/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9370 2021-09-18 15:44:54.000000 turbo-tunnel-0.9.2/turbo_tunnel/plugins/terminal.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1440 2021-09-18 15:44:54.000000 turbo-tunnel-0.9.2/turbo_tunnel/registry.py
+-rw-r--r--   0 runner    (1001) docker     (121)      623 2021-09-18 15:44:54.000000 turbo-tunnel-0.9.2/turbo_tunnel/route.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8868 2021-09-18 15:44:54.000000 turbo-tunnel-0.9.2/turbo_tunnel/server.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5178 2021-09-18 15:44:54.000000 turbo-tunnel-0.9.2/turbo_tunnel/socks.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18438 2021-09-18 15:44:54.000000 turbo-tunnel-0.9.2/turbo_tunnel/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18831 2021-09-18 15:44:54.000000 turbo-tunnel-0.9.2/turbo_tunnel/tunnel.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11037 2021-09-18 15:44:54.000000 turbo-tunnel-0.9.2/turbo_tunnel/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11967 2021-09-18 15:44:54.000000 turbo-tunnel-0.9.2/turbo_tunnel/websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-18 15:45:03.654047 turbo-tunnel-0.9.2/turbo_tunnel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     6539 2021-09-18 15:45:03.000000 turbo-tunnel-0.9.2/turbo_tunnel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      673 2021-09-18 15:45:03.000000 turbo-tunnel-0.9.2/turbo_tunnel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-18 15:45:03.000000 turbo-tunnel-0.9.2/turbo_tunnel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       61 2021-09-18 15:45:03.000000 turbo-tunnel-0.9.2/turbo_tunnel.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       92 2021-09-18 15:45:03.000000 turbo-tunnel-0.9.2/turbo_tunnel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2021-09-18 15:45:03.000000 turbo-tunnel-0.9.2/turbo_tunnel.egg-info/top_level.txt
```

### Comparing `turbo-tunnel-0.9.1/README.md` & `turbo-tunnel-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `turbo-tunnel-0.9.1/setup.py` & `turbo-tunnel-0.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `turbo-tunnel-0.9.1/turbo_tunnel/__main__.py` & `turbo-tunnel-0.9.2/turbo_tunnel/__main__.py`

 * *Files identical despite different names*

### Comparing `turbo-tunnel-0.9.1/turbo_tunnel/chain.py` & `turbo-tunnel-0.9.2/turbo_tunnel/chain.py`

 * *Files identical despite different names*

### Comparing `turbo-tunnel-0.9.1/turbo_tunnel/conf.py` & `turbo-tunnel-0.9.2/turbo_tunnel/conf.py`

 * *Files identical despite different names*

### Comparing `turbo-tunnel-0.9.1/turbo_tunnel/https.py` & `turbo-tunnel-0.9.2/turbo_tunnel/https.py`

 * *Files identical despite different names*

### Comparing `turbo-tunnel-0.9.1/turbo_tunnel/plugins/__init__.py` & `turbo-tunnel-0.9.2/turbo_tunnel/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `turbo-tunnel-0.9.1/turbo_tunnel/plugins/terminal.py` & `turbo-tunnel-0.9.2/turbo_tunnel/plugins/terminal.py`

 * *Files identical despite different names*

### Comparing `turbo-tunnel-0.9.1/turbo_tunnel/registry.py` & `turbo-tunnel-0.9.2/turbo_tunnel/registry.py`

 * *Files identical despite different names*

### Comparing `turbo-tunnel-0.9.1/turbo_tunnel/route.py` & `turbo-tunnel-0.9.2/turbo_tunnel/route.py`

 * *Files identical despite different names*

### Comparing `turbo-tunnel-0.9.1/turbo_tunnel/server.py` & `turbo-tunnel-0.9.2/turbo_tunnel/server.py`

 * *Files identical despite different names*

### Comparing `turbo-tunnel-0.9.1/turbo_tunnel/socks.py` & `turbo-tunnel-0.9.2/turbo_tunnel/socks.py`

 * *Files identical despite different names*

### Comparing `turbo-tunnel-0.9.1/turbo_tunnel/ssh.py` & `turbo-tunnel-0.9.2/turbo_tunnel/ssh.py`

 * *Files 1% similar despite different names*

```diff
@@ -381,33 +381,41 @@
                 utils.logger.error(
                     "[%s] Connect ssh server %s:%d auth failed: %s"
                     % (self.__class__.__name__, self._url.host, self._url.port, e)
                 )
                 ssh_conn.abort()
                 await ssh_conn.wait_closed()
                 return None
+            else:
+                ssh_conn.set_keepalive(10)
             self.__class__.ssh_conns[key] = ssh_conn
         return self.__class__.ssh_conns[key]
 
     async def connect(self):
         ssh_conn = await self.create_ssh_conn()
         if not ssh_conn:
             return False
-
         try:
-            self._reader, self._writer = await ssh_conn.open_connection(
-                self._addr, self._port
+            self._reader, self._writer = await asyncio.wait_for(
+                ssh_conn.open_connection(self._addr, self._port), self.__class__.timeout
             )
         except asyncssh.ChannelOpenError as e:
             utils.logger.warn(
                 "[%s] Connect %s:%d over %s failed: %s"
                 % (self.__class__.__name__, self._addr, self._port, self._url, e)
             )
             return False
-        return True
+        except asyncio.TimeoutError:
+            utils.logger.warn(
+                "[%s] Connect %s:%d over %s timeout"
+                % (self.__class__.__name__, self._addr, self._port, self._url)
+            )
+            return False
+        else:
+            return True
 
     async def read(self):
         if self._reader:
             buffer = await self._reader.read(4096)
             if buffer:
                 return buffer
         raise utils.TunnelClosedError()
```

### Comparing `turbo-tunnel-0.9.1/turbo_tunnel/tunnel.py` & `turbo-tunnel-0.9.2/turbo_tunnel/tunnel.py`

 * *Files identical despite different names*

### Comparing `turbo-tunnel-0.9.1/turbo_tunnel/utils.py` & `turbo-tunnel-0.9.2/turbo_tunnel/utils.py`

 * *Files identical despite different names*

### Comparing `turbo-tunnel-0.9.1/turbo_tunnel/websocket.py` & `turbo-tunnel-0.9.2/turbo_tunnel/websocket.py`

 * *Files identical despite different names*

### Comparing `turbo-tunnel-0.9.1/turbo_tunnel.egg-info/SOURCES.txt` & `turbo-tunnel-0.9.2/turbo_tunnel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

