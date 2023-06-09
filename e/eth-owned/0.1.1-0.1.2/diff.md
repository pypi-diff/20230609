# Comparing `tmp/eth-owned-0.1.1.tar.gz` & `tmp/eth-owned-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eth-owned-0.1.1.tar", last modified: Mon May 15 14:12:51 2023, max compression
+gzip compressed data, was "dist/eth-owned-0.1.2.tar", last modified: Fri Jun  9 09:34:28 2023, max compression
```

## Comparing `eth-owned-0.1.1.tar` & `eth-owned-0.1.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-15 14:12:51.909987 eth-owned-0.1.1/
--rw-r--r--   0 lash      (1000) lash      (1000)     3216 2021-04-17 09:25:30.000000 eth-owned-0.1.1/LICENSE
--rw-r--r--   0 lash      (1000) lash      (1000)       43 2021-08-24 19:44:28.000000 eth-owned-0.1.1/MANIFEST.in
--rw-r--r--   0 lash      (1000) lash      (1000)      708 2023-05-15 14:12:51.909987 eth-owned-0.1.1/PKG-INFO
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-15 14:12:51.909987 eth-owned-0.1.1/eth_owned/
--rw-r--r--   0 lash      (1000) lash      (1000)       62 2023-03-25 13:46:48.000000 eth-owned-0.1.1/eth_owned/__init__.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-15 14:12:51.909987 eth-owned-0.1.1/eth_owned/data/
--rw-r--r--   0 lash      (1000) lash      (1000)     3138 2023-02-28 20:25:47.000000 eth-owned-0.1.1/eth_owned/data/Owned.bin
--rw-r--r--   0 lash      (1000) lash      (1000)     1020 2023-02-28 20:25:47.000000 eth-owned-0.1.1/eth_owned/data/Owned.json
--rw-r--r--   0 lash      (1000) lash      (1000)     1502 2023-02-28 20:25:47.000000 eth-owned-0.1.1/eth_owned/data/OwnedSimple.bin
--rw-r--r--   0 lash      (1000) lash      (1000)      655 2023-02-28 20:25:47.000000 eth-owned-0.1.1/eth_owned/data/OwnedSimple.json
--rw-r--r--   0 lash      (1000) lash      (1000)     4116 2023-02-28 20:25:47.000000 eth-owned-0.1.1/eth_owned/data/VoidOwner.bin
--rw-r--r--   0 lash      (1000) lash      (1000)      556 2023-02-28 20:25:47.000000 eth-owned-0.1.1/eth_owned/data/VoidOwner.json
--rw-r--r--   0 lash      (1000) lash      (1000)       85 2021-04-17 05:52:58.000000 eth-owned-0.1.1/eth_owned/data/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1620 2023-03-25 13:46:21.000000 eth-owned-0.1.1/eth_owned/owned.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-15 14:12:51.909987 eth-owned-0.1.1/eth_owned/runnable/
--rw-r--r--   0 lash      (1000) lash      (1000)     2101 2021-10-24 14:08:49.000000 eth-owned-0.1.1/eth_owned/runnable/owner.py
--rw-r--r--   0 lash      (1000) lash      (1000)     4216 2021-10-24 14:07:02.000000 eth-owned-0.1.1/eth_owned/runnable/void.py
--rw-r--r--   0 lash      (1000) lash      (1000)     4015 2021-10-24 14:05:55.000000 eth-owned-0.1.1/eth_owned/runnable/void_deploy.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-15 14:12:51.909987 eth-owned-0.1.1/eth_owned/unittest/
--rw-r--r--   0 lash      (1000) lash      (1000)       65 2023-02-28 20:31:30.000000 eth-owned-0.1.1/eth_owned/unittest/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1348 2023-03-25 13:47:19.000000 eth-owned-0.1.1/eth_owned/unittest/base.py
--rw-r--r--   0 lash      (1000) lash      (1000)     5019 2023-03-25 13:48:57.000000 eth-owned-0.1.1/eth_owned/unittest/interface.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1406 2021-08-24 19:44:28.000000 eth-owned-0.1.1/eth_owned/void.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-15 14:12:51.909987 eth-owned-0.1.1/eth_owned.egg-info/
--rw-r--r--   0 lash      (1000) lash      (1000)      708 2023-05-15 14:12:51.000000 eth-owned-0.1.1/eth_owned.egg-info/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)      735 2023-05-15 14:12:51.000000 eth-owned-0.1.1/eth_owned.egg-info/SOURCES.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-05-15 14:12:51.000000 eth-owned-0.1.1/eth_owned.egg-info/dependency_links.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       60 2023-05-15 14:12:51.000000 eth-owned-0.1.1/eth_owned.egg-info/entry_points.txt
--rw-r--r--   0 lash      (1000) lash      (1000)      114 2023-05-15 14:12:51.000000 eth-owned-0.1.1/eth_owned.egg-info/requires.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       10 2023-05-15 14:12:51.000000 eth-owned-0.1.1/eth_owned.egg-info/top_level.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       52 2023-05-15 14:07:11.000000 eth-owned-0.1.1/requirements.txt
--rw-r--r--   0 lash      (1000) lash      (1000)     1012 2023-05-15 14:12:51.913320 eth-owned-0.1.1/setup.cfg
--rw-r--r--   0 lash      (1000) lash      (1000)      642 2021-04-17 09:25:26.000000 eth-owned-0.1.1/setup.py
--rw-r--r--   0 lash      (1000) lash      (1000)       37 2021-04-17 06:02:27.000000 eth-owned-0.1.1/test_requirements.txt
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-15 14:12:51.909987 eth-owned-0.1.1/tests/
--rw-r--r--   0 lash      (1000) lash      (1000)      262 2023-02-28 20:33:12.000000 eth-owned-0.1.1/tests/test_owned.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-09 09:34:28.246656 eth-owned-0.1.2/
+-rw-r--r--   0 lash      (1000) lash      (1000)     3216 2021-04-17 09:25:30.000000 eth-owned-0.1.2/LICENSE
+-rw-r--r--   0 lash      (1000) lash      (1000)       43 2021-08-24 19:44:28.000000 eth-owned-0.1.2/MANIFEST.in
+-rw-r--r--   0 lash      (1000) lash      (1000)      715 2023-06-09 09:34:28.246656 eth-owned-0.1.2/PKG-INFO
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-09 09:34:28.239989 eth-owned-0.1.2/eth_owned/
+-rw-r--r--   0 lash      (1000) lash      (1000)       62 2023-03-25 13:46:48.000000 eth-owned-0.1.2/eth_owned/__init__.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-09 09:34:28.243322 eth-owned-0.1.2/eth_owned/data/
+-rw-r--r--   0 lash      (1000) lash      (1000)     3138 2023-02-28 20:25:47.000000 eth-owned-0.1.2/eth_owned/data/Owned.bin
+-rw-r--r--   0 lash      (1000) lash      (1000)     1020 2023-02-28 20:25:47.000000 eth-owned-0.1.2/eth_owned/data/Owned.json
+-rw-r--r--   0 lash      (1000) lash      (1000)     1502 2023-02-28 20:25:47.000000 eth-owned-0.1.2/eth_owned/data/OwnedSimple.bin
+-rw-r--r--   0 lash      (1000) lash      (1000)      655 2023-02-28 20:25:47.000000 eth-owned-0.1.2/eth_owned/data/OwnedSimple.json
+-rw-r--r--   0 lash      (1000) lash      (1000)     4116 2023-02-28 20:25:47.000000 eth-owned-0.1.2/eth_owned/data/VoidOwner.bin
+-rw-r--r--   0 lash      (1000) lash      (1000)      556 2023-02-28 20:25:47.000000 eth-owned-0.1.2/eth_owned/data/VoidOwner.json
+-rw-r--r--   0 lash      (1000) lash      (1000)       85 2021-04-17 05:52:58.000000 eth-owned-0.1.2/eth_owned/data/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1620 2023-03-25 13:46:21.000000 eth-owned-0.1.2/eth_owned/owned.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-09 09:34:28.243322 eth-owned-0.1.2/eth_owned/runnable/
+-rw-r--r--   0 lash      (1000) lash      (1000)     2101 2021-10-24 14:08:49.000000 eth-owned-0.1.2/eth_owned/runnable/owner.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     4216 2021-10-24 14:07:02.000000 eth-owned-0.1.2/eth_owned/runnable/void.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     4015 2021-10-24 14:05:55.000000 eth-owned-0.1.2/eth_owned/runnable/void_deploy.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-09 09:34:28.246656 eth-owned-0.1.2/eth_owned/unittest/
+-rw-r--r--   0 lash      (1000) lash      (1000)      128 2023-06-09 09:27:31.000000 eth-owned-0.1.2/eth_owned/unittest/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1348 2023-03-25 13:47:19.000000 eth-owned-0.1.2/eth_owned/unittest/base.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     5018 2023-06-09 09:27:28.000000 eth-owned-0.1.2/eth_owned/unittest/interface.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1406 2021-08-24 19:44:28.000000 eth-owned-0.1.2/eth_owned/void.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-09 09:34:28.243322 eth-owned-0.1.2/eth_owned.egg-info/
+-rw-r--r--   0 lash      (1000) lash      (1000)      715 2023-06-09 09:34:28.000000 eth-owned-0.1.2/eth_owned.egg-info/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)      735 2023-06-09 09:34:28.000000 eth-owned-0.1.2/eth_owned.egg-info/SOURCES.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-06-09 09:34:28.000000 eth-owned-0.1.2/eth_owned.egg-info/dependency_links.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       60 2023-06-09 09:34:28.000000 eth-owned-0.1.2/eth_owned.egg-info/entry_points.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)      114 2023-06-09 09:34:28.000000 eth-owned-0.1.2/eth_owned.egg-info/requires.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       10 2023-06-09 09:34:28.000000 eth-owned-0.1.2/eth_owned.egg-info/top_level.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       52 2023-05-15 14:07:11.000000 eth-owned-0.1.2/requirements.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)     1019 2023-06-09 09:34:28.246656 eth-owned-0.1.2/setup.cfg
+-rw-r--r--   0 lash      (1000) lash      (1000)      642 2021-04-17 09:25:26.000000 eth-owned-0.1.2/setup.py
+-rw-r--r--   0 lash      (1000) lash      (1000)       37 2021-04-17 06:02:27.000000 eth-owned-0.1.2/test_requirements.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-09 09:34:28.246656 eth-owned-0.1.2/tests/
+-rw-r--r--   0 lash      (1000) lash      (1000)      262 2023-02-28 20:33:12.000000 eth-owned-0.1.2/tests/test_owned.py
```

### Comparing `eth-owned-0.1.1/LICENSE` & `eth-owned-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `eth-owned-0.1.1/PKG-INFO` & `eth-owned-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: eth-owned
-Version: 0.1.1
+Version: 0.1.2
 Summary: EIP 173 interface and tools
-Home-page: https://gitlab.com/cicnet/eth-owned
+Home-page: https://holbrook.no/src/eth-owned/log.html
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: AGPL3
 Keywords: ethereum
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: No Input/Output (Daemon)
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: testing
 License-File: LICENSE
```

