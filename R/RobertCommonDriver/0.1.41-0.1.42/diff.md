# Comparing `tmp/RobertCommonDriver-0.1.41.tar.gz` & `tmp/RobertCommonDriver-0.1.42.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RobertCommonDriver-0.1.41.tar", last modified: Fri May 26 06:57:25 2023, max compression
+gzip compressed data, was "RobertCommonDriver-0.1.42.tar", last modified: Fri Jun  9 09:58:37 2023, max compression
```

## Comparing `RobertCommonDriver-0.1.41.tar` & `RobertCommonDriver-0.1.42.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 06:57:25.583469 RobertCommonDriver-0.1.41/
--rw-rw-rw-   0        0        0     1067 2021-08-09 02:56:17.000000 RobertCommonDriver-0.1.41/LICENSE
--rw-rw-rw-   0        0        0       44 2021-08-09 07:19:42.000000 RobertCommonDriver-0.1.41/MANIFEST.in
--rw-rw-rw-   0        0        0     1744 2023-05-26 06:57:25.582466 RobertCommonDriver-0.1.41/PKG-INFO
--rw-rw-rw-   0        0        0     1059 2022-01-13 07:06:32.000000 RobertCommonDriver-0.1.41/README.md
-drwxrwxrwx   0        0        0        0 2023-05-26 06:57:25.499331 RobertCommonDriver-0.1.41/RobertCommonDriver.egg-info/
--rw-rw-rw-   0        0        0     1744 2023-05-26 06:57:25.000000 RobertCommonDriver-0.1.41/RobertCommonDriver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2802 2023-05-26 06:57:25.000000 RobertCommonDriver-0.1.41/RobertCommonDriver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 06:57:25.000000 RobertCommonDriver-0.1.41/RobertCommonDriver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      186 2023-05-26 06:57:25.000000 RobertCommonDriver-0.1.41/RobertCommonDriver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-05-26 06:57:25.000000 RobertCommonDriver-0.1.41/RobertCommonDriver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      199 2023-04-19 11:58:47.000000 RobertCommonDriver-0.1.41/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-05-26 06:57:25.500330 RobertCommonDriver-0.1.41/robertcommondriver/
--rw-rw-rw-   0        0        0        2 2021-08-09 03:27:49.000000 RobertCommonDriver-0.1.41/robertcommondriver/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 06:57:25.501331 RobertCommonDriver-0.1.41/robertcommondriver/system/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonDriver-0.1.41/robertcommondriver/system/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 06:57:25.516494 RobertCommonDriver-0.1.41/robertcommondriver/system/driver/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonDriver-0.1.41/robertcommondriver/system/driver/__init__.py
--rw-rw-rw-   0        0        0    87350 2023-05-26 02:15:16.000000 RobertCommonDriver-0.1.41/robertcommondriver/system/driver/bacnet.py
--rw-rw-rw-   0        0        0   495630 2023-04-11 03:08:18.000000 RobertCommonDriver-0.1.41/robertcommondriver/system/driver/bacnetc.py
--rw-rw-rw-   0        0        0     6025 2023-05-09 08:30:24.000000 RobertCommonDriver-0.1.41/robertcommondriver/system/driver/base.py
--rw-rw-rw-   0        0        0        0 2021-10-25 01:55:43.000000 RobertCommonDriver-0.1.41/robertcommondriver/system/driver/iec104.py
--rw-rw-rw-   0        0        0    38314 2023-05-26 02:15:16.000000 RobertCommonDriver-0.1.41/robertcommondriver/system/driver/modbus.py
--rw-rw-rw-   0        0        0    14000 2022-12-01 09:27:31.000000 RobertCommonDriver-0.1.41/robertcommondriver/system/driver/obix.py
--rw-rw-rw-   0        0        0    60819 2023-04-03 06:02:51.000000 RobertCommonDriver-0.1.41/robertcommondriver/system/driver/opcda.py
--rw-rw-rw-   0        0        0    17013 2022-12-01 09:27:31.000000 RobertCommonDriver-0.1.41/robertcommondriver/system/driver/opcda_openopc.py
--rw-rw-rw-   0        0        0    15955 2022-12-01 09:27:31.000000 RobertCommonDriver-0.1.41/robertcommondriver/system/driver/opcua.py
--rw-rw-rw-   0        0        0    33482 2022-12-14 03:05:41.000000 RobertCommonDriver-0.1.41/robertcommondriver/system/driver/plcs7.py
--rw-rw-rw-   0        0        0    16586 2022-12-14 03:07:06.000000 RobertCommonDriver-0.1.41/robertcommondriver/system/driver/snmp.py
-drwxrwxrwx   0        0        0        0 2023-05-26 06:57:25.538701 RobertCommonDriver-0.1.41/robertcommondriver/system/iot/
--rw-rw-rw-   0        0        0        0 2022-06-15 07:27:26.000000 RobertCommonDriver-0.1.41/robertcommondriver/system/iot/__init__.py
--rw-rw-rw-   0        0        0    67070 2023-05-23 12:30:50.000000 RobertCommonDriver-0.1.41/robertcommondriver/system/iot/base.py
--rw-rw-rw-   0        0        0    65934 2023-05-26 02:15:16.000000 RobertCommonDriver-0.1.41/robertcommondriver/system/iot/iot_bacnet.py
--rw-rw-rw-   0        0        0   566090 2023-05-26 02:15:16.000000 RobertCommonDriver-0.1.41/robertcommondriver/system/iot/iot_bacnet_mstp.py
--rw-rw-rw-   0        0        0    46987 2023-05-26 02:15:16.000000 RobertCommonDriver-0.1.41/robertcommondriver/system/iot/iot_iec104.py
--rw-rw-rw-   0        0        0    34343 2023-05-26 02:15:16.000000 RobertCommonDriver-0.1.41/robertcommondriver/system/iot/iot_modbus.py
--rw-rw-rw-   0        0        0    18368 2023-04-27 02:18:02.000000 RobertCommonDriver-0.1.41/robertcommondriver/system/iot/iot_obix.py
--rw-rw-rw-   0        0        0    62043 2023-05-26 02:15:16.000000 RobertCommonDriver-0.1.41/robertcommondriver/system/iot/iot_opcda.py
--rw-rw-rw-   0        0        0    24991 2023-05-26 02:15:16.000000 RobertCommonDriver-0.1.41/robertcommondriver/system/iot/iot_opcua.py
--rw-rw-rw-   0        0        0    43449 2023-05-16 08:00:18.000000 RobertCommonDriver-0.1.41/robertcommondriver/system/iot/iot_plc_ab.py
--rw-rw-rw-   0        0        0    51679 2023-05-16 08:00:18.000000 RobertCommonDriver-0.1.41/robertcommondriver/system/iot/iot_plc_mitsubishi.py
--rw-rw-rw-   0        0        0    41711 2023-05-26 02:15:16.000000 RobertCommonDriver-0.1.41/robertcommondriver/system/iot/iot_plc_omron.py
--rw-rw-rw-   0        0        0    32984 2023-05-26 02:15:16.000000 RobertCommonDriver-0.1.41/robertcommondriver/system/iot/iot_plc_s7.py
--rw-rw-rw-   0        0        0    44835 2023-05-26 02:15:16.000000 RobertCommonDriver-0.1.41/robertcommondriver/system/iot/iot_plc_siemens.py
--rw-rw-rw-   0        0        0    13003 2023-04-17 05:43:15.000000 RobertCommonDriver-0.1.41/robertcommondriver/system/iot/iot_snmp.py
--rw-rw-rw-   0        0        0       42 2023-05-26 06:57:25.583469 RobertCommonDriver-0.1.41/setup.cfg
--rw-rw-rw-   0        0        0     3881 2023-05-26 02:15:16.000000 RobertCommonDriver-0.1.41/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-26 06:57:25.540697 RobertCommonDriver-0.1.41/tests/
--rw-rw-rw-   0        0        0        0 2021-07-27 06:06:01.000000 RobertCommonDriver-0.1.41/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 06:57:25.541696 RobertCommonDriver-0.1.41/tests/test_system/
--rw-rw-rw-   0        0        0        0 2021-07-27 06:49:45.000000 RobertCommonDriver-0.1.41/tests/test_system/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 06:57:25.556396 RobertCommonDriver-0.1.41/tests/test_system/test_driver/
--rw-rw-rw-   0        0        0        0 2021-08-06 06:51:11.000000 RobertCommonDriver-0.1.41/tests/test_system/test_driver/__init__.py
--rw-rw-rw-   0        0        0     6948 2022-06-08 07:19:27.000000 RobertCommonDriver-0.1.41/tests/test_system/test_driver/test_bacnet.py
--rw-rw-rw-   0        0        0     2038 2022-04-14 03:52:19.000000 RobertCommonDriver-0.1.41/tests/test_system/test_driver/test_bacnet1.py
--rw-rw-rw-   0        0        0     3839 2022-08-02 01:50:14.000000 RobertCommonDriver-0.1.41/tests/test_system/test_driver/test_bacnetc.py
--rw-rw-rw-   0        0        0     7865 2022-06-14 02:23:23.000000 RobertCommonDriver-0.1.41/tests/test_system/test_driver/test_bacnetv1.py
--rw-rw-rw-   0        0        0     2008 2022-01-13 07:23:11.000000 RobertCommonDriver-0.1.41/tests/test_system/test_driver/test_modbus.py
--rw-rw-rw-   0        0        0     9784 2022-07-21 02:42:09.000000 RobertCommonDriver-0.1.41/tests/test_system/test_driver/test_obix.py
--rw-rw-rw-   0        0        0     5912 2022-07-07 09:34:12.000000 RobertCommonDriver-0.1.41/tests/test_system/test_driver/test_opcda.py
--rw-rw-rw-   0        0        0     1686 2022-07-13 03:25:06.000000 RobertCommonDriver-0.1.41/tests/test_system/test_driver/test_opcua.py
--rw-rw-rw-   0        0        0     2443 2022-08-12 05:55:46.000000 RobertCommonDriver-0.1.41/tests/test_system/test_driver/test_plcs7.py
--rw-rw-rw-   0        0        0     1444 2022-07-12 05:58:47.000000 RobertCommonDriver-0.1.41/tests/test_system/test_driver/test_snmp.py
-drwxrwxrwx   0        0        0        0 2023-05-26 06:57:25.580030 RobertCommonDriver-0.1.41/tests/test_system/test_iot/
--rw-rw-rw-   0        0        0        0 2022-06-15 07:28:45.000000 RobertCommonDriver-0.1.41/tests/test_system/test_iot/__init__.py
--rw-rw-rw-   0        0        0     3227 2022-06-20 07:43:32.000000 RobertCommonDriver-0.1.41/tests/test_system/test_iot/test_bacnet1.py
--rw-rw-rw-   0        0        0    22758 2023-05-22 08:58:48.000000 RobertCommonDriver-0.1.41/tests/test_system/test_iot/test_iot_bacnet.py
--rw-rw-rw-   0        0        0    20074 2023-04-17 06:34:20.000000 RobertCommonDriver-0.1.41/tests/test_system/test_iot/test_iot_bacnet_mstp.py
--rw-rw-rw-   0        0        0     1283 2023-04-14 08:30:44.000000 RobertCommonDriver-0.1.41/tests/test_system/test_iot/test_iot_iec104.py
--rw-rw-rw-   0        0        0    15816 2023-05-23 12:02:23.000000 RobertCommonDriver-0.1.41/tests/test_system/test_iot/test_iot_modbus.py
--rw-rw-rw-   0        0        0     4714 2023-04-13 03:12:39.000000 RobertCommonDriver-0.1.41/tests/test_system/test_iot/test_iot_obix.py
--rw-rw-rw-   0        0        0     2288 2023-04-13 02:01:19.000000 RobertCommonDriver-0.1.41/tests/test_system/test_iot/test_iot_opcda.py
--rw-rw-rw-   0        0        0     3663 2023-05-09 08:04:00.000000 RobertCommonDriver-0.1.41/tests/test_system/test_iot/test_iot_opcua.py
--rw-rw-rw-   0        0        0     1374 2023-04-14 09:46:49.000000 RobertCommonDriver-0.1.41/tests/test_system/test_iot/test_iot_plc_ab.py
--rw-rw-rw-   0        0        0     2510 2023-04-14 09:44:42.000000 RobertCommonDriver-0.1.41/tests/test_system/test_iot/test_iot_plc_mitsubishi.py
--rw-rw-rw-   0        0        0     2836 2023-04-14 09:45:55.000000 RobertCommonDriver-0.1.41/tests/test_system/test_iot/test_iot_plc_omron.py
--rw-rw-rw-   0        0        0     9628 2023-05-25 08:18:30.000000 RobertCommonDriver-0.1.41/tests/test_system/test_iot/test_iot_plc_s7.py
--rw-rw-rw-   0        0        0     4154 2023-04-14 09:43:43.000000 RobertCommonDriver-0.1.41/tests/test_system/test_iot/test_iot_plc_siemens.py
--rw-rw-rw-   0        0        0      350 2022-08-16 09:35:34.000000 RobertCommonDriver-0.1.41/tests/test_system/test_iot/test_iot_plc_simenses1.py
--rw-rw-rw-   0        0        0     2292 2023-04-17 05:38:28.000000 RobertCommonDriver-0.1.41/tests/test_system/test_iot/test_iot_snmp.py
+drwxrwxrwx   0        0        0        0 2023-06-09 09:58:37.113941 RobertCommonDriver-0.1.42/
+-rw-rw-rw-   0        0        0     1067 2021-08-09 02:56:17.000000 RobertCommonDriver-0.1.42/LICENSE
+-rw-rw-rw-   0        0        0       44 2021-08-09 07:19:42.000000 RobertCommonDriver-0.1.42/MANIFEST.in
+-rw-rw-rw-   0        0        0      850 2023-06-09 09:58:37.112593 RobertCommonDriver-0.1.42/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2023-06-02 07:57:02.000000 RobertCommonDriver-0.1.42/README.md
+drwxrwxrwx   0        0        0        0 2023-06-09 09:58:37.030483 RobertCommonDriver-0.1.42/RobertCommonDriver.egg-info/
+-rw-rw-rw-   0        0        0      850 2023-06-09 09:58:36.000000 RobertCommonDriver-0.1.42/RobertCommonDriver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2802 2023-06-09 09:58:36.000000 RobertCommonDriver-0.1.42/RobertCommonDriver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 09:58:36.000000 RobertCommonDriver-0.1.42/RobertCommonDriver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      186 2023-06-09 09:58:36.000000 RobertCommonDriver-0.1.42/RobertCommonDriver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-06-09 09:58:36.000000 RobertCommonDriver-0.1.42/RobertCommonDriver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      199 2023-04-19 11:58:47.000000 RobertCommonDriver-0.1.42/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 09:58:37.031483 RobertCommonDriver-0.1.42/robertcommondriver/
+-rw-rw-rw-   0        0        0        2 2021-08-09 03:27:49.000000 RobertCommonDriver-0.1.42/robertcommondriver/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 09:58:37.032485 RobertCommonDriver-0.1.42/robertcommondriver/system/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonDriver-0.1.42/robertcommondriver/system/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 09:58:37.045996 RobertCommonDriver-0.1.42/robertcommondriver/system/driver/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonDriver-0.1.42/robertcommondriver/system/driver/__init__.py
+-rw-rw-rw-   0        0        0    87436 2023-06-09 02:14:48.000000 RobertCommonDriver-0.1.42/robertcommondriver/system/driver/bacnet.py
+-rw-rw-rw-   0        0        0   495630 2023-04-11 03:08:18.000000 RobertCommonDriver-0.1.42/robertcommondriver/system/driver/bacnetc.py
+-rw-rw-rw-   0        0        0     6074 2023-06-09 02:14:48.000000 RobertCommonDriver-0.1.42/robertcommondriver/system/driver/base.py
+-rw-rw-rw-   0        0        0        0 2021-10-25 01:55:43.000000 RobertCommonDriver-0.1.42/robertcommondriver/system/driver/iec104.py
+-rw-rw-rw-   0        0        0    38348 2023-06-08 07:41:58.000000 RobertCommonDriver-0.1.42/robertcommondriver/system/driver/modbus.py
+-rw-rw-rw-   0        0        0    14000 2022-12-01 09:27:31.000000 RobertCommonDriver-0.1.42/robertcommondriver/system/driver/obix.py
+-rw-rw-rw-   0        0        0    60844 2023-06-08 07:41:58.000000 RobertCommonDriver-0.1.42/robertcommondriver/system/driver/opcda.py
+-rw-rw-rw-   0        0        0    17038 2023-06-08 07:41:58.000000 RobertCommonDriver-0.1.42/robertcommondriver/system/driver/opcda_openopc.py
+-rw-rw-rw-   0        0        0    15983 2023-06-08 07:41:58.000000 RobertCommonDriver-0.1.42/robertcommondriver/system/driver/opcua.py
+-rw-rw-rw-   0        0        0    33512 2023-06-08 07:41:58.000000 RobertCommonDriver-0.1.42/robertcommondriver/system/driver/plcs7.py
+-rw-rw-rw-   0        0        0    16600 2023-06-08 07:41:58.000000 RobertCommonDriver-0.1.42/robertcommondriver/system/driver/snmp.py
+drwxrwxrwx   0        0        0        0 2023-06-09 09:58:37.067191 RobertCommonDriver-0.1.42/robertcommondriver/system/iot/
+-rw-rw-rw-   0        0        0        0 2022-06-15 07:27:26.000000 RobertCommonDriver-0.1.42/robertcommondriver/system/iot/__init__.py
+-rw-rw-rw-   0        0        0    68887 2023-06-09 09:05:11.000000 RobertCommonDriver-0.1.42/robertcommondriver/system/iot/base.py
+-rw-rw-rw-   0        0        0    65695 2023-06-09 08:26:24.000000 RobertCommonDriver-0.1.42/robertcommondriver/system/iot/iot_bacnet.py
+-rw-rw-rw-   0        0        0   566106 2023-06-09 08:36:24.000000 RobertCommonDriver-0.1.42/robertcommondriver/system/iot/iot_bacnet_mstp.py
+-rw-rw-rw-   0        0        0    46883 2023-06-09 08:36:24.000000 RobertCommonDriver-0.1.42/robertcommondriver/system/iot/iot_iec104.py
+-rw-rw-rw-   0        0        0    34014 2023-06-09 08:36:24.000000 RobertCommonDriver-0.1.42/robertcommondriver/system/iot/iot_modbus.py
+-rw-rw-rw-   0        0        0    18268 2023-06-09 08:36:24.000000 RobertCommonDriver-0.1.42/robertcommondriver/system/iot/iot_obix.py
+-rw-rw-rw-   0        0        0    61893 2023-06-09 08:55:51.000000 RobertCommonDriver-0.1.42/robertcommondriver/system/iot/iot_opcda.py
+-rw-rw-rw-   0        0        0    24773 2023-06-09 08:44:21.000000 RobertCommonDriver-0.1.42/robertcommondriver/system/iot/iot_opcua.py
+-rw-rw-rw-   0        0        0    43247 2023-06-09 08:55:51.000000 RobertCommonDriver-0.1.42/robertcommondriver/system/iot/iot_plc_ab.py
+-rw-rw-rw-   0        0        0    51493 2023-06-09 08:55:51.000000 RobertCommonDriver-0.1.42/robertcommondriver/system/iot/iot_plc_mitsubishi.py
+-rw-rw-rw-   0        0        0    41509 2023-06-09 08:55:51.000000 RobertCommonDriver-0.1.42/robertcommondriver/system/iot/iot_plc_omron.py
+-rw-rw-rw-   0        0        0    32738 2023-06-09 09:05:11.000000 RobertCommonDriver-0.1.42/robertcommondriver/system/iot/iot_plc_s7.py
+-rw-rw-rw-   0        0        0    44863 2023-06-09 08:55:51.000000 RobertCommonDriver-0.1.42/robertcommondriver/system/iot/iot_plc_siemens.py
+-rw-rw-rw-   0        0        0    12926 2023-06-09 08:55:51.000000 RobertCommonDriver-0.1.42/robertcommondriver/system/iot/iot_snmp.py
+-rw-rw-rw-   0        0        0       42 2023-06-09 09:58:37.113941 RobertCommonDriver-0.1.42/setup.cfg
+-rw-rw-rw-   0        0        0     3881 2023-06-09 09:33:34.000000 RobertCommonDriver-0.1.42/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 09:58:37.068615 RobertCommonDriver-0.1.42/tests/
+-rw-rw-rw-   0        0        0        0 2021-07-27 06:06:01.000000 RobertCommonDriver-0.1.42/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 09:58:37.068615 RobertCommonDriver-0.1.42/tests/test_system/
+-rw-rw-rw-   0        0        0        0 2021-07-27 06:49:45.000000 RobertCommonDriver-0.1.42/tests/test_system/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 09:58:37.082620 RobertCommonDriver-0.1.42/tests/test_system/test_driver/
+-rw-rw-rw-   0        0        0        0 2021-08-06 06:51:11.000000 RobertCommonDriver-0.1.42/tests/test_system/test_driver/__init__.py
+-rw-rw-rw-   0        0        0     6948 2022-06-08 07:19:27.000000 RobertCommonDriver-0.1.42/tests/test_system/test_driver/test_bacnet.py
+-rw-rw-rw-   0        0        0     2038 2022-04-14 03:52:19.000000 RobertCommonDriver-0.1.42/tests/test_system/test_driver/test_bacnet1.py
+-rw-rw-rw-   0        0        0     3839 2022-08-02 01:50:14.000000 RobertCommonDriver-0.1.42/tests/test_system/test_driver/test_bacnetc.py
+-rw-rw-rw-   0        0        0     7865 2022-06-14 02:23:23.000000 RobertCommonDriver-0.1.42/tests/test_system/test_driver/test_bacnetv1.py
+-rw-rw-rw-   0        0        0     2008 2022-01-13 07:23:11.000000 RobertCommonDriver-0.1.42/tests/test_system/test_driver/test_modbus.py
+-rw-rw-rw-   0        0        0     9784 2022-07-21 02:42:09.000000 RobertCommonDriver-0.1.42/tests/test_system/test_driver/test_obix.py
+-rw-rw-rw-   0        0        0     5912 2022-07-07 09:34:12.000000 RobertCommonDriver-0.1.42/tests/test_system/test_driver/test_opcda.py
+-rw-rw-rw-   0        0        0     1686 2022-07-13 03:25:06.000000 RobertCommonDriver-0.1.42/tests/test_system/test_driver/test_opcua.py
+-rw-rw-rw-   0        0        0     2443 2022-08-12 05:55:46.000000 RobertCommonDriver-0.1.42/tests/test_system/test_driver/test_plcs7.py
+-rw-rw-rw-   0        0        0     1444 2022-07-12 05:58:47.000000 RobertCommonDriver-0.1.42/tests/test_system/test_driver/test_snmp.py
+drwxrwxrwx   0        0        0        0 2023-06-09 09:58:37.111478 RobertCommonDriver-0.1.42/tests/test_system/test_iot/
+-rw-rw-rw-   0        0        0        0 2022-06-15 07:28:45.000000 RobertCommonDriver-0.1.42/tests/test_system/test_iot/__init__.py
+-rw-rw-rw-   0        0        0     3227 2022-06-20 07:43:32.000000 RobertCommonDriver-0.1.42/tests/test_system/test_iot/test_bacnet1.py
+-rw-rw-rw-   0        0        0    22758 2023-05-22 08:58:48.000000 RobertCommonDriver-0.1.42/tests/test_system/test_iot/test_iot_bacnet.py
+-rw-rw-rw-   0        0        0    20074 2023-04-17 06:34:20.000000 RobertCommonDriver-0.1.42/tests/test_system/test_iot/test_iot_bacnet_mstp.py
+-rw-rw-rw-   0        0        0     1283 2023-04-14 08:30:44.000000 RobertCommonDriver-0.1.42/tests/test_system/test_iot/test_iot_iec104.py
+-rw-rw-rw-   0        0        0    15816 2023-05-23 12:02:23.000000 RobertCommonDriver-0.1.42/tests/test_system/test_iot/test_iot_modbus.py
+-rw-rw-rw-   0        0        0     4707 2023-06-01 02:58:21.000000 RobertCommonDriver-0.1.42/tests/test_system/test_iot/test_iot_obix.py
+-rw-rw-rw-   0        0        0     2288 2023-04-13 02:01:19.000000 RobertCommonDriver-0.1.42/tests/test_system/test_iot/test_iot_opcda.py
+-rw-rw-rw-   0        0        0     3663 2023-05-09 08:04:00.000000 RobertCommonDriver-0.1.42/tests/test_system/test_iot/test_iot_opcua.py
+-rw-rw-rw-   0        0        0     1374 2023-04-14 09:46:49.000000 RobertCommonDriver-0.1.42/tests/test_system/test_iot/test_iot_plc_ab.py
+-rw-rw-rw-   0        0        0     2510 2023-04-14 09:44:42.000000 RobertCommonDriver-0.1.42/tests/test_system/test_iot/test_iot_plc_mitsubishi.py
+-rw-rw-rw-   0        0        0     2836 2023-04-14 09:45:55.000000 RobertCommonDriver-0.1.42/tests/test_system/test_iot/test_iot_plc_omron.py
+-rw-rw-rw-   0        0        0     9628 2023-05-25 08:18:30.000000 RobertCommonDriver-0.1.42/tests/test_system/test_iot/test_iot_plc_s7.py
+-rw-rw-rw-   0        0        0     4154 2023-04-14 09:43:43.000000 RobertCommonDriver-0.1.42/tests/test_system/test_iot/test_iot_plc_siemens.py
+-rw-rw-rw-   0        0        0      350 2022-08-16 09:35:34.000000 RobertCommonDriver-0.1.42/tests/test_system/test_iot/test_iot_plc_simenses1.py
+-rw-rw-rw-   0        0        0     2292 2023-04-17 05:38:28.000000 RobertCommonDriver-0.1.42/tests/test_system/test_iot/test_iot_snmp.py
```

### Comparing `RobertCommonDriver-0.1.41/LICENSE` & `RobertCommonDriver-0.1.42/LICENSE`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.41/RobertCommonDriver.egg-info/SOURCES.txt` & `RobertCommonDriver-0.1.42/RobertCommonDriver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.41/robertcommondriver/system/driver/bacnet.py` & `RobertCommonDriver-0.1.42/robertcommondriver/system/driver/bacnet.py`

 * *Files 0% similar despite different names*

