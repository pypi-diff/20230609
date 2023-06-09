# Comparing `tmp/ods_tools-3.0.6.tar.gz` & `tmp/ods_tools-3.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ods_tools-3.0.6.tar", last modified: Thu May 11 14:33:33 2023, max compression
+gzip compressed data, was "ods_tools-3.0.7.tar", last modified: Fri Jun  9 09:03:21 2023, max compression
```

## Comparing `ods_tools-3.0.6.tar` & `ods_tools-3.0.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:33:33.864809 ods_tools-3.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     8418 2023-05-11 14:33:33.864809 ods_tools-3.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8119 2023-05-11 14:33:13.000000 ods_tools-3.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:33:33.860809 ods_tools-3.0.6/ods_tools/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-11 14:33:13.000000 ods_tools-3.0.6/ods_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-05-11 14:33:13.000000 ods_tools-3.0.6/ods_tools/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:33:33.864809 ods_tools-3.0.6/ods_tools/oed/
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-11 14:33:13.000000 ods_tools-3.0.6/ods_tools/oed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-05-11 14:33:13.000000 ods_tools-3.0.6/ods_tools/oed/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     8981 2023-05-11 14:33:13.000000 ods_tools-3.0.6/ods_tools/oed/exposure.py
--rw-r--r--   0 runner    (1001) docker     (123)    11177 2023-05-11 14:33:13.000000 ods_tools-3.0.6/ods_tools/oed/forex.py
--rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-05-11 14:33:13.000000 ods_tools-3.0.6/ods_tools/oed/oed_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     9321 2023-05-11 14:33:13.000000 ods_tools-3.0.6/ods_tools/oed/setting_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    20875 2023-05-11 14:33:13.000000 ods_tools-3.0.6/ods_tools/oed/source.py
--rw-r--r--   0 runner    (1001) docker     (123)    14767 2023-05-11 14:33:13.000000 ods_tools-3.0.6/ods_tools/oed/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:33:33.864809 ods_tools-3.0.6/ods_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8418 2023-05-11 14:33:33.000000 ods_tools-3.0.6/ods_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-11 14:33:33.000000 ods_tools-3.0.6/ods_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 14:33:33.000000 ods_tools-3.0.6/ods_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-11 14:33:33.000000 ods_tools-3.0.6/ods_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-11 14:33:33.000000 ods_tools-3.0.6/ods_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-11 14:33:33.000000 ods_tools-3.0.6/ods_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 14:33:33.864809 ods_tools-3.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-05-11 14:33:13.000000 ods_tools-3.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:03:21.818235 ods_tools-3.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     8418 2023-06-09 09:03:21.814235 ods_tools-3.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8119 2023-06-09 09:03:04.000000 ods_tools-3.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:03:21.810235 ods_tools-3.0.7/ods_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-09 09:03:04.000000 ods_tools-3.0.7/ods_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-06-09 09:03:04.000000 ods_tools-3.0.7/ods_tools/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:03:21.814235 ods_tools-3.0.7/ods_tools/oed/
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-06-09 09:03:04.000000 ods_tools-3.0.7/ods_tools/oed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-06-09 09:03:04.000000 ods_tools-3.0.7/ods_tools/oed/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8981 2023-06-09 09:03:04.000000 ods_tools-3.0.7/ods_tools/oed/exposure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11177 2023-06-09 09:03:04.000000 ods_tools-3.0.7/ods_tools/oed/forex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-06-09 09:03:04.000000 ods_tools-3.0.7/ods_tools/oed/oed_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9317 2023-06-09 09:03:04.000000 ods_tools-3.0.7/ods_tools/oed/setting_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21203 2023-06-09 09:03:04.000000 ods_tools-3.0.7/ods_tools/oed/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14835 2023-06-09 09:03:04.000000 ods_tools-3.0.7/ods_tools/oed/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:03:21.814235 ods_tools-3.0.7/ods_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8418 2023-06-09 09:03:21.000000 ods_tools-3.0.7/ods_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-09 09:03:21.000000 ods_tools-3.0.7/ods_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 09:03:21.000000 ods_tools-3.0.7/ods_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-09 09:03:21.000000 ods_tools-3.0.7/ods_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-09 09:03:21.000000 ods_tools-3.0.7/ods_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-09 09:03:21.000000 ods_tools-3.0.7/ods_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 09:03:21.818235 ods_tools-3.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-06-09 09:03:04.000000 ods_tools-3.0.7/setup.py
```

### Comparing `ods_tools-3.0.6/PKG-INFO` & `ods_tools-3.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ods_tools
-Version: 3.0.6
+Version: 3.0.7
 Summary: Tools to manage ODS files
 Home-page: https://github.com/OasisLMF/OpenDataStandards
 Author: Oasis LMF
 Author-email: support@oasislmf.org
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `ods_tools-3.0.6/README.md` & `ods_tools-3.0.7/README.md`

 * *Files identical despite different names*

