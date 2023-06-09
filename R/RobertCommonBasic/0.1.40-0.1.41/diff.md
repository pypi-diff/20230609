# Comparing `tmp/RobertCommonBasic-0.1.40.tar.gz` & `tmp/RobertCommonBasic-0.1.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RobertCommonBasic-0.1.40.tar", last modified: Thu May 25 09:14:25 2023, max compression
+gzip compressed data, was "RobertCommonBasic-0.1.41.tar", last modified: Fri Jun  9 09:56:00 2023, max compression
```

## Comparing `RobertCommonBasic-0.1.40.tar` & `RobertCommonBasic-0.1.41.tar`

### file list

```diff
@@ -1,140 +1,140 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 09:14:25.400530 RobertCommonBasic-0.1.40/
--rw-rw-rw-   0        0        0     1067 2021-08-09 02:56:17.000000 RobertCommonBasic-0.1.40/LICENSE
--rw-rw-rw-   0        0        0       44 2021-08-09 07:19:42.000000 RobertCommonBasic-0.1.40/MANIFEST.in
--rw-rw-rw-   0        0        0     1739 2023-05-25 09:14:25.400530 RobertCommonBasic-0.1.40/PKG-INFO
--rw-rw-rw-   0        0        0     1057 2022-01-13 05:29:18.000000 RobertCommonBasic-0.1.40/README.md
-drwxrwxrwx   0        0        0        0 2023-05-25 09:14:25.279205 RobertCommonBasic-0.1.40/RobertCommonBasic.egg-info/
--rw-rw-rw-   0        0        0     1739 2023-05-25 09:14:25.000000 RobertCommonBasic-0.1.40/RobertCommonBasic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4467 2023-05-25 09:14:25.000000 RobertCommonBasic-0.1.40/RobertCommonBasic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 09:14:25.000000 RobertCommonBasic-0.1.40/RobertCommonBasic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      169 2023-05-25 09:14:25.000000 RobertCommonBasic-0.1.40/RobertCommonBasic.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-05-25 09:14:25.000000 RobertCommonBasic-0.1.40/RobertCommonBasic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      187 2023-05-23 06:22:21.000000 RobertCommonBasic-0.1.40/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-05-25 09:14:25.280208 RobertCommonBasic-0.1.40/robertcommonbasic/
--rw-rw-rw-   0        0        0        2 2021-08-09 03:27:49.000000 RobertCommonBasic-0.1.40/robertcommonbasic/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:14:25.281205 RobertCommonBasic-0.1.40/robertcommonbasic/basic/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:14:25.282714 RobertCommonBasic-0.1.40/robertcommonbasic/basic/base/
--rw-rw-rw-   0        0        0        0 2023-01-04 02:39:20.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/base/__init__.py
--rw-rw-rw-   0        0        0      471 2023-01-04 02:45:25.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/base/constant.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:14:25.285151 RobertCommonBasic-0.1.40/robertcommonbasic/basic/cache/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/cache/__init__.py
--rw-rw-rw-   0        0        0      667 2022-11-14 07:41:26.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/cache/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:14:25.287153 RobertCommonBasic-0.1.40/robertcommonbasic/basic/cls/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/cls/__init__.py
--rw-rw-rw-   0        0        0    12320 2023-05-09 08:30:50.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/cls/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:14:25.298418 RobertCommonBasic-0.1.40/robertcommonbasic/basic/data/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/data/__init__.py
--rw-rw-rw-   0        0        0    13611 2023-01-31 14:01:59.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/data/conversion.py
--rw-rw-rw-   0        0        0     4537 2022-11-14 07:54:50.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/data/crc16.py
--rw-rw-rw-   0        0        0     2169 2023-04-28 09:36:20.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/data/csv.py
--rw-rw-rw-   0        0        0    39297 2022-11-14 09:43:00.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/data/datatuple.py
--rw-rw-rw-   0        0        0     2528 2023-05-25 09:05:54.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/data/express.py
--rw-rw-rw-   0        0        0     8304 2022-11-14 09:43:00.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/data/frame.py
--rw-rw-rw-   0        0        0     1097 2022-11-14 09:48:07.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/data/nametuple.py
--rw-rw-rw-   0        0        0       62 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/data/type.py
--rw-rw-rw-   0        0        0    12943 2023-05-23 08:43:23.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/data/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:14:25.300422 RobertCommonBasic-0.1.40/robertcommonbasic/basic/decorator/
--rw-rw-rw-   0        0        0        0 2021-12-08 01:56:09.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/decorator/__init__.py
--rw-rw-rw-   0        0        0     1250 2022-12-05 08:07:43.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/decorator/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:14:25.303420 RobertCommonBasic-0.1.40/robertcommonbasic/basic/dt/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/dt/__init__.py
--rw-rw-rw-   0        0        0     4474 2022-12-28 02:51:52.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/dt/schedule.py
--rw-rw-rw-   0        0        0    10445 2023-05-18 03:32:13.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/dt/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:14:25.309851 RobertCommonBasic-0.1.40/robertcommonbasic/basic/encrypt/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/encrypt/__init__.py
--rw-rw-rw-   0        0        0      583 2022-11-14 07:14:55.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/encrypt/aes.py
--rw-rw-rw-   0        0        0     3856 2022-11-14 07:41:26.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/encrypt/dsa.py
--rw-rw-rw-   0        0        0      716 2023-03-09 07:09:06.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/encrypt/hash.py
--rw-rw-rw-   0        0        0      338 2022-11-14 07:14:55.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/encrypt/md5.py
--rw-rw-rw-   0        0        0     2661 2022-11-14 07:25:08.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/encrypt/rsa.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:14:25.312238 RobertCommonBasic-0.1.40/robertcommonbasic/basic/error/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/error/__init__.py
--rw-rw-rw-   0        0        0     2354 2022-11-14 09:50:44.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/error/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:14:25.315245 RobertCommonBasic-0.1.40/robertcommonbasic/basic/exector/
--rw-rw-rw-   0        0        0        0 2022-08-31 08:25:14.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/exector/__init__.py
--rw-rw-rw-   0        0        0     3641 2022-11-14 09:50:44.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/exector/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:14:25.327165 RobertCommonBasic-0.1.40/robertcommonbasic/basic/file/
--rw-rw-rw-   0        0        0        0 2022-11-18 02:39:00.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/file/__init__.py
--rw-rw-rw-   0        0        0     3053 2023-04-28 09:36:20.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/file/csv.py
--rw-rw-rw-   0        0        0     4951 2023-05-18 08:56:41.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/file/ini.py
--rw-rw-rw-   0        0        0     1035 2022-11-18 06:23:07.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/file/log.py
--rw-rw-rw-   0        0        0     3157 2022-11-24 03:18:18.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/file/xml.py
--rw-rw-rw-   0        0        0      339 2022-11-18 06:47:46.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/file/yaml.py
--rw-rw-rw-   0        0        0     3039 2023-03-08 07:31:52.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/file/zip.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:14:25.334249 RobertCommonBasic-0.1.40/robertcommonbasic/basic/log/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/log/__init__.py
--rw-rw-rw-   0        0        0     6070 2023-05-05 06:04:36.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/log/utils.py
--rw-rw-rw-   0        0        0     1366 2022-12-05 08:20:54.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/log/watch.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:14:25.337467 RobertCommonBasic-0.1.40/robertcommonbasic/basic/net/
--rw-rw-rw-   0        0        0        0 2022-06-29 12:44:36.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/net/__init__.py
--rw-rw-rw-   0        0        0     8521 2023-05-16 03:07:09.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/net/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:14:25.343541 RobertCommonBasic-0.1.40/robertcommonbasic/basic/os/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/os/__init__.py
--rw-rw-rw-   0        0        0      228 2022-12-14 09:03:01.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/os/cmd.py
--rw-rw-rw-   0        0        0      400 2022-06-29 09:34:23.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/os/env.py
--rw-rw-rw-   0        0        0     3446 2023-03-16 09:00:41.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/os/file.py
--rw-rw-rw-   0        0        0      533 2023-02-06 07:51:13.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/os/path.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:14:25.346423 RobertCommonBasic-0.1.40/robertcommonbasic/basic/process/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/process/__init__.py
--rw-rw-rw-   0        0        0     8845 2022-12-14 08:53:18.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/process/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:14:25.348426 RobertCommonBasic-0.1.40/robertcommonbasic/basic/profile/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/profile/__init__.py
--rw-rw-rw-   0        0        0     1264 2022-11-18 02:27:39.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/profile/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:14:25.351863 RobertCommonBasic-0.1.40/robertcommonbasic/basic/re/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/re/__init__.py
--rw-rw-rw-   0        0        0     1876 2023-05-25 09:11:33.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/re/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:14:25.355482 RobertCommonBasic-0.1.40/robertcommonbasic/basic/safetext/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/safetext/__init__.py
--rw-rw-rw-   0        0        0       91 2023-02-03 07:26:22.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/safetext/converter.py
--rw-rw-rw-   0        0        0      377 2022-11-18 02:33:07.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/safetext/funcs.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:14:25.360399 RobertCommonBasic-0.1.40/robertcommonbasic/basic/sugar/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/sugar/__init__.py
--rw-rw-rw-   0        0        0      377 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/sugar/funcs.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:14:25.362542 RobertCommonBasic-0.1.40/robertcommonbasic/basic/validation/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/validation/__init__.py
--rw-rw-rw-   0        0        0    36389 2023-02-21 08:51:30.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/validation/input.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:14:25.363549 RobertCommonBasic-0.1.40/robertcommonbasic/tests/
--rw-rw-rw-   0        0        0        0 2021-07-27 06:06:01.000000 RobertCommonBasic-0.1.40/robertcommonbasic/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:14:25.365549 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/
--rw-rw-rw-   0        0        0        0 2021-07-27 06:49:18.000000 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:14:25.367550 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_cls/
--rw-rw-rw-   0        0        0        0 2022-04-22 02:07:10.000000 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_cls/__init__.py
--rw-rw-rw-   0        0        0     1291 2023-03-02 14:03:08.000000 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_cls/test_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:14:25.373794 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_data/
--rw-rw-rw-   0        0        0        0 2022-01-19 07:38:20.000000 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_data/__init__.py
--rw-rw-rw-   0        0        0      928 2023-05-25 08:51:36.000000 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_data/test_conversion.py
--rw-rw-rw-   0        0        0     5920 2022-04-21 06:58:53.000000 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_data/test_datatupple.py
--rw-rw-rw-   0        0        0     2456 2022-01-27 05:56:15.000000 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_data/test_frame.py
--rw-rw-rw-   0        0        0     4649 2023-05-23 08:03:46.000000 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_data/test_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:14:25.375953 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_dt/
--rw-rw-rw-   0        0        0        0 2022-03-08 05:59:28.000000 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_dt/__init__.py
--rw-rw-rw-   0        0        0     2313 2023-05-25 08:43:02.000000 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_dt/test_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:14:25.381126 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_encrypt/
--rw-rw-rw-   0        0        0        0 2021-07-30 08:42:35.000000 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_encrypt/__init__.py
--rw-rw-rw-   0        0        0    32599 2022-07-03 01:41:08.000000 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_encrypt/test_dsa.py
--rw-rw-rw-   0        0        0      270 2022-07-03 01:04:51.000000 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_encrypt/test_md5.py
--rw-rw-rw-   0        0        0     3004 2022-11-22 07:10:43.000000 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_encrypt/test_rsa.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:14:25.383337 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_exector/
--rw-rw-rw-   0        0        0        0 2022-08-31 08:24:08.000000 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_exector/__init__.py
--rw-rw-rw-   0        0        0     1234 2022-12-05 09:33:27.000000 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_exector/test_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:14:25.389344 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_file/
--rw-rw-rw-   0        0        0        0 2022-11-18 06:48:14.000000 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_file/__init__.py
--rw-rw-rw-   0        0        0     1090 2023-02-03 06:30:00.000000 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_file/test_csv.py
--rw-rw-rw-   0        0        0     4285 2023-02-02 03:00:01.000000 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_file/test_xml.py
--rw-rw-rw-   0        0        0      705 2023-03-08 07:17:17.000000 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_file/test_zip.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:14:25.392343 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_net/
--rw-rw-rw-   0        0        0        0 2022-06-29 13:56:13.000000 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_net/__init__.py
--rw-rw-rw-   0        0        0      637 2023-05-16 02:40:06.000000 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_net/test_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:14:25.395529 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_os/
--rw-rw-rw-   0        0        0        0 2022-03-25 04:05:00.000000 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_os/__init__.py
--rw-rw-rw-   0        0        0      258 2022-06-29 09:29:01.000000 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_os/test_env.py
--rw-rw-rw-   0        0        0      449 2022-11-14 02:56:25.000000 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_os/test_file.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:14:25.397530 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_re/
--rw-rw-rw-   0        0        0        0 2022-05-18 02:57:45.000000 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_re/__init__.py
--rw-rw-rw-   0        0        0      670 2023-05-23 08:45:26.000000 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_re/test_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:14:25.399530 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_validation/
--rw-rw-rw-   0        0        0        0 2021-11-19 07:34:54.000000 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_validation/__init__.py
--rw-rw-rw-   0        0        0      218 2022-05-10 03:46:33.000000 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_validation/test_input.py
--rw-rw-rw-   0        0        0       42 2023-05-25 09:14:25.401529 RobertCommonBasic-0.1.40/setup.cfg
--rw-rw-rw-   0        0        0     3876 2023-05-25 09:11:33.000000 RobertCommonBasic-0.1.40/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 09:56:00.346027 RobertCommonBasic-0.1.41/
+-rw-rw-rw-   0        0        0     1067 2021-08-09 02:56:17.000000 RobertCommonBasic-0.1.41/LICENSE
+-rw-rw-rw-   0        0        0       44 2021-08-09 07:19:42.000000 RobertCommonBasic-0.1.41/MANIFEST.in
+-rw-rw-rw-   0        0        0      868 2023-06-09 09:56:00.346027 RobertCommonBasic-0.1.41/PKG-INFO
+-rw-rw-rw-   0        0        0      186 2023-06-02 07:56:40.000000 RobertCommonBasic-0.1.41/README.md
+drwxrwxrwx   0        0        0        0 2023-06-09 09:56:00.211968 RobertCommonBasic-0.1.41/RobertCommonBasic.egg-info/
+-rw-rw-rw-   0        0        0      868 2023-06-09 09:56:00.000000 RobertCommonBasic-0.1.41/RobertCommonBasic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4467 2023-06-09 09:56:00.000000 RobertCommonBasic-0.1.41/RobertCommonBasic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 09:56:00.000000 RobertCommonBasic-0.1.41/RobertCommonBasic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      169 2023-06-09 09:56:00.000000 RobertCommonBasic-0.1.41/RobertCommonBasic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-06-09 09:56:00.000000 RobertCommonBasic-0.1.41/RobertCommonBasic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      187 2023-05-23 06:22:21.000000 RobertCommonBasic-0.1.41/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 09:56:00.212969 RobertCommonBasic-0.1.41/robertcommonbasic/
+-rw-rw-rw-   0        0        0        2 2021-08-09 03:27:49.000000 RobertCommonBasic-0.1.41/robertcommonbasic/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 09:56:00.212969 RobertCommonBasic-0.1.41/robertcommonbasic/basic/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 09:56:00.214972 RobertCommonBasic-0.1.41/robertcommonbasic/basic/base/
+-rw-rw-rw-   0        0        0        0 2023-01-04 02:39:20.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/base/__init__.py
+-rw-rw-rw-   0        0        0      471 2023-01-04 02:45:25.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/base/constant.py
+drwxrwxrwx   0        0        0        0 2023-06-09 09:56:00.217409 RobertCommonBasic-0.1.41/robertcommonbasic/basic/cache/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/cache/__init__.py
+-rw-rw-rw-   0        0        0      667 2022-11-14 07:41:26.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/cache/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-09 09:56:00.219409 RobertCommonBasic-0.1.41/robertcommonbasic/basic/cls/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/cls/__init__.py
+-rw-rw-rw-   0        0        0    12853 2023-06-09 09:28:37.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/cls/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-09 09:56:00.234174 RobertCommonBasic-0.1.41/robertcommonbasic/basic/data/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/data/__init__.py
+-rw-rw-rw-   0        0        0    13611 2023-01-31 14:01:59.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/data/conversion.py
+-rw-rw-rw-   0        0        0     4537 2022-11-14 07:54:50.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/data/crc16.py
+-rw-rw-rw-   0        0        0     2169 2023-04-28 09:36:20.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/data/csv.py
+-rw-rw-rw-   0        0        0    39297 2022-11-14 09:43:00.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/data/datatuple.py
+-rw-rw-rw-   0        0        0     2528 2023-05-25 09:05:54.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/data/express.py
+-rw-rw-rw-   0        0        0     8304 2022-11-14 09:43:00.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/data/frame.py
+-rw-rw-rw-   0        0        0     1097 2022-11-14 09:48:07.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/data/nametuple.py
+-rw-rw-rw-   0        0        0       62 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/data/type.py
+-rw-rw-rw-   0        0        0    12943 2023-05-23 08:43:23.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/data/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-09 09:56:00.237181 RobertCommonBasic-0.1.41/robertcommonbasic/basic/decorator/
+-rw-rw-rw-   0        0        0        0 2021-12-08 01:56:09.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/decorator/__init__.py
+-rw-rw-rw-   0        0        0     1250 2022-12-05 08:07:43.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/decorator/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-09 09:56:00.241679 RobertCommonBasic-0.1.41/robertcommonbasic/basic/dt/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/dt/__init__.py
+-rw-rw-rw-   0        0        0     4474 2022-12-28 02:51:52.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/dt/schedule.py
+-rw-rw-rw-   0        0        0    10445 2023-05-18 03:32:13.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/dt/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-09 09:56:00.249686 RobertCommonBasic-0.1.41/robertcommonbasic/basic/encrypt/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/encrypt/__init__.py
+-rw-rw-rw-   0        0        0      583 2022-11-14 07:14:55.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/encrypt/aes.py
+-rw-rw-rw-   0        0        0     3856 2022-11-14 07:41:26.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/encrypt/dsa.py
+-rw-rw-rw-   0        0        0      716 2023-03-09 07:09:06.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/encrypt/hash.py
+-rw-rw-rw-   0        0        0      338 2022-11-14 07:14:55.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/encrypt/md5.py
+-rw-rw-rw-   0        0        0     2661 2022-11-14 07:25:08.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/encrypt/rsa.py
+drwxrwxrwx   0        0        0        0 2023-06-09 09:56:00.253038 RobertCommonBasic-0.1.41/robertcommonbasic/basic/error/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/error/__init__.py
+-rw-rw-rw-   0        0        0     2354 2022-11-14 09:50:44.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/error/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-09 09:56:00.255370 RobertCommonBasic-0.1.41/robertcommonbasic/basic/exector/
+-rw-rw-rw-   0        0        0        0 2022-08-31 08:25:14.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/exector/__init__.py
+-rw-rw-rw-   0        0        0     3641 2022-11-14 09:50:44.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/exector/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-09 09:56:00.263368 RobertCommonBasic-0.1.41/robertcommonbasic/basic/file/
+-rw-rw-rw-   0        0        0        0 2022-11-18 02:39:00.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/file/__init__.py
+-rw-rw-rw-   0        0        0     3053 2023-04-28 09:36:20.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/file/csv.py
+-rw-rw-rw-   0        0        0     4951 2023-05-18 08:56:41.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/file/ini.py
+-rw-rw-rw-   0        0        0     1035 2022-11-18 06:23:07.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/file/log.py
+-rw-rw-rw-   0        0        0     3157 2022-11-24 03:18:18.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/file/xml.py
+-rw-rw-rw-   0        0        0      339 2022-11-18 06:47:46.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/file/yaml.py
+-rw-rw-rw-   0        0        0     3039 2023-03-08 07:31:52.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/file/zip.py
+drwxrwxrwx   0        0        0        0 2023-06-09 09:56:00.267867 RobertCommonBasic-0.1.41/robertcommonbasic/basic/log/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/log/__init__.py
+-rw-rw-rw-   0        0        0     6582 2023-06-09 09:52:58.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/log/utils.py
+-rw-rw-rw-   0        0        0     1366 2022-12-05 08:20:54.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/log/watch.py
+drwxrwxrwx   0        0        0        0 2023-06-09 09:56:00.270480 RobertCommonBasic-0.1.41/robertcommonbasic/basic/net/
+-rw-rw-rw-   0        0        0        0 2022-06-29 12:44:36.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/net/__init__.py
+-rw-rw-rw-   0        0        0     8521 2023-05-16 03:07:09.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/net/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-09 09:56:00.281123 RobertCommonBasic-0.1.41/robertcommonbasic/basic/os/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/os/__init__.py
+-rw-rw-rw-   0        0        0      228 2022-12-14 09:03:01.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/os/cmd.py
+-rw-rw-rw-   0        0        0      400 2022-06-29 09:34:23.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/os/env.py
+-rw-rw-rw-   0        0        0     3446 2023-03-16 09:00:41.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/os/file.py
+-rw-rw-rw-   0        0        0      533 2023-02-06 07:51:13.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/os/path.py
+drwxrwxrwx   0        0        0        0 2023-06-09 09:56:00.284511 RobertCommonBasic-0.1.41/robertcommonbasic/basic/process/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/process/__init__.py
+-rw-rw-rw-   0        0        0     8845 2022-12-14 08:53:18.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/process/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-09 09:56:00.287021 RobertCommonBasic-0.1.41/robertcommonbasic/basic/profile/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/profile/__init__.py
+-rw-rw-rw-   0        0        0     1264 2022-11-18 02:27:39.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/profile/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-09 09:56:00.291642 RobertCommonBasic-0.1.41/robertcommonbasic/basic/re/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/re/__init__.py
+-rw-rw-rw-   0        0        0     1876 2023-05-25 09:11:33.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/re/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-09 09:56:00.295273 RobertCommonBasic-0.1.41/robertcommonbasic/basic/safetext/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/safetext/__init__.py
+-rw-rw-rw-   0        0        0       91 2023-02-03 07:26:22.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/safetext/converter.py
+-rw-rw-rw-   0        0        0      377 2022-11-18 02:33:07.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/safetext/funcs.py
+drwxrwxrwx   0        0        0        0 2023-06-09 09:56:00.298338 RobertCommonBasic-0.1.41/robertcommonbasic/basic/sugar/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/sugar/__init__.py
+-rw-rw-rw-   0        0        0      377 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/sugar/funcs.py
+drwxrwxrwx   0        0        0        0 2023-06-09 09:56:00.300756 RobertCommonBasic-0.1.41/robertcommonbasic/basic/validation/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/validation/__init__.py
+-rw-rw-rw-   0        0        0    36389 2023-02-21 08:51:30.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/validation/input.py
+drwxrwxrwx   0        0        0        0 2023-06-09 09:56:00.302763 RobertCommonBasic-0.1.41/robertcommonbasic/tests/
+-rw-rw-rw-   0        0        0        0 2021-07-27 06:06:01.000000 RobertCommonBasic-0.1.41/robertcommonbasic/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 09:56:00.303763 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/
+-rw-rw-rw-   0        0        0        0 2021-07-27 06:49:18.000000 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 09:56:00.305763 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_cls/
+-rw-rw-rw-   0        0        0        0 2022-04-22 02:07:10.000000 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_cls/__init__.py
+-rw-rw-rw-   0        0        0     1291 2023-03-02 14:03:08.000000 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_cls/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-09 09:56:00.317431 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_data/
+-rw-rw-rw-   0        0        0        0 2022-01-19 07:38:20.000000 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_data/__init__.py
+-rw-rw-rw-   0        0        0      928 2023-05-25 08:51:36.000000 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_data/test_conversion.py
+-rw-rw-rw-   0        0        0     5920 2022-04-21 06:58:53.000000 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_data/test_datatupple.py
+-rw-rw-rw-   0        0        0     2456 2022-01-27 05:56:15.000000 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_data/test_frame.py
+-rw-rw-rw-   0        0        0     4649 2023-05-23 08:03:46.000000 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_data/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-09 09:56:00.320918 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_dt/
+-rw-rw-rw-   0        0        0        0 2022-03-08 05:59:28.000000 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_dt/__init__.py
+-rw-rw-rw-   0        0        0     2313 2023-05-25 08:43:02.000000 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_dt/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-09 09:56:00.325971 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_encrypt/
+-rw-rw-rw-   0        0        0        0 2021-07-30 08:42:35.000000 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_encrypt/__init__.py
+-rw-rw-rw-   0        0        0    32599 2022-07-03 01:41:08.000000 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_encrypt/test_dsa.py
+-rw-rw-rw-   0        0        0      270 2022-07-03 01:04:51.000000 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_encrypt/test_md5.py
+-rw-rw-rw-   0        0        0     3004 2022-11-22 07:10:43.000000 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_encrypt/test_rsa.py
+drwxrwxrwx   0        0        0        0 2023-06-09 09:56:00.327977 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_exector/
+-rw-rw-rw-   0        0        0        0 2022-08-31 08:24:08.000000 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_exector/__init__.py
+-rw-rw-rw-   0        0        0     1234 2022-12-05 09:33:27.000000 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_exector/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-09 09:56:00.333978 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_file/
+-rw-rw-rw-   0        0        0        0 2022-11-18 06:48:14.000000 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_file/__init__.py
+-rw-rw-rw-   0        0        0     1090 2023-02-03 06:30:00.000000 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_file/test_csv.py
+-rw-rw-rw-   0        0        0     4285 2023-02-02 03:00:01.000000 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_file/test_xml.py
+-rw-rw-rw-   0        0        0      705 2023-03-08 07:17:17.000000 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_file/test_zip.py
+drwxrwxrwx   0        0        0        0 2023-06-09 09:56:00.335990 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_net/
+-rw-rw-rw-   0        0        0        0 2022-06-29 13:56:13.000000 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_net/__init__.py
+-rw-rw-rw-   0        0        0      637 2023-05-16 02:40:06.000000 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_net/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-09 09:56:00.339996 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_os/
+-rw-rw-rw-   0        0        0        0 2022-03-25 04:05:00.000000 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_os/__init__.py
+-rw-rw-rw-   0        0        0      258 2022-06-29 09:29:01.000000 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_os/test_env.py
+-rw-rw-rw-   0        0        0      449 2022-11-14 02:56:25.000000 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_os/test_file.py
+drwxrwxrwx   0        0        0        0 2023-06-09 09:56:00.342013 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_re/
+-rw-rw-rw-   0        0        0        0 2022-05-18 02:57:45.000000 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_re/__init__.py
+-rw-rw-rw-   0        0        0      670 2023-05-23 08:45:26.000000 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_re/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-09 09:56:00.345029 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_validation/
+-rw-rw-rw-   0        0        0        0 2021-11-19 07:34:54.000000 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_validation/__init__.py
+-rw-rw-rw-   0        0        0      218 2022-05-10 03:46:33.000000 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_validation/test_input.py
+-rw-rw-rw-   0        0        0       42 2023-06-09 09:56:00.347027 RobertCommonBasic-0.1.41/setup.cfg
+-rw-rw-rw-   0        0        0     3876 2023-06-09 09:27:49.000000 RobertCommonBasic-0.1.41/setup.py
```

### Comparing `RobertCommonBasic-0.1.40/LICENSE` & `RobertCommonBasic-0.1.41/LICENSE`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.40/RobertCommonBasic.egg-info/SOURCES.txt` & `RobertCommonBasic-0.1.41/RobertCommonBasic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.40/robertcommonbasic/basic/cache/utils.py` & `RobertCommonBasic-0.1.41/robertcommonbasic/basic/cache/utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.40/robertcommonbasic/basic/cls/utils.py` & `RobertCommonBasic-0.1.41/robertcommonbasic/basic/cls/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from functools import wraps
 from func_timeout import func_timeout
 from func_timeout.exceptions import FunctionTimedOut
 from multiprocessing import Pool
 from queue import Queue
-from threading import Thread, Lock, Timer, Condition
+from threading import Thread, Lock, Timer, Condition, enumerate as thread_enumerate, currentThread
 from time import time, sleep
 from typing import Callable, Optional, Union, Any
 
 
 class Singleton(type):
     _instance_lock = Lock()
 
@@ -81,14 +81,26 @@
                 raise Exception(f'func({func.__name__}) time out')
             except Exception as e:
                 raise e
         return wrapper
     return inner_set_timeout_wrapper
 
 
+def get_current_thread() -> tuple:
+    return currentThread().ident, currentThread().getName()
+
+
+def get_threads() -> dict:
+    """获取线程"""
+    threads = {}
+    for item in thread_enumerate():
+        threads[item.ident] = item.getName()
+    return threads
+
+
 class RepeatingTimer:
 
     def __init__(self, interval, function, args=None, kwargs=None):
         self.interval = interval
         self.function = function
         self.args = args if args is not None else []
         self.kwargs = kwargs if kwargs is not None else {}
@@ -145,19 +157,19 @@
         if self.is_running():
             self.timer.cancel()
         self.timer = None
 
 
 class RepeatThreadPool:
 
-    def __init__(self, size: int, fun: Optional[Callable] = None, done_callback: Optional[Callable] = None, **kwargs):
+    def __init__(self, size: int, fun: Optional[Callable] = None, done_callback: Optional[Callable] = None, thread_name_prefix: str = '', **kwargs):
         self.kwargs = kwargs
         self.pool_size = size              # 线程池大小
         self.pool_fun = fun                # 线程函数
-        self.pools = ThreadPoolExecutor(self.pool_size)  # 线程池
+        self.pools = ThreadPoolExecutor(self.pool_size, thread_name_prefix)  # 线程池
         self.done_callback = done_callback              # 线程执行回调函数
 
         self.task_queue = Queue()               # 待处理队列
         self.task_cache = {}                    # 全部任务
         self.task_running = {}                  # 正在处理任务
         self.pool_status = 'running'
         self.task_finish: int = 0               # 已完成任务
@@ -227,19 +239,19 @@
 
     def info(self):
         return {'total': len(self.task_cache), 'running': len(self.task_running), 'finish': self.task_finish}
 
 
 class SimpleThreadPool:
 
-    def __init__(self, size: int, fun: Optional[Callable] = None, done_callback: Optional[Callable] = None, **kwargs):
+    def __init__(self, size: int, fun: Optional[Callable] = None, done_callback: Optional[Callable] = None, thread_name_prefix: str = '', **kwargs):
         self.kwargs = kwargs
         self.pool_size = size              # 线程池大小
         self.pool_fun = fun                # 线程函数
-        self.pools = ThreadPoolExecutor(self.pool_size)  # 线程池
+        self.pools = ThreadPoolExecutor(self.pool_size, thread_name_prefix)  # 线程池
         self.done_callback = done_callback              # 线程执行回调函数
         self.task_future = []
 
     def submit_task(self, task: Optional[Callable], *args, **kwargs):
         task = task if task else self.pool_fun
         if task is not None:
             self.task_future.append(self.pools.submit(task, *args, **kwargs))
@@ -257,23 +269,24 @@
                 else:
                     results_list.append(result)
         return results_dict if dict_result else results_list
 
 
 class ThreadPool:
 
-    def __init__(self, pool_size: int, pool_fun: Callable, fun_params: list):
+    def __init__(self, pool_size: int, pool_fun: Callable, fun_params: list, thread_name_prefix: str = ''):
         self.pool_size = pool_size
         self.pool_fun = pool_fun
         self.fun_params = fun_params
+        self.thread_name_prefix = thread_name_prefix
         self.pool_cost = 0
 
     def run(self, dict_result: bool = True):
         start = time()
-        with ThreadPoolExecutor(self.pool_size) as executor:
+        with ThreadPoolExecutor(self.pool_size, self.thread_name_prefix) as executor:
             futures = [executor.submit(self.pool_fun, *fun_param) for fun_param in self.fun_params]
 
         results_dict = {}
         results_list = []
         for future in as_completed(futures):
             result = future.result()
             if result is not None:
```