```diff
@@ -1491,15 +1491,15 @@
                         self.bacnet_application.protocolServicesSupported = pss.value
 
         except Exception as e:
             raise e
         return self.bacnet_application
 
     def _running_bacnet(self):
-        BaseCommon.function_thread(self._running_bacnet_thread, False).start()
+        BaseCommon.function_thread(self._running_bacnet_thread, False, f"bacnet({self})").start()
 
         # Wait for 1s to read data before delay start
         time.sleep(self.bacnet_cmd_interval)
 
     def _running_bacnet_thread(self):
         if self.bacnet_application_runing is False:
             if self._get_bacnet_application():
@@ -1508,15 +1508,15 @@
                 run(spin=0.1)
 
     # Search Bacnet devices
     def _search_bacnet_device_list(self) -> list:
         bacnet_device_list = []
         # Create a thread here to execute 10s and judge the timeout to end
 
-        BaseCommon.function_thread(fn=self._handle_search_bacnet_device, daemon=True).start()
+        BaseCommon.function_thread(fn=self._handle_search_bacnet_device, daemon=True, name=f"bacnet({self})").start()
 
         # Here to determine whether the thread has timed out and the timeout ends
         exit_thread = False
         while exit_thread is False:
             time.sleep(1)
             bacnet_device_list = self._end_search_bacnet_device()
             if bacnet_device_list is not None:
@@ -1601,15 +1601,15 @@
             bacnet_application = bacnet_app_class(bacnet_device, self.bacnet_server_ip, self)
             self.set_call_result('debug_log', content=f"bacnet({self}) get app: {bacnet_application}")
             if bacnet_application is not None:
                 if bacnet_application.bacnet_init_status is False:
                     logging.error(f'bacnet({self}) get application({self.bacnet_server_ip}) fail {bacnet_application.bacnet_exception}')
                     bacnet_application = self._release_bacnet_application_v1(bacnet_application)
                 else:
-                    BaseCommon.function_thread(self.control_status, False).start()
+                    BaseCommon.function_thread(self.control_status, False, f"bacnet({self})").start()
                     time.sleep(1)
                     return bacnet_application
         return None
 
     def _release_bacnet_application_v1(self, bacnet_application):
         try:
             if bacnet_application:
@@ -1629,15 +1629,15 @@
     def _search_bacnet_device_list_v1(self) -> list:
         self.bacnet_device_list = []
         bacnet_whois_application = None
         try:
             bacnet_whois_application = self._get_bacnet_application_v1(BacnetWhoIsIAmApplication)
             if bacnet_whois_application is not None:
 
-                BaseCommon.function_thread(fn=self._end_search_bacnet_device_v1, daemon=True, bacnet_application=bacnet_whois_application).start()
+                BaseCommon.function_thread(fn=self._end_search_bacnet_device_v1, daemon=True, bacnet_application=bacnet_whois_application, name=f"bacnet({self})").start()
 
                 bacnet_whois_application.discover_bacnet_device()
 
                 run(spin=0.1)
             return self.bacnet_device_list
         finally:
             bacnet_whois_application = self._release_bacnet_application_v1(bacnet_whois_application)
```

