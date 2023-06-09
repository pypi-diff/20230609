# Comparing `tmp/sirepo-bluesky-0.6.1.tar.gz` & `tmp/sirepo-bluesky-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sirepo-bluesky-0.6.1.tar", last modified: Fri May 26 14:22:52 2023, max compression
+gzip compressed data, was "sirepo-bluesky-0.6.2.tar", last modified: Fri Jun  9 16:49:00 2023, max compression
```

## Comparing `sirepo-bluesky-0.6.1.tar` & `sirepo-bluesky-0.6.2.tar`

### file list

```diff
@@ -1,49 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:22:52.029771 sirepo-bluesky-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-26 14:22:38.000000 sirepo-bluesky-0.6.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-05-26 14:22:38.000000 sirepo-bluesky-0.6.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-05-26 14:22:38.000000 sirepo-bluesky-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-26 14:22:38.000000 sirepo-bluesky-0.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-26 14:22:52.029771 sirepo-bluesky-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-05-26 14:22:38.000000 sirepo-bluesky-0.6.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:22:52.021771 sirepo-bluesky-0.6.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-05-26 14:22:38.000000 sirepo-bluesky-0.6.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-26 14:22:38.000000 sirepo-bluesky-0.6.1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:22:52.021771 sirepo-bluesky-0.6.1/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-05-26 14:22:38.000000 sirepo-bluesky-0.6.1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-26 14:22:38.000000 sirepo-bluesky-0.6.1/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-05-26 14:22:38.000000 sirepo-bluesky-0.6.1/docs/source/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-26 14:22:38.000000 sirepo-bluesky-0.6.1/docs/source/notebooks-new-api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-26 14:22:38.000000 sirepo-bluesky-0.6.1/docs/source/notebooks-old-api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7443 2023-05-26 14:22:38.000000 sirepo-bluesky-0.6.1/docs/source/release-history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-26 14:22:38.000000 sirepo-bluesky-0.6.1/docs/source/simulations.rst
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-26 14:22:38.000000 sirepo-bluesky-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-26 14:22:38.000000 sirepo-bluesky-0.6.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-26 14:22:52.029771 sirepo-bluesky-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-05-26 14:22:38.000000 sirepo-bluesky-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:22:52.029771 sirepo-bluesky-0.6.1/sirepo_bluesky/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-26 14:22:38.000000 sirepo-bluesky-0.6.1/sirepo_bluesky/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-26 14:22:52.029771 sirepo-bluesky-0.6.1/sirepo_bluesky/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-05-26 14:22:38.000000 sirepo-bluesky-0.6.1/sirepo_bluesky/madx_flyer.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-26 14:22:38.000000 sirepo-bluesky-0.6.1/sirepo_bluesky/madx_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    13429 2023-05-26 14:22:38.000000 sirepo-bluesky-0.6.1/sirepo_bluesky/shadow_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-05-26 14:22:38.000000 sirepo-bluesky-0.6.1/sirepo_bluesky/shadow_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8409 2023-05-26 14:22:38.000000 sirepo-bluesky-0.6.1/sirepo_bluesky/sirepo_bluesky.py
--rw-r--r--   0 runner    (1001) docker     (123)    15800 2023-05-26 14:22:38.000000 sirepo-bluesky-0.6.1/sirepo_bluesky/sirepo_flyer.py
--rw-r--r--   0 runner    (1001) docker     (123)    15129 2023-05-26 14:22:38.000000 sirepo-bluesky-0.6.1/sirepo_bluesky/sirepo_ophyd.py
--rw-r--r--   0 runner    (1001) docker     (123)    12002 2023-05-26 14:22:38.000000 sirepo-bluesky-0.6.1/sirepo_bluesky/srw_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-26 14:22:38.000000 sirepo-bluesky-0.6.1/sirepo_bluesky/srw_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:22:52.029771 sirepo-bluesky-0.6.1/sirepo_bluesky/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 14:22:38.000000 sirepo-bluesky-0.6.1/sirepo_bluesky/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-05-26 14:22:38.000000 sirepo-bluesky-0.6.1/sirepo_bluesky/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    15535 2023-05-26 14:22:38.000000 sirepo-bluesky-0.6.1/sirepo_bluesky/tests/test_bl_elements_as_ophyd_objs.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 14:22:38.000000 sirepo-bluesky-0.6.1/sirepo_bluesky/tests/test_entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-05-26 14:22:38.000000 sirepo-bluesky-0.6.1/sirepo_bluesky/tests/test_shadow_det.py
--rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-05-26 14:22:38.000000 sirepo-bluesky-0.6.1/sirepo_bluesky/tests/test_sirepo_flyer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-05-26 14:22:38.000000 sirepo-bluesky-0.6.1/sirepo_bluesky/tests/test_srw_det.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:22:52.025771 sirepo-bluesky-0.6.1/sirepo_bluesky.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-26 14:22:51.000000 sirepo-bluesky-0.6.1/sirepo_bluesky.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-26 14:22:51.000000 sirepo-bluesky-0.6.1/sirepo_bluesky.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 14:22:51.000000 sirepo-bluesky-0.6.1/sirepo_bluesky.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-26 14:22:51.000000 sirepo-bluesky-0.6.1/sirepo_bluesky.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-26 14:22:51.000000 sirepo-bluesky-0.6.1/sirepo_bluesky.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    68503 2023-05-26 14:22:38.000000 sirepo-bluesky-0.6.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:49:00.634703 sirepo-bluesky-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-09 16:48:49.000000 sirepo-bluesky-0.6.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-06-09 16:48:49.000000 sirepo-bluesky-0.6.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-06-09 16:48:49.000000 sirepo-bluesky-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-09 16:48:49.000000 sirepo-bluesky-0.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-09 16:49:00.634703 sirepo-bluesky-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-06-09 16:48:49.000000 sirepo-bluesky-0.6.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:49:00.626703 sirepo-bluesky-0.6.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-06-09 16:48:49.000000 sirepo-bluesky-0.6.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-06-09 16:48:49.000000 sirepo-bluesky-0.6.2/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:49:00.626703 sirepo-bluesky-0.6.2/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-06-09 16:48:49.000000 sirepo-bluesky-0.6.2/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-09 16:48:49.000000 sirepo-bluesky-0.6.2/docs/source/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-09 16:48:49.000000 sirepo-bluesky-0.6.2/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-06-09 16:48:49.000000 sirepo-bluesky-0.6.2/docs/source/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8378 2023-06-09 16:48:49.000000 sirepo-bluesky-0.6.2/docs/source/release-history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-09 16:48:49.000000 sirepo-bluesky-0.6.2/docs/source/simulations.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-09 16:48:50.000000 sirepo-bluesky-0.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-09 16:48:50.000000 sirepo-bluesky-0.6.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-09 16:49:00.634703 sirepo-bluesky-0.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-06-09 16:48:50.000000 sirepo-bluesky-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:49:00.634703 sirepo-bluesky-0.6.2/sirepo_bluesky/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-09 16:48:50.000000 sirepo-bluesky-0.6.2/sirepo_bluesky/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-09 16:49:00.634703 sirepo-bluesky-0.6.2/sirepo_bluesky/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-06-09 16:48:50.000000 sirepo-bluesky-0.6.2/sirepo_bluesky/madx_flyer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-09 16:48:50.000000 sirepo-bluesky-0.6.2/sirepo_bluesky/madx_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13429 2023-06-09 16:48:50.000000 sirepo-bluesky-0.6.2/sirepo_bluesky/shadow_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-06-09 16:48:50.000000 sirepo-bluesky-0.6.2/sirepo_bluesky/shadow_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8409 2023-06-09 16:48:50.000000 sirepo-bluesky-0.6.2/sirepo_bluesky/sirepo_bluesky.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15800 2023-06-09 16:48:50.000000 sirepo-bluesky-0.6.2/sirepo_bluesky/sirepo_flyer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15176 2023-06-09 16:48:50.000000 sirepo-bluesky-0.6.2/sirepo_bluesky/sirepo_ophyd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12002 2023-06-09 16:48:50.000000 sirepo-bluesky-0.6.2/sirepo_bluesky/srw_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-09 16:48:50.000000 sirepo-bluesky-0.6.2/sirepo_bluesky/srw_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:49:00.630703 sirepo-bluesky-0.6.2/sirepo_bluesky/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 16:48:50.000000 sirepo-bluesky-0.6.2/sirepo_bluesky/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-06-09 16:48:50.000000 sirepo-bluesky-0.6.2/sirepo_bluesky/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15535 2023-06-09 16:48:50.000000 sirepo-bluesky-0.6.2/sirepo_bluesky/tests/test_bl_elements_as_ophyd_objs.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-09 16:48:50.000000 sirepo-bluesky-0.6.2/sirepo_bluesky/tests/test_entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-06-09 16:48:50.000000 sirepo-bluesky-0.6.2/sirepo_bluesky/tests/test_shadow_det.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-06-09 16:48:50.000000 sirepo-bluesky-0.6.2/sirepo_bluesky/tests/test_sirepo_flyer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-06-09 16:48:50.000000 sirepo-bluesky-0.6.2/sirepo_bluesky/tests/test_srw_det.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:49:00.630703 sirepo-bluesky-0.6.2/sirepo_bluesky.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-09 16:49:00.000000 sirepo-bluesky-0.6.2/sirepo_bluesky.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-09 16:49:00.000000 sirepo-bluesky-0.6.2/sirepo_bluesky.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 16:49:00.000000 sirepo-bluesky-0.6.2/sirepo_bluesky.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-09 16:49:00.000000 sirepo-bluesky-0.6.2/sirepo_bluesky.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-09 16:49:00.000000 sirepo-bluesky-0.6.2/sirepo_bluesky.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    68503 2023-06-09 16:48:50.000000 sirepo-bluesky-0.6.2/versioneer.py
```

### Comparing `sirepo-bluesky-0.6.1/CONTRIBUTING.rst` & `sirepo-bluesky-0.6.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `sirepo-bluesky-0.6.1/LICENSE` & `sirepo-bluesky-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sirepo-bluesky-0.6.1/PKG-INFO` & `sirepo-bluesky-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sirepo-bluesky
-Version: 0.6.1
+Version: 0.6.2
 Summary: Sirepo-Bluesky interface
 Home-page: https://github.com/NSLS-II/sirepo-bluesky
 Author: Brookhaven National Laboratory
 Author-email: mrakitin@bnl.gov
 License: BSD (3-clause)
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
```

