# Comparing `tmp/blockchain-apis-0.1.1.tar.gz` & `tmp/blockchain-apis-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blockchain-apis-0.1.1.tar", last modified: Fri Jun  2 15:26:58 2023, max compression
+gzip compressed data, was "blockchain-apis-0.1.2.tar", last modified: Fri Jun  9 15:30:14 2023, max compression
```

## Comparing `blockchain-apis-0.1.1.tar` & `blockchain-apis-0.1.2.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-06-02 15:26:58.531387 blockchain-apis-0.1.1/
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1095 2023-05-30 13:02:28.000000 blockchain-apis-0.1.1/LICENSE
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4722 2023-06-02 15:26:58.531387 blockchain-apis-0.1.1/PKG-INFO
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3170 2023-06-02 14:42:47.000000 blockchain-apis-0.1.1/README.md
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)       38 2023-06-02 15:26:58.531387 blockchain-apis-0.1.1/setup.cfg
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1970 2023-06-02 15:26:36.000000 blockchain-apis-0.1.1/setup.py
-drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-06-02 15:26:58.523387 blockchain-apis-0.1.1/src/
-drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-06-02 15:26:58.523387 blockchain-apis-0.1.1/src/blockchain_apis.egg-info/
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4722 2023-06-02 15:26:58.000000 blockchain-apis-0.1.1/src/blockchain_apis.egg-info/PKG-INFO
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1718 2023-06-02 15:26:58.000000 blockchain-apis-0.1.1/src/blockchain_apis.egg-info/SOURCES.txt
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)        1 2023-06-02 15:26:58.000000 blockchain-apis-0.1.1/src/blockchain_apis.egg-info/dependency_links.txt
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)       17 2023-06-02 15:26:58.000000 blockchain-apis-0.1.1/src/blockchain_apis.egg-info/requires.txt
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)       15 2023-06-02 15:26:58.000000 blockchain-apis-0.1.1/src/blockchain_apis.egg-info/top_level.txt
-drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-06-02 15:26:58.527387 blockchain-apis-0.1.1/src/blockchainapis/
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)    24566 2023-06-02 14:37:21.000000 blockchain-apis-0.1.1/src/blockchainapis/BlockchainAPIs.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)    23995 2023-06-02 14:32:42.000000 blockchain-apis-0.1.1/src/blockchainapis/BlockchainAPIsSync.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      620 2023-06-02 15:16:57.000000 blockchain-apis-0.1.1/src/blockchainapis/__init__.py
-drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-06-02 15:26:58.527387 blockchain-apis-0.1.1/src/blockchainapis/exceptions/
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      454 2023-05-30 12:37:51.000000 blockchain-apis-0.1.1/src/blockchainapis/exceptions/BlockchainAPIsException.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      706 2023-06-02 14:30:29.000000 blockchain-apis-0.1.1/src/blockchainapis/exceptions/BlockchainNotSupportedException.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      699 2023-06-02 14:30:27.000000 blockchain-apis-0.1.1/src/blockchainapis/exceptions/ExchangeNotSupportedException.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      796 2023-06-02 14:30:24.000000 blockchain-apis-0.1.1/src/blockchainapis/exceptions/InvalidPageException.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      819 2023-06-02 14:30:21.000000 blockchain-apis-0.1.1/src/blockchainapis/exceptions/PairNotFoundException.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      798 2023-06-02 14:30:19.000000 blockchain-apis-0.1.1/src/blockchainapis/exceptions/TokenNotFoundException.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      733 2023-06-02 14:32:44.000000 blockchain-apis-0.1.1/src/blockchainapis/exceptions/TooManyRequestsException.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      716 2023-06-02 14:30:11.000000 blockchain-apis-0.1.1/src/blockchainapis/exceptions/UnauthorizedException.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      860 2023-06-02 14:32:35.000000 blockchain-apis-0.1.1/src/blockchainapis/exceptions/__init__.py
-drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-06-02 15:26:58.527387 blockchain-apis-0.1.1/src/blockchainapis/models/
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      860 2023-05-30 12:37:51.000000 blockchain-apis-0.1.1/src/blockchainapis/models/AmountIn.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      871 2023-05-30 12:37:51.000000 blockchain-apis-0.1.1/src/blockchainapis/models/AmountOut.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      580 2023-05-30 12:37:51.000000 blockchain-apis-0.1.1/src/blockchainapis/models/Blockchain.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      548 2023-05-30 12:37:51.000000 blockchain-apis-0.1.1/src/blockchainapis/models/Exchange.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      865 2023-06-02 14:27:29.000000 blockchain-apis-0.1.1/src/blockchainapis/models/Exchanges.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      678 2023-05-30 12:37:51.000000 blockchain-apis-0.1.1/src/blockchainapis/models/Pair.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      935 2023-06-02 14:28:25.000000 blockchain-apis-0.1.1/src/blockchainapis/models/Pairs.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      795 2023-05-30 12:37:51.000000 blockchain-apis-0.1.1/src/blockchainapis/models/Reserve.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      761 2023-05-30 12:37:51.000000 blockchain-apis-0.1.1/src/blockchainapis/models/Token.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1828 2023-06-02 14:28:34.000000 blockchain-apis-0.1.1/src/blockchainapis/models/Tokens.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1481 2023-06-02 14:07:13.000000 blockchain-apis-0.1.1/src/blockchainapis/models/__init__.py
-drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-06-02 15:26:58.531387 blockchain-apis-0.1.1/tests/
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1564 2023-06-02 14:28:02.000000 blockchain-apis-0.1.1/tests/test_amount_in.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1540 2023-06-02 14:36:02.000000 blockchain-apis-0.1.1/tests/test_amount_in_sync.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1568 2023-06-02 14:36:08.000000 blockchain-apis-0.1.1/tests/test_amount_out.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1544 2023-06-02 14:27:58.000000 blockchain-apis-0.1.1/tests/test_amount_out_sync.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      425 2023-06-02 14:36:12.000000 blockchain-apis-0.1.1/tests/test_blockchains.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      419 2023-06-02 14:36:10.000000 blockchain-apis-0.1.1/tests/test_blockchains_sync.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      569 2023-06-02 14:36:32.000000 blockchain-apis-0.1.1/tests/test_decimals.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      563 2023-06-02 14:36:19.000000 blockchain-apis-0.1.1/tests/test_decimals_sync.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1291 2023-06-02 14:36:44.000000 blockchain-apis-0.1.1/tests/test_exchanges.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1231 2023-06-02 14:36:34.000000 blockchain-apis-0.1.1/tests/test_exchanges_sync.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      593 2023-06-02 14:36:49.000000 blockchain-apis-0.1.1/tests/test_info.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      587 2023-06-02 14:36:46.000000 blockchain-apis-0.1.1/tests/test_info_sync.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2699 2023-06-02 14:36:53.000000 blockchain-apis-0.1.1/tests/test_pairs.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2567 2023-06-02 14:36:51.000000 blockchain-apis-0.1.1/tests/test_pairs_sync.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1392 2023-06-02 14:36:57.000000 blockchain-apis-0.1.1/tests/test_reserves.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1368 2023-06-02 14:36:55.000000 blockchain-apis-0.1.1/tests/test_reserves_sync.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1249 2023-06-02 14:37:01.000000 blockchain-apis-0.1.1/tests/test_tokens.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1189 2023-06-02 14:36:59.000000 blockchain-apis-0.1.1/tests/test_tokens_sync.py
+drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-06-09 15:30:14.941298 blockchain-apis-0.1.2/
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1095 2023-05-30 13:02:28.000000 blockchain-apis-0.1.2/LICENSE
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4722 2023-06-09 15:30:14.941298 blockchain-apis-0.1.2/PKG-INFO
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3170 2023-06-02 15:30:18.000000 blockchain-apis-0.1.2/README.md
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)       38 2023-06-09 15:30:14.941298 blockchain-apis-0.1.2/setup.cfg
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1970 2023-06-09 15:21:30.000000 blockchain-apis-0.1.2/setup.py
+drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-06-09 15:30:14.933297 blockchain-apis-0.1.2/src/
+drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-06-09 15:30:14.937297 blockchain-apis-0.1.2/src/blockchain_apis.egg-info/
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4722 2023-06-09 15:30:14.000000 blockchain-apis-0.1.2/src/blockchain_apis.egg-info/PKG-INFO
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1718 2023-06-09 15:30:14.000000 blockchain-apis-0.1.2/src/blockchain_apis.egg-info/SOURCES.txt
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)        1 2023-06-09 15:30:14.000000 blockchain-apis-0.1.2/src/blockchain_apis.egg-info/dependency_links.txt
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)       17 2023-06-09 15:30:14.000000 blockchain-apis-0.1.2/src/blockchain_apis.egg-info/requires.txt
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)       15 2023-06-09 15:30:14.000000 blockchain-apis-0.1.2/src/blockchain_apis.egg-info/top_level.txt
+drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-06-09 15:30:14.937297 blockchain-apis-0.1.2/src/blockchainapis/
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)    25822 2023-06-09 15:27:18.000000 blockchain-apis-0.1.2/src/blockchainapis/BlockchainAPIs.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)    25217 2023-06-09 15:27:15.000000 blockchain-apis-0.1.2/src/blockchainapis/BlockchainAPIsSync.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      622 2023-06-09 15:21:23.000000 blockchain-apis-0.1.2/src/blockchainapis/__init__.py
+drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-06-09 15:30:14.937297 blockchain-apis-0.1.2/src/blockchainapis/exceptions/
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      454 2023-06-09 15:18:43.000000 blockchain-apis-0.1.2/src/blockchainapis/exceptions/BlockchainAPIsException.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      681 2023-06-09 15:18:43.000000 blockchain-apis-0.1.2/src/blockchainapis/exceptions/BlockchainNotSupportedException.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      674 2023-06-09 15:18:43.000000 blockchain-apis-0.1.2/src/blockchainapis/exceptions/ExchangeNotSupportedException.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      771 2023-06-09 15:18:43.000000 blockchain-apis-0.1.2/src/blockchainapis/exceptions/InvalidPageException.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      794 2023-06-09 15:18:43.000000 blockchain-apis-0.1.2/src/blockchainapis/exceptions/PairNotFoundException.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      773 2023-06-09 15:18:43.000000 blockchain-apis-0.1.2/src/blockchainapis/exceptions/TokenNotFoundException.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      708 2023-06-09 15:18:43.000000 blockchain-apis-0.1.2/src/blockchainapis/exceptions/TooManyRequestsException.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      691 2023-06-09 15:18:43.000000 blockchain-apis-0.1.2/src/blockchainapis/exceptions/UnauthorizedException.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      922 2023-06-09 15:18:43.000000 blockchain-apis-0.1.2/src/blockchainapis/exceptions/__init__.py
+drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-06-09 15:30:14.941298 blockchain-apis-0.1.2/src/blockchainapis/models/
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      859 2023-06-09 15:18:43.000000 blockchain-apis-0.1.2/src/blockchainapis/models/AmountIn.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      870 2023-06-09 15:18:43.000000 blockchain-apis-0.1.2/src/blockchainapis/models/AmountOut.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      579 2023-06-09 15:18:43.000000 blockchain-apis-0.1.2/src/blockchainapis/models/Blockchain.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      547 2023-06-09 15:18:43.000000 blockchain-apis-0.1.2/src/blockchainapis/models/Exchange.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      863 2023-06-09 15:18:43.000000 blockchain-apis-0.1.2/src/blockchainapis/models/Exchanges.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      677 2023-06-09 15:18:43.000000 blockchain-apis-0.1.2/src/blockchainapis/models/Pair.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      933 2023-06-09 15:18:43.000000 blockchain-apis-0.1.2/src/blockchainapis/models/Pairs.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      794 2023-06-09 15:18:43.000000 blockchain-apis-0.1.2/src/blockchainapis/models/Reserve.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      760 2023-06-09 15:18:43.000000 blockchain-apis-0.1.2/src/blockchainapis/models/Token.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1826 2023-06-09 15:18:43.000000 blockchain-apis-0.1.2/src/blockchainapis/models/Tokens.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1475 2023-06-09 15:18:43.000000 blockchain-apis-0.1.2/src/blockchainapis/models/__init__.py
+drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-06-09 15:30:14.941298 blockchain-apis-0.1.2/tests/
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1564 2023-06-09 15:18:43.000000 blockchain-apis-0.1.2/tests/test_amount_in.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1540 2023-06-09 15:18:43.000000 blockchain-apis-0.1.2/tests/test_amount_in_sync.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1568 2023-06-09 15:18:43.000000 blockchain-apis-0.1.2/tests/test_amount_out.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1544 2023-06-09 15:18:43.000000 blockchain-apis-0.1.2/tests/test_amount_out_sync.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      425 2023-06-09 15:18:43.000000 blockchain-apis-0.1.2/tests/test_blockchains.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      419 2023-06-09 15:18:43.000000 blockchain-apis-0.1.2/tests/test_blockchains_sync.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      569 2023-06-09 15:18:43.000000 blockchain-apis-0.1.2/tests/test_decimals.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      563 2023-06-09 15:18:43.000000 blockchain-apis-0.1.2/tests/test_decimals_sync.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1291 2023-06-09 15:18:43.000000 blockchain-apis-0.1.2/tests/test_exchanges.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1231 2023-06-09 15:18:43.000000 blockchain-apis-0.1.2/tests/test_exchanges_sync.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      593 2023-06-09 15:18:43.000000 blockchain-apis-0.1.2/tests/test_info.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      587 2023-06-09 15:18:43.000000 blockchain-apis-0.1.2/tests/test_info_sync.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2699 2023-06-09 15:18:43.000000 blockchain-apis-0.1.2/tests/test_pairs.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2567 2023-06-09 15:18:43.000000 blockchain-apis-0.1.2/tests/test_pairs_sync.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1392 2023-06-09 15:18:43.000000 blockchain-apis-0.1.2/tests/test_reserves.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1368 2023-06-09 15:18:43.000000 blockchain-apis-0.1.2/tests/test_reserves_sync.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1249 2023-06-09 15:18:43.000000 blockchain-apis-0.1.2/tests/test_tokens.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1189 2023-06-09 15:18:43.000000 blockchain-apis-0.1.2/tests/test_tokens_sync.py
```

### Comparing `blockchain-apis-0.1.1/LICENSE` & `blockchain-apis-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.1/PKG-INFO` & `blockchain-apis-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blockchain-apis
-Version: 0.1.1
+Version: 0.1.2
 Summary: Fastest and easiest way to access decentralized finance data
 Home-page: https://www.blockchainapis.io
 Author: Clarensia
 Author-email: contact@blockchainapis.io
 License: MIT
 Project-URL: Documentation, https://api.blockchainapis.io/docs
 Project-URL: Source, https://github.com/blockchainapis/blockchain-apis-python-client
