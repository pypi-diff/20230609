# Comparing `tmp/fsa_logger-0.1.1-py3-none-any.whl.zip` & `tmp/fsa_logger-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 37988 bytes, number of entries: 20
+Zip file size: 37997 bytes, number of entries: 20
 -rw-r--r--  2.0 fat        0 b- defN 80-Jan-01 00:00 fsa_logger/__init__.py
 -rw-r--r--  2.0 fat        0 b- defN 80-Jan-01 00:00 fsa_logger/config/__init__.py
 -rw-r--r--  2.0 fat     2278 b- defN 80-Jan-01 00:00 fsa_logger/config/config.py
 -rw-r--r--  2.0 fat     1031 b- defN 80-Jan-01 00:00 fsa_logger/config/log_config.py
 -rw-r--r--  2.0 fat        0 b- defN 80-Jan-01 00:00 fsa_logger/fsa_cli/__init__.py
 -rw-r--r--  2.0 fat     4450 b- defN 80-Jan-01 00:00 fsa_logger/fsa_cli/cli_common.py
 -rw-r--r--  2.0 fat    11861 b- defN 80-Jan-01 00:00 fsa_logger/fsa_cli/cli_sensors.py
@@ -11,12 +11,12 @@
 -rw-r--r--  2.0 fat     2728 b- defN 80-Jan-01 00:00 fsa_logger/fsa_cli/labels.py
 -rw-r--r--  2.0 fat     4404 b- defN 80-Jan-01 00:00 fsa_logger/fsa_cli/main_cli.py
 -rw-r--r--  2.0 fat    20742 b- defN 80-Jan-01 00:00 fsa_logger/imu_sensor_service.py
 -rw-r--r--  2.0 fat     9293 b- defN 80-Jan-01 00:00 fsa_logger/sensor_api.py
 -rw-r--r--  2.0 fat    26657 b- defN 80-Jan-01 00:00 fsa_logger/sensor_controller.py
 -rw-r--r--  2.0 fat    17359 b- defN 80-Jan-01 00:00 fsa_logger/session_controller.py
 -rw-r--r--  2.0 fat     1740 b- defN 80-Jan-01 00:00 fsa_logger/utils.py
-?rw-r--r--  2.0 fat       38 b- defN 16-Jan-01 00:00 fsa_logger-0.1.1.dist-info/entry_points.txt
-?rw-r--r--  2.0 fat       88 b- defN 16-Jan-01 00:00 fsa_logger-0.1.1.dist-info/WHEEL
-?rw-r--r--  2.0 fat    36217 b- defN 16-Jan-01 00:00 fsa_logger-0.1.1.dist-info/METADATA
-?rw-r--r--  2.0 fat     1690 b- defN 16-Jan-01 00:00 fsa_logger-0.1.1.dist-info/RECORD
-20 files, 164123 bytes uncompressed, 35226 bytes compressed:  78.5%
+?rw-r--r--  2.0 fat       39 b- defN 16-Jan-01 00:00 fsa_logger-0.1.2.dist-info/entry_points.txt
+?rw-r--r--  2.0 fat       88 b- defN 16-Jan-01 00:00 fsa_logger-0.1.2.dist-info/WHEEL
+?rw-r--r--  2.0 fat    36217 b- defN 16-Jan-01 00:00 fsa_logger-0.1.2.dist-info/METADATA
+?rw-r--r--  2.0 fat     1690 b- defN 16-Jan-01 00:00 fsa_logger-0.1.2.dist-info/RECORD
+20 files, 164124 bytes uncompressed, 35235 bytes compressed:  78.5%
```

## zipnote {}

```diff
@@ -42,20 +42,20 @@
 
 Filename: fsa_logger/session_controller.py
 Comment: 
 
 Filename: fsa_logger/utils.py
 Comment: 
 
-Filename: fsa_logger-0.1.1.dist-info/entry_points.txt
+Filename: fsa_logger-0.1.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: fsa_logger-0.1.1.dist-info/WHEEL
+Filename: fsa_logger-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: fsa_logger-0.1.1.dist-info/METADATA
+Filename: fsa_logger-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: fsa_logger-0.1.1.dist-info/RECORD
+Filename: fsa_logger-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `fsa_logger-0.1.1.dist-info/METADATA` & `fsa_logger-0.1.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fsa-logger
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: amarco2
 Author-email: amarco@unizar.es
 Requires-Python: >=3.9,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

## Comparing `fsa_logger-0.1.1.dist-info/RECORD` & `fsa_logger-0.1.2.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -10,11 +10,11 @@
 fsa_logger/fsa_cli/labels.py,sha256=uOxan87gaxtwrus2cGLulMef3S53dY1GAFQhFkxsnC4,2728
 fsa_logger/fsa_cli/main_cli.py,sha256=bNiBTky3m2YV_Om9qv839hvdTPYZOP12Cnlqggde3hg,4404
 fsa_logger/imu_sensor_service.py,sha256=OW4VnC10Wb8hIobASbreVKXpjtB5XF8qIWMRtMHKKxo,20742
 fsa_logger/sensor_api.py,sha256=IX7-O3CQVeWYvHsRlp6LydCsVMTEp8oLyA2HMc5e6hM,9293
 fsa_logger/sensor_controller.py,sha256=aIfBKXNu-HKP-aTvtDc0zYWbb0RK5NFRUbtu1FyYyYU,26657
 fsa_logger/session_controller.py,sha256=v2zMH-bMtLReOkuEgEa4GpW6mPw-wvpqnYIVi-BO5kA,17359
 fsa_logger/utils.py,sha256=2BOfQR8KsZlf2n5QF7pge8kzgqjjEQePvSx5je5_Rhw,1740
-fsa_logger-0.1.1.dist-info/entry_points.txt,sha256=b0b2t6hVpZFI2iSoRCjO1_H5jbVmVCfpXZ91MyxgDLc,38
-fsa_logger-0.1.1.dist-info/WHEEL,sha256=bbU3AyvhQ312rVm7zzRQjs6axI1UYWC3nmFA2E6FFSI,88
-fsa_logger-0.1.1.dist-info/METADATA,sha256=Fb4jKflCSP-fx3InMA58uA8z_SCsa7lA4-Cxc63nEOM,36217
-fsa_logger-0.1.1.dist-info/RECORD,,
+fsa_logger-0.1.2.dist-info/entry_points.txt,sha256=eRLgXerpzYpEBapYILOke-LhUMsVjE8i34wr5zoGp48,39
+fsa_logger-0.1.2.dist-info/WHEEL,sha256=bbU3AyvhQ312rVm7zzRQjs6axI1UYWC3nmFA2E6FFSI,88
+fsa_logger-0.1.2.dist-info/METADATA,sha256=k_ilHLZYtBxaqjwN32B8GYDPSg_hOXwlb3CBOST6QF8,36217
+fsa_logger-0.1.2.dist-info/RECORD,,
```

