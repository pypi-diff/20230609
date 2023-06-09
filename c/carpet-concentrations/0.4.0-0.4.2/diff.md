# Comparing `tmp/carpet_concentrations-0.4.0.tar.gz` & `tmp/carpet_concentrations-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carpet_concentrations-0.4.0.tar", max compression
+gzip compressed data, was "carpet_concentrations-0.4.2.tar", max compression
```

## Comparing `carpet_concentrations-0.4.0.tar` & `carpet_concentrations-0.4.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1524 2023-06-07 05:02:12.405315 carpet_concentrations-0.4.0/LICENSE
--rw-r--r--   0        0        0     2093 2023-06-07 05:02:12.405315 carpet_concentrations-0.4.0/README.md
--rw-r--r--   0        0        0     4466 2023-06-07 05:50:26.459595 carpet_concentrations-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      199 2023-06-07 05:02:12.409315 carpet_concentrations-0.4.0/src/carpet_concentrations/__init__.py
--rw-r--r--   0        0        0     2975 2023-06-07 05:02:12.409315 carpet_concentrations-0.4.0/src/carpet_concentrations/attrs_utils.py
--rw-r--r--   0        0        0     2812 2023-06-07 05:02:12.409315 carpet_concentrations-0.4.0/src/carpet_concentrations/exceptions.py
--rw-r--r--   0        0        0      139 2023-06-07 05:02:12.409315 carpet_concentrations-0.4.0/src/carpet_concentrations/gridders/__init__.py
--rw-r--r--   0        0        0     6629 2023-06-07 05:02:12.409315 carpet_concentrations-0.4.0/src/carpet_concentrations/gridders/latitude_seasonality_gridder.py
--rw-r--r--   0        0        0       94 2023-06-07 05:02:12.409315 carpet_concentrations-0.4.0/src/carpet_concentrations/input4MIPs/__init__.py
--rw-r--r--   0        0        0    18464 2023-06-07 05:02:12.409315 carpet_concentrations-0.4.0/src/carpet_concentrations/input4MIPs/dataset.py
--rw-r--r--   0        0        0     1592 2023-06-07 05:02:12.409315 carpet_concentrations-0.4.0/src/carpet_concentrations/input4MIPs/metadata_options.py
--rw-r--r--   0        0        0        0 2023-06-07 05:02:12.409315 carpet_concentrations-0.4.0/src/carpet_concentrations/py.typed
--rw-r--r--   0        0        0     1429 2023-06-07 05:02:12.409315 carpet_concentrations-0.4.0/src/carpet_concentrations/testing.py
--rw-r--r--   0        0        0     4948 2023-06-07 05:02:12.409315 carpet_concentrations-0.4.0/src/carpet_concentrations/time.py
--rw-r--r--   0        0        0     1334 2023-06-07 05:02:12.409315 carpet_concentrations-0.4.0/src/carpet_concentrations/xarray_pint_utils.py
--rw-r--r--   0        0        0     3554 2023-06-07 05:02:12.409315 carpet_concentrations-0.4.0/src/carpet_concentrations/xarray_utils.py
--rw-r--r--   0        0        0     3438 1970-01-01 00:00:00.000000 carpet_concentrations-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1524 2023-06-09 03:16:43.933007 carpet_concentrations-0.4.2/LICENSE
+-rw-r--r--   0        0        0     2097 2023-06-09 03:16:43.933007 carpet_concentrations-0.4.2/README.md
+-rw-r--r--   0        0        0     4466 2023-06-09 03:16:43.937007 carpet_concentrations-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0      199 2023-06-09 03:16:43.937007 carpet_concentrations-0.4.2/src/carpet_concentrations/__init__.py
+-rw-r--r--   0        0        0     2975 2023-06-09 03:16:43.937007 carpet_concentrations-0.4.2/src/carpet_concentrations/attrs_utils.py
+-rw-r--r--   0        0        0     2812 2023-06-09 03:16:43.937007 carpet_concentrations-0.4.2/src/carpet_concentrations/exceptions.py
+-rw-r--r--   0        0        0      139 2023-06-09 03:16:43.937007 carpet_concentrations-0.4.2/src/carpet_concentrations/gridders/__init__.py
+-rw-r--r--   0        0        0     6629 2023-06-09 03:16:43.937007 carpet_concentrations-0.4.2/src/carpet_concentrations/gridders/latitude_seasonality_gridder.py
+-rw-r--r--   0        0        0       94 2023-06-09 03:16:43.937007 carpet_concentrations-0.4.2/src/carpet_concentrations/input4MIPs/__init__.py
+-rw-r--r--   0        0        0    18529 2023-06-09 03:16:43.937007 carpet_concentrations-0.4.2/src/carpet_concentrations/input4MIPs/dataset.py
+-rw-r--r--   0        0        0     1953 2023-06-09 03:16:43.937007 carpet_concentrations-0.4.2/src/carpet_concentrations/input4MIPs/metadata_options.py
+-rw-r--r--   0        0        0        0 2023-06-09 03:16:43.937007 carpet_concentrations-0.4.2/src/carpet_concentrations/py.typed
+-rw-r--r--   0        0        0     1429 2023-06-09 03:16:43.937007 carpet_concentrations-0.4.2/src/carpet_concentrations/testing.py
+-rw-r--r--   0        0        0     4948 2023-06-09 03:16:43.937007 carpet_concentrations-0.4.2/src/carpet_concentrations/time.py
+-rw-r--r--   0        0        0     1334 2023-06-09 03:16:43.937007 carpet_concentrations-0.4.2/src/carpet_concentrations/xarray_pint_utils.py
+-rw-r--r--   0        0        0     3554 2023-06-09 03:16:43.937007 carpet_concentrations-0.4.2/src/carpet_concentrations/xarray_utils.py
+-rw-r--r--   0        0        0     3442 1970-01-01 00:00:00.000000 carpet_concentrations-0.4.2/PKG-INFO
```

### Comparing `carpet_concentrations-0.4.0/LICENSE` & `carpet_concentrations-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `carpet_concentrations-0.4.0/README.md` & `carpet_concentrations-0.4.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # Carpet - Concentrations
 
 <!--- sec-begin-description -->
 
-[#1 badges here]
+[TODO badges here]
 
 Core tools for the development of greenhouse gas concentration input files (i.e. flying carpets).
 
 <!---
 Can use start-after and end-before directives in docs, see
 https://myst-parser.readthedocs.io/en/latest/syntax/organising_content.html#inserting-other-documents-directly-into-the-current-document
 -->
 
 <!--- sec-end-description -->
 
-Full documentation can be found at: [#2 read the docs link here]
+Full documentation can be found at: [TODO read the docs link here]
 
 ## Installation
 
 <!--- sec-begin-installation -->
 
 Carpet - Concentrations can be installed with conda or pip:
```

