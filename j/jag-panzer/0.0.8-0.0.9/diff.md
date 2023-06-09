# Comparing `tmp/jag-panzer-0.0.8.tar.gz` & `tmp/jag-panzer-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jag-panzer-0.0.8.tar", last modified: Fri Jun  9 02:50:39 2023, max compression
+gzip compressed data, was "jag-panzer-0.0.9.tar", last modified: Fri Jun  9 12:21:33 2023, max compression
```

## Comparing `jag-panzer-0.0.8.tar` & `jag-panzer-0.0.9.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 02:50:39.059449 jag-panzer-0.0.8/
--rw-rw-rw-   0        0        0      161 2023-06-09 00:40:57.000000 jag-panzer-0.0.8/LICENSE
--rw-rw-rw-   0        0        0       46 2023-06-09 02:05:06.000000 jag-panzer-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0      560 2023-06-09 02:50:39.059449 jag-panzer-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       26 2023-06-09 00:32:58.000000 jag-panzer-0.0.8/README.md
--rw-rw-rw-   0        0        0      108 2023-06-09 00:12:29.000000 jag-panzer-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0      671 2023-06-09 02:50:39.064446 jag-panzer-0.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-09 02:50:38.901186 jag-panzer-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-06-09 02:50:38.929162 jag-panzer-0.0.8/src/jag_panzer/
--rw-rw-rw-   0        0        0        0 2023-06-09 00:13:59.000000 jag-panzer-0.0.8/src/jag_panzer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 02:50:38.951160 jag-panzer-0.0.8/src/jag_panzer/assets/
-drwxrwxrwx   0        0        0        0 2023-06-09 02:50:38.960144 jag-panzer-0.0.8/src/jag_panzer/assets/dir_listing/
--rw-rw-rw-   0        0        0      356 2023-06-08 21:39:34.000000 jag-panzer-0.0.8/src/jag_panzer/assets/dir_listing/base.html
--rw-rw-rw-   0        0        0      446 2023-06-06 00:39:53.000000 jag-panzer-0.0.8/src/jag_panzer/assets/dir_listing/dir_icon.svg
--rw-rw-rw-   0        0        0      682 2023-06-07 06:27:42.000000 jag-panzer-0.0.8/src/jag_panzer/assets/dir_listing/download_icon.svg
--rw-rw-rw-   0        0        0      704 2023-06-06 00:40:06.000000 jag-panzer-0.0.8/src/jag_panzer/assets/dir_listing/file_icon.svg
--rw-rw-rw-   0        0        0       21 2023-06-06 01:12:59.000000 jag-panzer-0.0.8/src/jag_panzer/assets/dir_listing/script.js
--rw-rw-rw-   0        0        0     1355 2023-06-07 07:34:01.000000 jag-panzer-0.0.8/src/jag_panzer/assets/dir_listing/style.css
--rw-rw-rw-   0        0        0      260 2023-06-07 02:18:15.000000 jag-panzer-0.0.8/src/jag_panzer/assets/reject.html
--rw-rw-rw-   0        0        0    16948 2023-06-08 23:41:16.000000 jag-panzer-0.0.8/src/jag_panzer/base_room.py
-drwxrwxrwx   0        0        0        0 2023-06-09 02:50:38.966500 jag-panzer-0.0.8/src/jag_panzer/cgi/
--rw-rw-rw-   0        0        0        0 2023-06-09 00:00:24.000000 jag-panzer-0.0.8/src/jag_panzer/cgi/__init__.py
--rw-rw-rw-   0        0        0     5087 2023-06-03 17:16:43.000000 jag-panzer-0.0.8/src/jag_panzer/cgi/burn_power.py
--rw-rw-rw-   0        0        0      451 2023-06-03 17:16:43.000000 jag-panzer-0.0.8/src/jag_panzer/cgi/hitman.py
--rw-rw-rw-   0        0        0     6691 2023-06-03 17:16:43.000000 jag-panzer-0.0.8/src/jag_panzer/cgi/jag.py
-drwxrwxrwx   0        0        0        0 2023-06-09 02:50:38.967512 jag-panzer-0.0.8/src/jag_panzer/cgi/templates/
-drwxrwxrwx   0        0        0        0 2023-06-09 02:50:38.969510 jag-panzer-0.0.8/src/jag_panzer/cgi/templates/light_httpd/
-drwxrwxrwx   0        0        0        0 2023-06-09 02:50:38.973508 jag-panzer-0.0.8/src/jag_panzer/cgi/templates/light_httpd/conf-enabled/
--rw-rw-rw-   0        0        0       91 2023-06-03 17:16:43.000000 jag-panzer-0.0.8/src/jag_panzer/cgi/templates/light_httpd/conf-enabled/10-accesslog.conf
--rw-rw-rw-   0        0        0      306 2023-06-03 17:16:43.000000 jag-panzer-0.0.8/src/jag_panzer/cgi/templates/light_httpd/conf-enabled/10-cgi.conf
--rw-rw-rw-   0        0        0      454 2023-06-03 17:16:43.000000 jag-panzer-0.0.8/src/jag_panzer/cgi/templates/light_httpd/conf-enabled/10-status.conf
--rw-rw-rw-   0        0        0     2245 2023-06-03 17:16:43.000000 jag-panzer-0.0.8/src/jag_panzer/cgi/templates/light_httpd/server_prms.conf
--rw-rw-rw-   0        0        0      403 2023-06-03 17:16:43.000000 jag-panzer-0.0.8/src/jag_panzer/cgi/templates/unit.service
--rw-rw-rw-   0        0        0     2539 2023-06-08 21:42:17.000000 jag-panzer-0.0.8/src/jag_panzer/dir_list.py
--rw-rw-rw-   0        0        0      369 2023-06-07 05:17:03.000000 jag-panzer-0.0.8/src/jag_panzer/jag_util.py
-drwxrwxrwx   0        0        0        0 2023-06-09 02:50:38.907175 jag-panzer-0.0.8/src/jag_panzer/libs/
-drwxrwxrwx   0        0        0        0 2023-06-09 02:50:38.985506 jag-panzer-0.0.8/src/jag_panzer/libs/bs4/
--rw-rw-rw-   0        0        0    33822 2023-06-06 00:22:44.000000 jag-panzer-0.0.8/src/jag_panzer/libs/bs4/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 02:50:38.991488 jag-panzer-0.0.8/src/jag_panzer/libs/bs4/builder/
--rw-rw-rw-   0        0        0    24393 2023-06-06 00:22:44.000000 jag-panzer-0.0.8/src/jag_panzer/libs/bs4/builder/__init__.py
--rw-rw-rw-   0        0        0    19078 2023-06-06 00:22:44.000000 jag-panzer-0.0.8/src/jag_panzer/libs/bs4/builder/_html5lib.py
--rw-rw-rw-   0        0        0    14919 2023-06-06 00:22:44.000000 jag-panzer-0.0.8/src/jag_panzer/libs/bs4/builder/_htmlparser.py
--rw-rw-rw-   0        0        0    14904 2023-06-06 00:22:44.000000 jag-panzer-0.0.8/src/jag_panzer/libs/bs4/builder/_lxml.py
--rw-rw-rw-   0        0        0    10077 2023-06-06 00:22:44.000000 jag-panzer-0.0.8/src/jag_panzer/libs/bs4/css.py
--rw-rw-rw-   0        0        0    41158 2023-06-06 00:22:44.000000 jag-panzer-0.0.8/src/jag_panzer/libs/bs4/dammit.py
--rw-rw-rw-   0        0        0     7195 2023-06-06 00:22:44.000000 jag-panzer-0.0.8/src/jag_panzer/libs/bs4/diagnose.py
--rw-rw-rw-   0        0        0    92716 2023-06-06 00:22:44.000000 jag-panzer-0.0.8/src/jag_panzer/libs/bs4/element.py
--rw-rw-rw-   0        0        0     7184 2023-06-06 00:22:44.000000 jag-panzer-0.0.8/src/jag_panzer/libs/bs4/formatter.py
-drwxrwxrwx   0        0        0        0 2023-06-09 02:50:39.017474 jag-panzer-0.0.8/src/jag_panzer/libs/bs4/tests/
--rw-rw-rw-   0        0        0    48391 2023-06-06 00:22:44.000000 jag-panzer-0.0.8/src/jag_panzer/libs/bs4/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 02:50:39.035463 jag-panzer-0.0.8/src/jag_panzer/libs/bs4/tests/fuzz/
--rw-rw-rw-   0        0        0       23 2023-06-06 00:22:44.000000 jag-panzer-0.0.8/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-4818336571064320.testcase
--rw-rw-rw-   0        0        0       30 2023-06-06 00:22:44.000000 jag-panzer-0.0.8/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-4999465949331456.testcase
--rw-rw-rw-   0        0        0    19469 2023-06-06 00:22:44.000000 jag-panzer-0.0.8/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-5167584867909632.testcase
--rw-rw-rw-   0        0        0        5 2023-06-06 00:22:44.000000 jag-panzer-0.0.8/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-5703933063462912.testcase
--rw-rw-rw-   0        0        0       35 2023-06-06 00:22:44.000000 jag-panzer-0.0.8/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-5843991618256896.testcase
--rw-rw-rw-   0        0        0    51495 2023-06-06 00:22:44.000000 jag-panzer-0.0.8/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-5984173902397440.testcase
--rw-rw-rw-   0        0        0    10380 2023-06-06 00:22:44.000000 jag-panzer-0.0.8/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-6124268085182464.testcase
--rw-rw-rw-   0        0        0       19 2023-06-06 00:22:44.000000 jag-panzer-0.0.8/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-6241471367348224.testcase
--rw-rw-rw-   0        0        0     3546 2023-06-06 00:22:44.000000 jag-panzer-0.0.8/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-6450958476902400.testcase
--rw-rw-rw-   0        0        0      124 2023-06-06 00:22:44.000000 jag-panzer-0.0.8/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-6600557255327744.testcase
--rw-rw-rw-   0        0        0     2607 2023-06-06 00:22:44.000000 jag-panzer-0.0.8/src/jag_panzer/libs/bs4/tests/fuzz/crash-0d306a50c8ed8bcd0785b67000fcd5dea1d33f08.testcase
--rw-rw-rw-   0        0        0     1115 2023-06-06 00:22:44.000000 jag-panzer-0.0.8/src/jag_panzer/libs/bs4/tests/test_builder.py
--rw-rw-rw-   0        0        0     5114 2023-06-06 00:22:44.000000 jag-panzer-0.0.8/src/jag_panzer/libs/bs4/tests/test_builder_registry.py
--rw-rw-rw-   0        0        0    17279 2023-06-06 00:22:44.000000 jag-panzer-0.0.8/src/jag_panzer/libs/bs4/tests/test_css.py
--rw-rw-rw-   0        0        0    15451 2023-06-06 00:22:44.000000 jag-panzer-0.0.8/src/jag_panzer/libs/bs4/tests/test_dammit.py
--rw-rw-rw-   0        0        0     1127 2023-06-06 00:22:44.000000 jag-panzer-0.0.8/src/jag_panzer/libs/bs4/tests/test_docs.py
--rw-rw-rw-   0        0        0     2377 2023-06-06 00:22:44.000000 jag-panzer-0.0.8/src/jag_panzer/libs/bs4/tests/test_element.py
--rw-rw-rw-   0        0        0     4148 2023-06-06 00:22:44.000000 jag-panzer-0.0.8/src/jag_panzer/libs/bs4/tests/test_formatter.py
--rw-rw-rw-   0        0        0     3637 2023-06-06 00:22:44.000000 jag-panzer-0.0.8/src/jag_panzer/libs/bs4/tests/test_fuzz.py
--rw-rw-rw-   0        0        0     8322 2023-06-06 00:22:44.000000 jag-panzer-0.0.8/src/jag_panzer/libs/bs4/tests/test_html5lib.py
--rw-rw-rw-   0        0        0     6256 2023-06-06 00:22:44.000000 jag-panzer-0.0.8/src/jag_panzer/libs/bs4/tests/test_htmlparser.py
--rw-rw-rw-   0        0        0     7635 2023-06-06 00:22:44.000000 jag-panzer-0.0.8/src/jag_panzer/libs/bs4/tests/test_lxml.py
--rw-rw-rw-   0        0        0     5081 2023-06-06 00:22:44.000000 jag-panzer-0.0.8/src/jag_panzer/libs/bs4/tests/test_navigablestring.py
--rw-rw-rw-   0        0        0    14274 2023-06-06 00:22:44.000000 jag-panzer-0.0.8/src/jag_panzer/libs/bs4/tests/test_pageelement.py
--rw-rw-rw-   0        0        0    19877 2023-06-06 00:22:44.000000 jag-panzer-0.0.8/src/jag_panzer/libs/bs4/tests/test_soup.py
--rw-rw-rw-   0        0        0     9016 2023-06-06 00:22:44.000000 jag-panzer-0.0.8/src/jag_panzer/libs/bs4/tests/test_tag.py
--rw-rw-rw-   0        0        0    48129 2023-06-06 00:22:44.000000 jag-panzer-0.0.8/src/jag_panzer/libs/bs4/tests/test_tree.py
-drwxrwxrwx   0        0        0        0 2023-06-09 02:50:39.048456 jag-panzer-0.0.8/src/jag_panzer/libs/soupsieve/
--rw-rw-rw-   0        0        0     4630 2023-06-06 00:22:44.000000 jag-panzer-0.0.8/src/jag_panzer/libs/soupsieve/__init__.py
--rw-rw-rw-   0        0        0     6842 2023-06-06 00:22:44.000000 jag-panzer-0.0.8/src/jag_panzer/libs/soupsieve/__meta__.py
--rw-rw-rw-   0        0        0    58152 2023-06-06 00:22:44.000000 jag-panzer-0.0.8/src/jag_panzer/libs/soupsieve/css_match.py
--rw-rw-rw-   0        0        0    47063 2023-06-06 00:22:44.000000 jag-panzer-0.0.8/src/jag_panzer/libs/soupsieve/css_parser.py
--rw-rw-rw-   0        0        0    10337 2023-06-06 00:22:44.000000 jag-panzer-0.0.8/src/jag_panzer/libs/soupsieve/css_types.py
--rw-rw-rw-   0        0        0     4053 2023-06-06 00:22:44.000000 jag-panzer-0.0.8/src/jag_panzer/libs/soupsieve/pretty.py
--rw-rw-rw-   0        0        0        0 2023-06-06 00:22:44.000000 jag-panzer-0.0.8/src/jag_panzer/libs/soupsieve/py.typed
--rw-rw-rw-   0        0        0     3374 2023-06-06 00:22:44.000000 jag-panzer-0.0.8/src/jag_panzer/libs/soupsieve/util.py
-drwxrwxrwx   0        0        0        0 2023-06-09 02:50:39.056451 jag-panzer-0.0.8/src/jag_panzer/libs/yattag/
--rw-rw-rw-   0        0        0     1743 2023-03-03 09:07:48.000000 jag-panzer-0.0.8/src/jag_panzer/libs/yattag/__init__.py
--rw-rw-rw-   0        0        0    18197 2020-08-06 21:26:32.000000 jag-panzer-0.0.8/src/jag_panzer/libs/yattag/doc.py
--rw-rw-rw-   0        0        0    12029 2023-01-02 11:12:52.000000 jag-panzer-0.0.8/src/jag_panzer/libs/yattag/indentation.py
--rw-rw-rw-   0        0        0        0 2019-12-25 20:07:02.000000 jag-panzer-0.0.8/src/jag_panzer/libs/yattag/py.typed
--rw-rw-rw-   0        0        0    18081 2019-12-24 00:01:02.000000 jag-panzer-0.0.8/src/jag_panzer/libs/yattag/simpledoc.py
-drwxrwxrwx   0        0        0        0 2023-06-09 02:50:39.058450 jag-panzer-0.0.8/src/jag_panzer/mimes/
--rw-rw-rw-   0        0        0     2762 2023-06-03 17:16:43.000000 jag-panzer-0.0.8/src/jag_panzer/mimes/mime_types_base.py
--rw-rw-rw-   0        0        0     1938 2023-06-03 17:16:43.000000 jag-panzer-0.0.8/src/jag_panzer/response_codes.py
--rw-rw-rw-   0        0        0     7363 2023-06-08 23:38:46.000000 jag-panzer-0.0.8/src/jag_panzer/server.py
--rwxrwxrwx   0        0        0       12 2023-06-07 01:47:22.000000 jag-panzer-0.0.8/src/jag_panzer/test.cmd
-drwxrwxrwx   0        0        0        0 2023-06-09 02:50:38.949160 jag-panzer-0.0.8/src/jag_panzer.egg-info/
--rw-rw-rw-   0        0        0      560 2023-06-09 02:50:38.000000 jag-panzer-0.0.8/src/jag_panzer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3986 2023-06-09 02:50:38.000000 jag-panzer-0.0.8/src/jag_panzer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 02:50:38.000000 jag-panzer-0.0.8/src/jag_panzer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-09 02:50:38.000000 jag-panzer-0.0.8/src/jag_panzer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 12:21:33.589674 jag-panzer-0.0.9/
+-rw-rw-rw-   0        0        0      161 2023-06-09 00:40:57.000000 jag-panzer-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0       46 2023-06-09 02:05:06.000000 jag-panzer-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      560 2023-06-09 12:21:33.589674 jag-panzer-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       26 2023-06-09 00:32:58.000000 jag-panzer-0.0.9/README.md
+-rw-rw-rw-   0        0        0      108 2023-06-09 00:12:29.000000 jag-panzer-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0      671 2023-06-09 12:21:33.594671 jag-panzer-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-09 12:21:32.884925 jag-panzer-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-06-09 12:21:33.002743 jag-panzer-0.0.9/src/jag_panzer/
+-rw-rw-rw-   0        0        0        0 2023-06-09 00:13:59.000000 jag-panzer-0.0.9/src/jag_panzer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 12:21:33.028717 jag-panzer-0.0.9/src/jag_panzer/assets/
+drwxrwxrwx   0        0        0        0 2023-06-09 12:21:33.063698 jag-panzer-0.0.9/src/jag_panzer/assets/dir_listing/
+-rw-rw-rw-   0        0        0      356 2023-06-08 21:39:34.000000 jag-panzer-0.0.9/src/jag_panzer/assets/dir_listing/base.html
+-rw-rw-rw-   0        0        0      446 2023-06-06 00:39:53.000000 jag-panzer-0.0.9/src/jag_panzer/assets/dir_listing/dir_icon.svg
+-rw-rw-rw-   0        0        0      682 2023-06-07 06:27:42.000000 jag-panzer-0.0.9/src/jag_panzer/assets/dir_listing/download_icon.svg
+-rw-rw-rw-   0        0        0      704 2023-06-06 00:40:06.000000 jag-panzer-0.0.9/src/jag_panzer/assets/dir_listing/file_icon.svg
+-rw-rw-rw-   0        0        0       21 2023-06-06 01:12:59.000000 jag-panzer-0.0.9/src/jag_panzer/assets/dir_listing/script.js
+-rw-rw-rw-   0        0        0     1355 2023-06-07 07:34:01.000000 jag-panzer-0.0.9/src/jag_panzer/assets/dir_listing/style.css
+-rw-rw-rw-   0        0        0      260 2023-06-07 02:18:15.000000 jag-panzer-0.0.9/src/jag_panzer/assets/reject.html
+-rw-rw-rw-   0        0        0    18350 2023-06-09 12:04:50.000000 jag-panzer-0.0.9/src/jag_panzer/base_room.py
+drwxrwxrwx   0        0        0        0 2023-06-09 12:21:33.077690 jag-panzer-0.0.9/src/jag_panzer/cgi/
+-rw-rw-rw-   0        0        0        0 2023-06-09 00:00:24.000000 jag-panzer-0.0.9/src/jag_panzer/cgi/__init__.py
+-rw-rw-rw-   0        0        0     5087 2023-06-03 17:16:43.000000 jag-panzer-0.0.9/src/jag_panzer/cgi/burn_power.py
+-rw-rw-rw-   0        0        0      451 2023-06-03 17:16:43.000000 jag-panzer-0.0.9/src/jag_panzer/cgi/hitman.py
+-rw-rw-rw-   0        0        0     6691 2023-06-03 17:16:43.000000 jag-panzer-0.0.9/src/jag_panzer/cgi/jag.py
+drwxrwxrwx   0        0        0        0 2023-06-09 12:21:33.085317 jag-panzer-0.0.9/src/jag_panzer/cgi/templates/
+drwxrwxrwx   0        0        0        0 2023-06-09 12:21:33.087346 jag-panzer-0.0.9/src/jag_panzer/cgi/templates/light_httpd/
+drwxrwxrwx   0        0        0        0 2023-06-09 12:21:33.111301 jag-panzer-0.0.9/src/jag_panzer/cgi/templates/light_httpd/conf-enabled/
+-rw-rw-rw-   0        0        0       91 2023-06-03 17:16:43.000000 jag-panzer-0.0.9/src/jag_panzer/cgi/templates/light_httpd/conf-enabled/10-accesslog.conf
+-rw-rw-rw-   0        0        0      306 2023-06-03 17:16:43.000000 jag-panzer-0.0.9/src/jag_panzer/cgi/templates/light_httpd/conf-enabled/10-cgi.conf
+-rw-rw-rw-   0        0        0      454 2023-06-03 17:16:43.000000 jag-panzer-0.0.9/src/jag_panzer/cgi/templates/light_httpd/conf-enabled/10-status.conf
+-rw-rw-rw-   0        0        0     2245 2023-06-03 17:16:43.000000 jag-panzer-0.0.9/src/jag_panzer/cgi/templates/light_httpd/server_prms.conf
+-rw-rw-rw-   0        0        0      403 2023-06-03 17:16:43.000000 jag-panzer-0.0.9/src/jag_panzer/cgi/templates/unit.service
+-rw-rw-rw-   0        0        0     2539 2023-06-08 21:42:17.000000 jag-panzer-0.0.9/src/jag_panzer/dir_list.py
+-rw-rw-rw-   0        0        0      369 2023-06-07 05:17:03.000000 jag-panzer-0.0.9/src/jag_panzer/jag_util.py
+drwxrwxrwx   0        0        0        0 2023-06-09 12:21:32.892921 jag-panzer-0.0.9/src/jag_panzer/libs/
+drwxrwxrwx   0        0        0        0 2023-06-09 12:21:33.185260 jag-panzer-0.0.9/src/jag_panzer/libs/bs4/
+-rw-rw-rw-   0        0        0    33822 2023-06-06 00:22:44.000000 jag-panzer-0.0.9/src/jag_panzer/libs/bs4/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 12:21:33.233241 jag-panzer-0.0.9/src/jag_panzer/libs/bs4/builder/
+-rw-rw-rw-   0        0        0    24393 2023-06-06 00:22:44.000000 jag-panzer-0.0.9/src/jag_panzer/libs/bs4/builder/__init__.py
+-rw-rw-rw-   0        0        0    19078 2023-06-06 00:22:44.000000 jag-panzer-0.0.9/src/jag_panzer/libs/bs4/builder/_html5lib.py
+-rw-rw-rw-   0        0        0    14919 2023-06-06 00:22:44.000000 jag-panzer-0.0.9/src/jag_panzer/libs/bs4/builder/_htmlparser.py
+-rw-rw-rw-   0        0        0    14904 2023-06-06 00:22:44.000000 jag-panzer-0.0.9/src/jag_panzer/libs/bs4/builder/_lxml.py
+-rw-rw-rw-   0        0        0    10077 2023-06-06 00:22:44.000000 jag-panzer-0.0.9/src/jag_panzer/libs/bs4/css.py
+-rw-rw-rw-   0        0        0    41158 2023-06-06 00:22:44.000000 jag-panzer-0.0.9/src/jag_panzer/libs/bs4/dammit.py
+-rw-rw-rw-   0        0        0     7195 2023-06-06 00:22:44.000000 jag-panzer-0.0.9/src/jag_panzer/libs/bs4/diagnose.py
+-rw-rw-rw-   0        0        0    92716 2023-06-06 00:22:44.000000 jag-panzer-0.0.9/src/jag_panzer/libs/bs4/element.py
+-rw-rw-rw-   0        0        0     7184 2023-06-06 00:22:44.000000 jag-panzer-0.0.9/src/jag_panzer/libs/bs4/formatter.py
+drwxrwxrwx   0        0        0        0 2023-06-09 12:21:33.358160 jag-panzer-0.0.9/src/jag_panzer/libs/bs4/tests/
+-rw-rw-rw-   0        0        0    48391 2023-06-06 00:22:44.000000 jag-panzer-0.0.9/src/jag_panzer/libs/bs4/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 12:21:33.415129 jag-panzer-0.0.9/src/jag_panzer/libs/bs4/tests/fuzz/
+-rw-rw-rw-   0        0        0       23 2023-06-06 00:22:44.000000 jag-panzer-0.0.9/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-4818336571064320.testcase
+-rw-rw-rw-   0        0        0       30 2023-06-06 00:22:44.000000 jag-panzer-0.0.9/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-4999465949331456.testcase
+-rw-rw-rw-   0        0        0    19469 2023-06-06 00:22:44.000000 jag-panzer-0.0.9/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-5167584867909632.testcase
+-rw-rw-rw-   0        0        0        5 2023-06-06 00:22:44.000000 jag-panzer-0.0.9/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-5703933063462912.testcase
+-rw-rw-rw-   0        0        0       35 2023-06-06 00:22:44.000000 jag-panzer-0.0.9/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-5843991618256896.testcase
+-rw-rw-rw-   0        0        0    51495 2023-06-06 00:22:44.000000 jag-panzer-0.0.9/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-5984173902397440.testcase
+-rw-rw-rw-   0        0        0    10380 2023-06-06 00:22:44.000000 jag-panzer-0.0.9/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-6124268085182464.testcase
+-rw-rw-rw-   0        0        0       19 2023-06-06 00:22:44.000000 jag-panzer-0.0.9/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-6241471367348224.testcase
+-rw-rw-rw-   0        0        0     3546 2023-06-06 00:22:44.000000 jag-panzer-0.0.9/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-6450958476902400.testcase
+-rw-rw-rw-   0        0        0      124 2023-06-06 00:22:44.000000 jag-panzer-0.0.9/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-6600557255327744.testcase
+-rw-rw-rw-   0        0        0     2607 2023-06-06 00:22:44.000000 jag-panzer-0.0.9/src/jag_panzer/libs/bs4/tests/fuzz/crash-0d306a50c8ed8bcd0785b67000fcd5dea1d33f08.testcase
+-rw-rw-rw-   0        0        0     1115 2023-06-06 00:22:44.000000 jag-panzer-0.0.9/src/jag_panzer/libs/bs4/tests/test_builder.py
+-rw-rw-rw-   0        0        0     5114 2023-06-06 00:22:44.000000 jag-panzer-0.0.9/src/jag_panzer/libs/bs4/tests/test_builder_registry.py
+-rw-rw-rw-   0        0        0    17279 2023-06-06 00:22:44.000000 jag-panzer-0.0.9/src/jag_panzer/libs/bs4/tests/test_css.py
+-rw-rw-rw-   0        0        0    15451 2023-06-06 00:22:44.000000 jag-panzer-0.0.9/src/jag_panzer/libs/bs4/tests/test_dammit.py
+-rw-rw-rw-   0        0        0     1127 2023-06-06 00:22:44.000000 jag-panzer-0.0.9/src/jag_panzer/libs/bs4/tests/test_docs.py
+-rw-rw-rw-   0        0        0     2377 2023-06-06 00:22:44.000000 jag-panzer-0.0.9/src/jag_panzer/libs/bs4/tests/test_element.py
+-rw-rw-rw-   0        0        0     4148 2023-06-06 00:22:44.000000 jag-panzer-0.0.9/src/jag_panzer/libs/bs4/tests/test_formatter.py
+-rw-rw-rw-   0        0        0     3637 2023-06-06 00:22:44.000000 jag-panzer-0.0.9/src/jag_panzer/libs/bs4/tests/test_fuzz.py
+-rw-rw-rw-   0        0        0     8322 2023-06-06 00:22:44.000000 jag-panzer-0.0.9/src/jag_panzer/libs/bs4/tests/test_html5lib.py
+-rw-rw-rw-   0        0        0     6256 2023-06-06 00:22:44.000000 jag-panzer-0.0.9/src/jag_panzer/libs/bs4/tests/test_htmlparser.py
+-rw-rw-rw-   0        0        0     7635 2023-06-06 00:22:44.000000 jag-panzer-0.0.9/src/jag_panzer/libs/bs4/tests/test_lxml.py
+-rw-rw-rw-   0        0        0     5081 2023-06-06 00:22:44.000000 jag-panzer-0.0.9/src/jag_panzer/libs/bs4/tests/test_navigablestring.py
+-rw-rw-rw-   0        0        0    14274 2023-06-06 00:22:44.000000 jag-panzer-0.0.9/src/jag_panzer/libs/bs4/tests/test_pageelement.py
+-rw-rw-rw-   0        0        0    19877 2023-06-06 00:22:44.000000 jag-panzer-0.0.9/src/jag_panzer/libs/bs4/tests/test_soup.py
+-rw-rw-rw-   0        0        0     9016 2023-06-06 00:22:44.000000 jag-panzer-0.0.9/src/jag_panzer/libs/bs4/tests/test_tag.py
+-rw-rw-rw-   0        0        0    48129 2023-06-06 00:22:44.000000 jag-panzer-0.0.9/src/jag_panzer/libs/bs4/tests/test_tree.py
+drwxrwxrwx   0        0        0        0 2023-06-09 12:21:33.516070 jag-panzer-0.0.9/src/jag_panzer/libs/soupsieve/
+-rw-rw-rw-   0        0        0     4630 2023-06-06 00:22:44.000000 jag-panzer-0.0.9/src/jag_panzer/libs/soupsieve/__init__.py
+-rw-rw-rw-   0        0        0     6842 2023-06-06 00:22:44.000000 jag-panzer-0.0.9/src/jag_panzer/libs/soupsieve/__meta__.py
+-rw-rw-rw-   0        0        0    58152 2023-06-06 00:22:44.000000 jag-panzer-0.0.9/src/jag_panzer/libs/soupsieve/css_match.py
+-rw-rw-rw-   0        0        0    47063 2023-06-06 00:22:44.000000 jag-panzer-0.0.9/src/jag_panzer/libs/soupsieve/css_parser.py
+-rw-rw-rw-   0        0        0    10337 2023-06-06 00:22:44.000000 jag-panzer-0.0.9/src/jag_panzer/libs/soupsieve/css_types.py
+-rw-rw-rw-   0        0        0     4053 2023-06-06 00:22:44.000000 jag-panzer-0.0.9/src/jag_panzer/libs/soupsieve/pretty.py
+-rw-rw-rw-   0        0        0        0 2023-06-06 00:22:44.000000 jag-panzer-0.0.9/src/jag_panzer/libs/soupsieve/py.typed
+-rw-rw-rw-   0        0        0     3374 2023-06-06 00:22:44.000000 jag-panzer-0.0.9/src/jag_panzer/libs/soupsieve/util.py
+drwxrwxrwx   0        0        0        0 2023-06-09 12:21:33.568041 jag-panzer-0.0.9/src/jag_panzer/libs/yattag/
+-rw-rw-rw-   0        0        0     1743 2023-03-03 09:07:48.000000 jag-panzer-0.0.9/src/jag_panzer/libs/yattag/__init__.py
+-rw-rw-rw-   0        0        0    18197 2020-08-06 21:26:32.000000 jag-panzer-0.0.9/src/jag_panzer/libs/yattag/doc.py
+-rw-rw-rw-   0        0        0    12029 2023-01-02 11:12:52.000000 jag-panzer-0.0.9/src/jag_panzer/libs/yattag/indentation.py
+-rw-rw-rw-   0        0        0        0 2019-12-25 20:07:02.000000 jag-panzer-0.0.9/src/jag_panzer/libs/yattag/py.typed
+-rw-rw-rw-   0        0        0    18081 2019-12-24 00:01:02.000000 jag-panzer-0.0.9/src/jag_panzer/libs/yattag/simpledoc.py
+drwxrwxrwx   0        0        0        0 2023-06-09 12:21:33.571038 jag-panzer-0.0.9/src/jag_panzer/mimes/
+-rw-rw-rw-   0        0        0     2762 2023-06-03 17:16:43.000000 jag-panzer-0.0.9/src/jag_panzer/mimes/mime_types_base.py
+-rw-rw-rw-   0        0        0     1938 2023-06-03 17:16:43.000000 jag-panzer-0.0.9/src/jag_panzer/response_codes.py
+-rw-rw-rw-   0        0        0     7363 2023-06-08 23:38:46.000000 jag-panzer-0.0.9/src/jag_panzer/server.py
+-rwxrwxrwx   0        0        0       12 2023-06-07 01:47:22.000000 jag-panzer-0.0.9/src/jag_panzer/test.cmd
+drwxrwxrwx   0        0        0        0 2023-06-09 12:21:33.026718 jag-panzer-0.0.9/src/jag_panzer.egg-info/
+-rw-rw-rw-   0        0        0      560 2023-06-09 12:21:32.000000 jag-panzer-0.0.9/src/jag_panzer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3986 2023-06-09 12:21:32.000000 jag-panzer-0.0.9/src/jag_panzer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 12:21:32.000000 jag-panzer-0.0.9/src/jag_panzer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-09 12:21:32.000000 jag-panzer-0.0.9/src/jag_panzer.egg-info/top_level.txt
```

### Comparing `jag-panzer-0.0.8/PKG-INFO` & `jag-panzer-0.0.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jag-panzer
-Version: 0.0.8
+Version: 0.0.9
 Summary: Simple HTTP server allowing pure python workflow
 Home-page: https://github.com/MrKleiner/jag
 Author: Mr.Kleiner
 Author-email: megaadrenaline1055@gmail.com
 Project-URL: Bug Tracker, https://github.com/MrKleiner/jag/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `jag-panzer-0.0.8/setup.cfg` & `jag-panzer-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206a 6167 2d70 616e 7a65 720d 0a76   = jag-panzer..v
