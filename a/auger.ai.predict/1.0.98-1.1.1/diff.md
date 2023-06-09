# Comparing `tmp/auger.ai.predict-1.0.98-py3-none-any.whl.zip` & `tmp/auger.ai.predict-1.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,81 +1,81 @@
-Zip file size: 131693 bytes, number of entries: 79
--rw-r--r--  2.0 unx    22767 b- defN 22-Mar-23 10:40 auger_ml/AugerMLPreprocessors.py
--rw-r--r--  2.0 unx    16118 b- defN 22-Mar-23 10:40 auger_ml/FSClient.py
--rw-r--r--  2.0 unx     7967 b- defN 22-Mar-23 10:40 auger_ml/LocalFSClient.py
--rw-r--r--  2.0 unx    22415 b- defN 22-Mar-23 10:40 auger_ml/S3FSClient.py
--rw-r--r--  2.0 unx    16617 b- defN 22-Mar-23 10:40 auger_ml/Utils.py
--rw-r--r--  2.0 unx        0 b- defN 22-Mar-23 10:40 auger_ml/__init__.py
--rw-r--r--  2.0 unx     1803 b- defN 22-Mar-23 10:40 auger_ml/celery_logging.py
--rw-r--r--  2.0 unx    12945 b- defN 22-Mar-23 10:40 auger_ml/model_exporter.py
--rw-r--r--  2.0 unx    14926 b- defN 22-Mar-23 10:40 auger_ml/model_helper.py
--rw-r--r--  2.0 unx    16483 b- defN 22-Mar-23 10:40 auger_ml/model_review.py
--rw-r--r--  2.0 unx      389 b- defN 22-Mar-23 10:40 auger_ml/probabilistic_counter.py
--rw-r--r--  2.0 unx     1711 b- defN 22-Mar-23 10:40 auger_ml/warmstart_optimizer.py
--rw-r--r--  2.0 unx        0 b- defN 22-Mar-23 10:40 auger_ml/algorithms/__init__.py
--rw-r--r--  2.0 unx     5014 b- defN 22-Mar-23 10:40 auger_ml/algorithms/adam_wd.py
--rw-r--r--  2.0 unx      162 b- defN 22-Mar-23 10:40 auger_ml/algorithms/baseline.py
--rw-r--r--  2.0 unx     3427 b- defN 22-Mar-23 10:40 auger_ml/algorithms/cat_boost.py
--rw-r--r--  2.0 unx     1042 b- defN 22-Mar-23 10:40 auger_ml/algorithms/dnn.py
--rw-r--r--  2.0 unx    22697 b- defN 22-Mar-23 10:40 auger_ml/algorithms/dnn_base.py
--rw-r--r--  2.0 unx     2157 b- defN 22-Mar-23 10:40 auger_ml/algorithms/dnn_res.py
--rw-r--r--  2.0 unx     5147 b- defN 22-Mar-23 10:40 auger_ml/algorithms/dnn_shaped.py
--rw-r--r--  2.0 unx     1153 b- defN 22-Mar-23 10:40 auger_ml/algorithms/keras_mem.py
--rw-r--r--  2.0 unx     1298 b- defN 22-Mar-23 10:40 auger_ml/algorithms/linear.py
--rw-r--r--  2.0 unx     6782 b- defN 22-Mar-23 10:40 auger_ml/algorithms/mlp.py
--rw-r--r--  2.0 unx     1223 b- defN 22-Mar-23 10:40 auger_ml/algorithms/svm.py
--rw-r--r--  2.0 unx     1743 b- defN 22-Mar-23 10:40 auger_ml/algorithms/timeseries.py
--rw-r--r--  2.0 unx    11030 b- defN 22-Mar-23 10:40 auger_ml/algorithms/ts_dnn.py
--rw-r--r--  2.0 unx    12511 b- defN 22-Mar-23 10:40 auger_ml/algorithms/ts_dnn_cpu.py
--rw-r--r--  2.0 unx     3626 b- defN 22-Mar-23 10:40 auger_ml/algorithms/ts_lstm.py
--rw-r--r--  2.0 unx     1866 b- defN 22-Mar-23 10:40 auger_ml/algorithms/utils.py
--rw-r--r--  2.0 unx        0 b- defN 22-Mar-23 10:40 auger_ml/data_source/__init__.py
--rw-r--r--  2.0 unx     4856 b- defN 22-Mar-23 10:40 auger_ml/data_source/data_source_api.py
--rw-r--r--  2.0 unx    86557 b- defN 22-Mar-23 10:40 auger_ml/data_source/data_source_api_pandas.py
--rw-r--r--  2.0 unx     1123 b- defN 22-Mar-23 10:40 auger_ml/data_source/data_source_api_pandas_proxy.py
--rw-r--r--  2.0 unx     1361 b- defN 22-Mar-23 10:40 auger_ml/data_source/data_source_factory.py
--rw-r--r--  2.0 unx    15064 b- defN 22-Mar-23 10:40 auger_ml/data_source/group_splits.py
--rw-r--r--  2.0 unx      116 b- defN 22-Mar-23 10:40 auger_ml/data_splitters/BaseSplitter.py
--rw-r--r--  2.0 unx      711 b- defN 22-Mar-23 10:40 auger_ml/data_splitters/DFSparkDataPrep.py
--rw-r--r--  2.0 unx     1323 b- defN 22-Mar-23 10:40 auger_ml/data_splitters/SimpleSplitter.py
--rw-r--r--  2.0 unx     2295 b- defN 22-Mar-23 10:40 auger_ml/data_splitters/XYNumpyDataPrep.py
--rw-r--r--  2.0 unx        0 b- defN 22-Mar-23 10:40 auger_ml/data_splitters/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 22-Mar-23 10:40 auger_ml/ensembles/__init__.py
--rw-r--r--  2.0 unx    11044 b- defN 22-Mar-23 10:40 auger_ml/ensembles/algorithms.py
--rw-r--r--  2.0 unx    11014 b- defN 22-Mar-23 10:40 auger_ml/ensembles/base.py
--rw-r--r--  2.0 unx     6948 b- defN 22-Mar-23 10:40 auger_ml/ensembles/build.py
--rw-r--r--  2.0 unx     7541 b- defN 22-Mar-23 10:40 auger_ml/ensembles/deep_ensemble.py
--rw-r--r--  2.0 unx     6044 b- defN 22-Mar-23 10:40 auger_ml/ensembles/deep_super_learner.py
--rw-r--r--  2.0 unx     8981 b- defN 22-Mar-23 10:40 auger_ml/ensembles/greedy_selection.py
--rw-r--r--  2.0 unx     3138 b- defN 22-Mar-23 10:40 auger_ml/ensembles/load_data.py
--rw-r--r--  2.0 unx     1407 b- defN 22-Mar-23 10:40 auger_ml/ensembles/metrics.py
--rw-r--r--  2.0 unx    11820 b- defN 22-Mar-23 10:40 auger_ml/ensembles/super_learner.py
--rw-r--r--  2.0 unx     7087 b- defN 22-Mar-23 10:40 auger_ml/ensembles/utils.py
--rw-r--r--  2.0 unx        0 b- defN 22-Mar-23 10:40 auger_ml/ensembles/space/__init__.py
--rw-r--r--  2.0 unx      918 b- defN 22-Mar-23 10:40 auger_ml/ensembles/space/classifier.py
--rw-r--r--  2.0 unx      267 b- defN 22-Mar-23 10:40 auger_ml/ensembles/space/regressor.py
--rw-r--r--  2.0 unx        0 b- defN 22-Mar-23 10:40 auger_ml/preprocessors/__init__.py
--rw-r--r--  2.0 unx     1509 b- defN 22-Mar-23 10:40 auger_ml/preprocessors/base.py
--rw-r--r--  2.0 unx     3389 b- defN 22-Mar-23 10:40 auger_ml/preprocessors/categorical.py
--rw-r--r--  2.0 unx     2354 b- defN 22-Mar-23 10:40 auger_ml/preprocessors/date_time.py
--rw-r--r--  2.0 unx     1492 b- defN 22-Mar-23 10:40 auger_ml/preprocessors/dim_reduction.py
--rw-r--r--  2.0 unx     1067 b- defN 22-Mar-23 10:40 auger_ml/preprocessors/eliminate.py
--rw-r--r--  2.0 unx     1405 b- defN 22-Mar-23 10:40 auger_ml/preprocessors/extra.py
--rw-r--r--  2.0 unx     2159 b- defN 22-Mar-23 10:40 auger_ml/preprocessors/nan.py
--rw-r--r--  2.0 unx     1607 b- defN 22-Mar-23 10:40 auger_ml/preprocessors/scale.py
--rw-r--r--  2.0 unx    10689 b- defN 22-Mar-23 10:40 auger_ml/preprocessors/space.py
--rw-r--r--  2.0 unx     1911 b- defN 22-Mar-23 10:40 auger_ml/preprocessors/sparse.py
--rw-r--r--  2.0 unx    15532 b- defN 22-Mar-23 10:40 auger_ml/preprocessors/text.py
--rw-r--r--  2.0 unx        0 b- defN 22-Mar-23 10:40 auger_ml/preprocessors/time_series/__init__.py
--rw-r--r--  2.0 unx     1286 b- defN 22-Mar-23 10:40 auger_ml/preprocessors/time_series/embedding.py
--rw-r--r--  2.0 unx      580 b- defN 22-Mar-23 10:40 auger_ml/preprocessors/time_series/interpolate.py
--rw-r--r--  2.0 unx     1266 b- defN 22-Mar-23 10:40 auger_ml/preprocessors/time_series/resample.py
--rw-r--r--  2.0 unx     1524 b- defN 22-Mar-23 10:40 auger_ml/preprocessors/time_series/ssa.py
--rw-r--r--  2.0 unx        0 b- defN 22-Mar-23 10:40 auger_ml/scores/__init__.py
--rw-r--r--  2.0 unx     4269 b- defN 22-Mar-23 10:40 auger_ml/scores/classification.py
--rw-r--r--  2.0 unx     3437 b- defN 22-Mar-23 10:40 auger_ml/scores/regression.py
--rw-r--r--  2.0 unx    11357 b- defN 22-Mar-23 10:40 auger.ai.predict-1.0.98.dist-info/LICENSE
--rw-r--r--  2.0 unx     7046 b- defN 22-Mar-23 10:40 auger.ai.predict-1.0.98.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Mar-23 10:40 auger.ai.predict-1.0.98.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 22-Mar-23 10:40 auger.ai.predict-1.0.98.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     7067 b- defN 22-Mar-23 10:40 auger.ai.predict-1.0.98.dist-info/RECORD
-79 files, 485681 bytes uncompressed, 120389 bytes compressed:  75.2%
+Zip file size: 133536 bytes, number of entries: 79
+-rw-r--r--  2.0 unx    22767 b- defN 23-Jun-09 16:45 auger_ml/AugerMLPreprocessors.py
+-rw-r--r--  2.0 unx    16118 b- defN 23-Jun-09 16:45 auger_ml/FSClient.py
+-rw-r--r--  2.0 unx     7967 b- defN 23-Jun-09 16:45 auger_ml/LocalFSClient.py
+-rw-r--r--  2.0 unx    22439 b- defN 23-Jun-09 16:45 auger_ml/S3FSClient.py
+-rw-r--r--  2.0 unx    18206 b- defN 23-Jun-09 16:45 auger_ml/Utils.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-09 16:45 auger_ml/__init__.py
+-rw-r--r--  2.0 unx     1803 b- defN 23-Jun-09 16:45 auger_ml/celery_logging.py
+-rw-r--r--  2.0 unx    17782 b- defN 23-Jun-09 16:45 auger_ml/model_exporter.py
+-rw-r--r--  2.0 unx    17115 b- defN 23-Jun-09 16:45 auger_ml/model_helper.py
+-rw-r--r--  2.0 unx    16483 b- defN 23-Jun-09 16:45 auger_ml/model_review.py
+-rw-r--r--  2.0 unx      389 b- defN 23-Jun-09 16:45 auger_ml/probabilistic_counter.py
+-rw-r--r--  2.0 unx     1711 b- defN 23-Jun-09 16:45 auger_ml/warmstart_optimizer.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-09 16:45 auger_ml/algorithms/__init__.py
+-rw-r--r--  2.0 unx     5014 b- defN 23-Jun-09 16:45 auger_ml/algorithms/adam_wd.py
+-rw-r--r--  2.0 unx      162 b- defN 23-Jun-09 16:45 auger_ml/algorithms/baseline.py
+-rw-r--r--  2.0 unx     3427 b- defN 23-Jun-09 16:45 auger_ml/algorithms/cat_boost.py
+-rw-r--r--  2.0 unx     1042 b- defN 23-Jun-09 16:45 auger_ml/algorithms/dnn.py
+-rw-r--r--  2.0 unx    22697 b- defN 23-Jun-09 16:45 auger_ml/algorithms/dnn_base.py
+-rw-r--r--  2.0 unx     2157 b- defN 23-Jun-09 16:45 auger_ml/algorithms/dnn_res.py
+-rw-r--r--  2.0 unx     5147 b- defN 23-Jun-09 16:45 auger_ml/algorithms/dnn_shaped.py
+-rw-r--r--  2.0 unx     1153 b- defN 23-Jun-09 16:45 auger_ml/algorithms/keras_mem.py
+-rw-r--r--  2.0 unx     1298 b- defN 23-Jun-09 16:45 auger_ml/algorithms/linear.py
+-rw-r--r--  2.0 unx     6782 b- defN 23-Jun-09 16:45 auger_ml/algorithms/mlp.py
+-rw-r--r--  2.0 unx     1223 b- defN 23-Jun-09 16:45 auger_ml/algorithms/svm.py
+-rw-r--r--  2.0 unx     1743 b- defN 23-Jun-09 16:45 auger_ml/algorithms/timeseries.py
+-rw-r--r--  2.0 unx    11030 b- defN 23-Jun-09 16:45 auger_ml/algorithms/ts_dnn.py
+-rw-r--r--  2.0 unx    12511 b- defN 23-Jun-09 16:45 auger_ml/algorithms/ts_dnn_cpu.py
+-rw-r--r--  2.0 unx     3626 b- defN 23-Jun-09 16:45 auger_ml/algorithms/ts_lstm.py
+-rw-r--r--  2.0 unx     1866 b- defN 23-Jun-09 16:45 auger_ml/algorithms/utils.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-09 16:45 auger_ml/data_source/__init__.py
+-rw-r--r--  2.0 unx     4856 b- defN 23-Jun-09 16:45 auger_ml/data_source/data_source_api.py
+-rw-r--r--  2.0 unx    86619 b- defN 23-Jun-09 16:45 auger_ml/data_source/data_source_api_pandas.py
+-rw-r--r--  2.0 unx     1123 b- defN 23-Jun-09 16:45 auger_ml/data_source/data_source_api_pandas_proxy.py
+-rw-r--r--  2.0 unx     1361 b- defN 23-Jun-09 16:45 auger_ml/data_source/data_source_factory.py
+-rw-r--r--  2.0 unx    15064 b- defN 23-Jun-09 16:45 auger_ml/data_source/group_splits.py
+-rw-r--r--  2.0 unx      116 b- defN 23-Jun-09 16:45 auger_ml/data_splitters/BaseSplitter.py
+-rw-r--r--  2.0 unx      711 b- defN 23-Jun-09 16:45 auger_ml/data_splitters/DFSparkDataPrep.py
+-rw-r--r--  2.0 unx     1323 b- defN 23-Jun-09 16:45 auger_ml/data_splitters/SimpleSplitter.py
+-rw-r--r--  2.0 unx     2295 b- defN 23-Jun-09 16:45 auger_ml/data_splitters/XYNumpyDataPrep.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-09 16:45 auger_ml/data_splitters/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-09 16:45 auger_ml/ensembles/__init__.py
+-rw-r--r--  2.0 unx    11044 b- defN 23-Jun-09 16:45 auger_ml/ensembles/algorithms.py
+-rw-r--r--  2.0 unx    11014 b- defN 23-Jun-09 16:45 auger_ml/ensembles/base.py
+-rw-r--r--  2.0 unx     6948 b- defN 23-Jun-09 16:45 auger_ml/ensembles/build.py
+-rw-r--r--  2.0 unx     7541 b- defN 23-Jun-09 16:45 auger_ml/ensembles/deep_ensemble.py
+-rw-r--r--  2.0 unx     6044 b- defN 23-Jun-09 16:45 auger_ml/ensembles/deep_super_learner.py
+-rw-r--r--  2.0 unx     8981 b- defN 23-Jun-09 16:45 auger_ml/ensembles/greedy_selection.py
+-rw-r--r--  2.0 unx     3138 b- defN 23-Jun-09 16:45 auger_ml/ensembles/load_data.py
+-rw-r--r--  2.0 unx     1407 b- defN 23-Jun-09 16:45 auger_ml/ensembles/metrics.py
+-rw-r--r--  2.0 unx    11820 b- defN 23-Jun-09 16:45 auger_ml/ensembles/super_learner.py
+-rw-r--r--  2.0 unx     7087 b- defN 23-Jun-09 16:45 auger_ml/ensembles/utils.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-09 16:45 auger_ml/ensembles/space/__init__.py
+-rw-r--r--  2.0 unx      918 b- defN 23-Jun-09 16:45 auger_ml/ensembles/space/classifier.py
+-rw-r--r--  2.0 unx      267 b- defN 23-Jun-09 16:45 auger_ml/ensembles/space/regressor.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-09 16:45 auger_ml/preprocessors/__init__.py
+-rw-r--r--  2.0 unx     1509 b- defN 23-Jun-09 16:45 auger_ml/preprocessors/base.py
+-rw-r--r--  2.0 unx     3389 b- defN 23-Jun-09 16:45 auger_ml/preprocessors/categorical.py
+-rw-r--r--  2.0 unx     2354 b- defN 23-Jun-09 16:45 auger_ml/preprocessors/date_time.py
+-rw-r--r--  2.0 unx     1492 b- defN 23-Jun-09 16:45 auger_ml/preprocessors/dim_reduction.py
+-rw-r--r--  2.0 unx     1067 b- defN 23-Jun-09 16:45 auger_ml/preprocessors/eliminate.py
+-rw-r--r--  2.0 unx     1405 b- defN 23-Jun-09 16:45 auger_ml/preprocessors/extra.py
+-rw-r--r--  2.0 unx     2159 b- defN 23-Jun-09 16:45 auger_ml/preprocessors/nan.py
+-rw-r--r--  2.0 unx     1607 b- defN 23-Jun-09 16:45 auger_ml/preprocessors/scale.py
+-rw-r--r--  2.0 unx    10689 b- defN 23-Jun-09 16:45 auger_ml/preprocessors/space.py
+-rw-r--r--  2.0 unx     1911 b- defN 23-Jun-09 16:45 auger_ml/preprocessors/sparse.py
+-rw-r--r--  2.0 unx    15532 b- defN 23-Jun-09 16:45 auger_ml/preprocessors/text.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-09 16:45 auger_ml/preprocessors/time_series/__init__.py
+-rw-r--r--  2.0 unx     1286 b- defN 23-Jun-09 16:45 auger_ml/preprocessors/time_series/embedding.py
+-rw-r--r--  2.0 unx      580 b- defN 23-Jun-09 16:45 auger_ml/preprocessors/time_series/interpolate.py
+-rw-r--r--  2.0 unx     1266 b- defN 23-Jun-09 16:45 auger_ml/preprocessors/time_series/resample.py
+-rw-r--r--  2.0 unx     1524 b- defN 23-Jun-09 16:45 auger_ml/preprocessors/time_series/ssa.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-09 16:45 auger_ml/scores/__init__.py
+-rw-r--r--  2.0 unx     4285 b- defN 23-Jun-09 16:45 auger_ml/scores/classification.py
+-rw-r--r--  2.0 unx     3454 b- defN 23-Jun-09 16:45 auger_ml/scores/regression.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jun-09 16:45 auger.ai.predict-1.1.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     7427 b- defN 23-Jun-09 16:45 auger.ai.predict-1.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-09 16:45 auger.ai.predict-1.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Jun-09 16:45 auger.ai.predict-1.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     7062 b- defN 23-Jun-09 16:45 auger.ai.predict-1.1.1.dist-info/RECORD
+79 files, 494791 bytes uncompressed, 122242 bytes compressed:  75.3%
```

## zipnote {}

```diff
@@ -216,23 +216,23 @@
 
 Filename: auger_ml/scores/classification.py
 Comment: 
 
 Filename: auger_ml/scores/regression.py
 Comment: 
 
