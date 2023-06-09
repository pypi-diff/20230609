# Comparing `tmp/secure-bucket-construct-2.1.8.tar.gz` & `tmp/secure-bucket-construct-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secure-bucket-construct-2.1.8.tar", last modified: Thu Oct 20 07:05:19 2022, max compression
+gzip compressed data, was "secure-bucket-construct-2.1.9.tar", last modified: Tue Dec  6 14:48:03 2022, max compression
```

## Comparing `secure-bucket-construct-2.1.8.tar` & `secure-bucket-construct-2.1.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 07:05:19.153537 secure-bucket-construct-2.1.8/
--rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-10-20 07:05:04.000000 secure-bucket-construct-2.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-10-20 07:05:04.000000 secure-bucket-construct-2.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2425 2022-10-20 07:05:19.153537 secure-bucket-construct-2.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1500 2022-10-20 07:05:04.000000 secure-bucket-construct-2.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      236 2022-10-20 07:05:04.000000 secure-bucket-construct-2.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-20 07:05:19.153537 secure-bucket-construct-2.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1794 2022-10-20 07:05:04.000000 secure-bucket-construct-2.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 07:05:19.153537 secure-bucket-construct-2.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 07:05:19.153537 secure-bucket-construct-2.1.8/src/secure_bucket_construct/
--rw-r--r--   0 runner    (1001) docker     (121)    14328 2022-10-20 07:05:04.000000 secure-bucket-construct-2.1.8/src/secure_bucket_construct/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 07:05:19.153537 secure-bucket-construct-2.1.8/src/secure_bucket_construct/_jsii/
--rw-r--r--   0 runner    (1001) docker     (121)      426 2022-10-20 07:05:04.000000 secure-bucket-construct-2.1.8/src/secure_bucket_construct/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15291 2022-10-20 07:05:04.000000 secure-bucket-construct-2.1.8/src/secure_bucket_construct/_jsii/secure_bucket_construct@2.1.8.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-20 07:05:04.000000 secure-bucket-construct-2.1.8/src/secure_bucket_construct/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 07:05:19.153537 secure-bucket-construct-2.1.8/src/secure_bucket_construct.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2425 2022-10-20 07:05:18.000000 secure-bucket-construct-2.1.8/src/secure_bucket_construct.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      503 2022-10-20 07:05:19.000000 secure-bucket-construct-2.1.8/src/secure_bucket_construct.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-20 07:05:18.000000 secure-bucket-construct-2.1.8/src/secure_bucket_construct.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      111 2022-10-20 07:05:18.000000 secure-bucket-construct-2.1.8/src/secure_bucket_construct.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-10-20 07:05:19.000000 secure-bucket-construct-2.1.8/src/secure_bucket_construct.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 14:48:03.405981 secure-bucket-construct-2.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2022-12-06 14:47:49.000000 secure-bucket-construct-2.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2022-12-06 14:47:49.000000 secure-bucket-construct-2.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2022-12-06 14:48:03.405981 secure-bucket-construct-2.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2022-12-06 14:47:49.000000 secure-bucket-construct-2.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2022-12-06 14:47:49.000000 secure-bucket-construct-2.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-06 14:48:03.405981 secure-bucket-construct-2.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2022-12-06 14:47:49.000000 secure-bucket-construct-2.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 14:48:03.401981 secure-bucket-construct-2.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 14:48:03.401981 secure-bucket-construct-2.1.9/src/secure_bucket_construct/
+-rw-r--r--   0 runner    (1001) docker     (123)    14944 2022-12-06 14:47:49.000000 secure-bucket-construct-2.1.9/src/secure_bucket_construct/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 14:48:03.405981 secure-bucket-construct-2.1.9/src/secure_bucket_construct/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2022-12-06 14:47:49.000000 secure-bucket-construct-2.1.9/src/secure_bucket_construct/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15287 2022-12-06 14:47:49.000000 secure-bucket-construct-2.1.9/src/secure_bucket_construct/_jsii/secure_bucket_construct@2.1.9.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-06 14:47:49.000000 secure-bucket-construct-2.1.9/src/secure_bucket_construct/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 14:48:03.401981 secure-bucket-construct-2.1.9/src/secure_bucket_construct.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2022-12-06 14:48:02.000000 secure-bucket-construct-2.1.9/src/secure_bucket_construct.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2022-12-06 14:48:03.000000 secure-bucket-construct-2.1.9/src/secure_bucket_construct.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-06 14:48:02.000000 secure-bucket-construct-2.1.9/src/secure_bucket_construct.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2022-12-06 14:48:03.000000 secure-bucket-construct-2.1.9/src/secure_bucket_construct.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2022-12-06 14:48:03.000000 secure-bucket-construct-2.1.9/src/secure_bucket_construct.egg-info/top_level.txt
```

### Comparing `secure-bucket-construct-2.1.8/LICENSE` & `secure-bucket-construct-2.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `secure-bucket-construct-2.1.8/PKG-INFO` & `secure-bucket-construct-2.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secure-bucket-construct
-Version: 2.1.8
+Version: 2.1.9
 Summary: secure_bucket_construct
 Home-page: https://github.com/yvthepief/secure_bucket_construct.git
 Author: Yvo van Zee<yvo@yvovanzee.nl>
 License: Apache-2.0
 Project-URL: Source, https://github.com/yvthepief/secure_bucket_construct.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `secure-bucket-construct-2.1.8/README.md` & `secure-bucket-construct-2.1.9/README.md`

 * *Files identical despite different names*

### Comparing `secure-bucket-construct-2.1.8/setup.py` & `secure-bucket-construct-2.1.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "secure-bucket-construct",
-    "version": "2.1.8",
+    "version": "2.1.9",
     "description": "secure_bucket_construct",
     "license": "Apache-2.0",
     "url": "https://github.com/yvthepief/secure_bucket_construct.git",
     "long_description_content_type": "text/markdown",
     "author": "Yvo van Zee<yvo@yvovanzee.nl>",
     "bdist_wheel": {
         "universal": true
@@ -22,25 +22,25 @@
     },
     "packages": [
         "secure_bucket_construct",
         "secure_bucket_construct._jsii"
     ],
     "package_data": {
         "secure_bucket_construct._jsii": [
-            "secure_bucket_construct@2.1.8.jsii.tgz"
+            "secure_bucket_construct@2.1.9.jsii.tgz"
         ],
         "secure_bucket_construct": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "aws-cdk-lib>=2.33.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
-        "jsii>=1.70.0, <2.0.0",
+        "jsii>=1.72.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `secure-bucket-construct-2.1.8/src/secure_bucket_construct/__init__.py` & `secure-bucket-construct-2.1.9/src/secure_bucket_construct/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -51,57 +51,57 @@
 import publication
 import typing_extensions
 
 from typeguard import check_type
 
 from ._jsii import *
 
-import aws_cdk
-import aws_cdk.aws_iam
-import aws_cdk.aws_kms
-import aws_cdk.aws_s3
-import constructs
+import aws_cdk as _aws_cdk_ceddda9d
+import aws_cdk.aws_iam as _aws_cdk_aws_iam_ceddda9d
+import aws_cdk.aws_kms as _aws_cdk_aws_kms_ceddda9d
+import aws_cdk.aws_s3 as _aws_cdk_aws_s3_ceddda9d
+import constructs as _constructs_77d1e7e8
 
 
 class SecureBucket(
-    constructs.Construct,
+    _constructs_77d1e7e8.Construct,
     metaclass=jsii.JSIIMeta,
     jsii_type="secure_bucket_construct.SecureBucket",
 ):
     def __init__(
         self,
-        scope: constructs.Construct,
+        scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
-        access_control: typing.Optional[aws_cdk.aws_s3.BucketAccessControl] = None,
+        access_control: typing.Optional[_aws_cdk_aws_s3_ceddda9d.BucketAccessControl] = None,
         auto_delete_objects: typing.Optional[builtins.bool] = None,
-        block_public_access: typing.Optional[aws_cdk.aws_s3.BlockPublicAccess] = None,
+        block_public_access: typing.Optional[_aws_cdk_aws_s3_ceddda9d.BlockPublicAccess] = None,
         bucket_key_enabled: typing.Optional[builtins.bool] = None,
         bucket_name: typing.Optional[builtins.str] = None,
-        cors: typing.Optional[typing.Sequence[typing.Union[aws_cdk.aws_s3.CorsRule, typing.Dict[str, typing.Any]]]] = None,
-        encryption: typing.Optional[aws_cdk.aws_s3.BucketEncryption] = None,
-        encryption_key: typing.Optional[aws_cdk.aws_kms.IKey] = None,
+        cors: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_s3_ceddda9d.CorsRule, typing.Dict[builtins.str, typing.Any]]]] = None,
+        encryption: typing.Optional[_aws_cdk_aws_s3_ceddda9d.BucketEncryption] = None,
+        encryption_key: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
         enforce_ssl: typing.Optional[builtins.bool] = None,
         event_bridge_enabled: typing.Optional[builtins.bool] = None,