### Comparing `eth-owned-0.1.1/eth_owned/data/Owned.bin` & `eth-owned-0.1.2/eth_owned/data/Owned.bin`

 * *Files identical despite different names*

### Comparing `eth-owned-0.1.1/eth_owned/data/Owned.json` & `eth-owned-0.1.2/eth_owned/data/Owned.json`

 * *Files identical despite different names*

### Comparing `eth-owned-0.1.1/eth_owned/data/OwnedSimple.bin` & `eth-owned-0.1.2/eth_owned/data/OwnedSimple.bin`

 * *Files identical despite different names*

### Comparing `eth-owned-0.1.1/eth_owned/data/OwnedSimple.json` & `eth-owned-0.1.2/eth_owned/data/OwnedSimple.json`

 * *Files identical despite different names*

### Comparing `eth-owned-0.1.1/eth_owned/data/VoidOwner.bin` & `eth-owned-0.1.2/eth_owned/data/VoidOwner.bin`

 * *Files identical despite different names*

### Comparing `eth-owned-0.1.1/eth_owned/data/VoidOwner.json` & `eth-owned-0.1.2/eth_owned/data/VoidOwner.json`

 * *Files identical despite different names*

### Comparing `eth-owned-0.1.1/eth_owned/owned.py` & `eth-owned-0.1.2/eth_owned/owned.py`

 * *Files identical despite different names*

