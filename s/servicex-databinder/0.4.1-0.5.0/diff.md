# Comparing `tmp/servicex_databinder-0.4.1.tar.gz` & `tmp/servicex_databinder-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "servicex_databinder-0.4.1.tar", last modified: Fri May 19 20:10:53 2023, max compression
+gzip compressed data, was "servicex_databinder-0.5.0.tar", last modified: Fri Jun  9 04:56:13 2023, max compression
```

## Comparing `servicex_databinder-0.4.1.tar` & `servicex_databinder-0.5.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 kchoi      (501) staff       (20)        0 2023-05-19 20:10:53.396991 servicex_databinder-0.4.1/
--rw-r--r--   0 kchoi      (501) staff       (20)     1521 2021-09-10 04:56:21.000000 servicex_databinder-0.4.1/LICENSE
--rw-r--r--   0 kchoi      (501) staff       (20)     9996 2023-05-19 20:10:53.396359 servicex_databinder-0.4.1/PKG-INFO
--rw-r--r--   0 kchoi      (501) staff       (20)     9230 2023-05-19 20:08:18.000000 servicex_databinder-0.4.1/README.md
-drwxr-xr-x   0 kchoi      (501) staff       (20)        0 2023-05-19 20:10:53.392432 servicex_databinder-0.4.1/servicex_databinder/
--rw-r--r--   0 kchoi      (501) staff       (20)      200 2023-05-19 20:06:27.000000 servicex_databinder-0.4.1/servicex_databinder/__init__.py
--rw-r--r--   0 kchoi      (501) staff       (20)     7030 2023-05-09 00:07:57.000000 servicex_databinder-0.4.1/servicex_databinder/configuration.py
--rw-r--r--   0 kchoi      (501) staff       (20)    10174 2023-05-09 00:07:45.000000 servicex_databinder-0.4.1/servicex_databinder/get_servicex_data.py
--rw-r--r--   0 kchoi      (501) staff       (20)     3135 2022-11-11 14:54:29.000000 servicex_databinder-0.4.1/servicex_databinder/old_frontend.py
--rw-r--r--   0 kchoi      (501) staff       (20)    14312 2022-11-10 06:04:16.000000 servicex_databinder-0.4.1/servicex_databinder/old_output.py
--rw-r--r--   0 kchoi      (501) staff       (20)     7138 2023-05-19 19:57:15.000000 servicex_databinder-0.4.1/servicex_databinder/output_handler.py
--rw-r--r--   0 kchoi      (501) staff       (20)     5313 2023-05-19 20:00:13.000000 servicex_databinder-0.4.1/servicex_databinder/request.py
--rw-r--r--   0 kchoi      (501) staff       (20)     1493 2023-05-05 22:26:25.000000 servicex_databinder-0.4.1/servicex_databinder/servicex_databinder.py
-drwxr-xr-x   0 kchoi      (501) staff       (20)        0 2023-05-19 20:10:53.394850 servicex_databinder-0.4.1/servicex_databinder.egg-info/
--rw-r--r--   0 kchoi      (501) staff       (20)     9996 2023-05-19 20:10:53.000000 servicex_databinder-0.4.1/servicex_databinder.egg-info/PKG-INFO
--rw-r--r--   0 kchoi      (501) staff       (20)      553 2023-05-19 20:10:53.000000 servicex_databinder-0.4.1/servicex_databinder.egg-info/SOURCES.txt
--rw-r--r--   0 kchoi      (501) staff       (20)        1 2023-05-19 20:10:53.000000 servicex_databinder-0.4.1/servicex_databinder.egg-info/dependency_links.txt
--rw-r--r--   0 kchoi      (501) staff       (20)      123 2023-05-19 20:10:53.000000 servicex_databinder-0.4.1/servicex_databinder.egg-info/requires.txt
--rw-r--r--   0 kchoi      (501) staff       (20)       20 2023-05-19 20:10:53.000000 servicex_databinder-0.4.1/servicex_databinder.egg-info/top_level.txt
--rw-r--r--   0 kchoi      (501) staff       (20)       38 2023-05-19 20:10:53.397081 servicex_databinder-0.4.1/setup.cfg
--rw-r--r--   0 kchoi      (501) staff       (20)     2117 2023-05-10 03:52:22.000000 servicex_databinder-0.4.1/setup.py
-drwxr-xr-x   0 kchoi      (501) staff       (20)        0 2023-05-19 20:10:53.395358 servicex_databinder-0.4.1/tests/
--rw-r--r--   0 kchoi      (501) staff       (20)     5461 2021-10-28 07:08:46.000000 servicex_databinder-0.4.1/tests/test_config.py
+drwxr-xr-x   0 kchoi      (501) staff       (20)        0 2023-06-09 04:56:13.464939 servicex_databinder-0.5.0/
+-rw-r--r--   0 kchoi      (501) staff       (20)     1521 2021-09-10 04:56:21.000000 servicex_databinder-0.5.0/LICENSE
+-rw-r--r--   0 kchoi      (501) staff       (20)    10606 2023-06-09 04:56:13.464344 servicex_databinder-0.5.0/PKG-INFO
+-rw-r--r--   0 kchoi      (501) staff       (20)     9840 2023-06-09 03:01:47.000000 servicex_databinder-0.5.0/README.md
+drwxr-xr-x   0 kchoi      (501) staff       (20)        0 2023-06-09 04:56:13.459845 servicex_databinder-0.5.0/servicex_databinder/
+-rw-r--r--   0 kchoi      (501) staff       (20)      200 2023-06-08 12:04:08.000000 servicex_databinder-0.5.0/servicex_databinder/__init__.py
+-rw-r--r--   0 kchoi      (501) staff       (20)     7573 2023-06-09 03:01:47.000000 servicex_databinder-0.5.0/servicex_databinder/configuration.py
+-rw-r--r--   0 kchoi      (501) staff       (20)     5938 2023-06-09 03:01:47.000000 servicex_databinder-0.5.0/servicex_databinder/get_servicex_data.py
+-rw-r--r--   0 kchoi      (501) staff       (20)     3135 2022-11-11 14:54:29.000000 servicex_databinder-0.5.0/servicex_databinder/old_frontend.py
+-rw-r--r--   0 kchoi      (501) staff       (20)    14312 2022-11-10 06:04:16.000000 servicex_databinder-0.5.0/servicex_databinder/old_output.py
+-rw-r--r--   0 kchoi      (501) staff       (20)     9357 2023-06-09 03:01:47.000000 servicex_databinder-0.5.0/servicex_databinder/output_handler.py
+-rw-r--r--   0 kchoi      (501) staff       (20)     5461 2023-06-09 03:01:47.000000 servicex_databinder-0.5.0/servicex_databinder/request.py
+-rw-r--r--   0 kchoi      (501) staff       (20)     1493 2023-06-01 08:29:34.000000 servicex_databinder-0.5.0/servicex_databinder/servicex_databinder.py
+drwxr-xr-x   0 kchoi      (501) staff       (20)        0 2023-06-09 04:56:13.462855 servicex_databinder-0.5.0/servicex_databinder.egg-info/
+-rw-r--r--   0 kchoi      (501) staff       (20)    10606 2023-06-09 04:56:13.000000 servicex_databinder-0.5.0/servicex_databinder.egg-info/PKG-INFO
+-rw-r--r--   0 kchoi      (501) staff       (20)      553 2023-06-09 04:56:13.000000 servicex_databinder-0.5.0/servicex_databinder.egg-info/SOURCES.txt
+-rw-r--r--   0 kchoi      (501) staff       (20)        1 2023-06-09 04:56:13.000000 servicex_databinder-0.5.0/servicex_databinder.egg-info/dependency_links.txt
+-rw-r--r--   0 kchoi      (501) staff       (20)      123 2023-06-09 04:56:13.000000 servicex_databinder-0.5.0/servicex_databinder.egg-info/requires.txt
+-rw-r--r--   0 kchoi      (501) staff       (20)       20 2023-06-09 04:56:13.000000 servicex_databinder-0.5.0/servicex_databinder.egg-info/top_level.txt
+-rw-r--r--   0 kchoi      (501) staff       (20)       38 2023-06-09 04:56:13.465046 servicex_databinder-0.5.0/setup.cfg
+-rw-r--r--   0 kchoi      (501) staff       (20)     2117 2023-05-30 02:20:52.000000 servicex_databinder-0.5.0/setup.py
+drwxr-xr-x   0 kchoi      (501) staff       (20)        0 2023-06-09 04:56:13.463442 servicex_databinder-0.5.0/tests/
+-rw-r--r--   0 kchoi      (501) staff       (20)     5461 2023-05-31 01:56:07.000000 servicex_databinder-0.5.0/tests/test_config.py
```

### Comparing `servicex_databinder-0.4.1/LICENSE` & `servicex_databinder-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `servicex_databinder-0.4.1/PKG-INFO` & `servicex_databinder-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: servicex_databinder
-Version: 0.4.1
+Version: 0.5.0
 Summary: ServiceX data management                     using a configuration file
 Home-page: https://github.com/kyungeonchoi/ServiceXDataBinder
 Author: KyungEon Choi (UT Austin)
 Author-email: kyungeonchoi@utexas.edu
 License: BSD 3-clause
 Platform: Any
 Classifier: Development Status :: 3 - Alpha
@@ -17,29 +17,29 @@
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ServiceX DataBinder
 
-<p align="right"> Release v0.4.1 </p>
+<p align="right"> Release v0.5.0 </p>
 
 [![PyPI version](https://badge.fury.io/py/servicex-databinder.svg)](https://badge.fury.io/py/servicex-databinder)
 
 `servicex-databinder` is a user-analysis data management package using a single configuration file. 
 Samples with external data sources (e.g. `RucioDID` or `XRootDFiles`) utilize ServiceX to deliver user-selected columns with optional row filtering.
 <!-- to interact with ServiceX instance to make ServiceX request(s) and manage ServiceX delivered data from a single configuration file. -->
 
 The following table shows supported ServiceX transformers by DataBinder
 
 | Input format | Code generator | Transformer | Output format
 | :--- | :---: | :---: | :---: |
 | ROOT Ntuple | func-adl | `uproot` | `root` or `parquet` |
 | ATLAS Release 21 xAOD | func-adl | `atlasr21`| `root` |
-<!-- | ROOT Ntuple | python function | `python`| -->
+| ROOT Ntuple | python function | `python`| `root` or `parquet` |
 
 <!-- [`ServiceX`](https://github.com/ssl-hep/ServiceX) is a scalable HEP event data extraction, transformation and delivery system. 
 
 ['ServiceX Client library'](https://github.com/ssl-hep/ServiceX_frontend) provides  --> 
 
 ## Prerequisite
 - [Access to a ServiceX instance](https://servicex.readthedocs.io/en/latest/user/getting-started/)
@@ -82,31 +82,34 @@
 Output format can be either `Apache parquet` or `ROOT ntuple` for `uproot` backend. Only `ROOT ntuple` format is supported for `xAOD` backend.
 
 
 The followings are available options:
 
 <!-- `General` block: -->
 | Option for `General` block | Description       | DataType |
-|:--------:|:------:|:------|
+|:--------:|:------|:------|
 | `ServiceXName`* | ServiceX backend name in your `servicex.yaml` file <br>  | `String` |
-| `OutputDirectory` | Path to the directory for ServiceX delivered files | `String` |
 | `OutputFormat`* | Output file format of ServiceX delivered data (`parquet` or `root` for `uproot` / `root` for `xaod`) | `String` |
+| `Transformer` | Set transformer for all Samples. Overwrites the default transformer in the `servicex.yaml` file.  | `String`|
+| `Delivery` | Delivery option; `LocalPath` (default) or `LocalCache` or `ObjectStore` | `String` |
+| `OutputDirectory` | Path to a directory for ServiceX delivered files | `String` |
 | `WriteOutputDict` | Name of an ouput yaml file containing Python nested dictionary of output file paths (located in the `OutputDirectory`) | `String` |
 | `IgnoreServiceXCache` | Ignore the existing ServiceX cache and force to make ServiceX requests | `Boolean` |
 <p align="right"> *Mandatory options</p>
 
 | Option for `Sample` block | Description       |DataType |
-|:--------:|:------:|:------|
-| `Name`   | sample name defined by a user |`String` |
+|:--------:|:------|:------|
+| `Name`   | Sample name defined by a user |`String` |
+| `Transformer` | Transformer for the given sample | `String`|
 | `RucioDID` | Rucio Dataset Id (DID) for a given sample; <br> Can be multiple DIDs separated by comma |`String` |
 | `XRootDFiles` | XRootD files (e.g. `root://`) for a given sample; <br> Can be multiple files separated by comma |`String` |
 | `Tree` | Name of the input ROOT `TTree`; <br> Can be multiple `TTree`s separated by comma (`uproot` ONLY) |`String` |
 | `Filter` | Selection in the TCut syntax, e.g. `jet_pt > 10e3 && jet_eta < 2.0` (TCut ONLY) |`String` |
 | `Columns` | List of columns (or branches) to be delivered; multiple columns separately by comma (TCut ONLY) |`String` |
