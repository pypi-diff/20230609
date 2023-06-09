# Comparing `tmp/huma_signals-0.2.1.tar.gz` & `tmp/huma_signals-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huma_signals-0.2.1.tar", max compression
+gzip compressed data, was "huma_signals-0.3.0.tar", max compression
```

## Comparing `huma_signals-0.2.1.tar` & `huma_signals-0.3.0.tar`

### file list

```diff
@@ -1,52 +1,56 @@
--rw-r--r--   0        0        0    34523 2023-05-06 00:10:02.616918 huma_signals-0.2.1/LICENSE
--rw-r--r--   0        0        0     2162 2023-05-17 23:08:07.445627 huma_signals-0.2.1/README.md
--rw-r--r--   0        0        0        0 2023-05-06 00:10:02.617555 huma_signals-0.2.1/huma_signals/__init__.py
--rw-r--r--   0        0        0        0 2023-05-17 01:58:33.941065 huma_signals-0.2.1/huma_signals/adapters/__init__.py
--rw-r--r--   0        0        0      586 2023-05-17 01:58:33.941184 huma_signals-0.2.1/huma_signals/adapters/ethereum_wallet/README.md
--rw-r--r--   0        0        0        0 2023-05-17 01:58:33.941215 huma_signals-0.2.1/huma_signals/adapters/ethereum_wallet/__init__.py
--rw-r--r--   0        0        0     3295 2023-05-17 01:58:33.941390 huma_signals-0.2.1/huma_signals/adapters/ethereum_wallet/adapter.py
--rw-r--r--   0        0        0      186 2023-05-17 01:58:33.941462 huma_signals-0.2.1/huma_signals/adapters/ethereum_wallet/settings.py
--rw-r--r--   0        0        0      586 2023-05-17 01:58:33.941558 huma_signals-0.2.1/huma_signals/adapters/lending_pools/README.md
--rw-r--r--   0        0        0        0 2023-05-17 01:58:33.941588 huma_signals-0.2.1/huma_signals/adapters/lending_pools/__init__.py
--rw-r--r--   0        0        0    23699 2023-05-17 01:58:33.941733 huma_signals-0.2.1/huma_signals/adapters/lending_pools/abi/BaseCreditPool.json
--rw-r--r--   0        0        0    30632 2023-05-17 01:58:33.941925 huma_signals-0.2.1/huma_signals/adapters/lending_pools/abi/BasePoolConfig.json
--rw-r--r--   0        0        0    32155 2023-05-17 01:58:33.942012 huma_signals-0.2.1/huma_signals/adapters/lending_pools/abi/ReceivableFactoringPool.json
--rw-r--r--   0        0        0    30290 2023-05-17 01:58:33.942126 huma_signals-0.2.1/huma_signals/adapters/lending_pools/abi/SuperfluidFactoringPool.json
--rw-r--r--   0        0        0     4719 2023-05-17 01:58:33.942333 huma_signals-0.2.1/huma_signals/adapters/lending_pools/adapter.py
--rw-r--r--   0        0        0     1938 2023-05-17 01:58:33.942403 huma_signals-0.2.1/huma_signals/adapters/lending_pools/registry.py
--rw-r--r--   0        0        0      158 2023-05-17 01:58:33.942479 huma_signals-0.2.1/huma_signals/adapters/lending_pools/settings.py
--rw-r--r--   0        0        0      582 2023-05-17 01:58:33.942545 huma_signals-0.2.1/huma_signals/adapters/models.py
--rw-r--r--   0        0        0      591 2023-05-17 01:58:33.942633 huma_signals-0.2.1/huma_signals/adapters/polygon_wallet/README.md
--rw-r--r--   0        0        0        0 2023-05-17 01:58:33.942663 huma_signals-0.2.1/huma_signals/adapters/polygon_wallet/__init__.py
--rw-r--r--   0        0        0     3406 2023-05-17 01:58:33.942804 huma_signals-0.2.1/huma_signals/adapters/polygon_wallet/adapter.py
--rw-r--r--   0        0        0      222 2023-05-17 01:58:33.942860 huma_signals-0.2.1/huma_signals/adapters/polygon_wallet/settings.py
--rw-r--r--   0        0        0      576 2023-05-17 01:58:33.942959 huma_signals-0.2.1/huma_signals/adapters/request_network/README.md
--rw-r--r--   0        0        0        0 2023-05-17 01:58:33.942989 huma_signals-0.2.1/huma_signals/adapters/request_network/__init__.py
--rw-r--r--   0        0        0     4372 2023-05-17 01:58:33.943071 huma_signals-0.2.1/huma_signals/adapters/request_network/models.py
--rw-r--r--   0        0        0     5889 2023-05-17 01:58:33.943221 huma_signals-0.2.1/huma_signals/adapters/request_network/request_invoice_adapter.py
--rw-r--r--   0        0        0     5202 2023-05-17 01:58:33.943386 huma_signals-0.2.1/huma_signals/adapters/request_network/request_transaction_adapter.py
--rw-r--r--   0        0        0      284 2023-05-17 01:58:33.943449 huma_signals-0.2.1/huma_signals/adapters/request_network/settings.py
--rw-r--r--   0        0        0        0 2023-05-17 01:58:33.943514 huma_signals-0.2.1/huma_signals/clients/__init__.py
--rw-r--r--   0        0        0        0 2023-05-17 01:58:33.943585 huma_signals-0.2.1/huma_signals/clients/eth_client/__init__.py
--rw-r--r--   0        0        0     1427 2023-05-17 01:58:33.943803 huma_signals-0.2.1/huma_signals/clients/eth_client/eth_client.py
--rw-r--r--   0        0        0      673 2023-05-17 01:58:33.943860 huma_signals-0.2.1/huma_signals/clients/eth_client/eth_types.py
--rw-r--r--   0        0        0        0 2023-05-17 01:58:33.943913 huma_signals-0.2.1/huma_signals/clients/polygon_client/__init__.py
--rw-r--r--   0        0        0     1503 2023-05-17 01:58:33.944103 huma_signals-0.2.1/huma_signals/clients/polygon_client/polygon_client.py
--rw-r--r--   0        0        0      685 2023-05-17 01:58:33.944154 huma_signals-0.2.1/huma_signals/clients/polygon_client/polygon_types.py
--rw-r--r--   0        0        0        0 2023-05-17 01:58:33.944206 huma_signals-0.2.1/huma_signals/clients/request_client/__init__.py
--rw-r--r--   0        0        0     8129 2023-05-17 01:58:33.944358 huma_signals-0.2.1/huma_signals/clients/request_client/request_client.py
--rw-r--r--   0        0        0      900 2023-05-17 01:58:33.944420 huma_signals-0.2.1/huma_signals/clients/request_client/request_types.py
--rw-r--r--   0        0        0        0 2023-05-06 00:10:02.617961 huma_signals-0.2.1/huma_signals/commons/__init__.py
--rw-r--r--   0        0        0      291 2023-05-17 01:58:33.944586 huma_signals-0.2.1/huma_signals/commons/chains.py
--rw-r--r--   0        0        0      330 2023-05-06 00:10:02.618090 huma_signals-0.2.1/huma_signals/commons/datetime_utils.py
--rw-r--r--   0        0        0      227 2023-05-06 00:10:02.618146 huma_signals-0.2.1/huma_signals/commons/pydantic_utils.py
--rw-r--r--   0        0        0      569 2023-05-06 00:10:02.618202 huma_signals-0.2.1/huma_signals/commons/string_utils.py
--rw-r--r--   0        0        0     1309 2023-05-06 00:10:02.618262 huma_signals-0.2.1/huma_signals/commons/tokens.py
--rw-r--r--   0        0        0     1078 2023-05-06 00:10:02.618330 huma_signals-0.2.1/huma_signals/commons/web3_utils.py
--rw-r--r--   0        0        0      499 2023-05-17 22:38:39.621240 huma_signals-0.2.1/huma_signals/dotenv/example.env
--rw-r--r--   0        0        0      946 2023-05-17 01:36:29.827407 huma_signals-0.2.1/huma_signals/exceptions.py
--rw-r--r--   0        0        0      322 2023-05-06 00:10:02.621231 huma_signals-0.2.1/huma_signals/models.py
--rw-r--r--   0        0        0        0 2023-05-10 00:22:05.269455 huma_signals-0.2.1/huma_signals/py.typed
--rw-r--r--   0        0        0     1563 2023-05-17 22:38:39.621299 huma_signals-0.2.1/huma_signals/settings.py
--rw-r--r--   0        0        0     2792 2023-05-17 23:08:07.445943 huma_signals-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     3110 1970-01-01 00:00:00.000000 huma_signals-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-06-09 00:12:10.919306 huma_signals-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2162 2023-06-09 00:12:10.919306 huma_signals-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-09 00:12:10.919306 huma_signals-0.3.0/huma_signals/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-09 00:12:10.919306 huma_signals-0.3.0/huma_signals/adapters/__init__.py
+-rw-r--r--   0        0        0      586 2023-06-09 00:12:10.919306 huma_signals-0.3.0/huma_signals/adapters/ethereum_wallet/README.md
+-rw-r--r--   0        0        0        0 2023-06-09 00:12:10.919306 huma_signals-0.3.0/huma_signals/adapters/ethereum_wallet/__init__.py
+-rw-r--r--   0        0        0     3088 2023-06-09 00:12:10.919306 huma_signals-0.3.0/huma_signals/adapters/ethereum_wallet/adapter.py
+-rw-r--r--   0        0        0      186 2023-06-09 00:12:10.919306 huma_signals-0.3.0/huma_signals/adapters/ethereum_wallet/settings.py
+-rw-r--r--   0        0        0      586 2023-06-09 00:12:10.919306 huma_signals-0.3.0/huma_signals/adapters/lending_pools/README.md
+-rw-r--r--   0        0        0        0 2023-06-09 00:12:10.919306 huma_signals-0.3.0/huma_signals/adapters/lending_pools/__init__.py
+-rw-r--r--   0        0        0    23699 2023-06-09 00:12:10.919306 huma_signals-0.3.0/huma_signals/adapters/lending_pools/abi/BaseCreditPool.json
+-rw-r--r--   0        0        0    30632 2023-06-09 00:12:10.919306 huma_signals-0.3.0/huma_signals/adapters/lending_pools/abi/BasePoolConfig.json
+-rw-r--r--   0        0        0    32155 2023-06-09 00:12:10.919306 huma_signals-0.3.0/huma_signals/adapters/lending_pools/abi/ReceivableFactoringPool.json
+-rw-r--r--   0        0        0    30290 2023-06-09 00:12:10.919306 huma_signals-0.3.0/huma_signals/adapters/lending_pools/abi/SuperfluidFactoringPool.json
+-rw-r--r--   0        0        0     4533 2023-06-09 00:12:10.919306 huma_signals-0.3.0/huma_signals/adapters/lending_pools/adapter.py
+-rw-r--r--   0        0        0     1938 2023-06-09 00:12:10.919306 huma_signals-0.3.0/huma_signals/adapters/lending_pools/registry.py
+-rw-r--r--   0        0        0      158 2023-06-09 00:12:10.919306 huma_signals-0.3.0/huma_signals/adapters/lending_pools/settings.py
+-rw-r--r--   0        0        0      145 2023-06-09 00:12:10.919306 huma_signals-0.3.0/huma_signals/adapters/models.py
+-rw-r--r--   0        0        0      591 2023-06-09 00:12:10.919306 huma_signals-0.3.0/huma_signals/adapters/polygon_wallet/README.md
+-rw-r--r--   0        0        0        0 2023-06-09 00:12:10.919306 huma_signals-0.3.0/huma_signals/adapters/polygon_wallet/__init__.py
+-rw-r--r--   0        0        0     3201 2023-06-09 00:12:10.919306 huma_signals-0.3.0/huma_signals/adapters/polygon_wallet/adapter.py
+-rw-r--r--   0        0        0      222 2023-06-09 00:12:10.919306 huma_signals-0.3.0/huma_signals/adapters/polygon_wallet/settings.py
+-rw-r--r--   0        0        0      576 2023-06-09 00:12:10.919306 huma_signals-0.3.0/huma_signals/adapters/request_network/README.md
+-rw-r--r--   0        0        0        0 2023-06-09 00:12:10.919306 huma_signals-0.3.0/huma_signals/adapters/request_network/__init__.py
+-rw-r--r--   0        0        0     4372 2023-06-09 00:12:10.919306 huma_signals-0.3.0/huma_signals/adapters/request_network/models.py
+-rw-r--r--   0        0        0     5464 2023-06-09 00:12:10.919306 huma_signals-0.3.0/huma_signals/adapters/request_network/request_invoice_adapter.py
+-rw-r--r--   0        0        0     4930 2023-06-09 00:12:10.919306 huma_signals-0.3.0/huma_signals/adapters/request_network/request_transaction_adapter.py
+-rw-r--r--   0        0        0      284 2023-06-09 00:12:10.919306 huma_signals-0.3.0/huma_signals/adapters/request_network/settings.py
+-rw-r--r--   0        0        0        0 2023-06-09 00:12:10.919306 huma_signals-0.3.0/huma_signals/adapters/superfluid/__init__.py
+-rw-r--r--   0        0        0      238 2023-06-09 00:12:10.919306 huma_signals-0.3.0/huma_signals/adapters/superfluid/settings.py
+-rw-r--r--   0        0        0     3587 2023-06-09 00:12:10.919306 huma_signals-0.3.0/huma_signals/adapters/superfluid/superfluid_adapter.py
+-rw-r--r--   0        0        0      436 2023-06-09 00:12:10.919306 huma_signals-0.3.0/huma_signals/adapters/superfluid/superfluid_models.py
+-rw-r--r--   0        0        0        0 2023-06-09 00:12:10.919306 huma_signals-0.3.0/huma_signals/clients/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-09 00:12:10.919306 huma_signals-0.3.0/huma_signals/clients/eth_client/__init__.py
+-rw-r--r--   0        0        0     1427 2023-06-09 00:12:10.919306 huma_signals-0.3.0/huma_signals/clients/eth_client/eth_client.py
+-rw-r--r--   0        0        0      673 2023-06-09 00:12:10.919306 huma_signals-0.3.0/huma_signals/clients/eth_client/eth_types.py
+-rw-r--r--   0        0        0        0 2023-06-09 00:12:10.919306 huma_signals-0.3.0/huma_signals/clients/polygon_client/__init__.py
+-rw-r--r--   0        0        0     1503 2023-06-09 00:12:10.919306 huma_signals-0.3.0/huma_signals/clients/polygon_client/polygon_client.py
+-rw-r--r--   0        0        0      685 2023-06-09 00:12:10.919306 huma_signals-0.3.0/huma_signals/clients/polygon_client/polygon_types.py
+-rw-r--r--   0        0        0        0 2023-06-09 00:12:10.919306 huma_signals-0.3.0/huma_signals/clients/request_client/__init__.py
+-rw-r--r--   0        0        0     8129 2023-06-09 00:12:10.919306 huma_signals-0.3.0/huma_signals/clients/request_client/request_client.py
+-rw-r--r--   0        0        0      900 2023-06-09 00:12:10.919306 huma_signals-0.3.0/huma_signals/clients/request_client/request_types.py
+-rw-r--r--   0        0        0        0 2023-06-09 00:12:10.919306 huma_signals-0.3.0/huma_signals/commons/__init__.py
+-rw-r--r--   0        0        0      291 2023-06-09 00:12:10.919306 huma_signals-0.3.0/huma_signals/commons/chains.py
+-rw-r--r--   0        0        0      330 2023-06-09 00:12:10.919306 huma_signals-0.3.0/huma_signals/commons/datetime_utils.py
+-rw-r--r--   0        0        0      227 2023-06-09 00:12:10.919306 huma_signals-0.3.0/huma_signals/commons/pydantic_utils.py
+-rw-r--r--   0        0        0      569 2023-06-09 00:12:10.919306 huma_signals-0.3.0/huma_signals/commons/string_utils.py
+-rw-r--r--   0        0        0     1309 2023-06-09 00:12:10.919306 huma_signals-0.3.0/huma_signals/commons/tokens.py
+-rw-r--r--   0        0        0     1078 2023-06-09 00:12:10.919306 huma_signals-0.3.0/huma_signals/commons/web3_utils.py
+-rw-r--r--   0        0        0      499 2023-06-09 00:12:10.919306 huma_signals-0.3.0/huma_signals/dotenv/example.env
+-rw-r--r--   0        0        0     1157 2023-06-09 00:12:10.919306 huma_signals-0.3.0/huma_signals/exceptions.py
+-rw-r--r--   0        0        0      322 2023-06-09 00:12:10.919306 huma_signals-0.3.0/huma_signals/models.py
+-rw-r--r--   0        0        0        0 2023-06-09 00:12:10.919306 huma_signals-0.3.0/huma_signals/py.typed
+-rw-r--r--   0        0        0     1563 2023-06-09 00:12:10.919306 huma_signals-0.3.0/huma_signals/settings.py
+-rw-r--r--   0        0        0     2792 2023-06-09 00:12:10.923307 huma_signals-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3110 1970-01-01 00:00:00.000000 huma_signals-0.3.0/PKG-INFO
```

### Comparing `huma_signals-0.2.1/LICENSE` & `huma_signals-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `huma_signals-0.2.1/README.md` & `huma_signals-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `huma_signals-0.2.1/huma_signals/adapters/ethereum_wallet/README.md` & `huma_signals-0.3.0/huma_signals/adapters/ethereum_wallet/README.md`

 * *Files identical despite different names*

### Comparing `huma_signals-0.2.1/huma_signals/adapters/ethereum_wallet/adapter.py` & `huma_signals-0.3.0/huma_signals/adapters/ethereum_wallet/adapter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import datetime
-from typing import Any, ClassVar
+from typing import Any
 
 from huma_signals import models
 from huma_signals.adapters import models as adapter_models
 from huma_signals.adapters.ethereum_wallet.settings import settings
 from huma_signals.clients.eth_client import eth_client, eth_types
 from huma_signals.commons import datetime_utils
 
