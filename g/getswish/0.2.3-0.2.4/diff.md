# Comparing `tmp/getswish-0.2.3.tar.gz` & `tmp/getswish-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getswish-0.2.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "getswish-0.2.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `getswish-0.2.3.tar` & `getswish-0.2.4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0      482 2023-06-01 04:53:33.993483 getswish-0.2.3/.github/workflows/pytest.yml
--rw-r--r--   0        0        0       82 2023-06-01 04:53:33.993483 getswish-0.2.3/.gitignore
--rw-r--r--   0        0        0      887 2023-06-02 13:20:54.296723 getswish-0.2.3/CHANGELOG.md
--rw-r--r--   0        0        0     1069 2023-06-01 04:53:33.993483 getswish-0.2.3/LICENSE
--rw-r--r--   0        0        0     5446 2023-06-01 08:01:03.944485 getswish-0.2.3/README.md
--rw-r--r--   0        0        0     1700 2023-06-01 05:43:50.553375 getswish-0.2.3/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestCertificate_1234679304.csr
--rw-r--r--   0        0        0     3247 2023-06-01 05:43:50.553375 getswish-0.2.3/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestCertificate_1234679304.key
--rw-r--r--   0        0        0     7165 2023-06-01 05:43:50.553375 getswish-0.2.3/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestCertificate_1234679304.p12
--rw-r--r--   0        0        0     6006 2023-06-01 05:43:50.553375 getswish-0.2.3/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestCertificate_1234679304.pem
--rw-r--r--   0        0        0     1700 2023-06-01 05:43:50.553375 getswish-0.2.3/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestSigningCertificate_1234679304.csr
--rw-r--r--   0        0        0     3243 2023-06-01 05:43:50.553375 getswish-0.2.3/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestSigningCertificate_1234679304.key
--rw-r--r--   0        0        0     7157 2023-06-01 05:43:50.553375 getswish-0.2.3/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestSigningCertificate_1234679304.p12
--rw-r--r--   0        0        0     6006 2023-06-01 05:43:50.553375 getswish-0.2.3/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestSigningCertificate_1234679304.pem
--rw-r--r--   0        0        0     1293 2023-06-01 05:43:50.561375 getswish-0.2.3/mss_test_1.9/Getswish_Test_Certificates/Swish_TLS_RootCA.pem
--rw-r--r--   0        0        0     1700 2023-06-01 05:43:50.561375 getswish-0.2.3/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9870474641.csr
--rw-r--r--   0        0        0     3243 2023-06-01 05:43:50.561375 getswish-0.2.3/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9870474641.key
--rw-r--r--   0        0        0     7157 2023-06-01 05:43:50.561375 getswish-0.2.3/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9870474641.p12
--rw-r--r--   0        0        0     6006 2023-06-01 05:43:50.561375 getswish-0.2.3/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9870474641.pem
--rw-r--r--   0        0        0     1752 2023-06-01 04:53:33.997484 getswish-0.2.3/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9871065216.csr
--rw-r--r--   0        0        0     3243 2023-06-01 04:53:33.997484 getswish-0.2.3/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9871065216.key
--rw-r--r--   0        0        0     7157 2023-06-01 04:53:33.997484 getswish-0.2.3/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9871065216.p12
--rw-r--r--   0        0        0     6009 2023-06-01 04:53:33.997484 getswish-0.2.3/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9871065216.pem
--rw-r--r--   0        0        0     7157 2023-06-01 05:43:50.553375 getswish-0.2.3/mss_test_1.9/Getswish_Test_Certificates/mss.p12
--rw-r--r--   0        0        0   464323 2023-06-01 05:43:50.561375 getswish-0.2.3/mss_test_1.9/MSS_UserGuide_v1.9.pdf
--rw-r--r--   0        0        0     2712 2023-06-01 05:43:50.565375 getswish-0.2.3/mss_test_1.9/readme.md
--rw-r--r--   0        0        0      312 2023-06-01 04:53:33.997484 getswish-0.2.3/noxfile.py
--rw-r--r--   0        0        0     1578 2023-06-01 05:13:56.386492 getswish-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      328 2023-06-02 13:23:52.483729 getswish-0.2.3/src/getswish/__init__.py
--rw-r--r--   0        0        0     6910 2023-06-01 08:00:02.363394 getswish-0.2.3/src/getswish/client.py
--rw-r--r--   0        0        0     1367 2023-06-01 05:56:09.109830 getswish-0.2.3/src/getswish/environments.py
--rw-r--r--   0        0        0      249 2023-06-01 04:53:33.997484 getswish-0.2.3/src/getswish/exceptions.py
--rw-r--r--   0        0        0     2914 2023-06-01 04:53:33.997484 getswish-0.2.3/src/getswish/models.py
--rw-r--r--   0        0        0     1109 2023-06-01 04:53:33.997484 getswish-0.2.3/src/getswish/utils.py
--rw-r--r--   0        0        0        0 2023-06-01 04:53:33.997484 getswish-0.2.3/tests/__init__.py
--rw-r--r--   0        0        0     5284 2023-06-01 08:28:40.092667 getswish-0.2.3/tests/fixtures.py
--rw-r--r--   0        0        0     4256 2023-06-01 08:29:34.917615 getswish-0.2.3/tests/test_client.py
--rw-r--r--   0        0        0      832 2023-06-01 04:53:34.001484 getswish-0.2.3/tests/test_exceptions.py
--rw-r--r--   0        0        0     1390 2023-06-01 04:53:34.001484 getswish-0.2.3/tests/test_models.py
--rw-r--r--   0        0        0     1695 2023-06-01 04:53:34.001484 getswish-0.2.3/tests/test_utils.py
--rw-r--r--   0        0        0     6338 1970-01-01 00:00:00.000000 getswish-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0      482 2023-06-01 04:53:33.993483 getswish-0.2.4/.github/workflows/pytest.yml
+-rw-r--r--   0        0        0       82 2023-06-01 04:53:33.993483 getswish-0.2.4/.gitignore
+-rw-r--r--   0        0        0     1067 2023-06-09 12:36:18.415229 getswish-0.2.4/CHANGELOG.md
+-rw-r--r--   0        0        0     1069 2023-06-01 04:53:33.993483 getswish-0.2.4/LICENSE
+-rw-r--r--   0        0        0     5446 2023-06-01 08:01:03.944485 getswish-0.2.4/README.md
+-rw-r--r--   0        0        0     1700 2022-09-05 11:33:53.000000 getswish-0.2.4/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestCertificate_1234679304.csr
+-rw-r--r--   0        0        0     3247 2022-09-05 11:33:53.000000 getswish-0.2.4/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestCertificate_1234679304.key
+-rw-r--r--   0        0        0     7165 2022-09-05 11:33:53.000000 getswish-0.2.4/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestCertificate_1234679304.p12
+-rw-r--r--   0        0        0     6006 2022-09-05 11:33:53.000000 getswish-0.2.4/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestCertificate_1234679304.pem
+-rw-r--r--   0        0        0     1700 2022-09-05 11:33:54.000000 getswish-0.2.4/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestSigningCertificate_1234679304.csr
+-rw-r--r--   0        0        0     3243 2022-09-05 11:33:54.000000 getswish-0.2.4/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestSigningCertificate_1234679304.key
+-rw-r--r--   0        0        0     7157 2022-09-05 11:33:53.000000 getswish-0.2.4/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestSigningCertificate_1234679304.p12
+-rw-r--r--   0        0        0     6006 2022-09-05 11:33:53.000000 getswish-0.2.4/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestSigningCertificate_1234679304.pem
+-rw-r--r--   0        0        0     1293 2023-05-29 09:37:59.000000 getswish-0.2.4/mss_test_1.9/Getswish_Test_Certificates/Swish_TLS_RootCA.pem
+-rw-r--r--   0        0        0     1700 2022-09-05 11:33:53.000000 getswish-0.2.4/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9870474641.csr
+-rw-r--r--   0        0        0     3243 2022-09-05 11:33:53.000000 getswish-0.2.4/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9870474641.key
+-rw-r--r--   0        0        0     7157 2022-09-05 11:33:53.000000 getswish-0.2.4/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9870474641.p12
+-rw-r--r--   0        0        0     6006 2022-09-05 11:33:53.000000 getswish-0.2.4/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9870474641.pem
+-rw-r--r--   0        0        0     1752 2023-06-01 04:53:33.997484 getswish-0.2.4/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9871065216.csr
+-rw-r--r--   0        0        0     3243 2023-06-01 04:53:33.997484 getswish-0.2.4/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9871065216.key
+-rw-r--r--   0        0        0     7157 2023-06-01 04:53:33.997484 getswish-0.2.4/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9871065216.p12
+-rw-r--r--   0        0        0     6009 2023-06-01 04:53:33.997484 getswish-0.2.4/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9871065216.pem
+-rw-r--r--   0        0        0     7157 2023-06-01 05:43:50.553375 getswish-0.2.4/mss_test_1.9/Getswish_Test_Certificates/mss.p12
+-rw-r--r--   0        0        0   464323 2023-06-01 05:43:50.561375 getswish-0.2.4/mss_test_1.9/MSS_UserGuide_v1.9.pdf
+-rw-r--r--   0        0        0     2849 2023-06-09 08:45:36.604212 getswish-0.2.4/mss_test_1.9/readme.md
+-rw-r--r--   0        0        0      312 2023-06-01 04:53:33.997484 getswish-0.2.4/noxfile.py
+-rw-r--r--   0        0        0     1578 2023-06-01 05:13:56.386492 getswish-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      328 2023-06-09 12:34:30.473644 getswish-0.2.4/src/getswish/__init__.py
+-rw-r--r--   0        0        0     6910 2023-06-01 08:00:02.363394 getswish-0.2.4/src/getswish/client.py
+-rw-r--r--   0        0        0     1367 2023-06-01 05:56:09.109830 getswish-0.2.4/src/getswish/environments.py
+-rw-r--r--   0        0        0      249 2023-06-01 04:53:33.997484 getswish-0.2.4/src/getswish/exceptions.py
+-rw-r--r--   0        0        0     2950 2023-06-09 12:33:23.784669 getswish-0.2.4/src/getswish/models.py
+-rw-r--r--   0        0        0     1109 2023-06-01 04:53:33.997484 getswish-0.2.4/src/getswish/utils.py
+-rw-r--r--   0        0        0        0 2023-06-01 04:53:33.997484 getswish-0.2.4/tests/__init__.py
+-rw-r--r--   0        0        0     5284 2023-06-01 08:28:40.092667 getswish-0.2.4/tests/fixtures.py
+-rw-r--r--   0        0        0     4256 2023-06-01 08:29:34.917615 getswish-0.2.4/tests/test_client.py
+-rw-r--r--   0        0        0      832 2023-06-01 04:53:34.001484 getswish-0.2.4/tests/test_exceptions.py
+-rw-r--r--   0        0        0     1390 2023-06-01 04:53:34.001484 getswish-0.2.4/tests/test_models.py
+-rw-r--r--   0        0        0     1695 2023-06-01 04:53:34.001484 getswish-0.2.4/tests/test_utils.py
+-rw-r--r--   0        0        0     6338 1970-01-01 00:00:00.000000 getswish-0.2.4/PKG-INFO
```

### Comparing `getswish-0.2.3/CHANGELOG.md` & `getswish-0.2.4/CHANGELOG.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.2.4] - 2023-06-09
+
+### Added
+
+- Added the undocumented Payout field callbackIdentifier that is
+  included when retrieving payout updates and only in production environment.
+
 ## [0.2.3] - 2023-06-02
 
 ### Added
 
 - Added logging.
 - Added nox as optional dependency.
