# Comparing `tmp/ns_lab_aws-23.6.9.tar.gz` & `tmp/ns_lab_aws-23.6.9.post1248.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ns_lab_aws-23.6.9.tar", last modified: Fri Jun  9 09:27:12 2023, max compression
+gzip compressed data, was "ns_lab_aws-23.6.9.post1248.tar", last modified: Fri Jun  9 10:46:48 2023, max compression
```

## Comparing `ns_lab_aws-23.6.9.tar` & `ns_lab_aws-23.6.9.post1248.tar`

### file list

```diff
@@ -1,27 +1,30 @@
-drwxr-xr-x   0 salavat    (501) staff       (20)        0 2023-06-09 09:27:12.055778 ns_lab_aws-23.6.9/
--rw-r--r--   0 salavat    (501) staff       (20)     4527 2023-06-09 09:27:12.055634 ns_lab_aws-23.6.9/PKG-INFO
--rw-r--r--   0 salavat    (501) staff       (20)     4055 2023-06-09 08:55:20.000000 ns_lab_aws-23.6.9/README.md
-drwxr-xr-x   0 salavat    (501) staff       (20)        0 2023-06-09 09:27:12.052905 ns_lab_aws-23.6.9/ns_lab_aws/
--rw-r--r--   0 salavat    (501) staff       (20)        0 2023-06-09 09:07:59.000000 ns_lab_aws-23.6.9/ns_lab_aws/__init__.py
--rw-r--r--   0 salavat    (501) staff       (20)      653 2023-06-09 09:13:32.000000 ns_lab_aws-23.6.9/ns_lab_aws/manager.py
-drwxr-xr-x   0 salavat    (501) staff       (20)        0 2023-06-09 09:27:12.054050 ns_lab_aws-23.6.9/ns_lab_aws/ns_aws/
--rw-r--r--   0 salavat    (501) staff       (20)        0 2023-06-06 18:43:17.000000 ns_lab_aws-23.6.9/ns_lab_aws/ns_aws/__init__.py
--rw-r--r--   0 salavat    (501) staff       (20)     9073 2023-06-09 09:10:40.000000 ns_lab_aws-23.6.9/ns_lab_aws/ns_aws/s3buckets.py
-drwxr-xr-x   0 salavat    (501) staff       (20)        0 2023-06-09 09:27:12.054707 ns_lab_aws-23.6.9/ns_lab_aws/ns_config/
--rw-r--r--   0 salavat    (501) staff       (20)        0 2023-06-06 18:44:36.000000 ns_lab_aws-23.6.9/ns_lab_aws/ns_config/__init__.py
--rw-r--r--   0 salavat    (501) staff       (20)      375 2023-06-07 17:04:22.000000 ns_lab_aws-23.6.9/ns_lab_aws/ns_config/libraries.py
--rw-r--r--   0 salavat    (501) staff       (20)     2931 2023-06-09 09:10:51.000000 ns_lab_aws-23.6.9/ns_lab_aws/ns_config/settings.py
-drwxr-xr-x   0 salavat    (501) staff       (20)        0 2023-06-09 09:27:12.055030 ns_lab_aws-23.6.9/ns_lab_aws/ns_console/
--rw-r--r--   0 salavat    (501) staff       (20)        0 2023-06-09 09:07:36.000000 ns_lab_aws-23.6.9/ns_lab_aws/ns_console/__init__.py
--rw-r--r--   0 salavat    (501) staff       (20)     3220 2023-06-09 09:10:45.000000 ns_lab_aws-23.6.9/ns_lab_aws/ns_console/client.py
-drwxr-xr-x   0 salavat    (501) staff       (20)        0 2023-06-09 09:27:12.055353 ns_lab_aws-23.6.9/ns_lab_aws/ns_converter/
--rw-r--r--   0 salavat    (501) staff       (20)        0 2023-06-07 10:54:42.000000 ns_lab_aws-23.6.9/ns_lab_aws/ns_converter/__init__.py
--rw-r--r--   0 salavat    (501) staff       (20)      237 2023-06-07 11:08:18.000000 ns_lab_aws-23.6.9/ns_lab_aws/ns_converter/converter.py
-drwxr-xr-x   0 salavat    (501) staff       (20)        0 2023-06-09 09:27:12.053772 ns_lab_aws-23.6.9/ns_lab_aws.egg-info/
--rw-r--r--   0 salavat    (501) staff       (20)     4527 2023-06-09 09:27:12.000000 ns_lab_aws-23.6.9/ns_lab_aws.egg-info/PKG-INFO
--rw-r--r--   0 salavat    (501) staff       (20)      538 2023-06-09 09:27:12.000000 ns_lab_aws-23.6.9/ns_lab_aws.egg-info/SOURCES.txt
--rw-r--r--   0 salavat    (501) staff       (20)        1 2023-06-09 09:27:12.000000 ns_lab_aws-23.6.9/ns_lab_aws.egg-info/dependency_links.txt
--rw-r--r--   0 salavat    (501) staff       (20)      223 2023-06-09 09:27:12.000000 ns_lab_aws-23.6.9/ns_lab_aws.egg-info/requires.txt
--rw-r--r--   0 salavat    (501) staff       (20)       11 2023-06-09 09:27:12.000000 ns_lab_aws-23.6.9/ns_lab_aws.egg-info/top_level.txt
--rw-r--r--   0 salavat    (501) staff       (20)      913 2023-06-09 09:24:53.000000 ns_lab_aws-23.6.9/pyproject.toml
--rw-r--r--   0 salavat    (501) staff       (20)       38 2023-06-09 09:27:12.055823 ns_lab_aws-23.6.9/setup.cfg
+drwxr-xr-x   0 salavat    (501) staff       (20)        0 2023-06-09 10:46:48.744837 ns_lab_aws-23.6.9.post1248/
+-rw-r--r--   0 salavat    (501) staff       (20)     4536 2023-06-09 10:46:48.744673 ns_lab_aws-23.6.9.post1248/PKG-INFO
+-rw-r--r--   0 salavat    (501) staff       (20)     4055 2023-06-09 08:55:20.000000 ns_lab_aws-23.6.9.post1248/README.md
+drwxr-xr-x   0 salavat    (501) staff       (20)        0 2023-06-09 10:46:48.740772 ns_lab_aws-23.6.9.post1248/ns_lab_aws/
+-rw-r--r--   0 salavat    (501) staff       (20)        0 2023-06-09 09:07:59.000000 ns_lab_aws-23.6.9.post1248/ns_lab_aws/__init__.py
+drwxr-xr-x   0 salavat    (501) staff       (20)        0 2023-06-09 10:46:48.743166 ns_lab_aws-23.6.9.post1248/ns_lab_aws/config/
+-rw-r--r--   0 salavat    (501) staff       (20)        0 2023-06-06 18:44:36.000000 ns_lab_aws-23.6.9.post1248/ns_lab_aws/config/__init__.py
+-rw-r--r--   0 salavat    (501) staff       (20)       89 2023-06-09 10:25:47.000000 ns_lab_aws-23.6.9.post1248/ns_lab_aws/config/environment.py
+-rw-r--r--   0 salavat    (501) staff       (20)      375 2023-06-07 17:04:22.000000 ns_lab_aws-23.6.9.post1248/ns_lab_aws/config/libraries.py
+-rw-r--r--   0 salavat    (501) staff       (20)      431 2023-06-09 10:23:04.000000 ns_lab_aws-23.6.9.post1248/ns_lab_aws/config/logging.py
+-rw-r--r--   0 salavat    (501) staff       (20)     2753 2023-06-09 10:40:40.000000 ns_lab_aws-23.6.9.post1248/ns_lab_aws/config/settings.py
+drwxr-xr-x   0 salavat    (501) staff       (20)        0 2023-06-09 10:46:48.743513 ns_lab_aws-23.6.9.post1248/ns_lab_aws/console/
+-rw-r--r--   0 salavat    (501) staff       (20)        0 2023-06-09 09:07:36.000000 ns_lab_aws-23.6.9.post1248/ns_lab_aws/console/__init__.py
+-rw-r--r--   0 salavat    (501) staff       (20)     2547 2023-06-09 09:57:29.000000 ns_lab_aws-23.6.9.post1248/ns_lab_aws/console/client.py
+drwxr-xr-x   0 salavat    (501) staff       (20)        0 2023-06-09 10:46:48.743871 ns_lab_aws-23.6.9.post1248/ns_lab_aws/converter/
+-rw-r--r--   0 salavat    (501) staff       (20)        0 2023-06-07 10:54:42.000000 ns_lab_aws-23.6.9.post1248/ns_lab_aws/converter/__init__.py
+-rw-r--r--   0 salavat    (501) staff       (20)      237 2023-06-07 11:08:18.000000 ns_lab_aws-23.6.9.post1248/ns_lab_aws/converter/converter.py
+-rw-r--r--   0 salavat    (501) staff       (20)      862 2023-06-09 10:29:29.000000 ns_lab_aws-23.6.9.post1248/ns_lab_aws/init.py
+-rw-r--r--   0 salavat    (501) staff       (20)      648 2023-06-09 09:54:04.000000 ns_lab_aws-23.6.9.post1248/ns_lab_aws/manager.py
+drwxr-xr-x   0 salavat    (501) staff       (20)        0 2023-06-09 10:46:48.744290 ns_lab_aws-23.6.9.post1248/ns_lab_aws/services/
+-rw-r--r--   0 salavat    (501) staff       (20)        0 2023-06-06 18:43:17.000000 ns_lab_aws-23.6.9.post1248/ns_lab_aws/services/__init__.py
+-rw-r--r--   0 salavat    (501) staff       (20)     9043 2023-06-09 09:55:59.000000 ns_lab_aws-23.6.9.post1248/ns_lab_aws/services/s3buckets.py
+drwxr-xr-x   0 salavat    (501) staff       (20)        0 2023-06-09 10:46:48.742054 ns_lab_aws-23.6.9.post1248/ns_lab_aws.egg-info/
+-rw-r--r--   0 salavat    (501) staff       (20)     4536 2023-06-09 10:46:48.000000 ns_lab_aws-23.6.9.post1248/ns_lab_aws.egg-info/PKG-INFO
+-rw-r--r--   0 salavat    (501) staff       (20)      602 2023-06-09 10:46:48.000000 ns_lab_aws-23.6.9.post1248/ns_lab_aws.egg-info/SOURCES.txt
+-rw-r--r--   0 salavat    (501) staff       (20)        1 2023-06-09 10:46:48.000000 ns_lab_aws-23.6.9.post1248/ns_lab_aws.egg-info/dependency_links.txt
+-rw-r--r--   0 salavat    (501) staff       (20)      223 2023-06-09 10:46:48.000000 ns_lab_aws-23.6.9.post1248/ns_lab_aws.egg-info/requires.txt
+-rw-r--r--   0 salavat    (501) staff       (20)       11 2023-06-09 10:46:48.000000 ns_lab_aws-23.6.9.post1248/ns_lab_aws.egg-info/top_level.txt
+-rw-r--r--   0 salavat    (501) staff       (20)      918 2023-06-09 09:49:13.000000 ns_lab_aws-23.6.9.post1248/pyproject.toml
+-rw-r--r--   0 salavat    (501) staff       (20)       38 2023-06-09 10:46:48.744891 ns_lab_aws-23.6.9.post1248/setup.cfg
```

### Comparing `ns_lab_aws-23.6.9/PKG-INFO` & `ns_lab_aws-23.6.9.post1248/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ns_lab_aws
-Version: 23.6.9
+Version: 23.6.9.post1248
 Summary: AWS Console Tool
 Author-email: Salavat Nigmatullin <salavat@nigmatullin.net>
 Project-URL: Homepage, https://github.com/salavatn/Python/tree/main/AWS
 Project-URL: Documentation, https://github.com/salavatn/Python/blob/main/AWS/README.md
 Project-URL: Changes, https://github.com/salavatn/Python/commits/main/AWS/README.md
 Keywords: aws,s3 bucket
 Requires-Python: >=3.8
