# Comparing `tmp/man_etl-0.0.7.tar.gz` & `tmp/man_etl-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "man_etl-0.0.7.tar", last modified: Thu Jun  8 16:34:17 2023, max compression
+gzip compressed data, was "man_etl-0.0.8.tar", last modified: Fri Jun  9 00:22:42 2023, max compression
```

## Comparing `man_etl-0.0.7.tar` & `man_etl-0.0.8.tar`

### file list

```diff
@@ -1,38 +1,48 @@
-drwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-08 16:48:41.370465 man_etl-0.0.7/
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)       51 2023-06-08 16:48:41.370465 man_etl-0.0.7/PKG-INFO
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)      374 2023-06-08 08:17:19.000000 man_etl-0.0.7/README.md
-drwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-08 16:48:39.233281 man_etl-0.0.7/man_etl/
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-07 17:32:55.000000 man_etl-0.0.7/man_etl/__init__.py
-drwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-08 16:48:39.902728 man_etl-0.0.7/man_etl/etl_pipelines/
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-08 16:46:59.000000 man_etl-0.0.7/man_etl/etl_pipelines/__init__.py
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)     1168 2023-06-08 13:36:53.000000 man_etl-0.0.7/man_etl/etl_pipelines/arctic_transform.py
-drwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-08 16:48:40.498578 man_etl-0.0.7/man_etl/etl_pipelines/core/
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-08 08:40:26.000000 man_etl-0.0.7/man_etl/etl_pipelines/core/__init__.py
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)     1363 2023-06-08 10:16:49.000000 man_etl-0.0.7/man_etl/etl_pipelines/core/arctic.py
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)      788 2023-06-08 10:01:21.000000 man_etl-0.0.7/man_etl/etl_pipelines/core/base.py
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)     2160 2023-06-08 16:45:40.000000 man_etl-0.0.7/man_etl/etl_pipelines/core/extractors.py
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)      468 2023-06-08 13:36:53.000000 man_etl-0.0.7/man_etl/etl_pipelines/core/storers.py
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)     1173 2023-06-08 16:45:57.000000 man_etl-0.0.7/man_etl/etl_pipelines/core/transformers.py
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)     1062 2023-06-08 16:36:50.000000 man_etl-0.0.7/man_etl/etl_pipelines/csv_to_arctic.py
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)      651 2023-06-08 13:36:53.000000 man_etl-0.0.7/man_etl/etl_pipelines/ons_to_arctic.py
-drwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-08 16:48:40.899660 man_etl-0.0.7/man_etl/etl_pipelines/util/
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-08 16:44:11.000000 man_etl-0.0.7/man_etl/etl_pipelines/util/__init__.py
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)       25 2023-06-08 13:36:53.000000 man_etl-0.0.7/man_etl/etl_pipelines/util/definitions.py
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)     1369 2023-06-08 13:36:53.000000 man_etl-0.0.7/man_etl/etl_pipelines/util/transforms.py
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)       97 2023-06-08 10:01:21.000000 man_etl-0.0.7/man_etl/etl_pipelines/util/utils.py
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)      147 2023-06-08 08:17:19.000000 man_etl-0.0.7/man_etl/generate_db.py
-drwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-08 16:48:41.296355 man_etl-0.0.7/man_etl/python/
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-07 17:32:56.000000 man_etl-0.0.7/man_etl/python/__init__.py
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)      612 2023-06-08 08:17:19.000000 man_etl-0.0.7/man_etl/python/app.py
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)       59 2023-06-07 17:32:57.000000 man_etl-0.0.7/man_etl/python/main.py
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)       94 2023-06-08 09:31:02.000000 man_etl-0.0.7/man_etl/python/pyarrow_client.py
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)       79 2023-06-08 08:17:19.000000 man_etl-0.0.7/man_etl/python/utils.py
-drwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-08 16:48:39.561092 man_etl-0.0.7/man_etl.egg-info/
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)       51 2023-06-08 16:48:33.000000 man_etl-0.0.7/man_etl.egg-info/PKG-INFO
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)      923 2023-06-08 16:48:37.000000 man_etl-0.0.7/man_etl.egg-info/SOURCES.txt
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)        1 2023-06-08 16:48:33.000000 man_etl-0.0.7/man_etl.egg-info/dependency_links.txt
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)       84 2023-06-08 16:48:34.000000 man_etl-0.0.7/man_etl.egg-info/entry_points.txt
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)       22 2023-06-08 16:48:34.000000 man_etl-0.0.7/man_etl.egg-info/requires.txt
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)        8 2023-06-08 16:48:34.000000 man_etl-0.0.7/man_etl.egg-info/top_level.txt
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)       38 2023-06-08 16:48:41.386800 man_etl-0.0.7/setup.cfg
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)      369 2023-06-08 16:48:24.000000 man_etl-0.0.7/setup.py
+drwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-09 12:28:25.830610 man_etl-0.0.8/
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)       51 2023-06-09 12:28:25.825611 man_etl-0.0.8/PKG-INFO
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)     2199 2023-06-09 08:21:22.000000 man_etl-0.0.8/README.md
+drwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-09 12:28:24.233780 man_etl-0.0.8/man_etl/
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-07 17:32:55.000000 man_etl-0.0.8/man_etl/__init__.py
+drwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-09 12:28:24.968619 man_etl-0.0.8/man_etl/etl_pipelines/
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-08 16:46:59.000000 man_etl-0.0.8/man_etl/etl_pipelines/__init__.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)      783 2023-06-09 09:46:43.000000 man_etl-0.0.8/man_etl/etl_pipelines/arctic_to_arrowflight.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)     1163 2023-06-08 17:11:20.000000 man_etl-0.0.8/man_etl/etl_pipelines/arctic_transform.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)     1227 2023-06-09 12:25:06.000000 man_etl-0.0.8/man_etl/etl_pipelines/arctic_transform_rf.py
+drwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-09 12:28:25.396591 man_etl-0.0.8/man_etl/etl_pipelines/core/
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-08 08:40:26.000000 man_etl-0.0.8/man_etl/etl_pipelines/core/__init__.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)     1363 2023-06-08 10:16:49.000000 man_etl-0.0.8/man_etl/etl_pipelines/core/arctic.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)      593 2023-06-08 17:31:07.000000 man_etl-0.0.8/man_etl/etl_pipelines/core/base.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)     2877 2023-06-09 09:46:43.000000 man_etl-0.0.8/man_etl/etl_pipelines/core/extractors.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)      648 2023-06-08 17:10:22.000000 man_etl-0.0.8/man_etl/etl_pipelines/core/pipeline.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)     1392 2023-06-09 12:25:41.000000 man_etl-0.0.8/man_etl/etl_pipelines/core/rf_extractor.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)     1516 2023-06-09 12:22:59.000000 man_etl-0.0.8/man_etl/etl_pipelines/core/rf_storer.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)     1832 2023-06-09 09:46:43.000000 man_etl-0.0.8/man_etl/etl_pipelines/core/storers.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)     1173 2023-06-09 12:22:56.000000 man_etl-0.0.8/man_etl/etl_pipelines/core/transformers.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)     1062 2023-06-08 17:15:55.000000 man_etl-0.0.8/man_etl/etl_pipelines/csv_to_arctic.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)      706 2023-06-09 12:23:44.000000 man_etl-0.0.8/man_etl/etl_pipelines/ons_arctic_to_arrowflight_rf.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)      747 2023-06-09 09:59:37.000000 man_etl-0.0.8/man_etl/etl_pipelines/ons_to_arctic.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)      727 2023-06-09 12:24:00.000000 man_etl-0.0.8/man_etl/etl_pipelines/ons_to_arctic_rf.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-09 11:35:52.000000 man_etl-0.0.8/man_etl/etl_pipelines/ons_to_arrowflight.py
+drwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-09 12:28:25.607409 man_etl-0.0.8/man_etl/etl_pipelines/util/
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-08 16:44:11.000000 man_etl-0.0.8/man_etl/etl_pipelines/util/__init__.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)       25 2023-06-08 13:36:53.000000 man_etl-0.0.8/man_etl/etl_pipelines/util/definitions.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)     1369 2023-06-08 13:36:53.000000 man_etl-0.0.8/man_etl/etl_pipelines/util/transforms.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)       97 2023-06-09 08:21:51.000000 man_etl-0.0.8/man_etl/etl_pipelines/util/utils.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)     1156 2023-06-09 12:25:29.000000 man_etl-0.0.8/man_etl/etl_pipelines/yf_arctic_to_arrowflight_rf.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)      848 2023-06-09 06:21:44.000000 man_etl-0.0.8/man_etl/etl_pipelines/yf_to_arctic.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)      647 2023-06-09 12:26:25.000000 man_etl-0.0.8/man_etl/etl_pipelines/yf_to_arctic_rf.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)      147 2023-06-08 08:17:19.000000 man_etl-0.0.8/man_etl/generate_db.py
+drwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-09 12:28:25.783784 man_etl-0.0.8/man_etl/python/
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-07 17:32:56.000000 man_etl-0.0.8/man_etl/python/__init__.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)      103 2023-06-08 17:30:09.000000 man_etl-0.0.8/man_etl/python/app.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)      749 2023-06-08 17:30:09.000000 man_etl-0.0.8/man_etl/python/pyarrow_client.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-09 09:46:43.000000 man_etl-0.0.8/man_etl/python/signal_constructor.py
+drwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-09 12:28:24.441406 man_etl-0.0.8/man_etl.egg-info/
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)       51 2023-06-09 12:28:20.000000 man_etl-0.0.8/man_etl.egg-info/PKG-INFO
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)     1399 2023-06-09 12:28:22.000000 man_etl-0.0.8/man_etl.egg-info/SOURCES.txt
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)        1 2023-06-09 12:28:20.000000 man_etl-0.0.8/man_etl.egg-info/dependency_links.txt
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)      828 2023-06-09 12:28:20.000000 man_etl-0.0.8/man_etl.egg-info/entry_points.txt
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)       13 2023-06-09 12:28:20.000000 man_etl-0.0.8/man_etl.egg-info/requires.txt
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)        8 2023-06-09 12:28:20.000000 man_etl-0.0.8/man_etl.egg-info/top_level.txt
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)       38 2023-06-09 12:28:25.831968 man_etl-0.0.8/setup.cfg
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)     1147 2023-06-09 12:26:57.000000 man_etl-0.0.8/setup.py
```

### Comparing `man_etl-0.0.7/man_etl/etl_pipelines/arctic_transform.py` & `man_etl-0.0.8/man_etl/etl_pipelines/arctic_transform.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,12 +17,12 @@
     logger.info(f'Initializing library {library}')
     arctic_lib = ArcticInitializer(libname=library)()
     logger.info(f'Extracting data from library: {library}')
     extracted_data = ArcticExtractor(library=arctic_lib).extract_many()
     logger.info(f'Transforming data.......')
     transformed_data = DataFrameTransformer(data=extracted_data, transformers=calcs).transform()
     logger.info(f'Storing transformed data in S3')