@@ -14,18 +14,14 @@
     total_received: int
     wallet_tenure_in_days: int
     total_income_90days: int
     total_transactions_90days: int
 
 
 class BaseEthereumWalletAdapter(adapter_models.SignalAdapterBase):
-    name: ClassVar[str] = "ethereum_wallet"
-    required_inputs: ClassVar[list[str]] = ["borrower_wallet_address"]
-    signals: ClassVar[list[str]] = list(EthereumWalletSignals.__fields__.keys())
-
     async def fetch(  # pylint: disable=arguments-differ
         self, borrower_wallet_address: str, *args: Any, **kwargs: Any
     ) -> EthereumWalletSignals:
         raise NotImplementedError
 
 
 class EthereumWalletAdapter(BaseEthereumWalletAdapter):
```

### Comparing `huma_signals-0.2.1/huma_signals/adapters/lending_pools/README.md` & `huma_signals-0.3.0/huma_signals/adapters/lending_pools/README.md`

 * *Files identical despite different names*

### Comparing `huma_signals-0.2.1/huma_signals/adapters/lending_pools/abi/BaseCreditPool.json` & `huma_signals-0.3.0/huma_signals/adapters/lending_pools/abi/BaseCreditPool.json`

 * *Files identical despite different names*

### Comparing `huma_signals-0.2.1/huma_signals/adapters/lending_pools/abi/BasePoolConfig.json` & `huma_signals-0.3.0/huma_signals/adapters/lending_pools/abi/BasePoolConfig.json`

 * *Files identical despite different names*

### Comparing `huma_signals-0.2.1/huma_signals/adapters/lending_pools/abi/ReceivableFactoringPool.json` & `huma_signals-0.3.0/huma_signals/adapters/lending_pools/abi/ReceivableFactoringPool.json`

 * *Files identical despite different names*

### Comparing `huma_signals-0.2.1/huma_signals/adapters/lending_pools/abi/SuperfluidFactoringPool.json` & `huma_signals-0.3.0/huma_signals/adapters/lending_pools/abi/SuperfluidFactoringPool.json`

 * *Files identical despite different names*

### Comparing `huma_signals-0.2.1/huma_signals/adapters/lending_pools/adapter.py` & `huma_signals-0.3.0/huma_signals/adapters/lending_pools/adapter.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import decimal
 import pathlib
