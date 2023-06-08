# Comparing `tmp/specctl-0.1.4.tar.gz` & `tmp/specctl-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "specctl-0.1.4.tar", max compression
+gzip compressed data, was "specctl-0.1.5.tar", max compression
```

## Comparing `specctl-0.1.4.tar` & `specctl-0.1.5.tar`

### file list

```diff
@@ -1,21 +1,24 @@
--rw-r--r--   0        0        0    10142 2023-05-09 01:54:35.901782 specctl-0.1.4/LICENSE
--rw-r--r--   0        0        0    12312 2023-05-22 06:31:33.527898 specctl-0.1.4/README.md
--rw-r--r--   0        0        0      441 2023-05-23 02:47:42.253843 specctl-0.1.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-19 00:47:05.045382 specctl-0.1.4/specctl/__init__.py
--rw-r--r--   0        0        0     1936 2023-05-22 06:31:33.528528 specctl-0.1.4/specctl/ecs2k8s/README.md
--rw-r--r--   0        0        0        0 2023-05-19 00:47:05.064218 specctl-0.1.4/specctl/ecs2k8s/__init__.py
--rw-r--r--   0        0        0    11027 2023-05-23 02:47:25.078738 specctl-0.1.4/specctl/ecs2k8s/ecs_parser.py
--rw-r--r--   0        0        0    11874 2023-05-23 02:47:25.079390 specctl-0.1.4/specctl/ecs2k8s/ecs_reader_writer.py
--rw-r--r--   0        0        0     2351 2023-05-19 00:47:05.062861 specctl-0.1.4/specctl/ecs2k8s/k8s_objects.py
--rw-r--r--   0        0        0     4561 2023-05-22 06:31:33.529266 specctl-0.1.4/specctl/k8s2ecs/README.md
--rw-r--r--   0        0        0        0 2023-05-19 00:47:05.074140 specctl-0.1.4/specctl/k8s2ecs/__init__.py
--rw-r--r--   0        0        0     1628 2023-05-19 00:47:05.083773 specctl-0.1.4/specctl/k8s2ecs/ecs_objects.py
--rw-r--r--   0        0        0     5176 2023-05-23 00:31:18.914322 specctl-0.1.4/specctl/k8s2ecs/ecs_output.py
--rw-r--r--   0        0        0    12229 2023-05-23 00:31:18.915252 specctl-0.1.4/specctl/k8s2ecs/ingress.py
--rw-r--r--   0        0        0    27795 2023-05-19 00:47:05.090036 specctl-0.1.4/specctl/k8s2ecs/k8s_parser.py
--rw-r--r--   0        0        0     6465 2023-05-19 00:47:05.088657 specctl-0.1.4/specctl/k8s2ecs/k8s_reader.py
--rw-r--r--   0        0        0     5453 2023-05-19 00:47:05.072663 specctl-0.1.4/specctl/k8s2ecs/tf_output.py
--rw-r--r--   0        0        0     1873 2023-05-19 00:47:05.092119 specctl-0.1.4/specctl/quantity.py
--rw-r--r--   0        0        0     5377 2023-05-19 00:47:05.091443 specctl-0.1.4/specctl/specctl.py
--rw-r--r--   0        0        0     1757 2023-05-19 00:47:05.071056 specctl-0.1.4/specctl/utils.py
--rw-r--r--   0        0        0    13063 1970-01-01 00:00:00.000000 specctl-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    10142 2023-05-09 01:54:35.901782 specctl-0.1.5/LICENSE
+-rw-r--r--   0        0        0    12312 2023-05-22 06:31:33.527898 specctl-0.1.5/README.md
+-rw-r--r--   0        0        0      441 2023-06-08 22:55:57.339166 specctl-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-19 00:47:05.045382 specctl-0.1.5/specctl/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 22:55:57.339424 specctl-0.1.5/specctl/dc2k8s/__init__.py
+-rw-r--r--   0        0        0     4222 2023-06-08 22:55:57.341004 specctl-0.1.5/specctl/dc2k8s/dc_parser.py
+-rw-r--r--   0        0        0     1242 2023-06-08 22:55:57.342585 specctl-0.1.5/specctl/dc2k8s/dc_reader_writer.py
+-rw-r--r--   0        0        0     1936 2023-05-22 06:31:33.528528 specctl-0.1.5/specctl/ecs2k8s/README.md
+-rw-r--r--   0        0        0        0 2023-05-19 00:47:05.064218 specctl-0.1.5/specctl/ecs2k8s/__init__.py
+-rw-r--r--   0        0        0    11028 2023-06-08 22:55:57.343929 specctl-0.1.5/specctl/ecs2k8s/ecs_parser.py
+-rw-r--r--   0        0        0    11852 2023-06-08 22:55:57.345110 specctl-0.1.5/specctl/ecs2k8s/ecs_reader_writer.py
+-rw-r--r--   0        0        0     4561 2023-05-22 06:31:33.529266 specctl-0.1.5/specctl/k8s2ecs/README.md
+-rw-r--r--   0        0        0        0 2023-05-19 00:47:05.074140 specctl-0.1.5/specctl/k8s2ecs/__init__.py
+-rw-r--r--   0        0        0     1628 2023-05-19 00:47:05.083773 specctl-0.1.5/specctl/k8s2ecs/ecs_objects.py
+-rw-r--r--   0        0        0     5176 2023-05-23 00:31:18.914322 specctl-0.1.5/specctl/k8s2ecs/ecs_output.py
+-rw-r--r--   0        0        0    12229 2023-05-23 00:31:18.915252 specctl-0.1.5/specctl/k8s2ecs/ingress.py
+-rw-r--r--   0        0        0    27795 2023-05-19 00:47:05.090036 specctl-0.1.5/specctl/k8s2ecs/k8s_parser.py
+-rw-r--r--   0        0        0     5760 2023-06-08 22:55:57.347252 specctl-0.1.5/specctl/k8s2ecs/k8s_reader.py
+-rw-r--r--   0        0        0     5453 2023-05-19 00:47:05.072663 specctl-0.1.5/specctl/k8s2ecs/tf_output.py
+-rw-r--r--   0        0        0     2743 2023-06-08 22:55:57.347964 specctl-0.1.5/specctl/k8s_objects.py
+-rw-r--r--   0        0        0     2347 2023-06-08 22:55:57.350107 specctl-0.1.5/specctl/quantity.py
+-rw-r--r--   0        0        0     6283 2023-06-08 22:55:57.351701 specctl-0.1.5/specctl/specctl.py
+-rw-r--r--   0        0        0     1729 2023-06-08 22:55:57.353818 specctl-0.1.5/specctl/utils.py
+-rw-r--r--   0        0        0    13063 1970-01-01 00:00:00.000000 specctl-0.1.5/PKG-INFO
```

### Comparing `specctl-0.1.4/LICENSE` & `specctl-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `specctl-0.1.4/README.md` & `specctl-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `specctl-0.1.4/specctl/ecs2k8s/README.md` & `specctl-0.1.5/specctl/ecs2k8s/README.md`

 * *Files identical despite different names*

### Comparing `specctl-0.1.4/specctl/ecs2k8s/ecs_parser.py` & `specctl-0.1.5/specctl/ecs2k8s/ecs_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # // Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
 # // SPDX-License-Identifier: Apache-2.0
