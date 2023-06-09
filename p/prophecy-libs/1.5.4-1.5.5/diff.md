# Comparing `tmp/prophecy-libs-1.5.4.tar.gz` & `tmp/prophecy-libs-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prophecy-libs-1.5.4.tar", last modified: Mon May 29 13:41:08 2023, max compression
+gzip compressed data, was "prophecy-libs-1.5.5.tar", last modified: Fri Jun  9 08:12:53 2023, max compression
```

## Comparing `prophecy-libs-1.5.4.tar` & `prophecy-libs-1.5.5.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-05-29 13:41:08.862583 prophecy-libs-1.5.4/
--rw-r--r--   0 jenkins    (109) jenkins    (114)      313 2023-05-29 13:41:08.862583 prophecy-libs-1.5.4/PKG-INFO
--rw-r--r--   0 jenkins    (109) jenkins    (114)       22 2023-03-12 14:51:36.000000 prophecy-libs-1.5.4/README.md
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-05-29 13:41:08.858582 prophecy-libs-1.5.4/prophecy/
--rw-r--r--   0 jenkins    (109) jenkins    (114)        0 2023-03-12 14:51:36.000000 prophecy-libs-1.5.4/prophecy/__init__.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-05-29 13:41:08.858582 prophecy-libs-1.5.4/prophecy/config/
--rw-r--r--   0 jenkins    (109) jenkins    (114)       27 2023-03-12 14:51:36.000000 prophecy-libs-1.5.4/prophecy/config/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     2221 2023-03-12 14:51:36.000000 prophecy-libs-1.5.4/prophecy/config/config_base.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     4346 2023-05-25 10:51:46.000000 prophecy-libs-1.5.4/prophecy/config/utils.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-05-29 13:41:08.858582 prophecy-libs-1.5.4/prophecy/libs/
--rw-r--r--   0 jenkins    (109) jenkins    (114)       20 2023-03-12 14:51:36.000000 prophecy-libs-1.5.4/prophecy/libs/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     1500 2023-05-26 15:20:32.000000 prophecy-libs-1.5.4/prophecy/libs/utils.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-05-29 13:41:08.858582 prophecy-libs-1.5.4/prophecy/lookups/
--rw-r--r--   0 jenkins    (109) jenkins    (114)     3191 2023-03-12 14:51:36.000000 prophecy-libs-1.5.4/prophecy/lookups/LookupsBase.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)       27 2023-03-12 14:51:36.000000 prophecy-libs-1.5.4/prophecy/lookups/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     3118 2023-03-12 14:51:36.000000 prophecy-libs-1.5.4/prophecy/random_data_creator.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-05-29 13:41:08.858582 prophecy-libs-1.5.4/prophecy/streaming/
--rw-r--r--   0 jenkins    (109) jenkins    (114)        0 2023-03-12 14:51:36.000000 prophecy-libs-1.5.4/prophecy/streaming/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     5283 2023-03-12 14:51:36.000000 prophecy-libs-1.5.4/prophecy/streaming/delta_lake_utils.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-05-29 13:41:08.862583 prophecy-libs-1.5.4/prophecy/test/
--rw-r--r--   0 jenkins    (109) jenkins    (114)       30 2023-03-12 14:51:36.000000 prophecy-libs-1.5.4/prophecy/test/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     1165 2023-05-15 15:31:20.000000 prophecy-libs-1.5.4/prophecy/test/base_test_case.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     9189 2023-04-19 07:54:52.000000 prophecy-libs-1.5.4/prophecy/test/utils.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-05-29 13:41:08.862583 prophecy-libs-1.5.4/prophecy/transpiler/
--rw-r--r--   0 jenkins    (109) jenkins    (114)      147 2023-05-26 15:20:32.000000 prophecy-libs-1.5.4/prophecy/transpiler/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)      789 2023-05-29 13:41:07.000000 prophecy-libs-1.5.4/prophecy/transpiler/abi_base.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)    22828 2023-05-29 13:41:07.000000 prophecy-libs-1.5.4/prophecy/transpiler/abi_core_fcns.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     1585 2023-05-29 13:41:07.000000 prophecy-libs-1.5.4/prophecy/transpiler/abi_fcn_wrapper.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     6515 2023-05-29 13:41:07.000000 prophecy-libs-1.5.4/prophecy/transpiler/dataframe_fcns.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     6393 2023-05-29 13:41:07.000000 prophecy-libs-1.5.4/prophecy/transpiler/fixed_file_schema.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-05-29 13:41:08.862583 prophecy-libs-1.5.4/prophecy/udfs/
--rw-r--r--   0 jenkins    (109) jenkins    (114)       87 2023-03-12 14:51:36.000000 prophecy-libs-1.5.4/prophecy/udfs/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     2154 2023-03-12 14:51:36.000000 prophecy-libs-1.5.4/prophecy/udfs/rest_api_udf.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)      172 2023-03-12 14:51:36.000000 prophecy-libs-1.5.4/prophecy/udfs/sample_udf.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)      988 2023-05-26 15:20:32.000000 prophecy-libs-1.5.4/prophecy/udfs/scala_udf_wrapper.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)    16532 2023-05-26 15:20:32.000000 prophecy-libs-1.5.4/prophecy/utils.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-05-29 13:41:08.862583 prophecy-libs-1.5.4/prophecy_libs.egg-info/
--rw-r--r--   0 jenkins    (109) jenkins    (114)      313 2023-05-29 13:41:08.000000 prophecy-libs-1.5.4/prophecy_libs.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (109) jenkins    (114)      992 2023-05-29 13:41:08.000000 prophecy-libs-1.5.4/prophecy_libs.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (109) jenkins    (114)        1 2023-05-29 13:41:08.000000 prophecy-libs-1.5.4/prophecy_libs.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (109) jenkins    (114)        1 2023-03-12 14:51:37.000000 prophecy-libs-1.5.4/prophecy_libs.egg-info/not-zip-safe
--rw-r--r--   0 jenkins    (109) jenkins    (114)       33 2023-05-29 13:41:08.000000 prophecy-libs-1.5.4/prophecy_libs.egg-info/requires.txt
--rw-r--r--   0 jenkins    (109) jenkins    (114)        9 2023-05-29 13:41:08.000000 prophecy-libs-1.5.4/prophecy_libs.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (109) jenkins    (114)       38 2023-05-29 13:41:08.862583 prophecy-libs-1.5.4/setup.cfg
--rw-r--r--   0 jenkins    (109) jenkins    (114)      474 2023-05-29 13:41:07.000000 prophecy-libs-1.5.4/setup.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-06-09 08:12:53.138308 prophecy-libs-1.5.5/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      313 2023-06-09 08:12:53.138308 prophecy-libs-1.5.5/PKG-INFO
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       22 2023-03-12 14:51:36.000000 prophecy-libs-1.5.5/README.md
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-06-09 08:12:53.130308 prophecy-libs-1.5.5/prophecy/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)        0 2023-03-12 14:51:36.000000 prophecy-libs-1.5.5/prophecy/__init__.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-06-09 08:12:53.130308 prophecy-libs-1.5.5/prophecy/config/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       27 2023-03-12 14:51:36.000000 prophecy-libs-1.5.5/prophecy/config/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     2221 2023-03-12 14:51:36.000000 prophecy-libs-1.5.5/prophecy/config/config_base.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     4442 2023-06-09 08:12:50.000000 prophecy-libs-1.5.5/prophecy/config/utils.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-06-09 08:12:53.130308 prophecy-libs-1.5.5/prophecy/libs/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       20 2023-03-12 14:51:36.000000 prophecy-libs-1.5.5/prophecy/libs/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     1500 2023-05-26 15:20:32.000000 prophecy-libs-1.5.5/prophecy/libs/utils.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-06-09 08:12:53.134308 prophecy-libs-1.5.5/prophecy/lookups/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     3191 2023-03-12 14:51:36.000000 prophecy-libs-1.5.5/prophecy/lookups/LookupsBase.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       27 2023-03-12 14:51:36.000000 prophecy-libs-1.5.5/prophecy/lookups/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     3118 2023-03-12 14:51:36.000000 prophecy-libs-1.5.5/prophecy/random_data_creator.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-06-09 08:12:53.134308 prophecy-libs-1.5.5/prophecy/streaming/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)        0 2023-03-12 14:51:36.000000 prophecy-libs-1.5.5/prophecy/streaming/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     5283 2023-03-12 14:51:36.000000 prophecy-libs-1.5.5/prophecy/streaming/delta_lake_utils.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-06-09 08:12:53.134308 prophecy-libs-1.5.5/prophecy/test/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       30 2023-03-12 14:51:36.000000 prophecy-libs-1.5.5/prophecy/test/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     1165 2023-05-15 15:31:20.000000 prophecy-libs-1.5.5/prophecy/test/base_test_case.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     9189 2023-04-19 07:54:52.000000 prophecy-libs-1.5.5/prophecy/test/utils.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-06-09 08:12:53.134308 prophecy-libs-1.5.5/prophecy/transpiler/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      147 2023-05-26 15:20:32.000000 prophecy-libs-1.5.5/prophecy/transpiler/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      789 2023-05-29 13:41:07.000000 prophecy-libs-1.5.5/prophecy/transpiler/abi_base.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)    22828 2023-05-29 13:41:07.000000 prophecy-libs-1.5.5/prophecy/transpiler/abi_core_fcns.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     1585 2023-05-29 13:41:07.000000 prophecy-libs-1.5.5/prophecy/transpiler/abi_fcn_wrapper.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     6515 2023-05-29 13:41:07.000000 prophecy-libs-1.5.5/prophecy/transpiler/dataframe_fcns.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     6393 2023-05-29 13:41:07.000000 prophecy-libs-1.5.5/prophecy/transpiler/fixed_file_schema.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-06-09 08:12:53.138308 prophecy-libs-1.5.5/prophecy/udfs/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       87 2023-03-12 14:51:36.000000 prophecy-libs-1.5.5/prophecy/udfs/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     2154 2023-03-12 14:51:36.000000 prophecy-libs-1.5.5/prophecy/udfs/rest_api_udf.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      172 2023-03-12 14:51:36.000000 prophecy-libs-1.5.5/prophecy/udfs/sample_udf.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      988 2023-05-26 15:20:32.000000 prophecy-libs-1.5.5/prophecy/udfs/scala_udf_wrapper.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)    16532 2023-05-26 15:20:32.000000 prophecy-libs-1.5.5/prophecy/utils.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-06-09 08:12:53.138308 prophecy-libs-1.5.5/prophecy_libs.egg-info/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      313 2023-06-09 08:12:52.000000 prophecy-libs-1.5.5/prophecy_libs.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      992 2023-06-09 08:12:53.000000 prophecy-libs-1.5.5/prophecy_libs.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (109) jenkins    (114)        1 2023-06-09 08:12:52.000000 prophecy-libs-1.5.5/prophecy_libs.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (109) jenkins    (114)        1 2023-03-12 14:51:37.000000 prophecy-libs-1.5.5/prophecy_libs.egg-info/not-zip-safe
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       33 2023-06-09 08:12:52.000000 prophecy-libs-1.5.5/prophecy_libs.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (109) jenkins    (114)        9 2023-06-09 08:12:52.000000 prophecy-libs-1.5.5/prophecy_libs.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       38 2023-06-09 08:12:53.138308 prophecy-libs-1.5.5/setup.cfg
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      474 2023-06-09 08:12:50.000000 prophecy-libs-1.5.5/setup.py
```

### Comparing `prophecy-libs-1.5.4/prophecy/config/config_base.py` & `prophecy-libs-1.5.5/prophecy/config/config_base.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.4/prophecy/config/utils.py` & `prophecy-libs-1.5.5/prophecy/config/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -38,53 +38,54 @@
         help="Overridden values in json format"
     )
     args = parser.parse_args()
 
     return args
 
 