-00000020: 6572 7369 6f6e 203d 2030 2e30 2e38 0d0a  ersion = 0.0.8..
+00000020: 6572 7369 6f6e 203d 2030 2e30 2e39 0d0a  ersion = 0.0.9..
 00000030: 6175 7468 6f72 203d 204d 722e 4b6c 6569  author = Mr.Klei
 00000040: 6e65 720d 0a61 7574 686f 725f 656d 6169  ner..author_emai
 00000050: 6c20 3d20 6d65 6761 6164 7265 6e61 6c69  l = megaadrenali
 00000060: 6e65 3130 3535 4067 6d61 696c 2e63 6f6d  ne1055@gmail.com
 00000070: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
 00000080: 5369 6d70 6c65 2048 5454 5020 7365 7276  Simple HTTP serv
 00000090: 6572 2061 6c6c 6f77 696e 6720 7075 7265  er allowing pure
```

### Comparing `jag-panzer-0.0.8/src/jag_panzer/assets/dir_listing/download_icon.svg` & `jag-panzer-0.0.9/src/jag_panzer/assets/dir_listing/download_icon.svg`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.8/src/jag_panzer/assets/dir_listing/file_icon.svg` & `jag-panzer-0.0.9/src/jag_panzer/assets/dir_listing/file_icon.svg`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.8/src/jag_panzer/assets/dir_listing/style.css` & `jag-panzer-0.0.9/src/jag_panzer/assets/dir_listing/style.css`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.8/src/jag_panzer/base_room.py` & `jag-panzer-0.0.9/src/jag_panzer/base_room.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,14 +55,15 @@
 	# If no file is provided - serve path from the request
 	def serve_file(self, tgt_file=None, respect_range=True):
 		request = self.request
 		response = self.response
 
 		if not request.abspath.is_file():
 			self.request.reject()
+			return
 
 		# all good - set content type and send the shit
 		response.content_type = (
 			request.srv_res.mimes['signed'].get(request.abspath.suffix)
 			or
 			'application/octet-stream'
 		)
@@ -70,15 +71,15 @@
 		# if the size is too big for a single flush - stream in chunks
 		# This is very important, because serving a 2kb svg in chunks slows the response time
 		# and serving an 18gb .mkv Blu-ray remux in a single flush is impossible
 		if request.abspath.stat().st_size > request.srv_res.cfg['static_cdn']['max_buffered_size']:
 			with open(str(request.abspath), 'r+b') as f:
 				# if request comes with a Range header - try serving the requested byterange
 				# '0-' VERY funny, fuck right off
-				if request.byterange and request.headers['range'].strip() != '0-' and respect_range:
+				if request.byterange and (request.headers['range'].strip() != '0-') and respect_range:
 					response.serve_range(f)
 				else:
 					response.stream_buffer(f, (1024*1024)*5)
 		else:
 			response.flush_buffer(request.abspath.read_bytes())
 
 		self.request.terminate()
@@ -182,14 +183,16 @@
 		self.headers = {
 			'Server': 'Jag',
 		}
 
 		self.content_type = 'application/octet-stream'
 		self.code = 200
 
+		self.offered_services = sv_services(self.request, self)
+
 	# dump headers and response code to the client
 	def send_preflight(self):
 		"""
 		Dump headers and response code to the client
 		"""
 
 		# send response code
@@ -315,14 +318,16 @@
 				aligned_reader = aligned_buf_read(buf, _start, _end)
 				while True:
 					data = aligned_reader.read(self.srv_res.cfg['chunk_stream_piece_size'])
 					if not data:
 						break
 					stream.send(data)
 
+		self.request.terminate()
+
 
 
 
 
 class cl_request:
 	def __init__(self, cl_con, cl_addr, srv_res):
 		self.cl_con = cl_con
@@ -365,14 +370,18 @@
 		self.head_buf = io.BytesIO()
 		self.body_buf = io.BytesIO()
 
 		double_rn = 0
 		expect_r = False
 
 		# important todo: This is extremely (relatively) slow
+		# simple http server from python base library does something like
+		# do 1 byte receive from client till \r\n\r\n
+		# OR
+		# Read 65535 bytes and then process the thing
 		while True:
 			data = self.cl_con.recv(65535)
 			for idx, char in enumerate(data):
 				# conlog('Char:', chr(char).encode())
 
 				if char != 10 and char != 13:
 					# conlog('^ no match, abort')
@@ -400,15 +409,15 @@
 					# conlog('Writing to body buffer:', bytes(data[(idx+1):]))
 					self.body_buf.write(bytes(data[(idx+1):]))
 					self.head_buf.write(bytes(data[:idx]))
 					break
 
 			if double_rn == 2:
 				conlog('Header Buf', self.head_buf.getvalue().decode())
-				conlog('Body Buf', self.body_buf.getvalue())
+				# conlog('Body Buf', self.body_buf.getvalue())
 				break
 
 			self.head_buf.write(data)
 
 	# Request evaluation has a dedicated function for easier error handling
 	def _eval_request(self):
 		# io = self.srv_res.pylib.io
@@ -441,14 +450,15 @@
 		# first - evaluate query params
 		self.query_params = {k:(''.join(v)) for (k,v) in urllib.parse.parse_qs(parsed_url.query, True).items()}
 
 		# then, evaluate path
 		decoded_url_path = urllib.parse.unquote(parsed_url.path)
 		self.abspath = self.srv_res.doc_root / Path(decoded_url_path.lstrip('/'))
 		self.relpath = Path(decoded_url_path.lstrip('/'))
+		self.trimpath = self.relpath
 
 		# Delete the first line as it's no longer needed
 		del header_data[0]
 
 		# parse the remaining headers into a dict
 		request_dict = {}
 		for line in header_data:
@@ -456,14 +466,16 @@
 			if line.strip() == '':
 				continue
 			line_split = line.split(': ')
 			request_dict[line_split[0].lower()] = ': '.join(line_split[1:])
 
 		dict_pretty_print(request_dict)
 
+		self.headers = request_dict
+
 
 	# Actions
 	# =================
 
 	# Properly collapse the tunnel between server and client
 	def terminate(self):
 		socket = self.srv_res.pylib.socket
@@ -480,14 +492,49 @@
 		self.response.content_type = 'text/html'
 		self.response.flush_buffer(
 			self.srv_res.reject_precache
 			.replace(b'$$reason', self.srv_res.response_codes[code].encode())
 			.replace(b'$$hint', str(hint).encode())
 		)
 
+	# I cannot be bothered. Here, have *args and fuckoff
+	def match_path(self, action_dict, *args, trim_path=True):
+		"""
+		Sample set/list:
+		{
+			('/pootis/sandwich/dispenser', func_name1),
+			('/pootis',                    func_name2),
+		}
+		"""
+		comparator = '/' + self.relpath.as_posix()
+
+		for rpath, func in action_dict:
+			# print(rpath, 'startswith', )
+			if comparator.startswith(rpath):
+				if trim_path:
+					self.trimpath = self.srv_res.pylib.Path(comparator.lstrip(rpath))
+				return func(self, self.response, self.response.offered_services, *args)
+
+		# if no match was found - return false
+		return False
+
+
+	def read_body_stream(self):
+		content_length = int(self.headers['content-length'])
+		read_progress = self.body_buf.seek(0, 2)
+		yield self.body_buf.getvalue()
+		while True:
+			if read_progress >= content_length:
+				break
+			# todo: finetune this value
+			# or expose it in the config
+			received_data = self.cl_con.recv(65535)
+			yield received_data
+			read_progress += len(received_data)
+
 
 	# Utility
 	# =================
 	def parse_kv(self, kvs, separator=',', key_to_lower=True):
 		pairs = kvs.split(separator)
 		result = {}
 		for pair in pairs:
@@ -592,32 +639,32 @@
 		srv_res.reload_libs()
 
 		# Evaluate the request
 		evaluated_request = cl_request(cl_con, cl_addr, srv_res)
 		conlog('Initialized basic room, evaluated request')
 
 		# Create service object
-		offered_services = sv_services(evaluated_request, evaluated_request.response)
+		# offered_services = sv_services(evaluated_request, evaluated_request.response)
 
 		# Now either pass the control to the room specified in the config
 		# or the default room
 		if srv_res.cfg['room_file']:
 			spec = importlib.util.spec_from_file_location('main', str(srv_res.cfg['room_file']))
 			custom_func = importlib.util.module_from_spec(spec)
 			spec.loader.exec_module(custom_func)
 			custom_func.main(
 				evaluated_request,
 				evaluated_request.response,
-				offered_services
+				evaluated_request.response.offered_services
 			)
 		else:
 			_default_room(
 				evaluated_request,
 				evaluated_request.response,
-				offered_services
+				evaluated_request.response.offered_services
 			)
 
 	except Exception as err:
 		conlog(
 			''.join(
 				traceback.format_exception(
 					type(err),
```

