# Comparing `tmp/ez_cqrs-1.1.3.tar.gz` & `tmp/ez_cqrs-1.1.4.tar.gz`

## Comparing `ez_cqrs-1.1.3.tar` & `ez_cqrs-1.1.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 ez_cqrs-1.1.3/.tool-versions
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 ez_cqrs-1.1.3/mkdocs.yml
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 ez_cqrs-1.1.3/.github/CODEOWNERS
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 ez_cqrs-1.1.3/.github/workflows/release.yml
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 ez_cqrs-1.1.3/.github/workflows/test.yml
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 ez_cqrs-1.1.3/.vscode/settings.json
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 ez_cqrs-1.1.3/docs/index.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-1.1.3/ez_cqrs/__init__.py
--rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 ez_cqrs-1.1.3/ez_cqrs/acid_exec.py
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 ez_cqrs-1.1.3/ez_cqrs/components.py
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 ez_cqrs-1.1.3/ez_cqrs/error.py
--rw-r--r--   0        0        0     2095 2020-02-02 00:00:00.000000 ez_cqrs-1.1.3/ez_cqrs/framework.py
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 ez_cqrs-1.1.3/ez_cqrs/handler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-1.1.3/ez_cqrs/py.typed
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 ez_cqrs-1.1.3/ez_cqrs/shared_state.py
--rw-r--r--   0        0        0     4144 2020-02-02 00:00:00.000000 ez_cqrs-1.1.3/ez_cqrs/testing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-1.1.3/ez_cqrs/utilities/__init__.py
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 ez_cqrs-1.1.3/ez_cqrs/utilities/cli.py
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 ez_cqrs-1.1.3/requirements/core.txt
--rw-r--r--   0        0        0     4063 2020-02-02 00:00:00.000000 ez_cqrs-1.1.3/requirements/dev.txt
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 ez_cqrs-1.1.3/scripts/new_release.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-1.1.3/tests/__init__.py
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 ez_cqrs-1.1.3/tests/integration/conftest.py
--rw-r--r--   0        0        0     7818 2020-02-02 00:00:00.000000 ez_cqrs-1.1.3/tests/integration/test_execution.py
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 ez_cqrs-1.1.3/tests/unit/test_acid_exec.py
--rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 ez_cqrs-1.1.3/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 ez_cqrs-1.1.3/LICENSE
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 ez_cqrs-1.1.3/README.md
--rw-r--r--   0        0        0     2585 2020-02-02 00:00:00.000000 ez_cqrs-1.1.3/pyproject.toml
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 ez_cqrs-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 ez_cqrs-1.1.4/.tool-versions
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 ez_cqrs-1.1.4/mkdocs.yml
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 ez_cqrs-1.1.4/.github/CODEOWNERS
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 ez_cqrs-1.1.4/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 ez_cqrs-1.1.4/.github/workflows/test.yml
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 ez_cqrs-1.1.4/.vscode/settings.json
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 ez_cqrs-1.1.4/docs/index.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-1.1.4/ez_cqrs/__init__.py
+-rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 ez_cqrs-1.1.4/ez_cqrs/acid_exec.py
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 ez_cqrs-1.1.4/ez_cqrs/components.py
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 ez_cqrs-1.1.4/ez_cqrs/error.py
+-rw-r--r--   0        0        0     2095 2020-02-02 00:00:00.000000 ez_cqrs-1.1.4/ez_cqrs/framework.py
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 ez_cqrs-1.1.4/ez_cqrs/handler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-1.1.4/ez_cqrs/py.typed
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 ez_cqrs-1.1.4/ez_cqrs/shared_state.py
+-rw-r--r--   0        0        0     4144 2020-02-02 00:00:00.000000 ez_cqrs-1.1.4/ez_cqrs/testing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-1.1.4/ez_cqrs/utilities/__init__.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 ez_cqrs-1.1.4/ez_cqrs/utilities/cli.py
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 ez_cqrs-1.1.4/requirements/core.txt
+-rw-r--r--   0        0        0     4063 2020-02-02 00:00:00.000000 ez_cqrs-1.1.4/requirements/dev.txt
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 ez_cqrs-1.1.4/scripts/new_release.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-1.1.4/tests/__init__.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 ez_cqrs-1.1.4/tests/integration/conftest.py
+-rw-r--r--   0        0        0     7818 2020-02-02 00:00:00.000000 ez_cqrs-1.1.4/tests/integration/test_execution.py
+-rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 ez_cqrs-1.1.4/tests/unit/test_acid_exec.py
+-rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 ez_cqrs-1.1.4/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 ez_cqrs-1.1.4/LICENSE
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 ez_cqrs-1.1.4/README.md
+-rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 ez_cqrs-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 ez_cqrs-1.1.4/PKG-INFO
```

### Comparing `ez_cqrs-1.1.3/.github/workflows/release.yml` & `ez_cqrs-1.1.4/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.1.3/.github/workflows/test.yml` & `ez_cqrs-1.1.4/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.1.3/.vscode/settings.json` & `ez_cqrs-1.1.4/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.1.3/ez_cqrs/acid_exec.py` & `ez_cqrs-1.1.4/ez_cqrs/acid_exec.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.1.3/ez_cqrs/components.py` & `ez_cqrs-1.1.4/ez_cqrs/components.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.1.3/ez_cqrs/error.py` & `ez_cqrs-1.1.4/ez_cqrs/error.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.1.3/ez_cqrs/framework.py` & `ez_cqrs-1.1.4/ez_cqrs/framework.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.1.3/ez_cqrs/handler.py` & `ez_cqrs-1.1.4/ez_cqrs/handler.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.1.3/ez_cqrs/shared_state.py` & `ez_cqrs-1.1.4/ez_cqrs/shared_state.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.1.3/ez_cqrs/testing.py` & `ez_cqrs-1.1.4/ez_cqrs/testing.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.1.3/requirements/core.txt` & `ez_cqrs-1.1.4/requirements/core.txt`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.1.3/requirements/dev.txt` & `ez_cqrs-1.1.4/requirements/dev.txt`

 * *Files 0% similar despite different names*

