# Comparing `tmp/DroidRpc-1.6.6.tar.gz` & `tmp/DroidRpc-1.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DroidRpc-1.6.6.tar", last modified: Mon Feb  6 07:25:32 2023, max compression
+gzip compressed data, was "DroidRpc-1.6.7.tar", last modified: Fri Jun  9 01:37:03 2023, max compression
```

## Comparing `DroidRpc-1.6.6.tar` & `DroidRpc-1.6.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 loratech  (1000) loratech  (1000)        0 2023-02-06 07:25:32.411384 DroidRpc-1.6.6/
--rwxrwxr-x   0 loratech  (1000) loratech  (1000)       25 2023-01-30 07:35:07.000000 DroidRpc-1.6.6/MANIFEST.in
--rw-rw-r--   0 loratech  (1000) loratech  (1000)      539 2023-02-06 07:25:32.411384 DroidRpc-1.6.6/PKG-INFO
--rwxrwxr-x   0 loratech  (1000) loratech  (1000)      274 2023-01-30 07:35:07.000000 DroidRpc-1.6.6/README.md
--rwxrwxr-x   0 loratech  (1000) loratech  (1000)      132 2023-01-24 15:27:46.000000 DroidRpc-1.6.6/requirements.txt
--rw-rw-r--   0 loratech  (1000) loratech  (1000)       38 2023-02-06 07:25:32.411384 DroidRpc-1.6.6/setup.cfg
--rwxrwxr-x   0 loratech  (1000) loratech  (1000)      777 2023-02-06 07:22:37.000000 DroidRpc-1.6.6/setup.py
-drwxrwxr-x   0 loratech  (1000) loratech  (1000)        0 2023-02-06 07:25:32.411384 DroidRpc-1.6.6/src/
-drwxrwxr-x   0 loratech  (1000) loratech  (1000)        0 2023-02-06 07:25:32.411384 DroidRpc-1.6.6/src/DroidRpc/
--rw-rw-r--   0 loratech  (1000) loratech  (1000)       25 2023-01-24 15:27:46.000000 DroidRpc-1.6.6/src/DroidRpc/__init__.py
--rw-rw-r--   0 loratech  (1000) loratech  (1000)     1767 2023-01-30 07:35:07.000000 DroidRpc-1.6.6/src/DroidRpc/droid_grpc.py
--rw-rw-r--   0 loratech  (1000) loratech  (1000)     5480 2023-01-30 07:35:07.000000 DroidRpc-1.6.6/src/DroidRpc/droid_pb2.py
-drwxrwxr-x   0 loratech  (1000) loratech  (1000)        0 2023-02-06 07:25:32.411384 DroidRpc-1.6.6/src/DroidRpc/formatting/
--rw-rw-r--   0 loratech  (1000) loratech  (1000)      388 2023-01-24 15:27:46.000000 DroidRpc-1.6.6/src/DroidRpc/formatting/__init__.py
--rw-rw-r--   0 loratech  (1000) loratech  (1000)    12806 2023-02-01 09:50:14.000000 DroidRpc-1.6.6/src/DroidRpc/formatting/converter.py
--rw-rw-r--   0 loratech  (1000) loratech  (1000)      398 2023-01-24 15:27:46.000000 DroidRpc-1.6.6/src/DroidRpc/formatting/datetime.py
--rw-rw-r--   0 loratech  (1000) loratech  (1000)    16730 2023-02-06 07:22:28.000000 DroidRpc-1.6.6/src/DroidRpc/main.py
--rw-rw-r--   0 loratech  (1000) loratech  (1000)     4446 2023-02-01 10:03:01.000000 DroidRpc-1.6.6/src/DroidRpc/raw_client_example.py
-drwxrwxr-x   0 loratech  (1000) loratech  (1000)        0 2023-02-06 07:25:32.411384 DroidRpc-1.6.6/src/DroidRpc.egg-info/
--rw-rw-r--   0 loratech  (1000) loratech  (1000)      539 2023-02-06 07:25:32.000000 DroidRpc-1.6.6/src/DroidRpc.egg-info/PKG-INFO
--rw-rw-r--   0 loratech  (1000) loratech  (1000)      504 2023-02-06 07:25:32.000000 DroidRpc-1.6.6/src/DroidRpc.egg-info/SOURCES.txt
--rw-rw-r--   0 loratech  (1000) loratech  (1000)        1 2023-02-06 07:25:32.000000 DroidRpc-1.6.6/src/DroidRpc.egg-info/dependency_links.txt
--rw-rw-r--   0 loratech  (1000) loratech  (1000)        1 2023-02-06 04:42:07.000000 DroidRpc-1.6.6/src/DroidRpc.egg-info/not-zip-safe
--rw-rw-r--   0 loratech  (1000) loratech  (1000)      132 2023-02-06 07:25:32.000000 DroidRpc-1.6.6/src/DroidRpc.egg-info/requires.txt
--rw-rw-r--   0 loratech  (1000) loratech  (1000)        9 2023-02-06 07:25:32.000000 DroidRpc-1.6.6/src/DroidRpc.egg-info/top_level.txt
+drwxrwxr-x   0 loratech  (1000) loratech  (1000)        0 2023-06-09 01:37:03.444829 DroidRpc-1.6.7/
+-rwxrwxr-x   0 loratech  (1000) loratech  (1000)       25 2023-05-05 03:50:53.000000 DroidRpc-1.6.7/MANIFEST.in
+-rw-rw-r--   0 loratech  (1000) loratech  (1000)      539 2023-06-09 01:37:03.444829 DroidRpc-1.6.7/PKG-INFO
+-rwxrwxr-x   0 loratech  (1000) loratech  (1000)      274 2023-05-05 03:50:53.000000 DroidRpc-1.6.7/README.md
+-rwxrwxr-x   0 loratech  (1000) loratech  (1000)      132 2023-05-05 03:50:53.000000 DroidRpc-1.6.7/requirements.txt
+-rw-rw-r--   0 loratech  (1000) loratech  (1000)       38 2023-06-09 01:37:03.444829 DroidRpc-1.6.7/setup.cfg
+-rwxrwxr-x   0 loratech  (1000) loratech  (1000)      777 2023-06-09 01:36:58.000000 DroidRpc-1.6.7/setup.py
+drwxrwxr-x   0 loratech  (1000) loratech  (1000)        0 2023-06-09 01:37:03.440829 DroidRpc-1.6.7/src/
+drwxrwxr-x   0 loratech  (1000) loratech  (1000)        0 2023-06-09 01:37:03.444829 DroidRpc-1.6.7/src/DroidRpc/
+-rw-rw-r--   0 loratech  (1000) loratech  (1000)       25 2023-05-05 03:50:53.000000 DroidRpc-1.6.7/src/DroidRpc/__init__.py
+-rw-rw-r--   0 loratech  (1000) loratech  (1000)     1767 2023-06-08 10:44:37.000000 DroidRpc-1.6.7/src/DroidRpc/droid_grpc.py
+-rw-rw-r--   0 loratech  (1000) loratech  (1000)     5572 2023-06-08 10:44:37.000000 DroidRpc-1.6.7/src/DroidRpc/droid_pb2.py
+drwxrwxr-x   0 loratech  (1000) loratech  (1000)        0 2023-06-09 01:37:03.444829 DroidRpc-1.6.7/src/DroidRpc/formatting/
+-rw-rw-r--   0 loratech  (1000) loratech  (1000)      388 2023-05-05 03:50:53.000000 DroidRpc-1.6.7/src/DroidRpc/formatting/__init__.py
+-rw-rw-r--   0 loratech  (1000) loratech  (1000)    12910 2023-06-08 10:44:23.000000 DroidRpc-1.6.7/src/DroidRpc/formatting/converter.py
+-rw-rw-r--   0 loratech  (1000) loratech  (1000)      398 2023-05-05 03:50:53.000000 DroidRpc-1.6.7/src/DroidRpc/formatting/datetime.py
+-rw-rw-r--   0 loratech  (1000) loratech  (1000)    16801 2023-06-08 11:33:24.000000 DroidRpc-1.6.7/src/DroidRpc/main.py
+-rw-rw-r--   0 loratech  (1000) loratech  (1000)     4446 2023-05-05 03:50:53.000000 DroidRpc-1.6.7/src/DroidRpc/raw_client_example.py
+drwxrwxr-x   0 loratech  (1000) loratech  (1000)        0 2023-06-09 01:37:03.444829 DroidRpc-1.6.7/src/DroidRpc.egg-info/
+-rw-rw-r--   0 loratech  (1000) loratech  (1000)      539 2023-06-09 01:37:03.000000 DroidRpc-1.6.7/src/DroidRpc.egg-info/PKG-INFO
+-rw-rw-r--   0 loratech  (1000) loratech  (1000)      504 2023-06-09 01:37:03.000000 DroidRpc-1.6.7/src/DroidRpc.egg-info/SOURCES.txt
+-rw-rw-r--   0 loratech  (1000) loratech  (1000)        1 2023-06-09 01:37:03.000000 DroidRpc-1.6.7/src/DroidRpc.egg-info/dependency_links.txt
+-rw-rw-r--   0 loratech  (1000) loratech  (1000)        1 2023-06-08 10:50:42.000000 DroidRpc-1.6.7/src/DroidRpc.egg-info/not-zip-safe
+-rw-rw-r--   0 loratech  (1000) loratech  (1000)      132 2023-06-09 01:37:03.000000 DroidRpc-1.6.7/src/DroidRpc.egg-info/requires.txt
+-rw-rw-r--   0 loratech  (1000) loratech  (1000)        9 2023-06-09 01:37:03.000000 DroidRpc-1.6.7/src/DroidRpc.egg-info/top_level.txt
```

### Comparing `DroidRpc-1.6.6/PKG-INFO` & `DroidRpc-1.6.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DroidRpc
-Version: 1.6.6
+Version: 1.6.7
 Summary: Python client for connecting to LORA Technologies' bot services.
 Home-page: https://asklora.ai
 Author: LORA Tech
 Author-email: asklora@loratechai.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `DroidRpc-1.6.6/setup.py` & `DroidRpc-1.6.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     long_description = f.read()
 
 with open("requirements.txt", "r", encoding="utf-8") as f:
     required = f.read().splitlines()
 
 setuptools.setup(
     name="DroidRpc",
-    version="1.6.6",
+    version="1.6.7",
     description="Python client for connecting to LORA Technologies' bot services.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://asklora.ai",
     license="MIT",
     install_requires=required,
     author="LORA Tech",
```