-from typing import Any, ClassVar, List
+from typing import Any, ClassVar
 
 import aiofiles
 import orjson
 import pydantic
 import structlog
 import web3
 from web3 import exceptions as web3_exceptions
@@ -52,18 +52,14 @@
 
 class LendingPoolAdapter(adapter_models.SignalAdapterBase):
     # TODO: move the hard coded values to EA settings cause these are not pool setting
     interval_in_days_max: ClassVar[int] = 90
     interval_in_days_min: ClassVar[int] = 0
     invoice_amount_ratio: ClassVar[float] = 0.8
 
-    name: ClassVar[str] = "lending_pool"
-    required_inputs: ClassVar[List[str]] = ["pool_address"]
-    signals: ClassVar[List[str]] = list(LendingPoolSignals.__fields__.keys())
-
     async def fetch(  # pylint: disable=arguments-differ
         self, pool_address: str, *args: Any, **kwargs: Any
     ) -> LendingPoolSignals:
         try:
             checksum_address = web3.Web3.to_checksum_address(pool_address)
             pool_settings = registry.POOL_REGISTRY[checksum_address]
         except KeyError as e:
```

### Comparing `huma_signals-0.2.1/huma_signals/adapters/lending_pools/registry.py` & `huma_signals-0.3.0/huma_signals/adapters/lending_pools/registry.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.2.1/huma_signals/adapters/polygon_wallet/README.md` & `huma_signals-0.3.0/huma_signals/adapters/polygon_wallet/README.md`

 * *Files identical despite different names*

### Comparing `huma_signals-0.2.1/huma_signals/adapters/polygon_wallet/adapter.py` & `huma_signals-0.3.0/huma_signals/adapters/polygon_wallet/adapter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import datetime
-from typing import Any, ClassVar
+from typing import Any
 
 import structlog
 
 from huma_signals import models
 from huma_signals.adapters import models as adapter_models
 from huma_signals.adapters.polygon_wallet.settings import settings
 from huma_signals.clients.polygon_client import polygon_client, polygon_types