### Comparing `RobertCommonDriver-0.1.41/robertcommondriver/system/driver/bacnetc.py` & `RobertCommonDriver-0.1.42/robertcommondriver/system/driver/bacnetc.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.41/robertcommondriver/system/driver/base.py` & `RobertCommonDriver-0.1.42/robertcommondriver/system/driver/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, Any, Callable
+from typing import Dict, Any, Callable, Optional
 from abc import abstractmethod
 from datetime import datetime
 from threading import Timer, Thread
 from ipaddress import ip_network, ip_address
 from psutil import net_if_addrs
 from re import compile as re_compile
 
@@ -66,16 +66,16 @@
 
         def cancel(self):
             if self.is_running():
                 self.timer.cancel()
             self.timer = None
 
     @staticmethod
-    def function_thread(fn: Callable, daemon: bool, *args, **kwargs):
-        return Thread(target=fn, args=args, kwargs=kwargs, daemon=daemon)
+    def function_thread(fn: Callable, daemon: bool, name: Optional[str] = None, *args, **kwargs):
+        return Thread(target=fn, name=name, args=args, kwargs=kwargs, daemon=daemon)
 
     @staticmethod
     def chunk_list(values: list, num: int):
         for i in range(0, len(values), num):
             yield values[i: i + num]
 
     @staticmethod
```

### Comparing `RobertCommonDriver-0.1.41/robertcommondriver/system/driver/modbus.py` & `RobertCommonDriver-0.1.42/robertcommondriver/system/driver/modbus.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,15 +145,15 @@
     def get_modbus_point_list(self):
         return self.modbus_point_list
 
 
 class ModbusEngine(Thread):
 
     def __init__(self, control_mode: str, device_address: str, dict_point: dict, modbus_time_out: int, modbus_multi_read: int, modbus_cmd_interval: float, callbacks: dict = {}):
-        Thread.__init__(self)
+        Thread.__init__(self, name=f"modbus({device_address})")
 
         self.control_mode = control_mode            # read/write
         self.device_address = device_address
         self.dict_point = dict_point
 
         # #modbus connect param ##########################
         self.modbus_time_out = modbus_time_out
```

### Comparing `RobertCommonDriver-0.1.41/robertcommondriver/system/driver/obix.py` & `RobertCommonDriver-0.1.42/robertcommondriver/system/driver/obix.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.41/robertcommondriver/system/driver/opcda.py` & `RobertCommonDriver-0.1.42/robertcommondriver/system/driver/opcda.py`

 * *Files 0% similar despite different names*

```diff
@@ -1077,15 +1077,15 @@
     def get_point_description(self):
         return self.point_description
 
 
 class OPCDAEngine(Thread):
 
     def __init__(self, server: str, host: str, action: str, group: str, read_limit: int, update_rate: int, point_dict: dict, call_back_func=None):
-        Thread.__init__(self)
+        Thread.__init__(self, name=f"OPCDA({server})")
 
         # param#########
         self.server = server
         self.host = host
         self.group = group
         self.action = action
```

### Comparing `RobertCommonDriver-0.1.41/robertcommondriver/system/driver/opcda_openopc.py` & `RobertCommonDriver-0.1.42/robertcommondriver/system/driver/opcda_openopc.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
     def get_point_description(self):
         return self.point_description
 
 
 class OPCDAEngine(Thread):
 
     def __init__(self, server: str, host: str, group: str, read_limit: int, update_rate: int, point_dict: dict, call_back_func=None):
-        Thread.__init__(self)
+        Thread.__init__(self, name=f"opcda({server})")
 
         # param#########
         self.server = server
         self.host = host
         self.group = group
 
         self.read_limit = read_limit
```

### Comparing `RobertCommonDriver-0.1.41/robertcommondriver/system/driver/opcua.py` & `RobertCommonDriver-0.1.42/robertcommondriver/system/driver/opcua.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     def get_point_node_id(self):
         return self.point_node_id
 
 
 class OPCUAEngine(Thread):
 
     def __init__(self, end_point: str, security_string: str, authentication: dict,  subscript_add: int, subscript_interval: int, point_dict: dict, call_back_func=None):
-        Thread.__init__(self)
+        Thread.__init__(self, name=f"opcua({end_point})")
 
         # param#########
         self.end_point = end_point
         self.security_string = security_string
         self.authentication = authentication
         self.subscript_add = subscript_add
         self.subscript_interval = subscript_interval
```

### Comparing `RobertCommonDriver-0.1.41/robertcommondriver/system/driver/plcs7.py` & `RobertCommonDriver-0.1.42/robertcommondriver/system/driver/plcs7.py`

 * *Files 0% similar despite different names*

```diff
@@ -247,15 +247,15 @@
 
 
 # SiemensS7
 class SiemensS7Engine(Thread):
 
     def __init__(self, control_mode: str, device_address: str, dict_point: dict, multi_read: int, cmd_interval: float,
                  send_timeout: int, rec_timeout: int):
-        Thread.__init__(self)
+        Thread.__init__(self, name=f"s7({device_address})")
 
         self.control_mode = control_mode  # read/write
         self.device_address = device_address
         self.dict_point = dict_point
         self.rack = -1
         self.slot = -1
```

### Comparing `RobertCommonDriver-0.1.41/robertcommondriver/system/driver/snmp.py` & `RobertCommonDriver-0.1.42/robertcommondriver/system/driver/snmp.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
 
 class SNMPEngine(Thread):
 
     def __init__(self, control_mode: str, snmp_transport: UdpTransportTarget,
                  snmp_auth: Union[CommunityData, UsmUserData], snmp_context: ContextData, cmd_interval: float,
                  limit: int, point_dict: dict, root_oid: str = '1.3', call_back_func=None):
-        Thread.__init__(self)
+        Thread.__init__(self, name=f"snmp")
 
         # param#########
         self.control_mode = control_mode
         self.cmd_interval = cmd_interval
         self.limit = limit
         self.snmp_auth = snmp_auth
         self.snmp_transport = snmp_transport
```

### Comparing `RobertCommonDriver-0.1.41/robertcommondriver/system/iot/base.py` & `RobertCommonDriver-0.1.42/robertcommondriver/system/iot/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -477,19 +477,19 @@
             return self.pool_status
 
         def info(self):
             return {'total': len(self.task_cache), 'running': len(self.task_running), 'finish': self.task_finish}
 
     class SimpleThreadPool:
 
-        def __init__(self, size: int, fun: Optional[Callable] = None, done_callback: Optional[Callable] = None, **kwargs):
+        def __init__(self, size: int, name_prefix: str = '', fun: Optional[Callable] = None, done_callback: Optional[Callable] = None, **kwargs):
             self.kwargs = kwargs
             self.pool_size = size              # 线程池大小
             self.pool_fun = fun                # 线程函数
-            self.pools = ThreadPoolExecutor(self.pool_size)  # 线程池
+            self.pools = ThreadPoolExecutor(self.pool_size, name_prefix)  # 线程池
             self.done_callback = done_callback              # 线程执行回调函数
             self.task_future = []
 
         def submit_task(self, task: Optional[Callable], *args, **kwargs):
             task = task if task else self.pool_fun
             if task is not None:
                 self.task_future.append(self.pools.submit(task, *args, **kwargs))
@@ -552,15 +552,15 @@
             self.valid = True
             self.host = host
             self.port = port
             self.sock = None
             self.timeout = timeout
             self.callbacks = {} if callbacks is None else callbacks
             self.connect()
-            IOTBaseCommon.function_thread(self.receive, True).start()
+            IOTBaseCommon.function_thread(self.receive, True, f"iecclient({host}:{port})").start()
             self.handle_connect()
 
         def __str__(self):
             return f"{self.host}:{self.port}"
 
         def __del__(self):
             self.exit()
@@ -644,15 +644,15 @@
             self.sock_type = sock_type
             self.host = host
             self.port = port
             self.sock = None
             self.timeout = timeout
             self.callbacks = {} if callbacks is None else callbacks
             self.connect()
-            IOTBaseCommon.function_thread(self.receive, True).start()
+            IOTBaseCommon.function_thread(self.receive, True, f"socket({host}:{port})").start()
             self.handle_connect()
 
         def __str__(self):
             return f"{self.host}:{self.port}"
 
         def __del__(self):
             self.exit()
@@ -728,15 +728,15 @@
     class SocketHandle:
 
         def __init__(self, conn: Optional[Any] = None, address: Optional[tuple] = None, server: Optional[Any] = None):
             self.conn = conn
             self.address = address
             self.server = server
             self.valid = True
-            IOTBaseCommon.function_thread(self.receive, True).start()
+            IOTBaseCommon.function_thread(self.receive, True, f"socket({address})").start()
 
         def __str__(self):
             if isinstance(self.address, tuple) and len(self.address) >= 2:
                 return f"{self.address[0]}:{self.address[1]}"
             return str(self.address)
 
         def __del__(self):
@@ -798,15 +798,15 @@
 
         def connect(self):
             self.sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
             self.sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
             self.sock.bind((self.host, self.port))
             self.sock.listen(self.size)
 
-            IOTBaseCommon.function_thread(self.accept, True).start()
+            IOTBaseCommon.function_thread(self.accept, True, f"server({self.host}:{self.port})").start()
 
         def socks(self):
             return self.sockets
 
         def accept(self):
             while self.valid is True:
                 conn, address = self.sock.accept()  # 接收连接
@@ -1181,22 +1181,22 @@
             self.exit()
             server_result = self.listen(self.host, self.port, self.size)
             if server_result.is_success is False:
                 server_result.contents[0] = None
                 result.msg = server_result.msg
             else:
                 self.iot_socket = server_result.contents[0]
-                IOTBaseCommon.function_thread(self.accept, True, self.iot_socket).start()
+                IOTBaseCommon.function_thread(self.accept, True, f"iot server({self.host}:{self.port})", self.iot_socket).start()
                 result.is_success = True
             return result
 
         def accept(self, socket: socket):
             while self.iot_socket is not None:
                 sock, addr = socket.accept()  # 接收连接
-                IOTBaseCommon.function_thread(self.receive_client, True, sock).start()
+                IOTBaseCommon.function_thread(self.receive_client, True, f"iot receive client({addr})", sock).start()
 
         def stop_server(self):
             result = IOTBaseCommon.IOTNetResult()
             with self.lock:
                 result = self.extra_on_disconnect(self.iot_socket)
                 self.exit()
                 return result
@@ -1238,16 +1238,16 @@
             self.word_length = 1  # 单个数据字节的长度，西门子为2，三菱，欧姆龙，modbusTcp就为1
             self.values = {}    # 数据集
 
         def simulate(self, address: Union[tuple, dict]):
             return IOTBaseCommon.IOTNetResult()
 
     @staticmethod
-    def function_thread(fn: Callable, daemon: bool, *args, **kwargs):
-        return Thread(target=fn, args=args, kwargs=kwargs, daemon=daemon)
+    def function_thread(fn: Callable, daemon: bool, name: Optional[str] = None, *args, **kwargs):
+        return Thread(target=fn, name=name, args=args, kwargs=kwargs, daemon=daemon)
 
     @staticmethod
     def chunk_list(values: list, num: int):
         for i in range(0, len(values), num):
             yield values[i: i + num]
 
     @staticmethod
@@ -1431,14 +1431,15 @@
         self.parent = kwargs.get('parent')  # 父节点
         self.tag = kwargs.get('tag', self.uuid)  # 关键信息
         self.log_limit = kwargs.get('log_limit', 500)  # 日志上限
         self.reinit_flag = True  # 重新初始化
         self.configs = {}
         self.points = {}
         self.devices = {}   # 设备点集合
+        self.results = self.results = {'success': {}, 'error': {}}   # 读取结果集
         self.enable = True
         self.exit_flag = False
         self.debug_pos = None
 
         self.client = None
         self.clients = None
         self.server = None
@@ -1511,15 +1512,14 @@
             call_logging = self.callbacks.get('call_logging')
             if call_logging:
                 call_logging(content=kwargs.get('content'))
             else:
                 error = kwargs.get('level')
                 if error == 'ERROR':
                     logging.error(kwargs.get('content'))