-        intelligent_tiering_configurations: typing.Optional[typing.Sequence[typing.Union[aws_cdk.aws_s3.IntelligentTieringConfiguration, typing.Dict[str, typing.Any]]]] = None,
-        inventories: typing.Optional[typing.Sequence[typing.Union[aws_cdk.aws_s3.Inventory, typing.Dict[str, typing.Any]]]] = None,
-        lifecycle_rules: typing.Optional[typing.Sequence[typing.Union[aws_cdk.aws_s3.LifecycleRule, typing.Dict[str, typing.Any]]]] = None,
-        metrics: typing.Optional[typing.Sequence[typing.Union[aws_cdk.aws_s3.BucketMetrics, typing.Dict[str, typing.Any]]]] = None,
-        notifications_handler_role: typing.Optional[aws_cdk.aws_iam.IRole] = None,
-        object_ownership: typing.Optional[aws_cdk.aws_s3.ObjectOwnership] = None,
+        intelligent_tiering_configurations: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_s3_ceddda9d.IntelligentTieringConfiguration, typing.Dict[builtins.str, typing.Any]]]] = None,
+        inventories: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_s3_ceddda9d.Inventory, typing.Dict[builtins.str, typing.Any]]]] = None,
+        lifecycle_rules: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_s3_ceddda9d.LifecycleRule, typing.Dict[builtins.str, typing.Any]]]] = None,
+        metrics: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_s3_ceddda9d.BucketMetrics, typing.Dict[builtins.str, typing.Any]]]] = None,
+        notifications_handler_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
+        object_ownership: typing.Optional[_aws_cdk_aws_s3_ceddda9d.ObjectOwnership] = None,
         public_read_access: typing.Optional[builtins.bool] = None,
