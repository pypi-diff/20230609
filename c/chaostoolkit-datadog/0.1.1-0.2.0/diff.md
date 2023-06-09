# Comparing `tmp/chaostoolkit-datadog-0.1.1.tar.gz` & `tmp/chaostoolkit-datadog-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/chaostoolkit-datadog-0.1.1.tar", last modified: Fri Nov 18 13:16:33 2022, max compression
+gzip compressed data, was "dist/chaostoolkit-datadog-0.2.0.tar", last modified: Fri Jun  9 08:42:27 2023, max compression
```

## Comparing `chaostoolkit-datadog-0.1.1.tar` & `chaostoolkit-datadog-0.2.0.tar`

### file list

```diff
@@ -1,31 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-18 13:16:33.000000 chaostoolkit-datadog-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-18 13:16:33.000000 chaostoolkit-datadog-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-18 13:16:33.000000 chaostoolkit-datadog-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     1261 2022-11-18 13:16:09.000000 chaostoolkit-datadog-0.1.1/.github/workflows/build.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      903 2022-11-18 13:16:09.000000 chaostoolkit-datadog-0.1.1/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1206 2022-11-18 13:16:09.000000 chaostoolkit-datadog-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)      431 2022-11-18 13:16:09.000000 chaostoolkit-datadog-0.1.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2022-11-18 13:16:09.000000 chaostoolkit-datadog-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      108 2022-11-18 13:16:09.000000 chaostoolkit-datadog-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      562 2022-11-18 13:16:09.000000 chaostoolkit-datadog-0.1.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)     4980 2022-11-18 13:16:33.000000 chaostoolkit-datadog-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3608 2022-11-18 13:16:09.000000 chaostoolkit-datadog-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-18 13:16:33.000000 chaostoolkit-datadog-0.1.1/chaosdatadog/
--rw-r--r--   0 runner    (1001) docker     (122)     1852 2022-11-18 13:16:09.000000 chaostoolkit-datadog-0.1.1/chaosdatadog/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-18 13:16:33.000000 chaostoolkit-datadog-0.1.1/chaosdatadog/slo/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-18 13:16:09.000000 chaostoolkit-datadog-0.1.1/chaosdatadog/slo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2112 2022-11-18 13:16:09.000000 chaostoolkit-datadog-0.1.1/chaosdatadog/slo/probes.py
--rw-r--r--   0 runner    (1001) docker     (122)     1046 2022-11-18 13:16:09.000000 chaostoolkit-datadog-0.1.1/chaosdatadog/slo/tolerances.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-18 13:16:33.000000 chaostoolkit-datadog-0.1.1/chaostoolkit_datadog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4980 2022-11-18 13:16:33.000000 chaostoolkit-datadog-0.1.1/chaostoolkit_datadog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      546 2022-11-18 13:16:33.000000 chaostoolkit-datadog-0.1.1/chaostoolkit_datadog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-18 13:16:33.000000 chaostoolkit-datadog-0.1.1/chaostoolkit_datadog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       48 2022-11-18 13:16:33.000000 chaostoolkit-datadog-0.1.1/chaostoolkit_datadog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2022-11-18 13:16:33.000000 chaostoolkit-datadog-0.1.1/chaostoolkit_datadog.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      174 2022-11-18 13:16:09.000000 chaostoolkit-datadog-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      118 2022-11-18 13:16:09.000000 chaostoolkit-datadog-0.1.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (122)       47 2022-11-18 13:16:09.000000 chaostoolkit-datadog-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2035 2022-11-18 13:16:33.000000 chaostoolkit-datadog-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      737 2022-11-18 13:16:09.000000 chaostoolkit-datadog-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-18 13:16:33.000000 chaostoolkit-datadog-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      541 2022-11-18 13:16:09.000000 chaostoolkit-datadog-0.1.1/tests/test_probes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:42:27.000000 chaostoolkit-datadog-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:42:27.000000 chaostoolkit-datadog-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:42:27.000000 chaostoolkit-datadog-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-09 08:42:05.000000 chaostoolkit-datadog-0.2.0/.github/workflows/build.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-09 08:42:05.000000 chaostoolkit-datadog-0.2.0/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-09 08:42:05.000000 chaostoolkit-datadog-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-09 08:42:05.000000 chaostoolkit-datadog-0.2.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-09 08:42:05.000000 chaostoolkit-datadog-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-09 08:42:05.000000 chaostoolkit-datadog-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-09 08:42:05.000000 chaostoolkit-datadog-0.2.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-06-09 08:42:27.000000 chaostoolkit-datadog-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-06-09 08:42:05.000000 chaostoolkit-datadog-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:42:27.000000 chaostoolkit-datadog-0.2.0/chaosdatadog/
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-06-09 08:42:05.000000 chaostoolkit-datadog-0.2.0/chaosdatadog/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:42:27.000000 chaostoolkit-datadog-0.2.0/chaosdatadog/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 08:42:05.000000 chaostoolkit-datadog-0.2.0/chaosdatadog/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-06-09 08:42:05.000000 chaostoolkit-datadog-0.2.0/chaosdatadog/metrics/probes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-09 08:42:05.000000 chaostoolkit-datadog-0.2.0/chaosdatadog/metrics/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:42:27.000000 chaostoolkit-datadog-0.2.0/chaosdatadog/slo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 08:42:05.000000 chaostoolkit-datadog-0.2.0/chaosdatadog/slo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-06-09 08:42:05.000000 chaostoolkit-datadog-0.2.0/chaosdatadog/slo/probes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-06-09 08:42:05.000000 chaostoolkit-datadog-0.2.0/chaosdatadog/slo/tolerances.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:42:27.000000 chaostoolkit-datadog-0.2.0/chaostoolkit_datadog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-06-09 08:42:27.000000 chaostoolkit-datadog-0.2.0/chaostoolkit_datadog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-09 08:42:27.000000 chaostoolkit-datadog-0.2.0/chaostoolkit_datadog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 08:42:27.000000 chaostoolkit-datadog-0.2.0/chaostoolkit_datadog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-09 08:42:27.000000 chaostoolkit-datadog-0.2.0/chaostoolkit_datadog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-09 08:42:27.000000 chaostoolkit-datadog-0.2.0/chaostoolkit_datadog.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-09 08:42:05.000000 chaostoolkit-datadog-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-09 08:42:05.000000 chaostoolkit-datadog-0.2.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-09 08:42:05.000000 chaostoolkit-datadog-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-09 08:42:27.000000 chaostoolkit-datadog-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-09 08:42:05.000000 chaostoolkit-datadog-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:42:27.000000 chaostoolkit-datadog-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-06-09 08:42:05.000000 chaostoolkit-datadog-0.2.0/tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-09 08:42:05.000000 chaostoolkit-datadog-0.2.0/tests/test_probes.py
```

### Comparing `chaostoolkit-datadog-0.1.1/.github/workflows/build.yaml` & `chaostoolkit-datadog-0.2.0/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `chaostoolkit-datadog-0.1.1/.github/workflows/release.yaml` & `chaostoolkit-datadog-0.2.0/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `chaostoolkit-datadog-0.1.1/.gitignore` & `chaostoolkit-datadog-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `chaostoolkit-datadog-0.1.1/LICENSE` & `chaostoolkit-datadog-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chaostoolkit-datadog-0.1.1/Makefile` & `chaostoolkit-datadog-0.2.0/Makefile`

 * *Files identical despite different names*