-    ArcticStorer(to_store=transformed_data, destination=arctic_lib).store_many()
+    ArcticStorer(to_store=transformed_data, destination=arctic_lib).store()
 
 
 if __name__ == "__main__":
     arctic_transform()
```

### Comparing `man_etl-0.0.7/man_etl/etl_pipelines/core/arctic.py` & `man_etl-0.0.8/man_etl/etl_pipelines/core/arctic.py`

 * *Files identical despite different names*

### Comparing `man_etl-0.0.7/man_etl/etl_pipelines/core/base.py` & `man_etl-0.0.8/man_etl/etl_pipelines/core/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,17 +16,10 @@
     @abc.abstractmethod
     def transform(self, *args, **kwargs) -> Any:
         raise NotImplementedError("please implement an extraction")
 
 
 @dataclass
 class Storer(abc.ABC):
-    destination: Any
-    to_store: Union[pd.DataFrame, Dict[str, pd.DataFrame]]
-
     @abc.abstractmethod
     def store(self):
         raise NotImplementedError("please implement a storer")
-
-    @abc.abstractmethod
-    def store_many(self):
-        raise NotImplementedError("please implement a storer")
```

### Comparing `man_etl-0.0.7/man_etl/etl_pipelines/core/extractors.py` & `man_etl-0.0.8/man_etl/etl_pipelines/core/extractors.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 import os
+from contextlib import contextmanager
+
 import pandas as pd
 import logging
 from man_etl.etl_pipelines.core.base import Extractor
