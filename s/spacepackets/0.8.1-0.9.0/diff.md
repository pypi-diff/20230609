# Comparing `tmp/spacepackets-0.8.1.tar.gz` & `tmp/spacepackets-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacepackets-0.8.1.tar", last modified: Tue May 24 12:08:02 2022, max compression
+gzip compressed data, was "spacepackets-0.9.0.tar", last modified: Tue Jun 14 09:18:44 2022, max compression
```

## Comparing `spacepackets-0.8.1.tar` & `spacepackets-0.9.0.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2022-05-24 12:08:02.771844 spacepackets-0.8.1/
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)    11357 2021-11-19 13:24:54.000000 spacepackets-0.8.1/LICENSE
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      629 2022-05-20 11:15:37.000000 spacepackets-0.8.1/NOTICE
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     7040 2022-05-24 12:08:02.771844 spacepackets-0.8.1/PKG-INFO
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     5433 2022-05-20 11:15:37.000000 spacepackets-0.8.1/README.md
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      103 2021-11-19 13:24:54.000000 spacepackets-0.8.1/pyproject.toml
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     1176 2022-05-24 12:08:02.771844 spacepackets-0.8.1/setup.cfg
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      328 2021-11-19 13:24:54.000000 spacepackets-0.8.1/setup.py
-drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2022-05-24 12:08:02.767844 spacepackets-0.8.1/spacepackets/
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)       22 2022-05-24 12:07:06.000000 spacepackets-0.8.1/spacepackets/__init__.py
-drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2022-05-24 12:08:02.767844 spacepackets-0.8.1/spacepackets/ccsds/
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)       43 2022-05-20 11:15:37.000000 spacepackets-0.8.1/spacepackets/ccsds/__init__.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)    10742 2022-05-20 11:15:37.000000 spacepackets-0.8.1/spacepackets/ccsds/spacepacket.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     4511 2022-05-20 11:15:37.000000 spacepackets-0.8.1/spacepackets/ccsds/time.py
-drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2022-05-24 12:08:02.767844 spacepackets-0.8.1/spacepackets/cfdp/
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      100 2022-05-20 11:15:37.000000 spacepackets-0.8.1/spacepackets/cfdp/__init__.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     3425 2022-05-20 11:15:37.000000 spacepackets-0.8.1/spacepackets/cfdp/conf.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     2924 2022-05-20 11:15:37.000000 spacepackets-0.8.1/spacepackets/cfdp/definitions.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     1410 2022-05-20 11:15:37.000000 spacepackets-0.8.1/spacepackets/cfdp/lv.py
-drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2022-05-24 12:08:02.771844 spacepackets-0.8.1/spacepackets/cfdp/pdu/
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      481 2022-05-20 11:15:37.000000 spacepackets-0.8.1/spacepackets/cfdp/pdu/__init__.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     3320 2022-05-20 11:15:37.000000 spacepackets-0.8.1/spacepackets/cfdp/pdu/ack.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     4157 2022-05-20 11:15:37.000000 spacepackets-0.8.1/spacepackets/cfdp/pdu/eof.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     6099 2022-05-20 11:15:37.000000 spacepackets-0.8.1/spacepackets/cfdp/pdu/file_data.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     5831 2022-05-20 11:15:37.000000 spacepackets-0.8.1/spacepackets/cfdp/pdu/file_directive.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     7559 2022-05-20 11:15:37.000000 spacepackets-0.8.1/spacepackets/cfdp/pdu/finished.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)    10465 2022-05-20 11:15:37.000000 spacepackets-0.8.1/spacepackets/cfdp/pdu/header.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     3159 2022-05-20 11:15:37.000000 spacepackets-0.8.1/spacepackets/cfdp/pdu/keep_alive.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     6982 2022-05-20 11:15:37.000000 spacepackets-0.8.1/spacepackets/cfdp/pdu/metadata.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     6745 2022-05-20 11:15:37.000000 spacepackets-0.8.1/spacepackets/cfdp/pdu/nak.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     1805 2022-05-20 11:15:37.000000 spacepackets-0.8.1/spacepackets/cfdp/pdu/prompt.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)    21373 2022-05-20 11:15:37.000000 spacepackets-0.8.1/spacepackets/cfdp/tlv.py
-drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2022-05-24 12:08:02.771844 spacepackets-0.8.1/spacepackets/ecss/
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      116 2022-05-20 11:15:37.000000 spacepackets-0.8.1/spacepackets/ecss/__init__.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     1647 2022-05-24 12:04:32.000000 spacepackets-0.8.1/spacepackets/ecss/conf.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      347 2022-05-24 11:50:51.000000 spacepackets-0.8.1/spacepackets/ecss/definitions.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     1640 2022-05-24 11:51:03.000000 spacepackets-0.8.1/spacepackets/ecss/pus_17_test.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     6387 2022-05-24 11:50:51.000000 spacepackets-0.8.1/spacepackets/ecss/pus_1_verification.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      611 2022-05-20 11:15:37.000000 spacepackets-0.8.1/spacepackets/ecss/pus_3_hk.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      366 2022-05-20 11:15:37.000000 spacepackets-0.8.1/spacepackets/ecss/pus_5_event.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)    14490 2022-05-24 12:06:43.000000 spacepackets-0.8.1/spacepackets/ecss/tc.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)    18243 2022-05-24 12:06:43.000000 spacepackets-0.8.1/spacepackets/ecss/tm.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      853 2021-11-19 13:24:54.000000 spacepackets-0.8.1/spacepackets/log.py
-drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2022-05-24 12:08:02.771844 spacepackets-0.8.1/spacepackets/uslp/
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      293 2022-05-20 11:15:37.000000 spacepackets-0.8.1/spacepackets/uslp/__init__.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      595 2022-05-20 11:15:37.000000 spacepackets-0.8.1/spacepackets/uslp/conf.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      376 2022-05-20 11:15:37.000000 spacepackets-0.8.1/spacepackets/uslp/definitions.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)    19564 2022-05-20 11:15:37.000000 spacepackets-0.8.1/spacepackets/uslp/frame.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     9857 2022-05-20 11:15:37.000000 spacepackets-0.8.1/spacepackets/uslp/header.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     1428 2022-05-20 11:15:37.000000 spacepackets-0.8.1/spacepackets/util.py
-drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2022-05-24 12:08:02.771844 spacepackets-0.8.1/spacepackets.egg-info/
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     7040 2022-05-24 12:08:02.000000 spacepackets-0.8.1/spacepackets.egg-info/PKG-INFO
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     1582 2022-05-24 12:08:02.000000 spacepackets-0.8.1/spacepackets.egg-info/SOURCES.txt
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)        1 2022-05-24 12:08:02.000000 spacepackets-0.8.1/spacepackets.egg-info/dependency_links.txt
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)       12 2022-05-24 12:08:02.000000 spacepackets-0.8.1/spacepackets.egg-info/requires.txt
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)       19 2022-05-24 12:08:02.000000 spacepackets-0.8.1/spacepackets.egg-info/top_level.txt
-drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2022-05-24 12:08:02.771844 spacepackets-0.8.1/tests/
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)        0 2021-11-19 13:24:54.000000 spacepackets-0.8.1/tests/__init__.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     5989 2022-05-20 11:15:37.000000 spacepackets-0.8.1/tests/test_ccsds.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)    12227 2022-05-20 11:15:37.000000 spacepackets-0.8.1/tests/test_cfdp.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     4691 2022-05-20 11:15:37.000000 spacepackets-0.8.1/tests/test_cfdp_file_data.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)    28241 2022-05-20 11:15:37.000000 spacepackets-0.8.1/tests/test_cfdp_pdus.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     9835 2022-05-20 11:15:37.000000 spacepackets-0.8.1/tests/test_cfdp_tlvs_lvs.py
--rwxrwxr-x   0 rmueller  (1000) rmueller  (1000)    15772 2022-05-20 11:15:37.000000 spacepackets-0.8.1/tests/test_ecss_pus.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)    23378 2022-05-20 11:15:37.000000 spacepackets-0.8.1/tests/test_uslp.py
+drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2022-06-14 09:18:44.494486 spacepackets-0.9.0/
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)    11357 2022-04-28 17:03:21.000000 spacepackets-0.9.0/LICENSE
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      629 2022-04-28 17:03:21.000000 spacepackets-0.9.0/NOTICE
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     7040 2022-06-14 09:18:44.494486 spacepackets-0.9.0/PKG-INFO
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     5433 2022-04-28 17:03:21.000000 spacepackets-0.9.0/README.md
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      103 2022-04-28 17:03:21.000000 spacepackets-0.9.0/pyproject.toml
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     1176 2022-06-14 09:18:44.498486 spacepackets-0.9.0/setup.cfg
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      328 2022-04-28 17:03:21.000000 spacepackets-0.9.0/setup.py
+drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2022-06-14 09:18:44.490486 spacepackets-0.9.0/spacepackets/
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)       22 2022-06-14 09:08:16.000000 spacepackets-0.9.0/spacepackets/__init__.py
+drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2022-06-14 09:18:44.494486 spacepackets-0.9.0/spacepackets/ccsds/
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)       43 2022-04-28 17:03:21.000000 spacepackets-0.9.0/spacepackets/ccsds/__init__.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)    11390 2022-06-14 09:16:04.000000 spacepackets-0.9.0/spacepackets/ccsds/spacepacket.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     4511 2022-04-28 17:03:21.000000 spacepackets-0.9.0/spacepackets/ccsds/time.py
+drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2022-06-14 09:18:44.494486 spacepackets-0.9.0/spacepackets/cfdp/
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      100 2022-04-28 17:03:21.000000 spacepackets-0.9.0/spacepackets/cfdp/__init__.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     3425 2022-04-28 17:03:21.000000 spacepackets-0.9.0/spacepackets/cfdp/conf.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     2924 2022-04-28 17:03:21.000000 spacepackets-0.9.0/spacepackets/cfdp/definitions.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     1410 2022-04-28 17:03:21.000000 spacepackets-0.9.0/spacepackets/cfdp/lv.py
+drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2022-06-14 09:18:44.494486 spacepackets-0.9.0/spacepackets/cfdp/pdu/
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      481 2022-04-28 17:03:21.000000 spacepackets-0.9.0/spacepackets/cfdp/pdu/__init__.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     3320 2022-04-28 17:03:21.000000 spacepackets-0.9.0/spacepackets/cfdp/pdu/ack.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     4157 2022-04-28 17:03:21.000000 spacepackets-0.9.0/spacepackets/cfdp/pdu/eof.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     6099 2022-04-28 17:03:21.000000 spacepackets-0.9.0/spacepackets/cfdp/pdu/file_data.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     5831 2022-04-28 17:03:21.000000 spacepackets-0.9.0/spacepackets/cfdp/pdu/file_directive.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     7559 2022-04-28 17:03:21.000000 spacepackets-0.9.0/spacepackets/cfdp/pdu/finished.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)    10465 2022-04-28 17:03:21.000000 spacepackets-0.9.0/spacepackets/cfdp/pdu/header.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     3159 2022-04-28 17:03:21.000000 spacepackets-0.9.0/spacepackets/cfdp/pdu/keep_alive.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     6982 2022-04-28 17:03:21.000000 spacepackets-0.9.0/spacepackets/cfdp/pdu/metadata.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     6745 2022-04-28 17:03:21.000000 spacepackets-0.9.0/spacepackets/cfdp/pdu/nak.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     1805 2022-04-28 17:03:21.000000 spacepackets-0.9.0/spacepackets/cfdp/pdu/prompt.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)    21373 2022-04-28 17:03:21.000000 spacepackets-0.9.0/spacepackets/cfdp/tlv.py
+drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2022-06-14 09:18:44.494486 spacepackets-0.9.0/spacepackets/ecss/
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      116 2022-04-28 17:03:21.000000 spacepackets-0.9.0/spacepackets/ecss/__init__.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     1647 2022-05-26 09:38:36.000000 spacepackets-0.9.0/spacepackets/ecss/conf.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      347 2022-05-26 09:38:36.000000 spacepackets-0.9.0/spacepackets/ecss/definitions.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     1640 2022-05-26 09:38:36.000000 spacepackets-0.9.0/spacepackets/ecss/pus_17_test.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     6387 2022-05-26 09:38:36.000000 spacepackets-0.9.0/spacepackets/ecss/pus_1_verification.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      611 2022-05-05 14:48:02.000000 spacepackets-0.9.0/spacepackets/ecss/pus_3_hk.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      366 2022-05-05 14:48:02.000000 spacepackets-0.9.0/spacepackets/ecss/pus_5_event.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)    14466 2022-06-14 09:04:14.000000 spacepackets-0.9.0/spacepackets/ecss/tc.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)    18219 2022-06-14 09:04:14.000000 spacepackets-0.9.0/spacepackets/ecss/tm.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      853 2022-04-28 17:03:21.000000 spacepackets-0.9.0/spacepackets/log.py
+drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2022-06-14 09:18:44.494486 spacepackets-0.9.0/spacepackets/uslp/
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      293 2022-04-28 17:03:21.000000 spacepackets-0.9.0/spacepackets/uslp/__init__.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      595 2022-04-28 17:03:21.000000 spacepackets-0.9.0/spacepackets/uslp/conf.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      376 2022-04-28 17:03:21.000000 spacepackets-0.9.0/spacepackets/uslp/definitions.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)    19564 2022-04-28 17:03:21.000000 spacepackets-0.9.0/spacepackets/uslp/frame.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     9857 2022-04-28 17:03:21.000000 spacepackets-0.9.0/spacepackets/uslp/header.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     1428 2022-04-28 17:03:21.000000 spacepackets-0.9.0/spacepackets/util.py
+drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2022-06-14 09:18:44.494486 spacepackets-0.9.0/spacepackets.egg-info/
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     7040 2022-06-14 09:18:44.000000 spacepackets-0.9.0/spacepackets.egg-info/PKG-INFO
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     1582 2022-06-14 09:18:44.000000 spacepackets-0.9.0/spacepackets.egg-info/SOURCES.txt
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)        1 2022-06-14 09:18:44.000000 spacepackets-0.9.0/spacepackets.egg-info/dependency_links.txt
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)       12 2022-06-14 09:18:44.000000 spacepackets-0.9.0/spacepackets.egg-info/requires.txt
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)       19 2022-06-14 09:18:44.000000 spacepackets-0.9.0/spacepackets.egg-info/top_level.txt
+drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2022-06-14 09:18:44.494486 spacepackets-0.9.0/tests/
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)        0 2022-04-28 17:03:21.000000 spacepackets-0.9.0/tests/__init__.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     7036 2022-06-14 09:16:04.000000 spacepackets-0.9.0/tests/test_ccsds.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)    12227 2022-04-28 17:03:21.000000 spacepackets-0.9.0/tests/test_cfdp.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     4691 2022-04-28 17:03:21.000000 spacepackets-0.9.0/tests/test_cfdp_file_data.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)    28241 2022-04-28 17:03:21.000000 spacepackets-0.9.0/tests/test_cfdp_pdus.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     9835 2022-04-28 17:03:21.000000 spacepackets-0.9.0/tests/test_cfdp_tlvs_lvs.py
+-rwxrwxr-x   0 rmueller  (1000) rmueller  (1000)    15772 2022-05-05 14:48:02.000000 spacepackets-0.9.0/tests/test_ecss_pus.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)    23378 2022-04-28 17:03:21.000000 spacepackets-0.9.0/tests/test_uslp.py
```

### Comparing `spacepackets-0.8.1/LICENSE` & `spacepackets-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spacepackets-0.8.1/NOTICE` & `spacepackets-0.9.0/NOTICE`

 * *Files identical despite different names*

### Comparing `spacepackets-0.8.1/PKG-INFO` & `spacepackets-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacepackets
-Version: 0.8.1
+Version: 0.9.0
 Summary: Various CCSDS and ECSS packet implementations
 Home-page: https://github.com/robamu-org/py-spacepackets
 Author: Robin Mueller
 Author-email: robin.mueller.m@gmail.com
 License: Apache-2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `spacepackets-0.8.1/README.md` & `spacepackets-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `spacepackets-0.8.1/setup.cfg` & `spacepackets-0.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `spacepackets-0.8.1/spacepackets/ccsds/spacepacket.py` & `spacepackets-0.9.0/spacepackets/ccsds/spacepacket.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 import enum
+import struct
 
 from typing import Tuple, Deque, List, Final
 from spacepackets.log import get_console_logger
 
 SPACE_PACKET_HEADER_SIZE: Final = 6
 
 
@@ -19,81 +20,100 @@
     UNSEGMENTED = 0b11
 
 
 class SpacePacketHeader:
     """This class encapsulates the space packet header.
     Packet reference: Blue Book CCSDS 133.0-B-2"""
 
+    SEQ_FLAG_MASK = 0xC000
+
     def __init__(
         self,
         packet_type: PacketTypes,
         apid: int,
-        source_sequence_count: int,
+        ssc: int,
         data_length: int,
         packet_version: int = 0b000,
-        secondary_header_flag: bool = True,
+        sec_header_flag: bool = True,
         sequence_flags: SequenceFlags = SequenceFlags.UNSEGMENTED,
     ):
         """Create a space packet header with the given field parameters
 
         :param packet_type: 0 for Telemetery, 1 for Telecommands
         :param apid: Application Process ID, should not be larger
             than 11 bits, deciaml 2074 or hex 0x7ff
-        :param source_sequence_count: Sequence counter, should not be larger than 0x3fff or
+        :param ssc: Source sequence counter, should not be larger than 0x3fff or
             decimal 16383
         :param data_length: Contains a length count C that equals one fewer than the length of the
             packet data field. Should not be larger than 65535 bytes
         :param packet_version:
-        :param secondary_header_flag:
+        :param sec_header_flag: Secondary header flag, 1 or True by default
         :param sequence_flags:
         :raises ValueError: On invalid parameters
         """
         self.packet_type = packet_type
         if apid > pow(2, 11) - 1 or apid < 0:
             logger = get_console_logger()
             logger.warning(
                 f"Invalid APID, exceeds maximum value {pow(2, 11) - 1} or negative"
             )
             raise ValueError
-        if source_sequence_count > pow(2, 14) - 1 or source_sequence_count < 0:
+        if ssc > pow(2, 14) - 1 or ssc < 0:
             logger = get_console_logger()
             logger.warning(
                 f"Invalid source sequence count, exceeds maximum value {pow(2, 14)- 1} or negative"
             )
             raise ValueError
         if data_length > pow(2, 16) - 1 or data_length < 0:
             logger = get_console_logger()
             logger.warning(
                 f"Invalid data length value, exceeds maximum value of {pow(2, 16) - 1} or negative"
             )
             raise ValueError
         self.apid = apid
-        self.ssc = source_sequence_count
-        self.secondary_header_flag = secondary_header_flag
+        self.ssc = ssc
+        self.sec_header_flag = sec_header_flag
         self.sequence_flags = sequence_flags
         self.psc = get_space_packet_sequence_control(
             sequence_flags=self.sequence_flags, source_sequence_count=self.ssc
         )
         self.version = packet_version
         self.data_length = data_length
         self.packet_id = get_space_packet_id_num(
             packet_type=self.packet_type,
-            secondary_header_flag=self.secondary_header_flag,
+            secondary_header_flag=self.sec_header_flag,
             apid=self.apid,
         )
 
+    @classmethod
+    def from_composite_fields(
+        cls,
+        packet_id: int,
+        psc: int,
+        data_length: int,
+        packet_version: int = 0b000,
+    ) -> SpacePacketHeader:
+        return SpacePacketHeader(
+            packet_type=PacketTypes(packet_id >> 12 & 0x01),
+            packet_version=packet_version,
+            sec_header_flag=bool((packet_id >> 11) & 0x01),
+            data_length=data_length,
+            sequence_flags=SequenceFlags((psc & cls.SEQ_FLAG_MASK) >> 14),
+            ssc=psc & (~cls.SEQ_FLAG_MASK),
+            apid=packet_id & 0x7FF,
+        )
+
     def pack(self) -> bytearray:
-        """Serialize raw space packet header into a bytearray"""
+        """Serialize raw space packet header into a bytearray, using big endian for each
+        2 octet field of the space packet header"""
         header = bytearray()
-        header.append((self.packet_id & 0xFF00) >> 8)
-        header.append(self.packet_id & 0xFF)
-        header.append((self.psc & 0xFF00) >> 8)
-        header.append(self.psc & 0xFF)
-        header.append((self.data_length & 0xFF00) >> 8)
-        header.append(self.data_length & 0xFF)
+        packet_id_with_version = self.version << 13 | self.packet_id
+        header.extend(struct.pack("!H", packet_id_with_version))
+        header.extend(struct.pack("!H", self.psc))
+        header.extend(struct.pack("!H", self.data_length))
         return header
 
     @property
     def header_len(self) -> int:
         return SPACE_PACKET_HEADER_SIZE
 
     @property
@@ -110,45 +130,43 @@
         """Unpack a raw space packet into the space packet header instance
         :raise ValueError: Raw packet length invalid
         """
         if len(space_packet_raw) < SPACE_PACKET_HEADER_SIZE:
             logger = get_console_logger()
             logger.warning("Packet size smaller than PUS header size!")
             raise ValueError
-        packet_type = space_packet_raw[0] & 0x10
-        if packet_type == 0:
-            packet_type = PacketTypes.TM
-        else:
-            packet_type = PacketTypes.TC
-        packet_version = space_packet_raw[0] >> 5
-        secondary_header_flag = (space_packet_raw[0] & 0x8) >> 3
-        apid = ((space_packet_raw[0] & 0x7) << 8) | space_packet_raw[1]
-        sequence_flags = (space_packet_raw[2] & 0xC0) >> 6
-        ssc = ((space_packet_raw[2] << 8) | space_packet_raw[3]) & 0x3FFF
-        data_length = space_packet_raw[4] << 8 | space_packet_raw[5]
+        packet_version = (space_packet_raw[0] >> 5) & 0b111
+        packet_type = PacketTypes((space_packet_raw[0] >> 4) & 0b1)
+        secondary_header_flag = (space_packet_raw[0] >> 3) & 0b1
+        apid = ((space_packet_raw[0] & 0b111) << 8) | space_packet_raw[1]
+        psc = struct.unpack("!H", space_packet_raw[2:4])[0]
+        sequence_flags = (psc & SpacePacketHeader.SEQ_FLAG_MASK) >> 14
+        ssc = psc & (~SpacePacketHeader.SEQ_FLAG_MASK)
         return SpacePacketHeader(
             packet_type=packet_type,
             apid=apid,
-            secondary_header_flag=bool(secondary_header_flag),
+            sec_header_flag=bool(secondary_header_flag),
             packet_version=packet_version,
-            data_length=data_length,
+            data_length=struct.unpack("!H", space_packet_raw[4:6])[0],
             sequence_flags=SequenceFlags(sequence_flags),
-            source_sequence_count=ssc,
+            ssc=ssc,
         )
 
     def __str__(self):
         return (
             f"Space Packet with Packet ID 0x{self.packet_id:04x}, APID {self.apid}, "
             f"SSC {self.ssc}, Data Length {self.data_length}"
         )
 
     def __repr__(self):
         return (
-            f"{self.__class__.__name__}(packet_type={self.packet_type!r}, "
-            f"packet_id={self.packet_id!r}, apid={self.apid!r}, ssc={self.ssc!r})"
+            f"{self.__class__.__name__}(packet_version={self.version!r}, "
+            f"packet_type={self.packet_type!r}, apid={self.apid!r}, ssc={self.ssc!r}),"
+            f"data_length={self.data_length!r}, sec_header_flag={self.sec_header_flag!r},"
+            f"sequence_flags={self.sequence_flags!r}"
         )
 
 
 def get_space_packet_id_bytes(
     packet_type: PacketTypes,
     secondary_header_flag: True,
     apid: int,
```