-| `FuncADL` | func-adl expression for a given sample |`String` |
+| `FuncADL` | Func-adl expression for a given sample |`String` |
 | `LocalPath` | File path directly from local path (NO ServiceX tranformation) | `String` |
 
  <!-- Options exclusively for TCut syntax (CANNOT combine with the option `FuncADL`) -->
 
  <!-- Option for func-adl expression (CANNOT combine with the option `Fitler` and `Columns`) -->
 
 A config file can be simplified by utilizing `Definition` block. You can define placeholders under `Definition` block, which will replace all matched placeholders in the values of `Sample` block. Note that placeholders must start with `DEF_`.
@@ -139,14 +142,23 @@
     Columns: lep_pt, lep_eta
   - Name: Background2
     Transformer: atlasr21
     RucioDID: DEF_Zee_input
     FuncADL: DEF_Zee_query
   - Name: Background3
     LocalPath: /Users/kchoi/Work/data/background3
+  - Name: Background4
+    Transformer: python
+    RucioDID: user.kchoi:user.kchoi.background4
+    Function: |
+      def run_query(input_filenames=None):
+          import awkward as ak, uproot
+          tree_name = "nominal"
+          o = uproot.lazy({input_filenames:tree_name})
+          return {"nominal: o}
 
 Definition:
   DEF_ttH_nominal_query: "Where(lambda e: e.met_met>150e3). \
               Select(lambda event: {'el_pt': event.el_pt, 'jet_e': event.jet_e, \
               'jet_pt': event.jet_pt, 'met_met': event.met_met})"
   DEF_ggH_input: "root://eospublic.cern.ch//eos/opendata/atlas/OutreachDatasets\
                   /2020-01-22/4lep/MC/mc_345060.ggH125_ZZ4lep.4lep.root"
```

### Comparing `servicex_databinder-0.4.1/README.md` & `servicex_databinder-0.5.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # ServiceX DataBinder
 
-<p align="right"> Release v0.4.1 </p>
+<p align="right"> Release v0.5.0 </p>
 
 [![PyPI version](https://badge.fury.io/py/servicex-databinder.svg)](https://badge.fury.io/py/servicex-databinder)
 
 `servicex-databinder` is a user-analysis data management package using a single configuration file. 
 Samples with external data sources (e.g. `RucioDID` or `XRootDFiles`) utilize ServiceX to deliver user-selected columns with optional row filtering.
 <!-- to interact with ServiceX instance to make ServiceX request(s) and manage ServiceX delivered data from a single configuration file. -->
 
 The following table shows supported ServiceX transformers by DataBinder
 
 | Input format | Code generator | Transformer | Output format
 | :--- | :---: | :---: | :---: |
 | ROOT Ntuple | func-adl | `uproot` | `root` or `parquet` |
 | ATLAS Release 21 xAOD | func-adl | `atlasr21`| `root` |
-<!-- | ROOT Ntuple | python function | `python`| -->
+| ROOT Ntuple | python function | `python`| `root` or `parquet` |
 
 <!-- [`ServiceX`](https://github.com/ssl-hep/ServiceX) is a scalable HEP event data extraction, transformation and delivery system. 
 
 ['ServiceX Client library'](https://github.com/ssl-hep/ServiceX_frontend) provides  --> 
 
 ## Prerequisite
 - [Access to a ServiceX instance](https://servicex.readthedocs.io/en/latest/user/getting-started/)
@@ -61,31 +61,34 @@
 Output format can be either `Apache parquet` or `ROOT ntuple` for `uproot` backend. Only `ROOT ntuple` format is supported for `xAOD` backend.
 
 
 The followings are available options:
 
 <!-- `General` block: -->
 | Option for `General` block | Description       | DataType |
-|:--------:|:------:|:------|
+|:--------:|:------|:------|
 | `ServiceXName`* | ServiceX backend name in your `servicex.yaml` file <br>  | `String` |
-| `OutputDirectory` | Path to the directory for ServiceX delivered files | `String` |
 | `OutputFormat`* | Output file format of ServiceX delivered data (`parquet` or `root` for `uproot` / `root` for `xaod`) | `String` |
+| `Transformer` | Set transformer for all Samples. Overwrites the default transformer in the `servicex.yaml` file.  | `String`|
+| `Delivery` | Delivery option; `LocalPath` (default) or `LocalCache` or `ObjectStore` | `String` |
+| `OutputDirectory` | Path to a directory for ServiceX delivered files | `String` |
 | `WriteOutputDict` | Name of an ouput yaml file containing Python nested dictionary of output file paths (located in the `OutputDirectory`) | `String` |
 | `IgnoreServiceXCache` | Ignore the existing ServiceX cache and force to make ServiceX requests | `Boolean` |
 <p align="right"> *Mandatory options</p>
 
 | Option for `Sample` block | Description       |DataType |
-|:--------:|:------:|:------|
-| `Name`   | sample name defined by a user |`String` |
+|:--------:|:------|:------|
+| `Name`   | Sample name defined by a user |`String` |
+| `Transformer` | Transformer for the given sample | `String`|
 | `RucioDID` | Rucio Dataset Id (DID) for a given sample; <br> Can be multiple DIDs separated by comma |`String` |
 | `XRootDFiles` | XRootD files (e.g. `root://`) for a given sample; <br> Can be multiple files separated by comma |`String` |
 | `Tree` | Name of the input ROOT `TTree`; <br> Can be multiple `TTree`s separated by comma (`uproot` ONLY) |`String` |
 | `Filter` | Selection in the TCut syntax, e.g. `jet_pt > 10e3 && jet_eta < 2.0` (TCut ONLY) |`String` |
 | `Columns` | List of columns (or branches) to be delivered; multiple columns separately by comma (TCut ONLY) |`String` |
-| `FuncADL` | func-adl expression for a given sample |`String` |
+| `FuncADL` | Func-adl expression for a given sample |`String` |
 | `LocalPath` | File path directly from local path (NO ServiceX tranformation) | `String` |
 
  <!-- Options exclusively for TCut syntax (CANNOT combine with the option `FuncADL`) -->
 
  <!-- Option for func-adl expression (CANNOT combine with the option `Fitler` and `Columns`) -->
 
 A config file can be simplified by utilizing `Definition` block. You can define placeholders under `Definition` block, which will replace all matched placeholders in the values of `Sample` block. Note that placeholders must start with `DEF_`.
@@ -118,14 +121,23 @@
     Columns: lep_pt, lep_eta
   - Name: Background2
     Transformer: atlasr21
     RucioDID: DEF_Zee_input
     FuncADL: DEF_Zee_query
   - Name: Background3
     LocalPath: /Users/kchoi/Work/data/background3
+  - Name: Background4
+    Transformer: python
+    RucioDID: user.kchoi:user.kchoi.background4
+    Function: |
+      def run_query(input_filenames=None):
+          import awkward as ak, uproot
+          tree_name = "nominal"
+          o = uproot.lazy({input_filenames:tree_name})
+          return {"nominal: o}
 
 Definition:
   DEF_ttH_nominal_query: "Where(lambda e: e.met_met>150e3). \
               Select(lambda event: {'el_pt': event.el_pt, 'jet_e': event.jet_e, \
               'jet_pt': event.jet_pt, 'met_met': event.met_met})"
   DEF_ggH_input: "root://eospublic.cern.ch//eos/opendata/atlas/OutreachDatasets\
                   /2020-01-22/4lep/MC/mc_345060.ggH125_ZZ4lep.4lep.root"
```

### Comparing `servicex_databinder-0.4.1/servicex_databinder/configuration.py` & `servicex_databinder-0.5.0/servicex_databinder/configuration.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,27 +14,29 @@
         input_config (Union[str, pathlib.Path, Dict[str, Any]]):
             path to config file or config as dict
     Returns:
         Dict[str, Any]: configuration
     """
 
     if isinstance(input_config, dict):
+        _decorate_defaults(input_config)
         _replace_definition_in_sample_block(input_config)
         _validate_config(input_config)
         return _update_backend_per_sample(input_config)
     else:
         file_path = pathlib.Path(input_config)
         log.info(f"Loading DataBinder config file: {file_path}")
         try:
             config = yaml.safe_load(file_path.read_text())
+            _decorate_defaults(config)
             _replace_definition_in_sample_block(config)
             _validate_config(config)
             return _update_backend_per_sample(config)
         except Exception:
-            raise FileNotFoundError(
+            raise SyntaxError(
                 f"Exception occured while reading config file: {file_path}"
                 )
 
 
 def _replace_definition_in_sample_block(config: Dict[str, Any]):
     flag = False
     if config.get('Definition'):
@@ -51,14 +53,56 @@
                                         .replace(repre, new_str)
                             flag = True
         return flag
     else:
         return flag
 
 
+def _update_backend_per_sample(config: Dict[str, Any]) -> Dict:
+    """ from servicex.yaml file """
+    backend_type = servicex_config.ServiceXConfigAdaptor()\
+        .get_backend_info(config['General']['ServiceXName'], "type")
+    if backend_type == "xaod":
+        pair = ("xaod", "atlasr21")
+    elif backend_type == "uproot":
+        pair = ("uproot", "uproot")
+
+    """ from General block """
+    if 'Transformer' in config['General'].keys():
+        if config['General']['Transformer'] == "atlasr21":
+            pair = ("xaod", "atlasr21")
+        elif config['General']['Transformer'] == "uproot":
+            pair = ("uproot", "uproot")
+        elif config['General']['Transformer'] == "python":
+            pair = ("uproot", "python")
+
+    """ from Sample block """
+    for (idx, sample) in zip(range(len(config['Sample'])), config['Sample']):
+        if 'Transformer' in sample.keys():
+            if sample['Transformer'] == "atlasr21":
+                config['Sample'][idx]['Type'] = "xaod"
+            elif sample['Transformer'] == "uproot":
+                config['Sample'][idx]['Type'] = "uproot"
+            elif sample['Transformer'] == "python":
+                config['Sample'][idx]['Type'] = "uproot"
+        else:
+            config['Sample'][idx]['Type'] = pair[0]
+            config['Sample'][idx]['Transformer'] = pair[1]
+
+    return config
+
+
+def _decorate_defaults(config: Dict[str, Any]) -> Dict:
+    if 'Delivery' in config['General'].keys():
+        config['General']['Delivery'] = config['General']['Delivery'].lower()
+    else:
+        config['General']['Delivery'] = 'localpath'
+    return config
+
+
 def _validate_config(config: Dict[str, Any]) -> bool:
     """Returns True if the config file is validated,
     otherwise raises exceptions.
     Checks that the config satisfies the json schema,
     and performs additional checks to
     validate the config further.
     Args:
@@ -67,20 +111,22 @@
         NotImplementedError
         ValueError
         KeyError
     Returns:
         bool: whether the validation was successful
     """
 
+    # Check Option names
     available_keys = [
         'General', 'ServiceXName', 'OutputDirectory', 'Transformer',
         'OutputFormat', 'WriteOutputDict', 'Name',
         'IgnoreLocalCache', 'Sample', 'RucioDID', 'XRootDFiles', 'Tree',
         'Filter', 'Columns', 'FuncADL', 'LocalPath', 'Definition',
-        'ServiceXBackendName', 'IgnoreServiceXCache'
+        'ServiceXBackendName', 'IgnoreServiceXCache',
+        'Delivery', 'Function'
         ]
 
     if 'General' not in config.keys() and 'Sample' not in config.keys():
         raise KeyError("You should have 'General' block and "
                        "at least one 'Sample' block in the config")
 
     keys_in_config = set()
@@ -90,24 +136,27 @@
     for sample in config['Sample']:
         for item in sample.keys():
             keys_in_config.add(item)
     for key in keys_in_config:
         if key not in available_keys:
             raise KeyError(f"Unknown Option {key} in the config")
 
+    # Check General block option values
+    if 'Delivery' in config['General'].keys():
+        if config['General']['Delivery'] not in [
+                'localpath', 'localcache', 'objectstore']:
+            raise ValueError(
+                f"Unsupported delivery option: {config['General']['Delivery']}"
+                f" - supported options: LocalPath, LocalCache, ObjectStore"
+                )
+
     if ('ServiceXName' not in config['General'].keys()) and \
             ('ServiceXBackendName' not in config['General'].keys()):
         raise KeyError("Option 'ServiceXName' is required in General block")
 
-    # if 'Transformer' not in config['General'].keys():
-    #     raise KeyError("Option 'Transformer' is required in General block")
-
-    # if 'OutputDirectory' not in config['General'].keys():
-    #     raise KeyError("OutputDirectory is required")
-
     if 'OutputFormat' not in config['General'].keys():
         raise KeyError("OutputFormat is required")
     elif config['General']['OutputFormat'].lower() != 'parquet' and \
             config['General']['OutputFormat'].lower() != 'root':
         raise ValueError("OutputFormat can be either parquet or root")
 
     for sample in config['Sample']:
@@ -140,41 +189,7 @@
             raise KeyError(
                 f"Sample {sample['Name']} - "
                 "You cannot use Filter with func-adl query"
                 )
 
     log.debug("config looks okay")
     return True
-
-
-def _update_backend_per_sample(config: Dict[str, Any]) -> Dict:
-    """ from servicex.yaml file """
-    backend_type = servicex_config.ServiceXConfigAdaptor()\
-        .get_backend_info(config['General']['ServiceXName'], "type")
-    if backend_type == "xaod":
-        pair = ("xaod", "atlasr21")
-    elif backend_type == "uproot":
-        pair = ("uproot", "uproot")
-
-    """ from General block """
-    if 'Transformer' in config['General'].keys():
-        if config['General']['Transformer'] == "atlasr21":
-            pair = ("xaod", "atlasr21")
-        elif config['General']['Transformer'] == "uproot":
-            pair = ("uproot", "uproot")
-        elif config['General']['Transformer'] == "python":
-            pair = ("uproot", "python")
-
-    """ from Sample block """
-    for (idx, sample) in zip(range(len(config['Sample'])), config['Sample']):
-        if 'Transformer' in sample.keys():
-            if sample['Transformer'] == "atlasr21":
-                config['Sample'][idx]['Type'] = "xaod"
-            elif sample['Transformer'] == "uproot":
-                config['Sample'][idx]['Type'] = "uproot"
-            elif sample['Transformer'] == "python":
-                config['Sample'][idx]['Type'] = "uproot"
-        else:
-            config['Sample'][idx]['Type'] = pair[0]
-            config['Sample'][idx]['Transformer'] = pair[1]
-
-    return config
```

### Comparing `servicex_databinder-0.4.1/servicex_databinder/old_frontend.py` & `servicex_databinder-0.5.0/servicex_databinder/old_frontend.py`

 * *Files identical despite different names*

### Comparing `servicex_databinder-0.4.1/servicex_databinder/old_output.py` & `servicex_databinder-0.5.0/servicex_databinder/old_output.py`

 * *Files identical despite different names*

### Comparing `servicex_databinder-0.4.1/servicex_databinder/request.py` & `servicex_databinder-0.5.0/servicex_databinder/request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Any, Dict, List
 import tcut_to_qastle as tq
 import qastle
 import ast
 import logging
+from base64 import b64encode
 from func_adl_servicex import ServiceXSourceXAOD # NOQA
 from servicex import ServiceXDataset # NOQA
 
 log = logging.getLogger(__name__)
 
 
 class ServiceXRequest():
@@ -33,19 +34,19 @@
         """
         Return a list containing ServiceX request(s) of the given sample
         """
         requests_sample = []
 
         if 'RucioDID' in sample.keys():
             dids = sample['RucioDID'].split(',')
-            if sample['Type'] == "uproot":
+            if sample['Transformer'] == "uproot":
                 trees = sample['Tree'].split(',')
                 log.debug(f"  Sample {sample['Name']} has "
                           f"{len(dids)} DID(s) and {len(trees)} Tree(s)")
-            elif sample['Type'] == "xaod":
+            else:
                 trees = ['dummy']
                 log.debug(f"  Sample {sample['Name']} has {len(dids)} DID(s)")
 
             for tree in trees:
                 for did in dids:
                     requests_sample.append(
                         {
@@ -56,20 +57,20 @@
                             'tree': tree.strip(),
                             'query': self._build_query(sample, tree.strip())
                         }
                     )
         elif 'XRootDFiles' in sample.keys():
             xrootd_filelist = [file.strip()
                                for file in sample['XRootDFiles'].split(",")]
-            if sample['Type'] == "uproot":
+            if sample['Transformer'] == "uproot":
                 trees = sample['Tree'].split(',')
                 log.debug(f"  Sample {sample['Name']} has "
                           f"{len(xrootd_filelist)} file(s) and "
                           f"{len(trees)} Tree(s)")
-            elif sample['Type'] == "xaod":
+            else:
                 trees = ['dummy']
                 log.debug(f"  Sample {sample['Name']} has "
                           f"{len(xrootd_filelist)} file(s)")
             for tree in trees:
                 requests_sample.append(
                     {
                         'Sample': sample['Name'],
@@ -126,7 +127,10 @@
                 qastle_query = qastle.python_ast_to_text_ast(o._q_ast)
                 return qastle_query
             except Exception:
                 log.exception(
                     "Exception occured for the query "
                     f"of Sample {sample['Name']}"
                     )
+        elif sample['Transformer'] == "python":
+            query = sample['Function']
+            return b64encode(query.encode("utf-8")).decode("utf-8")
```

### Comparing `servicex_databinder-0.4.1/servicex_databinder/servicex_databinder.py` & `servicex_databinder-0.5.0/servicex_databinder/servicex_databinder.py`

 * *Files identical despite different names*

### Comparing `servicex_databinder-0.4.1/servicex_databinder.egg-info/PKG-INFO` & `servicex_databinder-0.5.0/servicex_databinder.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: servicex-databinder
-Version: 0.4.1
+Version: 0.5.0
 Summary: ServiceX data management                     using a configuration file
 Home-page: https://github.com/kyungeonchoi/ServiceXDataBinder
 Author: KyungEon Choi (UT Austin)
 Author-email: kyungeonchoi@utexas.edu
 License: BSD 3-clause
 Platform: Any
 Classifier: Development Status :: 3 - Alpha
@@ -17,29 +17,29 @@
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ServiceX DataBinder
 
-<p align="right"> Release v0.4.1 </p>
+<p align="right"> Release v0.5.0 </p>
 
 [![PyPI version](https://badge.fury.io/py/servicex-databinder.svg)](https://badge.fury.io/py/servicex-databinder)
 
 `servicex-databinder` is a user-analysis data management package using a single configuration file. 
 Samples with external data sources (e.g. `RucioDID` or `XRootDFiles`) utilize ServiceX to deliver user-selected columns with optional row filtering.
 <!-- to interact with ServiceX instance to make ServiceX request(s) and manage ServiceX delivered data from a single configuration file. -->
 
 The following table shows supported ServiceX transformers by DataBinder
 
 | Input format | Code generator | Transformer | Output format
 | :--- | :---: | :---: | :---: |
 | ROOT Ntuple | func-adl | `uproot` | `root` or `parquet` |
 | ATLAS Release 21 xAOD | func-adl | `atlasr21`| `root` |
-<!-- | ROOT Ntuple | python function | `python`| -->
+| ROOT Ntuple | python function | `python`| `root` or `parquet` |
 
 <!-- [`ServiceX`](https://github.com/ssl-hep/ServiceX) is a scalable HEP event data extraction, transformation and delivery system. 
 
 ['ServiceX Client library'](https://github.com/ssl-hep/ServiceX_frontend) provides  --> 
 
 ## Prerequisite
 - [Access to a ServiceX instance](https://servicex.readthedocs.io/en/latest/user/getting-started/)
@@ -82,31 +82,34 @@
 Output format can be either `Apache parquet` or `ROOT ntuple` for `uproot` backend. Only `ROOT ntuple` format is supported for `xAOD` backend.
 
 
 The followings are available options:
 
 <!-- `General` block: -->
 | Option for `General` block | Description       | DataType |
-|:--------:|:------:|:------|
+|:--------:|:------|:------|
 | `ServiceXName`* | ServiceX backend name in your `servicex.yaml` file <br>  | `String` |
-| `OutputDirectory` | Path to the directory for ServiceX delivered files | `String` |
 | `OutputFormat`* | Output file format of ServiceX delivered data (`parquet` or `root` for `uproot` / `root` for `xaod`) | `String` |
+| `Transformer` | Set transformer for all Samples. Overwrites the default transformer in the `servicex.yaml` file.  | `String`|
+| `Delivery` | Delivery option; `LocalPath` (default) or `LocalCache` or `ObjectStore` | `String` |
+| `OutputDirectory` | Path to a directory for ServiceX delivered files | `String` |
 | `WriteOutputDict` | Name of an ouput yaml file containing Python nested dictionary of output file paths (located in the `OutputDirectory`) | `String` |
 | `IgnoreServiceXCache` | Ignore the existing ServiceX cache and force to make ServiceX requests | `Boolean` |
 <p align="right"> *Mandatory options</p>
 
 | Option for `Sample` block | Description       |DataType |
-|:--------:|:------:|:------|
-| `Name`   | sample name defined by a user |`String` |
+|:--------:|:------|:------|
+| `Name`   | Sample name defined by a user |`String` |
+| `Transformer` | Transformer for the given sample | `String`|
 | `RucioDID` | Rucio Dataset Id (DID) for a given sample; <br> Can be multiple DIDs separated by comma |`String` |
 | `XRootDFiles` | XRootD files (e.g. `root://`) for a given sample; <br> Can be multiple files separated by comma |`String` |
 | `Tree` | Name of the input ROOT `TTree`; <br> Can be multiple `TTree`s separated by comma (`uproot` ONLY) |`String` |
 | `Filter` | Selection in the TCut syntax, e.g. `jet_pt > 10e3 && jet_eta < 2.0` (TCut ONLY) |`String` |
 | `Columns` | List of columns (or branches) to be delivered; multiple columns separately by comma (TCut ONLY) |`String` |
-| `FuncADL` | func-adl expression for a given sample |`String` |
+| `FuncADL` | Func-adl expression for a given sample |`String` |
 | `LocalPath` | File path directly from local path (NO ServiceX tranformation) | `String` |
 
  <!-- Options exclusively for TCut syntax (CANNOT combine with the option `FuncADL`) -->
 
  <!-- Option for func-adl expression (CANNOT combine with the option `Fitler` and `Columns`) -->
 
 A config file can be simplified by utilizing `Definition` block. You can define placeholders under `Definition` block, which will replace all matched placeholders in the values of `Sample` block. Note that placeholders must start with `DEF_`.
@@ -139,14 +142,23 @@
     Columns: lep_pt, lep_eta
   - Name: Background2
     Transformer: atlasr21
     RucioDID: DEF_Zee_input
     FuncADL: DEF_Zee_query
   - Name: Background3
     LocalPath: /Users/kchoi/Work/data/background3
+  - Name: Background4
+    Transformer: python
+    RucioDID: user.kchoi:user.kchoi.background4
+    Function: |
+      def run_query(input_filenames=None):
+          import awkward as ak, uproot
+          tree_name = "nominal"
+          o = uproot.lazy({input_filenames:tree_name})
+          return {"nominal: o}
 
 Definition:
   DEF_ttH_nominal_query: "Where(lambda e: e.met_met>150e3). \
               Select(lambda event: {'el_pt': event.el_pt, 'jet_e': event.jet_e, \
               'jet_pt': event.jet_pt, 'met_met': event.met_met})"
   DEF_ggH_input: "root://eospublic.cern.ch//eos/opendata/atlas/OutreachDatasets\
                   /2020-01-22/4lep/MC/mc_345060.ggH125_ZZ4lep.4lep.root"
```

### Comparing `servicex_databinder-0.4.1/servicex_databinder.egg-info/SOURCES.txt` & `servicex_databinder-0.5.0/servicex_databinder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `servicex_databinder-0.4.1/setup.py` & `servicex_databinder-0.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `servicex_databinder-0.4.1/tests/test_config.py` & `servicex_databinder-0.5.0/tests/test_config.py`

 * *Files identical despite different names*

