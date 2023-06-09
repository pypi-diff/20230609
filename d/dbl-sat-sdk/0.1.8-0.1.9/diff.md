# Comparing `tmp/dbl_sat_sdk-0.1.8-py3-none-any.whl.zip` & `tmp/dbl_sat_sdk-0.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 20193 bytes, number of entries: 29
+Zip file size: 20162 bytes, number of entries: 29
 -rw-r--r--  2.0 unx        0 b- defN 22-Oct-07 03:48 clientpkgs/__init__.py
 -rw-r--r--  2.0 unx     2194 b- defN 22-Oct-20 03:11 clientpkgs/accounts_client.py
 -rw-r--r--  2.0 unx     5491 b- defN 22-Oct-20 03:15 clientpkgs/clusters_client.py
 -rw-r--r--  2.0 unx      375 b- defN 22-Oct-20 03:17 clientpkgs/db_sql_client.py
 -rw-r--r--  2.0 unx     1248 b- defN 22-Oct-20 03:11 clientpkgs/dbfs_client.py
 -rw-r--r--  2.0 unx      417 b- defN 22-Oct-20 03:15 clientpkgs/init_scripts_client.py
 -rw-r--r--  2.0 unx      407 b- defN 22-Oct-20 03:11 clientpkgs/ip_access_list.py
@@ -15,17 +15,17 @@
 -rw-r--r--  2.0 unx      355 b- defN 22-Oct-20 03:16 clientpkgs/repos_client.py
 -rw-r--r--  2.0 unx      496 b- defN 22-Oct-20 03:16 clientpkgs/scim_client.py
 -rw-r--r--  2.0 unx     1600 b- defN 22-Oct-20 03:11 clientpkgs/secrets_client.py
 -rw-r--r--  2.0 unx      382 b- defN 22-Oct-20 03:11 clientpkgs/tokens_client.py
 -rw-r--r--  2.0 unx     1402 b- defN 22-Oct-20 03:20 clientpkgs/workspace_client.py
 -rw-r--r--  2.0 unx     5101 b- defN 22-Oct-20 03:18 clientpkgs/ws_settings_client.py
 -rw-r--r--  2.0 unx        3 b- defN 22-Oct-07 03:48 core/__init__.py
--rw-r--r--  2.0 unx    11612 b- defN 22-Oct-21 03:08 core/dbclient.py
+-rw-r--r--  2.0 unx    12260 b- defN 22-Oct-21 03:49 core/dbclient.py
 -rw-r--r--  2.0 unx     1960 b- defN 22-Oct-19 04:35 core/logging_utils.py
--rw-r--r--  2.0 unx     3637 b- defN 22-Oct-21 03:27 core/parser.py
+-rw-r--r--  2.0 unx     2959 b- defN 22-Oct-21 03:49 core/parser.py
 -rw-r--r--  2.0 unx     1321 b- defN 22-Oct-07 03:48 core/wmconstants.py
--rw-r--r--  2.0 unx      735 b- defN 22-Oct-21 03:27 dbl_sat_sdk-0.1.8.dist-info/METADATA
--rw-r--r--  2.0 unx      320 b- defN 22-Oct-21 03:27 dbl_sat_sdk-0.1.8.dist-info/NOTICE
--rw-r--r--  2.0 unx       92 b- defN 22-Oct-21 03:27 dbl_sat_sdk-0.1.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 22-Oct-21 03:27 dbl_sat_sdk-0.1.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     2369 b- defN 22-Oct-21 03:27 dbl_sat_sdk-0.1.8.dist-info/RECORD
-29 files, 45707 bytes uncompressed, 16383 bytes compressed:  64.2%
+-rw-r--r--  2.0 unx      735 b- defN 22-Oct-21 03:49 dbl_sat_sdk-0.1.9.dist-info/METADATA
+-rw-r--r--  2.0 unx      320 b- defN 22-Oct-21 03:49 dbl_sat_sdk-0.1.9.dist-info/NOTICE
+-rw-r--r--  2.0 unx       92 b- defN 22-Oct-21 03:49 dbl_sat_sdk-0.1.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 22-Oct-21 03:49 dbl_sat_sdk-0.1.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     2369 b- defN 22-Oct-21 03:49 dbl_sat_sdk-0.1.9.dist-info/RECORD
+29 files, 45677 bytes uncompressed, 16352 bytes compressed:  64.2%
```

## zipnote {}

```diff
@@ -66,23 +66,23 @@
 
 Filename: core/parser.py
 Comment: 
 
 Filename: core/wmconstants.py
 Comment: 
 
-Filename: dbl_sat_sdk-0.1.8.dist-info/METADATA
+Filename: dbl_sat_sdk-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: dbl_sat_sdk-0.1.8.dist-info/NOTICE
+Filename: dbl_sat_sdk-0.1.9.dist-info/NOTICE
 Comment: 
 