### Comparing `RobertCommonBasic-0.1.40/robertcommonbasic/basic/data/conversion.py` & `RobertCommonBasic-0.1.41/robertcommonbasic/basic/data/conversion.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.40/robertcommonbasic/basic/data/crc16.py` & `RobertCommonBasic-0.1.41/robertcommonbasic/basic/data/crc16.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.40/robertcommonbasic/basic/data/csv.py` & `RobertCommonBasic-0.1.41/robertcommonbasic/basic/data/csv.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.40/robertcommonbasic/basic/data/datatuple.py` & `RobertCommonBasic-0.1.41/robertcommonbasic/basic/data/datatuple.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.40/robertcommonbasic/basic/data/express.py` & `RobertCommonBasic-0.1.41/robertcommonbasic/basic/data/express.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.40/robertcommonbasic/basic/data/frame.py` & `RobertCommonBasic-0.1.41/robertcommonbasic/basic/data/frame.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.40/robertcommonbasic/basic/data/nametuple.py` & `RobertCommonBasic-0.1.41/robertcommonbasic/basic/data/nametuple.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.40/robertcommonbasic/basic/data/utils.py` & `RobertCommonBasic-0.1.41/robertcommonbasic/basic/data/utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.40/robertcommonbasic/basic/decorator/utils.py` & `RobertCommonBasic-0.1.41/robertcommonbasic/basic/decorator/utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.40/robertcommonbasic/basic/dt/schedule.py` & `RobertCommonBasic-0.1.41/robertcommonbasic/basic/dt/schedule.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.40/robertcommonbasic/basic/dt/utils.py` & `RobertCommonBasic-0.1.41/robertcommonbasic/basic/dt/utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.40/robertcommonbasic/basic/encrypt/aes.py` & `RobertCommonBasic-0.1.41/robertcommonbasic/basic/encrypt/aes.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.40/robertcommonbasic/basic/encrypt/dsa.py` & `RobertCommonBasic-0.1.41/robertcommonbasic/basic/encrypt/dsa.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.40/robertcommonbasic/basic/encrypt/hash.py` & `RobertCommonBasic-0.1.41/robertcommonbasic/basic/encrypt/hash.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.40/robertcommonbasic/basic/encrypt/rsa.py` & `RobertCommonBasic-0.1.41/robertcommonbasic/basic/encrypt/rsa.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.40/robertcommonbasic/basic/error/utils.py` & `RobertCommonBasic-0.1.41/robertcommonbasic/basic/error/utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.40/robertcommonbasic/basic/exector/utils.py` & `RobertCommonBasic-0.1.41/robertcommonbasic/basic/exector/utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.40/robertcommonbasic/basic/file/csv.py` & `RobertCommonBasic-0.1.41/robertcommonbasic/basic/file/csv.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.40/robertcommonbasic/basic/file/ini.py` & `RobertCommonBasic-0.1.41/robertcommonbasic/basic/file/ini.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.40/robertcommonbasic/basic/file/log.py` & `RobertCommonBasic-0.1.41/robertcommonbasic/basic/file/log.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.40/robertcommonbasic/basic/file/xml.py` & `RobertCommonBasic-0.1.41/robertcommonbasic/basic/file/xml.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.40/robertcommonbasic/basic/file/zip.py` & `RobertCommonBasic-0.1.41/robertcommonbasic/basic/file/zip.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.40/robertcommonbasic/basic/log/utils.py` & `RobertCommonBasic-0.1.41/robertcommonbasic/basic/log/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from re import search
 from typing import Any, Optional
 from traceback import StackSummary, walk_stack
 from logging.handlers import TimedRotatingFileHandler
 
 from ..os.path import create_dir_if_not_exist
 from ..os.file import get_file_folder, get_file_name
