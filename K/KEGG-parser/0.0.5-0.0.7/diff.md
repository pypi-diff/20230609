# Comparing `tmp/KEGG-parser-0.0.5.tar.gz` & `tmp/KEGG-parser-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KEGG-parser-0.0.5.tar", last modified: Tue Mar 14 20:22:35 2023, max compression
+gzip compressed data, was "KEGG-parser-0.0.7.tar", last modified: Fri Jun  9 20:40:15 2023, max compression
```

## Comparing `KEGG-parser-0.0.5.tar` & `KEGG-parser-0.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 20:22:35.609127 KEGG-parser-0.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 20:22:35.609127 KEGG-parser-0.0.5/KEGG_parser/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-14 20:22:23.000000 KEGG-parser-0.0.5/KEGG_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-03-14 20:22:23.000000 KEGG-parser-0.0.5/KEGG_parser/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    13727 2023-03-14 20:22:23.000000 KEGG-parser-0.0.5/KEGG_parser/parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 20:22:35.609127 KEGG-parser-0.0.5/KEGG_parser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-03-14 20:22:35.000000 KEGG-parser-0.0.5/KEGG_parser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-03-14 20:22:35.000000 KEGG-parser-0.0.5/KEGG_parser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 20:22:35.000000 KEGG-parser-0.0.5/KEGG_parser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-14 20:22:35.000000 KEGG-parser-0.0.5/KEGG_parser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-14 20:22:35.000000 KEGG-parser-0.0.5/KEGG_parser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-03-14 20:22:23.000000 KEGG-parser-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-03-14 20:22:35.609127 KEGG-parser-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-03-14 20:22:23.000000 KEGG-parser-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-14 20:22:35.609127 KEGG-parser-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-03-14 20:22:23.000000 KEGG-parser-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 20:22:35.609127 KEGG-parser-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-03-14 20:22:23.000000 KEGG-parser-0.0.5/tests/test_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-03-14 20:22:23.000000 KEGG-parser-0.0.5/tests/test_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     8645 2023-03-14 20:22:23.000000 KEGG-parser-0.0.5/tests/test_parse_KEGG.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:40:15.970498 KEGG-parser-0.0.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:40:15.966498 KEGG-parser-0.0.7/KEGG_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-09 20:40:05.000000 KEGG-parser-0.0.7/KEGG_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-06-09 20:40:05.000000 KEGG-parser-0.0.7/KEGG_parser/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13727 2023-06-09 20:40:05.000000 KEGG-parser-0.0.7/KEGG_parser/parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:40:15.970498 KEGG-parser-0.0.7/KEGG_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-06-09 20:40:15.000000 KEGG-parser-0.0.7/KEGG_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-09 20:40:15.000000 KEGG-parser-0.0.7/KEGG_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 20:40:15.000000 KEGG-parser-0.0.7/KEGG_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-09 20:40:15.000000 KEGG-parser-0.0.7/KEGG_parser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-09 20:40:15.000000 KEGG-parser-0.0.7/KEGG_parser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-09 20:40:05.000000 KEGG-parser-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-06-09 20:40:15.970498 KEGG-parser-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-09 20:40:05.000000 KEGG-parser-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 20:40:15.970498 KEGG-parser-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-06-09 20:40:05.000000 KEGG-parser-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:40:15.970498 KEGG-parser-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-09 20:40:05.000000 KEGG-parser-0.0.7/tests/test_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-09 20:40:05.000000 KEGG-parser-0.0.7/tests/test_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8645 2023-06-09 20:40:05.000000 KEGG-parser-0.0.7/tests/test_parse_KEGG.py
```

### Comparing `KEGG-parser-0.0.5/KEGG_parser/downloader.py` & `KEGG-parser-0.0.7/KEGG_parser/downloader.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 import asyncio
 
 import aiohttp
+import requests
+import time
+from tqdm import tqdm
 
 from KEGG_parser.parsers import parse_ko
 
 
 def get_from_kegg_flat_file(file_loc, list_of_ids=None, parser=parse_ko):
     record_list = list()
     for entry in open(file_loc).read().split('///')[:-1]:
@@ -28,30 +31,60 @@
         async with session.get(url) as response:
             if response.status == 200:
                 return await response.text()
             elif response.status != 403:
                 raise ValueError('Bad HTTP request status %s: %s\n%s' % (response.status, response.reason, url))
         await asyncio.sleep(wait)
 
-    raise ValueError('KEGG has forbidden request after %s attempts' % attempts)
+    raise ValueError('KEGG has forbidden request after %s attempts for url %s , which returns a response status of %s' % 
+                     (attempts, url, response.status))
 
 
 async def kegg_download_manager(loop, list_of_ids):
     urls = ['http://rest.kegg.jp/get/%s' % '+'.join(chunk) for chunk in chunks(list(list_of_ids), 10)]
 
     async with aiohttp.ClientSession(loop=loop) as session:
         tasks = [download_coroutine(session, url) for url in urls]
         results = await asyncio.gather(*tasks)
 
     return [raw_record for raw_records in results for raw_record in raw_records.split('///')[:-1]]
 
+def download_synchronous(url, attempts=10):
+    for _ in range(attempts):
+        response = requests.get(url)
 