### Comparing `jag-panzer-0.0.8/src/jag_panzer/cgi/burn_power.py` & `jag-panzer-0.0.9/src/jag_panzer/cgi/burn_power.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.8/src/jag_panzer/cgi/jag.py` & `jag-panzer-0.0.9/src/jag_panzer/cgi/jag.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.8/src/jag_panzer/cgi/templates/light_httpd/server_prms.conf` & `jag-panzer-0.0.9/src/jag_panzer/cgi/templates/light_httpd/server_prms.conf`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.8/src/jag_panzer/dir_list.py` & `jag-panzer-0.0.9/src/jag_panzer/dir_list.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.8/src/jag_panzer/libs/bs4/__init__.py` & `jag-panzer-0.0.9/src/jag_panzer/libs/bs4/__init__.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.8/src/jag_panzer/libs/bs4/builder/__init__.py` & `jag-panzer-0.0.9/src/jag_panzer/libs/bs4/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.8/src/jag_panzer/libs/bs4/builder/_html5lib.py` & `jag-panzer-0.0.9/src/jag_panzer/libs/bs4/builder/_html5lib.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.8/src/jag_panzer/libs/bs4/builder/_htmlparser.py` & `jag-panzer-0.0.9/src/jag_panzer/libs/bs4/builder/_htmlparser.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.8/src/jag_panzer/libs/bs4/builder/_lxml.py` & `jag-panzer-0.0.9/src/jag_panzer/libs/bs4/builder/_lxml.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.8/src/jag_panzer/libs/bs4/css.py` & `jag-panzer-0.0.9/src/jag_panzer/libs/bs4/css.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.8/src/jag_panzer/libs/bs4/dammit.py` & `jag-panzer-0.0.9/src/jag_panzer/libs/bs4/dammit.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.8/src/jag_panzer/libs/bs4/diagnose.py` & `jag-panzer-0.0.9/src/jag_panzer/libs/bs4/diagnose.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.8/src/jag_panzer/libs/bs4/element.py` & `jag-panzer-0.0.9/src/jag_panzer/libs/bs4/element.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.8/src/jag_panzer/libs/bs4/formatter.py` & `jag-panzer-0.0.9/src/jag_panzer/libs/bs4/formatter.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.8/src/jag_panzer/libs/bs4/tests/__init__.py` & `jag-panzer-0.0.9/src/jag_panzer/libs/bs4/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.8/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-5167584867909632.testcase` & `jag-panzer-0.0.9/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-5167584867909632.testcase`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.8/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-5984173902397440.testcase` & `jag-panzer-0.0.9/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-5984173902397440.testcase`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.8/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-6124268085182464.testcase` & `jag-panzer-0.0.9/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-6124268085182464.testcase`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.8/src/jag_panzer/libs/bs4/tests/fuzz/crash-0d306a50c8ed8bcd0785b67000fcd5dea1d33f08.testcase` & `jag-panzer-0.0.9/src/jag_panzer/libs/bs4/tests/fuzz/crash-0d306a50c8ed8bcd0785b67000fcd5dea1d33f08.testcase`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.8/src/jag_panzer/libs/bs4/tests/test_builder.py` & `jag-panzer-0.0.9/src/jag_panzer/libs/bs4/tests/test_builder.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.8/src/jag_panzer/libs/bs4/tests/test_builder_registry.py` & `jag-panzer-0.0.9/src/jag_panzer/libs/bs4/tests/test_builder_registry.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.8/src/jag_panzer/libs/bs4/tests/test_css.py` & `jag-panzer-0.0.9/src/jag_panzer/libs/bs4/tests/test_css.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.8/src/jag_panzer/libs/bs4/tests/test_dammit.py` & `jag-panzer-0.0.9/src/jag_panzer/libs/bs4/tests/test_dammit.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.8/src/jag_panzer/libs/bs4/tests/test_docs.py` & `jag-panzer-0.0.9/src/jag_panzer/libs/bs4/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.8/src/jag_panzer/libs/bs4/tests/test_element.py` & `jag-panzer-0.0.9/src/jag_panzer/libs/bs4/tests/test_element.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.8/src/jag_panzer/libs/bs4/tests/test_formatter.py` & `jag-panzer-0.0.9/src/jag_panzer/libs/bs4/tests/test_formatter.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.8/src/jag_panzer/libs/bs4/tests/test_fuzz.py` & `jag-panzer-0.0.9/src/jag_panzer/libs/bs4/tests/test_fuzz.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.8/src/jag_panzer/libs/bs4/tests/test_html5lib.py` & `jag-panzer-0.0.9/src/jag_panzer/libs/bs4/tests/test_html5lib.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.8/src/jag_panzer/libs/bs4/tests/test_htmlparser.py` & `jag-panzer-0.0.9/src/jag_panzer/libs/bs4/tests/test_htmlparser.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.8/src/jag_panzer/libs/bs4/tests/test_lxml.py` & `jag-panzer-0.0.9/src/jag_panzer/libs/bs4/tests/test_lxml.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.8/src/jag_panzer/libs/bs4/tests/test_navigablestring.py` & `jag-panzer-0.0.9/src/jag_panzer/libs/bs4/tests/test_navigablestring.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.8/src/jag_panzer/libs/bs4/tests/test_pageelement.py` & `jag-panzer-0.0.9/src/jag_panzer/libs/bs4/tests/test_pageelement.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.8/src/jag_panzer/libs/bs4/tests/test_soup.py` & `jag-panzer-0.0.9/src/jag_panzer/libs/bs4/tests/test_soup.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.8/src/jag_panzer/libs/bs4/tests/test_tag.py` & `jag-panzer-0.0.9/src/jag_panzer/libs/bs4/tests/test_tag.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.8/src/jag_panzer/libs/bs4/tests/test_tree.py` & `jag-panzer-0.0.9/src/jag_panzer/libs/bs4/tests/test_tree.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.8/src/jag_panzer/libs/soupsieve/__init__.py` & `jag-panzer-0.0.9/src/jag_panzer/libs/soupsieve/__init__.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.8/src/jag_panzer/libs/soupsieve/__meta__.py` & `jag-panzer-0.0.9/src/jag_panzer/libs/soupsieve/__meta__.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.8/src/jag_panzer/libs/soupsieve/css_match.py` & `jag-panzer-0.0.9/src/jag_panzer/libs/soupsieve/css_match.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.8/src/jag_panzer/libs/soupsieve/css_parser.py` & `jag-panzer-0.0.9/src/jag_panzer/libs/soupsieve/css_parser.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.8/src/jag_panzer/libs/soupsieve/css_types.py` & `jag-panzer-0.0.9/src/jag_panzer/libs/soupsieve/css_types.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.8/src/jag_panzer/libs/soupsieve/pretty.py` & `jag-panzer-0.0.9/src/jag_panzer/libs/soupsieve/pretty.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.8/src/jag_panzer/libs/soupsieve/util.py` & `jag-panzer-0.0.9/src/jag_panzer/libs/soupsieve/util.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.8/src/jag_panzer/libs/yattag/__init__.py` & `jag-panzer-0.0.9/src/jag_panzer/libs/yattag/__init__.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.8/src/jag_panzer/libs/yattag/doc.py` & `jag-panzer-0.0.9/src/jag_panzer/libs/yattag/doc.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.8/src/jag_panzer/libs/yattag/indentation.py` & `jag-panzer-0.0.9/src/jag_panzer/libs/yattag/indentation.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.8/src/jag_panzer/libs/yattag/simpledoc.py` & `jag-panzer-0.0.9/src/jag_panzer/libs/yattag/simpledoc.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.8/src/jag_panzer/mimes/mime_types_base.py` & `jag-panzer-0.0.9/src/jag_panzer/mimes/mime_types_base.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.8/src/jag_panzer/response_codes.py` & `jag-panzer-0.0.9/src/jag_panzer/response_codes.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.8/src/jag_panzer/server.py` & `jag-panzer-0.0.9/src/jag_panzer/server.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.0.8/src/jag_panzer.egg-info/PKG-INFO` & `jag-panzer-0.0.9/src/jag_panzer.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jag-panzer
-Version: 0.0.8
+Version: 0.0.9
 Summary: Simple HTTP server allowing pure python workflow
 Home-page: https://github.com/MrKleiner/jag
 Author: Mr.Kleiner
 Author-email: megaadrenaline1055@gmail.com
 Project-URL: Bug Tracker, https://github.com/MrKleiner/jag/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `jag-panzer-0.0.8/src/jag_panzer.egg-info/SOURCES.txt` & `jag-panzer-0.0.9/src/jag_panzer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