-Filename: auger.ai.predict-1.0.98.dist-info/LICENSE
+Filename: auger.ai.predict-1.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: auger.ai.predict-1.0.98.dist-info/METADATA
+Filename: auger.ai.predict-1.1.1.dist-info/METADATA
 Comment: 
 
-Filename: auger.ai.predict-1.0.98.dist-info/WHEEL
+Filename: auger.ai.predict-1.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: auger.ai.predict-1.0.98.dist-info/top_level.txt
+Filename: auger.ai.predict-1.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: auger.ai.predict-1.0.98.dist-info/RECORD
+Filename: auger.ai.predict-1.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## auger_ml/S3FSClient.py

```diff
@@ -35,15 +35,15 @@
                 nTry += 1
                 time.sleep(delay*nTry)
             else:
                 raise
 
 def retry_handler(decorated):
     def wrapper(self, *args, **kwargs):
-        return retry_helper(lambda: decorated(self, *args, **kwargs), ['InvalidAccessKeyId', 'NoSuchKey'])
+        return retry_helper(lambda: decorated(self, *args, **kwargs), ['InvalidAccessKeyId', 'NoSuchKey', 'InvalidIdentityToken'])
 
     return wrapper
 
 class BotoClient:
     def __init__(self, region=None, aws_role_arn=None, endpoint_url=None):
         self.endpoint_url = endpoint_url or os.environ.get('S3_ENDPOINT_URL')
         self.aws_role_arn = aws_role_arn or os.environ.get('AWS_ROLE_ARN')
```

