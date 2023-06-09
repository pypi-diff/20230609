# Comparing `tmp/cf_clearance-0.29.1.tar.gz` & `tmp/cf_clearance-0.29.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cf_clearance-0.29.1.tar", last modified: Wed Jun  7 07:16:06 2023, max compression
+gzip compressed data, was "cf_clearance-0.29.2.tar", last modified: Fri Jun  9 04:16:31 2023, max compression
```

## Comparing `cf_clearance-0.29.1.tar` & `cf_clearance-0.29.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    11357 2022-05-30 06:44:14.187456 cf_clearance-0.29.1/LICENSE
--rw-r--r--   0        0        0     5689 2023-06-05 08:24:29.062628 cf_clearance-0.29.1/README.md
--rw-r--r--   0        0        0     6148 2022-05-30 06:47:41.987971 cf_clearance-0.29.1/cf_clearance/.DS_Store
--rw-r--r--   0        0        0      281 2023-06-07 07:14:13.027584 cf_clearance-0.29.1/cf_clearance/__init__.py
--rw-r--r--   0        0        0      118 2022-11-28 03:39:27.925358 cf_clearance-0.29.1/cf_clearance/errors.py
--rw-r--r--   0        0        0     1268 2022-11-28 03:39:27.925709 cf_clearance-0.29.1/cf_clearance/js/canvas.fingerprinting.js
--rw-r--r--   0        0        0     1846 2022-11-28 03:39:27.926018 cf_clearance-0.29.1/cf_clearance/js/chrome.global.js
--rw-r--r--   0        0        0     5662 2023-02-24 07:20:56.351353 cf_clearance-0.29.1/cf_clearance/js/chrome.plugin.js
--rw-r--r--   0        0        0     3575 2022-11-23 06:25:21.108178 cf_clearance-0.29.1/cf_clearance/js/chrome.runtime.js
--rw-r--r--   0        0        0       74 2022-11-28 03:39:27.926735 cf_clearance-0.29.1/cf_clearance/js/emulate.touch.js
--rw-r--r--   0        0        0     1083 2022-11-28 03:39:27.927066 cf_clearance-0.29.1/cf_clearance/js/navigator.permissions.js
--rw-r--r--   0        0        0      489 2022-12-07 10:09:49.695721 cf_clearance-0.29.1/cf_clearance/js/navigator.webdriver.js
--rw-r--r--   0        0        0     2058 2023-06-07 06:30:31.817778 cf_clearance-0.29.1/cf_clearance/retry.py
--rw-r--r--   0        0        0     3678 2022-11-28 03:39:27.927929 cf_clearance-0.29.1/cf_clearance/stealth.py
--rw-r--r--   0        0        0      772 2023-06-07 07:16:06.551887 cf_clearance-0.29.1/pyproject.toml
--rw-r--r--   0        0        0        0 2021-12-05 15:24:48.652965 cf_clearance-0.29.1/tests/__init__.py
--rw-r--r--   0        0        0     1805 2022-11-28 03:39:27.928856 cf_clearance-0.29.1/tests/test_async_cf.py
--rw-r--r--   0        0        0      715 2023-04-17 13:57:16.483813 cf_clearance-0.29.1/tests/test_common.py
--rw-r--r--   0        0        0      838 2023-06-07 04:12:39.890891 cf_clearance-0.29.1/tests/test_cron_challenge.py
--rw-r--r--   0        0        0     1660 2022-11-28 03:39:27.929569 cf_clearance-0.29.1/tests/test_sync_cf.py
--rw-r--r--   0        0        0     6248 1970-01-01 00:00:00.000000 cf_clearance-0.29.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-05-30 06:44:14.187456 cf_clearance-0.29.2/LICENSE
+-rw-r--r--   0        0        0     5689 2023-06-07 07:53:29.051659 cf_clearance-0.29.2/README.md
+-rw-r--r--   0        0        0     6148 2022-05-30 06:47:41.987971 cf_clearance-0.29.2/cf_clearance/.DS_Store
+-rw-r--r--   0        0        0      281 2023-06-09 04:15:48.860878 cf_clearance-0.29.2/cf_clearance/__init__.py
+-rw-r--r--   0        0        0      118 2023-06-07 07:53:29.052052 cf_clearance-0.29.2/cf_clearance/errors.py
+-rw-r--r--   0        0        0     1268 2023-06-07 07:53:29.052342 cf_clearance-0.29.2/cf_clearance/js/canvas.fingerprinting.js
+-rw-r--r--   0        0        0     1846 2023-06-07 07:53:29.052624 cf_clearance-0.29.2/cf_clearance/js/chrome.global.js
+-rw-r--r--   0        0        0     5662 2023-06-07 07:53:29.052917 cf_clearance-0.29.2/cf_clearance/js/chrome.plugin.js
+-rw-r--r--   0        0        0     3575 2022-11-23 06:25:21.108178 cf_clearance-0.29.2/cf_clearance/js/chrome.runtime.js
+-rw-r--r--   0        0        0       74 2023-06-07 07:53:29.053074 cf_clearance-0.29.2/cf_clearance/js/emulate.touch.js
+-rw-r--r--   0        0        0     1083 2023-06-07 07:53:29.053302 cf_clearance-0.29.2/cf_clearance/js/navigator.permissions.js
+-rw-r--r--   0        0        0      489 2023-06-07 07:53:29.053552 cf_clearance-0.29.2/cf_clearance/js/navigator.webdriver.js
+-rw-r--r--   0        0        0     2058 2023-06-07 07:53:29.053700 cf_clearance-0.29.2/cf_clearance/retry.py
+-rw-r--r--   0        0        0     3678 2023-06-07 07:53:29.053841 cf_clearance-0.29.2/cf_clearance/stealth.py
+-rw-r--r--   0        0        0     1060 2023-06-09 04:16:31.938178 cf_clearance-0.29.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2021-12-05 15:24:48.652965 cf_clearance-0.29.2/tests/__init__.py
+-rw-r--r--   0        0        0     1805 2023-06-07 07:53:29.055046 cf_clearance-0.29.2/tests/test_async_cf.py
+-rw-r--r--   0        0        0      715 2023-06-07 07:53:29.055195 cf_clearance-0.29.2/tests/test_common.py
+-rw-r--r--   0        0        0      838 2023-06-07 07:53:29.055295 cf_clearance-0.29.2/tests/test_cron_challenge.py
+-rw-r--r--   0        0        0     1660 2023-06-07 07:53:29.055526 cf_clearance-0.29.2/tests/test_sync_cf.py
+-rw-r--r--   0        0        0     6548 1970-01-01 00:00:00.000000 cf_clearance-0.29.2/PKG-INFO
```

### Comparing `cf_clearance-0.29.1/LICENSE` & `cf_clearance-0.29.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cf_clearance-0.29.1/README.md` & `cf_clearance-0.29.2/README.md`

 * *Files identical despite different names*

### Comparing `cf_clearance-0.29.1/cf_clearance/.DS_Store` & `cf_clearance-0.29.2/cf_clearance/.DS_Store`

 * *Files identical despite different names*

### Comparing `cf_clearance-0.29.1/cf_clearance/js/canvas.fingerprinting.js` & `cf_clearance-0.29.2/cf_clearance/js/canvas.fingerprinting.js`

 * *Files identical despite different names*

### Comparing `cf_clearance-0.29.1/cf_clearance/js/chrome.global.js` & `cf_clearance-0.29.2/cf_clearance/js/chrome.global.js`

 * *Files identical despite different names*

### Comparing `cf_clearance-0.29.1/cf_clearance/js/chrome.plugin.js` & `cf_clearance-0.29.2/cf_clearance/js/chrome.plugin.js`

 * *Files identical despite different names*

### Comparing `cf_clearance-0.29.1/cf_clearance/js/chrome.runtime.js` & `cf_clearance-0.29.2/cf_clearance/js/chrome.runtime.js`

 * *Files identical despite different names*

### Comparing `cf_clearance-0.29.1/cf_clearance/js/navigator.permissions.js` & `cf_clearance-0.29.2/cf_clearance/js/navigator.permissions.js`

 * *Files identical despite different names*

### Comparing `cf_clearance-0.29.1/cf_clearance/retry.py` & `cf_clearance-0.29.2/cf_clearance/retry.py`

 * *Files identical despite different names*

### Comparing `cf_clearance-0.29.1/cf_clearance/stealth.py` & `cf_clearance-0.29.2/cf_clearance/stealth.py`

 * *Files identical despite different names*

### Comparing `cf_clearance-0.29.1/tests/test_async_cf.py` & `cf_clearance-0.29.2/tests/test_async_cf.py`

 * *Files identical despite different names*

### Comparing `cf_clearance-0.29.1/tests/test_common.py` & `cf_clearance-0.29.2/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `cf_clearance-0.29.1/tests/test_cron_challenge.py` & `cf_clearance-0.29.2/tests/test_cron_challenge.py`

 * *Files identical despite different names*

### Comparing `cf_clearance-0.29.1/tests/test_sync_cf.py` & `cf_clearance-0.29.2/tests/test_sync_cf.py`

 * *Files identical despite different names*

### Comparing `cf_clearance-0.29.1/PKG-INFO` & `cf_clearance-0.29.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 Metadata-Version: 2.1
 Name: cf-clearance
-Version: 0.29.1
+Version: 0.29.2
 Summary: Purpose To make a cloudflare v2 challenge pass successfully, Can be use cf_clearance bypassed by cloudflare, However, with the cf_clearance, make sure you use the same IP and UA as when you got it.
 Author-Email: vvanglro <vvanglro@gmail.com>
 License: Apache-2.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Project-URL: Homepage, https://github.com/vvanglro/cf_clearance
 Project-URL: Repository, https://github.com/vvanglro/cf_clearance
 Requires-Python: <4,>=3.7
 Requires-Dist: playwright>=1.34.0
 Description-Content-Type: text/markdown
 
 # cf-clearance
```

