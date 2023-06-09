# Comparing `tmp/FuncsForSPO-5.1.5.tar.gz` & `tmp/FuncsForSPO-5.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FuncsForSPO-5.1.5.tar", last modified: Wed Jun  7 19:24:08 2023, max compression
+gzip compressed data, was "FuncsForSPO-5.2.0.tar", last modified: Fri Jun  9 19:08:53 2023, max compression
```

## Comparing `FuncsForSPO-5.1.5.tar` & `FuncsForSPO-5.2.0.tar`

### file list

```diff
@@ -1,75 +1,76 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 19:24:08.918992 FuncsForSPO-5.1.5/
-drwxrwxrwx   0        0        0        0 2023-06-07 19:24:08.459373 FuncsForSPO-5.1.5/FuncsForSPO/
-drwxrwxrwx   0        0        0        0 2023-06-07 19:24:08.529987 FuncsForSPO-5.1.5/FuncsForSPO/femails/
--rw-rw-rw-   0        0        0       86 2022-10-17 17:23:21.000000 FuncsForSPO-5.1.5/FuncsForSPO/femails/__init__.py
--rw-rw-rw-   0        0        0     7124 2023-03-30 20:56:34.000000 FuncsForSPO-5.1.5/FuncsForSPO/femails/femails.py
-drwxrwxrwx   0        0        0        0 2023-06-07 19:24:08.546845 FuncsForSPO-5.1.5/FuncsForSPO/fexceptions/
--rw-rw-rw-   0        0        0       18 2022-08-09 00:49:14.000000 FuncsForSPO-5.1.5/FuncsForSPO/fexceptions/__init__.py
--rw-rw-rw-   0        0        0      602 2022-12-18 16:11:53.000000 FuncsForSPO-5.1.5/FuncsForSPO/fexceptions/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-06-07 19:24:08.562395 FuncsForSPO-5.1.5/FuncsForSPO/fftp/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-5.1.5/FuncsForSPO/fftp/__init__.py
--rw-rw-rw-   0        0        0     6205 2022-12-16 20:50:05.000000 FuncsForSPO-5.1.5/FuncsForSPO/fftp/fftp.py
-drwxrwxrwx   0        0        0        0 2023-06-07 19:24:08.569930 FuncsForSPO-5.1.5/FuncsForSPO/flanguage/
--rw-rw-rw-   0        0        0        0 2023-06-05 14:56:28.000000 FuncsForSPO-5.1.5/FuncsForSPO/flanguage/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 19:24:08.575483 FuncsForSPO-5.1.5/FuncsForSPO/flanguage/translator/
--rw-rw-rw-   0        0        0        0 2023-06-05 14:56:28.000000 FuncsForSPO-5.1.5/FuncsForSPO/flanguage/translator/__init__.py
--rw-rw-rw-   0        0        0      817 2023-06-05 14:56:55.000000 FuncsForSPO-5.1.5/FuncsForSPO/flanguage/translator/translator.py
-drwxrwxrwx   0        0        0        0 2023-06-07 19:24:08.587874 FuncsForSPO-5.1.5/FuncsForSPO/fopenpyxl/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-5.1.5/FuncsForSPO/fopenpyxl/__init__.py
--rw-rw-rw-   0        0        0    11048 2022-08-16 17:53:19.000000 FuncsForSPO-5.1.5/FuncsForSPO/fopenpyxl/openpyxl_funcs.py
-drwxrwxrwx   0        0        0        0 2023-06-07 19:24:08.595445 FuncsForSPO-5.1.5/FuncsForSPO/fpdf/
--rw-rw-rw-   0        0        0       18 2023-06-02 20:07:40.000000 FuncsForSPO-5.1.5/FuncsForSPO/fpdf/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 19:24:08.662770 FuncsForSPO-5.1.5/FuncsForSPO/fpdf/fanalyser/
--rw-rw-rw-   0        0        0      195 2023-06-02 20:07:25.000000 FuncsForSPO-5.1.5/FuncsForSPO/fpdf/fanalyser/__init__.py
--rw-rw-rw-   0        0        0     6389 2023-06-07 19:18:22.000000 FuncsForSPO-5.1.5/FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py
--rw-rw-rw-   0        0        0     3699 2023-06-07 19:14:16.000000 FuncsForSPO-5.1.5/FuncsForSPO/fpdf/fanalyser/base.py
--rw-rw-rw-   0        0        0     1134 2023-06-07 11:25:27.000000 FuncsForSPO-5.1.5/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v1.py
--rw-rw-rw-   0        0        0     2019 2023-06-07 16:48:53.000000 FuncsForSPO-5.1.5/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v2.py
-drwxrwxrwx   0        0        0        0 2023-06-07 19:24:08.685747 FuncsForSPO-5.1.5/FuncsForSPO/fpdf/fcompress/
--rw-rw-rw-   0        0        0     9145 2023-06-06 21:38:19.000000 FuncsForSPO-5.1.5/FuncsForSPO/fpdf/fcompress/__compress_online.py
--rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-5.1.5/FuncsForSPO/fpdf/fcompress/__init__.py
--rw-rw-rw-   0        0        0     1640 2023-06-06 21:39:15.000000 FuncsForSPO-5.1.5/FuncsForSPO/fpdf/fcompress/compress.py
-drwxrwxrwx   0        0        0        0 2023-06-07 19:24:08.709742 FuncsForSPO-5.1.5/FuncsForSPO/fpdf/fhtml_to_pdf/
--rw-rw-rw-   0        0        0     7094 2023-02-23 17:58:00.000000 FuncsForSPO-5.1.5/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py
--rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-5.1.5/FuncsForSPO/fpdf/fhtml_to_pdf/__init__.py
--rw-rw-rw-   0        0        0     1577 2022-11-30 15:19:23.000000 FuncsForSPO-5.1.5/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py
-drwxrwxrwx   0        0        0        0 2023-06-07 19:24:08.715820 FuncsForSPO-5.1.5/FuncsForSPO/fpdf/fimgpdf/
--rw-rw-rw-   0        0        0    12539 2023-02-23 17:58:26.000000 FuncsForSPO-5.1.5/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py
-drwxrwxrwx   0        0        0        0 2023-06-07 19:24:08.734546 FuncsForSPO-5.1.5/FuncsForSPO/fpdf/focr/
--rw-rw-rw-   0        0        0      129 2022-11-17 11:12:22.000000 FuncsForSPO-5.1.5/FuncsForSPO/fpdf/focr/__init__.py
--rw-rw-rw-   0        0        0     9646 2023-06-06 20:32:25.000000 FuncsForSPO-5.1.5/FuncsForSPO/fpdf/focr/__ocr_online.py
--rw-rw-rw-   0        0        0     5303 2023-06-06 20:31:18.000000 FuncsForSPO-5.1.5/FuncsForSPO/fpdf/focr/orc.py
-drwxrwxrwx   0        0        0        0 2023-06-07 19:24:08.744243 FuncsForSPO-5.1.5/FuncsForSPO/fpdf/pdfutils/
--rw-rw-rw-   0        0        0       18 2023-06-02 20:07:40.000000 FuncsForSPO-5.1.5/FuncsForSPO/fpdf/pdfutils/__init__.py
--rw-rw-rw-   0        0        0     1217 2023-06-07 11:50:52.000000 FuncsForSPO-5.1.5/FuncsForSPO/fpdf/pdfutils/pdfutils.py
-drwxrwxrwx   0        0        0        0 2023-06-07 19:24:08.755365 FuncsForSPO-5.1.5/FuncsForSPO/fpysimplegui/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-5.1.5/FuncsForSPO/fpysimplegui/__init__.py
--rw-rw-rw-   0        0        0     4708 2023-01-20 11:52:18.000000 FuncsForSPO-5.1.5/FuncsForSPO/fpysimplegui/functions_for_sg.py
-drwxrwxrwx   0        0        0        0 2023-06-07 19:24:08.766652 FuncsForSPO-5.1.5/FuncsForSPO/fpython/
--rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-5.1.5/FuncsForSPO/fpython/__init__.py
--rw-rw-rw-   0        0        0    67096 2023-06-03 13:16:56.000000 FuncsForSPO-5.1.5/FuncsForSPO/fpython/functions_for_py.py
-drwxrwxrwx   0        0        0        0 2023-06-07 19:24:08.778837 FuncsForSPO-5.1.5/FuncsForSPO/fregex/
--rw-rw-rw-   0        0        0       24 2022-08-09 00:49:14.000000 FuncsForSPO-5.1.5/FuncsForSPO/fregex/__init__.py
--rw-rw-rw-   0        0        0    10406 2023-01-30 14:08:06.000000 FuncsForSPO-5.1.5/FuncsForSPO/fregex/functions_re.py
-drwxrwxrwx   0        0        0        0 2023-06-07 19:24:08.789803 FuncsForSPO-5.1.5/FuncsForSPO/fselenium/
--rw-rw-rw-   0        0        0       27 2022-08-09 00:49:14.000000 FuncsForSPO-5.1.5/FuncsForSPO/fselenium/__init__.py
--rw-rw-rw-   0        0        0    39083 2023-06-06 21:05:50.000000 FuncsForSPO-5.1.5/FuncsForSPO/fselenium/functions_selenium.py
-drwxrwxrwx   0        0        0        0 2023-06-07 19:24:08.803208 FuncsForSPO-5.1.5/FuncsForSPO/fsqlite/
--rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-5.1.5/FuncsForSPO/fsqlite/__init__.py
--rw-rw-rw-   0        0        0     1610 2022-12-18 16:12:26.000000 FuncsForSPO-5.1.5/FuncsForSPO/fsqlite/sqlite_functions.py
-drwxrwxrwx   0        0        0        0 2023-06-07 19:24:08.812749 FuncsForSPO-5.1.5/FuncsForSPO/fwinotify/
--rw-rw-rw-   0        0        0       16 2022-09-12 21:24:16.000000 FuncsForSPO-5.1.5/FuncsForSPO/fwinotify/__init__.py
--rw-rw-rw-   0        0        0     4896 2022-09-12 21:21:52.000000 FuncsForSPO-5.1.5/FuncsForSPO/fwinotify/fwinotify.py
-drwxrwxrwx   0        0        0        0 2023-06-07 19:24:08.841307 FuncsForSPO-5.1.5/FuncsForSPO/utils/
--rw-rw-rw-   0        0        0   114869 2023-03-31 19:29:18.000000 FuncsForSPO-5.1.5/FuncsForSPO/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-07 19:24:08.514114 FuncsForSPO-5.1.5/FuncsForSPO.egg-info/
--rw-rw-rw-   0        0        0     8026 2023-06-07 19:24:08.000000 FuncsForSPO-5.1.5/FuncsForSPO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1770 2023-06-07 19:24:08.000000 FuncsForSPO-5.1.5/FuncsForSPO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 19:24:08.000000 FuncsForSPO-5.1.5/FuncsForSPO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      194 2023-06-07 19:24:08.000000 FuncsForSPO-5.1.5/FuncsForSPO.egg-info/requires.txt
--rw-rw-rw-   0        0        0      458 2023-06-07 19:24:08.000000 FuncsForSPO-5.1.5/FuncsForSPO.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1074 2022-12-02 16:50:42.000000 FuncsForSPO-5.1.5/LICENSE
--rw-rw-rw-   0        0        0     8026 2023-06-07 19:24:08.913440 FuncsForSPO-5.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     7607 2023-01-21 19:11:53.000000 FuncsForSPO-5.1.5/README.md
--rw-rw-rw-   0        0        0       42 2023-06-07 19:24:08.919992 FuncsForSPO-5.1.5/setup.cfg
--rw-rw-rw-   0        0        0     2506 2023-06-07 19:24:03.000000 FuncsForSPO-5.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 19:08:53.223021 FuncsForSPO-5.2.0/
+drwxrwxrwx   0        0        0        0 2023-06-09 19:08:52.797171 FuncsForSPO-5.2.0/FuncsForSPO/
+drwxrwxrwx   0        0        0        0 2023-06-09 19:08:52.849384 FuncsForSPO-5.2.0/FuncsForSPO/femails/
+-rw-rw-rw-   0        0        0       86 2022-10-17 17:23:21.000000 FuncsForSPO-5.2.0/FuncsForSPO/femails/__init__.py
+-rw-rw-rw-   0        0        0     7124 2023-03-30 20:56:34.000000 FuncsForSPO-5.2.0/FuncsForSPO/femails/femails.py
+drwxrwxrwx   0        0        0        0 2023-06-09 19:08:52.860330 FuncsForSPO-5.2.0/FuncsForSPO/fexceptions/
+-rw-rw-rw-   0        0        0       18 2022-08-09 00:49:14.000000 FuncsForSPO-5.2.0/FuncsForSPO/fexceptions/__init__.py
+-rw-rw-rw-   0        0        0      602 2022-12-18 16:11:53.000000 FuncsForSPO-5.2.0/FuncsForSPO/fexceptions/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-06-09 19:08:52.870898 FuncsForSPO-5.2.0/FuncsForSPO/fftp/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-5.2.0/FuncsForSPO/fftp/__init__.py
+-rw-rw-rw-   0        0        0     6205 2022-12-16 20:50:05.000000 FuncsForSPO-5.2.0/FuncsForSPO/fftp/fftp.py
+drwxrwxrwx   0        0        0        0 2023-06-09 19:08:52.875178 FuncsForSPO-5.2.0/FuncsForSPO/flanguage/
+-rw-rw-rw-   0        0        0        0 2023-06-05 14:56:28.000000 FuncsForSPO-5.2.0/FuncsForSPO/flanguage/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 19:08:52.879438 FuncsForSPO-5.2.0/FuncsForSPO/flanguage/translator/
+-rw-rw-rw-   0        0        0        0 2023-06-05 14:56:28.000000 FuncsForSPO-5.2.0/FuncsForSPO/flanguage/translator/__init__.py
+-rw-rw-rw-   0        0        0      817 2023-06-05 14:56:55.000000 FuncsForSPO-5.2.0/FuncsForSPO/flanguage/translator/translator.py
+drwxrwxrwx   0        0        0        0 2023-06-09 19:08:52.890258 FuncsForSPO-5.2.0/FuncsForSPO/fopenpyxl/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-5.2.0/FuncsForSPO/fopenpyxl/__init__.py
+-rw-rw-rw-   0        0        0    11048 2022-08-16 17:53:19.000000 FuncsForSPO-5.2.0/FuncsForSPO/fopenpyxl/openpyxl_funcs.py
+drwxrwxrwx   0        0        0        0 2023-06-09 19:08:52.896362 FuncsForSPO-5.2.0/FuncsForSPO/fpdf/
+-rw-rw-rw-   0        0        0       18 2023-06-02 20:07:40.000000 FuncsForSPO-5.2.0/FuncsForSPO/fpdf/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 19:08:52.927778 FuncsForSPO-5.2.0/FuncsForSPO/fpdf/fanalyser/
+-rw-rw-rw-   0        0        0      195 2023-06-02 20:07:25.000000 FuncsForSPO-5.2.0/FuncsForSPO/fpdf/fanalyser/__init__.py
+-rw-rw-rw-   0        0        0     7446 2023-06-09 19:05:30.000000 FuncsForSPO-5.2.0/FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py
+-rw-rw-rw-   0        0        0     2419 2023-06-09 19:08:44.000000 FuncsForSPO-5.2.0/FuncsForSPO/fpdf/fanalyser/base.py
+-rw-rw-rw-   0        0        0     1138 2023-06-09 17:41:46.000000 FuncsForSPO-5.2.0/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v1.py
+-rw-rw-rw-   0        0        0     2019 2023-06-07 16:48:53.000000 FuncsForSPO-5.2.0/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v2.py
+-rw-rw-rw-   0        0        0     1340 2023-06-09 19:06:51.000000 FuncsForSPO-5.2.0/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v3.py
+drwxrwxrwx   0        0        0        0 2023-06-09 19:08:52.983698 FuncsForSPO-5.2.0/FuncsForSPO/fpdf/fcompress/
+-rw-rw-rw-   0        0        0     9145 2023-06-06 21:38:19.000000 FuncsForSPO-5.2.0/FuncsForSPO/fpdf/fcompress/__compress_online.py
+-rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-5.2.0/FuncsForSPO/fpdf/fcompress/__init__.py
+-rw-rw-rw-   0        0        0     1640 2023-06-06 21:39:15.000000 FuncsForSPO-5.2.0/FuncsForSPO/fpdf/fcompress/compress.py
+drwxrwxrwx   0        0        0        0 2023-06-09 19:08:53.014446 FuncsForSPO-5.2.0/FuncsForSPO/fpdf/fhtml_to_pdf/
+-rw-rw-rw-   0        0        0     7094 2023-02-23 17:58:00.000000 FuncsForSPO-5.2.0/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py
+-rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-5.2.0/FuncsForSPO/fpdf/fhtml_to_pdf/__init__.py
+-rw-rw-rw-   0        0        0     1577 2022-11-30 15:19:23.000000 FuncsForSPO-5.2.0/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py
+drwxrwxrwx   0        0        0        0 2023-06-09 19:08:53.020473 FuncsForSPO-5.2.0/FuncsForSPO/fpdf/fimgpdf/
+-rw-rw-rw-   0        0        0    12539 2023-02-23 17:58:26.000000 FuncsForSPO-5.2.0/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py
+drwxrwxrwx   0        0        0        0 2023-06-09 19:08:53.040624 FuncsForSPO-5.2.0/FuncsForSPO/fpdf/focr/
+-rw-rw-rw-   0        0        0      129 2022-11-17 11:12:22.000000 FuncsForSPO-5.2.0/FuncsForSPO/fpdf/focr/__init__.py
+-rw-rw-rw-   0        0        0     9646 2023-06-06 20:32:25.000000 FuncsForSPO-5.2.0/FuncsForSPO/fpdf/focr/__ocr_online.py
+-rw-rw-rw-   0        0        0     5303 2023-06-06 20:31:18.000000 FuncsForSPO-5.2.0/FuncsForSPO/fpdf/focr/orc.py
+drwxrwxrwx   0        0        0        0 2023-06-09 19:08:53.054329 FuncsForSPO-5.2.0/FuncsForSPO/fpdf/pdfutils/
+-rw-rw-rw-   0        0        0       18 2023-06-02 20:07:40.000000 FuncsForSPO-5.2.0/FuncsForSPO/fpdf/pdfutils/__init__.py
+-rw-rw-rw-   0        0        0     1217 2023-06-07 11:50:52.000000 FuncsForSPO-5.2.0/FuncsForSPO/fpdf/pdfutils/pdfutils.py
+drwxrwxrwx   0        0        0        0 2023-06-09 19:08:53.067592 FuncsForSPO-5.2.0/FuncsForSPO/fpysimplegui/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-5.2.0/FuncsForSPO/fpysimplegui/__init__.py
+-rw-rw-rw-   0        0        0     4708 2023-01-20 11:52:18.000000 FuncsForSPO-5.2.0/FuncsForSPO/fpysimplegui/functions_for_sg.py
+drwxrwxrwx   0        0        0        0 2023-06-09 19:08:53.080773 FuncsForSPO-5.2.0/FuncsForSPO/fpython/
+-rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-5.2.0/FuncsForSPO/fpython/__init__.py
+-rw-rw-rw-   0        0        0    67096 2023-06-03 13:16:56.000000 FuncsForSPO-5.2.0/FuncsForSPO/fpython/functions_for_py.py
+drwxrwxrwx   0        0        0        0 2023-06-09 19:08:53.093290 FuncsForSPO-5.2.0/FuncsForSPO/fregex/
+-rw-rw-rw-   0        0        0       24 2022-08-09 00:49:14.000000 FuncsForSPO-5.2.0/FuncsForSPO/fregex/__init__.py
+-rw-rw-rw-   0        0        0    10406 2023-01-30 14:08:06.000000 FuncsForSPO-5.2.0/FuncsForSPO/fregex/functions_re.py
+drwxrwxrwx   0        0        0        0 2023-06-09 19:08:53.104745 FuncsForSPO-5.2.0/FuncsForSPO/fselenium/
+-rw-rw-rw-   0        0        0       27 2022-08-09 00:49:14.000000 FuncsForSPO-5.2.0/FuncsForSPO/fselenium/__init__.py
+-rw-rw-rw-   0        0        0    39083 2023-06-06 21:05:50.000000 FuncsForSPO-5.2.0/FuncsForSPO/fselenium/functions_selenium.py
+drwxrwxrwx   0        0        0        0 2023-06-09 19:08:53.118956 FuncsForSPO-5.2.0/FuncsForSPO/fsqlite/
+-rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-5.2.0/FuncsForSPO/fsqlite/__init__.py
+-rw-rw-rw-   0        0        0     1610 2022-12-18 16:12:26.000000 FuncsForSPO-5.2.0/FuncsForSPO/fsqlite/sqlite_functions.py
+drwxrwxrwx   0        0        0        0 2023-06-09 19:08:53.132094 FuncsForSPO-5.2.0/FuncsForSPO/fwinotify/
+-rw-rw-rw-   0        0        0       16 2022-09-12 21:24:16.000000 FuncsForSPO-5.2.0/FuncsForSPO/fwinotify/__init__.py
+-rw-rw-rw-   0        0        0     4896 2022-09-12 21:21:52.000000 FuncsForSPO-5.2.0/FuncsForSPO/fwinotify/fwinotify.py
+drwxrwxrwx   0        0        0        0 2023-06-09 19:08:53.139625 FuncsForSPO-5.2.0/FuncsForSPO/utils/
+-rw-rw-rw-   0        0        0   114869 2023-03-31 19:29:18.000000 FuncsForSPO-5.2.0/FuncsForSPO/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-09 19:08:52.840086 FuncsForSPO-5.2.0/FuncsForSPO.egg-info/
+-rw-rw-rw-   0        0        0     8026 2023-06-09 19:08:52.000000 FuncsForSPO-5.2.0/FuncsForSPO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1815 2023-06-09 19:08:52.000000 FuncsForSPO-5.2.0/FuncsForSPO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 19:08:52.000000 FuncsForSPO-5.2.0/FuncsForSPO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      194 2023-06-09 19:08:52.000000 FuncsForSPO-5.2.0/FuncsForSPO.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      458 2023-06-09 19:08:52.000000 FuncsForSPO-5.2.0/FuncsForSPO.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1074 2022-12-02 16:50:42.000000 FuncsForSPO-5.2.0/LICENSE
+-rw-rw-rw-   0        0        0     8026 2023-06-09 19:08:53.219543 FuncsForSPO-5.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7607 2023-01-21 19:11:53.000000 FuncsForSPO-5.2.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-09 19:08:53.224528 FuncsForSPO-5.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     2506 2023-06-09 18:52:02.000000 FuncsForSPO-5.2.0/setup.py
```

### Comparing `FuncsForSPO-5.1.5/FuncsForSPO/femails/femails.py` & `FuncsForSPO-5.2.0/FuncsForSPO/femails/femails.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.5/FuncsForSPO/fexceptions/exceptions.py` & `FuncsForSPO-5.2.0/FuncsForSPO/fexceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.5/FuncsForSPO/fftp/fftp.py` & `FuncsForSPO-5.2.0/FuncsForSPO/fftp/fftp.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.5/FuncsForSPO/flanguage/translator/translator.py` & `FuncsForSPO-5.2.0/FuncsForSPO/flanguage/translator/translator.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.5/FuncsForSPO/fopenpyxl/openpyxl_funcs.py` & `FuncsForSPO-5.2.0/FuncsForSPO/fopenpyxl/openpyxl_funcs.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.5/FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py` & `FuncsForSPO-5.2.0/FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py`

 * *Files 14% similar despite different names*

```diff
@@ -96,32 +96,53 @@
             faz_log(repr(e), 'c*')
             faz_log(self.DRIVER.get_screenshot_as_base64(), 'i*')
             self.DRIVER.quit()
             raise ErroPDFAIException
 
 
 class GPTPDFV2(BotMain):    