## auger_ml/Utils.py

```diff
@@ -5,14 +5,15 @@
 import math
 import numbers
 import os
 import sys
 import traceback
 import uuid
 import json
+import types
 
 from .FSClient import *
 
 # For calculate_scores
 from auger_ml.scores.regression import *
 from auger_ml.scores.classification import *
 
@@ -454,15 +455,20 @@
     return params
 
 def convert_numpy_types(params):
     if params is None:
         return params
 
     if type(params) is dict:
-        for key, value in params.items():
+        for key, value in list(params.items()):
+            res = convert_simple_numpy_type(key)
+            if res is not None:
+                del params[key]
+                key = res
+
             params[key] = convert_numpy_types(value)
     elif type(params) is list:
         for idx, value in enumerate(params):
             params[idx] = convert_numpy_types(value)
     else:
         if isinstance(params, numbers.Number) and math.isinf(params):
             params = None
@@ -475,14 +481,16 @@
 
     return params
 
 def json_dumps_np(data, allow_nan=False):
     if not allow_nan:
         data = convert_nan_inf(data)
 
+    data = convert_numpy_types(data)
+
     return json.dumps(data, cls=NumpyJSONEncoder, allow_nan=allow_nan)
 
 def calculate_scores(options, y_test, X_test=None, estimator=None, y_pred=None, raise_main_score=True):
     from .model_helper import ModelHelper
     return ModelHelper.calculate_scores(options, y_test, X_test, estimator, y_pred, raise_main_score)
 
 def convert_time_from_str(time_arg):
@@ -525,14 +533,48 @@
     if desc:
         p = p[::-1]
     if top_n:
         p = p[:top_n]
 
     return ar1[p], ar2[p]
 
+def print_table(log, table_list, headers=None, hor_lines=True):
+    if isinstance(table_list, types.GeneratorType):
+        table_list = list(table_list)
+
+    if table_list is None or len(table_list) == 0:
+        return
+
+    col_list = headers
+    if not col_list:
+        col_list = list(table_list[0].keys() if table_list else [])
+    row_list = [col_list]  # 1st row = header
+    for item in table_list:
+        row_list.append([str(item.get(col)) if item.get(col) is not None else '' for col in col_list])
+    # maximun size of the col for each element
+    col_size = [max(map(len, col)) for col in zip(*row_list)]
+    # insert seperating line before every line, and extra one for ending.
+    if hor_lines:
+        for i in range(0, len(row_list) + 1)[::-1]:
+            row_list.insert(i, ['-' * i for i in col_size])
+    else:
+        i = 1
+        row_list.insert(i, ['-' * i for i in col_size])        
+    # two format for each content line and each separating line
+    format_str = ' | '.join(["{{:<{}}}".format(i) for i in col_size])
+    format_sep = '-+-'.join(["{{:<{}}}".format(i) for i in col_size])
+    for idx, item in enumerate(row_list):
+        if hor_lines:
+            if idx%2==0: #item[0][0] == '-':
+                log(format_sep.format(*item))
+            else:
+                log(format_str.format(*item))
+        else:
+            log(format_str.format(*item))
+
 # def load_arff_df_ex(path, csv_path=None):
 #     import arff
 #     import csv
 #     fs_client = FSClient()
 #     if csv_path is None:
 #         csv_path = path + '.csv'
 #     else:
```

