# Comparing `tmp/unicboard_billing_sdk-2.0.0.tar.gz` & `tmp/unicboard_billing_sdk-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unicboard_billing_sdk-2.0.0.tar", last modified: Fri May  5 08:54:45 2023, max compression
+gzip compressed data, was "unicboard_billing_sdk-2.0.2.tar", last modified: Fri Jun  9 09:56:13 2023, max compression
```

## Comparing `unicboard_billing_sdk-2.0.0.tar` & `unicboard_billing_sdk-2.0.2.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxr-x   0 artem9751  (1000) artem9751  (1000)        0 2023-05-05 08:54:45.766350 unicboard_billing_sdk-2.0.0/
--rw-rw-r--   0 artem9751  (1000) artem9751  (1000)     1062 2022-05-19 07:26:17.000000 unicboard_billing_sdk-2.0.0/LICENSE
--rw-rw-r--   0 artem9751  (1000) artem9751  (1000)     1571 2023-05-05 08:54:45.766350 unicboard_billing_sdk-2.0.0/PKG-INFO
--rw-rw-r--   0 artem9751  (1000) artem9751  (1000)      895 2023-03-30 09:19:40.000000 unicboard_billing_sdk-2.0.0/README.md
--rw-rw-r--   0 artem9751  (1000) artem9751  (1000)       38 2023-05-05 08:54:45.766350 unicboard_billing_sdk-2.0.0/setup.cfg
--rw-rw-r--   0 artem9751  (1000) artem9751  (1000)     1149 2023-05-05 08:53:56.000000 unicboard_billing_sdk-2.0.0/setup.py
-drwxrwxr-x   0 artem9751  (1000) artem9751  (1000)        0 2023-05-05 08:54:45.766350 unicboard_billing_sdk-2.0.0/unicboard_billing_sdk/
--rw-rw-r--   0 artem9751  (1000) artem9751  (1000)      100 2023-05-05 05:52:15.000000 unicboard_billing_sdk-2.0.0/unicboard_billing_sdk/__init__.py
--rw-rw-r--   0 artem9751  (1000) artem9751  (1000)     9415 2023-05-05 08:51:19.000000 unicboard_billing_sdk-2.0.0/unicboard_billing_sdk/billing_api_sdk.py
--rw-rw-r--   0 artem9751  (1000) artem9751  (1000)    12170 2023-05-05 08:51:19.000000 unicboard_billing_sdk-2.0.0/unicboard_billing_sdk/response_models.py
--rw-rw-r--   0 artem9751  (1000) artem9751  (1000)     6939 2023-05-05 08:51:19.000000 unicboard_billing_sdk-2.0.0/unicboard_billing_sdk/utils.py
-drwxrwxr-x   0 artem9751  (1000) artem9751  (1000)        0 2023-05-05 08:54:45.766350 unicboard_billing_sdk-2.0.0/unicboard_billing_sdk.egg-info/
--rw-rw-r--   0 artem9751  (1000) artem9751  (1000)     1571 2023-05-05 08:54:45.000000 unicboard_billing_sdk-2.0.0/unicboard_billing_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 artem9751  (1000) artem9751  (1000)      397 2023-05-05 08:54:45.000000 unicboard_billing_sdk-2.0.0/unicboard_billing_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 artem9751  (1000) artem9751  (1000)        1 2023-05-05 08:54:45.000000 unicboard_billing_sdk-2.0.0/unicboard_billing_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 artem9751  (1000) artem9751  (1000)       17 2023-05-05 08:54:45.000000 unicboard_billing_sdk-2.0.0/unicboard_billing_sdk.egg-info/requires.txt
--rw-rw-r--   0 artem9751  (1000) artem9751  (1000)       22 2023-05-05 08:54:45.000000 unicboard_billing_sdk-2.0.0/unicboard_billing_sdk.egg-info/top_level.txt
+drwxrwxr-x   0 artem9751  (1000) artem9751  (1000)        0 2023-06-09 09:56:13.932268 unicboard_billing_sdk-2.0.2/
+-rw-rw-r--   0 artem9751  (1000) artem9751  (1000)     1062 2023-06-09 09:52:16.000000 unicboard_billing_sdk-2.0.2/LICENSE
+-rw-rw-r--   0 artem9751  (1000) artem9751  (1000)    50177 2023-06-09 09:56:13.932268 unicboard_billing_sdk-2.0.2/PKG-INFO
+-rw-rw-r--   0 artem9751  (1000) artem9751  (1000)    49501 2023-06-09 09:52:16.000000 unicboard_billing_sdk-2.0.2/README.md
+-rw-rw-r--   0 artem9751  (1000) artem9751  (1000)       38 2023-06-09 09:56:13.932268 unicboard_billing_sdk-2.0.2/setup.cfg
+-rw-rw-r--   0 artem9751  (1000) artem9751  (1000)     1149 2023-06-09 09:53:37.000000 unicboard_billing_sdk-2.0.2/setup.py
+drwxrwxr-x   0 artem9751  (1000) artem9751  (1000)        0 2023-06-09 09:56:13.932268 unicboard_billing_sdk-2.0.2/unicboard_billing_sdk/
+-rw-rw-r--   0 artem9751  (1000) artem9751  (1000)      100 2023-06-09 09:52:16.000000 unicboard_billing_sdk-2.0.2/unicboard_billing_sdk/__init__.py
+-rw-rw-r--   0 artem9751  (1000) artem9751  (1000)    12231 2023-06-09 09:53:37.000000 unicboard_billing_sdk-2.0.2/unicboard_billing_sdk/billing_api_sdk.py
+-rw-rw-r--   0 artem9751  (1000) artem9751  (1000)      140 2023-06-09 09:53:37.000000 unicboard_billing_sdk-2.0.2/unicboard_billing_sdk/constants.py
+-rw-rw-r--   0 artem9751  (1000) artem9751  (1000)    12170 2023-06-09 09:52:16.000000 unicboard_billing_sdk-2.0.2/unicboard_billing_sdk/response_models.py
+-rw-rw-r--   0 artem9751  (1000) artem9751  (1000)     6939 2023-06-09 09:52:16.000000 unicboard_billing_sdk-2.0.2/unicboard_billing_sdk/utils.py
+drwxrwxr-x   0 artem9751  (1000) artem9751  (1000)        0 2023-06-09 09:56:13.932268 unicboard_billing_sdk-2.0.2/unicboard_billing_sdk.egg-info/
+-rw-rw-r--   0 artem9751  (1000) artem9751  (1000)    50177 2023-06-09 09:56:13.000000 unicboard_billing_sdk-2.0.2/unicboard_billing_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 artem9751  (1000) artem9751  (1000)      432 2023-06-09 09:56:13.000000 unicboard_billing_sdk-2.0.2/unicboard_billing_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 artem9751  (1000) artem9751  (1000)        1 2023-06-09 09:56:13.000000 unicboard_billing_sdk-2.0.2/unicboard_billing_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 artem9751  (1000) artem9751  (1000)       17 2023-06-09 09:56:13.000000 unicboard_billing_sdk-2.0.2/unicboard_billing_sdk.egg-info/requires.txt
+-rw-rw-r--   0 artem9751  (1000) artem9751  (1000)       22 2023-06-09 09:56:13.000000 unicboard_billing_sdk-2.0.2/unicboard_billing_sdk.egg-info/top_level.txt
```

### Comparing `unicboard_billing_sdk-2.0.0/LICENSE` & `unicboard_billing_sdk-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `unicboard_billing_sdk-2.0.0/setup.py` & `unicboard_billing_sdk-2.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 
 setup(
     name='unicboard_billing_sdk',
-    version='2.0.0',
+    version='2.0.2',
     description='Unicboard billing api',
     author='Unic-lab',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author_email='a.brilon@unic-lab.by',
     url='https://github.com/uniclab-01/billing-api',
     package_data={'': ['*.yml'], },
```

### Comparing `unicboard_billing_sdk-2.0.0/unicboard_billing_sdk/response_models.py` & `unicboard_billing_sdk-2.0.2/unicboard_billing_sdk/response_models.py`

 * *Files identical despite different names*

### Comparing `unicboard_billing_sdk-2.0.0/unicboard_billing_sdk/utils.py` & `unicboard_billing_sdk-2.0.2/unicboard_billing_sdk/utils.py`

 * *Files identical despite different names*