### Comparing `sirepo-bluesky-0.6.1/README.rst` & `sirepo-bluesky-0.6.2/README.rst`

 * *Files identical despite different names*

### Comparing `sirepo-bluesky-0.6.1/docs/Makefile` & `sirepo-bluesky-0.6.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sirepo-bluesky-0.6.1/docs/make.bat` & `sirepo-bluesky-0.6.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `sirepo-bluesky-0.6.1/docs/source/conf.py` & `sirepo-bluesky-0.6.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `sirepo-bluesky-0.6.1/docs/source/installation.rst` & `sirepo-bluesky-0.6.2/docs/source/installation.rst`

 * *Files 6% similar despite different names*

```diff
@@ -59,15 +59,16 @@
 Configuration of databroker
 ---------------------------
 
 To to access the collected data with the `databroker
 <https://blueskyproject.io/databroker>`_ library, we need to configure it. For
 that, please copy the `local.yml
 <https://github.com/NSLS-II/sirepo-bluesky/blob/main/examples/local.yml>`_
-configuration file to the ``~/.config/databroker/`` directory.
+configuration file to the ``~/.config/databroker/`` directory if using macOS or Linux. For Windows systems,
+copy the configuration file to the ``%APPDATA%\databroker`` directory.
 
 .. include:: ../../examples/local.yml
    :literal:
 
 
 Installation
 ------------
