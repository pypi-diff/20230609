# Comparing `tmp/esp-secure-cert-tool-0.9.8.tar.gz` & `tmp/esp-secure-cert-tool-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/esp-secure-cert-tool-0.9.8.tar", last modified: Wed May 10 15:42:53 2023, max compression
+gzip compressed data, was "dist/esp-secure-cert-tool-1.0.0.tar", last modified: Fri Jun  9 05:54:30 2023, max compression
```

## Comparing `esp-secure-cert-tool-0.9.8.tar` & `esp-secure-cert-tool-1.0.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:42:53.000000 esp-secure-cert-tool-0.9.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-10 15:42:41.000000 esp-secure-cert-tool-0.9.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-10 15:42:41.000000 esp-secure-cert-tool-0.9.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-05-10 15:42:53.000000 esp-secure-cert-tool-0.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-05-10 15:42:41.000000 esp-secure-cert-tool-0.9.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     9929 2023-05-10 15:42:41.000000 esp-secure-cert-tool-0.9.8/configure_esp_secure_cert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:42:53.000000 esp-secure-cert-tool-0.9.8/esp_secure_cert/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 15:42:41.000000 esp-secure-cert-tool-0.9.8/esp_secure_cert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11758 2023-05-10 15:42:41.000000 esp-secure-cert-tool-0.9.8/esp_secure_cert/configure_ds.py
--rw-r--r--   0 runner    (1001) docker     (123)     7606 2023-05-10 15:42:41.000000 esp-secure-cert-tool-0.9.8/esp_secure_cert/custflash_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-05-10 15:42:41.000000 esp-secure-cert-tool-0.9.8/esp_secure_cert/esp_secure_cert_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-05-10 15:42:41.000000 esp-secure-cert-tool-0.9.8/esp_secure_cert/nvs_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     7963 2023-05-10 15:42:41.000000 esp-secure-cert-tool-0.9.8/esp_secure_cert/tlv_format.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:42:53.000000 esp-secure-cert-tool-0.9.8/esp_secure_cert_tool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-05-10 15:42:53.000000 esp-secure-cert-tool-0.9.8/esp_secure_cert_tool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-10 15:42:53.000000 esp-secure-cert-tool-0.9.8/esp_secure_cert_tool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 15:42:53.000000 esp-secure-cert-tool-0.9.8/esp_secure_cert_tool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-10 15:42:53.000000 esp-secure-cert-tool-0.9.8/esp_secure_cert_tool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-10 15:42:53.000000 esp-secure-cert-tool-0.9.8/esp_secure_cert_tool.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-10 15:42:41.000000 esp-secure-cert-tool-0.9.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 15:42:53.000000 esp-secure-cert-tool-0.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-05-10 15:42:41.000000 esp-secure-cert-tool-0.9.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:54:30.000000 esp-secure-cert-tool-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-09 05:54:17.000000 esp-secure-cert-tool-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-09 05:54:17.000000 esp-secure-cert-tool-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-06-09 05:54:30.000000 esp-secure-cert-tool-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-06-09 05:54:17.000000 esp-secure-cert-tool-1.0.0/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15564 2023-06-09 05:54:17.000000 esp-secure-cert-tool-1.0.0/configure_esp_secure_cert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:54:30.000000 esp-secure-cert-tool-1.0.0/esp_secure_cert/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 05:54:17.000000 esp-secure-cert-tool-1.0.0/esp_secure_cert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-06-09 05:54:17.000000 esp-secure-cert-tool-1.0.0/esp_secure_cert/configure_ds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7606 2023-06-09 05:54:17.000000 esp-secure-cert-tool-1.0.0/esp_secure_cert/custflash_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9780 2023-06-09 05:54:17.000000 esp-secure-cert-tool-1.0.0/esp_secure_cert/efuse_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-06-09 05:54:17.000000 esp-secure-cert-tool-1.0.0/esp_secure_cert/esp_secure_cert_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-06-09 05:54:17.000000 esp-secure-cert-tool-1.0.0/esp_secure_cert/nvs_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14937 2023-06-09 05:54:17.000000 esp-secure-cert-tool-1.0.0/esp_secure_cert/tlv_format.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:54:30.000000 esp-secure-cert-tool-1.0.0/esp_secure_cert_tool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-06-09 05:54:30.000000 esp-secure-cert-tool-1.0.0/esp_secure_cert_tool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-09 05:54:30.000000 esp-secure-cert-tool-1.0.0/esp_secure_cert_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 05:54:30.000000 esp-secure-cert-tool-1.0.0/esp_secure_cert_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-09 05:54:30.000000 esp-secure-cert-tool-1.0.0/esp_secure_cert_tool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-09 05:54:30.000000 esp-secure-cert-tool-1.0.0/esp_secure_cert_tool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-09 05:54:17.000000 esp-secure-cert-tool-1.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 05:54:30.000000 esp-secure-cert-tool-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-06-09 05:54:17.000000 esp-secure-cert-tool-1.0.0/setup.py
```

### Comparing `esp-secure-cert-tool-0.9.8/LICENSE` & `esp-secure-cert-tool-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `esp-secure-cert-tool-0.9.8/PKG-INFO` & `esp-secure-cert-tool-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esp-secure-cert-tool
-Version: 0.9.8
+Version: 1.0.0
 Summary: A python utility which helps to configure and provisionthe ESP platform with PKI credentials into the esp_secure_cert partition
 Home-page: https://github.com/espressif/esp_secure_cert_mgr/blob/main/tools
 Author: Espressif Systems
 Author-email: 
 License: Apache-2.0
 Project-URL: Documentation, https://github.com/espressif/esp_secure_cert_mgr/blob/main/tools/README.md
 Project-URL: Source, https://github.com/espressif/esp_secure_cert_mgr/blob/main/tools/configure_esp_secure_cert.py
```