-    def __init__(self, file_pdf: str, prompt:str, headless: bool=True) -> str:
-        self.PDF_PATH = os.path.abspath(file_pdf)
+    def __init__(self, content_txt: str, prompt:str, headless: bool=True) -> str:
+        cria_dir_no_dir_de_trabalho_atual('tempdir')
+        faz_log('Criando arquivo em uma pasta temporária')
+        self.TXT_CONTENT = arquivo_com_caminho_absoluto('tempdir', 'temp.txt')
+        with open(self.TXT_CONTENT, 'w', encoding='utf-8') as f:
+            f.write(content_txt)
+        
+        
         self.PROMPT = prompt
         self.HEADLESS = headless
         super().__init__(self.HEADLESS)
     
     def run(self):
         try:
+            faz_log('Indo para askyourpdf')
             self.DRIVER.get('https://askyourpdf.com/')
             espera_elemento(self.WDW, (By.CSS_SELECTOR, 'input[type="file"]'), in_dom=True)
-            self.DRIVER.find_element(By.CSS_SELECTOR, 'input[type="file"]').send_keys(self.PDF_PATH)
-
+            self.DRIVER.find_element(By.CSS_SELECTOR, 'input[type="file"]').send_keys(self.TXT_CONTENT)
+            
+            faz_log('Documento enviado, aguardando entrada para o prompt')
             espera_input_limpa_e_envia_send_keys(self.WDW130, 'Adicione "AI RESPONSE" no final da sua resposta. '+self.PROMPT, (By.CSS_SELECTOR, 'textarea[placeholder="Write your question"]'))
             espera_elemento_disponivel_e_clica(self.WDW130, (By.CSS_SELECTOR, 'button[class*="ant-btn-default"]'))
             faz_log('Esperando a resposta')
             while True:
-                text = espera_e_retorna_elemento_text(self.WDW, (By.CSS_SELECTOR, 'div[style="padding: 5px;"]>div:last-of-type>div:last-of-type span'))
+                try:
+                    text = espera_e_retorna_elemento_text(self.WDW, (By.CSS_SELECTOR, 'div[style="padding: 5px;"]>div:last-of-type>div:last-of-type span'))
+                    faz_log(f'Resposta até agora: {text}')
+                    sleep(1)
+                except:...
                 if 'AI RES' in text:
                     break
+            faz_log('Recuperando o id do documento')
+            url = self.DRIVER.current_url
+            id_ = re.sub(r'.*?/chat/', '', url)
+            self.DRIVER.get('https://askyourpdf.com/delete')
+            espera_elemento_e_envia_send_keys(self.WDW, id_, (By.CSS_SELECTOR, 'input'))
+            espera_elemento_disponivel_e_clica(self.WDW, (By.CSS_SELECTOR, 'button'))
+            sleep(2)
+            faz_log('Documento deletado da base de dados!')
+            os.remove(self.TXT_CONTENT)
             return text
         except Exception as e:
             faz_log(repr(e), 'c*')
             faz_log(self.DRIVER.get_screenshot_as_base64(), 'i*')
             self.DRIVER.quit()
             raise ErroPDFAIException