```

### Comparing `blockchain-apis-0.1.1/README.md` & `blockchain-apis-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.1/setup.py` & `blockchain-apis-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
     
 setup(
     name = "blockchain-apis",
-    version = "0.1.1",
+    version = "0.1.2",
     author = "Clarensia",
     author_email = "contact@blockchainapis.io",
     description = "Fastest and easiest way to access decentralized finance data",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://www.blockchainapis.io",
     license="MIT",
```

### Comparing `blockchain-apis-0.1.1/src/blockchain_apis.egg-info/PKG-INFO` & `blockchain-apis-0.1.2/src/blockchain_apis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blockchain-apis
-Version: 0.1.1
+Version: 0.1.2
 Summary: Fastest and easiest way to access decentralized finance data
 Home-page: https://www.blockchainapis.io
 Author: Clarensia
 Author-email: contact@blockchainapis.io
 License: MIT
 Project-URL: Documentation, https://api.blockchainapis.io/docs
 Project-URL: Source, https://github.com/blockchainapis/blockchain-apis-python-client
```

### Comparing `blockchain-apis-0.1.1/src/blockchain_apis.egg-info/SOURCES.txt` & `blockchain-apis-0.1.2/src/blockchain_apis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.1/src/blockchainapis/BlockchainAPIs.py` & `blockchain-apis-0.1.2/src/blockchainapis/BlockchainAPIsSync.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from typing import Any, Dict, List
+import requests
 
-from aiohttp import ClientSession
+from typing import Any, Dict, List
+from urllib.parse import urljoin
 
 from .models import Blockchain
 from .models import Exchanges
 from .models import Exchange
 from .models import Pairs
 from .models import Pair
 from .models import Reserve
@@ -18,106 +19,95 @@
 from .exceptions import InvalidPageException
 from .exceptions import TokenNotFoundException
 from .exceptions import PairNotFoundException
 from .exceptions import TooManyRequestsException
 from .exceptions import UnauthorizedException
 
 
-class BlockchainAPIs:
+class BlockchainAPIsSync:
     """High-frequency DEX API
 
-        
-    Our API empowers you to access live financial data across multiple blockchains (currently supporting 6, with more on the way)
-    with unparalleled speed and efficiency.
+    Our API empowers you to access live financial data across multiple blockchains
+    (currently supporting 6, with more on the way) with unparalleled speed and efficiency.
     
-    What sets our API apart? We've optimized performance to deliver an impressive 1000+ calls per second per user, with a
-    lightning-fast processing time of less than 2 millisecond per request. Compare that to other solutions with a 20-millisecond
-    processing time and fewer requests per second, and it's clear why developers choose our API for their trading bots.
+    What sets our API apart? We've optimized performance to deliver an impressive 1000+
+    calls per second per user, with a lightning-fast processing time of less than 2 millisecond
+    per request. Compare that to other solutions with a 20-millisecond processing time and fewer
+    requests per second, and it's clear why developers choose our API for their trading bots.
     
-    Another game-changing feature is our seamless integration across various blockchains and protocols. With our API, you can reuse
-    the same code without changing a single line, simplifying the development process and saving you valuable time.
+    Another game-changing feature is our seamless integration across various blockchains and
+    protocols. With our API, you can reuse the same code without changing a single line, simplifying
+    the development process and saving you valuable time.
     
-    Ready to try it out? [Sign up for a free API key here](https://dashboard.blockchainapis.io) or start exploring the possibilities
-    on this page. Need support or have questions? Join our [Discord community](https://discord.gg/GphRMJXmS5) where our team and
-    fellow developers are eager to help you make the most of our powerful API.
-    """
+    Ready to try it out? [Sign up for a free API key here](https://dashboard.blockchainapis.io)
+    or start exploring the possibilities on this page. Need support or have questions? Join our
+    [Discord community](https://discord.gg/GphRMJXmS5) where our team and fellow developers are
+    eager to help you make the most of our powerful API.
 
-    _session: ClientSession
-    """The session that is used by async operation.
-    
-    This session must be closed at the end of your program or usage of the API.
-    
-    It can be closed with:
-    await blockchain_apis_instance.close()
-    
-    (replace blockchain_apis_instance with your instance of BlockchainAPIs)
+    Please note that this class is not async which is less optimized. To run more otpimized
+    requests, please use: BlockchainAPIs
     """
     
     def __init__(self, api_key: str | None = None):
-        """Creates a BlockchainAPIs async instance that allow you to make API calls.
+        """Creates a BlockchainAPIsSync sync instance that allow you to make API calls
+        in a synchronous way.
 
         The client works without an API key, but for better performance, we advise you
         to get one at: https://dashboard.blockchainapis.io
 
         :param api_key: Your API key, defaults to None
         :type api_key: str | None, optional
         """
-        self._api_key = api_key
         self._headers = {
             "accept": "application/json"
         }
         if api_key is not None:
             self._headers["api-key"] = api_key
-        self._session = ClientSession("https://api.blockchainapis.io")
+        self._base_url = "https://api.blockchainapis.io"
 
-    async def close(self):
-        """Close the async session object.
-        
-        You must call this method at the end of your program or when you have finished
-        working with BlockchainAPIs.
-        """
-        await self._session.close()
 
-    async def _do_request(self, path: str, params: Dict[str, Any] | None = None) -> Dict[str, Any]:
-        """Make raw API request (that return the json result).
+    def _do_request(self, path: str, params: Dict[str, Any] | None = None) -> Dict[str, Any]:
+        """Make a raw API request (that return the json result).
         
-        This method additionaly adds the user API key to the request if it is present.
+        It makes the request in a synchronous way and you don't need to close the
+        BlockchainAPIs instance.
 
-        :param path: The path to the request
+        :param path: The path of the request
         :type path: str
         :param params: The optional query parameters of the request, defaults to None
         :type params: Dict[str, Any] | None, optional
         :return: The json-formated result
-        :rtype: Dict[str, None]
+        :rtype: Dict[str, Any]
         """
-        async with self._session.get(path, params=params, headers=self._headers) as response:
-            if response.status != 200:
-                error_data = await response.json()
-                error_type = error_data["detail"]["error_type"]
-                match error_type:
-                    case "BlockchainNotSupportedException":
-                        raise BlockchainNotSupportedException(response.status, error_data["detail"]["detail"])
-                    case "ExchangeNotSupportedException":
-                        raise ExchangeNotSupportedException(response.status, error_data["detail"]["detail"])
-                    case "InvalidPageException":
-                        raise InvalidPageException(response.status, error_data["detail"]["detail"])
-                    case "TokenNotFoundException":
-                        raise TokenNotFoundException(response.status, error_data["detail"]["detail"])
-                    case "PairNotFoundException":
-                        raise PairNotFoundException(response.status, error_data["detail"]["detail"])
-                    case "TooManyRequestException":
-                        raise TooManyRequestsException(response.status, error_data["detail"]["detail"])
-                    case "UnauthorizedException":
-                        raise UnauthorizedException(response.status, error_data["detail"]["detail"])
-                    case unknown:
-                        raise Exception(f"Unkwnown Exception type: {unknown}.\nGot this exception while handling:\n{error_data} with status code: {response.status}")
+        url = urljoin(self._base_url, path)
+        response = requests.get(url, params=params, headers=self._headers)
+        if response.status_code != 200:
+            error_data = response.json()
+            error_type = error_data["detail"]["error_type"]
+            match error_type:
+                case "BlockchainNotSupportedException":
+                    raise BlockchainNotSupportedException(response.status, error_data["detail"]["detail"])
+                case "ExchangeNotSupportedException":
+                    raise ExchangeNotSupportedException(response.status, error_data["detail"]["detail"])
+                case "InvalidPageException":
+                    raise InvalidPageException(response.status, error_data["detail"]["detail"])
+                case "TokenNotFoundException":
+                    raise TokenNotFoundException(response.status, error_data["detail"]["detail"])
+                case "PairNotFoundException":
+                    raise PairNotFoundException(response.status, error_data["detail"]["detail"])
+                case "TooManyRequestsException":
+                    raise TooManyRequestsException(response.status, error_data["detail"]["detail"])
+                case "UnauthorizedException":
+                    raise UnauthorizedException(response.status, error_data["detail"]["detail"])
+                case unknown:
+                    raise Exception(f"Unkwnown Exception type: {unknown}.\nGot this exception while handling:\n{error_data} with status code: {response.status}")
 
-            return await response.json()
+        return response.json()
 
-    async def blockchains(self) -> List[Blockchain]:
+    def blockchains(self) -> List[Blockchain]:
         """Get the list of blockchains supported by the API
 
 
         :return: The list of the blockchains supported by the API.
         
         Using this method, you can find the id of the blockchain that you can use for
         other function calls.
@@ -133,36 +123,37 @@
                 "explorer": "https://snowtrace.io/"
             }
 
         ]
         ```
         :rtype: List[Blockchain]
         """
-        ret = await self._do_request("/v0/blockchains/")
+        ret = self._do_request("/v0/blockchains/")
         return [
             Blockchain(
                 blockchain=r["blockchain"],
                 name=r["name"],
                 chain_id=r["chain_id"],
                 explorer=r["explorer"]
             )
             for r in ret
         ]
 
-
-    async def exchanges(self, page: int = 1, blockchain: str | None = None) -> Exchanges:
+    def exchanges(self, page: int = 1, blockchain: str | None = None) -> Exchanges:
         """Get the list of supported exchanges by the API
 
-        @raises BlockchainNotSupportedException: When an invalid blockchain id is given
-        @raises InvalidPageException: When an invalid page is given
+        :raises BlockchainNotSupportedException: When an invalid blockchain id is given
+        :raises InvalidPageException: When an invalid page is given
 
         :param page: You can ignore this value for this version of the API., defaults to 1
         :type page: int, Optional
+        :example page: 1
         :param blockchain: The blockchain from which you want to get the exchanges, defaults to None
         :type blockchain: str, Optional
+        :example blockchain: ethereum
         :return: The list of all supported exchange of the API.
         
         You can use the exchange id responded from this for other API calls.
 
 
         Example response:
         ```json
@@ -190,37 +181,37 @@
         ```
         :rtype: Exchanges
         """
         params = {}
         params["page"] = page
         if blockchain is not None:
             params["blockchain"] = blockchain
-        ret = await self._do_request("/v0/exchanges/", params)
+        ret = self._do_request("/v0/exchanges/", params)
         return Exchanges(
             page=ret["page"],
             total_pages=ret["total_pages"],
             data=[
                 Exchange(
                     exchange=d["exchange"],
                     blockchain=d["blockchain"],
                     name=d["name"],
                     url=d["url"]
                 )
                 for d in ret["data"]
             ]
         )
 
-
-    async def info(self, exchange: str) -> Exchange:
+    def info(self, exchange: str) -> Exchange:
         """Get informations on a specific exchange
 
-        @raises ExchangeNotSupportedException: Thrown when an invalid exchange id is given
+        :raises ExchangeNotSupportedException: Thrown when an invalid exchange id is given
 
         :param exchange: The exchange to get the informations from
         :type exchange: str
+        :example exchange: uniswapv2_ethereum
         :return: Information on a specific exchange.
         
         These informations includes:
         - The blockchain id of the exchange
         - The id of the exchange
         - The name of the exchange
         - The url to access the exchange
@@ -237,36 +228,38 @@
         }
 
         ```
         :rtype: Exchange
         """
         params = {}
         params["exchange"] = exchange
-        ret = await self._do_request("/v0/exchanges/info", params)
+        ret = self._do_request("/v0/exchanges/info", params)
         return Exchange(
             exchange=ret["exchange"],
             blockchain=ret["blockchain"],
             name=ret["name"],
             url=ret["url"]
         )
 
-
-    async def pairs(self, page: int = 1, blockchain: str | None = None, exchange: str | None = None) -> Pairs:
+    def pairs(self, page: int = 1, blockchain: str | None = None, exchange: str | None = None) -> Pairs:
         """Get the list of pairs supported by the API
 
-        @raises BlockchainNotSupportedException: When an invalid blockchain id is given
-        @raises ExchangeNotSupportedException: When an invalid Exchange id is given
-        @raises InvalidPageException: When you give an invalid page number
+        :raises BlockchainNotSupportedException: When an invalid blockchain id is given
+        :raises ExchangeNotSupportedException: When an invalid Exchange id is given
+        :raises InvalidPageException: When you give an invalid page number
 
         :param page: Each request has a maximum of 100 results separated by page, defaults to 1
         :type page: int, Optional
+        :example page: 1
         :param blockchain: The blockchain from which you want to get the pairs, defaults to None
         :type blockchain: str, Optional
+        :example blockchain: ethereum
         :param exchange: The exchange from which you want to get the pairs, defaults to None
         :type exchange: str, Optional
+        :example exchange: uniswapv2_ethereum
         :return: The list of pairs supported by the API. It returns token addresses,
         blockchain, exchange and the fee that the pair has.
         
         The fee may vary depending on the exchange used.
 
 
         Example response:
@@ -297,15 +290,15 @@
         """
         params = {}
         params["page"] = page
         if blockchain is not None:
             params["blockchain"] = blockchain
         if exchange is not None:
             params["exchange"] = exchange
-        ret = await self._do_request("/v0/exchanges/pairs", params)
+        ret = self._do_request("/v0/exchanges/pairs", params)
         return Pairs(
             page=ret["page"],
             total_pages=ret["total_pages"],
             data=[
                 Pair(
                     blockchain=d["blockchain"],
                     exchange=d["exchange"],
@@ -313,30 +306,33 @@
                     token1=d["token1"],
                     fee=d["fee"]
                 )
                 for d in ret["data"]
             ]
         )
 
-
-    async def reserves(self, blockchain: str, token0: str, token1: str, exchange: str | None = None) -> List[Reserve]:
+    def reserves(self, blockchain: str, token0: str, token1: str, exchange: str | None = None) -> List[Reserve]:
         """Get the liquidity inside of the reserve of two tokens.
 
-        @raises BlockchainNotSupportedException: When an invalid blockchain id is given
-        @raises ExchangeNotSupportedException: When an invalid exchange id is given
-        @raises PairNotFoundException: When a pair is not found for the given blockchain or exchange
+        :raises BlockchainNotSupportedException: When an invalid blockchain id is given
+        :raises ExchangeNotSupportedException: When an invalid exchange id is given
+        :raises PairNotFoundException: When a pair is not found for the given blockchain or exchange
 
         :param blockchain: The id of the blockchain on which the exchange will happen. It is required because some tokens can have same address accross multiple blockchains
         :type blockchain: str
+        :example blockchain: ethereum
         :param token0: The address of the first token of the pair
         :type token0: str
+        :example token0: 0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2
         :param token1: The address of the second token of the pair
         :type token1: str
+        :example token1: 0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48
         :param exchange: The id of the exchange from which you want to get the reserve, defaults to None
         :type exchange: str, Optional
+        :example exchange: uniswapv2_ethereum
         :return: The list of all of the reserve for the given pair, blockchain and exchange.
         Can return an empty list if the given pair was not found.
 
 
         Example response:
         ```json
         [
@@ -355,45 +351,49 @@
         """
         params = {}
         params["blockchain"] = blockchain
         if exchange is not None:
             params["exchange"] = exchange
         params["token0"] = token0
         params["token1"] = token1
-        ret = await self._do_request("/v0/exchanges/pairs/reserves", params)
+        ret = self._do_request("/v0/exchanges/pairs/reserves", params)
         return [
             Reserve(
                 blockchain=r["blockchain"],
                 exchange=r["exchange"],
                 token0=r["token0"],
                 token1=r["token1"],
                 reserve0=r["reserve0"],
                 reserve1=r["reserve1"]
             )
             for r in ret
         ]
 
+    def amount_out(self, blockchain: str, tokenIn: str, tokenOut: str, amountIn: int, exchange: str | None = None) -> List[AmountOut]:
+        """Get the amount of tokenOut that you will get after selling amountIn tokenIn
 
-    async def amount_out(self, blockchain: str, tokenIn: str, tokenOut: str, amountIn: int, exchange: str | None = None) -> List[AmountOut]:
-        """Get the amount of token1 that you will get after selling amountIn token0
-
-        @raises BlockchainNotSupportedException: When an invalid blockchain id is given
-        @raises ExchangeNotSupportedException: When an invalid exchange id is given
-        @raises PairNotFoundException: When a pair is not found for the given blockchain or exchange
+        :raises BlockchainNotSupportedException: When an invalid blockchain id is given
+        :raises ExchangeNotSupportedException: When an invalid exchange id is given
+        :raises PairNotFoundException: When a pair is not found for the given blockchain or exchange
 
         :param blockchain: The id of the blockchain on which this exchange take place
         :type blockchain: str
+        :example blockchain: ethereum
         :param tokenIn: The address of the token that you sell
         :type tokenIn: str
+        :example tokenIn: 0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2
         :param tokenOut: The address of the token that you buy
         :type tokenOut: str
-        :param amountIn: The amount of token0 that you sell
+        :example tokenOut: 0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48
+        :param amountIn: The amount of tokenIn that you sell
         :type amountIn: int
+        :example amountIn: 1000000000000000000
         :param exchange: The exchange on which you want to do the trade, defaults to None
         :type exchange: str, Optional
+        :example exchange: uniswapv2_ethereum
         :return: The list of the amount out that you will get on all of the exchanges. It can return an empty list if the given pair was not found for the given parameters.
 
 
         Example response:
         ```json
         [
             {
@@ -412,45 +412,49 @@
         params = {}
         params["blockchain"] = blockchain
         params["tokenIn"] = tokenIn
         params["tokenOut"] = tokenOut
         params["amountIn"] = amountIn
         if exchange is not None:
             params["exchange"] = exchange
-        ret = await self._do_request("/v0/exchanges/pairs/amountOut", params)
+        ret = self._do_request("/v0/exchanges/pairs/amountOut", params)
         return [
             AmountOut(
                 blockchain=r["blockchain"],
                 exchange=r["exchange"],
                 tokenIn=r["tokenIn"],
                 tokenOut=r["tokenOut"],
                 amountIn=r["amountIn"],
                 amountOut=r["amountOut"]
             )
             for r in ret
         ]
 
+    def amount_in(self, blockchain: str, tokenIn: str, tokenOut: str, amountOut: int, exchange: str | None = None) -> List[AmountIn]:
+        """Get the amount of tokenIn that you need to sell in order to get amountOut tokenOut
 
-    async def amount_in(self, blockchain: str, tokenIn: str, tokenOut: str, amountOut: int, exchange: str | None = None) -> List[AmountIn]:
-        """Get the amount of token0 that you need to sell in order to get amountIn token1
-
-        @raises BlockchainNotSupportedException: When an invalid blockchain id is given
-        @raises ExchangeNotSupportedException: When an invalid exchange id is given
-        @raises PairNotFoundException: When a pair is not found for the given blockchain or exchange
+        :raises BlockchainNotSupportedException: When an invalid blockchain id is given
+        :raises ExchangeNotSupportedException: When an invalid exchange id is given
+        :raises PairNotFoundException: When a pair is not found for the given blockchain or exchange
 
         :param blockchain: The id of the blockchain on which this exchange take place
         :type blockchain: str
+        :example blockchain: ethereum
         :param tokenIn: The address of the token that you sell
         :type tokenIn: str
+        :example tokenIn: 0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48
         :param tokenOut: The address of the token that you buy
         :type tokenOut: str
-        :param amountOut: The amount of token1 that you are trying to get
+        :example tokenOut: 0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2
+        :param amountOut: The amount of tokenOut that you are trying to get
         :type amountOut: int
+        :example amountOut: 1000000000000000000
         :param exchange: The exchange on which you want to do the trade, defaults to None
         :type exchange: str, Optional
+        :example exchange: uniswapv2_ethereum
         :return: The list of amount in that you will get on all of the exchanges. It can return an empty list if the given pair was not found.
 
 
         Example response:
         ```json
         [
             {
@@ -469,38 +473,39 @@
         params = {}
         params["blockchain"] = blockchain
         params["tokenIn"] = tokenIn
         params["tokenOut"] = tokenOut
         params["amountOut"] = amountOut
         if exchange is not None:
             params["exchange"] = exchange
-        ret = await self._do_request("/v0/exchanges/pairs/amountIn", params)
+        ret = self._do_request("/v0/exchanges/pairs/amountIn", params)
         return [
             AmountIn(
                 blockchain=r["blockchain"],
                 exchange=r["exchange"],
                 tokenIn=r["tokenIn"],
                 tokenOut=r["tokenOut"],
                 amountIn=r["amountIn"],
                 amountOut=r["amountOut"]
             )
             for r in ret
         ]
 
-
-    async def tokens(self, page: int = 1, blockchain: str | None = None) -> Tokens:
+    def tokens(self, page: int = 1, blockchain: str | None = None) -> Tokens:
         """Get the list of supported tokens
 
-        @raises BlockchainNotSupportedException: When an invalid blockchain id is given
-        @raises InvalidPageException: When an invalid page number is given
+        :raises BlockchainNotSupportedException: When an invalid blockchain id is given
+        :raises InvalidPageException: When an invalid page number is given
 
         :param page: Each request have a limit of 100 data separated per pages, defaults to 1
         :type page: int, Optional
+        :example page: 1
         :param blockchain: The blockchain on which you want to get the tokens, defaults to None
         :type blockchain: str, Optional
+        :example blockchain: ethereum
         :return: The list of supported tokens ordered by market cap in a descending order.
         
         The market capitalization is in dollars, it can be null if the liquidity available for the given token is lower than 1000$.
         The market capitalization is based on USDT.
         
         The market capitalization of each token is computed as follow:
         average worth of token in liquidity pools * total token supply
@@ -560,40 +565,41 @@
         ```
         :rtype: Tokens
         """
         params = {}
         params["page"] = page
         if blockchain is not None:
             params["blockchain"] = blockchain
-        ret = await self._do_request("/v0/tokens/", params)
+        ret = self._do_request("/v0/tokens/", params)
         return Tokens(
             page=ret["page"],
             total_pages=ret["total_pages"],
             data=[
                 Token(
                     blockchain=d["blockchain"],
                     address=d["address"],
                     decimals=d["decimals"],
                     market_cap=d["market_cap"]
                 )
                 for d in ret["data"]
             ]
         )
 
-
-    async def info(self, blockchain: str, token: str) -> Token:
+    def info(self, blockchain: str, token: str) -> Token:
         """Get information on a specific token
 
-        @raises BlockchainNotSupportedException: When an invalid blockchain id is given
-        @raises TokenNotFoundException: When the given token is not found
+        :raises BlockchainNotSupportedException: When an invalid blockchain id is given
+        :raises TokenNotFoundException: When the given token is not found
 
         :param blockchain: The blockchain on which you want to get the information of the token
         :type blockchain: str
+        :example blockchain: ethereum
         :param token: The address of the token that you want to get the informations from
         :type token: str
+        :example token: 0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2
         :return: Informations on a specific token.
         
         This information includes:
         - The id of the blockchain that this token is
         - The address of the token
         - The decimals of it
         - The market cap
@@ -610,40 +616,40 @@
 
         ```
         :rtype: Token
         """
         params = {}
         params["blockchain"] = blockchain
         params["token"] = token
-        ret = await self._do_request("/v0/tokens/info", params)
+        ret = self._do_request("/v0/tokens/info", params)
         return Token(
             blockchain=ret["blockchain"],
             address=ret["address"],
             decimals=ret["decimals"],
             market_cap=ret["market_cap"]
         )
 
-
-    async def decimals(self, blockchain: str, token: str) -> int:
+    def decimals(self, blockchain: str, token: str) -> int:
         """Get the decimals of the given token
 
-        @raises HTTPValidationError: Validation Error
+        :raises HTTPValidationError: Validation Error
 
         :param blockchain: The id of the blockchain of the token
         :type blockchain: str
+        :example blockchain: ethereum
         :param token: The address of the token that you want to get the decimals from
         :type token: str
+        :example token: 0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2
         :return: The decimals of the specific token
 
 
         Example response:
         ```json
         16
         ```
         :rtype: int
         """
         params = {}
         params["blockchain"] = blockchain
         params["token"] = token
-        ret = await self._do_request("/v0/tokens/decimals", params)
+        ret = self._do_request("/v0/tokens/decimals", params)
         return int(ret)
-
```

### Comparing `blockchain-apis-0.1.1/src/blockchainapis/BlockchainAPIsSync.py` & `blockchain-apis-0.1.2/src/blockchainapis/BlockchainAPIs.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-import requests
-
 from typing import Any, Dict, List
-from urllib.parse import urljoin
+
+from aiohttp import ClientSession
 
 from .models import Blockchain
 from .models import Exchanges
 from .models import Exchange
 from .models import Pairs
 from .models import Pair
 from .models import Reserve
@@ -19,92 +18,108 @@
 from .exceptions import InvalidPageException
 from .exceptions import TokenNotFoundException
 from .exceptions import PairNotFoundException
 from .exceptions import TooManyRequestsException
 from .exceptions import UnauthorizedException
 
 
-class BlockchainAPIsSync:
+class BlockchainAPIs:
     """High-frequency DEX API
 
-    Our API empowers you to access live financial data across multiple blockchains (currently supporting 6, with more on the way)
-    with unparalleled speed and efficiency.
+    Our API empowers you to access live financial data across multiple blockchains
+    (currently supporting 6, with more on the way) with unparalleled speed and efficiency.
     
-    What sets our API apart? We've optimized performance to deliver an impressive 1000+ calls per second per user, with a
-    lightning-fast processing time of less than 2 millisecond per request. Compare that to other solutions with a 20-millisecond
-    processing time and fewer requests per second, and it's clear why developers choose our API for their trading bots.
+    What sets our API apart? We've optimized performance to deliver an impressive 1000+
+    calls per second per user, with a lightning-fast processing time of less than 2 millisecond
+    per request. Compare that to other solutions with a 20-millisecond processing time and fewer
+    requests per second, and it's clear why developers choose our API for their trading bots.
     
-    Another game-changing feature is our seamless integration across various blockchains and protocols. With our API, you can reuse
-    the same code without changing a single line, simplifying the development process and saving you valuable time.
+    Another game-changing feature is our seamless integration across various blockchains and
+    protocols. With our API, you can reuse the same code without changing a single line, simplifying
+    the development process and saving you valuable time.
     
-    Ready to try it out? [Sign up for a free API key here](https://dashboard.blockchainapis.io) or start exploring the possibilities
-    on this page. Need support or have questions? Join our [Discord community](https://discord.gg/GphRMJXmS5) where our team and
-    fellow developers are eager to help you make the most of our powerful API.
+    Ready to try it out? [Sign up for a free API key here](https://dashboard.blockchainapis.io)
+    or start exploring the possibilities on this page. Need support or have questions? Join our
+    [Discord community](https://discord.gg/GphRMJXmS5) where our team and fellow developers are
+    eager to help you make the most of our powerful API.
+    """
 
-    Please note that this class is using sync which is less optimized. To run more otpimized requests and take advantage of
-    modern async Python, please use: BlockchainAPIs
+    _session: ClientSession
+    """The session that is used by async operation.
+    
+    This session must be closed at the end of your program or usage of the API.
+    
+    It can be closed with:
+    await blockchain_apis_instance.close()
+    
+    (replace blockchain_apis_instance with your instance of BlockchainAPIs)
     """
     
     def __init__(self, api_key: str | None = None):
-        """Creates a BlockchainAPIsSync sync instance that allow you to make API calls
-        in a synchronous way.
+        """Creates a BlockchainAPIs async instance that allow you to make API calls.
 
         The client works without an API key, but for better performance, we advise you
         to get one at: https://dashboard.blockchainapis.io
 
         :param api_key: Your API key, defaults to None
         :type api_key: str | None, optional
         """
+        self._api_key = api_key
         self._headers = {
             "accept": "application/json"
         }
         if api_key is not None:
             self._headers["api-key"] = api_key
-        self._base_url = "https://api.blockchainapis.io"
+        self._session = ClientSession("https://api.blockchainapis.io")
 
+    async def close(self):
+        """Close the async session object.
+        
+        You must call this method at the end of your program or when you have finished
+        working with BlockchainAPIs.
+        """
+        await self._session.close()
 
-    def _do_request(self, path: str, params: Dict[str, Any] | None = None) -> Dict[str, Any]:
-        """Make a raw API request (that return the json result).
+    async def _do_request(self, path: str, params: Dict[str, Any] | None = None) -> Dict[str, Any]:
+        """Make raw API request (that return the json result).
         
-        It makes the request in a synchronous way and you don't need to close the
-        BlockchainAPIs instance.
+        This method additionaly adds the user API key to the request if it is present.
 
-        :param path: The path of the request
+        :param path: The path to the request
         :type path: str
         :param params: The optional query parameters of the request, defaults to None
         :type params: Dict[str, Any] | None, optional
         :return: The json-formated result
-        :rtype: Dict[str, Any]
+        :rtype: Dict[str, None]
         """
-        url = urljoin(self._base_url, path)
-        response = requests.get(url, params=params, headers=self._headers)
-        if response.status_code != 200:
-            error_data = response.json()
-            error_type = error_data["detail"]["error_type"]
-            match error_type:
-                case "BlockchainNotSupportedException":
-                    raise BlockchainNotSupportedException(response.status, error_data["detail"]["detail"])
-                case "ExchangeNotSupportedException":
-                    raise ExchangeNotSupportedException(response.status, error_data["detail"]["detail"])
-                case "InvalidPageException":
-                    raise InvalidPageException(response.status, error_data["detail"]["detail"])
-                case "TokenNotFoundException":
-                    raise TokenNotFoundException(response.status, error_data["detail"]["detail"])
-                case "PairNotFoundException":
-                    raise PairNotFoundException(response.status, error_data["detail"]["detail"])
-                case "TooManyRequestException":
-                    raise TooManyRequestsException(response.status, error_data["detail"]["detail"])
-                case "UnauthorizedException":
-                    raise UnauthorizedException(response.status, error_data["detail"]["detail"])
-                case unknown:
-                    raise Exception(f"Unkwnown Exception type: {unknown}.\nGot this exception while handling:\n{error_data} with status code: {response.status}")
+        async with self._session.get(path, params=params, headers=self._headers) as response:
+            if response.status != 200:
+                error_data = await response.json()
+                error_type = error_data["detail"]["error_type"]
+                match error_type:
+                    case "BlockchainNotSupportedException":
+                        raise BlockchainNotSupportedException(response.status, error_data["detail"]["detail"])
+                    case "ExchangeNotSupportedException":
+                        raise ExchangeNotSupportedException(response.status, error_data["detail"]["detail"])
+                    case "InvalidPageException":
+                        raise InvalidPageException(response.status, error_data["detail"]["detail"])
+                    case "TokenNotFoundException":
+                        raise TokenNotFoundException(response.status, error_data["detail"]["detail"])
+                    case "PairNotFoundException":
+                        raise PairNotFoundException(response.status, error_data["detail"]["detail"])
+                    case "TooManyRequestsException":
+                        raise TooManyRequestsException(response.status, error_data["detail"]["detail"])
+                    case "UnauthorizedException":
+                        raise UnauthorizedException(response.status, error_data["detail"]["detail"])
+                    case unknown:
+                        raise Exception(f"Unkwnown Exception type: {unknown}.\nGot this exception while handling:\n{error_data} with status code: {response.status}")
 
-        return response.json()
+            return await response.json()
 
-    def blockchains(self) -> List[Blockchain]:
+    async def blockchains(self) -> List[Blockchain]:
         """Get the list of blockchains supported by the API
 
 
         :return: The list of the blockchains supported by the API.
         
         Using this method, you can find the id of the blockchain that you can use for
         other function calls.
@@ -120,36 +135,37 @@
                 "explorer": "https://snowtrace.io/"
             }
 
         ]
         ```
         :rtype: List[Blockchain]
         """
-        ret = self._do_request("/v0/blockchains/")
+        ret = await self._do_request("/v0/blockchains/")
         return [
             Blockchain(
                 blockchain=r["blockchain"],
                 name=r["name"],
                 chain_id=r["chain_id"],
                 explorer=r["explorer"]
             )
             for r in ret
         ]
 
-
-    def exchanges(self, page: int = 1, blockchain: str | None = None) -> Exchanges:
+    async def exchanges(self, page: int = 1, blockchain: str | None = None) -> Exchanges:
         """Get the list of supported exchanges by the API
 
-        @raises BlockchainNotSupportedException: When an invalid blockchain id is given
-        @raises InvalidPageException: When an invalid page is given
+        :raises BlockchainNotSupportedException: When an invalid blockchain id is given
+        :raises InvalidPageException: When an invalid page is given
 
         :param page: You can ignore this value for this version of the API., defaults to 1
         :type page: int, Optional
+        :example page: 1
         :param blockchain: The blockchain from which you want to get the exchanges, defaults to None
         :type blockchain: str, Optional
+        :example blockchain: ethereum
         :return: The list of all supported exchange of the API.
         
         You can use the exchange id responded from this for other API calls.
 
 
         Example response:
         ```json
@@ -177,37 +193,37 @@
         ```
         :rtype: Exchanges
         """
         params = {}
         params["page"] = page
         if blockchain is not None:
             params["blockchain"] = blockchain
-        ret = self._do_request("/v0/exchanges/", params)
+        ret = await self._do_request("/v0/exchanges/", params)
         return Exchanges(
             page=ret["page"],
             total_pages=ret["total_pages"],
             data=[
                 Exchange(
                     exchange=d["exchange"],
                     blockchain=d["blockchain"],
                     name=d["name"],
                     url=d["url"]
                 )
                 for d in ret["data"]
             ]
         )
 
-
-    def info(self, exchange: str) -> Exchange:
+    async def info(self, exchange: str) -> Exchange:
         """Get informations on a specific exchange
 
-        @raises ExchangeNotSupportedException: Thrown when an invalid exchange id is given
+        :raises ExchangeNotSupportedException: Thrown when an invalid exchange id is given
 
         :param exchange: The exchange to get the informations from
         :type exchange: str
+        :example exchange: uniswapv2_ethereum
         :return: Information on a specific exchange.
         
         These informations includes:
         - The blockchain id of the exchange
         - The id of the exchange
         - The name of the exchange
         - The url to access the exchange
@@ -224,36 +240,38 @@
         }
 
         ```
         :rtype: Exchange
         """
         params = {}
         params["exchange"] = exchange
-        ret = self._do_request("/v0/exchanges/info", params)
+        ret = await self._do_request("/v0/exchanges/info", params)
         return Exchange(
             exchange=ret["exchange"],
             blockchain=ret["blockchain"],
             name=ret["name"],
             url=ret["url"]
         )
 
-
-    def pairs(self, page: int = 1, blockchain: str | None = None, exchange: str | None = None) -> Pairs:
+    async def pairs(self, page: int = 1, blockchain: str | None = None, exchange: str | None = None) -> Pairs:
         """Get the list of pairs supported by the API
 
-        @raises BlockchainNotSupportedException: When an invalid blockchain id is given
-        @raises ExchangeNotSupportedException: When an invalid Exchange id is given
-        @raises InvalidPageException: When you give an invalid page number
+        :raises BlockchainNotSupportedException: When an invalid blockchain id is given
+        :raises ExchangeNotSupportedException: When an invalid Exchange id is given
+        :raises InvalidPageException: When you give an invalid page number
 
         :param page: Each request has a maximum of 100 results separated by page, defaults to 1
         :type page: int, Optional
+        :example page: 1
         :param blockchain: The blockchain from which you want to get the pairs, defaults to None
         :type blockchain: str, Optional
+        :example blockchain: ethereum
         :param exchange: The exchange from which you want to get the pairs, defaults to None
         :type exchange: str, Optional
+        :example exchange: uniswapv2_ethereum
         :return: The list of pairs supported by the API. It returns token addresses,
         blockchain, exchange and the fee that the pair has.
         
         The fee may vary depending on the exchange used.
 
 
         Example response:
@@ -284,15 +302,15 @@
         """
         params = {}
         params["page"] = page
         if blockchain is not None:
             params["blockchain"] = blockchain
         if exchange is not None:
             params["exchange"] = exchange
-        ret = self._do_request("/v0/exchanges/pairs", params)
+        ret = await self._do_request("/v0/exchanges/pairs", params)
         return Pairs(
             page=ret["page"],
             total_pages=ret["total_pages"],
             data=[
                 Pair(
                     blockchain=d["blockchain"],
                     exchange=d["exchange"],
@@ -300,30 +318,33 @@
                     token1=d["token1"],
                     fee=d["fee"]
                 )
                 for d in ret["data"]
             ]
         )
 
-
-    def reserves(self, blockchain: str, token0: str, token1: str, exchange: str | None = None) -> List[Reserve]:
+    async def reserves(self, blockchain: str, token0: str, token1: str, exchange: str | None = None) -> List[Reserve]:
         """Get the liquidity inside of the reserve of two tokens.
 
-        @raises BlockchainNotSupportedException: When an invalid blockchain id is given
-        @raises ExchangeNotSupportedException: When an invalid exchange id is given
-        @raises PairNotFoundException: When a pair is not found for the given blockchain or exchange
+        :raises BlockchainNotSupportedException: When an invalid blockchain id is given
+        :raises ExchangeNotSupportedException: When an invalid exchange id is given
+        :raises PairNotFoundException: When a pair is not found for the given blockchain or exchange
 
         :param blockchain: The id of the blockchain on which the exchange will happen. It is required because some tokens can have same address accross multiple blockchains
         :type blockchain: str
+        :example blockchain: ethereum
         :param token0: The address of the first token of the pair
         :type token0: str
+        :example token0: 0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2
         :param token1: The address of the second token of the pair
         :type token1: str
+        :example token1: 0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48
         :param exchange: The id of the exchange from which you want to get the reserve, defaults to None
         :type exchange: str, Optional
+        :example exchange: uniswapv2_ethereum
         :return: The list of all of the reserve for the given pair, blockchain and exchange.
         Can return an empty list if the given pair was not found.
 
 
         Example response:
         ```json
         [
@@ -342,45 +363,49 @@
         """
         params = {}
         params["blockchain"] = blockchain
         if exchange is not None:
             params["exchange"] = exchange
         params["token0"] = token0
         params["token1"] = token1
-        ret = self._do_request("/v0/exchanges/pairs/reserves", params)
+        ret = await self._do_request("/v0/exchanges/pairs/reserves", params)
         return [
             Reserve(
                 blockchain=r["blockchain"],
                 exchange=r["exchange"],
                 token0=r["token0"],
                 token1=r["token1"],
                 reserve0=r["reserve0"],
                 reserve1=r["reserve1"]
             )
             for r in ret
         ]
 
+    async def amount_out(self, blockchain: str, tokenIn: str, tokenOut: str, amountIn: int, exchange: str | None = None) -> List[AmountOut]:
+        """Get the amount of tokenOut that you will get after selling amountIn tokenIn
 
-    def amount_out(self, blockchain: str, tokenIn: str, tokenOut: str, amountIn: int, exchange: str | None = None) -> List[AmountOut]:
-        """Get the amount of token1 that you will get after selling amountIn token0
-
-        @raises BlockchainNotSupportedException: When an invalid blockchain id is given
-        @raises ExchangeNotSupportedException: When an invalid exchange id is given
-        @raises PairNotFoundException: When a pair is not found for the given blockchain or exchange
+        :raises BlockchainNotSupportedException: When an invalid blockchain id is given
+        :raises ExchangeNotSupportedException: When an invalid exchange id is given
+        :raises PairNotFoundException: When a pair is not found for the given blockchain or exchange
 
         :param blockchain: The id of the blockchain on which this exchange take place
         :type blockchain: str
+        :example blockchain: ethereum
         :param tokenIn: The address of the token that you sell
         :type tokenIn: str
+        :example tokenIn: 0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2
         :param tokenOut: The address of the token that you buy
         :type tokenOut: str
-        :param amountIn: The amount of token0 that you sell
+        :example tokenOut: 0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48
+        :param amountIn: The amount of tokenIn that you sell
         :type amountIn: int
+        :example amountIn: 1000000000000000000
         :param exchange: The exchange on which you want to do the trade, defaults to None
         :type exchange: str, Optional
+        :example exchange: uniswapv2_ethereum
         :return: The list of the amount out that you will get on all of the exchanges. It can return an empty list if the given pair was not found for the given parameters.
 
 
         Example response:
         ```json
         [
             {
@@ -399,45 +424,49 @@
         params = {}
         params["blockchain"] = blockchain
         params["tokenIn"] = tokenIn
         params["tokenOut"] = tokenOut
         params["amountIn"] = amountIn
         if exchange is not None:
             params["exchange"] = exchange
-        ret = self._do_request("/v0/exchanges/pairs/amountOut", params)
+        ret = await self._do_request("/v0/exchanges/pairs/amountOut", params)
         return [
             AmountOut(
                 blockchain=r["blockchain"],
                 exchange=r["exchange"],
                 tokenIn=r["tokenIn"],
                 tokenOut=r["tokenOut"],
                 amountIn=r["amountIn"],
                 amountOut=r["amountOut"]
             )
             for r in ret
         ]
 
+    async def amount_in(self, blockchain: str, tokenIn: str, tokenOut: str, amountOut: int, exchange: str | None = None) -> List[AmountIn]:
+        """Get the amount of tokenIn that you need to sell in order to get amountOut tokenOut
 
-    def amount_in(self, blockchain: str, tokenIn: str, tokenOut: str, amountOut: int, exchange: str | None = None) -> List[AmountIn]:
-        """Get the amount of token0 that you need to sell in order to get amountIn token1
-
-        @raises BlockchainNotSupportedException: When an invalid blockchain id is given
-        @raises ExchangeNotSupportedException: When an invalid exchange id is given
-        @raises PairNotFoundException: When a pair is not found for the given blockchain or exchange
+        :raises BlockchainNotSupportedException: When an invalid blockchain id is given
+        :raises ExchangeNotSupportedException: When an invalid exchange id is given
+        :raises PairNotFoundException: When a pair is not found for the given blockchain or exchange
 
         :param blockchain: The id of the blockchain on which this exchange take place
         :type blockchain: str
+        :example blockchain: ethereum
         :param tokenIn: The address of the token that you sell
         :type tokenIn: str
+        :example tokenIn: 0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48
         :param tokenOut: The address of the token that you buy
         :type tokenOut: str
-        :param amountOut: The amount of token1 that you are trying to get
+        :example tokenOut: 0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2
+        :param amountOut: The amount of tokenOut that you are trying to get
         :type amountOut: int
+        :example amountOut: 1000000000000000000
         :param exchange: The exchange on which you want to do the trade, defaults to None
         :type exchange: str, Optional
+        :example exchange: uniswapv2_ethereum
         :return: The list of amount in that you will get on all of the exchanges. It can return an empty list if the given pair was not found.
 
 
         Example response:
         ```json
         [
             {
@@ -456,38 +485,39 @@
         params = {}
         params["blockchain"] = blockchain
         params["tokenIn"] = tokenIn
         params["tokenOut"] = tokenOut
         params["amountOut"] = amountOut
         if exchange is not None:
             params["exchange"] = exchange
-        ret = self._do_request("/v0/exchanges/pairs/amountIn", params)
+        ret = await self._do_request("/v0/exchanges/pairs/amountIn", params)
         return [
             AmountIn(
                 blockchain=r["blockchain"],
                 exchange=r["exchange"],
                 tokenIn=r["tokenIn"],
                 tokenOut=r["tokenOut"],
                 amountIn=r["amountIn"],
                 amountOut=r["amountOut"]
             )
             for r in ret
         ]
 
-
-    def tokens(self, page: int = 1, blockchain: str | None = None) -> Tokens:
+    async def tokens(self, page: int = 1, blockchain: str | None = None) -> Tokens:
         """Get the list of supported tokens
 
-        @raises BlockchainNotSupportedException: When an invalid blockchain id is given
-        @raises InvalidPageException: When an invalid page number is given
+        :raises BlockchainNotSupportedException: When an invalid blockchain id is given
+        :raises InvalidPageException: When an invalid page number is given
 
         :param page: Each request have a limit of 100 data separated per pages, defaults to 1
         :type page: int, Optional
+        :example page: 1
         :param blockchain: The blockchain on which you want to get the tokens, defaults to None
         :type blockchain: str, Optional
+        :example blockchain: ethereum
         :return: The list of supported tokens ordered by market cap in a descending order.
         
         The market capitalization is in dollars, it can be null if the liquidity available for the given token is lower than 1000$.
         The market capitalization is based on USDT.
         
         The market capitalization of each token is computed as follow:
         average worth of token in liquidity pools * total token supply
@@ -547,40 +577,41 @@
         ```
         :rtype: Tokens
         """
         params = {}
         params["page"] = page
         if blockchain is not None:
             params["blockchain"] = blockchain
-        ret = self._do_request("/v0/tokens/", params)
+        ret = await self._do_request("/v0/tokens/", params)
         return Tokens(
             page=ret["page"],
             total_pages=ret["total_pages"],
             data=[
                 Token(
                     blockchain=d["blockchain"],
                     address=d["address"],
                     decimals=d["decimals"],
                     market_cap=d["market_cap"]
                 )
                 for d in ret["data"]
             ]
         )
 
-
-    def info(self, blockchain: str, token: str) -> Token:
+    async def info(self, blockchain: str, token: str) -> Token:
         """Get information on a specific token
 
-        @raises BlockchainNotSupportedException: When an invalid blockchain id is given
-        @raises TokenNotFoundException: When the given token is not found
+        :raises BlockchainNotSupportedException: When an invalid blockchain id is given
+        :raises TokenNotFoundException: When the given token is not found
 
         :param blockchain: The blockchain on which you want to get the information of the token
         :type blockchain: str
+        :example blockchain: ethereum
         :param token: The address of the token that you want to get the informations from
         :type token: str
+        :example token: 0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2
         :return: Informations on a specific token.
         
         This information includes:
         - The id of the blockchain that this token is
         - The address of the token
         - The decimals of it
         - The market cap
@@ -597,40 +628,40 @@
 
         ```
         :rtype: Token
         """
         params = {}
         params["blockchain"] = blockchain
         params["token"] = token
-        ret = self._do_request("/v0/tokens/info", params)
+        ret = await self._do_request("/v0/tokens/info", params)
         return Token(
             blockchain=ret["blockchain"],
             address=ret["address"],
             decimals=ret["decimals"],
             market_cap=ret["market_cap"]
         )
 
-
-    def decimals(self, blockchain: str, token: str) -> int:
+    async def decimals(self, blockchain: str, token: str) -> int:
         """Get the decimals of the given token
 
-        @raises HTTPValidationError: Validation Error
+        :raises HTTPValidationError: Validation Error
 
         :param blockchain: The id of the blockchain of the token
         :type blockchain: str
+        :example blockchain: ethereum
         :param token: The address of the token that you want to get the decimals from
         :type token: str
+        :example token: 0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2
         :return: The decimals of the specific token
 
 
         Example response:
         ```json
         16
         ```
         :rtype: int
         """
         params = {}
         params["blockchain"] = blockchain
         params["token"] = token
-        ret = self._do_request("/v0/tokens/decimals", params)
+        ret = await self._do_request("/v0/tokens/decimals", params)
         return int(ret)
-
```

### Comparing `blockchain-apis-0.1.1/src/blockchainapis/__init__.py` & `blockchain-apis-0.1.2/src/blockchainapis/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """
-The blockchainapis package allow you to interact with Blockchain
+The blockchain-apis package allow you to interact with Blockchain
 APIs in a synchronous and asynchronous way.
 
 If you are starting on a new project, it is better to use the async
 class, which is called: BlockchainAPIs
 
 If you already have a project and don't want to bother with async,
 you can use the BlockchainAPIsSync class.
+
 """
 
 # Clarensia: https://www.clarensia.com is the company behind
 # the development of https://www.blockchainapis.io
 __author__ = "Clarensia"
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 
 from .BlockchainAPIs import BlockchainAPIs
 from .BlockchainAPIsSync import BlockchainAPIsSync
 
-__all__ = ["BlockchainAPIs"]
+__all__ = ['BlockchainAPIs']
```

### Comparing `blockchain-apis-0.1.1/src/blockchainapis/exceptions/BlockchainNotSupportedException.py` & `blockchain-apis-0.1.2/src/blockchainapis/exceptions/BlockchainNotSupportedException.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,22 @@
-from .BlockchainAPIsException import BlockchainAPIsException
+from . import BlockchainAPIsException
 
 class BlockchainNotSupportedException(BlockchainAPIsException):
     """
     Thrown when an Invalid blockchain id is put during a call to the API.
     
     To get the list of valid blockchain ids, call `/blockchains`
     """
 
-
     status_code: str
     """The error code returned by the call to the API
     
     For example: 422
     """
 
-
     detail: str
     """Some details about the error that occured
     
     For example:
     Blockchain with id "test" is not supported. You can find a list of valid blockchain ids in /blockchains
     """
```

### Comparing `blockchain-apis-0.1.1/src/blockchainapis/exceptions/ExchangeNotSupportedException.py` & `blockchain-apis-0.1.2/src/blockchainapis/exceptions/ExchangeNotSupportedException.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,22 @@
-from .BlockchainAPIsException import BlockchainAPIsException
+from . import BlockchainAPIsException
 
 class ExchangeNotSupportedException(BlockchainAPIsException):
     """
     Thrown when an Invalid exchange id is given during a call to the API.
     
     To get the list of supported exchange ids, call `/exchanges`
     """
 
-
     status_code: str
     """The error code returned by the call to the API
     
     For example: 422
     """
 
-
     detail: str
     """Some details about the error that occured
     
     For example:
     Exchange with id "test" is not supported. You can get the list of valid exchange ids in /exchanges
     """
```

### Comparing `blockchain-apis-0.1.1/src/blockchainapis/exceptions/InvalidPageException.py` & `blockchain-apis-0.1.2/src/blockchainapis/exceptions/InvalidPageException.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,28 @@
-from .BlockchainAPIsException import BlockchainAPIsException
+from . import BlockchainAPIsException
 
 class InvalidPageException(BlockchainAPIsException):
     """
     Thrown when you given an invalid page index during calls to responses that
     gives paginated results.
     
     An invalid page is:
     * A number lower or equal to 0
     * A page way too high
     
     You should start with 1 as page, and then the response object will give you
     the amount of pages available.
     """
 
-
     status_code: str
     """The error code returned by the call to the API
     
     For example: 400
     """
 
-
     detail: str
     """Some details about the error that occured
     
     For example:
     -2 is not a valid page number.
     """
```

### Comparing `blockchain-apis-0.1.1/src/blockchainapis/exceptions/PairNotFoundException.py` & `blockchain-apis-0.1.2/src/blockchainapis/exceptions/PairNotFoundException.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,23 @@
-from .BlockchainAPIsException import BlockchainAPIsException
+from . import BlockchainAPIsException
 
 class PairNotFoundException(BlockchainAPIsException):
     """
     Thrown when you try to get some data about a pair that does not exist.
     
     To avoid getting this error, you can get the list of available pairs for
     the blockchain and exchange that you are interested in by calling `/exchanges/pairs`
     """
 
-
     status_code: str
     """The error code returned by the call to the API
     
     For example: 422
     """
 
-
     detail: str
     """Some details about the error that occured
     
     For example:
     Pair 0x8E870D67F660D95d5be530380D0eC0bd388289E1->0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2 not found in blockchain Arbitrum
     """
```

### Comparing `blockchain-apis-0.1.1/src/blockchainapis/exceptions/TokenNotFoundException.py` & `blockchain-apis-0.1.2/src/blockchainapis/exceptions/TokenNotFoundException.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,24 @@
-from .BlockchainAPIsException import BlockchainAPIsException
+from . import BlockchainAPIsException
 
 class TokenNotFoundException(BlockchainAPIsException):
     """
     Thrown when you try to get informations on a token that does not exist inside of our database.
     
     At BlockchainAPIs, we only handle tokens that are inside of a liquidity pool.
     
     You can get a list of all of the available tokens by calling `/tokens`
     """
 
-
     status_code: str
     """The error code returned by the call to the API
     
     For example: 404
     """
 
-
     detail: str
     """Some details about the error that occured
     
     For example:
     Token 0x8E870D67F660D95d5be530380D0eC0bd388289E1 not found for blockchain ethereum
     """
```

### Comparing `blockchain-apis-0.1.1/src/blockchainapis/exceptions/TooManyRequestsException.py` & `blockchain-apis-0.1.2/src/blockchainapis/exceptions/TooManyRequestsException.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,24 @@
-from .BlockchainAPIsException import BlockchainAPIsException
+from . import BlockchainAPIsException
 
 class TooManyRequestsException(BlockchainAPIsException):
     """
     Thrown when you are doing more request than you are allowed to the API.
     
     To prevent this exception you can:
     - Lower the amount of requests that you make to the API per second
     - Upgrade your subscription at: https://dashboard.blockchainapis.io/
     """
 
-
     status_code: str
     """The error code returned by the call to the API
     
     For example: 429
     """
 
-
     detail: str
     """Some details about the error that occured
     
     For example:
     Too many requests
     """
```

### Comparing `blockchain-apis-0.1.1/src/blockchainapis/exceptions/UnauthorizedException.py` & `blockchain-apis-0.1.2/src/blockchainapis/exceptions/UnauthorizedException.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,25 @@
-from .BlockchainAPIsException import BlockchainAPIsException
+from . import BlockchainAPIsException
 
 class UnauthorizedException(BlockchainAPIsException):
     """
     Thrown when you are trying to make an API request with an invalid or expired
     API key.
     
     To prevent this exception, you can:
     - Make the request without an API key
     - Update/get a valid API key at: https://dashboard.blockchainapis.io/
     """
 
-
     status_code: str
     """The error code returned by the call to the API
     
     For example: 401
     """
 
-
     detail: str
     """Some details about the error that occured
     
     For example:
     Unauthorized
     """
```

### Comparing `blockchain-apis-0.1.1/src/blockchainapis/exceptions/__init__.py` & `blockchain-apis-0.1.2/src/blockchainapis/exceptions/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 """
 Contains the Exceptions that can be thrown from
 Blockchain APIs
 
 These exceptions are thrown when a call is made to Blockchain APIs
 and the response code is not 200 or 201
+
 """
 
+from .BlockchainAPIsException import BlockchainAPIsException
 from .BlockchainNotSupportedException import BlockchainNotSupportedException
 from .ExchangeNotSupportedException import ExchangeNotSupportedException
 from .InvalidPageException import InvalidPageException
-from .PairNotFoundException import PairNotFoundException
 from .TokenNotFoundException import TokenNotFoundException
+from .PairNotFoundException import PairNotFoundException
 from .TooManyRequestsException import TooManyRequestsException
 from .UnauthorizedException import UnauthorizedException
 
 __all__ = [
     "BlockchainNotSupportedException",
     "ExchangeNotSupportedException",
     "InvalidPageException",
-    "PairNotFoundException",
     "TokenNotFoundException",
+    "PairNotFoundException",
     "TooManyRequestsException",
     "UnauthorizedException"
 ]
```

### Comparing `blockchain-apis-0.1.1/src/blockchainapis/models/AmountIn.py` & `blockchain-apis-0.1.2/src/blockchainapis/models/AmountIn.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,8 +36,7 @@
     """
 
     amountOut: int
     """The amount of tokenOut that you wish to buy
 
     Example: 10000
     """
-
```

### Comparing `blockchain-apis-0.1.1/src/blockchainapis/models/AmountOut.py` & `blockchain-apis-0.1.2/src/blockchainapis/models/AmountOut.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,8 +36,7 @@
     """
 
     amountOut: int
     """The amount of tokenOut that you will get after selling amountIn tokenIn on this exchange
 
     Example: 11088529
     """
-
```

### Comparing `blockchain-apis-0.1.1/src/blockchainapis/models/Blockchain.py` & `blockchain-apis-0.1.2/src/blockchainapis/models/Blockchain.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,8 +24,7 @@
     """
 
     explorer: str
     """The url to the explorer of the blockchain
 
     Example: "https://snowtrace.io/"
     """
-
```

### Comparing `blockchain-apis-0.1.1/src/blockchainapis/models/Exchange.py` & `blockchain-apis-0.1.2/src/blockchainapis/models/Exchange.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,8 +24,7 @@
     """
 
     url: str
     """The url to the exchange
 
     Example: "https://exchange.lydia.finance/#/swap"
     """
-
```

### Comparing `blockchain-apis-0.1.1/src/blockchainapis/models/Exchanges.py` & `blockchain-apis-0.1.2/src/blockchainapis/models/Exchanges.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from dataclasses import dataclass
 from typing import List
-
 from . import Exchange
 
 
 @dataclass(slots=True, frozen=True)
 class Exchanges:
     """The Exchanges model"""
 
@@ -37,8 +36,7 @@
             "blockchain": "avalanche",
             "name": "Oliveswap",
             "url": "https://avax.olive.cash/",
             "fee": 250
         }
     ]
     """
-
```

### Comparing `blockchain-apis-0.1.1/src/blockchainapis/models/Pair.py` & `blockchain-apis-0.1.2/src/blockchainapis/models/Pair.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,8 +30,7 @@
     """
 
     fee: int
     """The fee of the pair in 100000 of percents (for example: 1000 is 1%)
 
     Example: 300
     """
-
```

### Comparing `blockchain-apis-0.1.1/src/blockchainapis/models/Pairs.py` & `blockchain-apis-0.1.2/src/blockchainapis/models/Pairs.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from dataclasses import dataclass
 from typing import List
-
 from . import Pair
 
 
 @dataclass(slots=True, frozen=True)
 class Pairs:
     """The Pairs model"""
 
@@ -37,8 +36,7 @@
             "exchange": "uniswapv2_ethereum",
             "token0": "0x8E870D67F660D95d5be530380D0eC0bd388289E1",
             "token1": "0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48",
             "fee": 300
         }
     ]
     """
-
```

### Comparing `blockchain-apis-0.1.1/src/blockchainapis/models/Reserve.py` & `blockchain-apis-0.1.2/src/blockchainapis/models/Reserve.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,8 +36,7 @@
     """
 
     reserve1: int
     """The amount of token1 inside of the reserve
 
     Example: 117592619550992960
     """
-
```

### Comparing `blockchain-apis-0.1.1/src/blockchainapis/models/Token.py` & `blockchain-apis-0.1.2/src/blockchainapis/models/Token.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,8 +29,7 @@
 
 The value is in dollars, it can be None if the liquidity of the token in pools is lower than 1000$
 
 This value is in Decimal, and is based on USDT.
 
     Example: Decimal(62609470.072472)
     """
-
```

### Comparing `blockchain-apis-0.1.1/src/blockchainapis/models/Tokens.py` & `blockchain-apis-0.1.2/src/blockchainapis/models/Tokens.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from dataclasses import dataclass
 from typing import List
-
 from . import Token
 
 
 @dataclass(slots=True, frozen=True)
 class Tokens:
     """The Tokens model"""
 
@@ -65,8 +64,7 @@
             "blockchain": "avalanche",
             "address": "0xc7198437980c041c805A1EDcbA50c1Ce5db95118",
             "decimals": 6,
             "market_cap": 62609470.072472
         }
     ]
     """
-
```

### Comparing `blockchain-apis-0.1.1/src/blockchainapis/models/__init__.py` & `blockchain-apis-0.1.2/src/blockchainapis/models/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Contains the models that are returned by the Blockchain APIs instance
 class.
 
 These models are all dataclasses that have the slots and frozen set to True.
 
 - `slots=True` Allow you to have more optimized access to the data
 - `frozen=True` This way you can't modify the returned values from the API.
-                Because what the API return is final it should not be modified.
+              Because what the API return is final it should not be modified.
 
 To access some data use the Python dot "." notation.
 
 For example:
 ```python
 blockchain_instance = Blockchain(
     blockchain="ethereum",
@@ -31,17 +31,16 @@
     chain_id=1,
     explorer="https://etherscan.io/"
 )
 
 # This will throw an exception, use the notation in the example
 # above please.
 print(blockchain_instance["blockchain"])
-```
-"""
 
+"""
 from .AmountIn import AmountIn
 from .AmountOut import AmountOut
 from .Blockchain import Blockchain
 from .Exchange import Exchange
 from .Exchanges import Exchanges
 from .Pair import Pair
 from .Pairs import Pairs
```

### Comparing `blockchain-apis-0.1.1/tests/test_amount_in.py` & `blockchain-apis-0.1.2/tests/test_amount_in.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.1/tests/test_amount_in_sync.py` & `blockchain-apis-0.1.2/tests/test_amount_in_sync.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.1/tests/test_amount_out.py` & `blockchain-apis-0.1.2/tests/test_amount_out.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.1/tests/test_amount_out_sync.py` & `blockchain-apis-0.1.2/tests/test_amount_out_sync.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.1/tests/test_decimals.py` & `blockchain-apis-0.1.2/tests/test_decimals.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.1/tests/test_decimals_sync.py` & `blockchain-apis-0.1.2/tests/test_decimals_sync.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.1/tests/test_exchanges.py` & `blockchain-apis-0.1.2/tests/test_exchanges.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.1/tests/test_exchanges_sync.py` & `blockchain-apis-0.1.2/tests/test_exchanges_sync.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.1/tests/test_info.py` & `blockchain-apis-0.1.2/tests/test_info.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.1/tests/test_info_sync.py` & `blockchain-apis-0.1.2/tests/test_info_sync.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.1/tests/test_pairs.py` & `blockchain-apis-0.1.2/tests/test_pairs.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.1/tests/test_pairs_sync.py` & `blockchain-apis-0.1.2/tests/test_pairs_sync.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.1/tests/test_reserves.py` & `blockchain-apis-0.1.2/tests/test_reserves.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.1/tests/test_reserves_sync.py` & `blockchain-apis-0.1.2/tests/test_reserves_sync.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.1/tests/test_tokens.py` & `blockchain-apis-0.1.2/tests/test_tokens.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.1/tests/test_tokens_sync.py` & `blockchain-apis-0.1.2/tests/test_tokens_sync.py`

 * *Files identical despite different names*

