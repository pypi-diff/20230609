# Comparing `tmp/bookio_fetchfox-0.5.0.tar.gz` & `tmp/bookio_fetchfox-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bookio_fetchfox-0.5.0.tar", max compression
+gzip compressed data, was "bookio_fetchfox-0.6.0.tar", max compression
```

## Comparing `bookio_fetchfox-0.5.0.tar` & `bookio_fetchfox-0.6.0.tar`

### file list

```diff
@@ -1,56 +1,57 @@
--rw-r--r--   0        0        0     3723 2023-06-08 23:09:31.623263 bookio_fetchfox-0.5.0/README.md
--rw-r--r--   0        0        0        0 2023-06-08 23:09:31.623263 bookio_fetchfox-0.5.0/fetchfox/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 23:09:31.623263 bookio_fetchfox-0.5.0/fetchfox/apis/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 23:09:31.623263 bookio_fetchfox-0.5.0/fetchfox/apis/algorand/__init__.py
--rw-r--r--   0        0        0     2140 2023-06-08 23:09:31.623263 bookio_fetchfox-0.5.0/fetchfox/apis/algorand/algonodecloud.py
--rw-r--r--   0        0        0      596 2023-06-08 23:09:31.623263 bookio_fetchfox-0.5.0/fetchfox/apis/algorand/algoxnftcom.py
--rw-r--r--   0        0        0     1349 2023-06-08 23:09:31.623263 bookio_fetchfox-0.5.0/fetchfox/apis/algorand/nfdomains.py
--rw-r--r--   0        0        0     1764 2023-06-08 23:09:31.623263 bookio_fetchfox-0.5.0/fetchfox/apis/algorand/nftexplorerapp.py
--rw-r--r--   0        0        0      592 2023-06-08 23:09:31.623263 bookio_fetchfox-0.5.0/fetchfox/apis/algorand/randswapcom.py
--rw-r--r--   0        0        0      262 2023-06-08 23:09:31.623263 bookio_fetchfox-0.5.0/fetchfox/apis/bookio.py
--rw-r--r--   0        0        0        0 2023-06-08 23:09:31.623263 bookio_fetchfox-0.5.0/fetchfox/apis/cardano/__init__.py
--rw-r--r--   0        0        0     2658 2023-06-08 23:09:31.623263 bookio_fetchfox-0.5.0/fetchfox/apis/cardano/blockfrostio.py
--rw-r--r--   0        0        0      734 2023-06-08 23:09:31.623263 bookio_fetchfox-0.5.0/fetchfox/apis/cardano/cnfttools.py
--rw-r--r--   0        0        0     1056 2023-06-08 23:09:31.623263 bookio_fetchfox-0.5.0/fetchfox/apis/cardano/handleme.py
--rw-r--r--   0        0        0     1606 2023-06-08 23:09:31.623263 bookio_fetchfox-0.5.0/fetchfox/apis/cardano/jpgstore.py
--rwxr-xr-x   0        0        0      675 2023-06-08 23:09:31.623263 bookio_fetchfox-0.5.0/fetchfox/apis/coingeckocom.py
--rw-r--r--   0        0        0        0 2023-06-08 23:09:31.623263 bookio_fetchfox-0.5.0/fetchfox/apis/evm/__init__.py
--rw-r--r--   0        0        0      963 2023-06-08 23:09:31.623263 bookio_fetchfox-0.5.0/fetchfox/apis/evm/ensideascom.py
--rw-r--r--   0        0        0     4147 2023-06-08 23:09:31.623263 bookio_fetchfox-0.5.0/fetchfox/apis/evm/moralisio.py
--rw-r--r--   0        0        0     2555 2023-06-08 23:09:31.623263 bookio_fetchfox-0.5.0/fetchfox/apis/evm/openseaio.py
--rw-r--r--   0        0        0      120 2023-06-08 23:09:31.623263 bookio_fetchfox-0.5.0/fetchfox/blockchains/__init__.py
--rw-r--r--   0        0        0       33 2023-06-08 23:09:31.623263 bookio_fetchfox-0.5.0/fetchfox/blockchains/algorand/__init__.py
--rw-r--r--   0        0        0     7852 2023-06-08 23:09:31.623263 bookio_fetchfox-0.5.0/fetchfox/blockchains/algorand/blockchain.py
--rw-r--r--   0        0        0      504 2023-06-08 23:09:31.623263 bookio_fetchfox-0.5.0/fetchfox/blockchains/algorand/utils.py
--rw-r--r--   0        0        0     2161 2023-06-08 23:09:31.623263 bookio_fetchfox-0.5.0/fetchfox/blockchains/base.py
--rw-r--r--   0        0        0       32 2023-06-08 23:09:31.623263 bookio_fetchfox-0.5.0/fetchfox/blockchains/cardano/__init__.py
--rw-r--r--   0        0        0    11921 2023-06-08 23:09:31.623263 bookio_fetchfox-0.5.0/fetchfox/blockchains/cardano/blockchain.py
--rw-r--r--   0        0        0     1061 2023-06-08 23:09:31.623263 bookio_fetchfox-0.5.0/fetchfox/blockchains/cardano/utils.py
--rw-r--r--   0        0        0       33 2023-06-08 23:09:31.623263 bookio_fetchfox-0.5.0/fetchfox/blockchains/ethereum/__init__.py
--rw-r--r--   0        0        0      547 2023-06-08 23:09:31.623263 bookio_fetchfox-0.5.0/fetchfox/blockchains/ethereum/blockchain.py
--rw-r--r--   0        0        0       28 2023-06-08 23:09:31.623263 bookio_fetchfox-0.5.0/fetchfox/blockchains/evm/__init__.py
--rw-r--r--   0        0        0     9571 2023-06-08 23:09:31.623263 bookio_fetchfox-0.5.0/fetchfox/blockchains/evm/blockchain.py
--rw-r--r--   0        0        0      619 2023-06-08 23:09:31.623263 bookio_fetchfox-0.5.0/fetchfox/blockchains/evm/utils.py
--rw-r--r--   0        0        0       32 2023-06-08 23:09:31.623263 bookio_fetchfox-0.5.0/fetchfox/blockchains/polygon/__init__.py
--rw-r--r--   0        0        0      548 2023-06-08 23:09:31.623263 bookio_fetchfox-0.5.0/fetchfox/blockchains/polygon/blockchain.py
--rw-r--r--   0        0        0      154 2023-06-08 23:09:31.623263 bookio_fetchfox-0.5.0/fetchfox/blockchains/utils.py
--rw-r--r--   0        0        0      322 2023-06-08 23:09:31.623263 bookio_fetchfox-0.5.0/fetchfox/checks.py
--rw-r--r--   0        0        0        0 2023-06-08 23:09:31.623263 bookio_fetchfox-0.5.0/fetchfox/constants/__init__.py
--rw-r--r--   0        0        0      158 2023-06-08 23:09:31.623263 bookio_fetchfox-0.5.0/fetchfox/constants/blockchains.py
--rw-r--r--   0        0        0      112 2023-06-08 23:09:31.623263 bookio_fetchfox-0.5.0/fetchfox/constants/currencies.py
--rw-r--r--   0        0        0      296 2023-06-08 23:09:31.623263 bookio_fetchfox-0.5.0/fetchfox/constants/marketplaces.py
--rw-r--r--   0        0        0       95 2023-06-08 23:09:31.623263 bookio_fetchfox-0.5.0/fetchfox/constants/sales.py
--rw-r--r--   0        0        0       28 2023-06-08 23:09:31.623263 bookio_fetchfox-0.5.0/fetchfox/constants/specials.py
--rw-r--r--   0        0        0      188 2023-06-08 23:09:31.623263 bookio_fetchfox-0.5.0/fetchfox/dtos/__init__.py
--rw-r--r--   0        0        0     2263 2023-06-08 23:09:31.623263 bookio_fetchfox-0.5.0/fetchfox/dtos/asset.py
--rw-r--r--   0        0        0     1215 2023-06-08 23:09:31.623263 bookio_fetchfox-0.5.0/fetchfox/dtos/campaign.py
--rw-r--r--   0        0        0      463 2023-06-08 23:09:31.623263 bookio_fetchfox-0.5.0/fetchfox/dtos/holding.py
--rw-r--r--   0        0        0     1409 2023-06-08 23:09:31.623263 bookio_fetchfox-0.5.0/fetchfox/dtos/listing.py
--rw-r--r--   0        0        0      365 2023-06-08 23:09:31.623263 bookio_fetchfox-0.5.0/fetchfox/dtos/rank.py
--rw-r--r--   0        0        0     1792 2023-06-08 23:09:31.623263 bookio_fetchfox-0.5.0/fetchfox/dtos/sale.py
--rw-r--r--   0        0        0        0 2023-06-08 23:09:31.623263 bookio_fetchfox-0.5.0/fetchfox/helpers/__init__.py
--rw-r--r--   0        0        0      150 2023-06-08 23:09:31.623263 bookio_fetchfox-0.5.0/fetchfox/helpers/formatters.py
--rw-r--r--   0        0        0     1895 2023-06-08 23:09:31.623263 bookio_fetchfox-0.5.0/fetchfox/rest.py
--rw-r--r--   0        0        0     1148 2023-06-08 23:09:31.639263 bookio_fetchfox-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     4986 1970-01-01 00:00:00.000000 bookio_fetchfox-0.5.0/setup.py
--rw-r--r--   0        0        0     4938 1970-01-01 00:00:00.000000 bookio_fetchfox-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     3723 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/apis/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/apis/algorand/__init__.py
+-rw-r--r--   0        0        0     2140 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/apis/algorand/algonodecloud.py
+-rw-r--r--   0        0        0      596 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/apis/algorand/algoxnftcom.py
+-rw-r--r--   0        0        0     1349 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/apis/algorand/nfdomains.py
+-rw-r--r--   0        0        0     1764 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/apis/algorand/nftexplorerapp.py
+-rw-r--r--   0        0        0      592 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/apis/algorand/randswapcom.py
+-rw-r--r--   0        0        0      262 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/apis/bookio.py
+-rw-r--r--   0        0        0        0 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/apis/cardano/__init__.py
+-rw-r--r--   0        0        0     2658 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/apis/cardano/blockfrostio.py
+-rw-r--r--   0        0        0      734 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/apis/cardano/cnfttools.py
+-rw-r--r--   0        0        0     1056 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/apis/cardano/handleme.py
+-rw-r--r--   0        0        0     1606 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/apis/cardano/jpgstore.py
+-rwxr-xr-x   0        0        0      675 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/apis/coingeckocom.py
+-rw-r--r--   0        0        0        0 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/apis/evm/__init__.py
+-rw-r--r--   0        0        0      963 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/apis/evm/ensideascom.py
+-rw-r--r--   0        0        0     4147 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/apis/evm/moralisio.py
+-rw-r--r--   0        0        0     2555 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/apis/evm/openseaio.py
+-rw-r--r--   0        0        0      120 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/blockchains/__init__.py
+-rw-r--r--   0        0        0       33 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/blockchains/algorand/__init__.py
+-rw-r--r--   0        0        0     7966 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/blockchains/algorand/blockchain.py
+-rw-r--r--   0        0        0      504 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/blockchains/algorand/utils.py
+-rw-r--r--   0        0        0     2163 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/blockchains/base.py
+-rw-r--r--   0        0        0       32 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/blockchains/cardano/__init__.py
+-rw-r--r--   0        0        0    12039 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/blockchains/cardano/blockchain.py
+-rw-r--r--   0        0        0     1061 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/blockchains/cardano/utils.py
+-rw-r--r--   0        0        0       33 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/blockchains/ethereum/__init__.py
+-rw-r--r--   0        0        0      547 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/blockchains/ethereum/blockchain.py
+-rw-r--r--   0        0        0       28 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/blockchains/evm/__init__.py
+-rw-r--r--   0        0        0     9685 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/blockchains/evm/blockchain.py
+-rw-r--r--   0        0        0      619 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/blockchains/evm/utils.py
+-rw-r--r--   0        0        0       32 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/blockchains/polygon/__init__.py
+-rw-r--r--   0        0        0      548 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/blockchains/polygon/blockchain.py
+-rw-r--r--   0        0        0      154 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/blockchains/utils.py
+-rw-r--r--   0        0        0      322 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/checks.py
+-rw-r--r--   0        0        0        0 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/constants/__init__.py
+-rw-r--r--   0        0        0      158 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/constants/blockchains.py
+-rw-r--r--   0        0        0      112 2023-06-09 12:41:03.732420 bookio_fetchfox-0.6.0/fetchfox/constants/currencies.py
+-rw-r--r--   0        0        0      296 2023-06-09 12:41:03.736420 bookio_fetchfox-0.6.0/fetchfox/constants/marketplaces.py
+-rw-r--r--   0        0        0       95 2023-06-09 12:41:03.736420 bookio_fetchfox-0.6.0/fetchfox/constants/sales.py
+-rw-r--r--   0        0        0       28 2023-06-09 12:41:03.736420 bookio_fetchfox-0.6.0/fetchfox/constants/specials.py
+-rw-r--r--   0        0        0      216 2023-06-09 12:41:03.736420 bookio_fetchfox-0.6.0/fetchfox/dtos/__init__.py
+-rw-r--r--   0        0        0     2263 2023-06-09 12:41:03.736420 bookio_fetchfox-0.6.0/fetchfox/dtos/asset.py
+-rw-r--r--   0        0        0     1215 2023-06-09 12:41:03.736420 bookio_fetchfox-0.6.0/fetchfox/dtos/campaign.py
+-rw-r--r--   0        0        0      285 2023-06-09 12:41:03.736420 bookio_fetchfox-0.6.0/fetchfox/dtos/floor.py
+-rw-r--r--   0        0        0      463 2023-06-09 12:41:03.736420 bookio_fetchfox-0.6.0/fetchfox/dtos/holding.py
+-rw-r--r--   0        0        0     1409 2023-06-09 12:41:03.736420 bookio_fetchfox-0.6.0/fetchfox/dtos/listing.py
+-rw-r--r--   0        0        0      365 2023-06-09 12:41:03.736420 bookio_fetchfox-0.6.0/fetchfox/dtos/rank.py
+-rw-r--r--   0        0        0     1792 2023-06-09 12:41:03.736420 bookio_fetchfox-0.6.0/fetchfox/dtos/sale.py
+-rw-r--r--   0        0        0        0 2023-06-09 12:41:03.736420 bookio_fetchfox-0.6.0/fetchfox/helpers/__init__.py
+-rw-r--r--   0        0        0      150 2023-06-09 12:41:03.736420 bookio_fetchfox-0.6.0/fetchfox/helpers/formatters.py
+-rw-r--r--   0        0        0     1895 2023-06-09 12:41:03.736420 bookio_fetchfox-0.6.0/fetchfox/rest.py
+-rw-r--r--   0        0        0     1148 2023-06-09 12:41:03.748420 bookio_fetchfox-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     4986 1970-01-01 00:00:00.000000 bookio_fetchfox-0.6.0/setup.py
+-rw-r--r--   0        0        0     4938 1970-01-01 00:00:00.000000 bookio_fetchfox-0.6.0/PKG-INFO
```

### Comparing `bookio_fetchfox-0.5.0/README.md` & `bookio_fetchfox-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.5.0/fetchfox/apis/algorand/algonodecloud.py` & `bookio_fetchfox-0.6.0/fetchfox/apis/algorand/algonodecloud.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.5.0/fetchfox/apis/algorand/algoxnftcom.py` & `bookio_fetchfox-0.6.0/fetchfox/apis/algorand/algoxnftcom.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.5.0/fetchfox/apis/algorand/nfdomains.py` & `bookio_fetchfox-0.6.0/fetchfox/apis/algorand/nfdomains.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.5.0/fetchfox/apis/algorand/nftexplorerapp.py` & `bookio_fetchfox-0.6.0/fetchfox/apis/algorand/nftexplorerapp.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.5.0/fetchfox/apis/algorand/randswapcom.py` & `bookio_fetchfox-0.6.0/fetchfox/apis/algorand/randswapcom.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.5.0/fetchfox/apis/cardano/blockfrostio.py` & `bookio_fetchfox-0.6.0/fetchfox/apis/cardano/blockfrostio.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.5.0/fetchfox/apis/cardano/cnfttools.py` & `bookio_fetchfox-0.6.0/fetchfox/apis/cardano/cnfttools.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.5.0/fetchfox/apis/cardano/handleme.py` & `bookio_fetchfox-0.6.0/fetchfox/apis/cardano/handleme.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.5.0/fetchfox/apis/cardano/jpgstore.py` & `bookio_fetchfox-0.6.0/fetchfox/apis/cardano/jpgstore.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.5.0/fetchfox/apis/coingeckocom.py` & `bookio_fetchfox-0.6.0/fetchfox/apis/coingeckocom.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.5.0/fetchfox/apis/evm/ensideascom.py` & `bookio_fetchfox-0.6.0/fetchfox/apis/evm/ensideascom.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.5.0/fetchfox/apis/evm/moralisio.py` & `bookio_fetchfox-0.6.0/fetchfox/apis/evm/moralisio.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.5.0/fetchfox/apis/evm/openseaio.py` & `bookio_fetchfox-0.6.0/fetchfox/apis/evm/openseaio.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.5.0/fetchfox/blockchains/algorand/blockchain.py` & `bookio_fetchfox-0.6.0/fetchfox/blockchains/algorand/blockchain.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from fetchfox.constants.currencies import ALGO
 from fetchfox.constants.marketplaces import (
     ALGOXNFT_COM,
     RANDGALLERY_COM,
     SHUFL_APP,
     UNKNOWN,
 )
