# Comparing `tmp/pytest-typhoon-xray-0.4.7.tar.gz` & `tmp/pytest-typhoon-xray-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-typhoon-xray-0.4.7.tar", last modified: Fri Nov  4 12:27:19 2022, max compression
+gzip compressed data, was "pytest-typhoon-xray-1.0.0.tar", last modified: Fri Jun  9 18:04:20 2023, max compression
```

## Comparing `pytest-typhoon-xray-0.4.7.tar` & `pytest-typhoon-xray-1.0.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 branko     (501) staff       (20)        0 2022-11-04 12:27:19.004866 pytest-typhoon-xray-0.4.7/
--rw-r--r--   0 branko     (501) staff       (20)     1068 2021-03-09 10:50:41.000000 pytest-typhoon-xray-0.4.7/LICENSE
--rw-r--r--   0 branko     (501) staff       (20)       97 2021-03-09 10:50:41.000000 pytest-typhoon-xray-0.4.7/MANIFEST.in
--rw-r--r--   0 branko     (501) staff       (20)     6875 2022-11-04 12:27:19.004710 pytest-typhoon-xray-0.4.7/PKG-INFO
--rw-r--r--   0 branko     (501) staff       (20)     5842 2022-03-28 08:12:31.000000 pytest-typhoon-xray-0.4.7/README.rst
-drwxr-xr-x   0 branko     (501) staff       (20)        0 2022-11-04 12:27:19.003279 pytest-typhoon-xray-0.4.7/pytest_typhoon_xray.egg-info/
--rw-r--r--   0 branko     (501) staff       (20)     6875 2022-11-04 12:27:18.000000 pytest-typhoon-xray-0.4.7/pytest_typhoon_xray.egg-info/PKG-INFO
--rw-r--r--   0 branko     (501) staff       (20)      418 2022-11-04 12:27:19.000000 pytest-typhoon-xray-0.4.7/pytest_typhoon_xray.egg-info/SOURCES.txt
--rw-r--r--   0 branko     (501) staff       (20)        1 2022-11-04 12:27:18.000000 pytest-typhoon-xray-0.4.7/pytest_typhoon_xray.egg-info/dependency_links.txt
--rw-r--r--   0 branko     (501) staff       (20)       34 2022-11-04 12:27:18.000000 pytest-typhoon-xray-0.4.7/pytest_typhoon_xray.egg-info/entry_points.txt
--rw-r--r--   0 branko     (501) staff       (20)       55 2022-11-04 12:27:18.000000 pytest-typhoon-xray-0.4.7/pytest_typhoon_xray.egg-info/requires.txt
--rw-r--r--   0 branko     (501) staff       (20)        7 2022-11-04 12:27:18.000000 pytest-typhoon-xray-0.4.7/pytest_typhoon_xray.egg-info/top_level.txt
--rw-r--r--   0 branko     (501) staff       (20)       38 2022-11-04 12:27:19.004907 pytest-typhoon-xray-0.4.7/setup.cfg
--rw-r--r--   0 branko     (501) staff       (20)     1607 2022-11-04 12:25:14.000000 pytest-typhoon-xray-0.4.7/setup.py
-drwxr-xr-x   0 branko     (501) staff       (20)        0 2022-11-04 12:27:19.004436 pytest-typhoon-xray-0.4.7/tytest/
--rw-r--r--   0 branko     (501) staff       (20)        0 2021-03-09 10:50:41.000000 pytest-typhoon-xray-0.4.7/tytest/__init__.py
--rw-r--r--   0 branko     (501) staff       (20)      654 2021-03-09 10:50:41.000000 pytest-typhoon-xray-0.4.7/tytest/exceptions.py
--rw-r--r--   0 branko     (501) staff       (20)     6059 2022-11-04 12:23:23.000000 pytest-typhoon-xray-0.4.7/tytest/plugin.py
--rw-r--r--   0 branko     (501) staff       (20)      476 2022-03-28 08:12:31.000000 pytest-typhoon-xray-0.4.7/tytest/runtime_settings.py
--rw-r--r--   0 branko     (501) staff       (20)     1229 2021-03-09 10:50:41.000000 pytest-typhoon-xray-0.4.7/tytest/utils.py
--rw-r--r--   0 branko     (501) staff       (20)     3339 2022-11-04 12:21:18.000000 pytest-typhoon-xray-0.4.7/tytest/xray_api.py
+drwxr-xr-x   0 branko     (501) staff       (20)        0 2023-06-09 18:04:20.560589 pytest-typhoon-xray-1.0.0/
+-rw-r--r--   0 branko     (501) staff       (20)     1068 2022-02-14 11:26:04.000000 pytest-typhoon-xray-1.0.0/LICENSE
+-rw-r--r--   0 branko     (501) staff       (20)       97 2022-02-14 11:26:04.000000 pytest-typhoon-xray-1.0.0/MANIFEST.in
+-rw-r--r--   0 branko     (501) staff       (20)     6895 2023-06-09 18:04:20.560483 pytest-typhoon-xray-1.0.0/PKG-INFO
+-rw-r--r--   0 branko     (501) staff       (20)     5842 2022-02-14 12:03:51.000000 pytest-typhoon-xray-1.0.0/README.rst
+drwxr-xr-x   0 branko     (501) staff       (20)        0 2023-06-09 18:04:20.559083 pytest-typhoon-xray-1.0.0/pytest_typhoon_xray.egg-info/
+-rw-r--r--   0 branko     (501) staff       (20)     6895 2023-06-09 18:04:20.000000 pytest-typhoon-xray-1.0.0/pytest_typhoon_xray.egg-info/PKG-INFO
+-rw-r--r--   0 branko     (501) staff       (20)      418 2023-06-09 18:04:20.000000 pytest-typhoon-xray-1.0.0/pytest_typhoon_xray.egg-info/SOURCES.txt
+-rw-r--r--   0 branko     (501) staff       (20)        1 2023-06-09 18:04:20.000000 pytest-typhoon-xray-1.0.0/pytest_typhoon_xray.egg-info/dependency_links.txt
+-rw-r--r--   0 branko     (501) staff       (20)       35 2023-06-09 18:04:20.000000 pytest-typhoon-xray-1.0.0/pytest_typhoon_xray.egg-info/entry_points.txt
+-rw-r--r--   0 branko     (501) staff       (20)       55 2023-06-09 18:04:20.000000 pytest-typhoon-xray-1.0.0/pytest_typhoon_xray.egg-info/requires.txt
+-rw-r--r--   0 branko     (501) staff       (20)        7 2023-06-09 18:04:20.000000 pytest-typhoon-xray-1.0.0/pytest_typhoon_xray.egg-info/top_level.txt
+-rw-r--r--   0 branko     (501) staff       (20)       38 2023-06-09 18:04:20.560625 pytest-typhoon-xray-1.0.0/setup.cfg
+-rw-r--r--   0 branko     (501) staff       (20)     1607 2023-06-09 18:02:10.000000 pytest-typhoon-xray-1.0.0/setup.py
+drwxr-xr-x   0 branko     (501) staff       (20)        0 2023-06-09 18:04:20.560154 pytest-typhoon-xray-1.0.0/tytest/
+-rw-r--r--   0 branko     (501) staff       (20)        0 2022-02-14 11:26:04.000000 pytest-typhoon-xray-1.0.0/tytest/__init__.py
+-rw-r--r--   0 branko     (501) staff       (20)      654 2022-02-14 11:26:04.000000 pytest-typhoon-xray-1.0.0/tytest/exceptions.py
+-rw-r--r--   0 branko     (501) staff       (20)     6059 2022-06-23 09:21:58.000000 pytest-typhoon-xray-1.0.0/tytest/plugin.py
+-rw-r--r--   0 branko     (501) staff       (20)      476 2022-02-14 11:39:31.000000 pytest-typhoon-xray-1.0.0/tytest/runtime_settings.py
+-rw-r--r--   0 branko     (501) staff       (20)     1229 2022-02-14 11:26:04.000000 pytest-typhoon-xray-1.0.0/tytest/utils.py
+-rw-r--r--   0 branko     (501) staff       (20)     3306 2023-06-09 18:00:12.000000 pytest-typhoon-xray-1.0.0/tytest/xray_api.py
```

### Comparing `pytest-typhoon-xray-0.4.7/LICENSE` & `pytest-typhoon-xray-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-typhoon-xray-0.4.7/PKG-INFO` & `pytest-typhoon-xray-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: pytest-typhoon-xray
-Version: 0.4.7
+Version: 1.0.0
 Summary: Typhoon HIL plugin for pytest
 Home-page: https://github.com/typhoon-hil/pytest-typhoon-xray
 Author: Branko Milosavljevic
 Author-email: branko@typhoon-hil.com
 Maintainer: Branko Milosavljevic
 Maintainer-email: branko@typhoon-hil.com
 License: MIT
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Testing
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -222,7 +223,9 @@
 .. _`Apache Software License 2.0`: http://www.apache.org/licenses/LICENSE-2.0
 .. _`cookiecutter-pytest-plugin`: https://github.com/pytest-dev/cookiecutter-pytest-plugin
 .. _`file an issue`: https://github.com/mbranko/pytest-tytest/issues
 .. _`pytest`: https://github.com/pytest-dev/pytest
 .. _`tox`: https://tox.readthedocs.io/en/latest/
 .. _`pip`: https://pypi.org/project/pip/
 .. _`PyPI`: https://pypi.org/project