@@ -18,18 +18,14 @@
     total_received: int
     wallet_tenure_in_days: int
     total_income_90days: float
     total_transactions_90days: int
 
 
 class BasePolygonWalletAdapter(adapter_models.SignalAdapterBase):
-    name: ClassVar[str] = "polygon_wallet"
-    required_inputs: ClassVar[list[str]] = ["borrower_wallet_address"]
-    signals: ClassVar[list[str]] = list(PolygonWalletSignals.__fields__.keys())
-
     async def fetch(  # pylint: disable=arguments-differ
         self, borrower_wallet_address: str, *args: Any, **kwargs: Any
     ) -> PolygonWalletSignals:
         raise NotImplementedError
 
 
 class PolygonWalletAdapter(BasePolygonWalletAdapter):
```

### Comparing `huma_signals-0.2.1/huma_signals/adapters/request_network/README.md` & `huma_signals-0.3.0/huma_signals/adapters/request_network/README.md`

 * *Files identical despite different names*

### Comparing `huma_signals-0.2.1/huma_signals/adapters/request_network/models.py` & `huma_signals-0.3.0/huma_signals/adapters/request_network/models.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.2.1/huma_signals/adapters/request_network/request_invoice_adapter.py` & `huma_signals-0.3.0/huma_signals/adapters/request_network/request_invoice_adapter.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import datetime
-from typing import Any, ClassVar
+from typing import Any
 
 import pandas as pd
 import structlog
 import web3
 
 from huma_signals import exceptions
 from huma_signals.adapters import models as adapter_models
