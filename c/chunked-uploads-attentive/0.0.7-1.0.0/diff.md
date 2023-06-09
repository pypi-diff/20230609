# Comparing `tmp/chunked-uploads-attentive-0.0.7.tar.gz` & `tmp/chunked-uploads-attentive-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chunked-uploads-attentive-0.0.7.tar", last modified: Thu Jun  1 18:43:50 2023, max compression
+gzip compressed data, was "chunked-uploads-attentive-1.0.0.tar", last modified: Fri Jun  9 06:00:19 2023, max compression
```

## Comparing `chunked-uploads-attentive-0.0.7.tar` & `chunked-uploads-attentive-1.0.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 18:43:50.370589 chunked-uploads-attentive-0.0.7/
--rw-rw-rw-   0        0        0      478 2023-06-01 18:43:50.367601 chunked-uploads-attentive-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-01 18:43:50.370589 chunked-uploads-attentive-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      925 2023-06-01 18:42:49.000000 chunked-uploads-attentive-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-01 18:43:50.323598 chunked-uploads-attentive-0.0.7/src/
-drwxrwxrwx   0        0        0        0 2023-06-01 18:43:50.333603 chunked-uploads-attentive-0.0.7/src/chunked_uploads_attentive.egg-info/
--rw-rw-rw-   0        0        0      478 2023-06-01 18:43:50.000000 chunked-uploads-attentive-0.0.7/src/chunked_uploads_attentive.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      527 2023-06-01 18:43:50.000000 chunked-uploads-attentive-0.0.7/src/chunked_uploads_attentive.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 18:43:50.000000 chunked-uploads-attentive-0.0.7/src/chunked_uploads_attentive.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-06-01 18:43:50.000000 chunked-uploads-attentive-0.0.7/src/chunked_uploads_attentive.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-01 18:43:50.000000 chunked-uploads-attentive-0.0.7/src/chunked_uploads_attentive.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-01 18:43:50.363594 chunked-uploads-attentive-0.0.7/src/uploads/
--rw-rw-rw-   0        0        0        0 2023-03-21 15:09:06.000000 chunked-uploads-attentive-0.0.7/src/uploads/__init__.py
--rw-rw-rw-   0        0        0      325 2023-04-20 11:41:44.000000 chunked-uploads-attentive-0.0.7/src/uploads/admin.py
--rw-rw-rw-   0        0        0      152 2023-04-20 11:41:44.000000 chunked-uploads-attentive-0.0.7/src/uploads/apps.py
--rw-rw-rw-   0        0        0      300 2023-04-20 11:41:44.000000 chunked-uploads-attentive-0.0.7/src/uploads/constants.py
--rw-rw-rw-   0        0        0      262 2023-02-13 12:36:18.000000 chunked-uploads-attentive-0.0.7/src/uploads/exceptions.py
--rw-rw-rw-   0        0        0     3853 2023-05-07 19:41:00.000000 chunked-uploads-attentive-0.0.7/src/uploads/models.py
--rw-rw-rw-   0        0        0      384 2023-04-20 11:41:44.000000 chunked-uploads-attentive-0.0.7/src/uploads/response.py
--rw-rw-rw-   0        0        0      578 2023-04-20 11:41:44.000000 chunked-uploads-attentive-0.0.7/src/uploads/serializers.py
--rw-rw-rw-   0        0        0     2750 2023-05-31 05:22:56.000000 chunked-uploads-attentive-0.0.7/src/uploads/settings.py
--rw-rw-rw-   0        0        0       63 2023-03-21 15:09:06.000000 chunked-uploads-attentive-0.0.7/src/uploads/tests.py
--rw-rw-rw-   0        0        0    12316 2023-05-31 05:23:58.000000 chunked-uploads-attentive-0.0.7/src/uploads/views.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:00:19.428584 chunked-uploads-attentive-1.0.0/
+-rw-rw-rw-   0        0        0      478 2023-06-09 06:00:19.426594 chunked-uploads-attentive-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-09 06:00:19.428584 chunked-uploads-attentive-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      925 2023-06-09 05:58:34.000000 chunked-uploads-attentive-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:00:19.389583 chunked-uploads-attentive-1.0.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-09 06:00:19.401583 chunked-uploads-attentive-1.0.0/src/chunked_uploads_attentive.egg-info/
+-rw-rw-rw-   0        0        0      478 2023-06-09 06:00:19.000000 chunked-uploads-attentive-1.0.0/src/chunked_uploads_attentive.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      527 2023-06-09 06:00:19.000000 chunked-uploads-attentive-1.0.0/src/chunked_uploads_attentive.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 06:00:19.000000 chunked-uploads-attentive-1.0.0/src/chunked_uploads_attentive.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-06-09 06:00:19.000000 chunked-uploads-attentive-1.0.0/src/chunked_uploads_attentive.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-09 06:00:19.000000 chunked-uploads-attentive-1.0.0/src/chunked_uploads_attentive.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 06:00:19.424583 chunked-uploads-attentive-1.0.0/src/uploads/
+-rw-rw-rw-   0        0        0        0 2023-03-21 15:09:06.000000 chunked-uploads-attentive-1.0.0/src/uploads/__init__.py
+-rw-rw-rw-   0        0        0      325 2023-04-20 11:41:44.000000 chunked-uploads-attentive-1.0.0/src/uploads/admin.py
+-rw-rw-rw-   0        0        0      152 2023-04-20 11:41:44.000000 chunked-uploads-attentive-1.0.0/src/uploads/apps.py
+-rw-rw-rw-   0        0        0      300 2023-04-20 11:41:44.000000 chunked-uploads-attentive-1.0.0/src/uploads/constants.py
+-rw-rw-rw-   0        0        0      262 2023-02-13 12:36:18.000000 chunked-uploads-attentive-1.0.0/src/uploads/exceptions.py
+-rw-rw-rw-   0        0        0     3532 2023-06-09 05:47:04.000000 chunked-uploads-attentive-1.0.0/src/uploads/models.py
+-rw-rw-rw-   0        0        0      384 2023-04-20 11:41:44.000000 chunked-uploads-attentive-1.0.0/src/uploads/response.py
+-rw-rw-rw-   0        0        0      578 2023-04-20 11:41:44.000000 chunked-uploads-attentive-1.0.0/src/uploads/serializers.py
+-rw-rw-rw-   0        0        0     2750 2023-05-31 05:22:56.000000 chunked-uploads-attentive-1.0.0/src/uploads/settings.py
+-rw-rw-rw-   0        0        0       63 2023-03-21 15:09:06.000000 chunked-uploads-attentive-1.0.0/src/uploads/tests.py
+-rw-rw-rw-   0        0        0    12316 2023-05-31 05:23:58.000000 chunked-uploads-attentive-1.0.0/src/uploads/views.py
```

### Comparing `chunked-uploads-attentive-0.0.7/setup.py` & `chunked-uploads-attentive-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.7'
+VERSION = '1.0.0'
 DESCRIPTION = 'Chunked Upload of files on gcs using Django'
 LONG_DESCRIPTION = 'A package that allows to transfer files and resume in case of data failure'
 
 # Setting up
 setup(
     name="chunked-uploads-attentive",
     version=VERSION,
```

### Comparing `chunked-uploads-attentive-0.0.7/src/chunked_uploads_attentive.egg-info/SOURCES.txt` & `chunked-uploads-attentive-1.0.0/src/chunked_uploads_attentive.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chunked-uploads-attentive-0.0.7/src/uploads/models.py` & `chunked-uploads-attentive-1.0.0/src/uploads/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import hashlib
 import uuid
 
 from django.db import models
 from django.conf import settings
 from django.core.files.uploadedfile import UploadedFile
 from django.utils import timezone
-from google.cloud import storage
 
 from .settings import (
     EXPIRATION_DELTA,
     UPLOAD_TO,
     STORAGE,
     DEFAULT_MODEL_USER_FIELD_NULL,
     DEFAULT_MODEL_USER_FIELD_BLANK,
@@ -62,21 +61,14 @@
         if getattr(self, "_md5", None) is None:
             md5 = hashlib.md5()
             for chunk in self.file.chunks():
                 md5.update(chunk)
             self._md5 = md5.hexdigest()
         return self._md5
 
-    def delete(self, delete_file=True, *args, **kwargs):
-        if self.file:
-            storage, path = self.file.storage, self.file.path
-        super(AbstractChunkedUpload, self).delete(*args, **kwargs)
-        if self.file and delete_file:
-            storage.delete(path)
-
     def __str__(self):
         return "<%s - upload_id: %s - bytes: %s - status: %s>" % (
             self.filename,
             self.upload_id,
             self.offset,
             self.status,
         )
```

### Comparing `chunked-uploads-attentive-0.0.7/src/uploads/serializers.py` & `chunked-uploads-attentive-1.0.0/src/uploads/serializers.py`

 * *Files identical despite different names*

### Comparing `chunked-uploads-attentive-0.0.7/src/uploads/settings.py` & `chunked-uploads-attentive-1.0.0/src/uploads/settings.py`

 * *Files identical despite different names*

### Comparing `chunked-uploads-attentive-0.0.7/src/uploads/views.py` & `chunked-uploads-attentive-1.0.0/src/uploads/views.py`

 * *Files identical despite different names*

