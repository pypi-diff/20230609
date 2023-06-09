# Comparing `tmp/Supplier API tester-2.0.3.tar.gz` & `tmp/Supplier API tester-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/supplier-api/supplier-api/supplier_api_tester/dist/.tmp-eiv8kbyn/Supplier API tester-2.0.3.tar", last modified: Wed Apr  5 13:41:08 2023, max compression
+gzip compressed data, was "/home/runner/work/supplier-api/supplier-api/supplier_api_tester/dist/.tmp-00fo2k8q/Supplier API tester-2.0.4.tar", last modified: Fri Jun  9 10:16:08 2023, max compression
```

## Comparing `Supplier API tester-2.0.3.tar` & `Supplier API tester-2.0.4.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:41:08.000000 Supplier API tester-2.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     7563 2023-04-05 13:41:08.000000 Supplier API tester-2.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7071 2023-04-05 13:40:58.000000 Supplier API tester-2.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:41:08.000000 Supplier API tester-2.0.3/Supplier_API_tester.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7563 2023-04-05 13:41:08.000000 Supplier API tester-2.0.3/Supplier_API_tester.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-04-05 13:41:08.000000 Supplier API tester-2.0.3/Supplier_API_tester.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 13:41:08.000000 Supplier API tester-2.0.3/Supplier_API_tester.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-05 13:41:08.000000 Supplier API tester-2.0.3/Supplier_API_tester.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-05 13:41:08.000000 Supplier API tester-2.0.3/Supplier_API_tester.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-05 13:41:08.000000 Supplier API tester-2.0.3/Supplier_API_tester.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-05 13:40:58.000000 Supplier API tester-2.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-05 13:41:08.000000 Supplier API tester-2.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-05 13:40:58.000000 Supplier API tester-2.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:41:08.000000 Supplier API tester-2.0.3/supplier_api_tester/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 13:40:58.000000 Supplier API tester-2.0.3/supplier_api_tester/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-04-05 13:40:58.000000 Supplier API tester-2.0.3/supplier_api_tester/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:41:08.000000 Supplier API tester-2.0.3/supplier_api_tester/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 13:40:58.000000 Supplier API tester-2.0.3/supplier_api_tester/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-04-05 13:40:58.000000 Supplier API tester-2.0.3/supplier_api_tester/v1/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-04-05 13:40:58.000000 Supplier API tester-2.0.3/supplier_api_tester/v1/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-04-05 13:40:58.000000 Supplier API tester-2.0.3/supplier_api_tester/v1/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-05 13:40:58.000000 Supplier API tester-2.0.3/supplier_api_tester/v1/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-05 13:40:58.000000 Supplier API tester-2.0.3/supplier_api_tester/v1/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-04-05 13:40:58.000000 Supplier API tester-2.0.3/supplier_api_tester/v1/printer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-04-05 13:40:58.000000 Supplier API tester-2.0.3/supplier_api_tester/v1/tester.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:41:08.000000 Supplier API tester-2.0.3/supplier_api_tester/v1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-04-05 13:40:58.000000 Supplier API tester-2.0.3/supplier_api_tester/v1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5892 2023-04-05 13:40:58.000000 Supplier API tester-2.0.3/supplier_api_tester/v1/tests/availability_timeslots.py
--rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-04-05 13:40:58.000000 Supplier API tester-2.0.3/supplier_api_tester/v1/tests/availability_variants.py
--rw-r--r--   0 runner    (1001) docker     (123)    10679 2023-04-05 13:40:58.000000 Supplier API tester-2.0.3/supplier_api_tester/v1/tests/booking.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-04-05 13:40:58.000000 Supplier API tester-2.0.3/supplier_api_tester/v1/tests/product_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     9280 2023-04-05 13:40:58.000000 Supplier API tester-2.0.3/supplier_api_tester/v1/tests/reservation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:41:08.000000 Supplier API tester-2.0.3/supplier_api_tester/v1/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 13:40:58.000000 Supplier API tester-2.0.3/supplier_api_tester/v1/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7983 2023-04-05 13:40:58.000000 Supplier API tester-2.0.3/supplier_api_tester/v1/utils/adapters.py
--rw-r--r--   0 runner    (1001) docker     (123)    12061 2023-04-05 13:40:58.000000 Supplier API tester-2.0.3/supplier_api_tester/v1/utils/availability.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-05 13:40:58.000000 Supplier API tester-2.0.3/supplier_api_tester/v1/utils/conversions.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-05 13:40:58.000000 Supplier API tester-2.0.3/supplier_api_tester/v1/utils/date.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-04-05 13:40:58.000000 Supplier API tester-2.0.3/supplier_api_tester/v1/utils/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-04-05 13:40:58.000000 Supplier API tester-2.0.3/supplier_api_tester/v1/utils/reservation.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-05 13:40:58.000000 Supplier API tester-2.0.3/supplier_api_tester/v1/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:41:08.000000 Supplier API tester-2.0.3/supplier_api_tester/v2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 13:40:58.000000 Supplier API tester-2.0.3/supplier_api_tester/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-04-05 13:40:58.000000 Supplier API tester-2.0.3/supplier_api_tester/v2/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-04-05 13:40:58.000000 Supplier API tester-2.0.3/supplier_api_tester/v2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-04-05 13:40:58.000000 Supplier API tester-2.0.3/supplier_api_tester/v2/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-05 13:40:58.000000 Supplier API tester-2.0.3/supplier_api_tester/v2/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-04-05 13:40:58.000000 Supplier API tester-2.0.3/supplier_api_tester/v2/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-04-05 13:40:58.000000 Supplier API tester-2.0.3/supplier_api_tester/v2/printer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-05 13:40:58.000000 Supplier API tester-2.0.3/supplier_api_tester/v2/tester.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:41:08.000000 Supplier API tester-2.0.3/supplier_api_tester/v2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-04-05 13:40:58.000000 Supplier API tester-2.0.3/supplier_api_tester/v2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-04-05 13:40:58.000000 Supplier API tester-2.0.3/supplier_api_tester/v2/tests/availability_variants.py
--rw-r--r--   0 runner    (1001) docker     (123)    10477 2023-04-05 13:40:58.000000 Supplier API tester-2.0.3/supplier_api_tester/v2/tests/booking.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-05 13:40:58.000000 Supplier API tester-2.0.3/supplier_api_tester/v2/tests/product_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-04-05 13:40:58.000000 Supplier API tester-2.0.3/supplier_api_tester/v2/tests/reservation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:41:08.000000 Supplier API tester-2.0.3/supplier_api_tester/v2/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 13:40:58.000000 Supplier API tester-2.0.3/supplier_api_tester/v2/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7751 2023-04-05 13:40:58.000000 Supplier API tester-2.0.3/supplier_api_tester/v2/utils/adapters.py
--rw-r--r--   0 runner    (1001) docker     (123)    11085 2023-04-05 13:40:58.000000 Supplier API tester-2.0.3/supplier_api_tester/v2/utils/availability.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-05 13:40:58.000000 Supplier API tester-2.0.3/supplier_api_tester/v2/utils/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-05 13:40:58.000000 Supplier API tester-2.0.3/supplier_api_tester/v2/utils/conversions.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-05 13:40:58.000000 Supplier API tester-2.0.3/supplier_api_tester/v2/utils/date.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-05 13:40:58.000000 Supplier API tester-2.0.3/supplier_api_tester/v2/utils/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-04-05 13:40:58.000000 Supplier API tester-2.0.3/supplier_api_tester/v2/utils/reservation.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-05 13:40:58.000000 Supplier API tester-2.0.3/supplier_api_tester/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:16:08.000000 Supplier API tester-2.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     7563 2023-06-09 10:16:08.000000 Supplier API tester-2.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7071 2023-06-09 10:15:56.000000 Supplier API tester-2.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:16:08.000000 Supplier API tester-2.0.4/Supplier_API_tester.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7563 2023-06-09 10:16:08.000000 Supplier API tester-2.0.4/Supplier_API_tester.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-06-09 10:16:08.000000 Supplier API tester-2.0.4/Supplier_API_tester.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 10:16:08.000000 Supplier API tester-2.0.4/Supplier_API_tester.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-09 10:16:08.000000 Supplier API tester-2.0.4/Supplier_API_tester.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-09 10:16:08.000000 Supplier API tester-2.0.4/Supplier_API_tester.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-09 10:16:08.000000 Supplier API tester-2.0.4/Supplier_API_tester.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-09 10:15:56.000000 Supplier API tester-2.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-09 10:16:08.000000 Supplier API tester-2.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-09 10:15:56.000000 Supplier API tester-2.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:16:08.000000 Supplier API tester-2.0.4/supplier_api_tester/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 10:15:56.000000 Supplier API tester-2.0.4/supplier_api_tester/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-06-09 10:15:56.000000 Supplier API tester-2.0.4/supplier_api_tester/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:16:08.000000 Supplier API tester-2.0.4/supplier_api_tester/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 10:15:56.000000 Supplier API tester-2.0.4/supplier_api_tester/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-06-09 10:15:56.000000 Supplier API tester-2.0.4/supplier_api_tester/v1/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-06-09 10:15:56.000000 Supplier API tester-2.0.4/supplier_api_tester/v1/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-06-09 10:15:56.000000 Supplier API tester-2.0.4/supplier_api_tester/v1/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-09 10:15:56.000000 Supplier API tester-2.0.4/supplier_api_tester/v1/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-09 10:15:56.000000 Supplier API tester-2.0.4/supplier_api_tester/v1/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-06-09 10:15:56.000000 Supplier API tester-2.0.4/supplier_api_tester/v1/printer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-09 10:15:56.000000 Supplier API tester-2.0.4/supplier_api_tester/v1/tester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:16:08.000000 Supplier API tester-2.0.4/supplier_api_tester/v1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-06-09 10:15:56.000000 Supplier API tester-2.0.4/supplier_api_tester/v1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5892 2023-06-09 10:15:56.000000 Supplier API tester-2.0.4/supplier_api_tester/v1/tests/availability_timeslots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-06-09 10:15:56.000000 Supplier API tester-2.0.4/supplier_api_tester/v1/tests/availability_variants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10679 2023-06-09 10:15:56.000000 Supplier API tester-2.0.4/supplier_api_tester/v1/tests/booking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-06-09 10:15:56.000000 Supplier API tester-2.0.4/supplier_api_tester/v1/tests/product_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9280 2023-06-09 10:15:56.000000 Supplier API tester-2.0.4/supplier_api_tester/v1/tests/reservation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:16:08.000000 Supplier API tester-2.0.4/supplier_api_tester/v1/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 10:15:56.000000 Supplier API tester-2.0.4/supplier_api_tester/v1/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7983 2023-06-09 10:15:56.000000 Supplier API tester-2.0.4/supplier_api_tester/v1/utils/adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12061 2023-06-09 10:15:56.000000 Supplier API tester-2.0.4/supplier_api_tester/v1/utils/availability.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-09 10:15:56.000000 Supplier API tester-2.0.4/supplier_api_tester/v1/utils/conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-09 10:15:56.000000 Supplier API tester-2.0.4/supplier_api_tester/v1/utils/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-09 10:15:56.000000 Supplier API tester-2.0.4/supplier_api_tester/v1/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-06-09 10:15:56.000000 Supplier API tester-2.0.4/supplier_api_tester/v1/utils/reservation.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-09 10:15:56.000000 Supplier API tester-2.0.4/supplier_api_tester/v1/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:16:08.000000 Supplier API tester-2.0.4/supplier_api_tester/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 10:15:56.000000 Supplier API tester-2.0.4/supplier_api_tester/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-06-09 10:15:56.000000 Supplier API tester-2.0.4/supplier_api_tester/v2/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-06-09 10:15:56.000000 Supplier API tester-2.0.4/supplier_api_tester/v2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-06-09 10:15:56.000000 Supplier API tester-2.0.4/supplier_api_tester/v2/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-09 10:15:56.000000 Supplier API tester-2.0.4/supplier_api_tester/v2/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-06-09 10:15:56.000000 Supplier API tester-2.0.4/supplier_api_tester/v2/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-06-09 10:15:56.000000 Supplier API tester-2.0.4/supplier_api_tester/v2/printer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-09 10:15:56.000000 Supplier API tester-2.0.4/supplier_api_tester/v2/tester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:16:08.000000 Supplier API tester-2.0.4/supplier_api_tester/v2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-09 10:15:56.000000 Supplier API tester-2.0.4/supplier_api_tester/v2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-06-09 10:15:56.000000 Supplier API tester-2.0.4/supplier_api_tester/v2/tests/availability_variants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10477 2023-06-09 10:15:56.000000 Supplier API tester-2.0.4/supplier_api_tester/v2/tests/booking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-09 10:15:56.000000 Supplier API tester-2.0.4/supplier_api_tester/v2/tests/product_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-06-09 10:15:56.000000 Supplier API tester-2.0.4/supplier_api_tester/v2/tests/reservation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:16:08.000000 Supplier API tester-2.0.4/supplier_api_tester/v2/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 10:15:56.000000 Supplier API tester-2.0.4/supplier_api_tester/v2/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-06-09 10:15:56.000000 Supplier API tester-2.0.4/supplier_api_tester/v2/utils/adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11085 2023-06-09 10:15:56.000000 Supplier API tester-2.0.4/supplier_api_tester/v2/utils/availability.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-09 10:15:56.000000 Supplier API tester-2.0.4/supplier_api_tester/v2/utils/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-09 10:15:56.000000 Supplier API tester-2.0.4/supplier_api_tester/v2/utils/conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-09 10:15:56.000000 Supplier API tester-2.0.4/supplier_api_tester/v2/utils/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-06-09 10:15:56.000000 Supplier API tester-2.0.4/supplier_api_tester/v2/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-06-09 10:15:56.000000 Supplier API tester-2.0.4/supplier_api_tester/v2/utils/reservation.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-09 10:15:56.000000 Supplier API tester-2.0.4/supplier_api_tester/version.py
```

### Comparing `Supplier API tester-2.0.3/PKG-INFO` & `Supplier API tester-2.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Supplier API tester
-Version: 2.0.3
+Version: 2.0.4
 Summary: Console tool for validating the Supplier API implementation
 Author: Tiqets Team
 Author-email: connections@tiqets.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Supplier API tester-2.0.3/README.md` & `Supplier API tester-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `Supplier API tester-2.0.3/Supplier_API_tester.egg-info/PKG-INFO` & `Supplier API tester-2.0.4/Supplier_API_tester.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Supplier-API-tester
-Version: 2.0.3
+Version: 2.0.4
 Summary: Console tool for validating the Supplier API implementation
 Author: Tiqets Team
 Author-email: connections@tiqets.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Supplier API tester-2.0.3/Supplier_API_tester.egg-info/SOURCES.txt` & `Supplier API tester-2.0.4/Supplier_API_tester.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Supplier API tester-2.0.3/setup.py` & `Supplier API tester-2.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `Supplier API tester-2.0.3/supplier_api_tester/cli.py` & `Supplier API tester-2.0.4/supplier_api_tester/cli.py`

 * *Files identical despite different names*

### Comparing `Supplier API tester-2.0.3/supplier_api_tester/v1/cli.py` & `Supplier API tester-2.0.4/supplier_api_tester/v1/cli.py`

 * *Files identical despite different names*

### Comparing `Supplier API tester-2.0.3/supplier_api_tester/v1/client.py` & `Supplier API tester-2.0.4/supplier_api_tester/v1/client.py`

 * *Files identical despite different names*

### Comparing `Supplier API tester-2.0.3/supplier_api_tester/v1/decorators.py` & `Supplier API tester-2.0.4/supplier_api_tester/v1/decorators.py`

 * *Files identical despite different names*

### Comparing `Supplier API tester-2.0.3/supplier_api_tester/v1/models.py` & `Supplier API tester-2.0.4/supplier_api_tester/v1/models.py`

 * *Files identical despite different names*

### Comparing `Supplier API tester-2.0.3/supplier_api_tester/v1/printer.py` & `Supplier API tester-2.0.4/supplier_api_tester/v1/printer.py`

 * *Files identical despite different names*

### Comparing `Supplier API tester-2.0.3/supplier_api_tester/v1/tester.py` & `Supplier API tester-2.0.4/supplier_api_tester/v1/tester.py`

 * *Files identical despite different names*

### Comparing `Supplier API tester-2.0.3/supplier_api_tester/v1/tests/__init__.py` & `Supplier API tester-2.0.4/supplier_api_tester/v1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Supplier API tester-2.0.3/supplier_api_tester/v1/tests/availability_timeslots.py` & `Supplier API tester-2.0.4/supplier_api_tester/v1/tests/availability_timeslots.py`

 * *Files identical despite different names*

### Comparing `Supplier API tester-2.0.3/supplier_api_tester/v1/tests/availability_variants.py` & `Supplier API tester-2.0.4/supplier_api_tester/v1/tests/availability_variants.py`

 * *Files identical despite different names*

### Comparing `Supplier API tester-2.0.3/supplier_api_tester/v1/tests/booking.py` & `Supplier API tester-2.0.4/supplier_api_tester/v1/tests/booking.py`

 * *Files identical despite different names*

### Comparing `Supplier API tester-2.0.3/supplier_api_tester/v1/tests/product_catalog.py` & `Supplier API tester-2.0.4/supplier_api_tester/v1/tests/product_catalog.py`

 * *Files identical despite different names*

### Comparing `Supplier API tester-2.0.3/supplier_api_tester/v1/tests/reservation.py` & `Supplier API tester-2.0.4/supplier_api_tester/v1/tests/reservation.py`

 * *Files identical despite different names*

### Comparing `Supplier API tester-2.0.3/supplier_api_tester/v1/utils/adapters.py` & `Supplier API tester-2.0.4/supplier_api_tester/v1/utils/adapters.py`

 * *Files identical despite different names*

### Comparing `Supplier API tester-2.0.3/supplier_api_tester/v1/utils/availability.py` & `Supplier API tester-2.0.4/supplier_api_tester/v1/utils/availability.py`

 * *Files identical despite different names*

### Comparing `Supplier API tester-2.0.3/supplier_api_tester/v1/utils/errors.py` & `Supplier API tester-2.0.4/supplier_api_tester/v1/utils/errors.py`

 * *Files identical despite different names*

### Comparing `Supplier API tester-2.0.3/supplier_api_tester/v1/utils/reservation.py` & `Supplier API tester-2.0.4/supplier_api_tester/v1/utils/reservation.py`

 * *Files identical despite different names*

### Comparing `Supplier API tester-2.0.3/supplier_api_tester/v2/cli.py` & `Supplier API tester-2.0.4/supplier_api_tester/v2/cli.py`

 * *Files identical despite different names*

### Comparing `Supplier API tester-2.0.3/supplier_api_tester/v2/client.py` & `Supplier API tester-2.0.4/supplier_api_tester/v2/client.py`

 * *Files identical despite different names*

### Comparing `Supplier API tester-2.0.3/supplier_api_tester/v2/decorators.py` & `Supplier API tester-2.0.4/supplier_api_tester/v2/decorators.py`

 * *Files identical despite different names*

### Comparing `Supplier API tester-2.0.3/supplier_api_tester/v2/models.py` & `Supplier API tester-2.0.4/supplier_api_tester/v2/models.py`

 * *Files identical despite different names*

### Comparing `Supplier API tester-2.0.3/supplier_api_tester/v2/printer.py` & `Supplier API tester-2.0.4/supplier_api_tester/v2/printer.py`

 * *Files identical despite different names*

### Comparing `Supplier API tester-2.0.3/supplier_api_tester/v2/tester.py` & `Supplier API tester-2.0.4/supplier_api_tester/v2/tester.py`

 * *Files identical despite different names*

### Comparing `Supplier API tester-2.0.3/supplier_api_tester/v2/tests/__init__.py` & `Supplier API tester-2.0.4/supplier_api_tester/v2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Supplier API tester-2.0.3/supplier_api_tester/v2/tests/availability_variants.py` & `Supplier API tester-2.0.4/supplier_api_tester/v2/tests/availability_variants.py`

 * *Files identical despite different names*

### Comparing `Supplier API tester-2.0.3/supplier_api_tester/v2/tests/booking.py` & `Supplier API tester-2.0.4/supplier_api_tester/v2/tests/booking.py`

 * *Files identical despite different names*

### Comparing `Supplier API tester-2.0.3/supplier_api_tester/v2/tests/product_catalog.py` & `Supplier API tester-2.0.4/supplier_api_tester/v2/tests/product_catalog.py`

 * *Files identical despite different names*

### Comparing `Supplier API tester-2.0.3/supplier_api_tester/v2/tests/reservation.py` & `Supplier API tester-2.0.4/supplier_api_tester/v2/tests/reservation.py`

 * *Files identical despite different names*

### Comparing `Supplier API tester-2.0.3/supplier_api_tester/v2/utils/adapters.py` & `Supplier API tester-2.0.4/supplier_api_tester/v2/utils/adapters.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,26 +51,27 @@
 def parse_availability_variants(raw_response: Response, response: Dict) -> List[DailyVariants]:
     """Getting and testing response from the /availability endpoint"""
     if type(response) is not dict:
         raise FailedTest(
             message='The response should be a JSON Object',
             response=raw_response,
         )