-def get_from_kegg_api(loop, list_of_ids, parser):
-    return [parser(raw_record) for raw_record in loop.run_until_complete(kegg_download_manager(loop, list_of_ids))]
+        if response.status_code == 200:
+            return response.text
+    
+    # if none of our attempts have returned OK
+    raise ValueError('KEGG has forbidden request after %s attempts for url %s , which returns a response status of %s' % 
+                     (attempts, url, response.status_code))
 
+def kegg_download_manager_synchronous(list_of_ids, wait=1):
+    """This is a backup in case the async downloading is forbidden."""
+    urls = ['http://rest.kegg.jp/get/%s' % '+'.join(chunk) for chunk in chunks(list(list_of_ids), 10)]
+    num_urls = len(urls)
+    print(f"Total urls to download: {num_urls}. Progress will be shown below.")
+    results = []
+    for url in tqdm(urls):
+        results.append(download_synchronous(url))
+        time.sleep(wait)
+
+    return [raw_record for raw_records in results for raw_record in raw_records.split('///')[:-1]]
+
+
+
+def get_from_kegg_api(loop, list_of_ids, parser):
+    try:
+        return [parser(raw_record) for raw_record in loop.run_until_complete(kegg_download_manager(loop, list_of_ids))]
+    except ValueError:
+        print("Asynchronous downloading of KEGG records has failed. KEGG parser will try to download data sequentially."
+              "This will be slower.")
+        time.sleep(30)
+        return [parser(raw_record) for raw_record in kegg_download_manager_synchronous(list_of_ids)]
 
 def get_kegg_record_dict(list_of_ids, parser, records_file_loc=None, verbose=False):
     if records_file_loc is None:
         loop = asyncio.get_event_loop()
         records = get_from_kegg_api(loop, list_of_ids, parser)
     else:
         records = get_from_kegg_flat_file(records_file_loc, list_of_ids, parser)
```

### Comparing `KEGG-parser-0.0.5/KEGG_parser/parsers.py` & `KEGG-parser-0.0.7/KEGG_parser/parsers.py`

 * *Files identical despite different names*

### Comparing `KEGG-parser-0.0.5/KEGG_parser.egg-info/PKG-INFO` & `KEGG-parser-0.0.7/KEGG_parser.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: KEGG-parser
-Version: 0.0.5
+Version: 0.0.7
 Summary: KEGG Parser: A tool for parsing and converting KEGG data into manipulable Python objects.
 Home-page: https://github.com/lozuponelab/KEGG_parser/
-Download-URL: https://github.com/lozuponelab/KEGG_parser/tarball/0.0.5
+Download-URL: https://github.com/lozuponelab/KEGG_parser/tarball/0.0.7
 Author: Kumar Thurimella
 Author-email: lozuponelab.dev@olucdenver.onmicrosoft.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # KEGG-parser
 [![PyPI](https://img.shields.io/pypi/v/KEGG-parser.svg?style=flat)](https://pypi.python.org/pypi/KEGG-parser) ![Build Status](https://github.com/lozuponelab/KEGG_parser/actions/workflows/main.yml/badge.svg)
```

### Comparing `KEGG-parser-0.0.5/LICENSE` & `KEGG-parser-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `KEGG-parser-0.0.5/PKG-INFO` & `KEGG-parser-0.0.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: KEGG-parser
-Version: 0.0.5
+Version: 0.0.7
 Summary: KEGG Parser: A tool for parsing and converting KEGG data into manipulable Python objects.
 Home-page: https://github.com/lozuponelab/KEGG_parser/
-Download-URL: https://github.com/lozuponelab/KEGG_parser/tarball/0.0.5
+Download-URL: https://github.com/lozuponelab/KEGG_parser/tarball/0.0.7
 Author: Kumar Thurimella
 Author-email: lozuponelab.dev@olucdenver.onmicrosoft.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # KEGG-parser
 [![PyPI](https://img.shields.io/pypi/v/KEGG-parser.svg?style=flat)](https://pypi.python.org/pypi/KEGG-parser) ![Build Status](https://github.com/lozuponelab/KEGG_parser/actions/workflows/main.yml/badge.svg)
```

### Comparing `KEGG-parser-0.0.5/setup.py` & `KEGG-parser-0.0.7/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 __author__ = 'lozuponelab'
 __version__ = version
 
 setup(
       name="KEGG-parser",
       version=__version__,
       setup_requires=['pytest-runner'],
-      tests_require=['pytest'],
-      install_requires=['aiohttp'],
+      tests_require=['pytest', 'requests'],
+      install_requires=['aiohttp', 'asyncio', 'tqdm', 'requests'],
       packages=find_packages(),
       description="KEGG Parser: A tool for parsing and converting KEGG data into manipulable Python objects.",
       long_description=long_description,
       long_description_content_type='text/markdown',
       author="Kumar Thurimella",
       author_email='lozuponelab.dev@olucdenver.onmicrosoft.com',
       url="https://github.com/lozuponelab/KEGG_parser/",
```

### Comparing `KEGG-parser-0.0.5/tests/test_downloader.py` & `KEGG-parser-0.0.7/tests/test_downloader.py`

 * *Files identical despite different names*

### Comparing `KEGG-parser-0.0.5/tests/test_fixtures.py` & `KEGG-parser-0.0.7/tests/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `KEGG-parser-0.0.5/tests/test_parse_KEGG.py` & `KEGG-parser-0.0.7/tests/test_parse_KEGG.py`

 * *Files identical despite different names*

