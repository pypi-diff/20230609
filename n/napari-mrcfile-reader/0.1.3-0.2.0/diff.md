# Comparing `tmp/napari-mrcfile-reader-0.1.3.tar.gz` & `tmp/napari-mrcfile-reader-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-mrcfile-reader-0.1.3.tar", last modified: Thu Sep 16 12:19:00 2021, max compression
+gzip compressed data, was "napari-mrcfile-reader-0.2.0.tar", last modified: Thu Jun  8 22:53:57 2023, max compression
```

## Comparing `napari-mrcfile-reader-0.1.3.tar` & `napari-mrcfile-reader-0.2.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-16 12:19:00.751345 napari-mrcfile-reader-0.1.3/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-16 12:19:00.743345 napari-mrcfile-reader-0.1.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-16 12:19:00.747345 napari-mrcfile-reader-0.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2152 2021-09-16 12:18:49.000000 napari-mrcfile-reader-0.1.3/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1000 2021-09-16 12:18:49.000000 napari-mrcfile-reader-0.1.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1492 2021-09-16 12:18:49.000000 napari-mrcfile-reader-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      121 2021-09-16 12:18:49.000000 napari-mrcfile-reader-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3429 2021-09-16 12:19:00.751345 napari-mrcfile-reader-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2421 2021-09-16 12:18:49.000000 napari-mrcfile-reader-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (121)  2301932 2021-09-16 12:18:49.000000 napari-mrcfile-reader-0.1.3/example.gif
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-16 12:19:00.751345 napari-mrcfile-reader-0.1.3/napari_mrcfile_reader/
--rw-r--r--   0 runner    (1001) docker     (121)      225 2021-09-16 12:18:49.000000 napari-mrcfile-reader-0.1.3/napari_mrcfile_reader/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-16 12:19:00.751345 napari-mrcfile-reader-0.1.3/napari_mrcfile_reader/_tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-16 12:18:49.000000 napari-mrcfile-reader-0.1.3/napari_mrcfile_reader/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      945 2021-09-16 12:18:49.000000 napari-mrcfile-reader-0.1.3/napari_mrcfile_reader/_tests/test_mrcfile_reader.py
--rw-r--r--   0 runner    (1001) docker     (121)      142 2021-09-16 12:19:00.000000 napari-mrcfile-reader-0.1.3/napari_mrcfile_reader/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     2837 2021-09-16 12:18:49.000000 napari-mrcfile-reader-0.1.3/napari_mrcfile_reader/mrcfile_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-16 12:19:00.751345 napari-mrcfile-reader-0.1.3/napari_mrcfile_reader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3429 2021-09-16 12:19:00.000000 napari-mrcfile-reader-0.1.3/napari_mrcfile_reader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      597 2021-09-16 12:19:00.000000 napari-mrcfile-reader-0.1.3/napari_mrcfile_reader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-16 12:19:00.000000 napari-mrcfile-reader-0.1.3/napari_mrcfile_reader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       56 2021-09-16 12:19:00.000000 napari-mrcfile-reader-0.1.3/napari_mrcfile_reader.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       53 2021-09-16 12:19:00.000000 napari-mrcfile-reader-0.1.3/napari_mrcfile_reader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2021-09-16 12:19:00.000000 napari-mrcfile-reader-0.1.3/napari_mrcfile_reader.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       53 2021-09-16 12:18:49.000000 napari-mrcfile-reader-0.1.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-09-16 12:19:00.751345 napari-mrcfile-reader-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1946 2021-09-16 12:18:49.000000 napari-mrcfile-reader-0.1.3/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)      492 2021-09-16 12:18:49.000000 napari-mrcfile-reader-0.1.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:57.991822 napari-mrcfile-reader-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:57.983821 napari-mrcfile-reader-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:57.987822 napari-mrcfile-reader-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-06-08 22:53:29.000000 napari-mrcfile-reader-0.2.0/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-06-08 22:53:29.000000 napari-mrcfile-reader-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-08 22:53:29.000000 napari-mrcfile-reader-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-08 22:53:29.000000 napari-mrcfile-reader-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-06-08 22:53:57.991822 napari-mrcfile-reader-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-06-08 22:53:29.000000 napari-mrcfile-reader-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)  2301932 2023-06-08 22:53:29.000000 napari-mrcfile-reader-0.2.0/example.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-08 22:53:29.000000 napari-mrcfile-reader-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-06-08 22:53:57.991822 napari-mrcfile-reader-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:57.987822 napari-mrcfile-reader-0.2.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:29.000000 napari-mrcfile-reader-0.2.0/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:57.987822 napari-mrcfile-reader-0.2.0/src/napari_mrcfile_reader/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-08 22:53:29.000000 napari-mrcfile-reader-0.2.0/src/napari_mrcfile_reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-06-08 22:53:29.000000 napari-mrcfile-reader-0.2.0/src/napari_mrcfile_reader/_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:57.991822 napari-mrcfile-reader-0.2.0/src/napari_mrcfile_reader/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-08 22:53:29.000000 napari-mrcfile-reader-0.2.0/src/napari_mrcfile_reader/_tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-08 22:53:57.000000 napari-mrcfile-reader-0.2.0/src/napari_mrcfile_reader/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-08 22:53:29.000000 napari-mrcfile-reader-0.2.0/src/napari_mrcfile_reader/napari.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:57.987822 napari-mrcfile-reader-0.2.0/src/napari_mrcfile_reader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-06-08 22:53:57.000000 napari-mrcfile-reader-0.2.0/src/napari_mrcfile_reader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-08 22:53:57.000000 napari-mrcfile-reader-0.2.0/src/napari_mrcfile_reader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 22:53:57.000000 napari-mrcfile-reader-0.2.0/src/napari_mrcfile_reader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-08 22:53:57.000000 napari-mrcfile-reader-0.2.0/src/napari_mrcfile_reader.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-08 22:53:57.000000 napari-mrcfile-reader-0.2.0/src/napari_mrcfile_reader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-08 22:53:57.000000 napari-mrcfile-reader-0.2.0/src/napari_mrcfile_reader.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-08 22:53:29.000000 napari-mrcfile-reader-0.2.0/tox.ini
```

### Comparing `napari-mrcfile-reader-0.1.3/.gitignore` & `napari-mrcfile-reader-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `napari-mrcfile-reader-0.1.3/LICENSE` & `napari-mrcfile-reader-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-mrcfile-reader-0.1.3/PKG-INFO` & `napari-mrcfile-reader-0.2.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 Metadata-Version: 2.1
 Name: napari-mrcfile-reader
-Version: 0.1.3
-Summary: read MRC format image files into napari
+Version: 0.2.0
+Summary: Read MRC2014 files in napari using mrcfile.
 Home-page: https://github.com/alisterburt/napari-mrcfile-reader
 Author: Alister Burt
 Author-email: alisterburt@gmail.com
-License: BSD-3
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Testing
+License: BSD-3-Clause
+Project-URL: Bug Tracker, https://github.com/alisterburt/napari-mrcfile-reader/issues
+Project-URL: Documentation, https://github.com/alisterburt/napari-mrcfile-reader#README.md
+Project-URL: Source Code, https://github.com/alisterburt/napari-mrcfile-reader
+Project-URL: User Support, https://github.com/alisterburt/napari-mrcfile-reader/issues
+Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: napari
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: BSD License
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Scientific/Engineering :: Image Processing
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: testing
 License-File: LICENSE
 
 # napari-mrcfile-reader
 
 [![License](https://img.shields.io/pypi/l/napari-mrcfile-reader.svg?color=green)](https://github.com/alisterburt/napari-mrcfile-reader/raw/master/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/napari-mrcfile-reader.svg?color=green)](https://pypi.org/project/napari-mrcfile-reader)
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-mrcfile-reader.svg?color=green)](https://python.org)
@@ -75,8 +78,7 @@
 [Mozilla Public License 2.0]: https://www.mozilla.org/media/MPL/2.0/index.txt
 [cookiecutter-napari-plugin]: https://github.com/napari/cookiecutter-napari-plugin
 [file an issue]: https://github.com/alisterburt/napari-mrcfile-reader/issues
 [napari]: https://github.com/napari/napari
 [tox]: https://tox.readthedocs.io/en/latest/
 [pip]: https://pypi.org/project/pip/
 [PyPI]: https://pypi.org/
-
```