### Comparing `DroidRpc-1.6.6/src/DroidRpc/droid_grpc.py` & `DroidRpc-1.6.7/src/DroidRpc/droid_grpc.py`

 * *Files identical despite different names*

### Comparing `DroidRpc-1.6.6/src/DroidRpc/droid_pb2.py` & `DroidRpc-1.6.7/src/DroidRpc/droid_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,25 +9,25 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0b\x64roid.proto\x12\x07\x64roidv3\"\xc6\x03\n\x12\x42\x61tchCreateRequest\x12\x0e\n\x06ticker\x18\x01 \x01(\x0c\x12\x11\n\tspot_date\x18\x02 \x01(\x0c\x12\x0e\n\x06\x62ot_id\x18\x03 \x01(\x0c\x12\x19\n\x11investment_amount\x18\x04 \x01(\x0c\x12\r\n\x05price\x18\x05 \x01(\x0c\x12\x0e\n\x06margin\x18\x06 \x01(\x0c\x12\x10\n\x08\x66raction\x18\x07 \x01(\x0c\x12\x14\n\x0cmultiplier_1\x18\x08 \x01(\x0c\x12\x14\n\x0cmultiplier_2\x18\t \x01(\x0c\x12\x10\n\x08\x63urrency\x18\n \x01(\x0c\x12\x13\n\x0btime_to_exp\x18\x0b \x01(\x0c\x12\x13\n\x0boption_type\x18\x0c \x01(\x0c\x12\x10\n\x08\x62ot_type\x18\r \x01(\x0c\x12\x1b\n\x13\x61tm_volatility_spot\x18\x0e \x01(\x0c\x12\x1f\n\x17\x61tm_volatility_one_year\x18\x0f \x01(\x0c\x12\x1f\n\x17\x61tm_volatility_infinity\x18\x10 \x01(\x0c\x12\r\n\x05slope\x18\x11 \x01(\x0c\x12\x11\n\tslope_inf\x18\x12 \x01(\x0c\x12\r\n\x05\x64\x65riv\x18\x13 \x01(\x0c\x12\x11\n\tderiv_inf\x18\x14 \x01(\x0c\x12\t\n\x01q\x18\x15 \x01(\x0c\x12\t\n\x01r\x18\x16 \x01(\x0c\"\x91\x04\n\x11\x42\x61tchHedgeRequest\x12\x0e\n\x06ticker\x18\x01 \x01(\x0c\x12\x11\n\tspot_date\x18\x02 \x01(\x0c\x12\x0e\n\x06\x62ot_id\x18\x03 \x01(\x0c\x12\x19\n\x11investment_amount\x18\x04 \x01(\x0c\x12\r\n\x05price\x18\x05 \x01(\x0c\x12\x0e\n\x06margin\x18\x06 \x01(\x0c\x12\x10\n\x08\x66raction\x18\x07 \x01(\x0c\x12\x16\n\x0elast_share_num\x18\x08 \x01(\x0c\x12\x1b\n\x13total_bot_share_num\x18\t \x01(\x0c\x12\x13\n\x0b\x65xpire_date\x18\n \x01(\x0c\x12\x15\n\rprice_level_1\x18\x0b \x01(\x0c\x12\x15\n\rprice_level_2\x18\x0c \x01(\x0c\x12\x10\n\x08\x63urrency\x18\r \x01(\x0c\x12\x13\n\x0btime_to_exp\x18\x0e \x01(\x0c\x12\x13\n\x0boption_type\x18\x0f \x01(\x0c\x12\x10\n\x08\x62ot_type\x18\x10 \x01(\x0c\x12\x1b\n\x13\x61tm_volatility_spot\x18\x11 \x01(\x0c\x12\x1f\n\x17\x61tm_volatility_one_year\x18\x12 \x01(\x0c\x12\x1f\n\x17\x61tm_volatility_infinity\x18\x13 \x01(\x0c\x12\r\n\x05slope\x18\x14 \x01(\x0c\x12\x11\n\tslope_inf\x18\x15 \x01(\x0c\x12\r\n\x05\x64\x65riv\x18\x16 \x01(\x0c\x12\x11\n\tderiv_inf\x18\x17 \x01(\x0c\x12\t\n\x01q\x18\x18 \x01(\x0c\x12\t\n\x01r\x18\x19 \x01(\x0c\"\x86\x05\n\x13\x42\x61tchCreateResponse\x12\x0e\n\x06ticker\x18\x01 \x01(\x0c\x12\x11\n\tspot_date\x18\x02 \x01(\x0c\x12\x0e\n\x06\x62ot_id\x18\x03 \x01(\x0c\x12\x19\n\x11investment_amount\x18\x04 \x01(\x0c\x12\r\n\x05price\x18\x05 \x01(\x0c\x12\x0e\n\x06margin\x18\x06 \x01(\x0c\x12\x10\n\x08\x66raction\x18\x07 \x01(\x0c\x12\x14\n\x0cmultiplier_1\x18\x08 \x01(\x0c\x12\x14\n\x0cmultiplier_2\x18\t \x01(\x0c\x12\r\n\x05\x64\x65lta\x18\n \x01(\x0c\x12\x11\n\tshare_num\x18\x0b \x01(\x0c\x12\x18\n\x10share_num_change\x18\x0c \x01(\x0c\x12\x1b\n\x13total_bot_share_num\x18\r \x01(\x0c\x12\x13\n\x0b\x65xpire_date\x18\x0e \x01(\x0c\x12\x0e\n\x06status\x18\x0f \x01(\x0c\x12\x15\n\rprice_level_1\x18\x10 \x01(\x0c\x12\x15\n\rprice_level_2\x18\x11 \x01(\x0c\x12\x17\n\x0fmax_loss_amount\x18\x12 \x01(\x0c\x12\x14\n\x0cmax_loss_pct\x18\x13 \x01(\x0c\x12\x16\n\x0emax_loss_price\x18\x14 \x01(\x0c\x12\x1c\n\x14target_profit_amount\x18\x15 \x01(\x0c\x12\x19\n\x11target_profit_pct\x18\x16 \x01(\x0c\x12\x1b\n\x13target_profit_price\x18\x17 \x01(\x0c\x12\x13\n\x0b\x63lassic_vol\x18\x18 \x01(\x0c\x12\x10\n\x08vol_spot\x18\x19 \x01(\x0c\x12\x13\n\x0bvol_price_1\x18\x1a \x01(\x0c\x12\x13\n\x0bvol_price_2\x18\x1b \x01(\x0c\x12\t\n\x01q\x18\x1c \x01(\x0c\x12\t\n\x01r\x18\x1d \x01(\x0c\x12\x14\n\x0coption_price\x18\x1e \x01(\x0c\"\xa5\x02\n\x12\x42\x61tchHedgeResponse\x12\x0e\n\x06ticker\x18\x01 \x01(\x0c\x12\x11\n\tspot_date\x18\x02 \x01(\x0c\x12\x0e\n\x06\x62ot_id\x18\x03 \x01(\x0c\x12\x19\n\x11investment_amount\x18\x04 \x01(\x0c\x12\r\n\x05price\x18\x05 \x01(\x0c\x12\r\n\x05\x64\x65lta\x18\x06 \x01(\x0c\x12\x11\n\tshare_num\x18\x07 \x01(\x0c\x12\x18\n\x10share_num_change\x18\x08 \x01(\x0c\x12\x0e\n\x06status\x18\t \x01(\x0c\x12\x10\n\x08vol_spot\x18\n \x01(\x0c\x12\x13\n\x0bvol_price_1\x18\x0b \x01(\x0c\x12\x13\n\x0bvol_price_2\x18\x0c \x01(\x0c\x12\t\n\x01q\x18\r \x01(\x0c\x12\t\n\x01r\x18\x0e \x01(\x0c\x12\x14\n\x0coption_price\x18\x0f \x01(\x0c\x32\x9a\x01\n\x05\x44roid\x12I\n\nCreateBots\x12\x1b.droidv3.BatchCreateRequest\x1a\x1c.droidv3.BatchCreateResponse\"\x00\x12\x46\n\tHedgeBots\x12\x1a.droidv3.BatchHedgeRequest\x1a\x1b.droidv3.BatchHedgeResponse\"\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0b\x64roid.proto\x12\x07\x64roidv3\"\xdb\x03\n\x12\x42\x61tchCreateRequest\x12\x0e\n\x06ticker\x18\x01 \x01(\x0c\x12\x11\n\tspot_date\x18\x02 \x01(\x0c\x12\x0e\n\x06\x62ot_id\x18\x03 \x01(\x0c\x12\x19\n\x11investment_amount\x18\x04 \x01(\x0c\x12\r\n\x05price\x18\x05 \x01(\x0c\x12\x0e\n\x06margin\x18\x06 \x01(\x0c\x12\x10\n\x08\x66raction\x18\x07 \x01(\x0c\x12\x14\n\x0cmultiplier_1\x18\x08 \x01(\x0c\x12\x14\n\x0cmultiplier_2\x18\t \x01(\x0c\x12\x10\n\x08\x63urrency\x18\n \x01(\x0c\x12\x13\n\x0btime_to_exp\x18\x0b \x01(\x0c\x12\x13\n\x0boption_type\x18\x0c \x01(\x0c\x12\x10\n\x08\x62ot_type\x18\r \x01(\x0c\x12\x1b\n\x13\x61tm_volatility_spot\x18\x0e \x01(\x0c\x12\x1f\n\x17\x61tm_volatility_one_year\x18\x0f \x01(\x0c\x12\x1f\n\x17\x61tm_volatility_infinity\x18\x10 \x01(\x0c\x12\r\n\x05slope\x18\x11 \x01(\x0c\x12\x11\n\tslope_inf\x18\x12 \x01(\x0c\x12\r\n\x05\x64\x65riv\x18\x13 \x01(\x0c\x12\x11\n\tderiv_inf\x18\x14 \x01(\x0c\x12\t\n\x01q\x18\x15 \x01(\x0c\x12\t\n\x01r\x18\x16 \x01(\x0c\x12\x13\n\x0b\x63lassic_vol\x18\x17 \x01(\x0c\"\xa6\x04\n\x11\x42\x61tchHedgeRequest\x12\x0e\n\x06ticker\x18\x01 \x01(\x0c\x12\x11\n\tspot_date\x18\x02 \x01(\x0c\x12\x0e\n\x06\x62ot_id\x18\x03 \x01(\x0c\x12\x19\n\x11investment_amount\x18\x04 \x01(\x0c\x12\r\n\x05price\x18\x05 \x01(\x0c\x12\x0e\n\x06margin\x18\x06 \x01(\x0c\x12\x10\n\x08\x66raction\x18\x07 \x01(\x0c\x12\x16\n\x0elast_share_num\x18\x08 \x01(\x0c\x12\x1b\n\x13total_bot_share_num\x18\t \x01(\x0c\x12\x13\n\x0b\x65xpire_date\x18\n \x01(\x0c\x12\x15\n\rprice_level_1\x18\x0b \x01(\x0c\x12\x15\n\rprice_level_2\x18\x0c \x01(\x0c\x12\x10\n\x08\x63urrency\x18\r \x01(\x0c\x12\x13\n\x0btime_to_exp\x18\x0e \x01(\x0c\x12\x13\n\x0boption_type\x18\x0f \x01(\x0c\x12\x10\n\x08\x62ot_type\x18\x10 \x01(\x0c\x12\x1b\n\x13\x61tm_volatility_spot\x18\x11 \x01(\x0c\x12\x1f\n\x17\x61tm_volatility_one_year\x18\x12 \x01(\x0c\x12\x1f\n\x17\x61tm_volatility_infinity\x18\x13 \x01(\x0c\x12\r\n\x05slope\x18\x14 \x01(\x0c\x12\x11\n\tslope_inf\x18\x15 \x01(\x0c\x12\r\n\x05\x64\x65riv\x18\x16 \x01(\x0c\x12\x11\n\tderiv_inf\x18\x17 \x01(\x0c\x12\t\n\x01q\x18\x18 \x01(\x0c\x12\t\n\x01r\x18\x19 \x01(\x0c\x12\x13\n\x0b\x63lassic_vol\x18\x1a \x01(\x0c\"\x86\x05\n\x13\x42\x61tchCreateResponse\x12\x0e\n\x06ticker\x18\x01 \x01(\x0c\x12\x11\n\tspot_date\x18\x02 \x01(\x0c\x12\x0e\n\x06\x62ot_id\x18\x03 \x01(\x0c\x12\x19\n\x11investment_amount\x18\x04 \x01(\x0c\x12\r\n\x05price\x18\x05 \x01(\x0c\x12\x0e\n\x06margin\x18\x06 \x01(\x0c\x12\x10\n\x08\x66raction\x18\x07 \x01(\x0c\x12\x14\n\x0cmultiplier_1\x18\x08 \x01(\x0c\x12\x14\n\x0cmultiplier_2\x18\t \x01(\x0c\x12\r\n\x05\x64\x65lta\x18\n \x01(\x0c\x12\x11\n\tshare_num\x18\x0b \x01(\x0c\x12\x18\n\x10share_num_change\x18\x0c \x01(\x0c\x12\x1b\n\x13total_bot_share_num\x18\r \x01(\x0c\x12\x13\n\x0b\x65xpire_date\x18\x0e \x01(\x0c\x12\x0e\n\x06status\x18\x0f \x01(\x0c\x12\x15\n\rprice_level_1\x18\x10 \x01(\x0c\x12\x15\n\rprice_level_2\x18\x11 \x01(\x0c\x12\x17\n\x0fmax_loss_amount\x18\x12 \x01(\x0c\x12\x14\n\x0cmax_loss_pct\x18\x13 \x01(\x0c\x12\x16\n\x0emax_loss_price\x18\x14 \x01(\x0c\x12\x1c\n\x14target_profit_amount\x18\x15 \x01(\x0c\x12\x19\n\x11target_profit_pct\x18\x16 \x01(\x0c\x12\x1b\n\x13target_profit_price\x18\x17 \x01(\x0c\x12\x13\n\x0b\x63lassic_vol\x18\x18 \x01(\x0c\x12\x10\n\x08vol_spot\x18\x19 \x01(\x0c\x12\x13\n\x0bvol_price_1\x18\x1a \x01(\x0c\x12\x13\n\x0bvol_price_2\x18\x1b \x01(\x0c\x12\t\n\x01q\x18\x1c \x01(\x0c\x12\t\n\x01r\x18\x1d \x01(\x0c\x12\x14\n\x0coption_price\x18\x1e \x01(\x0c\"\xa5\x02\n\x12\x42\x61tchHedgeResponse\x12\x0e\n\x06ticker\x18\x01 \x01(\x0c\x12\x11\n\tspot_date\x18\x02 \x01(\x0c\x12\x0e\n\x06\x62ot_id\x18\x03 \x01(\x0c\x12\x19\n\x11investment_amount\x18\x04 \x01(\x0c\x12\r\n\x05price\x18\x05 \x01(\x0c\x12\r\n\x05\x64\x65lta\x18\x06 \x01(\x0c\x12\x11\n\tshare_num\x18\x07 \x01(\x0c\x12\x18\n\x10share_num_change\x18\x08 \x01(\x0c\x12\x0e\n\x06status\x18\t \x01(\x0c\x12\x10\n\x08vol_spot\x18\n \x01(\x0c\x12\x13\n\x0bvol_price_1\x18\x0b \x01(\x0c\x12\x13\n\x0bvol_price_2\x18\x0c \x01(\x0c\x12\t\n\x01q\x18\r \x01(\x0c\x12\t\n\x01r\x18\x0e \x01(\x0c\x12\x14\n\x0coption_price\x18\x0f \x01(\x0c\x32\x9a\x01\n\x05\x44roid\x12I\n\nCreateBots\x12\x1b.droidv3.BatchCreateRequest\x1a\x1c.droidv3.BatchCreateResponse\"\x00\x12\x46\n\tHedgeBots\x12\x1a.droidv3.BatchHedgeRequest\x1a\x1b.droidv3.BatchHedgeResponse\"\x00\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'droid_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   _BATCHCREATEREQUEST._serialized_start=25
-  _BATCHCREATEREQUEST._serialized_end=479
-  _BATCHHEDGEREQUEST._serialized_start=482
-  _BATCHHEDGEREQUEST._serialized_end=1011
-  _BATCHCREATERESPONSE._serialized_start=1014
-  _BATCHCREATERESPONSE._serialized_end=1660
-  _BATCHHEDGERESPONSE._serialized_start=1663
-  _BATCHHEDGERESPONSE._serialized_end=1956
-  _DROID._serialized_start=1959
-  _DROID._serialized_end=2113
+  _BATCHCREATEREQUEST._serialized_end=500
+  _BATCHHEDGEREQUEST._serialized_start=503
+  _BATCHHEDGEREQUEST._serialized_end=1053
+  _BATCHCREATERESPONSE._serialized_start=1056
+  _BATCHCREATERESPONSE._serialized_end=1702
+  _BATCHHEDGERESPONSE._serialized_start=1705
+  _BATCHHEDGERESPONSE._serialized_end=1998
+  _DROID._serialized_start=2001
+  _DROID._serialized_end=2155
 # @@protoc_insertion_point(module_scope)
