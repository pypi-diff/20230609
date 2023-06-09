# Comparing `tmp/latch_aws-0.1.0.tar.gz` & `tmp/latch_aws-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latch_aws-0.1.0.tar", max compression
+gzip compressed data, was "latch_aws-0.1.1.tar", max compression
```

## Comparing `latch_aws-0.1.0.tar` & `latch_aws-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     7052 2023-05-31 20:53:02.454014 latch_aws-0.1.0/LICENSE
--rw-r--r--   0        0        0       13 2023-05-31 20:53:27.998551 latch_aws-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-05-31 20:53:02.473001 latch_aws-0.1.0/latch_aws/__init__.py
--rw-r--r--   0        0        0     9677 2023-05-31 20:59:03.645324 latch_aws-0.1.0/latch_aws/aws.py
--rw-r--r--   0        0        0        0 2023-05-31 20:53:02.473127 latch_aws-0.1.0/latch_aws/py.typed
--rw-r--r--   0        0        0     1264 2023-05-31 20:59:18.208850 latch_aws-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      785 1970-01-01 00:00:00.000000 latch_aws-0.1.0/setup.py
--rw-r--r--   0        0        0      641 1970-01-01 00:00:00.000000 latch_aws-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     7052 2023-05-31 20:53:02.454014 latch_aws-0.1.1/LICENSE
+-rw-r--r--   0        0        0       13 2023-05-31 20:53:27.998551 latch_aws-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 20:53:02.473001 latch_aws-0.1.1/latch_aws/__init__.py
+-rw-r--r--   0        0        0     9677 2023-06-09 18:38:21.628052 latch_aws-0.1.1/latch_aws/aws.py
+-rw-r--r--   0        0        0     1082 2023-06-09 18:39:00.979163 latch_aws-0.1.1/latch_aws/client_pool.py
+-rw-r--r--   0        0        0        0 2023-05-31 20:53:02.473127 latch_aws-0.1.1/latch_aws/py.typed
+-rw-r--r--   0        0        0     1264 2023-06-09 18:39:42.103862 latch_aws-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      785 1970-01-01 00:00:00.000000 latch_aws-0.1.1/setup.py
+-rw-r--r--   0        0        0      641 1970-01-01 00:00:00.000000 latch_aws-0.1.1/PKG-INFO
```

### Comparing `latch_aws-0.1.0/LICENSE` & `latch_aws-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `latch_aws-0.1.0/latch_aws/aws.py` & `latch_aws-0.1.1/latch_aws/aws.py`

 * *Files identical despite different names*

### Comparing `latch_aws-0.1.0/pyproject.toml` & `latch_aws-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "latch-aws"
-version = "0.1.0"
+version = "0.1.1"
 description = "Traced and managed aws resources"
 authors = ["Max Smolin <max@latch.bio>"]
 license = "CC0 1.0"
 readme = "README.md"
 packages = [{include = "latch_aws"}]
 
 [tool.poetry.dependencies]
```

### Comparing `latch_aws-0.1.0/setup.py` & `latch_aws-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
  'latch-data-validation>=0.1.3,<0.2.0',
  'latch-o11y>=0.1.4,<0.2.0',
  'opentelemetry-sdk>=1.15.0,<2.0.0',
  'types-aiobotocore[s3]>=2.4.2,<3.0.0']
 
 setup_kwargs = {
     'name': 'latch-aws',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'Traced and managed aws resources',
     'long_description': '# python-aws\n',
     'author': 'Max Smolin',
     'author_email': 'max@latch.bio',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `latch_aws-0.1.0/PKG-INFO` & `latch_aws-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: latch-aws
-Version: 0.1.0
+Version: 0.1.1
 Summary: Traced and managed aws resources
 License: CC0 1.0
 Author: Max Smolin
 Author-email: max@latch.bio
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