### Comparing `spacepackets-0.8.1/spacepackets/ccsds/time.py` & `spacepackets-0.9.0/spacepackets/ccsds/time.py`

 * *Files identical despite different names*

### Comparing `spacepackets-0.8.1/spacepackets/cfdp/conf.py` & `spacepackets-0.9.0/spacepackets/cfdp/conf.py`

 * *Files identical despite different names*

### Comparing `spacepackets-0.8.1/spacepackets/cfdp/definitions.py` & `spacepackets-0.9.0/spacepackets/cfdp/definitions.py`

 * *Files identical despite different names*

### Comparing `spacepackets-0.8.1/spacepackets/cfdp/lv.py` & `spacepackets-0.9.0/spacepackets/cfdp/lv.py`

 * *Files identical despite different names*

### Comparing `spacepackets-0.8.1/spacepackets/cfdp/pdu/ack.py` & `spacepackets-0.9.0/spacepackets/cfdp/pdu/ack.py`

 * *Files identical despite different names*

### Comparing `spacepackets-0.8.1/spacepackets/cfdp/pdu/eof.py` & `spacepackets-0.9.0/spacepackets/cfdp/pdu/eof.py`

 * *Files identical despite different names*

### Comparing `spacepackets-0.8.1/spacepackets/cfdp/pdu/file_data.py` & `spacepackets-0.9.0/spacepackets/cfdp/pdu/file_data.py`

 * *Files identical despite different names*