## auger_ml/model_exporter.py

```diff
@@ -18,17 +18,27 @@
 class ModelExporter(object):
     def __init__(self, options):
         self.options = options
 
     def load_model(self, model_path):
         from auger_ml.preprocessors.space import ppspace_is_timeseries_model
 
-        model = FSClient().loadObjectFromFile(os.path.join(model_path, "model.pkl.gz"))
-
         options = FSClient().readJSONFile(os.path.join(model_path, "options.json"))
+
+        try:
+            model = FSClient().loadObjectFromFile(os.path.join(model_path, "model.pkl.gz"))
+        except AttributeError as e:
+            logging.error("Cannot load model: %s. Probably due to backward compatibility broken. Will reexport model."%model_path)
+            if os.environ.get("BROKER_URL"):
+                from auger_ml.core.model_exporter_ex import ModelExporterEx
+                ModelExporterEx.reexport_model(self.options, model_path, options)
+                model = FSClient().loadObjectFromFile(os.path.join(model_path, "model.pkl.gz"))
+            else:
+                raise Exception("Auger model error: %s"%str(e))
+
         timeseries_model = options.get('timeSeriesFeatures') and ppspace_is_timeseries_model(options.get('algorithm_name'))
 
         return model, timeseries_model
 
     def preprocess_target(self, model_path, data_path=None, records=None, features=None):
         return ModelHelper.preprocess_target(model_path, data_path, records, features)
 
@@ -133,30 +143,113 @@
                 params = copy.deepcopy(self.options)
                 params = AugerML.update_task_params(params)
 
             return os.path.join(params['augerInfo']['modelsPath'], pipeline_id)
 
     def predict_by_model(self, model_path, path_to_predict=None, records=None, features=None,
         threshold=None, predict_value_num=None, json_result=False, count_in_result=False,
-        prediction_date=None, prediction_id=None, no_features_in_result=None, output=None):
+        prediction_date=None, prediction_id=None, no_features_in_result=None, output=None, 
+        predict_labels=False, score=False):
 
-        ds, options = self.predict_by_model_to_ds(model_path, path_to_predict, records, features,
-            threshold, predict_value_num, no_features_in_result=no_features_in_result)
+        if predict_labels:
+            ds, options = self.predict_labels_by_model_to_ds(model_path, path_to_predict, records, features,
+                threshold, predict_value_num, no_features_in_result=no_features_in_result,
+                predict_labels=predict_labels)            
+        else:    
+            ds, options = self.predict_by_model_to_ds(model_path, path_to_predict, records, features,
+                threshold, predict_value_num, no_features_in_result=no_features_in_result)
         if ds is None:
             return None
 
         gzip_predict_file = False
 
         if ds.count() > options.get('max_predict_records_to_gzip', 1000):
             gzip_predict_file = True
 
-        return ModelHelper.save_prediction(ds, prediction_id, json_result, count_in_result,
+        scores = None
+        if score:
+            score_true_data = DataSourceAPIPandas.create_dataframe(path_to_predict, records, features)
+            predictions = ds.df.copy()
+            scores = self.score_by_model(model_path, predict_path=predictions, predictions=predictions, 
+                test_path = score_true_data)
+
+        return  ModelHelper.save_prediction(ds, prediction_id, json_result, count_in_result,
             prediction_date, model_path, options.get('uid'), gzip_predict_file=gzip_predict_file,
-            output=output)
+            output=output, scores=scores)
+
+    def predict_labels_by_model_to_ds(self, model_path, path_to_predict=None, records=None, features=None,
+        threshold=None, predict_value_num=None, no_features_in_result=None, predict_labels=None):
+
+        #from modAL.batch import uncertainty_batch_sampling
+        #from modAL.uncertainty import uncertainty_sampling
+        #import modAL
+        from importlib import import_module
+        from modAL.models import ActiveLearner
+        from functools import partial
+
+        if not isinstance(predict_labels, dict):
+            predict_labels = self.options.get('predict_labels', {})
+
+        query_strategy_name = predict_labels.get('query_strategy', 'modAL.uncertainty.uncertainty_sampling')
+        module_name = '.'.join(query_strategy_name.split('.')[:2])
+        query_name = query_strategy_name.split('.')[-1]
+        #print(module_name, query_name)
+        query_strategy = getattr(import_module(module_name), query_name)
+        query_strategy_args = predict_labels.get('query_strategy_args', {'n_instances': 10})
+
+        X_test, Y_test, target_categoricals, data_features = self.preprocess_data(model_path,
+            data_path=path_to_predict, records=records, features=features, predict_value_num=predict_value_num)
+
+        model, _ = self.load_model(model_path)
 
+        if X_test is None:
+            return None, {}
+
+        options = FSClient().readJSONFile(os.path.join(model_path, "options.json"))
+
+        learner = ActiveLearner(
+            estimator=model,
+            query_strategy=partial(query_strategy, **query_strategy_args),
+            on_transformed=False
+        )
+        query_index, query_instance = learner.query(X_test.values)
+        ds1 = DataSourceAPIPandas.create_dataframe(path_to_predict, records, features)
+        ds = DataSourceAPIPandas({})
+        ds.df = ds1.df[data_features].iloc[query_index]
+        return ds, options
+
+    def _call_predict(self, model, X_test, model_path, options):
+        try:
+            return model.predict(X_test)
+        except AttributeError as e:
+            logging.error("Cannot predict with model model: %s. Probably due to backward compatibility broken. Will reexport model."%model_path)
+            if os.environ.get("BROKER_URL"):
+                from auger_ml.core.model_exporter_ex import ModelExporterEx
+                ModelExporterEx.reexport_model(self.options, model_path, options)
+                model, timeseries_model = self.load_model(model_path)
+                return model.predict(X_test)
+            else:
+                raise Exception("Auger model error: %s"%str(e))
+
+    def _call_predict_proba(self, model, X_test):
+        results_proba = None
+        if hasattr(model, 'predict_proba') and callable(getattr(model, 'predict_proba')):
+            try:
+                results_proba = model.predict_proba(X_test)
+            except AttributeError as e:
+                if 'predict_proba' in str(e):
+                    logging.info("predict_proba is property, try _predict_proba")
+                    results_proba = model._predict_proba(X_test)
+                else:
+                    raise    
+        elif hasattr(model, 'decision_function'):
+            results_proba = model.decision_function(X_test)
+
+        return results_proba
+            
     def predict_by_model_to_ds(self, model_path, path_to_predict=None, records=None, features=None,
         threshold=None, predict_value_num=None, no_features_in_result=None):
 
         from auger_ml.preprocessors.space import ppspace_is_timeseries_model
 
         X_test, Y_test, target_categoricals, data_features = self.preprocess_data(model_path,
             data_path=path_to_predict, records=records, features=features, predict_value_num=predict_value_num)
@@ -187,31 +280,32 @@
             })
         else:
             results = None
             results_proba = None
             proba_classes = None
             if threshold:
                 try:
-                    if hasattr(model, 'predict_proba') and callable(getattr(model, 'predict_proba')):
-                        try:
-                            results_proba = model.predict_proba(X_test)
-                        except AttributeError as e:
-                            logging.info("predict_proba is property, try _predict_proba")
-                            results_proba = model._predict_proba(X_test)
-
-                    elif hasattr(model, 'decision_function'):
-                        results_proba = model.decision_function(X_test)
-
-                    if results_proba is not None:
-                        proba_classes = list(model.classes_)
-                except:
-                    logging.exception("predict_proba failed.")
+                    results_proba = self._call_predict_proba(model, X_test)
+                except AttributeError as e:
+                    logging.error("Cannot predict with model model: %s. Probably due to backward compatibility broken. Will reexport model."%model_path)
+                    if os.environ.get("BROKER_URL"):
+                        from auger_ml.core.model_exporter_ex import ModelExporterEx
+                        ModelExporterEx.reexport_model(self.options, model_path, options)
+                        model, timeseries_model = self.load_model(model_path)
+                        results_proba = self._call_predict_proba(model, X_test)
+                    else:
+                        raise Exception("Auger model error: %s"%str(e))
+                        
+                except Exception as e:
+                    logging.exception("predict_proba failed: %s"%str(e))
 
-            if results_proba is None:
-                results = model.predict(X_test)
+            if results_proba is not None:
+                proba_classes = list(model.classes_)
+            else:
+                results = self._call_predict(model, X_test, model_path, options)
 
             target_categories = None
             if options['targetFeature'] in target_categoricals:
                 target_categories = target_categoricals[options['targetFeature']]['categories']
 
             result_cols = ModelHelper.process_prediction(ds,
                 results, results_proba, proba_classes,
@@ -263,28 +357,28 @@
             y_pred = self.predict_by_model_ts_recursive(model_path,
                 path_to_predict=predict_path, records=records, features=features, start_prediction_num=start_prediction_num)
         else:
             if predictions is None:
                 predictions = self.predict_by_model(model_path, path_to_predict=predict_path,
                     records=records, features=features)
 
-            if predict_path:
+            if predict_path is not None:
                 y_pred, target_categoricals = self.preprocess_target(model_path, data_path=predictions)
             else:
                 y_pred, target_categoricals = self.preprocess_target(model_path, records=predictions, features=[options.get('targetFeature')])
 
             #TODO: support proba scores and threshold
 
         if test_path is None and test_records is None:
             test_path = predict_path
 
         y_true, target_categoricals = self.preprocess_target(model_path, data_path=test_path,
             records=test_records, features=test_features)
 
-        if predict_path is not None and test_path == predict_path:
+        if predict_path is not None and isinstance(predict_path, str) and test_path == predict_path:
             y_true = y_true[:len(y_pred)]
 
         test_roi_data = None
         if options.get('scoring')=='roi':
             test_roi_data = DataSourceAPIPandas.create_dataframe(data_path=test_path,
                 records=test_records, features=test_features).df
```