-from fetchfox.dtos import AssetDTO, HoldingDTO, ListingDTO, SaleDTO
+from fetchfox.dtos import AssetDTO, FloorDTO, HoldingDTO, ListingDTO, SaleDTO
 from . import utils
 
 logger = logging.getLogger(__name__)
 
 
 class Algorand(Blockchain):
     def __init__(self, nftexplorerapp_api_key: str = None):
@@ -164,26 +164,32 @@
                 price=listing["price"] // 10**6,
                 currency=self.currency,
                 listed_at=listed_at,
                 listed_by=listing["seller"],
                 marketplace_url=f"https://algoxnft.com/asset/{asset_id}",
             )
 
-    def get_floor(self, collection_id: str, *args, **kwargs) -> Optional[ListingDTO]:
+    def get_floor(self, collection_id: str, *args, **kwargs) -> FloorDTO:
         self.check_collection_id(collection_id)
 
         floor = None
+        count = 0
 
         for listing in self.get_listings(collection_id):
+            count += 1
+
             if floor is None:
                 floor = listing
             elif listing.usd < floor.usd:
                 floor = listing
 
-        return floor
+        return FloorDTO(
+            listing=floor,
+            listing_count=count,
+        )
 
     def get_sales(self, collection_id: str, *args, **kwargs) -> Iterable[SaleDTO]:
         self.check_collection_id(collection_id)
 
         venues = {
             "algoxnft": ALGOXNFT_COM,
             "randgallery": RANDGALLERY_COM,
```

### Comparing `bookio_fetchfox-0.5.0/fetchfox/blockchains/base.py` & `bookio_fetchfox-0.6.0/fetchfox/blockchains/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from abc import abstractmethod
 from typing import Iterable, Optional
 
 from fetchfox.apis import coingeckocom
 from fetchfox.dtos import (
     AssetDTO,
     CampaignDTO,
+    FloorDTO,
     HoldingDTO,
     ListingDTO,
     RankDTO,
     SaleDTO,
 )
 
 
@@ -49,15 +50,15 @@
         raise NotImplementedError()
 
     @abstractmethod
     def get_listings(self, collection_id: str, *args, **kwargs) -> Iterable[ListingDTO]:
         raise NotImplementedError()
 
     @abstractmethod
-    def get_floor(self, collection_id: str, *args, **kwargs) -> Optional[ListingDTO]:
+    def get_floor(self, collection_id: str, *args, **kwargs) -> FloorDTO:
         raise NotImplementedError()
 
     def get_rank(self, collection_id: str, asset_id: str, *args, **kwargs) -> RankDTO:
         raise NotImplementedError()
 
     def get_ranks(self, collection_id: str, *args, **kwargs) -> Iterable[RankDTO]:
         raise NotImplementedError()
```

### Comparing `bookio_fetchfox-0.5.0/fetchfox/blockchains/cardano/blockchain.py` & `bookio_fetchfox-0.6.0/fetchfox/blockchains/cardano/blockchain.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from fetchfox.blockchains.base import Blockchain
 from fetchfox.constants.blockchains import CARDANO
 from fetchfox.constants.currencies import ADA
 from fetchfox.constants.marketplaces import JPG_STORE
 from fetchfox.dtos import (
     AssetDTO,
     CampaignDTO,
+    FloorDTO,
     HoldingDTO,
     ListingDTO,
     RankDTO,
     SaleDTO,
     SaleType,
 )
 from fetchfox.helpers import formatters
@@ -253,26 +254,32 @@
                 currency=self.currency,
                 listed_at=listed_at,
                 listed_by=None,
                 tx_hash=listing["tx_hash"],
                 marketplace_url=f"https://www.jpg.store/asset/{asset_id}",
             )
 
