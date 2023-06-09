# Comparing `tmp/s3fs-2023.5.0.tar.gz` & `tmp/s3fs-2023.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s3fs-2023.5.0.tar", last modified: Sun May  7 19:14:19 2023, max compression
+gzip compressed data, was "s3fs-2023.6.0.tar", last modified: Fri Jun  9 17:44:35 2023, max compression
```

## Comparing `s3fs-2023.5.0.tar` & `s3fs-2023.6.0.tar`

### file list

```diff
@@ -1,35 +1,39 @@
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-07 19:14:19.290045 s3fs-2023.5.0/
--rw-r--r--   0 mdurant    (502) staff       (20)     1505 2022-09-18 01:28:11.000000 s3fs-2023.5.0/LICENSE.txt
--rw-r--r--   0 mdurant    (502) staff       (20)      225 2022-09-18 01:28:11.000000 s3fs-2023.5.0/MANIFEST.in
--rw-r--r--   0 mdurant    (502) staff       (20)     1341 2023-05-07 19:14:19.290121 s3fs-2023.5.0/PKG-INFO
--rw-r--r--   0 mdurant    (502) staff       (20)      620 2022-09-18 01:28:11.000000 s3fs-2023.5.0/README.rst
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-07 19:14:19.282518 s3fs-2023.5.0/docs/
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-07 19:14:19.285810 s3fs-2023.5.0/docs/source/
--rw-r--r--   0 mdurant    (502) staff       (20)      906 2023-02-23 19:42:13.000000 s3fs-2023.5.0/docs/source/api.rst
--rw-r--r--   0 mdurant    (502) staff       (20)     4290 2023-05-07 19:13:40.000000 s3fs-2023.5.0/docs/source/changelog.rst
--rw-r--r--   0 mdurant    (502) staff       (20)      151 2022-09-18 01:28:11.000000 s3fs-2023.5.0/docs/source/development.rst
--rw-r--r--   0 mdurant    (502) staff       (20)    11489 2023-04-25 15:48:31.000000 s3fs-2023.5.0/docs/source/index.rst
--rw-r--r--   0 mdurant    (502) staff       (20)      530 2022-09-18 01:28:11.000000 s3fs-2023.5.0/docs/source/install.rst
--rw-r--r--   0 mdurant    (502) staff       (20)       64 2023-05-07 19:13:40.000000 s3fs-2023.5.0/requirements.txt
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-07 19:14:19.290876 s3fs-2023.5.0/s3fs/
--rw-r--r--   0 mdurant    (502) staff       (20)      160 2022-09-18 01:28:11.000000 s3fs-2023.5.0/s3fs/__init__.py
--rw-r--r--   0 mdurant    (502) staff       (20)      500 2023-05-07 19:14:19.290935 s3fs-2023.5.0/s3fs/_version.py
--rw-r--r--   0 mdurant    (502) staff       (20)    82930 2023-05-05 14:01:13.000000 s3fs-2023.5.0/s3fs/core.py
--rw-r--r--   0 mdurant    (502) staff       (20)     7779 2022-09-18 01:28:11.000000 s3fs-2023.5.0/s3fs/errors.py
--rw-r--r--   0 mdurant    (502) staff       (20)      237 2022-09-18 01:28:11.000000 s3fs-2023.5.0/s3fs/mapping.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-07 19:14:19.289887 s3fs-2023.5.0/s3fs/tests/
--rw-r--r--   0 mdurant    (502) staff       (20)        0 2022-09-18 01:28:11.000000 s3fs-2023.5.0/s3fs/tests/__init__.py
--rw-r--r--   0 mdurant    (502) staff       (20)     2859 2022-09-18 01:28:11.000000 s3fs-2023.5.0/s3fs/tests/test_mapping.py
--rw-r--r--   0 mdurant    (502) staff       (20)    79706 2023-05-05 14:56:21.000000 s3fs-2023.5.0/s3fs/tests/test_s3fs.py
--rw-r--r--   0 mdurant    (502) staff       (20)      370 2022-09-18 01:28:11.000000 s3fs-2023.5.0/s3fs/tests/test_utils.py
--rw-r--r--   0 mdurant    (502) staff       (20)     5246 2023-01-02 15:39:19.000000 s3fs-2023.5.0/s3fs/utils.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-07 19:14:19.288810 s3fs-2023.5.0/s3fs.egg-info/
--rw-r--r--   0 mdurant    (502) staff       (20)     1341 2023-05-07 19:14:19.000000 s3fs-2023.5.0/s3fs.egg-info/PKG-INFO
--rw-r--r--   0 mdurant    (502) staff       (20)      561 2023-05-07 19:14:19.000000 s3fs-2023.5.0/s3fs.egg-info/SOURCES.txt
--rw-r--r--   0 mdurant    (502) staff       (20)        1 2023-05-07 19:14:19.000000 s3fs-2023.5.0/s3fs.egg-info/dependency_links.txt
--rw-r--r--   0 mdurant    (502) staff       (20)        1 2022-10-19 15:15:30.000000 s3fs-2023.5.0/s3fs.egg-info/not-zip-safe
--rw-r--r--   0 mdurant    (502) staff       (20)      135 2023-05-07 19:14:19.000000 s3fs-2023.5.0/s3fs.egg-info/requires.txt
--rw-r--r--   0 mdurant    (502) staff       (20)        5 2023-05-07 19:14:19.000000 s3fs-2023.5.0/s3fs.egg-info/top_level.txt
--rw-r--r--   0 mdurant    (502) staff       (20)      438 2023-05-07 19:14:19.290481 s3fs-2023.5.0/setup.cfg
--rwxr-xr-x   0 mdurant    (502) staff       (20)     1365 2023-02-23 19:42:13.000000 s3fs-2023.5.0/setup.py
--rw-r--r--   0 mdurant    (502) staff       (20)    78281 2022-09-18 01:28:11.000000 s3fs-2023.5.0/versioneer.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-06-09 17:44:35.783417 s3fs-2023.6.0/
+-rw-r--r--   0 mdurant    (502) staff       (20)     1505 2022-09-18 01:28:11.000000 s3fs-2023.6.0/LICENSE.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)      225 2022-09-18 01:28:11.000000 s3fs-2023.6.0/MANIFEST.in
+-rw-r--r--   0 mdurant    (502) staff       (20)     1341 2023-06-09 17:44:35.783497 s3fs-2023.6.0/PKG-INFO
+-rw-r--r--   0 mdurant    (502) staff       (20)      620 2022-09-18 01:28:11.000000 s3fs-2023.6.0/README.rst
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-06-09 17:44:35.776402 s3fs-2023.6.0/docs/
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-06-09 17:44:35.779387 s3fs-2023.6.0/docs/source/
+-rw-r--r--   0 mdurant    (502) staff       (20)      906 2023-02-23 19:42:13.000000 s3fs-2023.6.0/docs/source/api.rst
+-rw-r--r--   0 mdurant    (502) staff       (20)     4408 2023-06-09 17:43:54.000000 s3fs-2023.6.0/docs/source/changelog.rst
+-rw-r--r--   0 mdurant    (502) staff       (20)      151 2022-09-18 01:28:11.000000 s3fs-2023.6.0/docs/source/development.rst
+-rw-r--r--   0 mdurant    (502) staff       (20)    11489 2023-04-25 15:48:31.000000 s3fs-2023.6.0/docs/source/index.rst
+-rw-r--r--   0 mdurant    (502) staff       (20)      530 2022-09-18 01:28:11.000000 s3fs-2023.6.0/docs/source/install.rst
+-rw-r--r--   0 mdurant    (502) staff       (20)       64 2023-06-09 17:43:54.000000 s3fs-2023.6.0/requirements.txt
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-06-09 17:44:35.784392 s3fs-2023.6.0/s3fs/
+-rw-r--r--   0 mdurant    (502) staff       (20)      160 2022-09-18 01:28:11.000000 s3fs-2023.6.0/s3fs/__init__.py
+-rw-r--r--   0 mdurant    (502) staff       (20)      500 2023-06-09 17:44:35.784450 s3fs-2023.6.0/s3fs/_version.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    83809 2023-06-09 17:43:54.000000 s3fs-2023.6.0/s3fs/core.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     7779 2022-09-18 01:28:11.000000 s3fs-2023.6.0/s3fs/errors.py
+-rw-r--r--   0 mdurant    (502) staff       (20)      237 2022-09-18 01:28:11.000000 s3fs-2023.6.0/s3fs/mapping.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-06-09 17:44:35.782571 s3fs-2023.6.0/s3fs/tests/
+-rw-r--r--   0 mdurant    (502) staff       (20)        0 2022-09-18 01:28:11.000000 s3fs-2023.6.0/s3fs/tests/__init__.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-06-09 17:44:35.783132 s3fs-2023.6.0/s3fs/tests/derived/
+-rw-r--r--   0 mdurant    (502) staff       (20)        0 2023-06-05 15:35:23.000000 s3fs-2023.6.0/s3fs/tests/derived/__init__.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     3583 2023-06-05 15:35:23.000000 s3fs-2023.6.0/s3fs/tests/derived/s3fs_fixtures.py
+-rw-r--r--   0 mdurant    (502) staff       (20)      314 2023-06-05 15:35:23.000000 s3fs-2023.6.0/s3fs/tests/derived/s3fs_test.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     2859 2022-09-18 01:28:11.000000 s3fs-2023.6.0/s3fs/tests/test_mapping.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    80275 2023-06-09 17:43:54.000000 s3fs-2023.6.0/s3fs/tests/test_s3fs.py
+-rw-r--r--   0 mdurant    (502) staff       (20)      370 2022-09-18 01:28:11.000000 s3fs-2023.6.0/s3fs/tests/test_utils.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     5246 2023-01-02 15:39:19.000000 s3fs-2023.6.0/s3fs/utils.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-06-09 17:44:35.781887 s3fs-2023.6.0/s3fs.egg-info/
+-rw-r--r--   0 mdurant    (502) staff       (20)     1341 2023-06-09 17:44:35.000000 s3fs-2023.6.0/s3fs.egg-info/PKG-INFO
+-rw-r--r--   0 mdurant    (502) staff       (20)      660 2023-06-09 17:44:35.000000 s3fs-2023.6.0/s3fs.egg-info/SOURCES.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)        1 2023-06-09 17:44:35.000000 s3fs-2023.6.0/s3fs.egg-info/dependency_links.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)        1 2022-10-19 15:15:30.000000 s3fs-2023.6.0/s3fs.egg-info/not-zip-safe
+-rw-r--r--   0 mdurant    (502) staff       (20)      135 2023-06-09 17:44:35.000000 s3fs-2023.6.0/s3fs.egg-info/requires.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)        5 2023-06-09 17:44:35.000000 s3fs-2023.6.0/s3fs.egg-info/top_level.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)      438 2023-06-09 17:44:35.783911 s3fs-2023.6.0/setup.cfg
+-rwxr-xr-x   0 mdurant    (502) staff       (20)     1365 2023-02-23 19:42:13.000000 s3fs-2023.6.0/setup.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    78281 2022-09-18 01:28:11.000000 s3fs-2023.6.0/versioneer.py
```

### Comparing `s3fs-2023.5.0/LICENSE.txt` & `s3fs-2023.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `s3fs-2023.5.0/PKG-INFO` & `s3fs-2023.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s3fs
-Version: 2023.5.0
+Version: 2023.6.0
 Summary: Convenient Filesystem interface over S3
 Home-page: http://github.com/fsspec/s3fs/
 Maintainer: Martin Durant
 Maintainer-email: mdurant@continuum.io
 License: BSD
 Keywords: s3,boto
 Classifier: Development Status :: 4 - Beta
```

