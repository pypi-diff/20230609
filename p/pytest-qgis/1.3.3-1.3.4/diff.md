# Comparing `tmp/pytest-qgis-1.3.3.tar.gz` & `tmp/pytest-qgis-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-qgis-1.3.3.tar", last modified: Wed May 31 14:42:19 2023, max compression
+gzip compressed data, was "pytest-qgis-1.3.4.tar", last modified: Fri Jun  9 12:32:21 2023, max compression
```

## Comparing `pytest-qgis-1.3.3.tar` & `pytest-qgis-1.3.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:42:19.171253 pytest-qgis-1.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)    18073 2023-05-31 14:42:10.000000 pytest-qgis-1.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7409 2023-05-31 14:42:19.171253 pytest-qgis-1.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-05-31 14:42:10.000000 pytest-qgis-1.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-31 14:42:19.171253 pytest-qgis-1.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-31 14:42:10.000000 pytest-qgis-1.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:42:19.167253 pytest-qgis-1.3.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:42:19.167253 pytest-qgis-1.3.3/src/pytest_qgis/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-31 14:42:10.000000 pytest-qgis-1.3.3/src/pytest_qgis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-31 14:42:10.000000 pytest-qgis-1.3.3/src/pytest_qgis/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-31 14:42:10.000000 pytest-qgis-1.3.3/src/pytest_qgis/mock_qgis_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:42:10.000000 pytest-qgis-1.3.3/src/pytest_qgis/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    16281 2023-05-31 14:42:10.000000 pytest-qgis-1.3.3/src/pytest_qgis/pytest_qgis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-05-31 14:42:10.000000 pytest-qgis-1.3.3/src/pytest_qgis/qgis_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8502 2023-05-31 14:42:10.000000 pytest-qgis-1.3.3/src/pytest_qgis/qgis_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     6074 2023-05-31 14:42:10.000000 pytest-qgis-1.3.3/src/pytest_qgis/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:42:19.171253 pytest-qgis-1.3.3/src/pytest_qgis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7409 2023-05-31 14:42:19.000000 pytest-qgis-1.3.3/src/pytest_qgis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-31 14:42:19.000000 pytest-qgis-1.3.3/src/pytest_qgis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 14:42:19.000000 pytest-qgis-1.3.3/src/pytest_qgis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-31 14:42:19.000000 pytest-qgis-1.3.3/src/pytest_qgis.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-31 14:42:19.000000 pytest-qgis-1.3.3/src/pytest_qgis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-31 14:42:19.000000 pytest-qgis-1.3.3/src/pytest_qgis.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:42:19.171253 pytest-qgis-1.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-05-31 14:42:10.000000 pytest-qgis-1.3.3/tests/test_ini.py
--rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-05-31 14:42:10.000000 pytest-qgis-1.3.3/tests/test_pytest_qgis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-05-31 14:42:10.000000 pytest-qgis-1.3.3/tests/test_qgis_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-05-31 14:42:10.000000 pytest-qgis-1.3.3/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:32:21.546595 pytest-qgis-1.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    18073 2023-06-09 12:32:12.000000 pytest-qgis-1.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7664 2023-06-09 12:32:21.546595 pytest-qgis-1.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-06-09 12:32:12.000000 pytest-qgis-1.3.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-09 12:32:21.546595 pytest-qgis-1.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-09 12:32:12.000000 pytest-qgis-1.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:32:21.542595 pytest-qgis-1.3.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:32:21.546595 pytest-qgis-1.3.4/src/pytest_qgis/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-09 12:32:12.000000 pytest-qgis-1.3.4/src/pytest_qgis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-09 12:32:12.000000 pytest-qgis-1.3.4/src/pytest_qgis/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-06-09 12:32:12.000000 pytest-qgis-1.3.4/src/pytest_qgis/mock_qgis_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 12:32:12.000000 pytest-qgis-1.3.4/src/pytest_qgis/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    16365 2023-06-09 12:32:12.000000 pytest-qgis-1.3.4/src/pytest_qgis/pytest_qgis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-06-09 12:32:12.000000 pytest-qgis-1.3.4/src/pytest_qgis/qgis_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8502 2023-06-09 12:32:12.000000 pytest-qgis-1.3.4/src/pytest_qgis/qgis_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6074 2023-06-09 12:32:12.000000 pytest-qgis-1.3.4/src/pytest_qgis/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:32:21.546595 pytest-qgis-1.3.4/src/pytest_qgis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7664 2023-06-09 12:32:21.000000 pytest-qgis-1.3.4/src/pytest_qgis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-09 12:32:21.000000 pytest-qgis-1.3.4/src/pytest_qgis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 12:32:21.000000 pytest-qgis-1.3.4/src/pytest_qgis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-09 12:32:21.000000 pytest-qgis-1.3.4/src/pytest_qgis.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-09 12:32:21.000000 pytest-qgis-1.3.4/src/pytest_qgis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-09 12:32:21.000000 pytest-qgis-1.3.4/src/pytest_qgis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:32:21.546595 pytest-qgis-1.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-06-09 12:32:12.000000 pytest-qgis-1.3.4/tests/test_ini.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-06-09 12:32:12.000000 pytest-qgis-1.3.4/tests/test_pytest_qgis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-06-09 12:32:12.000000 pytest-qgis-1.3.4/tests/test_qgis_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-06-09 12:32:12.000000 pytest-qgis-1.3.4/tests/test_utils.py
```

### Comparing `pytest-qgis-1.3.3/LICENSE` & `pytest-qgis-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-qgis-1.3.3/PKG-INFO` & `pytest-qgis-1.3.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-qgis
-Version: 1.3.3
+Version: 1.3.4
 Summary: A pytest plugin for testing QGIS python plugins
 Home-page: https://github.com/GispoCoding/pytest-qgis
 Author: Joona Laine
 Author-email: info@gispo.fi
 Maintainer: Gispo Ltd.
 Maintainer-email: info@gispo.fi
 License: GNU GPL v2.0