+
+
```

### Comparing `pytest-typhoon-xray-0.4.7/README.rst` & `pytest-typhoon-xray-1.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `pytest-typhoon-xray-0.4.7/pytest_typhoon_xray.egg-info/PKG-INFO` & `pytest-typhoon-xray-1.0.0/pytest_typhoon_xray.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: pytest-typhoon-xray
-Version: 0.4.7
+Version: 1.0.0
 Summary: Typhoon HIL plugin for pytest
 Home-page: https://github.com/typhoon-hil/pytest-typhoon-xray
 Author: Branko Milosavljevic
 Author-email: branko@typhoon-hil.com
 Maintainer: Branko Milosavljevic
 Maintainer-email: branko@typhoon-hil.com
 License: MIT
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Testing
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -222,7 +223,9 @@
 .. _`Apache Software License 2.0`: http://www.apache.org/licenses/LICENSE-2.0
 .. _`cookiecutter-pytest-plugin`: https://github.com/pytest-dev/cookiecutter-pytest-plugin
 .. _`file an issue`: https://github.com/mbranko/pytest-tytest/issues
 .. _`pytest`: https://github.com/pytest-dev/pytest
 .. _`tox`: https://tox.readthedocs.io/en/latest/
 .. _`pip`: https://pypi.org/project/pip/
 .. _`PyPI`: https://pypi.org/project
+
+
```

