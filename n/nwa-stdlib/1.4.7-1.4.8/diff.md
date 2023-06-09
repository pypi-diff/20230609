# Comparing `tmp/nwa-stdlib-1.4.7.tar.gz` & `tmp/nwa_stdlib-1.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nwa-stdlib-1.4.7.tar", last modified: Tue May  2 08:30:58 2023, max compression
+gzip compressed data, was "nwa_stdlib-1.4.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `nwa-stdlib-1.4.7.tar` & `nwa_stdlib-1.4.8.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0      362 2023-05-02 08:30:51.328867 nwa-stdlib-1.4.7/.bumpversion.cfg
--rw-r--r--   0        0        0      550 2023-05-02 08:30:51.328867 nwa-stdlib-1.4.7/.github/workflows/publish-release.yaml
--rw-r--r--   0        0        0     1895 2023-05-02 08:30:51.332867 nwa-stdlib-1.4.7/.github/workflows/scheduled-build.yml
--rw-r--r--   0        0        0      807 2023-05-02 08:30:51.332867 nwa-stdlib-1.4.7/.github/workflows/test-package.yaml
--rw-r--r--   0        0        0     1111 2023-05-02 08:30:51.332867 nwa-stdlib-1.4.7/.gitignore
--rw-r--r--   0        0        0     2130 2023-05-02 08:30:51.332867 nwa-stdlib-1.4.7/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1150 2023-05-02 08:30:51.332867 nwa-stdlib-1.4.7/.stignore
--rw-r--r--   0        0        0    11381 2023-05-02 08:30:51.332867 nwa-stdlib-1.4.7/LICENSE
--rw-r--r--   0        0        0      109 2023-05-02 08:30:51.332867 nwa-stdlib-1.4.7/NOTICE
--rw-r--r--   0        0        0     1420 2023-05-02 08:30:51.332867 nwa-stdlib-1.4.7/README.md
--rw-r--r--   0        0        0     1580 2023-05-02 08:30:51.332867 nwa-stdlib-1.4.7/benchmarks/benchmark_async_cache_with_json.py
--rw-r--r--   0        0        0     1724 2023-05-02 08:30:51.332867 nwa-stdlib-1.4.7/benchmarks/benchmark_async_cache_with_orjson.py
--rw-r--r--   0        0        0     1287 2023-05-02 08:30:51.332867 nwa-stdlib-1.4.7/benchmarks/benchmark_async_cache_with_pickle.py
--rw-r--r--   0        0        0      985 2023-05-02 08:30:51.332867 nwa-stdlib-1.4.7/benchmarks/shared.py
--rw-r--r--   0        0        0     2399 2023-05-02 08:30:51.332867 nwa-stdlib-1.4.7/docs/debugging.md
--rw-r--r--   0        0        0      709 2023-05-02 08:30:51.332867 nwa-stdlib-1.4.7/nwastdlib/__init__.py
--rw-r--r--   0        0        0     2609 2023-05-02 08:30:51.332867 nwa-stdlib-1.4.7/nwastdlib/asyncio.py
--rw-r--r--   0        0        0     8098 2023-05-02 08:30:51.332867 nwa-stdlib-1.4.7/nwastdlib/asyncio_cache.py
--rw-r--r--   0        0        0     1796 2023-05-02 08:30:51.332867 nwa-stdlib-1.4.7/nwastdlib/debugging.py
--rw-r--r--   0        0        0     1165 2023-05-02 08:30:51.332867 nwa-stdlib-1.4.7/nwastdlib/ex.py
--rw-r--r--   0        0        0     1096 2023-05-02 08:30:51.332867 nwa-stdlib-1.4.7/nwastdlib/f.py
--rw-r--r--   0        0        0     4237 2023-05-02 08:30:51.332867 nwa-stdlib-1.4.7/nwastdlib/logging.py
--rw-r--r--   0        0        0        0 2023-05-02 08:30:51.332867 nwa-stdlib-1.4.7/nwastdlib/py.typed
--rw-r--r--   0        0        0      803 2023-05-02 08:30:51.332867 nwa-stdlib-1.4.7/nwastdlib/settings.py
--rw-r--r--   0        0        0     3239 2023-05-02 08:30:51.332867 nwa-stdlib-1.4.7/nwastdlib/url.py
--rw-r--r--   0        0        0     1271 2023-05-02 08:30:51.332867 nwa-stdlib-1.4.7/nwastdlib/version.py
--rw-r--r--   0        0        0     2233 2023-05-02 08:30:51.332867 nwa-stdlib-1.4.7/pyproject.toml
--rw-r--r--   0        0        0       35 2023-05-02 08:30:51.332867 nwa-stdlib-1.4.7/requirements/all.txt
--rw-r--r--   0        0        0       78 2023-05-02 08:30:51.332867 nwa-stdlib-1.4.7/requirements/base.txt
--rw-r--r--   0        0        0       36 2023-05-02 08:30:51.332867 nwa-stdlib-1.4.7/requirements/dev.txt
--rw-r--r--   0        0        0      306 2023-05-02 08:30:51.332867 nwa-stdlib-1.4.7/requirements/test.txt
--rw-r--r--   0        0        0     1108 2023-05-02 08:30:51.332867 nwa-stdlib-1.4.7/setup.cfg
--rw-r--r--   0        0        0        0 2023-05-02 08:30:51.332867 nwa-stdlib-1.4.7/tests/__init__.py
--rw-r--r--   0        0        0     1311 2023-05-02 08:30:51.332867 nwa-stdlib-1.4.7/tests/test_asyncio.py
--rw-r--r--   0        0        0     4730 2023-05-02 08:30:51.332867 nwa-stdlib-1.4.7/tests/test_asyncio_cache.py
--rw-r--r--   0        0        0     3716 1970-01-01 00:00:00.000000 nwa-stdlib-1.4.7/PKG-INFO
+-rw-r--r--   0        0        0      363 2023-06-09 14:49:11.246152 nwa_stdlib-1.4.8/.bumpversion.cfg
+-rw-r--r--   0        0        0      550 2023-06-09 14:49:11.246152 nwa_stdlib-1.4.8/.github/workflows/publish-release.yaml
+-rw-r--r--   0        0        0     1895 2023-06-09 14:49:11.246152 nwa_stdlib-1.4.8/.github/workflows/scheduled-build.yml
+-rw-r--r--   0        0        0      807 2023-06-09 14:49:11.246152 nwa_stdlib-1.4.8/.github/workflows/test-package.yaml
+-rw-r--r--   0        0        0     1111 2023-06-09 14:49:11.246152 nwa_stdlib-1.4.8/.gitignore
+-rw-r--r--   0        0        0     2164 2023-06-09 14:49:11.246152 nwa_stdlib-1.4.8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1150 2023-06-09 14:49:11.246152 nwa_stdlib-1.4.8/.stignore
+-rw-r--r--   0        0        0    11381 2023-06-09 14:49:11.246152 nwa_stdlib-1.4.8/LICENSE
+-rw-r--r--   0        0        0      109 2023-06-09 14:49:11.246152 nwa_stdlib-1.4.8/NOTICE
+-rw-r--r--   0        0        0     1420 2023-06-09 14:49:11.246152 nwa_stdlib-1.4.8/README.md
+-rw-r--r--   0        0        0     1580 2023-06-09 14:49:11.246152 nwa_stdlib-1.4.8/benchmarks/benchmark_async_cache_with_json.py
+-rw-r--r--   0        0        0     1724 2023-06-09 14:49:11.246152 nwa_stdlib-1.4.8/benchmarks/benchmark_async_cache_with_orjson.py
+-rw-r--r--   0        0        0     1287 2023-06-09 14:49:11.246152 nwa_stdlib-1.4.8/benchmarks/benchmark_async_cache_with_pickle.py
+-rw-r--r--   0        0        0      985 2023-06-09 14:49:11.246152 nwa_stdlib-1.4.8/benchmarks/shared.py
+-rw-r--r--   0        0        0     2399 2023-06-09 14:49:11.246152 nwa_stdlib-1.4.8/docs/debugging.md
+-rw-r--r--   0        0        0      709 2023-06-09 14:49:11.246152 nwa_stdlib-1.4.8/nwastdlib/__init__.py
+-rw-r--r--   0        0        0     2609 2023-06-09 14:49:11.246152 nwa_stdlib-1.4.8/nwastdlib/asyncio.py
+-rw-r--r--   0        0        0     8098 2023-06-09 14:49:11.246152 nwa_stdlib-1.4.8/nwastdlib/asyncio_cache.py
+-rw-r--r--   0        0        0     1796 2023-06-09 14:49:11.246152 nwa_stdlib-1.4.8/nwastdlib/debugging.py
+-rw-r--r--   0        0        0     1165 2023-06-09 14:49:11.246152 nwa_stdlib-1.4.8/nwastdlib/ex.py
+-rw-r--r--   0        0        0     1096 2023-06-09 14:49:11.246152 nwa_stdlib-1.4.8/nwastdlib/f.py
+-rw-r--r--   0        0        0     4237 2023-06-09 14:49:11.246152 nwa_stdlib-1.4.8/nwastdlib/logging.py
+-rw-r--r--   0        0        0        0 2023-06-09 14:49:11.246152 nwa_stdlib-1.4.8/nwastdlib/py.typed
+-rw-r--r--   0        0        0      803 2023-06-09 14:49:11.246152 nwa_stdlib-1.4.8/nwastdlib/settings.py
+-rw-r--r--   0        0        0     3239 2023-06-09 14:49:11.246152 nwa_stdlib-1.4.8/nwastdlib/url.py
+-rw-r--r--   0        0        0     1271 2023-06-09 14:49:11.246152 nwa_stdlib-1.4.8/nwastdlib/version.py
+-rw-r--r--   0        0        0     2334 2023-06-09 14:49:11.246152 nwa_stdlib-1.4.8/pyproject.toml
+-rw-r--r--   0        0        0       35 2023-06-09 14:49:11.246152 nwa_stdlib-1.4.8/requirements/all.txt
+-rw-r--r--   0        0        0       78 2023-06-09 14:49:11.250152 nwa_stdlib-1.4.8/requirements/base.txt
+-rw-r--r--   0        0        0       36 2023-06-09 14:49:11.250152 nwa_stdlib-1.4.8/requirements/dev.txt
+-rw-r--r--   0        0        0      306 2023-06-09 14:49:11.250152 nwa_stdlib-1.4.8/requirements/test.txt
+-rw-r--r--   0        0        0     1108 2023-06-09 14:49:11.250152 nwa_stdlib-1.4.8/setup.cfg
+-rw-r--r--   0        0        0        0 2023-06-09 14:49:11.250152 nwa_stdlib-1.4.8/tests/__init__.py
+-rw-r--r--   0        0        0     1311 2023-06-09 14:49:11.250152 nwa_stdlib-1.4.8/tests/test_asyncio.py
+-rw-r--r--   0        0        0     4730 2023-06-09 14:49:11.250152 nwa_stdlib-1.4.8/tests/test_asyncio_cache.py
+-rw-r--r--   0        0        0     3752 1970-01-01 00:00:00.000000 nwa_stdlib-1.4.8/PKG-INFO
```

### Comparing `nwa-stdlib-1.4.7/.github/workflows/publish-release.yaml` & `nwa_stdlib-1.4.8/.github/workflows/publish-release.yaml`

 * *Files identical despite different names*

### Comparing `nwa-stdlib-1.4.7/.github/workflows/scheduled-build.yml` & `nwa_stdlib-1.4.8/.github/workflows/scheduled-build.yml`

 * *Files identical despite different names*

### Comparing `nwa-stdlib-1.4.7/.github/workflows/test-package.yaml` & `nwa_stdlib-1.4.8/.github/workflows/test-package.yaml`

 * *Files identical despite different names*

### Comparing `nwa-stdlib-1.4.7/.gitignore` & `nwa_stdlib-1.4.8/.gitignore`

 * *Files identical despite different names*

### Comparing `nwa-stdlib-1.4.7/.pre-commit-config.yaml` & `nwa_stdlib-1.4.8/.pre-commit-config.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     hooks:
       - id: blacken-docs
         additional_dependencies: [black==22.1.0]
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.4.0
     hooks:
       - id: trailing-whitespace