```

### Comparing `DroidRpc-1.6.6/src/DroidRpc/formatting/converter.py` & `DroidRpc-1.6.7/src/DroidRpc/formatting/converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,23 +8,24 @@
 from DroidRpc.droid_pb2 import (
     BatchCreateRequest,
     BatchCreateResponse,
     BatchHedgeRequest,
     BatchHedgeResponse,
 )
 
+
 def array_to_bytes(array: np.ndarray):
     """
     Converts a numpy array to a bytestream.
     """
 
     # If using default: certain value may not be ndarray. Convert first.
     if type(array) in [float, bool, str, int]:
         array = np.array(array)
-    
+
     if array is None:
         return None
 
     if isinstance(array, np.ndarray):
         output = BytesIO()
         np.save(output, array, allow_pickle=False)
         return output.getvalue()
@@ -33,20 +34,21 @@
 
 
 def bytes_to_array(bytestream: BytesIO, dtype: Union[str, np.dtype]):
     """
     Converts a bytestream into a numpy array.
     """
     try:
-        if bytestream == b'': # Protobuf byte equivalent of "None"
+        if bytestream == b'':  # Protobuf byte equivalent of "None"
             return None
         return np.load(BytesIO(bytestream), allow_pickle=False).astype(dtype)
     except Exception as e:
         raise type(e)(f"Error converting {bytestream} to array") from e
 
