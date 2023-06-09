# Comparing `tmp/stac-asset-0.0.3.tar.gz` & `tmp/stac-asset-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stac-asset-0.0.3.tar", last modified: Wed May 31 21:50:05 2023, max compression
+gzip compressed data, was "stac-asset-0.0.4.tar", last modified: Fri Jun  9 18:32:33 2023, max compression
```

## Comparing `stac-asset-0.0.3.tar` & `stac-asset-0.0.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 gadomski   (501) staff       (20)        0 2023-05-31 21:50:05.937831 stac-asset-0.0.3/
--rw-r--r--   0 gadomski   (501) staff       (20)    11357 2023-05-23 19:38:34.000000 stac-asset-0.0.3/LICENSE
--rw-r--r--   0 gadomski   (501) staff       (20)     6706 2023-05-31 21:50:05.937168 stac-asset-0.0.3/PKG-INFO
--rw-r--r--   0 gadomski   (501) staff       (20)     6110 2023-05-26 20:55:38.000000 stac-asset-0.0.3/README.md
--rw-r--r--   0 gadomski   (501) staff       (20)     1041 2023-05-31 21:48:19.000000 stac-asset-0.0.3/pyproject.toml
--rw-r--r--   0 gadomski   (501) staff       (20)       38 2023-05-31 21:50:05.938099 stac-asset-0.0.3/setup.cfg
-drwxr-xr-x   0 gadomski   (501) staff       (20)        0 2023-05-31 21:50:05.912603 stac-asset-0.0.3/src/
-drwxr-xr-x   0 gadomski   (501) staff       (20)        0 2023-05-31 21:50:05.924307 stac-asset-0.0.3/src/stac_asset/
--rw-r--r--   0 gadomski   (501) staff       (20)     1233 2023-05-26 20:55:38.000000 stac-asset-0.0.3/src/stac_asset/__init__.py
--rw-r--r--   0 gadomski   (501) staff       (20)      393 2023-05-25 12:54:26.000000 stac-asset-0.0.3/src/stac_asset/__main__.py
--rw-r--r--   0 gadomski   (501) staff       (20)     6420 2023-05-31 21:45:32.000000 stac-asset-0.0.3/src/stac_asset/client.py
--rw-r--r--   0 gadomski   (501) staff       (20)     1178 2023-05-31 21:45:32.000000 stac-asset-0.0.3/src/stac_asset/earthdata_client.py
--rw-r--r--   0 gadomski   (501) staff       (20)      615 2023-05-31 21:45:32.000000 stac-asset-0.0.3/src/stac_asset/errors.py
--rw-r--r--   0 gadomski   (501) staff       (20)     1022 2023-05-31 21:45:32.000000 stac-asset-0.0.3/src/stac_asset/filesystem_client.py
--rw-r--r--   0 gadomski   (501) staff       (20)     4389 2023-05-31 21:45:32.000000 stac-asset-0.0.3/src/stac_asset/functions.py
--rw-r--r--   0 gadomski   (501) staff       (20)     1459 2023-05-31 21:45:32.000000 stac-asset-0.0.3/src/stac_asset/http_client.py
--rw-r--r--   0 gadomski   (501) staff       (20)     3749 2023-05-31 21:45:32.000000 stac-asset-0.0.3/src/stac_asset/planetary_computer_client.py
--rw-r--r--   0 gadomski   (501) staff       (20)     2129 2023-05-31 21:45:32.000000 stac-asset-0.0.3/src/stac_asset/s3_client.py
--rw-r--r--   0 gadomski   (501) staff       (20)      370 2023-05-26 20:10:27.000000 stac-asset-0.0.3/src/stac_asset/strategy.py
--rw-r--r--   0 gadomski   (501) staff       (20)      780 2023-05-31 21:45:32.000000 stac-asset-0.0.3/src/stac_asset/types.py
--rw-r--r--   0 gadomski   (501) staff       (20)     2602 2023-05-31 21:45:32.000000 stac-asset-0.0.3/src/stac_asset/usgs_eros_client.py
-drwxr-xr-x   0 gadomski   (501) staff       (20)        0 2023-05-31 21:50:05.930077 stac-asset-0.0.3/src/stac_asset.egg-info/
--rw-r--r--   0 gadomski   (501) staff       (20)     6706 2023-05-31 21:50:05.000000 stac-asset-0.0.3/src/stac_asset.egg-info/PKG-INFO
--rw-r--r--   0 gadomski   (501) staff       (20)      812 2023-05-31 21:50:05.000000 stac-asset-0.0.3/src/stac_asset.egg-info/SOURCES.txt
--rw-r--r--   0 gadomski   (501) staff       (20)        1 2023-05-31 21:50:05.000000 stac-asset-0.0.3/src/stac_asset.egg-info/dependency_links.txt
--rw-r--r--   0 gadomski   (501) staff       (20)      236 2023-05-31 21:50:05.000000 stac-asset-0.0.3/src/stac_asset.egg-info/requires.txt
--rw-r--r--   0 gadomski   (501) staff       (20)       11 2023-05-31 21:50:05.000000 stac-asset-0.0.3/src/stac_asset.egg-info/top_level.txt
-drwxr-xr-x   0 gadomski   (501) staff       (20)        0 2023-05-31 21:50:05.936149 stac-asset-0.0.3/tests/
--rw-r--r--   0 gadomski   (501) staff       (20)      353 2023-05-31 21:36:43.000000 stac-asset-0.0.3/tests/test_download.py
--rw-r--r--   0 gadomski   (501) staff       (20)      707 2023-05-26 20:58:46.000000 stac-asset-0.0.3/tests/test_earthdata_client.py
--rw-r--r--   0 gadomski   (501) staff       (20)     2156 2023-05-26 20:29:22.000000 stac-asset-0.0.3/tests/test_filesystem_client.py
--rw-r--r--   0 gadomski   (501) staff       (20)      416 2023-05-25 20:46:44.000000 stac-asset-0.0.3/tests/test_open.py
--rw-r--r--   0 gadomski   (501) staff       (20)      704 2023-05-25 19:53:19.000000 stac-asset-0.0.3/tests/test_planetary_computer_client.py
--rw-r--r--   0 gadomski   (501) staff       (20)     1187 2023-05-26 13:07:26.000000 stac-asset-0.0.3/tests/test_s3_client.py
--rw-r--r--   0 gadomski   (501) staff       (20)      869 2023-05-25 12:54:26.000000 stac-asset-0.0.3/tests/test_usgs_eros_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:32:33.380683 stac-asset-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-09 18:32:23.000000 stac-asset-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8216 2023-06-09 18:32:33.380683 stac-asset-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7343 2023-06-09 18:32:23.000000 stac-asset-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-09 18:32:23.000000 stac-asset-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 18:32:33.380683 stac-asset-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:32:33.376683 stac-asset-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:32:33.380683 stac-asset-0.0.4/src/stac_asset/
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-06-09 18:32:23.000000 stac-asset-0.0.4/src/stac_asset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-06-09 18:32:23.000000 stac-asset-0.0.4/src/stac_asset/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12051 2023-06-09 18:32:23.000000 stac-asset-0.0.4/src/stac_asset/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-06-09 18:32:23.000000 stac-asset-0.0.4/src/stac_asset/earthdata_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-09 18:32:23.000000 stac-asset-0.0.4/src/stac_asset/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-06-09 18:32:23.000000 stac-asset-0.0.4/src/stac_asset/filesystem_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-06-09 18:32:23.000000 stac-asset-0.0.4/src/stac_asset/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-06-09 18:32:23.000000 stac-asset-0.0.4/src/stac_asset/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-06-09 18:32:23.000000 stac-asset-0.0.4/src/stac_asset/planetary_computer_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-06-09 18:32:23.000000 stac-asset-0.0.4/src/stac_asset/s3_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-09 18:32:23.000000 stac-asset-0.0.4/src/stac_asset/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-09 18:32:23.000000 stac-asset-0.0.4/src/stac_asset/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-06-09 18:32:23.000000 stac-asset-0.0.4/src/stac_asset/usgs_eros_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:32:33.380683 stac-asset-0.0.4/src/stac_asset.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8216 2023-06-09 18:32:33.000000 stac-asset-0.0.4/src/stac_asset.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-06-09 18:32:33.000000 stac-asset-0.0.4/src/stac_asset.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 18:32:33.000000 stac-asset-0.0.4/src/stac_asset.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-09 18:32:33.000000 stac-asset-0.0.4/src/stac_asset.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-09 18:32:33.000000 stac-asset-0.0.4/src/stac_asset.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-09 18:32:33.000000 stac-asset-0.0.4/src/stac_asset.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:32:33.380683 stac-asset-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-06-09 18:32:23.000000 stac-asset-0.0.4/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-09 18:32:23.000000 stac-asset-0.0.4/tests/test_earthdata_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-06-09 18:32:23.000000 stac-asset-0.0.4/tests/test_filesystem_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-09 18:32:23.000000 stac-asset-0.0.4/tests/test_planetary_computer_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-06-09 18:32:23.000000 stac-asset-0.0.4/tests/test_s3_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-09 18:32:23.000000 stac-asset-0.0.4/tests/test_usgs_eros_client.py
```

### Comparing `stac-asset-0.0.3/LICENSE` & `stac-asset-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `stac-asset-0.0.3/PKG-INFO` & `stac-asset-0.0.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,55 +1,68 @@
-Metadata-Version: 2.1
-Name: stac-asset
-Version: 0.0.3
-Summary: Read, download, and write STAC assets across platforms and providers
-Author-email: Pete Gadomski <pete.gadomski@gmail.com>
-License: Apache-2.0
-Project-URL: repository, https://github.com/gadomski/stac-asset
-Project-URL: changelog, https://github.com/gadomski/stac-asset/blob/main/CHANGELOG.md
-Keywords: stac,async
-Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 3 - Alpha
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: docs
-License-File: LICENSE
-
 # stac-asset
 
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/gadomski/stac-asset/ci.yaml?style=for-the-badge)](https://github.com/gadomski/stac-asset/actions/workflows/ci.yaml)
 [![Read the Docs](https://img.shields.io/readthedocs/stac-asset?style=for-the-badge)](https://stac-asset.readthedocs.io/en/stable/)
 [![PyPI](https://img.shields.io/pypi/v/stac-asset?style=for-the-badge)](https://pypi.org/project/stac-asset)
 
 Download STAC Assets using a variety of authentication schemes.
 
 ## Installation
 
 ```shell
 pip install stac-asset
 ```
 
+To use the command-line interface (CLI):
+
+```shell
+pip install 'stac-asset[cli]'
+```
+
 ## Usage
 
+### API
+
 Here's how to download a STAC [Item](https://github.com/radiantearth/stac-spec/blob/master/item-spec/item-spec.md) and all of its assets to a local directory using the top-level function.
 The correct [client](#clients) will be guessed from the assets' href.
 Each asset's href will be updated to point to the local file.
 
 ```python
 import stac_asset
 
 href = "https://raw.githubusercontent.com/radiantearth/stac-spec/master/examples/simple-item.json"
 await stac_asset.download_item_from_href(href, ".")
 ```
 
+### CLI
+
 To download an item using the command line:
 
-```python
-python -m stac_asset https://raw.githubusercontent.com/radiantearth/stac-spec/master/examples/simple-item.json .
+```shell
+stac-asset download https://raw.githubusercontent.com/radiantearth/stac-spec/master/examples/simple-item.json
+```
+
+To download all assets from the results of a [pystac-client](https://github.com/stac-utils/pystac-client) search, and save the item collection to a file named `item-collection.json`:
+
+```shell
+stac-client search https://planetarycomputer.microsoft.com/api/stac/v1 -c landsat-c2-l2 --max-items 1 | \
+    stac-asset download > item-collection.json
+```
+
+If you'd like to only download certain assets, e.g. a preview image, you can use the include `-i` flag:
+
+```shell
+stac-client search https://planetarycomputer.microsoft.com/api/stac/v1 -c landsat-c2-l2 --max-items 1 | \
+    stac-asset download -i rendered_preview -q
+```
+
+If you do a lot of downloads, you may want an alias:
+
+```shell
+alias stac-download="stac-asset download"
 ```
 
 See [the documentation](https://stac-asset.readthedocs.io/en/stable/index.html) for more examples and complete API documentation.
 
 ### Clients
 
 This library comes with several clients, each tailored for a specific data provider model and authentication scheme.
@@ -105,23 +118,30 @@
   - [x] http
   - [x] s3
     - [x] requestor pays
     - [ ] custom endpoint
   - [x] custom authentication
     - [x] Planetary Computer
     - [x] USGS EROS
-    - [ ] NASA
+    - [x]  NASA
 - [ ] Copy directly from source to destination ("skip local")
 - [ ] Add new assets to an item
 - [ ] Update an existing asset
 - [ ] Delete assets
 - [ ] Templated paths on download
 - [ ] (possible) Support the file extension's local path
 - [ ] Checksum validation and creation
-- [ ] CLI
+- [x] CLI
+
+## Versioning
+
+This project does its best to adhere to [semantic versioning](https://semver.org/).
+Any module, class, constant, or function that does not begin with a `_` is considered part of our public API for versioning purposes.
+Our command-line interface (CLI) is NOT considered part of our public API, and may change in breaking ways at any time.
+If you need stability promises, use our API.
 
 ## Contributing
 
 Use Github [issues](https://github.com/gadomski/stac-asset/issues) to report bugs and request new features.
 Use Github [pull requests](https://github.com/gadomski/stac-asset/pulls) to fix bugs and propose new features.
 
 ## Developing
```

### Comparing `stac-asset-0.0.3/README.md` & `stac-asset-0.0.4/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,38 +1,91 @@
+Metadata-Version: 2.1
+Name: stac-asset
+Version: 0.0.4
+Summary: Read and download STAC assets across platforms and providers
+Author-email: Pete Gadomski <pete.gadomski@gmail.com>
+License: Apache-2.0
+Project-URL: repository, https://github.com/gadomski/stac-asset
+Project-URL: changelog, https://github.com/gadomski/stac-asset/blob/main/CHANGELOG.md
+Keywords: stac,async
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Development Status :: 3 - Alpha
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: cli
+Provides-Extra: dev
+Provides-Extra: docs
+License-File: LICENSE
+
 # stac-asset
 
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/gadomski/stac-asset/ci.yaml?style=for-the-badge)](https://github.com/gadomski/stac-asset/actions/workflows/ci.yaml)
 [![Read the Docs](https://img.shields.io/readthedocs/stac-asset?style=for-the-badge)](https://stac-asset.readthedocs.io/en/stable/)
 [![PyPI](https://img.shields.io/pypi/v/stac-asset?style=for-the-badge)](https://pypi.org/project/stac-asset)
 
 Download STAC Assets using a variety of authentication schemes.
 
 ## Installation
 
 ```shell
 pip install stac-asset
 ```
 
+To use the command-line interface (CLI):
+
+```shell
+pip install 'stac-asset[cli]'
+```
+
 ## Usage
 
+### API
+
 Here's how to download a STAC [Item](https://github.com/radiantearth/stac-spec/blob/master/item-spec/item-spec.md) and all of its assets to a local directory using the top-level function.
 The correct [client](#clients) will be guessed from the assets' href.
 Each asset's href will be updated to point to the local file.
 
 ```python
 import stac_asset
 
 href = "https://raw.githubusercontent.com/radiantearth/stac-spec/master/examples/simple-item.json"
 await stac_asset.download_item_from_href(href, ".")
 ```
 
+### CLI
+
 To download an item using the command line:
 
-```python
-python -m stac_asset https://raw.githubusercontent.com/radiantearth/stac-spec/master/examples/simple-item.json .
+```shell
+stac-asset download https://raw.githubusercontent.com/radiantearth/stac-spec/master/examples/simple-item.json
+```
+
+To download all assets from the results of a [pystac-client](https://github.com/stac-utils/pystac-client) search, and save the item collection to a file named `item-collection.json`:
+
+```shell
+stac-client search https://planetarycomputer.microsoft.com/api/stac/v1 -c landsat-c2-l2 --max-items 1 | \
+    stac-asset download > item-collection.json
+```
+
+If you'd like to only download certain assets, e.g. a preview image, you can use the include `-i` flag:
+
+```shell
+stac-client search https://planetarycomputer.microsoft.com/api/stac/v1 -c landsat-c2-l2 --max-items 1 | \
+    stac-asset download -i rendered_preview -q
+```
+
+If you do a lot of downloads, you may want an alias:
+
+```shell
+alias stac-download="stac-asset download"
 ```
 
 See [the documentation](https://stac-asset.readthedocs.io/en/stable/index.html) for more examples and complete API documentation.
 
 ### Clients
 
 This library comes with several clients, each tailored for a specific data provider model and authentication scheme.
@@ -88,23 +141,30 @@
   - [x] http
   - [x] s3
     - [x] requestor pays
     - [ ] custom endpoint
   - [x] custom authentication
     - [x] Planetary Computer
     - [x] USGS EROS
-    - [ ] NASA
+    - [x]  NASA
 - [ ] Copy directly from source to destination ("skip local")
 - [ ] Add new assets to an item
 - [ ] Update an existing asset
 - [ ] Delete assets
 - [ ] Templated paths on download
 - [ ] (possible) Support the file extension's local path
 - [ ] Checksum validation and creation
-- [ ] CLI
+- [x] CLI
+
+## Versioning
+
+This project does its best to adhere to [semantic versioning](https://semver.org/).
+Any module, class, constant, or function that does not begin with a `_` is considered part of our public API for versioning purposes.
+Our command-line interface (CLI) is NOT considered part of our public API, and may change in breaking ways at any time.
+If you need stability promises, use our API.
 
 ## Contributing
 
 Use Github [issues](https://github.com/gadomski/stac-asset/issues) to report bugs and request new features.
 Use Github [pull requests](https://github.com/gadomski/stac-asset/pulls) to fix bugs and propose new features.
 
 ## Developing
```

### Comparing `stac-asset-0.0.3/src/stac_asset/__init__.py` & `stac-asset-0.0.4/src/stac_asset/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,48 +1,51 @@
-"""Get STAC Assets from various platforms and using different authentication schemes.
+"""Read and download STAC items, item collections, and assets.
 
-The core class is :py:class:`Client`, which defines a common interface.
-Other clients inherit from :py:class:`Client` to implement any custom behavior.
+The core class is :py:class:`Client`, which defines a common interface for
+accessing assets. There are also some free functions, :py:func:`download_item`
+and :py:func:`download_item_collection`, which provide simple one-shot
+interfaces for downloading assets.
+
+Writing items, item collections, and assets is currently unsupported, but is on
+the roadmap.
 """
 
 
 from .client import Client
 from .earthdata_client import EarthdataClient
 from .errors import (
-    AssetDownloadException,
-    AssetDownloadWarning,
-    AssetOverwriteException,
+    AssetDownloadError,
+    AssetOverwriteError,
+    CantIncludeAndExclude,
+    DownloadError,
+    DownloadWarning,
 )
 from .filesystem_client import FilesystemClient
 from .functions import (
-    download_href,
     download_item,
-    download_item_from_href,
+    download_item_collection,
     guess_client,
-    open_href,
-    read_file,
 )
 from .http_client import HttpClient
 from .planetary_computer_client import PlanetaryComputerClient
 from .s3_client import S3Client
 from .strategy import FileNameStrategy
 from .usgs_eros_client import UsgsErosClient
 
 __all__ = [
-    "AssetDownloadWarning",
-    "AssetDownloadException",
-    "AssetOverwriteException",
+    "DownloadWarning",
+    "AssetDownloadError",
+    "AssetOverwriteError",
+    "CantIncludeAndExclude",
     "Client",
+    "DownloadError",
     "EarthdataClient",
     "FileNameStrategy",
     "FilesystemClient",
     "HttpClient",
     "PlanetaryComputerClient",
     "S3Client",
     "UsgsErosClient",
-    "download_href",
     "download_item",
-    "download_item_from_href",
+    "download_item_collection",
     "guess_client",
-    "open_href",
-    "read_file",
 ]
```

### Comparing `stac-asset-0.0.3/src/stac_asset/earthdata_client.py` & `stac-asset-0.0.4/src/stac_asset/earthdata_client.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,20 +6,37 @@
 
 from aiohttp import ClientSession
 
 from .http_client import HttpClient
 
 
 class EarthdataClient(HttpClient):
+    """Access data from https://www.earthdata.nasa.gov/."""
+
     @classmethod
     async def default(cls) -> EarthdataClient:
+        """Logs in to Earthdata and returns the default earthdata client.
+
+        Uses a token stored in the ``EARTHDATA_PAT`` environment variable.
+        """
         return await cls.login()
 
     @classmethod
     async def login(cls, token: Optional[str] = None) -> EarthdataClient:
+        """Logs in to Earthdata and returns a client.
+
+        If token is not provided, it is read from the ``EARTHDATA_PAT``
+        environment variable.
+
+        Args:
+            token: The Earthdata bearer token
+
+        Returns:
+            EarthdataClient: A client configured to use the bearer token
+        """
         if token is None:
             try:
                 token = os.environ["EARTHDATA_PAT"]
             except KeyError:
                 raise ValueError(
                     "token was not provided, and EARTHDATA_PAT environment variable "
                     "not set"
```

### Comparing `stac-asset-0.0.3/src/stac_asset/filesystem_client.py` & `stac-asset-0.0.4/src/stac_asset/filesystem_client.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,14 +12,26 @@
 class FilesystemClient(Client):
     """A simple client for moving files around on the filesystem.
 
     Mostly used for testing, but could be useful in some real-world cases.
     """
 
     async def open_url(self, url: URL) -> AsyncIterator[bytes]:
+        """Iterates over data from a local url.
+
+        Args:
+            url: The url to read bytes from
+
+        Yields:
+            AsyncIterator[bytes]: An iterator over the file's bytes.
+
+        Raises:
+            ValueError: Raised if the url has a scheme. This behavior will
+                change if/when we support Windows paths.
+        """
         if url.scheme:
             raise ValueError(
                 "cannot read a file with the filesystem client if it has a url scheme: "
                 + str(url)
             )
         async with aiofiles.open(url.path, "rb") as f:
             async for chunk in f:
```

### Comparing `stac-asset-0.0.3/src/stac_asset/http_client.py` & `stac-asset-0.0.4/src/stac_asset/http_client.py`

 * *Files 21% similar despite different names*

```diff
@@ -28,14 +28,25 @@
         return cls(session)
 
     def __init__(self, session: ClientSession) -> None:
         super().__init__()
         self.session = session
 
     async def open_url(self, url: URL) -> AsyncIterator[bytes]:
+        """Opens a url with this client's session and iterates over its bytes.
+
+        Args:
+            url: The url to open
+
+        Yields:
+            AsyncIterator[bytes]: An iterator over the file's bytes
+
+        Raises:
+            :py:class:`aiohttp.ClientResponseError`: Raised if the response is not OK
+        """
         async with self.session.get(url) as response:
             response.raise_for_status()
             async for chunk, _ in response.content.iter_chunks():
                 yield chunk
 
     async def __aenter__(self) -> HttpClient:
         return self
```

### Comparing `stac-asset-0.0.3/src/stac_asset/types.py` & `stac-asset-0.0.4/src/stac_asset/types.py`

 * *Files identical despite different names*

### Comparing `stac-asset-0.0.3/src/stac_asset/usgs_eros_client.py` & `stac-asset-0.0.4/src/stac_asset/usgs_eros_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,34 +7,43 @@
 
 from aiohttp import ClientSession
 
 from .http_client import HttpClient
 
 
 class UsgsErosClient(HttpClient):
+    """A client for fetching data from USGS EROS.
+
+    This includes landsat data.
+    """
+
     @classmethod
     async def default(
         cls,
     ) -> UsgsErosClient:
-        """Logs in to the USGS EROS system using your environment variables."""
+        """Logs in to the USGS EROS system using your environment variables.
+
+        Returns:
+            UsgsErosClient: A client that has been logged in to the USGS EROS system
+        """
         return await cls.login()
 
     @classmethod
     async def login(
         cls,
         username: Optional[str] = None,
         pat: Optional[str] = None,
     ) -> UsgsErosClient:
-        """Retrieves a token from USGS EROS that will be used for all requests.
+        """Logs in to the USGS EROS system and returns a configured client.
 
         Args:
             username: Your USGS EROS username. Will be read from the
-                USGS_EROS_USERNAME environment variable if not provided.
+                ``USGS_EROS_USERNAME`` environment variable if not provided.
             pat: Your USGS EROS personal access token. Will be read from the
-                USGS_EROS_PAT environment variable if not provided.
+                ``USGS_EROS_PAT`` environment variable if not provided.
         """
         if username is None:
             try:
                 username = os.environ["USGS_EROS_USERNAME"]
             except KeyError:
                 raise ValueError(
                     "USGS_EROS_USERNAME is not set as an environment variable, "
```

### Comparing `stac-asset-0.0.3/src/stac_asset.egg-info/PKG-INFO` & `stac-asset-0.0.4/src/stac_asset.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 Metadata-Version: 2.1
 Name: stac-asset
-Version: 0.0.3
-Summary: Read, download, and write STAC assets across platforms and providers
+Version: 0.0.4
+Summary: Read and download STAC assets across platforms and providers
 Author-email: Pete Gadomski <pete.gadomski@gmail.com>
 License: Apache-2.0
 Project-URL: repository, https://github.com/gadomski/stac-asset
 Project-URL: changelog, https://github.com/gadomski/stac-asset/blob/main/CHANGELOG.md
 Keywords: stac,async
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: cli
 Provides-Extra: dev
 Provides-Extra: docs
 License-File: LICENSE
 
 # stac-asset
 
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/gadomski/stac-asset/ci.yaml?style=for-the-badge)](https://github.com/gadomski/stac-asset/actions/workflows/ci.yaml)
@@ -25,31 +31,61 @@
 
 ## Installation
 
 ```shell
 pip install stac-asset
 ```
 
+To use the command-line interface (CLI):
+
+```shell
+pip install 'stac-asset[cli]'
+```
+
 ## Usage
 
+### API
+
 Here's how to download a STAC [Item](https://github.com/radiantearth/stac-spec/blob/master/item-spec/item-spec.md) and all of its assets to a local directory using the top-level function.
 The correct [client](#clients) will be guessed from the assets' href.
 Each asset's href will be updated to point to the local file.
 
 ```python
 import stac_asset
 
 href = "https://raw.githubusercontent.com/radiantearth/stac-spec/master/examples/simple-item.json"
 await stac_asset.download_item_from_href(href, ".")
 ```
 
+### CLI
+
 To download an item using the command line:
 
-```python
-python -m stac_asset https://raw.githubusercontent.com/radiantearth/stac-spec/master/examples/simple-item.json .
+```shell
+stac-asset download https://raw.githubusercontent.com/radiantearth/stac-spec/master/examples/simple-item.json
+```
+
+To download all assets from the results of a [pystac-client](https://github.com/stac-utils/pystac-client) search, and save the item collection to a file named `item-collection.json`:
+
+```shell
+stac-client search https://planetarycomputer.microsoft.com/api/stac/v1 -c landsat-c2-l2 --max-items 1 | \
+    stac-asset download > item-collection.json
+```
+
+If you'd like to only download certain assets, e.g. a preview image, you can use the include `-i` flag:
+
+```shell
+stac-client search https://planetarycomputer.microsoft.com/api/stac/v1 -c landsat-c2-l2 --max-items 1 | \
+    stac-asset download -i rendered_preview -q
+```
+
+If you do a lot of downloads, you may want an alias:
+
+```shell
+alias stac-download="stac-asset download"
 ```
 
 See [the documentation](https://stac-asset.readthedocs.io/en/stable/index.html) for more examples and complete API documentation.
 
 ### Clients
 
 This library comes with several clients, each tailored for a specific data provider model and authentication scheme.
@@ -105,23 +141,30 @@
   - [x] http
   - [x] s3
     - [x] requestor pays
     - [ ] custom endpoint
   - [x] custom authentication
     - [x] Planetary Computer
     - [x] USGS EROS
-    - [ ] NASA
+    - [x]  NASA
 - [ ] Copy directly from source to destination ("skip local")
 - [ ] Add new assets to an item
 - [ ] Update an existing asset
 - [ ] Delete assets
 - [ ] Templated paths on download
 - [ ] (possible) Support the file extension's local path
 - [ ] Checksum validation and creation
-- [ ] CLI
+- [x] CLI
+
+## Versioning
+
+This project does its best to adhere to [semantic versioning](https://semver.org/).
+Any module, class, constant, or function that does not begin with a `_` is considered part of our public API for versioning purposes.
+Our command-line interface (CLI) is NOT considered part of our public API, and may change in breaking ways at any time.
+If you need stability promises, use our API.
 
 ## Contributing
 
 Use Github [issues](https://github.com/gadomski/stac-asset/issues) to report bugs and request new features.
 Use Github [pull requests](https://github.com/gadomski/stac-asset/pulls) to fix bugs and propose new features.
 
 ## Developing
```

### Comparing `stac-asset-0.0.3/src/stac_asset.egg-info/SOURCES.txt` & `stac-asset-0.0.4/src/stac_asset.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 LICENSE
 README.md
 pyproject.toml
 src/stac_asset/__init__.py
-src/stac_asset/__main__.py
+src/stac_asset/_cli.py
 src/stac_asset/client.py
 src/stac_asset/earthdata_client.py
 src/stac_asset/errors.py
 src/stac_asset/filesystem_client.py
 src/stac_asset/functions.py
 src/stac_asset/http_client.py
 src/stac_asset/planetary_computer_client.py
 src/stac_asset/s3_client.py
 src/stac_asset/strategy.py
 src/stac_asset/types.py
 src/stac_asset/usgs_eros_client.py
 src/stac_asset.egg-info/PKG-INFO
 src/stac_asset.egg-info/SOURCES.txt
 src/stac_asset.egg-info/dependency_links.txt
+src/stac_asset.egg-info/entry_points.txt
 src/stac_asset.egg-info/requires.txt
 src/stac_asset.egg-info/top_level.txt
-tests/test_download.py
+tests/test_cli.py
 tests/test_earthdata_client.py
 tests/test_filesystem_client.py
-tests/test_open.py
 tests/test_planetary_computer_client.py
 tests/test_s3_client.py
 tests/test_usgs_eros_client.py
```

### Comparing `stac-asset-0.0.3/tests/test_earthdata_client.py` & `stac-asset-0.0.4/tests/test_earthdata_client.py`

 * *Files identical despite different names*

### Comparing `stac-asset-0.0.3/tests/test_filesystem_client.py` & `stac-asset-0.0.4/tests/test_filesystem_client.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,48 +1,74 @@
 import os.path
 from pathlib import Path
 
 import pytest
-from pystac import Asset, Item
+from pystac import Asset, Item, ItemCollection
 from stac_asset import (
-    AssetDownloadWarning,
-    AssetOverwriteException,
+    AssetOverwriteError,
+    CantIncludeAndExclude,
+    DownloadError,
+    DownloadWarning,
     FileNameStrategy,
     FilesystemClient,
 )
 
 pytestmark = pytest.mark.asyncio
 
 
 @pytest.fixture
-def href() -> str:
+def asset_href() -> str:
     return str(Path(__file__).parent / "data" / "20201211_223832_CS2.jpg")
 
 
-async def test_download(tmp_path: Path, href: str) -> None:
+async def test_download(tmp_path: Path, asset_href: str) -> None:
     async with FilesystemClient() as client:
-        await client.download_href(href, tmp_path / "out.jpg")
-        assert os.path.getsize(tmp_path / "out.jpg") == 31367
+        await client.download_href(asset_href, tmp_path / "out.jpg")
 
+    assert os.path.getsize(tmp_path / "out.jpg") == 31367
 
-async def test_item_download(tmp_path: Path, item: Item) -> None:
+
+async def test_download_item(tmp_path: Path, item: Item) -> None:
     async with FilesystemClient() as client:
         item = await client.download_item(item, tmp_path)
-        assert Path(tmp_path / f"{item.id}.json").exists()
 
-        asset = item.assets["data"]
-        assert asset.href == "./20201211_223832_CS2.jpg"
+    assert Path(tmp_path / "item.json").exists()
+    asset = item.assets["data"]
+    assert asset.href == "./20201211_223832_CS2.jpg"
+
+
+async def test_download_item_collection(
+    tmp_path: Path, item_collection: ItemCollection
+) -> None:
+    async with FilesystemClient() as client:
+        await client.download_item_collection(item_collection, tmp_path)
+
+    assert os.path.exists(tmp_path / "item-collection.json")
+    assert os.path.exists(tmp_path / "test-item" / "20201211_223832_CS2.jpg")
 
 
 async def test_item_download_404(tmp_path: Path, item: Item) -> None:
     item.assets["missing-asset"] = Asset(href=str(Path(__file__).parent / "not-a-file"))
     async with FilesystemClient() as client:
-        with pytest.warns(AssetDownloadWarning):
+        with pytest.raises(DownloadError):
             await client.download_item(item, tmp_path)
+
+    assert not (tmp_path / "not-a-file").exists()
+
+
+async def test_item_download_404_warn(tmp_path: Path, item: Item) -> None:
+    item.assets["missing-asset"] = Asset(href=str(Path(__file__).parent / "not-a-file"))
+    async with FilesystemClient() as client:
+        with pytest.warns(DownloadWarning):
+            item = await client.download_item(
+                item, tmp_path, warn_on_download_error=True
+            )
+
     assert not (tmp_path / "not-a-file").exists()
+    assert "missing-asset" not in item.assets
 
 
 async def test_item_download_no_directory(tmp_path: Path, item: Item) -> None:
     async with FilesystemClient() as client:
         with pytest.raises(FileNotFoundError):
             await client.download_item(
                 item, tmp_path / "doesnt-exist", make_directory=False
@@ -50,15 +76,37 @@
 
 
 async def test_item_download_key(tmp_path: Path, item: Item) -> None:
     async with FilesystemClient() as client:
         await client.download_item(
             item, tmp_path, asset_file_name_strategy=FileNameStrategy.KEY
         )
-        assert Path(tmp_path / "data.jpg").exists()
+
+    assert Path(tmp_path / "data.jpg").exists()
 
 
 async def test_item_download_same_file_name(tmp_path: Path, item: Item) -> None:
     item.assets["other-data"] = item.assets["data"].clone()
     async with FilesystemClient() as client:
-        with pytest.raises(AssetOverwriteException):
+        with pytest.raises(AssetOverwriteError):
             await client.download_item(item, tmp_path)
+
+
+async def test_include(tmp_path: Path, item: Item) -> None:
+    item.assets["other-data"] = item.assets["data"].clone()
+    async with FilesystemClient() as client:
+        await client.download_item(item, tmp_path, include=["data"])
+
+
+async def test_exclude(tmp_path: Path, item: Item) -> None:
+    item.assets["other-data"] = item.assets["data"].clone()
+    async with FilesystemClient() as client:
+        await client.download_item(item, tmp_path, exclude=["other-data"])
+
+
+async def test_cant_include_and_exclude(tmp_path: Path, item: Item) -> None:
+    item.assets["other-data"] = item.assets["data"].clone()
+    async with FilesystemClient() as client:
+        with pytest.raises(CantIncludeAndExclude):
+            await client.download_item(
+                item, tmp_path, include=["data"], exclude=["other-data"]
+            )
```

### Comparing `stac-asset-0.0.3/tests/test_planetary_computer_client.py` & `stac-asset-0.0.4/tests/test_planetary_computer_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 pytestmark = [
     pytest.mark.network_access,
     pytest.mark.asyncio,
 ]
 
 
 @pytest.fixture
-def href() -> str:
+def asset_href() -> str:
     return "https://sentinel2l2a01.blob.core.windows.net/sentinel2-l2/48/X/VR/2023/05/24/S2B_MSIL2A_20230524T084609_N0509_R107_T48XVR_20230524T120352.SAFE/GRANULE/L2A_T48XVR_A032451_20230524T084603/QI_DATA/T48XVR_20230524T084609_PVI.tif"
 
 
-async def test_download(tmp_path: Path, href: str) -> None:
+async def test_download(tmp_path: Path, asset_href: str) -> None:
     async with await PlanetaryComputerClient.default() as client:
-        await client.download_href(href, tmp_path / "out.tif")
-        assert os.path.getsize(tmp_path / "out.tif") == 4096
+        await client.download_href(asset_href, tmp_path / "out.tif")
+
+    assert os.path.getsize(tmp_path / "out.tif") == 4096
```

### Comparing `stac-asset-0.0.3/tests/test_usgs_eros_client.py` & `stac-asset-0.0.4/tests/test_usgs_eros_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,18 +12,19 @@
     ),
     pytest.mark.network_access,
     pytest.mark.asyncio,
 ]
 
 
 @pytest.fixture
-def href() -> str:
+def asset_href() -> str:
     return (
         "https://landsatlook.usgs.gov/data/collection02/level-2/standard/oli-tirs/2022/004"
         "/004/LC08_L2SP_004004_20220519_20220525_02_T1/LC08_L2SP_004004_20220519_20220525_02_T1_thumb_small.jpeg"
     )
 
 
-async def test_download(tmp_path: Path, href: str) -> None:
+async def test_download(tmp_path: Path, asset_href: str) -> None:
     async with await UsgsErosClient.login() as client:
-        await client.download_href(href, tmp_path / "out.jpg")
-        assert os.path.getsize(tmp_path / "out.jpg") == 18517
+        await client.download_href(asset_href, tmp_path / "out.jpg")
+
+    assert os.path.getsize(tmp_path / "out.jpg") == 18517
```