-                    # logging.error(f"[{kwargs.get('pos')}]: {kwargs.get('content')}")
             self.save_log(kwargs.get('content'))
 
     def simulate(self, **kwargs):
         raise NotImplementedError()
 
     def info(self, **kwargs) -> dict:
         return self.infos
@@ -1537,21 +1537,26 @@
     def control(self, enable: bool = True):
         self.enable = enable
 
     def discover(self, **kwargs):
         pass
 
     def delay(self, delay: Union[int, float] = 1):
+        self.pending()
+
+        while self.kwargs.get('configs', {}).get('enabled', True) is False:
+            time.sleep(1)
+
         if isinstance(delay, int):
-            while self.kwargs.get('enabled', True) is True and delay > 0:
+            while delay > 0:
                 time.sleep(1)
                 delay = delay - 1
         elif isinstance(delay, float):
             _delay = int(delay)
-            while self.kwargs.get('enabled', True) is True and _delay > 0:
+            while _delay > 0:
                 time.sleep(1)
                 _delay = _delay - 1
             time.sleep(delay - _delay)
 
     def save_log(self, log_content: str):
         if isinstance(log_content, str) and len(log_content) > 0:
             if len(self.logs) >= self.log_limit:
@@ -1567,14 +1572,15 @@
         for template in templates:
             point[template.get('code')] = template.get('default')
         point.update(**kwargs)
         return point
 
     @property
     def stack_pos(self):
+        return f"base.py(900)"
         return f"{IOTBaseCommon.get_file_name(stack()[1][1])}({stack()[1][2]})"
 
     def add_stack(self, content: Optional[str] = None):
         """添加程序位置"""
         self.debug_pos = f"{IOTBaseCommon.get_datetime_str()}: {IOTBaseCommon.get_file_name(stack()[1][1])}({stack()[1][2]}){'' if content is None else content}"
 
     def debug(self):
@@ -1615,7 +1621,39 @@
     @property
     def get_write_quality(self):
         return 'write_quality'
 
     @property
     def get_write_result(self):
         return 'write_result'
+
+    def update_results(self, names: Optional[Union[str, list]], quality: bool, result: Optional[Any], **kwargs):
+        """更新结果集"""
+        if quality is True and result is None:
+            self.results = {'count': len(names), 'success': {}, 'error': {}, 'start': IOTBaseCommon.get_datetime()}
+
+        if isinstance(names, str):
+            names = [names]
+        if isinstance(names, list):
+            for name in names:
+                if quality is True:
+                    self.results['success'][name] = result
+                else:
+                    if result not in self.results['error'].keys():
+                        self.results['error'][result] = []
+                    self.results['error'][result].append(name)
+
+    def get_results(self, show_error: bool = True) -> dict:
+        """获取结果集"""
+        now = IOTBaseCommon.get_datetime()
+        start = self.results.get('start', now)
+        success = self.results.get('success', {})
+        error = self.results.get('error', {})
+        count = self.results.get('count', 0)
+        self.update_info(read=count, response=success, cost='{:.2f}'.format((now - start).total_seconds()))
+
+        if show_error:
+            for err, names in error.items():
+                names = sorted(list(set(names)))
+                self.logging(content=f"get value({len(names)}) fail({err})", level='ERROR', source=','.join(names), pos=self.stack_pos)
+
+        return success
```

### Comparing `RobertCommonDriver-0.1.41/robertcommondriver/system/iot/iot_bacnet.py` & `RobertCommonDriver-0.1.42/robertcommondriver/system/iot/iot_bacnet.py`

 * *Files 0% similar despite different names*

```diff
@@ -680,15 +680,15 @@
         if self.bacnet_application is None:
             if bacnet_device is None:
                 bacnet_device = self.device(**self.kwargs)
 
             bacnet_application = bacnet_app_class(bacnet_device, self.bacnet_server_ip, callbacks={'logging': self.logging, 'i_am': self._call_back_i_am, 'cov': self._call_back_cov, 'write': None if self.is_client else self._call_back_write}, **self.kwargs)
             if bacnet_application is not None:
                 bacnet_application.add_capability(ReadWritePropertyMultipleServices)
-                IOTBaseCommon.function_thread(self.control, False).start()
+                IOTBaseCommon.function_thread(self.control, False, str(self)).start()
                 self.parent.delay(1)
                 self.bacnet_application = bacnet_application
         return self.bacnet_application
 
     def _release_application(self, bacnet_application):
         try:
             if bacnet_application:
@@ -700,17 +700,14 @@
             self.logging(content=f"release {self.bacnet_server_ip} fail {e.__str__()}", level='ERROR', pos=self.stack_pos)
         finally:
             if bacnet_application:
                 del bacnet_application
             bacnet_application = None
 
     def _send_request(self, request, wait_result: bool = True, context: Optional[IOCBContext] = None):
-        if self.parent is not None and hasattr(self.parent, 'pending'):
-            self.parent.pending()
-
         if self._get_application():
             request.apduInvokeID = self._get_application().get_next_invoke_id(request.pduDestination)
             self.logging(content=f"send({self.process}) {request.apduInvokeID} {request.__class__.__name__}", pos=self.stack_pos)
             return self._get_application().send_request(request, wait_result, context, self.process)
         return None
 
     def _find_reason(self, apdu) -> str:
@@ -1078,16 +1075,17 @@
 
             templates.append({'name': '超时(ms)' if lan == 'ch' else 'Timeout(ms)', 'required': True, 'code': 'timeout', 'type': 'int', 'default': 5000, 'enum': [], 'tip': ''})
         return templates
 
     def read(self, **kwargs):
         self.update_info(used=IOTBaseCommon.get_datetime_str())
 
-        results = {}
         names = kwargs.get('names', list(self.points.keys()))
+        self.update_results(names, True, None)
+
         read_items = {}
         for name in names:
             point = self.points.get(name)
             if point:
                 target_address = point.get('point_device_address')
                 object_type = point.get('point_type')
                 instance_number = point.get('point_address')
@@ -1106,21 +1104,19 @@
             if point:
                 target_address = point.get('point_device_address')
                 object_type = point.get('point_type')
                 instance_number = point.get('point_address')
                 point_property = point.get('point_property', 'presentValue')
                 value = self._get_value(name, target_address, object_type, instance_number, point_property)
                 if value is not None:
-                    results[name] = value
+                    self.update_results(name, True, value)
             else:
-                self.logging(content=f"read point({name}) fail(UnExist)", level='ERROR', source=name, pos=self.stack_pos)
+                self.update_results(name, False, 'UnExist')
 
-        self.update_info(read=len(names), response=len(results))
-
-        return results
+        return self.get_results()
 
     def write(self, **kwargs):
         self.update_info(used=IOTBaseCommon.get_datetime_str())
 
         results = {}
         values = kwargs.get('values', {})
         for name, value in values.items():
@@ -1228,15 +1224,15 @@
 
     def _get_value(self, name: str, target_address: str, object_type: str, instance_number: int, point_property: str):
         if self._get_client():
             quality, value = self.client.value(target_address, object_type, instance_number, point_property)
             if quality == 'Good':
                 return value
             else:
-                self.logging(content=f"read point({name}) fail({value})", level='ERROR', source=name, pos=self.stack_pos)
+                self.update_results(name, False, value)
         return None
 
     def _write(self, name: str, target_address: str, object_type: str, instance_number: int, property_name: str, value):
         try:
             if self._get_client():
                 return self.client.write(target_address=target_address, object_type=object_type, instance_number=instance_number, property_name=property_name, value=value)
         except Exception as e:
```

### Comparing `RobertCommonDriver-0.1.41/robertcommondriver/system/iot/iot_bacnet_mstp.py` & `RobertCommonDriver-0.1.42/robertcommondriver/system/iot/iot_bacnet_mstp.py`

 * *Files 0% similar despite different names*

```diff
@@ -11747,15 +11747,15 @@
             comm.events['OnWhoIs'] = self.callback_whois
             comm.events['OnIam'] = self.callback_i_am
             comm.events['OnReadPropertyRequest'] = self.callback_read_property_request
             comm.events['OnCOVNotification'] = self.callback_cov_notification
             comm.events['OnEventNotify'] = self.callback_event_notify
 
             if kwargs.get('whois') is True and (type == BACnetDefine.BACnetAddressTypes.IP or isinstance(comm.m_client, BACnetMstpProtocolTransport)):
-                IOTBaseCommon.function_thread(self.discover, True, args=(comm,)).start()
+                IOTBaseCommon.function_thread(self.discover, True, f"{self}", args=(comm,)).start()
 
             if isinstance(comm.m_client, BACnetMstpProtocolTransport):
                 comm.m_client.events['FrameRecieved'] = self.callback_mstp_frame
 
             comm.Start()
 
             time.sleep(1)
@@ -12067,22 +12067,23 @@
             templates.append({'name': '设备重试' if lan == 'ch' else 'Bacnet Retries', 'required': True, 'code': 'retry', 'type': 'int', 'default': 2, 'enum': [], 'tip': ''})
             templates.append({'name': '设备segmentation' if lan == 'ch' else 'Bacnet Sever segmentation', 'required': True, 'code': 'segmentation', 'type': 'int', 'default': 65, 'enum': [], 'tip': ''})
             templates.append({'name': '设备vendor' if lan == 'ch' else 'Bacnet Sever vendor', 'required': True, 'code': 'vendor_identifier', 'type': 'int', 'default': 15, 'enum': [], 'tip': ''})
 
             if mode == 0:
                 templates.append({'name': '批量读取个数' if lan == 'ch' else 'Multi Read', 'required': True, 'code': 'multi_read', 'type': 'int', 'default': 20, 'enum': [], 'tip': ''})
                 templates.append({'name': '命令间隔(s)' if lan == 'ch' else 'Cmd Interval(s)', 'required': True, 'code': 'cmd_interval', 'type': 'float', 'default': 0.3, 'enum': [], 'tip': ''})
-            templates.append({'name': '超时(s)' if lan == 'ch' else 'Timeout(ms)', 'required': True, 'code': 'timeout', 'type': 'int', 'default': 5, 'enum': [], 'tip': ''})
+            templates.append({'name': '超时(ms)' if lan == 'ch' else 'Timeout(ms)', 'required': True, 'code': 'timeout', 'type': 'int', 'default': 5000, 'enum': [], 'tip': ''})
         return templates
 
     def read(self, **kwargs):
         self.update_info(used=IOTBaseCommon.get_datetime_str())
 
-        results = {}
         names = kwargs.get('names', list(self.points.keys()))
+        self.update_results(names, True, None)
+
         read_items = {}
         for name in names:
             point = self.points.get(name)
             if point:
                 target_address = point.get('point_device_address')
                 object_type = self.convert_type(point.get('point_type'))[0]
                 instance_number = point.get('point_address')
@@ -12101,28 +12102,27 @@
             if point:
                 target_address = point.get('point_device_address')
                 object_type = self.convert_type(point.get('point_type'))[0]
                 instance_number = point.get('point_address')
                 point_property = point.get('point_property', 'presentValue')
                 value = self._get_value(name, target_address, object_type, instance_number, point_property)
                 if value is not None:
-                    results[name] = value
-
-        self.update_info(read=len(names), response=len(results))
+                    self.update_results(name, True, value)
+            else:
+                self.update_results(name, False, 'UnExist')
 
-        return results
+        return self.get_results()
 
     def write(self, **kwargs):
         self.update_info(used=IOTBaseCommon.get_datetime_str())
 
         results = {}
         values = kwargs.get('values', {})
         for name, value in values.items():
             point = self.points.get(name)
-
             if point:
                 target_address = point.get('point_device_address')
                 object_type = self.convert_type(point.get('point_type'))[0]
                 instance_number = point.get('point_address')
                 point_property = point.get('point_property', 'presentValue')
                 if target_address is not None and object_type is not None and instance_number is not None:
                     result = self._write(name, target_address, object_type, instance_number, point_property, value)
@@ -12255,15 +12255,15 @@
 
     def _get_value(self, name: str, target_address: str, object_type: str, instance_number: int, point_property: str):
         if self._get_client():
             quality, value = self.application._get_value(self.client, target_address, object_type, instance_number, point_property)
             if quality == 'Good':
                 return value
             else:
-                self.logging(content=f"get value({name}) fail({value})", level='ERROR', source=name, pos=self.stack_pos)
+                self.update_results(name, False, value)
         return None
 
     def _write(self, name: str, target_address: str, object_type: int, instance_number: int, property_name: str, value):
         error_msg = ''
         try:
             if self._get_client():
                 return self.application.write(self.client, target_address=target_address, object_type=object_type, instance_number=instance_number, property_name=property_name, value=value)
```

### Comparing `RobertCommonDriver-0.1.41/robertcommondriver/system/iot/iot_iec104.py` & `RobertCommonDriver-0.1.42/robertcommondriver/system/iot/iot_iec104.py`

 * *Files 2% similar despite different names*

```diff
@@ -1012,16 +1012,16 @@
             ])
 
         return templates
 
     def read(self, **kwargs):
         self.update_info(used=IOTBaseCommon.get_datetime_str())
 
-        results = {}
         names = kwargs.get('names', list(self.points.keys()))
+        self.update_results(names, True, None)
         read_items = []
         for name in names:
             point = self.points.get(name)
             if point:
                 type = point.get('point_type')  # 单点遥信
                 address = point.get('point_address')    # 点地址
                 if type is not None and address is not None:
@@ -1033,18 +1033,18 @@
             point = self.points.get(name)
             if point:
                 type = point.get('point_type')  # 单点遥信
                 address = point.get('point_address')  # 点地址
                 if type is not None and address is not None:
                     value = self._get_value(name, f"{self.configs.get('host')}:{self.configs.get('port')}", address, type)
                     if value is not None:
-                        results[name] = value
-
-        self.update_info(read=len(names), response=len(results))
-        return results
+                        self.update_results(name, True, value)
+            else:
+                self.update_results(name, False, 'UnExist')
+        return self.get_results()
 
     def write(self, **kwargs):
         self.update_info(used=IOTBaseCommon.get_datetime_str())
         results = {}
         values = kwargs.get('values', {})
         for name, value in values.items():
             point = self.points.get(name)
@@ -1072,15 +1072,14 @@
         try:
             if len(read_items) > 0 and self._get_client():
                 self.wait_event = Event()
                 self._send_zongzhao(self._get_client())
                 if self.wait_event.wait(self.configs.get('timeout', 4)) is False:
                     raise Exception(f"response time out")
         except Exception as e:
-            self.logging(content=f"iec104 read fail({e.__str__()})", level='ERROR', pos=self.stack_pos)
             for read_item in read_items:
                 self.update_device(f"{self.configs.get('host')}:{self.configs.get('port')}", read_item, **self.gen_read_write_result(False, e.__str__()))
 
     def _write(self, type: int, address: int, value):
         raise NotImplementedError()
 
     def _release_client(self):
@@ -1180,15 +1179,15 @@
                 if value is not None:
                     return value
                 else:
                     raise Exception(f"value is none")
             else:
                 raise Exception(str(value))
         except Exception as e:
-            self.logging(content=f"get value({name}) fail({e.__str__()})", level='ERROR', source=name, pos=self.stack_pos)
+            self.update_results(name, False, e.__str__())
         return None
 
     def _send_frame(self, type_id: int, cause_id: int, datas: bytes):
         if self.client is not None:
             self.logging(content=f"iec104 send {self._get_frame_name(type_id, cause_id)}: [{self.client.format_bytes(datas)}]", pos=self.stack_pos)
             self.client.send(datas)
```

### Comparing `RobertCommonDriver-0.1.41/robertcommondriver/system/iot/iot_modbus.py` & `RobertCommonDriver-0.1.42/robertcommondriver/system/iot/iot_modbus.py`

 * *Files 2% similar despite different names*

```diff
@@ -203,16 +203,16 @@
                 ])
 
         return templates
 
     def read(self, **kwargs):
         self.update_info(used=IOTBaseCommon.get_datetime_str())
 
-        results = {}
         names = kwargs.get('names', list(self.points.keys()))
+        self.update_results(names, True, None)
         read_items = {}
         for name in names:
             point = self.points.get(name)
             if point:
                 device_address = point.get('point_device_address')
                 slave_id = point.get('point_slave_id')
                 fun_code = point.get('point_fun_code')
@@ -245,18 +245,18 @@
                 address = point.get('point_address')
                 data_type = point.get('point_data_type')
                 data_length = point.get('point_data_length', 0)
                 data_order = point.get('point_data_order', 0)
                 if device_address is not None and slave_id is not None and fun_code is not None and address is not None and data_type is not None and data_length is not None:
                     value = self.get_value(name, device_address, slave_id, fun_code, address, data_length, data_type, data_order)
                     if value is not None:
-                        results[name] = value
-
-        self.update_info(read=len(names), response=len(results))
-        return results
+                        self.update_results(name, True, value)
+            else:
+                self.update_results(name, False, 'UnExist')
+        return self.get_results()
 
     def write(self, **kwargs):
         self.update_info(used=IOTBaseCommon.get_datetime_str())
 
         results = {}
         values = kwargs.get('values', {})
         for name, value in values.items():
@@ -429,46 +429,44 @@
                 else:
                     fun_code = modbus_tk_defines.WRITE_MULTIPLE_COILS
         return fun_code
 
     def _send_read_cmd(self, address: str, slave_id: int, add_start: int, add_end: int, fun_code: int):
         err_msg = None
         try:
-            self.pending()
             fun_code = self._change_fun_code(fun_code)
             if self._get_client(address) is not None:
                 self.logging(content=f"modbus({address}) read ({slave_id}-{fun_code}-[{add_start}-{add_end}])", pos=self.stack_pos)
                 value_list = self._get_client(address).execute(slave_id, fun_code, add_start, add_end - add_start + 1)
                 for index in range(0, len(value_list)):
                     self.update_device(address, IOTModbus.gen_key(slave_id, fun_code, add_start + index), **self.gen_read_write_result(True, value_list[index]))
         except (socket_timeout, ConnectionRefusedError, ConnectionResetError) as e:  # connect
             err_msg = f"connect fail: {e.__str__()}"
             self._release_client(address)
         except Exception as e:  # other
             err_msg = e.__str__()
         finally:
             if err_msg is not None:
-                self.logging(content=f"modbus({address}) read ({slave_id}-{fun_code}-[{add_start}-{add_end}]) fail({err_msg})", level='ERROR', pos=self.stack_pos)
                 for i in range(add_start, add_end + 1):
                     self.update_device(address, IOTModbus.gen_key(slave_id, fun_code, i), **self.gen_read_write_result(False, err_msg))
 
     def _read_address(self, *args, **kwargs) -> dict:
         (address, slave_items) = args
         results = {}
         read_units = self.cread_read_units(address, slave_items)
         for k, modbus_units in read_units.items():
             for modbus_unit in modbus_units:
                 if modbus_unit.get_modbus_id >= 0 and 0 <= modbus_unit.get_modbus_start <= modbus_unit.get_modbus_end and 0 < modbus_unit.get_modbus_fun < 17:
                     self._send_read_cmd(modbus_unit.get_modbus_address, modbus_unit.get_modbus_id, modbus_unit.get_modbus_start, modbus_unit.get_modbus_end, modbus_unit.get_modbus_fun)
-            time.sleep(self.configs.get('cmd_interval', 0.3))
+            self.delay(self.configs.get('cmd_interval', 0.3))
         return results
 
     def _read(self, read_items: dict) -> dict:
         if len(read_items) > 0:
-            jobs = IOTBaseCommon.SimpleThreadPool(len(read_items))
+            jobs = IOTBaseCommon.SimpleThreadPool(len(read_items), f"{self}")
             for address, slaves in read_items.items():
                 jobs.submit_task(self._read_address, address, slaves)
             return jobs.done()
         return {}
     
     @staticmethod
     def convert_value(length: int, type: int, order: int, values: list = []):
@@ -495,15 +493,15 @@
                         values.append(value)
                     else:
                         raise Exception(f"({key}) is none")
                 else:
                     raise Exception(str(value))
             return IOTModbus.convert_value(length, type, order, values)
         except Exception as e:
-            self.logging(content=f"get value({name}) fail({e.__str__()})", level='ERROR', source=name, pos=self.stack_pos)
+            self.update_results(name, False, e.__str__())
         return None
 
     def _convert_value_to_vector(self, src_type: int, src_order: int, dst_type: int, value):
         if src_type == IOTBaseCommon.DataTransform.TypeFormat.BOOL_ARRAY.value:
             return value
         return IOTBaseCommon.DataTransform.convert_value(value, IOTBaseCommon.DataTransform.TypeFormat(src_type), IOTBaseCommon.DataTransform.TypeFormat(dst_type), format=IOTBaseCommon.DataTransform.DataFormat(src_order))
 
@@ -534,15 +532,14 @@
         except (socket_timeout, ConnectionRefusedError, ConnectionResetError) as e:  # connect
             err_msg = f"connect fail: {e.__str__()}"
             self._release_client(address)
         except Exception as e:  # other
             err_msg = e.__str__()
         finally:
             if err_msg is not None:
-                self.logging(content=f"modbus({address}) write ({slave_id}-{fun_code}-{start}) fail({err_msg})", level='ERROR', pos=self.stack_pos)
                 self.update_device(address, IOTModbus.gen_key(slave_id, fun_code, start), **self.gen_read_write_result(False, err_msg, False))
 
     def _get_server(self, address: str):
         server = self.servers.get(address, {}).get('server')
         if server is None:
             modbus_info = self._get_address_info(address)
             if 'type' in modbus_info.keys():
```

### Comparing `RobertCommonDriver-0.1.41/robertcommondriver/system/iot/iot_obix.py` & `RobertCommonDriver-0.1.42/robertcommondriver/system/iot/iot_obix.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,16 +48,17 @@
                 {'required': True, 'name': '过期时间' if lan == 'ch' else 'Reltime', 'code': 'reltime', 'type': 'string', 'default': 'PT30M', 'enum': [], 'tip': ''},
                 {'required': True, 'name': '最大点位限制' if lan == 'ch' else 'Limit', 'code': 'limit', 'type': 'int', 'default': 10000, 'enum': [], 'tip': ''},
                 {'required': True, 'name': '读取超时(s)' if lan == 'ch' else 'Timeout(s)', 'code': 'timeout', 'type': 'int', 'default': 30, 'enum': [], 'tip': ''}])
         return templates
 
     def read(self, **kwargs):
         self.update_info(used=IOTBaseCommon.get_datetime_str())
-        results = {}
         names = kwargs.get('names', list(self.points.keys()))
+        self.update_results(names, True, None)
+
         read_items = []
         for name in names:
             point = self.points.get(name)
             if point:
                 point_url = point.get('point_url')
                 if point_url is not None:
                     if not point_url.endswith('/'):
@@ -74,18 +75,18 @@
         for name in names:
             point = self.points.get(name)
             if point:
                 point_url = point.get('point_url')
                 point_type = point.get('point_type')
                 value = self.get_value(name, point_url, point_type)
                 if value is not None:
-                    results[name] = value
-
-        self.update_info(read=len(names), response=len(results))
-        return results
+                    self.update_results(name, True, value)
+            else:
+                self.update_results(name, False, 'UnExist')
+        return self.get_results()
 
     def write(self, **kwargs):
         self.update_info(used=IOTBaseCommon.get_datetime_str())
         results = {}
         values = kwargs.get('values', {})
         for name, value in values.items():
             point = self.points.get(name)
@@ -241,15 +242,14 @@
                     self._set_reltime()
 
                 self._add_points(items)
 
             self._pool_refresh()
         except Exception as e:
             self._del_watch()
-            self.logging(content=f"obix read fail({e.__str__()})", level='ERROR', pos=self.stack_pos)
             for item in items:
                 self.update_device(self.configs.get('url'), item, **self.gen_read_write_result(False, e.__str__()))
 
     def get_value(self, name: str, url: str, type: str):
         try:
             [result, value] = self.get_device_property(self.configs.get('url'), url, [self.get_read_quality, self.get_read_result])
             if result is True:
@@ -257,15 +257,15 @@
                     converter = self.converters.get(type, str)
                     return str(value) if type != 'bool' else str(int(converter(value)))
                 else:
                     raise Exception(f"({name}) is none")
             else:
                 raise Exception(str(value))
         except Exception as e:
-            self.logging(content=f"get value({name}) fail({e.__str__()})", level='ERROR', source=name, pos=self.stack_pos)
+            self.update_results(name, False, e.__str__())
         return None
 
     def _write(self, url: str, type: str, value):
         return IOTBaseCommon.send_request(url=f"{self.watch.get('url')}{url.replace('/out/', '/')}", data=f'<{type} val="{str(value).lower()}" />', method='POST', auth=HTTPBasicAuth(self.configs.get('username'), self.configs.get('password')), timeout=self.configs.get('timeout', 5)).success
 
     def _gen_name(self, point_url, folder_name) -> str:
         try:
```

### Comparing `RobertCommonDriver-0.1.41/robertcommondriver/system/iot/iot_opcda.py` & `RobertCommonDriver-0.1.42/robertcommondriver/system/iot/iot_opcda.py`

 * *Files 0% similar despite different names*

```diff
@@ -1045,15 +1045,15 @@
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.reinit()
 
     def reinit(self):
         self.exit_flag = False
-        IOTBaseCommon.function_thread(self.pump_wait_msg, False).start()
+        IOTBaseCommon.function_thread(self.pump_wait_msg, False, f"opcda pump").start()
 
     def exit(self):
         self.exit_flag = True
         self.close()
         self.reinit()
 
     @classmethod
@@ -1083,16 +1083,17 @@
             ])
         return templates
     
     # ##API#############
     def read(self, **kwargs):
         self.update_info(used=IOTBaseCommon.get_datetime_str())
 
-        results = {}
         names = kwargs.get('names', list(self.points.keys()))
+        self.update_results(names, True, None)
+
         read_items = []
         for name in names:
             point = self.points.get(name)
             if point:
                 tag = point.get('point_tag')
                 if tag is not None and tag not in read_items:
                     read_items.append(tag)
@@ -1101,18 +1102,18 @@
 
         for name in names:
             point = self.points.get(name)
             if point:
                 tag = point.get('point_tag')
                 value = self._get_value(name, tag)
                 if value is not None:
-                    results[name] = value
-
-        self.update_info(read=len(names), response=len(results))
-        return results
+                    self.update_results(name, True, value)
+            else:
+                self.update_results(name, False, 'UnExist')
+        return self.get_results()
 
     def write(self, **kwargs):
         self.update_info(used=IOTBaseCommon.get_datetime_str())
 
         results = {}
         write_items = {}
         values = kwargs.get('values', {})
@@ -1232,54 +1233,53 @@
             time.sleep(0.1)
 
     def _read(self, tags: list):
         try:
             if len(tags) > 0 and self._get_client():
                 chunk_tags = IOTBaseCommon.chunk_list(tags, self.configs.get('read_limit', 100))
                 for chunk_tag in chunk_tags:
+                    self.delay(0.0001)
                     values = self._get_client().read(self.configs.get('group'), chunk_tag, self.configs.get('action'))
                     for tag, value in values.items():
                         if isinstance(value, list):
                             if len(value) >= 4:
                                 (v, status, time, error, update) = value
                                 if status == 'Good':
                                     self.update_device(self.configs.get('server'), tag, **self.gen_read_write_result(True, v))
                                 else:
                                     self.update_device(self.configs.get('server'), tag, **self.gen_read_write_result(False, f"[{status}] {error}"))
                         else:
                             self.update_device(self.configs.get('server'), tag, **self.gen_read_write_result(False, f"{value}"))
         except Exception as e:
             for tag in tags:
                 self.update_device(self.configs.get('server'), tag, **self.gen_read_write_result(False, e.__str__()))