-from ..dt.utils import get_datetime_from_stamp
 
 
 LOG_FORMAT = '[%(asctime)s] level: [%(levelname)s] module: [%(filename)s] func: [%(funcName)s] lineno: [%(lineno)d] msg: [%(message)s]'
 LOG_TIME_FORMAT = '%Y-%m-%d %H:%M:%S'
 
 
 class MyLoggerHandler(logging.Handler):
@@ -49,36 +48,38 @@
         self.utc = time.strftime("%Y-%m-%d %H:%M:%S", time.gmtime(int(self.tm)))
         _stack = stack()[1]
         self.record = {'level': log_level, 'levelname': '{0:<5s}'.format(logging.getLevelName(log_level))[:5], 'utc': self.utc, 'asctime': time.strftime(log_time_fmt, time.localtime(self.tm)) if kwargs.get('is_utc', False) is False else self.utc, 'message': msg, 'filename': get_file_name(_stack[1]), 'funcName': _stack[3], 'lineno': _stack[2], **kwargs}
 
     def format_msg(self) -> str:
         return f"{self.fmt % self.record}"
 
-    def format_source_msg(self) -> str:
-        fmt = '[%(asctime)s] level: [%(levelname)s] module: [%(filename)s] source: [%(source)s] msg: [%(message)s]'
+    def format_source_msg(self, fmt: str = '[%(asctime)s] level: [%(levelname)s] module: [%(filename)s] msg: [%(message)s] source: [%(source)s]') -> str:
         return f"{fmt % self.record}"
 
     def get_msg(self):
         return str(self.record.get('message'))
 
     def get_record(self, columns: Optional[dict] = None) -> dict:
         record = {}
         if isinstance(columns, dict) and len(columns) > 0:
             for k, v in columns.items():
                 record[v] = self.record.get(k)
         else:
             record = self.record
         return record
 
