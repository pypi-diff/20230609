# Comparing `tmp/fdserver-23.5.30.tar.gz` & `tmp/fdserver-23.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fdserver-23.5.30.tar", last modified: Tue May 30 16:10:27 2023, max compression
+gzip compressed data, was "fdserver-23.6.9.tar", last modified: Fri Jun  9 20:24:51 2023, max compression
```

## Comparing `fdserver-23.5.30.tar` & `fdserver-23.6.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-30 16:10:27.029061 fdserver-23.5.30/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     7652 2022-06-28 19:46:07.000000 fdserver-23.5.30/LICENSE.md
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4186 2023-05-30 16:10:27.028061 fdserver-23.5.30/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3406 2023-05-30 16:06:27.000000 fdserver-23.5.30/README.md
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-30 16:10:27.026061 fdserver-23.5.30/fdserver/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2022-12-28 15:00:34.000000 fdserver-23.5.30/fdserver/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    33920 2023-02-07 19:28:09.000000 fdserver-23.5.30/fdserver/__main__.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-30 16:10:27.028061 fdserver-23.5.30/fdserver/data/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5445 2023-02-01 20:40:07.000000 fdserver-23.5.30/fdserver/data/k6gte-fdserver-128.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1271 2023-02-01 20:38:54.000000 fdserver-23.5.30/fdserver/data/k6gte-fdserver-32.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2649 2023-02-01 20:39:12.000000 fdserver-23.5.30/fdserver/data/k6gte-fdserver-64.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      302 2023-02-01 20:41:35.000000 fdserver-23.5.30/fdserver/data/k6gte-fdserver.desktop
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13503 2023-02-01 20:40:13.000000 fdserver-23.5.30/fdserver/data/k6gte.fdserver.svg
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1216 2023-05-30 16:06:27.000000 fdserver-23.5.30/fdserver/data/server_preferences.json
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-30 16:10:27.028061 fdserver-23.5.30/fdserver/lib/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2022-12-28 15:01:16.000000 fdserver-23.5.30/fdserver/lib/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11955 2023-02-01 14:55:26.000000 fdserver-23.5.30/fdserver/lib/server_database.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       47 2023-05-30 16:06:27.000000 fdserver-23.5.30/fdserver/lib/version.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1289 2022-12-28 03:38:12.000000 fdserver-23.5.30/fdserver/lib/versiontest.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-30 16:10:27.027061 fdserver-23.5.30/fdserver.egg-info/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4186 2023-05-30 16:10:27.000000 fdserver-23.5.30/fdserver.egg-info/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      566 2023-05-30 16:10:27.000000 fdserver-23.5.30/fdserver.egg-info/SOURCES.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2023-05-30 16:10:27.000000 fdserver-23.5.30/fdserver.egg-info/dependency_links.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       51 2023-05-30 16:10:27.000000 fdserver-23.5.30/fdserver.egg-info/entry_points.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       19 2023-05-30 16:10:27.000000 fdserver-23.5.30/fdserver.egg-info/top_level.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1000 2023-05-30 16:06:27.000000 fdserver-23.5.30/pyproject.toml
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2023-05-30 16:10:27.029061 fdserver-23.5.30/setup.cfg
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-09 20:24:51.863779 fdserver-23.6.9/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     7652 2022-06-28 19:46:07.000000 fdserver-23.6.9/LICENSE.md
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4262 2023-06-09 20:24:51.862779 fdserver-23.6.9/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3483 2023-06-09 20:22:41.000000 fdserver-23.6.9/README.md
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-09 20:24:51.860779 fdserver-23.6.9/fdserver/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2022-12-28 15:00:34.000000 fdserver-23.6.9/fdserver/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    34719 2023-06-09 18:52:22.000000 fdserver-23.6.9/fdserver/__main__.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-09 20:24:51.861779 fdserver-23.6.9/fdserver/data/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5445 2023-02-01 20:40:07.000000 fdserver-23.6.9/fdserver/data/k6gte-fdserver-128.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1271 2023-02-01 20:38:54.000000 fdserver-23.6.9/fdserver/data/k6gte-fdserver-32.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2649 2023-02-01 20:39:12.000000 fdserver-23.6.9/fdserver/data/k6gte-fdserver-64.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      302 2023-02-01 20:41:35.000000 fdserver-23.6.9/fdserver/data/k6gte-fdserver.desktop
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13503 2023-02-01 20:40:13.000000 fdserver-23.6.9/fdserver/data/k6gte.fdserver.svg
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1216 2023-05-30 16:06:27.000000 fdserver-23.6.9/fdserver/data/server_preferences.json
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-09 20:24:51.862779 fdserver-23.6.9/fdserver/lib/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2022-12-28 15:01:16.000000 fdserver-23.6.9/fdserver/lib/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12382 2023-06-09 19:06:47.000000 fdserver-23.6.9/fdserver/lib/server_database.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       46 2023-06-09 20:20:22.000000 fdserver-23.6.9/fdserver/lib/version.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1289 2022-12-28 03:38:12.000000 fdserver-23.6.9/fdserver/lib/versiontest.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-09 20:24:51.861779 fdserver-23.6.9/fdserver.egg-info/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4262 2023-06-09 20:24:51.000000 fdserver-23.6.9/fdserver.egg-info/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      566 2023-06-09 20:24:51.000000 fdserver-23.6.9/fdserver.egg-info/SOURCES.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2023-06-09 20:24:51.000000 fdserver-23.6.9/fdserver.egg-info/dependency_links.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       51 2023-06-09 20:24:51.000000 fdserver-23.6.9/fdserver.egg-info/entry_points.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       19 2023-06-09 20:24:51.000000 fdserver-23.6.9/fdserver.egg-info/top_level.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      999 2023-06-09 20:20:38.000000 fdserver-23.6.9/pyproject.toml
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2023-06-09 20:24:51.863779 fdserver-23.6.9/setup.cfg
```

### Comparing `fdserver-23.5.30/LICENSE.md` & `fdserver-23.6.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fdserver-23.5.30/PKG-INFO` & `fdserver-23.6.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fdserver
-Version: 23.5.30
+Version: 23.6.9
 Summary: Field Day group logging server
 Author-email: Michael Bridak <michael.bridak@gmail.com>
 Project-URL: Homepage, https://github.com/mbridak/fdserver
 Project-URL: Bug Tracker, https://github.com/mbridak/fdserver/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -51,15 +51,22 @@
 ## Screenshot
 
 ![main display](https://github.com/mbridak/fdserver/raw/master/pics/server_pic.png)
 
 ## Installation
 
 ```bash
+# install
 pip install fdserver
+
+# update
+pip install -U fdserver
+
+# remove
+pip uninstall fdserver
 ```
 
 ```text
 usage: fdserver [-h] [-l]
 
 Field Day aggregation server.
```

### Comparing `fdserver-23.5.30/README.md` & `fdserver-23.6.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,22 @@
 ## Screenshot
 
 ![main display](https://github.com/mbridak/fdserver/raw/master/pics/server_pic.png)
 
 ## Installation
 
 ```bash
+# install
 pip install fdserver
+
+# update
+pip install -U fdserver
+
+# remove
+pip uninstall fdserver
 ```
 
 ```text
 usage: fdserver [-h] [-l]
 
 Field Day aggregation server.
```

### Comparing `fdserver-23.5.30/fdserver/__main__.py` & `fdserver-23.6.9/fdserver/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -710,15 +710,14 @@
             except JSONDecodeError as err:
                 the_error = f"Not JSON: {err}\n{payload}\n"
                 logging.debug(the_error)
                 continue
             logging.debug("%s", json_data)
             timestamp = strftime("%H:%M:%S", gmtime())
             if json_data.get("cmd") == "POST":
-
                 DB.log_contact(
                     (
                         json_data.get("unique_id"),
                         json_data.get("hiscall"),
                         json_data.get("class"),
                         json_data.get("section"),
                         json_data.get("date_and_time"),
@@ -764,14 +763,30 @@
                 continue
 
             if json_data.get("cmd") == "GET":
                 LOG.add_item(f"[{timestamp}] {json_data}")
                 comm_log()
                 continue
 
+            if json_data.get("cmd") == "DUPE":
+                LOG.add_item(f"[{timestamp}] Checking Dupe: {json_data.get('contact')}")
+                packet = {"cmd": "RESPONSE"}
+                packet["recipient"] = json_data.get("station")
+                packet["subject"] = "DUPE"
+                packet["contact"] = json_data.get("contact")
+                _call = json_data.get("contact")
+                _mode = json_data.get("mode")
+                _band = json_data.get("band")
+                the_count = DB.get_dupe_status(_call, _band, _mode)
+                packet["isdupe"] = the_count
+                bytes_to_send = bytes(dumps(packet), encoding="ascii")
+                s.sendto(bytes_to_send, (MULTICAST_GROUP, MULTICAST_PORT))
+                comm_log()
+                continue
+
             if json_data.get("cmd") == "DELETE":
                 LOG.add_item(f"[{timestamp}] Deleting: {json_data.get('unique_id')}")
                 DB.delete_contact(json_data.get("unique_id"))
                 comm_log()
                 packet = {"cmd": "RESPONSE"}
                 packet["recipient"] = json_data.get("station")
                 packet["subject"] = "DELETE"
@@ -845,15 +860,14 @@
                 s.sendto(bytes_to_send, (MULTICAST_GROUP, MULTICAST_PORT))
                 LOG.add_item(f"[{timestamp}] GROUPQUERY: {json_data.get('station')}")
                 comm_log()
                 continue
 
             if json_data.get("cmd") == "CHAT":
                 if "@stats" in json_data.get("message"):
-
                     bands = ["160", "80", "40", "20", "15", "10", "6", "2"]
                     blist = []
                     list_o_bands = DB.get_bands()
                     if list_o_bands:
                         for count in list_o_bands:
                             blist.append(count[0])
```

### Comparing `fdserver-23.5.30/fdserver/data/k6gte-fdserver-128.png` & `fdserver-23.6.9/fdserver/data/k6gte-fdserver-128.png`

 * *Files identical despite different names*

### Comparing `fdserver-23.5.30/fdserver/data/k6gte-fdserver-32.png` & `fdserver-23.6.9/fdserver/data/k6gte-fdserver-32.png`

 * *Files identical despite different names*

### Comparing `fdserver-23.5.30/fdserver/data/k6gte-fdserver-64.png` & `fdserver-23.6.9/fdserver/data/k6gte-fdserver-64.png`

 * *Files identical despite different names*

### Comparing `fdserver-23.5.30/fdserver/data/k6gte.fdserver.svg` & `fdserver-23.6.9/fdserver/data/k6gte.fdserver.svg`

 * *Files identical despite different names*

### Comparing `fdserver-23.5.30/fdserver/data/server_preferences.json` & `fdserver-23.6.9/fdserver/data/server_preferences.json`

 * *Files identical despite different names*

### Comparing `fdserver-23.5.30/fdserver/lib/server_database.py` & `fdserver-23.6.9/fdserver/lib/server_database.py`

 * *Files 1% similar despite different names*

```diff
@@ -283,7 +283,17 @@
 
     def get_grids(self) -> tuple:
         """returns a tuple of unique grids in the log."""
         with sqlite3.connect(self.database) as conn:
             cursor = conn.cursor()
             cursor.execute("select DISTINCT grid from contacts")
             return cursor.fetchall()
+
+    def get_dupe_status(self, call, band, mode):
+        """See is call exists on band/mode return bool"""
+        with sqlite3.connect(self.database) as conn:
+            cursor = conn.cursor()
+            cursor.execute(
+                f"select count(*) as dupecount from contacts where "
+                f"callsign = '{call}' AND band = '{band}' AND mode = '{mode}';"
+            )
+            return cursor.fetchone()[0]
```

### Comparing `fdserver-23.5.30/fdserver/lib/versiontest.py` & `fdserver-23.6.9/fdserver/lib/versiontest.py`

 * *Files identical despite different names*

### Comparing `fdserver-23.5.30/fdserver.egg-info/PKG-INFO` & `fdserver-23.6.9/fdserver.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fdserver
-Version: 23.5.30
+Version: 23.6.9
 Summary: Field Day group logging server
 Author-email: Michael Bridak <michael.bridak@gmail.com>
 Project-URL: Homepage, https://github.com/mbridak/fdserver
 Project-URL: Bug Tracker, https://github.com/mbridak/fdserver/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -51,15 +51,22 @@
 ## Screenshot
 
 ![main display](https://github.com/mbridak/fdserver/raw/master/pics/server_pic.png)
 
 ## Installation
 
 ```bash
+# install
 pip install fdserver
+
+# update
+pip install -U fdserver
+
+# remove
+pip uninstall fdserver
 ```
 
 ```text
 usage: fdserver [-h] [-l]
 
 Field Day aggregation server.
```

### Comparing `fdserver-23.5.30/fdserver.egg-info/SOURCES.txt` & `fdserver-23.6.9/fdserver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fdserver-23.5.30/pyproject.toml` & `fdserver-23.6.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fdserver" 
-version = "23.5.30"
+version = "23.6.9"
 description = "Field Day group logging server"
 readme = "README.md"
 requires-python = ">=3.9"
 authors = [
   { name="Michael Bridak", email="michael.bridak@gmail.com" },
 ]
 dependencies = [
```