```

### Comparing `sirepo-bluesky-0.6.1/docs/source/release-history.rst` & `sirepo-bluesky-0.6.2/docs/source/release-history.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,55 @@
 ===============
 Release History
 ===============
 
+v0.6.2 (2023-06-09)
+-------------------
+This is a maintenance release with small API, tests, packaging, and documentation updates.
+
+API
+...
+- Fixed the ``BeamStatisticsReport``'s default values which cannot be a
+  dictionary (discovered when using `bluesky v1.11.0
+  <https://github.com/bluesky/bluesky/releases/tag/v1.11.0>`_).
+
+Packaging
+.........
+- Added ``xraylib`` to the list of requirements as ``shadow3`` does not
+  automatically install it, and imports of ``xraylib`` will print the
+  information about that missing library, even for irrelevant code (like
+  MAD-X). Adding the package as a dependency explicitly silences the messages.
+
+- Remove pinning of the ``urllib3`` package as the issue is resolved on the
+  ``vcrpy`` side.
+
+Documentation
+.............
+- Updated databroker configuration instructions for Windows.
+- Removed old API examples.
+
+Tests
+.....
+- Removed a test for ``BeamStatisticsReport`` for the old API.
+
+
 v0.6.1 (2023-05-26)
 -------------------
 This is a maintenance release primarily addressing the packaging, continuous
 integration, and testing matters.
 
 API
 ...
 - Fixed the deprecated API call ``bluesky-auth`` -> ``auth-bluesky-login`` to
   authenticate with Sirepo using the _bluesky_ auth method.
 
 Tests
 .....
