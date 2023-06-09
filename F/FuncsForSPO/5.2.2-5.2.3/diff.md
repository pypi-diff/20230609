# Comparing `tmp/FuncsForSPO-5.2.2.tar.gz` & `tmp/FuncsForSPO-5.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FuncsForSPO-5.2.2.tar", last modified: Fri Jun  9 19:38:35 2023, max compression
+gzip compressed data, was "FuncsForSPO-5.2.3.tar", last modified: Fri Jun  9 19:43:26 2023, max compression
```

## Comparing `FuncsForSPO-5.2.2.tar` & `FuncsForSPO-5.2.3.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 19:38:35.503705 FuncsForSPO-5.2.2/
-drwxrwxrwx   0        0        0        0 2023-06-09 19:38:35.121937 FuncsForSPO-5.2.2/FuncsForSPO/
-drwxrwxrwx   0        0        0        0 2023-06-09 19:38:35.178411 FuncsForSPO-5.2.2/FuncsForSPO/femails/
--rw-rw-rw-   0        0        0       86 2022-10-17 17:23:21.000000 FuncsForSPO-5.2.2/FuncsForSPO/femails/__init__.py
--rw-rw-rw-   0        0        0     7124 2023-03-30 20:56:34.000000 FuncsForSPO-5.2.2/FuncsForSPO/femails/femails.py
-drwxrwxrwx   0        0        0        0 2023-06-09 19:38:35.188549 FuncsForSPO-5.2.2/FuncsForSPO/fexceptions/
--rw-rw-rw-   0        0        0       18 2022-08-09 00:49:14.000000 FuncsForSPO-5.2.2/FuncsForSPO/fexceptions/__init__.py
--rw-rw-rw-   0        0        0      602 2022-12-18 16:11:53.000000 FuncsForSPO-5.2.2/FuncsForSPO/fexceptions/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-06-09 19:38:35.198451 FuncsForSPO-5.2.2/FuncsForSPO/fftp/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-5.2.2/FuncsForSPO/fftp/__init__.py
--rw-rw-rw-   0        0        0     6205 2022-12-16 20:50:05.000000 FuncsForSPO-5.2.2/FuncsForSPO/fftp/fftp.py
-drwxrwxrwx   0        0        0        0 2023-06-09 19:38:35.203540 FuncsForSPO-5.2.2/FuncsForSPO/flanguage/
--rw-rw-rw-   0        0        0        0 2023-06-05 14:56:28.000000 FuncsForSPO-5.2.2/FuncsForSPO/flanguage/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 19:38:35.206544 FuncsForSPO-5.2.2/FuncsForSPO/flanguage/translator/
--rw-rw-rw-   0        0        0        0 2023-06-05 14:56:28.000000 FuncsForSPO-5.2.2/FuncsForSPO/flanguage/translator/__init__.py
--rw-rw-rw-   0        0        0      817 2023-06-05 14:56:55.000000 FuncsForSPO-5.2.2/FuncsForSPO/flanguage/translator/translator.py
-drwxrwxrwx   0        0        0        0 2023-06-09 19:38:35.217419 FuncsForSPO-5.2.2/FuncsForSPO/fopenpyxl/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-5.2.2/FuncsForSPO/fopenpyxl/__init__.py
--rw-rw-rw-   0        0        0    11048 2022-08-16 17:53:19.000000 FuncsForSPO-5.2.2/FuncsForSPO/fopenpyxl/openpyxl_funcs.py
-drwxrwxrwx   0        0        0        0 2023-06-09 19:38:35.221439 FuncsForSPO-5.2.2/FuncsForSPO/fpdf/
--rw-rw-rw-   0        0        0       18 2023-06-02 20:07:40.000000 FuncsForSPO-5.2.2/FuncsForSPO/fpdf/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 19:38:35.254016 FuncsForSPO-5.2.2/FuncsForSPO/fpdf/fanalyser/
--rw-rw-rw-   0        0        0      195 2023-06-02 20:07:25.000000 FuncsForSPO-5.2.2/FuncsForSPO/fpdf/fanalyser/__init__.py
--rw-rw-rw-   0        0        0     7801 2023-06-09 19:38:18.000000 FuncsForSPO-5.2.2/FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py
--rw-rw-rw-   0        0        0     2419 2023-06-09 19:08:44.000000 FuncsForSPO-5.2.2/FuncsForSPO/fpdf/fanalyser/base.py
--rw-rw-rw-   0        0        0     1138 2023-06-09 17:41:46.000000 FuncsForSPO-5.2.2/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v1.py
--rw-rw-rw-   0        0        0     2019 2023-06-07 16:48:53.000000 FuncsForSPO-5.2.2/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v2.py
--rw-rw-rw-   0        0        0     1340 2023-06-09 19:06:51.000000 FuncsForSPO-5.2.2/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v3.py
-drwxrwxrwx   0        0        0        0 2023-06-09 19:38:35.276388 FuncsForSPO-5.2.2/FuncsForSPO/fpdf/fcompress/
--rw-rw-rw-   0        0        0     9145 2023-06-06 21:38:19.000000 FuncsForSPO-5.2.2/FuncsForSPO/fpdf/fcompress/__compress_online.py
--rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-5.2.2/FuncsForSPO/fpdf/fcompress/__init__.py
--rw-rw-rw-   0        0        0     1640 2023-06-06 21:39:15.000000 FuncsForSPO-5.2.2/FuncsForSPO/fpdf/fcompress/compress.py
-drwxrwxrwx   0        0        0        0 2023-06-09 19:38:35.298645 FuncsForSPO-5.2.2/FuncsForSPO/fpdf/fhtml_to_pdf/
--rw-rw-rw-   0        0        0     7094 2023-02-23 17:58:00.000000 FuncsForSPO-5.2.2/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py
--rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-5.2.2/FuncsForSPO/fpdf/fhtml_to_pdf/__init__.py
--rw-rw-rw-   0        0        0     1577 2022-11-30 15:19:23.000000 FuncsForSPO-5.2.2/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py
-drwxrwxrwx   0        0        0        0 2023-06-09 19:38:35.304842 FuncsForSPO-5.2.2/FuncsForSPO/fpdf/fimgpdf/
--rw-rw-rw-   0        0        0    12539 2023-02-23 17:58:26.000000 FuncsForSPO-5.2.2/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py
-drwxrwxrwx   0        0        0        0 2023-06-09 19:38:35.323765 FuncsForSPO-5.2.2/FuncsForSPO/fpdf/focr/
--rw-rw-rw-   0        0        0      129 2022-11-17 11:12:22.000000 FuncsForSPO-5.2.2/FuncsForSPO/fpdf/focr/__init__.py
--rw-rw-rw-   0        0        0     9646 2023-06-06 20:32:25.000000 FuncsForSPO-5.2.2/FuncsForSPO/fpdf/focr/__ocr_online.py
--rw-rw-rw-   0        0        0     5303 2023-06-06 20:31:18.000000 FuncsForSPO-5.2.2/FuncsForSPO/fpdf/focr/orc.py
-drwxrwxrwx   0        0        0        0 2023-06-09 19:38:35.336573 FuncsForSPO-5.2.2/FuncsForSPO/fpdf/pdfutils/
--rw-rw-rw-   0        0        0       18 2023-06-02 20:07:40.000000 FuncsForSPO-5.2.2/FuncsForSPO/fpdf/pdfutils/__init__.py
--rw-rw-rw-   0        0        0     1217 2023-06-07 11:50:52.000000 FuncsForSPO-5.2.2/FuncsForSPO/fpdf/pdfutils/pdfutils.py
-drwxrwxrwx   0        0        0        0 2023-06-09 19:38:35.345620 FuncsForSPO-5.2.2/FuncsForSPO/fpysimplegui/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-5.2.2/FuncsForSPO/fpysimplegui/__init__.py
--rw-rw-rw-   0        0        0     4708 2023-01-20 11:52:18.000000 FuncsForSPO-5.2.2/FuncsForSPO/fpysimplegui/functions_for_sg.py
-drwxrwxrwx   0        0        0        0 2023-06-09 19:38:35.356152 FuncsForSPO-5.2.2/FuncsForSPO/fpython/
--rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-5.2.2/FuncsForSPO/fpython/__init__.py
--rw-rw-rw-   0        0        0    67096 2023-06-03 13:16:56.000000 FuncsForSPO-5.2.2/FuncsForSPO/fpython/functions_for_py.py
-drwxrwxrwx   0        0        0        0 2023-06-09 19:38:35.367462 FuncsForSPO-5.2.2/FuncsForSPO/fregex/
--rw-rw-rw-   0        0        0       24 2022-08-09 00:49:14.000000 FuncsForSPO-5.2.2/FuncsForSPO/fregex/__init__.py
--rw-rw-rw-   0        0        0    10406 2023-01-30 14:08:06.000000 FuncsForSPO-5.2.2/FuncsForSPO/fregex/functions_re.py
-drwxrwxrwx   0        0        0        0 2023-06-09 19:38:35.377701 FuncsForSPO-5.2.2/FuncsForSPO/fselenium/
--rw-rw-rw-   0        0        0       27 2022-08-09 00:49:14.000000 FuncsForSPO-5.2.2/FuncsForSPO/fselenium/__init__.py
--rw-rw-rw-   0        0        0    39083 2023-06-06 21:05:50.000000 FuncsForSPO-5.2.2/FuncsForSPO/fselenium/functions_selenium.py
-drwxrwxrwx   0        0        0        0 2023-06-09 19:38:35.389424 FuncsForSPO-5.2.2/FuncsForSPO/fsqlite/
--rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-5.2.2/FuncsForSPO/fsqlite/__init__.py
--rw-rw-rw-   0        0        0     1610 2022-12-18 16:12:26.000000 FuncsForSPO-5.2.2/FuncsForSPO/fsqlite/sqlite_functions.py
-drwxrwxrwx   0        0        0        0 2023-06-09 19:38:35.399885 FuncsForSPO-5.2.2/FuncsForSPO/fwinotify/
--rw-rw-rw-   0        0        0       16 2022-09-12 21:24:16.000000 FuncsForSPO-5.2.2/FuncsForSPO/fwinotify/__init__.py
--rw-rw-rw-   0        0        0     4896 2022-09-12 21:21:52.000000 FuncsForSPO-5.2.2/FuncsForSPO/fwinotify/fwinotify.py
-drwxrwxrwx   0        0        0        0 2023-06-09 19:38:35.405327 FuncsForSPO-5.2.2/FuncsForSPO/utils/
--rw-rw-rw-   0        0        0   114869 2023-03-31 19:29:18.000000 FuncsForSPO-5.2.2/FuncsForSPO/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-09 19:38:35.169663 FuncsForSPO-5.2.2/FuncsForSPO.egg-info/
--rw-rw-rw-   0        0        0     8026 2023-06-09 19:38:34.000000 FuncsForSPO-5.2.2/FuncsForSPO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1815 2023-06-09 19:38:35.000000 FuncsForSPO-5.2.2/FuncsForSPO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 19:38:34.000000 FuncsForSPO-5.2.2/FuncsForSPO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      194 2023-06-09 19:38:34.000000 FuncsForSPO-5.2.2/FuncsForSPO.egg-info/requires.txt
--rw-rw-rw-   0        0        0      458 2023-06-09 19:38:34.000000 FuncsForSPO-5.2.2/FuncsForSPO.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1074 2022-12-02 16:50:42.000000 FuncsForSPO-5.2.2/LICENSE
--rw-rw-rw-   0        0        0     8026 2023-06-09 19:38:35.498530 FuncsForSPO-5.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     7607 2023-01-21 19:11:53.000000 FuncsForSPO-5.2.2/README.md
--rw-rw-rw-   0        0        0       42 2023-06-09 19:38:35.504716 FuncsForSPO-5.2.2/setup.cfg
--rw-rw-rw-   0        0        0     2506 2023-06-09 19:38:27.000000 FuncsForSPO-5.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 19:43:26.180350 FuncsForSPO-5.2.3/
+drwxrwxrwx   0        0        0        0 2023-06-09 19:43:25.762128 FuncsForSPO-5.2.3/FuncsForSPO/
+drwxrwxrwx   0        0        0        0 2023-06-09 19:43:25.828464 FuncsForSPO-5.2.3/FuncsForSPO/femails/
+-rw-rw-rw-   0        0        0       86 2022-10-17 17:23:21.000000 FuncsForSPO-5.2.3/FuncsForSPO/femails/__init__.py
+-rw-rw-rw-   0        0        0     7124 2023-03-30 20:56:34.000000 FuncsForSPO-5.2.3/FuncsForSPO/femails/femails.py
+drwxrwxrwx   0        0        0        0 2023-06-09 19:43:25.838239 FuncsForSPO-5.2.3/FuncsForSPO/fexceptions/
+-rw-rw-rw-   0        0        0       18 2022-08-09 00:49:14.000000 FuncsForSPO-5.2.3/FuncsForSPO/fexceptions/__init__.py
+-rw-rw-rw-   0        0        0      602 2022-12-18 16:11:53.000000 FuncsForSPO-5.2.3/FuncsForSPO/fexceptions/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-06-09 19:43:25.880276 FuncsForSPO-5.2.3/FuncsForSPO/fftp/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-5.2.3/FuncsForSPO/fftp/__init__.py
+-rw-rw-rw-   0        0        0     6205 2022-12-16 20:50:05.000000 FuncsForSPO-5.2.3/FuncsForSPO/fftp/fftp.py
+drwxrwxrwx   0        0        0        0 2023-06-09 19:43:25.886762 FuncsForSPO-5.2.3/FuncsForSPO/flanguage/
+-rw-rw-rw-   0        0        0        0 2023-06-05 14:56:28.000000 FuncsForSPO-5.2.3/FuncsForSPO/flanguage/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 19:43:25.894297 FuncsForSPO-5.2.3/FuncsForSPO/flanguage/translator/
+-rw-rw-rw-   0        0        0        0 2023-06-05 14:56:28.000000 FuncsForSPO-5.2.3/FuncsForSPO/flanguage/translator/__init__.py
+-rw-rw-rw-   0        0        0      817 2023-06-05 14:56:55.000000 FuncsForSPO-5.2.3/FuncsForSPO/flanguage/translator/translator.py
+drwxrwxrwx   0        0        0        0 2023-06-09 19:43:25.904892 FuncsForSPO-5.2.3/FuncsForSPO/fopenpyxl/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-5.2.3/FuncsForSPO/fopenpyxl/__init__.py
+-rw-rw-rw-   0        0        0    11048 2022-08-16 17:53:19.000000 FuncsForSPO-5.2.3/FuncsForSPO/fopenpyxl/openpyxl_funcs.py
+drwxrwxrwx   0        0        0        0 2023-06-09 19:43:25.911467 FuncsForSPO-5.2.3/FuncsForSPO/fpdf/
+-rw-rw-rw-   0        0        0       18 2023-06-02 20:07:40.000000 FuncsForSPO-5.2.3/FuncsForSPO/fpdf/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 19:43:25.940307 FuncsForSPO-5.2.3/FuncsForSPO/fpdf/fanalyser/
+-rw-rw-rw-   0        0        0      195 2023-06-02 20:07:25.000000 FuncsForSPO-5.2.3/FuncsForSPO/fpdf/fanalyser/__init__.py
+-rw-rw-rw-   0        0        0     7741 2023-06-09 19:43:08.000000 FuncsForSPO-5.2.3/FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py
+-rw-rw-rw-   0        0        0     2419 2023-06-09 19:08:44.000000 FuncsForSPO-5.2.3/FuncsForSPO/fpdf/fanalyser/base.py
+-rw-rw-rw-   0        0        0     1138 2023-06-09 17:41:46.000000 FuncsForSPO-5.2.3/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v1.py
+-rw-rw-rw-   0        0        0     2019 2023-06-07 16:48:53.000000 FuncsForSPO-5.2.3/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v2.py
+-rw-rw-rw-   0        0        0     1340 2023-06-09 19:06:51.000000 FuncsForSPO-5.2.3/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v3.py
+drwxrwxrwx   0        0        0        0 2023-06-09 19:43:25.960226 FuncsForSPO-5.2.3/FuncsForSPO/fpdf/fcompress/
+-rw-rw-rw-   0        0        0     9145 2023-06-06 21:38:19.000000 FuncsForSPO-5.2.3/FuncsForSPO/fpdf/fcompress/__compress_online.py
+-rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-5.2.3/FuncsForSPO/fpdf/fcompress/__init__.py
+-rw-rw-rw-   0        0        0     1640 2023-06-06 21:39:15.000000 FuncsForSPO-5.2.3/FuncsForSPO/fpdf/fcompress/compress.py
+drwxrwxrwx   0        0        0        0 2023-06-09 19:43:25.976171 FuncsForSPO-5.2.3/FuncsForSPO/fpdf/fhtml_to_pdf/
+-rw-rw-rw-   0        0        0     7094 2023-02-23 17:58:00.000000 FuncsForSPO-5.2.3/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py
+-rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-5.2.3/FuncsForSPO/fpdf/fhtml_to_pdf/__init__.py
+-rw-rw-rw-   0        0        0     1577 2022-11-30 15:19:23.000000 FuncsForSPO-5.2.3/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py
+drwxrwxrwx   0        0        0        0 2023-06-09 19:43:25.981491 FuncsForSPO-5.2.3/FuncsForSPO/fpdf/fimgpdf/
+-rw-rw-rw-   0        0        0    12539 2023-02-23 17:58:26.000000 FuncsForSPO-5.2.3/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py
+drwxrwxrwx   0        0        0        0 2023-06-09 19:43:25.996294 FuncsForSPO-5.2.3/FuncsForSPO/fpdf/focr/
+-rw-rw-rw-   0        0        0      129 2022-11-17 11:12:22.000000 FuncsForSPO-5.2.3/FuncsForSPO/fpdf/focr/__init__.py
+-rw-rw-rw-   0        0        0     9646 2023-06-06 20:32:25.000000 FuncsForSPO-5.2.3/FuncsForSPO/fpdf/focr/__ocr_online.py
+-rw-rw-rw-   0        0        0     5303 2023-06-06 20:31:18.000000 FuncsForSPO-5.2.3/FuncsForSPO/fpdf/focr/orc.py
+drwxrwxrwx   0        0        0        0 2023-06-09 19:43:26.006471 FuncsForSPO-5.2.3/FuncsForSPO/fpdf/pdfutils/
+-rw-rw-rw-   0        0        0       18 2023-06-02 20:07:40.000000 FuncsForSPO-5.2.3/FuncsForSPO/fpdf/pdfutils/__init__.py
+-rw-rw-rw-   0        0        0     1217 2023-06-07 11:50:52.000000 FuncsForSPO-5.2.3/FuncsForSPO/fpdf/pdfutils/pdfutils.py
+drwxrwxrwx   0        0        0        0 2023-06-09 19:43:26.016115 FuncsForSPO-5.2.3/FuncsForSPO/fpysimplegui/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-5.2.3/FuncsForSPO/fpysimplegui/__init__.py
+-rw-rw-rw-   0        0        0     4708 2023-01-20 11:52:18.000000 FuncsForSPO-5.2.3/FuncsForSPO/fpysimplegui/functions_for_sg.py
+drwxrwxrwx   0        0        0        0 2023-06-09 19:43:26.026946 FuncsForSPO-5.2.3/FuncsForSPO/fpython/
+-rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-5.2.3/FuncsForSPO/fpython/__init__.py
+-rw-rw-rw-   0        0        0    67096 2023-06-03 13:16:56.000000 FuncsForSPO-5.2.3/FuncsForSPO/fpython/functions_for_py.py
+drwxrwxrwx   0        0        0        0 2023-06-09 19:43:26.035478 FuncsForSPO-5.2.3/FuncsForSPO/fregex/
+-rw-rw-rw-   0        0        0       24 2022-08-09 00:49:14.000000 FuncsForSPO-5.2.3/FuncsForSPO/fregex/__init__.py
+-rw-rw-rw-   0        0        0    10406 2023-01-30 14:08:06.000000 FuncsForSPO-5.2.3/FuncsForSPO/fregex/functions_re.py
+drwxrwxrwx   0        0        0        0 2023-06-09 19:43:26.046638 FuncsForSPO-5.2.3/FuncsForSPO/fselenium/
+-rw-rw-rw-   0        0        0       27 2022-08-09 00:49:14.000000 FuncsForSPO-5.2.3/FuncsForSPO/fselenium/__init__.py
+-rw-rw-rw-   0        0        0    39083 2023-06-06 21:05:50.000000 FuncsForSPO-5.2.3/FuncsForSPO/fselenium/functions_selenium.py
+drwxrwxrwx   0        0        0        0 2023-06-09 19:43:26.059375 FuncsForSPO-5.2.3/FuncsForSPO/fsqlite/
+-rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-5.2.3/FuncsForSPO/fsqlite/__init__.py
+-rw-rw-rw-   0        0        0     1610 2022-12-18 16:12:26.000000 FuncsForSPO-5.2.3/FuncsForSPO/fsqlite/sqlite_functions.py
+drwxrwxrwx   0        0        0        0 2023-06-09 19:43:26.067983 FuncsForSPO-5.2.3/FuncsForSPO/fwinotify/
+-rw-rw-rw-   0        0        0       16 2022-09-12 21:24:16.000000 FuncsForSPO-5.2.3/FuncsForSPO/fwinotify/__init__.py
+-rw-rw-rw-   0        0        0     4896 2022-09-12 21:21:52.000000 FuncsForSPO-5.2.3/FuncsForSPO/fwinotify/fwinotify.py
+drwxrwxrwx   0        0        0        0 2023-06-09 19:43:26.074220 FuncsForSPO-5.2.3/FuncsForSPO/utils/
+-rw-rw-rw-   0        0        0   114869 2023-03-31 19:29:18.000000 FuncsForSPO-5.2.3/FuncsForSPO/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-09 19:43:25.816781 FuncsForSPO-5.2.3/FuncsForSPO.egg-info/
+-rw-rw-rw-   0        0        0     8026 2023-06-09 19:43:25.000000 FuncsForSPO-5.2.3/FuncsForSPO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1815 2023-06-09 19:43:25.000000 FuncsForSPO-5.2.3/FuncsForSPO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 19:43:25.000000 FuncsForSPO-5.2.3/FuncsForSPO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      194 2023-06-09 19:43:25.000000 FuncsForSPO-5.2.3/FuncsForSPO.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      458 2023-06-09 19:43:25.000000 FuncsForSPO-5.2.3/FuncsForSPO.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1074 2022-12-02 16:50:42.000000 FuncsForSPO-5.2.3/LICENSE
+-rw-rw-rw-   0        0        0     8026 2023-06-09 19:43:26.176322 FuncsForSPO-5.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     7607 2023-01-21 19:11:53.000000 FuncsForSPO-5.2.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-09 19:43:26.181348 FuncsForSPO-5.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     2506 2023-06-09 19:43:19.000000 FuncsForSPO-5.2.3/setup.py
```

### Comparing `FuncsForSPO-5.2.2/FuncsForSPO/femails/femails.py` & `FuncsForSPO-5.2.3/FuncsForSPO/femails/femails.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.2.2/FuncsForSPO/fexceptions/exceptions.py` & `FuncsForSPO-5.2.3/FuncsForSPO/fexceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.2.2/FuncsForSPO/fftp/fftp.py` & `FuncsForSPO-5.2.3/FuncsForSPO/fftp/fftp.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.2.2/FuncsForSPO/flanguage/translator/translator.py` & `FuncsForSPO-5.2.3/FuncsForSPO/flanguage/translator/translator.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.2.2/FuncsForSPO/fopenpyxl/openpyxl_funcs.py` & `FuncsForSPO-5.2.3/FuncsForSPO/fopenpyxl/openpyxl_funcs.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.2.2/FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py` & `FuncsForSPO-5.2.3/FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,17 +128,16 @@
                     text = espera_e_retorna_elemento_text(self.WDW, (By.CSS_SELECTOR, 'div[style="padding: 5px;"]>div:last-of-type>div:last-of-type span'))
                     faz_log(f'Resposta até agora: {text}')
                     sleep(1)
                 except:...
                 if 'AI RES' in text:
                     break
                 if 'try again.' in text.lower():
