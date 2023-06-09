# Comparing `tmp/aptos_sdk-0.6.2.tar.gz` & `tmp/aptos_sdk-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aptos_sdk-0.6.2.tar", max compression
+gzip compressed data, was "aptos_sdk-0.6.3.tar", max compression
```

## Comparing `aptos_sdk-0.6.2.tar` & `aptos_sdk-0.6.3.tar`

### file list

```diff
@@ -1,15 +1,17 @@
--rw-r--r--   0        0        0     2746 2023-06-06 10:45:46.911352 aptos_sdk-0.6.2/README.md
--rw-r--r--   0        0        0       70 2023-03-20 22:18:46.787532 aptos_sdk-0.6.2/aptos_sdk/__init__.py
--rw-r--r--   0        0        0     5651 2023-03-22 16:06:08.428473 aptos_sdk-0.6.2/aptos_sdk/account.py
--rw-r--r--   0        0        0     5873 2023-05-12 23:36:33.034261 aptos_sdk-0.6.2/aptos_sdk/account_address.py
--rw-r--r--   0        0        0    18891 2023-06-01 17:39:30.476859 aptos_sdk-0.6.2/aptos_sdk/aptos_token_client.py
--rw-r--r--   0        0        0    26553 2023-06-06 10:45:46.911540 aptos_sdk-0.6.2/aptos_sdk/async_client.py
--rw-r--r--   0        0        0     5811 2023-03-27 16:58:44.414814 aptos_sdk-0.6.2/aptos_sdk/authenticator.py
--rw-r--r--   0        0        0    10447 2023-03-20 22:18:46.787856 aptos_sdk-0.6.2/aptos_sdk/bcs.py
--rw-r--r--   0        0        0    24350 2023-06-06 10:45:46.911858 aptos_sdk-0.6.2/aptos_sdk/client.py
--rw-r--r--   0        0        0    12056 2023-03-27 16:58:44.414953 aptos_sdk-0.6.2/aptos_sdk/ed25519.py
--rw-r--r--   0        0        0      277 2023-06-06 10:45:46.912067 aptos_sdk-0.6.2/aptos_sdk/metadata.py
--rw-r--r--   0        0        0    26552 2023-06-01 17:39:30.543085 aptos_sdk-0.6.2/aptos_sdk/transactions.py
--rw-r--r--   0        0        0     8991 2023-03-20 22:18:46.788343 aptos_sdk-0.6.2/aptos_sdk/type_tag.py
--rw-r--r--   0        0        0      763 2023-06-06 10:45:46.912325 aptos_sdk-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     3670 1970-01-01 00:00:00.000000 aptos_sdk-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     2746 2023-06-03 10:15:17.666676 aptos_sdk-0.6.3/README.md
+-rw-r--r--   0        0        0       70 2023-05-26 05:51:23.736675 aptos_sdk-0.6.3/aptos_sdk/__init__.py
+-rw-r--r--   0        0        0     5651 2023-05-26 05:51:23.723342 aptos_sdk-0.6.3/aptos_sdk/account.py
+-rw-r--r--   0        0        0     5873 2023-05-26 05:51:23.630008 aptos_sdk-0.6.3/aptos_sdk/account_address.py
+-rw-r--r--   0        0        0     8546 2023-06-09 00:05:39.956760 aptos_sdk-0.6.3/aptos_sdk/account_sequence_number.py
+-rw-r--r--   0        0        0    20257 2023-06-09 02:20:19.940022 aptos_sdk-0.6.3/aptos_sdk/aptos_token_client.py
+-rw-r--r--   0        0        0    27697 2023-06-09 02:20:19.943356 aptos_sdk-0.6.3/aptos_sdk/async_client.py
+-rw-r--r--   0        0        0     5811 2023-05-26 05:51:23.743342 aptos_sdk-0.6.3/aptos_sdk/authenticator.py
+-rw-r--r--   0        0        0    10447 2023-05-26 05:51:23.720008 aptos_sdk-0.6.3/aptos_sdk/bcs.py
+-rw-r--r--   0        0        0    24350 2023-06-09 02:20:19.910022 aptos_sdk-0.6.3/aptos_sdk/client.py
+-rw-r--r--   0        0        0    12056 2023-05-26 05:51:23.716675 aptos_sdk-0.6.3/aptos_sdk/ed25519.py
+-rw-r--r--   0        0        0      277 2023-06-03 10:15:17.666676 aptos_sdk-0.6.3/aptos_sdk/metadata.py
+-rw-r--r--   0        0        0     8405 2023-06-09 00:05:39.910093 aptos_sdk-0.6.3/aptos_sdk/transaction_worker.py
+-rw-r--r--   0        0        0    26552 2023-06-09 02:20:19.920022 aptos_sdk-0.6.3/aptos_sdk/transactions.py
+-rw-r--r--   0        0        0     8991 2023-05-26 05:51:23.730008 aptos_sdk-0.6.3/aptos_sdk/type_tag.py
+-rw-r--r--   0        0        0      762 2023-06-09 01:08:05.026671 aptos_sdk-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0     3628 1970-01-01 00:00:00.000000 aptos_sdk-0.6.3/PKG-INFO
```

### Comparing `aptos_sdk-0.6.2/README.md` & `aptos_sdk-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `aptos_sdk-0.6.2/aptos_sdk/account.py` & `aptos_sdk-0.6.3/aptos_sdk/account.py`

 * *Files identical despite different names*