-def get_resource_file_content(resource_file_name):
+def get_resource_file_content(resource_file_name, config_package):
     try:
         # python 3.7+
         import importlib.resources
-        with importlib.resources.open_text("prophecy_config_instances", f"{resource_file_name}") as file:
+        with importlib.resources.open_text(config_package, f"{resource_file_name}") as file:
             data = file.read()
     except:
         # python < 3.7
         import importlib.util
-        config_instances_path = importlib.util.find_spec("prophecy_config_instances").submodule_search_locations[0]
+        config_instances_path = importlib.util.find_spec(config_package).submodule_search_locations[0]
         config_file_path = f"{config_instances_path}/{resource_file_name}"
         with open(config_file_path, 'r') as file:
             data = file.read()
     return data
 
 
 # 1 arg parse_config() for backward compatibility.
-def parse_config(args, pipeline_dot_conf=None):
+def parse_config(args, pipeline_dot_conf=None, config_package=None):
+    config_package = "prophecy_config_instances" if config_package is None else config_package
     if args.file is not None:
         if hasattr(args, "defaultConfFile"):
             default_config = ConfigFactory.parse_file(
                 args.defaultConfFile) if args.defaultConfFile is not None else ConfigFactory.parse_string("{}")
             conf = ConfigFactory.parse_file(args.file).with_fallback(default_config)
         else:
             conf = ConfigFactory.parse_file(args.file)
     elif args.confInstance is not None:
         try:
             # python 3.7+
             import importlib.resources
             with importlib.resources.open_text(
-                    "prophecy_config_instances",
+                    config_package,
                     "{instance}.json".format(instance=args.confInstance),
             ) as file:
                 data = file.read()
                 conf = ConfigFactory.parse_string(data)
         except:
             # python < 3.7
             import importlib.util
