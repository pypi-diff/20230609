# Comparing `tmp/uw_saml-1.2.2.tar.gz` & `tmp/uw_saml-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uw_saml-1.2.2.tar", max compression
+gzip compressed data, was "uw_saml-1.2.3.tar", max compression
```

## Comparing `uw_saml-1.2.2.tar` & `uw_saml-1.2.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      564 2023-05-03 22:16:45.560744 uw_saml-1.2.2/LICENSE
--rw-r--r--   0        0        0      606 2023-05-03 22:16:45.564744 uw_saml-1.2.2/pyproject.toml
--rw-r--r--   0        0        0       53 2023-05-03 22:16:45.564744 uw_saml-1.2.2/uw_saml2/VERSION
--rw-r--r--   0        0        0       70 2023-05-03 22:16:45.564744 uw_saml-1.2.2/uw_saml2/__init__.py
--rw-r--r--   0        0        0     3221 2023-05-03 22:16:45.564744 uw_saml-1.2.2/uw_saml2/auth.py
--rw-r--r--   0        0        0      389 2023-05-03 22:16:45.564744 uw_saml-1.2.2/uw_saml2/idp/__init__.py
--rw-r--r--   0        0        0     1619 2023-05-03 22:16:45.564744 uw_saml-1.2.2/uw_saml2/idp/attribute.py
--rw-r--r--   0        0        0     9878 2023-05-03 22:16:45.564744 uw_saml-1.2.2/uw_saml2/idp/federated.py
--rw-r--r--   0        0        0     2589 2023-05-03 22:16:45.564744 uw_saml-1.2.2/uw_saml2/idp/uw.py
--rw-r--r--   0        0        0     1538 2023-05-03 22:16:45.564744 uw_saml-1.2.2/uw_saml2/mock.py
--rw-r--r--   0        0        0      279 2023-05-03 22:16:45.564744 uw_saml-1.2.2/uw_saml2/python3_saml.py
--rw-r--r--   0        0        0     2302 2023-05-03 22:16:45.564744 uw_saml-1.2.2/uw_saml2/sp.py
--rw-r--r--   0        0        0      732 1970-01-01 00:00:00.000000 uw_saml-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0      564 2023-06-08 22:58:14.080633 uw_saml-1.2.3/LICENSE
+-rw-r--r--   0        0        0      606 2023-06-08 22:58:14.080633 uw_saml-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0       53 2023-06-08 22:58:14.080633 uw_saml-1.2.3/uw_saml2/VERSION
+-rw-r--r--   0        0        0       70 2023-06-08 22:58:14.080633 uw_saml-1.2.3/uw_saml2/__init__.py
+-rw-r--r--   0        0        0     3221 2023-06-08 22:58:14.080633 uw_saml-1.2.3/uw_saml2/auth.py
+-rw-r--r--   0        0        0      389 2023-06-08 22:58:14.080633 uw_saml-1.2.3/uw_saml2/idp/__init__.py
+-rw-r--r--   0        0        0     1619 2023-06-08 22:58:14.080633 uw_saml-1.2.3/uw_saml2/idp/attribute.py
+-rw-r--r--   0        0        0    12055 2023-06-08 22:58:14.080633 uw_saml-1.2.3/uw_saml2/idp/federated.py
+-rw-r--r--   0        0        0     2589 2023-06-08 22:58:14.080633 uw_saml-1.2.3/uw_saml2/idp/uw.py
+-rw-r--r--   0        0        0     1538 2023-06-08 22:58:14.080633 uw_saml-1.2.3/uw_saml2/mock.py
+-rw-r--r--   0        0        0      279 2023-06-08 22:58:14.080633 uw_saml-1.2.3/uw_saml2/python3_saml.py
+-rw-r--r--   0        0        0     2302 2023-06-08 22:58:14.080633 uw_saml-1.2.3/uw_saml2/sp.py
+-rw-r--r--   0        0        0      732 1970-01-01 00:00:00.000000 uw_saml-1.2.3/PKG-INFO
```

### Comparing `uw_saml-1.2.2/LICENSE` & `uw_saml-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `uw_saml-1.2.2/pyproject.toml` & `uw_saml-1.2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "uw-saml"
-version = "1.2.2"
+version = "1.2.3"
 description = "A UW-specific adapter to the python3-saml package."
 authors = []
 license = "Apache 2.0"
 packages = [
     { include = 'uw_saml2' }
 ]
```

### Comparing `uw_saml-1.2.2/uw_saml2/auth.py` & `uw_saml-1.2.3/uw_saml2/auth.py`

 * *Files identical despite different names*

### Comparing `uw_saml-1.2.2/uw_saml2/idp/attribute.py` & `uw_saml-1.2.3/uw_saml2/idp/attribute.py`

 * *Files identical despite different names*

### Comparing `uw_saml-1.2.2/uw_saml2/idp/federated.py` & `uw_saml-1.2.3/uw_saml2/idp/federated.py`

 * *Files 18% similar despite different names*

