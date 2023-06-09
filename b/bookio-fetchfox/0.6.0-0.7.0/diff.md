# Comparing `tmp/bookio_fetchfox-0.6.0.tar.gz` & `tmp/bookio_fetchfox-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bookio_fetchfox-0.6.0.tar", max compression
+gzip compressed data, was "bookio_fetchfox-0.7.0.tar", max compression
```

## Comparing `bookio_fetchfox-0.6.0.tar` & `bookio_fetchfox-0.7.0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0     3723 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/README.md
--rw-r--r--   0        0        0        0 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/__init__.py
--rw-r--r--   0        0        0        0 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/apis/__init__.py
--rw-r--r--   0        0        0        0 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/apis/algorand/__init__.py
--rw-r--r--   0        0        0     2140 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/apis/algorand/algonodecloud.py
--rw-r--r--   0        0        0      596 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/apis/algorand/algoxnftcom.py
--rw-r--r--   0        0        0     1349 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/apis/algorand/nfdomains.py
--rw-r--r--   0        0        0     1764 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/apis/algorand/nftexplorerapp.py
--rw-r--r--   0        0        0      592 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/apis/algorand/randswapcom.py
--rw-r--r--   0        0        0      262 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/apis/bookio.py
--rw-r--r--   0        0        0        0 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/apis/cardano/__init__.py
--rw-r--r--   0        0        0     2658 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/apis/cardano/blockfrostio.py
--rw-r--r--   0        0        0      734 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/apis/cardano/cnfttools.py
--rw-r--r--   0        0        0     1056 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/apis/cardano/handleme.py
--rw-r--r--   0        0        0     1606 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/apis/cardano/jpgstore.py
--rwxr-xr-x   0        0        0      675 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/apis/coingeckocom.py
--rw-r--r--   0        0        0        0 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/apis/evm/__init__.py
--rw-r--r--   0        0        0      963 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/apis/evm/ensideascom.py
--rw-r--r--   0        0        0     4147 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/apis/evm/moralisio.py
--rw-r--r--   0        0        0     2555 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/apis/evm/openseaio.py
--rw-r--r--   0        0        0      120 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/blockchains/__init__.py
--rw-r--r--   0        0        0       33 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/blockchains/algorand/__init__.py
--rw-r--r--   0        0        0     7966 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/blockchains/algorand/blockchain.py
--rw-r--r--   0        0        0      504 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/blockchains/algorand/utils.py
--rw-r--r--   0        0        0     2163 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/blockchains/base.py
--rw-r--r--   0        0        0       32 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/blockchains/cardano/__init__.py
--rw-r--r--   0        0        0    12039 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/blockchains/cardano/blockchain.py
--rw-r--r--   0        0        0     1061 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/blockchains/cardano/utils.py
--rw-r--r--   0        0        0       33 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/blockchains/ethereum/__init__.py
--rw-r--r--   0        0        0      547 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/blockchains/ethereum/blockchain.py
--rw-r--r--   0        0        0       28 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/blockchains/evm/__init__.py
--rw-r--r--   0        0        0     9685 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/blockchains/evm/blockchain.py
--rw-r--r--   0        0        0      619 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/blockchains/evm/utils.py
--rw-r--r--   0        0        0       32 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/blockchains/polygon/__init__.py
--rw-r--r--   0        0        0      548 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/blockchains/polygon/blockchain.py
--rw-r--r--   0        0        0      154 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/blockchains/utils.py
--rw-r--r--   0        0        0      322 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/checks.py
--rw-r--r--   0        0        0        0 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/constants/__init__.py
--rw-r--r--   0        0        0      158 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/constants/blockchains.py
--rw-r--r--   0        0        0      112 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/constants/currencies.py
--rw-r--r--   0        0        0      296 2023-06-09 12:41:03.736420 bookio_fetchfox-0.6.0/fetchfox/constants/marketplaces.py
--rw-r--r--   0        0        0       95 2023-06-09 12:41:03.736420 bookio_fetchfox-0.6.0/fetchfox/constants/sales.py
--rw-r--r--   0        0        0       28 2023-06-09 12:41:03.736420 bookio_fetchfox-0.6.0/fetchfox/constants/specials.py
--rw-r--r--   0        0        0      216 2023-06-09 12:41:03.736420 bookio_fetchfox-0.6.0/fetchfox/dtos/__init__.py
--rw-r--r--   0        0        0     2263 2023-06-09 12:41:03.736420 bookio_fetchfox-0.6.0/fetchfox/dtos/asset.py
--rw-r--r--   0        0        0     1215 2023-06-09 12:41:03.736420 bookio_fetchfox-0.6.0/fetchfox/dtos/campaign.py
--rw-r--r--   0        0        0      285 2023-06-09 12:41:03.736420 bookio_fetchfox-0.6.0/fetchfox/dtos/floor.py
--rw-r--r--   0        0        0      463 2023-06-09 12:41:03.736420 bookio_fetchfox-0.6.0/fetchfox/dtos/holding.py
--rw-r--r--   0        0        0     1409 2023-06-09 12:41:03.736420 bookio_fetchfox-0.6.0/fetchfox/dtos/listing.py
--rw-r--r--   0        0        0      365 2023-06-09 12:41:03.736420 bookio_fetchfox-0.6.0/fetchfox/dtos/rank.py
--rw-r--r--   0        0        0     1792 2023-06-09 12:41:03.736420 bookio_fetchfox-0.6.0/fetchfox/dtos/sale.py
--rw-r--r--   0        0        0        0 2023-06-09 12:41:03.736420 bookio_fetchfox-0.6.0/fetchfox/helpers/__init__.py
--rw-r--r--   0        0        0      150 2023-06-09 12:41:03.736420 bookio_fetchfox-0.6.0/fetchfox/helpers/formatters.py
--rw-r--r--   0        0        0     1895 2023-06-09 12:41:03.736420 bookio_fetchfox-0.6.0/fetchfox/rest.py
--rw-r--r--   0        0        0     1148 2023-06-09 12:41:03.748420 bookio_fetchfox-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     4986 1970-01-01 00:00:00.000000 bookio_fetchfox-0.6.0/setup.py
--rw-r--r--   0        0        0     4938 1970-01-01 00:00:00.000000 bookio_fetchfox-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     3723 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/apis/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/apis/algorand/__init__.py
+-rw-r--r--   0        0        0     2140 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/apis/algorand/algonodecloud.py
+-rw-r--r--   0        0        0      596 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/apis/algorand/algoxnftcom.py
+-rw-r--r--   0        0        0     1349 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/apis/algorand/nfdomains.py
+-rw-r--r--   0        0        0     1764 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/apis/algorand/nftexplorerapp.py
+-rw-r--r--   0        0        0      592 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/apis/algorand/randswapcom.py
+-rw-r--r--   0        0        0      262 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/apis/bookio.py
+-rw-r--r--   0        0        0        0 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/apis/cardano/__init__.py
+-rw-r--r--   0        0        0     2658 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/apis/cardano/blockfrostio.py
+-rw-r--r--   0        0        0      734 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/apis/cardano/cnfttools.py
+-rw-r--r--   0        0        0     1056 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/apis/cardano/handleme.py
+-rw-r--r--   0        0        0     1606 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/apis/cardano/jpgstore.py
+-rwxr-xr-x   0        0        0      675 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/apis/coingeckocom.py
+-rw-r--r--   0        0        0        0 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/apis/evm/__init__.py
+-rw-r--r--   0        0        0      963 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/apis/evm/ensideascom.py
+-rw-r--r--   0        0        0     4147 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/apis/evm/moralisio.py
+-rw-r--r--   0        0        0     2555 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/apis/evm/openseaio.py
+-rw-r--r--   0        0        0      120 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/blockchains/__init__.py
+-rw-r--r--   0        0        0       33 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/blockchains/algorand/__init__.py
+-rw-r--r--   0        0        0     8307 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/blockchains/algorand/blockchain.py
+-rw-r--r--   0        0        0      504 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/blockchains/algorand/utils.py
+-rw-r--r--   0        0        0     2380 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/blockchains/base.py
+-rw-r--r--   0        0        0       32 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/blockchains/cardano/__init__.py
+-rw-r--r--   0        0        0    12461 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/blockchains/cardano/blockchain.py
+-rw-r--r--   0        0        0     1061 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/blockchains/cardano/utils.py
+-rw-r--r--   0        0        0       33 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/blockchains/ethereum/__init__.py
+-rw-r--r--   0        0        0      666 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/blockchains/ethereum/blockchain.py
+-rw-r--r--   0        0        0       28 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/blockchains/evm/__init__.py
+-rw-r--r--   0        0        0     9983 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/blockchains/evm/blockchain.py
+-rw-r--r--   0        0        0      619 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/blockchains/evm/utils.py
+-rw-r--r--   0        0        0       32 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/blockchains/polygon/__init__.py
+-rw-r--r--   0        0        0      670 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/blockchains/polygon/blockchain.py
+-rw-r--r--   0        0        0      154 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/blockchains/utils.py
+-rw-r--r--   0        0        0      322 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/checks.py
+-rw-r--r--   0        0        0        0 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/constants/__init__.py
+-rw-r--r--   0        0        0      158 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/constants/blockchains.py
+-rw-r--r--   0        0        0      112 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/constants/currencies.py
+-rw-r--r--   0        0        0      296 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/constants/marketplaces.py
+-rw-r--r--   0        0        0       95 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/constants/sales.py
+-rw-r--r--   0        0        0       28 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/constants/specials.py
+-rw-r--r--   0        0        0      216 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/dtos/__init__.py
+-rw-r--r--   0        0        0     2263 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/dtos/asset.py
+-rw-r--r--   0        0        0     3435 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/dtos/campaign.py
+-rw-r--r--   0        0        0      285 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/dtos/floor.py
+-rw-r--r--   0        0        0      463 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/dtos/holding.py
+-rw-r--r--   0        0        0     1409 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/dtos/listing.py
+-rw-r--r--   0        0        0      365 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/dtos/rank.py
+-rw-r--r--   0        0        0     1792 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/dtos/sale.py
+-rw-r--r--   0        0        0        0 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/helpers/__init__.py
+-rw-r--r--   0        0        0      150 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/helpers/formatters.py
+-rw-r--r--   0        0        0     1895 2023-06-09 15:33:23.419378 bookio_fetchfox-0.7.0/fetchfox/rest.py
+-rw-r--r--   0        0        0     1148 2023-06-09 15:33:23.431378 bookio_fetchfox-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     4986 1970-01-01 00:00:00.000000 bookio_fetchfox-0.7.0/setup.py
+-rw-r--r--   0        0        0     4938 1970-01-01 00:00:00.000000 bookio_fetchfox-0.7.0/PKG-INFO
```

### Comparing `bookio_fetchfox-0.6.0/README.md` & `bookio_fetchfox-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.6.0/fetchfox/apis/algorand/algonodecloud.py` & `bookio_fetchfox-0.7.0/fetchfox/apis/algorand/algonodecloud.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.6.0/fetchfox/apis/algorand/algoxnftcom.py` & `bookio_fetchfox-0.7.0/fetchfox/apis/algorand/algoxnftcom.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.6.0/fetchfox/apis/algorand/nfdomains.py` & `bookio_fetchfox-0.7.0/fetchfox/apis/algorand/nfdomains.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.6.0/fetchfox/apis/algorand/nftexplorerapp.py` & `bookio_fetchfox-0.7.0/fetchfox/apis/algorand/nftexplorerapp.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.6.0/fetchfox/apis/algorand/randswapcom.py` & `bookio_fetchfox-0.7.0/fetchfox/apis/algorand/randswapcom.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.6.0/fetchfox/apis/cardano/blockfrostio.py` & `bookio_fetchfox-0.7.0/fetchfox/apis/cardano/blockfrostio.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.6.0/fetchfox/apis/cardano/cnfttools.py` & `bookio_fetchfox-0.7.0/fetchfox/apis/cardano/cnfttools.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.6.0/fetchfox/apis/cardano/handleme.py` & `bookio_fetchfox-0.7.0/fetchfox/apis/cardano/handleme.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.6.0/fetchfox/apis/cardano/jpgstore.py` & `bookio_fetchfox-0.7.0/fetchfox/apis/cardano/jpgstore.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.6.0/fetchfox/apis/coingeckocom.py` & `bookio_fetchfox-0.7.0/fetchfox/apis/coingeckocom.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.6.0/fetchfox/apis/evm/ensideascom.py` & `bookio_fetchfox-0.7.0/fetchfox/apis/evm/ensideascom.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.6.0/fetchfox/apis/evm/moralisio.py` & `bookio_fetchfox-0.7.0/fetchfox/apis/evm/moralisio.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.6.0/fetchfox/apis/evm/openseaio.py` & `bookio_fetchfox-0.7.0/fetchfox/apis/evm/openseaio.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.6.0/fetchfox/blockchains/algorand/blockchain.py` & `bookio_fetchfox-0.7.0/fetchfox/blockchains/algorand/blockchain.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 from datetime import datetime
-from typing import Iterable, Optional
+from typing import Iterable
 
 import pytz
 
 from fetchfox.apis.algorand import (
     algonodecloud,
     nfdomains,
     randswapcom,
@@ -16,15 +16,15 @@
 from fetchfox.constants.currencies import ALGO
 from fetchfox.constants.marketplaces import (
     ALGOXNFT_COM,
     RANDGALLERY_COM,
     SHUFL_APP,
     UNKNOWN,
 )
-from fetchfox.dtos import AssetDTO, FloorDTO, HoldingDTO, ListingDTO, SaleDTO
+from fetchfox.dtos import AssetDTO, CampaignDTO, FloorDTO, HoldingDTO, ListingDTO, SaleDTO
 from . import utils
 
 logger = logging.getLogger(__name__)
 
 
 class Algorand(Blockchain):
     def __init__(self, nftexplorerapp_api_key: str = None):
@@ -44,14 +44,20 @@
         if not utils.is_asset_id(asset_id):
             raise ValueError(f"{asset_id} is not a valid algorand asset id")
 
     def check_wallet(self, wallet: str):
         if not utils.is_wallet(wallet):
             raise ValueError(f"{wallet} is not a valid algorand address or nfdomain")
 
+    def explorer_url(self, collection_id: str) -> str:
+        return f"https://algoexplorer.io/address/{collection_id}"
+
+    def marketplace_url(self, collection_id: str) -> str:
+        return f"https://www.randgallery.com/algo-collection/?address={collection_id}"
+
     def get_assets(self, collection_id: str, fetch_metadata: bool = True, *args, **kwargs) -> Iterable[AssetDTO]:
         self.check_collection_id(collection_id)
 
         for asset_id in algonodecloud.get_assets(collection_id):
             if fetch_metadata:
                 yield self.get_asset(
                     collection_id=collection_id,
@@ -74,14 +80,17 @@
 
         return AssetDTO(
             collection_id=collection_id,
             asset_id=asset_id,
             metadata=metadata,
         )
 
+    def get_campaigns(self) -> Iterable[CampaignDTO]:
+        return
+
     def get_holdings(self, wallet: str, *args, **kwargs) -> Iterable[HoldingDTO]:
         self.check_wallet(wallet)
 
         if utils.is_nf_domain(wallet):
             wallet = nfdomains.resolve_nf_domain(wallet)
 
         holdings = algonodecloud.get_holdings(wallet)
```

### Comparing `bookio_fetchfox-0.6.0/fetchfox/blockchains/base.py` & `bookio_fetchfox-0.7.0/fetchfox/blockchains/base.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from abc import abstractmethod
-from typing import Iterable, Optional
+from typing import Iterable
 
 from fetchfox.apis import coingeckocom
 from fetchfox.dtos import (
     AssetDTO,
     CampaignDTO,
     FloorDTO,
     HoldingDTO,
@@ -31,14 +31,22 @@
         raise NotImplementedError()
 
     @abstractmethod
     def check_wallet(self, wallet: str):
         raise NotImplementedError()
 
     @abstractmethod
+    def explorer_url(self, collection_id: str) -> str:
+        raise NotImplementedError()
+
+    @abstractmethod
+    def marketplace_url(self, collection_id: str) -> str:
+        raise NotImplementedError()
+
+    @abstractmethod
     def get_assets(self, collection_id: str, fetch_metadata: bool = True, *args, **kwargs) -> Iterable[AssetDTO]:
         raise NotImplementedError()
 
     @abstractmethod
     def get_asset(self, collection_id: str, asset_id: str, *args, **kwargs) -> AssetDTO:
         raise NotImplementedError()
```

### Comparing `bookio_fetchfox-0.6.0/fetchfox/blockchains/cardano/blockchain.py` & `bookio_fetchfox-0.7.0/fetchfox/blockchains/cardano/blockchain.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 from datetime import datetime
 from functools import lru_cache
-from typing import Iterable, Optional
+from typing import Iterable
 
 import pytz
 
 from fetchfox.apis import bookio
 from fetchfox.apis.cardano import blockfrostio, cnfttools, handleme, jpgstore
 from fetchfox.blockchains.base import Blockchain
 from fetchfox.constants.blockchains import CARDANO
@@ -47,14 +47,20 @@
         if not utils.is_asset_id(asset_id):
             raise ValueError(f"{asset_id} is not a valid cardano asset id")
 
     def check_wallet(self, wallet: str):
         if not utils.is_wallet(wallet):
             raise ValueError(f"{wallet} is not a valid cardano address, stake key or ada handle")
 
+    def explorer_url(self, collection_id: str) -> str:
+        return f"https://cardanoscan.io/tokenPolicy/{collection_id}"
+
+    def marketplace_url(self, collection_id: str) -> str:
+        return f"https://www.jpg.store/collection/{collection_id}"
+
     @lru_cache
     def get_stake_key(self, wallet: str) -> str:
         self.check_wallet(wallet)
 
         if utils.is_stake_key(wallet):
             return wallet
 
@@ -118,28 +124,31 @@
         for campaign in bookio.campaigns():
             if campaign["blockchain"] != CARDANO:
                 continue
 
             landing = campaign["landing"]
             pricing = landing["price_description"].replace(" (+2 ADA that will be returned with your eBook)", "").strip()
 
+            collection_id = landing["lottery"]["collection_id"]
             start_at = campaign["start_at"]
 
             yield CampaignDTO(
                 blockchain=CARDANO,
                 parlamint_id=campaign["id"],
-                collection_id=landing["lottery"]["collection_id"],
+                collection_id=collection_id,
                 name=campaign["display_name"],
                 description=campaign["landing"]["opener"],
-                supply=campaign["total_deas"],
-                limit=campaign["max_quantity"],
                 price=landing["price"],
+                supply=campaign["total_deas"],
                 pricing=pricing,
-                rarity_chart_url=landing["rarity_chart_url"],
+                limit=campaign["max_quantity"],
                 start_at=formatters.timestamp(start_at["start_at"]),
+                explorer_url=f"https://pool.pm/nfts/{collection_id}",
+                marketplace_url=self.marketplace_url(collection_id),
+                rarity_chart_url=landing["rarity_chart_url"],
             )
 
     def get_holdings(self, wallet: str, *args, **kwargs) -> Iterable[HoldingDTO]:
         self.check_wallet(wallet)
 
         stake_address = self.get_stake_key(wallet)
```

### Comparing `bookio_fetchfox-0.6.0/fetchfox/blockchains/cardano/utils.py` & `bookio_fetchfox-0.7.0/fetchfox/blockchains/cardano/utils.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.6.0/fetchfox/blockchains/ethereum/blockchain.py` & `bookio_fetchfox-0.7.0/fetchfox/blockchains/polygon/blockchain.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from fetchfox.blockchains.evm import Evm
-from fetchfox.constants.blockchains import ETHEREUM
-from fetchfox.constants.currencies import ETH
+from fetchfox.constants.blockchains import POLYGON
+from fetchfox.constants.currencies import MATIC
 
 
-class Ethereum(Evm):
+class Polygon(Evm):
     def __init__(
         self,
         moralisio_api_key: str = None,
         openseaio_api_key: str = None,
     ):
         super().__init__(
-            name=ETHEREUM,
-            currency=ETH,
-            logo="https://s2.coinmarketcap.com/static/img/coins/64x64/1027.png",
+            name=POLYGON,
+            currency=MATIC,
+            logo="https://s2.coinmarketcap.com/static/img/coins/64x64/3890.png",
             moralisio_api_key=moralisio_api_key,
             openseaio_api_key=openseaio_api_key,
         )
+
+    def explorer_url(self, collection_id: str) -> str:
+        return f"https://polygonscan.com/address/{collection_id}"
```

### Comparing `bookio_fetchfox-0.6.0/fetchfox/blockchains/evm/blockchain.py` & `bookio_fetchfox-0.7.0/fetchfox/blockchains/evm/blockchain.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 import logging
 from datetime import datetime
-from typing import Iterable, Optional
+from typing import Iterable
 
 import pytz
 
 from fetchfox.apis import bookio
 from fetchfox.apis.evm import moralisio, ensideascom, openseaio
 from fetchfox.blockchains.base import Blockchain
 from fetchfox.constants.blockchains import ETHEREUM, POLYGON
@@ -32,14 +32,17 @@
         if not utils.is_asset_id(asset_id):
             raise ValueError(f"{asset_id} is not a valid {self.name} asset id")
 
     def check_wallet(self, wallet: str):
         if not utils.is_wallet(wallet):
             raise ValueError(f"{wallet} is not a valid {self.name} address or ens domain")
 
+    def marketplace_url(self, collection_id: str) -> str:
+        return f"https://opensea.io/assets?search[query]={collection_id}"
+
     def get_assets(self, collection_id: str, fetch_metadata: bool = True, *args, **kwargs) -> Iterable[AssetDTO]:
         self.check_collection_id(collection_id)
 
         if fetch_metadata:
             asset_id = -1
 
             while True:
@@ -101,26 +104,30 @@
             if campaign["network"] != network:
                 continue
 
             landing = campaign["landing"]
             platform = campaign["platform"]
             start_at = campaign["start_at"]
 
+            collection_id = platform["ThirdWeb"]["contract_address"]
+
             yield CampaignDTO(
                 blockchain=self.name,
                 parlamint_id=campaign["id"],
-                collection_id=platform["ThirdWeb"]["contract_address"],
+                collection_id=collection_id,
                 name=campaign["display_name"],
                 description=campaign["landing"]["opener"],
                 price=landing["price"],
                 supply=campaign["total_deas"],
-                limit=campaign["max_quantity"],
                 pricing=landing["price_description"],
-                rarity_chart_url=landing["rarity_chart_url"],
+                limit=campaign["max_quantity"],
                 start_at=formatters.timestamp(start_at["start_at"]),
+                explorer_url=self.explorer_url(collection_id),
+                marketplace_url=self.marketplace_url(collection_id),
+                rarity_chart_url=landing["rarity_chart_url"],
             )
 
     def get_holdings(self, wallet: str, *args, **kwargs) -> Iterable[HoldingDTO]:
         self.check_wallet(wallet)
 
         if utils.is_ens_domain(wallet):
             wallet = ensideascom.resolve_ens_domain(wallet)
```

### Comparing `bookio_fetchfox-0.6.0/fetchfox/blockchains/evm/utils.py` & `bookio_fetchfox-0.7.0/fetchfox/blockchains/evm/utils.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.6.0/fetchfox/dtos/asset.py` & `bookio_fetchfox-0.7.0/fetchfox/dtos/asset.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.6.0/fetchfox/dtos/campaign.py` & `bookio_fetchfox-0.7.0/fetchfox/dtos/sale.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,44 +1,63 @@
 from datetime import datetime
+from enum import Enum
+from typing import List
 
+from fetchfox.apis import coingeckocom
 
-class CampaignDTO:
+
+class SaleType(str, Enum):
+    OFFER = "OFFER"
+    COLLECTION_OFFER = "INSTANT"
+    PURCHASE = "PURCHASE"
+    CREDIT_CARD = "CREDIT_CARD"
+
+
+class SaleDTO:
     def __init__(
         self,
-        blockchain: str,
-        parlamint_id: str,
+        identifier: str,
         collection_id: str,
-        name: str,
-        description: str,
-        price: int,
-        supply: int,
-        pricing: str,
-        limit: int,
-        rarity_chart_url: str,
-        start_at: datetime,
+        asset_ids: List[str],
+        asset_names: List[str],
+        tx_hash: str,
+        marketplace: str,
+        price: float,
+        currency: str,
+        confirmed_at: datetime,
+        type: SaleType = SaleType.PURCHASE,
+        sale_id: str = None,
+        sold_by: str = None,
+        bought_by: str = None,
+        marketplace_url: str = None,
+        explorer_url: str = None,
     ):
-        self.blockchain: str = blockchain
-
-        self.parlamint_id: str = parlamint_id.lower()
-        self.collection_id: str = collection_id.lower() if collection_id else None
-
-        self.name: str = name
-        self.description: str = description
-        self.price: int = price
-        self.supply: int = supply
-        self.pricing: str = pricing.replace("<br>", "\n").strip()
-        self.limit: int = limit
-        self.rarity_chart_url: str = rarity_chart_url
-        self.start_at: datetime = start_at
+        self.identifier: str = identifier
+        self.collection_id: str = collection_id
+        self.asset_ids: List[str] = asset_ids
+        self.asset_names: List[str] = asset_names
+        self.tx_hash: str = tx_hash
+        self.marketplace: str = marketplace
+        self.price: float = price
+        self.currency: str = currency
+        self.confirmed_at: datetime = confirmed_at
+        self.type: SaleType = type
+        self.sale_id: str = sale_id
+        self.sold_by: str = sold_by
+        self.bought_by: str = bought_by
+        self.marketplace_url: str = marketplace_url
+        self.explorer_url: str = explorer_url
 
     @property
-    def new(self) -> bool:
-        now = datetime.utcnow().replace(tzinfo=pytz.UTC)
+    def usd(self) -> float:
+        return self.price * coingeckocom.usd(self.currency)
 
-        return self.start_at > now
+    @property
+    def first(self) -> str:
+        return self.asset_ids[0]
 
     @property
-    def parlamint_url(self) -> str:
-        return f"https://app.book.io/parlamint/campaigns/{self.parlamint_id}"
+    def is_bundle(self) -> bool:
+        return len(self.asset_ids) > 1
 
-    def __repr__(self):
-        return f"{self.name} ({self.collection_id})"
+    def __repr__(self) -> str:
+        return f"{self.collection_id}/{self.first} x {self.price} {self.currency} ({self.marketplace})"
```

### Comparing `bookio_fetchfox-0.6.0/fetchfox/dtos/listing.py` & `bookio_fetchfox-0.7.0/fetchfox/dtos/listing.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.6.0/fetchfox/rest.py` & `bookio_fetchfox-0.7.0/fetchfox/rest.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.6.0/pyproject.toml` & `bookio_fetchfox-0.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bookio-fetchfox"
-version = "0.6.0"
+version = "0.7.0"
 description = "Collection of API services to fetch information from several blockchains."
 documentation = "https://github.com/book-io/fetchfox/blob/main/README.md"
 homepage = "https://github.com/book-io/fetchfox"
 license = "MIT"
 readme = "README.md"
 
 authors = [
```

### Comparing `bookio_fetchfox-0.6.0/setup.py` & `bookio_fetchfox-0.7.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
  'asyncio>=3.4.3,<4.0.0',
  'backoff>=2.2.1,<3.0.0',
  'cachetools>=5.3.1,<6.0.0',
  'pytz>=2023.3,<2024.0']
 
 setup_kwargs = {
     'name': 'bookio-fetchfox',
-    'version': '0.6.0',
+    'version': '0.7.0',
     'description': 'Collection of API services to fetch information from several blockchains.',
     'long_description': '# book.io / fetchfox\n\n> Collection of API services to fetch information from several blockchains.\n\n![](https://s2.coinmarketcap.com/static/img/coins/64x64/4030.png)\n![](https://s2.coinmarketcap.com/static/img/coins/64x64/2010.png)\n![](https://s2.coinmarketcap.com/static/img/coins/64x64/1027.png)\n![](https://s2.coinmarketcap.com/static/img/coins/64x64/3890.png)\n\n\n## Supported Blockchains\n\n### Algorand\n\n```python\nimport os\nfrom fetchfox.blockchains import Algorand\n\nalgorand = Algorand(\n    nftexplorerapp_api_key=os.getenv("NFTEXPLORER_API_KEY"),\n)\n\n# Brave New World\ncreator_address = "6WII6ES4H6UW7G7T7RJX63CUNPKJEPEGQ3PTYVVU3JHJ652W34GCJV5OVY"\n\nfor asset in algorand.get_assets(creator_address):\n    print(asset)\n```\n\n#### Services\n\n* get_asset ([algonode.cloud](https://algonode.cloud))\n* get_assets ([algonode.cloud](https://algonode.cloud))\n* get_holdings ([algonode.cloud](https://algonode.cloud))\n* get_snapshot ([algonode.cloud](https://algonode.cloud))\n* get_campaigns ([book.io](https://book.io))\n* get_listings ([randgallery.com](https://randgallery.com) / [algoxnft.com](https://algoxnft.com))\n* get_floor ([randgallery.com](https://randgallery.com) / [algoxnft.com](https://algoxnft.com))\n* get_sales ([nftexplorer.app¹](https://nftexplorer.app))\n\n\n### Cardano\n\n```python\nimport os\nfrom fetchfox.blockchains import Cardano\n\ncardano = Cardano(\n    blockfrostio_project_id=os.getenv("BLOCKFROST_PROJECT_ID"),\n)\n\n# Gutenberg Bible\npolicy_id = "477cec772adb1466b301fb8161f505aa66ed1ee8d69d3e7984256a43"\n\nfor asset in cardano.get_assets(policy_id):\n    print(asset)\n```\n\n#### Services\n\n* get_asset ([blockfrost.io²](https://blockfrost.io))\n* get_assets ([blockfrost.io²](https://blockfrost.io))\n* get_holdings ([blockfrost.io²](https://blockfrost.io))\n* get_campaigns ([book.io](https://book.io))\n* get_snapshot ([blockfrost.io²](https://blockfrost.io))\n* get_listings ([jpg.store](https://jpg.store))\n* get_floor ([jpg.store](https://jpg.store))\n* get_sales ([jpg.store](https://jpg.store))\n* get_ranks ([cnft.tools](https://cnft.tools))\n\n\n### EVM (Ethereum and Polygon)\n\n```python\nimport os\nfrom fetchfox.blockchains import Ethereum, Polygon\n\nethereum = Ethereum(\n    geckodriver_path=os.getenv("GECKODRIVER_PATH"),\n    moralisio_api_key=os.getenv("MORALIS_API_KEY"),\n    openseaio_api_key=os.getenv("OPENSEA_API_KEY"),\n)\n\npolygon = Polygon(\n    geckodriver_path=os.getenv("GECKODRIVER_PATH"),\n    moralisio_api_key=os.getenv("MORALIS_API_KEY"),\n    openseaio_api_key=os.getenv("OPENSEA_API_KEY"),\n)\n\n\n# Alice in Wonderland\ncontract_address = "0x919da7fef646226f88f70305201de392ff365059"\n\nfor asset in ethereum.get_assets(contract_address):\n    print(asset)\n\n# Art of War\ncontract_address = "0xb56010e0500e4f163758881603b8083996ae47ec"\n\nfor asset in polygon.get_assets(contract_address):\n    print(asset)\n```\n\n#### Services\n\n* get_asset ([moralis.io³](https://moralis.io))\n* get_assets ([moralis.io³](https://moralis.io))\n* get_holdings ([moralis.io³](https://moralis.io))\n* get_snapshot ([moralis.io³](https://moralis.io))\n* get_campaigns ([book.io](https://book.io))\n* get_listings ([opensea.io⁴](https://opensea.io))\n* get_floor ([opensea.io⁴](https://opensea.io))\n* get_sales ([opensea.io⁴](https://opensea.io))\n\n\n> ¹ **nftexplorer.app** services require an [api key](https://www.nftexplorer.app/nftx-api).\n> \n> ² **blockfrost.io** services require a [project id](https://blockfrost.dev/docs/overview/plans-and-billing).\n> \n> ³ **moralis.io** services require an [api key](https://moralis.io/pricing).\n> \n> ⁴ **opensea.io** some services also require an [api key](https://docs.opensea.io/reference/api-keys). \n\n---\n\n![fetch, the fox](https://i.imgur.com/fm6mqzS.png)\n> fetch, the fox\n\n',
     'author': 'Fede',
     'author_email': 'fede@book.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/book-io/fetchfox',
```

### Comparing `bookio_fetchfox-0.6.0/PKG-INFO` & `bookio_fetchfox-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bookio-fetchfox
-Version: 0.6.0
+Version: 0.7.0
 Summary: Collection of API services to fetch information from several blockchains.
 Home-page: https://github.com/book-io/fetchfox
 License: MIT
 Keywords: book.io,blockchain,crypto,algorand,cardano,ethereum,polygon
 Author: Fede
 Author-email: fede@book.io
 Requires-Python: >=3.8,<4.0
```

