# Comparing `tmp/mypy-boto3-acm-pca-1.26.151.tar.gz` & `tmp/mypy-boto3-acm-pca-1.26.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-acm-pca-1.26.151.tar", last modified: Fri Jun  9 19:47:15 2023, max compression
+gzip compressed data, was "mypy-boto3-acm-pca-1.26.45.tar", last modified: Fri Jan  6 20:32:17 2023, max compression
```

## Comparing `mypy-boto3-acm-pca-1.26.151.tar` & `mypy-boto3-acm-pca-1.26.45.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:47:15.790883 mypy-boto3-acm-pca-1.26.151/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-09 19:46:56.000000 mypy-boto3-acm-pca-1.26.151/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17166 2023-06-09 19:47:15.790883 mypy-boto3-acm-pca-1.26.151/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15678 2023-06-09 19:46:56.000000 mypy-boto3-acm-pca-1.26.151/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:47:15.790883 mypy-boto3-acm-pca-1.26.151/mypy_boto3_acm_pca/
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-06-09 19:46:56.000000 mypy-boto3-acm-pca-1.26.151/mypy_boto3_acm_pca/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-06-09 19:46:56.000000 mypy-boto3-acm-pca-1.26.151/mypy_boto3_acm_pca/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-06-09 19:46:56.000000 mypy-boto3-acm-pca-1.26.151/mypy_boto3_acm_pca/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22381 2023-06-09 19:46:56.000000 mypy-boto3-acm-pca-1.26.151/mypy_boto3_acm_pca/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    22345 2023-06-09 19:46:56.000000 mypy-boto3-acm-pca-1.26.151/mypy_boto3_acm_pca/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11147 2023-06-09 19:46:56.000000 mypy-boto3-acm-pca-1.26.151/mypy_boto3_acm_pca/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11145 2023-06-09 19:46:56.000000 mypy-boto3-acm-pca-1.26.151/mypy_boto3_acm_pca/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-06-09 19:46:56.000000 mypy-boto3-acm-pca-1.26.151/mypy_boto3_acm_pca/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-06-09 19:46:56.000000 mypy-boto3-acm-pca-1.26.151/mypy_boto3_acm_pca/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 19:46:56.000000 mypy-boto3-acm-pca-1.26.151/mypy_boto3_acm_pca/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    27342 2023-06-09 19:46:57.000000 mypy-boto3-acm-pca-1.26.151/mypy_boto3_acm_pca/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    27299 2023-06-09 19:46:57.000000 mypy-boto3-acm-pca-1.26.151/mypy_boto3_acm_pca/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-09 19:46:56.000000 mypy-boto3-acm-pca-1.26.151/mypy_boto3_acm_pca/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-06-09 19:46:56.000000 mypy-boto3-acm-pca-1.26.151/mypy_boto3_acm_pca/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-06-09 19:46:56.000000 mypy-boto3-acm-pca-1.26.151/mypy_boto3_acm_pca/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:47:15.790883 mypy-boto3-acm-pca-1.26.151/mypy_boto3_acm_pca.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17166 2023-06-09 19:47:15.000000 mypy-boto3-acm-pca-1.26.151/mypy_boto3_acm_pca.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-09 19:47:15.000000 mypy-boto3-acm-pca-1.26.151/mypy_boto3_acm_pca.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 19:47:15.000000 mypy-boto3-acm-pca-1.26.151/mypy_boto3_acm_pca.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 19:47:15.000000 mypy-boto3-acm-pca-1.26.151/mypy_boto3_acm_pca.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-09 19:47:15.000000 mypy-boto3-acm-pca-1.26.151/mypy_boto3_acm_pca.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-09 19:47:15.000000 mypy-boto3-acm-pca-1.26.151/mypy_boto3_acm_pca.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 19:47:15.790883 mypy-boto3-acm-pca-1.26.151/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-06-09 19:46:56.000000 mypy-boto3-acm-pca-1.26.151/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 20:32:17.806611 mypy-boto3-acm-pca-1.26.45/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-06 20:32:06.000000 mypy-boto3-acm-pca-1.26.45/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17184 2023-01-06 20:32:17.798611 mypy-boto3-acm-pca-1.26.45/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15698 2023-01-06 20:32:06.000000 mypy-boto3-acm-pca-1.26.45/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 20:32:17.798611 mypy-boto3-acm-pca-1.26.45/mypy_boto3_acm_pca/
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-01-06 20:32:06.000000 mypy-boto3-acm-pca-1.26.45/mypy_boto3_acm_pca/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-01-06 20:32:06.000000 mypy-boto3-acm-pca-1.26.45/mypy_boto3_acm_pca/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-01-06 20:32:06.000000 mypy-boto3-acm-pca-1.26.45/mypy_boto3_acm_pca/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22382 2023-01-06 20:32:06.000000 mypy-boto3-acm-pca-1.26.45/mypy_boto3_acm_pca/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22346 2023-01-06 20:32:06.000000 mypy-boto3-acm-pca-1.26.45/mypy_boto3_acm_pca/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10838 2023-01-06 20:32:07.000000 mypy-boto3-acm-pca-1.26.45/mypy_boto3_acm_pca/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10836 2023-01-06 20:32:06.000000 mypy-boto3-acm-pca-1.26.45/mypy_boto3_acm_pca/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-01-06 20:32:06.000000 mypy-boto3-acm-pca-1.26.45/mypy_boto3_acm_pca/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-01-06 20:32:06.000000 mypy-boto3-acm-pca-1.26.45/mypy_boto3_acm_pca/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-06 20:32:06.000000 mypy-boto3-acm-pca-1.26.45/mypy_boto3_acm_pca/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    27342 2023-01-06 20:32:07.000000 mypy-boto3-acm-pca-1.26.45/mypy_boto3_acm_pca/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27299 2023-01-06 20:32:07.000000 mypy-boto3-acm-pca-1.26.45/mypy_boto3_acm_pca/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-06 20:32:06.000000 mypy-boto3-acm-pca-1.26.45/mypy_boto3_acm_pca/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-01-06 20:32:06.000000 mypy-boto3-acm-pca-1.26.45/mypy_boto3_acm_pca/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-01-06 20:32:06.000000 mypy-boto3-acm-pca-1.26.45/mypy_boto3_acm_pca/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 20:32:17.798611 mypy-boto3-acm-pca-1.26.45/mypy_boto3_acm_pca.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17184 2023-01-06 20:32:17.000000 mypy-boto3-acm-pca-1.26.45/mypy_boto3_acm_pca.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-01-06 20:32:17.000000 mypy-boto3-acm-pca-1.26.45/mypy_boto3_acm_pca.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-06 20:32:17.000000 mypy-boto3-acm-pca-1.26.45/mypy_boto3_acm_pca.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-06 20:32:17.000000 mypy-boto3-acm-pca-1.26.45/mypy_boto3_acm_pca.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-06 20:32:17.000000 mypy-boto3-acm-pca-1.26.45/mypy_boto3_acm_pca.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-01-06 20:32:17.000000 mypy-boto3-acm-pca-1.26.45/mypy_boto3_acm_pca.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-06 20:32:17.806611 mypy-boto3-acm-pca-1.26.45/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-01-06 20:32:06.000000 mypy-boto3-acm-pca-1.26.45/setup.py
```

### Comparing `mypy-boto3-acm-pca-1.26.151/LICENSE` & `mypy-boto3-acm-pca-1.26.45/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Vlad Emelianov
+Copyright (c) 2022 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mypy-boto3-acm-pca-1.26.151/PKG-INFO` & `mypy-boto3-acm-pca-1.26.45/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-acm-pca
-Version: 1.26.151
-Summary: Type annotations for boto3.ACMPCA 1.26.151 service generated with mypy-boto3-builder 7.14.5
+Version: 1.26.45
+Summary: Type annotations for boto3.ACMPCA 1.26.45 service generated with mypy-boto3-builder 7.12.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-acm-pca"></a>
 
 # mypy-boto3-acm-pca
 
 [![PyPI - mypy-boto3-acm-pca](https://img.shields.io/pypi/v/mypy-boto3-acm-pca.svg?color=blue)](https://pypi.org/project/mypy-boto3-acm-pca)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-acm-pca.svg?color=blue)](https://pypi.org/project/mypy-boto3-acm-pca)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-acm-pca?color=blue)](https://pypistats.org/packages/mypy-boto3-acm-pca)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ACMPCA 1.26.151](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA)
+[boto3.ACMPCA 1.26.45](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-acm-pca docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca/).
 
 See how it helps to find and fix potential bugs:
 
@@ -460,42 +460,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers drop-in type annotations for you and makes sure that:
+updates. It delivers a drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from `botocore` schemas.
+  annotations extracted from the documentation (blame `botocore` docs if types
+  are incorrect).
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
-  libraries
+- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.resource` calls
-- Auto discovery of types for `session.client` and `session.resource` calls
+- Auto discovery of types for `boto3.client` and `boto3.session` calls
+- Auto discovery of types for `session.client` and `session.session` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-acm-pca-1.26.151/README.md` & `mypy-boto3-acm-pca-1.26.45/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-acm-pca"></a>
 
 # mypy-boto3-acm-pca
 
 [![PyPI - mypy-boto3-acm-pca](https://img.shields.io/pypi/v/mypy-boto3-acm-pca.svg?color=blue)](https://pypi.org/project/mypy-boto3-acm-pca)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-acm-pca.svg?color=blue)](https://pypi.org/project/mypy-boto3-acm-pca)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-acm-pca?color=blue)](https://pypistats.org/packages/mypy-boto3-acm-pca)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ACMPCA 1.26.151](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA)
+[boto3.ACMPCA 1.26.45](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-acm-pca docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca/).
 
 See how it helps to find and fix potential bugs:
 
@@ -428,42 +428,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers drop-in type annotations for you and makes sure that:
+updates. It delivers a drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from `botocore` schemas.
+  annotations extracted from the documentation (blame `botocore` docs if types
+  are incorrect).
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
-  libraries
+- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.resource` calls
-- Auto discovery of types for `session.client` and `session.resource` calls
+- Auto discovery of types for `boto3.client` and `boto3.session` calls
+- Auto discovery of types for `session.client` and `session.session` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-acm-pca-1.26.151/mypy_boto3_acm_pca/__init__.py` & `mypy-boto3-acm-pca-1.26.45/mypy_boto3_acm_pca/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-pca-1.26.151/mypy_boto3_acm_pca/__init__.pyi` & `mypy-boto3-acm-pca-1.26.45/mypy_boto3_acm_pca/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-pca-1.26.151/mypy_boto3_acm_pca/__main__.py` & `mypy-boto3-acm-pca-1.26.45/mypy_boto3_acm_pca/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ACMPCA 1.26.151\nVersion:         1.26.151\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.ACMPCA 1.26.45\nVersion:         1.26.45\nBuilder version:"
+        " 7.12.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.151")
+    print("1.26.45")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-acm-pca-1.26.151/mypy_boto3_acm_pca/client.py` & `mypy-boto3-acm-pca-1.26.45/mypy_boto3_acm_pca/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -172,15 +172,15 @@
         CertificateAuthorityArn: str,
         Principal: str,
         Actions: Sequence[ActionTypeType],
         SourceAccount: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Grants one or more permissions on a private CA to the Certificate Manager (ACM)
-        service principal ( `acm.amazonaws.com`).
+        service principal ( `acm.amazonaws.com` ).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA.Client.create_permission)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca/client/#create_permission)
         """
 
     def delete_certificate_authority(
         self, *, CertificateAuthorityArn: str, PermanentDeletionTimeInDays: int = ...
```

### Comparing `mypy-boto3-acm-pca-1.26.151/mypy_boto3_acm_pca/client.pyi` & `mypy-boto3-acm-pca-1.26.45/mypy_boto3_acm_pca/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -163,15 +163,15 @@
         CertificateAuthorityArn: str,
         Principal: str,
         Actions: Sequence[ActionTypeType],
         SourceAccount: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Grants one or more permissions on a private CA to the Certificate Manager (ACM)
-        service principal ( `acm.amazonaws.com`).
+        service principal ( `acm.amazonaws.com` ).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA.Client.create_permission)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca/client/#create_permission)
         """
     def delete_certificate_authority(
         self, *, CertificateAuthorityArn: str, PermanentDeletionTimeInDays: int = ...
     ) -> EmptyResponseMetadataTypeDef:
```

### Comparing `mypy-boto3-acm-pca-1.26.151/mypy_boto3_acm_pca/literals.py` & `mypy-boto3-acm-pca-1.26.45/mypy_boto3_acm_pca/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,26 +145,24 @@
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
-    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
-    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
@@ -250,15 +248,14 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
-    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
@@ -269,20 +266,18 @@
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
-    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
-    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
     "kinesis-video-webrtc-storage",
     "kinesisanalytics",
@@ -313,15 +308,14 @@
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
-    "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
@@ -340,19 +334,16 @@
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
-    "osis",
     "outposts",
     "panorama",
-    "payment-cryptography",
-    "payment-cryptography-data",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
@@ -432,20 +423,18 @@
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
-    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
-    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
@@ -474,25 +463,21 @@
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
-    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
-    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
-    "eu-central-2",
     "eu-north-1",
     "eu-south-1",
-    "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
```

### Comparing `mypy-boto3-acm-pca-1.26.151/mypy_boto3_acm_pca/literals.pyi` & `mypy-boto3-acm-pca-1.26.45/mypy_boto3_acm_pca/literals.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -143,26 +143,24 @@
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
-    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
-    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
@@ -248,15 +246,14 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
-    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
@@ -267,20 +264,18 @@
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
-    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
-    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
     "kinesis-video-webrtc-storage",
     "kinesisanalytics",
