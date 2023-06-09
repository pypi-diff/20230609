# Comparing `tmp/awstuff-0.21.tar.gz` & `tmp/awstuff-0.211.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awstuff-0.21.tar", last modified: Thu Jun  8 20:52:09 2023, max compression
+gzip compressed data, was "awstuff-0.211.tar", last modified: Fri Jun  9 00:44:34 2023, max compression
```

## Comparing `awstuff-0.21.tar` & `awstuff-0.211.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 20:52:09.077214 awstuff-0.21/
--rw-rw-rw-   0        0        0      237 2023-06-08 20:52:09.077214 awstuff-0.21/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-08 20:52:09.059214 awstuff-0.21/awstuff/
--rw-rw-rw-   0        0        0     4911 2023-06-08 20:40:31.000000 awstuff-0.21/awstuff/Functions.py
--rw-rw-rw-   0        0        0       33 2023-05-17 00:29:39.000000 awstuff-0.21/awstuff/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-08 20:52:09.076212 awstuff-0.21/awstuff.egg-info/
--rw-rw-rw-   0        0        0      237 2023-06-08 20:52:08.000000 awstuff-0.21/awstuff.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      213 2023-06-08 20:52:09.000000 awstuff-0.21/awstuff.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 20:52:08.000000 awstuff-0.21/awstuff.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 16:50:18.000000 awstuff-0.21/awstuff.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        8 2023-06-08 20:52:08.000000 awstuff-0.21/awstuff.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-08 20:52:09.079212 awstuff-0.21/setup.cfg
--rw-rw-rw-   0        0        0      256 2023-06-08 20:51:09.000000 awstuff-0.21/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 00:44:34.245024 awstuff-0.211/
+-rw-rw-rw-   0        0        0      238 2023-06-09 00:44:34.245024 awstuff-0.211/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-09 00:44:34.231022 awstuff-0.211/awstuff/
+-rw-rw-rw-   0        0        0     4869 2023-06-08 20:59:31.000000 awstuff-0.211/awstuff/Functions.py
+-rw-rw-rw-   0        0        0       33 2023-05-17 00:29:39.000000 awstuff-0.211/awstuff/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 00:44:34.244025 awstuff-0.211/awstuff.egg-info/
+-rw-rw-rw-   0        0        0      238 2023-06-09 00:44:34.000000 awstuff-0.211/awstuff.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      213 2023-06-09 00:44:34.000000 awstuff-0.211/awstuff.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 00:44:34.000000 awstuff-0.211/awstuff.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 16:50:18.000000 awstuff-0.211/awstuff.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        8 2023-06-09 00:44:34.000000 awstuff-0.211/awstuff.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-09 00:44:34.247023 awstuff-0.211/setup.cfg
+-rw-rw-rw-   0        0        0      257 2023-06-09 00:44:05.000000 awstuff-0.211/setup.py
```

### Comparing `awstuff-0.21/awstuff/Functions.py` & `awstuff-0.211/awstuff/Functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 import boto3
 import botocore
 import os
 import sys
 import yaml
-import csv
-import json
-from typing import List
 
 class Functions:
     """ Helper functions for interacting with AWS"""
 
 
     def parse_yaml(file):
         """Exposes configuration YAML file
@@ -36,14 +33,15 @@
         """
         try:
             return boto3.resource("s3")
         except Exception as e:
             print(f"Can't connect to S3. Error: {e}")
             sys.exit(1)
 
+
     def assure_s3_bucket(s3, bckt):
         """Check if bucket exists and create if not
 
         Args:
             s3 (boto3 resource): boto3 S3 resource
             bckt (S3 bucket): S3 bucket
         """
@@ -53,15 +51,16 @@
         except botocore.exceptions.ClientError as e:
             print(f'Error code: {e}')
             if e.response["Error"]["Code"] == "404":
                 print ('Bucket failed head_bucket() call, likely does not exist')
                 s3.create_bucket(Bucket = bckt)
                 print(f'Created {bckt}')
 
-    def diff_bucket_objs(s3, bucket_1, prefix_1, bucket_2, prefix_2, match_extensions=True):
+
+    def diff_bucket_objs(s3, bucket_1, prefix_1, bucket_2, prefix_2, match_extensions=False):
         """Identifies the objects in bucket_1 that are not in bucket_2 by key including prefix and extension
 
         Args:
             s3 (boto3 resource): boto3 S3 resource
             bucket_1 (S3 bucket): 1st S3 bucket
             prefix_1 (String): prefix for objects in bucket 1
             bucket_2 (S3 bucket): 2nd S3 bucket
@@ -108,14 +107,15 @@
         
         for key, result in zip(objects, results):
             if result['ResponseMetadata']['HTTPStatusCode'] == 200:
                 print(f'Copied over: {key}')
         
         print(f'Copying complete, {dest_prefix} folder on destination bucket updated. {ct} objects copied over.')
 
+
     def search_s3_bucket_contents(s3_client, bucket_name, search_term):
         """Searches for a given search term in the contents of an S3 bucket.
 
         Args:
             bucket_name (str): The name of the S3 bucket to search.
             search_term (str): The term to search for in the bucket contents.
 
@@ -126,7 +126,8 @@
             object_key = obj['Key']
             response = s3_client.get_object(Bucket=bucket_name, Key=object_key)
             content = response['Body'].read().decode('utf-8')  # Assuming text content, adjust decoding based on content type
 
             if search_term in content:
                 print(f"Found '{search_term}' in object: {object_key}")
                 break
+
```