```

### Comparing `ns_lab_aws-23.6.9/README.md` & `ns_lab_aws-23.6.9.post1248/README.md`

 * *Files identical despite different names*

### Comparing `ns_lab_aws-23.6.9/ns_lab_aws/manager.py` & `ns_lab_aws-23.6.9.post1248/ns_lab_aws/manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-from ns_lab_aws.ns_console.client import S3Client 
-from ns_lab_aws.ns_config.settings import logger, s3_parser
+from ns_lab_aws.console.client import S3Client 
+from ns_lab_aws.config.settings import logger, s3_parser
 
 
 s3_client = S3Client()
 
 
 args        = s3_parser.parse_args()
 s3_list     = args.list
 s3_create   = args.create
 s3_delete   = args.delete
 s3_bucket   = args.bucket
 s3_force    = args.force
 s3_content  = args.content
 s3_file     = args.file
 
+
 if s3_list:    
     s3_client.s3_bucket_list()
 
 if s3_delete:
     s3_client.s3_bucket_delete(s3_bucket, s3_force)
 
 if s3_content:
```

### Comparing `ns_lab_aws-23.6.9/ns_lab_aws/ns_aws/s3buckets.py` & `ns_lab_aws-23.6.9.post1248/ns_lab_aws/services/s3buckets.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-from ns_lab_aws.ns_converter.converter import convert_bytes
-from ns_lab_aws.ns_config.settings import aws_session, aws_region
-from ns_lab_aws.ns_config.settings import logger
-from ns_lab_aws.ns_config.libraries import List, Union, Dict, Any
-from ns_lab_aws.ns_config.libraries import print
-from ns_lab_aws.ns_config.libraries import threading, os
-
-import time
+from ns_lab_aws.converter.converter import convert_bytes
+from ns_lab_aws.config.settings import aws_session, aws_region
+from ns_lab_aws.config.settings import logger
+from ns_lab_aws.config.libraries import List, Union, Dict, Any
+from ns_lab_aws.config.libraries import print
+from ns_lab_aws.config.libraries import threading, os 
 
 
 logger = logger.getLogger('NS_AWS:S3Buckets')
 
 
 class S3Buckets:
     '''Class for AWS S3 buckets'''
