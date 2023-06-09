# Comparing `tmp/yirgachefe-0.1.5.tar.gz` & `tmp/yirgachefe-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/yirgachefe-0.1.5.tar", last modified: Tue Oct 18 06:05:29 2022, max compression
+gzip compressed data, was "yirgachefe-0.1.6.tar", last modified: Fri Jun  9 02:52:57 2023, max compression
```

## Comparing `yirgachefe-0.1.5.tar` & `yirgachefe-0.1.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 winDy      (501) staff       (20)        0 2022-10-18 06:05:29.000000 yirgachefe-0.1.5/
--rw-r--r--   0 winDy      (501) staff       (20)    11346 2022-03-31 05:07:27.000000 yirgachefe-0.1.5/LICENSE
--rw-r--r--   0 winDy      (501) staff       (20)     2183 2022-10-18 06:05:29.000000 yirgachefe-0.1.5/PKG-INFO
--rw-r--r--   0 winDy      (501) staff       (20)     1826 2022-03-31 05:25:34.000000 yirgachefe-0.1.5/README.md
--rw-r--r--   0 winDy      (501) staff       (20)      117 2022-10-18 06:05:29.000000 yirgachefe-0.1.5/setup.cfg
--rw-r--r--   0 winDy      (501) staff       (20)     1125 2022-10-18 06:02:55.000000 yirgachefe-0.1.5/setup.py
-drwxr-xr-x   0 winDy      (501) staff       (20)        0 2022-10-18 06:05:29.000000 yirgachefe-0.1.5/tests/
--rw-r--r--   0 winDy      (501) staff       (20)        0 2021-05-03 11:40:20.000000 yirgachefe-0.1.5/tests/__init__.py
--rw-r--r--   0 winDy      (501) staff       (20)     2579 2021-05-04 06:02:48.000000 yirgachefe-0.1.5/tests/test_config.py
--rw-r--r--   0 winDy      (501) staff       (20)     2795 2021-12-16 02:32:46.000000 yirgachefe-0.1.5/tests/test_logging.py
-drwxr-xr-x   0 winDy      (501) staff       (20)        0 2022-10-18 06:05:29.000000 yirgachefe-0.1.5/yirgachefe/
--rw-r--r--   0 winDy      (501) staff       (20)      418 2022-10-18 06:01:37.000000 yirgachefe-0.1.5/yirgachefe/__init__.py
--rw-r--r--   0 winDy      (501) staff       (20)     4651 2021-12-16 02:32:46.000000 yirgachefe-0.1.5/yirgachefe/config_.py
--rw-r--r--   0 winDy      (501) staff       (20)     3138 2022-10-18 05:57:50.000000 yirgachefe-0.1.5/yirgachefe/logger_.py
--rw-r--r--   0 winDy      (501) staff       (20)      778 2022-03-31 05:07:27.000000 yirgachefe-0.1.5/yirgachefe/logger_.pyi
-drwxr-xr-x   0 winDy      (501) staff       (20)        0 2022-10-18 06:05:29.000000 yirgachefe-0.1.5/yirgachefe.egg-info/
--rw-r--r--   0 winDy      (501) staff       (20)     2183 2022-10-18 06:05:29.000000 yirgachefe-0.1.5/yirgachefe.egg-info/PKG-INFO
--rw-r--r--   0 winDy      (501) staff       (20)      370 2022-10-18 06:05:29.000000 yirgachefe-0.1.5/yirgachefe.egg-info/SOURCES.txt
--rw-r--r--   0 winDy      (501) staff       (20)        1 2022-10-18 06:05:29.000000 yirgachefe-0.1.5/yirgachefe.egg-info/dependency_links.txt
--rw-r--r--   0 winDy      (501) staff       (20)      108 2022-10-18 06:05:29.000000 yirgachefe-0.1.5/yirgachefe.egg-info/requires.txt
--rw-r--r--   0 winDy      (501) staff       (20)       17 2022-10-18 06:05:29.000000 yirgachefe-0.1.5/yirgachefe.egg-info/top_level.txt
+drwxr-xr-x   0 windy      (501) staff       (20)        0 2023-06-09 02:52:57.466028 yirgachefe-0.1.6/
+-rw-r--r--   0 windy      (501) staff       (20)    11346 2023-04-17 03:36:00.000000 yirgachefe-0.1.6/LICENSE
+-rw-r--r--   0 windy      (501) staff       (20)     2251 2023-06-09 02:52:57.466202 yirgachefe-0.1.6/PKG-INFO
+-rw-r--r--   0 windy      (501) staff       (20)     1894 2023-06-09 02:42:08.000000 yirgachefe-0.1.6/README.md
+-rw-r--r--   0 windy      (501) staff       (20)      117 2023-06-09 02:52:57.466853 yirgachefe-0.1.6/setup.cfg
+-rw-r--r--   0 windy      (501) staff       (20)     1125 2023-06-09 02:51:57.000000 yirgachefe-0.1.6/setup.py
+drwxr-xr-x   0 windy      (501) staff       (20)        0 2023-06-09 02:52:57.461568 yirgachefe-0.1.6/tests/
+-rw-r--r--   0 windy      (501) staff       (20)        0 2023-04-17 03:36:00.000000 yirgachefe-0.1.6/tests/__init__.py
+-rw-r--r--   0 windy      (501) staff       (20)     2579 2023-04-17 03:36:00.000000 yirgachefe-0.1.6/tests/test_config.py
+-rw-r--r--   0 windy      (501) staff       (20)     2795 2023-04-17 03:36:00.000000 yirgachefe-0.1.6/tests/test_logging.py
+drwxr-xr-x   0 windy      (501) staff       (20)        0 2023-06-09 02:52:57.463588 yirgachefe-0.1.6/yirgachefe/
+-rw-r--r--   0 windy      (501) staff       (20)      418 2023-04-17 03:36:00.000000 yirgachefe-0.1.6/yirgachefe/__init__.py
+-rw-r--r--   0 windy      (501) staff       (20)     5229 2023-06-09 02:43:50.000000 yirgachefe-0.1.6/yirgachefe/config_.py
+-rw-r--r--   0 windy      (501) staff       (20)     3138 2023-04-17 03:36:00.000000 yirgachefe-0.1.6/yirgachefe/logger_.py
+-rw-r--r--   0 windy      (501) staff       (20)      778 2023-04-17 03:36:00.000000 yirgachefe-0.1.6/yirgachefe/logger_.pyi
+drwxr-xr-x   0 windy      (501) staff       (20)        0 2023-06-09 02:52:57.465599 yirgachefe-0.1.6/yirgachefe.egg-info/
+-rw-r--r--   0 windy      (501) staff       (20)     2251 2023-06-09 02:52:57.000000 yirgachefe-0.1.6/yirgachefe.egg-info/PKG-INFO
+-rw-r--r--   0 windy      (501) staff       (20)      413 2023-06-09 02:52:57.000000 yirgachefe-0.1.6/yirgachefe.egg-info/SOURCES.txt
+-rw-r--r--   0 windy      (501) staff       (20)        1 2023-06-09 02:52:57.000000 yirgachefe-0.1.6/yirgachefe.egg-info/dependency_links.txt
+-rw-r--r--   0 windy      (501) staff       (20)      108 2023-06-09 02:52:57.000000 yirgachefe-0.1.6/yirgachefe.egg-info/requires.txt
+-rw-r--r--   0 windy      (501) staff       (20)       17 2023-06-09 02:52:57.000000 yirgachefe-0.1.6/yirgachefe.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `yirgachefe-0.1.5/LICENSE` & `yirgachefe-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `yirgachefe-0.1.5/PKG-INFO` & `yirgachefe-0.1.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yirgachefe
-Version: 0.1.5
+Version: 0.1.6
 Summary: Convenience of configuration and logging.
 Home-page: https://github.com/iconloop/Yirgachefe
 Author: ICONLOOP
 Author-email: t_core@iconloop.com
 Requires-Python: >=3.7.5
 Description-Content-Type: text/markdown
 Provides-Extra: tests
