# Comparing `tmp/tap-zendesk-2.0.0.tar.gz` & `tmp/tap-zendesk-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap-zendesk-2.0.0.tar", last modified: Thu May 25 14:08:08 2023, max compression
+gzip compressed data, was "dist/tap-zendesk-2.0.1.tar", last modified: Mon Jun  5 09:01:55 2023, max compression
```

## Comparing `tap-zendesk-2.0.0.tar` & `tap-zendesk-2.0.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-25 14:08:08.052697 tap-zendesk-2.0.0/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32393 2023-05-04 11:11:44.000000 tap-zendesk-2.0.0/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       93 2023-05-04 11:11:44.000000 tap-zendesk-2.0.0/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      282 2023-05-25 14:08:08.052697 tap-zendesk-2.0.0/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1553 2023-05-04 11:11:44.000000 tap-zendesk-2.0.0/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       79 2023-05-25 14:08:08.052697 tap-zendesk-2.0.0/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      877 2023-05-25 14:06:36.000000 tap-zendesk-2.0.0/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-25 14:08:08.044697 tap-zendesk-2.0.0/tap_zendesk/
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)     7863 2023-05-04 11:11:44.000000 tap-zendesk-2.0.0/tap_zendesk/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3673 2023-05-04 11:11:44.000000 tap-zendesk-2.0.0/tap_zendesk/discover.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8390 2023-05-25 11:43:11.000000 tap-zendesk-2.0.0/tap_zendesk/http.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4101 2023-05-04 11:11:44.000000 tap-zendesk-2.0.0/tap_zendesk/metrics.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-25 14:08:08.048697 tap-zendesk-2.0.0/tap_zendesk/schemas/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      694 2023-05-04 11:11:44.000000 tap-zendesk-2.0.0/tap_zendesk/schemas/group_memberships.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      607 2023-05-04 11:11:44.000000 tap-zendesk-2.0.0/tap_zendesk/schemas/groups.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1744 2023-05-04 11:11:44.000000 tap-zendesk-2.0.0/tap_zendesk/schemas/macros.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1619 2023-05-04 11:11:44.000000 tap-zendesk-2.0.0/tap_zendesk/schemas/organizations.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      842 2023-05-04 11:11:44.000000 tap-zendesk-2.0.0/tap_zendesk/schemas/satisfaction_ratings.json
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-25 14:08:08.052697 tap-zendesk-2.0.0/tap_zendesk/schemas/shared/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2615 2023-05-04 11:11:44.000000 tap-zendesk-2.0.0/tap_zendesk/schemas/shared/attachments.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2493 2023-05-04 11:11:44.000000 tap-zendesk-2.0.0/tap_zendesk/schemas/shared/metadata.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2340 2023-05-04 11:11:44.000000 tap-zendesk-2.0.0/tap_zendesk/schemas/shared/via.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2375 2023-05-04 11:11:44.000000 tap-zendesk-2.0.0/tap_zendesk/schemas/sla_policies.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      225 2023-05-04 11:11:44.000000 tap-zendesk-2.0.0/tap_zendesk/schemas/tags.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18549 2023-05-04 11:11:44.000000 tap-zendesk-2.0.0/tap_zendesk/schemas/ticket_audits.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1058 2023-05-04 11:11:44.000000 tap-zendesk-2.0.0/tap_zendesk/schemas/ticket_comments.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3004 2023-05-04 11:11:44.000000 tap-zendesk-2.0.0/tap_zendesk/schemas/ticket_fields.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1583 2023-05-04 11:11:44.000000 tap-zendesk-2.0.0/tap_zendesk/schemas/ticket_forms.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4434 2023-05-04 11:11:44.000000 tap-zendesk-2.0.0/tap_zendesk/schemas/ticket_metrics.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6744 2023-05-04 11:11:44.000000 tap-zendesk-2.0.0/tap_zendesk/schemas/tickets.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6263 2023-05-04 11:11:44.000000 tap-zendesk-2.0.0/tap_zendesk/schemas/users.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    24869 2023-05-25 11:43:11.000000 tap-zendesk-2.0.0/tap_zendesk/streams.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2473 2023-05-04 11:11:44.000000 tap-zendesk-2.0.0/tap_zendesk/sync.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-25 14:08:08.048697 tap-zendesk-2.0.0/tap_zendesk.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      282 2023-05-25 14:08:07.000000 tap-zendesk-2.0.0/tap_zendesk.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1307 2023-05-25 14:08:07.000000 tap-zendesk-2.0.0/tap_zendesk.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-25 14:08:07.000000 tap-zendesk-2.0.0/tap_zendesk.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       49 2023-05-25 14:08:07.000000 tap-zendesk-2.0.0/tap_zendesk.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      125 2023-05-25 14:08:07.000000 tap-zendesk-2.0.0/tap_zendesk.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       12 2023-05-25 14:08:07.000000 tap-zendesk-2.0.0/tap_zendesk.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-25 14:08:08.052697 tap-zendesk-2.0.0/test/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3865 2023-05-25 11:43:11.000000 tap-zendesk-2.0.0/test/test_all_fields.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8646 2023-05-25 07:10:58.000000 tap-zendesk-2.0.0/test/test_all_streams.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3283 2023-05-04 11:11:44.000000 tap-zendesk-2.0.0/test/test_automatic_fields.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6792 2023-05-04 11:11:44.000000 tap-zendesk-2.0.0/test/test_bookmarks.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2102 2023-05-04 11:11:44.000000 tap-zendesk-2.0.0/test/test_custom_fields_discover.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6986 2023-05-04 11:11:44.000000 tap-zendesk-2.0.0/test/test_discovery.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2706 2023-05-04 11:11:44.000000 tap-zendesk-2.0.0/test/test_minimal_selection.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3168 2023-05-04 11:11:44.000000 tap-zendesk-2.0.0/test/test_pagination.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10384 2023-05-25 07:10:58.000000 tap-zendesk-2.0.0/test/test_standard_bookmark.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10085 2023-05-25 07:10:58.000000 tap-zendesk-2.0.0/test/test_start_date.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-05 09:01:55.000000 tap-zendesk-2.0.1/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       93 2023-05-30 04:15:54.000000 tap-zendesk-2.0.1/MANIFEST.in
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-05 09:01:55.000000 tap-zendesk-2.0.1/tap_zendesk/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8122 2023-06-05 09:01:37.000000 tap-zendesk-2.0.1/tap_zendesk/http.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4101 2023-05-30 04:15:54.000000 tap-zendesk-2.0.1/tap_zendesk/metrics.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-05 09:01:55.000000 tap-zendesk-2.0.1/tap_zendesk/schemas/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4434 2023-05-30 04:15:54.000000 tap-zendesk-2.0.1/tap_zendesk/schemas/ticket_metrics.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6744 2023-05-30 04:15:54.000000 tap-zendesk-2.0.1/tap_zendesk/schemas/tickets.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      694 2023-05-30 04:15:54.000000 tap-zendesk-2.0.1/tap_zendesk/schemas/group_memberships.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2375 2023-05-30 04:15:54.000000 tap-zendesk-2.0.1/tap_zendesk/schemas/sla_policies.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1058 2023-05-30 04:15:54.000000 tap-zendesk-2.0.1/tap_zendesk/schemas/ticket_comments.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      607 2023-05-30 04:15:54.000000 tap-zendesk-2.0.1/tap_zendesk/schemas/groups.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      225 2023-05-30 04:15:54.000000 tap-zendesk-2.0.1/tap_zendesk/schemas/tags.json
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-05 09:01:55.000000 tap-zendesk-2.0.1/tap_zendesk/schemas/shared/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2615 2023-05-30 04:15:54.000000 tap-zendesk-2.0.1/tap_zendesk/schemas/shared/attachments.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2493 2023-05-30 04:15:54.000000 tap-zendesk-2.0.1/tap_zendesk/schemas/shared/metadata.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2340 2023-05-30 04:15:54.000000 tap-zendesk-2.0.1/tap_zendesk/schemas/shared/via.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18549 2023-05-30 04:15:54.000000 tap-zendesk-2.0.1/tap_zendesk/schemas/ticket_audits.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1744 2023-05-30 04:15:54.000000 tap-zendesk-2.0.1/tap_zendesk/schemas/macros.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1583 2023-05-30 04:15:54.000000 tap-zendesk-2.0.1/tap_zendesk/schemas/ticket_forms.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6263 2023-05-30 04:15:54.000000 tap-zendesk-2.0.1/tap_zendesk/schemas/users.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      842 2023-05-30 04:15:54.000000 tap-zendesk-2.0.1/tap_zendesk/schemas/satisfaction_ratings.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3004 2023-05-30 04:15:54.000000 tap-zendesk-2.0.1/tap_zendesk/schemas/ticket_fields.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1619 2023-05-30 04:15:54.000000 tap-zendesk-2.0.1/tap_zendesk/schemas/organizations.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    24869 2023-05-31 06:52:44.000000 tap-zendesk-2.0.1/tap_zendesk/streams.py
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)     8280 2023-06-05 09:01:37.000000 tap-zendesk-2.0.1/tap_zendesk/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2473 2023-05-30 04:15:54.000000 tap-zendesk-2.0.1/tap_zendesk/sync.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3673 2023-05-30 04:15:54.000000 tap-zendesk-2.0.1/tap_zendesk/discover.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-05 09:01:55.000000 tap-zendesk-2.0.1/tap_zendesk.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      125 2023-06-05 09:01:55.000000 tap-zendesk-2.0.1/tap_zendesk.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-05 09:01:55.000000 tap-zendesk-2.0.1/tap_zendesk.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2023-06-05 09:01:55.000000 tap-zendesk-2.0.1/tap_zendesk.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      297 2023-06-05 09:01:55.000000 tap-zendesk-2.0.1/tap_zendesk.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1307 2023-06-05 09:01:55.000000 tap-zendesk-2.0.1/tap_zendesk.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       12 2023-06-05 09:01:55.000000 tap-zendesk-2.0.1/tap_zendesk.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-05 09:01:55.000000 tap-zendesk-2.0.1/test/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3168 2023-05-30 04:15:54.000000 tap-zendesk-2.0.1/test/test_pagination.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8646 2023-05-30 04:15:54.000000 tap-zendesk-2.0.1/test/test_all_streams.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3865 2023-05-31 06:52:44.000000 tap-zendesk-2.0.1/test/test_all_fields.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2706 2023-05-30 04:15:54.000000 tap-zendesk-2.0.1/test/test_minimal_selection.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2102 2023-05-30 04:15:54.000000 tap-zendesk-2.0.1/test/test_custom_fields_discover.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6986 2023-05-30 04:15:54.000000 tap-zendesk-2.0.1/test/test_discovery.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10384 2023-05-30 04:15:54.000000 tap-zendesk-2.0.1/test/test_standard_bookmark.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3283 2023-05-30 04:15:54.000000 tap-zendesk-2.0.1/test/test_automatic_fields.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10085 2023-05-30 04:15:54.000000 tap-zendesk-2.0.1/test/test_start_date.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6792 2023-05-30 04:15:54.000000 tap-zendesk-2.0.1/test/test_bookmarks.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      100 2023-06-05 09:01:55.000000 tap-zendesk-2.0.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      297 2023-06-05 09:01:55.000000 tap-zendesk-2.0.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      877 2023-06-05 09:01:37.000000 tap-zendesk-2.0.1/setup.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32393 2023-05-30 04:15:54.000000 tap-zendesk-2.0.1/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1553 2023-05-30 04:15:54.000000 tap-zendesk-2.0.1/README.md
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `tap-zendesk-2.0.0/LICENSE` & `tap-zendesk-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tap-zendesk-2.0.0/README.md` & `tap-zendesk-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `tap-zendesk-2.0.0/setup.py` & `tap-zendesk-2.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 
 from setuptools import setup
 
 setup(name='tap-zendesk',
-      version='2.0.0',
+      version='2.0.1',
       description='Singer.io tap for extracting data from the Zendesk API',
       author='Stitch',
       url='https://singer.io',
       classifiers=['Programming Language :: Python :: 3 :: Only'],
       py_modules=['tap_zendesk'],
       install_requires=[
           'singer-python==5.12.2',
```

### Comparing `tap-zendesk-2.0.0/tap_zendesk/__init__.py` & `tap-zendesk-2.0.1/tap_zendesk/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,19 @@
 import json
 import sys
 
 from zenpy import Zenpy
 import requests
 from requests import Session
 from requests.adapters import HTTPAdapter
+from requests.exceptions import Timeout, ChunkedEncodingError
+from urllib3.exceptions import ProtocolError
 import singer
 from singer import metadata, metrics as singer_metrics
+import backoff
 from tap_zendesk import metrics as zendesk_metrics
 from tap_zendesk.discover import discover_streams
 from tap_zendesk.streams import STREAMS
 from tap_zendesk.sync import sync_stream
 
 LOGGER = singer.get_logger()
 
@@ -32,77 +35,92 @@
     "email",
     "api_token",
 ]
 
 # patch Session.request to record HTTP request metrics
 request = Session.request
 
+
+@backoff.on_exception(backoff.expo,
+                      (ConnectionError, ConnectionResetError, Timeout, ChunkedEncodingError,
+                       ProtocolError),
+                      max_tries=5,
+                      factor=2)
 def request_metrics_patch(self, method, url, **kwargs):
     with singer_metrics.http_request_timer(None):
         response = request(self, method, url, **kwargs)
         LOGGER.info("Request: %s, Response ETag: %s, Request Id: %s",
                     url,
                     response.headers.get('ETag', 'Not present'),
                     response.headers.get('X-Request-Id', 'Not present'))
         return response
 
+
 Session.request = request_metrics_patch
+
+
 # end patch
 
 def do_discover(client, config):
     LOGGER.info("Starting discover")
     catalog = {"streams": discover_streams(client, config)}
     json.dump(catalog, sys.stdout, indent=2)
     LOGGER.info("Finished discover")
 
+
 def stream_is_selected(mdata):
     return mdata.get((), {}).get('selected', False)
 
+
 def get_selected_streams(catalog):
     selected_stream_names = []
     for stream in catalog.streams:
         mdata = metadata.to_map(stream.metadata)
         if stream_is_selected(mdata):
             selected_stream_names.append(stream.tap_stream_id)
     return selected_stream_names
 
 
 SUB_STREAMS = {
     'tickets': ['ticket_audits', 'ticket_metrics', 'ticket_comments']
 }
 
+
 def get_sub_stream_names():
     sub_stream_names = []
     for parent_stream in SUB_STREAMS:
         sub_stream_names.extend(SUB_STREAMS[parent_stream])
     return sub_stream_names
 
+
 class DependencyException(Exception):
     pass
 
+
 def validate_dependencies(selected_stream_ids):
     errs = []
     msg_tmpl = ("Unable to extract {0} data. "
                 "To receive {0} data, you also need to select {1}.")
     for parent_stream_name in SUB_STREAMS:
         sub_stream_names = SUB_STREAMS[parent_stream_name]
         for sub_stream_name in sub_stream_names:
             if sub_stream_name in selected_stream_ids and parent_stream_name not in selected_stream_ids:
                 errs.append(msg_tmpl.format(sub_stream_name, parent_stream_name))
 
     if errs:
         raise DependencyException(" ".join(errs))
 
+
 def populate_class_schemas(catalog, selected_stream_names):
     for stream in catalog.streams:
         if stream.tap_stream_id in selected_stream_names:
             STREAMS[stream.tap_stream_id].stream = stream
 
-def do_sync(client, catalog, state, config):
 
+def do_sync(client, catalog, state, config):
     selected_stream_names = get_selected_streams(catalog)
     validate_dependencies(selected_stream_names)
     populate_class_schemas(catalog, selected_stream_names)
     all_sub_stream_names = get_sub_stream_names()
 
     for stream in catalog.streams:
         stream_name = stream.tap_stream_id
@@ -117,27 +135,27 @@
         #         starting_stream = None
         #     else:
         #         LOGGER.info("%s: Skipping - already synced", stream_name)
         #         continue
         # else:
         #     LOGGER.info("%s: Starting", stream_name)
 
-
         key_properties = metadata.get(mdata, (), 'table-key-properties')
         singer.write_schema(stream_name, stream.schema.to_dict(), key_properties)
 
         sub_stream_names = SUB_STREAMS.get(stream_name)
         if sub_stream_names:
             for sub_stream_name in sub_stream_names:
                 if sub_stream_name not in selected_stream_names:
                     continue
                 sub_stream = STREAMS[sub_stream_name].stream
                 sub_mdata = metadata.to_map(sub_stream.metadata)
                 sub_key_properties = metadata.get(sub_mdata, (), 'table-key-properties')
-                singer.write_schema(sub_stream.tap_stream_id, sub_stream.schema.to_dict(), sub_key_properties)
+                singer.write_schema(sub_stream.tap_stream_id, sub_stream.schema.to_dict(),
+                                    sub_key_properties)
 
         # parent stream will sync sub stream
         if stream_name in all_sub_stream_names:
             continue
 
         LOGGER.info("%s: Starting sync", stream_name)
         instance = STREAMS[stream_name](client, config)
@@ -146,66 +164,71 @@
         LOGGER.info("%s: Completed sync (%s rows)", stream_name, counter_value)
         zendesk_metrics.log_aggregate_rates()
 
     singer.write_state(state)
     LOGGER.info("Finished sync")
     zendesk_metrics.log_aggregate_rates()
 
+
 def oauth_auth(args):
     if not set(OAUTH_CONFIG_KEYS).issubset(args.config.keys()):
         LOGGER.debug("OAuth authentication unavailable.")
         return None
 
     LOGGER.info("Using OAuth authentication.")
     return {
         "subdomain": args.config['subdomain'],
         "oauth_token": args.config['access_token'],
     }
 
+
 def api_token_auth(args):
     if not set(API_TOKEN_CONFIG_KEYS).issubset(args.config.keys()):
         LOGGER.debug("API Token authentication unavailable.")
         return None
 
     LOGGER.info("Using API Token authentication.")
     return {
         "subdomain": args.config['subdomain'],
         "email": args.config['email'],
         "token": args.config['api_token']
     }
 
+
 def get_session(config):
     """ Add partner information to requests Session object if specified in the config. """
     if not all(k in config for k in ["marketplace_name",
                                      "marketplace_organization_id",
                                      "marketplace_app_id"]):
         return None
     session = requests.Session()
     # Using Zenpy's default adapter args, following the method outlined here:
     # https://github.com/facetoe/zenpy/blob/master/docs/zenpy.rst#usage
     session.mount("https://", HTTPAdapter(**Zenpy.http_adapter_kwargs()))
     session.headers["X-Zendesk-Marketplace-Name"] = config.get("marketplace_name", "")
-    session.headers["X-Zendesk-Marketplace-Organization-Id"] = str(config.get("marketplace_organization_id", ""))
+    session.headers["X-Zendesk-Marketplace-Organization-Id"] = str(
+        config.get("marketplace_organization_id", ""))
     session.headers["X-Zendesk-Marketplace-App-Id"] = str(config.get("marketplace_app_id", ""))
     return session
 
+
 @singer.utils.handle_top_exception(LOGGER)
 def main():
     parsed_args = singer.utils.parse_args(REQUIRED_CONFIG_KEYS)
 
     # Set request timeout to config param `request_timeout` value.
     config_request_timeout = parsed_args.config.get('request_timeout')
     if config_request_timeout and float(config_request_timeout):
         request_timeout = float(config_request_timeout)
     else:
-        request_timeout = REQUEST_TIMEOUT # If value is 0, "0", "" or not passed then it sets default to 300 seconds.
+        request_timeout = REQUEST_TIMEOUT  # If value is 0, "0", "" or not passed then it sets default to 300 seconds.
     # OAuth has precedence
     creds = oauth_auth(parsed_args) or api_token_auth(parsed_args)
     session = get_session(parsed_args.config)
-    client = Zenpy(session=session, timeout=request_timeout, **creds) # Pass request timeout
+    client = Zenpy(session=session, timeout=request_timeout, **creds)  # Pass request timeout
 
     if not client:
         LOGGER.error("""No suitable authentication keys provided.""")
 
     if parsed_args.discover:
         # passing the config to check the authentication in the do_discover method
         do_discover(client, parsed_args.config)
```

### Comparing `tap-zendesk-2.0.0/tap_zendesk/discover.py` & `tap-zendesk-2.0.1/tap_zendesk/discover.py`

 * *Files identical despite different names*

### Comparing `tap-zendesk-2.0.0/tap_zendesk/http.py` & `tap-zendesk-2.0.1/tap_zendesk/http.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from time import sleep
 import backoff
 import requests
 import singer
-from requests.exceptions import Timeout, HTTPError
+from requests.exceptions import Timeout, HTTPError, ChunkedEncodingError, ConnectionError
+from urllib3.exceptions import ProtocolError
 
 
 
 LOGGER = singer.get_logger()
 
 
 class ZendeskError(Exception):
@@ -103,25 +104,19 @@
 
     if status_code == 429:
         sleep_time = int(exception.response.headers['Retry-After'])
         LOGGER.info("Caught HTTP 429, retrying request in %s seconds", sleep_time)
         sleep(sleep_time)
         return False
 
-    return 400 <=status_code < 500
+    if status_code == 409:
+        # retry ZendeskConflictError for at-least 10 times
+        return False
 
-def should_retry_error(exception):
-    """
-        Return true if exception is required to retry otherwise return false
-    """
-    if isinstance(exception, ZendeskConflictError):
-        return True
-    if isinstance(exception,Exception) and isinstance(exception.args[0][1],ConnectionResetError):
-        return True
-    return False
+    return 400 <=status_code < 500
 
 def raise_for_error(response):
     """ Error handling method which throws custom error. Class for each error defined above which extends `ZendeskError`.
     This method map the status code with `ERROR_CODE_EXCEPTION_MAPPING` dictionary and accordingly raise the error.
     If status_code is 200 then simply return json response.
     """
     try:
@@ -136,24 +131,21 @@
                 response.status_code,
                 response_json.get("message", ERROR_CODE_EXCEPTION_MAPPING.get(
                     response.status_code, {}).get("message", "Unknown Error")))
         exc = ERROR_CODE_EXCEPTION_MAPPING.get(
             response.status_code, {}).get("raise_exception", ZendeskError)
         raise exc(message, response) from None
 