@@ -311,15 +306,14 @@
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
-    "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
@@ -338,19 +332,16 @@
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
-    "osis",
     "outposts",
     "panorama",
-    "payment-cryptography",
-    "payment-cryptography-data",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
@@ -430,20 +421,18 @@
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
-    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
-    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
@@ -472,25 +461,21 @@
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
-    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
-    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
-    "eu-central-2",
     "eu-north-1",
     "eu-south-1",
-    "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
```

### Comparing `mypy-boto3-acm-pca-1.26.151/mypy_boto3_acm_pca/paginator.py` & `mypy-boto3-acm-pca-1.26.45/mypy_boto3_acm_pca/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-pca-1.26.151/mypy_boto3_acm_pca/paginator.pyi` & `mypy-boto3-acm-pca-1.26.45/mypy_boto3_acm_pca/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-pca-1.26.151/mypy_boto3_acm_pca/type_defs.py` & `mypy-boto3-acm-pca-1.26.45/mypy_boto3_acm_pca/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-pca-1.26.151/mypy_boto3_acm_pca/type_defs.pyi` & `mypy-boto3-acm-pca-1.26.45/mypy_boto3_acm_pca/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-pca-1.26.151/mypy_boto3_acm_pca/waiter.py` & `mypy-boto3-acm-pca-1.26.45/mypy_boto3_acm_pca/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-pca-1.26.151/mypy_boto3_acm_pca/waiter.pyi` & `mypy-boto3-acm-pca-1.26.45/mypy_boto3_acm_pca/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-pca-1.26.151/mypy_boto3_acm_pca.egg-info/PKG-INFO` & `mypy-boto3-acm-pca-1.26.45/mypy_boto3_acm_pca.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-acm-pca
-Version: 1.26.151
-Summary: Type annotations for boto3.ACMPCA 1.26.151 service generated with mypy-boto3-builder 7.14.5
+Version: 1.26.45
+Summary: Type annotations for boto3.ACMPCA 1.26.45 service generated with mypy-boto3-builder 7.12.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-acm-pca"></a>
 
 # mypy-boto3-acm-pca
 
 [![PyPI - mypy-boto3-acm-pca](https://img.shields.io/pypi/v/mypy-boto3-acm-pca.svg?color=blue)](https://pypi.org/project/mypy-boto3-acm-pca)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-acm-pca.svg?color=blue)](https://pypi.org/project/mypy-boto3-acm-pca)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-acm-pca?color=blue)](https://pypistats.org/packages/mypy-boto3-acm-pca)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ACMPCA 1.26.151](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA)
+[boto3.ACMPCA 1.26.45](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-acm-pca docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca/).
 
 See how it helps to find and fix potential bugs:
 
@@ -460,42 +460,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers drop-in type annotations for you and makes sure that:
+updates. It delivers a drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from `botocore` schemas.
+  annotations extracted from the documentation (blame `botocore` docs if types
+  are incorrect).
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
-  libraries
+- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.resource` calls
-- Auto discovery of types for `session.client` and `session.resource` calls
+- Auto discovery of types for `boto3.client` and `boto3.session` calls
+- Auto discovery of types for `session.client` and `session.session` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-acm-pca-1.26.151/mypy_boto3_acm_pca.egg-info/SOURCES.txt` & `mypy-boto3-acm-pca-1.26.45/mypy_boto3_acm_pca.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-pca-1.26.151/setup.py` & `mypy-boto3-acm-pca-1.26.45/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 """
 Setup script for mypy-boto3-acm-pca.
 """
-from pathlib import Path
+from os.path import abspath, dirname
 
 from setuptools import setup
 
-LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
+LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-acm-pca",
-    version="1.26.151",
+    version="1.26.45",
     packages=["mypy_boto3_acm_pca"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ACMPCA 1.26.151 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.ACMPCA 1.26.45 service generated with mypy-boto3-builder 7.12.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -45,11 +44,11 @@
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
-        'typing-extensions>=4.1.0; python_version<"3.9"',
+        "typing-extensions>=4.1.0",
     ],
     zip_safe=False,
 )
```