@@ -12,30 +12,22 @@
 from huma_signals.adapters.request_network import models
 from huma_signals.adapters.request_network.settings import settings
 from huma_signals.clients.request_client import request_client
 from huma_signals.commons import chains
 
 logger = structlog.get_logger(__name__)
 
-_ALLOWED_PAYER_ADDRESSES = {"0x2177d6C4eC1a6511184CA6FfAb4FD1d1F5bFF39f".lower()}
 _WALLET_ADAPTER_BY_CHAIN = {
     chains.Chain.ETHEREUM: ethereum_wallet_adapter.EthereumWalletAdapter,
     chains.Chain.GOERLI: ethereum_wallet_adapter.EthereumWalletAdapter,
     chains.Chain.POLYGON: polygon_wallet_adapter.PolygonWalletAdapter,
 }
 
 
 class RequestInvoiceAdapter(adapter_models.SignalAdapterBase):
-    name: ClassVar[str] = "request_network"
-    required_inputs: ClassVar[list[str]] = [
-        "borrower_wallet_address",
-        "receivable_param",
-    ]
-    signals: ClassVar[list[str]] = list(models.RequestInvoiceSignals.__fields__.keys())
-
     def __init__(  # pylint: disable=too-many-arguments
         self,
         request_client_: request_client.BaseRequestClient | None = None,
         wallet_adapter: ethereum_wallet_adapter.BaseEthereumWalletAdapter
         | polygon_wallet_adapter.BasePolygonWalletAdapter
         | None = None,
         request_network_subgraph_endpoint_url: str = settings.request_network_subgraph_endpoint_url,
@@ -123,10 +115,9 @@
             ),
             borrower_own_invoice=(
                 invoice.token_owner.lower() == borrower_wallet_address.lower()
             ),
             payer_match_payee=(invoice.payer.lower() == invoice.payee.lower()),
             days_until_due_date=(invoice.due_date - datetime.datetime.utcnow()).days,
             invoice_amount=invoice.amount,