-from man_etl.etl_pipelines.util.definitions import TRANSFORM
 from arcticdb.version_store.library import Library
 from typing import List, Dict
 from dataclasses import dataclass
-
+from datetime import datetime, timedelta
+import yfinance as yf
 
 from pyarrow._flight import FlightClient
+
+from man_etl.etl_pipelines.util.definitions import TRANSFORM
 from man_etl.etl_pipelines.util.utils import SERVER_MAPPINGS
 from pyarrow import flight
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger('Logger')
 
 
@@ -25,44 +29,62 @@
         csv_hash = {}
         for csv in csv_list:
             stock = csv.split(".csv")[0]
             csv_hash[stock] = pd.read_csv(f"{self.csv_path}/{csv}")
         return csv_hash
 
 class YFExtractor(Extractor):
+    symbols: List = ['AAPL', 'GOOGL', 'MSFT']
+
     def extract(self):
-        pass
+        data = {}
+        end = datetime.now().date()
+        start = end - timedelta(days=365)
+        start_str = start.strftime('%Y-%m-%d')
+        end_str = end.strftime('%Y-%m-%d')
+        for symbol in self.symbols:
+            data[symbol] = yf.download(symbol, start=start_str, end=end_str, interval='1d')
+        return data
 
 @dataclass
 class ArcticExtractor(Extractor):
     library: Library
 
     def extract(self, symbol: str) -> pd.DataFrame:
         return self.library.read(symbol).data
 
     def extract_many(self) -> Dict:
         data = {}
         for sym in self._get_raw_symbols():
             data[sym] = self.extract(sym)
         return data
     