+
 def create_request_proto_to_dict(req: BatchCreateRequest) -> Dict[str, bytes]:
     """
     Converts a create bots request into a dictionary.
     Note: Casting from bytes is done by the validator.
     """
     try:
         props = {
@@ -68,22 +70,25 @@
             "atm_volatility_infinity": req.atm_volatility_infinity,
             "slope": req.slope,
             "slope_inf": req.slope_inf,
             "deriv": req.deriv,
             "deriv_inf": req.deriv_inf,
             "q": req.q,
             "r": req.r,
+            "classic_vol": req.classic_vol
         }
-        props = {k: v for k, v in props.items() if v != b''} # Remove empty values
+        # Remove empty values
+        props = {k: v for k, v in props.items() if v != b''}
         return props
     except AttributeError as e:
         raise ValueError("Input field(s) missing") from e
     except Exception as e:
         raise e
 
+
 def hedge_request_proto_to_dict(req: BatchHedgeRequest) -> Dict[str, bytes]:
     """
     Converts a hedge bots request into a dictionary.
     Note: Casting from bytes is done by the validator.
     """
     try:
         props = {
@@ -108,22 +113,25 @@
             "atm_volatility_infinity": req.atm_volatility_infinity,
             "slope": req.slope,
             "slope_inf": req.slope_inf,
             "deriv": req.deriv,
             "deriv_inf": req.deriv_inf,
             "q": req.q,
             "r": req.r,
+            "classic_vol": req.classic_vol
         }
