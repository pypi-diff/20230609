# Comparing `tmp/cdk-pgstac-4.1.0.tar.gz` & `tmp/cdk-pgstac-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-pgstac-4.1.0.tar", last modified: Tue May 30 00:10:54 2023, max compression
+gzip compressed data, was "cdk-pgstac-4.2.0.tar", last modified: Fri Jun  9 03:13:36 2023, max compression
```

## Comparing `cdk-pgstac-4.1.0.tar` & `cdk-pgstac-4.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:10:54.343108 cdk-pgstac-4.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-30 00:10:45.000000 cdk-pgstac-4.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-30 00:10:45.000000 cdk-pgstac-4.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-30 00:10:54.343108 cdk-pgstac-4.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-30 00:10:45.000000 cdk-pgstac-4.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-30 00:10:45.000000 cdk-pgstac-4.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 00:10:54.343108 cdk-pgstac-4.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-30 00:10:45.000000 cdk-pgstac-4.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:10:54.343108 cdk-pgstac-4.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:10:54.343108 cdk-pgstac-4.1.0/src/cdk_pgstac/
--rw-r--r--   0 runner    (1001) docker     (123)   124828 2023-05-30 00:10:45.000000 cdk-pgstac-4.1.0/src/cdk_pgstac/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:10:54.343108 cdk-pgstac-4.1.0/src/cdk_pgstac/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-30 00:10:45.000000 cdk-pgstac-4.1.0/src/cdk_pgstac/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   161106 2023-05-30 00:10:45.000000 cdk-pgstac-4.1.0/src/cdk_pgstac/_jsii/cdk-pgstac@4.1.0.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 00:10:45.000000 cdk-pgstac-4.1.0/src/cdk_pgstac/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:10:54.343108 cdk-pgstac-4.1.0/src/cdk_pgstac.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-30 00:10:53.000000 cdk-pgstac-4.1.0/src/cdk_pgstac.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-30 00:10:54.000000 cdk-pgstac-4.1.0/src/cdk_pgstac.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 00:10:53.000000 cdk-pgstac-4.1.0/src/cdk_pgstac.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-30 00:10:54.000000 cdk-pgstac-4.1.0/src/cdk_pgstac.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-30 00:10:54.000000 cdk-pgstac-4.1.0/src/cdk_pgstac.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 03:13:36.781808 cdk-pgstac-4.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-09 03:13:25.000000 cdk-pgstac-4.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-09 03:13:25.000000 cdk-pgstac-4.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-09 03:13:36.781808 cdk-pgstac-4.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-09 03:13:25.000000 cdk-pgstac-4.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-09 03:13:25.000000 cdk-pgstac-4.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 03:13:36.781808 cdk-pgstac-4.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-09 03:13:25.000000 cdk-pgstac-4.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 03:13:36.777808 cdk-pgstac-4.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 03:13:36.777808 cdk-pgstac-4.2.0/src/cdk_pgstac/
+-rw-r--r--   0 runner    (1001) docker     (123)   133159 2023-06-09 03:13:25.000000 cdk-pgstac-4.2.0/src/cdk_pgstac/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 03:13:36.781808 cdk-pgstac-4.2.0/src/cdk_pgstac/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-09 03:13:25.000000 cdk-pgstac-4.2.0/src/cdk_pgstac/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   165491 2023-06-09 03:13:25.000000 cdk-pgstac-4.2.0/src/cdk_pgstac/_jsii/cdk-pgstac@4.2.0.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 03:13:25.000000 cdk-pgstac-4.2.0/src/cdk_pgstac/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 03:13:36.777808 cdk-pgstac-4.2.0/src/cdk_pgstac.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-09 03:13:36.000000 cdk-pgstac-4.2.0/src/cdk_pgstac.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-09 03:13:36.000000 cdk-pgstac-4.2.0/src/cdk_pgstac.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 03:13:36.000000 cdk-pgstac-4.2.0/src/cdk_pgstac.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-09 03:13:36.000000 cdk-pgstac-4.2.0/src/cdk_pgstac.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-09 03:13:36.000000 cdk-pgstac-4.2.0/src/cdk_pgstac.egg-info/top_level.txt
```

### Comparing `cdk-pgstac-4.1.0/LICENSE` & `cdk-pgstac-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-pgstac-4.1.0/PKG-INFO` & `cdk-pgstac-4.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-pgstac
-Version: 4.1.0
+Version: 4.2.0
 Summary: A set of constructs deploying pgSTAC with CDK
 Home-page: https://github.com/developmentseed/cdk-pgstac.git
 Author: Anthony Lukach<anthony@developmentseed.org>
 License: ISC
 Project-URL: Source, https://github.com/developmentseed/cdk-pgstac.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `cdk-pgstac-4.1.0/README.md` & `cdk-pgstac-4.2.0/README.md`

 * *Files identical despite different names*