```

### Comparing `getswish-0.2.3/LICENSE` & `getswish-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `getswish-0.2.3/README.md` & `getswish-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `getswish-0.2.3/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestCertificate_1234679304.csr` & `getswish-0.2.4/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestCertificate_1234679304.csr`

 * *Files identical despite different names*

### Comparing `getswish-0.2.3/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestCertificate_1234679304.key` & `getswish-0.2.4/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestCertificate_1234679304.key`

 * *Files identical despite different names*

### Comparing `getswish-0.2.3/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestCertificate_1234679304.p12` & `getswish-0.2.4/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestCertificate_1234679304.p12`

 * *Files identical despite different names*

### Comparing `getswish-0.2.3/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestCertificate_1234679304.pem` & `getswish-0.2.4/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestCertificate_1234679304.pem`

 * *Files identical despite different names*

### Comparing `getswish-0.2.3/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestSigningCertificate_1234679304.csr` & `getswish-0.2.4/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestSigningCertificate_1234679304.csr`

 * *Files identical despite different names*

### Comparing `getswish-0.2.3/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestSigningCertificate_1234679304.key` & `getswish-0.2.4/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestSigningCertificate_1234679304.key`

 * *Files identical despite different names*

### Comparing `getswish-0.2.3/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestSigningCertificate_1234679304.p12` & `getswish-0.2.4/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestSigningCertificate_1234679304.p12`

 * *Files identical despite different names*

### Comparing `getswish-0.2.3/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestSigningCertificate_1234679304.pem` & `getswish-0.2.4/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestSigningCertificate_1234679304.pem`

 * *Files identical despite different names*

### Comparing `getswish-0.2.3/mss_test_1.9/Getswish_Test_Certificates/Swish_TLS_RootCA.pem` & `getswish-0.2.4/mss_test_1.9/Getswish_Test_Certificates/Swish_TLS_RootCA.pem`

 * *Files identical despite different names*

### Comparing `getswish-0.2.3/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9870474641.csr` & `getswish-0.2.4/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9870474641.csr`

 * *Files identical despite different names*

### Comparing `getswish-0.2.3/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9870474641.key` & `getswish-0.2.4/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9870474641.key`

 * *Files identical despite different names*

### Comparing `getswish-0.2.3/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9870474641.p12` & `getswish-0.2.4/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9870474641.p12`

 * *Files identical despite different names*

### Comparing `getswish-0.2.3/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9870474641.pem` & `getswish-0.2.4/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9870474641.pem`

 * *Files identical despite different names*

### Comparing `getswish-0.2.3/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9871065216.csr` & `getswish-0.2.4/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9871065216.csr`

 * *Files identical despite different names*

### Comparing `getswish-0.2.3/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9871065216.key` & `getswish-0.2.4/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9871065216.key`

 * *Files identical despite different names*

### Comparing `getswish-0.2.3/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9871065216.p12` & `getswish-0.2.4/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9871065216.p12`

 * *Files identical despite different names*

### Comparing `getswish-0.2.3/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9871065216.pem` & `getswish-0.2.4/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9871065216.pem`

 * *Files identical despite different names*

### Comparing `getswish-0.2.3/mss_test_1.9/Getswish_Test_Certificates/mss.p12` & `getswish-0.2.4/mss_test_1.9/Getswish_Test_Certificates/mss.p12`

 * *Files identical despite different names*

### Comparing `getswish-0.2.3/mss_test_1.9/MSS_UserGuide_v1.9.pdf` & `getswish-0.2.4/mss_test_1.9/MSS_UserGuide_v1.9.pdf`

 * *Files identical despite different names*

### Comparing `getswish-0.2.3/mss_test_1.9/readme.md` & `getswish-0.2.4/mss_test_1.9/readme.md`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 This directory (zip-file) contains a *User Guide* on how to use the
 *Merchant Swish Simulator (MSS)* together with the test
 *authentication* certificates that are needed in order to properly
 communicate with the server. 
 Please also look at our updated documentation,
 https://developer.swish.nu/
 https://developer.swish.nu/api/mss/v1
-
+[Swish_Merchant_TestSigningCertificate_1234679304.p12](Getswish_Test_Certificates%2FSwish_Merchant_TestSigningCertificate_1234679304.p12)
 For payout requests a specific *Swish_Merchant_TestSigningCertificate*
 is provided that **must** be used to sign the payout request payload
 (create the signature property value). No other signing certificate
 will be accepted by MSS but result in error message returned to
 caller.
 
 # List of provided files #
```