```

### Comparing `ns_lab_aws-23.6.9/ns_lab_aws/ns_config/settings.py` & `ns_lab_aws-23.6.9.post1248/ns_lab_aws/config/settings.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,13 @@
-from ns_lab_aws.ns_config.libraries import load_dotenv
-from ns_lab_aws.ns_config.libraries import os
-from ns_lab_aws.ns_config.libraries import boto3 
-from ns_lab_aws.ns_config.libraries import logging, logging_config, colorlog
-from ns_lab_aws.ns_config.libraries import Console, Table, box
-from ns_lab_aws.ns_config.libraries import argparse
-
-# from ns_config.libraries import Console, Table, box
-# from ns_config.libraries import pytz, datetime
-# from ns_config.libraries import Faker
+from ns_lab_aws.config.libraries import load_dotenv
+from ns_lab_aws.config.libraries import os
+from ns_lab_aws.config.libraries import boto3  
+from ns_lab_aws.config.libraries import logging, logging_config, colorlog
+from ns_lab_aws.config.libraries import Console, Table, box
+from ns_lab_aws.config.libraries import argparse
 
 
 # Setting-1: Load environment variables
 load_env = load_dotenv(dotenv_path='.env')
 
 
 # Setting-2: Load AWS credentials and create AWS Session