+    def extract_all(self):
+        data = {}
+        for sym in self.library.list_symbols():
+            data[sym] = self.extract(sym)
+        return data
+    
     def _get_raw_symbols(self):
         return [sym for sym in self.library.list_symbols() if TRANSFORM not in sym]
 
 class ArrowFlightExtractor(Extractor):
     def __init__(self, endpoint, filepath):
         self.endpoint = endpoint
         self.filepath = filepath
 
-    @property
+    @contextmanager
     def client_connection(self) -> FlightClient:
-        yield flight.connect(self.endpoint)
+        try:
+            yield flight.connect(self.endpoint)
+        finally:
+            logger.info("closed connection")
 
     def extract(self) -> pd.DataFrame:
-        with self.client_connection as client:
+        with self.client_connection() as client:
             self.vendor_flight = client.get_flight_info(flight.FlightDescriptor.for_path(self.filepath))
             reader = client.do_get(self.vendor_flight.endpoints[0].ticket)
             data_table = reader.read_all()
             return data_table.to_pandas()
 
     @classmethod
     def parquet(cls, filepath: str):
```

### Comparing `man_etl-0.0.7/man_etl/etl_pipelines/core/transformers.py` & `man_etl-0.0.8/man_etl/etl_pipelines/core/transformers.py`

 * *Files identical despite different names*

### Comparing `man_etl-0.0.7/man_etl/etl_pipelines/csv_to_arctic.py` & `man_etl-0.0.8/man_etl/etl_pipelines/csv_to_arctic.py`

 * *Files identical despite different names*

### Comparing `man_etl-0.0.7/man_etl/etl_pipelines/util/transforms.py` & `man_etl-0.0.8/man_etl/etl_pipelines/util/transforms.py`

 * *Files identical despite different names*