### Comparing `getswish-0.2.3/pyproject.toml` & `getswish-0.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `getswish-0.2.3/src/getswish/client.py` & `getswish-0.2.4/src/getswish/client.py`

 * *Files identical despite different names*

### Comparing `getswish-0.2.3/src/getswish/environments.py` & `getswish-0.2.4/src/getswish/environments.py`

 * *Files identical despite different names*

### Comparing `getswish-0.2.3/src/getswish/models.py` & `getswish-0.2.4/src/getswish/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,14 +79,15 @@
     callback_url: str = None
     status: str = None
     date_created: str = None
     date_paid: str = None
     error_code: str = None
     error_message: str = None
     additional_information: str = None
+    callback_identifier: str = None
 
     @staticmethod
     def from_service(payout_create_object: dict) -> Payout:
         """Map service response format to local Payout class."""
 
         return Payout(**{f_name_conv(k, camel2snake, True): v for k, v in payout_create_object.items()})
```

### Comparing `getswish-0.2.3/src/getswish/utils.py` & `getswish-0.2.4/src/getswish/utils.py`

 * *Files identical despite different names*

### Comparing `getswish-0.2.3/tests/fixtures.py` & `getswish-0.2.4/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `getswish-0.2.3/tests/test_client.py` & `getswish-0.2.4/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `getswish-0.2.3/tests/test_exceptions.py` & `getswish-0.2.4/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `getswish-0.2.3/tests/test_models.py` & `getswish-0.2.4/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `getswish-0.2.3/tests/test_utils.py` & `getswish-0.2.4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `getswish-0.2.3/PKG-INFO` & `getswish-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getswish
-Version: 0.2.3
+Version: 0.2.4
 Summary: Getswish python client library
 Keywords: swish,getswish,payment,payout
 Author-email: Daniel Nibon <daniel@nibon.se>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