@@ -19,15 +15,15 @@
 aws_secret  = os.getenv('AWS_SECRET')
 aws_region  = os.getenv('AWS_REGION')
 aws_params  = {
     'aws_access_key_id':     aws_access,
     'aws_secret_access_key': aws_secret,
     'region_name':           aws_region
 }
-print(aws_params)
+
 aws_session = boto3.Session(**aws_params)
 
 
 # Setting-3: Logging
 logging_config.fileConfig('logging.conf')
 logger = logging
```

### Comparing `ns_lab_aws-23.6.9/ns_lab_aws/ns_console/client.py` & `ns_lab_aws-23.6.9.post1248/ns_lab_aws/console/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from ns_lab_aws.ns_aws.s3buckets import S3Buckets
-from ns_lab_aws.ns_config.settings import table_buckets, table_files, console
-from ns_lab_aws.ns_config.settings import s3_parser
-from ns_lab_aws.ns_config.settings import logger
+from ns_lab_aws.services.s3buckets import S3Buckets
+from ns_lab_aws.config.settings import table_buckets, table_files, console
+from ns_lab_aws.config.settings import s3_parser
+from ns_lab_aws.config.settings import logger
 from rich import print
 
 from rich.tree import Tree
 
 
 # logger = logger.getLogger(__name__)
 logger = logger.getLogger('NS_CONSOLE:Client')