### Comparing `carpet_concentrations-0.4.0/pyproject.toml` & `carpet_concentrations-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.coverage.run]
 source = ["src"]
 branch = true
 
 [tool.poetry]
 name = "carpet-concentrations"
-version = "0.4.0"
+version = "0.4.2"
 description = "Core tools for the development of greenhouse gas concentration input files (i.e. flying carpets)."
 authors = ["Zebedee Nicholls <zebedee.nicholls@climate-resource.com>"]
 readme = "README.md"
 packages = [{include = "carpet_concentrations", from = "src"}]
 license = "BSD-3-Clause"
 
 [tool.commitizen]
-version = "0.4.0"
+version = "0.4.2"
 version_files = ["pyproject.toml:^version"]
 tag_format = "v$version"
 major_version_zero = true
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `carpet_concentrations-0.4.0/src/carpet_concentrations/attrs_utils.py` & `carpet_concentrations-0.4.2/src/carpet_concentrations/attrs_utils.py`

 * *Files identical despite different names*

### Comparing `carpet_concentrations-0.4.0/src/carpet_concentrations/exceptions.py` & `carpet_concentrations-0.4.2/src/carpet_concentrations/exceptions.py`

 * *Files identical despite different names*

### Comparing `carpet_concentrations-0.4.0/src/carpet_concentrations/gridders/latitude_seasonality_gridder.py` & `carpet_concentrations-0.4.2/src/carpet_concentrations/gridders/latitude_seasonality_gridder.py`

 * *Files identical despite different names*

### Comparing `carpet_concentrations-0.4.0/src/carpet_concentrations/input4MIPs/dataset.py` & `carpet_concentrations-0.4.2/src/carpet_concentrations/input4MIPs/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from attrs.validators import in_, matches_re
 
 from carpet_concentrations.input4MIPs.metadata_options import (
     ACTIVITY_ID_OPTIONS,
     CONVENTION_OPTIONS,
     CREATION_DATE_REGEX,
     DATASET_CATEGORY_OPTIONS,
+    FREQUENCY_OPTIONS,
     INCLUDES_EMAIL_REGEX,
     UUID_REGEX,
 )
 from carpet_concentrations.time import get_start_of_next_month, split_time_to_year_month
 
 if TYPE_CHECKING:
     from pathlib import Path