### Comparing `aptos_sdk-0.6.2/aptos_sdk/account_address.py` & `aptos_sdk-0.6.3/aptos_sdk/account_address.py`

 * *Files identical despite different names*

### Comparing `aptos_sdk-0.6.2/aptos_sdk/aptos_token_client.py` & `aptos_sdk-0.6.3/aptos_sdk/aptos_token_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -334,17 +334,15 @@
         read_resources = await self.client.account_resources(address)
         for resource in read_resources:
             if resource["type"] in ReadObject.resource_map:
                 resource_obj = ReadObject.resource_map[resource["type"]]
                 resources[resource_obj] = resource_obj.parse(resource["data"])
         return ReadObject(resources)
 
-    async def create_collection(
-        self,
-        creator: Account,
+    def create_collection_payload(
         description: str,
         max_supply: int,
         name: str,
         uri: str,
         mutable_description: bool,
         mutable_royalty: bool,
         mutable_uri: bool,
@@ -352,15 +350,15 @@
         mutable_token_name: bool,
         mutable_token_properties: bool,
         mutable_token_uri: bool,
         tokens_burnable_by_creator: bool,
         tokens_freezable_by_creator: bool,
         royalty_numerator: int,
         royalty_denominator: int,
-    ) -> str:
+    ) -> TransactionPayload:
         transaction_arguments = [
             TransactionArgument(description, Serializer.str),
             TransactionArgument(max_supply, Serializer.u64),
             TransactionArgument(name, Serializer.str),
             TransactionArgument(uri, Serializer.str),
             TransactionArgument(mutable_description, Serializer.bool),
             TransactionArgument(mutable_royalty, Serializer.bool),
@@ -378,28 +376,64 @@
         payload = EntryFunction.natural(
             "0x4::aptos_token",
             "create_collection",
             [],
             transaction_arguments,
         )
 
+        return TransactionPayload(payload)
+
+    async def create_collection(
+        self,
+        creator: Account,
+        description: str,
+        max_supply: int,
+        name: str,
+        uri: str,
+        mutable_description: bool,
+        mutable_royalty: bool,
+        mutable_uri: bool,
+        mutable_token_description: bool,
+        mutable_token_name: bool,
+        mutable_token_properties: bool,
+        mutable_token_uri: bool,
+        tokens_burnable_by_creator: bool,
+        tokens_freezable_by_creator: bool,
+        royalty_numerator: int,
+        royalty_denominator: int,
+    ) -> str:
+        payload = create_collection_payload(
+            description,
+            max_supply,
+            name,
+            uri,
+            mutable_description,
+            mutable_royalty,
+            mutable_uri,
+            mutable_token_description,
+            mutable_token_name,
+            mutable_token_properties,
+            mutable_token_uri,
+            tokens_burnable_by_creator,
+            tokens_freezable_by_creator,
+            royalty_numerator,
+            royalty_denominator,
+        )
         signed_transaction = await self.client.create_bcs_signed_transaction(
-            creator, TransactionPayload(payload)
+            creator, payload
         )
         return await self.client.submit_bcs_transaction(signed_transaction)
 
-    async def mint_token(
-        self,
-        creator: Account,
+    def mint_token_payload(
         collection: str,
         description: str,
         name: str,
         uri: str,
         properties: PropertyMap,
-    ) -> str:
+    ) -> TransactionPayload:
         (property_names, property_types, property_values) = properties.to_tuple()
         transaction_arguments = [
             TransactionArgument(collection, Serializer.str),
             TransactionArgument(description, Serializer.str),
             TransactionArgument(name, Serializer.str),
             TransactionArgument(uri, Serializer.str),
             TransactionArgument(
@@ -416,16 +450,28 @@
         payload = EntryFunction.natural(
             "0x4::aptos_token",
             "mint",
             [],
             transaction_arguments,
         )
 
+        return TransactionPayload(payload)
+
+    async def mint_token(
+        self,
+        creator: Account,
+        collection: str,
+        description: str,
+        name: str,
+        uri: str,
+        properties: PropertyMap,
+    ) -> str:
+        payload = mint_token_payload(collection, description, name, uri, properties)
         signed_transaction = await self.client.create_bcs_signed_transaction(
-            creator, TransactionPayload(payload)
+            creator, payload
         )
         return await self.client.submit_bcs_transaction(signed_transaction)
 
     async def mint_soul_bound_token(
         self,
         creator: Account,
         collection: str,
```

### Comparing `aptos_sdk-0.6.2/aptos_sdk/async_client.py` & `aptos_sdk-0.6.3/aptos_sdk/async_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # Copyright © Aptos Foundation
 # SPDX-License-Identifier: Apache-2.0
 
+import asyncio
+import logging
 import time
 from typing import Any, Dict, List, Optional
 
 import httpx
 
 from . import ed25519
 from .account import Account
@@ -16,15 +18,14 @@
     EntryFunction,
     MultiAgentRawTransaction,
     RawTransaction,
     SignedTransaction,
     TransactionArgument,
     TransactionPayload,
 )
-from .type_tag import StructTag, TypeTag
 
 U64_MAX = 18446744073709551615
 
 
 class ClientConfig:
     """Common configuration for clients, particularly for submitting transactions"""
 
@@ -49,15 +50,18 @@
         limits = httpx.Limits()
         # Default timeouts but do not set a pool timeout, since the idea is that jobs will wait as
         # long as progress is being made.
         timeout = httpx.Timeout(60.0, pool=None)
         # Default headers
         headers = {Metadata.APTOS_HEADER: Metadata.get_aptos_header_val()}
         self.client = httpx.AsyncClient(
-            http2=client_config.http2, limits=limits, timeout=timeout, headers=headers
+            http2=client_config.http2,
+            limits=limits,
+            timeout=timeout,
+            headers=headers,
         )
         self.client_config = client_config
         self._chain_id = None
 
     async def close(self):
         await self.client.aclose()
 
@@ -91,15 +95,15 @@
     ) -> int:
         """Returns the test coin balance associated with the account"""
         resource = await self.account_resource(
             account_address,
             "0x1::coin::CoinStore<0x1::aptos_coin::AptosCoin>",
             ledger_version,
         )
-        return resource["data"]["coin"]["value"]
+        return int(resource["data"]["coin"]["value"])
 
     async def account_sequence_number(
         self, account_address: AccountAddress, ledger_version: int = None
     ) -> int:
         account_res = await self.account(account_address, ledger_version)
         return int(account_res["sequence_number"])
 
@@ -136,14 +140,18 @@
         response = await self.client.get(request)
         if response.status_code == 404:
             raise AccountNotFound(f"{account_address}", account_address)
         if response.status_code >= 400:
             raise ApiError(f"{response.text} - {account_address}", response.status_code)
         return response.json()
 
+    async def current_timestamp(self) -> float:
+        info = await self.info()
+        return float(info["ledger_timestamp"]) / 1_000_000
+
     async def get_table_item(
         self,
         handle: str,
         key_type: str,
         value_type: str,
         key: Any,
         ledger_version: int = None,
@@ -319,23 +327,37 @@
         """
 
         count = 0
         while await self.transaction_pending(txn_hash):
             assert (
                 count < self.client_config.transaction_wait_in_seconds
             ), f"transaction {txn_hash} timed out"
-            time.sleep(1)
+            await asyncio.sleep(1)
             count += 1
         response = await self.client.get(
             f"{self.base_url}/transactions/by_hash/{txn_hash}"
         )
         assert (
             "success" in response.json() and response.json()["success"]
         ), f"{response.text} - {txn_hash}"
 
+    async def account_transaction_sequence_number_status(
+        self, address: AccountAddress, sequence_number: int
+    ) -> bool:
+        """Retrieve the state of a transaction by account and sequence number."""
+
+        response = await self.client.get(
+            f"{self.base_url}/accounts/{address}/transactions?limit=1&start={sequence_number}"
+        )
+        if response.status_code >= 400:
+            logging.info(f"k {response}")
+            raise ApiError(response.text, response.status_code)
+        data = response.json()
+        return len(data) == 1 and data[0]["type"] != "pending_transaction"
+
     #
     # Transaction helpers
     #
 
     async def create_multi_agent_bcs_transaction(
         self,
         sender: Account,
@@ -373,30 +395,43 @@
                 ],
             )
         )
 
         return SignedTransaction(raw_transaction.inner(), authenticator)
 
     async def create_bcs_transaction(
-        self, sender: Account, payload: TransactionPayload
+        self,
+        sender: Account,
+        payload: TransactionPayload,
+        sequence_number: Optional[int] = None,
     ) -> RawTransaction:
+        sequence_number = (
+            sequence_number
+            if sequence_number is not None
+            else await self.account_sequence_number(sender.address())
+        )
         return RawTransaction(
             sender.address(),
-            await self.account_sequence_number(sender.address()),
+            sequence_number,
             payload,
             self.client_config.max_gas_amount,
             self.client_config.gas_unit_price,
             int(time.time()) + self.client_config.expiration_ttl,
             await self.chain_id(),
         )
 
     async def create_bcs_signed_transaction(
-        self, sender: Account, payload: TransactionPayload
+        self,
+        sender: Account,
+        payload: TransactionPayload,
+        sequence_number: Optional[int] = None,
     ) -> SignedTransaction:
-        raw_transaction = await self.create_bcs_transaction(sender, payload)
+        raw_transaction = await self.create_bcs_transaction(
+            sender, payload, sequence_number
+        )
         signature = sender.sign(raw_transaction.keyed())
         authenticator = Authenticator(
             Ed25519Authenticator(sender.public_key(), signature)
         )
         return SignedTransaction(raw_transaction, authenticator)
 
     #
@@ -407,41 +442,45 @@
         self, sender: Account, recipient: AccountAddress, amount: int
     ) -> str:
         """Transfer a given coin amount from a given Account to the recipient's account address.
         Returns the sequence number of the transaction used to transfer."""
 
         payload = {
             "type": "entry_function_payload",
-            "function": "0x1::coin::transfer",
-            "type_arguments": ["0x1::aptos_coin::AptosCoin"],
+            "function": "0x1::aptos_account::transfer",
+            "type_arguments": [],
             "arguments": [
                 f"{recipient}",
                 str(amount),
             ],
         }
         return await self.submit_transaction(sender, payload)
 
     # :!:>bcs_transfer
     async def bcs_transfer(
-        self, sender: Account, recipient: AccountAddress, amount: int
+        self,
+        sender: Account,
+        recipient: AccountAddress,
+        amount: int,
+        sequence_number: Optional[int] = None,
     ) -> str:
         transaction_arguments = [
             TransactionArgument(recipient, Serializer.struct),
             TransactionArgument(amount, Serializer.u64),
         ]
 
         payload = EntryFunction.natural(
-            "0x1::coin",
+            "0x1::aptos_account",
             "transfer",
-            [TypeTag(StructTag.from_str("0x1::aptos_coin::AptosCoin"))],
+            [],
             transaction_arguments,
         )
 
         signed_transaction = await self.create_bcs_signed_transaction(
-            sender, TransactionPayload(payload)
+            sender, TransactionPayload(payload), sequence_number=sequence_number
         )
         return await self.submit_bcs_transaction(signed_transaction)
 
     # <:!:bcs_transfer
 
     #
     # Token transaction wrappers
```

### Comparing `aptos_sdk-0.6.2/aptos_sdk/authenticator.py` & `aptos_sdk-0.6.3/aptos_sdk/authenticator.py`

 * *Files identical despite different names*

### Comparing `aptos_sdk-0.6.2/aptos_sdk/bcs.py` & `aptos_sdk-0.6.3/aptos_sdk/bcs.py`

 * *Files identical despite different names*

### Comparing `aptos_sdk-0.6.2/aptos_sdk/client.py` & `aptos_sdk-0.6.3/aptos_sdk/client.py`

 * *Files identical despite different names*

### Comparing `aptos_sdk-0.6.2/aptos_sdk/ed25519.py` & `aptos_sdk-0.6.3/aptos_sdk/ed25519.py`

 * *Files identical despite different names*

### Comparing `aptos_sdk-0.6.2/aptos_sdk/transactions.py` & `aptos_sdk-0.6.3/aptos_sdk/transactions.py`

 * *Files identical despite different names*

### Comparing `aptos_sdk-0.6.2/aptos_sdk/type_tag.py` & `aptos_sdk-0.6.3/aptos_sdk/type_tag.py`

 * *Files identical despite different names*

### Comparing `aptos_sdk-0.6.2/pyproject.toml` & `aptos_sdk-0.6.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [tool.poetry]
 name = "aptos-sdk"
-version = "0.6.2"
+version = "0.6.3"
 description = "Aptos SDK"
 authors = ["Aptos Labs <opensource@aptoslabs.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/aptos-labs/aptos-core"
 homepage = "https://github.com/aptos-labs/aptos-core/tree/main/ecosystem/python/sdk"
 keywords = ["web3", "sdk", "aptos", "blockchain"]
 
 [tool.poetry.dependencies]
 h2 = "^4.1.0"
 httpx = "^0.23.0"
 PyNaCl = "^1.5.0"
 python = ">=3.7,<4.0"
-importlib = "^1.0.4"
 
 [tool.poetry.dev-dependencies]
 autoflake = "1.4.0"
 black = "^22.6.0"
+coverage = "^7.2.4"
 flake8 = ">=3.8.3,<6.0.0"
 isort = "^5.10.1"
 mypy = "^0.982"
 mypy-extensions = "^0.4.3"
 typing-extensions = "^4.4.0"
 
 [build-system]
```

### Comparing `aptos_sdk-0.6.2/PKG-INFO` & `aptos_sdk-0.6.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aptos-sdk
-Version: 0.6.2
+Version: 0.6.3
 Summary: Aptos SDK
 Home-page: https://github.com/aptos-labs/aptos-core/tree/main/ecosystem/python/sdk
 License: Apache-2.0
 Keywords: web3,sdk,aptos,blockchain
 Author: Aptos Labs
 Author-email: opensource@aptoslabs.com
 Requires-Python: >=3.7,<4.0
@@ -14,15 +14,14 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyNaCl (>=1.5.0,<2.0.0)
 Requires-Dist: h2 (>=4.1.0,<5.0.0)
 Requires-Dist: httpx (>=0.23.0,<0.24.0)
-Requires-Dist: importlib (>=1.0.4,<2.0.0)
 Project-URL: Repository, https://github.com/aptos-labs/aptos-core
 Description-Content-Type: text/markdown
 
 # Aptos Python SDK
 [![Discord][discord-image]][discord-url]
 [![PyPI Package Version][pypi-image-version]][pypi-url]
 [![PyPI Package Downloads][pypi-image-downloads]][pypi-url]
```