### Comparing `esp-secure-cert-tool-0.9.8/README.md` & `esp-secure-cert-tool-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `esp-secure-cert-tool-0.9.8/esp_secure_cert/custflash_format.py` & `esp-secure-cert-tool-1.0.0/esp_secure_cert/custflash_format.py`

 * *Files identical despite different names*

### Comparing `esp-secure-cert-tool-0.9.8/esp_secure_cert/esp_secure_cert_helper.py` & `esp-secure-cert-tool-1.0.0/esp_secure_cert/esp_secure_cert_helper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 from typing import Dict
 from cryptography.hazmat.primitives import serialization
 from cryptography.hazmat.backends import default_backend
-from cryptography.x509 import load_pem_x509_certificate, load_der_x509_certificate
+from cryptography.x509 import (
+    load_pem_x509_certificate,
+    load_der_x509_certificate
+)
 
-def load_private_key(key_file_path: str, password: str = None) -> Dict[str, str]:
+
+def load_private_key(key_file_path: str,
+                     password: str = None) -> Dict[str, str]:
     """
     Load a private key from a file in either PEM or DER format.
 
     Args:
         key_file_path (str): Path to the private key file.
-        password (str): Password to decrypt the private key, if it is encrypted.
-
+        password (str): Password to decrypt the private key,
+                        if it is encrypted.
     Returns:
         Dict[str, str]: A dictionary with the `"encoding"` and `"bytes"` keys.
-        The `"encoding"` key holds a value of type `str` (a member of the `serialization.Encoding`
-        enum) and the `"bytes"` key holds a value of type `bytes`.
+        The `"encoding"` key holds a value
+        of type `str` (a member of the `serialization.Encoding` enum)
+        and the `"bytes"` key holds a value of type `bytes`.
 
     Raises:
         FileNotFoundError: If the private key file cannot be found or read.
         ValueError: If the private key file is not in PEM or DER format.
 
     """
     result = {}
@@ -27,45 +33,68 @@
         with open(key_file_path, "rb") as key_file:
             key = key_file.read()
     except FileNotFoundError:
         raise FileNotFoundError(f"Key file not found: {key_file_path}")
 
     try:
         # Attempt to load the key as a PEM-encoded private key
-        private_key = serialization.load_pem_private_key(key, password=password, backend=default_backend())
+        private_key = serialization.load_pem_private_key(
+                key,
+                password=password,
+                backend=default_backend())
+
         result["encoding"] = serialization.Encoding.PEM.value
-        result["bytes"] = private_key.private_bytes(encoding=serialization.Encoding.PEM,
-                                                    format=serialization.PrivateFormat.TraditionalOpenSSL,
-                                                    encryption_algorithm=serialization.NoEncryption())
+        key_encoding = serialization.Encoding.PEM
+        key_enc_alg = serialization.NoEncryption()
+        priv_key_format = serialization.PrivateFormat.TraditionalOpenSSL
+
+        result["bytes"] = private_key.private_bytes(
+            encoding=key_encoding,
+            format=priv_key_format,
+            encryption_algorithm=key_enc_alg
+        )
+        result["key_instance"] = private_key
         return result
     except ValueError:
         pass
 
     try:
-        private_key = serialization.load_der_private_key(key, password=password, backend=default_backend())
+        private_key = serialization.load_der_private_key(
+            key,
+            password=password,
+            backend=default_backend()
+        )
         result["encoding"] = serialization.Encoding.DER.value