### Comparing `napari-mrcfile-reader-0.1.3/README.md` & `napari-mrcfile-reader-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `napari-mrcfile-reader-0.1.3/example.gif` & `napari-mrcfile-reader-0.2.0/example.gif`

 * *Files identical despite different names*

### Comparing `napari-mrcfile-reader-0.1.3/napari_mrcfile_reader/_tests/test_mrcfile_reader.py` & `napari-mrcfile-reader-0.2.0/src/napari_mrcfile_reader/_tests/test_reader.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-import numpy as np
 import mrcfile
+import numpy as np
+
 from napari_mrcfile_reader import napari_get_reader
 
 
 # tmp_path is a pytest fixture
 def test_reader(tmp_path):
-    # write a fake MRC file using mrcfile
+    """An example of how you might test your plugin."""
+
+    # write some fake data using your supported file format
     my_test_file = str(tmp_path / "myfile.mrc")
     original_data = np.random.rand(20, 20).astype(np.float32)
-    mrcfile.new(my_test_file, original_data)
+    mrcfile.write(my_test_file, original_data)
 
     # try to read it back in
     reader = napari_get_reader(my_test_file)
     assert callable(reader)
 
     # make sure we're delivering the right format
     layer_data_list = reader(my_test_file)
```

### Comparing `napari-mrcfile-reader-0.1.3/napari_mrcfile_reader/mrcfile_reader.py` & `napari-mrcfile-reader-0.2.0/src/napari_mrcfile_reader/_reader.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,20 @@
 """
-This module is an mrc file reader plugin for napari.
+This module is an example of a barebones numpy reader plugin for napari.
 
-It implements the ``napari_get_reader`` hook specification to create
-a reader plugin.
-see: https://napari.org/docs/plugins/hook_specifications.html
-
-Replace code below accordingly.  For complete documentation see:
-https://napari.org/docs/plugins/for_plugin_developers.html
+It implements the Reader specification, but your plugin may choose to
+implement multiple readers or even other plugin contributions. see:
+https://napari.org/stable/plugins/guides.html?#readers
 """