### Comparing `eth-owned-0.1.1/eth_owned/runnable/owner.py` & `eth-owned-0.1.2/eth_owned/runnable/owner.py`

 * *Files identical despite different names*

### Comparing `eth-owned-0.1.1/eth_owned/runnable/void.py` & `eth-owned-0.1.2/eth_owned/runnable/void.py`

 * *Files identical despite different names*

### Comparing `eth-owned-0.1.1/eth_owned/runnable/void_deploy.py` & `eth-owned-0.1.2/eth_owned/runnable/void_deploy.py`

 * *Files identical despite different names*

### Comparing `eth-owned-0.1.1/eth_owned/unittest/base.py` & `eth-owned-0.1.2/eth_owned/unittest/base.py`

 * *Files identical despite different names*

### Comparing `eth-owned-0.1.1/eth_owned/unittest/interface.py` & `eth-owned-0.1.2/eth_owned/unittest/interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,10 +120,9 @@
 #        c = Owned(self.chain_spec, nonce_oracle=nonce_oracle, gas_oracle=gas_oracle, signer=self.signer)
 #        (tx_hash_hex, o) = c.transfer_ownership(self.address, self.accounts[0], self.accounts[1], final=True)
 #        r = self.conn.do(o)
 #        o = receipt(tx_hash_hex)
 #        r = self.conn.do(o)
 #        self.assertEqual(r['status'], 0)
 
