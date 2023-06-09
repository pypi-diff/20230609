# Comparing `tmp/devvio_util-1.5.2.tar.gz` & `tmp/devvio_util-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devvio_util-1.5.2.tar", last modified: Sun Jun  4 00:43:36 2023, max compression
+gzip compressed data, was "devvio_util-1.5.3.tar", last modified: Fri Jun  9 02:51:03 2023, max compression
```

## Comparing `devvio_util-1.5.2.tar` & `devvio_util-1.5.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 00:43:36.421477 devvio_util-1.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-04 00:43:36.421477 devvio_util-1.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 00:43:29.000000 devvio_util-1.5.2/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 00:43:36.417477 devvio_util-1.5.2/devvio_util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 00:43:29.000000 devvio_util-1.5.2/devvio_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-04 00:43:29.000000 devvio_util-1.5.2/devvio_util/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-06-04 00:43:29.000000 devvio_util-1.5.2/devvio_util/lib_creds.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 00:43:36.421477 devvio_util-1.5.2/devvio_util/primitives/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 00:43:29.000000 devvio_util-1.5.2/devvio_util/primitives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-06-04 00:43:29.000000 devvio_util-1.5.2/devvio_util/primitives/address.py
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-04 00:43:29.000000 devvio_util-1.5.2/devvio_util/primitives/atomic_transaction_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-06-04 00:43:29.000000 devvio_util-1.5.2/devvio_util/primitives/chainstate.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-04 00:43:29.000000 devvio_util-1.5.2/devvio_util/primitives/devv_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5842 2023-06-04 00:43:29.000000 devvio_util-1.5.2/devvio_util/primitives/devv_sign.py
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-06-04 00:43:29.000000 devvio_util-1.5.2/devvio_util/primitives/final_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-06-04 00:43:29.000000 devvio_util-1.5.2/devvio_util/primitives/signature.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-04 00:43:29.000000 devvio_util-1.5.2/devvio_util/primitives/smart_coin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-06-04 00:43:29.000000 devvio_util-1.5.2/devvio_util/primitives/summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     7504 2023-06-04 00:43:29.000000 devvio_util-1.5.2/devvio_util/primitives/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-06-04 00:43:29.000000 devvio_util-1.5.2/devvio_util/primitives/transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-06-04 00:43:29.000000 devvio_util-1.5.2/devvio_util/primitives/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-06-04 00:43:29.000000 devvio_util-1.5.2/devvio_util/primitives/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-06-04 00:43:29.000000 devvio_util-1.5.2/devvio_util/psql_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 00:43:36.417477 devvio_util-1.5.2/devvio_util.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-04 00:43:36.000000 devvio_util-1.5.2/devvio_util.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-04 00:43:36.000000 devvio_util-1.5.2/devvio_util.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 00:43:36.000000 devvio_util-1.5.2/devvio_util.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 00:43:36.000000 devvio_util-1.5.2/devvio_util.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-04 00:43:36.000000 devvio_util-1.5.2/devvio_util.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-04 00:43:36.421477 devvio_util-1.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-04 00:43:29.000000 devvio_util-1.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 02:51:03.498459 devvio_util-1.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-09 02:51:03.498459 devvio_util-1.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 02:50:54.000000 devvio_util-1.5.3/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 02:51:03.490459 devvio_util-1.5.3/devvio_util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 02:50:54.000000 devvio_util-1.5.3/devvio_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-09 02:50:54.000000 devvio_util-1.5.3/devvio_util/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-06-09 02:50:54.000000 devvio_util-1.5.3/devvio_util/lib_creds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 02:51:03.494459 devvio_util-1.5.3/devvio_util/primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 02:50:54.000000 devvio_util-1.5.3/devvio_util/primitives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-06-09 02:50:54.000000 devvio_util-1.5.3/devvio_util/primitives/address.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-09 02:50:54.000000 devvio_util-1.5.3/devvio_util/primitives/atomic_transaction_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-06-09 02:50:54.000000 devvio_util-1.5.3/devvio_util/primitives/chainstate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-09 02:50:54.000000 devvio_util-1.5.3/devvio_util/primitives/devv_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9773 2023-06-09 02:50:54.000000 devvio_util-1.5.3/devvio_util/primitives/devv_sign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-06-09 02:50:54.000000 devvio_util-1.5.3/devvio_util/primitives/final_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-06-09 02:50:54.000000 devvio_util-1.5.3/devvio_util/primitives/signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-09 02:50:54.000000 devvio_util-1.5.3/devvio_util/primitives/smart_coin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-06-09 02:50:54.000000 devvio_util-1.5.3/devvio_util/primitives/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12179 2023-06-09 02:50:54.000000 devvio_util-1.5.3/devvio_util/primitives/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-06-09 02:50:54.000000 devvio_util-1.5.3/devvio_util/primitives/transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-06-09 02:50:54.000000 devvio_util-1.5.3/devvio_util/primitives/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-06-09 02:50:54.000000 devvio_util-1.5.3/devvio_util/primitives/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-06-09 02:50:54.000000 devvio_util-1.5.3/devvio_util/psql_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 02:51:03.490459 devvio_util-1.5.3/devvio_util.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-09 02:51:03.000000 devvio_util-1.5.3/devvio_util.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-09 02:51:03.000000 devvio_util-1.5.3/devvio_util.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 02:51:03.000000 devvio_util-1.5.3/devvio_util.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 02:51:03.000000 devvio_util-1.5.3/devvio_util.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-09 02:51:03.000000 devvio_util-1.5.3/devvio_util.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-09 02:51:03.498459 devvio_util-1.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-09 02:50:54.000000 devvio_util-1.5.3/setup.py
```

### Comparing `devvio_util-1.5.2/devvio_util/config.py` & `devvio_util-1.5.3/devvio_util/config.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.2/devvio_util/lib_creds.py` & `devvio_util-1.5.3/devvio_util/lib_creds.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.2/devvio_util/primitives/address.py` & `devvio_util-1.5.3/devvio_util/primitives/address.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,17 @@
         return self.get_size()
 
     # get address size (without buffer)
     def get_size(self) -> int:
         return self._size
 
     # get address bytes