-        result["bytes"] = private_key.private_bytes(encoding=serialization.Encoding.DER,
-                                                    format=serialization.PrivateFormat.TraditionalOpenSSL,
-                                                    encryption_algorithm=serialization.NoEncryption())
+        key_encoding = serialization.Encoding.DER
+        priv_key_format = serialization.PrivateFormat.TraditionalOpenSSL
+        key_enc_alg = serialization.NoEncryption()
+        result["bytes"] = private_key.private_bytes(
+            encoding=key_encoding,
+            format=priv_key_format,
+            encryption_algorithm=key_enc_alg
+        )
+        result["key_instance"] = private_key
         return result
     except ValueError:
-        raise ValueError("Unsupported key encoding format, Please provide PEM or DER encoded key")
+        raise ValueError("Unsupported key encoding format,"
+                         " Please provide PEM or DER encoded key")
 
 
 def load_certificate(cert_file_path: str) -> Dict[str, str]:
     """
     Load a certificate from a file in either PEM or DER format.
 
     Args:
         cert_file_path (str): The path to the certificate file.
 
     Returns:
         Dict[str, str]: A dictionary with the `"encoding"` and `"bytes"` keys.
-        The `"encoding"` key holds a value of type `str` (a member of the `serialization.Encoding`
-        enum) and the `"bytes"` key holds a value of type `bytes`.
+        The `"encoding"` key holds a value of
+        type `str` (a member of the `serialization.Encoding enum)
+        and the `"bytes"` key holds a value of type `bytes`.
 
     Raises:
         FileNotFoundError: If the certificate file cannot be found or read.
         ValueError: If the certificate file is not in PEM or DER format.
     """
     result = {}
 
@@ -74,20 +103,24 @@
             cert_data = cert_file.read()
     except FileNotFoundError:
         raise FileNotFoundError(f"Cert file not found: {cert_file_path}")
 
     try:
         cert = load_pem_x509_certificate(cert_data, backend=default_backend())
         result["encoding"] = serialization.Encoding.PEM.value
-        result["bytes"] = cert.public_bytes(encoding=serialization.Encoding.PEM)
+        cert_encoding = serialization.Encoding.PEM
+        result["bytes"] = cert.public_bytes(encoding=cert_encoding)
+        result["cert_instance"] = cert
         return result
     except ValueError:
         pass
 
     try:
         cert = load_der_x509_certificate(cert_data, backend=default_backend())
         result["encoding"] = serialization.Encoding.DER.value
-        result["bytes"] = cert.public_bytes(encoding=serialization.Encoding.DER)
+        cert_encoding = serialization.Encoding.DER
+        result["bytes"] = cert.public_bytes(encoding=cert_encoding)
+        result["cert_instance"] = cert
         return result
     except ValueError:
-        raise ValueError("Unsupported certificate encoding format, Please provide PEM or DER encoded certificate")
-
+        raise ValueError("Unsupported certificate encoding format,"
+                         "Please provide PEM or DER encoded certificate")
```

### Comparing `esp-secure-cert-tool-0.9.8/esp_secure_cert/nvs_format.py` & `esp-secure-cert-tool-1.0.0/esp_secure_cert/nvs_format.py`

 * *Files identical despite different names*

### Comparing `esp-secure-cert-tool-0.9.8/esp_secure_cert_tool.egg-info/PKG-INFO` & `esp-secure-cert-tool-1.0.0/esp_secure_cert_tool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esp-secure-cert-tool
-Version: 0.9.8
+Version: 1.0.0
 Summary: A python utility which helps to configure and provisionthe ESP platform with PKI credentials into the esp_secure_cert partition
 Home-page: https://github.com/espressif/esp_secure_cert_mgr/blob/main/tools
 Author: Espressif Systems
 Author-email: 
 License: Apache-2.0
 Project-URL: Documentation, https://github.com/espressif/esp_secure_cert_mgr/blob/main/tools/README.md
 Project-URL: Source, https://github.com/espressif/esp_secure_cert_mgr/blob/main/tools/configure_esp_secure_cert.py
```

### Comparing `esp-secure-cert-tool-0.9.8/setup.py` & `esp-secure-cert-tool-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     print(
         "Package setuptools is missing from your Python installation. "
         "Please see the installation section in the esp-secure-cert-tool "
         "documentation for instructions on how to install it."
     )
     exit(1)
 
-VERSION = "0.9.8"
+VERSION = "1.0.0"
 
 long_description = """
 ====================
 esp-secure-cert-tool
 ====================
 The python utility helps to configure and provision the device with
 PKI credentials to generate the esp_secure_cert partition.
```