### Comparing `spacepackets-0.8.1/spacepackets/cfdp/pdu/file_directive.py` & `spacepackets-0.9.0/spacepackets/cfdp/pdu/file_directive.py`

 * *Files identical despite different names*

### Comparing `spacepackets-0.8.1/spacepackets/cfdp/pdu/finished.py` & `spacepackets-0.9.0/spacepackets/cfdp/pdu/finished.py`

 * *Files identical despite different names*

### Comparing `spacepackets-0.8.1/spacepackets/cfdp/pdu/header.py` & `spacepackets-0.9.0/spacepackets/cfdp/pdu/header.py`

 * *Files identical despite different names*

### Comparing `spacepackets-0.8.1/spacepackets/cfdp/pdu/keep_alive.py` & `spacepackets-0.9.0/spacepackets/cfdp/pdu/keep_alive.py`

 * *Files identical despite different names*

### Comparing `spacepackets-0.8.1/spacepackets/cfdp/pdu/metadata.py` & `spacepackets-0.9.0/spacepackets/cfdp/pdu/metadata.py`

 * *Files identical despite different names*

### Comparing `spacepackets-0.8.1/spacepackets/cfdp/pdu/nak.py` & `spacepackets-0.9.0/spacepackets/cfdp/pdu/nak.py`

 * *Files identical despite different names*