## auger_ml/model_helper.py

```diff
@@ -1,13 +1,13 @@
 import datetime
 import os
 from celery.utils.log import get_task_logger
 logging = get_task_logger(__name__)
 
-from auger_ml.Utils import get_uid, get_uid4, sort_arrays
+from auger_ml.Utils import get_uid, get_uid4, sort_arrays, print_table
 from auger_ml.FSClient import FSClient
 from auger_ml.data_source.data_source_api_pandas import DataSourceAPIPandas
 
 
 class ModelHelper(object):
 
     @staticmethod
@@ -151,20 +151,22 @@
                 if scoring == options.get('scoring', None) and raise_main_score:
                     raise
 
                 logging.error("Score %s for algorithm %s failed to build: %s" % (
                     scoring, options.get('algorithm_name'), str(e)))
                 all_scores[scoring] = 0
 
+        #print(options['uid'], all_scores)
         return all_scores
 
     @staticmethod
     def calculate_roi(options, test_roi_data, y_test, y_pred):
         from auger_ml.roi.calculator import Calculator as RoiCalculator
 
+        #logging.info(f"Calc roi for: {options.get('uid')}")
         if not options.get('roi_metric'):
             return 0
 
         if test_roi_data is None:
             logging.error("calculate_roi failed: roi data is none.")
             return 0
 
@@ -188,18 +190,68 @@
             revenue=options['roi_metric']['revenue'],
             investment=options['roi_metric']['investment'],
             known_vars=known_vars,
             vars_mapping=vars_mapping,
         )
 
         res = calc.calculate(test_roi_data)
+
+        #ModelHelper.print_roi_result(res)
         #logging.info("ROI result: %s"%res)
+
         return res["roi"]
 
     @staticmethod
+    def print_roi_result(res):
+
+        gainers_table = []
+        if res['filtered_rows'] and 'data_date' in res['filtered_rows'][0]:
+            map_items = {}
+
+            res['filtered_rows'].sort(key=lambda f: f['data_date'], reverse=True)
+            for item in res['filtered_rows']:
+                if item['data_date'] in map_items:
+                    map_items[item['data_date']].append(item)
+                else:
+                    map_items[item['data_date']] = [item]
+
+            total_cost = 0
+            total_sell = 0
+            for key, items in map_items.items():
+
+                for item in items:
+                    gainers_table.append({
+                        'Date': item['data_date'],
+                        'ID': item.get('identifier', ''),
+                        'Actual': item['a2ml_actual'],
+                        'Pred': item['a2ml_predicted'],
+                        'cost_basis': item.get('cost_basis', 0),
+                        'ClA': "%.2f"%item.get('close_ask', 0), 
+                    })
+                    if item['a2ml_actual']:
+                        total_cost += item.get('cost_basis', 100)
+                        total_sell += item.get('cost_basis', 100)*(1+item['a2ml_actual'])
+                
+            logging.info(f'ROI: {total_cost}, {total_sell}, {(total_sell-total_cost)/total_cost}')
+        else:
+            #print(res)
+            for item in res['filtered_rows']:
+                gainers_table.append({
+                    'Actual': item['a2ml_actual'],
+                    'Pred': item['a2ml_predicted'],
+                })
+                
+        def print_log(msg, *args, **kwargs):
+            #print(msg, *args, **kwargs)
+            logging.info(msg, *args, **kwargs)
+
+        if gainers_table:    
+            print_table(print_log, gainers_table, hor_lines=False)
+
+    @staticmethod
     def preprocess_target(model_path, data_path=None, records=None, features=None):
         ds = DataSourceAPIPandas.create_dataframe(data_path, records, features)
 
         return ModelHelper.preprocess_target_ds(model_path, ds)
 
     @staticmethod
     def preprocess_target_ds(model_path, ds):
@@ -265,15 +317,15 @@
                 result_cols.append(col_name)
 
         return result_cols
                 
     @staticmethod
     def save_prediction(ds, prediction_id,
         json_result, count_in_result, prediction_date, model_path, model_id, output=None,
-        gzip_predict_file=False):
+        gzip_predict_file=False, scores=None):
 
         path_to_predict = ds.options.get('data_path')
         # Id for whole prediction (can contains many rows)
         if not prediction_id:
             prediction_id = get_uid()
 
         result = {}
@@ -289,22 +341,26 @@
                 if gzip_predict_file:
                     predict_path += ".gz"
 
             ds.saveToFile(predict_path)
 
             if count_in_result:
                 result = {'result_path': predict_path, 'count': ds.count()}
+                if scores:
+                    result['scores'] = scores
             else:
                 result = predict_path
         else:
             if json_result:
                 result = ds.df.to_json(orient='split', index=False)
             elif ds.loaded_columns:
                 predicted = ds.df.to_dict('split')
                 result = {'data': predicted.get('data', []), 'columns': predicted.get('columns')}
+                if scores:
+                    result['scores'] = scores
             else:
                 result = ds.df.to_dict('records')
 
         return result
 
     @staticmethod
     def revertCategories(results, categories):
```