-    def get_floor(self, collection_id: str, discriminator: str = None, *args, **kwargs) -> Optional[ListingDTO]:
+    def get_floor(self, collection_id: str, discriminator: str = None, *args, **kwargs) -> FloorDTO:
         self.check_collection_id(collection_id)
 
         floor = None
+        count = 0
 
         for listing in self.get_listings(collection_id, discriminator=discriminator):
+            count += 1
+
             if floor is None:
                 floor = listing
             elif listing.usd < floor.usd:
                 floor = listing
 
-        return floor
+        return FloorDTO(
+            listing=floor,
+            listing_count=count,
+        )
 
     def get_sales(self, collection_id: str, discriminator: str = None, *args, **kwargs) -> Iterable[SaleDTO]:
         self.check_collection_id(collection_id)
 
         for sale in jpgstore.get_sales(collection_id):
             tx_hash = sale["tx_hash"]
```

### Comparing `bookio_fetchfox-0.5.0/fetchfox/blockchains/cardano/utils.py` & `bookio_fetchfox-0.6.0/fetchfox/blockchains/cardano/utils.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.5.0/fetchfox/blockchains/ethereum/blockchain.py` & `bookio_fetchfox-0.6.0/fetchfox/blockchains/ethereum/blockchain.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.5.0/fetchfox/blockchains/evm/blockchain.py` & `bookio_fetchfox-0.6.0/fetchfox/blockchains/evm/blockchain.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import pytz
 
 from fetchfox.apis import bookio
 from fetchfox.apis.evm import moralisio, ensideascom, openseaio
 from fetchfox.blockchains.base import Blockchain
 from fetchfox.constants.blockchains import ETHEREUM, POLYGON
 from fetchfox.constants.marketplaces import OPENSEA_IO
