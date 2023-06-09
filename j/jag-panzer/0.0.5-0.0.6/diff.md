# Comparing `tmp/jag-panzer-0.0.5.tar.gz` & `tmp/jag-panzer-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jag-panzer-0.0.5.tar", last modified: Fri Jun  9 01:30:24 2023, max compression
+gzip compressed data, was "jag-panzer-0.0.6.tar", last modified: Fri Jun  9 01:42:15 2023, max compression
```

## Comparing `jag-panzer-0.0.5.tar` & `jag-panzer-0.0.6.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 01:30:24.215074 jag-panzer-0.0.5/
--rw-rw-rw-   0        0        0      161 2023-06-09 00:40:57.000000 jag-panzer-0.0.5/LICENSE
--rw-rw-rw-   0        0        0       66 2023-06-09 01:10:21.000000 jag-panzer-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0      560 2023-06-09 01:30:24.215074 jag-panzer-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       26 2023-06-09 00:32:58.000000 jag-panzer-0.0.5/README.md
--rw-rw-rw-   0        0        0      108 2023-06-09 00:12:29.000000 jag-panzer-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0      671 2023-06-09 01:30:24.221056 jag-panzer-0.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-09 01:30:24.024544 jag-panzer-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-06-09 01:30:24.047521 jag-panzer-0.0.5/src/jag_panzer/
--rw-rw-rw-   0        0        0        0 2023-06-09 00:13:59.000000 jag-panzer-0.0.5/src/jag_panzer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 01:30:24.069508 jag-panzer-0.0.5/src/jag_panzer/assets/
-drwxrwxrwx   0        0        0        0 2023-06-09 01:30:24.080014 jag-panzer-0.0.5/src/jag_panzer/assets/dir_listing/
--rw-rw-rw-   0        0        0      356 2023-06-08 21:39:34.000000 jag-panzer-0.0.5/src/jag_panzer/assets/dir_listing/base.html
--rw-rw-rw-   0        0        0      446 2023-06-06 00:39:53.000000 jag-panzer-0.0.5/src/jag_panzer/assets/dir_listing/dir_icon.svg
--rw-rw-rw-   0        0        0      682 2023-06-07 06:27:42.000000 jag-panzer-0.0.5/src/jag_panzer/assets/dir_listing/download_icon.svg
--rw-rw-rw-   0        0        0      704 2023-06-06 00:40:06.000000 jag-panzer-0.0.5/src/jag_panzer/assets/dir_listing/file_icon.svg
--rw-rw-rw-   0        0        0       21 2023-06-06 01:12:59.000000 jag-panzer-0.0.5/src/jag_panzer/assets/dir_listing/script.js
--rw-rw-rw-   0        0        0     1355 2023-06-07 07:34:01.000000 jag-panzer-0.0.5/src/jag_panzer/assets/dir_listing/style.css
--rw-rw-rw-   0        0        0      260 2023-06-07 02:18:15.000000 jag-panzer-0.0.5/src/jag_panzer/assets/reject.html
--rw-rw-rw-   0        0        0    16948 2023-06-08 23:41:16.000000 jag-panzer-0.0.5/src/jag_panzer/base_room.py
-drwxrwxrwx   0        0        0        0 2023-06-09 01:30:24.091539 jag-panzer-0.0.5/src/jag_panzer/cgi/
--rw-rw-rw-   0        0        0        0 2023-06-09 00:00:24.000000 jag-panzer-0.0.5/src/jag_panzer/cgi/__init__.py
--rw-rw-rw-   0        0        0     5087 2023-06-03 17:16:43.000000 jag-panzer-0.0.5/src/jag_panzer/cgi/burn_power.py
--rw-rw-rw-   0        0        0      451 2023-06-03 17:16:43.000000 jag-panzer-0.0.5/src/jag_panzer/cgi/hitman.py
--rw-rw-rw-   0        0        0     6691 2023-06-03 17:16:43.000000 jag-panzer-0.0.5/src/jag_panzer/cgi/jag.py
-drwxrwxrwx   0        0        0        0 2023-06-09 01:30:24.093537 jag-panzer-0.0.5/src/jag_panzer/cgi/templates/
-drwxrwxrwx   0        0        0        0 2023-06-09 01:30:24.094537 jag-panzer-0.0.5/src/jag_panzer/cgi/templates/light_httpd/
-drwxrwxrwx   0        0        0        0 2023-06-09 01:30:24.099534 jag-panzer-0.0.5/src/jag_panzer/cgi/templates/light_httpd/conf-enabled/
--rw-rw-rw-   0        0        0       91 2023-06-03 17:16:43.000000 jag-panzer-0.0.5/src/jag_panzer/cgi/templates/light_httpd/conf-enabled/10-accesslog.conf
--rw-rw-rw-   0        0        0      306 2023-06-03 17:16:43.000000 jag-panzer-0.0.5/src/jag_panzer/cgi/templates/light_httpd/conf-enabled/10-cgi.conf
--rw-rw-rw-   0        0        0      454 2023-06-03 17:16:43.000000 jag-panzer-0.0.5/src/jag_panzer/cgi/templates/light_httpd/conf-enabled/10-status.conf
--rw-rw-rw-   0        0        0     2245 2023-06-03 17:16:43.000000 jag-panzer-0.0.5/src/jag_panzer/cgi/templates/light_httpd/server_prms.conf
--rw-rw-rw-   0        0        0      403 2023-06-03 17:16:43.000000 jag-panzer-0.0.5/src/jag_panzer/cgi/templates/unit.service
--rw-rw-rw-   0        0        0     2539 2023-06-08 21:42:17.000000 jag-panzer-0.0.5/src/jag_panzer/dir_list.py
--rw-rw-rw-   0        0        0      369 2023-06-07 05:17:03.000000 jag-panzer-0.0.5/src/jag_panzer/jag_util.py
-drwxrwxrwx   0        0        0        0 2023-06-09 01:30:24.030531 jag-panzer-0.0.5/src/jag_panzer/libs/
-drwxrwxrwx   0        0        0        0 2023-06-09 01:30:24.115525 jag-panzer-0.0.5/src/jag_panzer/libs/bs4/
--rw-rw-rw-   0        0        0    33822 2023-06-06 00:22:44.000000 jag-panzer-0.0.5/src/jag_panzer/libs/bs4/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 01:30:24.125519 jag-panzer-0.0.5/src/jag_panzer/libs/bs4/builder/
--rw-rw-rw-   0        0        0    24393 2023-06-06 00:22:44.000000 jag-panzer-0.0.5/src/jag_panzer/libs/bs4/builder/__init__.py
--rw-rw-rw-   0        0        0    19078 2023-06-06 00:22:44.000000 jag-panzer-0.0.5/src/jag_panzer/libs/bs4/builder/_html5lib.py
--rw-rw-rw-   0        0        0    14919 2023-06-06 00:22:44.000000 jag-panzer-0.0.5/src/jag_panzer/libs/bs4/builder/_htmlparser.py
--rw-rw-rw-   0        0        0    14904 2023-06-06 00:22:44.000000 jag-panzer-0.0.5/src/jag_panzer/libs/bs4/builder/_lxml.py
--rw-rw-rw-   0        0        0    10077 2023-06-06 00:22:44.000000 jag-panzer-0.0.5/src/jag_panzer/libs/bs4/css.py
--rw-rw-rw-   0        0        0    41158 2023-06-06 00:22:44.000000 jag-panzer-0.0.5/src/jag_panzer/libs/bs4/dammit.py
--rw-rw-rw-   0        0        0     7195 2023-06-06 00:22:44.000000 jag-panzer-0.0.5/src/jag_panzer/libs/bs4/diagnose.py
--rw-rw-rw-   0        0        0    92716 2023-06-06 00:22:44.000000 jag-panzer-0.0.5/src/jag_panzer/libs/bs4/element.py
--rw-rw-rw-   0        0        0     7184 2023-06-06 00:22:44.000000 jag-panzer-0.0.5/src/jag_panzer/libs/bs4/formatter.py
-drwxrwxrwx   0        0        0        0 2023-06-09 01:30:24.158501 jag-panzer-0.0.5/src/jag_panzer/libs/bs4/tests/
--rw-rw-rw-   0        0        0    48391 2023-06-06 00:22:44.000000 jag-panzer-0.0.5/src/jag_panzer/libs/bs4/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 01:30:24.182088 jag-panzer-0.0.5/src/jag_panzer/libs/bs4/tests/fuzz/
--rw-rw-rw-   0        0        0       23 2023-06-06 00:22:44.000000 jag-panzer-0.0.5/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-4818336571064320.testcase
--rw-rw-rw-   0        0        0       30 2023-06-06 00:22:44.000000 jag-panzer-0.0.5/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-4999465949331456.testcase
--rw-rw-rw-   0        0        0    19469 2023-06-06 00:22:44.000000 jag-panzer-0.0.5/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-5167584867909632.testcase
--rw-rw-rw-   0        0        0        5 2023-06-06 00:22:44.000000 jag-panzer-0.0.5/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-5703933063462912.testcase
--rw-rw-rw-   0        0        0       35 2023-06-06 00:22:44.000000 jag-panzer-0.0.5/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-5843991618256896.testcase
--rw-rw-rw-   0        0        0    51495 2023-06-06 00:22:44.000000 jag-panzer-0.0.5/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-5984173902397440.testcase
--rw-rw-rw-   0        0        0    10380 2023-06-06 00:22:44.000000 jag-panzer-0.0.5/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-6124268085182464.testcase
--rw-rw-rw-   0        0        0       19 2023-06-06 00:22:44.000000 jag-panzer-0.0.5/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-6241471367348224.testcase
--rw-rw-rw-   0        0        0     3546 2023-06-06 00:22:44.000000 jag-panzer-0.0.5/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-6450958476902400.testcase
--rw-rw-rw-   0        0        0      124 2023-06-06 00:22:44.000000 jag-panzer-0.0.5/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-6600557255327744.testcase
--rw-rw-rw-   0        0        0     2607 2023-06-06 00:22:44.000000 jag-panzer-0.0.5/src/jag_panzer/libs/bs4/tests/fuzz/crash-0d306a50c8ed8bcd0785b67000fcd5dea1d33f08.testcase
--rw-rw-rw-   0        0        0     1115 2023-06-06 00:22:44.000000 jag-panzer-0.0.5/src/jag_panzer/libs/bs4/tests/test_builder.py
--rw-rw-rw-   0        0        0     5114 2023-06-06 00:22:44.000000 jag-panzer-0.0.5/src/jag_panzer/libs/bs4/tests/test_builder_registry.py
--rw-rw-rw-   0        0        0    17279 2023-06-06 00:22:44.000000 jag-panzer-0.0.5/src/jag_panzer/libs/bs4/tests/test_css.py
--rw-rw-rw-   0        0        0    15451 2023-06-06 00:22:44.000000 jag-panzer-0.0.5/src/jag_panzer/libs/bs4/tests/test_dammit.py
--rw-rw-rw-   0        0        0     1127 2023-06-06 00:22:44.000000 jag-panzer-0.0.5/src/jag_panzer/libs/bs4/tests/test_docs.py
--rw-rw-rw-   0        0        0     2377 2023-06-06 00:22:44.000000 jag-panzer-0.0.5/src/jag_panzer/libs/bs4/tests/test_element.py
--rw-rw-rw-   0        0        0     4148 2023-06-06 00:22:44.000000 jag-panzer-0.0.5/src/jag_panzer/libs/bs4/tests/test_formatter.py
--rw-rw-rw-   0        0        0     3637 2023-06-06 00:22:44.000000 jag-panzer-0.0.5/src/jag_panzer/libs/bs4/tests/test_fuzz.py
--rw-rw-rw-   0        0        0     8322 2023-06-06 00:22:44.000000 jag-panzer-0.0.5/src/jag_panzer/libs/bs4/tests/test_html5lib.py
--rw-rw-rw-   0        0        0     6256 2023-06-06 00:22:44.000000 jag-panzer-0.0.5/src/jag_panzer/libs/bs4/tests/test_htmlparser.py
--rw-rw-rw-   0        0        0     7635 2023-06-06 00:22:44.000000 jag-panzer-0.0.5/src/jag_panzer/libs/bs4/tests/test_lxml.py
--rw-rw-rw-   0        0        0     5081 2023-06-06 00:22:44.000000 jag-panzer-0.0.5/src/jag_panzer/libs/bs4/tests/test_navigablestring.py
--rw-rw-rw-   0        0        0    14274 2023-06-06 00:22:44.000000 jag-panzer-0.0.5/src/jag_panzer/libs/bs4/tests/test_pageelement.py
--rw-rw-rw-   0        0        0    19877 2023-06-06 00:22:44.000000 jag-panzer-0.0.5/src/jag_panzer/libs/bs4/tests/test_soup.py
--rw-rw-rw-   0        0        0     9016 2023-06-06 00:22:44.000000 jag-panzer-0.0.5/src/jag_panzer/libs/bs4/tests/test_tag.py
--rw-rw-rw-   0        0        0    48129 2023-06-06 00:22:44.000000 jag-panzer-0.0.5/src/jag_panzer/libs/bs4/tests/test_tree.py
-drwxrwxrwx   0        0        0        0 2023-06-09 01:30:24.200067 jag-panzer-0.0.5/src/jag_panzer/libs/soupsieve/
--rw-rw-rw-   0        0        0     4630 2023-06-06 00:22:44.000000 jag-panzer-0.0.5/src/jag_panzer/libs/soupsieve/__init__.py
--rw-rw-rw-   0        0        0     6842 2023-06-06 00:22:44.000000 jag-panzer-0.0.5/src/jag_panzer/libs/soupsieve/__meta__.py
--rw-rw-rw-   0        0        0    58152 2023-06-06 00:22:44.000000 jag-panzer-0.0.5/src/jag_panzer/libs/soupsieve/css_match.py
--rw-rw-rw-   0        0        0    47063 2023-06-06 00:22:44.000000 jag-panzer-0.0.5/src/jag_panzer/libs/soupsieve/css_parser.py
--rw-rw-rw-   0        0        0    10337 2023-06-06 00:22:44.000000 jag-panzer-0.0.5/src/jag_panzer/libs/soupsieve/css_types.py
--rw-rw-rw-   0        0        0     4053 2023-06-06 00:22:44.000000 jag-panzer-0.0.5/src/jag_panzer/libs/soupsieve/pretty.py
--rw-rw-rw-   0        0        0        0 2023-06-06 00:22:44.000000 jag-panzer-0.0.5/src/jag_panzer/libs/soupsieve/py.typed
--rw-rw-rw-   0        0        0     3374 2023-06-06 00:22:44.000000 jag-panzer-0.0.5/src/jag_panzer/libs/soupsieve/util.py
-drwxrwxrwx   0        0        0        0 2023-06-09 01:30:24.212063 jag-panzer-0.0.5/src/jag_panzer/libs/yattag/
--rw-rw-rw-   0        0        0     1743 2023-03-03 09:07:48.000000 jag-panzer-0.0.5/src/jag_panzer/libs/yattag/__init__.py
--rw-rw-rw-   0        0        0    18197 2020-08-06 21:26:32.000000 jag-panzer-0.0.5/src/jag_panzer/libs/yattag/doc.py
--rw-rw-rw-   0        0        0    12029 2023-01-02 11:12:52.000000 jag-panzer-0.0.5/src/jag_panzer/libs/yattag/indentation.py
--rw-rw-rw-   0        0        0        0 2019-12-25 20:07:02.000000 jag-panzer-0.0.5/src/jag_panzer/libs/yattag/py.typed
--rw-rw-rw-   0        0        0    18081 2019-12-24 00:01:02.000000 jag-panzer-0.0.5/src/jag_panzer/libs/yattag/simpledoc.py
-drwxrwxrwx   0        0        0        0 2023-06-09 01:30:24.213062 jag-panzer-0.0.5/src/jag_panzer/mimes/
--rw-rw-rw-   0        0        0     2762 2023-06-03 17:16:43.000000 jag-panzer-0.0.5/src/jag_panzer/mimes/mime_types_base.py
--rw-rw-rw-   0        0        0     1938 2023-06-03 17:16:43.000000 jag-panzer-0.0.5/src/jag_panzer/response_codes.py
--rw-rw-rw-   0        0        0     7363 2023-06-08 23:38:46.000000 jag-panzer-0.0.5/src/jag_panzer/server.py
--rwxrwxrwx   0        0        0       12 2023-06-07 01:47:22.000000 jag-panzer-0.0.5/src/jag_panzer/test.cmd
-drwxrwxrwx   0        0        0        0 2023-06-09 01:30:24.068520 jag-panzer-0.0.5/src/jag_panzer.egg-info/
--rw-rw-rw-   0        0        0      560 2023-06-09 01:30:23.000000 jag-panzer-0.0.5/src/jag_panzer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3986 2023-06-09 01:30:24.000000 jag-panzer-0.0.5/src/jag_panzer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 01:30:23.000000 jag-panzer-0.0.5/src/jag_panzer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-09 01:30:23.000000 jag-panzer-0.0.5/src/jag_panzer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 01:42:15.680115 jag-panzer-0.0.6/
+-rw-rw-rw-   0        0        0      161 2023-06-09 00:40:57.000000 jag-panzer-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0       66 2023-06-09 01:10:21.000000 jag-panzer-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      560 2023-06-09 01:42:15.680115 jag-panzer-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       26 2023-06-09 00:32:58.000000 jag-panzer-0.0.6/README.md
+-rw-rw-rw-   0        0        0      108 2023-06-09 00:12:29.000000 jag-panzer-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0      671 2023-06-09 01:42:15.685113 jag-panzer-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-09 01:42:15.513134 jag-panzer-0.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-06-09 01:42:15.542117 jag-panzer-0.0.6/src/jag_panzer/
+-rw-rw-rw-   0        0        0        0 2023-06-09 00:13:59.000000 jag-panzer-0.0.6/src/jag_panzer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 01:42:15.564716 jag-panzer-0.0.6/src/jag_panzer/assets/
+drwxrwxrwx   0        0        0        0 2023-06-09 01:42:15.575696 jag-panzer-0.0.6/src/jag_panzer/assets/dir_listing/
+-rw-rw-rw-   0        0        0      356 2023-06-08 21:39:34.000000 jag-panzer-0.0.6/src/jag_panzer/assets/dir_listing/base.html
+-rw-rw-rw-   0        0        0      446 2023-06-06 00:39:53.000000 jag-panzer-0.0.6/src/jag_panzer/assets/dir_listing/dir_icon.svg
+-rw-rw-rw-   0        0        0      682 2023-06-07 06:27:42.000000 jag-panzer-0.0.6/src/jag_panzer/assets/dir_listing/download_icon.svg
+-rw-rw-rw-   0        0        0      704 2023-06-06 00:40:06.000000 jag-panzer-0.0.6/src/jag_panzer/assets/dir_listing/file_icon.svg
+-rw-rw-rw-   0        0        0       21 2023-06-06 01:12:59.000000 jag-panzer-0.0.6/src/jag_panzer/assets/dir_listing/script.js
+-rw-rw-rw-   0        0        0     1355 2023-06-07 07:34:01.000000 jag-panzer-0.0.6/src/jag_panzer/assets/dir_listing/style.css
+-rw-rw-rw-   0        0        0      260 2023-06-07 02:18:15.000000 jag-panzer-0.0.6/src/jag_panzer/assets/reject.html
+-rw-rw-rw-   0        0        0    16948 2023-06-08 23:41:16.000000 jag-panzer-0.0.6/src/jag_panzer/base_room.py
+drwxrwxrwx   0        0        0        0 2023-06-09 01:42:15.581692 jag-panzer-0.0.6/src/jag_panzer/cgi/
+-rw-rw-rw-   0        0        0        0 2023-06-09 00:00:24.000000 jag-panzer-0.0.6/src/jag_panzer/cgi/__init__.py
+-rw-rw-rw-   0        0        0     5087 2023-06-03 17:16:43.000000 jag-panzer-0.0.6/src/jag_panzer/cgi/burn_power.py
+-rw-rw-rw-   0        0        0      451 2023-06-03 17:16:43.000000 jag-panzer-0.0.6/src/jag_panzer/cgi/hitman.py
+-rw-rw-rw-   0        0        0     6691 2023-06-03 17:16:43.000000 jag-panzer-0.0.6/src/jag_panzer/cgi/jag.py
+drwxrwxrwx   0        0        0        0 2023-06-09 01:42:15.582692 jag-panzer-0.0.6/src/jag_panzer/cgi/templates/
+drwxrwxrwx   0        0        0        0 2023-06-09 01:42:15.583692 jag-panzer-0.0.6/src/jag_panzer/cgi/templates/light_httpd/
+drwxrwxrwx   0        0        0        0 2023-06-09 01:42:15.590687 jag-panzer-0.0.6/src/jag_panzer/cgi/templates/light_httpd/conf-enabled/
+-rw-rw-rw-   0        0        0       91 2023-06-03 17:16:43.000000 jag-panzer-0.0.6/src/jag_panzer/cgi/templates/light_httpd/conf-enabled/10-accesslog.conf
+-rw-rw-rw-   0        0        0      306 2023-06-03 17:16:43.000000 jag-panzer-0.0.6/src/jag_panzer/cgi/templates/light_httpd/conf-enabled/10-cgi.conf
+-rw-rw-rw-   0        0        0      454 2023-06-03 17:16:43.000000 jag-panzer-0.0.6/src/jag_panzer/cgi/templates/light_httpd/conf-enabled/10-status.conf
+-rw-rw-rw-   0        0        0     2245 2023-06-03 17:16:43.000000 jag-panzer-0.0.6/src/jag_panzer/cgi/templates/light_httpd/server_prms.conf
+-rw-rw-rw-   0        0        0      403 2023-06-03 17:16:43.000000 jag-panzer-0.0.6/src/jag_panzer/cgi/templates/unit.service
+-rw-rw-rw-   0        0        0     2539 2023-06-08 21:42:17.000000 jag-panzer-0.0.6/src/jag_panzer/dir_list.py
+-rw-rw-rw-   0        0        0      369 2023-06-07 05:17:03.000000 jag-panzer-0.0.6/src/jag_panzer/jag_util.py
+drwxrwxrwx   0        0        0        0 2023-06-09 01:42:15.520130 jag-panzer-0.0.6/src/jag_panzer/libs/
+drwxrwxrwx   0        0        0        0 2023-06-09 01:42:15.600168 jag-panzer-0.0.6/src/jag_panzer/libs/bs4/
+-rw-rw-rw-   0        0        0    33822 2023-06-06 00:22:44.000000 jag-panzer-0.0.6/src/jag_panzer/libs/bs4/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 01:42:15.606158 jag-panzer-0.0.6/src/jag_panzer/libs/bs4/builder/
+-rw-rw-rw-   0        0        0    24393 2023-06-06 00:22:44.000000 jag-panzer-0.0.6/src/jag_panzer/libs/bs4/builder/__init__.py
+-rw-rw-rw-   0        0        0    19078 2023-06-06 00:22:44.000000 jag-panzer-0.0.6/src/jag_panzer/libs/bs4/builder/_html5lib.py
+-rw-rw-rw-   0        0        0    14919 2023-06-06 00:22:44.000000 jag-panzer-0.0.6/src/jag_panzer/libs/bs4/builder/_htmlparser.py
+-rw-rw-rw-   0        0        0    14904 2023-06-06 00:22:44.000000 jag-panzer-0.0.6/src/jag_panzer/libs/bs4/builder/_lxml.py
+-rw-rw-rw-   0        0        0    10077 2023-06-06 00:22:44.000000 jag-panzer-0.0.6/src/jag_panzer/libs/bs4/css.py
+-rw-rw-rw-   0        0        0    41158 2023-06-06 00:22:44.000000 jag-panzer-0.0.6/src/jag_panzer/libs/bs4/dammit.py
+-rw-rw-rw-   0        0        0     7195 2023-06-06 00:22:44.000000 jag-panzer-0.0.6/src/jag_panzer/libs/bs4/diagnose.py
+-rw-rw-rw-   0        0        0    92716 2023-06-06 00:22:44.000000 jag-panzer-0.0.6/src/jag_panzer/libs/bs4/element.py
+-rw-rw-rw-   0        0        0     7184 2023-06-06 00:22:44.000000 jag-panzer-0.0.6/src/jag_panzer/libs/bs4/formatter.py
+drwxrwxrwx   0        0        0        0 2023-06-09 01:42:15.634143 jag-panzer-0.0.6/src/jag_panzer/libs/bs4/tests/
+-rw-rw-rw-   0        0        0    48391 2023-06-06 00:22:44.000000 jag-panzer-0.0.6/src/jag_panzer/libs/bs4/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 01:42:15.654130 jag-panzer-0.0.6/src/jag_panzer/libs/bs4/tests/fuzz/
+-rw-rw-rw-   0        0        0       23 2023-06-06 00:22:44.000000 jag-panzer-0.0.6/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-4818336571064320.testcase
+-rw-rw-rw-   0        0        0       30 2023-06-06 00:22:44.000000 jag-panzer-0.0.6/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-4999465949331456.testcase
+-rw-rw-rw-   0        0        0    19469 2023-06-06 00:22:44.000000 jag-panzer-0.0.6/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-5167584867909632.testcase
+-rw-rw-rw-   0        0        0        5 2023-06-06 00:22:44.000000 jag-panzer-0.0.6/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-5703933063462912.testcase
+-rw-rw-rw-   0        0        0       35 2023-06-06 00:22:44.000000 jag-panzer-0.0.6/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-5843991618256896.testcase
+-rw-rw-rw-   0        0        0    51495 2023-06-06 00:22:44.000000 jag-panzer-0.0.6/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-5984173902397440.testcase
+-rw-rw-rw-   0        0        0    10380 2023-06-06 00:22:44.000000 jag-panzer-0.0.6/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-6124268085182464.testcase
+-rw-rw-rw-   0        0        0       19 2023-06-06 00:22:44.000000 jag-panzer-0.0.6/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-6241471367348224.testcase
+-rw-rw-rw-   0        0        0     3546 2023-06-06 00:22:44.000000 jag-panzer-0.0.6/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-6450958476902400.testcase
+-rw-rw-rw-   0        0        0      124 2023-06-06 00:22:44.000000 jag-panzer-0.0.6/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-6600557255327744.testcase
+-rw-rw-rw-   0        0        0     2607 2023-06-06 00:22:44.000000 jag-panzer-0.0.6/src/jag_panzer/libs/bs4/tests/fuzz/crash-0d306a50c8ed8bcd0785b67000fcd5dea1d33f08.testcase
+-rw-rw-rw-   0        0        0     1115 2023-06-06 00:22:44.000000 jag-panzer-0.0.6/src/jag_panzer/libs/bs4/tests/test_builder.py
+-rw-rw-rw-   0        0        0     5114 2023-06-06 00:22:44.000000 jag-panzer-0.0.6/src/jag_panzer/libs/bs4/tests/test_builder_registry.py
+-rw-rw-rw-   0        0        0    17279 2023-06-06 00:22:44.000000 jag-panzer-0.0.6/src/jag_panzer/libs/bs4/tests/test_css.py
+-rw-rw-rw-   0        0        0    15451 2023-06-06 00:22:44.000000 jag-panzer-0.0.6/src/jag_panzer/libs/bs4/tests/test_dammit.py
+-rw-rw-rw-   0        0        0     1127 2023-06-06 00:22:44.000000 jag-panzer-0.0.6/src/jag_panzer/libs/bs4/tests/test_docs.py
+-rw-rw-rw-   0        0        0     2377 2023-06-06 00:22:44.000000 jag-panzer-0.0.6/src/jag_panzer/libs/bs4/tests/test_element.py
+-rw-rw-rw-   0        0        0     4148 2023-06-06 00:22:44.000000 jag-panzer-0.0.6/src/jag_panzer/libs/bs4/tests/test_formatter.py
+-rw-rw-rw-   0        0        0     3637 2023-06-06 00:22:44.000000 jag-panzer-0.0.6/src/jag_panzer/libs/bs4/tests/test_fuzz.py
+-rw-rw-rw-   0        0        0     8322 2023-06-06 00:22:44.000000 jag-panzer-0.0.6/src/jag_panzer/libs/bs4/tests/test_html5lib.py
+-rw-rw-rw-   0        0        0     6256 2023-06-06 00:22:44.000000 jag-panzer-0.0.6/src/jag_panzer/libs/bs4/tests/test_htmlparser.py
+-rw-rw-rw-   0        0        0     7635 2023-06-06 00:22:44.000000 jag-panzer-0.0.6/src/jag_panzer/libs/bs4/tests/test_lxml.py
+-rw-rw-rw-   0        0        0     5081 2023-06-06 00:22:44.000000 jag-panzer-0.0.6/src/jag_panzer/libs/bs4/tests/test_navigablestring.py
+-rw-rw-rw-   0        0        0    14274 2023-06-06 00:22:44.000000 jag-panzer-0.0.6/src/jag_panzer/libs/bs4/tests/test_pageelement.py
+-rw-rw-rw-   0        0        0    19877 2023-06-06 00:22:44.000000 jag-panzer-0.0.6/src/jag_panzer/libs/bs4/tests/test_soup.py
+-rw-rw-rw-   0        0        0     9016 2023-06-06 00:22:44.000000 jag-panzer-0.0.6/src/jag_panzer/libs/bs4/tests/test_tag.py
+-rw-rw-rw-   0        0        0    48129 2023-06-06 00:22:44.000000 jag-panzer-0.0.6/src/jag_panzer/libs/bs4/tests/test_tree.py
+drwxrwxrwx   0        0        0        0 2023-06-09 01:42:15.668136 jag-panzer-0.0.6/src/jag_panzer/libs/soupsieve/
+-rw-rw-rw-   0        0        0     4630 2023-06-06 00:22:44.000000 jag-panzer-0.0.6/src/jag_panzer/libs/soupsieve/__init__.py
+-rw-rw-rw-   0        0        0     6842 2023-06-06 00:22:44.000000 jag-panzer-0.0.6/src/jag_panzer/libs/soupsieve/__meta__.py
+-rw-rw-rw-   0        0        0    58152 2023-06-06 00:22:44.000000 jag-panzer-0.0.6/src/jag_panzer/libs/soupsieve/css_match.py
+-rw-rw-rw-   0        0        0    47063 2023-06-06 00:22:44.000000 jag-panzer-0.0.6/src/jag_panzer/libs/soupsieve/css_parser.py
+-rw-rw-rw-   0        0        0    10337 2023-06-06 00:22:44.000000 jag-panzer-0.0.6/src/jag_panzer/libs/soupsieve/css_types.py
+-rw-rw-rw-   0        0        0     4053 2023-06-06 00:22:44.000000 jag-panzer-0.0.6/src/jag_panzer/libs/soupsieve/pretty.py
+-rw-rw-rw-   0        0        0        0 2023-06-06 00:22:44.000000 jag-panzer-0.0.6/src/jag_panzer/libs/soupsieve/py.typed
+-rw-rw-rw-   0        0        0     3374 2023-06-06 00:22:44.000000 jag-panzer-0.0.6/src/jag_panzer/libs/soupsieve/util.py
+drwxrwxrwx   0        0        0        0 2023-06-09 01:42:15.676119 jag-panzer-0.0.6/src/jag_panzer/libs/yattag/
+-rw-rw-rw-   0        0        0     1743 2023-03-03 09:07:48.000000 jag-panzer-0.0.6/src/jag_panzer/libs/yattag/__init__.py
+-rw-rw-rw-   0        0        0    18197 2020-08-06 21:26:32.000000 jag-panzer-0.0.6/src/jag_panzer/libs/yattag/doc.py
+-rw-rw-rw-   0        0        0    12029 2023-01-02 11:12:52.000000 jag-panzer-0.0.6/src/jag_panzer/libs/yattag/indentation.py
+-rw-rw-rw-   0        0        0        0 2019-12-25 20:07:02.000000 jag-panzer-0.0.6/src/jag_panzer/libs/yattag/py.typed
+-rw-rw-rw-   0        0        0    18081 2019-12-24 00:01:02.000000 jag-panzer-0.0.6/src/jag_panzer/libs/yattag/simpledoc.py
+drwxrwxrwx   0        0        0        0 2023-06-09 01:42:15.678117 jag-panzer-0.0.6/src/jag_panzer/mimes/
+-rw-rw-rw-   0        0        0     2762 2023-06-03 17:16:43.000000 jag-panzer-0.0.6/src/jag_panzer/mimes/mime_types_base.py
+-rw-rw-rw-   0        0        0     1938 2023-06-03 17:16:43.000000 jag-panzer-0.0.6/src/jag_panzer/response_codes.py
+-rw-rw-rw-   0        0        0     7363 2023-06-08 23:38:46.000000 jag-panzer-0.0.6/src/jag_panzer/server.py
+-rwxrwxrwx   0        0        0       12 2023-06-07 01:47:22.000000 jag-panzer-0.0.6/src/jag_panzer/test.cmd
+drwxrwxrwx   0        0        0        0 2023-06-09 01:42:15.562701 jag-panzer-0.0.6/src/jag_panzer.egg-info/
+-rw-rw-rw-   0        0        0      560 2023-06-09 01:42:15.000000 jag-panzer-0.0.6/src/jag_panzer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3986 2023-06-09 01:42:15.000000 jag-panzer-0.0.6/src/jag_panzer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 01:42:15.000000 jag-panzer-0.0.6/src/jag_panzer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-09 01:42:15.000000 jag-panzer-0.0.6/src/jag_panzer.egg-info/top_level.txt
```

### Comparing `jag-panzer-0.0.5/PKG-INFO` & `jag-panzer-0.0.6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jag-panzer
-Version: 0.0.5
+Version: 0.0.6
 Summary: Simple HTTP server allowing pure python workflow
 Home-page: https://github.com/MrKleiner/jag
 Author: Mr.Kleiner
 Author-email: megaadrenaline1055@gmail.com
 Project-URL: Bug Tracker, https://github.com/MrKleiner/jag/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `jag-panzer-0.0.5/setup.cfg` & `jag-panzer-0.0.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206a 6167 2d70 616e 7a65 720d 0a76   = jag-panzer..v