### Comparing `ods_tools-3.0.6/ods_tools/main.py` & `ods_tools-3.0.7/ods_tools/main.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,16 +6,21 @@
     'convert',
     'check'
 ]
 
 import argparse
 import logging
 
-from ods_tools.oed import OedExposure, OdsException
 from ods_tools import logger
+from ods_tools.oed import (
+    OedExposure,
+    OdsException,
+    ModelSettingSchema,
+    AnalysisSettingSchema,
+)
 
 
 def get_oed_exposure(config_json=None, oed_dir=None, **kwargs):
     if config_json:
         return OedExposure.from_config(config_json, **kwargs)
     elif oed_dir:
         return OedExposure.from_dir(oed_dir, **kwargs)
@@ -30,16 +35,29 @@
         if value is not None:
             exposure_kwargs[param] = value
     return exposure_kwargs
 
 
 def check(**kwargs):
     """run the check command on Exposure"""
-    oed_exposure = get_oed_exposure(**extract_exposure_args(kwargs))
-    oed_exposure.check(**kwargs)
+    logger = logging.getLogger(__name__)
+    args_set = {k for k, v in kwargs.items() if v is not None}
+    args_exp = set(['location', 'account', 'ri_info', 'ri_scope'])
+
+    try:
+        if args_exp.intersection(set(args_set)):
+            oed_exposure = get_oed_exposure(**extract_exposure_args(kwargs))
+            oed_exposure.check()
+        if 'analysis_settings_json' in args_set:
+            AnalysisSettingSchema().validate_file(kwargs['analysis_settings_json'])
+        if 'model_settings_json' in args_set:
+            ModelSettingSchema().validate_file(kwargs['model_settings_json'])
+    except OdsException as e:
+        logger.error('Validation failed:')
+        logger.error(e)
 
 
 def convert(**kwargs):
     """Convert exposure data to an other format (ex: csv to parquet)"""
     path = kwargs.pop('output_dir', None) or kwargs.get('oed_dir', None)
     if not path:
         raise OdsException('--output-dir or --oed-dir need to be provided to perform convert')
@@ -66,15 +84,15 @@
 main_parser = argparse.ArgumentParser()
 
 oed_exposure_creation = """
 there are several options to specify the exposure data,
  - by providing  the path to each OED source using `--location`, `--account`, `--ri-info`, `--ri-scope`.
  - by providing  an OED config json file using `--config-json`.
  - by providing  the path to the directory where the exposure is stored using `--oed-dir`.
- 
+
 if multiple options are use at the same time, --config-json will have the priority over --oed-dir
 specific paths (--location, --account, --ri-info, --ri-scope) will overwrite the path found in (--config-json or --oed-dir)
  """
 
 
 convert_description = """
 convert OED files to an other format
@@ -94,14 +112,16 @@
 check_description = """
 check exposure data.
 """
 
 check_command = command_parser.add_parser('check', description=check_description + oed_exposure_creation,
                                           formatter_class=argparse.RawTextHelpFormatter)
 add_exposure_data_args(check_command)
+check_command.add_argument('--model-settings-json', help='Path to Model settings meta-data file to check', default=None)
+check_command.add_argument('--analysis-settings-json', help='Path to Analysis settings file to check', default=None)
 check_command.add_argument('-v', '--logging-level', help='logging level (debug:10, info:20, warning:30, error:40, critical:50)',
                            default=30, type=int)
 
 
 def main():
     """command line interface for ODS conversion between csv and parquet"""
     kwargs = vars(main_parser.parse_args())
```

### Comparing `ods_tools-3.0.6/ods_tools/oed/__init__.py` & `ods_tools-3.0.7/ods_tools/oed/__init__.py`

 * *Files identical despite different names*

### Comparing `ods_tools-3.0.6/ods_tools/oed/common.py` & `ods_tools-3.0.7/ods_tools/oed/common.py`

 * *Files identical despite different names*

### Comparing `ods_tools-3.0.6/ods_tools/oed/exposure.py` & `ods_tools-3.0.7/ods_tools/oed/exposure.py`

 * *Files identical despite different names*

### Comparing `ods_tools-3.0.6/ods_tools/oed/forex.py` & `ods_tools-3.0.7/ods_tools/oed/forex.py`

 * *Files identical despite different names*

### Comparing `ods_tools-3.0.6/ods_tools/oed/oed_schema.py` & `ods_tools-3.0.7/ods_tools/oed/oed_schema.py`

 * *Files identical despite different names*

### Comparing `ods_tools-3.0.6/ods_tools/oed/setting_schema.py` & `ods_tools-3.0.7/ods_tools/oed/setting_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,15 @@
         """
         Replaces the dictionary value of key with replace_value in the obj dictionary.
         """
         if not isinstance(obj, (dict, list)):
             return None  # base case exit
 
         if key_old in obj:
-            obj[key_new] = obj.pop(key_old)
+            obj[key_new] = obj[key_old]
 
         if isinstance(obj, dict):
             for k, v in obj.items():
                 self._remap_key(v, key_new, key_old)
         else:
             for v in obj:
                 self._remap_key(v, key_new, key_old)
```

### Comparing `ods_tools-3.0.6/ods_tools/oed/source.py` & `ods_tools-3.0.7/ods_tools/oed/source.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from pathlib import Path
 import mimetypes
 
+import logging
 import pandas as pd
 import numpy as np
 from chardet.universaldetector import UniversalDetector
 
 from .common import OED_TYPE_TO_NAME, OdsException, PANDAS_COMPRESSION_MAP, PANDAS_DEFAULT_NULL_VALUES, is_relative, BLANK_VALUES
 from .forex import convert_currency
 from .oed_schema import OedSchema
 
+logger = logging.getLogger(__file__)
+
 try:
     from functools import cached_property
 except ImportError:  # support for python < 3.8
     _missing = object()
 
     class cached_property(object):
         """A decorator that converts a function into a lazy property.  The