-from fetchfox.dtos import AssetDTO, CampaignDTO, HoldingDTO, ListingDTO, SaleDTO
+from fetchfox.dtos import AssetDTO, CampaignDTO, FloorDTO, HoldingDTO, ListingDTO, SaleDTO
 from fetchfox.helpers import formatters
 from . import utils
 
 logger = logging.getLogger(__name__)
 
 
 class Evm(Blockchain):
@@ -206,26 +206,32 @@
                 currency=price["currency"].replace("WETH", "ETH"),
                 listed_at=listed_at,
                 listed_by=parameters["offerer"],
                 tx_hash=listing["order_hash"],
                 marketplace_url=marketplace_url,
             )
 
-    def get_floor(self, collection_id: str, *args, **kwargs) -> Optional[ListingDTO]:
+    def get_floor(self, collection_id: str, *args, **kwargs) -> FloorDTO:
         self.check_collection_id(collection_id)
 
         floor = None
+        count = 0
 
         for listing in self.get_listings(collection_id):
+            count += 1
+
             if floor is None:
                 floor = listing
             elif listing.usd < floor.usd:
                 floor = listing
 
-        return floor
+        return FloorDTO(
+            listing=floor,
+            listing_count=count,
+        )
 
     def get_sales(self, collection_id: str, slug: str = None, *args, **kwargs) -> Iterable[SaleDTO]:
         self.check_collection_id(collection_id)
 
         sales = openseaio.get_sales(
             collection_id,
             api_key=self.openseaio_api_key,
```

### Comparing `bookio_fetchfox-0.5.0/fetchfox/blockchains/evm/utils.py` & `bookio_fetchfox-0.6.0/fetchfox/blockchains/evm/utils.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.5.0/fetchfox/blockchains/polygon/blockchain.py` & `bookio_fetchfox-0.6.0/fetchfox/blockchains/polygon/blockchain.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.5.0/fetchfox/dtos/asset.py` & `bookio_fetchfox-0.6.0/fetchfox/dtos/asset.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.5.0/fetchfox/dtos/campaign.py` & `bookio_fetchfox-0.6.0/fetchfox/dtos/campaign.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.5.0/fetchfox/dtos/listing.py` & `bookio_fetchfox-0.6.0/fetchfox/dtos/listing.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.5.0/fetchfox/dtos/sale.py` & `bookio_fetchfox-0.6.0/fetchfox/dtos/sale.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.5.0/fetchfox/rest.py` & `bookio_fetchfox-0.6.0/fetchfox/rest.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.5.0/pyproject.toml` & `bookio_fetchfox-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bookio-fetchfox"
-version = "0.5.0"
+version = "0.6.0"
 description = "Collection of API services to fetch information from several blockchains."
 documentation = "https://github.com/book-io/fetchfox/blob/main/README.md"
 homepage = "https://github.com/book-io/fetchfox"
 license = "MIT"
 readme = "README.md"
 
 authors = [
```

### Comparing `bookio_fetchfox-0.5.0/setup.py` & `bookio_fetchfox-0.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
  'asyncio>=3.4.3,<4.0.0',
  'backoff>=2.2.1,<3.0.0',
  'cachetools>=5.3.1,<6.0.0',
  'pytz>=2023.3,<2024.0']
 
 setup_kwargs = {
     'name': 'bookio-fetchfox',
-    'version': '0.5.0',
+    'version': '0.6.0',
     'description': 'Collection of API services to fetch information from several blockchains.',
     'long_description': '# book.io / fetchfox\n\n> Collection of API services to fetch information from several blockchains.\n\n![](https://s2.coinmarketcap.com/static/img/coins/64x64/4030.png)\n![](https://s2.coinmarketcap.com/static/img/coins/64x64/2010.png)\n![](https://s2.coinmarketcap.com/static/img/coins/64x64/1027.png)\n![](https://s2.coinmarketcap.com/static/img/coins/64x64/3890.png)\n\n\n## Supported Blockchains\n\n### Algorand\n\n```python\nimport os\nfrom fetchfox.blockchains import Algorand\n\nalgorand = Algorand(\n    nftexplorerapp_api_key=os.getenv("NFTEXPLORER_API_KEY"),\n)\n\n# Brave New World\ncreator_address = "6WII6ES4H6UW7G7T7RJX63CUNPKJEPEGQ3PTYVVU3JHJ652W34GCJV5OVY"\n\nfor asset in algorand.get_assets(creator_address):\n    print(asset)\n```\n\n#### Services\n\n* get_asset ([algonode.cloud](https://algonode.cloud))\n* get_assets ([algonode.cloud](https://algonode.cloud))\n* get_holdings ([algonode.cloud](https://algonode.cloud))\n* get_snapshot ([algonode.cloud](https://algonode.cloud))\n* get_campaigns ([book.io](https://book.io))\n* get_listings ([randgallery.com](https://randgallery.com) / [algoxnft.com](https://algoxnft.com))\n* get_floor ([randgallery.com](https://randgallery.com) / [algoxnft.com](https://algoxnft.com))\n* get_sales ([nftexplorer.app¹](https://nftexplorer.app))\n\n\n### Cardano\n\n```python\nimport os\nfrom fetchfox.blockchains import Cardano\n\ncardano = Cardano(\n    blockfrostio_project_id=os.getenv("BLOCKFROST_PROJECT_ID"),\n)\n\n# Gutenberg Bible\npolicy_id = "477cec772adb1466b301fb8161f505aa66ed1ee8d69d3e7984256a43"\n\nfor asset in cardano.get_assets(policy_id):\n    print(asset)\n```\n\n#### Services\n\n* get_asset ([blockfrost.io²](https://blockfrost.io))\n* get_assets ([blockfrost.io²](https://blockfrost.io))\n* get_holdings ([blockfrost.io²](https://blockfrost.io))\n* get_campaigns ([book.io](https://book.io))\n* get_snapshot ([blockfrost.io²](https://blockfrost.io))\n* get_listings ([jpg.store](https://jpg.store))\n* get_floor ([jpg.store](https://jpg.store))\n* get_sales ([jpg.store](https://jpg.store))\n* get_ranks ([cnft.tools](https://cnft.tools))\n\n\n### EVM (Ethereum and Polygon)\n\n```python\nimport os\nfrom fetchfox.blockchains import Ethereum, Polygon\n\nethereum = Ethereum(\n    geckodriver_path=os.getenv("GECKODRIVER_PATH"),\n    moralisio_api_key=os.getenv("MORALIS_API_KEY"),\n    openseaio_api_key=os.getenv("OPENSEA_API_KEY"),\n)\n\npolygon = Polygon(\n    geckodriver_path=os.getenv("GECKODRIVER_PATH"),\n    moralisio_api_key=os.getenv("MORALIS_API_KEY"),\n    openseaio_api_key=os.getenv("OPENSEA_API_KEY"),\n)\n\n\n# Alice in Wonderland\ncontract_address = "0x919da7fef646226f88f70305201de392ff365059"\n\nfor asset in ethereum.get_assets(contract_address):\n    print(asset)\n\n# Art of War\ncontract_address = "0xb56010e0500e4f163758881603b8083996ae47ec"\n\nfor asset in polygon.get_assets(contract_address):\n    print(asset)\n```\n\n#### Services\n\n* get_asset ([moralis.io³](https://moralis.io))\n* get_assets ([moralis.io³](https://moralis.io))\n* get_holdings ([moralis.io³](https://moralis.io))\n* get_snapshot ([moralis.io³](https://moralis.io))\n* get_campaigns ([book.io](https://book.io))\n* get_listings ([opensea.io⁴](https://opensea.io))\n* get_floor ([opensea.io⁴](https://opensea.io))\n* get_sales ([opensea.io⁴](https://opensea.io))\n\n\n> ¹ **nftexplorer.app** services require an [api key](https://www.nftexplorer.app/nftx-api).\n> \n> ² **blockfrost.io** services require a [project id](https://blockfrost.dev/docs/overview/plans-and-billing).\n> \n> ³ **moralis.io** services require an [api key](https://moralis.io/pricing).\n> \n> ⁴ **opensea.io** some services also require an [api key](https://docs.opensea.io/reference/api-keys). \n\n---\n\n![fetch, the fox](https://i.imgur.com/fm6mqzS.png)\n> fetch, the fox\n\n',
     'author': 'Fede',
     'author_email': 'fede@book.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/book-io/fetchfox',
```

### Comparing `bookio_fetchfox-0.5.0/PKG-INFO` & `bookio_fetchfox-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bookio-fetchfox
-Version: 0.5.0
+Version: 0.6.0
 Summary: Collection of API services to fetch information from several blockchains.
 Home-page: https://github.com/book-io/fetchfox
 License: MIT
 Keywords: book.io,blockchain,crypto,algorand,cardano,ethereum,polygon
 Author: Fede
 Author-email: fede@book.io
 Requires-Python: >=3.8,<4.0
```