-            self.logging(content=f"opcda read fail({e.__str__()})", level='ERROR', pos=self.stack_pos)
 
     def _get_value(self, name: str, tag: str):
         try:
             [result, value] = self.get_device_property(self.configs.get('server'), tag, [self.get_read_quality, self.get_read_result])
             if result is True:
                 if value is not None:
                     return value
                 else:
                     raise Exception(f"value is none")
             else:
                 raise Exception(str(value))
         except Exception as e:
-            self.logging(content=f"get value({name}) fail({e.__str__()})", level='ERROR', source=name, pos=self.stack_pos)
+            self.update_results(name, False, e.__str__())
         return None
 
     def _write(self, set_values: dict):
         try:
             if len(set_values) > 0 and self._get_client():
                 values = self._get_client().write(self.configs.get('group'), set_values)
                 for tag, [status, result] in values.items():
                     self.update_device(self.configs.get('server'), tag, **self.gen_read_write_result(status, result, False))
         except Exception as e:
             for tag in set_values.keys():
                 self.update_device(self.configs.get('server'), tag, **self.gen_read_write_result(False, e.__str__(), False))
-            self.logging(content=f"opcda read fail({e.__str__()})", level='ERROR', pos=self.stack_pos)
 
     def close(self):
         if self.client is not None:
             self.client = self._release_client(self.client)
 
     def info(self, **kwargs):
         if self._get_client():
```

### Comparing `RobertCommonDriver-0.1.41/robertcommondriver/system/iot/iot_opcua.py` & `RobertCommonDriver-0.1.42/robertcommondriver/system/iot/iot_opcua.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,16 +95,16 @@
                 templates.append({'required': True, 'name': 'OPC服务名称' if lan == 'ch' else 'Name', 'code': 'name', 'type': 'string', 'default': 'OPCUAServer', 'enum': [], 'tip': ''})
                 templates.append({'required': True, 'name': 'OPC根目录' if lan == 'ch' else 'Root', 'code': 'root', 'type': 'string', 'default': 'Robert', 'enum': [], 'tip': ''})
         return templates
 
     def read(self, **kwargs):
         self.update_info(used=IOTBaseCommon.get_datetime_str())
 
-        results = {}
         names = kwargs.get('names', list(self.points.keys()))
+        self.update_results(names, True, None)
 
         read_items = []
         for name in names:
             point = self.points.get(name)
             if point:
                 node_id = point.get('point_node_id')
                 if node_id is not None:
@@ -118,17 +118,18 @@
             if point:
                 node_id = point.get('point_node_id')
                 if node_id is not None:
                     value = self.get_value(name, node_id)
                     if value is not None:
                         if isinstance(value, list):
                             value = value[0]
-                        results[name] = value
-        self.update_info(read=len(names), response=len(results))
-        return results
+                        self.update_results(name, True, value)
+            else:
+                self.update_results(name, False, 'UnExist')
+        return self.get_results()
 
     def write(self, **kwargs):
         self.update_info(used=IOTBaseCommon.get_datetime_str())
 
         results = {}
         values = kwargs.get('values', {})
         for name, value in values.items():
@@ -204,15 +205,15 @@
                 if value is not None:
                     return value
                 else:
                     raise Exception(f"value is none")
             else:
                 raise Exception(str(value))
         except Exception as e:
-            self.logging(content=f"get value({name}) fail({e.__str__()})", level='ERROR', source=name, pos=self.stack_pos)
+            self.update_results(name, False, e.__str__())
         return None
 
     def _get_client(self):
         if self.client is not None:
             try:
                 root = self.client.get_root_node().get_children()
             except Exception as e:
@@ -359,24 +360,22 @@
                                         self.update_device(self.configs.get('endpoint'), ids[index], sub_node=sub_node)
                                         self.subs.append(sub_node)
                                 self.logging(content=f"subscribe size({len(sub_nodes)})")
             except Exception as e:
                 self._release_client()
                 for item in read_items:
                     self.update_device(self.configs.get('endpoint'), item, **self.gen_read_write_result(False, e.__str__()))
-                self.logging(content=f"opcua read fail({e.__str__()})", level='ERROR', pos=self.stack_pos)
 
     def _write(self, node, value):
         try:
             if self._get_client():
                 self._get_client().get_node(node).set_value(ua.Variant(value))
                 self.update_device(self.configs.get('endpoint'), node, **self.gen_read_write_result(True, None, False))
         except Exception as e:
             self.update_device(self.configs.get('endpoint'), node, **self.gen_read_write_result(False, e.__str__(), False))
-            self.logging(content=f"opcua write({node}) fail({e.__str__()})", level='ERROR', pos=self.stack_pos)
 
     def _get_server(self):
         if self.server is None:
             server = Server()
             server.set_endpoint(self.configs.get('endpoint'))
             server.set_server_name(self.configs.get('name', 'Robert OPC UA Server'))
             # 设置客户端连接的所有可能端点策略
```

### Comparing `RobertCommonDriver-0.1.41/robertcommondriver/system/iot/iot_plc_ab.py` & `RobertCommonDriver-0.1.42/robertcommondriver/system/iot/iot_plc_ab.py`

 * *Files 2% similar despite different names*

```diff
@@ -656,16 +656,17 @@
                 ])
             templates.append({'required': True, 'name': '超时(s)' if lan == 'ch' else 'Timeout(s)', 'code': 'timeout', 'type': 'int', 'default': 15, 'enum': [], 'tip': ''})
         return templates
 
     def read(self, **kwargs):
         self.update_info(used=IOTBaseCommon.get_datetime_str())
 
-        results = {}
         names = kwargs.get('names', list(self.points.keys()))
+        self.update_results(names, True, None)
+
         read_items = {}
         for name in names:
             point = self.points.get(name)
             if point:
                 device_address = point.get('point_device_address')
                 address = point.get('point_address')
                 type = point.get('point_type')
@@ -682,18 +683,18 @@
             if point:
                 device_address = point.get('point_device_address')
                 address = point.get('point_address')
                 type = point.get('point_type')
                 if device_address is not None and address is not None and type is not None:
                     value = self._get_value(name, device_address, address, type)
                     if value is not None:
-                        results[name] = value
-
-        self.update_info(read=len(names), response=len(results))
-        return results
+                        self.update_results(name, True, value)
+            else:
+                self.update_results(name, False, 'UnExist')
+        return self.get_results()
 
     def write(self, **kwargs):
         self.update_info(used=IOTBaseCommon.get_datetime_str())
 
         results = {}
         values = kwargs.get('values', {})
         write_items = {}
@@ -787,28 +788,27 @@
                                 else:
                                     self.update_device(f"{address}", f"{item.contents[0]}_{item.contents[2]}", **self.gen_read_write_result(False, item.msg))
                     else:
                         raise Exception(f"{result.msg}")
         except Exception as e:
             for (ad, type) in ab_item_list:
                 self.update_device(f"{address}", f"{ad}_{type}", **self.gen_read_write_result(False, e.__str__()))
-            self.logging(content=f"plc({address}) read fail({e.__str__()})", level='ERROR', pos=self.stack_pos)
 
     def _read_address(self, *args, **kwargs) -> dict:
         (address, ab_items) = args
         results = {}
         units = IOTBaseCommon.chunk_list(ab_items, self.configs.get('multi_read'))
         for unit in units:
             self._send_read_cmd(address, unit)
             self.delay(self.configs.get('cmd_interval', 0.3))
         return results
 
     def _read(self, read_items: dict):
         if len(read_items) > 0:
-            jobs = IOTBaseCommon.SimpleThreadPool(len(read_items))
+            jobs = IOTBaseCommon.SimpleThreadPool(len(read_items), f"{self}")
             for address, ab_items in read_items.items():
                 jobs.submit_task(self._read_address, address, ab_items)
             return jobs.done()
         return {}
 
     def _get_value(self, name: str, device_address: str, address: str, type: int):
         try:
@@ -817,15 +817,15 @@
                 if value is not None:
                     return value
                 else:
                     raise Exception(f"value is none")
             else:
                 raise Exception(str(value))
         except Exception as e:
-            self.logging(content=f"get value({name}) fail({e.__str__()})", level='ERROR', source=name, pos=self.stack_pos)
+            self.update_results(name, False, e.__str__())
         return None
 
     def _send_write_cmd(self, address: str, ab_item_list: list):
         try:
             if self._get_client(address) is not None and len(ab_item_list) > 0:
                 result = self._get_client(address).write(ab_item_list)
                 if isinstance(result, IOTBaseCommon.IOTNetResult):
@@ -840,25 +840,24 @@
                                 else:
                                     self.update_device(f"{address}", f"{item.contents[0]}_{item.contents[2]}",  **self.gen_read_write_result(False, item.msg, False))
                     else:
                         raise Exception(f"{result.msg}")
         except Exception as e:
             for (ad, type, value) in ab_item_list:
                 self.update_device(f"{address}", f"{ad}_{type}", **self.gen_read_write_result(False, e.__str__(), False))
-            self.logging(content=f"plc({address}) write fail({e.__str__()})", level='ERROR', pos=self.stack_pos)
 
     def _write_address(self, *args, **kwargs) -> dict:
         (address, ab_items) = args
         results = {}
         units = IOTBaseCommon.chunk_list(ab_items, self.configs.get('multi_read'))
         for unit in units:
             self._send_write_cmd(address, unit)
             self.delay(self.configs.get('cmd_interval', 0.3))
         return results
 
     def _write(self, write_items: dict):
         if len(write_items) > 0:
-            jobs = IOTBaseCommon.SimpleThreadPool(len(write_items))
+            jobs = IOTBaseCommon.SimpleThreadPool(len(write_items), f"{self}")
             for address, ab_items in write_items.items():
                 jobs.submit_task(self._write_address, address, ab_items)
             return jobs.done()
         return {}