-import numpy as np
-from napari_plugin_engine import napari_hook_implementation
 import mrcfile
+import numpy as np
 
 
-@napari_hook_implementation
 def napari_get_reader(path):
-    """A basic implementation of the napari_get_reader hook specification.
+    """A basic implementation of a Reader contribution.
 
     Parameters
     ----------
     path : str or list of str
         Path to file, or list of paths.
 
     Returns
@@ -31,15 +26,23 @@
     if isinstance(path, list):
         # reader plugins may be handed single path, or a list of paths.
         # if it is a list, it is assumed to be an image stack...
         # so we are only going to look at the first file.
         path = path[0]
 
     # if we know we cannot read the file, we immediately return None.
-    extensions = ".mrc", ".mrcs", ".map"
+    extensions = (
+        '.mrc',
+        '.mrcs',
+        '.map',
+        '.st',
+        '.rec',
+        '.preali',
+        '.ali',
+    )
     if not path.endswith(extensions):
         return None
 
     # otherwise we return the *function* that can read ``path``.
     return reader_function
 
 
@@ -63,18 +66,30 @@
         a dict of keyword arguments for the corresponding viewer.add_* method
         in napari, and layer_type is a lower-case string naming the type of layer.
         Both "meta", and "layer_type" are optional. napari will default to
         layer_type=="image" if not provided
     """
     # handle both a string and a list of strings
     paths = [path] if isinstance(path, str) else path
-    # load all files into array
-    arrays = [mrcfile.open(_path, permissive=True).data for _path in paths]
-    # stack arrays into single array
-    data = np.squeeze(np.stack(arrays))
 
     # optional kwargs for the corresponding viewer.add_* method
     # https://napari.org/docs/api/napari.components.html#module-napari.components.add_layers_mixin
     add_kwargs = {}
 
-    layer_type = "image"  # optional, default is "image"
-    return [(data, add_kwargs, layer_type)]
+    # optional, default is "image"
+    layer_type = "image"
+
+    # load all files into array
+    layer_data = []
+    for _path in paths:
+
+        # Read mrcfile as a memory mapped file
+        data = mrcfile.mmap(_path, permissive=True).data
+
+        # Append two layers if the data type is complex
+        if data.dtype in [np.complex64, np.complex128]:
+            layer_data.append((np.abs(data), {"name": "amplitude"}, layer_type))
+            layer_data.append((np.angle(data), {"name": "phase"}, layer_type))
+        else:
+            layer_data.append((data, add_kwargs, layer_type))
+
+    return layer_data
```

### Comparing `napari-mrcfile-reader-0.1.3/napari_mrcfile_reader.egg-info/PKG-INFO` & `napari-mrcfile-reader-0.2.0/src/napari_mrcfile_reader.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 Metadata-Version: 2.1
 Name: napari-mrcfile-reader
-Version: 0.1.3
-Summary: read MRC format image files into napari
+Version: 0.2.0
+Summary: Read MRC2014 files in napari using mrcfile.
 Home-page: https://github.com/alisterburt/napari-mrcfile-reader
 Author: Alister Burt
 Author-email: alisterburt@gmail.com
-License: BSD-3
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Testing
+License: BSD-3-Clause
+Project-URL: Bug Tracker, https://github.com/alisterburt/napari-mrcfile-reader/issues
+Project-URL: Documentation, https://github.com/alisterburt/napari-mrcfile-reader#README.md
+Project-URL: Source Code, https://github.com/alisterburt/napari-mrcfile-reader
+Project-URL: User Support, https://github.com/alisterburt/napari-mrcfile-reader/issues
+Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: napari
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: BSD License
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Scientific/Engineering :: Image Processing
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: testing
 License-File: LICENSE
 
 # napari-mrcfile-reader
 
 [![License](https://img.shields.io/pypi/l/napari-mrcfile-reader.svg?color=green)](https://github.com/alisterburt/napari-mrcfile-reader/raw/master/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/napari-mrcfile-reader.svg?color=green)](https://pypi.org/project/napari-mrcfile-reader)
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-mrcfile-reader.svg?color=green)](https://python.org)
@@ -75,8 +78,7 @@
 [Mozilla Public License 2.0]: https://www.mozilla.org/media/MPL/2.0/index.txt
 [cookiecutter-napari-plugin]: https://github.com/napari/cookiecutter-napari-plugin
 [file an issue]: https://github.com/alisterburt/napari-mrcfile-reader/issues
 [napari]: https://github.com/napari/napari
 [tox]: https://tox.readthedocs.io/en/latest/
 [pip]: https://pypi.org/project/pip/
 [PyPI]: https://pypi.org/
-
```

### Comparing `napari-mrcfile-reader-0.1.3/napari_mrcfile_reader.egg-info/SOURCES.txt` & `napari-mrcfile-reader-0.2.0/src/napari_mrcfile_reader.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 .gitignore
 LICENSE
 MANIFEST.in
 README.md
 example.gif
-requirements.txt
-setup.py
+pyproject.toml
+setup.cfg
 tox.ini
 .github/workflows/test_and_deploy.yml
-napari_mrcfile_reader/__init__.py
-napari_mrcfile_reader/_version.py
-napari_mrcfile_reader/mrcfile_reader.py
-napari_mrcfile_reader.egg-info/PKG-INFO
-napari_mrcfile_reader.egg-info/SOURCES.txt
-napari_mrcfile_reader.egg-info/dependency_links.txt
-napari_mrcfile_reader.egg-info/entry_points.txt
-napari_mrcfile_reader.egg-info/requires.txt
-napari_mrcfile_reader.egg-info/top_level.txt
-napari_mrcfile_reader/_tests/__init__.py
-napari_mrcfile_reader/_tests/test_mrcfile_reader.py
+src/__init__.py
+src/napari_mrcfile_reader/__init__.py
+src/napari_mrcfile_reader/_reader.py
+src/napari_mrcfile_reader/_version.py
+src/napari_mrcfile_reader/napari.yaml
+src/napari_mrcfile_reader.egg-info/PKG-INFO
+src/napari_mrcfile_reader.egg-info/SOURCES.txt
+src/napari_mrcfile_reader.egg-info/dependency_links.txt
+src/napari_mrcfile_reader.egg-info/entry_points.txt
+src/napari_mrcfile_reader.egg-info/requires.txt
+src/napari_mrcfile_reader.egg-info/top_level.txt
+src/napari_mrcfile_reader/_tests/test_reader.py
```