-        props = {k: v for k, v in props.items() if v != b''} # Remove empty values
+        # Remove empty values
+        props = {k: v for k, v in props.items() if v != b''}
         return props
     except AttributeError as e:
         raise ValueError("Input field(s) missing") from e
     except Exception as e:
         raise e
 
+
 def create_response_proto_to_dict(res: BatchCreateResponse) -> Dict[str, bytes]:
     """
     Converts a BotBatchCreatorResponse into a dictionary.
     """
     f = bytes_to_array
     try:
         props = {
@@ -160,14 +168,15 @@
         }
         return props
     except AttributeError as e:
         raise ValueError("Input field(s) missing") from e
     except Exception as e:
         raise e
 
+
 def hedge_response_proto_to_dict(res: BatchHedgeResponse) -> Dict[str, bytes]:
     """
     Converts a BotBatchHedgerResponse into a dictionary.
     """
     f = bytes_to_array
     try:
         props = {
@@ -189,14 +198,15 @@
         }
         return props
     except AttributeError as e:
         raise ValueError("Input field(s) missing") from e
     except Exception as e:
         raise e
 
+
 def create_request_dict_to_proto(req: Dict[str, bytes]) -> BatchCreateRequest:
     """
     Converts a dictionary of `NDArray` into a BotBatchCreatorRequest.
     """
     f = array_to_bytes
     try:
         props = {
@@ -224,14 +234,15 @@
             "r": f(req.get("r", None)),
         }
         props = {k: v for k, v in props.items() if v is not None}
         return BatchCreateRequest(**props)
     except KeyError as e:
         raise ValueError("Missing field") from e
 
