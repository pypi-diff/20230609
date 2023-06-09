# Comparing `tmp/cloudvault-1.1.tar.gz` & `tmp/cloudvault-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudvault-1.1.tar", last modified: Fri Jun  9 02:02:54 2023, max compression
+gzip compressed data, was "cloudvault-1.2.tar", last modified: Fri Jun  9 10:39:38 2023, max compression
```

## Comparing `cloudvault-1.1.tar` & `cloudvault-1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-09 02:02:54.909027 cloudvault-1.1/
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     1073 2023-06-09 00:48:41.000000 cloudvault-1.1/LICENSE
--rw-------   0 u0_a269  (10269) u0_a269  (10269)       35 2023-06-09 00:40:39.000000 cloudvault-1.1/MANIFEST.in
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     1836 2023-06-09 02:02:54.912360 cloudvault-1.1/PKG-INFO
--rw-------   0 u0_a269  (10269) u0_a269  (10269)      764 2023-06-09 01:49:53.000000 cloudvault-1.1/README.md
-drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-09 02:02:54.895694 cloudvault-1.1/cloudvault/
--rw-------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-09 00:15:52.000000 cloudvault-1.1/cloudvault/__init__.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     1110 2023-06-08 23:24:22.000000 cloudvault-1.1/cloudvault/cloud_storage.py
-drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-09 02:02:54.909027 cloudvault-1.1/cloudvault.egg-info/
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     1836 2023-06-09 02:02:53.000000 cloudvault-1.1/cloudvault.egg-info/PKG-INFO
--rw-------   0 u0_a269  (10269) u0_a269  (10269)      283 2023-06-09 02:02:54.000000 cloudvault-1.1/cloudvault.egg-info/SOURCES.txt
--rw-------   0 u0_a269  (10269) u0_a269  (10269)        1 2023-06-09 02:02:53.000000 cloudvault-1.1/cloudvault.egg-info/dependency_links.txt
--rw-------   0 u0_a269  (10269) u0_a269  (10269)       31 2023-06-09 02:02:53.000000 cloudvault-1.1/cloudvault.egg-info/requires.txt
--rw-------   0 u0_a269  (10269) u0_a269  (10269)       11 2023-06-09 02:02:53.000000 cloudvault-1.1/cloudvault.egg-info/top_level.txt
--rw-------   0 u0_a269  (10269) u0_a269  (10269)      103 2023-06-09 00:35:34.000000 cloudvault-1.1/pyproject.toml
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     1098 2023-06-09 02:02:54.919027 cloudvault-1.1/setup.cfg
--rw-------   0 u0_a269  (10269) u0_a269  (10269)       38 2023-06-09 00:39:39.000000 cloudvault-1.1/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-09 10:39:38.644663 cloudvault-1.2/
+-rw-rw----   0 root         (0) everybody  (9997)     1073 2023-06-09 09:34:11.000000 cloudvault-1.2/LICENSE
+-rw-rw----   0 root         (0) everybody  (9997)       35 2023-06-09 09:34:11.000000 cloudvault-1.2/MANIFEST.in
+-rw-rw----   0 root         (0) everybody  (9997)     1836 2023-06-09 10:39:38.644663 cloudvault-1.2/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      764 2023-06-09 09:34:11.000000 cloudvault-1.2/README.md
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-09 10:39:38.614663 cloudvault-1.2/cloudvault/
+-rw-rw----   0 root         (0) everybody  (9997)        0 2023-06-09 09:34:11.000000 cloudvault-1.2/cloudvault/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)     1129 2023-06-09 10:32:08.000000 cloudvault-1.2/cloudvault/cloud_storage.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-09 10:39:38.637997 cloudvault-1.2/cloudvault.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)     1836 2023-06-09 10:39:37.000000 cloudvault-1.2/cloudvault.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      283 2023-06-09 10:39:38.000000 cloudvault-1.2/cloudvault.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-06-09 10:39:37.000000 cloudvault-1.2/cloudvault.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)       31 2023-06-09 10:39:37.000000 cloudvault-1.2/cloudvault.egg-info/requires.txt
+-rw-rw----   0 root         (0) everybody  (9997)       11 2023-06-09 10:39:37.000000 cloudvault-1.2/cloudvault.egg-info/top_level.txt
+-rw-rw----   0 root         (0) everybody  (9997)      103 2023-06-09 09:34:11.000000 cloudvault-1.2/pyproject.toml
+-rw-rw----   0 root         (0) everybody  (9997)     1098 2023-06-09 10:39:38.651330 cloudvault-1.2/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-06-09 09:34:11.000000 cloudvault-1.2/setup.py
```

### Comparing `cloudvault-1.1/LICENSE` & `cloudvault-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudvault-1.1/PKG-INFO` & `cloudvault-1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudvault
-Version: 1.1
+Version: 1.2
 Summary: A Django package for managing file uploads to cloud[Cloudinary]. It is an alternative for AWS S-3 Bucket.
 Home-page: https://github.com/codewitgabi/cloudvault
 Author: Gabriel Michael Ojomakpene (codewitgabi)
 Author-email: codewitgabi222@gmail.vom
 License: MIT-licence
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `cloudvault-1.1/README.md` & `cloudvault-1.2/README.md`

 * *Files identical despite different names*

### Comparing `cloudvault-1.1/cloudvault.egg-info/PKG-INFO` & `cloudvault-1.2/cloudvault.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudvault
-Version: 1.1
+Version: 1.2
 Summary: A Django package for managing file uploads to cloud[Cloudinary]. It is an alternative for AWS S-3 Bucket.
 Home-page: https://github.com/codewitgabi/cloudvault
 Author: Gabriel Michael Ojomakpene (codewitgabi)
 Author-email: codewitgabi222@gmail.vom
 License: MIT-licence
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `cloudvault-1.1/setup.cfg` & `cloudvault-1.2/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cloudvault
-version = 1.1
+version = 1.2
 description = A Django package for managing file uploads to cloud[Cloudinary]. It is an alternative for AWS S-3 Bucket.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/codewitgabi/cloudvault
 author = Gabriel Michael Ojomakpene (codewitgabi)
 author_email = codewitgabi222@gmail.vom
 license = MIT-licence
```