-- Recreated `vcrpy <https://vcrpy.readthedocs.io/en/latest/>`_ cassettes for the
-  tests using old API (to be deprecated in the future).
+- Recreated `vcrpy <https://vcrpy.readthedocs.io/en/latest/>`_ cassettes for
+  the tests using old API (to be deprecated in the future).
 - Fixed beam statistics report test.
 
 CI improvements
 ...............
 - Applied `NSLS-II/start-sirepo-action
   <https://github.com/NSLS-II/start-sirepo-action>`_ to start Sirepo in the CI
   workflows (used in other repositories which need Sirepo with predefined
```

### Comparing `sirepo-bluesky-0.6.1/docs/source/simulations.rst` & `sirepo-bluesky-0.6.2/docs/source/simulations.rst`

 * *Files identical despite different names*

### Comparing `sirepo-bluesky-0.6.1/setup.py` & `sirepo-bluesky-0.6.2/setup.py`

 * *Files identical despite different names*

### Comparing `sirepo-bluesky-0.6.1/sirepo_bluesky/__init__.py` & `sirepo-bluesky-0.6.2/sirepo_bluesky/__init__.py`

 * *Files identical despite different names*

### Comparing `sirepo-bluesky-0.6.1/sirepo_bluesky/madx_flyer.py` & `sirepo-bluesky-0.6.2/sirepo_bluesky/madx_flyer.py`

 * *Files identical despite different names*

### Comparing `sirepo-bluesky-0.6.1/sirepo_bluesky/shadow_detector.py` & `sirepo-bluesky-0.6.2/sirepo_bluesky/shadow_detector.py`

 * *Files identical despite different names*

### Comparing `sirepo-bluesky-0.6.1/sirepo_bluesky/shadow_handler.py` & `sirepo-bluesky-0.6.2/sirepo_bluesky/shadow_handler.py`

 * *Files identical despite different names*

### Comparing `sirepo-bluesky-0.6.1/sirepo_bluesky/sirepo_bluesky.py` & `sirepo-bluesky-0.6.2/sirepo_bluesky/sirepo_bluesky.py`

 * *Files identical despite different names*

### Comparing `sirepo-bluesky-0.6.1/sirepo_bluesky/sirepo_flyer.py` & `sirepo-bluesky-0.6.2/sirepo_bluesky/sirepo_flyer.py`

 * *Files identical despite different names*

### Comparing `sirepo-bluesky-0.6.1/sirepo_bluesky/sirepo_ophyd.py` & `sirepo-bluesky-0.6.2/sirepo_bluesky/sirepo_ophyd.py`

 * *Files 0% similar despite different names*

```diff
@@ -253,15 +253,15 @@
         return NullStatus()
 
 
 class BeamStatisticsReport(DeviceWithJSONData):
     # NOTE: TES aperture changes don't seem to change the beam statistics
     # report graph on the website?
 
-    report = Cpt(Signal, value={}, kind="normal")
+    report = Cpt(Signal, value="", kind="normal")  # values are always strings, not dictionaries
 
     def __init__(self, connection, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.connection = connection
 
     def trigger(self, *args, **kwargs):
         logger.debug(f"Custom trigger for {self.name}")
@@ -280,19 +280,19 @@
         # We call the trigger on super at the end to update the sirepo_data_json
         # and the corresponding hash after the simulation is run.
         super().trigger(*args, **kwargs)
         return NullStatus()
 
     def stage(self):
         super().stage()
-        self.report.put({})
+        self.report.put("")
 
     def unstage(self):
         super().unstage()
-        self.report.put({})
+        self.report.put("")
 
 
 class SirepoSignalGrazingAngle(SirepoSignal):
     def set(self, value):
         super().set(value)
         ret = self.parent.connection.compute_grazing_orientation(self._sirepo_dict)
         # State is added to the ret dict from compute_grazing_orientation and we
```

### Comparing `sirepo-bluesky-0.6.1/sirepo_bluesky/srw_detector.py` & `sirepo-bluesky-0.6.2/sirepo_bluesky/srw_detector.py`

 * *Files identical despite different names*

### Comparing `sirepo-bluesky-0.6.1/sirepo_bluesky/srw_handler.py` & `sirepo-bluesky-0.6.2/sirepo_bluesky/srw_handler.py`

 * *Files identical despite different names*

### Comparing `sirepo-bluesky-0.6.1/sirepo_bluesky/tests/conftest.py` & `sirepo-bluesky-0.6.2/sirepo_bluesky/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sirepo-bluesky-0.6.1/sirepo_bluesky/tests/test_bl_elements_as_ophyd_objs.py` & `sirepo-bluesky-0.6.2/sirepo_bluesky/tests/test_bl_elements_as_ophyd_objs.py`

 * *Files identical despite different names*

### Comparing `sirepo-bluesky-0.6.1/sirepo_bluesky/tests/test_sirepo_flyer.py` & `sirepo-bluesky-0.6.2/sirepo_bluesky/tests/test_sirepo_flyer.py`

 * *Files identical despite different names*

### Comparing `sirepo-bluesky-0.6.1/sirepo_bluesky/tests/test_srw_det.py` & `sirepo-bluesky-0.6.2/sirepo_bluesky/tests/test_srw_det.py`

 * *Files identical despite different names*

### Comparing `sirepo-bluesky-0.6.1/sirepo_bluesky.egg-info/PKG-INFO` & `sirepo-bluesky-0.6.2/sirepo_bluesky.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sirepo-bluesky
-Version: 0.6.1
+Version: 0.6.2
 Summary: Sirepo-Bluesky interface
 Home-page: https://github.com/NSLS-II/sirepo-bluesky
 Author: Brookhaven National Laboratory
 Author-email: mrakitin@bnl.gov
 License: BSD (3-clause)
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
```

### Comparing `sirepo-bluesky-0.6.1/sirepo_bluesky.egg-info/SOURCES.txt` & `sirepo-bluesky-0.6.2/sirepo_bluesky.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -7,18 +7,17 @@
 requirements.txt
 setup.cfg
 setup.py
 versioneer.py
 docs/Makefile
 docs/make.bat
 docs/source/conf.py
+docs/source/examples.rst
 docs/source/index.rst
 docs/source/installation.rst
-docs/source/notebooks-new-api.rst
-docs/source/notebooks-old-api.rst
 docs/source/release-history.rst
 docs/source/simulations.rst
 sirepo_bluesky/__init__.py
 sirepo_bluesky/_version.py
 sirepo_bluesky/madx_flyer.py
 sirepo_bluesky/madx_handler.py
 sirepo_bluesky/shadow_detector.py
```

### Comparing `sirepo-bluesky-0.6.1/versioneer.py` & `sirepo-bluesky-0.6.2/versioneer.py`

 * *Files identical despite different names*

