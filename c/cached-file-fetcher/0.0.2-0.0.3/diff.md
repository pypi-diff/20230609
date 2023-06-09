# Comparing `tmp/cached-file-fetcher-0.0.2.tar.gz` & `tmp/cached-file-fetcher-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cached-file-fetcher-0.0.2.tar", last modified: Fri Jun  9 20:43:51 2023, max compression
+gzip compressed data, was "cached-file-fetcher-0.0.3.tar", last modified: Fri Jun  9 20:56:02 2023, max compression
```

## Comparing `cached-file-fetcher-0.0.2.tar` & `cached-file-fetcher-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-06-09 20:43:51.401278 cached-file-fetcher-0.0.2/
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1071 2023-06-09 19:41:09.000000 cached-file-fetcher-0.0.2/LICENSE
--rw-r--r--   0 panacea   (1000) panacea   (1000)      612 2023-06-09 20:43:51.401278 cached-file-fetcher-0.0.2/PKG-INFO
--rw-r--r--   0 panacea   (1000) panacea   (1000)      984 2023-06-09 20:43:44.000000 cached-file-fetcher-0.0.2/pyproject.toml
--rw-r--r--   0 panacea   (1000) panacea   (1000)       38 2023-06-09 20:43:51.401278 cached-file-fetcher-0.0.2/setup.cfg
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-06-09 20:43:51.401278 cached-file-fetcher-0.0.2/src/
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-06-09 20:43:51.401278 cached-file-fetcher-0.0.2/src/cached_file_fetcher/
--rw-r--r--   0 panacea   (1000) panacea   (1000)     2979 2023-06-09 20:40:41.000000 cached-file-fetcher-0.0.2/src/cached_file_fetcher/__init__.py
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-06-09 20:43:51.401278 cached-file-fetcher-0.0.2/src/cached_file_fetcher.egg-info/
--rw-r--r--   0 panacea   (1000) panacea   (1000)      612 2023-06-09 20:43:51.000000 cached-file-fetcher-0.0.2/src/cached_file_fetcher.egg-info/PKG-INFO
--rw-r--r--   0 panacea   (1000) panacea   (1000)      318 2023-06-09 20:43:51.000000 cached-file-fetcher-0.0.2/src/cached_file_fetcher.egg-info/SOURCES.txt
--rw-r--r--   0 panacea   (1000) panacea   (1000)        1 2023-06-09 20:43:51.000000 cached-file-fetcher-0.0.2/src/cached_file_fetcher.egg-info/dependency_links.txt
--rw-r--r--   0 panacea   (1000) panacea   (1000)       32 2023-06-09 20:43:51.000000 cached-file-fetcher-0.0.2/src/cached_file_fetcher.egg-info/requires.txt
--rw-r--r--   0 panacea   (1000) panacea   (1000)       20 2023-06-09 20:43:51.000000 cached-file-fetcher-0.0.2/src/cached_file_fetcher.egg-info/top_level.txt
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-06-09 20:43:51.401278 cached-file-fetcher-0.0.2/test/
--rw-r--r--   0 panacea   (1000) panacea   (1000)     3311 2023-06-09 20:43:37.000000 cached-file-fetcher-0.0.2/test/test_file_fetcher.py
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-06-09 20:56:02.671041 cached-file-fetcher-0.0.3/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1071 2023-06-09 19:41:09.000000 cached-file-fetcher-0.0.3/LICENSE
+-rw-r--r--   0 panacea   (1000) panacea   (1000)      612 2023-06-09 20:56:02.671041 cached-file-fetcher-0.0.3/PKG-INFO
+-rw-r--r--   0 panacea   (1000) panacea   (1000)      984 2023-06-09 20:55:49.000000 cached-file-fetcher-0.0.3/pyproject.toml
+-rw-r--r--   0 panacea   (1000) panacea   (1000)       38 2023-06-09 20:56:02.671041 cached-file-fetcher-0.0.3/setup.cfg
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-06-09 20:56:02.661041 cached-file-fetcher-0.0.3/src/
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-06-09 20:56:02.671041 cached-file-fetcher-0.0.3/src/cached_file_fetcher/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     3001 2023-06-09 20:55:35.000000 cached-file-fetcher-0.0.3/src/cached_file_fetcher/__init__.py
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-06-09 20:56:02.671041 cached-file-fetcher-0.0.3/src/cached_file_fetcher.egg-info/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)      612 2023-06-09 20:56:02.000000 cached-file-fetcher-0.0.3/src/cached_file_fetcher.egg-info/PKG-INFO
+-rw-r--r--   0 panacea   (1000) panacea   (1000)      318 2023-06-09 20:56:02.000000 cached-file-fetcher-0.0.3/src/cached_file_fetcher.egg-info/SOURCES.txt
+-rw-r--r--   0 panacea   (1000) panacea   (1000)        1 2023-06-09 20:56:02.000000 cached-file-fetcher-0.0.3/src/cached_file_fetcher.egg-info/dependency_links.txt
+-rw-r--r--   0 panacea   (1000) panacea   (1000)       32 2023-06-09 20:56:02.000000 cached-file-fetcher-0.0.3/src/cached_file_fetcher.egg-info/requires.txt
+-rw-r--r--   0 panacea   (1000) panacea   (1000)       20 2023-06-09 20:56:02.000000 cached-file-fetcher-0.0.3/src/cached_file_fetcher.egg-info/top_level.txt
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-06-09 20:56:02.671041 cached-file-fetcher-0.0.3/test/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     3311 2023-06-09 20:44:55.000000 cached-file-fetcher-0.0.3/test/test_file_fetcher.py
```

### Comparing `cached-file-fetcher-0.0.2/LICENSE` & `cached-file-fetcher-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cached-file-fetcher-0.0.2/PKG-INFO` & `cached-file-fetcher-0.0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cached-file-fetcher
-Version: 0.0.2
+Version: 0.0.3
 Summary: Fetches files from s3, and caches them on local disk while maintaining a size-limited LRU cache.
 Author-email: TuneFlow <contact@info.tuneflow.com>
 Project-URL: Homepage, https://github.com/andantei/file-fetcher
 Project-URL: Bug Tracker, https://github.com/andantei/file-fetcher/issues
 Keywords: file,fetcher
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cached-file-fetcher-0.0.2/pyproject.toml` & `cached-file-fetcher-0.0.3/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "cached-file-fetcher"
-version = "0.0.2"
+version = "0.0.3"
 authors = [{ name = "TuneFlow", email = "contact@info.tuneflow.com" }]
 description = "Fetches files from s3, and caches them on local disk while maintaining a size-limited LRU cache."
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = [
     'file',
     'fetcher'
```

### Comparing `cached-file-fetcher-0.0.2/src/cached_file_fetcher/__init__.py` & `cached-file-fetcher-0.0.3/src/cached_file_fetcher/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,17 +50,18 @@
         self.lru[file_key] = file_path
 
         # Check if the file exists on the disk
         if os.path.exists(file_path):
             return file_path
         
         # Download the file from s3
-        print(f'Downloading file {file_key} to {file_path}')
+        s3_key = f'{self.s3_prefix}/{file_key}'
+        print(f'Downloading file {s3_key} to {file_path}')
         try:
-            self.s3.download_file(self.s3_bucket, f'{self.s3_prefix}/{file_key}', file_path)
+            self.s3.download_file(self.s3_bucket, s3_key, file_path)
             return file_path
         except Exception as e:
             print(e)
             return None
     
     def remove_file(self, file_key):
         '''
```

### Comparing `cached-file-fetcher-0.0.2/src/cached_file_fetcher.egg-info/PKG-INFO` & `cached-file-fetcher-0.0.3/src/cached_file_fetcher.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cached-file-fetcher
-Version: 0.0.2
+Version: 0.0.3
 Summary: Fetches files from s3, and caches them on local disk while maintaining a size-limited LRU cache.
 Author-email: TuneFlow <contact@info.tuneflow.com>
 Project-URL: Homepage, https://github.com/andantei/file-fetcher
 Project-URL: Bug Tracker, https://github.com/andantei/file-fetcher/issues
 Keywords: file,fetcher
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cached-file-fetcher-0.0.2/test/test_file_fetcher.py` & `cached-file-fetcher-0.0.3/test/test_file_fetcher.py`

 * *Files identical despite different names*