-                    self.apaga_arquivo_da_base_do_site()
-                    self.DRIVER.close()
-                    raise ErroPDFAIException('Ocorreu um erro interno no site, tente novamente.')
+                    text = text + '  Não foi possível ter uma interpretação adequada. Tente outro prompt'
+                    break
             faz_log('Recuperando o id do documento')
             self.apaga_arquivo_da_base_do_site()
             self.DRIVER.close()
             return text
         except Exception as e:
             faz_log(repr(e), 'c*')
             faz_log(self.DRIVER.get_screenshot_as_base64(), 'i*')
```

### Comparing `FuncsForSPO-5.2.2/FuncsForSPO/fpdf/fanalyser/base.py` & `FuncsForSPO-5.2.3/FuncsForSPO/fpdf/fanalyser/base.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.2.2/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v1.py` & `FuncsForSPO-5.2.3/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v1.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.2.2/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v2.py` & `FuncsForSPO-5.2.3/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v2.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.2.2/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v3.py` & `FuncsForSPO-5.2.3/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v3.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.2.2/FuncsForSPO/fpdf/fcompress/__compress_online.py` & `FuncsForSPO-5.2.3/FuncsForSPO/fpdf/fcompress/__compress_online.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.2.2/FuncsForSPO/fpdf/fcompress/compress.py` & `FuncsForSPO-5.2.3/FuncsForSPO/fpdf/fcompress/compress.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.2.2/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py` & `FuncsForSPO-5.2.3/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.2.2/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py` & `FuncsForSPO-5.2.3/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.2.2/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py` & `FuncsForSPO-5.2.3/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.2.2/FuncsForSPO/fpdf/focr/__ocr_online.py` & `FuncsForSPO-5.2.3/FuncsForSPO/fpdf/focr/__ocr_online.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.2.2/FuncsForSPO/fpdf/focr/orc.py` & `FuncsForSPO-5.2.3/FuncsForSPO/fpdf/focr/orc.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.2.2/FuncsForSPO/fpdf/pdfutils/pdfutils.py` & `FuncsForSPO-5.2.3/FuncsForSPO/fpdf/pdfutils/pdfutils.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.2.2/FuncsForSPO/fpysimplegui/functions_for_sg.py` & `FuncsForSPO-5.2.3/FuncsForSPO/fpysimplegui/functions_for_sg.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.2.2/FuncsForSPO/fpython/functions_for_py.py` & `FuncsForSPO-5.2.3/FuncsForSPO/fpython/functions_for_py.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.2.2/FuncsForSPO/fregex/functions_re.py` & `FuncsForSPO-5.2.3/FuncsForSPO/fregex/functions_re.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.2.2/FuncsForSPO/fselenium/functions_selenium.py` & `FuncsForSPO-5.2.3/FuncsForSPO/fselenium/functions_selenium.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.2.2/FuncsForSPO/fsqlite/sqlite_functions.py` & `FuncsForSPO-5.2.3/FuncsForSPO/fsqlite/sqlite_functions.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.2.2/FuncsForSPO/fwinotify/fwinotify.py` & `FuncsForSPO-5.2.3/FuncsForSPO/fwinotify/fwinotify.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.2.2/FuncsForSPO/utils/utils.py` & `FuncsForSPO-5.2.3/FuncsForSPO/utils/utils.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.2.2/FuncsForSPO.egg-info/PKG-INFO` & `FuncsForSPO-5.2.3/FuncsForSPO.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FuncsForSPO
-Version: 5.2.2
+Version: 5.2.3
 Summary: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Home-page: https://github.com/githubpaycon/FuncsForSPO
 Author: Gabriel Lopes de Souza
 Author-email: githubpaycon@gmail.com
 License: MIT License
 Keywords: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Description-Content-Type: text/markdown
```

### Comparing `FuncsForSPO-5.2.2/FuncsForSPO.egg-info/SOURCES.txt` & `FuncsForSPO-5.2.3/FuncsForSPO.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.2.2/LICENSE` & `FuncsForSPO-5.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.2.2/PKG-INFO` & `FuncsForSPO-5.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FuncsForSPO
-Version: 5.2.2
+Version: 5.2.3
 Summary: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Home-page: https://github.com/githubpaycon/FuncsForSPO
 Author: Gabriel Lopes de Souza
 Author-email: githubpaycon@gmail.com
 License: MIT License
 Keywords: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Description-Content-Type: text/markdown
```

### Comparing `FuncsForSPO-5.2.2/README.md` & `FuncsForSPO-5.2.3/README.md`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.2.2/setup.py` & `FuncsForSPO-5.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 from setuptools import setup
 
-version = '5.2.2'
+version = '5.2.3'
 
 with open("README.md", "r", encoding='utf-8') as fh:
     readme = fh.read()
     setup(
         name='FuncsForSPO',
         version=version,
         url='https://github.com/githubpaycon/FuncsForSPO',
```

