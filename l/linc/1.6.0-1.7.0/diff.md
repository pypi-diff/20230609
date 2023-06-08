# Comparing `tmp/linc-1.6.0.tar.gz` & `tmp/linc-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linc-1.6.0.tar", max compression
+gzip compressed data, was "linc-1.7.0.tar", max compression
```

## Comparing `linc-1.6.0.tar` & `linc-1.7.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      331 2023-06-07 01:03:22.218726 linc-1.6.0/linc/__init__.py
--rw-r--r--   0        0        0     1109 2023-06-07 01:03:22.218726 linc-1.6.0/linc/cli.py
--rw-r--r--   0        0        0       96 2023-06-07 01:03:22.232840 linc-1.6.0/linc/config/__init__.py
--rw-r--r--   0        0        0       35 2023-06-07 01:03:22.232840 linc-1.6.0/linc/config/default-config.toml
--rw-r--r--   0        0        0     1276 2023-06-07 13:28:15.945042 linc-1.6.0/linc/config/models.py
--rw-r--r--   0        0        0      967 2023-06-07 01:03:22.232840 linc-1.6.0/linc/config/read.py
--rw-r--r--   0        0        0     3183 2023-06-07 13:34:35.874796 linc-1.6.0/linc/convertion.py
--rw-r--r--   0        0        0     2846 2023-06-07 01:03:22.234945 linc-1.6.0/linc/models.py
--rw-r--r--   0        0        0       80 2023-06-07 01:03:22.236254 linc-1.6.0/linc/parse/__init__.py
--rw-r--r--   0        0        0       42 2023-06-07 01:03:22.236254 linc-1.6.0/linc/parse/constants.py
--rw-r--r--   0        0        0     1016 2023-06-07 01:03:22.236254 linc-1.6.0/linc/parse/dataset.py
--rw-r--r--   0        0        0      256 2023-06-07 01:03:22.236254 linc-1.6.0/linc/parse/file.py
--rw-r--r--   0        0        0     2860 2023-06-07 01:03:22.236254 linc-1.6.0/linc/parse/header.py
--rw-r--r--   0        0        0      355 2023-06-07 01:03:22.236254 linc-1.6.0/linc/parse/utils.py
--rw-r--r--   0        0        0     1810 2023-06-07 13:25:10.157503 linc-1.6.0/linc/reader.py
--rw-r--r--   0        0        0     1468 2023-06-07 01:03:22.236254 linc-1.6.0/linc/utils.py
--rw-r--r--   0        0        0     1332 2023-06-07 01:03:22.239644 linc-1.6.0/linc/write/common.py
--rw-r--r--   0        0        0     6259 2023-06-07 01:03:22.239644 linc-1.6.0/linc/write/writer_nc.py
--rw-r--r--   0        0        0      659 2023-06-07 13:38:53.822694 linc-1.6.0/pyproject.toml
--rw-r--r--   0        0        0      139 2023-06-07 01:03:22.218726 linc-1.6.0/README.md
--rw-r--r--   0        0        0      773 1970-01-01 00:00:00.000000 linc-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0      331 2023-06-07 01:03:22.218726 linc-1.7.0/linc/__init__.py
+-rw-r--r--   0        0        0     1109 2023-06-07 01:03:22.218726 linc-1.7.0/linc/cli.py
+-rw-r--r--   0        0        0       96 2023-06-07 01:03:22.232840 linc-1.7.0/linc/config/__init__.py
+-rw-r--r--   0        0        0       35 2023-06-07 01:03:22.232840 linc-1.7.0/linc/config/default-config.toml
+-rw-r--r--   0        0        0     1276 2023-06-07 13:28:15.945042 linc-1.7.0/linc/config/models.py
+-rw-r--r--   0        0        0      967 2023-06-07 01:03:22.232840 linc-1.7.0/linc/config/read.py
+-rw-r--r--   0        0        0     3154 2023-06-08 22:49:08.303808 linc-1.7.0/linc/convertion.py
+-rw-r--r--   0        0        0     2846 2023-06-07 01:03:22.234945 linc-1.7.0/linc/models.py
+-rw-r--r--   0        0        0       80 2023-06-07 01:03:22.236254 linc-1.7.0/linc/parse/__init__.py
+-rw-r--r--   0        0        0       42 2023-06-07 01:03:22.236254 linc-1.7.0/linc/parse/constants.py
+-rw-r--r--   0        0        0     1128 2023-06-08 22:49:12.937070 linc-1.7.0/linc/parse/dataset.py
+-rw-r--r--   0        0        0      256 2023-06-07 01:03:22.236254 linc-1.7.0/linc/parse/file.py
+-rw-r--r--   0        0        0     2860 2023-06-07 01:03:22.236254 linc-1.7.0/linc/parse/header.py
+-rw-r--r--   0        0        0      355 2023-06-07 01:03:22.236254 linc-1.7.0/linc/parse/utils.py
+-rw-r--r--   0        0        0     1810 2023-06-07 13:25:10.157503 linc-1.7.0/linc/reader.py
+-rw-r--r--   0        0        0     1468 2023-06-07 01:03:22.236254 linc-1.7.0/linc/utils.py
+-rw-r--r--   0        0        0     1332 2023-06-07 01:03:22.239644 linc-1.7.0/linc/write/common.py
+-rw-r--r--   0        0        0     6259 2023-06-07 01:03:22.239644 linc-1.7.0/linc/write/writer_nc.py
+-rw-r--r--   0        0        0      659 2023-06-08 22:53:55.640762 linc-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0      139 2023-06-07 01:03:22.218726 linc-1.7.0/README.md
+-rw-r--r--   0        0        0      773 1970-01-01 00:00:00.000000 linc-1.7.0/PKG-INFO
```

### Comparing `linc-1.6.0/linc/cli.py` & `linc-1.7.0/linc/cli.py`

 * *Files identical despite different names*

### Comparing `linc-1.6.0/linc/config/models.py` & `linc-1.7.0/linc/config/models.py`

 * *Files identical despite different names*

### Comparing `linc-1.6.0/linc/config/read.py` & `linc-1.7.0/linc/config/read.py`

 * *Files identical despite different names*

### Comparing `linc-1.6.0/linc/convertion.py` & `linc-1.7.0/linc/convertion.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+
 import numpy as np
 import pandas as pd
 
 
 from .models import Channel, DataFile, DataFileU32, MeasurementTypeEnum
 from .utils import device_id_to_str
 from .config import Config