-        removal_policy: typing.Optional[aws_cdk.RemovalPolicy] = None,
-        server_access_logs_bucket: typing.Optional[aws_cdk.aws_s3.IBucket] = None,
+        removal_policy: typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy] = None,
+        server_access_logs_bucket: typing.Optional[_aws_cdk_aws_s3_ceddda9d.IBucket] = None,
         server_access_logs_prefix: typing.Optional[builtins.str] = None,
         transfer_acceleration: typing.Optional[builtins.bool] = None,
         versioned: typing.Optional[builtins.bool] = None,
         website_error_document: typing.Optional[builtins.str] = None,
         website_index_document: typing.Optional[builtins.str] = None,
-        website_redirect: typing.Optional[typing.Union[aws_cdk.aws_s3.RedirectTarget, typing.Dict[str, typing.Any]]] = None,
-        website_routing_rules: typing.Optional[typing.Sequence[typing.Union[aws_cdk.aws_s3.RoutingRule, typing.Dict[str, typing.Any]]]] = None,
+        website_redirect: typing.Optional[typing.Union[_aws_cdk_aws_s3_ceddda9d.RedirectTarget, typing.Dict[builtins.str, typing.Any]]] = None,
+        website_routing_rules: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_s3_ceddda9d.RoutingRule, typing.Dict[builtins.str, typing.Any]]]] = None,
     ) -> None:
         '''
         :param scope: -
         :param id: -
         :param access_control: Specifies a canned ACL that grants predefined permissions to the bucket. Default: BucketAccessControl.PRIVATE
         :param auto_delete_objects: Whether all objects should be automatically deleted when the bucket is removed from the stack or when the stack is deleted. Requires the ``removalPolicy`` to be set to ``RemovalPolicy.DESTROY``. **Warning** if you have deployed a bucket with ``autoDeleteObjects: true``, switching this to ``false`` in a CDK version *before* ``1.126.0`` will lead to all objects in the bucket being deleted. Be sure to update your bucket resources by deploying with CDK version ``1.126.0`` or later **before** switching this value to ``false``. Default: false
         :param block_public_access: The block public access configuration of this bucket. Default: - CloudFormation defaults will apply. New buckets and objects don't allow public access, but users can modify bucket policies or object permissions to allow public access
@@ -126,50 +126,18 @@
         :param versioned: Whether this bucket should have versioning turned on or not. Default: false
         :param website_error_document: The name of the error document (e.g. "404.html") for the website. ``websiteIndexDocument`` must also be set if this is set. Default: - No error document.
         :param website_index_document: The name of the index document (e.g. "index.html") for the website. Enables static website hosting for this bucket. Default: - No index document.
         :param website_redirect: Specifies the redirect behavior of all requests to a website endpoint of a bucket. If you specify this property, you can't specify "websiteIndexDocument", "websiteErrorDocument" nor , "websiteRoutingRules". Default: - No redirection.
         :param website_routing_rules: Rules that define when a redirect is applied and the redirect behavior. Default: - No redirection rules.
         '''
         if __debug__:
-            def stub(
-                scope: constructs.Construct,
-                id: builtins.str,
-                *,
-                access_control: typing.Optional[aws_cdk.aws_s3.BucketAccessControl] = None,
-                auto_delete_objects: typing.Optional[builtins.bool] = None,
-                block_public_access: typing.Optional[aws_cdk.aws_s3.BlockPublicAccess] = None,
-                bucket_key_enabled: typing.Optional[builtins.bool] = None,
-                bucket_name: typing.Optional[builtins.str] = None,
-                cors: typing.Optional[typing.Sequence[typing.Union[aws_cdk.aws_s3.CorsRule, typing.Dict[str, typing.Any]]]] = None,
-                encryption: typing.Optional[aws_cdk.aws_s3.BucketEncryption] = None,
-                encryption_key: typing.Optional[aws_cdk.aws_kms.IKey] = None,
-                enforce_ssl: typing.Optional[builtins.bool] = None,
-                event_bridge_enabled: typing.Optional[builtins.bool] = None,
-                intelligent_tiering_configurations: typing.Optional[typing.Sequence[typing.Union[aws_cdk.aws_s3.IntelligentTieringConfiguration, typing.Dict[str, typing.Any]]]] = None,
-                inventories: typing.Optional[typing.Sequence[typing.Union[aws_cdk.aws_s3.Inventory, typing.Dict[str, typing.Any]]]] = None,
-                lifecycle_rules: typing.Optional[typing.Sequence[typing.Union[aws_cdk.aws_s3.LifecycleRule, typing.Dict[str, typing.Any]]]] = None,
-                metrics: typing.Optional[typing.Sequence[typing.Union[aws_cdk.aws_s3.BucketMetrics, typing.Dict[str, typing.Any]]]] = None,
-                notifications_handler_role: typing.Optional[aws_cdk.aws_iam.IRole] = None,
-                object_ownership: typing.Optional[aws_cdk.aws_s3.ObjectOwnership] = None,
-                public_read_access: typing.Optional[builtins.bool] = None,
-                removal_policy: typing.Optional[aws_cdk.RemovalPolicy] = None,
-                server_access_logs_bucket: typing.Optional[aws_cdk.aws_s3.IBucket] = None,
-                server_access_logs_prefix: typing.Optional[builtins.str] = None,
-                transfer_acceleration: typing.Optional[builtins.bool] = None,
-                versioned: typing.Optional[builtins.bool] = None,
-                website_error_document: typing.Optional[builtins.str] = None,
-                website_index_document: typing.Optional[builtins.str] = None,
-                website_redirect: typing.Optional[typing.Union[aws_cdk.aws_s3.RedirectTarget, typing.Dict[str, typing.Any]]] = None,
-                website_routing_rules: typing.Optional[typing.Sequence[typing.Union[aws_cdk.aws_s3.RoutingRule, typing.Dict[str, typing.Any]]]] = None,
-            ) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__25f568a5935f126e6ba9e9aa00c4a5d82eaa0961270a2c7279c8e5c39da279c6)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
-        props = aws_cdk.aws_s3.BucketProps(
+        props = _aws_cdk_aws_s3_ceddda9d.BucketProps(
             access_control=access_control,
             auto_delete_objects=auto_delete_objects,
             block_public_access=block_public_access,
             bucket_key_enabled=bucket_key_enabled,
             bucket_name=bucket_name,
             cors=cors,
             encryption=encryption,
@@ -194,25 +162,63 @@
             website_routing_rules=website_routing_rules,
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
     @builtins.property
     @jsii.member(jsii_name="bucket")
-    def bucket(self) -> aws_cdk.aws_s3.Bucket:
-        return typing.cast(aws_cdk.aws_s3.Bucket, jsii.get(self, "bucket"))
+    def bucket(self) -> _aws_cdk_aws_s3_ceddda9d.Bucket:
+        return typing.cast(_aws_cdk_aws_s3_ceddda9d.Bucket, jsii.get(self, "bucket"))
 
     @bucket.setter
-    def bucket(self, value: aws_cdk.aws_s3.Bucket) -> None:
+    def bucket(self, value: _aws_cdk_aws_s3_ceddda9d.Bucket) -> None:
         if __debug__:
-            def stub(value: aws_cdk.aws_s3.Bucket) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__ab720b716985dd12ee16838610bc73e3b50228bdc2c7eda38dc0a4e4be5cbf1b)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "bucket", value)
 
 
 __all__ = [
     "SecureBucket",
 ]
 
 publication.publish()