```

### Comparing `RobertCommonDriver-0.1.41/robertcommondriver/system/iot/iot_plc_mitsubishi.py` & `RobertCommonDriver-0.1.42/robertcommondriver/system/iot/iot_plc_mitsubishi.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 
 """
 https://www.cnblogs.com/dathlin/p/7469679.html
 FX5U配置：
     参数-FX5UCPU-模块参数-以太网端口
         SLMP连接设备-TCP
 
+小端方式
+
 地址：
     第一种，使用系统的类来标识，比如M200，写成(MelsecDataType.M, 200)的表示形式，这样也可以去MelsecDataType里面找到所有支持的数据类型。
     第二种，使用字符串表示，这个组件里所有的读写操作提供字符串表示的重载方法，所有的支持访问的类型对应如下，字符串的表示方式存在十进制和十六进制的区别：  
         输入继电器："X100","X1A0"            // 字符串为十六进制机制
         输出继电器："Y100" ,"Y1A0"           // 字符串为十六进制机制
         内部继电器："M100","M200"           // 字符串为十进制
         锁存继电器："L100"  ,"L200"           // 字符串为十进制
@@ -813,16 +815,17 @@
                 ])
             templates.append({'required': True, 'name': '超时(s)' if lan == 'ch' else 'Timeout(s)', 'code': 'timeout', 'type': 'int', 'default': 15, 'enum': [], 'tip': ''})
         return templates
 
     def read(self, **kwargs):
         self.update_info(used=IOTBaseCommon.get_datetime_str())
 
-        results = {}
         names = kwargs.get('names', list(self.points.keys()))
+        self.update_results(names, True, None)
+
         read_items = {}
         for name in names:
             point = self.points.get(name)
             if point:
                 device_address = point.get('point_device_address')
                 address = point.get('point_address')
                 type = point.get('point_type')
@@ -839,18 +842,18 @@
             if point:
                 device_address = point.get('point_device_address')
                 address = point.get('point_address')
                 type = point.get('point_type')
                 if device_address is not None and address is not None and type is not None:
                     value = self._get_value(name, device_address, address, type)
                     if value is not None:
-                        results[name] = value
-
-        self.update_info(read=len(names), response=len(results))
-        return results
+                        self.update_results(name, True, value)
+            else:
+                self.update_results(name, False, 'UnExist')
+        return self.get_results()
 
     def write(self, **kwargs):
         self.update_info(used=IOTBaseCommon.get_datetime_str())
 
         results = {}
         values = kwargs.get('values', {})
         write_items = {}
@@ -944,28 +947,27 @@
                                 else:
                                     self.update_device(f"{address}", f"{item.contents[0]}_{item.contents[7]}", **self.gen_read_write_result(False, item.msg))
                     else:
                         raise Exception(f"{result.msg}")
         except Exception as e:
             for (ad, type) in mitsubishi_list:
                 self.update_device(f"{address}", f"{ad}_{type}", **self.gen_read_write_result(False, e.__str__()))
-            self.logging(content=f"plc({address}) read fail({e.__str__()})", level='ERROR', pos=self.stack_pos)
 
     def _read_address(self, *args, **kwargs) -> dict:
         (address, mitsubishis) = args
         results = {}
         units = IOTBaseCommon.chunk_list(mitsubishis, self.configs.get('multi_read'))
         for unit in units:
             self._send_read_cmd(address, unit)
             self.delay(self.configs.get('cmd_interval', 0.3))
         return results
 
     def _read(self, read_items: dict):
         if len(read_items) > 0:
-            jobs = IOTBaseCommon.SimpleThreadPool(len(read_items))
+            jobs = IOTBaseCommon.SimpleThreadPool(len(read_items), f"{self}")
             for address, mitsubishis in read_items.items():
                 jobs.submit_task(self._read_address, address, mitsubishis)
             return jobs.done()
         return {}
 
     def _get_value(self, name: str, device_address: str, address: str, type: int):
         try:
@@ -974,15 +976,15 @@
                 if value is not None:
                     return value
                 else:
                     raise Exception(f"value is none")
             else:
                 raise Exception(str(value))
         except Exception as e:
-            self.logging(content=f"get value({name}) fail({e.__str__()})", level='ERROR', source=name, pos=self.stack_pos)
+            self.update_results(name, False, e.__str__())
         return None
 
     def _send_write_cmd(self, address: str, mitsubishi_list: list):
         try:
             if self._get_client(address) is not None and len(mitsubishi_list) > 0:
                 result = self._get_client(address).write(mitsubishi_list)
                 if isinstance(result, IOTBaseCommon.IOTNetResult):
@@ -997,28 +999,27 @@
                                 else:
                                     self.update_device(f"{address}", f"{item.contents[0]}_{item.contents[7]}",  **self.gen_read_write_result(False, item.msg, False))
                     else:
                         raise Exception(f"{result.msg}")
         except Exception as e:
             for (ad, type, value) in mitsubishi_list:
                 self.update_device(f"{address}", f"{ad}_{type}", **self.gen_read_write_result(False, e.__str__(), False))
-            self.logging(content=f"plc({address}) write fail({e.__str__()})", level='ERROR', pos=self.stack_pos)
 
     def _write_address(self, *args, **kwargs) -> dict:
         (address, mitsubishis) = args
         results = {}
         units = IOTBaseCommon.chunk_list(mitsubishis, self.configs.get('multi_read'))
         for unit in units:
             self._send_write_cmd(address, unit)
             self.delay(self.configs.get('cmd_interval', 0.3))
         return results
 
     def _write(self, write_items: dict):
         if len(write_items) > 0:
-            jobs = IOTBaseCommon.SimpleThreadPool(len(write_items))
+            jobs = IOTBaseCommon.SimpleThreadPool(len(write_items), f"{self}")
             for address, mitsubishis in write_items.items():
                 jobs.submit_task(self._write_address, address, mitsubishis)
             return jobs.done()
         return {}
 
     def _release_server(self, address: str):
         try:
```

### Comparing `RobertCommonDriver-0.1.41/robertcommondriver/system/iot/iot_plc_omron.py` & `RobertCommonDriver-0.1.42/robertcommondriver/system/iot/iot_plc_omron.py`

 * *Files 1% similar despite different names*

```diff
@@ -576,16 +576,17 @@
                 ])
             templates.append({'required': True, 'name': '超时(s)' if lan == 'ch' else 'Timeout(s)', 'code': 'timeout', 'type': 'int', 'default': 15, 'enum': [], 'tip': ''})
         return templates
 
     def read(self, **kwargs):
         self.update_info(used=IOTBaseCommon.get_datetime_str())
 
-        results = {}
         names = kwargs.get('names', list(self.points.keys()))
+        self.update_results(names, True, None)
+
         read_items = {}
         for name in names:
             point = self.points.get(name)
             if point:
                 device_address = point.get('point_device_address')
                 address = point.get('point_address')
                 type = point.get('point_type')
@@ -602,18 +603,18 @@
             if point:
                 device_address = point.get('point_device_address')
                 address = point.get('point_address')
                 type = point.get('point_type')
                 if device_address is not None and address is not None and type is not None:
                     value = self._get_value(name, device_address, address, type)
                     if value is not None:
-                        results[name] = value
-
-        self.update_info(read=len(names), response=len(results))
-        return results
+                        self.update_results(name, True, value)
+            else:
+                self.update_results(name, False, 'UnExist')
+        return self.get_results()
 
     def write(self, **kwargs):
         self.update_info(used=IOTBaseCommon.get_datetime_str())
 
         results = {}
         values = kwargs.get('values', {})
         write_items = {}
@@ -733,28 +734,27 @@
                                 else:
                                     self.update_device(f"{address}", f"{item.contents[0]}_{item.contents[7]}", **self.gen_read_write_result(False, item.msg))
                     else:
                         raise Exception(f"{result.msg}")
         except Exception as e:
             for (ad, type) in omron_item_list:
                 self.update_device(f"{address}", f"{ad}_{type}", **self.gen_read_write_result(False, e.__str__()))
-            self.logging(content=f"plc({address}) read fail({e.__str__()})", level='ERROR', pos=self.stack_pos)
 
     def _read_address(self, *args, **kwargs) -> dict:
         (address, omron_items) = args
         results = {}
         units = IOTBaseCommon.chunk_list(omron_items, self.configs.get('multi_read'))
         for unit in units:
             self._send_read_cmd(address, unit)
             self.delay(self.configs.get('cmd_interval', 0.3))
         return results
 
     def _read(self, read_items: dict):
         if len(read_items) > 0:
-            jobs = IOTBaseCommon.SimpleThreadPool(len(read_items))
+            jobs = IOTBaseCommon.SimpleThreadPool(len(read_items), f"{self}")
             for address, omron_items in read_items.items():
                 jobs.submit_task(self._read_address, address, omron_items)
             return jobs.done()
         return {}
 
     def _get_value(self, name: str, device_address: str, address: str, type: int):
         try:
@@ -763,15 +763,15 @@
                 if value is not None:
                     return value
                 else:
                     raise Exception(f"value is none")
             else:
                 raise Exception(str(value))
         except Exception as e:
-            self.logging(content=f"get value({name}) fail({e.__str__()})", level='ERROR', source=name, pos=self.stack_pos)
+            self.update_results(name, False, e.__str__())
         return None
 
     def _send_write_cmd(self, address: str, omron_item_list: list):
         try:
             if self._get_client(address) is not None and len(omron_item_list) > 0:
                 result = self._get_client(address).write(omron_item_list)
                 if isinstance(result, IOTBaseCommon.IOTNetResult):
@@ -786,28 +786,27 @@
                                 else:
                                     self.update_device(f"{address}", f"{item.contents[0]}_{item.contents[7]}",  **self.gen_read_write_result(False, item.msg, False))
                     else:
                         raise Exception(f"{result.msg}")
         except Exception as e:
             for (ad, type, value) in omron_item_list:
                 self.update_device(f"{address}", f"{ad}_{type}", **self.gen_read_write_result(False, e.__str__(), False))
-            self.logging(content=f"plc({address}) write fail({e.__str__()})", level='ERROR', pos=self.stack_pos)
 
     def _write_address(self, *args, **kwargs) -> dict:
         (address, omron_items) = args
         results = {}
         units = IOTBaseCommon.chunk_list(omron_items, self.configs.get('multi_read'))
         for unit in units:
             self._send_write_cmd(address, unit)
             self.delay(self.configs.get('cmd_interval', 0.3))
         return results
 
     def _write(self, write_items: dict):
         if len(write_items) > 0:
-            jobs = IOTBaseCommon.SimpleThreadPool(len(write_items))
+            jobs = IOTBaseCommon.SimpleThreadPool(len(write_items), f"{self}")
             for address, omron_items in write_items.items():
                 jobs.submit_task(self._write_address, address, omron_items)
             return jobs.done()
         return {}
 
     def _get_server(self, address: str):
         server = self.servers.get(address, {}).get('server')
```

### Comparing `RobertCommonDriver-0.1.41/robertcommondriver/system/iot/iot_plc_s7.py` & `RobertCommonDriver-0.1.42/robertcommondriver/system/iot/iot_plc_s7.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,18 @@
 '''
 pip install python-snap7==0.10
 
 Note：
     snap7_server需要使用64位环境
     最大连读个数20
     指定dll位置
-    
+    大端模式
+        网络传输一般采用大端序，也被称之为网络字节序，或网络序。IP协议中定义大端序为网络字节序。
+        高字节放在内存的地地址
+        
     windows:
         snap7.dll is added to the python installation directory or any directory in the system environment
 
     linux install dll 
         下载压缩包:
             https://sourceforge.net/projects/snap7/files/下载snap7-full-1.4.2.7z
         
@@ -276,16 +279,17 @@
                     {'required': True, 'name': '接收超时(ms)' if lan == 'ch' else 'Recv Timeout(ms)', 'code': 'rec_timeout', 'type': 'int', 'default': 3500, 'enum': [], 'tip': ''},
                 ])
         return templates
 
     def read(self, **kwargs):
         self.update_info(used=IOTBaseCommon.get_datetime_str())
 
-        results = {}
         names = kwargs.get('names', list(self.points.keys()))
+        self.update_results(names, True, None)
+
         read_items = {}
         for name in names:
             point = self.points.get(name)
             if point:
                 device_address = point.get('point_device_address')
                 address = point.get('point_address')
                 if device_address is not None and address is not None:
@@ -300,18 +304,18 @@
             point = self.points.get(name)
             if point:
                 device_address = point.get('point_device_address')
                 address = point.get('point_address')
                 if device_address is not None and address is not None:
                     value = self.get_value(name, device_address, address)
                     if value is not None:
-                        results[name] = value
-
-        self.update_info(read=len(names), response=len(results))
-        return results
+                        self.update_results(name, True, value)
+            else:
+                self.update_results(name, False, 'UnExist')
+        return self.get_results()
 
     def write(self, **kwargs):
         self.update_info(used=IOTBaseCommon.get_datetime_str())
 
         results = {}
         values = kwargs.get('values', {})
         for name, value in values.items():
@@ -436,34 +440,32 @@
                     try:
                         if s7_item.Result:
                             raise Exception(error_text(s7_item.Result))
                         else:
                             self._parse_result(address, s7_key, s7_item)
                     except Exception as e:
                         self.update_device(address, s7_key, **self.gen_read_write_result(False, e.__str__()))
-                        self.logging(content=f"plc({address}) read{'' if process is None else f'({process})'} ({s7_key}) fail({e.__str__()})", level='ERROR', pos=self.stack_pos)
         except Exception as e:
             for s7_item in s7_item_list:
                 self.update_device(address, self._gen_key(s7_item.Area, s7_item.DBNumber, s7_item.Start, s7_item.Amount), **self.gen_read_write_result(False, e.__str__()))
-            self.logging(content=f"plc({address}) read{'' if process is None else f'({process})'} fail({e.__str__()})", level='ERROR', pos=self.stack_pos)
 
     def _read_address(self, *args, **kwargs) -> dict:
         (address, s7_items) = args
         results = {}
         read_units = self._cread_read_units(address, sorted(s7_items))
 
         units = list(IOTBaseCommon.chunk_list(list(read_units.values()), self.configs.get('multi_read')))
         for i, unit in enumerate(units):
             self._send_read_cmd(address, unit, f"{i}/{len(units)}")
             self.delay(self.configs.get('cmd_interval', 0.3))
         return results
 
     def _read(self, read_items: dict):
         if len(read_items) > 0:
-            jobs = IOTBaseCommon.SimpleThreadPool(len(read_items))
+            jobs = IOTBaseCommon.SimpleThreadPool(len(read_items), f"{self}")
             for address, s7_items in read_items.items():
                 jobs.submit_task(self._read_address, address, s7_items)
             return jobs.done()
         return {}
 
     def _get_s7_item(self, address: str):
         # DB2,REAL10,VT_R4 I0.6
@@ -566,15 +568,15 @@
                     else:
                         return value
                 else:
                     raise Exception(f"value is none")
             else:
                 raise Exception(str(value))
         except Exception as e:
-            self.logging(content=f"get value({name}) fail({e.__str__()})", level='ERROR', source=name, pos=self.stack_pos)
+            self.update_results(name, False, e.__str__())
         return None
 
     def _conver_set_data_value(self, reading, value, type, addr):
         if type == IOTBaseCommon.DataTransform.TypeFormat.BOOL:
             snap7_util.set_bool(reading, 0, addr, bool(int(str(value))))
         else:
             reading = bytearray(IOTBaseCommon.DataTransform.convert_values_to_bytes(value, type, little_endian=False))
@@ -594,15 +596,14 @@
                 result[0] = self._get_client(device_address).write_area(area, db, start, reading)
                 return self.update_device(device_address, s7_key, **self.gen_read_write_result(True, None, False))
             err_msg = 'Unknown'
         except Exception as e:  # other
             err_msg = e.__str__()
         finally:
             if err_msg is not None:
-                self.logging(content=f"plc({device_address}) write({s7_key}) fail({err_msg})", level='ERROR', pos=self.stack_pos)
                 self.update_device(device_address, s7_key, **self.gen_read_write_result(False, err_msg, False))
 
     def _get_server(self, port: int = 102):
         server = self.servers.get(port, {}).get('server')
         if server is None:
             self._load_library()
             server = snap7_server.Server()
```

### Comparing `RobertCommonDriver-0.1.41/robertcommondriver/system/iot/iot_plc_siemens.py` & `RobertCommonDriver-0.1.42/robertcommondriver/system/iot/iot_plc_siemens.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 from enum import Enum
 
 from typing import List, Dict, Any, Union, Optional
 
 from .base import IOTBaseCommon, IOTDriver
 
 """
+大端模式
+        网络传输一般采用大端序，也被称之为网络字节序，或网络序。IP协议中定义大端序为网络字节序。
+        高字节放在内存的地地址
+        
 点地址
     6/192.168.1.172/102/0/1
 
 rack是机架号，slot卡槽号
     s7-200 0, 1
     s7-300 0, 2
     s7-400 具体看硬件组态
@@ -644,14 +648,16 @@
         return templates
 
     def read(self, **kwargs):
         self.update_info(used=IOTBaseCommon.get_datetime_str())
 
         results = {}
         names = kwargs.get('names', list(self.points.keys()))
+        self.update_results(names, True, None)
+
         read_items = {}
         for name in names:
             point = self.points.get(name)
             if point:
                 device_address = point.get('point_device_address')
                 address = point.get('point_address')
                 type = point.get('point_type')
@@ -668,18 +674,18 @@
             if point:
                 device_address = point.get('point_device_address')
                 address = point.get('point_address')
                 type = point.get('point_type')
                 if device_address is not None and address is not None and type is not None:
                     value = self._get_value(name, device_address, address, type)
                     if value is not None:
-                        results[name] = value
-
-        self.update_info(read=len(names), response=len(results))
-        return results
+                        self.update_results(name, True, value)
+            else:
+                self.update_results(name, False, 'UnExist')
+        return self.get_results()
 
     def write(self, **kwargs):
         self.update_info(used=IOTBaseCommon.get_datetime_str())
 
         results = {}
         values = kwargs.get('values', {})
         write_items = {}