@@ -12,15 +12,15 @@
 Provides-Extra: dev
 License-File: LICENSE
 
 # Yirgachefe
 A library for the convenience of configuring environment variables, configuration files, and logger.
 
 ## Prerequisite
-- Python 3.7.9
+- Python 3.9.x or higher
 
 ## Quick start
 The configuration file format is JSON, and the default location is [CWD]/configure.json.
 * CWD: Current working directory (you can get it with 'os.getcwd()')
 
 ### Example configure.json
 ```json
@@ -44,18 +44,21 @@
 ## Custom Usage
 
 ### Default configure.json.
 * This value is set internally and is used even if the file doesn't exist.
 * You can use the changed value by explicitly setting it in the file.
 ```json
 {
-  "debug": false,
-  "log_level": "WARNING",
+  "debug": true,
+  "log_level": "DEBUG",
   "log_format": "%(asctime)s,%(msecs)03d %(process)d %(thread)d %(levelname)s %(filename)s(%(lineno)d) %(message)s",
-  "log_path": "project-sample.log"
+  "log_path": "Yirgachefe.log",
+  "log_when": "d",
+  "log_interval": 1,
+  "log_backup_count": 5
 }
 ```
 * debug: Set stream handler to logging with coloredlog.
 * log_level: Log level for logging.
 * log_format: Log format for logging.
 * log_path: Write a file log if present (optional)
```