-00000020: 6572 7369 6f6e 203d 2030 2e30 2e35 0d0a  ersion = 0.0.5..
+00000020: 6572 7369 6f6e 203d 2030 2e30 2e36 0d0a  ersion = 0.0.6..
 00000030: 6175 7468 6f72 203d 204d 722e 4b6c 6569  author = Mr.Klei
 00000040: 6e65 720d 0a61 7574 686f 725f 656d 6169  ner..author_emai
 00000050: 6c20 3d20 6d65 6761 6164 7265 6e61 6c69  l = megaadrenali
 00000060: 6e65 3130 3535 4067 6d61 696c 2e63 6f6d  ne1055@gmail.com
 00000070: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
 00000080: 5369 6d70 6c65 2048 5454 5020 7365 7276  Simple HTTP serv
 00000090: 6572 2061 6c6c 6f77 696e 6720 7075 7265  er allowing pure
```

### Comparing `jag-panzer-0.0.5/src/jag_panzer/assets/dir_listing/download_icon.svg` & `jag-panzer-0.0.6/src/jag_panzer/assets/dir_listing/download_icon.svg`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.5/src/jag_panzer/assets/dir_listing/file_icon.svg` & `jag-panzer-0.0.6/src/jag_panzer/assets/dir_listing/file_icon.svg`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.5/src/jag_panzer/assets/dir_listing/style.css` & `jag-panzer-0.0.6/src/jag_panzer/assets/dir_listing/style.css`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.5/src/jag_panzer/base_room.py` & `jag-panzer-0.0.6/src/jag_panzer/base_room.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.5/src/jag_panzer/cgi/burn_power.py` & `jag-panzer-0.0.6/src/jag_panzer/cgi/burn_power.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.5/src/jag_panzer/cgi/jag.py` & `jag-panzer-0.0.6/src/jag_panzer/cgi/jag.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.5/src/jag_panzer/cgi/templates/light_httpd/server_prms.conf` & `jag-panzer-0.0.6/src/jag_panzer/cgi/templates/light_httpd/server_prms.conf`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.5/src/jag_panzer/dir_list.py` & `jag-panzer-0.0.6/src/jag_panzer/dir_list.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.5/src/jag_panzer/libs/bs4/__init__.py` & `jag-panzer-0.0.6/src/jag_panzer/libs/bs4/__init__.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.5/src/jag_panzer/libs/bs4/builder/__init__.py` & `jag-panzer-0.0.6/src/jag_panzer/libs/bs4/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.5/src/jag_panzer/libs/bs4/builder/_html5lib.py` & `jag-panzer-0.0.6/src/jag_panzer/libs/bs4/builder/_html5lib.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.5/src/jag_panzer/libs/bs4/builder/_htmlparser.py` & `jag-panzer-0.0.6/src/jag_panzer/libs/bs4/builder/_htmlparser.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.5/src/jag_panzer/libs/bs4/builder/_lxml.py` & `jag-panzer-0.0.6/src/jag_panzer/libs/bs4/builder/_lxml.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.5/src/jag_panzer/libs/bs4/css.py` & `jag-panzer-0.0.6/src/jag_panzer/libs/bs4/css.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.5/src/jag_panzer/libs/bs4/dammit.py` & `jag-panzer-0.0.6/src/jag_panzer/libs/bs4/dammit.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.5/src/jag_panzer/libs/bs4/diagnose.py` & `jag-panzer-0.0.6/src/jag_panzer/libs/bs4/diagnose.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.5/src/jag_panzer/libs/bs4/element.py` & `jag-panzer-0.0.6/src/jag_panzer/libs/bs4/element.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.5/src/jag_panzer/libs/bs4/formatter.py` & `jag-panzer-0.0.6/src/jag_panzer/libs/bs4/formatter.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.5/src/jag_panzer/libs/bs4/tests/__init__.py` & `jag-panzer-0.0.6/src/jag_panzer/libs/bs4/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.5/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-5167584867909632.testcase` & `jag-panzer-0.0.6/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-5167584867909632.testcase`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.5/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-5984173902397440.testcase` & `jag-panzer-0.0.6/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-5984173902397440.testcase`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.5/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-6124268085182464.testcase` & `jag-panzer-0.0.6/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-6124268085182464.testcase`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.5/src/jag_panzer/libs/bs4/tests/fuzz/crash-0d306a50c8ed8bcd0785b67000fcd5dea1d33f08.testcase` & `jag-panzer-0.0.6/src/jag_panzer/libs/bs4/tests/fuzz/crash-0d306a50c8ed8bcd0785b67000fcd5dea1d33f08.testcase`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.5/src/jag_panzer/libs/bs4/tests/test_builder.py` & `jag-panzer-0.0.6/src/jag_panzer/libs/bs4/tests/test_builder.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.5/src/jag_panzer/libs/bs4/tests/test_builder_registry.py` & `jag-panzer-0.0.6/src/jag_panzer/libs/bs4/tests/test_builder_registry.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.5/src/jag_panzer/libs/bs4/tests/test_css.py` & `jag-panzer-0.0.6/src/jag_panzer/libs/bs4/tests/test_css.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.5/src/jag_panzer/libs/bs4/tests/test_dammit.py` & `jag-panzer-0.0.6/src/jag_panzer/libs/bs4/tests/test_dammit.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.5/src/jag_panzer/libs/bs4/tests/test_docs.py` & `jag-panzer-0.0.6/src/jag_panzer/libs/bs4/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.5/src/jag_panzer/libs/bs4/tests/test_element.py` & `jag-panzer-0.0.6/src/jag_panzer/libs/bs4/tests/test_element.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.5/src/jag_panzer/libs/bs4/tests/test_formatter.py` & `jag-panzer-0.0.6/src/jag_panzer/libs/bs4/tests/test_formatter.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.5/src/jag_panzer/libs/bs4/tests/test_fuzz.py` & `jag-panzer-0.0.6/src/jag_panzer/libs/bs4/tests/test_fuzz.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.5/src/jag_panzer/libs/bs4/tests/test_html5lib.py` & `jag-panzer-0.0.6/src/jag_panzer/libs/bs4/tests/test_html5lib.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.5/src/jag_panzer/libs/bs4/tests/test_htmlparser.py` & `jag-panzer-0.0.6/src/jag_panzer/libs/bs4/tests/test_htmlparser.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.5/src/jag_panzer/libs/bs4/tests/test_lxml.py` & `jag-panzer-0.0.6/src/jag_panzer/libs/bs4/tests/test_lxml.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.5/src/jag_panzer/libs/bs4/tests/test_navigablestring.py` & `jag-panzer-0.0.6/src/jag_panzer/libs/bs4/tests/test_navigablestring.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.5/src/jag_panzer/libs/bs4/tests/test_pageelement.py` & `jag-panzer-0.0.6/src/jag_panzer/libs/bs4/tests/test_pageelement.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.5/src/jag_panzer/libs/bs4/tests/test_soup.py` & `jag-panzer-0.0.6/src/jag_panzer/libs/bs4/tests/test_soup.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.5/src/jag_panzer/libs/bs4/tests/test_tag.py` & `jag-panzer-0.0.6/src/jag_panzer/libs/bs4/tests/test_tag.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.5/src/jag_panzer/libs/bs4/tests/test_tree.py` & `jag-panzer-0.0.6/src/jag_panzer/libs/bs4/tests/test_tree.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.5/src/jag_panzer/libs/soupsieve/__init__.py` & `jag-panzer-0.0.6/src/jag_panzer/libs/soupsieve/__init__.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.5/src/jag_panzer/libs/soupsieve/__meta__.py` & `jag-panzer-0.0.6/src/jag_panzer/libs/soupsieve/__meta__.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.5/src/jag_panzer/libs/soupsieve/css_match.py` & `jag-panzer-0.0.6/src/jag_panzer/libs/soupsieve/css_match.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.5/src/jag_panzer/libs/soupsieve/css_parser.py` & `jag-panzer-0.0.6/src/jag_panzer/libs/soupsieve/css_parser.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.5/src/jag_panzer/libs/soupsieve/css_types.py` & `jag-panzer-0.0.6/src/jag_panzer/libs/soupsieve/css_types.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.5/src/jag_panzer/libs/soupsieve/pretty.py` & `jag-panzer-0.0.6/src/jag_panzer/libs/soupsieve/pretty.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.5/src/jag_panzer/libs/soupsieve/util.py` & `jag-panzer-0.0.6/src/jag_panzer/libs/soupsieve/util.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.5/src/jag_panzer/libs/yattag/__init__.py` & `jag-panzer-0.0.6/src/jag_panzer/libs/yattag/__init__.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.5/src/jag_panzer/libs/yattag/doc.py` & `jag-panzer-0.0.6/src/jag_panzer/libs/yattag/doc.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.5/src/jag_panzer/libs/yattag/indentation.py` & `jag-panzer-0.0.6/src/jag_panzer/libs/yattag/indentation.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.5/src/jag_panzer/libs/yattag/simpledoc.py` & `jag-panzer-0.0.6/src/jag_panzer/libs/yattag/simpledoc.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.5/src/jag_panzer/mimes/mime_types_base.py` & `jag-panzer-0.0.6/src/jag_panzer/mimes/mime_types_base.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.5/src/jag_panzer/response_codes.py` & `jag-panzer-0.0.6/src/jag_panzer/response_codes.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.5/src/jag_panzer/server.py` & `jag-panzer-0.0.6/src/jag_panzer/server.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.5/src/jag_panzer.egg-info/PKG-INFO` & `jag-panzer-0.0.6/src/jag_panzer.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jag-panzer
-Version: 0.0.5
+Version: 0.0.6
 Summary: Simple HTTP server allowing pure python workflow
 Home-page: https://github.com/MrKleiner/jag
 Author: Mr.Kleiner
 Author-email: megaadrenaline1055@gmail.com
 Project-URL: Bug Tracker, https://github.com/MrKleiner/jag/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `jag-panzer-0.0.5/src/jag_panzer.egg-info/SOURCES.txt` & `jag-panzer-0.0.6/src/jag_panzer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