-    def get_canonical(self) -> bytes:
+    def get_canonical(self, legacy: bool = False) -> bytes:
+        if legacy:
+            return self._canonical[1:]
         return self._canonical
 
     # get formatted address
     def get_hex_str(self) -> str:
         if not self._canonical:
             raise Exception('Address is not initialized!')
         return self._canonical.hex()[2:].upper()
```

### Comparing `devvio_util-1.5.2/devvio_util/primitives/chainstate.py` & `devvio_util-1.5.3/devvio_util/primitives/chainstate.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.2/devvio_util/primitives/devv_constants.py` & `devvio_util-1.5.3/devvio_util/primitives/devv_constants.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.2/devvio_util/primitives/final_block.py` & `devvio_util-1.5.3/devvio_util/primitives/final_block.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.2/devvio_util/primitives/signature.py` & `devvio_util-1.5.3/devvio_util/primitives/signature.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,17 @@
         return self.get_size()
 
     # get sig length (without prefix)
     def get_size(self) -> int:
         return self._size
 
     # get raw sig
-    def get_canonical(self) -> bytes:
+    def get_canonical(self, legacy: bool = False) -> bytes:
+        if legacy:
+            return self._canonical[1:]
         return self._canonical
 
     # return hex representation (without prefix)
     def get_hex_str(self) -> str:
         if not self._canonical:
             raise Exception('Signature is not initialized!')
         return self._canonical.hex()[2:].upper()
```

### Comparing `devvio_util-1.5.2/devvio_util/primitives/smart_coin.py` & `devvio_util-1.5.3/devvio_util/primitives/smart_coin.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.2/devvio_util/primitives/summary.py` & `devvio_util-1.5.3/devvio_util/primitives/summary.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.2/devvio_util/primitives/transfer.py` & `devvio_util-1.5.3/devvio_util/primitives/transfer.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.2/devvio_util/primitives/utils.py` & `devvio_util-1.5.3/devvio_util/primitives/utils.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.2/devvio_util/primitives/validation.py` & `devvio_util-1.5.3/devvio_util/primitives/validation.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.2/devvio_util/psql_mixin.py` & `devvio_util-1.5.3/devvio_util/psql_mixin.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.2/devvio_util.egg-info/SOURCES.txt` & `devvio_util-1.5.3/devvio_util.egg-info/SOURCES.txt`

 * *Files identical despite different names*