-Filename: dbl_sat_sdk-0.1.8.dist-info/WHEEL
+Filename: dbl_sat_sdk-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: dbl_sat_sdk-0.1.8.dist-info/top_level.txt
+Filename: dbl_sat_sdk-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: dbl_sat_sdk-0.1.8.dist-info/RECORD
+Filename: dbl_sat_sdk-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## core/dbclient.py

```diff
@@ -1,13 +1,14 @@
 '''dbclient'''
 import json
 import base64
 import time
 import requests
 import urllib3
+import logging
 from core.logging_utils import LoggingUtils
 from core import parser as pars
 
 urllib3.disable_warnings(category = urllib3.exceptions.InsecureRequestWarning)
 
 
 global PPRINT_J
@@ -35,15 +36,16 @@
         configs = pars.parse_input_jsonargs(inp_configs)
         self._configs=configs
         self._workspace_id = configs['workspace_id']
         self._raw_url = configs['url'].strip()
         self._url=self._raw_url
         self._account_id = configs['account_id'].strip()
         self._cloud_type = self.parse_cloud_type()
-        self._verbosity = configs['verbosity']
+        self._verbosity = SatDBClient.get_log_level(inp_configs['verbosity'])
+        LoggingUtils.set_logger_level(self._verbosity)
         self._cluster_id=configs['clusterid'].strip()
         self._token = ''
         self._raw_token = configs['token'].strip()
         self._master_name = configs['mastername'].strip()
         self._master_password = configs['masterpwd'].strip()
 
     def _update_token_master(self):
@@ -275,14 +277,28 @@
             cloudtype='azure'
         if 'cloud.databricks' in self._raw_url:
             cloudtype='aws'
         if 'gcp.databricks' in self._raw_url:
             cloudtype='gcp'
         return cloudtype
 
+    #DEBUG < INFO < WARNING < ERROR < CRITICAL
+    # pylint: disable=multiple-statements
+    @staticmethod
+    def get_log_level( vloglevel):
+        '''get log level that is set'''
+        vloglevel=vloglevel.upper()
+        if vloglevel == "DEBUG": return logging.DEBUG
+        elif vloglevel == "INFO": return logging.INFO
+        elif vloglevel == "WARNING": return logging.WARNING
+        elif vloglevel == "ERROR": return logging.ERROR
+        elif vloglevel == "CRITICAL": return logging.CRITICAL
+    # pylint: enable=multiple-statements
+
+
     # @staticmethod
     # def listdir(f_path):
     #     ls = os.listdir(f_path)
     #     for x in ls:
     #         # remove hidden directories / files from function
     #         if x.startswith('.'):
     #             continue
```

## core/parser.py

```diff
@@ -10,15 +10,15 @@
     LOGGR = LoggingUtils.get_logger()
 
 def set_defaults(args):
     '''set defaults if not detected in incoming json'''
     if 'url' not in args.keys():
         args.update({'url':''})
     if 'verbosity' not in args.keys():
-        args.update({'verbosity':'false'})
+        args.update({'verbosity':'info'})
 
 
 def url_validation(url):
     '''validate url patterns'''
     # pylint: disable=anomalous-backslash-in-string
     if '/?o=' in url:
         # if the workspace_id exists, lets remove it from the URL
@@ -28,27 +28,14 @@
     elif 'com/' == url[-4:]:
         url = url[:-1]
     return url.rstrip("/")
     # pylint: enable=anomalous-backslash-in-string
 
 
 
-#DEBUG < INFO < WARNING < ERROR < CRITICAL
-# pylint: disable=multiple-statements
-def get_log_level(vloglevel):
-    '''get log level that is set'''
-    vloglevel=vloglevel.upper()
-    if vloglevel == "DEBUG": return logging.DEBUG
-    elif vloglevel == "INFO": return logging.INFO
-    elif vloglevel == "WARNING": return logging.WARNING
-    elif vloglevel == "ERROR": return logging.ERROR
-    elif vloglevel == "CRITICAL": return logging.CRITICAL
-# pylint: enable=multiple-statements
-
-
 def str2bool(vinput):
     '''convert string to bool'''
     return vinput.lower() in ("yes", "true", "t", "1")
 
 #dummy values. Not real values
 # {'account_id': 'dadbb045-e629-4e8c-b408-dc6b3ac3d4eb', 'export_db': 'logs', 'verify_ssl': 'False', 'verbosity': 'info', 
 # 'email_alerts': '', 'master_name_scope': 'sat_master_scope', 'master_name_key': 'user', 'master_pwd_scope': 'sat_master_scope', 
@@ -59,17 +46,14 @@
 def parse_input_jsonargs(inp_configs):
     '''parse and validate incoming json string and return json'''
     if isinstance(inp_configs, str):
         inp_configs =json.loads(inp_configs)
     set_defaults(inp_configs)
     url = url_validation(inp_configs['url'])
     inp_configs.update({'url':url})
-    print('-' + json.dumps(inp_configs))
-    inp_configs.update({'verbosity':get_log_level(inp_configs['verbosity'])})
-    LoggingUtils.loglevel=inp_configs['verbosity'] #update class variable
     ## validate values are present    
     if inp_configs['account_id'] == '':
         raise ValueError('Account ID cannot be empty')
     if inp_configs['clusterid'] == '':
         raise ValueError('Cluster ID cannot be empty')
     if inp_configs['mastername'] == '':
         raise ValueError('Master name cannot be empty')
```

