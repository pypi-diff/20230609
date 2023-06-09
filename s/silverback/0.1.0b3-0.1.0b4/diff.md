# Comparing `tmp/silverback-0.1.0b3.tar.gz` & `tmp/silverback-0.1.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "silverback-0.1.0b3.tar", last modified: Thu Jun  8 03:38:52 2023, max compression
+gzip compressed data, was "silverback-0.1.0b4.tar", last modified: Fri Jun  9 01:47:46 2023, max compression
```

## Comparing `silverback-0.1.0b3.tar` & `silverback-0.1.0b4.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:38:52.707865 silverback-0.1.0b3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:38:52.707865 silverback-0.1.0b3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:38:52.707865 silverback-0.1.0b3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-08 03:37:46.000000 silverback-0.1.0b3/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-08 03:37:46.000000 silverback-0.1.0b3/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-08 03:37:46.000000 silverback-0.1.0b3/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-08 03:37:46.000000 silverback-0.1.0b3/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-08 03:37:46.000000 silverback-0.1.0b3/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:38:52.707865 silverback-0.1.0b3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-08 03:37:46.000000 silverback-0.1.0b3/.github/workflows/codeql.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-08 03:37:46.000000 silverback-0.1.0b3/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-08 03:37:46.000000 silverback-0.1.0b3/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-08 03:37:46.000000 silverback-0.1.0b3/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-08 03:37:46.000000 silverback-0.1.0b3/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-06-08 03:37:46.000000 silverback-0.1.0b3/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-08 03:37:46.000000 silverback-0.1.0b3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-08 03:37:46.000000 silverback-0.1.0b3/.mdformat.toml
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-08 03:37:46.000000 silverback-0.1.0b3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-06-08 03:37:46.000000 silverback-0.1.0b3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-08 03:37:46.000000 silverback-0.1.0b3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-06-08 03:38:52.711865 silverback-0.1.0b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-08 03:37:46.000000 silverback-0.1.0b3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-08 03:37:46.000000 silverback-0.1.0b3/example.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-08 03:37:46.000000 silverback-0.1.0b3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-08 03:38:52.711865 silverback-0.1.0b3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-06-08 03:37:46.000000 silverback-0.1.0b3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:38:52.707865 silverback-0.1.0b3/silverback/
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-08 03:37:46.000000 silverback-0.1.0b3/silverback/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-08 03:37:46.000000 silverback-0.1.0b3/silverback/_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-06-08 03:37:46.000000 silverback-0.1.0b3/silverback/_importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-06-08 03:37:46.000000 silverback-0.1.0b3/silverback/application.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-06-08 03:37:46.000000 silverback-0.1.0b3/silverback/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-06-08 03:37:46.000000 silverback-0.1.0b3/silverback/middlewares.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 03:37:46.000000 silverback-0.1.0b3/silverback/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-06-08 03:37:46.000000 silverback-0.1.0b3/silverback/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-06-08 03:37:46.000000 silverback-0.1.0b3/silverback/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-08 03:37:46.000000 silverback-0.1.0b3/silverback/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-08 03:38:52.000000 silverback-0.1.0b3/silverback/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:38:52.707865 silverback-0.1.0b3/silverback.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-06-08 03:38:52.000000 silverback-0.1.0b3/silverback.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-08 03:38:52.000000 silverback-0.1.0b3/silverback.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 03:38:52.000000 silverback-0.1.0b3/silverback.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-08 03:38:52.000000 silverback-0.1.0b3/silverback.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 03:38:52.000000 silverback-0.1.0b3/silverback.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-08 03:38:52.000000 silverback-0.1.0b3/silverback.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-08 03:38:52.000000 silverback-0.1.0b3/silverback.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:38:52.707865 silverback-0.1.0b3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 03:37:46.000000 silverback-0.1.0b3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:47:46.475680 silverback-0.1.0b4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:47:46.475680 silverback-0.1.0b4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:47:46.475680 silverback-0.1.0b4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-09 01:46:32.000000 silverback-0.1.0b4/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-09 01:46:32.000000 silverback-0.1.0b4/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-09 01:46:32.000000 silverback-0.1.0b4/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-09 01:46:32.000000 silverback-0.1.0b4/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-09 01:46:32.000000 silverback-0.1.0b4/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:47:46.475680 silverback-0.1.0b4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-09 01:46:32.000000 silverback-0.1.0b4/.github/workflows/codeql.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-09 01:46:32.000000 silverback-0.1.0b4/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-09 01:46:32.000000 silverback-0.1.0b4/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-09 01:46:32.000000 silverback-0.1.0b4/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-09 01:46:32.000000 silverback-0.1.0b4/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-06-09 01:46:32.000000 silverback-0.1.0b4/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-09 01:46:32.000000 silverback-0.1.0b4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-09 01:46:32.000000 silverback-0.1.0b4/.mdformat.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-09 01:46:32.000000 silverback-0.1.0b4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-06-09 01:46:32.000000 silverback-0.1.0b4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-09 01:46:32.000000 silverback-0.1.0b4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-06-09 01:47:46.475680 silverback-0.1.0b4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-09 01:46:32.000000 silverback-0.1.0b4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-09 01:46:32.000000 silverback-0.1.0b4/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-09 01:46:32.000000 silverback-0.1.0b4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-09 01:47:46.475680 silverback-0.1.0b4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-06-09 01:46:32.000000 silverback-0.1.0b4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:47:46.475680 silverback-0.1.0b4/silverback/
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-09 01:46:32.000000 silverback-0.1.0b4/silverback/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-09 01:46:32.000000 silverback-0.1.0b4/silverback/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-06-09 01:46:32.000000 silverback-0.1.0b4/silverback/_importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-06-09 01:46:32.000000 silverback-0.1.0b4/silverback/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-06-09 01:46:32.000000 silverback-0.1.0b4/silverback/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-06-09 01:46:32.000000 silverback-0.1.0b4/silverback/middlewares.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 01:46:32.000000 silverback-0.1.0b4/silverback/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-06-09 01:46:32.000000 silverback-0.1.0b4/silverback/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-06-09 01:46:32.000000 silverback-0.1.0b4/silverback/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-09 01:46:32.000000 silverback-0.1.0b4/silverback/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-09 01:47:45.000000 silverback-0.1.0b4/silverback/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:47:46.475680 silverback-0.1.0b4/silverback.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-06-09 01:47:46.000000 silverback-0.1.0b4/silverback.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-09 01:47:46.000000 silverback-0.1.0b4/silverback.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 01:47:46.000000 silverback-0.1.0b4/silverback.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-09 01:47:46.000000 silverback-0.1.0b4/silverback.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 01:47:46.000000 silverback-0.1.0b4/silverback.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-09 01:47:46.000000 silverback-0.1.0b4/silverback.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-09 01:47:46.000000 silverback-0.1.0b4/silverback.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:47:46.475680 silverback-0.1.0b4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 01:46:32.000000 silverback-0.1.0b4/tests/__init__.py
```

### Comparing `silverback-0.1.0b3/.github/ISSUE_TEMPLATE/bug.md` & `silverback-0.1.0b4/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0b3/.github/ISSUE_TEMPLATE/feature.md` & `silverback-0.1.0b4/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0b3/.github/ISSUE_TEMPLATE/work-item.md` & `silverback-0.1.0b4/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0b3/.github/release-drafter.yml` & `silverback-0.1.0b4/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0b3/.github/workflows/codeql.yaml` & `silverback-0.1.0b4/.github/workflows/codeql.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0b3/.github/workflows/commitlint.yaml` & `silverback-0.1.0b4/.github/workflows/commitlint.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0b3/.github/workflows/prtitle.yaml` & `silverback-0.1.0b4/.github/workflows/prtitle.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0b3/.github/workflows/publish.yaml` & `silverback-0.1.0b4/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0b3/.github/workflows/test.yaml` & `silverback-0.1.0b4/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0b3/.gitignore` & `silverback-0.1.0b4/.gitignore`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0b3/.pre-commit-config.yaml` & `silverback-0.1.0b4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0b3/CONTRIBUTING.md` & `silverback-0.1.0b4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0b3/LICENSE` & `silverback-0.1.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0b3/PKG-INFO` & `silverback-0.1.0b4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: silverback
-Version: 0.1.0b3
+Version: 0.1.0b4
 Summary: Ape SDK for the Silverback platform
 Home-page: https://github.com/SilverBackLtd/sdk
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Description: # Quick Start
```

