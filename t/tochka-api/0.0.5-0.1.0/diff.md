# Comparing `tmp/tochka_api-0.0.5.tar.gz` & `tmp/tochka_api-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tochka_api-0.0.5.tar", last modified: Fri Sep 30 06:59:08 2022, max compression
+gzip compressed data, was "tochka_api-0.1.0.tar", last modified: Fri Jun  9 18:37:08 2023, max compression
```

## Comparing `tochka_api-0.0.5.tar` & `tochka_api-0.1.0.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-09-30 06:59:08.563888 tochka_api-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (122)    16724 2022-09-30 06:59:04.000000 tochka_api-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     1699 2022-09-30 06:59:08.563888 tochka_api-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1256 2022-09-30 06:59:04.000000 tochka_api-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       78 2022-09-30 06:59:04.000000 tochka_api-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-09-30 06:59:08.563888 tochka_api-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1048 2022-09-30 06:59:04.000000 tochka_api-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-09-30 06:59:08.559888 tochka_api-0.0.5/tochka_api/
--rw-r--r--   0 runner    (1001) docker     (122)       30 2022-09-30 06:59:04.000000 tochka_api-0.0.5/tochka_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-09-30 06:59:08.563888 tochka_api-0.0.5/tochka_api/exceptions/
--rw-r--r--   0 runner    (1001) docker     (122)       55 2022-09-30 06:59:04.000000 tochka_api-0.0.5/tochka_api/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1041 2022-09-30 06:59:04.000000 tochka_api-0.0.5/tochka_api/exceptions/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-09-30 06:59:08.563888 tochka_api-0.0.5/tochka_api/models/
--rw-r--r--   0 runner    (1001) docker     (122)      116 2022-09-30 06:59:04.000000 tochka_api-0.0.5/tochka_api/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2093 2022-09-30 06:59:04.000000 tochka_api-0.0.5/tochka_api/models/permissions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-09-30 06:59:08.563888 tochka_api-0.0.5/tochka_api/models/responses/
--rw-r--r--   0 runner    (1001) docker     (122)      614 2022-09-30 06:59:04.000000 tochka_api-0.0.5/tochka_api/models/responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1869 2022-09-30 06:59:04.000000 tochka_api-0.0.5/tochka_api/models/responses/accounts.py
--rw-r--r--   0 runner    (1001) docker     (122)     1922 2022-09-30 06:59:04.000000 tochka_api-0.0.5/tochka_api/models/responses/balances.py
--rw-r--r--   0 runner    (1001) docker     (122)      477 2022-09-30 06:59:04.000000 tochka_api-0.0.5/tochka_api/models/responses/base.py
--rw-r--r--   0 runner    (1001) docker     (122)      738 2022-09-30 06:59:04.000000 tochka_api-0.0.5/tochka_api/models/responses/consents.py
--rw-r--r--   0 runner    (1001) docker     (122)      455 2022-09-30 06:59:04.000000 tochka_api-0.0.5/tochka_api/models/responses/sbp_accounts.py
--rw-r--r--   0 runner    (1001) docker     (122)     2832 2022-09-30 06:59:04.000000 tochka_api-0.0.5/tochka_api/models/responses/sbp_legal.py
--rw-r--r--   0 runner    (1001) docker     (122)      613 2022-09-30 06:59:04.000000 tochka_api-0.0.5/tochka_api/models/responses/sbp_merchants.py
--rw-r--r--   0 runner    (1001) docker     (122)     2718 2022-09-30 06:59:04.000000 tochka_api-0.0.5/tochka_api/models/responses/sbp_qr.py
--rw-r--r--   0 runner    (1001) docker     (122)      899 2022-09-30 06:59:04.000000 tochka_api-0.0.5/tochka_api/models/responses/sbp_refunds.py
--rw-r--r--   0 runner    (1001) docker     (122)     2470 2022-09-30 06:59:04.000000 tochka_api-0.0.5/tochka_api/models/tokens.py
--rw-r--r--   0 runner    (1001) docker     (122)      266 2022-09-30 06:59:04.000000 tochka_api-0.0.5/tochka_api/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-09-30 06:59:08.559888 tochka_api-0.0.5/tochka_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1699 2022-09-30 06:59:08.000000 tochka_api-0.0.5/tochka_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      818 2022-09-30 06:59:08.000000 tochka_api-0.0.5/tochka_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-09-30 06:59:08.000000 tochka_api-0.0.5/tochka_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       59 2022-09-30 06:59:08.000000 tochka_api-0.0.5/tochka_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2022-09-30 06:59:08.000000 tochka_api-0.0.5/tochka_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:37:08.419723 tochka_api-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16724 2023-06-09 18:37:04.000000 tochka_api-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7320 2023-06-09 18:37:08.419723 tochka_api-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-06-09 18:37:04.000000 tochka_api-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-09 18:37:04.000000 tochka_api-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 18:37:08.419723 tochka_api-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-09 18:37:04.000000 tochka_api-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:37:08.415723 tochka_api-0.1.0/tochka_api/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-09 18:37:04.000000 tochka_api-0.1.0/tochka_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:37:08.415723 tochka_api-0.1.0/tochka_api/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-09 18:37:04.000000 tochka_api-0.1.0/tochka_api/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-09 18:37:04.000000 tochka_api-0.1.0/tochka_api/exceptions/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:37:08.415723 tochka_api-0.1.0/tochka_api/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-09 18:37:04.000000 tochka_api-0.1.0/tochka_api/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-06-09 18:37:04.000000 tochka_api-0.1.0/tochka_api/models/permissions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:37:08.419723 tochka_api-0.1.0/tochka_api/models/responses/
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-09 18:37:04.000000 tochka_api-0.1.0/tochka_api/models/responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-06-09 18:37:04.000000 tochka_api-0.1.0/tochka_api/models/responses/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-06-09 18:37:04.000000 tochka_api-0.1.0/tochka_api/models/responses/balances.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-09 18:37:04.000000 tochka_api-0.1.0/tochka_api/models/responses/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-09 18:37:04.000000 tochka_api-0.1.0/tochka_api/models/responses/consents.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-09 18:37:04.000000 tochka_api-0.1.0/tochka_api/models/responses/sbp_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-06-09 18:37:04.000000 tochka_api-0.1.0/tochka_api/models/responses/sbp_legal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-09 18:37:04.000000 tochka_api-0.1.0/tochka_api/models/responses/sbp_merchants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-06-09 18:37:04.000000 tochka_api-0.1.0/tochka_api/models/responses/sbp_qr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-09 18:37:04.000000 tochka_api-0.1.0/tochka_api/models/responses/sbp_refunds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-06-09 18:37:04.000000 tochka_api-0.1.0/tochka_api/models/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-09 18:37:04.000000 tochka_api-0.1.0/tochka_api/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-06-09 18:37:04.000000 tochka_api-0.1.0/tochka_api/token_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:37:08.415723 tochka_api-0.1.0/tochka_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7320 2023-06-09 18:37:08.000000 tochka_api-0.1.0/tochka_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-09 18:37:08.000000 tochka_api-0.1.0/tochka_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 18:37:08.000000 tochka_api-0.1.0/tochka_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-09 18:37:08.000000 tochka_api-0.1.0/tochka_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-09 18:37:08.000000 tochka_api-0.1.0/tochka_api.egg-info/top_level.txt
```

### Comparing `tochka_api-0.0.5/LICENSE` & `tochka_api-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tochka_api-0.0.5/setup.py` & `tochka_api-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,14 @@
     url="https://github.com/WhiteApfel/tochka_api",
     license="Mozilla Public License 2.0",
     author="WhiteApfel",
     author_email="white@pfel.ru",
     description="Simple Tochka Bank Open API client",
     install_requires=requirements(),
     project_urls={
-        "Source code": "https://github.com/WhiteApfel/pyQiwiP2P",
+        "Source code": "https://github.com/WhiteApfel/tochka-api",
         "Write me": "https://t.me/whiteapfel",
     },
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     keywords="tochka openapi api bank",
 )