@@ -799,28 +805,27 @@
                                 else:
                                     self.update_device(f"{address}", f"{item.contents[0]}_{item.contents[6]}", **self.gen_read_write_result(False, item.msg))
                     else:
                         raise Exception(f"{result.msg}")
         except Exception as e:
             for (ad, type) in s7_item_list:
                 self.update_device(f"{address}", f"{ad}_{type}", **self.gen_read_write_result(False, e.__str__()))
-            self.logging(content=f"plc({address}) read fail({e.__str__()})", level='ERROR', pos=self.stack_pos)
 
     def _read_address(self, *args, **kwargs) -> dict:
         (address, s7_items) = args
         results = {}
         units = IOTBaseCommon.chunk_list(s7_items, self.configs.get('multi_read'))
         for unit in units:
             self._send_read_cmd(address, unit)
             self.delay(self.configs.get('cmd_interval', 0.3))
         return results
 
     def _read(self, read_items: dict):
         if len(read_items) > 0:
-            jobs = IOTBaseCommon.SimpleThreadPool(len(read_items))
+            jobs = IOTBaseCommon.SimpleThreadPool(len(read_items), f"{self}")
             for address, s7_items in read_items.items():
                 jobs.submit_task(self._read_address, address, s7_items)
             return jobs.done()
         return {}
 
     def _get_value(self, name: str, device_address: str, address: str, type: int):
         try:
@@ -829,15 +834,15 @@
                 if value is not None:
                     return value
                 else:
                     raise Exception(f"value is none")
             else:
                 raise Exception(str(value))
         except Exception as e:
-            self.logging(content=f"get value({name}) fail({e.__str__()})", level='ERROR', source=name, pos=self.stack_pos)
+            self.update_results(name, False, e.__str__())
         return None
 
     def _send_write_cmd(self, address: str, s7_item_list: list):
         try:
             if self._get_client(address) is not None and len(s7_item_list) > 0:
                 result = self._get_client(address).write(s7_item_list)
                 if isinstance(result, IOTBaseCommon.IOTNetResult):
@@ -852,28 +857,27 @@
                                 else:
                                     self.update_device(f"{address}", f"{item.contents[0]}_{item.contents[6]}",  **self.gen_read_write_result(False, item.msg, False))
                     else:
                         raise Exception(f"{result.msg}")
         except Exception as e:
             for (ad, type, value) in s7_item_list:
                 self.update_device(f"{address}", f"{ad}_{type}", **self.gen_read_write_result(False, e.__str__(), False))
-            self.logging(content=f"plc({address}) write fail({e.__str__()})", level='ERROR', pos=self.stack_pos)
 
     def _write_address(self, *args, **kwargs) -> dict:
         (address, s7_items) = args
         results = {}
         units = IOTBaseCommon.chunk_list(s7_items, self.configs.get('multi_read'))
         for unit in units:
             self._send_write_cmd(address, unit)
             self.delay(self.configs.get('cmd_interval', 0.3))
         return results
 
     def _write(self, write_items: dict):
         if len(write_items) > 0:
-            jobs = IOTBaseCommon.SimpleThreadPool(len(write_items))
+            jobs = IOTBaseCommon.SimpleThreadPool(len(write_items), f"{self}")
             for address, s7_items in write_items.items():
                 jobs.submit_task(self._write_address, address, s7_items)
             return jobs.done()
         return {}
 
     def _get_server(self, address: str):
         server = self.servers.get(address, {}).get('server')
```

### Comparing `RobertCommonDriver-0.1.41/robertcommondriver/system/iot/iot_snmp.py` & `RobertCommonDriver-0.1.42/robertcommondriver/system/iot/iot_snmp.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,16 +41,17 @@
             ])
 
         return templates
 
     def read(self, **kwargs):
         self.update_info(used=IOTBaseCommon.get_datetime_str())
 
-        results = {}
         names = kwargs.get('names', list(self.points.keys()))
+        self.update_results(names, True, None)
+
         read_items = {}
         for name in names:
             point = self.points.get(name)
             if point:
                 oid = point.get('point_oid')
                 device_host = point.get('point_device_address')    # 192.168.1.200/161/v1/public/private
                 if oid is not None and device_host is not None:
@@ -66,18 +67,19 @@
             point = self.points.get(name)
             if point:
                 oid = point.get('point_oid')
                 device_host = point.get('point_device_address')  # 192.168.1.200/161/v1/public/private
                 if oid is not None and device_host is not None:
                     value = self._get_value(name, device_host, oid)
                     if value is not None:
-                        results[name] = value
+                        self.update_results(name, True, value)
+            else:
+                self.update_results(name, False, 'UnExist')
+        return self.get_results()
 
-        self.update_info(read=len(names), response=len(results))
-        return results
 
     def write(self, **kwargs):
         self.update_info(used=IOTBaseCommon.get_datetime_str())
         results = {}
         values = kwargs.get('values', {})
         for name, value in values.items():
             point = self.points.get(name)
@@ -101,15 +103,15 @@
         self.update_info(used=IOTBaseCommon.get_datetime_str())
         return self._ping(kwargs.get('host'), port=kwargs.get('port', 161), comunity=kwargs.get('comunity', 'public'))
 
     def discover(self, **kwargs):
         self.update_info(used=IOTBaseCommon.get_datetime_str())
         networks = IOTBaseCommon.get_networks(kwargs.get('address'))
         self.logging(content=f"discover({kwargs.get('address')})")
-        jobs = IOTBaseCommon.SimpleThreadPool(kwargs.get('limit', 40))
+        jobs = IOTBaseCommon.SimpleThreadPool(kwargs.get('limit', 40), f"{self}")
         for ip in networks:
             jobs.submit_task(self._discover, host=ip)
         results = jobs.done(False)
         self.update_info(discover=len(results))
         return results
 
     def scan(self, **kwargs):
@@ -119,15 +121,15 @@
         root = kwargs.get('root', '1.3')
         self.logging(content=f"scan({address}) {root}")
         try:
             auth, transport, context = self._get_connect_info(address)
             for (error, status, index, var_binds) in bulkCmd(SnmpEngine(), auth, transport, context, 0, 25, ObjectType(ObjectIdentity(root)), lookupMib=False, lexicographicMode=False, ignoreNonIncreasingOid=True):
                 if error:
                     self.logging(content=f"scan({address}) fail({error})", level='ERROR')
-                    break
+                    continue
                 if not status:
                     for var_bind in var_binds:
                         name = IOTBaseCommon.format_name(var_bind[0].prettyPrint())
                         value = var_bind[1].prettyPrint()
                         type = var_bind[1].__class__.__name__
                         results[name] = self.create_point(point_name=name, point_name_alias=name, point_device_address=address, point_oid=name, point_type=type, point_description=name, point_value=value)
                         self.logging(content=f"recv {len(results)} point({name})")
@@ -156,15 +158,15 @@
         )
         if not error and not status:
             return True
         return False
 
     def _read(self, read_items: dict):
         if len(read_items) > 0:
-            jobs = IOTBaseCommon.SimpleThreadPool(len(read_items))
+            jobs = IOTBaseCommon.SimpleThreadPool(len(read_items), f"{self}")
             for address, oids in read_items.items():
                 jobs.submit_task(self._read_oids, address, oids)
             return jobs.done()
         return {}
 
     def _get_connect_info(self, address: str):
         infos = address.split('/')  # '192.168.1.200/161/v1/public/private'
@@ -194,15 +196,14 @@
                 elif status:
                     raise Exception(f"{status.prettyPrint()} at {index and var_binds[int(index) - 1][0] or '?'}")
                 else:
                     for var_bind in var_binds:
                         print(' = '.join([x.prettyPrint() for x in var_bind]))
                         self.update_device(f"{address}", str(var_bind[0]), **self.gen_read_write_result(True, var_bind[1].prettyPrint()))
             except Exception as e:
-                self.logging(content=f"snmp read fail({e.__str__()})", level='ERROR', pos=self.stack_pos)
                 for id in oid:
                     self.update_device(f"{address}", str(id[0]), **self.gen_read_write_result(False, e.__str__()))
             self.delay(self.configs.get('cmd_interval', 1))
         return results
 
     def _write(self, address: str, oid: str, value):
         try:
@@ -228,9 +229,9 @@
                 if value is not None:
                     return value
                 else:
                     raise Exception(f"value is none")
             else:
                 raise Exception(str(value))
         except Exception as e:
-            self.logging(content=f"get value({name}) fail({e.__str__()})", level='ERROR', source=name, pos=self.stack_pos)
+            self.update_results(name, False, e.__str__())
         return None
```

### Comparing `RobertCommonDriver-0.1.41/setup.py` & `RobertCommonDriver-0.1.42/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 # Package meta-data.
 NAME = 'RobertCommonDriver'
 DESCRIPTION = 'Robert Common Driver Library'
 URL = 'https://github.com/hun0423/RobertCommonDriver'
 EMAIL = '851010070@qq.com'
 AUTHOR = 'Robert0423'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.1.41'
-DATE = '2023-05-26'
+VERSION = '0.1.42'
+DATE = '2023-06-09'
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
 }
 
 # The rest you shouldn't have to touch too much :)
```

### Comparing `RobertCommonDriver-0.1.41/tests/test_system/test_driver/test_bacnet.py` & `RobertCommonDriver-0.1.42/tests/test_system/test_driver/test_bacnet.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.41/tests/test_system/test_driver/test_bacnet1.py` & `RobertCommonDriver-0.1.42/tests/test_system/test_driver/test_bacnet1.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.41/tests/test_system/test_driver/test_bacnetc.py` & `RobertCommonDriver-0.1.42/tests/test_system/test_driver/test_bacnetc.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.41/tests/test_system/test_driver/test_bacnetv1.py` & `RobertCommonDriver-0.1.42/tests/test_system/test_driver/test_bacnetv1.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.41/tests/test_system/test_driver/test_modbus.py` & `RobertCommonDriver-0.1.42/tests/test_system/test_driver/test_modbus.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.41/tests/test_system/test_driver/test_obix.py` & `RobertCommonDriver-0.1.42/tests/test_system/test_driver/test_obix.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.41/tests/test_system/test_driver/test_opcda.py` & `RobertCommonDriver-0.1.42/tests/test_system/test_driver/test_opcda.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.41/tests/test_system/test_driver/test_opcua.py` & `RobertCommonDriver-0.1.42/tests/test_system/test_driver/test_opcua.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.41/tests/test_system/test_driver/test_plcs7.py` & `RobertCommonDriver-0.1.42/tests/test_system/test_driver/test_plcs7.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.41/tests/test_system/test_driver/test_snmp.py` & `RobertCommonDriver-0.1.42/tests/test_system/test_driver/test_snmp.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.41/tests/test_system/test_iot/test_bacnet1.py` & `RobertCommonDriver-0.1.42/tests/test_system/test_iot/test_bacnet1.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.41/tests/test_system/test_iot/test_iot_bacnet.py` & `RobertCommonDriver-0.1.42/tests/test_system/test_iot/test_iot_bacnet.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.41/tests/test_system/test_iot/test_iot_bacnet_mstp.py` & `RobertCommonDriver-0.1.42/tests/test_system/test_iot/test_iot_bacnet_mstp.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.41/tests/test_system/test_iot/test_iot_iec104.py` & `RobertCommonDriver-0.1.42/tests/test_system/test_iot/test_iot_iec104.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.41/tests/test_system/test_iot/test_iot_modbus.py` & `RobertCommonDriver-0.1.42/tests/test_system/test_iot/test_iot_modbus.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.41/tests/test_system/test_iot/test_iot_obix.py` & `RobertCommonDriver-0.1.42/tests/test_system/test_iot/test_iot_obix.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,17 +69,16 @@
                 result = driver.read()  # 读取点
                 print(result)
         except Exception as e:
             print(e.__str__())
         time.sleep(35)
 
 
-
 def test_scan():
     driver = IOTObix(configs={'username': 'colliers', 'password': 'C0ll1ers!', 'url': 'https://58.28.208.154:52443', 'filiter': ['obix:Point'], 'timeout': 20}, points={})
     driver.logging(call_logging=logging_print)
     if driver.ping() is True:
         result = driver.scan(limit=10)  # 读取点
-        values_to_csv(result, 'test.csv', False, True)
+        values_to_csv(result, 'queen.csv', False, True)
 
 
-test_read_queen()
+test_scan()
```

### Comparing `RobertCommonDriver-0.1.41/tests/test_system/test_iot/test_iot_opcda.py` & `RobertCommonDriver-0.1.42/tests/test_system/test_iot/test_iot_opcda.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.41/tests/test_system/test_iot/test_iot_opcua.py` & `RobertCommonDriver-0.1.42/tests/test_system/test_iot/test_iot_opcua.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.41/tests/test_system/test_iot/test_iot_plc_ab.py` & `RobertCommonDriver-0.1.42/tests/test_system/test_iot/test_iot_plc_ab.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.41/tests/test_system/test_iot/test_iot_plc_mitsubishi.py` & `RobertCommonDriver-0.1.42/tests/test_system/test_iot/test_iot_plc_mitsubishi.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.41/tests/test_system/test_iot/test_iot_plc_omron.py` & `RobertCommonDriver-0.1.42/tests/test_system/test_iot/test_iot_plc_omron.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.41/tests/test_system/test_iot/test_iot_plc_s7.py` & `RobertCommonDriver-0.1.42/tests/test_system/test_iot/test_iot_plc_s7.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.41/tests/test_system/test_iot/test_iot_plc_siemens.py` & `RobertCommonDriver-0.1.42/tests/test_system/test_iot/test_iot_plc_siemens.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.41/tests/test_system/test_iot/test_iot_snmp.py` & `RobertCommonDriver-0.1.42/tests/test_system/test_iot/test_iot_snmp.py`

 * *Files identical despite different names*

