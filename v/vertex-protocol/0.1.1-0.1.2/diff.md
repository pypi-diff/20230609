# Comparing `tmp/vertex_protocol-0.1.1.tar.gz` & `tmp/vertex_protocol-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vertex_protocol-0.1.1.tar", max compression
+gzip compressed data, was "vertex_protocol-0.1.2.tar", max compression
```

## Comparing `vertex_protocol-0.1.1.tar` & `vertex_protocol-0.1.2.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0      982 2023-06-09 06:52:38.447127 vertex_protocol-0.1.1/README.md
--rw-r--r--   0        0        0     1445 2023-06-09 06:52:38.447127 vertex_protocol-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-09 06:52:38.447127 vertex_protocol-0.1.1/vertex_protocol/__init__.py
--rw-r--r--   0        0        0     6628 2023-06-09 06:52:38.447127 vertex_protocol-0.1.1/vertex_protocol/client/__init__.py
--rw-r--r--   0        0        0      580 2023-06-09 06:52:38.447127 vertex_protocol-0.1.1/vertex_protocol/client/apis/__init__.py
--rw-r--r--   0        0        0     1394 2023-06-09 06:52:38.447127 vertex_protocol-0.1.1/vertex_protocol/client/apis/base.py
--rw-r--r--   0        0        0     1108 2023-06-09 06:52:38.447127 vertex_protocol-0.1.1/vertex_protocol/client/apis/market/__init__.py
--rw-r--r--   0        0        0     3404 2023-06-09 06:52:38.447127 vertex_protocol-0.1.1/vertex_protocol/client/apis/market/execute.py
--rw-r--r--   0        0        0    10070 2023-06-09 06:52:38.447127 vertex_protocol-0.1.1/vertex_protocol/client/apis/market/query.py
--rw-r--r--   0        0        0      746 2023-06-09 06:52:38.447127 vertex_protocol-0.1.1/vertex_protocol/client/apis/perp/__init__.py
--rw-r--r--   0        0        0     1438 2023-06-09 06:52:38.447127 vertex_protocol-0.1.1/vertex_protocol/client/apis/perp/query.py
--rw-r--r--   0        0        0     1027 2023-06-09 06:52:38.447127 vertex_protocol-0.1.1/vertex_protocol/client/apis/spot/__init__.py
--rw-r--r--   0        0        0     1191 2023-06-09 06:52:38.447127 vertex_protocol-0.1.1/vertex_protocol/client/apis/spot/base.py
--rw-r--r--   0        0        0     4745 2023-06-09 06:52:38.447127 vertex_protocol-0.1.1/vertex_protocol/client/apis/spot/execute.py
--rw-r--r--   0        0        0     2933 2023-06-09 06:52:38.447127 vertex_protocol-0.1.1/vertex_protocol/client/apis/spot/query.py
--rw-r--r--   0        0        0     1307 2023-06-09 06:52:38.447127 vertex_protocol-0.1.1/vertex_protocol/client/apis/subaccount/__init__.py
--rw-r--r--   0        0        0     2023 2023-06-09 06:52:38.447127 vertex_protocol-0.1.1/vertex_protocol/client/apis/subaccount/execute.py
--rw-r--r--   0        0        0     3162 2023-06-09 06:52:38.447127 vertex_protocol-0.1.1/vertex_protocol/client/apis/subaccount/query.py
--rw-r--r--   0        0        0     2551 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/client/context.py
--rw-r--r--   0        0        0     8404 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/contracts/__init__.py
--rw-r--r--   0        0        0    11702 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/contracts/abis/Endpoint.json
--rw-r--r--   0        0        0    55374 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/contracts/abis/FQuerier.json
--rw-r--r--   0        0        0    16980 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/contracts/abis/IClearinghouse.json
--rw-r--r--   0        0        0     3385 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/contracts/abis/IERC20.json
--rw-r--r--   0        0        0     4723 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/contracts/abis/IEndpoint.json
--rw-r--r--   0        0        0    13112 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/contracts/abis/IOffchainBook.json
--rw-r--r--   0        0        0    21812 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/contracts/abis/IPerpEngine.json
--rw-r--r--   0        0        0     8410 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/contracts/abis/IProductEngine.json
--rw-r--r--   0        0        0    18858 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/contracts/abis/ISpotEngine.json
--rw-r--r--   0        0        0     5698 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/contracts/abis/MockERC20.json
--rw-r--r--   0        0        0     1022 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/contracts/deployments/deployment.arbitrumGoerli.json
--rw-r--r--   0        0        0      993 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/contracts/deployments/deployment.arbitrumOne.json
--rw-r--r--   0        0        0      908 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/contracts/deployments/deployment.test.json
--rw-r--r--   0        0        0     1414 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/contracts/eip712/__init__.py
--rw-r--r--   0        0        0     1183 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/contracts/eip712/domain.py
--rw-r--r--   0        0        0     2511 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/contracts/eip712/sign.py
--rw-r--r--   0        0        0     3222 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/contracts/eip712/types.py
--rw-r--r--   0        0        0     1526 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/contracts/loader.py
--rw-r--r--   0        0        0     2747 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/contracts/types.py
--rw-r--r--   0        0        0     1127 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/engine_client/__init__.py
--rw-r--r--   0        0        0    18437 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/engine_client/execute.py
--rw-r--r--   0        0        0    11077 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/engine_client/query.py
--rw-r--r--   0        0        0     3413 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/engine_client/types/__init__.py
--rw-r--r--   0        0        0    18340 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/engine_client/types/execute.py
--rw-r--r--   0        0        0     3426 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/engine_client/types/models.py
--rw-r--r--   0        0        0     9473 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/engine_client/types/query.py
--rw-r--r--   0        0        0      926 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/indexer_client/__init__.py
--rw-r--r--   0        0        0    11025 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/indexer_client/query.py
--rw-r--r--   0        0        0      273 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/indexer_client/types/__init__.py
--rw-r--r--   0        0        0     5588 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/indexer_client/types/models.py
--rw-r--r--   0        0        0    12079 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/indexer_client/types/query.py
--rw-r--r--   0        0        0      933 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/utils/__init__.py
--rw-r--r--   0        0        0      341 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/utils/backend.py
--rw-r--r--   0        0        0     5216 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/utils/bytes32.py
--rw-r--r--   0        0        0       99 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/utils/enum.py
--rw-r--r--   0        0        0     1136 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/utils/exceptions.py
--rw-r--r--   0        0        0     1094 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/utils/expiration.py
--rw-r--r--   0        0        0      927 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/utils/math.py
--rw-r--r--   0        0        0     1887 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/utils/model.py
--rw-r--r--   0        0        0      809 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/utils/nonce.py
--rw-r--r--   0        0        0      491 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/utils/subaccount.py
--rw-r--r--   0        0        0     1530 1970-01-01 00:00:00.000000 vertex_protocol-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      982 2023-06-09 21:31:43.097292 vertex_protocol-0.1.2/README.md
+-rw-r--r--   0        0        0     1665 2023-06-09 21:31:43.101292 vertex_protocol-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-09 21:31:43.101292 vertex_protocol-0.1.2/vertex_protocol/__init__.py
+-rw-r--r--   0        0        0     6628 2023-06-09 21:31:43.101292 vertex_protocol-0.1.2/vertex_protocol/client/__init__.py
+-rw-r--r--   0        0        0      580 2023-06-09 21:31:43.101292 vertex_protocol-0.1.2/vertex_protocol/client/apis/__init__.py
+-rw-r--r--   0        0        0     1394 2023-06-09 21:31:43.101292 vertex_protocol-0.1.2/vertex_protocol/client/apis/base.py
+-rw-r--r--   0        0        0     1108 2023-06-09 21:31:43.101292 vertex_protocol-0.1.2/vertex_protocol/client/apis/market/__init__.py
+-rw-r--r--   0        0        0     3404 2023-06-09 21:31:43.101292 vertex_protocol-0.1.2/vertex_protocol/client/apis/market/execute.py
+-rw-r--r--   0        0        0    10070 2023-06-09 21:31:43.101292 vertex_protocol-0.1.2/vertex_protocol/client/apis/market/query.py
+-rw-r--r--   0        0        0      746 2023-06-09 21:31:43.101292 vertex_protocol-0.1.2/vertex_protocol/client/apis/perp/__init__.py
+-rw-r--r--   0        0        0     1438 2023-06-09 21:31:43.101292 vertex_protocol-0.1.2/vertex_protocol/client/apis/perp/query.py
+-rw-r--r--   0        0        0     1027 2023-06-09 21:31:43.101292 vertex_protocol-0.1.2/vertex_protocol/client/apis/spot/__init__.py
+-rw-r--r--   0        0        0     1191 2023-06-09 21:31:43.101292 vertex_protocol-0.1.2/vertex_protocol/client/apis/spot/base.py
+-rw-r--r--   0        0        0     4745 2023-06-09 21:31:43.101292 vertex_protocol-0.1.2/vertex_protocol/client/apis/spot/execute.py
+-rw-r--r--   0        0        0     2933 2023-06-09 21:31:43.101292 vertex_protocol-0.1.2/vertex_protocol/client/apis/spot/query.py
+-rw-r--r--   0        0        0     1307 2023-06-09 21:31:43.101292 vertex_protocol-0.1.2/vertex_protocol/client/apis/subaccount/__init__.py
+-rw-r--r--   0        0        0     2023 2023-06-09 21:31:43.101292 vertex_protocol-0.1.2/vertex_protocol/client/apis/subaccount/execute.py
+-rw-r--r--   0        0        0     3162 2023-06-09 21:31:43.101292 vertex_protocol-0.1.2/vertex_protocol/client/apis/subaccount/query.py
+-rw-r--r--   0        0        0     2551 2023-06-09 21:31:43.101292 vertex_protocol-0.1.2/vertex_protocol/client/context.py
+-rw-r--r--   0        0        0     8264 2023-06-09 21:31:43.105292 vertex_protocol-0.1.2/vertex_protocol/contracts/__init__.py
+-rw-r--r--   0        0        0    11702 2023-06-09 21:31:43.105292 vertex_protocol-0.1.2/vertex_protocol/contracts/abis/Endpoint.json
+-rw-r--r--   0        0        0    55374 2023-06-09 21:31:43.105292 vertex_protocol-0.1.2/vertex_protocol/contracts/abis/FQuerier.json
+-rw-r--r--   0        0        0    16980 2023-06-09 21:31:43.105292 vertex_protocol-0.1.2/vertex_protocol/contracts/abis/IClearinghouse.json
+-rw-r--r--   0        0        0     3385 2023-06-09 21:31:43.105292 vertex_protocol-0.1.2/vertex_protocol/contracts/abis/IERC20.json
+-rw-r--r--   0        0        0     4723 2023-06-09 21:31:43.105292 vertex_protocol-0.1.2/vertex_protocol/contracts/abis/IEndpoint.json
+-rw-r--r--   0        0        0    13112 2023-06-09 21:31:43.105292 vertex_protocol-0.1.2/vertex_protocol/contracts/abis/IOffchainBook.json
+-rw-r--r--   0        0        0    21812 2023-06-09 21:31:43.105292 vertex_protocol-0.1.2/vertex_protocol/contracts/abis/IPerpEngine.json
+-rw-r--r--   0        0        0     8410 2023-06-09 21:31:43.105292 vertex_protocol-0.1.2/vertex_protocol/contracts/abis/IProductEngine.json
+-rw-r--r--   0        0        0    18858 2023-06-09 21:31:43.105292 vertex_protocol-0.1.2/vertex_protocol/contracts/abis/ISpotEngine.json
+-rw-r--r--   0        0        0     5698 2023-06-09 21:31:43.105292 vertex_protocol-0.1.2/vertex_protocol/contracts/abis/MockERC20.json
+-rw-r--r--   0        0        0     1013 2023-06-09 21:31:43.105292 vertex_protocol-0.1.2/vertex_protocol/contracts/deployments/deployment.arbitrumGoerli.json
+-rw-r--r--   0        0        0      993 2023-06-09 21:31:43.105292 vertex_protocol-0.1.2/vertex_protocol/contracts/deployments/deployment.arbitrumOne.json
+-rw-r--r--   0        0        0      908 2023-06-09 21:31:43.105292 vertex_protocol-0.1.2/vertex_protocol/contracts/deployments/deployment.test.json
+-rw-r--r--   0        0        0      426 2023-06-09 21:31:43.105292 vertex_protocol-0.1.2/vertex_protocol/contracts/eip712/__init__.py
+-rw-r--r--   0        0        0     1189 2023-06-09 21:31:43.105292 vertex_protocol-0.1.2/vertex_protocol/contracts/eip712/domain.py
+-rw-r--r--   0        0        0     2484 2023-06-09 21:31:43.105292 vertex_protocol-0.1.2/vertex_protocol/contracts/eip712/sign.py
+-rw-r--r--   0        0        0     4636 2023-06-09 21:31:43.105292 vertex_protocol-0.1.2/vertex_protocol/contracts/eip712/types.py
+-rw-r--r--   0        0        0     1526 2023-06-09 21:31:43.105292 vertex_protocol-0.1.2/vertex_protocol/contracts/loader.py
+-rw-r--r--   0        0        0     2747 2023-06-09 21:31:43.105292 vertex_protocol-0.1.2/vertex_protocol/contracts/types.py
+-rw-r--r--   0        0        0     1127 2023-06-09 21:31:43.105292 vertex_protocol-0.1.2/vertex_protocol/engine_client/__init__.py
+-rw-r--r--   0        0        0    18437 2023-06-09 21:31:43.105292 vertex_protocol-0.1.2/vertex_protocol/engine_client/execute.py
+-rw-r--r--   0        0        0    11077 2023-06-09 21:31:43.105292 vertex_protocol-0.1.2/vertex_protocol/engine_client/query.py
+-rw-r--r--   0        0        0     5739 2023-06-09 21:31:43.105292 vertex_protocol-0.1.2/vertex_protocol/engine_client/types/__init__.py
+-rw-r--r--   0        0        0    18331 2023-06-09 21:31:43.105292 vertex_protocol-0.1.2/vertex_protocol/engine_client/types/execute.py
+-rw-r--r--   0        0        0     3426 2023-06-09 21:31:43.105292 vertex_protocol-0.1.2/vertex_protocol/engine_client/types/models.py
+-rw-r--r--   0        0        0     9473 2023-06-09 21:31:43.105292 vertex_protocol-0.1.2/vertex_protocol/engine_client/types/query.py
+-rw-r--r--   0        0        0      926 2023-06-09 21:31:43.105292 vertex_protocol-0.1.2/vertex_protocol/indexer_client/__init__.py
+-rw-r--r--   0        0        0    11025 2023-06-09 21:31:43.105292 vertex_protocol-0.1.2/vertex_protocol/indexer_client/query.py
+-rw-r--r--   0        0        0     2979 2023-06-09 21:31:43.105292 vertex_protocol-0.1.2/vertex_protocol/indexer_client/types/__init__.py
+-rw-r--r--   0        0        0     5588 2023-06-09 21:31:43.105292 vertex_protocol-0.1.2/vertex_protocol/indexer_client/types/models.py
+-rw-r--r--   0        0        0    12079 2023-06-09 21:31:43.105292 vertex_protocol-0.1.2/vertex_protocol/indexer_client/types/query.py
+-rw-r--r--   0        0        0      933 2023-06-09 21:31:43.105292 vertex_protocol-0.1.2/vertex_protocol/utils/__init__.py
+-rw-r--r--   0        0        0      341 2023-06-09 21:31:43.105292 vertex_protocol-0.1.2/vertex_protocol/utils/backend.py
+-rw-r--r--   0        0        0     5216 2023-06-09 21:31:43.105292 vertex_protocol-0.1.2/vertex_protocol/utils/bytes32.py
+-rw-r--r--   0        0        0       99 2023-06-09 21:31:43.105292 vertex_protocol-0.1.2/vertex_protocol/utils/enum.py
+-rw-r--r--   0        0        0     1136 2023-06-09 21:31:43.105292 vertex_protocol-0.1.2/vertex_protocol/utils/exceptions.py
+-rw-r--r--   0        0        0     1094 2023-06-09 21:31:43.105292 vertex_protocol-0.1.2/vertex_protocol/utils/expiration.py
+-rw-r--r--   0        0        0      927 2023-06-09 21:31:43.105292 vertex_protocol-0.1.2/vertex_protocol/utils/math.py
+-rw-r--r--   0        0        0     1887 2023-06-09 21:31:43.109292 vertex_protocol-0.1.2/vertex_protocol/utils/model.py
+-rw-r--r--   0        0        0      809 2023-06-09 21:31:43.109292 vertex_protocol-0.1.2/vertex_protocol/utils/nonce.py
+-rw-r--r--   0        0        0      491 2023-06-09 21:31:43.109292 vertex_protocol-0.1.2/vertex_protocol/utils/subaccount.py
+-rw-r--r--   0        0        0     1715 1970-01-01 00:00:00.000000 vertex_protocol-0.1.2/PKG-INFO
```

### Comparing `vertex_protocol-0.1.1/README.md` & `vertex_protocol-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.1/vertex_protocol/client/__init__.py` & `vertex_protocol-0.1.2/vertex_protocol/client/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.1/vertex_protocol/client/apis/__init__.py` & `vertex_protocol-0.1.2/vertex_protocol/client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.1/vertex_protocol/client/apis/base.py` & `vertex_protocol-0.1.2/vertex_protocol/client/apis/base.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.1/vertex_protocol/client/apis/market/__init__.py` & `vertex_protocol-0.1.2/vertex_protocol/client/apis/market/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.1/vertex_protocol/client/apis/market/execute.py` & `vertex_protocol-0.1.2/vertex_protocol/client/apis/market/execute.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.1/vertex_protocol/client/apis/market/query.py` & `vertex_protocol-0.1.2/vertex_protocol/client/apis/market/query.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.1/vertex_protocol/client/apis/perp/__init__.py` & `vertex_protocol-0.1.2/vertex_protocol/client/apis/perp/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.1/vertex_protocol/client/apis/perp/query.py` & `vertex_protocol-0.1.2/vertex_protocol/client/apis/perp/query.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.1/vertex_protocol/client/apis/spot/__init__.py` & `vertex_protocol-0.1.2/vertex_protocol/client/apis/spot/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.1/vertex_protocol/client/apis/spot/base.py` & `vertex_protocol-0.1.2/vertex_protocol/client/apis/spot/base.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.1/vertex_protocol/client/apis/spot/execute.py` & `vertex_protocol-0.1.2/vertex_protocol/client/apis/spot/execute.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.1/vertex_protocol/client/apis/spot/query.py` & `vertex_protocol-0.1.2/vertex_protocol/client/apis/spot/query.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.1/vertex_protocol/client/apis/subaccount/__init__.py` & `vertex_protocol-0.1.2/vertex_protocol/client/apis/subaccount/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.1/vertex_protocol/client/apis/subaccount/execute.py` & `vertex_protocol-0.1.2/vertex_protocol/client/apis/subaccount/execute.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.1/vertex_protocol/client/apis/subaccount/query.py` & `vertex_protocol-0.1.2/vertex_protocol/client/apis/subaccount/query.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.1/vertex_protocol/client/context.py` & `vertex_protocol-0.1.2/vertex_protocol/client/context.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.1/vertex_protocol/contracts/__init__.py` & `vertex_protocol-0.1.2/vertex_protocol/contracts/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,18 +7,14 @@
 from web3.contract.contract import ContractFunction
 from eth_account.signers.local import LocalAccount
 from vertex_protocol.contracts.loader import load_abi
 from vertex_protocol.contracts.types import DepositCollateralParams, VertexAbiName
 from vertex_protocol.utils.bytes32 import subaccount_name_to_bytes12, zero_address
 from vertex_protocol.utils.exceptions import InvalidProductId
 from vertex_protocol.contracts.types import *
