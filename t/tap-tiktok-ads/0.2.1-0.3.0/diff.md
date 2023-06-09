# Comparing `tmp/tap-tiktok-ads-0.2.1.tar.gz` & `tmp/tap-tiktok-ads-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap-tiktok-ads-0.2.1.tar", last modified: Thu Feb  9 18:15:53 2023, max compression
+gzip compressed data, was "tap-tiktok-ads-0.3.0.tar", last modified: Fri Jun  9 07:47:42 2023, max compression
```

## Comparing `tap-tiktok-ads-0.2.1.tar` & `tap-tiktok-ads-0.3.0.tar`

### file list

```diff
@@ -1,30 +1,38 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-09 18:15:53.396255 tap-tiktok-ads-0.2.1/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32387 2023-01-31 11:09:28.000000 tap-tiktok-ads-0.2.1/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       54 2023-01-31 11:09:28.000000 tap-tiktok-ads-0.2.1/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      297 2023-02-09 18:15:53.396255 tap-tiktok-ads-0.2.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7970 2023-01-31 11:09:28.000000 tap-tiktok-ads-0.2.1/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       79 2023-02-09 18:15:53.400255 tap-tiktok-ads-0.2.1/setup.cfg
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)      790 2023-02-09 17:53:10.000000 tap-tiktok-ads-0.2.1/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-09 18:15:53.396255 tap-tiktok-ads-0.2.1/tap_tiktok_ads/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1798 2023-02-09 17:53:10.000000 tap-tiktok-ads-0.2.1/tap_tiktok_ads/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7393 2023-02-09 17:53:10.000000 tap-tiktok-ads-0.2.1/tap_tiktok_ads/client.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      674 2023-01-31 11:09:28.000000 tap-tiktok-ads-0.2.1/tap_tiktok_ads/discover.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-09 18:15:53.396255 tap-tiktok-ads-0.2.1/tap_tiktok_ads/schemas/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5078 2023-01-31 11:09:28.000000 tap-tiktok-ads-0.2.1/tap_tiktok_ads/schemas/ad_insights.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3153 2023-01-31 11:09:28.000000 tap-tiktok-ads-0.2.1/tap_tiktok_ads/schemas/ad_insights_by_age_and_gender.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3082 2023-01-31 11:09:28.000000 tap-tiktok-ads-0.2.1/tap_tiktok_ads/schemas/ad_insights_by_country.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3078 2023-01-31 11:09:28.000000 tap-tiktok-ads-0.2.1/tap_tiktok_ads/schemas/ad_insights_by_platform.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10070 2023-02-09 17:53:10.000000 tap-tiktok-ads-0.2.1/tap_tiktok_ads/schemas/adgroups.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3802 2023-01-31 11:09:28.000000 tap-tiktok-ads-0.2.1/tap_tiktok_ads/schemas/ads.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2095 2023-01-31 11:09:28.000000 tap-tiktok-ads-0.2.1/tap_tiktok_ads/schemas/advertisers.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1531 2023-02-09 17:53:10.000000 tap-tiktok-ads-0.2.1/tap_tiktok_ads/schemas/campaigns.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1009 2023-01-31 11:09:28.000000 tap-tiktok-ads-0.2.1/tap_tiktok_ads/schemas.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16979 2023-02-09 17:53:10.000000 tap-tiktok-ads-0.2.1/tap_tiktok_ads/streams.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1630 2023-02-09 17:53:10.000000 tap-tiktok-ads-0.2.1/tap_tiktok_ads/sync.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-09 18:15:53.396255 tap-tiktok-ads-0.2.1/tap_tiktok_ads.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      297 2023-02-09 18:15:53.000000 tap-tiktok-ads-0.2.1/tap_tiktok_ads.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      780 2023-02-09 18:15:53.000000 tap-tiktok-ads-0.2.1/tap_tiktok_ads.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-02-09 18:15:53.000000 tap-tiktok-ads-0.2.1/tap_tiktok_ads.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       66 2023-02-09 18:15:53.000000 tap-tiktok-ads-0.2.1/tap_tiktok_ads.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       79 2023-02-09 18:15:53.000000 tap-tiktok-ads-0.2.1/tap_tiktok_ads.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       15 2023-02-09 18:15:53.000000 tap-tiktok-ads-0.2.1/tap_tiktok_ads.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-09 07:47:42.125490 tap-tiktok-ads-0.3.0/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32387 2022-09-02 08:09:40.000000 tap-tiktok-ads-0.3.0/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       54 2022-09-02 08:09:40.000000 tap-tiktok-ads-0.3.0/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      263 2023-06-09 07:47:42.125490 tap-tiktok-ads-0.3.0/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7970 2022-09-02 08:09:40.000000 tap-tiktok-ads-0.3.0/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       79 2023-06-09 07:47:42.125490 tap-tiktok-ads-0.3.0/setup.cfg
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)      790 2023-06-09 06:51:29.000000 tap-tiktok-ads-0.3.0/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-09 07:47:42.121490 tap-tiktok-ads-0.3.0/tap_tiktok_ads/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1798 2023-05-24 06:51:41.000000 tap-tiktok-ads-0.3.0/tap_tiktok_ads/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7638 2023-06-09 06:51:29.000000 tap-tiktok-ads-0.3.0/tap_tiktok_ads/client.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      674 2022-09-02 08:09:40.000000 tap-tiktok-ads-0.3.0/tap_tiktok_ads/discover.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-09 07:47:42.125490 tap-tiktok-ads-0.3.0/tap_tiktok_ads/schemas/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5078 2022-09-02 08:09:40.000000 tap-tiktok-ads-0.3.0/tap_tiktok_ads/schemas/ad_insights.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3153 2022-09-02 08:09:40.000000 tap-tiktok-ads-0.3.0/tap_tiktok_ads/schemas/ad_insights_by_age_and_gender.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3082 2022-09-02 08:09:40.000000 tap-tiktok-ads-0.3.0/tap_tiktok_ads/schemas/ad_insights_by_country.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3078 2022-09-02 08:09:40.000000 tap-tiktok-ads-0.3.0/tap_tiktok_ads/schemas/ad_insights_by_platform.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10070 2023-05-16 05:53:52.000000 tap-tiktok-ads-0.3.0/tap_tiktok_ads/schemas/adgroups.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3802 2022-09-02 08:09:40.000000 tap-tiktok-ads-0.3.0/tap_tiktok_ads/schemas/ads.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2095 2022-09-02 08:09:40.000000 tap-tiktok-ads-0.3.0/tap_tiktok_ads/schemas/advertisers.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1531 2023-05-16 05:53:52.000000 tap-tiktok-ads-0.3.0/tap_tiktok_ads/schemas/campaigns.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1009 2022-09-02 08:09:40.000000 tap-tiktok-ads-0.3.0/tap_tiktok_ads/schemas.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16979 2023-05-16 05:53:52.000000 tap-tiktok-ads-0.3.0/tap_tiktok_ads/streams.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1630 2023-05-26 18:02:58.000000 tap-tiktok-ads-0.3.0/tap_tiktok_ads/sync.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-09 07:47:42.121490 tap-tiktok-ads-0.3.0/tap_tiktok_ads.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      263 2023-06-09 07:47:41.000000 tap-tiktok-ads-0.3.0/tap_tiktok_ads.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      965 2023-06-09 07:47:42.000000 tap-tiktok-ads-0.3.0/tap_tiktok_ads.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-09 07:47:41.000000 tap-tiktok-ads-0.3.0/tap_tiktok_ads.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       55 2023-06-09 07:47:41.000000 tap-tiktok-ads-0.3.0/tap_tiktok_ads.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       79 2023-06-09 07:47:41.000000 tap-tiktok-ads-0.3.0/tap_tiktok_ads.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       15 2023-06-09 07:47:41.000000 tap-tiktok-ads-0.3.0/tap_tiktok_ads.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-09 07:47:42.125490 tap-tiktok-ads-0.3.0/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4633 2023-05-16 05:53:52.000000 tap-tiktok-ads-0.3.0/tests/test_all_fields.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2269 2023-05-16 05:53:52.000000 tap-tiktok-ads-0.3.0/tests/test_automatic_fields.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8049 2023-05-16 05:53:52.000000 tap-tiktok-ads-0.3.0/tests/test_bookmarks.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6083 2023-05-16 05:53:52.000000 tap-tiktok-ads-0.3.0/tests/test_discovery.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9068 2023-06-09 06:51:29.000000 tap-tiktok-ads-0.3.0/tests/test_interrupted_sync.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3174 2023-05-16 05:53:52.000000 tap-tiktok-ads-0.3.0/tests/test_pagination.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7075 2023-06-09 06:51:29.000000 tap-tiktok-ads-0.3.0/tests/test_start_date.py
```

### Comparing `tap-tiktok-ads-0.2.1/LICENSE` & `tap-tiktok-ads-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tap-tiktok-ads-0.2.1/README.md` & `tap-tiktok-ads-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `tap-tiktok-ads-0.2.1/setup.py` & `tap-tiktok-ads-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name="tap-tiktok-ads",
-    version="0.2.1",
+    version="0.3.0",
     description="Singer.io tap for extracting data",
     author="Stitch",
     url="http://singer.io",
     classifiers=["Programming Language :: Python :: 3 :: Only"],
     py_modules=["tap_tiktok_ads"],
     install_requires=[
         "singer-python==5.13.0",
```

