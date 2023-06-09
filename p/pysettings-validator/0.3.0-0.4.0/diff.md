# Comparing `tmp/pysettings-validator-0.3.0.tar.gz` & `tmp/pysettings-validator-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysettings-validator-0.3.0.tar", last modified: Thu Jun  8 17:46:29 2023, max compression
+gzip compressed data, was "pysettings-validator-0.4.0.tar", last modified: Fri Jun  9 12:59:20 2023, max compression
```

## Comparing `pysettings-validator-0.3.0.tar` & `pysettings-validator-0.4.0.tar`

### file list

```diff
@@ -1,22 +1,25 @@
-drwxr-xr-x   0 palazzem  (1051) palazzem  (1051)        0 2023-06-08 17:46:29.703604 pysettings-validator-0.3.0/
--rw-r--r--   0 palazzem  (1051) palazzem  (1051)     1527 2023-06-08 15:50:52.000000 pysettings-validator-0.3.0/LICENSE
--rw-r--r--   0 palazzem  (1051) palazzem  (1051)     6405 2023-06-08 17:46:29.703604 pysettings-validator-0.3.0/PKG-INFO
--rw-r--r--   0 palazzem  (1051) palazzem  (1051)     5593 2023-06-08 17:42:49.000000 pysettings-validator-0.3.0/README.md
-drwxr-xr-x   0 palazzem  (1051) palazzem  (1051)        0 2023-06-08 17:46:29.703604 pysettings-validator-0.3.0/pysettings/
--rw-r--r--   0 palazzem  (1051) palazzem  (1051)        0 2023-06-08 15:50:52.000000 pysettings-validator-0.3.0/pysettings/__init__.py
--rw-r--r--   0 palazzem  (1051) palazzem  (1051)     4642 2023-06-08 17:42:49.000000 pysettings-validator-0.3.0/pysettings/base.py
--rw-r--r--   0 palazzem  (1051) palazzem  (1051)      330 2023-06-08 15:50:52.000000 pysettings-validator-0.3.0/pysettings/exceptions.py
--rw-r--r--   0 palazzem  (1051) palazzem  (1051)     1542 2023-06-08 17:30:19.000000 pysettings-validator-0.3.0/pysettings/options.py
--rw-r--r--   0 palazzem  (1051) palazzem  (1051)      843 2023-06-08 15:50:52.000000 pysettings-validator-0.3.0/pysettings/validators.py
-drwxr-xr-x   0 palazzem  (1051) palazzem  (1051)        0 2023-06-08 17:46:29.703604 pysettings-validator-0.3.0/pysettings_validator.egg-info/
--rw-r--r--   0 palazzem  (1051) palazzem  (1051)     6405 2023-06-08 17:46:29.000000 pysettings-validator-0.3.0/pysettings_validator.egg-info/PKG-INFO
--rw-r--r--   0 palazzem  (1051) palazzem  (1051)      409 2023-06-08 17:46:29.000000 pysettings-validator-0.3.0/pysettings_validator.egg-info/SOURCES.txt
--rw-r--r--   0 palazzem  (1051) palazzem  (1051)        1 2023-06-08 17:46:29.000000 pysettings-validator-0.3.0/pysettings_validator.egg-info/dependency_links.txt
--rw-r--r--   0 palazzem  (1051) palazzem  (1051)       11 2023-06-08 17:46:29.000000 pysettings-validator-0.3.0/pysettings_validator.egg-info/top_level.txt
--rw-r--r--   0 palazzem  (1051) palazzem  (1051)       38 2023-06-08 17:46:29.703604 pysettings-validator-0.3.0/setup.cfg
--rw-r--r--   0 palazzem  (1051) palazzem  (1051)     3317 2023-06-08 17:43:16.000000 pysettings-validator-0.3.0/setup.py
-drwxr-xr-x   0 palazzem  (1051) palazzem  (1051)        0 2023-06-08 17:46:29.703604 pysettings-validator-0.3.0/tests/
--rw-r--r--   0 palazzem  (1051) palazzem  (1051)      348 2023-06-08 17:42:49.000000 pysettings-validator-0.3.0/tests/test_fixtures.py
--rw-r--r--   0 palazzem  (1051) palazzem  (1051)     2355 2023-06-08 15:50:52.000000 pysettings-validator-0.3.0/tests/test_options.py
--rw-r--r--   0 palazzem  (1051) palazzem  (1051)     4713 2023-06-08 17:42:49.000000 pysettings-validator-0.3.0/tests/test_settings.py
--rw-r--r--   0 palazzem  (1051) palazzem  (1051)     1562 2023-06-08 15:50:52.000000 pysettings-validator-0.3.0/tests/test_validators.py
+drwxr-xr-x   0 palazzem  (1051) palazzem  (1051)        0 2023-06-09 12:59:20.166484 pysettings-validator-0.4.0/
+-rw-r--r--   0 palazzem  (1051) palazzem  (1051)     1527 2023-06-08 15:50:52.000000 pysettings-validator-0.4.0/LICENSE
+-rw-r--r--   0 palazzem  (1051) palazzem  (1051)     5930 2023-06-09 12:59:20.166484 pysettings-validator-0.4.0/PKG-INFO
+-rw-r--r--   0 palazzem  (1051) palazzem  (1051)     5118 2023-06-09 12:55:52.000000 pysettings-validator-0.4.0/README.md
+drwxr-xr-x   0 palazzem  (1051) palazzem  (1051)        0 2023-06-09 12:59:20.166484 pysettings-validator-0.4.0/pysettings/
+-rw-r--r--   0 palazzem  (1051) palazzem  (1051)        0 2023-06-08 15:50:52.000000 pysettings-validator-0.4.0/pysettings/__init__.py
+-rw-r--r--   0 palazzem  (1051) palazzem  (1051)     4642 2023-06-08 17:42:49.000000 pysettings-validator-0.4.0/pysettings/base.py
+-rw-r--r--   0 palazzem  (1051) palazzem  (1051)      330 2023-06-08 15:50:52.000000 pysettings-validator-0.4.0/pysettings/exceptions.py
+-rw-r--r--   0 palazzem  (1051) palazzem  (1051)     1542 2023-06-08 17:30:19.000000 pysettings-validator-0.4.0/pysettings/options.py
+drwxr-xr-x   0 palazzem  (1051) palazzem  (1051)        0 2023-06-09 12:59:20.166484 pysettings-validator-0.4.0/pysettings/test/
+-rw-r--r--   0 palazzem  (1051) palazzem  (1051)       69 2023-06-09 12:55:52.000000 pysettings-validator-0.4.0/pysettings/test/__init__.py
+-rw-r--r--   0 palazzem  (1051) palazzem  (1051)     2886 2023-06-09 12:55:52.000000 pysettings-validator-0.4.0/pysettings/test/wrappers.py
+-rw-r--r--   0 palazzem  (1051) palazzem  (1051)      843 2023-06-08 15:50:52.000000 pysettings-validator-0.4.0/pysettings/validators.py
+drwxr-xr-x   0 palazzem  (1051) palazzem  (1051)        0 2023-06-09 12:59:20.166484 pysettings-validator-0.4.0/pysettings_validator.egg-info/
+-rw-r--r--   0 palazzem  (1051) palazzem  (1051)     5930 2023-06-09 12:59:20.000000 pysettings-validator-0.4.0/pysettings_validator.egg-info/PKG-INFO
+-rw-r--r--   0 palazzem  (1051) palazzem  (1051)      465 2023-06-09 12:59:20.000000 pysettings-validator-0.4.0/pysettings_validator.egg-info/SOURCES.txt
+-rw-r--r--   0 palazzem  (1051) palazzem  (1051)        1 2023-06-09 12:59:20.000000 pysettings-validator-0.4.0/pysettings_validator.egg-info/dependency_links.txt
+-rw-r--r--   0 palazzem  (1051) palazzem  (1051)       11 2023-06-09 12:59:20.000000 pysettings-validator-0.4.0/pysettings_validator.egg-info/top_level.txt
+-rw-r--r--   0 palazzem  (1051) palazzem  (1051)       38 2023-06-09 12:59:20.166484 pysettings-validator-0.4.0/setup.cfg
+-rw-r--r--   0 palazzem  (1051) palazzem  (1051)     3317 2023-06-09 12:56:09.000000 pysettings-validator-0.4.0/setup.py
+drwxr-xr-x   0 palazzem  (1051) palazzem  (1051)        0 2023-06-09 12:59:20.166484 pysettings-validator-0.4.0/tests/
+-rw-r--r--   0 palazzem  (1051) palazzem  (1051)     2355 2023-06-08 15:50:52.000000 pysettings-validator-0.4.0/tests/test_options.py
+-rw-r--r--   0 palazzem  (1051) palazzem  (1051)     4713 2023-06-08 17:42:49.000000 pysettings-validator-0.4.0/tests/test_settings.py
+-rw-r--r--   0 palazzem  (1051) palazzem  (1051)     1562 2023-06-08 15:50:52.000000 pysettings-validator-0.4.0/tests/test_validators.py
+-rw-r--r--   0 palazzem  (1051) palazzem  (1051)     1936 2023-06-09 12:55:52.000000 pysettings-validator-0.4.0/tests/test_wrappers.py
```

### Comparing `pysettings-validator-0.3.0/LICENSE` & `pysettings-validator-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pysettings-validator-0.3.0/PKG-INFO` & `pysettings-validator-0.4.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysettings-validator
-Version: 0.3.0
+Version: 0.4.0
 Summary: Python package to store your application settings. Validators are built-in!
 Home-page: https://github.com/palazzem/pysettings
 Author: Emanuele Palazzetti
 Author-email: emanuele.palazzetti@gmail.com
 License: BSD 3-Clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -129,54 +129,34 @@
 
 ### Test your Settings (pytest)
 
 If you need to change some of your settings during tests, you can use the following snippet
 to restore the previous settings after each test:
 
 ```python
-# tests/fixtures/settings.py
-from pysettings.base import BaseSettings
-from pysettings.options import Option
-from pysettings.validators import is_https_url
-
-# Class definition
-class TestSettings(BaseSettings):
-    url = Option(validators=[is_https_url])
-    description = Option()
-
-# Use settings in your application
-settings = TestSettings()
-settings.url = "https://example.com"
-settings.description = "A shiny Website!"
-settings.is_valid()
-
 # tests/conftest.py
-import copy
-import pytest
-
-from .fixtures import settings as config
+from app.config import settings as app_settings   # Import your global settings
+from pysettings.test import SettingsWrapper       # Import settings wrapper
 
 
-@pytest.fixture
+@pytest.fixture(scope="function")
 def settings():
-    previous_config = copy.deepcopy(config.settings)
-    yield config.settings
-    config.settings = previous_config
+    wrapper = SettingsWrapper(app_settings)
+    # (Optional) Include test overrides
+    wrapper.DATABASE_URL = "sqlite://"
+    yield wrapper
+    # Restore original settings
+    wrapper.finalize()
 
 # tests/test_settings.py
-def test_settings_changes_1(settings):
-    assert settings.description == "A shiny Website!"
-    settings.description = "Test 1"
-    assert settings.description == "Test 1"
-
+def test_settings(settings):
+    # Change settings for this test only
+    settings.BATCH_SIZE = 100
 
-def test_settings_changes_2(settings):
-    assert settings.description == "A shiny Website!"
-    settings.description = "Test 2"
-    assert settings.description == "Test 2"
+    # ... Test your code ...
 ```
 
 ## Development
 
 We accept external contributions even though the project is mostly designed for personal
 needs. If you think some parts can be exposed with a more generic interface, feel free
 to open a GitHub issue and to discuss your suggestion.