-
     available_variants: List[DailyVariants] = []
     try:
         for day, day_availability in response.items():
             # extract timeslot component from the day value: YYYY-MM-DDTHH:MM
             date_time_value = datetime.fromisoformat(day)
+            timeslot_hour: str = str(date_time_value.time().hour)
+            timeslot_minutes: str = str(date_time_value.time().minute)
             available_variants.append(
                 dacite.from_dict(
                     data_class=DailyVariants,
                     data={
                         'date': str(date_time_value.date()),
-                        'timeslot': f'{date_time_value.time().hour}:{date_time_value.time().minute}',
+                        'timeslot': f'{timeslot_hour.zfill(2)}:{timeslot_minutes.zfill(2)}',
                         'available_tickets': day_availability.get('available_tickets', 0),
                         'variants': [
                             {**v}
                             for v in day_availability.get('variants', [])
                         ]
                     },
                     config=dacite.Config(
```

### Comparing `Supplier API tester-2.0.3/supplier_api_tester/v2/utils/availability.py` & `Supplier API tester-2.0.4/supplier_api_tester/v2/utils/availability.py`

 * *Files identical despite different names*

### Comparing `Supplier API tester-2.0.3/supplier_api_tester/v2/utils/catalog.py` & `Supplier API tester-2.0.4/supplier_api_tester/v2/utils/catalog.py`

 * *Files identical despite different names*

### Comparing `Supplier API tester-2.0.3/supplier_api_tester/v2/utils/errors.py` & `Supplier API tester-2.0.4/supplier_api_tester/v2/utils/errors.py`

 * *Files identical despite different names*

### Comparing `Supplier API tester-2.0.3/supplier_api_tester/v2/utils/reservation.py` & `Supplier API tester-2.0.4/supplier_api_tester/v2/utils/reservation.py`

 * *Files identical despite different names*