-    def print(self):
+    def print_str(self, simple_fmt: str = '[%(asctime)s] level: [%(levelname)s] module: [%(filename)s] msg: [%(message)s]', source_fmt: str = '[%(asctime)s] level: [%(levelname)s] module: [%(filename)s] msg: [%(message)s] source: [%(source)s]') -> str:
         source = self.record.get('source')
         if source is None:      # 通讯日志
-            print(self.format_msg())
+            return self.format_source_msg(simple_fmt)
         else:       # 点位日志
-            print(self.format_source_msg())
+            return self.format_source_msg(source_fmt)
+
+    def print(self, simple_fmt: str = '[%(asctime)s] level: [%(levelname)s] module: [%(filename)s] msg: [%(message)s]', source_fmt: str = '[%(asctime)s] level: [%(levelname)s] module: [%(filename)s] msg: [%(message)s] source: [%(source)s]'):
+        print(self.print_str(simple_fmt, source_fmt))
 
 
 class MyStdout:
 
     def __init__(self, autoreset: bool = True):
         init(autoreset=autoreset)
         self.stdout_bak = sys.stdout
@@ -115,23 +116,22 @@
         handler_file.setLevel(log_level)
         attach_handles.append(handler_file)
         if kwargs.get('is_utc', False) is True:
             logging.Formatter.converter = utc
         return logging.basicConfig(level=log_level, format=log_format, datefmt=log_time_fmt, handlers=attach_handles)
 
 