@@ -85,15 +85,15 @@
 
 ### Utility tools
 
 * `clean_qgis_layer` decorator found in `pytest_qgis.utils` is a decorator which can be used with `QgsMapLayer` fixtures
   to ensure that they are cleaned properly if they are used but not added to the `QgsProject`. This is only needed with
   layers with other than memory provider.
    ```python
-   # conftest.py of start of a test file
+   # conftest.py or start of a test file
    import pytest
    from pytest_qgis.utils import clean_qgis_layer
    from qgis.core import QgsVectorLayer
 
    @pytest.fixture()
    @clean_qgis_layer
    def some_layer() -> QgsVectorLayer:
@@ -103,19 +103,21 @@
 
 ### Hooks
 
 * `pytest_configure` hook is used to initialize and
   configure [`QgsApplication`](https://qgis.org/pyqgis/master/core/QgsApplication.html). With QGIS >= 3.18 it is also
   used to patch `qgis.utils.iface` with `qgis_iface` automatically.
 
+  > Be careful not to import modules importing `qgis.utils.iface` in the root of conftest, because the `pytest_configure` hook has not yet patched `iface` in that point. See [this issue](https://github.com/GispoCoding/pytest-qgis/issues/35) for details.
+
 ### Command line options
 
 * `--qgis_disable_gui` can be used to disable graphical user interface in tests. This speeds up the tests that use Qt
   widgets of the plugin.
-* `--qgis_disable_init` can be used to prevent QGIS (QgsApllication) from initializing. Mainly used in internal testing.
+* `--qgis_disable_init` can be used to prevent QGIS (QgsApplication) from initializing. Mainly used in internal testing.
 
 ### ini-options
 
 * `qgis_qui_enabled` whether the QUI will be visible or not. Defaults to `True`. Command line
   option `--qgis_disable_gui` will override this.
 * `qgis_canvas_width` width of the QGIS canvas in pixels. Defaults to 600.
 * `qgis_canvas_height` height of the QGIS canvas in pixels. Defaults to 600.
```

### Comparing `pytest-qgis-1.3.3/README.md` & `pytest-qgis-1.3.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
 ### Utility tools
 
 * `clean_qgis_layer` decorator found in `pytest_qgis.utils` is a decorator which can be used with `QgsMapLayer` fixtures
   to ensure that they are cleaned properly if they are used but not added to the `QgsProject`. This is only needed with
   layers with other than memory provider.
    ```python
-   # conftest.py of start of a test file
+   # conftest.py or start of a test file
    import pytest
    from pytest_qgis.utils import clean_qgis_layer
    from qgis.core import QgsVectorLayer
 
    @pytest.fixture()
    @clean_qgis_layer
    def some_layer() -> QgsVectorLayer:
@@ -70,19 +70,21 @@
 
 ### Hooks
 
 * `pytest_configure` hook is used to initialize and
   configure [`QgsApplication`](https://qgis.org/pyqgis/master/core/QgsApplication.html). With QGIS >= 3.18 it is also
   used to patch `qgis.utils.iface` with `qgis_iface` automatically.
 
+  > Be careful not to import modules importing `qgis.utils.iface` in the root of conftest, because the `pytest_configure` hook has not yet patched `iface` in that point. See [this issue](https://github.com/GispoCoding/pytest-qgis/issues/35) for details.
+
 ### Command line options
 
 * `--qgis_disable_gui` can be used to disable graphical user interface in tests. This speeds up the tests that use Qt
   widgets of the plugin.
-* `--qgis_disable_init` can be used to prevent QGIS (QgsApllication) from initializing. Mainly used in internal testing.
+* `--qgis_disable_init` can be used to prevent QGIS (QgsApplication) from initializing. Mainly used in internal testing.
 
 ### ini-options
 
 * `qgis_qui_enabled` whether the QUI will be visible or not. Defaults to `True`. Command line
   option `--qgis_disable_gui` will override this.
 * `qgis_canvas_width` width of the QGIS canvas in pixels. Defaults to 600.
 * `qgis_canvas_height` height of the QGIS canvas in pixels. Defaults to 600.
```