-
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `eth-owned-0.1.1/eth_owned/void.py` & `eth-owned-0.1.2/eth_owned/void.py`

 * *Files identical despite different names*

### Comparing `eth-owned-0.1.1/eth_owned.egg-info/PKG-INFO` & `eth-owned-0.1.2/eth_owned.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: eth-owned
-Version: 0.1.1
+Version: 0.1.2
 Summary: EIP 173 interface and tools
-Home-page: https://gitlab.com/cicnet/eth-owned
+Home-page: https://holbrook.no/src/eth-owned/log.html
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: AGPL3
 Keywords: ethereum
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: No Input/Output (Daemon)
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: testing
 License-File: LICENSE
```

### Comparing `eth-owned-0.1.1/eth_owned.egg-info/SOURCES.txt` & `eth-owned-0.1.2/eth_owned.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eth-owned-0.1.1/setup.cfg` & `eth-owned-0.1.2/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [metadata]
 name = eth-owned
-version = 0.1.1
+version = 0.1.2
 description = EIP 173 interface and tools
 author = Louis Holbrook
 author_email = dev@holbrook.no
-url = https://gitlab.com/cicnet/eth-owned
+url = https://holbrook.no/src/eth-owned/log.html
 keywords = 
 	ethereum
 classifiers = 
 	Programming Language :: Python :: 3
 	Operating System :: OS Independent
 	Development Status :: 3 - Alpha
 	Environment :: No Input/Output (Daemon)
@@ -18,15 +18,15 @@
 	Topic :: Software Development :: Libraries
 license = AGPL3
 licence_files = 
 	LICENSE.txt
 
 [options]
 include_package_data = True
-python_requires = >= 3.7
+python_requires = >= 3.8
 packages = 
 	eth_owned
 	eth_owned.data
 	eth_owned.unittest
 	eth_owned.runnable
 
 [options.extras_require]
```

### Comparing `eth-owned-0.1.1/setup.py` & `eth-owned-0.1.2/setup.py`

 * *Files identical despite different names*

