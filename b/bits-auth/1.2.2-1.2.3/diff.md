# Comparing `tmp/bits-auth-1.2.2.tar.gz` & `tmp/bits-auth-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bits-auth-1.2.2.tar", last modified: Sat Apr 30 16:57:39 2022, max compression
+gzip compressed data, was "bits-auth-1.2.3.tar", last modified: Fri Jun  9 16:04:21 2023, max compression
```

## Comparing `bits-auth-1.2.2.tar` & `bits-auth-1.2.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-sr-x   0 karlsson  (1001) lukwam    (1001)        0 2022-04-30 16:57:39.000000 bits-auth-1.2.2/
--rw-r--r--   0 karlsson  (1001) lukwam    (1001)      198 2022-04-30 16:57:39.000000 bits-auth-1.2.2/PKG-INFO
--rw-r--r--   0 karlsson  (1001) lukwam    (1001)       38 2019-02-28 04:52:09.000000 bits-auth-1.2.2/README.md
-drwxr-sr-x   0 karlsson  (1001) lukwam    (1001)        0 2022-04-30 16:57:38.000000 bits-auth-1.2.2/bits/
--rw-r--r--   0 karlsson  (1001) lukwam    (1001)       89 2019-09-23 16:02:36.000000 bits-auth-1.2.2/bits/__init__.py
-drwxr-sr-x   0 karlsson  (1001) lukwam    (1001)        0 2022-04-30 16:57:38.000000 bits-auth-1.2.2/bits/auth/
--rw-r--r--   0 karlsson  (1001) lukwam    (1001)    40493 2022-04-30 16:56:57.000000 bits-auth-1.2.2/bits/auth/__init__.py
-drwxr-sr-x   0 karlsson  (1001) lukwam    (1001)        0 2022-04-30 16:57:39.000000 bits-auth-1.2.2/bits_auth.egg-info/
--rw-r--r--   0 karlsson  (1001) lukwam    (1001)      198 2022-04-30 16:57:37.000000 bits-auth-1.2.2/bits_auth.egg-info/PKG-INFO
--rw-r--r--   0 karlsson  (1001) lukwam    (1001)      263 2022-04-30 16:57:38.000000 bits-auth-1.2.2/bits_auth.egg-info/SOURCES.txt
--rw-r--r--   0 karlsson  (1001) lukwam    (1001)        1 2022-04-30 16:57:37.000000 bits-auth-1.2.2/bits_auth.egg-info/dependency_links.txt
--rw-r--r--   0 karlsson  (1001) lukwam    (1001)        1 2019-02-28 06:49:43.000000 bits-auth-1.2.2/bits_auth.egg-info/not-zip-safe
--rw-r--r--   0 karlsson  (1001) lukwam    (1001)       20 2022-04-30 16:57:38.000000 bits-auth-1.2.2/bits_auth.egg-info/requires.txt
--rw-r--r--   0 karlsson  (1001) lukwam    (1001)        5 2022-04-30 16:57:38.000000 bits-auth-1.2.2/bits_auth.egg-info/top_level.txt
--rw-r--r--   0 karlsson  (1001) lukwam    (1001)      121 2022-04-30 16:57:39.000000 bits-auth-1.2.2/setup.cfg
--rw-r--r--   0 karlsson  (1001) lukwam    (1001)     1041 2022-04-30 16:57:07.000000 bits-auth-1.2.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 16:04:21.170493 bits-auth-1.2.3/
+-rw-r--r--   0 root         (0) root         (0)      170 2023-06-09 16:04:21.171929 bits-auth-1.2.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2019-07-08 19:13:08.000000 bits-auth-1.2.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 16:04:21.099113 bits-auth-1.2.3/bits/
+-rw-r--r--   0 root         (0) root         (0)       89 2021-03-19 15:15:17.000000 bits-auth-1.2.3/bits/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 16:04:21.107076 bits-auth-1.2.3/bits/auth/
+-rw-r--r--   0 root         (0) root         (0)    40416 2023-06-09 15:51:37.000000 bits-auth-1.2.3/bits/auth/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 16:04:21.162705 bits-auth-1.2.3/bits_auth.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      170 2023-06-09 16:04:21.000000 bits-auth-1.2.3/bits_auth.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      263 2023-06-09 16:04:21.000000 bits-auth-1.2.3/bits_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 16:04:21.000000 bits-auth-1.2.3/bits_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 15:58:54.000000 bits-auth-1.2.3/bits_auth.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       20 2023-06-09 16:04:21.000000 bits-auth-1.2.3/bits_auth.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-09 16:04:21.000000 bits-auth-1.2.3/bits_auth.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      121 2023-06-09 16:04:21.177522 bits-auth-1.2.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1041 2023-06-09 15:52:26.000000 bits-auth-1.2.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `bits-auth-1.2.2/bits/auth/__init__.py` & `bits-auth-1.2.3/bits/auth/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -958,20 +958,19 @@
         params = self.secrets.resolve({
             'token': self.settings['github']['token'],
             'verbose': self.verbose,
         })
         return Travis(**params)
 
     def vast(self):
-        """Return an authenticated Vast object."""
+        """Connect to vast api."""
         from bitsapiclient.services.vast import Vast
         params = self.secrets.resolve({
             'server': self.settings['vast']['server'],
-            'username': self.settings['vast']['username'],
-            'password': self.settings['vast']['password'],
+            'api_key': self.settings['vast']['api_key'],
         })
         return Vast(**params)
 
     def vmware(self):
         """Connect to VMWare API."""
         from bitsapiclient.services.vmware import VMWare
         params = self.secrets.resolve({
```

### Comparing `bits-auth-1.2.2/setup.py` & `bits-auth-1.2.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 from setuptools import setup, find_packages
 
 
 setup(
     name='bits-auth',
 
-    version='1.2.2',
+    version='1.2.3',
 
     description='BITS Auth',
     long_description='',
 
     author='Lukas Karlsson',
     author_email='karlsson@broadinstitute.org',
```