### Comparing `silverback-0.1.0b3/README.md` & `silverback-0.1.0b4/README.md`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0b3/example.py` & `silverback-0.1.0b4/example.py`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0b3/pyproject.toml` & `silverback-0.1.0b4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0b3/setup.py` & `silverback-0.1.0b4/setup.py`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0b3/silverback/_cli.py` & `silverback-0.1.0b4/silverback/_cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import asyncio
 import os
 
 import click
-from ape.cli import AccountAliasPromptChoice, NetworkBoundCommand, network_option
+from ape.cli import AccountAliasPromptChoice, NetworkBoundCommand, ape_cli_context, network_option
 
 from silverback._importer import import_from_string
 from silverback.runner import LiveRunner
 
 
 @click.group()
 def cli():
     """Work with SilverBack applications in local context (using Ape)."""
 
 
 @cli.command(cls=NetworkBoundCommand)
+@ape_cli_context()
 @network_option()
 @click.option("--account", type=AccountAliasPromptChoice(), default=None)
 @click.option("-x", "--max-exceptions", type=int, default=3)
 @click.argument("path")
 def run(network, account, max_exceptions, path):
     os.environ["SILVERBACK_NETWORK_CHOICE"] = network
```

### Comparing `silverback-0.1.0b3/silverback/_importer.py` & `silverback-0.1.0b4/silverback/_importer.py`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0b3/silverback/application.py` & `silverback-0.1.0b4/silverback/application.py`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0b3/silverback/exceptions.py` & `silverback-0.1.0b4/silverback/exceptions.py`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0b3/silverback/middlewares.py` & `silverback-0.1.0b4/silverback/middlewares.py`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0b3/silverback/runner.py` & `silverback-0.1.0b4/silverback/runner.py`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0b3/silverback/settings.py` & `silverback-0.1.0b4/silverback/settings.py`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0b3/silverback/utils.py` & `silverback-0.1.0b4/silverback/utils.py`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0b3/silverback.egg-info/PKG-INFO` & `silverback-0.1.0b4/silverback.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: silverback
-Version: 0.1.0b3
+Version: 0.1.0b4
 Summary: Ape SDK for the Silverback platform
 Home-page: https://github.com/SilverBackLtd/sdk
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Description: # Quick Start
```

### Comparing `silverback-0.1.0b3/silverback.egg-info/SOURCES.txt` & `silverback-0.1.0b4/silverback.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0b3/silverback.egg-info/requires.txt` & `silverback-0.1.0b4/silverback.egg-info/requires.txt`

 * *Files identical despite different names*

