# Comparing `tmp/poe_api-0.4.5-py3-none-any.whl.zip` & `tmp/poe_api-0.4.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 40872 bytes, number of entries: 42
--rw-r--r--  2.0 unx    21084 b- defN 23-Jun-07 21:13 poe.py
+Zip file size: 40873 bytes, number of entries: 42
+-rw-r--r--  2.0 unx    21094 b- defN 23-Jun-09 20:19 poe.py
 -rw-r--r--  2.0 unx     1093 b- defN 23-May-27 23:16 poe_graphql/AddHumanMessageMutation.graphql
 -rw-r--r--  2.0 unx      504 b- defN 23-Jun-04 03:20 poe_graphql/AddMessageBreakMutation.graphql
 -rw-r--r--  2.0 unx      180 b- defN 23-May-27 23:16 poe_graphql/AutoSubscriptionMutation.graphql
 -rw-r--r--  2.0 unx       97 b- defN 23-May-27 23:16 poe_graphql/BioFragment.graphql
 -rw-r--r--  2.0 unx       73 b- defN 23-May-27 23:16 poe_graphql/ChatAddedSubscription.graphql
 -rw-r--r--  2.0 unx      100 b- defN 23-May-27 23:16 poe_graphql/ChatFragment.graphql
 -rw-r--r--  2.0 unx    11486 b- defN 23-Jun-04 03:16 poe_graphql/ChatListPaginationQuery.graphql
@@ -32,13 +32,13 @@
 -rw-r--r--  2.0 unx      147 b- defN 23-May-27 23:16 poe_graphql/SummarizeQuotePostQuery.graphql
 -rw-r--r--  2.0 unx      180 b- defN 23-May-27 23:16 poe_graphql/SummarizeSharePostQuery.graphql
 -rw-r--r--  2.0 unx      368 b- defN 23-May-27 23:16 poe_graphql/UserSnippetFragment.graphql
 -rw-r--r--  2.0 unx      400 b- defN 23-May-27 23:16 poe_graphql/ViewerInfoQuery.graphql
 -rw-r--r--  2.0 unx     1038 b- defN 23-May-27 23:16 poe_graphql/ViewerStateFragment.graphql
 -rw-r--r--  2.0 unx      657 b- defN 23-May-27 23:16 poe_graphql/ViewerStateUpdatedSubscription.graphql
 -rw-r--r--  2.0 unx        0 b- defN 23-May-27 23:16 poe_graphql/__init__.py
--rw-r--r--  2.0 unx    35149 b- defN 23-Jun-07 21:16 poe_api-0.4.5.dist-info/LICENSE
--rw-r--r--  2.0 unx    18099 b- defN 23-Jun-07 21:16 poe_api-0.4.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-07 21:16 poe_api-0.4.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-Jun-07 21:16 poe_api-0.4.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     3969 b- defN 23-Jun-07 21:16 poe_api-0.4.5.dist-info/RECORD
-42 files, 104687 bytes uncompressed, 34330 bytes compressed:  67.2%
+-rw-r--r--  2.0 unx    35149 b- defN 23-Jun-09 20:21 poe_api-0.4.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx    18099 b- defN 23-Jun-09 20:21 poe_api-0.4.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-09 20:21 poe_api-0.4.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-Jun-09 20:21 poe_api-0.4.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     3969 b- defN 23-Jun-09 20:21 poe_api-0.4.6.dist-info/RECORD
+42 files, 104697 bytes uncompressed, 34331 bytes compressed:  67.2%
```

## zipnote {}

```diff
@@ -105,23 +105,23 @@
 
 Filename: poe_graphql/ViewerStateUpdatedSubscription.graphql
 Comment: 
 
 Filename: poe_graphql/__init__.py
 Comment: 
 
-Filename: poe_api-0.4.5.dist-info/LICENSE
+Filename: poe_api-0.4.6.dist-info/LICENSE
 Comment: 
 
-Filename: poe_api-0.4.5.dist-info/METADATA
+Filename: poe_api-0.4.6.dist-info/METADATA
 Comment: 
 
-Filename: poe_api-0.4.5.dist-info/WHEEL
+Filename: poe_api-0.4.6.dist-info/WHEEL
 Comment: 
 
-Filename: poe_api-0.4.5.dist-info/top_level.txt
+Filename: poe_api-0.4.6.dist-info/top_level.txt
 Comment: 
 
-Filename: poe_api-0.4.5.dist-info/RECORD
+Filename: poe_api-0.4.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## poe.py