-            # payer_on_allowlist=(invoice.payer.lower() in _ALLOWED_PAYER_ADDRESSES),
             payer_on_allowlist=True,
         )
```

### Comparing `huma_signals-0.2.1/huma_signals/adapters/request_network/request_transaction_adapter.py` & `huma_signals-0.3.0/huma_signals/adapters/request_network/request_transaction_adapter.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, ClassVar, List
+from typing import Any
 
 import pandas as pd
 import structlog
 import web3
 
 from huma_signals import exceptions
 from huma_signals.adapters import models as adapter_models
@@ -19,23 +19,14 @@
     chains.Chain.ETHEREUM: ethereum_wallet_adapter.EthereumWalletAdapter,
     chains.Chain.GOERLI: ethereum_wallet_adapter.EthereumWalletAdapter,
     chains.Chain.POLYGON: polygon_wallet_adapter.PolygonWalletAdapter,
 }
 
 
 class RequestTransactionAdapter(adapter_models.SignalAdapterBase):
-    name: ClassVar[str] = "request_transaction"
-    required_inputs: ClassVar[List[str]] = [
-        "payer_address",
-        "payee_address",
-    ]
-    signals: ClassVar[List[str]] = list(
-        models.RequestTransactionSignals.__fields__.keys()
-    )
-
     def __init__(  # pylint: disable=too-many-arguments
         self,
         request_client_: request_client.BaseRequestClient | None = None,
         wallet_adapter: ethereum_wallet_adapter.BaseEthereumWalletAdapter
         | polygon_wallet_adapter.BasePolygonWalletAdapter
         | None = None,
         request_network_subgraph_endpoint_url: str = settings.request_network_subgraph_endpoint_url,
```

### Comparing `huma_signals-0.2.1/huma_signals/clients/eth_client/eth_client.py` & `huma_signals-0.3.0/huma_signals/clients/eth_client/eth_client.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.2.1/huma_signals/clients/eth_client/eth_types.py` & `huma_signals-0.3.0/huma_signals/clients/eth_client/eth_types.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.2.1/huma_signals/clients/polygon_client/polygon_client.py` & `huma_signals-0.3.0/huma_signals/clients/polygon_client/polygon_client.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.2.1/huma_signals/clients/polygon_client/polygon_types.py` & `huma_signals-0.3.0/huma_signals/clients/polygon_client/polygon_types.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.2.1/huma_signals/clients/request_client/request_client.py` & `huma_signals-0.3.0/huma_signals/clients/request_client/request_client.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.2.1/huma_signals/clients/request_client/request_types.py` & `huma_signals-0.3.0/huma_signals/clients/request_client/request_types.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.2.1/huma_signals/commons/string_utils.py` & `huma_signals-0.3.0/huma_signals/commons/string_utils.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.2.1/huma_signals/commons/tokens.py` & `huma_signals-0.3.0/huma_signals/commons/tokens.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.2.1/huma_signals/commons/web3_utils.py` & `huma_signals-0.3.0/huma_signals/commons/web3_utils.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.2.1/huma_signals/exceptions.py` & `huma_signals-0.3.0/huma_signals/exceptions.py`

 * *Files 27% similar despite different names*

```diff
@@ -26,7 +26,16 @@
     def __init__(self, message: str) -> None:
         super().__init__(message=message)
 
 
 class RequestException(HumaSignalException):
     def __init__(self, message: str) -> None:
         super().__init__(message=message)
+
+
+class SuperfluidException(HumaSignalException):
+    def __init__(self, message: str) -> None:
+        super().__init__(message=message)
+
+
+class SuperfluidStreamNotFoundException(SuperfluidException):
+    pass
```

### Comparing `huma_signals-0.2.1/huma_signals/settings.py` & `huma_signals-0.3.0/huma_signals/settings.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.2.1/pyproject.toml` & `huma_signals-0.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "huma-signals"
-version = "0.2.1"
+version = "0.3.0"
 description = "Enables access to high-quality signals about a borrower's income, assets, and liabilities."
 authors = ["Jiatu Liu <jiatu@huma.finance>", "Ji Peng <ji@huma.finance>"]
 license = "AGPL v3"
 readme = "README.md"
 packages = [{include = "huma_signals"}]
 homepage = "https://github.com/00labs/huma-signals/"
 documentation = "https://docs.huma.finance/developer-guidelines/decentralized_signal_portfolio"
```

### Comparing `huma_signals-0.2.1/PKG-INFO` & `huma_signals-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huma-signals
-Version: 0.2.1
+Version: 0.3.0
 Summary: Enables access to high-quality signals about a borrower's income, assets, and liabilities.
 Home-page: https://github.com/00labs/huma-signals/
 License: AGPL v3
 Author: Jiatu Liu
 Author-email: jiatu@huma.finance
 Requires-Python: >=3.10,<3.11
 Classifier: License :: Other/Proprietary License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: huma-signals Version: 0.2.1 Summary: Enables access
+Metadata-Version: 2.1 Name: huma-signals Version: 0.3.0 Summary: Enables access
 to high-quality signals about a borrower's income, assets, and liabilities.
 Home-page: https://github.com/00labs/huma-signals/ License: AGPL v3 Author:
 Jiatu Liu Author-email: jiatu@huma.finance Requires-Python: >=3.10,<3.11
 Classifier: License :: Other/Proprietary License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: aiofiles (>=22.1.0,<23.0.0) Requires-Dist: httpx
 (>=0.24.0,<0.25.0) Requires-Dist: orjson (>=3.8.5,<4.0.0) Requires-Dist: pandas
```

