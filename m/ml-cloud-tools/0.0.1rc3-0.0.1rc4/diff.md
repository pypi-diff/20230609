# Comparing `tmp/ml_cloud_tools-0.0.1rc3.tar.gz` & `tmp/ml_cloud_tools-0.0.1rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml_cloud_tools-0.0.1rc3.tar", last modified: Wed Jul 28 07:56:24 2021, max compression
+gzip compressed data, was "ml_cloud_tools-0.0.1rc4.tar", last modified: Wed Jul 28 12:54:26 2021, max compression
```

## Comparing `ml_cloud_tools-0.0.1rc3.tar` & `ml_cloud_tools-0.0.1rc4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-28 07:56:24.338690 ml_cloud_tools-0.0.1rc3/
--rw-r--r--   0 runner    (1001) docker     (121)     5519 2021-07-28 07:56:14.000000 ml_cloud_tools-0.0.1rc3/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     6564 2021-07-28 07:56:14.000000 ml_cloud_tools-0.0.1rc3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)     1180 2021-07-28 07:56:14.000000 ml_cloud_tools-0.0.1rc3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       57 2021-07-28 07:56:14.000000 ml_cloud_tools-0.0.1rc3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2450 2021-07-28 07:56:24.338690 ml_cloud_tools-0.0.1rc3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      731 2021-07-28 07:56:14.000000 ml_cloud_tools-0.0.1rc3/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      651 2021-07-28 07:56:14.000000 ml_cloud_tools-0.0.1rc3/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (121)      522 2021-07-28 07:56:14.000000 ml_cloud_tools-0.0.1rc3/THIRD-PARTY-NOTICES
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-28 07:56:24.338690 ml_cloud_tools-0.0.1rc3/ml_cloud_tools/
--rw-r--r--   0 runner    (1001) docker     (121)      270 2021-07-28 07:56:14.000000 ml_cloud_tools-0.0.1rc3/ml_cloud_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6735 2021-07-28 07:56:14.000000 ml_cloud_tools-0.0.1rc3/ml_cloud_tools/s3.py
--rw-r--r--   0 runner    (1001) docker     (121)      430 2021-07-28 07:56:14.000000 ml_cloud_tools-0.0.1rc3/ml_cloud_tools/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-28 07:56:24.338690 ml_cloud_tools-0.0.1rc3/ml_cloud_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2450 2021-07-28 07:56:24.000000 ml_cloud_tools-0.0.1rc3/ml_cloud_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      393 2021-07-28 07:56:24.000000 ml_cloud_tools-0.0.1rc3/ml_cloud_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-28 07:56:24.000000 ml_cloud_tools-0.0.1rc3/ml_cloud_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      116 2021-07-28 07:56:24.000000 ml_cloud_tools-0.0.1rc3/ml_cloud_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2021-07-28 07:56:24.000000 ml_cloud_tools-0.0.1rc3/ml_cloud_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      738 2021-07-28 07:56:14.000000 ml_cloud_tools-0.0.1rc3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      235 2021-07-28 07:56:24.338690 ml_cloud_tools-0.0.1rc3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2979 2021-07-28 07:56:14.000000 ml_cloud_tools-0.0.1rc3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-28 12:54:26.759505 ml_cloud_tools-0.0.1rc4/
+-rw-r--r--   0 runner    (1001) docker     (121)     5519 2021-07-28 12:54:13.000000 ml_cloud_tools-0.0.1rc4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     6564 2021-07-28 12:54:13.000000 ml_cloud_tools-0.0.1rc4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1180 2021-07-28 12:54:13.000000 ml_cloud_tools-0.0.1rc4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2021-07-28 12:54:13.000000 ml_cloud_tools-0.0.1rc4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     2450 2021-07-28 12:54:26.759505 ml_cloud_tools-0.0.1rc4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      731 2021-07-28 12:54:13.000000 ml_cloud_tools-0.0.1rc4/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      651 2021-07-28 12:54:13.000000 ml_cloud_tools-0.0.1rc4/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (121)      522 2021-07-28 12:54:13.000000 ml_cloud_tools-0.0.1rc4/THIRD-PARTY-NOTICES
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-28 12:54:26.759505 ml_cloud_tools-0.0.1rc4/ml_cloud_tools/
+-rw-r--r--   0 runner    (1001) docker     (121)      270 2021-07-28 12:54:13.000000 ml_cloud_tools-0.0.1rc4/ml_cloud_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8025 2021-07-28 12:54:13.000000 ml_cloud_tools-0.0.1rc4/ml_cloud_tools/s3.py
+-rw-r--r--   0 runner    (1001) docker     (121)      430 2021-07-28 12:54:13.000000 ml_cloud_tools-0.0.1rc4/ml_cloud_tools/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-28 12:54:26.759505 ml_cloud_tools-0.0.1rc4/ml_cloud_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2450 2021-07-28 12:54:26.000000 ml_cloud_tools-0.0.1rc4/ml_cloud_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      393 2021-07-28 12:54:26.000000 ml_cloud_tools-0.0.1rc4/ml_cloud_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-28 12:54:26.000000 ml_cloud_tools-0.0.1rc4/ml_cloud_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      116 2021-07-28 12:54:26.000000 ml_cloud_tools-0.0.1rc4/ml_cloud_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2021-07-28 12:54:26.000000 ml_cloud_tools-0.0.1rc4/ml_cloud_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      738 2021-07-28 12:54:13.000000 ml_cloud_tools-0.0.1rc4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      235 2021-07-28 12:54:26.759505 ml_cloud_tools-0.0.1rc4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2979 2021-07-28 12:54:13.000000 ml_cloud_tools-0.0.1rc4/setup.py
```

### Comparing `ml_cloud_tools-0.0.1rc3/CODE_OF_CONDUCT.md` & `ml_cloud_tools-0.0.1rc4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `ml_cloud_tools-0.0.1rc3/CONTRIBUTING.md` & `ml_cloud_tools-0.0.1rc4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ml_cloud_tools-0.0.1rc3/LICENSE` & `ml_cloud_tools-0.0.1rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `ml_cloud_tools-0.0.1rc3/PKG-INFO` & `ml_cloud_tools-0.0.1rc4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml_cloud_tools
-Version: 0.0.1rc3
+Version: 0.0.1rc4
 Summary: ML Tools for the Cloud
 Home-page: https://github.com/telekom/ml-cloud-tools
 Author: Philip May
 Author-email: philip.may@t-systems.com
 Maintainer: Philip May
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/telekom/ml-cloud-tools/issues
```

### Comparing `ml_cloud_tools-0.0.1rc3/README.md` & `ml_cloud_tools-0.0.1rc4/README.md`

 * *Files identical despite different names*

### Comparing `ml_cloud_tools-0.0.1rc3/SECURITY.md` & `ml_cloud_tools-0.0.1rc4/SECURITY.md`

 * *Files identical despite different names*

### Comparing `ml_cloud_tools-0.0.1rc3/THIRD-PARTY-NOTICES` & `ml_cloud_tools-0.0.1rc4/THIRD-PARTY-NOTICES`

 * *Files identical despite different names*

### Comparing `ml_cloud_tools-0.0.1rc3/ml_cloud_tools/s3.py` & `ml_cloud_tools-0.0.1rc4/ml_cloud_tools/s3.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,32 +5,38 @@
 
 
 """S3 tools."""
 
 import logging
 import os
 from pathlib import Path
