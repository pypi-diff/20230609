# Comparing `tmp/mlogconfig-0.2.2.tar.gz` & `tmp/mlogconfig-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlogconfig-0.2.2.tar", last modified: Fri Apr 14 16:17:59 2023, max compression
+gzip compressed data, was "mlogconfig-0.2.3.tar", max compression
```

## Comparing `mlogconfig-0.2.2.tar` & `mlogconfig-0.2.3.tar`

### file list

```diff
@@ -1,13 +1,6 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 16:17:59.647324 mlogconfig-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (122)     1099 2023-04-14 16:17:49.000000 mlogconfig-0.2.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-04-14 16:17:49.000000 mlogconfig-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     3547 2023-04-14 16:17:59.647324 mlogconfig-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2751 2023-04-14 16:17:49.000000 mlogconfig-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 16:17:59.647324 mlogconfig-0.2.2/mlogconfig.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3547 2023-04-14 16:17:59.000000 mlogconfig-0.2.2/mlogconfig.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      210 2023-04-14 16:17:59.000000 mlogconfig-0.2.2/mlogconfig.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-14 16:17:59.000000 mlogconfig-0.2.2/mlogconfig.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       36 2023-04-14 16:17:59.000000 mlogconfig-0.2.2/mlogconfig.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-14 16:17:59.000000 mlogconfig-0.2.2/mlogconfig.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-14 16:17:59.647324 mlogconfig-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1283 2023-04-14 16:17:49.000000 mlogconfig-0.2.2/setup.py
+-rw-r--r--   0        0        0     1099 2023-06-09 20:25:09.193459 mlogconfig-0.2.3/LICENSE.md
+-rw-r--r--   0        0        0     2614 2023-06-09 20:25:09.193459 mlogconfig-0.2.3/README.md
+-rw-r--r--   0        0        0     3144 2023-06-09 20:25:09.193459 mlogconfig-0.2.3/mlogconfig/mlogconfig.py
+-rw-r--r--   0        0        0      901 2023-06-09 20:25:09.193459 mlogconfig-0.2.3/mlogconfig/modules/validate.py
+-rw-r--r--   0        0        0      557 2023-06-09 20:25:24.910405 mlogconfig-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     3383 1970-01-01 00:00:00.000000 mlogconfig-0.2.3/PKG-INFO
```

### Comparing `mlogconfig-0.2.2/LICENSE.md` & `mlogconfig-0.2.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mlogconfig-0.2.2/PKG-INFO` & `mlogconfig-0.2.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 Metadata-Version: 2.1
 Name: mlogconfig
-Version: 0.2.2
-Summary: A simple logging setup utility that configures logging with file, console, syslog, and Windows event log handlers.
-Home-page: https://github.com/talltechy/mlogconfig
-Author: Matt Wyen
+Version: 0.2.3
+Summary: This module provides a configurable logging setup for Python applications. It supports logging to console, file, syslog (for Linux and macOS), and Windows Event Log. The user can enable or disable each logging method as needed.
+License: MIT
+Author: Matt
 Author-email: matt@mattwyen.me
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
+Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-License-File: LICENSE.md
 
 # [mlogconfig.py](mlogconfig.py)
 
 [![linting: pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)](https://github.com/pylint-dev/pylint)
-[![Upload Python Package](https://github.com/talltechy/mlogconfig/actions/workflows/python-publish.yml/badge.svg)](https://github.com/talltechy/mlogconfig/actions/workflows/python-publish.yml)
-[![PyPI](https://img.shields.io/pypi/v/mlogconfig?label=PyPI%20Package%20Version&style=flat-square)](https://pypi.org/project/mlogconfig/)
+[![PyPI](https://img.shields.io/pypi/v/mlogconfig?label=PyPI%20Package%20Version)](https://pypi.org/project/mlogconfig/)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/mlogconfig?color=blue)
 [![CodeQL](https://github.com/talltechy/mlogconfig/actions/workflows/github-code-scanning/codeql/badge.svg?branch=main)](https://github.com/talltechy/mlogconfig/actions/workflows/github-code-scanning/codeql)
 
 This module provides a configurable logging setup for Python applications. It supports logging to console, file, syslog (for Linux and macOS), and Windows Event Log. The user can enable or disable each logging method as needed.
 
 ## Features
 
 - Logging to console, file, syslog, and Windows Event Log
@@ -86,7 +83,8 @@
 ## Contributing
 
 Contributions are welcome! Please read the [contributing guidelines](https://github.com/talltechy/mlogconfig/blob/main/CONTRIBUTING.md) before submitting pull requests or opening issues.
 
 ## License
 
 MLogConfig is licensed under the [MIT License](https://github.com/talltechy/mlogconfig/blob/main/LICENSE.md).
+
```

### Comparing `mlogconfig-0.2.2/README.md` & `mlogconfig-0.2.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # [mlogconfig.py](mlogconfig.py)
 
 [![linting: pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)](https://github.com/pylint-dev/pylint)
-[![Upload Python Package](https://github.com/talltechy/mlogconfig/actions/workflows/python-publish.yml/badge.svg)](https://github.com/talltechy/mlogconfig/actions/workflows/python-publish.yml)
-[![PyPI](https://img.shields.io/pypi/v/mlogconfig?label=PyPI%20Package%20Version&style=flat-square)](https://pypi.org/project/mlogconfig/)
+[![PyPI](https://img.shields.io/pypi/v/mlogconfig?label=PyPI%20Package%20Version)](https://pypi.org/project/mlogconfig/)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/mlogconfig?color=blue)
 [![CodeQL](https://github.com/talltechy/mlogconfig/actions/workflows/github-code-scanning/codeql/badge.svg?branch=main)](https://github.com/talltechy/mlogconfig/actions/workflows/github-code-scanning/codeql)
 
 This module provides a configurable logging setup for Python applications. It supports logging to console, file, syslog (for Linux and macOS), and Windows Event Log. The user can enable or disable each logging method as needed.
 
 ## Features
 
 - Logging to console, file, syslog, and Windows Event Log
```