### Comparing `yirgachefe-0.1.5/README.md` & `yirgachefe-0.1.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Yirgachefe
 A library for the convenience of configuring environment variables, configuration files, and logger.
 
 ## Prerequisite
-- Python 3.7.9
+- Python 3.9.x or higher
 
 ## Quick start
 The configuration file format is JSON, and the default location is [CWD]/configure.json.
 * CWD: Current working directory (you can get it with 'os.getcwd()')
 
 ### Example configure.json
 ```json
@@ -30,18 +30,21 @@
 ## Custom Usage
 
 ### Default configure.json.
 * This value is set internally and is used even if the file doesn't exist.
 * You can use the changed value by explicitly setting it in the file.
 ```json
 {
-  "debug": false,
-  "log_level": "WARNING",
+  "debug": true,
+  "log_level": "DEBUG",
   "log_format": "%(asctime)s,%(msecs)03d %(process)d %(thread)d %(levelname)s %(filename)s(%(lineno)d) %(message)s",
-  "log_path": "project-sample.log"
+  "log_path": "Yirgachefe.log",
+  "log_when": "d",
+  "log_interval": 1,
+  "log_backup_count": 5
 }
 ```
 * debug: Set stream handler to logging with coloredlog.
 * log_level: Log level for logging.
 * log_format: Log format for logging.
 * log_path: Write a file log if present (optional)
```