```diff
@@ -28,14 +28,50 @@
         8EQ2uSOElcY7ZBx+55yAzCW8TSGA3TMLRcKXozfk++HFoLEXbZaTo447BUb9b82U
         Mv42rFI66/59obGWdQ6UHyGCvyN4FBd4nYCcpM6pKxOfhMbAA7F6rcCRYisSjkZe
         5FymL4FYVDuJ6WdSaWEIbpojD8+nnJpS8Yal/8qicwMWCT9VpUDHmsZC5WiKmTXm
         RXE3esrKhhuPEkK1Qk0mLw==
     """
 
 
+class CascadiaAzureIdp(IdpConfig):
+    """
+    Cascadia Azure configuration to replace CascadiaIdp (also, using FH as template)
+    App Federation Metadata Url https://login.microsoftonline.com/2505efd9-9f5d-4941-865c-03c9b1b88613/federationmetadata/2007-06/federationmetadata.xml?appid=668d7144-d842-4069-a70b-cae9f6ccc14f
+    Login URL: https://login.microsoftonline.com/2505efd9-9f5d-4941-865c-03c9b1b88613/saml2
+    Azure AD Identifier: https://sts.windows.net/2505efd9-9f5d-4941-865c-03c9b1b88613/
+    Logout URL: https://login.microsoftonline.com/2505efd9-9f5d-4941-865c-03c9b1b88613/saml2
+    """
+
+    _azure_tenant_id = "2505efd9-9f5d-4941-865c-03c9b1b88613"
+    _attribute_prefix = "http://schemas.xmlsoap.org/ws/2005/05/identity/claims"
+    _attribute_prefix2 = "http://schemas.microsoft.com/identity/claims"
+
+    entity_id = f"https://sts.windows.net/{_azure_tenant_id}/"
+    sso_url = f"https://login.microsoftonline.com/{_azure_tenant_id}/saml2"
+    id_attribute = "employeeNumber"
+    x509_cert = """
+        MIIC8DCCAdigAwIBAgIQW2YmoB9jVZBN+X8BnmMIbTANBgkqhkiG9w0BAQsFADA0
+        MTIwMAYDVQQDEylNaWNyb3NvZnQgQXp1cmUgRmVkZXJhdGVkIFNTTyBDZXJ0aWZp
+        Y2F0ZTAeFw0yMzA1MDEyMTQ1MDVaFw0yNjA1MDEyMTQ1MDVaMDQxMjAwBgNVBAMT
+        KU1pY3Jvc29mdCBBenVyZSBGZWRlcmF0ZWQgU1NPIENlcnRpZmljYXRlMIIBIjAN
+        BgkqhkiG9w0BAQEFAAOCAQ8AMIIBCgKCAQEAr+dzHUWeBI5HozHBuB1hFSh67A7m
+        lPJxqnNsw4rGV72niCDSzn8eFZUWH2RDQjWRWdjWaaE39ZTPmrAlhi9II0Ezw8IW
+        /kGprP/OF9qtXgYZ3Vd0iLSowtmPtvfVDYHs42VHd1pcCGZO68L9cnk0rxJayqjN
+        itljXIIrQ4nqSO2aSCx66m/jA6mGFj36+wJle8zHcBPFKlIxaGLx04A72EPVb8Sp
+        s4yc1gKhdEHrvGjmqnjlz997iU1H8esLDAwMihO6Ha6tFdj29/JPCTJMWM2bY4dw
+        juTEMncRodHVBADdtvasW6JlhcH6KNqvClxU0/x+1dkiiF/2icHYatdHdQIDAQAB
+        MA0GCSqGSIb3DQEBCwUAA4IBAQBRhl49scTEf17CBrT9Lk5vsFCrcS/wMpSi569t
+        hUmxrQmx9jyEfQ7M4b3bH50nTU6Z/2whJq1Fcy3gHL8zB8UvGLHWnTE2wHQ1+Yzs
+        u+mkjAUOgSiFGX5aVHAco6eU/MwgIBcgA4D0+hmcVlrWQlmdq/juXQ7Bto7KYMu+
+        52ui4kMavtgftgtfrNmE9b/eKFqTA3wYEXLZVJzclMm3g3VItWnfvRpF/eG8CpjI
+        wJPxARowqyxR5q6PWX5JzOtFzuCx0vJ/jI0o8iAg53fOitgDFj3E6/qxjPhoDY+Q
+        Pq4dr8god4m9Nr6k8kFWBbL2sXn1GC72SDeuvk0Q4X3t8tLb
+    """
+
+
 class CollegenetIdp(IdpConfig):
     """
     One thing of note about collegenet is that it encrypts attributes and thus
     requires an SP cert and key.
     """
 
     _idp_url = "https://shibboleth-idp.collegenet.com"
```

### Comparing `uw_saml-1.2.2/uw_saml2/idp/uw.py` & `uw_saml-1.2.3/uw_saml2/idp/uw.py`

 * *Files identical despite different names*

### Comparing `uw_saml-1.2.2/uw_saml2/mock.py` & `uw_saml-1.2.3/uw_saml2/mock.py`

 * *Files identical despite different names*

### Comparing `uw_saml-1.2.2/uw_saml2/sp.py` & `uw_saml-1.2.3/uw_saml2/sp.py`

 * *Files identical despite different names*

### Comparing `uw_saml-1.2.2/PKG-INFO` & `uw_saml-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uw-saml
-Version: 1.2.2
+Version: 1.2.3
 Summary: A UW-specific adapter to the python3-saml package.
 License: Apache 2.0
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