-from typing import Any, Dict, Optional
+from typing import Any, Dict, List, Optional
 
 import boto3
 
 
 _logger = logging.getLogger(__name__)
 
 
-def _get_s3_bucket(s3_bucket_name: Optional[str] = None):
+def _get_s3_bucket_name(s3_bucket_name) -> str:
     if s3_bucket_name is None:
         s3_bucket_name = os.getenv("DEFAULT_S3_BUCKET_NAME")
     if s3_bucket_name is None:
         raise ValueError(
             "S3 bucket name must be set by parameter or the "
             "'DEFAULT_S3_BUCKET_NAME' environment variable!"
         )
-    # see https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#bucket
+    return s3_bucket_name
+
+
+def _get_s3_bucket(s3_bucket_name: Optional[str] = None):
+    s3_bucket_name = _get_s3_bucket_name(s3_bucket_name)
+    # see https://boto3.amazonaws.com/v1/documentation/api/latest/reference/core/boto3.html?highlight=resource#boto3.resource  # NOQA: E501
     s3_resource = boto3.resource("s3")
+    # see https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#bucket
     bucket = s3_resource.Bucket(s3_bucket_name)
     return bucket
 
 
 def copy_s3_file_to_file(
     s3_file_name: str,
     local_file_name: str,
@@ -151,7 +157,35 @@
             _logger.debug("Skipping dir %s", file_path.as_posix())
         else:
             s3_file_path = final_s3_dir_path / file_path.relative_to(local_dir_path)
             _logger.debug("Copying %s to S3 %s", file_path.as_posix(), s3_file_path.as_posix())
             # see https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Bucket.upload_file  # NOQA: E501
             s3_bucket.upload_file(file_path.as_posix(), s3_file_path.as_posix(), **s3_kwargs)
     return final_s3_dir_path.as_posix()
+
+
+def list_s3_files(
+    s3_dir_name: str,
+    max_files: int = 100,
+    s3_bucket_name: Optional[str] = None,
+) -> List[str]:
+    """List files in S3 directory."""
+    s3_bucket_name = _get_s3_bucket_name(s3_bucket_name)
+    s3_client = boto3.client("s3")
+    response = s3_client.list_objects_v2(
+        Bucket=s3_bucket_name, Prefix=s3_dir_name, MaxKeys=max_files
+    )
+    if response["KeyCount"] == 0:
+        _logger.warning("S3 s3_dir_name %s empty", s3_dir_name)
+        return []
+    files = [key_dict["Key"] for key_dict in response["Contents"]]
+    while response["IsTruncated"]:
+        _logger.debug("Got continuation token, re-listing")
+        continuation_token = response["NextContinuationToken"]
+        response = s3_client.list_objects_v2(
+            Bucket=s3_bucket_name,
+            Prefix=s3_dir_name,
+            MaxKeys=max_files,
+            ContinuationToken=continuation_token,
+        )
+        files.extend(key_dict["Key"] for key_dict in response["Contents"])
+    return files
```

### Comparing `ml_cloud_tools-0.0.1rc3/ml_cloud_tools.egg-info/PKG-INFO` & `ml_cloud_tools-0.0.1rc4/ml_cloud_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-cloud-tools
-Version: 0.0.1rc3
+Version: 0.0.1rc4
 Summary: ML Tools for the Cloud
 Home-page: https://github.com/telekom/ml-cloud-tools
 Author: Philip May
 Author-email: philip.may@t-systems.com
 Maintainer: Philip May
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/telekom/ml-cloud-tools/issues
```

### Comparing `ml_cloud_tools-0.0.1rc3/pyproject.toml` & `ml_cloud_tools-0.0.1rc4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ml_cloud_tools-0.0.1rc3/setup.py` & `ml_cloud_tools-0.0.1rc4/setup.py`

 * *Files identical despite different names*