```diff
@@ -122,15 +122,15 @@
     #   rich
 pymdown-extensions==10.0.1
     # via mkdocs-material
 pyparsing==3.0.9
     # via pip-requirements-parser
 pyproject-hooks==1.0.0
     # via build
-pyrgo==0.2.5
+pyrgo==0.3.0
     # via ez_cqrs (pyproject.toml)
 pytest==7.3.1
     # via
     #   pyrgo
     #   pytest-asyncio
     #   pytest-cov
 pytest-asyncio==0.21.0
```

### Comparing `ez_cqrs-1.1.3/scripts/new_release.py` & `ez_cqrs-1.1.4/scripts/new_release.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.1.3/tests/integration/conftest.py` & `ez_cqrs-1.1.4/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.1.3/tests/integration/test_execution.py` & `ez_cqrs-1.1.4/tests/integration/test_execution.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.1.3/tests/unit/test_acid_exec.py` & `ez_cqrs-1.1.4/tests/unit/test_acid_exec.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.1.3/.gitignore` & `ez_cqrs-1.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.1.3/LICENSE` & `ez_cqrs-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.1.3/pyproject.toml` & `ez_cqrs-1.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ez_cqrs"
-version = "1.1.3"
+version = "1.1.4"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 authors = [
@@ -18,15 +18,15 @@
     "mashumaro[orjson]",
     "result",
     "pydantic"
 ]
 
 [project.optional-dependencies]
 dev = [
-    "pyrgo",
+    "pyrgo>=0.3.0",
     "pytest-cov",
     "pytest-asyncio",
 ]
 
 [project.urls]
 Documentation = "https://github.com/Tomperez98/ez-cqrs#readme"
 Issues = "https://github.com/Tomperez98/ez-cqrs/issues"
```

### Comparing `ez_cqrs-1.1.3/PKG-INFO` & `ez_cqrs-1.1.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: ez_cqrs
-Version: 1.1.3
+Version: 1.1.4
 Project-URL: Documentation, https://github.com/Tomperez98/ez-cqrs#readme
 Project-URL: Issues, https://github.com/Tomperez98/ez-cqrs/issues
 Project-URL: Source, https://github.com/Tomperez98/ez-cqrs
 Author-email: Tomas Perez Alvarez <tomasperezalvarez@gmail.com>
 License-File: LICENSE
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Requires-Dist: mashumaro[orjson]
 Requires-Dist: pydantic
 Requires-Dist: result
 Provides-Extra: dev
-Requires-Dist: pyrgo; extra == 'dev'
+Requires-Dist: pyrgo>=0.3.0; extra == 'dev'
 Requires-Dist: pytest-asyncio; extra == 'dev'
 Requires-Dist: pytest-cov; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # ez-cqrs
 
 A lightweight, opinionated framework to write software in a procedural way.
```