### Comparing `tap-tiktok-ads-0.2.1/tap_tiktok_ads/__init__.py` & `tap-tiktok-ads-0.3.0/tap_tiktok_ads/__init__.py`

 * *Files identical despite different names*

### Comparing `tap-tiktok-ads-0.2.1/tap_tiktok_ads/client.py` & `tap-tiktok-ads-0.3.0/tap_tiktok_ads/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,17 +24,20 @@
         self.message = message
         self.response = response
 
 def should_retry(e):
     """ Return true if exception is required to retry otherwise return false """
     response = e.response
     error_code = response.json().get("code")
-    # Backoff in case of 50000 error code. Refer doc: https://ads.tiktok.com/marketing_api/docs?id=1714940022762498 
+    # Backoff in case of below error codes. Refer doc: https://ads.tiktok.com/marketing_api/docs?rid=xmtaqatxqj8&id=1737172488964097
     # for more information.
-    if error_code == 50000:
+    if error_code in (40200, 40201, 40202, 40700, 50000, 50002):
+        return True
+    if (type(e) == Exception and type(e.args[0][1]) == ConnectionResetError) or type(e) == ConnectionResetError:
+        # Tap raises Exception: ConnectionResetError(104, 'Connection reset by peer').
         return True
 
 class TikTokClient:
     def __init__(self,
                  access_token,
                  advertiser_id,
                  sandbox=False,
@@ -60,15 +63,15 @@
             self.__request_timeout = float(request_timeout)
         else:
             self.__request_timeout = REQUEST_TIMEOUT
 
     # Backoff the request after 5 minutes in case of 50000 error code
     @backoff.on_exception(backoff.constant,
                           (TikTokAdsClientError),
-                          max_time=600, # 10 minutes
+                          max_tries=3,
                           interval=300, # 5 minutes
                           giveup=lambda e: not should_retry(e),
                           jitter=None)
     @backoff.on_exception(backoff.expo,
                           requests.Timeout, # backoff for "Timeout" error
                           max_tries=MAX_TRIES,
                           factor=2)
@@ -115,15 +118,15 @@
             adv_response = self.get(path='advertiser/info/', headers=headers,
                                         params=params)
             return bool(adv_response.get('message') == 'OK')
 
     # Backoff the request after 5 minutes in case of 50000 error code
     @backoff.on_exception(backoff.constant,
                           (TikTokAdsClientError),
-                          max_time=600, # 10 minutes
+                          max_tries=3,
                           interval=300, # 5 minutes
                           giveup=lambda e: not should_retry(e),
                           jitter=None)
     @backoff.on_exception(backoff.expo,
                           requests.Timeout, # backoff for "Timeout" error
                           max_tries=MAX_TRIES,
                           factor=2)
```

### Comparing `tap-tiktok-ads-0.2.1/tap_tiktok_ads/discover.py` & `tap-tiktok-ads-0.3.0/tap_tiktok_ads/discover.py`

 * *Files identical despite different names*

### Comparing `tap-tiktok-ads-0.2.1/tap_tiktok_ads/schemas/ad_insights.json` & `tap-tiktok-ads-0.3.0/tap_tiktok_ads/schemas/ad_insights.json`

 * *Files identical despite different names*

### Comparing `tap-tiktok-ads-0.2.1/tap_tiktok_ads/schemas/ad_insights_by_age_and_gender.json` & `tap-tiktok-ads-0.3.0/tap_tiktok_ads/schemas/ad_insights_by_age_and_gender.json`

 * *Files identical despite different names*

### Comparing `tap-tiktok-ads-0.2.1/tap_tiktok_ads/schemas/ad_insights_by_country.json` & `tap-tiktok-ads-0.3.0/tap_tiktok_ads/schemas/ad_insights_by_country.json`

 * *Files identical despite different names*

### Comparing `tap-tiktok-ads-0.2.1/tap_tiktok_ads/schemas/ad_insights_by_platform.json` & `tap-tiktok-ads-0.3.0/tap_tiktok_ads/schemas/ad_insights_by_platform.json`

 * *Files identical despite different names*

### Comparing `tap-tiktok-ads-0.2.1/tap_tiktok_ads/schemas/adgroups.json` & `tap-tiktok-ads-0.3.0/tap_tiktok_ads/schemas/adgroups.json`

 * *Files identical despite different names*

### Comparing `tap-tiktok-ads-0.2.1/tap_tiktok_ads/schemas/ads.json` & `tap-tiktok-ads-0.3.0/tap_tiktok_ads/schemas/ads.json`

 * *Files identical despite different names*

### Comparing `tap-tiktok-ads-0.2.1/tap_tiktok_ads/schemas/advertisers.json` & `tap-tiktok-ads-0.3.0/tap_tiktok_ads/schemas/advertisers.json`

 * *Files identical despite different names*

### Comparing `tap-tiktok-ads-0.2.1/tap_tiktok_ads/schemas/campaigns.json` & `tap-tiktok-ads-0.3.0/tap_tiktok_ads/schemas/campaigns.json`

 * *Files identical despite different names*

### Comparing `tap-tiktok-ads-0.2.1/tap_tiktok_ads/schemas.py` & `tap-tiktok-ads-0.3.0/tap_tiktok_ads/schemas.py`

 * *Files identical despite different names*

### Comparing `tap-tiktok-ads-0.2.1/tap_tiktok_ads/streams.py` & `tap-tiktok-ads-0.3.0/tap_tiktok_ads/streams.py`

 * *Files identical despite different names*

### Comparing `tap-tiktok-ads-0.2.1/tap_tiktok_ads/sync.py` & `tap-tiktok-ads-0.3.0/tap_tiktok_ads/sync.py`

 * *Files identical despite different names*

### Comparing `tap-tiktok-ads-0.2.1/tap_tiktok_ads.egg-info/SOURCES.txt` & `tap-tiktok-ads-0.3.0/tap_tiktok_ads.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -18,8 +18,15 @@
 tap_tiktok_ads/schemas/ad_insights.json
 tap_tiktok_ads/schemas/ad_insights_by_age_and_gender.json
 tap_tiktok_ads/schemas/ad_insights_by_country.json
 tap_tiktok_ads/schemas/ad_insights_by_platform.json
 tap_tiktok_ads/schemas/adgroups.json
 tap_tiktok_ads/schemas/ads.json
 tap_tiktok_ads/schemas/advertisers.json
-tap_tiktok_ads/schemas/campaigns.json
+tap_tiktok_ads/schemas/campaigns.json
+tests/test_all_fields.py
+tests/test_automatic_fields.py
+tests/test_bookmarks.py
+tests/test_discovery.py
+tests/test_interrupted_sync.py
+tests/test_pagination.py
+tests/test_start_date.py
```