## auger_ml/data_source/data_source_api_pandas.py

```diff
@@ -1537,15 +1537,16 @@
                                 cv = StratifiedGroupKFold(n_splits=max(cv_num, 2), random_state=randomSeed, shuffle=shuffleData)
                             else:
                                 cv = StratifiedKFold(n_splits=max(cv_num, 2), random_state=randomSeed, shuffle=shuffleData)
                         else:
                             if groups is not None:
                                 cv = GroupKFold(n_splits=max(cv_num, 2))
                             else:
-                                cv = KFold(n_splits=max(cv_num, 2), random_state=randomSeed, shuffle=shuffleData)
+                                cv = KFold(n_splits=max(cv_num, 2), 
+                                    random_state=randomSeed if shuffleData else None, shuffle=shuffleData)
 
                 if cv is not None:
                     cv_iter = list(cv.split(features, target, groups))
 
                     ds_roi = None
                     if self.options.get('roi_metric'):
                         ds_roi = DataSourceAPIPandas(self.options).load_roi_features()
```

## auger_ml/scores/classification.py

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 import pandas
 from sklearn.metrics import make_scorer, recall_score, average_precision_score
 from sklearn.metrics import confusion_matrix
 from sklearn.metrics import matthews_corrcoef as mcc
-from sklearn.metrics import SCORERS
+from sklearn.metrics._scorer import _SCORERS
 
 
 def kappa(y_true, y_pred, weights=None, allow_off_by_one=False):
     """ https://en.wikipedia.org/wiki/Cohen%27s_kappa """
     # assert (len(y_true) == len(y_probs))
     try:
         if type(y_true) == pandas.DataFrame:
@@ -95,15 +95,15 @@
 
 cohen_kappa_score = make_scorer(kappa)
 matthews_corrcoef = make_scorer(matthews)
 gini_score = make_scorer(gini, needs_threshold=True)
 norm_macro_recall_scorer = make_scorer(norm_macro_recall_score)
 average_precision_score_weighted_scorer = make_scorer(average_precision_score_weighted_score)
 
-SCORERS['cohen_kappa_score'] = cohen_kappa_score
-SCORERS['matthews_corrcoef'] = matthews_corrcoef
-SCORERS['gini'] = gini_score
-SCORERS['norm_macro_recall'] = norm_macro_recall_scorer
-SCORERS['average_precision_score_weighted'] = average_precision_score_weighted_scorer
-SCORERS['AUC_weighted'] = SCORERS['roc_auc_ovr_weighted']
+_SCORERS['cohen_kappa_score'] = cohen_kappa_score
+_SCORERS['matthews_corrcoef'] = matthews_corrcoef
+_SCORERS['gini'] = gini_score
+_SCORERS['norm_macro_recall'] = norm_macro_recall_scorer
+_SCORERS['average_precision_score_weighted'] = average_precision_score_weighted_scorer
+_SCORERS['AUC_weighted'] = _SCORERS['roc_auc_ovr_weighted']
```

## auger_ml/scores/regression.py

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 from sklearn.metrics import make_scorer, mean_squared_error, mean_squared_log_error, mean_absolute_error
-from sklearn.metrics import SCORERS
+from sklearn.metrics._scorer import _SCORERS
 
 
 EPSILON = 1e-10
 
 def _error(actual: np.ndarray, predicted: np.ndarray):
     """ Simple error """
     return actual - predicted
@@ -80,15 +80,15 @@
 neg_mape_scorer = make_scorer(neg_mape_score)
 mda_scorer = make_scorer(mda_score)
 neg_rmse_scorer = make_scorer(neg_rmse_score)
 nmae_scorer = make_scorer(nmae_score)
 nrmse_scorer = make_scorer(nrmse_score)
 spearman_correlation_scorer = make_scorer(spearman_correlation_score)
 
-SCORERS['neg_rmsle'] = neg_rmsle_scorer
-SCORERS['neg_mase'] = neg_mase_scorer
-SCORERS['neg_mape'] = neg_mape_scorer
-SCORERS['mda'] = mda_scorer
-SCORERS['neg_rmse'] = neg_rmse_scorer
-SCORERS['normalized_mean_absolute_error'] = nmae_scorer
-SCORERS['normalized_root_mean_squared_error'] = nrmse_scorer
-SCORERS['spearman_correlation'] = spearman_correlation_scorer
+_SCORERS['neg_rmsle'] = neg_rmsle_scorer
+_SCORERS['neg_mase'] = neg_mase_scorer
+_SCORERS['neg_mape'] = neg_mape_scorer
+_SCORERS['mda'] = mda_scorer
+_SCORERS['neg_rmse'] = neg_rmse_scorer
+_SCORERS['normalized_mean_absolute_error'] = nmae_scorer
+_SCORERS['normalized_root_mean_squared_error'] = nrmse_scorer
+_SCORERS['spearman_correlation'] = spearman_correlation_scorer
```