### Comparing `pytest-typhoon-xray-0.4.7/setup.py` & `pytest-typhoon-xray-1.0.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 def read(fname):
     file_path = os.path.join(os.path.dirname(__file__), fname)
     return codecs.open(file_path, encoding='utf-8').read()
 
 
 setup(
     name='pytest-typhoon-xray',
-    version='0.4.7',
+    version='1.0.0',
     author='Branko Milosavljevic',
     author_email='branko@typhoon-hil.com',
     maintainer='Branko Milosavljevic',
     maintainer_email='branko@typhoon-hil.com',
     license='MIT',
     url='https://github.com/typhoon-hil/pytest-typhoon-xray',
     description='Typhoon HIL plugin for pytest',
```

### Comparing `pytest-typhoon-xray-0.4.7/tytest/exceptions.py` & `pytest-typhoon-xray-1.0.0/tytest/exceptions.py`

 * *Files identical despite different names*

### Comparing `pytest-typhoon-xray-0.4.7/tytest/plugin.py` & `pytest-typhoon-xray-1.0.0/tytest/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-typhoon-xray-0.4.7/tytest/utils.py` & `pytest-typhoon-xray-1.0.0/tytest/utils.py`

 * *Files identical despite different names*

### Comparing `pytest-typhoon-xray-0.4.7/tytest/xray_api.py` & `pytest-typhoon-xray-1.0.0/tytest/xray_api.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- coding: utf-8 -*-
 
 from datetime import datetime
 from json import JSONDecodeError
 
 import requests
+from requests.auth import HTTPBasicAuth
 from tzlocal import get_localzone
 from .runtime_settings import Settings
 from .exceptions import XrayAuthError, XraySubmissionError, JiraError
 
 
 def to_xray_timestamp(ts):
     local_tz = get_localzone()
@@ -29,20 +30,17 @@
     return {'Authorization': f'Bearer {Settings.XRAY_TOKEN}'}
 
 
 def send_test_results(test_results):
     if not Settings.XRAY_SERVER and not Settings.XRAY_PLAN_KEY:
         return None
     if Settings.XRAY_SERVER:
-        headers = {
-            'Authorization': f'Bearer {Settings.JIRA_TOKEN}',
-            'Content-type': 'application/json'
-        }
+        basic = HTTPBasicAuth(Settings.JIRA_USER, Settings.JIRA_TOKEN)
         r = requests.post(f'{Settings.JIRA_HOST}/rest/raven/1.0/import/execution',
-                          headers=headers, json=test_results)
+                          auth=basic, json=test_results)
     else:
         headers = authenticate_xray()
         r = requests.post(f'{Settings.XRAY_HOST}/api/v1/import/execution',
                           headers=headers, json=test_results)
     if r.status_code != 200 and not Settings.XRAY_FAIL_SILENTLY:
         raise XraySubmissionError
     try:
```

