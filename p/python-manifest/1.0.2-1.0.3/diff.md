# Comparing `tmp/python_manifest-1.0.2-py3-none-any.whl.zip` & `tmp/python_manifest-1.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 18245 bytes, number of entries: 20
+Zip file size: 18224 bytes, number of entries: 20
 -rw-r--r--  2.0 unx      230 b- defN 80-Jan-01 00:00 manifest/__init__.py
 -rw-r--r--  2.0 unx     8972 b- defN 80-Jan-01 00:00 manifest/base.py
 -rw-r--r--  2.0 unx      324 b- defN 80-Jan-01 00:00 manifest/expressions/__init__.py
 -rw-r--r--  2.0 unx     3988 b- defN 80-Jan-01 00:00 manifest/expressions/operations.py
 -rw-r--r--  2.0 unx     3232 b- defN 80-Jan-01 00:00 manifest/expressions/resolve.py
 -rw-r--r--  2.0 unx     1169 b- defN 80-Jan-01 00:00 manifest/hooks.py
 -rw-r--r--  2.0 unx     2085 b- defN 80-Jan-01 00:00 manifest/instantiable.py
--rw-r--r--  2.0 unx     9658 b- defN 80-Jan-01 00:00 manifest/parse.py
+-rw-r--r--  2.0 unx     9565 b- defN 80-Jan-01 00:00 manifest/parse.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 manifest/py.typed
 -rw-r--r--  2.0 unx      386 b- defN 80-Jan-01 00:00 manifest/serializers/__init__.py
 -rw-r--r--  2.0 unx      272 b- defN 80-Jan-01 00:00 manifest/serializers/base.py
 -rw-r--r--  2.0 unx      503 b- defN 80-Jan-01 00:00 manifest/serializers/jsons.py
 -rw-r--r--  2.0 unx      353 b- defN 80-Jan-01 00:00 manifest/serializers/noop.py
 -rw-r--r--  2.0 unx      356 b- defN 80-Jan-01 00:00 manifest/serializers/tomls.py
 -rw-r--r--  2.0 unx      350 b- defN 80-Jan-01 00:00 manifest/serializers/yamls.py
 -rw-r--r--  2.0 unx     9635 b- defN 80-Jan-01 00:00 manifest/utils.py
--rw-r--r--  2.0 unx     1078 b- defN 80-Jan-01 00:00 python_manifest-1.0.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     5581 b- defN 80-Jan-01 00:00 python_manifest-1.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 python_manifest-1.0.2.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1627 b- defN 16-Jan-01 00:00 python_manifest-1.0.2.dist-info/RECORD
-20 files, 49887 bytes uncompressed, 15595 bytes compressed:  68.7%
+-rw-r--r--  2.0 unx     1078 b- defN 80-Jan-01 00:00 python_manifest-1.0.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5581 b- defN 80-Jan-01 00:00 python_manifest-1.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 python_manifest-1.0.3.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1627 b- defN 16-Jan-01 00:00 python_manifest-1.0.3.dist-info/RECORD
+20 files, 49794 bytes uncompressed, 15574 bytes compressed:  68.7%
```

## zipnote {}

```diff
@@ -42,20 +42,20 @@
 
 Filename: manifest/serializers/yamls.py
 Comment: 
 
 Filename: manifest/utils.py
 Comment: 
 
-Filename: python_manifest-1.0.2.dist-info/LICENSE
+Filename: python_manifest-1.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: python_manifest-1.0.2.dist-info/METADATA
+Filename: python_manifest-1.0.3.dist-info/METADATA
 Comment: 
 
-Filename: python_manifest-1.0.2.dist-info/WHEEL
+Filename: python_manifest-1.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: python_manifest-1.0.2.dist-info/RECORD
+Filename: python_manifest-1.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## manifest/parse.py

```diff
@@ -129,14 +129,16 @@
     :param pre_process_hooks: A list of hooks to be called before serializing the data.
     :type pre_process_hooks: list[Callable]
     :param post_process_hooks: A list of hooks to be called after serializing the data.
     :type post_process_hooks: list[Callable]
     :return: The number of bytes written to the file.
     :rtype: int
     """
+    assert isinstance(data, dict), "`data` must be a dictionary"
+
     # Get the serializer for the file type
     serializer = get_serializer_from_type(
         _type=determine_file_type(
             get_filename_suffix(file)
         ),
         _default=default_serializer
     )
@@ -188,25 +190,22 @@
     # Pre-process the file contents
     for pre_hook in pre_process_hooks:
         raw_data = await execute_hook(pre_hook, raw_data)
 
     # Deserialize the file contents
     data: dict = serializer.loads(raw_data)
 
-    # Make sure the deserialized contents are a dictionary
-    assert isinstance(data, dict), f"Deserialized contents must be a dictionary, not {type(data)}"
+    # Handle empty files
+    if not data:
+        data = {}
 
     # Post-process the file contents
     for post_hook in post_process_hooks:
         data = await execute_hook(post_hook, data)
 
-    # Handle empty files
-    if not data:
-        data = {}
-
     return data
 
 
 async def parse_files(
     files: list[str],
     pre_process_hooks: list[Callable] = [],
     post_process_hooks: list[Callable] = [],
```