@@ -55,15 +56,15 @@
 
     Conventions: str = field(validator=in_(CONVENTION_OPTIONS))
     """CF conventions adhered to by the dataset"""
 
     dataset_category: str = field(validator=in_(DATASET_CATEGORY_OPTIONS))
     """Datset category"""
 
-    frequency: str
+    frequency: str = field(validator=in_(FREQUENCY_OPTIONS))
     """Time frequency of the dataset"""
 
     further_info_url: str
     """URL with further information"""
 
     grid_label: str
     """Grid label of the dataset"""
```

### Comparing `carpet_concentrations-0.4.0/src/carpet_concentrations/input4MIPs/metadata_options.py` & `carpet_concentrations-0.4.2/src/carpet_concentrations/input4MIPs/metadata_options.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 """
 Metdata options
 
 This module could be refactored so that it is autogenerated from some other
 source (or simply be an adapter to some other API) in future to remove the
 need for manual updates.
+
+This might be the right source: https://github.com/PCMDI/input4MIPs-cmor-tables
 """
 from __future__ import annotations
 
 import re
+from collections.abc import Container
 
 ACTIVITY_ID_OPTIONS: tuple[str, ...] = ("input4MIPs",)
 """
 Valid options for "activity_id""
 """
 
 CONVENTION_OPTIONS: tuple[str, ...] = ("CF-1.7 CMIP-6.2", "CF-1.6")
@@ -54,7 +57,27 @@
 
 UUID_REGEX: re.Pattern[str] = re.compile(
     r"^hdl:21.14100\/[0-9a-z]{8}-[0-9a-z]{4}-[0-9a-z]{4}-[0-9a-z]{4}-[0-9a-z]{12}$"
 )
 """
 Regular expression that checks the creation date is formatted correctly
 """
+
+FREQUENCY_OPTIONS: Container[str] = (
+    "1hr",
+    "1hrCM",
+    "1hrPt",
+    "3hr",
+    "3hrPt",
+    "6hr",
+    "6hrPt",
+    "day",
+    "dec",
+    "fx",
+    "mon",
+    "monC",
+    "monPt",
+    "subhrPt",
+    "yr",
+    "yrC",
+    "yrPt",
+)
```

### Comparing `carpet_concentrations-0.4.0/src/carpet_concentrations/testing.py` & `carpet_concentrations-0.4.2/src/carpet_concentrations/testing.py`

 * *Files identical despite different names*

### Comparing `carpet_concentrations-0.4.0/src/carpet_concentrations/time.py` & `carpet_concentrations-0.4.2/src/carpet_concentrations/time.py`

 * *Files identical despite different names*

### Comparing `carpet_concentrations-0.4.0/src/carpet_concentrations/xarray_pint_utils.py` & `carpet_concentrations-0.4.2/src/carpet_concentrations/xarray_pint_utils.py`

 * *Files identical despite different names*

### Comparing `carpet_concentrations-0.4.0/src/carpet_concentrations/xarray_utils.py` & `carpet_concentrations-0.4.2/src/carpet_concentrations/xarray_utils.py`

 * *Files identical despite different names*

### Comparing `carpet_concentrations-0.4.0/PKG-INFO` & `carpet_concentrations-0.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carpet-concentrations
-Version: 0.4.0
+Version: 0.4.2
 Summary: Core tools for the development of greenhouse gas concentration input files (i.e. flying carpets).
 License: BSD-3-Clause
 Author: Zebedee Nicholls
 Author-email: zebedee.nicholls@climate-resource.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
@@ -30,26 +30,26 @@
 Requires-Dist: xarray (>=2023.4.2,<2024.0.0)
 Description-Content-Type: text/markdown
 
 # Carpet - Concentrations
 
 <!--- sec-begin-description -->
 
-[#1 badges here]
+[TODO badges here]
 
 Core tools for the development of greenhouse gas concentration input files (i.e. flying carpets).
 
 <!---
 Can use start-after and end-before directives in docs, see
 https://myst-parser.readthedocs.io/en/latest/syntax/organising_content.html#inserting-other-documents-directly-into-the-current-document
 -->
 
 <!--- sec-end-description -->
 
-Full documentation can be found at: [#2 read the docs link here]
+Full documentation can be found at: [TODO read the docs link here]
 
 ## Installation
 
 <!--- sec-begin-installation -->
 
 Carpet - Concentrations can be installed with conda or pip:
```