+
+def _typecheckingstub__25f568a5935f126e6ba9e9aa00c4a5d82eaa0961270a2c7279c8e5c39da279c6(
+    scope: _constructs_77d1e7e8.Construct,
+    id: builtins.str,
+    *,
+    access_control: typing.Optional[_aws_cdk_aws_s3_ceddda9d.BucketAccessControl] = None,
+    auto_delete_objects: typing.Optional[builtins.bool] = None,
+    block_public_access: typing.Optional[_aws_cdk_aws_s3_ceddda9d.BlockPublicAccess] = None,
+    bucket_key_enabled: typing.Optional[builtins.bool] = None,
+    bucket_name: typing.Optional[builtins.str] = None,
+    cors: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_s3_ceddda9d.CorsRule, typing.Dict[builtins.str, typing.Any]]]] = None,
+    encryption: typing.Optional[_aws_cdk_aws_s3_ceddda9d.BucketEncryption] = None,
+    encryption_key: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
+    enforce_ssl: typing.Optional[builtins.bool] = None,
+    event_bridge_enabled: typing.Optional[builtins.bool] = None,
+    intelligent_tiering_configurations: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_s3_ceddda9d.IntelligentTieringConfiguration, typing.Dict[builtins.str, typing.Any]]]] = None,
+    inventories: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_s3_ceddda9d.Inventory, typing.Dict[builtins.str, typing.Any]]]] = None,
+    lifecycle_rules: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_s3_ceddda9d.LifecycleRule, typing.Dict[builtins.str, typing.Any]]]] = None,
+    metrics: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_s3_ceddda9d.BucketMetrics, typing.Dict[builtins.str, typing.Any]]]] = None,
+    notifications_handler_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
+    object_ownership: typing.Optional[_aws_cdk_aws_s3_ceddda9d.ObjectOwnership] = None,
+    public_read_access: typing.Optional[builtins.bool] = None,
+    removal_policy: typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy] = None,
+    server_access_logs_bucket: typing.Optional[_aws_cdk_aws_s3_ceddda9d.IBucket] = None,
+    server_access_logs_prefix: typing.Optional[builtins.str] = None,
+    transfer_acceleration: typing.Optional[builtins.bool] = None,
+    versioned: typing.Optional[builtins.bool] = None,
+    website_error_document: typing.Optional[builtins.str] = None,
+    website_index_document: typing.Optional[builtins.str] = None,
+    website_redirect: typing.Optional[typing.Union[_aws_cdk_aws_s3_ceddda9d.RedirectTarget, typing.Dict[builtins.str, typing.Any]]] = None,
+    website_routing_rules: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_s3_ceddda9d.RoutingRule, typing.Dict[builtins.str, typing.Any]]]] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__ab720b716985dd12ee16838610bc73e3b50228bdc2c7eda38dc0a4e4be5cbf1b(
+    value: _aws_cdk_aws_s3_ceddda9d.Bucket,
+) -> None:
+    """Type checking stubs"""
+    pass
```

### Comparing `secure-bucket-construct-2.1.8/src/secure_bucket_construct.egg-info/PKG-INFO` & `secure-bucket-construct-2.1.9/src/secure_bucket_construct.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secure-bucket-construct
-Version: 2.1.8
+Version: 2.1.9
 Summary: secure_bucket_construct
 Home-page: https://github.com/yvthepief/secure_bucket_construct.git
 Author: Yvo van Zee<yvo@yvovanzee.nl>
 License: Apache-2.0
 Project-URL: Source, https://github.com/yvthepief/secure_bucket_construct.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