### Comparing `pytest-qgis-1.3.3/setup.cfg` & `pytest-qgis-1.3.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [metadata]
 name = pytest-qgis
 author = Joona Laine
 author_email = info@gispo.fi
 maintainer = Gispo Ltd.
 maintainer_email = info@gispo.fi
-version = 1.3.3
+version = 1.3.4
 description = A pytest plugin for testing QGIS python plugins
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = pytest,qgis,QGIS,PyQGIS
 url = https://github.com/GispoCoding/pytest-qgis
 license = GNU GPL v2.0
 classifiers =
```

### Comparing `pytest-qgis-1.3.3/setup.py` & `pytest-qgis-1.3.4/setup.py`

 * *Files identical despite different names*

### Comparing `pytest-qgis-1.3.3/src/pytest_qgis/__init__.py` & `pytest-qgis-1.3.4/src/pytest_qgis/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest-qgis-1.3.3/src/pytest_qgis/_version.py` & `pytest-qgis-1.3.4/src/pytest_qgis/_version.py`

 * *Files identical despite different names*

### Comparing `pytest-qgis-1.3.3/src/pytest_qgis/mock_qgis_classes.py` & `pytest-qgis-1.3.4/src/pytest_qgis/mock_qgis_classes.py`

 * *Files identical despite different names*

### Comparing `pytest-qgis-1.3.3/src/pytest_qgis/pytest_qgis.py` & `pytest-qgis-1.3.4/src/pytest_qgis/pytest_qgis.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,23 +18,23 @@
 #  You should have received a copy of the GNU General Public License
 #  along with pytest-qgis.  If not, see <https://www.gnu.org/licenses/>.
 
 
 import os.path
 import shutil
 import sys
+import tempfile
 import time
 import warnings
 from collections import namedtuple
 from pathlib import Path
 from typing import TYPE_CHECKING, Optional
 from unittest import mock
 
 import pytest
-from _pytest.tmpdir import TempPathFactory
 from qgis.core import Qgis, QgsApplication, QgsProject, QgsRectangle, QgsVectorLayer
 from qgis.gui import QgisInterface as QgisInterfaceOrig
 from qgis.gui import QgsGui, QgsLayerTreeMapCanvasBridge, QgsMapCanvas
 from qgis.PyQt import QtCore, QtWidgets, sip
 from qgis.PyQt.QtCore import QCoreApplication
 from qgis.PyQt.QtWidgets import QMainWindow, QMessageBox, QWidget
 
@@ -88,14 +88,15 @@
 )
 
 _APP: Optional[QgsApplication] = None
 _CANVAS: Optional[QgsMapCanvas] = None
 _IFACE: Optional[QgisInterface] = None
 _PARENT: Optional[QtWidgets.QWidget] = None
 _AUTOUSE_QGIS: Optional[bool] = None
+_QGIS_CONFIG_PATH: Optional[Path] = None
 
 try:
     _QGIS_VERSION = Qgis.versionInt()
 except AttributeError:
     _QGIS_VERSION = Qgis.QGIS_VERSION_INT
 
 
@@ -149,14 +150,16 @@
     yield _APP if not request.config._plugin_settings.qgis_init_disabled else None
 
     if not request.config._plugin_settings.qgis_init_disabled:
         assert _APP
         if not sip.isdeleted(_CANVAS) and _CANVAS is not None:
             _CANVAS.deleteLater()
         _APP.exitQgis()
+        if _QGIS_CONFIG_PATH and _QGIS_CONFIG_PATH.exists():
+            shutil.rmtree(_QGIS_CONFIG_PATH)
 
 
 @pytest.fixture(scope="session")
 def qgis_parent(qgis_app: QgsApplication) -> QWidget:
     return _PARENT
 
 
@@ -276,21 +279,20 @@
             qgis_parent,
             _parse_show_map_marker(show_map_marker),
             tmp_path,
         )
 
 
 def _start_and_configure_qgis_app(config: "Config") -> None:
-    global _APP, _CANVAS, _IFACE, _PARENT
+    global _APP, _CANVAS, _IFACE, _PARENT, _QGIS_CONFIG_PATH
     settings: Settings = config._plugin_settings  # type: ignore
 
     # Use temporary path for QGIS config
