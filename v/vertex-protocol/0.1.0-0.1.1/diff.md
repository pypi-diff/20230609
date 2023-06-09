# Comparing `tmp/vertex_protocol-0.1.0.tar.gz` & `tmp/vertex_protocol-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vertex_protocol-0.1.0.tar", max compression
+gzip compressed data, was "vertex_protocol-0.1.1.tar", max compression
```

## Comparing `vertex_protocol-0.1.0.tar` & `vertex_protocol-0.1.1.tar`

### file list

```diff
@@ -1,60 +1,62 @@
--rw-r--r--   0        0        0      982 2023-06-07 03:41:37.008998 vertex_protocol-0.1.0/README.md
--rw-r--r--   0        0        0     1306 2023-06-07 06:59:57.709295 vertex_protocol-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-07 07:36:40.080054 vertex_protocol-0.1.0/vertex_protocol/__init__.py
--rw-r--r--   0        0        0     6337 2023-06-07 07:16:46.777415 vertex_protocol-0.1.0/vertex_protocol/client/__init__.py
--rw-r--r--   0        0        0      580 2023-06-07 03:05:24.947488 vertex_protocol-0.1.0/vertex_protocol/client/apis/__init__.py
--rw-r--r--   0        0        0     1394 2023-06-07 03:30:14.791304 vertex_protocol-0.1.0/vertex_protocol/client/apis/base.py
--rw-r--r--   0        0        0     1108 2023-06-07 03:00:31.114291 vertex_protocol-0.1.0/vertex_protocol/client/apis/market/__init__.py
--rw-r--r--   0        0        0     3404 2023-06-07 02:55:40.588679 vertex_protocol-0.1.0/vertex_protocol/client/apis/market/execute.py
--rw-r--r--   0        0        0    10070 2023-06-07 07:35:12.721722 vertex_protocol-0.1.0/vertex_protocol/client/apis/market/query.py
--rw-r--r--   0        0        0      746 2023-06-07 03:38:00.660790 vertex_protocol-0.1.0/vertex_protocol/client/apis/perp/__init__.py
--rw-r--r--   0        0        0     1438 2023-06-07 03:38:00.661620 vertex_protocol-0.1.0/vertex_protocol/client/apis/perp/query.py
--rw-r--r--   0        0        0     1027 2023-06-07 03:26:52.736204 vertex_protocol-0.1.0/vertex_protocol/client/apis/spot/__init__.py
--rw-r--r--   0        0        0     1191 2023-06-07 07:39:02.706785 vertex_protocol-0.1.0/vertex_protocol/client/apis/spot/base.py
--rw-r--r--   0        0        0     4745 2023-06-07 07:39:02.706988 vertex_protocol-0.1.0/vertex_protocol/client/apis/spot/execute.py
--rw-r--r--   0        0        0     2933 2023-06-07 07:39:02.707191 vertex_protocol-0.1.0/vertex_protocol/client/apis/spot/query.py
--rw-r--r--   0        0        0     1307 2023-06-07 03:00:31.114726 vertex_protocol-0.1.0/vertex_protocol/client/apis/subaccount/__init__.py
--rw-r--r--   0        0        0     2023 2023-06-07 03:34:15.877255 vertex_protocol-0.1.0/vertex_protocol/client/apis/subaccount/execute.py
--rw-r--r--   0        0        0     3162 2023-06-07 07:35:12.724061 vertex_protocol-0.1.0/vertex_protocol/client/apis/subaccount/query.py
--rw-r--r--   0        0        0     2551 2023-06-07 07:35:12.736012 vertex_protocol-0.1.0/vertex_protocol/client/context.py
--rw-r--r--   0        0        0     8404 2023-06-07 07:45:33.309830 vertex_protocol-0.1.0/vertex_protocol/contracts/__init__.py
--rw-r--r--   0        0        0    11702 2023-06-06 05:19:10.949304 vertex_protocol-0.1.0/vertex_protocol/contracts/abis/Endpoint.json
--rw-r--r--   0        0        0    55374 2023-06-06 05:19:10.949492 vertex_protocol-0.1.0/vertex_protocol/contracts/abis/FQuerier.json
--rw-r--r--   0        0        0    16980 2023-06-06 05:28:55.009718 vertex_protocol-0.1.0/vertex_protocol/contracts/abis/IClearinghouse.json
--rw-r--r--   0        0        0     3385 2023-06-06 05:19:10.949672 vertex_protocol-0.1.0/vertex_protocol/contracts/abis/IERC20.json
--rw-r--r--   0        0        0     4723 2023-06-06 05:19:10.949743 vertex_protocol-0.1.0/vertex_protocol/contracts/abis/IEndpoint.json
--rw-r--r--   0        0        0    13112 2023-06-06 05:19:10.949822 vertex_protocol-0.1.0/vertex_protocol/contracts/abis/IOffchainBook.json
--rw-r--r--   0        0        0    21812 2023-06-06 05:19:10.949937 vertex_protocol-0.1.0/vertex_protocol/contracts/abis/IPerpEngine.json
--rw-r--r--   0        0        0     8410 2023-06-06 05:19:10.950037 vertex_protocol-0.1.0/vertex_protocol/contracts/abis/IProductEngine.json
--rw-r--r--   0        0        0    18858 2023-06-06 05:19:10.950211 vertex_protocol-0.1.0/vertex_protocol/contracts/abis/ISpotEngine.json
--rw-r--r--   0        0        0     5698 2023-06-06 05:19:10.950331 vertex_protocol-0.1.0/vertex_protocol/contracts/abis/MockERC20.json
--rw-r--r--   0        0        0     1022 2023-06-05 21:40:33.793972 vertex_protocol-0.1.0/vertex_protocol/contracts/deployments/deployment.arbitrumGoerli.json
--rw-r--r--   0        0        0      993 2023-06-05 21:40:33.794121 vertex_protocol-0.1.0/vertex_protocol/contracts/deployments/deployment.arbitrumOne.json
--rw-r--r--   0        0        0     1414 2023-06-07 07:45:08.000152 vertex_protocol-0.1.0/vertex_protocol/contracts/eip712/__init__.py
--rw-r--r--   0        0        0     1183 2023-06-07 07:35:12.726691 vertex_protocol-0.1.0/vertex_protocol/contracts/eip712/domain.py
--rw-r--r--   0        0        0     2511 2023-06-07 07:35:12.729074 vertex_protocol-0.1.0/vertex_protocol/contracts/eip712/sign.py
--rw-r--r--   0        0        0     3222 2023-06-07 05:29:59.758025 vertex_protocol-0.1.0/vertex_protocol/contracts/eip712/types.py
--rw-r--r--   0        0        0     1526 2023-06-07 05:53:08.430048 vertex_protocol-0.1.0/vertex_protocol/contracts/loader.py
--rw-r--r--   0        0        0     2704 2023-06-07 07:44:51.477194 vertex_protocol-0.1.0/vertex_protocol/contracts/types.py
--rw-r--r--   0        0        0     1127 2023-06-07 07:09:15.934941 vertex_protocol-0.1.0/vertex_protocol/engine_client/__init__.py
--rw-r--r--   0        0        0    18307 2023-06-07 07:35:12.781157 vertex_protocol-0.1.0/vertex_protocol/engine_client/execute.py
--rw-r--r--   0        0        0    11054 2023-06-07 07:35:12.753146 vertex_protocol-0.1.0/vertex_protocol/engine_client/query.py
--rw-r--r--   0        0        0     3375 2023-06-07 04:23:03.194653 vertex_protocol-0.1.0/vertex_protocol/engine_client/types/__init__.py
--rw-r--r--   0        0        0    18324 2023-06-07 07:35:12.777389 vertex_protocol-0.1.0/vertex_protocol/engine_client/types/execute.py
--rw-r--r--   0        0        0     3404 2023-06-07 04:38:14.745486 vertex_protocol-0.1.0/vertex_protocol/engine_client/types/models.py
--rw-r--r--   0        0        0     9451 2023-06-06 20:20:54.979555 vertex_protocol-0.1.0/vertex_protocol/engine_client/types/query.py
--rw-r--r--   0        0        0      926 2023-06-07 07:09:15.934044 vertex_protocol-0.1.0/vertex_protocol/indexer_client/__init__.py
--rw-r--r--   0        0        0    10902 2023-06-07 07:35:12.758081 vertex_protocol-0.1.0/vertex_protocol/indexer_client/query.py
--rw-r--r--   0        0        0      273 2023-06-07 05:21:49.543086 vertex_protocol-0.1.0/vertex_protocol/indexer_client/types/__init__.py
--rw-r--r--   0        0        0     5549 2023-06-05 21:40:33.800033 vertex_protocol-0.1.0/vertex_protocol/indexer_client/types/models.py
--rw-r--r--   0        0        0    12057 2023-06-07 05:27:22.784326 vertex_protocol-0.1.0/vertex_protocol/indexer_client/types/query.py
--rw-r--r--   0        0        0      933 2023-06-07 08:05:57.996160 vertex_protocol-0.1.0/vertex_protocol/utils/__init__.py
--rw-r--r--   0        0        0      319 2023-06-06 21:07:37.350807 vertex_protocol-0.1.0/vertex_protocol/utils/backend.py
--rw-r--r--   0        0        0     5216 2023-06-07 07:52:47.374227 vertex_protocol-0.1.0/vertex_protocol/utils/bytes32.py
--rw-r--r--   0        0        0     1136 2023-06-07 07:39:02.708054 vertex_protocol-0.1.0/vertex_protocol/utils/exceptions.py
--rw-r--r--   0        0        0     1094 2023-06-07 07:35:12.737300 vertex_protocol-0.1.0/vertex_protocol/utils/expiration.py
--rw-r--r--   0        0        0      927 2023-06-07 07:35:12.736520 vertex_protocol-0.1.0/vertex_protocol/utils/math.py
--rw-r--r--   0        0        0     1887 2023-06-07 07:55:07.208882 vertex_protocol-0.1.0/vertex_protocol/utils/model.py
--rw-r--r--   0        0        0      809 2023-06-07 07:35:12.739559 vertex_protocol-0.1.0/vertex_protocol/utils/nonce.py
--rw-r--r--   0        0        0      491 2023-06-07 07:53:37.553869 vertex_protocol-0.1.0/vertex_protocol/utils/subaccount.py
--rw-r--r--   0        0        0     1479 1970-01-01 00:00:00.000000 vertex_protocol-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      982 2023-06-09 06:52:38.447127 vertex_protocol-0.1.1/README.md
+-rw-r--r--   0        0        0     1445 2023-06-09 06:52:38.447127 vertex_protocol-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-09 06:52:38.447127 vertex_protocol-0.1.1/vertex_protocol/__init__.py
+-rw-r--r--   0        0        0     6628 2023-06-09 06:52:38.447127 vertex_protocol-0.1.1/vertex_protocol/client/__init__.py
+-rw-r--r--   0        0        0      580 2023-06-09 06:52:38.447127 vertex_protocol-0.1.1/vertex_protocol/client/apis/__init__.py
+-rw-r--r--   0        0        0     1394 2023-06-09 06:52:38.447127 vertex_protocol-0.1.1/vertex_protocol/client/apis/base.py
+-rw-r--r--   0        0        0     1108 2023-06-09 06:52:38.447127 vertex_protocol-0.1.1/vertex_protocol/client/apis/market/__init__.py
+-rw-r--r--   0        0        0     3404 2023-06-09 06:52:38.447127 vertex_protocol-0.1.1/vertex_protocol/client/apis/market/execute.py
+-rw-r--r--   0        0        0    10070 2023-06-09 06:52:38.447127 vertex_protocol-0.1.1/vertex_protocol/client/apis/market/query.py
+-rw-r--r--   0        0        0      746 2023-06-09 06:52:38.447127 vertex_protocol-0.1.1/vertex_protocol/client/apis/perp/__init__.py
+-rw-r--r--   0        0        0     1438 2023-06-09 06:52:38.447127 vertex_protocol-0.1.1/vertex_protocol/client/apis/perp/query.py
+-rw-r--r--   0        0        0     1027 2023-06-09 06:52:38.447127 vertex_protocol-0.1.1/vertex_protocol/client/apis/spot/__init__.py
+-rw-r--r--   0        0        0     1191 2023-06-09 06:52:38.447127 vertex_protocol-0.1.1/vertex_protocol/client/apis/spot/base.py
+-rw-r--r--   0        0        0     4745 2023-06-09 06:52:38.447127 vertex_protocol-0.1.1/vertex_protocol/client/apis/spot/execute.py
+-rw-r--r--   0        0        0     2933 2023-06-09 06:52:38.447127 vertex_protocol-0.1.1/vertex_protocol/client/apis/spot/query.py
+-rw-r--r--   0        0        0     1307 2023-06-09 06:52:38.447127 vertex_protocol-0.1.1/vertex_protocol/client/apis/subaccount/__init__.py
+-rw-r--r--   0        0        0     2023 2023-06-09 06:52:38.447127 vertex_protocol-0.1.1/vertex_protocol/client/apis/subaccount/execute.py
+-rw-r--r--   0        0        0     3162 2023-06-09 06:52:38.447127 vertex_protocol-0.1.1/vertex_protocol/client/apis/subaccount/query.py
+-rw-r--r--   0        0        0     2551 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/client/context.py
+-rw-r--r--   0        0        0     8404 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/contracts/__init__.py
+-rw-r--r--   0        0        0    11702 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/contracts/abis/Endpoint.json
+-rw-r--r--   0        0        0    55374 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/contracts/abis/FQuerier.json
+-rw-r--r--   0        0        0    16980 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/contracts/abis/IClearinghouse.json
+-rw-r--r--   0        0        0     3385 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/contracts/abis/IERC20.json
+-rw-r--r--   0        0        0     4723 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/contracts/abis/IEndpoint.json
+-rw-r--r--   0        0        0    13112 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/contracts/abis/IOffchainBook.json
+-rw-r--r--   0        0        0    21812 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/contracts/abis/IPerpEngine.json
+-rw-r--r--   0        0        0     8410 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/contracts/abis/IProductEngine.json
+-rw-r--r--   0        0        0    18858 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/contracts/abis/ISpotEngine.json
+-rw-r--r--   0        0        0     5698 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/contracts/abis/MockERC20.json
+-rw-r--r--   0        0        0     1022 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/contracts/deployments/deployment.arbitrumGoerli.json
+-rw-r--r--   0        0        0      993 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/contracts/deployments/deployment.arbitrumOne.json
+-rw-r--r--   0        0        0      908 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/contracts/deployments/deployment.test.json
+-rw-r--r--   0        0        0     1414 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/contracts/eip712/__init__.py
+-rw-r--r--   0        0        0     1183 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/contracts/eip712/domain.py
+-rw-r--r--   0        0        0     2511 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/contracts/eip712/sign.py
+-rw-r--r--   0        0        0     3222 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/contracts/eip712/types.py
+-rw-r--r--   0        0        0     1526 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/contracts/loader.py
+-rw-r--r--   0        0        0     2747 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/contracts/types.py
+-rw-r--r--   0        0        0     1127 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/engine_client/__init__.py
+-rw-r--r--   0        0        0    18437 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/engine_client/execute.py
+-rw-r--r--   0        0        0    11077 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/engine_client/query.py
+-rw-r--r--   0        0        0     3413 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/engine_client/types/__init__.py
+-rw-r--r--   0        0        0    18340 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/engine_client/types/execute.py
+-rw-r--r--   0        0        0     3426 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/engine_client/types/models.py
+-rw-r--r--   0        0        0     9473 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/engine_client/types/query.py
+-rw-r--r--   0        0        0      926 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/indexer_client/__init__.py
+-rw-r--r--   0        0        0    11025 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/indexer_client/query.py
+-rw-r--r--   0        0        0      273 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/indexer_client/types/__init__.py
+-rw-r--r--   0        0        0     5588 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/indexer_client/types/models.py
+-rw-r--r--   0        0        0    12079 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/indexer_client/types/query.py
+-rw-r--r--   0        0        0      933 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/utils/__init__.py
+-rw-r--r--   0        0        0      341 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/utils/backend.py
+-rw-r--r--   0        0        0     5216 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/utils/bytes32.py
+-rw-r--r--   0        0        0       99 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/utils/enum.py
+-rw-r--r--   0        0        0     1136 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/utils/exceptions.py
+-rw-r--r--   0        0        0     1094 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/utils/expiration.py
+-rw-r--r--   0        0        0      927 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/utils/math.py
+-rw-r--r--   0        0        0     1887 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/utils/model.py
+-rw-r--r--   0        0        0      809 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/utils/nonce.py
+-rw-r--r--   0        0        0      491 2023-06-09 06:52:38.451127 vertex_protocol-0.1.1/vertex_protocol/utils/subaccount.py
+-rw-r--r--   0        0        0     1530 1970-01-01 00:00:00.000000 vertex_protocol-0.1.1/PKG-INFO
```

### Comparing `vertex_protocol-0.1.0/README.md` & `vertex_protocol-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.0/pyproject.toml` & `vertex_protocol-0.1.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "vertex-protocol"
-version = "0.1.0"
+version = "0.1.1"
 description = "Vertex Protocol SDK"
 authors = ["Jeury Mejia <jeury@vertexprotocol.com>"]
 readme = "README.md"
 packages = [{include = "vertex_protocol"}]
 include = ["vertex_protocol/*.json"]
 keywords = ["vertex protocol", "vertex sdk", "vertex protocol api"]
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = "^3.10"
 pydantic = "^1.10.7"
 web3 = "^6.4.0"
 eth-account = "^0.8.0"
 
 [tool.poetry.group.dev.dependencies]
 ruff = "*"
 black = "*"