-def convert_msg(log_content: str):
-    if len(log_content) > 0:
-        if log_content.find('] level: [') > 0:
-            if log_content.find('] source: [') > 0:     #点错误
-                result = search(r'\[(?P<asctime>.*?)] level: \[(?P<level>.*?)] module: \[(?P<module>.*?)] source: \[(?P<source>.*?)] msg: \[(?P<msg>.*)]', log_content)
-            else:
-                result = search(r'\[(?P<asctime>.*?)] level: \[(?P<level>.*?)] module: \[(?P<module>.*?)] func: \[(?P<func>.*?)] lineno: \[(?P<lineno>.*?)] msg: \[(?P<msg>.*)]', log_content)
-            if result is not None:
-                return result.groupdict()
+def convert_msg(log_content: str, default_fmt: str = r'\[(?P<asctime>.*?)] level: \[(?P<level>.*?)] module: \[(?P<module>.*?)] func: \[(?P<func>.*?)] lineno: \[(?P<lineno>.*?)] msg: \[(?P<msg>.*)]', source_fmt: str = r'\[(?P<asctime>.*?)] level: \[(?P<level>.*?)] module: \[(?P<module>.*?)] source: \[(?P<source>.*?)] msg: \[(?P<msg>.*)]'):
+    if log_content.find('] level: [') > 0:
+        if log_content.find('] source: [') > 0:     #点错误
+            result = search(source_fmt, log_content)
+        else:
+            result = search(default_fmt, log_content)
+        if result is not None:
+            return result.groupdict()
     return log_content
 
 
 def format_log(log_content: Any):
     func = stack()[1]
     return {'file': get_file_name(func[1]), 'func': func[3], 'lineno': func[2], 'msg': log_content}