+
 def hedge_request_dict_to_proto(req: Dict[str, bytes]) -> BatchHedgeRequest:
     """
     Converts a dictionary of `NDArray` into a BotBatchHedgerRequest.
     """
     f = array_to_bytes
     try:
         props = {
@@ -262,14 +273,15 @@
             "r": f(req.get("r", None)),
         }
         props = {k: v for k, v in props.items() if v is not None}
         return BatchHedgeRequest(**props)
     except KeyError as e:
         raise ValueError("Missing field") from e
 
+
 def input_dict_to_array(inputs: Dict[str, Union[str, float, list]],
                         to_list: bool = True) \
         -> Dict[str, np.ndarray]:
     """
     [TO BE DEPRECATED]
     Converts values of an input dictionary from `typing.Any` to `NDArray` with the 
     correct dtype (key name determines the dtype via dict lookup).
@@ -285,20 +297,21 @@
     Returns:
         Dictionary of inputs with values converted to np.NDArray and correct dtype.
     """
     from src.validator import input_dtypes
     return {k: np.array([v] if to_list else v).astype(input_dtypes[k])
             for k, v in inputs.items()}
 
+
 def input_array_to_byte(inputs: Dict[str, np.ndarray]) -> Dict[str, BytesIO]:
     """
     Converts values of an input dictionary of `NDArrays` to `bytes`.
     Specifically, used to create arguments to be passed to validator dataclasses 
     when creating props during testing.
 
     Args:
         inputs: Dictionary of inputs
-    
+
     Returns:
         Dictionary of inputs with values converted to bytes.
     """
     return {k: array_to_bytes(v) for k, v in inputs.items()}
