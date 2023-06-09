# Comparing `tmp/xpystac-0.0.1.tar.gz` & `tmp/xpystac-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xpystac-0.0.1.tar", last modified: Mon Mar 13 18:33:38 2023, max compression
+gzip compressed data, was "xpystac-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `xpystac-0.0.1.tar` & `xpystac-0.1.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     2039 2023-03-13 18:33:29.814729 xpystac-0.0.1/README.md
--rw-r--r--   0        0        0      622 2023-03-13 18:33:29.814729 xpystac-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       22 2023-03-13 18:33:29.818729 xpystac-0.0.1/xpystac/__init__.py
--rw-r--r--   0        0        0     2351 2023-03-13 18:33:29.818729 xpystac-0.0.1/xpystac/core.py
--rw-r--r--   0        0        0      235 2023-03-13 18:33:29.818729 xpystac-0.0.1/xpystac/utils.py
--rw-r--r--   0        0        0      654 2023-03-13 18:33:29.818729 xpystac-0.0.1/xpystac/xarray_plugin.py
--rw-r--r--   0        0        0     2475 1970-01-01 00:00:00.000000 xpystac-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     2041 2023-06-09 14:57:10.030114 xpystac-0.1.0/README.md
+-rw-r--r--   0        0        0      622 2023-06-09 14:57:10.030114 xpystac-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-06-09 14:57:10.030114 xpystac-0.1.0/xpystac/__init__.py
+-rw-r--r--   0        0        0     2355 2023-06-09 14:57:10.030114 xpystac-0.1.0/xpystac/core.py
+-rw-r--r--   0        0        0      235 2023-06-09 14:57:10.030114 xpystac-0.1.0/xpystac/utils.py
+-rw-r--r--   0        0        0      656 2023-06-09 14:57:10.030114 xpystac-0.1.0/xpystac/xarray_plugin.py
+-rw-r--r--   0        0        0     2477 1970-01-01 00:00:00.000000 xpystac-0.1.0/PKG-INFO
```

### Comparing `xpystac-0.0.1/README.md` & `xpystac-0.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 xr.open_dataset(asset)
 ```
 ref: https://planetarycomputer.microsoft.com/docs/quickstarts/reading-zarr-data/
 
 ## Install
 
 ```bash
-pip install git+https://github.com/jsignell/xpystac
+pip install git+https://github.com/stac-utils/xpystac
 ```
 
 ## How it works
 
 When you call ``xarray.open_dataset(object, engine="stac")`` this library maps that open call to the correct library.
 Depending on the ``type`` of ``object`` that might be [stackstac](https://github.com/gjoseph92/stackstac)
 or back to ``xarray.open_dataset`` itself but with the engine and other options pulled from the pystac object.
```

### Comparing `xpystac-0.0.1/pyproject.toml` & `xpystac-0.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xpystac-0.0.1/xpystac/core.py` & `xpystac-0.1.0/xpystac/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,9 +60,9 @@
         default_kwargs = {"engine": "rasterio"}
     elif obj.media_type == "application/vnd+zarr":
         _import_optional_dependency("zarr")
         default_kwargs = {"engine": "zarr"}
     else:
         default_kwargs = {}
 
-    ds = xarray.open_dataset(obj.href, **default_kwargs, **open_kwargs, **kwargs)
+    ds = xarray.open_dataset(obj.href, **{**default_kwargs, **open_kwargs, **kwargs})
     return ds
```

### Comparing `xpystac-0.0.1/xpystac/xarray_plugin.py` & `xpystac-0.1.0/xpystac/xarray_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,8 +19,8 @@
     open_dataset_parameters = ["obj", "drop_variables"]
 
     def guess_can_open(self, obj):
         return isinstance(obj, (pystac.Asset, pystac.Item, pystac.ItemCollection))
 
     description = "Open pystac objects in Xarray"
 
-    url = "https://github.com/jsignell/xpystac"
+    url = "https://github.com/stac-utils/xpystac"
```

### Comparing `xpystac-0.0.1/PKG-INFO` & `xpystac-0.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xpystac
-Version: 0.0.1
+Version: 0.1.0
 Summary: Extend xarray.open_dataset to accept pystac objects
 Author-email: Julia Signell <jsignell@element84.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: xarray
 Requires-Dist: pystac>=1.0.0b3
@@ -75,15 +75,15 @@
 xr.open_dataset(asset)
 ```
 ref: https://planetarycomputer.microsoft.com/docs/quickstarts/reading-zarr-data/
 
 ## Install
 
 ```bash
-pip install git+https://github.com/jsignell/xpystac
+pip install git+https://github.com/stac-utils/xpystac
 ```
 
 ## How it works
 
 When you call ``xarray.open_dataset(object, engine="stac")`` this library maps that open call to the correct library.
 Depending on the ``type`` of ``object`` that might be [stackstac](https://github.com/gjoseph92/stackstac)
 or back to ``xarray.open_dataset`` itself but with the engine and other options pulled from the pystac object.
```