-import time
+
 
 
 class S3Client:
     def __init__(self):
         self.s3_buckets = S3Buckets()
 
     def s3_bucket_list(self) -> None:
@@ -79,44 +79,7 @@
     def s3_bucket_create(self, bucket_name):
         self.s3_buckets.create_bucket(bucket_name)
 
     def s3_bucket_upload(self, bucket_name, file_path):
         # file_name = 'my_pdf_document.pdf'
         self.s3_buckets.upload_file(bucket_name, file_path)
 
-
-# args        = s3_parser.parse_args()
-# s3_list     = args.list
-# s3_create   = args.create
-# s3_delete   = args.delete
-# s3_bucket   = args.bucket
-# s3_force    = args.force
-# s3_content  = args.content
-# s3_file     = args.file
-
-# if s3_list:    
-#     s3_bucket_list()
-
-# if s3_delete:
-#     s3_bucket_delete(s3_bucket, s3_force)
-
-# if s3_content:
-#     s3_bucket_content(s3_bucket)
-
-# if s3_create:
-#     s3_bucket_create(s3_bucket)
-
-
-# if s3_file:
-#     print('File:', s3_file)
-#     print('Bucket:', s3_bucket)
-#     print('Force:', s3_force)
-#     s3_bucket_upload(s3_bucket, s3_file)
-
-
-
-
-
-
-
-
-# webapp2-dev-serverlessdeploymentbucket-j4yn3xoell07
```

### Comparing `ns_lab_aws-23.6.9/ns_lab_aws.egg-info/PKG-INFO` & `ns_lab_aws-23.6.9.post1248/ns_lab_aws.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ns-lab-aws
-Version: 23.6.9
+Version: 23.6.9.post1248
 Summary: AWS Console Tool
 Author-email: Salavat Nigmatullin <salavat@nigmatullin.net>
 Project-URL: Homepage, https://github.com/salavatn/Python/tree/main/AWS
 Project-URL: Documentation, https://github.com/salavatn/Python/blob/main/AWS/README.md
 Project-URL: Changes, https://github.com/salavatn/Python/commits/main/AWS/README.md
 Keywords: aws,s3 bucket
 Requires-Python: >=3.8
```

### Comparing `ns_lab_aws-23.6.9/ns_lab_aws.egg-info/SOURCES.txt` & `ns_lab_aws-23.6.9.post1248/ns_lab_aws.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 README.md
 pyproject.toml
 ns_lab_aws/__init__.py
+ns_lab_aws/init.py
 ns_lab_aws/manager.py
 ns_lab_aws.egg-info/PKG-INFO
 ns_lab_aws.egg-info/SOURCES.txt
 ns_lab_aws.egg-info/dependency_links.txt
 ns_lab_aws.egg-info/requires.txt
 ns_lab_aws.egg-info/top_level.txt
-ns_lab_aws/ns_aws/__init__.py
-ns_lab_aws/ns_aws/s3buckets.py
-ns_lab_aws/ns_config/__init__.py
-ns_lab_aws/ns_config/libraries.py
-ns_lab_aws/ns_config/settings.py
-ns_lab_aws/ns_console/__init__.py
-ns_lab_aws/ns_console/client.py
-ns_lab_aws/ns_converter/__init__.py
-ns_lab_aws/ns_converter/converter.py
+ns_lab_aws/config/__init__.py
+ns_lab_aws/config/environment.py
+ns_lab_aws/config/libraries.py
+ns_lab_aws/config/logging.py
+ns_lab_aws/config/settings.py
+ns_lab_aws/console/__init__.py
+ns_lab_aws/console/client.py
+ns_lab_aws/converter/__init__.py
+ns_lab_aws/converter/converter.py
+ns_lab_aws/services/__init__.py
+ns_lab_aws/services/s3buckets.py
```

### Comparing `ns_lab_aws-23.6.9/pyproject.toml` & `ns_lab_aws-23.6.9.post1248/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ns_lab_aws"
-version = "23.06.09"
+version = "23.06.09-1248"
 description = "AWS Console Tool"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["aws", "s3 bucket"]
 dependencies = [
     "boto3==1.26.147",
     "botocore==1.29.147",
```