## Comparing `dbl_sat_sdk-0.1.8.dist-info/METADATA` & `dbl_sat_sdk-0.1.9.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbl-sat-sdk
-Version: 0.1.8
+Version: 0.1.9
 Summary: Databricks Security Analysis Tool
 Home-page: https://databricks.com/learn/labs
 Author: Arun Pamulapati, Anindita Mahapatra, Ram Murali
 Author-email: labs@databricks.com
 License: https://github.com/databrickslabs/profile/blob/master/LICENSE
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
```

## Comparing `dbl_sat_sdk-0.1.8.dist-info/RECORD` & `dbl_sat_sdk-0.1.9.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 clientpkgs/repos_client.py,sha256=kML5fm_3Uct7YI81SpyVOaakFpSts63hTegutwFqa_8,355
 clientpkgs/scim_client.py,sha256=Vgi4f5cOmp57VKztXKj8T3BYanRtPH19AZePibRMNLY,496
 clientpkgs/secrets_client.py,sha256=onbCtpBd-5zoSukWevpOTPmd-dnOUrSFctmZt_o0HEA,1600
 clientpkgs/tokens_client.py,sha256=-zPVNntB8j01ZDbXeddvsV4Nppa33q_o8hgDhvl2xS8,382
 clientpkgs/workspace_client.py,sha256=BGKlqi-hB5lVY4-93K6Hr1Ovmus1qTdBqGvkALivc0s,1402
 clientpkgs/ws_settings_client.py,sha256=cmHbJVmu4DoRzF6lxQ4j0wq-KuCJffyxEG7aemeUp68,5101
 core/__init__.py,sha256=ajz1GSNU9xYVrFEDSz6Xwg7amWQ_yvW75tQa1ZvRIWc,3
-core/dbclient.py,sha256=twlYQ-sMZ8XB7LpcsURwdKviYi5ZCjI59xmobSRuvto,11612
+core/dbclient.py,sha256=zlcrWfrS3LOVrQmkM0KRAu1p7P4uv7GeLd-u_iioJ1w,12260
 core/logging_utils.py,sha256=AllgawGgYkhlzh5bvN3TfXLRBPkjKWo14q213pVGe2E,1960
-core/parser.py,sha256=1eXLWu5FyjLH27pm4RyxoN2JMY6_FENStIIRqkLRyYw,3637
+core/parser.py,sha256=_V9hRyi-qV1aBOy4SkHbG7Llo07OibjuRmsiHcHEN7g,2959
 core/wmconstants.py,sha256=GzN41wXYmFfrJYYHtXCguqmK6zTJDq9gGDuw1xf0PIY,1321
-dbl_sat_sdk-0.1.8.dist-info/METADATA,sha256=-qbdSo8f7vmU7Q6e7W6tly9SXT9x8f4ze8JhQ89Dz1g,735
-dbl_sat_sdk-0.1.8.dist-info/NOTICE,sha256=POLipUF2k4vN9qWJYiWabZ5iBI0mOlVV_J_kFpyilEg,320
-dbl_sat_sdk-0.1.8.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-dbl_sat_sdk-0.1.8.dist-info/top_level.txt,sha256=LnTjvDc2mlXT9Bf_kD8ha4qKoxBLnocFiOTKgTdv2pY,16
-dbl_sat_sdk-0.1.8.dist-info/RECORD,,
+dbl_sat_sdk-0.1.9.dist-info/METADATA,sha256=Ii3t0JrIOePdzqAhz5zW4bZds0wAnY5BuXU-GQP2-Kk,735
+dbl_sat_sdk-0.1.9.dist-info/NOTICE,sha256=POLipUF2k4vN9qWJYiWabZ5iBI0mOlVV_J_kFpyilEg,320
+dbl_sat_sdk-0.1.9.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+dbl_sat_sdk-0.1.9.dist-info/top_level.txt,sha256=LnTjvDc2mlXT9Bf_kD8ha4qKoxBLnocFiOTKgTdv2pY,16
+dbl_sat_sdk-0.1.9.dist-info/RECORD,,
```