@@ -22,25 +22,32 @@
 python-dotenv = "^1.0.0"
 sphinx = "^6.2.1"
 sphinx-rtd-theme = "^1.2.1"
 sphinx-autodoc-typehints = "^1.12.0"
 pycycle = "^0.0.8"
 mypy = "^1.3.0"
 types-requests = "^2.31.0.1"
+coverage = "^7.2.7"
 
 [tool.poetry.scripts]
 test = "pytest:main"
 engine-sanity = "sanity.engine_client:run"
 indexer-sanity = "sanity.indexer_client:run"
 contracts-sanity = "sanity.contracts:run"
 client-sanity = "sanity.vertex_client:run"
 
 [[tool.poetry.source]]
 name = "private"
 url = "https://github.com/vertex-protocol/vertex-python-sdk"
+priority = "primary"
+
+
+[[tool.poetry.source]]
+name = "PyPI"
+priority = "primary"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 88
@@ -54,9 +61,12 @@
   | \.tox
   | \.venv
   | _build
   | buck-out
   | build
   | dist
   | venv
+  | venv3.9
+  | venv3.10
+  | venv3.11
 )/
 '''
```

### Comparing `vertex_protocol-0.1.0/vertex_protocol/client/__init__.py` & `vertex_protocol-0.1.1/vertex_protocol/client/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from enum import StrEnum
 import logging
 from vertex_protocol.client.apis.market import MarketAPI
 from vertex_protocol.client.apis.perp import PerpAPI
 from vertex_protocol.client.apis.spot import SpotAPI
 from vertex_protocol.client.apis.subaccount import SubaccountAPI
 from vertex_protocol.client.context import (
     VertexClientContext,
@@ -10,15 +9,15 @@
     create_vertex_client_context,
 )
 from vertex_protocol.contracts import VertexContractsContext
 from vertex_protocol.contracts.loader import load_deployment
 from vertex_protocol.contracts.types import VertexNetwork
 from vertex_protocol.engine_client.types import Signer
 from vertex_protocol.utils.backend import VertexBackendURL
-
+from vertex_protocol.utils.enum import StrEnum
 from vertex_protocol.client.context import *
 
 from pydantic import parse_obj_as
 
 
 class VertexClientMode(StrEnum):
     """
@@ -26,19 +25,22 @@
 
     Attributes:
         MAINNET: For operating in Vertex's mainnet environment.
 
         TESTNET: For operating in Vertex's testnet environment.
 
         DEVNET: For local development.
+
+        TESTING: For running tests.
     """
 
     MAINNET = "mainnet"
     TESTNET = "testnet"
     DEVNET = "devnet"
+    TESTING = "testing"
 
 
 class VertexClient:
     """
     The primary client interface for interacting with Vertex Protocol.
 
     This client consolidates the functionality of various aspects of Vertex such as spot, market,
@@ -152,14 +154,19 @@
                 VertexNetwork.ARBITRUM_GOERLI.value,
             ),
             VertexClientMode.DEVNET: (
                 VertexBackendURL.DEVNET_ENGINE.value,
                 VertexBackendURL.DEVNET_INDEXER.value,
                 VertexNetwork.HARDHAT.value,
             ),
+            VertexClientMode.TESTING: (
+                VertexBackendURL.DEVNET_ENGINE.value,
+                VertexBackendURL.DEVNET_INDEXER.value,
+                VertexNetwork.TESTING.value,
+            ),
         }[client_mode]
     except KeyError:
         raise Exception(f"Mode provided `{client_mode}` not supported!")
 
 
 __all__ = [
     "VertexClient",
```

### Comparing `vertex_protocol-0.1.0/vertex_protocol/client/apis/__init__.py` & `vertex_protocol-0.1.1/vertex_protocol/client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.0/vertex_protocol/client/apis/base.py` & `vertex_protocol-0.1.1/vertex_protocol/client/apis/base.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.0/vertex_protocol/client/apis/market/__init__.py` & `vertex_protocol-0.1.1/vertex_protocol/client/apis/market/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.0/vertex_protocol/client/apis/market/execute.py` & `vertex_protocol-0.1.1/vertex_protocol/client/apis/market/execute.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.0/vertex_protocol/client/apis/market/query.py` & `vertex_protocol-0.1.1/vertex_protocol/client/apis/market/query.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.0/vertex_protocol/client/apis/perp/__init__.py` & `vertex_protocol-0.1.1/vertex_protocol/client/apis/perp/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.0/vertex_protocol/client/apis/perp/query.py` & `vertex_protocol-0.1.1/vertex_protocol/client/apis/perp/query.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.0/vertex_protocol/client/apis/spot/__init__.py` & `vertex_protocol-0.1.1/vertex_protocol/client/apis/spot/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.0/vertex_protocol/client/apis/spot/base.py` & `vertex_protocol-0.1.1/vertex_protocol/client/apis/spot/base.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.0/vertex_protocol/client/apis/spot/execute.py` & `vertex_protocol-0.1.1/vertex_protocol/client/apis/spot/execute.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.0/vertex_protocol/client/apis/spot/query.py` & `vertex_protocol-0.1.1/vertex_protocol/client/apis/spot/query.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.0/vertex_protocol/client/apis/subaccount/__init__.py` & `vertex_protocol-0.1.1/vertex_protocol/client/apis/subaccount/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.0/vertex_protocol/client/apis/subaccount/execute.py` & `vertex_protocol-0.1.1/vertex_protocol/client/apis/subaccount/execute.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.0/vertex_protocol/client/apis/subaccount/query.py` & `vertex_protocol-0.1.1/vertex_protocol/client/apis/subaccount/query.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.0/vertex_protocol/client/context.py` & `vertex_protocol-0.1.1/vertex_protocol/client/context.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.0/vertex_protocol/contracts/__init__.py` & `vertex_protocol-0.1.1/vertex_protocol/contracts/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.0/vertex_protocol/contracts/abis/Endpoint.json` & `vertex_protocol-0.1.1/vertex_protocol/contracts/abis/Endpoint.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.0/vertex_protocol/contracts/abis/FQuerier.json` & `vertex_protocol-0.1.1/vertex_protocol/contracts/abis/FQuerier.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.0/vertex_protocol/contracts/abis/IClearinghouse.json` & `vertex_protocol-0.1.1/vertex_protocol/contracts/abis/IClearinghouse.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.0/vertex_protocol/contracts/abis/IERC20.json` & `vertex_protocol-0.1.1/vertex_protocol/contracts/abis/IERC20.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.0/vertex_protocol/contracts/abis/IEndpoint.json` & `vertex_protocol-0.1.1/vertex_protocol/contracts/abis/IEndpoint.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.0/vertex_protocol/contracts/abis/IOffchainBook.json` & `vertex_protocol-0.1.1/vertex_protocol/contracts/abis/IOffchainBook.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.0/vertex_protocol/contracts/abis/IPerpEngine.json` & `vertex_protocol-0.1.1/vertex_protocol/contracts/abis/IPerpEngine.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.0/vertex_protocol/contracts/abis/IProductEngine.json` & `vertex_protocol-0.1.1/vertex_protocol/contracts/abis/IProductEngine.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.0/vertex_protocol/contracts/abis/ISpotEngine.json` & `vertex_protocol-0.1.1/vertex_protocol/contracts/abis/ISpotEngine.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.0/vertex_protocol/contracts/abis/MockERC20.json` & `vertex_protocol-0.1.1/vertex_protocol/contracts/abis/MockERC20.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.0/vertex_protocol/contracts/deployments/deployment.arbitrumGoerli.json` & `vertex_protocol-0.1.1/vertex_protocol/contracts/deployments/deployment.arbitrumGoerli.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.0/vertex_protocol/contracts/deployments/deployment.arbitrumOne.json` & `vertex_protocol-0.1.1/vertex_protocol/contracts/deployments/deployment.arbitrumOne.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.0/vertex_protocol/contracts/eip712/__init__.py` & `vertex_protocol-0.1.1/vertex_protocol/contracts/eip712/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.0/vertex_protocol/contracts/eip712/domain.py` & `vertex_protocol-0.1.1/vertex_protocol/contracts/eip712/domain.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.0/vertex_protocol/contracts/eip712/sign.py` & `vertex_protocol-0.1.1/vertex_protocol/contracts/eip712/sign.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.0/vertex_protocol/contracts/eip712/types.py` & `vertex_protocol-0.1.1/vertex_protocol/contracts/eip712/types.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.0/vertex_protocol/contracts/loader.py` & `vertex_protocol-0.1.1/vertex_protocol/contracts/loader.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.0/vertex_protocol/contracts/types.py` & `vertex_protocol-0.1.1/vertex_protocol/contracts/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from pydantic import AnyUrl, Field
-from enum import StrEnum
+from vertex_protocol.utils.enum import StrEnum
 
 from vertex_protocol.utils.model import VertexBaseModel
 
 
 class VertexNetwork(StrEnum):
     """
     Enumeration representing various network environments for the Vertex protocol.
     """
 
     ARBITRUM_ONE = "arbitrumOne"
     ARBITRUM_GOERLI = "arbitrumGoerli"
     HARDHAT = "localhost"
+    TESTING = "test"
 
 
 class VertexAbiName(StrEnum):
     """
     Enumeration representing various contract names for which the ABI can be loaded in the Vertex protocol.
     """
```

### Comparing `vertex_protocol-0.1.0/vertex_protocol/engine_client/__init__.py` & `vertex_protocol-0.1.1/vertex_protocol/engine_client/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.0/vertex_protocol/engine_client/execute.py` & `vertex_protocol-0.1.1/vertex_protocol/engine_client/execute.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,16 +53,16 @@
 
         Args:
             opts (EngineClientOpts): Options for the client.
 
             querier (EngineQueryClient, optional): An EngineQueryClient instance. If not provided, a new one is created.
         """
         self._querier = querier or EngineQueryClient(opts)
-        self._opts = EngineClientOpts.parse_obj(opts)
-        self.url = self._opts.url
+        self._opts: EngineClientOpts = EngineClientOpts.parse_obj(opts)
+        self.url: str = self._opts.url
 
     def _inject_owner_if_needed(self, params: Type[BaseParams]) -> Type[BaseParams]:
         """
         Inject the owner if needed.
 
         Args:
             params (Type[BaseParams]): The parameters.
@@ -125,33 +125,36 @@
         """
         params = deepcopy(params)
         params = self._inject_owner_if_needed(params)
         params = self._inject_nonce_if_needed(params)
         return params
 
     @singledispatchmethod
-    def execute(self, params: ExecuteParams) -> ExecuteResponse:
+    def execute(self, params: ExecuteParams | ExecuteRequest) -> ExecuteResponse:
         """
         Executes the operation defined by the provided parameters.
 
         Args:
             params (ExecuteParams): The parameters for the operation to execute. This can represent a variety of operations, such as placing orders, cancelling orders, and more.
 
         Returns:
             ExecuteResponse: The response from the executed operation.
         """
-        return self._execute(to_execute_request(params))
+        req: ExecuteRequest = (
+            params if isinstance(params, ExecuteRequest) else to_execute_request(params)  # type: ignore
+        )
+        return self._execute(req)
 
     @execute.register
-    def _(self, req: dict | ExecuteRequest) -> ExecuteResponse:
+    def _(self, req: dict) -> ExecuteResponse:
         """
         Overloaded method to execute the operation defined by the provided request.
 
         Args:
-            req (dict | ExecuteRequest): The request data for the operation to execute. Can be a dictionary or an instance of ExecuteRequest.
+            req (dict): The request data for the operation to execute. Can be a dictionary or an instance of ExecuteRequest.
 
         Returns:
             ExecuteResponse: The response from the executed operation.
         """
         parsed_req: ExecuteRequest = VertexBaseModel.parse_obj(req)  # type: ignore
         return self._execute(parsed_req)
```

### Comparing `vertex_protocol-0.1.0/vertex_protocol/engine_client/query.py` & `vertex_protocol-0.1.1/vertex_protocol/engine_client/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,16 +52,16 @@
     def __init__(self, opts: EngineClientOpts):
         """
         Initialize EngineQueryClient with provided options.
 
         Args:
             opts (EngineClientOpts): Options for the client.
         """
-        self._opts = EngineClientOpts.parse_obj(opts)
-        self.url = self._opts.url
+        self._opts: EngineClientOpts = EngineClientOpts.parse_obj(opts)
+        self.url: str = self._opts.url
 
     def query(self, req: QueryRequest) -> QueryResponse:
         """
         Send a query to the engine.
 
         Args:
             req (QueryRequest): The query request parameters.
```

### Comparing `vertex_protocol-0.1.0/vertex_protocol/engine_client/types/__init__.py` & `vertex_protocol-0.1.1/vertex_protocol/engine_client/types/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from eth_account import Account
 from eth_account.signers.local import LocalAccount
-from typing import Optional
+from typing import Optional, Union
 from pydantic import BaseModel, AnyUrl, validator, root_validator
 
 PrivateKey = str
-Signer = LocalAccount | PrivateKey
+Signer = Union[LocalAccount, PrivateKey]
 
 
 class EngineClientOpts(BaseModel):
     """
     Model defining the configuration options for the Engine Client. It includes various parameters such as the URL,
     the signer, the linked signer, the chain ID, and others.
 
@@ -22,15 +22,15 @@
 
     Notes:
         - The class also includes several methods for validating and sanitizing the input values.
         - "linked_signer" cannot be set if "signer" is not set.
     """
 
     url: AnyUrl
-    signer: Optional[Signer] = None
+    signer: Optional[Union[LocalAccount, PrivateKey]] = None
     linked_signer: Optional[Signer] = None
     chain_id: Optional[int] = None
     endpoint_addr: Optional[str] = None
     book_addrs: Optional[list[str]] = None
 
     class Config:
         arbitrary_types_allowed = True
```

### Comparing `vertex_protocol-0.1.0/vertex_protocol/engine_client/types/execute.py` & `vertex_protocol-0.1.1/vertex_protocol/engine_client/types/execute.py`

 * *Files 0% similar despite different names*

```diff
@@ -564,8 +564,8 @@
         ),
         MintLpParams: (MintLpRequest, VertexExecuteType.MINT_LP.value),
         BurnLpParams: (BurnLpRequest, VertexExecuteType.BURN_LP.value),
         LinkSignerParams: (LinkSignerRequest, VertexExecuteType.LINK_SIGNER.value),
     }
 
     RequestClass, field_name = execute_request_mapping[type(params)]
-    return RequestClass(**{field_name: params})
+    return RequestClass(**{field_name: params})  # type: ignore
```

### Comparing `vertex_protocol-0.1.0/vertex_protocol/engine_client/types/models.py` & `vertex_protocol-0.1.1/vertex_protocol/engine_client/types/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import Annotated
-from enum import StrEnum
+from vertex_protocol.utils.enum import StrEnum
 from vertex_protocol.utils.model import VertexBaseModel
 from pydantic import conlist
 
 
 class ResponseStatus(StrEnum):
     SUCCESS = "success"
     FAILURE = "failure"
```

### Comparing `vertex_protocol-0.1.0/vertex_protocol/engine_client/types/query.py` & `vertex_protocol-0.1.1/vertex_protocol/engine_client/types/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from enum import StrEnum
+from vertex_protocol.utils.enum import StrEnum
 from typing import Optional
 from pydantic import validator
 from vertex_protocol.utils.model import VertexBaseModel
 from vertex_protocol.engine_client.types.models import (
     ApplyDeltaTx,
     BurnLpTx,
     EngineStatus,
```

### Comparing `vertex_protocol-0.1.0/vertex_protocol/indexer_client/__init__.py` & `vertex_protocol-0.1.1/vertex_protocol/indexer_client/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.0/vertex_protocol/indexer_client/query.py` & `vertex_protocol-0.1.1/vertex_protocol/indexer_client/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import requests
-
 from functools import singledispatchmethod
 from vertex_protocol.indexer_client.types import IndexerClientOpts
 from vertex_protocol.indexer_client.types.query import (
     IndexerCandlesticksParams,
     IndexerCandlesticksData,
     IndexerEventsParams,
     IndexerEventsData,
@@ -54,32 +53,35 @@
         Args:
             opts (IndexerClientOpts): Client configuration options for connecting and interacting with the indexer service.
         """
         self._opts = IndexerClientOpts.parse_obj(opts)
         self.url = self._opts.url
 
     @singledispatchmethod
-    def query(self, params: IndexerParams) -> IndexerResponse:
+    def query(self, params: IndexerParams | IndexerRequest) -> IndexerResponse:
         """
         Sends a query request to the indexer service and returns the response.
 
         The `query` method is overloaded to accept either `IndexerParams` or a dictionary or `IndexerRequest`
         as the input parameters. Based on the type of the input, the appropriate internal method is invoked
         to process the query request.
 
         Args:
             params (IndexerParams | dict | IndexerRequest): The parameters for the query request.
 
         Returns:
             IndexerResponse: The response from the indexer service.
         """
-        return self._query(to_indexer_request(params))
+        req: IndexerRequest = (
+            params if isinstance(params, IndexerRequest) else to_indexer_request(params)  # type: ignore
+        )
+        return self._query(req)
 
     @query.register
-    def _(self, req: dict | IndexerRequest) -> IndexerResponse:
+    def _(self, req: dict) -> IndexerResponse:
         return self._query(VertexBaseModel.parse_obj(req))  # type: ignore
 
     def _query(self, req: IndexerRequest) -> IndexerResponse:
         res = requests.post(f"{self.url}/indexer", json=req.dict())
         if res.status_code != 200:
             raise Exception(res.text)
         return IndexerResponse(data=res.json())
```

### Comparing `vertex_protocol-0.1.0/vertex_protocol/indexer_client/types/models.py` & `vertex_protocol-0.1.1/vertex_protocol/indexer_client/types/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from enum import IntEnum, StrEnum
+from enum import IntEnum
+from vertex_protocol.utils.enum import StrEnum
+
 from typing import Any, Optional
 from vertex_protocol.engine_client.types.models import (
     PerpProduct,
     PerpProductBalance,
     SpotProduct,
     SpotProductBalance,
 )
```

### Comparing `vertex_protocol-0.1.0/vertex_protocol/indexer_client/types/query.py` & `vertex_protocol-0.1.1/vertex_protocol/indexer_client/types/query.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from enum import StrEnum
+from vertex_protocol.utils.enum import StrEnum
 from typing import Optional
 
 from pydantic import Field
 from vertex_protocol.indexer_client.types.models import (
     IndexerCandlestick,
     IndexerCandlesticksGranularity,
     IndexerEvent,
```

### Comparing `vertex_protocol-0.1.0/vertex_protocol/utils/__init__.py` & `vertex_protocol-0.1.1/vertex_protocol/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.0/vertex_protocol/utils/bytes32.py` & `vertex_protocol-0.1.1/vertex_protocol/utils/bytes32.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.0/vertex_protocol/utils/exceptions.py` & `vertex_protocol-0.1.1/vertex_protocol/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.0/vertex_protocol/utils/expiration.py` & `vertex_protocol-0.1.1/vertex_protocol/utils/expiration.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.0/vertex_protocol/utils/math.py` & `vertex_protocol-0.1.1/vertex_protocol/utils/math.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.0/vertex_protocol/utils/model.py` & `vertex_protocol-0.1.1/vertex_protocol/utils/model.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.0/vertex_protocol/utils/nonce.py` & `vertex_protocol-0.1.1/vertex_protocol/utils/nonce.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-0.1.0/PKG-INFO` & `vertex_protocol-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: vertex-protocol
-Version: 0.1.0
+Version: 0.1.1
 Summary: Vertex Protocol SDK
 Keywords: vertex protocol,vertex sdk,vertex protocol api
 Author: Jeury Mejia
 Author-email: jeury@vertexprotocol.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: eth-account (>=0.8.0,<0.9.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: web3 (>=6.4.0,<7.0.0)
 Description-Content-Type: text/markdown
 
 # Vertex Python SDK
```