### Comparing `spacepackets-0.8.1/spacepackets/cfdp/pdu/prompt.py` & `spacepackets-0.9.0/spacepackets/cfdp/pdu/prompt.py`

 * *Files identical despite different names*

### Comparing `spacepackets-0.8.1/spacepackets/cfdp/tlv.py` & `spacepackets-0.9.0/spacepackets/cfdp/tlv.py`

 * *Files identical despite different names*

### Comparing `spacepackets-0.8.1/spacepackets/ecss/conf.py` & `spacepackets-0.9.0/spacepackets/ecss/conf.py`

 * *Files identical despite different names*

### Comparing `spacepackets-0.8.1/spacepackets/ecss/pus_17_test.py` & `spacepackets-0.9.0/spacepackets/ecss/pus_17_test.py`

 * *Files identical despite different names*

### Comparing `spacepackets-0.8.1/spacepackets/ecss/pus_1_verification.py` & `spacepackets-0.9.0/spacepackets/ecss/pus_1_verification.py`

 * *Files identical despite different names*

### Comparing `spacepackets-0.8.1/spacepackets/ecss/pus_3_hk.py` & `spacepackets-0.9.0/spacepackets/ecss/pus_3_hk.py`

 * *Files identical despite different names*

### Comparing `spacepackets-0.8.1/spacepackets/ecss/tc.py` & `spacepackets-0.9.0/spacepackets/ecss/tc.py`

 * *Files 0% similar despite different names*

