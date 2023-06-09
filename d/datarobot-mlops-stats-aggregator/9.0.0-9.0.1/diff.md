# Comparing `tmp/datarobot_mlops_stats_aggregator-9.0.0-py2.py3-none-any.whl.zip` & `tmp/datarobot_mlops_stats_aggregator-9.0.1-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
 Zip file size: 17011 bytes, number of entries: 11
--rw-r--r--  2.0 unx      812 b- defN 23-Feb-16 20:33 datarobot/mlops/stats_aggregator/__init__.py
--rw-r--r--  2.0 unx    15046 b- defN 23-Feb-16 20:33 datarobot/mlops/stats_aggregator/aggregation.py
--rw-r--r--  2.0 unx      888 b- defN 23-Feb-16 20:33 datarobot/mlops/stats_aggregator/constants.py
--rw-r--r--  2.0 unx     6528 b- defN 23-Feb-16 20:33 datarobot/mlops/stats_aggregator/histogram.py
--rw-r--r--  2.0 unx    12097 b- defN 23-Feb-16 20:33 datarobot/mlops/stats_aggregator/merging.py
--rw-r--r--  2.0 unx     9380 b- defN 23-Feb-16 20:33 datarobot/mlops/stats_aggregator/type_conversion.py
--rw-r--r--  2.0 unx     2982 b- defN 23-Feb-16 20:33 datarobot/mlops/stats_aggregator/types.py
--rw-r--r--  2.0 unx     2201 b- defN 23-Feb-16 20:34 datarobot_mlops_stats_aggregator-9.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Feb-16 20:34 datarobot_mlops_stats_aggregator-9.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Feb-16 20:34 datarobot_mlops_stats_aggregator-9.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1114 b- defN 23-Feb-16 20:34 datarobot_mlops_stats_aggregator-9.0.0.dist-info/RECORD
-11 files, 51168 bytes uncompressed, 15065 bytes compressed:  70.6%
+-rw-r--r--  2.0 unx      812 b- defN 23-Jun-09 20:57 datarobot/mlops/stats_aggregator/__init__.py
+-rw-r--r--  2.0 unx    15046 b- defN 23-Jun-09 20:57 datarobot/mlops/stats_aggregator/aggregation.py
+-rw-r--r--  2.0 unx      888 b- defN 23-Jun-09 20:57 datarobot/mlops/stats_aggregator/constants.py
+-rw-r--r--  2.0 unx     6528 b- defN 23-Jun-09 20:57 datarobot/mlops/stats_aggregator/histogram.py
+-rw-r--r--  2.0 unx    12097 b- defN 23-Jun-09 20:57 datarobot/mlops/stats_aggregator/merging.py
+-rw-r--r--  2.0 unx     9370 b- defN 23-Jun-09 20:57 datarobot/mlops/stats_aggregator/type_conversion.py
+-rw-r--r--  2.0 unx     2982 b- defN 23-Jun-09 20:57 datarobot/mlops/stats_aggregator/types.py
+-rw-r--r--  2.0 unx     2201 b- defN 23-Jun-09 20:58 datarobot_mlops_stats_aggregator-9.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jun-09 20:58 datarobot_mlops_stats_aggregator-9.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Jun-09 20:58 datarobot_mlops_stats_aggregator-9.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1114 b- defN 23-Jun-09 20:58 datarobot_mlops_stats_aggregator-9.0.1.dist-info/RECORD
+11 files, 51158 bytes uncompressed, 15065 bytes compressed:  70.6%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: datarobot/mlops/stats_aggregator/type_conversion.py
 Comment: 
 
 Filename: datarobot/mlops/stats_aggregator/types.py
 Comment: 
 
-Filename: datarobot_mlops_stats_aggregator-9.0.0.dist-info/METADATA
+Filename: datarobot_mlops_stats_aggregator-9.0.1.dist-info/METADATA
 Comment: 
 
-Filename: datarobot_mlops_stats_aggregator-9.0.0.dist-info/WHEEL
+Filename: datarobot_mlops_stats_aggregator-9.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: datarobot_mlops_stats_aggregator-9.0.0.dist-info/top_level.txt
+Filename: datarobot_mlops_stats_aggregator-9.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: datarobot_mlops_stats_aggregator-9.0.0.dist-info/RECORD
+Filename: datarobot_mlops_stats_aggregator-9.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## datarobot/mlops/stats_aggregator/__init__.py