-            config_instances_path = importlib.util.find_spec("prophecy_config_instances").submodule_search_locations[0]
+            config_instances_path = importlib.util.find_spec(config_package).submodule_search_locations[0]
             config_file_path = f"{config_instances_path}/{args.confInstance}.json"
             with open(config_file_path, 'r') as file:
                 data = file.read()
                 conf = ConfigFactory.parse_string(data)
     else:
         conf = ConfigFactory.parse_string("{}")
 
@@ -97,15 +98,15 @@
             c = config.split("=", 1)
             conf.put(c[0], c[1])
 
     if pipeline_dot_conf is not None:
         # `resolve=False` is important here because variable substitution should happen after overriding
         try:
             # Check in resources/
-            pipeline_default_conf = ConfigFactory.parse_string(get_resource_file_content(pipeline_dot_conf),
+            pipeline_default_conf = ConfigFactory.parse_string(get_resource_file_content(pipeline_dot_conf, config_package),
                                                                resolve=False)
         except:
             # Check as full file path
             pipeline_default_conf = ConfigFactory.parse_file(pipeline_dot_conf, resolve=False)
         # `resolve=True` so that variables get substituted at this step with overridden values
         # pipeline_dot_conf contains default values for a given pipeline. It should have the lowest priority,
         conf = conf.with_fallback(pipeline_default_conf, resolve=True)
```

### Comparing `prophecy-libs-1.5.4/prophecy/libs/utils.py` & `prophecy-libs-1.5.5/prophecy/libs/utils.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.4/prophecy/lookups/LookupsBase.py` & `prophecy-libs-1.5.5/prophecy/lookups/LookupsBase.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.4/prophecy/random_data_creator.py` & `prophecy-libs-1.5.5/prophecy/random_data_creator.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.4/prophecy/streaming/delta_lake_utils.py` & `prophecy-libs-1.5.5/prophecy/streaming/delta_lake_utils.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.4/prophecy/test/base_test_case.py` & `prophecy-libs-1.5.5/prophecy/test/base_test_case.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.4/prophecy/test/utils.py` & `prophecy-libs-1.5.5/prophecy/test/utils.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.4/prophecy/transpiler/abi_base.py` & `prophecy-libs-1.5.5/prophecy/transpiler/abi_base.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.4/prophecy/transpiler/abi_core_fcns.py` & `prophecy-libs-1.5.5/prophecy/transpiler/abi_core_fcns.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.4/prophecy/transpiler/abi_fcn_wrapper.py` & `prophecy-libs-1.5.5/prophecy/transpiler/abi_fcn_wrapper.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.4/prophecy/transpiler/dataframe_fcns.py` & `prophecy-libs-1.5.5/prophecy/transpiler/dataframe_fcns.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.4/prophecy/transpiler/fixed_file_schema.py` & `prophecy-libs-1.5.5/prophecy/transpiler/fixed_file_schema.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.4/prophecy/udfs/rest_api_udf.py` & `prophecy-libs-1.5.5/prophecy/udfs/rest_api_udf.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.4/prophecy/udfs/scala_udf_wrapper.py` & `prophecy-libs-1.5.5/prophecy/udfs/scala_udf_wrapper.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.4/prophecy/utils.py` & `prophecy-libs-1.5.5/prophecy/utils.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.4/prophecy_libs.egg-info/SOURCES.txt` & `prophecy-libs-1.5.5/prophecy_libs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