```

### Comparing `RobertCommonBasic-0.1.40/robertcommonbasic/basic/log/watch.py` & `RobertCommonBasic-0.1.41/robertcommonbasic/basic/log/watch.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.40/robertcommonbasic/basic/net/utils.py` & `RobertCommonBasic-0.1.41/robertcommonbasic/basic/net/utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.40/robertcommonbasic/basic/os/file.py` & `RobertCommonBasic-0.1.41/robertcommonbasic/basic/os/file.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.40/robertcommonbasic/basic/os/path.py` & `RobertCommonBasic-0.1.41/robertcommonbasic/basic/os/path.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.40/robertcommonbasic/basic/process/utils.py` & `RobertCommonBasic-0.1.41/robertcommonbasic/basic/process/utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.40/robertcommonbasic/basic/profile/utils.py` & `RobertCommonBasic-0.1.41/robertcommonbasic/basic/profile/utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.40/robertcommonbasic/basic/re/utils.py` & `RobertCommonBasic-0.1.41/robertcommonbasic/basic/re/utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.40/robertcommonbasic/basic/validation/input.py` & `RobertCommonBasic-0.1.41/robertcommonbasic/basic/validation/input.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_cls/test_utils.py` & `RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_cls/test_utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_data/test_conversion.py` & `RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_data/test_conversion.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_data/test_datatupple.py` & `RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_data/test_datatupple.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_data/test_frame.py` & `RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_data/test_frame.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_data/test_utils.py` & `RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_data/test_utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_dt/test_utils.py` & `RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_dt/test_utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_encrypt/test_dsa.py` & `RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_encrypt/test_dsa.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_encrypt/test_rsa.py` & `RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_encrypt/test_rsa.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_exector/test_utils.py` & `RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_exector/test_utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_file/test_csv.py` & `RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_file/test_csv.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_file/test_xml.py` & `RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_file/test_xml.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_file/test_zip.py` & `RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_file/test_zip.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_net/test_utils.py` & `RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_net/test_utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_re/test_utils.py` & `RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_re/test_utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.40/setup.py` & `RobertCommonBasic-0.1.41/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 # Package meta-data.
 NAME = 'RobertCommonBasic'
 DESCRIPTION = 'Robert Common Basic Library'
 URL = 'https://github.com/hun0423/RobertCommonBasic'
 EMAIL = '851010070@qq.com'
 AUTHOR = 'Robert0423'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.1.40'
-DATE = '2023-05-25'
+VERSION = '0.1.41'
+DATE = '2023-06-09'
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
 }
 
 # The rest you shouldn't have to touch too much :)
```