-from vertex_protocol.contracts.eip712 import *
-from vertex_protocol.contracts.eip712.domain import *
-from vertex_protocol.contracts.eip712.sign import *
-from vertex_protocol.contracts.eip712.types import *
 
 
 class VertexContractsContext(BaseModel):
     """
     Holds the context for various Vertex contracts.
 
     Attributes:
@@ -217,8 +213,11 @@
 
 
 __all__ = [
     "VertexContractsContext",
     "VertexContracts",
     "DepositCollateralParams",
     "VertexExecuteType",
+    "VertexNetwork",
+    "VertexAbiName",
+    "VertexDeployment",
 ]
```

### Comparing `vertex_protocol-0.1.1/vertex_protocol/contracts/abis/Endpoint.json` & `vertex_protocol-0.1.2/vertex_protocol/contracts/abis/Endpoint.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.1/vertex_protocol/contracts/abis/FQuerier.json` & `vertex_protocol-0.1.2/vertex_protocol/contracts/abis/FQuerier.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.1/vertex_protocol/contracts/abis/IClearinghouse.json` & `vertex_protocol-0.1.2/vertex_protocol/contracts/abis/IClearinghouse.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.1/vertex_protocol/contracts/abis/IERC20.json` & `vertex_protocol-0.1.2/vertex_protocol/contracts/abis/IERC20.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.1/vertex_protocol/contracts/abis/IEndpoint.json` & `vertex_protocol-0.1.2/vertex_protocol/contracts/abis/IEndpoint.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.1/vertex_protocol/contracts/abis/IOffchainBook.json` & `vertex_protocol-0.1.2/vertex_protocol/contracts/abis/IOffchainBook.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.1/vertex_protocol/contracts/abis/IPerpEngine.json` & `vertex_protocol-0.1.2/vertex_protocol/contracts/abis/IPerpEngine.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.1/vertex_protocol/contracts/abis/IProductEngine.json` & `vertex_protocol-0.1.2/vertex_protocol/contracts/abis/IProductEngine.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.1/vertex_protocol/contracts/abis/ISpotEngine.json` & `vertex_protocol-0.1.2/vertex_protocol/contracts/abis/ISpotEngine.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.1/vertex_protocol/contracts/abis/MockERC20.json` & `vertex_protocol-0.1.2/vertex_protocol/contracts/abis/MockERC20.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.1/vertex_protocol/contracts/deployments/deployment.arbitrumGoerli.json` & `vertex_protocol-0.1.2/vertex_protocol/contracts/deployments/deployment.arbitrumOne.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5%*

 * *Differences: {"'clearinghouse'": "'0xAE1ec28d6225dCE2ff787dcb8CE11cF6D3AE064f'",*

 * * "'clearinghouseLiq'": "'0xA22e80900b8A7929D9DC8Ebb81b4a7Cb6267325a'",*

 * * "'deployer'": "'0xB746472C10f9F128FF9F5029f424cC91bb1D8C3a'",*

 * * "'endpoint'": "'0xbbEE07B3e8121227AfCFe1E2B82772246226128e'",*

 * * "'explorerUrl'": "'https://explorer.arbitrum.io'",*

 * * "'feeCalculator'": "'0x2259440579447D0625a5E28dfF3E743d207e8890'",*

 * * "'nodeUrl'": "'https://arb1.arbitrum.io/rpc'",*

 * * "'perpEngine'": "'0xb74C78cca0FADAFBeE52B2f48A67eE8c834b5fd1'",*

 * * "'querier'":  […]*

```diff
@@ -1,17 +1,17 @@
 {
-    "clearinghouse": "0x66256D9663fc368A1285d94E58615B0bf2Ac38f4",
-    "clearinghouseLiq": "0xF3ba85Fa07cC5a3bF2b497c9DA29326b94D6BD64",
-    "deployer": "0x3c06e307BA6Ab81E8Ff6661c1559ce8027744AE5",
-    "endpoint": "0xBF16E41fb4AC9922545bfc1500F67064dc2dcC3B",
-    "explorerUrl": "https://goerli-rollup-explorer.arbitrum.io",
-    "feeCalculator": "0xb49Fb5Fbcd83c37BA843193bD4B7c8BE8567317d",
-    "nodeUrl": "https://goerli-rollup.arbitrum.io/rpc",
-    "perpEngine": "0xb5c1dF73e4e5498A9472d27B40A1285b1B83C2d4",
-    "querier": "0x1A599F3C70d6266C5744cd3a73d2AFAb57E32289",
-    "quote": "0x179522635726710Dd7D2035a81d856de4Aa7836c",
-    "spotEngine": "0x4764083CdA637ff5335326b7e53b3f544E633870",
-    "startBlock": 7648965,
-    "subgraphCandleSticksUrl": "https://api.thegraph.com/subgraphs/name/vertex-protocol/vertex-goerli-candlesticks",
-    "subgraphCoreUrl": "https://api.thegraph.com/subgraphs/name/vertex-protocol/vertex-goerli-core",
-    "subgraphMarketsUrl": "https://api.thegraph.com/subgraphs/name/vertex-protocol/vertex-goerli-markets"
+    "clearinghouse": "0xAE1ec28d6225dCE2ff787dcb8CE11cF6D3AE064f",
+    "clearinghouseLiq": "0xA22e80900b8A7929D9DC8Ebb81b4a7Cb6267325a",
+    "deployer": "0xB746472C10f9F128FF9F5029f424cC91bb1D8C3a",
+    "endpoint": "0xbbEE07B3e8121227AfCFe1E2B82772246226128e",
+    "explorerUrl": "https://explorer.arbitrum.io",
+    "feeCalculator": "0x2259440579447D0625a5E28dfF3E743d207e8890",
+    "nodeUrl": "https://arb1.arbitrum.io/rpc",
+    "perpEngine": "0xb74C78cca0FADAFBeE52B2f48A67eE8c834b5fd1",
+    "querier": "0x1693273B443699bee277eCbc60e2C8027E91995d",
+    "quote": "0xff970a61a04b1ca14834a43f5de4533ebddb5cc8",
+    "spotEngine": "0x32d91Af2B17054D575A7bF1ACfa7615f41CCEfaB",
+    "startBlock": 67108377,
+    "subgraphCandleSticksUrl": "https://api.thegraph.com/subgraphs/name/vertex-protocol/vertex-prod-candlesticks",
+    "subgraphCoreUrl": "https://api.thegraph.com/subgraphs/name/vertex-protocol/vertex-prod-core",
+    "subgraphMarketsUrl": "https://api.thegraph.com/subgraphs/name/vertex-protocol/vertex-prod-markets"
 }
```

### Comparing `vertex_protocol-0.1.1/vertex_protocol/contracts/deployments/deployment.arbitrumOne.json` & `vertex_protocol-0.1.2/vertex_protocol/contracts/deployments/deployment.arbitrumGoerli.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5%*

 * *Differences: {"'clearinghouse'": "'0x61B10E98049B00d4D863e3637D9E14Acd23ad8a3'",*

 * * "'clearinghouseLiq'": "'0x0Ad860cdd3e7d427EebeDaC925a57a0628198f4E'",*

 * * "'deployer'": "'0x3c06e307BA6Ab81E8Ff6661c1559ce8027744AE5'",*

 * * "'endpoint'": "'0x5956D6f55011678b2CAB217cD21626F7668ba6c5'",*

 * * "'explorerUrl'": "'https://goerli-rollup-explorer.arbitrum.io'",*

 * * "'feeCalculator'": "'0xd783855BF9c238eEd6152b370Bf860863E63F432'",*

 * * "'nodeUrl'": "'https://goerli-rollup.arbitrum.io/rpc'",*

 * * "'perpEngine'": "'0xa18fd8DA4F3c919a57ae7083b20cB4f3336 […]*

```diff
@@ -1,17 +1,17 @@
 {
-    "clearinghouse": "0xAE1ec28d6225dCE2ff787dcb8CE11cF6D3AE064f",
-    "clearinghouseLiq": "0xA22e80900b8A7929D9DC8Ebb81b4a7Cb6267325a",
-    "deployer": "0xB746472C10f9F128FF9F5029f424cC91bb1D8C3a",
-    "endpoint": "0xbbEE07B3e8121227AfCFe1E2B82772246226128e",
-    "explorerUrl": "https://explorer.arbitrum.io",
-    "feeCalculator": "0x2259440579447D0625a5E28dfF3E743d207e8890",
-    "nodeUrl": "https://arb1.arbitrum.io/rpc",
-    "perpEngine": "0xb74C78cca0FADAFBeE52B2f48A67eE8c834b5fd1",
-    "querier": "0x1693273B443699bee277eCbc60e2C8027E91995d",
-    "quote": "0xff970a61a04b1ca14834a43f5de4533ebddb5cc8",
-    "spotEngine": "0x32d91Af2B17054D575A7bF1ACfa7615f41CCEfaB",
-    "startBlock": 67108377,
-    "subgraphCandleSticksUrl": "https://api.thegraph.com/subgraphs/name/vertex-protocol/vertex-prod-candlesticks",
-    "subgraphCoreUrl": "https://api.thegraph.com/subgraphs/name/vertex-protocol/vertex-prod-core",
-    "subgraphMarketsUrl": "https://api.thegraph.com/subgraphs/name/vertex-protocol/vertex-prod-markets"
+    "clearinghouse": "0x61B10E98049B00d4D863e3637D9E14Acd23ad8a3",
+    "clearinghouseLiq": "0x0Ad860cdd3e7d427EebeDaC925a57a0628198f4E",
+    "deployer": "0x3c06e307BA6Ab81E8Ff6661c1559ce8027744AE5",
+    "endpoint": "0x5956D6f55011678b2CAB217cD21626F7668ba6c5",
+    "explorerUrl": "https://goerli-rollup-explorer.arbitrum.io",
+    "feeCalculator": "0xd783855BF9c238eEd6152b370Bf860863E63F432",
+    "nodeUrl": "https://goerli-rollup.arbitrum.io/rpc",
+    "perpEngine": "0xa18fd8DA4F3c919a57ae7083b20cB4f333645795",
+    "querier": "0xFc69d0f1d70825248C9F9582d13F93D60b6b56De",
+    "quote": "0x179522635726710Dd7D2035a81d856de4Aa7836c",
+    "spotEngine": "0x960a7C6D35EC89A1294E1B7383292f211Fe8CA1d",
+    "startBlock": 24870025,
+    "subgraphCandleSticksUrl": "https://api.thegraph.com/subgraphs/name/vertex-protocol/vertex-dev-candlesticks",
+    "subgraphCoreUrl": "https://api.thegraph.com/subgraphs/name/vertex-protocol/vertex-dev-core",
+    "subgraphMarketsUrl": "https://api.thegraph.com/subgraphs/name/vertex-protocol/vertex-dev-markets"
 }
```

### Comparing `vertex_protocol-0.1.1/vertex_protocol/contracts/deployments/deployment.test.json` & `vertex_protocol-0.1.2/vertex_protocol/contracts/deployments/deployment.test.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.1/vertex_protocol/contracts/eip712/domain.py` & `vertex_protocol-0.1.2/vertex_protocol/contracts/eip712/domain.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from vertex_protocol.contracts.eip712 import EIP712Domain
+from vertex_protocol.contracts.eip712.types import EIP712Domain
 
 
 def get_vertex_eip712_domain(verifying_contract: str, chain_id: int) -> EIP712Domain:
     """
     Util to create an EIP712Domain instance specific to Vertex.
 
     Args:
```

### Comparing `vertex_protocol-0.1.1/vertex_protocol/contracts/eip712/sign.py` & `vertex_protocol-0.1.2/vertex_protocol/contracts/eip712/sign.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from eth_account.signers.local import LocalAccount
-from vertex_protocol.contracts.eip712 import EIP712TypedData, EIP712Types
 from vertex_protocol.contracts.eip712.domain import (
     get_eip712_domain_type,
     get_vertex_eip712_domain,
 )
-from vertex_protocol.contracts.eip712.types import get_vertex_eip712_type
+from vertex_protocol.contracts.eip712.types import (
+    EIP712TypedData,
+    EIP712Types,
+    get_vertex_eip712_type,
+)
 from eth_account.messages import encode_structured_data, _hash_eip191_message
 
 from vertex_protocol.contracts.types import VertexExecuteType
 
 
 def build_eip712_typed_data(
     execute: VertexExecuteType, msg: dict, verifying_contract: str, chain_id: int
```

### Comparing `vertex_protocol-0.1.1/vertex_protocol/contracts/loader.py` & `vertex_protocol-0.1.2/vertex_protocol/contracts/loader.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.1/vertex_protocol/contracts/types.py` & `vertex_protocol-0.1.2/vertex_protocol/contracts/types.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.1/vertex_protocol/engine_client/__init__.py` & `vertex_protocol-0.1.2/vertex_protocol/engine_client/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.1/vertex_protocol/engine_client/execute.py` & `vertex_protocol-0.1.2/vertex_protocol/engine_client/execute.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.1/vertex_protocol/engine_client/query.py` & `vertex_protocol-0.1.2/vertex_protocol/engine_client/query.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.1/vertex_protocol/engine_client/types/execute.py` & `vertex_protocol-0.1.2/vertex_protocol/engine_client/types/execute.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,34 +72,40 @@
 
 class OrderParams(BaseParams):
     """
     Class for defining the parameters of an order.
 
     Attributes:
         priceX18 (int): The price of the order with a precision of 18 decimal places.
+
         amount (int): The amount of the asset to be bought or sold in the order.
+
         expiration (int): The unix timestamp at which the order will expire.
+
         nonce (int): A unique number used to prevent replay attacks. By default, a new nonce is generated.
-            see `gen_order_nonce` for more info.
+        see `gen_order_nonce` for more info.
     """
 
     priceX18: int
     amount: int
     expiration: int
     nonce: int = gen_order_nonce()
 
 
 class PlaceOrderParams(SignatureParams):
     """
     Class for defining the parameters needed to place an order.
 
     Attributes:
         product_id (int): The id of the product for which the order is being placed.
+
         order (OrderParams): The parameters of the order.
+
         digest (Optional[str]): An optional hash of the order data.
+
         spot_leverage (Optional[bool]): An optional flag indicating whether leverage should be used for the order. By default, leverage is assumed.
     """
 
     product_id: int
     order: OrderParams
     digest: Optional[str]
     spot_leverage: Optional[bool]
@@ -150,32 +156,37 @@
 
 class WithdrawCollateralParams(BaseParamsSigned):
     """
     Parameters required to withdraw collateral from a specific product.
 
     Attributes:
         productId (int): The ID of the product to withdraw collateral from.
+
         amount (int): The amount of collateral to be withdrawn.
+
         spot_leverage (Optional[bool]): Indicates whether leverage is to be used. Defaults to True.
-            If set to False, the transaction fails if it causes a borrow on the subaccount.
+        If set to False, the transaction fails if it causes a borrow on the subaccount.
     """
 
     productId: int
     amount: int
     spot_leverage: Optional[bool]
 
 
 class LiquidateSubaccountParams(BaseParamsSigned):
     """
     Parameters required to liquidate a subaccount.
 
     Attributes:
         liquidatee (Subaccount): The subaccount that is to be liquidated.
+
         mode (int): The mode of liquidation.
+
         healthGroup (int): The ID of the health group associated with the product being traded.
+
         amount (int): The amount to be liquidated.
 
     Methods:
         serialize_liquidatee(cls, v: Subaccount) -> bytes: Validates and converts the liquidatee subaccount to bytes32 format.
     """
 
     liquidatee: Subaccount
@@ -190,19 +201,23 @@
 
 class MintLpParams(BaseParamsSigned):
     """
     Parameters required for minting a liquidity provider token for a specific product in a subaccount.
 
     Attributes:
         productId (int): The ID of the product.
+
         amountBase (int): The amount of base to be consumed by minting LPs multiplied by 1e18.
+
         quoteAmountLow (int): The minimum amount of quote to be consumed by minting LPs multiplied by 1e18.
+
         quoteAmountHigh (int): The maximum amount of quote to be consumed by minting LPs multiplied by 1e18.
+
         spot_leverage (Optional[bool]): Indicates whether leverage is to be used. Defaults to True.
-            If set to False, the transaction fails if it causes a borrow on the subaccount.
+        If set to False, the transaction fails if it causes a borrow on the subaccount.
     """
 
     productId: int
     amountBase: int
     quoteAmountLow: int
     quoteAmountHigh: int
     spot_leverage: Optional[bool]
@@ -211,14 +226,15 @@
 class BurnLpParams(BaseParamsSigned):
     """
     This class represents the parameters required to burn a liquidity provider
     token for a specific product in a subaccount.
 
     Attributes:
         productId (int): The ID of the product.
+
         amount (int): Combined amount of base + quote to burn multiplied by 1e18.
     """
 
     productId: int
     amount: int
 
 
@@ -279,17 +295,20 @@
 
 class TxRequest(VertexBaseModel):
     """
     Parameters for a transaction request.
 
     Attributes:
         tx (dict): The transaction details.
+
         signature (str): The signature for the transaction.
+
         spot_leverage (Optional[bool]): Indicates whether leverage should be used. If set to false,
-            it denotes no borrowing. Defaults to true.
+        it denotes no borrowing. Defaults to true.
+
         digest (Optional[str]): The digest of the transaction.
 
     Methods:
         serialize: Validates and serializes the transaction parameters.
     """
 
     tx: dict
@@ -348,14 +367,15 @@
     Parameters for a cancel orders request.
 
     Attributes:
         cancel_orders (CancelOrdersParams): The parameters of the orders to be cancelled.
 
     Methods:
         serialize: Serializes 'digests' in 'cancel_orders' into their hexadecimal representation.
+
         to_tx_request: Validates and converts 'cancel_orders' into a transaction request.
     """
 
     cancel_orders: CancelOrdersParams
 
     @validator("cancel_orders")
     def serialize(cls, v: CancelOrdersParams) -> CancelOrdersParams:
@@ -395,14 +415,15 @@
     Parameters for a withdraw collateral request.
 
     Attributes:
         withdraw_collateral (WithdrawCollateralParams): The parameters of the collateral to be withdrawn.
 
     Methods:
         serialize: Validates and converts the 'amount' attribute of 'withdraw_collateral' to string.
+
         to_tx_request: Validates and converts 'withdraw_collateral' into a transaction request.
     """
 
     withdraw_collateral: WithdrawCollateralParams
 
     @validator("withdraw_collateral")
     def serialize(cls, v: WithdrawCollateralParams) -> WithdrawCollateralParams:
@@ -417,15 +438,16 @@
     Parameters for a liquidate subaccount request.
 
     Attributes:
         liquidate_subaccount (LiquidateSubaccountParams): The parameters for the subaccount to be liquidated.
 
     Methods:
         serialize: Validates and converts the 'amount' attribute and the 'liquidatee' attribute
-                   of 'liquidate_subaccount' to their proper serialized forms.
+        of 'liquidate_subaccount' to their proper serialized forms.
+
         to_tx_request: Validates and converts 'liquidate_subaccount' into a transaction request.
     """
 
     liquidate_subaccount: LiquidateSubaccountParams
 
     @validator("liquidate_subaccount")
     def serialize(cls, v: LiquidateSubaccountParams) -> LiquidateSubaccountParams:
@@ -441,15 +463,16 @@
     Parameters for a mint LP request.
 
     Attributes:
         mint_lp (MintLpParams): The parameters for minting liquidity.
 
     Methods:
         serialize: Validates and converts the 'amountBase', 'quoteAmountLow', and 'quoteAmountHigh'
-                   attributes of 'mint_lp' to their proper serialized forms.
+        attributes of 'mint_lp' to their proper serialized forms.
+
         to_tx_request: Validates and converts 'mint_lp' into a transaction request.
     """
 
     mint_lp: MintLpParams
 
     @validator("mint_lp")
     def serialize(cls, v: MintLpParams) -> MintLpParams:
@@ -464,14 +487,15 @@
     Parameters for a burn LP request.
 
     Attributes:
         burn_lp (BurnLpParams): The parameters for burning liquidity.
 
     Methods:
         serialize: Validates and converts the 'amount' attribute of 'burn_lp' to its proper serialized form.
+
         to_tx_request: Validates and converts 'burn_lp' into a transaction request.
     """
 
     burn_lp: BurnLpParams
 
     @validator("burn_lp")
     def serialize(cls, v: BurnLpParams) -> BurnLpParams:
@@ -486,14 +510,15 @@
     Parameters for a request to link a signer to a subaccount.
 
     Attributes:
         link_signer (LinkSignerParams): Parameters including the subaccount to be linked.
 
     Methods:
         serialize: Validates and converts the 'signer' attribute of 'link_signer' into its hexadecimal representation.
+
         to_tx_request: Validates and converts 'link_signer' into a transaction request.
     """
 
     link_signer: LinkSignerParams
 
     @validator("link_signer")
     def serialize(cls, v: LinkSignerParams) -> LinkSignerParams:
@@ -517,17 +542,21 @@
 
 class ExecuteResponse(VertexBaseModel):
     """
     Represents the response returned from executing a request.
 
     Attributes:
         status (ResponseStatus): The status of the response.
+
         signature (Optional[str]): The signature of the response. Only present if the request was successfully executed.
+
         error_code (Optional[int]): The error code, if any error occurred during the execution of the request.
+
         error (Optional[str]): The error message, if any error occurred during the execution of the request.
+
         req (Optional[dict]): The original request that was executed.
     """
 
     status: ResponseStatus
     signature: Optional[str]
     error_code: Optional[int]
     error: Optional[str]
```

### Comparing `vertex_protocol-0.1.1/vertex_protocol/engine_client/types/models.py` & `vertex_protocol-0.1.2/vertex_protocol/engine_client/types/models.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.1/vertex_protocol/engine_client/types/query.py` & `vertex_protocol-0.1.2/vertex_protocol/engine_client/types/query.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.1/vertex_protocol/indexer_client/__init__.py` & `vertex_protocol-0.1.2/vertex_protocol/indexer_client/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.1/vertex_protocol/indexer_client/query.py` & `vertex_protocol-0.1.2/vertex_protocol/indexer_client/query.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.1/vertex_protocol/indexer_client/types/models.py` & `vertex_protocol-0.1.2/vertex_protocol/indexer_client/types/models.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.1/vertex_protocol/indexer_client/types/query.py` & `vertex_protocol-0.1.2/vertex_protocol/indexer_client/types/query.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.1/vertex_protocol/utils/__init__.py` & `vertex_protocol-0.1.2/vertex_protocol/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.1/vertex_protocol/utils/bytes32.py` & `vertex_protocol-0.1.2/vertex_protocol/utils/bytes32.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.1/vertex_protocol/utils/exceptions.py` & `vertex_protocol-0.1.2/vertex_protocol/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.1/vertex_protocol/utils/expiration.py` & `vertex_protocol-0.1.2/vertex_protocol/utils/expiration.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.1/vertex_protocol/utils/math.py` & `vertex_protocol-0.1.2/vertex_protocol/utils/math.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.1/vertex_protocol/utils/model.py` & `vertex_protocol-0.1.2/vertex_protocol/utils/model.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.1/vertex_protocol/utils/nonce.py` & `vertex_protocol-0.1.2/vertex_protocol/utils/nonce.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.1/PKG-INFO` & `vertex_protocol-0.1.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 Metadata-Version: 2.1
 Name: vertex-protocol
-Version: 0.1.1
+Version: 0.1.2
 Summary: Vertex Protocol SDK
+Home-page: https://vertexprotocol.com/
 Keywords: vertex protocol,vertex sdk,vertex protocol api
 Author: Jeury Mejia
 Author-email: jeury@vertexprotocol.com
+Maintainer: Frank Jia
+Maintainer-email: frank@vertexprotocol.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: eth-account (>=0.8.0,<0.9.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: web3 (>=6.4.0,<7.0.0)
+Project-URL: Documentation, https://vertex-protocol.github.io/vertex-python-sdk/
 Description-Content-Type: text/markdown
 
 # Vertex Python SDK
 
 ```python
 print("Hello Vertex")
 ```
```