```

### Comparing `DroidRpc-1.6.6/src/DroidRpc/main.py` & `DroidRpc-1.6.7/src/DroidRpc/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -381,14 +381,15 @@
         # TODO: Use self.create_bots() instead, reduce code duplication
         conn_err = False
         for _ in range(self.max_retries):
             try:
                 resp = await next(self._pool_itr)["stub"].CreateBots(
                     BatchCreateRequest(**inputs))
                 break
+            # TODO: better error handling here (e.g. for TimeoutError)
             except ConnectionRefusedError:
                 print('DROID connection error. Retrying...')
                 self._remove_dead_subclients()
                 conn_err = True
         if conn_err:
             self.renew_pool()
             # TODO: Schedule renewing of subclients
```

### Comparing `DroidRpc-1.6.6/src/DroidRpc/raw_client_example.py` & `DroidRpc-1.6.7/src/DroidRpc/raw_client_example.py`

 * *Files identical despite different names*

### Comparing `DroidRpc-1.6.6/src/DroidRpc.egg-info/PKG-INFO` & `DroidRpc-1.6.7/src/DroidRpc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DroidRpc
-Version: 1.6.6
+Version: 1.6.7
 Summary: Python client for connecting to LORA Technologies' bot services.
 Home-page: https://asklora.ai
 Author: LORA Tech
 Author-email: asklora@loratechai.com
 License: MIT
 Description-Content-Type: text/markdown
```

