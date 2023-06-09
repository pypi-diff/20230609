# Comparing `tmp/rhoova-0.0.8.tar.gz` & `tmp/rhoova-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rhoova-0.0.8.tar", last modified: Wed Mar  2 15:13:13 2022, max compression
+gzip compressed data, was "rhoova-0.0.9.tar", last modified: Wed May 18 18:39:19 2022, max compression
```

## Comparing `rhoova-0.0.8.tar` & `rhoova-0.0.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
-drwxrwxrwx   0        0        0        0 2022-03-02 15:13:13.387954 rhoova-0.0.8/
--rw-rw-rw-   0        0        0      497 2022-03-02 15:13:13.388965 rhoova-0.0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-03-02 15:13:13.387954 rhoova-0.0.8/rhoova/
--rw-rw-rw-   0        0        0     6379 2022-03-02 15:12:31.961372 rhoova-0.0.8/rhoova/Client.py
--rw-rw-rw-   0        0        0        2 2021-09-08 00:04:14.071324 rhoova-0.0.8/rhoova/__init__.py
--rw-rw-rw-   0        0        0       40 2021-09-08 01:08:25.936934 rhoova-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      733 2022-03-02 15:13:02.607418 rhoova-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-05-18 18:39:19.429538 rhoova-0.0.9/
+-rw-rw-rw-   0        0        0      497 2022-05-18 18:39:19.429538 rhoova-0.0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2022-05-18 18:39:19.429538 rhoova-0.0.9/rhoova/
+-rw-rw-rw-   0        0        0     6421 2022-05-18 18:38:42.959596 rhoova-0.0.9/rhoova/Client.py
+-rw-rw-rw-   0        0        0        2 2021-09-08 00:04:14.071324 rhoova-0.0.9/rhoova/__init__.py
+-rw-rw-rw-   0        0        0       40 2021-09-08 01:08:25.936934 rhoova-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      733 2022-05-18 18:38:57.269691 rhoova-0.0.9/setup.py
```

### Comparing `rhoova-0.0.8/rhoova/Client.py` & `rhoova-0.0.9/rhoova/Client.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 
 class CalculationType(enum.Enum):
     INTEREST_RATES_SWAP = "interest_rates_swap_calculator"
     FIXED_RATE_BOND = "fixed_rate_bond"
     VANILLA_OPTION = "vanilla_option_calculator"
     YIELD_CURVE = "yield_curve_calculator"
+    FLOATING_BOND = "floating_rate_bond"
 
 
 class DataType(enum.Enum):
     YIELD_CURVE = 0
     YIELD_DATA = 1
     FIXED_RATE_BOND_DEFINITION = 2
     VANILLA_OPTION_DEFINITION = 3
```

### Comparing `rhoova-0.0.8/setup.py` & `rhoova-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 
 setup(
     name='rhoova',
     packages=['rhoova'],
-    version='0.0.8',
+    version='0.0.9',
     license='MIT',
     description='Rhoova Client',
     author='Ekinoks Software',
     author_email='ali.turan@ekinokssoftware.com',
     # url='https://github.com/user/reponame',
     # download_url='https://github.com/user/reponame/archive/v_01.tar.gz',
     keywords=['RHOOVA', 'CLIENT'],
```