+        exclude: .bumpversion.cfg
       - id: end-of-file-fixer
       - id: check-docstring-first
       - id: check-json
       - id: check-yaml
         exclude: (charts/*|.gitlab-ci.yml)
       - id: debug-statements
       - id: requirements-txt-fixer
```

### Comparing `nwa-stdlib-1.4.7/.stignore` & `nwa_stdlib-1.4.8/.stignore`

 * *Files identical despite different names*

### Comparing `nwa-stdlib-1.4.7/LICENSE` & `nwa_stdlib-1.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nwa-stdlib-1.4.7/README.md` & `nwa_stdlib-1.4.8/README.md`

 * *Files identical despite different names*

### Comparing `nwa-stdlib-1.4.7/benchmarks/benchmark_async_cache_with_json.py` & `nwa_stdlib-1.4.8/benchmarks/benchmark_async_cache_with_json.py`

 * *Files identical despite different names*

### Comparing `nwa-stdlib-1.4.7/benchmarks/benchmark_async_cache_with_orjson.py` & `nwa_stdlib-1.4.8/benchmarks/benchmark_async_cache_with_orjson.py`

 * *Files identical despite different names*

### Comparing `nwa-stdlib-1.4.7/benchmarks/benchmark_async_cache_with_pickle.py` & `nwa_stdlib-1.4.8/benchmarks/benchmark_async_cache_with_pickle.py`

 * *Files identical despite different names*

### Comparing `nwa-stdlib-1.4.7/benchmarks/shared.py` & `nwa_stdlib-1.4.8/benchmarks/shared.py`

 * *Files identical despite different names*

### Comparing `nwa-stdlib-1.4.7/docs/debugging.md` & `nwa_stdlib-1.4.8/docs/debugging.md`

 * *Files identical despite different names*

### Comparing `nwa-stdlib-1.4.7/nwastdlib/__init__.py` & `nwa_stdlib-1.4.8/nwastdlib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,12 +9,12 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 """The NWA-stdlib module."""
 
-__version__ = "1.4.7"
+__version__ = "1.4.8"
 
 from nwastdlib.f import const, identity
 
 __all__ = ["const", "identity"]
```

### Comparing `nwa-stdlib-1.4.7/nwastdlib/asyncio.py` & `nwa_stdlib-1.4.8/nwastdlib/asyncio.py`

 * *Files identical despite different names*

### Comparing `nwa-stdlib-1.4.7/nwastdlib/asyncio_cache.py` & `nwa_stdlib-1.4.8/nwastdlib/asyncio_cache.py`

 * *Files identical despite different names*

### Comparing `nwa-stdlib-1.4.7/nwastdlib/debugging.py` & `nwa_stdlib-1.4.8/nwastdlib/debugging.py`

 * *Files identical despite different names*

### Comparing `nwa-stdlib-1.4.7/nwastdlib/ex.py` & `nwa_stdlib-1.4.8/nwastdlib/ex.py`

 * *Files identical despite different names*

### Comparing `nwa-stdlib-1.4.7/nwastdlib/f.py` & `nwa_stdlib-1.4.8/nwastdlib/f.py`

 * *Files identical despite different names*

### Comparing `nwa-stdlib-1.4.7/nwastdlib/logging.py` & `nwa_stdlib-1.4.8/nwastdlib/logging.py`

 * *Files identical despite different names*

### Comparing `nwa-stdlib-1.4.7/nwastdlib/settings.py` & `nwa_stdlib-1.4.8/nwastdlib/settings.py`

 * *Files identical despite different names*

### Comparing `nwa-stdlib-1.4.7/nwastdlib/url.py` & `nwa_stdlib-1.4.8/nwastdlib/url.py`

 * *Files identical despite different names*

### Comparing `nwa-stdlib-1.4.7/nwastdlib/version.py` & `nwa_stdlib-1.4.8/nwastdlib/version.py`

 * *Files identical despite different names*

### Comparing `nwa-stdlib-1.4.7/pyproject.toml` & `nwa_stdlib-1.4.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -28,15 +28,16 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.9",
 ]
 requires = [
     "structlog~=22.1.0",
     "colorama~=0.4.3",
-    "redis~=4.4.2"
+    "redis>=4.5.3, <4.6.0",  # Required for anyio 3.7 https://github.com/redis/redis-py/issues/2633
+    "anyio>=3.7.0",
 ]
 description-file = "README.md"
 requires-python = ">=3.9"
 
 [tool.flit.metadata.urls]
 Documentation = "https://workfloworchestrator.org/"
```

### Comparing `nwa-stdlib-1.4.7/setup.cfg` & `nwa_stdlib-1.4.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `nwa-stdlib-1.4.7/tests/test_asyncio.py` & `nwa_stdlib-1.4.8/tests/test_asyncio.py`

 * *Files identical despite different names*

### Comparing `nwa-stdlib-1.4.7/tests/test_asyncio_cache.py` & `nwa_stdlib-1.4.8/tests/test_asyncio_cache.py`

 * *Files identical despite different names*

### Comparing `nwa-stdlib-1.4.7/PKG-INFO` & `nwa_stdlib-1.4.8/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwa-stdlib
-Version: 1.4.7
+Version: 1.4.8
 Summary: The NWA-stdlib module.
 Home-page: https://github.com/workfloworchestrator/nwa-stdlib
 Author: SURF
 Author-email: automation-beheer@surf.nl
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
@@ -24,15 +24,16 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: structlog~=22.1.0
 Requires-Dist: colorama~=0.4.3
-Requires-Dist: redis~=4.4.2
+Requires-Dist: redis>=4.5.3, <4.6.0
+Requires-Dist: anyio>=3.7.0
 Requires-Dist: bumpversion ; extra == "dev"
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: types-redis ; extra == "dev"
 Requires-Dist: anyio ; extra == "test"
 Requires-Dist: black ; extra == "test"
 Requires-Dist: fakeredis ; extra == "test"
 Requires-Dist: flake8 ; extra == "test"
```

