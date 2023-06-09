# Comparing `tmp/python_pulsechain-0.1.2.tar.gz` & `tmp/python_pulsechain-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_pulsechain-0.1.2.tar", max compression
+gzip compressed data, was "python_pulsechain-0.1.3.tar", max compression
```

## Comparing `python_pulsechain-0.1.2.tar` & `python_pulsechain-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1068 2023-05-28 17:32:44.886854 python_pulsechain-0.1.2/LICENSE
--rw-r--r--   0        0        0       96 2023-05-29 20:24:55.522194 python_pulsechain-0.1.2/pulsechain/__init__.py
--rw-r--r--   0        0        0     4322 2023-05-29 20:22:41.619811 python_pulsechain-0.1.2/pulsechain/account.py
--rw-r--r--   0        0        0     1675 2023-05-29 20:22:33.161714 python_pulsechain-0.1.2/pulsechain/token.py
--rw-r--r--   0        0        0     1533 2023-05-29 20:21:56.386910 python_pulsechain-0.1.2/pulsechain/transaction.py
--rw-r--r--   0        0        0      555 2023-05-28 17:40:48.504476 python_pulsechain-0.1.2/pulsechain/utils.py
--rw-r--r--   0        0        0      647 2023-05-29 20:17:16.864734 python_pulsechain-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1827 2023-05-29 20:15:37.545898 python_pulsechain-0.1.2/README.md
--rw-r--r--   0        0        0     2506 1970-01-01 00:00:00.000000 python_pulsechain-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-05-28 17:32:44.886854 python_pulsechain-0.1.3/LICENSE
+-rw-r--r--   0        0        0       96 2023-05-29 20:24:55.522194 python_pulsechain-0.1.3/pulsechain/__init__.py
+-rw-r--r--   0        0        0     7736 2023-06-07 21:12:20.134904 python_pulsechain-0.1.3/pulsechain/account.py
+-rw-r--r--   0        0        0     1712 2023-06-07 21:06:37.550649 python_pulsechain-0.1.3/pulsechain/token.py
+-rw-r--r--   0        0        0     1604 2023-06-07 21:06:37.542649 python_pulsechain-0.1.3/pulsechain/transaction.py
+-rw-r--r--   0        0        0      884 2023-06-07 21:01:01.764531 python_pulsechain-0.1.3/pulsechain/utils.py
+-rw-r--r--   0        0        0      647 2023-06-07 21:06:37.538621 python_pulsechain-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1827 2023-05-29 20:15:37.545898 python_pulsechain-0.1.3/README.md
+-rw-r--r--   0        0        0     2506 1970-01-01 00:00:00.000000 python_pulsechain-0.1.3/PKG-INFO
```

### Comparing `python_pulsechain-0.1.2/LICENSE` & `python_pulsechain-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python_pulsechain-0.1.2/pulsechain/token.py` & `python_pulsechain-0.1.3/pulsechain/token.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 with transaction part of the PulseChain explorer API.
 """
 from typing import Dict, Any
 
 import requests
 
 from pulsechain import API_URL
+from pulsechain.utils import check_result
 
 
 def get_token(contract_address: str) -> Dict[str, Any]:
     """
     Fetch the ERC-20 or ERC-721 token by contract address.
 
     :param contract_address: The contract address to fetch the token for.
@@ -23,16 +24,15 @@
     params = {
         "module": "token",
         "action": "getToken",
         "contractaddress": contract_address,
     }
 
     response = requests.get(API_URL, params=params, timeout=10)
-    data = response.json()
-    return data
+    return check_result(response.json())
 
 
 def get_token_holders(
     contract_address: str, page: int = 1, offset: int = 10
 ) -> Dict[str, Any]:
     """
     Fetch the token holders by contract address.
@@ -51,9 +51,8 @@
         "action": "getTokenHolders",
         "contractaddress": contract_address,
         "page": page,
         "offset": offset,
     }
 
     response = requests.get(API_URL, params=params, timeout=10)
-    data = response.json()
-    return data
+    return check_result(response.json())
```

### Comparing `python_pulsechain-0.1.2/pulsechain/transaction.py` & `python_pulsechain-0.1.3/pulsechain/transaction.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 with transaction part of the PulseChain explorer API.
 """
 from typing import Dict, Any
 
 import requests
 
 from pulsechain import API_URL
+from pulsechain.utils import check_result
 
 
 def get_transaction_info(txhash: str, index: int = None) -> Dict[str, Any]:
     """
     Fetch the transaction info.
 
     :param txhash: The hash of the transaction.
@@ -28,15 +29,15 @@
         "txhash": txhash,
     }
 
     if index is not None:
         params["index"] = index
 
     response = requests.get(API_URL, params=params, timeout=10)
-    return response.json()
+    return check_result(response.json())
 
 
 def get_transaction_receipt_status(txhash):
     """
     Fetch the receipt status of a given transaction on PulseChain.
 
     :param txhash: The transaction hash to fetch the receipt status for.
@@ -50,8 +51,8 @@
     params = {
         'module': 'transaction',
         'action': 'gettxreceiptstatus',
         'txhash': txhash
     }
 
     response = requests.get(base_url, params=params, timeout=10)
-    return response.json()
+    return check_result(response.json())
```

### Comparing `python_pulsechain-0.1.2/pyproject.toml` & `python_pulsechain-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-pulsechain"
-version = "0.1.2"
+version = "0.1.3"
 description = "Python implementation for PulseChain API"
 license = "MIT"
 repository = "https://github.com/crypto-ralph/python-pulsechain"
 authors = ["CryptoRalph <doxter@protonmail.com>"]
 readme = "README.md"
 include = [
     "LICENSE",
```

### Comparing `python_pulsechain-0.1.2/README.md` & `python_pulsechain-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `python_pulsechain-0.1.2/PKG-INFO` & `python_pulsechain-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-pulsechain
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python implementation for PulseChain API
 Home-page: https://github.com/crypto-ralph/python-pulsechain
 License: MIT
 Author: CryptoRalph
 Author-email: doxter@protonmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