-    tmp_path_factory = TempPathFactory.from_config(config, _ispytest=True)
-    config_path = tmp_path_factory.mktemp("qgis-test")
-    os.environ["QGIS_CUSTOM_CONFIG_PATH"] = str(config_path)
+    _QGIS_CONFIG_PATH = Path(tempfile.mkdtemp(prefix="pytest-qgis"))
+    os.environ["QGIS_CUSTOM_CONFIG_PATH"] = str(_QGIS_CONFIG_PATH)
 
     if not settings.qgis_init_disabled:
         _APP = QgsApplication([], GUIenabled=settings.gui_enabled)
         _APP.initQgis()
         QgsGui.editorWidgetRegistry().initEditors()
     _PARENT = QMainWindow()
     _CANVAS = QgsMapCanvas(_PARENT)
```

### Comparing `pytest-qgis-1.3.3/src/pytest_qgis/qgis_bot.py` & `pytest-qgis-1.3.4/src/pytest_qgis/qgis_bot.py`

 * *Files identical despite different names*

### Comparing `pytest-qgis-1.3.3/src/pytest_qgis/qgis_interface.py` & `pytest-qgis-1.3.4/src/pytest_qgis/qgis_interface.py`

 * *Files identical despite different names*

### Comparing `pytest-qgis-1.3.3/src/pytest_qgis/utils.py` & `pytest-qgis-1.3.4/src/pytest_qgis/utils.py`

 * *Files identical despite different names*

### Comparing `pytest-qgis-1.3.3/src/pytest_qgis.egg-info/PKG-INFO` & `pytest-qgis-1.3.4/src/pytest_qgis.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-qgis
-Version: 1.3.3
+Version: 1.3.4
 Summary: A pytest plugin for testing QGIS python plugins
 Home-page: https://github.com/GispoCoding/pytest-qgis
 Author: Joona Laine
 Author-email: info@gispo.fi
 Maintainer: Gispo Ltd.
 Maintainer-email: info@gispo.fi
 License: GNU GPL v2.0
@@ -85,15 +85,15 @@
 
 ### Utility tools
 
 * `clean_qgis_layer` decorator found in `pytest_qgis.utils` is a decorator which can be used with `QgsMapLayer` fixtures
   to ensure that they are cleaned properly if they are used but not added to the `QgsProject`. This is only needed with
   layers with other than memory provider.
    ```python
-   # conftest.py of start of a test file
+   # conftest.py or start of a test file
    import pytest
    from pytest_qgis.utils import clean_qgis_layer
    from qgis.core import QgsVectorLayer
 
    @pytest.fixture()
    @clean_qgis_layer
    def some_layer() -> QgsVectorLayer:
@@ -103,19 +103,21 @@
 
 ### Hooks
 
 * `pytest_configure` hook is used to initialize and
   configure [`QgsApplication`](https://qgis.org/pyqgis/master/core/QgsApplication.html). With QGIS >= 3.18 it is also
   used to patch `qgis.utils.iface` with `qgis_iface` automatically.
 
+  > Be careful not to import modules importing `qgis.utils.iface` in the root of conftest, because the `pytest_configure` hook has not yet patched `iface` in that point. See [this issue](https://github.com/GispoCoding/pytest-qgis/issues/35) for details.
+
 ### Command line options
 
 * `--qgis_disable_gui` can be used to disable graphical user interface in tests. This speeds up the tests that use Qt
   widgets of the plugin.
-* `--qgis_disable_init` can be used to prevent QGIS (QgsApllication) from initializing. Mainly used in internal testing.
+* `--qgis_disable_init` can be used to prevent QGIS (QgsApplication) from initializing. Mainly used in internal testing.
 
 ### ini-options
 
 * `qgis_qui_enabled` whether the QUI will be visible or not. Defaults to `True`. Command line
   option `--qgis_disable_gui` will override this.
 * `qgis_canvas_width` width of the QGIS canvas in pixels. Defaults to 600.
 * `qgis_canvas_height` height of the QGIS canvas in pixels. Defaults to 600.
```

### Comparing `pytest-qgis-1.3.3/src/pytest_qgis.egg-info/SOURCES.txt` & `pytest-qgis-1.3.4/src/pytest_qgis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest-qgis-1.3.3/tests/test_ini.py` & `pytest-qgis-1.3.4/tests/test_ini.py`

 * *Files identical despite different names*

### Comparing `pytest-qgis-1.3.3/tests/test_pytest_qgis.py` & `pytest-qgis-1.3.4/tests/test_pytest_qgis.py`

 * *Files identical despite different names*

### Comparing `pytest-qgis-1.3.3/tests/test_qgis_bot.py` & `pytest-qgis-1.3.4/tests/test_qgis_bot.py`

 * *Files identical despite different names*

### Comparing `pytest-qgis-1.3.3/tests/test_utils.py` & `pytest-qgis-1.3.4/tests/test_utils.py`

 * *Files identical despite different names*