-@backoff.on_exception(backoff.expo,
-                      (ZendeskConflictError),
-                      max_tries=10,
-                      giveup=lambda e: not should_retry_error(e))
+
 @backoff.on_exception(backoff.expo,
                       (HTTPError, ZendeskError), # Added support of backoff for all unhandled status codes.
                       max_tries=10,
                       giveup=is_fatal)
 @backoff.on_exception(backoff.expo,
-                    (ConnectionError, Timeout),#As ConnectionError error and timeout error does not have attribute status_code,
+                    (ConnectionError, ConnectionResetError, Timeout, ChunkedEncodingError, ProtocolError),#As ConnectionError error and timeout error does not have attribute status_code,
                     max_tries=5, # here we added another backoff expression.
                     factor=2)
 def call_api(url, request_timeout, params, headers):
     response = requests.get(url, params=params, headers=headers, timeout=request_timeout) # Pass request timeout
     raise_for_error(response)
     return response
```

### Comparing `tap-zendesk-2.0.0/tap_zendesk/metrics.py` & `tap-zendesk-2.0.1/tap_zendesk/metrics.py`

 * *Files identical despite different names*

### Comparing `tap-zendesk-2.0.0/tap_zendesk/schemas/group_memberships.json` & `tap-zendesk-2.0.1/tap_zendesk/schemas/group_memberships.json`

 * *Files identical despite different names*

### Comparing `tap-zendesk-2.0.0/tap_zendesk/schemas/groups.json` & `tap-zendesk-2.0.1/tap_zendesk/schemas/groups.json`

 * *Files identical despite different names*

### Comparing `tap-zendesk-2.0.0/tap_zendesk/schemas/macros.json` & `tap-zendesk-2.0.1/tap_zendesk/schemas/macros.json`

 * *Files identical despite different names*

### Comparing `tap-zendesk-2.0.0/tap_zendesk/schemas/organizations.json` & `tap-zendesk-2.0.1/tap_zendesk/schemas/organizations.json`

 * *Files identical despite different names*

### Comparing `tap-zendesk-2.0.0/tap_zendesk/schemas/satisfaction_ratings.json` & `tap-zendesk-2.0.1/tap_zendesk/schemas/satisfaction_ratings.json`

 * *Files identical despite different names*

### Comparing `tap-zendesk-2.0.0/tap_zendesk/schemas/shared/attachments.json` & `tap-zendesk-2.0.1/tap_zendesk/schemas/shared/attachments.json`

 * *Files identical despite different names*

### Comparing `tap-zendesk-2.0.0/tap_zendesk/schemas/shared/metadata.json` & `tap-zendesk-2.0.1/tap_zendesk/schemas/shared/metadata.json`

 * *Files identical despite different names*

### Comparing `tap-zendesk-2.0.0/tap_zendesk/schemas/shared/via.json` & `tap-zendesk-2.0.1/tap_zendesk/schemas/shared/via.json`

 * *Files identical despite different names*

### Comparing `tap-zendesk-2.0.0/tap_zendesk/schemas/sla_policies.json` & `tap-zendesk-2.0.1/tap_zendesk/schemas/sla_policies.json`

 * *Files identical despite different names*

### Comparing `tap-zendesk-2.0.0/tap_zendesk/schemas/ticket_audits.json` & `tap-zendesk-2.0.1/tap_zendesk/schemas/ticket_audits.json`

 * *Files identical despite different names*

### Comparing `tap-zendesk-2.0.0/tap_zendesk/schemas/ticket_comments.json` & `tap-zendesk-2.0.1/tap_zendesk/schemas/ticket_comments.json`

 * *Files identical despite different names*

### Comparing `tap-zendesk-2.0.0/tap_zendesk/schemas/ticket_fields.json` & `tap-zendesk-2.0.1/tap_zendesk/schemas/ticket_fields.json`

 * *Files identical despite different names*

### Comparing `tap-zendesk-2.0.0/tap_zendesk/schemas/ticket_forms.json` & `tap-zendesk-2.0.1/tap_zendesk/schemas/ticket_forms.json`

 * *Files identical despite different names*

### Comparing `tap-zendesk-2.0.0/tap_zendesk/schemas/ticket_metrics.json` & `tap-zendesk-2.0.1/tap_zendesk/schemas/ticket_metrics.json`

 * *Files identical despite different names*

### Comparing `tap-zendesk-2.0.0/tap_zendesk/schemas/tickets.json` & `tap-zendesk-2.0.1/tap_zendesk/schemas/tickets.json`

 * *Files identical despite different names*

### Comparing `tap-zendesk-2.0.0/tap_zendesk/schemas/users.json` & `tap-zendesk-2.0.1/tap_zendesk/schemas/users.json`

 * *Files identical despite different names*

### Comparing `tap-zendesk-2.0.0/tap_zendesk/streams.py` & `tap-zendesk-2.0.1/tap_zendesk/streams.py`

 * *Files identical despite different names*

### Comparing `tap-zendesk-2.0.0/tap_zendesk/sync.py` & `tap-zendesk-2.0.1/tap_zendesk/sync.py`

 * *Files identical despite different names*

### Comparing `tap-zendesk-2.0.0/tap_zendesk.egg-info/SOURCES.txt` & `tap-zendesk-2.0.1/tap_zendesk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tap-zendesk-2.0.0/test/test_all_fields.py` & `tap-zendesk-2.0.1/test/test_all_fields.py`

 * *Files identical despite different names*

### Comparing `tap-zendesk-2.0.0/test/test_all_streams.py` & `tap-zendesk-2.0.1/test/test_all_streams.py`

 * *Files identical despite different names*

### Comparing `tap-zendesk-2.0.0/test/test_automatic_fields.py` & `tap-zendesk-2.0.1/test/test_automatic_fields.py`

 * *Files identical despite different names*

### Comparing `tap-zendesk-2.0.0/test/test_bookmarks.py` & `tap-zendesk-2.0.1/test/test_bookmarks.py`

 * *Files identical despite different names*

### Comparing `tap-zendesk-2.0.0/test/test_custom_fields_discover.py` & `tap-zendesk-2.0.1/test/test_custom_fields_discover.py`

 * *Files identical despite different names*

### Comparing `tap-zendesk-2.0.0/test/test_discovery.py` & `tap-zendesk-2.0.1/test/test_discovery.py`

 * *Files identical despite different names*

### Comparing `tap-zendesk-2.0.0/test/test_minimal_selection.py` & `tap-zendesk-2.0.1/test/test_minimal_selection.py`

 * *Files identical despite different names*

### Comparing `tap-zendesk-2.0.0/test/test_pagination.py` & `tap-zendesk-2.0.1/test/test_pagination.py`

 * *Files identical despite different names*

### Comparing `tap-zendesk-2.0.0/test/test_standard_bookmark.py` & `tap-zendesk-2.0.1/test/test_standard_bookmark.py`

 * *Files identical despite different names*

### Comparing `tap-zendesk-2.0.0/test/test_start_date.py` & `tap-zendesk-2.0.1/test/test_start_date.py`

 * *Files identical despite different names*