### Comparing `chaostoolkit-datadog-0.1.1/PKG-INFO` & `chaostoolkit-datadog-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chaostoolkit-datadog
-Version: 0.1.1
+Version: 0.2.0
 Summary: Chaos Toolkit extension for DataDog
 Home-page: https://chaostoolkit.org
 Author: Chaos Toolkit
 Author-email: contact@chaostoolkit.org
 License: Apache License Version 2.0
 Project-URL: Docs: RTD, https://chaostoolkit.org/drivers/datadog/
 Project-URL: CI: GitHub, https://github.com/chaostoolkit-incubator/chaostoolkit-datadog/actions
@@ -29,15 +29,15 @@
 License-File: LICENSE
 
 # Chaos Toolkit Extension Template
 
 [![Version](https://img.shields.io/pypi/v/chaostoolkit-datadog.svg)](https://img.shields.io/pypi/v/chaostoolkit-datadog.svg)
 [![License](https://img.shields.io/pypi/l/chaostoolkit-datadog.svg)](https://img.shields.io/pypi/l/chaostoolkit-datadog.svg)
 
-![Build](https://github.com/chaostoolkit-incubator/chaostoolkit-datadog/workflows/Build/badge.svg)
+[![Build, Test, and Lint](https://github.com/chaostoolkit-incubator/chaostoolkit-datadog/actions/workflows/build.yaml/badge.svg)](https://github.com/chaostoolkit-incubator/chaostoolkit-datadog/actions/workflows/build.yaml)
 [![Python versions](https://img.shields.io/pypi/pyversions/chaostoolkit-datadog.svg)](https://www.python.org/)
 
 This project contains Chaos Toolkit activities and tolerances to work
 with DataDog.
 
 ## Install
```

### Comparing `chaostoolkit-datadog-0.1.1/README.md` & `chaostoolkit-datadog-0.2.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Chaos Toolkit Extension Template
 
 [![Version](https://img.shields.io/pypi/v/chaostoolkit-datadog.svg)](https://img.shields.io/pypi/v/chaostoolkit-datadog.svg)
 [![License](https://img.shields.io/pypi/l/chaostoolkit-datadog.svg)](https://img.shields.io/pypi/l/chaostoolkit-datadog.svg)
 
-![Build](https://github.com/chaostoolkit-incubator/chaostoolkit-datadog/workflows/Build/badge.svg)
+[![Build, Test, and Lint](https://github.com/chaostoolkit-incubator/chaostoolkit-datadog/actions/workflows/build.yaml/badge.svg)](https://github.com/chaostoolkit-incubator/chaostoolkit-datadog/actions/workflows/build.yaml)
 [![Python versions](https://img.shields.io/pypi/pyversions/chaostoolkit-datadog.svg)](https://www.python.org/)
 
 This project contains Chaos Toolkit activities and tolerances to work
 with DataDog.
 
 ## Install
```

### Comparing `chaostoolkit-datadog-0.1.1/chaosdatadog/__init__.py` & `chaostoolkit-datadog-0.2.0/chaosdatadog/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Discovery,
     Secrets,
 )
 from datadog_api_client import ApiClient
 from datadog_api_client import Configuration as DDCfg
 from logzero import logger
 
-__version__ = "0.1.1"
+__version__ = "0.2.0"
 
 
 @contextmanager
 def get_client(
     configuration: Configuration = None, secrets: Secrets = None, **kwargs
 ) -> Generator[ApiClient, None, None]:
     configuration = configuration or {}
@@ -59,9 +59,10 @@
     """
     Extract metadata from actions, probes and tolerances
     exposed by this extension.
     """
     activities = []  # type: ignore
 
     activities.extend(discover_probes("chaosdatadog.slo.probes"))
+    activities.extend(discover_probes("chaosdatadog.metrics.probes"))
 
     return activities
```

### Comparing `chaostoolkit-datadog-0.1.1/chaosdatadog/slo/probes.py` & `chaostoolkit-datadog-0.2.0/chaosdatadog/slo/probes.py`

 * *Files identical despite different names*

### Comparing `chaostoolkit-datadog-0.1.1/chaosdatadog/slo/tolerances.py` & `chaostoolkit-datadog-0.2.0/chaosdatadog/slo/tolerances.py`

 * *Files identical despite different names*

### Comparing `chaostoolkit-datadog-0.1.1/chaostoolkit_datadog.egg-info/PKG-INFO` & `chaostoolkit-datadog-0.2.0/chaostoolkit_datadog.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chaostoolkit-datadog
-Version: 0.1.1
+Version: 0.2.0
 Summary: Chaos Toolkit extension for DataDog
 Home-page: https://chaostoolkit.org
 Author: Chaos Toolkit
 Author-email: contact@chaostoolkit.org
 License: Apache License Version 2.0
 Project-URL: Docs: RTD, https://chaostoolkit.org/drivers/datadog/
 Project-URL: CI: GitHub, https://github.com/chaostoolkit-incubator/chaostoolkit-datadog/actions
@@ -29,15 +29,15 @@
 License-File: LICENSE
 
 # Chaos Toolkit Extension Template
 
 [![Version](https://img.shields.io/pypi/v/chaostoolkit-datadog.svg)](https://img.shields.io/pypi/v/chaostoolkit-datadog.svg)
 [![License](https://img.shields.io/pypi/l/chaostoolkit-datadog.svg)](https://img.shields.io/pypi/l/chaostoolkit-datadog.svg)
 
-![Build](https://github.com/chaostoolkit-incubator/chaostoolkit-datadog/workflows/Build/badge.svg)
+[![Build, Test, and Lint](https://github.com/chaostoolkit-incubator/chaostoolkit-datadog/actions/workflows/build.yaml/badge.svg)](https://github.com/chaostoolkit-incubator/chaostoolkit-datadog/actions/workflows/build.yaml)
 [![Python versions](https://img.shields.io/pypi/pyversions/chaostoolkit-datadog.svg)](https://www.python.org/)
 
 This project contains Chaos Toolkit activities and tolerances to work
 with DataDog.
 
 ## Install
```

### Comparing `chaostoolkit-datadog-0.1.1/chaostoolkit_datadog.egg-info/SOURCES.txt` & `chaostoolkit-datadog-0.2.0/chaostoolkit_datadog.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -8,16 +8,20 @@
 requirements-dev.txt
 requirements.txt
 setup.cfg
 setup.py
 .github/workflows/build.yaml
 .github/workflows/release.yaml
 chaosdatadog/__init__.py
+chaosdatadog/metrics/__init__.py
+chaosdatadog/metrics/probes.py
+chaosdatadog/metrics/utils.py
 chaosdatadog/slo/__init__.py
 chaosdatadog/slo/probes.py
 chaosdatadog/slo/tolerances.py
 chaostoolkit_datadog.egg-info/PKG-INFO
 chaostoolkit_datadog.egg-info/SOURCES.txt
 chaostoolkit_datadog.egg-info/dependency_links.txt
 chaostoolkit_datadog.egg-info/requires.txt
 chaostoolkit_datadog.egg-info/top_level.txt
+tests/test_metrics.py
 tests/test_probes.py
```

### Comparing `chaostoolkit-datadog-0.1.1/setup.cfg` & `chaostoolkit-datadog-0.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `chaostoolkit-datadog-0.1.1/setup.py` & `chaostoolkit-datadog-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `chaostoolkit-datadog-0.1.1/tests/test_probes.py` & `chaostoolkit-datadog-0.2.0/tests/test_probes.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from chaosdatadog.slo.probes import get_slo
 
 
 @patch("datadog_api_client.api_client.rest", autospec=False)
 def test_get_slo(rest):
     r = MagicMock()
     r.getheader.return_value = None
+    r.headers = {"Content-Type": "application/json"}
     r.data = json.dumps({}).encode("utf-8")
     cl = MagicMock()
     cl.request.return_value = r
     cl.configuration.unstable_operations = {"get_slo_history": False}
     rest.RESTClientObject.return_value = cl
 
     results = get_slo(slo_id="slo1")
```

