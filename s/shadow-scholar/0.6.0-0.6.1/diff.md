# Comparing `tmp/shadow-scholar-0.6.0.tar.gz` & `tmp/shadow-scholar-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shadow-scholar-0.6.0.tar", last modified: Thu May 11 23:17:06 2023, max compression
+gzip compressed data, was "shadow-scholar-0.6.1.tar", last modified: Thu Jun  8 23:20:32 2023, max compression
```

## Comparing `shadow-scholar-0.6.0.tar` & `shadow-scholar-0.6.1.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-05-11 23:17:06.767712 shadow-scholar-0.6.0/
--rw-r--r--   0 lucas      (502) staff       (20)    11357 2023-01-30 22:02:35.000000 shadow-scholar-0.6.0/LICENSE
--rw-r--r--   0 lucas      (502) staff       (20)      106 2023-04-11 19:13:05.000000 shadow-scholar-0.6.0/MANIFEST.in
--rw-r--r--   0 lucas      (502) staff       (20)     6263 2023-05-11 23:17:06.767545 shadow-scholar-0.6.0/PKG-INFO
--rw-r--r--   0 lucas      (502) staff       (20)     5651 2023-05-11 23:16:57.000000 shadow-scholar-0.6.0/README.md
--rw-r--r--   0 lucas      (502) staff       (20)     2028 2023-05-11 23:16:57.000000 shadow-scholar-0.6.0/pyproject.toml
--rw-r--r--   0 lucas      (502) staff       (20)       38 2023-05-11 23:17:06.767762 shadow-scholar-0.6.0/setup.cfg
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-05-11 23:17:06.749837 shadow-scholar-0.6.0/src/
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-05-11 23:17:06.752549 shadow-scholar-0.6.0/src/shadow_scholar/
--rw-r--r--   0 lucas      (502) staff       (20)      604 2023-05-11 23:16:57.000000 shadow-scholar-0.6.0/src/shadow_scholar/__init__.py
--rw-r--r--   0 lucas      (502) staff       (20)       59 2023-03-03 22:16:56.000000 shadow-scholar-0.6.0/src/shadow_scholar/__main__.py
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-05-11 23:17:06.753511 shadow-scholar-0.6.0/src/shadow_scholar/app/
--rw-r--r--   0 lucas      (502) staff       (20)        0 2023-02-14 02:56:52.000000 shadow-scholar-0.6.0/src/shadow_scholar/app/__init__.py
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-05-11 23:17:06.754315 shadow-scholar-0.6.0/src/shadow_scholar/app/chat_s2/
--rw-r--r--   0 lucas      (502) staff       (20)        0 2023-03-02 18:48:43.000000 shadow-scholar-0.6.0/src/shadow_scholar/app/chat_s2/__init__.py
--rw-r--r--   0 lucas      (502) staff       (20)     8837 2023-05-11 23:15:29.000000 shadow-scholar-0.6.0/src/shadow_scholar/app/chat_s2/library.py
--rw-r--r--   0 lucas      (502) staff       (20)     6656 2023-05-11 22:13:47.000000 shadow-scholar-0.6.0/src/shadow_scholar/app/chat_s2/llm.py
--rw-r--r--   0 lucas      (502) staff       (20)     1995 2023-04-11 19:13:05.000000 shadow-scholar-0.6.0/src/shadow_scholar/app/chat_s2/logging.py
--rw-r--r--   0 lucas      (502) staff       (20)    19018 2023-05-11 22:13:47.000000 shadow-scholar-0.6.0/src/shadow_scholar/app/chat_s2/main.py
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-05-11 23:17:06.754599 shadow-scholar-0.6.0/src/shadow_scholar/app/chat_s2/res/
--rw-r--r--   0 lucas      (502) staff       (20)     4871 2023-03-24 00:59:46.000000 shadow-scholar-0.6.0/src/shadow_scholar/app/chat_s2/res/logo.svg
--rw-r--r--   0 lucas      (502) staff       (20)      960 2023-04-11 19:13:05.000000 shadow-scholar-0.6.0/src/shadow_scholar/app/chat_s2/res/style.css
--rw-r--r--   0 lucas      (502) staff       (20)     6153 2023-05-11 22:13:47.000000 shadow-scholar-0.6.0/src/shadow_scholar/app/chat_s2/search.py
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-05-11 23:17:06.757995 shadow-scholar-0.6.0/src/shadow_scholar/app/galactica/
--rw-r--r--   0 lucas      (502) staff       (20)        0 2023-02-23 21:23:12.000000 shadow-scholar-0.6.0/src/shadow_scholar/app/galactica/__init__.py
--rw-r--r--   0 lucas      (502) staff       (20)     8596 2023-02-23 21:23:12.000000 shadow-scholar-0.6.0/src/shadow_scholar/app/galactica/_old.py
--rw-r--r--   0 lucas      (502) staff       (20)     9251 2023-02-23 21:23:12.000000 shadow-scholar-0.6.0/src/shadow_scholar/app/galactica/constants.py
--rw-r--r--   0 lucas      (502) staff       (20)     8755 2023-03-03 21:48:10.000000 shadow-scholar-0.6.0/src/shadow_scholar/app/galactica/convert_to_int8.py
--rw-r--r--   0 lucas      (502) staff       (20)  1290127 2023-02-23 21:23:12.000000 shadow-scholar-0.6.0/src/shadow_scholar/app/galactica/example.png
--rw-r--r--   0 lucas      (502) staff       (20)    16518 2023-04-03 06:48:20.000000 shadow-scholar-0.6.0/src/shadow_scholar/app/galactica/galai_model.py
--rw-r--r--   0 lucas      (502) staff       (20)     1490 2023-02-23 21:23:12.000000 shadow-scholar-0.6.0/src/shadow_scholar/app/galactica/galai_parallel_policy.py
--rw-r--r--   0 lucas      (502) staff       (20)     5433 2023-02-23 21:23:12.000000 shadow-scholar-0.6.0/src/shadow_scholar/app/galactica/galai_utils.py
--rw-r--r--   0 lucas      (502) staff       (20)     9211 2023-03-24 00:59:46.000000 shadow-scholar-0.6.0/src/shadow_scholar/app/galactica/main.py
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-05-11 23:17:06.758401 shadow-scholar-0.6.0/src/shadow_scholar/app/hello_world/
--rw-r--r--   0 lucas      (502) staff       (20)        0 2023-03-03 22:16:55.000000 shadow-scholar-0.6.0/src/shadow_scholar/app/hello_world/__init__.py
--rw-r--r--   0 lucas      (502) staff       (20)        0 2023-03-09 19:05:25.000000 shadow-scholar-0.6.0/src/shadow_scholar/app/hello_world/gradio.css
--rw-r--r--   0 lucas      (502) staff       (20)     1622 2023-05-11 23:16:57.000000 shadow-scholar-0.6.0/src/shadow_scholar/app/hello_world/main.py
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-05-11 23:17:06.759810 shadow-scholar-0.6.0/src/shadow_scholar/app/hello_world/res/
--rw-r--r--   0 lucas      (502) staff       (20)   151710 2023-03-09 19:05:25.000000 shadow-scholar-0.6.0/src/shadow_scholar/app/hello_world/res/logo.png
--rw-r--r--   0 lucas      (502) staff       (20)      252 2023-03-24 00:59:46.000000 shadow-scholar-0.6.0/src/shadow_scholar/app/hello_world/res/style.css
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-05-11 23:17:06.760510 shadow-scholar-0.6.0/src/shadow_scholar/app/llama/
--rw-r--r--   0 lucas      (502) staff       (20)        0 2023-03-02 18:48:43.000000 shadow-scholar-0.6.0/src/shadow_scholar/app/llama/__init__.py
--rw-r--r--   0 lucas      (502) staff       (20)    11621 2023-03-24 00:59:46.000000 shadow-scholar-0.6.0/src/shadow_scholar/app/llama/main.py
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-05-11 23:17:06.761786 shadow-scholar-0.6.0/src/shadow_scholar/app/pdod/
--rw-r--r--   0 lucas      (502) staff       (20)        0 2023-04-17 02:25:19.000000 shadow-scholar-0.6.0/src/shadow_scholar/app/pdod/__init__.py
--rw-r--r--   0 lucas      (502) staff       (20)     1051 2023-05-11 23:16:57.000000 shadow-scholar-0.6.0/src/shadow_scholar/app/pdod/caches.py
--rw-r--r--   0 lucas      (502) staff       (20)     5099 2023-04-17 02:25:19.000000 shadow-scholar-0.6.0/src/shadow_scholar/app/pdod/datasets.py
--rw-r--r--   0 lucas      (502) staff       (20)     5524 2023-04-17 02:25:19.000000 shadow-scholar-0.6.0/src/shadow_scholar/app/pdod/main.py
--rw-r--r--   0 lucas      (502) staff       (20)     2454 2023-04-17 02:25:19.000000 shadow-scholar-0.6.0/src/shadow_scholar/app/pdod/mmda_utils.py
--rw-r--r--   0 lucas      (502) staff       (20)     7874 2023-04-17 02:25:19.000000 shadow-scholar-0.6.0/src/shadow_scholar/app/pdod/rankers.py
--rw-r--r--   0 lucas      (502) staff       (20)     1342 2023-04-17 02:25:19.000000 shadow-scholar-0.6.0/src/shadow_scholar/app/pdod/reg_utils.py
--rw-r--r--   0 lucas      (502) staff       (20)     2804 2023-04-17 02:25:19.000000 shadow-scholar-0.6.0/src/shadow_scholar/app/pdod/slicers.py
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-05-11 23:17:06.762188 shadow-scholar-0.6.0/src/shadow_scholar/app/qa/
--rw-r--r--   0 lucas      (502) staff       (20)        0 2023-02-14 02:56:52.000000 shadow-scholar-0.6.0/src/shadow_scholar/app/qa/__init__.py
--rw-r--r--   0 lucas      (502) staff       (20)     7112 2023-04-03 06:48:20.000000 shadow-scholar-0.6.0/src/shadow_scholar/app/qa/data.py
--rw-r--r--   0 lucas      (502) staff       (20)     7014 2023-03-21 21:27:24.000000 shadow-scholar-0.6.0/src/shadow_scholar/app/qa/main.py
--rw-r--r--   0 lucas      (502) staff       (20)    16138 2023-05-11 23:16:57.000000 shadow-scholar-0.6.0/src/shadow_scholar/cli.py
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-05-11 23:17:06.762458 shadow-scholar-0.6.0/src/shadow_scholar/collections/
--rw-r--r--   0 lucas      (502) staff       (20)        0 2023-02-14 02:56:52.000000 shadow-scholar-0.6.0/src/shadow_scholar/collections/__init__.py
--rw-r--r--   0 lucas      (502) staff       (20)     5254 2023-05-11 23:16:57.000000 shadow-scholar-0.6.0/src/shadow_scholar/collections/athena.py
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-05-11 23:17:06.766291 shadow-scholar-0.6.0/src/shadow_scholar/collections/queries/
--rw-r--r--   0 lucas      (502) staff       (20)     1177 2023-03-24 00:59:46.000000 shadow-scholar-0.6.0/src/shadow_scholar/collections/queries/acl_anthology.sql
--rw-r--r--   0 lucas      (502) staff       (20)     3419 2023-02-14 02:56:52.000000 shadow-scholar-0.6.0/src/shadow_scholar/collections/queries/s2ag_abstracts.sql
--rw-r--r--   0 lucas      (502) staff       (20)      980 2023-02-14 02:56:52.000000 shadow-scholar-0.6.0/src/shadow_scholar/collections/queries/s2ag_authors.sql
--rw-r--r--   0 lucas      (502) staff       (20)      690 2023-02-14 02:56:52.000000 shadow-scholar-0.6.0/src/shadow_scholar/collections/queries/s2ag_citations.sql
--rw-r--r--   0 lucas      (502) staff       (20)      348 2023-02-14 02:56:52.000000 shadow-scholar-0.6.0/src/shadow_scholar/collections/queries/s2ag_embeddings.sql
--rw-r--r--   0 lucas      (502) staff       (20)      239 2023-02-14 02:56:52.000000 shadow-scholar-0.6.0/src/shadow_scholar/collections/queries/s2ag_paper_ids.sql
--rw-r--r--   0 lucas      (502) staff       (20)     3256 2023-02-14 02:56:52.000000 shadow-scholar-0.6.0/src/shadow_scholar/collections/queries/s2ag_papers.sql
--rw-r--r--   0 lucas      (502) staff       (20)      431 2023-02-14 02:56:52.000000 shadow-scholar-0.6.0/src/shadow_scholar/collections/queries/s2ag_publication_venues.sql
--rw-r--r--   0 lucas      (502) staff       (20)     4581 2023-02-14 02:56:52.000000 shadow-scholar-0.6.0/src/shadow_scholar/collections/queries/s2ag_s2orc.sql
--rw-r--r--   0 lucas      (502) staff       (20)      203 2023-02-14 02:56:52.000000 shadow-scholar-0.6.0/src/shadow_scholar/collections/queries/s2ag_tldrs.sql
--rw-r--r--   0 lucas      (502) staff       (20)      637 2023-05-11 23:16:57.000000 shadow-scholar-0.6.0/src/shadow_scholar/hello_world.py
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-05-11 23:17:06.766929 shadow-scholar-0.6.0/src/shadow_scholar/util/
--rw-r--r--   0 lucas      (502) staff       (20)        0 2023-05-11 23:16:57.000000 shadow-scholar-0.6.0/src/shadow_scholar/util/__init__.py
--rw-r--r--   0 lucas      (502) staff       (20)     1134 2023-05-11 23:16:57.000000 shadow-scholar-0.6.0/src/shadow_scholar/util/s2_api.py
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-05-11 23:17:06.753371 shadow-scholar-0.6.0/src/shadow_scholar.egg-info/
--rw-r--r--   0 lucas      (502) staff       (20)     6263 2023-05-11 23:17:06.000000 shadow-scholar-0.6.0/src/shadow_scholar.egg-info/PKG-INFO
--rw-r--r--   0 lucas      (502) staff       (20)     2697 2023-05-11 23:17:06.000000 shadow-scholar-0.6.0/src/shadow_scholar.egg-info/SOURCES.txt
--rw-r--r--   0 lucas      (502) staff       (20)        1 2023-05-11 23:17:06.000000 shadow-scholar-0.6.0/src/shadow_scholar.egg-info/dependency_links.txt
--rw-r--r--   0 lucas      (502) staff       (20)       50 2023-05-11 23:17:06.000000 shadow-scholar-0.6.0/src/shadow_scholar.egg-info/entry_points.txt
--rw-r--r--   0 lucas      (502) staff       (20)      238 2023-05-11 23:17:06.000000 shadow-scholar-0.6.0/src/shadow_scholar.egg-info/requires.txt
--rw-r--r--   0 lucas      (502) staff       (20)       15 2023-05-11 23:17:06.000000 shadow-scholar-0.6.0/src/shadow_scholar.egg-info/top_level.txt
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-05-11 23:17:06.767254 shadow-scholar-0.6.0/tests/
--rw-r--r--   0 lucas      (502) staff       (20)      354 2023-02-14 02:56:52.000000 shadow-scholar-0.6.0/tests/test_imports.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-06-08 23:20:32.096571 shadow-scholar-0.6.1/
+-rw-r--r--   0 lucas      (502) staff       (20)    11357 2023-01-30 22:02:35.000000 shadow-scholar-0.6.1/LICENSE
+-rw-r--r--   0 lucas      (502) staff       (20)      106 2023-04-11 19:13:05.000000 shadow-scholar-0.6.1/MANIFEST.in
+-rw-r--r--   0 lucas      (502) staff       (20)     6263 2023-06-08 23:20:32.096443 shadow-scholar-0.6.1/PKG-INFO
+-rw-r--r--   0 lucas      (502) staff       (20)     5651 2023-05-11 23:16:57.000000 shadow-scholar-0.6.1/README.md
+-rw-r--r--   0 lucas      (502) staff       (20)     2028 2023-06-08 23:15:53.000000 shadow-scholar-0.6.1/pyproject.toml
+-rw-r--r--   0 lucas      (502) staff       (20)       38 2023-06-08 23:20:32.096617 shadow-scholar-0.6.1/setup.cfg
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-06-08 23:20:32.076287 shadow-scholar-0.6.1/src/
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-06-08 23:20:32.084561 shadow-scholar-0.6.1/src/shadow_scholar/
+-rw-r--r--   0 lucas      (502) staff       (20)      604 2023-05-11 23:16:57.000000 shadow-scholar-0.6.1/src/shadow_scholar/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)       59 2023-03-03 22:16:56.000000 shadow-scholar-0.6.1/src/shadow_scholar/__main__.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-06-08 23:20:32.086808 shadow-scholar-0.6.1/src/shadow_scholar/app/
+-rw-r--r--   0 lucas      (502) staff       (20)        0 2023-02-14 02:56:52.000000 shadow-scholar-0.6.1/src/shadow_scholar/app/__init__.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-06-08 23:20:32.087954 shadow-scholar-0.6.1/src/shadow_scholar/app/chat_s2/
+-rw-r--r--   0 lucas      (502) staff       (20)        0 2023-03-02 18:48:43.000000 shadow-scholar-0.6.1/src/shadow_scholar/app/chat_s2/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)     8837 2023-05-11 23:15:29.000000 shadow-scholar-0.6.1/src/shadow_scholar/app/chat_s2/library.py
+-rw-r--r--   0 lucas      (502) staff       (20)     6656 2023-05-11 22:13:47.000000 shadow-scholar-0.6.1/src/shadow_scholar/app/chat_s2/llm.py
+-rw-r--r--   0 lucas      (502) staff       (20)     1995 2023-04-11 19:13:05.000000 shadow-scholar-0.6.1/src/shadow_scholar/app/chat_s2/logging.py
+-rw-r--r--   0 lucas      (502) staff       (20)    19018 2023-05-11 22:13:47.000000 shadow-scholar-0.6.1/src/shadow_scholar/app/chat_s2/main.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-06-08 23:20:32.088226 shadow-scholar-0.6.1/src/shadow_scholar/app/chat_s2/res/
+-rw-r--r--   0 lucas      (502) staff       (20)     4871 2023-03-24 00:59:46.000000 shadow-scholar-0.6.1/src/shadow_scholar/app/chat_s2/res/logo.svg
+-rw-r--r--   0 lucas      (502) staff       (20)      960 2023-04-11 19:13:05.000000 shadow-scholar-0.6.1/src/shadow_scholar/app/chat_s2/res/style.css
+-rw-r--r--   0 lucas      (502) staff       (20)     6153 2023-05-11 22:13:47.000000 shadow-scholar-0.6.1/src/shadow_scholar/app/chat_s2/search.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-06-08 23:20:32.091433 shadow-scholar-0.6.1/src/shadow_scholar/app/galactica/
+-rw-r--r--   0 lucas      (502) staff       (20)        0 2023-02-23 21:23:12.000000 shadow-scholar-0.6.1/src/shadow_scholar/app/galactica/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)     8596 2023-02-23 21:23:12.000000 shadow-scholar-0.6.1/src/shadow_scholar/app/galactica/_old.py
+-rw-r--r--   0 lucas      (502) staff       (20)     9251 2023-02-23 21:23:12.000000 shadow-scholar-0.6.1/src/shadow_scholar/app/galactica/constants.py
+-rw-r--r--   0 lucas      (502) staff       (20)     8755 2023-03-03 21:48:10.000000 shadow-scholar-0.6.1/src/shadow_scholar/app/galactica/convert_to_int8.py
+-rw-r--r--   0 lucas      (502) staff       (20)  1290127 2023-02-23 21:23:12.000000 shadow-scholar-0.6.1/src/shadow_scholar/app/galactica/example.png
+-rw-r--r--   0 lucas      (502) staff       (20)    16518 2023-04-03 06:48:20.000000 shadow-scholar-0.6.1/src/shadow_scholar/app/galactica/galai_model.py
+-rw-r--r--   0 lucas      (502) staff       (20)     1490 2023-02-23 21:23:12.000000 shadow-scholar-0.6.1/src/shadow_scholar/app/galactica/galai_parallel_policy.py
+-rw-r--r--   0 lucas      (502) staff       (20)     5433 2023-02-23 21:23:12.000000 shadow-scholar-0.6.1/src/shadow_scholar/app/galactica/galai_utils.py
+-rw-r--r--   0 lucas      (502) staff       (20)     9211 2023-03-24 00:59:46.000000 shadow-scholar-0.6.1/src/shadow_scholar/app/galactica/main.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-06-08 23:20:32.091785 shadow-scholar-0.6.1/src/shadow_scholar/app/hello_world/
+-rw-r--r--   0 lucas      (502) staff       (20)        0 2023-03-03 22:16:55.000000 shadow-scholar-0.6.1/src/shadow_scholar/app/hello_world/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)        0 2023-03-09 19:05:25.000000 shadow-scholar-0.6.1/src/shadow_scholar/app/hello_world/gradio.css
+-rw-r--r--   0 lucas      (502) staff       (20)     1622 2023-05-11 23:19:36.000000 shadow-scholar-0.6.1/src/shadow_scholar/app/hello_world/main.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-06-08 23:20:32.092485 shadow-scholar-0.6.1/src/shadow_scholar/app/hello_world/res/
+-rw-r--r--   0 lucas      (502) staff       (20)   151710 2023-03-09 19:05:25.000000 shadow-scholar-0.6.1/src/shadow_scholar/app/hello_world/res/logo.png
+-rw-r--r--   0 lucas      (502) staff       (20)      252 2023-03-24 00:59:46.000000 shadow-scholar-0.6.1/src/shadow_scholar/app/hello_world/res/style.css
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-06-08 23:20:32.092720 shadow-scholar-0.6.1/src/shadow_scholar/app/llama/
+-rw-r--r--   0 lucas      (502) staff       (20)        0 2023-03-02 18:48:43.000000 shadow-scholar-0.6.1/src/shadow_scholar/app/llama/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)    11621 2023-03-24 00:59:46.000000 shadow-scholar-0.6.1/src/shadow_scholar/app/llama/main.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-06-08 23:20:32.093750 shadow-scholar-0.6.1/src/shadow_scholar/app/pdod/
+-rw-r--r--   0 lucas      (502) staff       (20)        0 2023-04-17 02:25:19.000000 shadow-scholar-0.6.1/src/shadow_scholar/app/pdod/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)     1051 2023-05-11 23:16:57.000000 shadow-scholar-0.6.1/src/shadow_scholar/app/pdod/caches.py
+-rw-r--r--   0 lucas      (502) staff       (20)     5099 2023-04-17 02:25:19.000000 shadow-scholar-0.6.1/src/shadow_scholar/app/pdod/datasets.py
+-rw-r--r--   0 lucas      (502) staff       (20)     5524 2023-04-17 02:25:19.000000 shadow-scholar-0.6.1/src/shadow_scholar/app/pdod/main.py
+-rw-r--r--   0 lucas      (502) staff       (20)     2454 2023-04-17 02:25:19.000000 shadow-scholar-0.6.1/src/shadow_scholar/app/pdod/mmda_utils.py
+-rw-r--r--   0 lucas      (502) staff       (20)     7874 2023-04-17 02:25:19.000000 shadow-scholar-0.6.1/src/shadow_scholar/app/pdod/rankers.py
+-rw-r--r--   0 lucas      (502) staff       (20)     1342 2023-04-17 02:25:19.000000 shadow-scholar-0.6.1/src/shadow_scholar/app/pdod/reg_utils.py
+-rw-r--r--   0 lucas      (502) staff       (20)     2804 2023-04-17 02:25:19.000000 shadow-scholar-0.6.1/src/shadow_scholar/app/pdod/slicers.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-06-08 23:20:32.094162 shadow-scholar-0.6.1/src/shadow_scholar/app/qa/
+-rw-r--r--   0 lucas      (502) staff       (20)        0 2023-02-14 02:56:52.000000 shadow-scholar-0.6.1/src/shadow_scholar/app/qa/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)     7112 2023-04-03 06:48:20.000000 shadow-scholar-0.6.1/src/shadow_scholar/app/qa/data.py
+-rw-r--r--   0 lucas      (502) staff       (20)     7014 2023-03-21 21:27:24.000000 shadow-scholar-0.6.1/src/shadow_scholar/app/qa/main.py
+-rw-r--r--   0 lucas      (502) staff       (20)    16138 2023-05-11 23:21:30.000000 shadow-scholar-0.6.1/src/shadow_scholar/cli.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-06-08 23:20:32.094398 shadow-scholar-0.6.1/src/shadow_scholar/collections/
+-rw-r--r--   0 lucas      (502) staff       (20)        0 2023-02-14 02:56:52.000000 shadow-scholar-0.6.1/src/shadow_scholar/collections/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)     5254 2023-05-11 23:16:57.000000 shadow-scholar-0.6.1/src/shadow_scholar/collections/athena.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-06-08 23:20:32.095750 shadow-scholar-0.6.1/src/shadow_scholar/collections/queries/
+-rw-r--r--   0 lucas      (502) staff       (20)     1177 2023-03-24 00:59:46.000000 shadow-scholar-0.6.1/src/shadow_scholar/collections/queries/acl_anthology.sql
+-rw-r--r--   0 lucas      (502) staff       (20)     3419 2023-02-14 02:56:52.000000 shadow-scholar-0.6.1/src/shadow_scholar/collections/queries/s2ag_abstracts.sql
+-rw-r--r--   0 lucas      (502) staff       (20)      980 2023-02-14 02:56:52.000000 shadow-scholar-0.6.1/src/shadow_scholar/collections/queries/s2ag_authors.sql
+-rw-r--r--   0 lucas      (502) staff       (20)      690 2023-02-14 02:56:52.000000 shadow-scholar-0.6.1/src/shadow_scholar/collections/queries/s2ag_citations.sql
+-rw-r--r--   0 lucas      (502) staff       (20)      348 2023-02-14 02:56:52.000000 shadow-scholar-0.6.1/src/shadow_scholar/collections/queries/s2ag_embeddings.sql
+-rw-r--r--   0 lucas      (502) staff       (20)      239 2023-02-14 02:56:52.000000 shadow-scholar-0.6.1/src/shadow_scholar/collections/queries/s2ag_paper_ids.sql
+-rw-r--r--   0 lucas      (502) staff       (20)     3256 2023-02-14 02:56:52.000000 shadow-scholar-0.6.1/src/shadow_scholar/collections/queries/s2ag_papers.sql
+-rw-r--r--   0 lucas      (502) staff       (20)      431 2023-02-14 02:56:52.000000 shadow-scholar-0.6.1/src/shadow_scholar/collections/queries/s2ag_publication_venues.sql
+-rw-r--r--   0 lucas      (502) staff       (20)     4581 2023-02-14 02:56:52.000000 shadow-scholar-0.6.1/src/shadow_scholar/collections/queries/s2ag_s2orc.sql
+-rw-r--r--   0 lucas      (502) staff       (20)      203 2023-02-14 02:56:52.000000 shadow-scholar-0.6.1/src/shadow_scholar/collections/queries/s2ag_tldrs.sql
+-rw-r--r--   0 lucas      (502) staff       (20)      637 2023-05-11 23:16:57.000000 shadow-scholar-0.6.1/src/shadow_scholar/hello_world.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-06-08 23:20:32.095987 shadow-scholar-0.6.1/src/shadow_scholar/util/
+-rw-r--r--   0 lucas      (502) staff       (20)        0 2023-05-11 23:16:57.000000 shadow-scholar-0.6.1/src/shadow_scholar/util/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)     1134 2023-05-11 23:16:57.000000 shadow-scholar-0.6.1/src/shadow_scholar/util/s2_api.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-06-08 23:20:32.086694 shadow-scholar-0.6.1/src/shadow_scholar.egg-info/
+-rw-r--r--   0 lucas      (502) staff       (20)     6263 2023-06-08 23:20:32.000000 shadow-scholar-0.6.1/src/shadow_scholar.egg-info/PKG-INFO
+-rw-r--r--   0 lucas      (502) staff       (20)     2697 2023-06-08 23:20:32.000000 shadow-scholar-0.6.1/src/shadow_scholar.egg-info/SOURCES.txt
+-rw-r--r--   0 lucas      (502) staff       (20)        1 2023-06-08 23:20:32.000000 shadow-scholar-0.6.1/src/shadow_scholar.egg-info/dependency_links.txt
+-rw-r--r--   0 lucas      (502) staff       (20)       50 2023-06-08 23:20:32.000000 shadow-scholar-0.6.1/src/shadow_scholar.egg-info/entry_points.txt
+-rw-r--r--   0 lucas      (502) staff       (20)      238 2023-06-08 23:20:32.000000 shadow-scholar-0.6.1/src/shadow_scholar.egg-info/requires.txt
+-rw-r--r--   0 lucas      (502) staff       (20)       15 2023-06-08 23:20:32.000000 shadow-scholar-0.6.1/src/shadow_scholar.egg-info/top_level.txt
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-06-08 23:20:32.096135 shadow-scholar-0.6.1/tests/
+-rw-r--r--   0 lucas      (502) staff       (20)      354 2023-02-14 02:56:52.000000 shadow-scholar-0.6.1/tests/test_imports.py
```

### Comparing `shadow-scholar-0.6.0/LICENSE` & `shadow-scholar-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `shadow-scholar-0.6.0/PKG-INFO` & `shadow-scholar-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shadow-scholar
-Version: 0.6.0
+Version: 0.6.1
 Summary: 🎓🕶️ A collection of utilities and demos from the Semantic Scholar Research Team 🕶️🎓
 Author-email: Luca Soldaini <lucas@allenai.org>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/allenai/shadow-scholar
 Project-URL: Source, https://github.com/allenai/shadow-scholar
 Project-URL: Tracker, https://github.com/allenai/shadow-scholar/issues
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `shadow-scholar-0.6.0/README.md` & `shadow-scholar-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `shadow-scholar-0.6.0/pyproject.toml` & `shadow-scholar-0.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "shadow-scholar"
-version = "0.6.0"
+version = "0.6.1"
 description = "🎓🕶️ A collection of utilities and demos from the Semantic Scholar Research Team 🕶️🎓"
 authors = [
     {name = "Luca Soldaini", email = "lucas@allenai.org" }
 ]
 license = {text = "Apache-2.0"}
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `shadow-scholar-0.6.0/src/shadow_scholar/__init__.py` & `shadow-scholar-0.6.1/src/shadow_scholar/__init__.py`

 * *Files identical despite different names*

### Comparing `shadow-scholar-0.6.0/src/shadow_scholar/app/chat_s2/library.py` & `shadow-scholar-0.6.1/src/shadow_scholar/app/chat_s2/library.py`

 * *Files identical despite different names*

### Comparing `shadow-scholar-0.6.0/src/shadow_scholar/app/chat_s2/llm.py` & `shadow-scholar-0.6.1/src/shadow_scholar/app/chat_s2/llm.py`

 * *Files identical despite different names*

### Comparing `shadow-scholar-0.6.0/src/shadow_scholar/app/chat_s2/logging.py` & `shadow-scholar-0.6.1/src/shadow_scholar/app/chat_s2/logging.py`

 * *Files identical despite different names*

### Comparing `shadow-scholar-0.6.0/src/shadow_scholar/app/chat_s2/main.py` & `shadow-scholar-0.6.1/src/shadow_scholar/app/chat_s2/main.py`

 * *Files identical despite different names*

### Comparing `shadow-scholar-0.6.0/src/shadow_scholar/app/chat_s2/res/logo.svg` & `shadow-scholar-0.6.1/src/shadow_scholar/app/chat_s2/res/logo.svg`

 * *Files identical despite different names*

### Comparing `shadow-scholar-0.6.0/src/shadow_scholar/app/chat_s2/res/style.css` & `shadow-scholar-0.6.1/src/shadow_scholar/app/chat_s2/res/style.css`

 * *Files identical despite different names*

### Comparing `shadow-scholar-0.6.0/src/shadow_scholar/app/chat_s2/search.py` & `shadow-scholar-0.6.1/src/shadow_scholar/app/chat_s2/search.py`

 * *Files identical despite different names*

### Comparing `shadow-scholar-0.6.0/src/shadow_scholar/app/galactica/_old.py` & `shadow-scholar-0.6.1/src/shadow_scholar/app/galactica/_old.py`

 * *Files identical despite different names*

### Comparing `shadow-scholar-0.6.0/src/shadow_scholar/app/galactica/constants.py` & `shadow-scholar-0.6.1/src/shadow_scholar/app/galactica/constants.py`

 * *Files identical despite different names*

### Comparing `shadow-scholar-0.6.0/src/shadow_scholar/app/galactica/convert_to_int8.py` & `shadow-scholar-0.6.1/src/shadow_scholar/app/galactica/convert_to_int8.py`

 * *Files identical despite different names*

### Comparing `shadow-scholar-0.6.0/src/shadow_scholar/app/galactica/example.png` & `shadow-scholar-0.6.1/src/shadow_scholar/app/galactica/example.png`

 * *Files identical despite different names*

### Comparing `shadow-scholar-0.6.0/src/shadow_scholar/app/galactica/galai_model.py` & `shadow-scholar-0.6.1/src/shadow_scholar/app/galactica/galai_model.py`

 * *Files identical despite different names*

### Comparing `shadow-scholar-0.6.0/src/shadow_scholar/app/galactica/galai_parallel_policy.py` & `shadow-scholar-0.6.1/src/shadow_scholar/app/galactica/galai_parallel_policy.py`

 * *Files identical despite different names*

### Comparing `shadow-scholar-0.6.0/src/shadow_scholar/app/galactica/galai_utils.py` & `shadow-scholar-0.6.1/src/shadow_scholar/app/galactica/galai_utils.py`

 * *Files identical despite different names*

### Comparing `shadow-scholar-0.6.0/src/shadow_scholar/app/galactica/main.py` & `shadow-scholar-0.6.1/src/shadow_scholar/app/galactica/main.py`

 * *Files identical despite different names*

### Comparing `shadow-scholar-0.6.0/src/shadow_scholar/app/hello_world/main.py` & `shadow-scholar-0.6.1/src/shadow_scholar/app/hello_world/main.py`

 * *Files identical despite different names*

### Comparing `shadow-scholar-0.6.0/src/shadow_scholar/app/hello_world/res/logo.png` & `shadow-scholar-0.6.1/src/shadow_scholar/app/hello_world/res/logo.png`

 * *Files identical despite different names*

### Comparing `shadow-scholar-0.6.0/src/shadow_scholar/app/llama/main.py` & `shadow-scholar-0.6.1/src/shadow_scholar/app/llama/main.py`

 * *Files identical despite different names*

### Comparing `shadow-scholar-0.6.0/src/shadow_scholar/app/pdod/caches.py` & `shadow-scholar-0.6.1/src/shadow_scholar/app/pdod/caches.py`

 * *Files identical despite different names*

### Comparing `shadow-scholar-0.6.0/src/shadow_scholar/app/pdod/datasets.py` & `shadow-scholar-0.6.1/src/shadow_scholar/app/pdod/datasets.py`

 * *Files identical despite different names*

### Comparing `shadow-scholar-0.6.0/src/shadow_scholar/app/pdod/main.py` & `shadow-scholar-0.6.1/src/shadow_scholar/app/pdod/main.py`

 * *Files identical despite different names*

### Comparing `shadow-scholar-0.6.0/src/shadow_scholar/app/pdod/mmda_utils.py` & `shadow-scholar-0.6.1/src/shadow_scholar/app/pdod/mmda_utils.py`

 * *Files identical despite different names*

### Comparing `shadow-scholar-0.6.0/src/shadow_scholar/app/pdod/rankers.py` & `shadow-scholar-0.6.1/src/shadow_scholar/app/pdod/rankers.py`

 * *Files identical despite different names*

### Comparing `shadow-scholar-0.6.0/src/shadow_scholar/app/pdod/reg_utils.py` & `shadow-scholar-0.6.1/src/shadow_scholar/app/pdod/reg_utils.py`

 * *Files identical despite different names*

### Comparing `shadow-scholar-0.6.0/src/shadow_scholar/app/pdod/slicers.py` & `shadow-scholar-0.6.1/src/shadow_scholar/app/pdod/slicers.py`

 * *Files identical despite different names*

### Comparing `shadow-scholar-0.6.0/src/shadow_scholar/app/qa/data.py` & `shadow-scholar-0.6.1/src/shadow_scholar/app/qa/data.py`

 * *Files identical despite different names*

### Comparing `shadow-scholar-0.6.0/src/shadow_scholar/app/qa/main.py` & `shadow-scholar-0.6.1/src/shadow_scholar/app/qa/main.py`

 * *Files identical despite different names*

### Comparing `shadow-scholar-0.6.0/src/shadow_scholar/cli.py` & `shadow-scholar-0.6.1/src/shadow_scholar/cli.py`

 * *Files identical despite different names*

### Comparing `shadow-scholar-0.6.0/src/shadow_scholar/collections/athena.py` & `shadow-scholar-0.6.1/src/shadow_scholar/collections/athena.py`

 * *Files identical despite different names*

### Comparing `shadow-scholar-0.6.0/src/shadow_scholar/collections/queries/acl_anthology.sql` & `shadow-scholar-0.6.1/src/shadow_scholar/collections/queries/acl_anthology.sql`

 * *Files identical despite different names*

### Comparing `shadow-scholar-0.6.0/src/shadow_scholar/collections/queries/s2ag_abstracts.sql` & `shadow-scholar-0.6.1/src/shadow_scholar/collections/queries/s2ag_abstracts.sql`

 * *Files identical despite different names*

### Comparing `shadow-scholar-0.6.0/src/shadow_scholar/collections/queries/s2ag_authors.sql` & `shadow-scholar-0.6.1/src/shadow_scholar/collections/queries/s2ag_authors.sql`

 * *Files identical despite different names*

### Comparing `shadow-scholar-0.6.0/src/shadow_scholar/collections/queries/s2ag_citations.sql` & `shadow-scholar-0.6.1/src/shadow_scholar/collections/queries/s2ag_citations.sql`

 * *Files identical despite different names*

### Comparing `shadow-scholar-0.6.0/src/shadow_scholar/collections/queries/s2ag_papers.sql` & `shadow-scholar-0.6.1/src/shadow_scholar/collections/queries/s2ag_papers.sql`

 * *Files identical despite different names*

### Comparing `shadow-scholar-0.6.0/src/shadow_scholar/collections/queries/s2ag_s2orc.sql` & `shadow-scholar-0.6.1/src/shadow_scholar/collections/queries/s2ag_s2orc.sql`

 * *Files identical despite different names*

### Comparing `shadow-scholar-0.6.0/src/shadow_scholar/hello_world.py` & `shadow-scholar-0.6.1/src/shadow_scholar/hello_world.py`

 * *Files identical despite different names*

### Comparing `shadow-scholar-0.6.0/src/shadow_scholar/util/s2_api.py` & `shadow-scholar-0.6.1/src/shadow_scholar/util/s2_api.py`

 * *Files identical despite different names*

### Comparing `shadow-scholar-0.6.0/src/shadow_scholar.egg-info/PKG-INFO` & `shadow-scholar-0.6.1/src/shadow_scholar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shadow-scholar
-Version: 0.6.0
+Version: 0.6.1
 Summary: 🎓🕶️ A collection of utilities and demos from the Semantic Scholar Research Team 🕶️🎓
 Author-email: Luca Soldaini <lucas@allenai.org>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/allenai/shadow-scholar
 Project-URL: Source, https://github.com/allenai/shadow-scholar
 Project-URL: Tracker, https://github.com/allenai/shadow-scholar/issues
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `shadow-scholar-0.6.0/src/shadow_scholar.egg-info/SOURCES.txt` & `shadow-scholar-0.6.1/src/shadow_scholar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