## Comparing `python_manifest-1.0.2.dist-info/LICENSE` & `python_manifest-1.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `python_manifest-1.0.2.dist-info/METADATA` & `python_manifest-1.0.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-manifest
-Version: 1.0.2
+Version: 1.0.3
 Summary: A modern toolkit for working with application manifests and configurations.
 Home-page: https://github.com/emergentmethods/python-manifest
 License: MIT
 Author: Timothy Pogue
 Author-email: tim@emergentmethods.ai
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `python_manifest-1.0.2.dist-info/RECORD` & `python_manifest-1.0.3.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 manifest/__init__.py,sha256=lPR8D6XQ8nBPlRQEKelo78kQ0gMKANeprcMEZKRevwo,230
 manifest/base.py,sha256=muQpNSF8bVrKPnRKhfs3xfyHYswfqZMgwMZJjDGtOYk,8972
 manifest/expressions/__init__.py,sha256=YVRb_gL_yIzfJZhXQejRrAErcA77rNBXKzvQKsLtjSs,324
 manifest/expressions/operations.py,sha256=Djrk1Psr5EswbYcXMlmn0BpNOnc6YcVhI8wXQakaqxQ,3988
 manifest/expressions/resolve.py,sha256=9TW7ArbnSRL0VsWfe4QYIAYsZmiWBqIGWx5yrQp_fjA,3232
 manifest/hooks.py,sha256=xXvivqUIfS56tNvW340YESbzD6Tmhju0x2N4A76JMnQ,1169
 manifest/instantiable.py,sha256=TlzW04amYQF26X_iqJU2MMsvplCMogUM6XTwljdwFcc,2085
-manifest/parse.py,sha256=xTsm2DRWfzX0fBp2sNWD14TF5mqLdFe-PvbER9YMezo,9658
+manifest/parse.py,sha256=nsK93CLMkC62ru9G-KmFjDNAsBzawjkxbkIvL2adxIc,9565
 manifest/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 manifest/serializers/__init__.py,sha256=4d2mNeR4nZTdHC7Dg5ab7_whcXF_BsXvrhm8whJMeas,386
 manifest/serializers/base.py,sha256=So6sMP502D0fXN84Np0a_c5IGyq4gLWmMXfDwN6xAPg,272
 manifest/serializers/jsons.py,sha256=iK5Tswidrc3CLqeg4YaBNH7Ev6C7cVAQo6pEmDjncIM,503
 manifest/serializers/noop.py,sha256=x0sqDyLDFI-g6K5EnXUex3UVmwLvq-nMFoBj_iNpTys,353
 manifest/serializers/tomls.py,sha256=QxSGa4nWs3SqJAF-Y_64zGfEn_BgPOVs5-bxvS7X6Ro,356
 manifest/serializers/yamls.py,sha256=th77AOLV4I10t_SOLIlqQAsiSGzACzia71vGIi-1Cf0,350
 manifest/utils.py,sha256=T96gPjGVC-IwfblXB24fKVRxHt66txpZYE3Umk4EQdk,9635
-python_manifest-1.0.2.dist-info/LICENSE,sha256=DEqEB7tSTdQp6PHFAw4I1MyZU02bPaXoSULcNI_49bw,1078
-python_manifest-1.0.2.dist-info/METADATA,sha256=Od1tmUGvs0LpNJU7xB5SzjAAIain2CZtOiUI5qhqSlI,5581
-python_manifest-1.0.2.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
-python_manifest-1.0.2.dist-info/RECORD,,
+python_manifest-1.0.3.dist-info/LICENSE,sha256=DEqEB7tSTdQp6PHFAw4I1MyZU02bPaXoSULcNI_49bw,1078
+python_manifest-1.0.3.dist-info/METADATA,sha256=s7FtvoxLqG5RXR0PPC3vdVuBf3wYh1w79H-4xu0cgWY,5581
+python_manifest-1.0.3.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+python_manifest-1.0.3.dist-info/RECORD,,
```

