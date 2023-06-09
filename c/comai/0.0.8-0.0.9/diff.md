# Comparing `tmp/comai-0.0.8.tar.gz` & `tmp/comai-0.0.9.tar.gz`

## Comparing `comai-0.0.8.tar` & `comai-0.0.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 comai-0.0.8/.github/workflows/release.yml
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 comai-0.0.8/.github/workflows/tests.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 comai-0.0.8/src/comai/__init__.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 comai-0.0.8/src/comai/__main__.py
--rwxr-xr-x   0        0        0     2672 2020-02-02 00:00:00.000000 comai-0.0.8/src/comai/cli.py
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 comai-0.0.8/src/comai/config.py
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 comai-0.0.8/tests/test_comai.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 comai-0.0.8/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 comai-0.0.8/LICENSE
--rw-r--r--   0        0        0     2306 2020-02-02 00:00:00.000000 comai-0.0.8/README.md
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 comai-0.0.8/pyproject.toml
--rw-r--r--   0        0        0    43802 2020-02-02 00:00:00.000000 comai-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 comai-0.0.9/.github/workflows/release.yml
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 comai-0.0.9/.github/workflows/tests.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 comai-0.0.9/src/comai/__init__.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 comai-0.0.9/src/comai/__main__.py
+-rwxr-xr-x   0        0        0     2672 2020-02-02 00:00:00.000000 comai-0.0.9/src/comai/cli.py
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 comai-0.0.9/src/comai/config.py
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 comai-0.0.9/tests/test_comai.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 comai-0.0.9/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 comai-0.0.9/LICENSE
+-rw-r--r--   0        0        0     2984 2020-02-02 00:00:00.000000 comai-0.0.9/README.md
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 comai-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0    44480 2020-02-02 00:00:00.000000 comai-0.0.9/PKG-INFO
```

### Comparing `comai-0.0.8/.github/workflows/release.yml` & `comai-0.0.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `comai-0.0.8/.github/workflows/tests.yml` & `comai-0.0.9/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `comai-0.0.8/src/comai/cli.py` & `comai-0.0.9/src/comai/cli.py`

 * *Files identical despite different names*

### Comparing `comai-0.0.8/src/comai/config.py` & `comai-0.0.9/src/comai/config.py`

 * *Files identical despite different names*

### Comparing `comai-0.0.8/tests/test_comai.py` & `comai-0.0.9/tests/test_comai.py`

 * *Files identical despite different names*

### Comparing `comai-0.0.8/LICENSE` & `comai-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `comai-0.0.8/pyproject.toml` & `comai-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `comai-0.0.8/PKG-INFO` & `comai-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comai
-Version: 0.0.8
+Version: 0.0.9
 Summary: AI powered console assistant
 Project-URL: homepage, https://github.com/ricopinazo/comai
 Project-URL: repository, https://github.com/ricopinazo/comai
 Project-URL: issues, https://github.com/ricopinazo/comai/issues
 Author-email: Pedro Rico <ricopinazo@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
@@ -696,14 +696,29 @@
 Requires-Dist: hatchling; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: python-dotenv; extra == 'test'
 Description-Content-Type: text/markdown
 
 # Comai - The AI powered terminal assistant
 
+<p align="left">
+<a href="https://github.com/ricopinazo/comai/actions/workflows/tests.yml/badge.svg">
+<img alt="Test and Build" src="https://github.com/ricopinazo/comai/actions/workflows/tests.yml/badge.svg" />
+</a>
+<a href="https://github.com/ricopinazo/comai/releases">
+<img alt="Latest Release" src="https://img.shields.io/github/v/release/ricopinazo/comai?color=brightgreen&include_prereleases" />
+</a>
+<a href="https://pypi.org/project/comai/">
+<img alt="PyPI" src="https://img.shields.io/pypi/v/comai">
+</a>
+<a href="https://github.com/ricopinazo/comai/issues">
+<img alt="Issues" src="https://img.shields.io/github/issues/ricopinazo/comai?color=brightgreen" />
+</a>
+</p>
+
 `comai` is an open source terminal assistant powered by OpenAI API that enables you to interact with your command line interface using natural language instructions. It simplifies your workflow by converting natural language queries into executable commands. No more memorizing complex syntax. Just chat with `comai` using plain English!
 
 ## Installation 🚀
 
 Getting `comai` up and running is a breeze. Simply use `pip` to install the latest tested version:
 
 ```shell
```