@@ -226,14 +229,16 @@
         ods_fields = exposure.get_input_fields(oed_type)
         column_to_field = OedSchema.column_to_field(oed_df.columns, ods_fields)
         oed_df = cls.as_oed_type(oed_df, column_to_field)
         oed_df = cls.prepare_df(oed_df, column_to_field, ods_fields)
         if exposure.use_field:
             oed_df = OedSchema.use_field(oed_df, ods_fields)
         oed_source.dataframe = oed_df
+        if oed_df.empty:
+            logger.info(f'{oed_source.oed_name} {oed_source} is empty')
         oed_source.loaded = True
         return oed_source
 
     @classmethod
     def from_filepath(cls, exposure, oed_type, filepath, read_param=None):
         """
         OedSource Constructor from a filepath
@@ -284,14 +289,16 @@
             else:
                 raise OdsException(f'Unsupported stream format {format}')
         except Exception as e:
             raise OdsException('Failed to read stream data') from e
 
         oed_source.dataframe = oed_df
         oed_source.loaded = True
+        if oed_df.empty:
+            logger.info(f'{oed_source.oed_name} {oed_source} is empty')
         return oed_source
 
     @classmethod
     def as_oed_type(cls, oed_df, column_to_field):
         pd_dtype = {}
         to_tmp_dtype = {}
         for column in oed_df.columns:
@@ -347,18 +354,20 @@
                         if field_info['Default'] != 'n/a':
                             df[col] = df[col].fillna(df[col].dtype.type(field_info['Default'])).astype(field_info['pd_dtype'])
         return df
 
     @cached_property
     def dataframe(self):
         """Dataframe view of the OedSource, loaded once"""
-        self.loaded = True
         df = self.load_dataframe()
         if self.exposure.use_field:
             df = OedSchema.use_field(df, self.exposure.get_input_fields(self.oed_type))
+        self.loaded = True
+        if df.empty:
+            logger.info(f'{self.oed_name} {self} is empty')
         return df
 
     @property
     def current_source(self):
         """
         current version of the oed source
         Returns:
```

### Comparing `ods_tools-3.0.6/ods_tools/oed/validator.py` & `ods_tools-3.0.7/ods_tools/oed/validator.py`

 * *Files 0% similar despite different names*

```diff
@@ -186,14 +186,16 @@
         using Oed perils list specification, check that Peril column have valid peril values
         Returns:
             list of invalid_data
         """
         invalid_data = []
         for oed_source in self.exposure.get_oed_sources():
             identifier_field = self.identifier_field_maps[oed_source]
+            if oed_source.dataframe.empty:
+                continue
             for column in oed_source.dataframe.columns.intersection(set(OED_PERIL_COLUMNS)):
                 peril_values = oed_source.dataframe[column].str.split(';').apply(pd.Series, 1).stack()
                 invalid_perils = oed_source.dataframe.iloc[
                     peril_values[~peril_values.isin(
                         set(self.exposure.oed_schema.schema['perils']['info']) | BLANK_VALUES
                     )].index.droplevel(-1)]
                 if not invalid_perils.empty:
```

### Comparing `ods_tools-3.0.6/ods_tools.egg-info/PKG-INFO` & `ods_tools-3.0.7/ods_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ods-tools
-Version: 3.0.6
+Version: 3.0.7
 Summary: Tools to manage ODS files
 Home-page: https://github.com/OasisLMF/OpenDataStandards
 Author: Oasis LMF
 Author-email: support@oasislmf.org
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `ods_tools-3.0.6/setup.py` & `ods_tools-3.0.7/setup.py`

 * *Files identical despite different names*