```diff
@@ -216,18 +216,18 @@
             secondary_header_len=self.data_field_header.get_header_size(
                 pus_version=pus_version
             ),
             app_data_len=len(app_data),
         )
         self.space_packet_header = SpacePacketHeader(
             apid=apid,
-            secondary_header_flag=bool(secondary_header_flag),
+            sec_header_flag=bool(secondary_header_flag),
             packet_type=PacketTypes.TC,
             data_length=data_length,
-            source_sequence_count=ssc,
+            ssc=ssc,
         )
         self._app_data = app_data
         self._valid = True
         self._crc = 0
 
     def __repr__(self):
         """Returns the representation of a class instance."""
```

### Comparing `spacepackets-0.8.1/spacepackets/ecss/tm.py` & `spacepackets-0.9.0/spacepackets/ecss/tm.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,18 +68,18 @@
         self._source_data = source_data
         data_length = self.get_source_data_length(
             timestamp_len=PusTelemetry.PUS_TIMESTAMP_SIZE, pus_version=pus_version
         )
         self.space_packet_header = SpacePacketHeader(
             apid=apid,
             packet_type=packet_type,
-            secondary_header_flag=secondary_header_flag,
+            sec_header_flag=secondary_header_flag,
             packet_version=packet_version,
             data_length=data_length,
-            source_sequence_count=ssc,
+            ssc=ssc,
         )
         self.secondary_packet_header = PusTmSecondaryHeader(
             pus_version=pus_version,
             service_id=service,
             subservice_id=subservice,
             message_counter=message_counter,
             destination_id=destination_id,
```

### Comparing `spacepackets-0.8.1/spacepackets/log.py` & `spacepackets-0.9.0/spacepackets/log.py`

 * *Files identical despite different names*

### Comparing `spacepackets-0.8.1/spacepackets/uslp/conf.py` & `spacepackets-0.9.0/spacepackets/uslp/conf.py`

 * *Files identical despite different names*

### Comparing `spacepackets-0.8.1/spacepackets/uslp/frame.py` & `spacepackets-0.9.0/spacepackets/uslp/frame.py`

 * *Files identical despite different names*

### Comparing `spacepackets-0.8.1/spacepackets/uslp/header.py` & `spacepackets-0.9.0/spacepackets/uslp/header.py`

 * *Files identical despite different names*

### Comparing `spacepackets-0.8.1/spacepackets/util.py` & `spacepackets-0.9.0/spacepackets/util.py`

 * *Files identical despite different names*

### Comparing `spacepackets-0.8.1/spacepackets.egg-info/PKG-INFO` & `spacepackets-0.9.0/spacepackets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacepackets
-Version: 0.8.1
+Version: 0.9.0
 Summary: Various CCSDS and ECSS packet implementations
 Home-page: https://github.com/robamu-org/py-spacepackets
 Author: Robin Mueller
 Author-email: robin.mueller.m@gmail.com
 License: Apache-2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `spacepackets-0.8.1/spacepackets.egg-info/SOURCES.txt` & `spacepackets-0.9.0/spacepackets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spacepackets-0.8.1/tests/test_ccsds.py` & `spacepackets-0.9.0/tests/test_ccsds.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,16 +16,17 @@
 
 
 class TestCcsds(TestCase):
     def test_spacepacket(self):
         sp_header = SpacePacketHeader(
             apid=0x02,
             data_length=22,
-            source_sequence_count=52,
+            ssc=52,
             packet_type=PacketTypes.TC,
+            sequence_flags=SequenceFlags.FIRST_SEGMENT,
         )
         self.assertEqual(sp_header.apid, 0x02)
         self.assertEqual(sp_header.ssc, 52)
         self.assertEqual(sp_header.data_length, 22)
         self.assertEqual(sp_header.packet_type, PacketTypes.TC)
         sp_packed = sp_header.pack()
         self.assertEqual(get_apid_from_raw_space_packet(raw_packet=sp_packed), 0x02)
@@ -34,34 +35,39 @@
         )
         sp_unpacked = SpacePacketHeader.unpack(space_packet_raw=sp_packed)
         self.assertRaises(
             ValueError,
             SpacePacketHeader,
             apid=982292,
             data_length=22,
-            source_sequence_count=52,
+            ssc=52,
             packet_type=PacketTypes.TC,
         )
         self.assertRaises(
             ValueError,
             SpacePacketHeader,
             apid=0x02,
             data_length=679393,
-            source_sequence_count=52,
+            ssc=52,
             packet_type=PacketTypes.TC,
         )
         self.assertRaises(
             ValueError,
             SpacePacketHeader,
             apid=0x02,
             data_length=22,
-            source_sequence_count=96030,
+            ssc=96030,
             packet_type=PacketTypes.TC,
         )
         self.assertRaises(ValueError, SpacePacketHeader.unpack, bytearray())
+        self.assertEqual(sp_unpacked.packet_type, PacketTypes.TC)
+        self.assertEqual(sp_unpacked.apid, 0x02)
+        self.assertEqual(sp_unpacked.version, 0b000)
+        self.assertEqual(sp_unpacked.ssc, 52)
+        self.assertEqual(sp_unpacked.sequence_flags, SequenceFlags.FIRST_SEGMENT)
         print(sp_header)
         print(sp_header.__repr__())
 
         byte_one, byte_two = get_space_packet_id_bytes(
             packet_type=PacketTypes.TC, apid=0x3FF, secondary_header_flag=True
         )
         self.assertEqual(byte_two, 0xFF)
@@ -91,23 +97,41 @@
             source_sequence_count=0x3FFF,
             sequence_flags=5,
         )
 
         raw_header = get_space_packet_header(
             packet_id=packet_id, packet_sequence_control=psc, data_length=22
         )
-        self.assertEqual(raw_header[0], (packet_id & 0xFF00) >> 8)
+        self.assertEqual(raw_header[0], ((packet_id & 0xFF00) >> 8) & 0x1FFF)
         self.assertEqual(raw_header[1], packet_id & 0xFF)
         self.assertEqual(raw_header[2], (psc & 0xFF00) >> 8)
         self.assertEqual(raw_header[3], psc & 0xFF)
         self.assertEqual(raw_header[4], (22 & 0xFF00) >> 8)
         self.assertEqual(raw_header[5], 22 & 0xFF)
 
+        header_from_composite = SpacePacketHeader.from_composite_fields(
+            packet_id=packet_id, psc=psc, data_length=22
+        )
+        self.assertEqual(header_from_composite.pack(), raw_header)
+        header_tm = SpacePacketHeader(
+            packet_type=PacketTypes.TM,
+            sequence_flags=SequenceFlags.UNSEGMENTED,
+            apid=0x12,
+            data_length=7,
+            ssc=28,
+        )
+        raw = header_tm.pack()
+        header_tm_back = SpacePacketHeader.unpack(raw)
+        self.assertEqual(header_tm_back.packet_type, PacketTypes.TM)
+        self.assertEqual(header_tm_back.apid, 0x12)
+        self.assertEqual(header_tm_back.version, 0b000)
+        self.assertEqual(header_tm_back.ssc, 28)
+        self.assertEqual(header_tm_back.data_length, 7)
+
     def test_sp_parser(self):
-        raw_buffer = bytearray()
         tm_packet = PusTelemetry(service=17, subservice=2, pus_version=PusVersion.PUS_C)
         packet_ids = (tm_packet.packet_id,)
         tm_packet_raw = tm_packet.pack()
         packet_deque = deque()
         packet_deque.appendleft(tm_packet_raw)
         packet_deque.appendleft(tm_packet_raw)
         sp_list = parse_space_packets(
```

### Comparing `spacepackets-0.8.1/tests/test_cfdp.py` & `spacepackets-0.9.0/tests/test_cfdp.py`

 * *Files identical despite different names*

### Comparing `spacepackets-0.8.1/tests/test_cfdp_file_data.py` & `spacepackets-0.9.0/tests/test_cfdp_file_data.py`

 * *Files identical despite different names*

### Comparing `spacepackets-0.8.1/tests/test_cfdp_pdus.py` & `spacepackets-0.9.0/tests/test_cfdp_pdus.py`

 * *Files identical despite different names*

### Comparing `spacepackets-0.8.1/tests/test_cfdp_tlvs_lvs.py` & `spacepackets-0.9.0/tests/test_cfdp_tlvs_lvs.py`

 * *Files identical despite different names*

### Comparing `spacepackets-0.8.1/tests/test_ecss_pus.py` & `spacepackets-0.9.0/tests/test_ecss_pus.py`

 * *Files identical despite different names*

### Comparing `spacepackets-0.8.1/tests/test_uslp.py` & `spacepackets-0.9.0/tests/test_uslp.py`

 * *Files identical despite different names*

