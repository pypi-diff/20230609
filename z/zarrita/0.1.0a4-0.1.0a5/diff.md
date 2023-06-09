# Comparing `tmp/zarrita-0.1.0a4.tar.gz` & `tmp/zarrita-0.1.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zarrita-0.1.0a4.tar", max compression
+gzip compressed data, was "zarrita-0.1.0a5.tar", max compression
```

## Comparing `zarrita-0.1.0a4.tar` & `zarrita-0.1.0a5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1105 2023-05-09 09:12:03.956626 zarrita-0.1.0a4/LICENSE
--rw-r--r--   0        0        0     2311 2023-06-08 08:19:54.182773 zarrita-0.1.0a4/README.md
--rw-r--r--   0        0        0      696 2023-06-08 12:11:30.092430 zarrita-0.1.0a4/pyproject.toml
--rw-r--r--   0        0        0     1085 2023-06-07 11:49:09.452172 zarrita-0.1.0a4/zarrita/__init__.py
--rw-r--r--   0        0        0    19595 2023-06-08 12:06:03.005900 zarrita-0.1.0a4/zarrita/array.py
--rw-r--r--   0        0        0    13242 2023-06-08 12:06:11.862323 zarrita-0.1.0a4/zarrita/array_v2.py
--rw-r--r--   0        0        0    12285 2023-06-08 07:24:44.647554 zarrita-0.1.0a4/zarrita/codecs.py
--rw-r--r--   0        0        0     4314 2023-06-07 20:03:42.377098 zarrita-0.1.0a4/zarrita/common.py
--rw-r--r--   0        0        0     4181 2023-06-07 15:17:15.193840 zarrita-0.1.0a4/zarrita/group.py
--rw-r--r--   0        0        0     4735 2023-06-07 15:17:10.125767 zarrita-0.1.0a4/zarrita/group_v2.py
--rw-r--r--   0        0        0     7259 2023-06-07 12:49:15.942016 zarrita-0.1.0a4/zarrita/indexing.py
--rw-r--r--   0        0        0     5374 2023-06-08 07:17:39.694424 zarrita-0.1.0a4/zarrita/metadata.py
--rw-r--r--   0        0        0    20531 2023-06-08 12:06:20.763281 zarrita-0.1.0a4/zarrita/sharding.py
--rw-r--r--   0        0        0     5391 2023-06-07 20:04:34.652580 zarrita-0.1.0a4/zarrita/store.py
--rw-r--r--   0        0        0     2555 2023-06-02 09:33:41.528984 zarrita-0.1.0a4/zarrita/sync.py
--rw-r--r--   0        0        0     3827 2023-06-06 13:35:33.794530 zarrita-0.1.0a4/zarrita/value_handle.py
--rw-r--r--   0        0        0     3012 1970-01-01 00:00:00.000000 zarrita-0.1.0a4/PKG-INFO
+-rw-r--r--   0        0        0     1105 2023-05-09 09:12:03.956626 zarrita-0.1.0a5/LICENSE
+-rw-r--r--   0        0        0     2311 2023-06-08 08:19:54.182773 zarrita-0.1.0a5/README.md
+-rw-r--r--   0        0        0      696 2023-06-09 12:23:32.908465 zarrita-0.1.0a5/pyproject.toml
+-rw-r--r--   0        0        0     1085 2023-06-07 11:49:09.452172 zarrita-0.1.0a5/zarrita/__init__.py
+-rw-r--r--   0        0        0    19605 2023-06-09 11:30:35.987863 zarrita-0.1.0a5/zarrita/array.py
+-rw-r--r--   0        0        0    13242 2023-06-08 12:06:11.862323 zarrita-0.1.0a5/zarrita/array_v2.py
+-rw-r--r--   0        0        0    12363 2023-06-09 11:37:23.257106 zarrita-0.1.0a5/zarrita/codecs.py
+-rw-r--r--   0        0        0     4314 2023-06-07 20:03:42.377098 zarrita-0.1.0a5/zarrita/common.py
+-rw-r--r--   0        0        0     4181 2023-06-07 15:17:15.193840 zarrita-0.1.0a5/zarrita/group.py
+-rw-r--r--   0        0        0     4735 2023-06-07 15:17:10.125767 zarrita-0.1.0a5/zarrita/group_v2.py
+-rw-r--r--   0        0        0     7259 2023-06-07 12:49:15.942016 zarrita-0.1.0a5/zarrita/indexing.py
+-rw-r--r--   0        0        0     5374 2023-06-08 07:17:39.694424 zarrita-0.1.0a5/zarrita/metadata.py
+-rw-r--r--   0        0        0    20531 2023-06-08 12:06:20.763281 zarrita-0.1.0a5/zarrita/sharding.py
+-rw-r--r--   0        0        0     5391 2023-06-07 20:04:34.652580 zarrita-0.1.0a5/zarrita/store.py
+-rw-r--r--   0        0        0     2555 2023-06-02 09:33:41.528984 zarrita-0.1.0a5/zarrita/sync.py
+-rw-r--r--   0        0        0     3827 2023-06-06 13:35:33.794530 zarrita-0.1.0a5/zarrita/value_handle.py
+-rw-r--r--   0        0        0     3012 1970-01-01 00:00:00.000000 zarrita-0.1.0a5/PKG-INFO
```

### Comparing `zarrita-0.1.0a4/LICENSE` & `zarrita-0.1.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `zarrita-0.1.0a4/README.md` & `zarrita-0.1.0a5/README.md`

 * *Files identical despite different names*