```

### Comparing `FuncsForSPO-5.1.5/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v1.py` & `FuncsForSPO-5.2.0/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v1.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,9 +18,11 @@
 	"""
     # CREDENTIALS EXEMPLE -> (username, password)
     app = GPTPDFV1(file_pdf=file_pdf, credentials=credentials, prompt=prompt, headless=headless)
     text = app.run()
     return text
 
 
+
+
 # file_pdf='initial_9232.pdf', prompt='analise e me fale em portugues esse pdf', headless=True, credentials=('githubpaycon', 'bolarede792')
```

### Comparing `FuncsForSPO-5.1.5/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v2.py` & `FuncsForSPO-5.2.0/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v2.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.5/FuncsForSPO/fpdf/fcompress/__compress_online.py` & `FuncsForSPO-5.2.0/FuncsForSPO/fpdf/fcompress/__compress_online.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.5/FuncsForSPO/fpdf/fcompress/compress.py` & `FuncsForSPO-5.2.0/FuncsForSPO/fpdf/fcompress/compress.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.5/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py` & `FuncsForSPO-5.2.0/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.5/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py` & `FuncsForSPO-5.2.0/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.5/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py` & `FuncsForSPO-5.2.0/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.5/FuncsForSPO/fpdf/focr/__ocr_online.py` & `FuncsForSPO-5.2.0/FuncsForSPO/fpdf/focr/__ocr_online.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.5/FuncsForSPO/fpdf/focr/orc.py` & `FuncsForSPO-5.2.0/FuncsForSPO/fpdf/focr/orc.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.5/FuncsForSPO/fpdf/pdfutils/pdfutils.py` & `FuncsForSPO-5.2.0/FuncsForSPO/fpdf/pdfutils/pdfutils.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.5/FuncsForSPO/fpysimplegui/functions_for_sg.py` & `FuncsForSPO-5.2.0/FuncsForSPO/fpysimplegui/functions_for_sg.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.5/FuncsForSPO/fpython/functions_for_py.py` & `FuncsForSPO-5.2.0/FuncsForSPO/fpython/functions_for_py.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.5/FuncsForSPO/fregex/functions_re.py` & `FuncsForSPO-5.2.0/FuncsForSPO/fregex/functions_re.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.5/FuncsForSPO/fselenium/functions_selenium.py` & `FuncsForSPO-5.2.0/FuncsForSPO/fselenium/functions_selenium.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.5/FuncsForSPO/fsqlite/sqlite_functions.py` & `FuncsForSPO-5.2.0/FuncsForSPO/fsqlite/sqlite_functions.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.5/FuncsForSPO/fwinotify/fwinotify.py` & `FuncsForSPO-5.2.0/FuncsForSPO/fwinotify/fwinotify.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.5/FuncsForSPO/utils/utils.py` & `FuncsForSPO-5.2.0/FuncsForSPO/utils/utils.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.5/FuncsForSPO.egg-info/PKG-INFO` & `FuncsForSPO-5.2.0/FuncsForSPO.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FuncsForSPO
-Version: 5.1.5
+Version: 5.2.0
 Summary: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Home-page: https://github.com/githubpaycon/FuncsForSPO
 Author: Gabriel Lopes de Souza
 Author-email: githubpaycon@gmail.com
 License: MIT License
 Keywords: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Description-Content-Type: text/markdown
```

### Comparing `FuncsForSPO-5.1.5/FuncsForSPO.egg-info/SOURCES.txt` & `FuncsForSPO-5.2.0/FuncsForSPO.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 FuncsForSPO/fopenpyxl/openpyxl_funcs.py
 FuncsForSPO/fpdf/__init__.py
 FuncsForSPO/fpdf/fanalyser/__init__.py
 FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py
 FuncsForSPO/fpdf/fanalyser/base.py
 FuncsForSPO/fpdf/fanalyser/pdfanalyser_v1.py
 FuncsForSPO/fpdf/fanalyser/pdfanalyser_v2.py
+FuncsForSPO/fpdf/fanalyser/pdfanalyser_v3.py
 FuncsForSPO/fpdf/fcompress/__compress_online.py
 FuncsForSPO/fpdf/fcompress/__init__.py
 FuncsForSPO/fpdf/fcompress/compress.py
 FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py
 FuncsForSPO/fpdf/fhtml_to_pdf/__init__.py
 FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py
 FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py
```

### Comparing `FuncsForSPO-5.1.5/LICENSE` & `FuncsForSPO-5.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.5/PKG-INFO` & `FuncsForSPO-5.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FuncsForSPO
-Version: 5.1.5
+Version: 5.2.0
 Summary: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Home-page: https://github.com/githubpaycon/FuncsForSPO
 Author: Gabriel Lopes de Souza
 Author-email: githubpaycon@gmail.com
 License: MIT License
 Keywords: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Description-Content-Type: text/markdown
```

### Comparing `FuncsForSPO-5.1.5/README.md` & `FuncsForSPO-5.2.0/README.md`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.5/setup.py` & `FuncsForSPO-5.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 from setuptools import setup
 
-version = '5.1.5'
+version = '5.2.0'
 
 with open("README.md", "r", encoding='utf-8') as fh:
     readme = fh.read()
     setup(
         name='FuncsForSPO',
         version=version,
         url='https://github.com/githubpaycon/FuncsForSPO',
```