```

### Comparing `tochka_api-0.0.5/tochka_api/exceptions/base.py` & `tochka_api-0.1.0/tochka_api/exceptions/base.py`

 * *Files identical despite different names*

### Comparing `tochka_api-0.0.5/tochka_api/models/permissions.py` & `tochka_api-0.1.0/tochka_api/models/permissions.py`

 * *Files identical despite different names*

### Comparing `tochka_api-0.0.5/tochka_api/models/responses/__init__.py` & `tochka_api-0.1.0/tochka_api/models/responses/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from .base import TochkaBaseResponse, TochkaBooleanResponse
 from .consents import ConsentsResponse
 from .balances import BalanceResponse
 from .sbp_legal import (
     SbpLegalEntityResponse,
     SbpCustomerInfoResponse,
-    SbpRegisterLegalEntity,
+    SbpRegisterLegalEntityResponse,
     SbpAccountsResponse,
 )
 from .sbp_refunds import SbpPaymentsResponse, SbpRefundResponse
 from .sbp_qr import (
     SbpQrsResponse,
     SbpRegisterQrResponse,
     SbpQrPaymentDataResponse,
```

### Comparing `tochka_api-0.0.5/tochka_api/models/responses/accounts.py` & `tochka_api-0.1.0/tochka_api/models/responses/accounts.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     scheme: str = Field(..., alias="schemeName")
     identification: str
     name: str
 
 
 class Account(BaseModel):
     customer_code: str = Field(..., alias="customerCode")
-    account_id: str = Field(..., alias="accountId")
+    account: str = Field(..., alias="accountId")
     transit_account: str | None = Field(None, alias="transitAccount")
     status: Literal["Enabled", "Disabled", "Deleted", "ProForma", "Pending"]
     status_updated_at: datetime = Field(..., alias="statusUpdateDateTime")
     currency: str
     account_type: Literal["Business", "Personal"] = Field(..., alias="accountType")
     account_sub_type: Literal[
         "CreditCard",
```

### Comparing `tochka_api-0.0.5/tochka_api/models/responses/balances.py` & `tochka_api-0.1.0/tochka_api/models/responses/balances.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 class Amount(BaseModel):
     total: Decimal = Field(..., alias="OpeningAvailable")
     available: Decimal = Field(..., alias="ClosingAvailable")
     hold: Decimal = Field(..., alias="Expected")
 
 
 class Balance(BaseModel):
-    account_id: str = Field(..., alias="accountId")
+    account: str = Field(..., alias="accountId")
     indicator: Literal["Credit", "Debit"] = Field(..., alias="creditDebitIndicator")
     created_at: datetime = Field(..., alias="dateTime")
     currency: str
     amount: Amount
 
 
 class BalanceResponse(TochkaBaseResponse):
```

### Comparing `tochka_api-0.0.5/tochka_api/models/responses/consents.py` & `tochka_api-0.1.0/tochka_api/models/responses/consents.py`

 * *Files identical despite different names*

### Comparing `tochka_api-0.0.5/tochka_api/models/responses/sbp_legal.py` & `tochka_api-0.1.0/tochka_api/models/responses/sbp_legal.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,27 +24,31 @@
 class SbpMerchant(SbpLegalAddress):
     status: Literal["Active", "Suspended"]
     created_at: datetime = Field(..., alias="createdAt")
     legal_id: str = Field(..., alias="legalId")
     merchant_id: str = Field(..., alias="merchantId")
     brand: str = Field(..., alias="brandName")
     capabilities: Literal["001", "010", "011"]
-    phone: str = Field(..., alias="contactPhoneNumber")
+    phone: str | None = Field(None, alias="contactPhoneNumber")
     mcc: str
     additional_contacts: list[dict] | None = Field(None, alias="additionalContacts")
 
 
 class SbpAccount(BaseModel):
-    account_id: str = Field(..., alias="accountId")
+    account: str = Field(..., alias="accountId")
     status: Literal["Active", "Suspended"]
     created_at: datetime = Field(..., alias="createdAt")
     legal_id: str = Field(..., alias="legalId")
 
 
 class SbpCustomerInfoResponse(SbpLegalAddress, SbpLegalDetails, TochkaBaseResponse):
+    """
+    Refers to CustomerInfoResponseV3 https://enter.tochka.com/doc/v2/redoc/tag/swagger.json
+    """
+
     status: Literal["Active", "Suspended"]
     created_at: datetime = Field(..., alias="createdAt")
     customer_code: str = Field(..., alias="customerCode")
     legal_id: str = Field(..., alias="legalId")
     merchants: list[SbpMerchant] = Field(..., alias="MerchantList")
     accounts: list[SbpAccount] = Field(..., alias="AccountList")
 
@@ -52,15 +56,15 @@
 class SbpLegalEntityResponse(SbpLegalAddress, SbpLegalDetails, TochkaBaseResponse):
     status: Literal["Active", "Suspended"]
     created_at: datetime = Field(..., alias="createdAt")
     customer_code: str = Field(..., alias="customerCode")
     legal_id: str = Field(..., alias="legalId")
 
 
-class SbpRegisterLegalEntity(TochkaBaseResponse):
+class SbpRegisterLegalEntityResponse(TochkaBaseResponse):
     legal_id: str = Field(..., alias="legalId")
 
 
 class SbpAccountsResponse(TochkaBaseResponse):
     sbp_accounts: list[SbpAccount] = Field(..., alias="AccountList")
 
     @root_validator(pre=True)
```

### Comparing `tochka_api-0.0.5/tochka_api/models/responses/sbp_merchants.py` & `tochka_api-0.1.0/tochka_api/models/responses/sbp_merchants.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from datetime import datetime
 
-from pydantic import Field, BaseModel, root_validator
-
 from models.responses import TochkaBaseResponse
 from models.responses.sbp_legal import SbpMerchant
+from pydantic import BaseModel, Field, root_validator
 
 
 class SbpMerchantsResponse(TochkaBaseResponse):
     merchants: list[SbpMerchant] = Field(..., alias="MerchantList")
 
     @root_validator(pre=True)
     def one_merchant(cls, values: dict):
```

### Comparing `tochka_api-0.0.5/tochka_api/models/responses/sbp_refunds.py` & `tochka_api-0.1.0/tochka_api/models/responses/sbp_refunds.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         "Accepted",
         "InProgress",
         "Rejected",
         "Error",
         "Timeout",
     ]
     message: str
-    trx_id: str = Field(..., alias="trxId")
+    trx_id: str = Field(..., alias="refTransactionId")
 
 
 class SbpPaymentsResponse(TochkaBaseResponse):
     payments: list[Payment] = Field(..., alias="Payments")
 
 
 class SbpRefundResponse(TochkaBaseResponse):
```

### Comparing `tochka_api-0.0.5/tochka_api.egg-info/SOURCES.txt` & `tochka_api-0.1.0/tochka_api.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 tochka_api/__init__.py
 tochka_api/settings.py
+tochka_api/token_manager.py
 tochka_api.egg-info/PKG-INFO
 tochka_api.egg-info/SOURCES.txt
 tochka_api.egg-info/dependency_links.txt
 tochka_api.egg-info/requires.txt
 tochka_api.egg-info/top_level.txt
 tochka_api/exceptions/__init__.py
 tochka_api/exceptions/base.py
```