### Comparing `zarrita-0.1.0a4/pyproject.toml` & `zarrita-0.1.0a5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zarrita"
-version = "0.1.0a4"
+version = "0.1.0a5"
 description = ""
 authors = ["Norman Rzepka <code@normanrz.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.11"
```

### Comparing `zarrita-0.1.0a4/zarrita/__init__.py` & `zarrita-0.1.0a5/zarrita/__init__.py`

 * *Files identical despite different names*

### Comparing `zarrita-0.1.0a4/zarrita/array.py` & `zarrita-0.1.0a5/zarrita/array.py`

 * *Files 1% similar despite different names*

```diff
@@ -436,15 +436,15 @@
         if np.isscalar(value):
             # setting a scalar value
             pass
         else:
             if not hasattr(value, "shape"):
                 value = np.asarray(value, self.metadata.dtype)
             assert value.shape == sel_shape
-            if value.dtype != self.metadata.dtype:
+            if value.dtype.name != self.metadata.dtype.name:
                 value = value.astype(self.metadata.dtype, order="A")
 
         # merging with existing data and encoding chunks
         await concurrent_map(
             [
                 (
                     value,
```

### Comparing `zarrita-0.1.0a4/zarrita/array_v2.py` & `zarrita-0.1.0a5/zarrita/array_v2.py`

 * *Files identical despite different names*

### Comparing `zarrita-0.1.0a4/zarrita/codecs.py` & `zarrita-0.1.0a5/zarrita/codecs.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,16 @@
     f: Callable[
         [np.ndarray, "CoreArrayMetadata"], Awaitable[Union[None, np.ndarray, BytesLike]]
     ],
 ):
     chunk_array = await chunk_value_handle.toarray()
     if chunk_array is None:
         return NoneValueHandle()
-    chunk_array = chunk_array.view(dtype=array_metadata.dtype)
+    if chunk_array.dtype.name != array_metadata.dtype.name:
+        chunk_array = chunk_array.view(dtype=array_metadata.dtype)
     result = await f(chunk_array, array_metadata)
     if result is None:
         return NoneValueHandle()
     elif (
         isinstance(result, bytes)
         or isinstance(result, bytearray)
         or isinstance(result, memoryview)
@@ -295,17 +296,16 @@
     async def inner_encode(
         self,
         chunk_array: np.ndarray,
         _array_metadata: "CoreArrayMetadata",
     ) -> BytesLike:
         byteorder = self._get_byteorder(chunk_array)
         if self.configuration.endian != byteorder:
-            chunk_array = chunk_array.astype(
-                dtype=chunk_array.dtype.newbyteorder(byteorder)
-            )
+            new_dtype = chunk_array.dtype.newbyteorder(self.configuration.endian)
+            chunk_array = chunk_array.astype(new_dtype)
         return chunk_array.tobytes()
 
 
 @frozen
 class TransposeCodec(ArrayArrayCodec):
     configuration: TransposeCodecConfigurationMetadata
```

### Comparing `zarrita-0.1.0a4/zarrita/common.py` & `zarrita-0.1.0a5/zarrita/common.py`

 * *Files identical despite different names*

### Comparing `zarrita-0.1.0a4/zarrita/group.py` & `zarrita-0.1.0a5/zarrita/group.py`

 * *Files identical despite different names*

### Comparing `zarrita-0.1.0a4/zarrita/group_v2.py` & `zarrita-0.1.0a5/zarrita/group_v2.py`

 * *Files identical despite different names*

### Comparing `zarrita-0.1.0a4/zarrita/indexing.py` & `zarrita-0.1.0a5/zarrita/indexing.py`

 * *Files identical despite different names*

### Comparing `zarrita-0.1.0a4/zarrita/metadata.py` & `zarrita-0.1.0a5/zarrita/metadata.py`

 * *Files identical despite different names*

### Comparing `zarrita-0.1.0a4/zarrita/sharding.py` & `zarrita-0.1.0a5/zarrita/sharding.py`

 * *Files identical despite different names*

### Comparing `zarrita-0.1.0a4/zarrita/store.py` & `zarrita-0.1.0a5/zarrita/store.py`

 * *Files identical despite different names*

### Comparing `zarrita-0.1.0a4/zarrita/sync.py` & `zarrita-0.1.0a5/zarrita/sync.py`

 * *Files identical despite different names*

### Comparing `zarrita-0.1.0a4/zarrita/value_handle.py` & `zarrita-0.1.0a5/zarrita/value_handle.py`

 * *Files identical despite different names*

### Comparing `zarrita-0.1.0a4/PKG-INFO` & `zarrita-0.1.0a5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zarrita
-Version: 0.1.0a4
+Version: 0.1.0a5
 Summary: 
 License: MIT
 Author: Norman Rzepka
 Author-email: code@normanrz.com
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

