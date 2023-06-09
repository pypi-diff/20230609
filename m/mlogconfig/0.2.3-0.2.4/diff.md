# Comparing `tmp/mlogconfig-0.2.3.tar.gz` & `tmp/mlogconfig-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlogconfig-0.2.3.tar", max compression
+gzip compressed data, was "mlogconfig-0.2.4.tar", max compression
```

## Comparing `mlogconfig-0.2.3.tar` & `mlogconfig-0.2.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1099 2023-06-09 20:25:09.193459 mlogconfig-0.2.3/LICENSE.md
--rw-r--r--   0        0        0     2614 2023-06-09 20:25:09.193459 mlogconfig-0.2.3/README.md
--rw-r--r--   0        0        0     3144 2023-06-09 20:25:09.193459 mlogconfig-0.2.3/mlogconfig/mlogconfig.py
--rw-r--r--   0        0        0      901 2023-06-09 20:25:09.193459 mlogconfig-0.2.3/mlogconfig/modules/validate.py
--rw-r--r--   0        0        0      557 2023-06-09 20:25:24.910405 mlogconfig-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     3383 1970-01-01 00:00:00.000000 mlogconfig-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1099 2023-06-09 21:41:42.657471 mlogconfig-0.2.4/LICENSE.md
+-rw-r--r--   0        0        0     2614 2023-06-09 21:41:42.657471 mlogconfig-0.2.4/README.md
+-rw-r--r--   0        0        0     3145 2023-06-09 21:41:42.657471 mlogconfig-0.2.4/mlogconfig/mlogconfig.py
+-rw-r--r--   0        0        0      901 2023-06-09 21:41:42.657471 mlogconfig-0.2.4/mlogconfig/modules/validate.py
+-rw-r--r--   0        0        0      557 2023-06-09 21:42:01.078083 mlogconfig-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     3383 1970-01-01 00:00:00.000000 mlogconfig-0.2.4/PKG-INFO
```

### Comparing `mlogconfig-0.2.3/LICENSE.md` & `mlogconfig-0.2.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mlogconfig-0.2.3/README.md` & `mlogconfig-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `mlogconfig-0.2.3/mlogconfig/mlogconfig.py` & `mlogconfig-0.2.4/mlogconfig/mlogconfig.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import datetime
 import platform
 import logging
 import argparse
 from logging import Formatter, StreamHandler, getLogger
 from logging.handlers import SysLogHandler
 from typing import Union
-from modules.validate import validate_file
+from .modules.validate import validate_file
 
 def setup_logging(
     file_path: str,
     error_log_file_path: str,
     console_logging: bool = False,
     syslog_logging: bool = False,
     log_level: Union[int, str] = logging.INFO,
```

### Comparing `mlogconfig-0.2.3/mlogconfig/modules/validate.py` & `mlogconfig-0.2.4/mlogconfig/modules/validate.py`

 * *Files identical despite different names*

### Comparing `mlogconfig-0.2.3/pyproject.toml` & `mlogconfig-0.2.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mlogconfig"
-version = "v0.2.3"
+version = "v0.2.4"
 description = "This module provides a configurable logging setup for Python applications. It supports logging to console, file, syslog (for Linux and macOS), and Windows Event Log. The user can enable or disable each logging method as needed."
 authors = ["Matt <matt@mattwyen.me>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

### Comparing `mlogconfig-0.2.3/PKG-INFO` & `mlogconfig-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlogconfig
-Version: 0.2.3
+Version: 0.2.4
 Summary: This module provides a configurable logging setup for Python applications. It supports logging to console, file, syslog (for Linux and macOS), and Windows Event Log. The user can enable or disable each logging method as needed.
 License: MIT
 Author: Matt
 Author-email: matt@mattwyen.me
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