## Comparing `auger.ai.predict-1.0.98.dist-info/LICENSE` & `auger.ai.predict-1.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `auger.ai.predict-1.0.98.dist-info/METADATA` & `auger.ai.predict-1.1.1.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auger.ai.predict
-Version: 1.0.98
+Version: 1.1.1
 Summary: Auger ML predict python and command line interface
 Home-page: https://github.com/deeplearninc/auger-ai
 Author: Deep Learn, Inc.
 Author-email: augerai@dplrn.com
 License: Apache
 Keywords: augerai auger ai machine learning automl deeplearn api sdk prediction predict
 Platform: any
@@ -14,39 +14,46 @@
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3
 Description-Content-Type: text/markdown
-License-File: LICENSE
 Provides-Extra: all
-Requires-Dist: pandas (==1.3.5) ; extra == 'all'
-Requires-Dist: six (==1.15.0) ; extra == 'all'
-Requires-Dist: scipy (==1.5.2) ; extra == 'all'
-Requires-Dist: scikit-learn (==0.24.2) ; extra == 'all'
-Requires-Dist: catboost (==1.0.4) ; extra == 'all'
-Requires-Dist: lightgbm (==3.3.2) ; extra == 'all'
+Requires-Dist: numpy (==1.23.5) ; extra == 'all'
+Requires-Dist: pandas (==1.5.0) ; extra == 'all'
+Requires-Dist: six (==1.16.0) ; extra == 'all'
+Requires-Dist: scipy (==1.9.1) ; extra == 'all'
+Requires-Dist: scikit-learn (==1.2.0) ; extra == 'all'
+Requires-Dist: xgboost (==1.6.2) ; extra == 'all'
+Requires-Dist: catboost (<2.0,>1.0) ; extra == 'all'
+Requires-Dist: lightgbm (<3.4,>3.3) ; extra == 'all'
+Requires-Dist: modAL-python ; extra == 'all'
 Requires-Dist: joblib ; extra == 'all'
 Requires-Dist: boto3 ; extra == 'all'
 Requires-Dist: s3fs (==0.4.2) ; extra == 'all'
 Requires-Dist: stopit ; extra == 'all'
-Requires-Dist: smart-open (==5.1.0) ; extra == 'all'
-Requires-Dist: celery (==5.2.2) ; extra == 'all'
+Requires-Dist: smart-open (==6.2.0) ; extra == 'all'
+Requires-Dist: kombu (==5.2.4) ; extra == 'all'
+Requires-Dist: celery (==5.2.7) ; extra == 'all'
 Provides-Extra: no_cat_lgbm
-Requires-Dist: pandas (==1.3.5) ; extra == 'no_cat_lgbm'
-Requires-Dist: six (==1.15.0) ; extra == 'no_cat_lgbm'
-Requires-Dist: scipy (==1.5.2) ; extra == 'no_cat_lgbm'
-Requires-Dist: scikit-learn (==0.24.2) ; extra == 'no_cat_lgbm'
+Requires-Dist: numpy (==1.23.5) ; extra == 'no_cat_lgbm'
+Requires-Dist: pandas (==1.5.0) ; extra == 'no_cat_lgbm'
+Requires-Dist: six (==1.16.0) ; extra == 'no_cat_lgbm'
+Requires-Dist: scipy (==1.9.1) ; extra == 'no_cat_lgbm'
+Requires-Dist: scikit-learn (==1.2.0) ; extra == 'no_cat_lgbm'
+Requires-Dist: xgboost (==1.6.2) ; extra == 'no_cat_lgbm'
+Requires-Dist: modAL-python ; extra == 'no_cat_lgbm'
 Requires-Dist: joblib ; extra == 'no_cat_lgbm'
 Requires-Dist: boto3 ; extra == 'no_cat_lgbm'
 Requires-Dist: s3fs (==0.4.2) ; extra == 'no_cat_lgbm'
 Requires-Dist: stopit ; extra == 'no_cat_lgbm'
-Requires-Dist: smart-open (==5.1.0) ; extra == 'no_cat_lgbm'
-Requires-Dist: celery (==5.2.2) ; extra == 'no_cat_lgbm'
+Requires-Dist: smart-open (==6.2.0) ; extra == 'no_cat_lgbm'
+Requires-Dist: kombu (==5.2.4) ; extra == 'no_cat_lgbm'
+Requires-Dist: celery (==5.2.7) ; extra == 'no_cat_lgbm'
 
 # Install
 ```
 pip install auger.ai.predict
 ```
 
 # Auger.ai.predict
@@ -111,15 +118,15 @@
 
       # data is an array of arrays to get predictions for, input your data below
       # each record should contain values for each feature
       records = [[],[]]
 
       if path_to_predict:
           path_to_predict=os.path.abspath(path_to_predict)
-              
+
       predictions = ModelExporter({}).predict_by_model(
           records=records,
           model_path=model_path,
           path_to_predict=path_to_predict,
           features=features,
           threshold=threshold
       )
```

## Comparing `auger.ai.predict-1.0.98.dist-info/RECORD` & `auger.ai.predict-1.1.1.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 auger_ml/AugerMLPreprocessors.py,sha256=Lnef7J5ILj0sLUTObCMvEydpwVYLmOjIU0zaLpJGWtM,22767
 auger_ml/FSClient.py,sha256=lTxKD25gJs4JreuRiF397EzuVE0ivTzI-eNqwn0-Bkk,16118
 auger_ml/LocalFSClient.py,sha256=lP27Vizp74mOQkyxmXR1E0sy5ft-ZfAS20eIZzzfbns,7967
-auger_ml/S3FSClient.py,sha256=g7p_1sWytJVGbq3fU9M16_wLOTWi2-mOuVBTJPGqTgQ,22415
-auger_ml/Utils.py,sha256=gRQtwas_ABW9Kq-FInFuqpN4nMk9hS1LigDJFCh66Nk,16617
+auger_ml/S3FSClient.py,sha256=P_E_K1gMyuF6qTLWgDFCZsIRXO3_4M5mtwS58s2cSfU,22439
+auger_ml/Utils.py,sha256=nxr0WMersGNIkXcWb1pNlzjYBmWl6BCqaxm9QHllFIU,18206
 auger_ml/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 auger_ml/celery_logging.py,sha256=jrZV2D88ydjyc2dDZEFR89vKQK2GEJXZHJ-MAIRyX2U,1803