@@ -44,17 +45,15 @@
 
     return DataFile(header=data_file.header, dataset=final_dataset)
 
 
 def _to_physical(channel: Channel, dataset: pd.Series, config: Config) -> pd.Series:
     match channel.device_id.type:
         case MeasurementTypeEnum.ANALOG:
-            _d = (1000 * dataset * channel.dc_dr) / (
-                channel.shots * (2**channel.adc_bits - 1)
-            )
+            _d = dataset * ( 1000*channel.dc_dr/ ( channel.shots * (2**channel.adc_bits - 1) ) )
         case MeasurementTypeEnum.PHOTONCOUNTING:
             _d = (dataset * config.lidar.bins_per_microsecond) / (
                 channel.shots  # Microseconds conversion output in MHz
             )
         case MeasurementTypeEnum.POWERMETER:
             _d = dataset / channel.shots  # Just apply normalization
         case MeasurementTypeEnum.POWERMETER_PHOTODIODE:
```

### Comparing `linc-1.6.0/linc/models.py` & `linc-1.7.0/linc/models.py`

 * *Files identical despite different names*

### Comparing `linc-1.6.0/linc/parse/header.py` & `linc-1.7.0/linc/parse/header.py`

 * *Files identical despite different names*

### Comparing `linc-1.6.0/linc/reader.py` & `linc-1.7.0/linc/reader.py`

 * *Files identical despite different names*

### Comparing `linc-1.6.0/linc/utils.py` & `linc-1.7.0/linc/utils.py`

 * *Files identical despite different names*

### Comparing `linc-1.6.0/linc/write/common.py` & `linc-1.7.0/linc/write/common.py`

 * *Files identical despite different names*

### Comparing `linc-1.6.0/linc/write/writer_nc.py` & `linc-1.7.0/linc/write/writer_nc.py`

 * *Files identical despite different names*

### Comparing `linc-1.6.0/pyproject.toml` & `linc-1.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "linc"
-version = "1.6.0"
+version = "1.7.0"
 description = "A package to handle LICEL Binary format"
 authors = ["Juan Diego <jdlar@eafit.edu.co>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
```

### Comparing `linc-1.6.0/PKG-INFO` & `linc-1.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linc
-Version: 1.6.0
+Version: 1.7.0
 Summary: A package to handle LICEL Binary format
 License: MIT
 Author: Juan Diego
 Author-email: jdlar@eafit.edu.co
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

