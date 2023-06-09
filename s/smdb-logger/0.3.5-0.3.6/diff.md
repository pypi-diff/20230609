# Comparing `tmp/smdb_logger-0.3.5.tar.gz` & `tmp/smdb_logger-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smdb_logger-0.3.5.tar", last modified: Thu Apr 13 12:11:25 2023, max compression
+gzip compressed data, was "smdb_logger-0.3.6.tar", last modified: Fri Jun  9 14:39:34 2023, max compression
```

## Comparing `smdb_logger-0.3.5.tar` & `smdb_logger-0.3.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 12:11:25.688798 smdb_logger-0.3.5/
--rw-rw-rw-   0        0        0     4178 2023-04-13 12:11:25.688798 smdb_logger-0.3.5/PKG-INFO
--rw-rw-rw-   0        0        0     3569 2022-07-15 12:30:38.000000 smdb_logger-0.3.5/README.md
--rw-rw-rw-   0        0        0      108 2021-03-04 15:16:38.000000 smdb_logger-0.3.5/pyproject.toml
--rw-rw-rw-   0        0        0      694 2023-04-13 12:11:25.693300 smdb_logger-0.3.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-13 12:11:25.680797 smdb_logger-0.3.5/smdb_logger/
--rw-rw-rw-   0        0        0    10205 2023-04-13 12:10:50.000000 smdb_logger-0.3.5/smdb_logger/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:11:25.688299 smdb_logger-0.3.5/smdb_logger.egg-info/
--rw-rw-rw-   0        0        0     4178 2023-04-13 12:11:25.000000 smdb_logger-0.3.5/smdb_logger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      198 2023-04-13 12:11:25.000000 smdb_logger-0.3.5/smdb_logger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 12:11:25.000000 smdb_logger-0.3.5/smdb_logger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-04-13 12:11:25.000000 smdb_logger-0.3.5/smdb_logger.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 14:39:34.735614 smdb_logger-0.3.6/
+-rw-rw-rw-   0        0        0     4178 2023-06-09 14:39:34.735614 smdb_logger-0.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3569 2022-07-15 12:30:38.000000 smdb_logger-0.3.6/README.md
+-rw-rw-rw-   0        0        0      108 2021-03-04 15:16:38.000000 smdb_logger-0.3.6/pyproject.toml
+-rw-rw-rw-   0        0        0      694 2023-06-09 14:39:34.739615 smdb_logger-0.3.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-09 14:39:34.725612 smdb_logger-0.3.6/smdb_logger/
+-rw-rw-rw-   0        0        0    10191 2023-06-09 14:38:31.000000 smdb_logger-0.3.6/smdb_logger/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 14:39:34.735114 smdb_logger-0.3.6/smdb_logger.egg-info/
+-rw-rw-rw-   0        0        0     4178 2023-06-09 14:39:34.000000 smdb_logger-0.3.6/smdb_logger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      198 2023-06-09 14:39:34.000000 smdb_logger-0.3.6/smdb_logger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 14:39:34.000000 smdb_logger-0.3.6/smdb_logger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-06-09 14:39:34.000000 smdb_logger-0.3.6/smdb_logger.egg-info/top_level.txt
```

### Comparing `smdb_logger-0.3.5/PKG-INFO` & `smdb_logger-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smdb_logger
-Version: 0.3.5
+Version: 0.3.6
 Summary: Logger used by Server Monitoring Discord Bot and all extentions made by me
 Home-page: https://github.com/NightKey/Server-monitoring-discord-bot
 Author: Janthó Dávid
 Author-email: davidjantho@gmail.com
 Project-URL: Bug Tracker, https://github.com/NightKey/Server-monitoring-discord-bot/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `smdb_logger-0.3.5/README.md` & `smdb_logger-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `smdb_logger-0.3.5/setup.cfg` & `smdb_logger-0.3.6/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2073 6d64 625f 6c6f 6767 6572 0d0a   = smdb_logger..
-00000020: 7665 7273 696f 6e20 3d20 302e 332e 350d  version = 0.3.5.
+00000020: 7665 7273 696f 6e20 3d20 302e 332e 360d  version = 0.3.6.
 00000030: 0a61 7574 686f 7220 3d20 4a61 6e74 68c3  .author = Janth.
 00000040: b320 44c3 a176 6964 0d0a 6175 7468 6f72  . D..vid..author
 00000050: 5f65 6d61 696c 203d 2064 6176 6964 6a61  _email = davidja
 00000060: 6e74 686f 4067 6d61 696c 2e63 6f6d 0d0a  ntho@gmail.com..
 00000070: 6465 7363 7269 7074 696f 6e20 3d20 4c6f  description = Lo
 00000080: 6767 6572 2075 7365 6420 6279 2053 6572  gger used by Ser
 00000090: 7665 7220 4d6f 6e69 746f 7269 6e67 2044  ver Monitoring D
```

### Comparing `smdb_logger-0.3.5/smdb_logger/__init__.py` & `smdb_logger-0.3.6/smdb_logger/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
         if timestamp is None:
             timestamp = time()
         return datetime.fromtimestamp(timestamp)
 
     def __check_logfile(self) -> None:
         if self.max_logfile_size != -1 and path.exists(path.join(self.log_folder, self.log_file)) and (path.getsize(path.join(self.log_folder, self.log_file)) / (1024 ^ 2)) > self.max_logfile_size:
             tmp = self.log_file.split(".")
-            tmp[0] += str(self.get_date().strftime(format_string=r"%y.%m.%d-%I"))
+            tmp[0] += str(self.get_date().strftime(r"%y.%m.%d-%I"))
             new_name = ".".join(tmp)
             rename(path.join(self.log_folder, self.log_file),
                    path.join(self.log_folder, new_name))
             with open(path.join(self.log_folder, self.log_file), "w") as f:
                 pass
 
         if self.max_logfile_lifetime != -1:
```

### Comparing `smdb_logger-0.3.5/smdb_logger.egg-info/PKG-INFO` & `smdb_logger-0.3.6/smdb_logger.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smdb-logger
-Version: 0.3.5
+Version: 0.3.6
 Summary: Logger used by Server Monitoring Discord Bot and all extentions made by me
 Home-page: https://github.com/NightKey/Server-monitoring-discord-bot
 Author: Janthó Dávid
 Author-email: davidjantho@gmail.com
 Project-URL: Bug Tracker, https://github.com/NightKey/Server-monitoring-discord-bot/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