### Comparing `cdk-pgstac-4.1.0/setup.py` & `cdk-pgstac-4.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-pgstac",
-    "version": "4.1.0",
+    "version": "4.2.0",
     "description": "A set of constructs deploying pgSTAC with CDK",
     "license": "ISC",
     "url": "https://github.com/developmentseed/cdk-pgstac.git",
     "long_description_content_type": "text/markdown",
     "author": "Anthony Lukach<anthony@developmentseed.org>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk_pgstac",
         "cdk_pgstac._jsii"
     ],
     "package_data": {
         "cdk_pgstac._jsii": [
-            "cdk-pgstac@4.1.0.jsii.tgz"
+            "cdk-pgstac@4.2.0.jsii.tgz"
         ],
         "cdk_pgstac": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdk-pgstac-4.1.0/src/cdk_pgstac/__init__.py` & `cdk-pgstac-4.2.0/src/cdk_pgstac/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 
 import aws_cdk
 import aws_cdk.aws_apigateway
 import aws_cdk.aws_dynamodb
 import aws_cdk.aws_ec2
 import aws_cdk.aws_iam
 import aws_cdk.aws_kms
+import aws_cdk.aws_lambda
 import aws_cdk.aws_lambda_python_alpha
 import aws_cdk.aws_logs
 import aws_cdk.aws_rds
 import aws_cdk.aws_s3
 import aws_cdk.aws_secretsmanager
 import constructs
 
@@ -2435,23 +2436,224 @@
 
     def __repr__(self) -> str:
         return "StacIngestorProps(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
+@jsii.data_type(
+    jsii_type="cdk-pgstac.TitilerPgStacApiLambdaProps",
+    jsii_struct_bases=[],
+    name_mapping={
+        "db": "db",
+        "db_secret": "dbSecret",
+        "subnet_selection": "subnetSelection",
+        "vpc": "vpc",
+        "api_env": "apiEnv",
+        "buckets": "buckets",
+    },
+)
+class TitilerPgStacApiLambdaProps:
+    def __init__(
+        self,
+        *,
+        db: aws_cdk.aws_rds.IDatabaseInstance,
+        db_secret: aws_cdk.aws_secretsmanager.ISecret,
+        subnet_selection: typing.Union[aws_cdk.aws_ec2.SubnetSelection, typing.Dict[str, typing.Any]],
+        vpc: aws_cdk.aws_ec2.IVpc,
+        api_env: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
+        buckets: typing.Optional[typing.Sequence[builtins.str]] = None,
+    ) -> None:
+        '''
+        :param db: (experimental) RDS Instance with installed pgSTAC.
+        :param db_secret: (experimental) Secret containing connection information for pgSTAC database.
+        :param subnet_selection: (experimental) Subnet into which the lambda should be deployed.
+        :param vpc: (experimental) VPC into which the lambda should be deployed.
+        :param api_env: (experimental) Customized environment variables to send to titiler-pgstac runtime.
+        :param buckets: (experimental) list of buckets the lambda will be granted access to.
+
+        :stability: experimental
+        '''
+        if isinstance(subnet_selection, dict):
+            subnet_selection = aws_cdk.aws_ec2.SubnetSelection(**subnet_selection)
+        if __debug__:
+            type_hints = typing.get_type_hints(TitilerPgStacApiLambdaProps.__init__)
+            check_type(argname="argument db", value=db, expected_type=type_hints["db"])
+            check_type(argname="argument db_secret", value=db_secret, expected_type=type_hints["db_secret"])
+            check_type(argname="argument subnet_selection", value=subnet_selection, expected_type=type_hints["subnet_selection"])
+            check_type(argname="argument vpc", value=vpc, expected_type=type_hints["vpc"])
+            check_type(argname="argument api_env", value=api_env, expected_type=type_hints["api_env"])
+            check_type(argname="argument buckets", value=buckets, expected_type=type_hints["buckets"])
+        self._values: typing.Dict[str, typing.Any] = {
+            "db": db,
+            "db_secret": db_secret,
+            "subnet_selection": subnet_selection,
+            "vpc": vpc,
+        }
+        if api_env is not None:
+            self._values["api_env"] = api_env
+        if buckets is not None:
+            self._values["buckets"] = buckets
+
+    @builtins.property
+    def db(self) -> aws_cdk.aws_rds.IDatabaseInstance:
+        '''(experimental) RDS Instance with installed pgSTAC.
+
+        :stability: experimental
+        '''
+        result = self._values.get("db")
+        assert result is not None, "Required property 'db' is missing"
+        return typing.cast(aws_cdk.aws_rds.IDatabaseInstance, result)
+
+    @builtins.property
+    def db_secret(self) -> aws_cdk.aws_secretsmanager.ISecret:
+        '''(experimental) Secret containing connection information for pgSTAC database.
+
+        :stability: experimental
+        '''
+        result = self._values.get("db_secret")
+        assert result is not None, "Required property 'db_secret' is missing"
+        return typing.cast(aws_cdk.aws_secretsmanager.ISecret, result)
+
+    @builtins.property
+    def subnet_selection(self) -> aws_cdk.aws_ec2.SubnetSelection:
+        '''(experimental) Subnet into which the lambda should be deployed.
+
+        :stability: experimental
+        '''
+        result = self._values.get("subnet_selection")
+        assert result is not None, "Required property 'subnet_selection' is missing"
+        return typing.cast(aws_cdk.aws_ec2.SubnetSelection, result)
+
+    @builtins.property
+    def vpc(self) -> aws_cdk.aws_ec2.IVpc:
+        '''(experimental) VPC into which the lambda should be deployed.
+
+        :stability: experimental
+        '''
+        result = self._values.get("vpc")
+        assert result is not None, "Required property 'vpc' is missing"
+        return typing.cast(aws_cdk.aws_ec2.IVpc, result)
+
+    @builtins.property
+    def api_env(self) -> typing.Optional[typing.Mapping[builtins.str, builtins.str]]:
+        '''(experimental) Customized environment variables to send to titiler-pgstac runtime.
+
+        :stability: experimental
+        '''
+        result = self._values.get("api_env")
+        return typing.cast(typing.Optional[typing.Mapping[builtins.str, builtins.str]], result)
+
+    @builtins.property
+    def buckets(self) -> typing.Optional[typing.List[builtins.str]]:
+        '''(experimental) list of buckets the lambda will be granted access to.
+
+        :stability: experimental
+        '''
+        result = self._values.get("buckets")
+        return typing.cast(typing.Optional[typing.List[builtins.str]], result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "TitilerPgStacApiLambdaProps(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
+class TitilerPgstacApiLambda(
+    constructs.Construct,
+    metaclass=jsii.JSIIMeta,
+    jsii_type="cdk-pgstac.TitilerPgstacApiLambda",
+):
+    '''
+    :stability: experimental
+    '''
+
+    def __init__(
+        self,
+        scope: constructs.Construct,
+        id: builtins.str,
+        *,
+        db: aws_cdk.aws_rds.IDatabaseInstance,
+        db_secret: aws_cdk.aws_secretsmanager.ISecret,
+        subnet_selection: typing.Union[aws_cdk.aws_ec2.SubnetSelection, typing.Dict[str, typing.Any]],
+        vpc: aws_cdk.aws_ec2.IVpc,
+        api_env: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
+        buckets: typing.Optional[typing.Sequence[builtins.str]] = None,
+    ) -> None:
+        '''
+        :param scope: -
+        :param id: -
+        :param db: (experimental) RDS Instance with installed pgSTAC.
+        :param db_secret: (experimental) Secret containing connection information for pgSTAC database.
+        :param subnet_selection: (experimental) Subnet into which the lambda should be deployed.
+        :param vpc: (experimental) VPC into which the lambda should be deployed.
+        :param api_env: (experimental) Customized environment variables to send to titiler-pgstac runtime.
+        :param buckets: (experimental) list of buckets the lambda will be granted access to.
+
+        :stability: experimental
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(TitilerPgstacApiLambda.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+        props = TitilerPgStacApiLambdaProps(
+            db=db,
+            db_secret=db_secret,
+            subnet_selection=subnet_selection,
+            vpc=vpc,
+            api_env=api_env,
+            buckets=buckets,
+        )
+
+        jsii.create(self.__class__, self, [scope, id, props])
+
+    @builtins.property
+    @jsii.member(jsii_name="url")
+    def url(self) -> builtins.str:
+        '''
+        :stability: experimental
+        '''
+        return typing.cast(builtins.str, jsii.get(self, "url"))
+
+    @builtins.property
+    @jsii.member(jsii_name="titilerPgstacLambdaFunction")
+    def titiler_pgstac_lambda_function(self) -> aws_cdk.aws_lambda.Function:
+        '''
+        :stability: experimental
+        '''
+        return typing.cast(aws_cdk.aws_lambda.Function, jsii.get(self, "titilerPgstacLambdaFunction"))
+
+    @titiler_pgstac_lambda_function.setter
+    def titiler_pgstac_lambda_function(
+        self,
+        value: aws_cdk.aws_lambda.Function,
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(TitilerPgstacApiLambda, "titiler_pgstac_lambda_function").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "titilerPgstacLambdaFunction", value)
+
+
 __all__ = [
     "ApiEntrypoint",
     "BastionHost",
     "BastionHostProps",
     "BootstrapPgStac",
     "BootstrapPgStacProps",
     "DatabaseParameters",
     "PgStacApiLambda",
     "PgStacApiLambdaProps",
     "PgStacDatabase",
     "PgStacDatabaseProps",
     "StacIngestor",
     "StacIngestorProps",
+    "TitilerPgStacApiLambdaProps",
+    "TitilerPgstacApiLambda",
 ]
 
 publication.publish()
```

### Comparing `cdk-pgstac-4.1.0/src/cdk_pgstac.egg-info/PKG-INFO` & `cdk-pgstac-4.2.0/src/cdk_pgstac.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-pgstac
-Version: 4.1.0
+Version: 4.2.0
 Summary: A set of constructs deploying pgSTAC with CDK
 Home-page: https://github.com/developmentseed/cdk-pgstac.git
 Author: Anthony Lukach<anthony@developmentseed.org>
 License: ISC
 Project-URL: Source, https://github.com/developmentseed/cdk-pgstac.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