```diff
@@ -212,15 +212,15 @@
   def get_bots(self, download_next_data=True):
     logger.info("Downloading all bots...")
     if download_next_data:
       next_data = self.get_next_data(overwrite_vars=True)
     else:
       next_data = self.next_data
 
-    if not "availableBots" in self.viewer:
+    if not "availableBotsConnection" in self.viewer:
       raise RuntimeError("Invalid token or no bots are available.")
     bot_list_url = f'https://poe.com/_next/data/{self.next_data["buildId"]}/index.json'
     bot_list = self.viewer["availableBotsConnection"]["edges"]
 
     threads = []
     bots = {}
```

## Comparing `poe_api-0.4.5.dist-info/LICENSE` & `poe_api-0.4.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `poe_api-0.4.5.dist-info/METADATA` & `poe_api-0.4.6.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poe-api
-Version: 0.4.5
+Version: 0.4.6
 Summary: A reverse engineered API wrapper for Quora's Poe
 Home-page: https://github.com/ading2210/poe-api
 Author: ading2210
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
```

## Comparing `poe_api-0.4.5.dist-info/RECORD` & `poe_api-0.4.6.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-poe.py,sha256=bqi7hmx35knTE23MMMVw0DWdLM4Z0LsXd5RTq4hs4Og,21084
+poe.py,sha256=CQ4qwqH49eDzNumBwiKITQzgLivG6DiX0Ja4etOhZNI,21094
 poe_graphql/AddHumanMessageMutation.graphql,sha256=Va4SoysKE2qPlJfbwoKp6mNv0vs5hnVR20g8hPvAxdY,1093
 poe_graphql/AddMessageBreakMutation.graphql,sha256=lFDgYYX0ZTHso-ZQwm-oUk-HaSTRqOmj-zIjBQRL2sM,504
 poe_graphql/AutoSubscriptionMutation.graphql,sha256=3i8EnqwUrjOcJ2Hxly-lKhwPBJdbpO99POiM_K6jVD4,180
 poe_graphql/BioFragment.graphql,sha256=3ZdXaPtuHK38bG10WFH6bvpebcyrTLu5fs-ddtfLjf0,97
 poe_graphql/ChatAddedSubscription.graphql,sha256=NFLZJAwi0V2WQea1oelyRUrtNrwOE58NOeX8ChzVE10,73
 poe_graphql/ChatFragment.graphql,sha256=NFVSvT3NdYlEquue3yTHPu9ezCIgx6k1OXJZo2ytIzU,100
 poe_graphql/ChatListPaginationQuery.graphql,sha256=WameJV_yyS6Ey_VKn7okXAzR45AE9wOB2U6QlRgp-M4,11486
@@ -31,12 +31,12 @@
 poe_graphql/SummarizeQuotePostQuery.graphql,sha256=V4PQ1XkEDCsVR3z7h4SLsonZsWG7RptFd6JPwlGwOvE,147
 poe_graphql/SummarizeSharePostQuery.graphql,sha256=iCN8oiUUp2jfsiBxmsTA7k3_60E0MNwA5gnNrhnYpJc,180
 poe_graphql/UserSnippetFragment.graphql,sha256=Eg8rK7XM6-HqVJkpEBY0bJaYqF-FdDdWdg-Jj3VTnF0,368
 poe_graphql/ViewerInfoQuery.graphql,sha256=Xtn-VGGiknKgrW81s7YfIJwhmilobrSqiCObpoJdYfw,400
 poe_graphql/ViewerStateFragment.graphql,sha256=aicUJncsRpPBh_L2xqDv0aHcUIPIsDrDFPfDs3jcFoU,1038
 poe_graphql/ViewerStateUpdatedSubscription.graphql,sha256=1dPs0WuOLl4ybZXm4bUF60eVc94O10EkKOtqnQYODic,657
 poe_graphql/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-poe_api-0.4.5.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-poe_api-0.4.5.dist-info/METADATA,sha256=Qj4akTZ38s2-3n2neht45XUHGrEuRaRCM_adeYmZjJU,18099
-poe_api-0.4.5.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-poe_api-0.4.5.dist-info/top_level.txt,sha256=7Sk_jA5I5n3fNZ1671pcBau4TWZLe6UXCEnCD5NhGGI,16
-poe_api-0.4.5.dist-info/RECORD,,
+poe_api-0.4.6.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+poe_api-0.4.6.dist-info/METADATA,sha256=4CQN1BC_CGbWIubizQw7-fRDpIilWRGDqHEyndyY_gw,18099
+poe_api-0.4.6.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+poe_api-0.4.6.dist-info/top_level.txt,sha256=7Sk_jA5I5n3fNZ1671pcBau4TWZLe6UXCEnCD5NhGGI,16
+poe_api-0.4.6.dist-info/RECORD,,
```