```diff
@@ -14,8 +14,8 @@
 from __future__ import absolute_import
 
 from .aggregation import aggregate_stats
 from .merging import merge_stats
 from .types import FeatureType
 
 __all__ = ["aggregate_stats", "merge_stats", "FeatureType"]
-__version__ = '9.0.0'
+__version__ = '9.0.1'
```

## datarobot/mlops/stats_aggregator/type_conversion.py

```diff
@@ -41,15 +41,15 @@
     Return np.nan if value can't be converted.
 
     Based on common.utilities.metadata.date2int, but without fancy error handling.
     """
     if x == "" or x is None or pd.isnull(x) or x == "nan":
         return np.nan
 
-    if isinstance(x, (float, np.float, np.float32, np.float64)):
+    if isinstance(x, (float, np.float32, np.float64)):
         if float.is_integer(x):
             x = int(x)
     try:
         return d2iw.date2intWrapper(six.text_type(x), fmt.encode("utf-8"), skip_tz=skip_tz)
 
     except (ValueError, TypeError):
         # Unlike common.utilities.metadata.date2int, always return np.nan if a value won't convert
```

## Comparing `datarobot_mlops_stats_aggregator-9.0.0.dist-info/METADATA` & `datarobot_mlops_stats_aggregator-9.0.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datarobot-mlops-stats-aggregator
-Version: 9.0.0
+Version: 9.0.1
 Summary: datarobot-mlops-stats-aggregator library to compute statistics aggregations
 Home-page: http://datarobot.com
 Author: DataRobot
 Author-email: info@datarobot.com
 License: DataRobot Tool and Utility Agreement
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `datarobot_mlops_stats_aggregator-9.0.0.dist-info/RECORD` & `datarobot_mlops_stats_aggregator-9.0.1.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-datarobot/mlops/stats_aggregator/__init__.py,sha256=TO6eBT3a3IepIiVjZxbPd7adGjhc08S8O9Jr3IEUsXU,812
+datarobot/mlops/stats_aggregator/__init__.py,sha256=khSs_eRhD2_Q2jiczwWsVbMqqcJMLltncA_uZ7ZlfPY,812
 datarobot/mlops/stats_aggregator/aggregation.py,sha256=X5am7_M0vqqX3ZmnkPjhv286FW7U2Z1FRu701dXIKGc,15046
 datarobot/mlops/stats_aggregator/constants.py,sha256=e-pqtDD2dlXXTfcUYz4AL5GgkrMrOP3XChklh9iRB8g,888
 datarobot/mlops/stats_aggregator/histogram.py,sha256=KtA0hwIyT9wG-3LjFYnixqBlFMgywWjuhrXPgxIopwE,6528
 datarobot/mlops/stats_aggregator/merging.py,sha256=wr-2MZunpk-iR4UTsNX1ivEieZbkadNOhMU4YT7oWQw,12097
-datarobot/mlops/stats_aggregator/type_conversion.py,sha256=2ZpBicsudV_gOtZt8qGbfeKyQ2LjwpFPGtLAOh5GdzY,9380
+datarobot/mlops/stats_aggregator/type_conversion.py,sha256=9qBpD8zV_Hx3ZDX80h_DPnsYr0kzy0dYJ7O2iiWKNUA,9370
 datarobot/mlops/stats_aggregator/types.py,sha256=zdCg-5lDIH2MhbgRFt-Mlt6wvnm9oPGJngydJOlPSy8,2982
-datarobot_mlops_stats_aggregator-9.0.0.dist-info/METADATA,sha256=Drkwa4mpOPGW7YtOIfMaLMRgaJVu5jM1SayVzBfTOTY,2201
-datarobot_mlops_stats_aggregator-9.0.0.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-datarobot_mlops_stats_aggregator-9.0.0.dist-info/top_level.txt,sha256=RTK5ZHErXe7mZUlXWQRjQpqFdWw3qmpF95Lz7ViL2Lc,10
-datarobot_mlops_stats_aggregator-9.0.0.dist-info/RECORD,,
+datarobot_mlops_stats_aggregator-9.0.1.dist-info/METADATA,sha256=HvtGk7AwBugZP23HD3ih0qRvlWVaVUOew_YshstCobw,2201
+datarobot_mlops_stats_aggregator-9.0.1.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+datarobot_mlops_stats_aggregator-9.0.1.dist-info/top_level.txt,sha256=RTK5ZHErXe7mZUlXWQRjQpqFdWw3qmpF95Lz7ViL2Lc,10
+datarobot_mlops_stats_aggregator-9.0.1.dist-info/RECORD,,
```