-auger_ml/model_exporter.py,sha256=fWMNWpmtIFMblqbAMcpLGulAJzV9gTYPiIEpoZwaGts,12945
-auger_ml/model_helper.py,sha256=o5kLuGZwWTZiMoXYbRNla-lJ74izG3CaSsnNNaKB9u4,14926
+auger_ml/model_exporter.py,sha256=vVtG32hcRqNjU2cmte4CRUckzNk-SqlBEJzMiQvqK0E,17782
+auger_ml/model_helper.py,sha256=V3sM0GHKswfopEjauaoXwwUPEX3rnKJNbpZDHtnfcwY,17115
 auger_ml/model_review.py,sha256=QrUtoZV2BbOa-oD9-xP9kkeL1Sno1N25Dv5oCqXeohs,16483
 auger_ml/probabilistic_counter.py,sha256=-ZWe_n7twR85cCdpihbNdnatF9cWv1fgn3Wd-C63Z54,389
 auger_ml/warmstart_optimizer.py,sha256=g-VKWbHN8FtA_HP57LMlxQ4z_7ugnTvLYhczI9lsAlI,1711
 auger_ml/algorithms/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 auger_ml/algorithms/adam_wd.py,sha256=pJSHrlZh9ZDB_V19SwtdJkoKvXsOsctCRWX8RhIqh8k,5014
 auger_ml/algorithms/baseline.py,sha256=V--4wj8mjMsYfKYzN5zwEWlG4zPSrIi5oCqC7OQkLs0,162
 auger_ml/algorithms/cat_boost.py,sha256=7GO9rzP9DAuWumz1HO_Br-gsfyZFAkmCmV-LUaUx6Bg,3427
@@ -25,15 +25,15 @@
 auger_ml/algorithms/timeseries.py,sha256=zSJkrOrLRhYMq70dO4Az0iSweiVGPMTPLBIqsi6DJmM,1743
 auger_ml/algorithms/ts_dnn.py,sha256=J-JQgGlPt3Vp6A2gF_vssA7YUTKmHTaccNKt48NcdyU,11030
 auger_ml/algorithms/ts_dnn_cpu.py,sha256=u-wAuIuV0HDh9eq6nR7bZyo6qiYtKTgtBMgjxcnxo6g,12511
 auger_ml/algorithms/ts_lstm.py,sha256=OQWXTJnNwFn6Baf_mqXaM5dDtn92TGpEMROcNpmNtcs,3626
 auger_ml/algorithms/utils.py,sha256=7nFMZpfR_NjKeF_Jo3nAyT3nDfea_NabRjRgaE9cy98,1866
 auger_ml/data_source/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 auger_ml/data_source/data_source_api.py,sha256=wx0rZjpd93bMavHCF8ej65zZfdXftbep7NMdP1sciLY,4856
-auger_ml/data_source/data_source_api_pandas.py,sha256=yaEb6ioF_u8H_KtD_JSYcR_Mj4EAoo26tkYEov4yxhE,86557
+auger_ml/data_source/data_source_api_pandas.py,sha256=G6I4UaYOEXajm6Gr0lNTq30xjjxtoy4WOHo8z87Q8B0,86619
 auger_ml/data_source/data_source_api_pandas_proxy.py,sha256=uR9mRvtvxkO-C6KgmQ2VWvVJc55mRj-h3kcB_vYJfVE,1123
 auger_ml/data_source/data_source_factory.py,sha256=X2NBrhe085-M5VKf7FHEK1aeLoK06RzJQLMu1JrdEkQ,1361
 auger_ml/data_source/group_splits.py,sha256=LFrc7nvDT1a3aHGs4iS2aOEK9zq56Adw2O1hChXTaMA,15064
 auger_ml/data_splitters/BaseSplitter.py,sha256=_HWfnLHGSeu3oI11ymCXjRjomD_jkvkTfs68dVk_Ehg,116
 auger_ml/data_splitters/DFSparkDataPrep.py,sha256=bGQ8Ri5EIbZdwFO3w5E9QlJmA2VZn8JuvnetksJ4NeE,711
 auger_ml/data_splitters/SimpleSplitter.py,sha256=WjrIwt_bZXeKnq8xH7Z0gMag_hMqJBRcjfR4GIQtuug,1323
 auger_ml/data_splitters/XYNumpyDataPrep.py,sha256=BDS7O3xfMYPG00_HkoeqPuhXxDLliDmznR8UmxZyKA8,2295
@@ -66,14 +66,14 @@
 auger_ml/preprocessors/text.py,sha256=T4XWpy6JsCGtkFIXVQ81ovAena5KPoY4Aq-hT1I10wc,15532
 auger_ml/preprocessors/time_series/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 auger_ml/preprocessors/time_series/embedding.py,sha256=tWh5zKCIRJT4pBgmwflP1pidanP7AgU0XpYQ4NlJbio,1286
 auger_ml/preprocessors/time_series/interpolate.py,sha256=ONYV671I8aGs87qh_qCW_9nyZZXuuTDNAJcfajbVjWc,580
 auger_ml/preprocessors/time_series/resample.py,sha256=ZYBj0ewQi_Z0IEm4BY56qj2vOiR9ABzJeNXAkHI0mBc,1266
 auger_ml/preprocessors/time_series/ssa.py,sha256=oR-4nV_RGZDCTKQPH8Yx_y6qiozUcs3WVPJPcO7nEZ4,1524
 auger_ml/scores/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-auger_ml/scores/classification.py,sha256=wN415V1_EHlqNXONdBbg6NZ4eufSggD81Mo9r6YqGSQ,4269
-auger_ml/scores/regression.py,sha256=kXqlIYrwi8uCNeYqMt9K2rbfSb5CEKT7BWiLVMHmFGM,3437
-auger.ai.predict-1.0.98.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-auger.ai.predict-1.0.98.dist-info/METADATA,sha256=yhw5Uwwnnin-cwqFpODtnIGvOqmLzDYKpOnW1urYRSI,7046
-auger.ai.predict-1.0.98.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-auger.ai.predict-1.0.98.dist-info/top_level.txt,sha256=OAZTv-tyoAj0z0-_xEhhdpntAR17SQ5SaK9p8IkxmXU,9
-auger.ai.predict-1.0.98.dist-info/RECORD,,
+auger_ml/scores/classification.py,sha256=BwXRRHo2ARS125VwC4V_x9aKRReZtdyzZdgZblacWXs,4285
+auger_ml/scores/regression.py,sha256=TuM3aKxYcBZnMjs9OUr6o0Gl4EIA9uJpgRwV2MWqjY0,3454
+auger.ai.predict-1.1.1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+auger.ai.predict-1.1.1.dist-info/METADATA,sha256=MYU9Hr6nchSr7j_pL0_wHPZvvvgOTygMpW-ZmHHRwtM,7427
+auger.ai.predict-1.1.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+auger.ai.predict-1.1.1.dist-info/top_level.txt,sha256=OAZTv-tyoAj0z0-_xEhhdpntAR17SQ5SaK9p8IkxmXU,9
+auger.ai.predict-1.1.1.dist-info/RECORD,,
```