### Comparing `s3fs-2023.5.0/README.rst` & `s3fs-2023.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `s3fs-2023.5.0/docs/source/api.rst` & `s3fs-2023.6.0/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `s3fs-2023.5.0/docs/source/changelog.rst` & `s3fs-2023.6.0/docs/source/changelog.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 Changelog
 =========
 
+2023.6.0
+--------
+
+- allow versions in info.exists (#746)
+- streaming file to update it's size for tell (#745, 741)
+
+
 2023.5.0
 --------
 
 - Fix "_" in xattrs tests (#732)
 - Fix file pointer already at end of file when retrying put (#731)
 - Fix repeated find corrupting cache (#730)
 - Remove duplicate class definition (#727)
```

### Comparing `s3fs-2023.5.0/docs/source/index.rst` & `s3fs-2023.6.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `s3fs-2023.5.0/docs/source/install.rst` & `s3fs-2023.6.0/docs/source/install.rst`

 * *Files identical despite different names*

### Comparing `s3fs-2023.5.0/s3fs/core.py` & `s3fs-2023.6.0/s3fs/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -963,26 +963,47 @@
                     for o in files
                     if o["name"].rstrip("/") == path and o["type"] != "directory"
                 ]
             if detail:
                 return files
         return files if detail else sorted([o["name"] for o in files])
 
+    def _exists_in_cache(self, path, bucket, key, version_id):
+        fullpath = "/".join((bucket, key))
+
+        try:
+            entries = self._ls_from_cache(fullpath)
+        except FileNotFoundError:
+            return False
+
+        if entries is None:
+            return None
+
+        if not self.version_aware or version_id is None:
+            return True
+
+        for entry in entries:
+            if entry["name"] == fullpath and entry.get("VersionId") == version_id:
+                return True
+
+        # dircache doesn't support multiple versions, so we really can't tell if
+        # the one we want exists.
+        return None
+
     async def _exists(self, path):
         if path in ["", "/"]:
             # the root always exists, even if anon
             return True
         path = self._strip_protocol(path)
         bucket, key, version_id = self.split_path(path)
         if key:
-            try:
-                if self._ls_from_cache(path):
-                    return True
-            except FileNotFoundError:
-                return False
+            exists_in_cache = self._exists_in_cache(path, bucket, key, version_id)
+            if exists_in_cache is not None:
+                return exists_in_cache
+
             try:
                 await self._info(path, bucket, key, version_id=version_id)
                 return True
             except FileNotFoundError:
                 return False
         elif self.dircache.get(bucket, False):
             return True
@@ -1212,33 +1233,35 @@
                 body.close()
             except Exception:
                 pass
 
     async def _info(self, path, bucket=None, key=None, refresh=False, version_id=None):
         path = self._strip_protocol(path)
         bucket, key, path_version_id = self.split_path(path)
+        fullpath = "/".join((bucket, key))
+
         if version_id is not None:
             if not self.version_aware:
                 raise ValueError(
                     "version_id cannot be specified if the "
                     "filesystem is not version aware"
                 )
         if path in ["/", ""]:
             return {"name": path, "size": 0, "type": "directory"}
         version_id = _coalesce_version_id(path_version_id, version_id)
         if not refresh:
-            out = self._ls_from_cache(path)
+            out = self._ls_from_cache(fullpath)
             if out is not None:
                 if self.version_aware and version_id is not None:
                     # If cached info does not match requested version_id,
                     # fallback to calling head_object
                     out = [
                         o
                         for o in out
-                        if o["name"] == path and version_id == o.get("VersionId")
+                        if o["name"] == fullpath and version_id == o.get("VersionId")
                     ]
                     if out:
                         return out[0]
                 else:
                     out = [o for o in out if o["name"] == path]
                     if out:
                         return out[0]
@@ -2291,21 +2314,26 @@
 
 class S3AsyncStreamedFile(AbstractAsyncStreamedFile):
     def __init__(self, fs, path, mode):
         self.fs = fs
         self.path = path
         self.mode = mode
         self.r = None
+        self.loc = 0
+        self.size = None
 
     async def read(self, length=-1):
         if self.r is None:
             bucket, key, gen = self.fs.split_path(self.path)
             r = await self.fs._call_s3("get_object", Bucket=bucket, Key=key)
+            self.size = int(r["ResponseMetadata"]["HTTPHeaders"]["content-length"])
             self.r = r["Body"]
-        return await self.r.read(length)
+        out = await self.r.read(length)
+        self.loc += len(out)
+        return out
 
 
 def _fetch_range(fs, bucket, key, version_id, start, end, req_kw=None):
     if req_kw is None:
         req_kw = {}
     if start == end:
         logger.debug(
```

### Comparing `s3fs-2023.5.0/s3fs/errors.py` & `s3fs-2023.6.0/s3fs/errors.py`

 * *Files identical despite different names*

### Comparing `s3fs-2023.5.0/s3fs/tests/test_mapping.py` & `s3fs-2023.6.0/s3fs/tests/test_mapping.py`

 * *Files identical despite different names*

### Comparing `s3fs-2023.5.0/s3fs/tests/test_s3fs.py` & `s3fs-2023.6.0/s3fs/tests/test_s3fs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1348,15 +1348,14 @@
         ContentLanguage="ru-RU",
         ContentType="text/csv",
         Expires=datetime.datetime(2015, 1, 1, 0, 0, tzinfo=tzutc()),
         Metadata={"string": "string"},
         ServerSideEncryption="AES256",
         StorageClass="REDUCED_REDUNDANCY",
         WebsiteRedirectLocation="https://www.example.com/",
-        BucketKeyEnabled=False,
     )
     with s3.open(a, "wb", **head) as f:
         f.write(b"data")
 
     with s3.open(a, "ab") as f:
         f.write(b"other")
 
@@ -1505,16 +1504,19 @@
     # Ensure merge mode updates value of existing key and adds new one
     new_tagset = {"tag2": "updatedvalue2", "tag3": "value3"}
     s3.put_tags(fname, new_tagset, mode="m")
     tagset.update(new_tagset)
     assert s3.get_tags(fname) == tagset
 
 
-def test_versions(s3):
-    versioned_file = versioned_bucket_name + "/versioned_file"
+@pytest.mark.parametrize("prefix", ["", "/dir", "/dir/subdir"])
+def test_versions(s3, prefix):
+    parent = versioned_bucket_name + prefix
+    versioned_file = parent + "/versioned_file"
+
     s3 = S3FileSystem(
         anon=False, version_aware=True, client_kwargs={"endpoint_url": endpoint_uri}
     )
     with s3.open(versioned_file, "wb") as fo:
         fo.write(b"1")
     first_version = fo.version_id
 
@@ -1534,14 +1536,25 @@
         assert fo.version_id == second_version
         assert fo.read() == b"2"
 
     with s3.open(versioned_file, version_id=first_version) as fo:
         assert fo.version_id == first_version
         assert fo.read() == b"1"
 
+    versioned_file_v1 = f"{versioned_file}?versionId={first_version}"
+    versioned_file_v2 = f"{versioned_file}?versionId={second_version}"
+
+    assert s3.ls(parent) == [versioned_file]
+    assert set(s3.ls(parent, versions=True)) == {versioned_file_v1, versioned_file_v2}
+
+    assert s3.exists(versioned_file_v1)
+    assert s3.info(versioned_file_v1)
+    assert s3.exists(versioned_file_v2)
+    assert s3.info(versioned_file_v2)
+
 
 def test_list_versions_many(s3):
     # moto doesn't actually behave in the same way that s3 does here so this doesn't test
     # anything really in moto 1.2
     s3 = S3FileSystem(
         anon=False, version_aware=True, client_kwargs={"endpoint_url": endpoint_uri}
     )
@@ -2611,13 +2624,15 @@
             skip_instance_cache=True,
         )
         await fs._mkdir(test_bucket_name)
         await fs._pipe(fn, data)
         f = await fs.open_async(fn, mode="rb", block_seze=1000)
         while True:
             got = await f.read(1000)
+            assert f.size == len(data)
+            assert f.tell()
             if not got:
                 break
             out.append(got)
 
     asyncio.run(read_stream())
     assert b"".join(out) == data
```

### Comparing `s3fs-2023.5.0/s3fs/utils.py` & `s3fs-2023.6.0/s3fs/utils.py`

 * *Files identical despite different names*

### Comparing `s3fs-2023.5.0/s3fs.egg-info/PKG-INFO` & `s3fs-2023.6.0/s3fs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s3fs
-Version: 2023.5.0
+Version: 2023.6.0
 Summary: Convenient Filesystem interface over S3
 Home-page: http://github.com/fsspec/s3fs/
 Maintainer: Martin Durant
 Maintainer-email: mdurant@continuum.io
 License: BSD
 Keywords: s3,boto
 Classifier: Development Status :: 4 - Beta
```

### Comparing `s3fs-2023.5.0/s3fs.egg-info/SOURCES.txt` & `s3fs-2023.6.0/s3fs.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -21,8 +21,11 @@
 s3fs.egg-info/dependency_links.txt
 s3fs.egg-info/not-zip-safe
 s3fs.egg-info/requires.txt
 s3fs.egg-info/top_level.txt
 s3fs/tests/__init__.py
 s3fs/tests/test_mapping.py
 s3fs/tests/test_s3fs.py
-s3fs/tests/test_utils.py
+s3fs/tests/test_utils.py
+s3fs/tests/derived/__init__.py
+s3fs/tests/derived/s3fs_fixtures.py
+s3fs/tests/derived/s3fs_test.py
```

### Comparing `s3fs-2023.5.0/setup.py` & `s3fs-2023.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `s3fs-2023.5.0/versioneer.py` & `s3fs-2023.6.0/versioneer.py`

 * *Files identical despite different names*