-from . import k8s_objects
+from .. import k8s_objects
 import json
 import copy
 import re
 from ..utils import dict_check
 import logging
 
 logger = logging.getLogger(__name__)
```

### Comparing `specctl-0.1.4/specctl/ecs2k8s/ecs_reader_writer.py` & `specctl-0.1.5/specctl/ecs2k8s/ecs_reader_writer.py`

 * *Files 0% similar despite different names*

```diff
@@ -277,14 +277,12 @@
                 write_yaml(k8s_file, v)
 
             if len(svc_namespace) > 0:
                 k8s_ns = namespace_parser(svc_namespace)
                 for k,v in k8s_ns.items():
                     k8s_file = os.path.join(output_dir, k+".yaml")
                     write_yaml(k8s_file, [v])
-                
-                
-
+            
     logger.log(100, "Please see %s directory for kubernetes artifacts" %(options.get("output_directory")))
```

### Comparing `specctl-0.1.4/specctl/ecs2k8s/k8s_objects.py` & `specctl-0.1.5/specctl/k8s_objects.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,38 @@
     },
     "spec": {
         "selector": {},
         "type":"ClusterIP",
         "ports":[]
     }
 }
+
+K8S_DAEMONSET = {
+    "apiVersion":"apps/v1",
+    "kind":"DaemonSet",
+    "metadata": {
+        "name": "",
+        "labels":{}
+    },
+    "spec":{ 
+        "selector": {
+            "matchLabels": {}
+        },
+        "template" : {
+            "metadata": {
+                "labels":{}
+            },
+            "spec":{
+                "containers":[]
+            }
+        }
+    }
+
+}
+
 K8S_DEPLOYMENT = {
     "apiVersion": "apps/v1",
     "kind": "Deployment",
     "metadata": {
         "name": ""
     },
     "spec": {
```

### Comparing `specctl-0.1.4/specctl/k8s2ecs/README.md` & `specctl-0.1.5/specctl/k8s2ecs/README.md`

 * *Files identical despite different names*

### Comparing `specctl-0.1.4/specctl/k8s2ecs/ecs_objects.py` & `specctl-0.1.5/specctl/k8s2ecs/ecs_objects.py`

 * *Files identical despite different names*

### Comparing `specctl-0.1.4/specctl/k8s2ecs/ecs_output.py` & `specctl-0.1.5/specctl/k8s2ecs/ecs_output.py`

 * *Files identical despite different names*

### Comparing `specctl-0.1.4/specctl/k8s2ecs/ingress.py` & `specctl-0.1.5/specctl/k8s2ecs/ingress.py`

 * *Files identical despite different names*

### Comparing `specctl-0.1.4/specctl/k8s2ecs/k8s_parser.py` & `specctl-0.1.5/specctl/k8s2ecs/k8s_parser.py`

 * *Files identical despite different names*

### Comparing `specctl-0.1.4/specctl/k8s2ecs/k8s_reader.py` & `specctl-0.1.5/specctl/k8s2ecs/k8s_reader.py`

 * *Files 11% similar despite different names*

```diff
@@ -124,25 +124,8 @@
         logger.info("%s namespace has %d pod security group objects"%(ns,len(sgp_objects["items"])))
         for sgp in sgp_objects["items"]:
             annt = sgp["metadata"]["annotations"]
             if annt is not None:
                 last_cfg = annt.get("kubectl.kubernetes.io/last-applied-configuration")
                 if last_cfg is not None:
                     security_groups.append(json.loads(last_cfg))
-    return(services+deployments+secrets+configmaps+ingress+service_accounts+security_groups)
-
-
-# This function will parse the K8s yaml files. It will convert the YAML to dictionary objects
-def k8s_yaml_to_dict(yaml_files):
-    dict_list = []
-    # read all the K8s spec YAML files as dictionaries
-    for yf in yaml_files:
-        logger.info("Reading YAML from %s file"%(yf))
-        with open(yf, 'r') as input_stream:
-            try:
-                for schema in yaml.safe_load_all(input_stream):
-                    dict_list.append(schema)
-            except:
-                logger.error("Error reading %s YAML file %s"%(yf, yaml.YAMLError))
-    # this will be the output dictionary which will have
-    # list of deployments, services, pods, secrets, and configmaps
-    return (dict_list)
+    return(services+deployments+secrets+configmaps+ingress+service_accounts+security_groups)
```

### Comparing `specctl-0.1.4/specctl/k8s2ecs/tf_output.py` & `specctl-0.1.5/specctl/k8s2ecs/tf_output.py`

 * *Files identical despite different names*

### Comparing `specctl-0.1.4/specctl/specctl.py` & `specctl-0.1.5/specctl/specctl.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 # // Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
 # // SPDX-License-Identifier: Apache-2.0
 import click
 import json
+import yaml 
 from os import listdir, makedirs
 from os.path import isdir, isfile, join
 
 # ecs to k8s 
 from .ecs2k8s.ecs_reader_writer import ecs_reader_writer
 
 # k8s to ecs
-from .k8s2ecs.k8s_reader import k8s_yaml_to_dict, k8s_cluster_extract
+from .k8s2ecs.k8s_reader import k8s_cluster_extract
 from .k8s2ecs.k8s_parser import k8s_parser
 from .k8s2ecs.ecs_output import ecs_print
 from .k8s2ecs.tf_output import terraform_print
 
+# docker compose to k8s
+from .dc2k8s.dc_reader_writer import dc_reader_writer
+
 import logging
 import logging.config
 LOGGING_CONFIG = { 
     'version': 1,
     'disable_existing_loggers': False,
     'formatters': { 
         'standard': { 
@@ -39,41 +43,64 @@
             'propagate': False
         }
     } 
 }
 logging.config.dictConfig(LOGGING_CONFIG)
 logger = logging.getLogger()
 
-def e2k_cli_hanlder(options):
+# reads yaml file(s) from source and returns dictionary list
+def yaml_reader(source):
+    yaml_files = []
+    dict_list = []
+    if isfile(source) and source.lower().endswith(('.yaml','yml')): yaml_files.append(source)
+    if isdir(source):
+        yaml_files = [join(source,f) for f in listdir(source) if isfile(join(source, f)) and f.lower().endswith(('.yaml','yml'))]   
+   
+    for yf in yaml_files:
+        logger.info("Reading YAML from %s file"%(yf))
+        with open(yf, 'r') as input_stream:
+            try:
+                for schema in yaml.safe_load_all(input_stream):
+                    dict_list.append(schema)
+            except:
+                logger.error("Error reading %s YAML file %s"%(yf, yaml.YAMLError))
+    return (dict_list)
+
+def e2k_cli_handler(options):
     ecs_reader_writer(options)
     return
 
 def k2e_cli_handler(source, context, options):
     spec_list = []
     if len(source)<=0:
         spec_list=k8s_cluster_extract(options.get("namespaces"), context)    
     else:
-        yaml_files = []
-        if isfile(source) and source.lower().endswith(('.yaml','yml')): yaml_files.append(source)
-        if isdir(source):
-            yaml_files = [join(source,f) for f in listdir(source) if isfile(join(source, f)) and f.lower().endswith(('.yaml','yml'))]
-        spec_list=k8s_yaml_to_dict(yaml_files)
+        spec_list=yaml_reader(source)
     
     if len(spec_list) <= 0:
         logger.warning("Found no K8s specification object")
         return
     output_dict=k8s_parser(spec_list)
     ecs_print(output_dict, options)
     terraform_print(output_dict, options)
     return
 
+def d2k_cli_handler(source, options):
+    spec_list=yaml_reader(source)
+    if len(spec_list) <= 0:
+        logger.warning("Found no docker compose specification object")
+        return
+    dc_reader_writer(spec_list, options)
+    return 
+
+
 # Click cli entry point function
 @click.command()
-@click.option("-m","--mode", default="k2e", type=click.Choice(["k2e","e2k"], case_sensitive=False), help="Transform mode - k2e K8s-to-ECS, e2k ECS-to-K8s")
-@click.option("-s", "--source", default="", type=str, help="Path to k8s spec file or dir")
+@click.option("-m","--mode", default="k2e", type=click.Choice(["k2e","e2k","d2k"], case_sensitive=False), help="Transform mode - k2e K8s-to-ECS, e2k ECS-to-K8s, d2k Docker Compose-to-K8s")
+@click.option("-s", "--source", default="", type=str, help="Path to YAML specification file or directory")
 @click.option("-c", "--context", default="", type=str, help="Kubeconfig context name to load")
 @click.option("-l", "--log_level", default="WARNING", type=click.Choice(["DEBUG","INFO","WARNING","ERROR","CRITICAL"], case_sensitive=False), help="Select log level")
 @click.option("-n", "--namespaces", default="", type=str, help="Only fetch namespaces specified here as comma separated string. Applies only when converting from K8s clusters and not from spec files")
 @click.option("--td_file",default="taskdefinition.json", help="File to write ECS task definition json")
 @click.option("--sd_file",default="servicedefinition.json", help="File to write ECS service definition json")
 @click.option("--input_file", default="", help="File with additional input parameters for task, container, and/or services")
 @click.option("--tfvars_file", default="terraform.tfvars", help="File to write the Terraform tfvars")
@@ -109,12 +136,15 @@
         "region_name" : ecs_region_name,
         "sgp": sgp
         }
     if mode == "k2e":
         k2e_cli_handler(source, context, options)
         return
     if mode == "e2k":
-        e2k_cli_hanlder(options)
+        e2k_cli_handler(options)
+        return
+    if mode == "d2k":
+        d2k_cli_handler(source, options)
         return
     if mode == "e2f":
         logger.info("ECS EC2 to ECS FG is coming soon!")
         return
```

### Comparing `specctl-0.1.4/specctl/utils.py` & `specctl-0.1.5/specctl/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # // Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
 # // SPDX-License-Identifier: Apache-2.0
-from .quantity import parse_quantity
+from .quantity import parse_quantity 
 import math
 
 FARGATE_AVAILABLE_SKUS = {
     256   : {"min":1024, "max":2048,    "incr":1024},
     512   : {"min":1024, "max":4096,    "incr":1024},
     1024  : {"min":2048, "max":8192,    "incr":1024},
     2048  : {"min":4096, "max":16384,   "incr":1024},
@@ -46,17 +46,8 @@
                 fg_sku = {"cpu":c, "memory":m}
                 break
     return(fg_sku)
 
 # simple util functions
 def dict_check(dict):
     if dict is None or len(dict)==0: return False
-    return True
-
-
-
-            
-
-
-    
-
-    
+    return True
```

### Comparing `specctl-0.1.4/PKG-INFO` & `specctl-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specctl
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 License: Apache 2.0
 Author: Arvind Soni
 Author-email: arvindsoni@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