```

### Comparing `pysettings-validator-0.3.0/README.md` & `pysettings-validator-0.4.0/pysettings_validator.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: pysettings-validator
+Version: 0.4.0
+Summary: Python package to store your application settings. Validators are built-in!
+Home-page: https://github.com/palazzem/pysettings
+Author: Emanuele Palazzetti
+Author-email: emanuele.palazzetti@gmail.com
+License: BSD 3-Clause
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.7.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
 # pysettings
 
 [![PyPI version](https://badge.fury.io/py/pysettings-validator.svg)](https://badge.fury.io/py/pysettings-validator)
 [![Linting](https://github.com/palazzem/pysettings/actions/workflows/linting.yaml/badge.svg?branch=master)](https://github.com/palazzem/pysettings/actions/workflows/linting.yaml)
 [![Testing](https://github.com/palazzem/pysettings/actions/workflows/testing.yaml/badge.svg?branch=master)](https://github.com/palazzem/pysettings/actions/workflows/testing.yaml)
 
 Pysettings is a Python package to store your application settings. Compared to some
@@ -107,54 +129,34 @@
 
 ### Test your Settings (pytest)
 
 If you need to change some of your settings during tests, you can use the following snippet
 to restore the previous settings after each test:
 
 ```python
-# tests/fixtures/settings.py
-from pysettings.base import BaseSettings
-from pysettings.options import Option
-from pysettings.validators import is_https_url
-
-# Class definition
-class TestSettings(BaseSettings):
-    url = Option(validators=[is_https_url])
-    description = Option()
-
-# Use settings in your application
-settings = TestSettings()
-settings.url = "https://example.com"
-settings.description = "A shiny Website!"
-settings.is_valid()
-
 # tests/conftest.py
-import copy
-import pytest
+from app.config import settings as app_settings   # Import your global settings
+from pysettings.test import SettingsWrapper       # Import settings wrapper
 
-from .fixtures import settings as config
 
-
-@pytest.fixture
+@pytest.fixture(scope="function")
 def settings():
-    previous_config = copy.deepcopy(config.settings)
-    yield config.settings
-    config.settings = previous_config
+    wrapper = SettingsWrapper(app_settings)
+    # (Optional) Include test overrides
+    wrapper.DATABASE_URL = "sqlite://"
+    yield wrapper
+    # Restore original settings
+    wrapper.finalize()
 
 # tests/test_settings.py
-def test_settings_changes_1(settings):
-    assert settings.description == "A shiny Website!"
-    settings.description = "Test 1"
-    assert settings.description == "Test 1"
-
+def test_settings(settings):
+    # Change settings for this test only
+    settings.BATCH_SIZE = 100
 
-def test_settings_changes_2(settings):
-    assert settings.description == "A shiny Website!"
-    settings.description = "Test 2"
-    assert settings.description == "Test 2"
+    # ... Test your code ...
 ```
 
 ## Development
 
 We accept external contributions even though the project is mostly designed for personal
 needs. If you think some parts can be exposed with a more generic interface, feel free
 to open a GitHub issue and to discuss your suggestion.
```

### Comparing `pysettings-validator-0.3.0/pysettings/base.py` & `pysettings-validator-0.4.0/pysettings/base.py`

 * *Files identical despite different names*

### Comparing `pysettings-validator-0.3.0/pysettings/options.py` & `pysettings-validator-0.4.0/pysettings/options.py`

 * *Files identical despite different names*

### Comparing `pysettings-validator-0.3.0/pysettings/validators.py` & `pysettings-validator-0.4.0/pysettings/validators.py`

 * *Files identical despite different names*

### Comparing `pysettings-validator-0.3.0/pysettings_validator.egg-info/PKG-INFO` & `pysettings-validator-0.4.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: pysettings-validator
-Version: 0.3.0
-Summary: Python package to store your application settings. Validators are built-in!
-Home-page: https://github.com/palazzem/pysettings
-Author: Emanuele Palazzetti
-Author-email: emanuele.palazzetti@gmail.com
-License: BSD 3-Clause
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
 # pysettings
 
 [![PyPI version](https://badge.fury.io/py/pysettings-validator.svg)](https://badge.fury.io/py/pysettings-validator)
 [![Linting](https://github.com/palazzem/pysettings/actions/workflows/linting.yaml/badge.svg?branch=master)](https://github.com/palazzem/pysettings/actions/workflows/linting.yaml)
 [![Testing](https://github.com/palazzem/pysettings/actions/workflows/testing.yaml/badge.svg?branch=master)](https://github.com/palazzem/pysettings/actions/workflows/testing.yaml)
 
 Pysettings is a Python package to store your application settings. Compared to some
@@ -129,54 +107,34 @@
 
 ### Test your Settings (pytest)
 
 If you need to change some of your settings during tests, you can use the following snippet
 to restore the previous settings after each test:
 
 ```python
-# tests/fixtures/settings.py
-from pysettings.base import BaseSettings
-from pysettings.options import Option
-from pysettings.validators import is_https_url
-
-# Class definition
-class TestSettings(BaseSettings):
-    url = Option(validators=[is_https_url])
-    description = Option()
-
-# Use settings in your application
-settings = TestSettings()
-settings.url = "https://example.com"
-settings.description = "A shiny Website!"
-settings.is_valid()
-
 # tests/conftest.py
-import copy
-import pytest
+from app.config import settings as app_settings   # Import your global settings
+from pysettings.test import SettingsWrapper       # Import settings wrapper
 
-from .fixtures import settings as config
 
-
-@pytest.fixture
+@pytest.fixture(scope="function")
 def settings():
-    previous_config = copy.deepcopy(config.settings)
-    yield config.settings
-    config.settings = previous_config
+    wrapper = SettingsWrapper(app_settings)
+    # (Optional) Include test overrides
+    wrapper.DATABASE_URL = "sqlite://"
+    yield wrapper
+    # Restore original settings
+    wrapper.finalize()
 
 # tests/test_settings.py
-def test_settings_changes_1(settings):
-    assert settings.description == "A shiny Website!"
-    settings.description = "Test 1"
-    assert settings.description == "Test 1"
-
+def test_settings(settings):
+    # Change settings for this test only
+    settings.BATCH_SIZE = 100
 
-def test_settings_changes_2(settings):
-    assert settings.description == "A shiny Website!"
-    settings.description = "Test 2"
-    assert settings.description == "Test 2"
+    # ... Test your code ...
 ```
 
 ## Development
 
 We accept external contributions even though the project is mostly designed for personal
 needs. If you think some parts can be exposed with a more generic interface, feel free
 to open a GitHub issue and to discuss your suggestion.
```

### Comparing `pysettings-validator-0.3.0/setup.py` & `pysettings-validator-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 
-VERSION = "0.3.0"
+VERSION = "0.4.0"
 
 # What packages are required for this module to be executed?
 REQUIRES_PYTHON = ">=3.7.0"
 REQUIRED = []
 
 # What packages are optional?
 EXTRAS = {}
```

### Comparing `pysettings-validator-0.3.0/tests/test_options.py` & `pysettings-validator-0.4.0/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `pysettings-validator-0.3.0/tests/test_settings.py` & `pysettings-validator-0.4.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `pysettings-validator-0.3.0/tests/test_validators.py` & `pysettings-validator-0.4.0/tests/test_validators.py`

 * *Files identical despite different names*