### Comparing `yirgachefe-0.1.5/setup.py` & `yirgachefe-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     ]
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup_options = {
     "name": "yirgachefe",
-    "version": "0.1.5",
+    "version": "0.1.6",
     "url": "https://github.com/iconloop/Yirgachefe",
     "author": "ICONLOOP",
     "author_email": "t_core@iconloop.com",
     "description": "Convenience of configuration and logging.",
     "long_description": long_description,
     "long_description_content_type": "text/markdown",
     "package_data": {"yirgachefe": ["logger_.pyi"]},
```

### Comparing `yirgachefe-0.1.5/tests/test_config.py` & `yirgachefe-0.1.6/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `yirgachefe-0.1.5/tests/test_logging.py` & `yirgachefe-0.1.6/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `yirgachefe-0.1.5/yirgachefe/config_.py` & `yirgachefe-0.1.6/yirgachefe/config_.py`

 * *Files 22% similar despite different names*

```diff
@@ -47,23 +47,32 @@
         self._update_log_options()
 
     def __getitem__(self, key):
         return self._config[key]
 
     def _set_common_default(self):
         if 'debug' not in self._config:
-            self._logger.debug("config['debug'] is not configured. So default(False) is used.")
-            self._config['debug'] = False
+            self._logger.debug("config['debug'] is not configured. So default(True) is used.")
+            self._config['debug'] = True
         if 'log_level' not in self._config:
-            self._logger.debug("config['log_level'] is not configured. So default(logging.WARNING) is used.")
-            self._config['log_level'] = logging.getLevelName(logging.WARNING)
+            self._logger.debug("config['log_level'] is not configured. So default(logging.DEBUG) is used.")
+            self._config['log_level'] = logging.getLevelName(logging.DEBUG)
         if 'log_format' not in self._config:
             self._logger.debug("config['log_format'] is not in configured. So default is used.")
             self._config['log_format'] = \
                 "%(asctime)s,%(msecs)03d %(process)d %(thread)d %(levelname)s %(filename)s(%(lineno)d) %(message)s"
+        if 'log_when' not in self._config:
+            self._logger.debug("config['log_when'] is not in configured. So default(d) is used.")
+            self._config['log_when'] = "d"
+        if 'log_interval' not in self._config:
+            self._logger.debug("config['log_interval'] is not in configured. So default(1) is used.")
+            self._config['log_interval'] = 1
+        if 'log_backup_count' not in self._config:
+            self._logger.debug("config['log_backup_count'] is not in configured. So default(5) is used.")
+            self._config['log_backup_count'] = 5
 
     def _load_config_file(self, config_path: Path, check_exist=True):
         if not check_exist and not config_path.is_file():
             return
 
         with open(config_path, 'r') as config_file:
             self._config.update(json.load(config_file))
```

### Comparing `yirgachefe-0.1.5/yirgachefe/logger_.py` & `yirgachefe-0.1.6/yirgachefe/logger_.py`

 * *Files identical despite different names*

### Comparing `yirgachefe-0.1.5/yirgachefe/logger_.pyi` & `yirgachefe-0.1.6/yirgachefe/logger_.pyi`

 * *Files identical despite different names*

### Comparing `yirgachefe-0.1.5/yirgachefe.egg-info/PKG-INFO` & `yirgachefe-0.1.6/yirgachefe.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yirgachefe
-Version: 0.1.5
+Version: 0.1.6
 Summary: Convenience of configuration and logging.
 Home-page: https://github.com/iconloop/Yirgachefe
 Author: ICONLOOP
 Author-email: t_core@iconloop.com
 Requires-Python: >=3.7.5
 Description-Content-Type: text/markdown
 Provides-Extra: tests
@@ -12,15 +12,15 @@
 Provides-Extra: dev
 License-File: LICENSE
 
 # Yirgachefe
 A library for the convenience of configuring environment variables, configuration files, and logger.
 
 ## Prerequisite
-- Python 3.7.9
+- Python 3.9.x or higher
 
 ## Quick start
 The configuration file format is JSON, and the default location is [CWD]/configure.json.
 * CWD: Current working directory (you can get it with 'os.getcwd()')
 
 ### Example configure.json
 ```json
@@ -44,18 +44,21 @@
 ## Custom Usage
 
 ### Default configure.json.
 * This value is set internally and is used even if the file doesn't exist.
 * You can use the changed value by explicitly setting it in the file.
 ```json
 {
-  "debug": false,
-  "log_level": "WARNING",
+  "debug": true,
+  "log_level": "DEBUG",
   "log_format": "%(asctime)s,%(msecs)03d %(process)d %(thread)d %(levelname)s %(filename)s(%(lineno)d) %(message)s",
-  "log_path": "project-sample.log"
+  "log_path": "Yirgachefe.log",
+  "log_when": "d",
+  "log_interval": 1,
+  "log_backup_count": 5
 }
 ```
 * debug: Set stream handler to logging with coloredlog.
 * log_level: Log level for logging.
 * log_format: Log format for logging.
 * log_path: Write a file log if present (optional)
```

