# Comparing `tmp/gbpcli-1.4.0.tar.gz` & `tmp/gbpcli-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gbpcli-1.4.0.tar", last modified: Fri Feb  3 03:37:57 2023, max compression
+gzip compressed data, was "gbpcli-1.5.0.tar", last modified: Thu Jun  8 23:06:32 2023, max compression
```

## Comparing `gbpcli-1.4.0.tar` & `gbpcli-1.5.0.tar`

### file list

```diff
@@ -1,81 +1,87 @@
--rw-r--r--   0 marduk    (1000) users      (100)      654 2023-01-31 12:56:34.446597 gbpcli-1.4.0/LICENSE
--rw-r--r--   0 marduk    (1000) users      (100)     3707 2023-02-03 03:32:50.164600 gbpcli-1.4.0/README.md
--rw-r--r--   0 marduk    (1000) users      (100)     1844 2023-01-20 04:06:43.084420 gbpcli-1.4.0/pyproject.toml
--rw-r--r--   0 marduk    (1000) users      (100)    14146 2023-02-02 13:25:30.249061 gbpcli-1.4.0/src/gbpcli/__init__.py
--rw-r--r--   0 marduk    (1000) users      (100)      108 2022-09-05 18:14:24.258925 gbpcli-1.4.0/src/gbpcli/__main__.py
--rw-r--r--   0 marduk    (1000) users      (100)        0 2022-09-05 18:14:24.258925 gbpcli-1.4.0/src/gbpcli/py.typed
--rw-r--r--   0 marduk    (1000) users      (100)      195 2023-01-02 21:58:07.125538 gbpcli-1.4.0/src/gbpcli/queries/build.graphql
--rw-r--r--   0 marduk    (1000) users      (100)      144 2022-10-04 22:58:21.349383 gbpcli-1.4.0/src/gbpcli/queries/builds.graphql
--rw-r--r--   0 marduk    (1000) users      (100)      215 2022-10-12 12:48:42.261841 gbpcli-1.4.0/src/gbpcli/queries/builds_with_packages.graphql
--rw-r--r--   0 marduk    (1000) users      (100)       90 2022-09-05 18:14:24.259925 gbpcli-1.4.0/src/gbpcli/queries/create_note.graphql
--rw-r--r--   0 marduk    (1000) users      (100)      256 2022-09-05 18:14:24.259925 gbpcli-1.4.0/src/gbpcli/queries/diff.graphql
--rw-r--r--   0 marduk    (1000) users      (100)       60 2022-09-05 18:14:24.259925 gbpcli-1.4.0/src/gbpcli/queries/keep_build.graphql
--rw-r--r--   0 marduk    (1000) users      (100)       71 2022-09-05 18:14:24.259925 gbpcli-1.4.0/src/gbpcli/queries/latest.graphql
--rw-r--r--   0 marduk    (1000) users      (100)       53 2022-09-05 18:14:24.259925 gbpcli-1.4.0/src/gbpcli/queries/logs.graphql
--rw-r--r--   0 marduk    (1000) users      (100)       39 2022-10-12 12:48:42.261841 gbpcli-1.4.0/src/gbpcli/queries/machine_names.graphql
--rw-r--r--   0 marduk    (1000) users      (100)      103 2022-10-03 11:17:00.242651 gbpcli-1.4.0/src/gbpcli/queries/machines.graphql
--rw-r--r--   0 marduk    (1000) users      (100)       57 2022-09-05 18:14:24.260925 gbpcli-1.4.0/src/gbpcli/queries/packages.graphql
--rw-r--r--   0 marduk    (1000) users      (100)       85 2022-09-05 18:14:24.260925 gbpcli-1.4.0/src/gbpcli/queries/publish.graphql
--rw-r--r--   0 marduk    (1000) users      (100)       61 2022-09-05 18:14:24.260925 gbpcli-1.4.0/src/gbpcli/queries/pull.graphql
--rw-r--r--   0 marduk    (1000) users      (100)       63 2022-09-05 18:14:24.260925 gbpcli-1.4.0/src/gbpcli/queries/release_build.graphql
--rw-r--r--   0 marduk    (1000) users      (100)      106 2022-09-05 18:14:24.261925 gbpcli-1.4.0/src/gbpcli/queries/resolve_tag.graphql
--rw-r--r--   0 marduk    (1000) users      (100)       68 2022-09-05 18:14:24.261925 gbpcli-1.4.0/src/gbpcli/queries/schedule_build.graphql
--rw-r--r--   0 marduk    (1000) users      (100)      211 2022-09-05 18:14:24.261925 gbpcli-1.4.0/src/gbpcli/queries/search_notes.graphql
--rw-r--r--   0 marduk    (1000) users      (100)       91 2022-09-05 18:14:24.261925 gbpcli-1.4.0/src/gbpcli/queries/tag_build.graphql
--rw-r--r--   0 marduk    (1000) users      (100)      110 2022-09-05 18:14:24.261925 gbpcli-1.4.0/src/gbpcli/queries/untag_build.graphql
--rw-r--r--   0 marduk    (1000) users      (100)        0 2022-09-05 18:14:24.261925 gbpcli-1.4.0/src/gbpcli/subcommands/__init__.py
--rw-r--r--   0 marduk    (1000) users      (100)      530 2023-01-20 12:56:54.675183 gbpcli-1.4.0/src/gbpcli/subcommands/build.py
--rw-r--r--   0 marduk    (1000) users      (100)     3088 2023-01-20 12:56:54.675183 gbpcli-1.4.0/src/gbpcli/subcommands/diff.py
--rw-r--r--   0 marduk    (1000) users      (100)     3862 2023-01-20 12:56:54.675183 gbpcli-1.4.0/src/gbpcli/subcommands/inspect.py
--rw-r--r--   0 marduk    (1000) users      (100)      880 2023-01-20 12:56:54.675183 gbpcli-1.4.0/src/gbpcli/subcommands/keep.py
--rw-r--r--   0 marduk    (1000) users      (100)      692 2023-01-20 12:56:54.675183 gbpcli-1.4.0/src/gbpcli/subcommands/latest.py
--rw-r--r--   0 marduk    (1000) users      (100)     2094 2023-01-20 12:56:54.675183 gbpcli-1.4.0/src/gbpcli/subcommands/list.py
--rw-r--r--   0 marduk    (1000) users      (100)      787 2023-01-20 12:56:54.675183 gbpcli-1.4.0/src/gbpcli/subcommands/logs.py
--rw-r--r--   0 marduk    (1000) users      (100)     1621 2023-01-20 12:56:54.675183 gbpcli-1.4.0/src/gbpcli/subcommands/machines.py
--rw-r--r--   0 marduk    (1000) users      (100)     3227 2023-01-20 12:56:54.675183 gbpcli-1.4.0/src/gbpcli/subcommands/notes.py
--rw-r--r--   0 marduk    (1000) users      (100)      840 2023-01-20 12:56:54.675183 gbpcli-1.4.0/src/gbpcli/subcommands/packages.py
--rw-r--r--   0 marduk    (1000) users      (100)      745 2023-01-20 12:56:54.675183 gbpcli-1.4.0/src/gbpcli/subcommands/publish.py
--rw-r--r--   0 marduk    (1000) users      (100)      603 2023-01-20 12:56:54.675183 gbpcli-1.4.0/src/gbpcli/subcommands/pull.py
--rw-r--r--   0 marduk    (1000) users      (100)     2576 2023-01-20 12:56:54.675183 gbpcli-1.4.0/src/gbpcli/subcommands/status.py
--rw-r--r--   0 marduk    (1000) users      (100)     1250 2023-01-20 12:56:54.675183 gbpcli-1.4.0/src/gbpcli/subcommands/tag.py
--rw-r--r--   0 marduk    (1000) users      (100)     4039 2023-01-20 12:56:54.675183 gbpcli-1.4.0/src/gbpcli/utils.py
--rw-r--r--   0 marduk    (1000) users      (100)     4026 2023-01-31 13:08:29.756420 gbpcli-1.4.0/tests/__init__.py
--rw-r--r--   0 marduk    (1000) users      (100)       51 2021-11-09 18:24:04.826960 gbpcli-1.4.0/tests/data/create_note.json
--rw-r--r--   0 marduk    (1000) users      (100)     1770 2022-10-03 14:06:49.960295 gbpcli-1.4.0/tests/data/diff.json
--rw-r--r--   0 marduk    (1000) users      (100)      405 2022-02-15 12:17:15.614583 gbpcli-1.4.0/tests/data/diff_no_content.json
--rw-r--r--   0 marduk    (1000) users      (100)    10329 2022-10-12 12:48:42.261841 gbpcli-1.4.0/tests/data/inspect.ndjson
--rw-r--r--   0 marduk    (1000) users      (100)       76 2021-11-09 18:24:04.826960 gbpcli-1.4.0/tests/data/keep_build.json
--rw-r--r--   0 marduk    (1000) users      (100)       84 2022-02-15 12:17:42.117647 gbpcli-1.4.0/tests/data/latest.json
--rw-r--r--   0 marduk    (1000) users      (100)      355 2023-01-03 00:09:05.307268 gbpcli-1.4.0/tests/data/lighthouse.12672.json
--rw-r--r--   0 marduk    (1000) users      (100)    16680 2022-10-03 14:06:49.960295 gbpcli-1.4.0/tests/data/list.json
--rw-r--r--   0 marduk    (1000) users      (100)    12865 2022-08-09 01:32:16.919583 gbpcli-1.4.0/tests/data/list_with_packages.json
--rw-r--r--   0 marduk    (1000) users      (100)       85 2021-10-11 10:44:26.503390 gbpcli-1.4.0/tests/data/logs.json
--rw-r--r--   0 marduk    (1000) users      (100)     1499 2022-10-03 12:25:21.908033 gbpcli-1.4.0/tests/data/machines.json
--rw-r--r--   0 marduk    (1000) users      (100)    11936 2021-11-20 13:43:30.858627 gbpcli-1.4.0/tests/data/packages.json
--rw-r--r--   0 marduk    (1000) users      (100)     6959 2021-11-09 18:24:04.826960 gbpcli-1.4.0/tests/data/packages.txt
--rw-r--r--   0 marduk    (1000) users      (100)      129 2022-02-15 12:18:55.829810 gbpcli-1.4.0/tests/data/publish.json
--rw-r--r--   0 marduk    (1000) users      (100)       77 2021-11-09 18:24:04.826960 gbpcli-1.4.0/tests/data/pull.json
--rw-r--r--   0 marduk    (1000) users      (100)       80 2021-11-09 18:24:04.826960 gbpcli-1.4.0/tests/data/release_build.json
--rw-r--r--   0 marduk    (1000) users      (100)       83 2021-10-11 10:44:26.504390 gbpcli-1.4.0/tests/data/schedule_build.json
--rw-r--r--   0 marduk    (1000) users      (100)      798 2022-08-08 04:05:57.003949 gbpcli-1.4.0/tests/data/search_notes.json
--rw-r--r--   0 marduk    (1000) users      (100)      584 2022-10-03 00:09:10.558796 gbpcli-1.4.0/tests/data/status.json
--rw-r--r--   0 marduk    (1000) users      (100)       89 2022-08-08 03:06:02.871203 gbpcli-1.4.0/tests/data/tag_build.json
--rw-r--r--   0 marduk    (1000) users      (100)       89 2022-08-08 03:09:13.886678 gbpcli-1.4.0/tests/data/untag_build.json
--rw-r--r--   0 marduk    (1000) users      (100)      626 2023-01-20 12:56:54.675183 gbpcli-1.4.0/tests/test_build.py
--rw-r--r--   0 marduk    (1000) users      (100)     4689 2023-01-20 12:56:54.675183 gbpcli-1.4.0/tests/test_diff.py
--rw-r--r--   0 marduk    (1000) users      (100)     2792 2023-01-20 12:56:54.675183 gbpcli-1.4.0/tests/test_entrypoint.py
--rw-r--r--   0 marduk    (1000) users      (100)     5769 2023-01-20 12:56:54.675183 gbpcli-1.4.0/tests/test_gbp.py
--rw-r--r--   0 marduk    (1000) users      (100)    11352 2023-01-20 12:56:54.675183 gbpcli-1.4.0/tests/test_inspect.py
--rw-r--r--   0 marduk    (1000) users      (100)     1692 2023-01-20 12:56:54.675183 gbpcli-1.4.0/tests/test_keep.py
--rw-r--r--   0 marduk    (1000) users      (100)     1120 2023-01-20 12:56:54.675183 gbpcli-1.4.0/tests/test_latest.py
--rw-r--r--   0 marduk    (1000) users      (100)     1995 2023-01-20 12:56:54.676184 gbpcli-1.4.0/tests/test_list.py
--rw-r--r--   0 marduk    (1000) users      (100)     1075 2023-01-20 12:56:54.676184 gbpcli-1.4.0/tests/test_logs.py
--rw-r--r--   0 marduk    (1000) users      (100)     2226 2023-01-20 12:56:54.676184 gbpcli-1.4.0/tests/test_machines.py
--rw-r--r--   0 marduk    (1000) users      (100)     5642 2023-01-20 12:56:54.676184 gbpcli-1.4.0/tests/test_notes.py
--rw-r--r--   0 marduk    (1000) users      (100)     1120 2023-01-20 12:56:54.676184 gbpcli-1.4.0/tests/test_packages.py
--rw-r--r--   0 marduk    (1000) users      (100)     1134 2023-01-20 12:56:54.676184 gbpcli-1.4.0/tests/test_publish.py
--rw-r--r--   0 marduk    (1000) users      (100)      615 2023-01-20 12:56:54.676184 gbpcli-1.4.0/tests/test_pull.py
--rw-r--r--   0 marduk    (1000) users      (100)     2647 2023-01-20 12:56:54.676184 gbpcli-1.4.0/tests/test_status.py
--rw-r--r--   0 marduk    (1000) users      (100)     1691 2023-01-20 12:56:54.676184 gbpcli-1.4.0/tests/test_tag.py
--rw-r--r--   0 marduk    (1000) users      (100)     5837 2023-01-20 12:56:54.676184 gbpcli-1.4.0/tests/test_utils.py
--rw-------   0 marduk    (1000) users      (100)     4327 2023-02-03 03:37:57.409634 gbpcli-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0      654 2023-02-25 13:20:56.364600 gbpcli-1.5.0/LICENSE
+-rw-r--r--   0        0        0     3707 2023-02-25 13:20:56.365600 gbpcli-1.5.0/README.md
+-rw-r--r--   0        0        0     1835 2023-06-08 23:06:32.073585 gbpcli-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0    11601 2023-06-04 23:31:11.836617 gbpcli-1.5.0/src/gbpcli/__init__.py
+-rw-r--r--   0        0        0      108 2022-09-05 18:14:24.258925 gbpcli-1.5.0/src/gbpcli/__main__.py
+-rw-r--r--   0        0        0     2369 2023-03-19 20:53:02.457971 gbpcli-1.5.0/src/gbpcli/graphql.py
+-rw-r--r--   0        0        0        0 2022-09-05 18:14:24.258925 gbpcli-1.5.0/src/gbpcli/py.typed
+-rw-r--r--   0        0        0      195 2023-01-02 21:58:07.125538 gbpcli-1.5.0/src/gbpcli/queries/build.graphql
+-rw-r--r--   0        0        0      144 2022-10-04 22:58:21.349383 gbpcli-1.5.0/src/gbpcli/queries/builds.graphql
+-rw-r--r--   0        0        0      215 2022-10-12 12:48:42.261841 gbpcli-1.5.0/src/gbpcli/queries/builds_with_packages.graphql
+-rw-r--r--   0        0        0       90 2022-09-05 18:14:24.259925 gbpcli-1.5.0/src/gbpcli/queries/create_note.graphql
+-rw-r--r--   0        0        0      256 2022-09-05 18:14:24.259925 gbpcli-1.5.0/src/gbpcli/queries/diff.graphql
+-rw-r--r--   0        0        0       60 2022-09-05 18:14:24.259925 gbpcli-1.5.0/src/gbpcli/queries/keep_build.graphql
+-rw-r--r--   0        0        0       71 2022-09-05 18:14:24.259925 gbpcli-1.5.0/src/gbpcli/queries/latest.graphql
+-rw-r--r--   0        0        0       53 2022-09-05 18:14:24.259925 gbpcli-1.5.0/src/gbpcli/queries/logs.graphql
+-rw-r--r--   0        0        0       39 2022-10-12 12:48:42.261841 gbpcli-1.5.0/src/gbpcli/queries/machine_names.graphql
+-rw-r--r--   0        0        0      103 2022-10-03 11:17:00.242651 gbpcli-1.5.0/src/gbpcli/queries/machines.graphql
+-rw-r--r--   0        0        0       57 2022-09-05 18:14:24.260925 gbpcli-1.5.0/src/gbpcli/queries/packages.graphql
+-rw-r--r--   0        0        0       85 2022-09-05 18:14:24.260925 gbpcli-1.5.0/src/gbpcli/queries/publish.graphql
+-rw-r--r--   0        0        0       61 2022-09-05 18:14:24.260925 gbpcli-1.5.0/src/gbpcli/queries/pull.graphql
+-rw-r--r--   0        0        0       63 2022-09-05 18:14:24.260925 gbpcli-1.5.0/src/gbpcli/queries/release_build.graphql
+-rw-r--r--   0        0        0      106 2022-09-05 18:14:24.261925 gbpcli-1.5.0/src/gbpcli/queries/resolve_tag.graphql
+-rw-r--r--   0        0        0       68 2022-09-05 18:14:24.261925 gbpcli-1.5.0/src/gbpcli/queries/schedule_build.graphql
+-rw-r--r--   0        0        0      252 2023-03-20 02:47:01.244810 gbpcli-1.5.0/src/gbpcli/queries/search.graphql
+-rw-r--r--   0        0        0       91 2022-09-05 18:14:24.261925 gbpcli-1.5.0/src/gbpcli/queries/tag_build.graphql
+-rw-r--r--   0        0        0      110 2022-09-05 18:14:24.261925 gbpcli-1.5.0/src/gbpcli/queries/untag_build.graphql
+-rw-r--r--   0        0        0     3707 2023-03-19 17:24:48.975558 gbpcli-1.5.0/src/gbpcli/render.py
+-rw-r--r--   0        0        0     1383 2023-06-04 16:18:21.948227 gbpcli-1.5.0/src/gbpcli/subcommands/__init__.py
+-rw-r--r--   0        0        0      456 2023-06-04 23:31:11.836617 gbpcli-1.5.0/src/gbpcli/subcommands/build.py
+-rw-r--r--   0        0        0     3021 2023-06-04 16:18:21.948227 gbpcli-1.5.0/src/gbpcli/subcommands/diff.py
+-rw-r--r--   0        0        0     3863 2023-06-04 16:18:21.948227 gbpcli-1.5.0/src/gbpcli/subcommands/inspect.py
+-rw-r--r--   0        0        0      790 2023-06-04 16:18:21.948227 gbpcli-1.5.0/src/gbpcli/subcommands/keep.py
+-rw-r--r--   0        0        0      622 2023-06-04 16:18:21.948227 gbpcli-1.5.0/src/gbpcli/subcommands/latest.py
+-rw-r--r--   0        0        0     1593 2023-06-04 16:18:21.948227 gbpcli-1.5.0/src/gbpcli/subcommands/list.py
+-rw-r--r--   0        0        0     1301 2023-06-04 16:18:21.948227 gbpcli-1.5.0/src/gbpcli/subcommands/logs.py
+-rw-r--r--   0        0        0     1561 2023-06-04 16:18:21.948227 gbpcli-1.5.0/src/gbpcli/subcommands/machines.py
+-rw-r--r--   0        0        0     2912 2023-06-04 16:18:21.948227 gbpcli-1.5.0/src/gbpcli/subcommands/notes.py
+-rw-r--r--   0        0        0      755 2023-06-04 16:18:21.948227 gbpcli-1.5.0/src/gbpcli/subcommands/packages.py
+-rw-r--r--   0        0        0      657 2023-06-04 16:18:21.948227 gbpcli-1.5.0/src/gbpcli/subcommands/publish.py
+-rw-r--r--   0        0        0      529 2023-06-04 16:18:21.948227 gbpcli-1.5.0/src/gbpcli/subcommands/pull.py
+-rw-r--r--   0        0        0     2567 2023-06-04 16:18:21.948227 gbpcli-1.5.0/src/gbpcli/subcommands/status.py
+-rw-r--r--   0        0        0     1178 2023-06-04 16:18:21.948227 gbpcli-1.5.0/src/gbpcli/subcommands/tag.py
+-rw-r--r--   0        0        0     1480 2023-02-28 03:19:35.708985 gbpcli-1.5.0/src/gbpcli/theme.py
+-rw-r--r--   0        0        0     1460 2023-05-06 15:20:54.186681 gbpcli-1.5.0/src/gbpcli/utils.py
+-rw-r--r--   0        0        0     4161 2023-06-04 16:18:21.949227 gbpcli-1.5.0/tests/__init__.py
+-rw-r--r--   0        0        0       51 2021-11-09 18:24:04.826960 gbpcli-1.5.0/tests/data/create_note.json
+-rw-r--r--   0        0        0     1770 2022-10-03 14:06:49.960295 gbpcli-1.5.0/tests/data/diff.json
+-rw-r--r--   0        0        0      405 2022-02-15 12:17:15.614583 gbpcli-1.5.0/tests/data/diff_no_content.json
+-rw-r--r--   0        0        0    10329 2022-10-12 12:48:42.261841 gbpcli-1.5.0/tests/data/inspect.ndjson
+-rw-r--r--   0        0        0       76 2021-11-09 18:24:04.826960 gbpcli-1.5.0/tests/data/keep_build.json
+-rw-r--r--   0        0        0       84 2022-02-15 12:17:42.117647 gbpcli-1.5.0/tests/data/latest.json
+-rw-r--r--   0        0        0      355 2023-01-03 00:09:05.307268 gbpcli-1.5.0/tests/data/lighthouse.12672.json
+-rw-r--r--   0        0        0    16680 2022-10-03 14:06:49.960295 gbpcli-1.5.0/tests/data/list.json
+-rw-r--r--   0        0        0    12865 2022-08-09 01:32:16.919583 gbpcli-1.5.0/tests/data/list_with_packages.json
+-rw-r--r--   0        0        0       85 2021-10-11 10:44:26.503390 gbpcli-1.5.0/tests/data/logs.json
+-rw-r--r--   0        0        0     1499 2022-10-03 12:25:21.908033 gbpcli-1.5.0/tests/data/machines.json
+-rw-r--r--   0        0        0    11936 2021-11-20 13:43:30.858627 gbpcli-1.5.0/tests/data/packages.json
+-rw-r--r--   0        0        0     6959 2021-11-09 18:24:04.826960 gbpcli-1.5.0/tests/data/packages.txt
+-rw-r--r--   0        0        0      129 2022-02-15 12:18:55.829810 gbpcli-1.5.0/tests/data/publish.json
+-rw-r--r--   0        0        0       77 2021-11-09 18:24:04.826960 gbpcli-1.5.0/tests/data/pull.json
+-rw-r--r--   0        0        0       80 2021-11-09 18:24:04.826960 gbpcli-1.5.0/tests/data/release_build.json
+-rw-r--r--   0        0        0       83 2021-10-11 10:44:26.504390 gbpcli-1.5.0/tests/data/schedule_build.json
+-rw-r--r--   0        0        0      468 2023-03-20 02:47:01.244810 gbpcli-1.5.0/tests/data/search_notes.json
+-rw-r--r--   0        0        0      584 2022-10-03 00:09:10.558796 gbpcli-1.5.0/tests/data/status.json
+-rw-r--r--   0        0        0       89 2022-08-08 03:06:02.871203 gbpcli-1.5.0/tests/data/tag_build.json
+-rw-r--r--   0        0        0       89 2022-08-08 03:09:13.886678 gbpcli-1.5.0/tests/data/untag_build.json
+-rw-r--r--   0        0        0      614 2023-06-04 16:18:21.949227 gbpcli-1.5.0/tests/test_build.py
+-rw-r--r--   0        0        0     4922 2023-06-04 16:18:21.949227 gbpcli-1.5.0/tests/test_diff.py
+-rw-r--r--   0        0        0     2833 2023-05-20 22:14:10.519712 gbpcli-1.5.0/tests/test_entrypoint.py
+-rw-r--r--   0        0        0     1964 2023-03-20 02:47:01.244810 gbpcli-1.5.0/tests/test_gbp.py
+-rw-r--r--   0        0        0     2330 2023-02-28 00:30:55.388901 gbpcli-1.5.0/tests/test_graphql.py
+-rw-r--r--   0        0        0    11320 2023-06-04 16:18:21.949227 gbpcli-1.5.0/tests/test_inspect.py
+-rw-r--r--   0        0        0     1654 2023-06-04 16:18:21.949227 gbpcli-1.5.0/tests/test_keep.py
+-rw-r--r--   0        0        0     1107 2023-06-04 16:18:21.949227 gbpcli-1.5.0/tests/test_latest.py
+-rw-r--r--   0        0        0     1973 2023-06-04 16:18:21.949227 gbpcli-1.5.0/tests/test_list.py
+-rw-r--r--   0        0        0     1658 2023-06-04 16:18:21.949227 gbpcli-1.5.0/tests/test_logs.py
+-rw-r--r--   0        0        0     2219 2023-06-04 16:18:21.949227 gbpcli-1.5.0/tests/test_machines.py
+-rw-r--r--   0        0        0     5386 2023-06-04 16:18:21.949227 gbpcli-1.5.0/tests/test_notes.py
+-rw-r--r--   0        0        0     1100 2023-06-04 16:18:21.949227 gbpcli-1.5.0/tests/test_packages.py
+-rw-r--r--   0        0        0     1126 2023-06-04 16:18:21.949227 gbpcli-1.5.0/tests/test_publish.py
+-rw-r--r--   0        0        0      606 2023-05-20 22:10:39.185359 gbpcli-1.5.0/tests/test_pull.py
+-rw-r--r--   0        0        0     1386 2023-03-19 18:37:19.694606 gbpcli-1.5.0/tests/test_render.py
+-rw-r--r--   0        0        0     2629 2023-06-04 16:18:21.949227 gbpcli-1.5.0/tests/test_status.py
+-rw-r--r--   0        0        0     1699 2023-06-04 16:18:21.949227 gbpcli-1.5.0/tests/test_tag.py
+-rw-r--r--   0        0        0     2320 2023-02-28 03:24:47.008778 gbpcli-1.5.0/tests/test_theme.py
+-rw-r--r--   0        0        0     4161 2023-04-29 21:56:57.622759 gbpcli-1.5.0/tests/test_utils.py
+-rw-r--r--   0        0        0     4440 1970-01-01 00:00:00.000000 gbpcli-1.5.0/PKG-INFO
```

### Comparing `gbpcli-1.4.0/LICENSE` & `gbpcli-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gbpcli-1.4.0/README.md` & `gbpcli-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `gbpcli-1.4.0/pyproject.toml` & `gbpcli-1.5.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 classifiers = [
     "Environment :: Console",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Operating System :: POSIX :: Linux",
     "Topic :: System :: Software Distribution",
     "Programming Language :: Python :: 3",
 ]
-version = "1.4.0"
+version = "1.5.0"
 
 [project.license]
 text = "GPL3+"
 
 [project.urls]
 homepage = "https://github.com/enku/gbpcli"
 repository = "https://github.com/enku/gbpcli"
@@ -47,17 +47,17 @@
 status = "gbpcli.subcommands.status"
 tag = "gbpcli.subcommands.tag"
 
 [project.optional-dependencies]
 
 [build-system]
 requires = [
-    "pdm-pep517>=1.0.0",
+    "pdm-backend",
 ]
-build-backend = "pdm.pep517.api"
+build-backend = "pdm.backend"
 
 [tool.pdm.version]
 source = "scm"
 
 [tool.pdm.dev-dependencies]
 dev = [
     "black",
```

### Comparing `gbpcli-1.4.0/src/gbpcli/__init__.py` & `gbpcli-1.5.0/src/gbpcli/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,80 +1,28 @@
 """Command Line interface for Gentoo Build Publisher"""
 from __future__ import annotations
 
 import argparse
 import datetime
 import os
 import sys
+import warnings
 from dataclasses import dataclass
-from enum import IntEnum
-from importlib import resources
+from enum import Enum, IntEnum
 from importlib.metadata import entry_points, version
 from typing import IO, Any, Callable, Optional, TypeAlias, TypeVar
 
 import requests
 import rich.console
 import yarl
 from rich.theme import Theme
 
-LOCAL_TIMEZONE = datetime.datetime.now().astimezone().tzinfo
-DEFAULT_URL = os.getenv("BUILD_PUBLISHER_URL", "http://localhost/")
-
-ColorMap = dict[str, str]
-
-DEFAULT_THEME: ColorMap = {
-    "box": "default",
-    "build_id": "bold",
-    "header": "bold",
-    "keep": "yellow",
-    "machine": "blue",
-    "mymachine": "default",
-    "note": "default",
-    "note_flag": "blue",
-    "package": "magenta",
-    "published": "bold green",
-    "tag": "yellow",
-    "timestamp": "default",
-    "yes": "green",
-    "no": "default",
-    "added": "green",
-    "removed": "red",
-}
-
-
-class APIError(Exception):
-    """When an error is returned by the REST API"""
-
-    def __init__(self, errors, data) -> None:
-        super().__init__(errors)
-        self.data = data
-
-
-class Queries:
-    """Python interface to raw queries/*.graphql files"""
-
-    def __getattr__(self, name: str) -> str:
-        query_file = resources.files("gbpcli") / "queries" / f"{name}.graphql"
-        try:
-            return query_file.read_text(encoding="UTF-8")
-        except FileNotFoundError:
-            raise AttributeError(name) from None
-
-    def to_dict(self) -> dict[str, str]:
-        """Return the queries as a dict"""
-        files = (resources.files("gbpcli") / "queries").iterdir()
-
-        return {
-            filename.name[:-8]: getattr(self, filename.name[:-8])
-            for filename in files
-            if filename.name.endswith(".graphql")
-        }
+from gbpcli import graphql, theme
 
-
-queries = Queries()
+DEFAULT_URL = os.getenv("BUILD_PUBLISHER_URL", "http://localhost/")
 
 
 @dataclass(frozen=True)
 class BuildInfo:
     """Metatada about a Build
 
     Retrieved from the API.
@@ -159,92 +107,87 @@
     """Diff status"""
 
     REMOVED = -1
     CHANGED = 0
     ADDED = 1
 
 
+class SearchField(Enum):
+    """Search fields"""
+
+    # pylint: disable=invalid-name
+
+    logs = "LOGS"
+    notes = "NOTES"
+
+
 @dataclass
 class Change:
     """Item in a diff"""
 
     item: str
     status: Status
 
 
+@dataclass(frozen=True)
+class Console:
+    """Output sinks for handlers"""
+
+    out: rich.console.Console
+    err: rich.console.Console
+
+
 class GBP:
     """Python wrapper for the Gentoo Build Publisher API"""
 
-    headers = {"Accept-Encoding": "gzip, deflate"}
-
-    def __init__(self, url: str, exit_gracefully_on_requests_errors=True) -> None:
-        self.url = str(yarl.URL(url) / "graphql")
-        self.session = requests.Session()
-        self.exit_gracefully_on_requests_errors = exit_gracefully_on_requests_errors
-
-    def query(self, query: str, variables: dict[str, Any] | None = None):
-        """Execute the given GraphQL query using the given input variables"""
-        json = {"query": query, "variables": variables}
-
-        try:
-            response = self.session.post(self.url, json=json, headers=self.headers)
-        except requests.exceptions.ConnectionError as error:
-            if self.exit_gracefully_on_requests_errors:
-                error_message = str(error)
-                print(error_message, file=sys.stderr)
-                raise SystemExit(-1) from None
-
-            raise
-
-        response.raise_for_status()
-        response_json = response.json()
-        return response_json.get("data"), response_json.get("errors")
+    def __init__(self, url: str) -> None:
+        self.query = graphql.Queries(yarl.URL(url) / "graphql")
 
     def machines(self) -> list[tuple[str, int, dict]]:
         """Handler for subcommand"""
-        data = self.check(queries.machines)
+        data = graphql.check(self.query.machines())
 
         return [
             (i["machine"], i["buildCount"], i["latestBuild"]) for i in data["machines"]
         ]
 
     def machine_names(self) -> list["str"]:
         """Return the list of machine names
 
         Machines having builds.
         """
-        machines = self.check(queries.machine_names)["machines"]
+        machines = graphql.check(self.query.machine_names())["machines"]
 
         return [machine["machine"] for machine in machines]
 
     def publish(self, build: Build) -> None:
         """Publish the given build"""
-        self.check(queries.publish, {"id": build.id})
+        graphql.check(self.query.publish(id=build.id))
 
     def pull(self, build: Build) -> None:
         """Pull the given build"""
-        self.check(queries.pull, {"id": build.id})
+        graphql.check(self.query.pull(id=build.id))
 
     def latest(self, machine: str) -> Optional[Build]:
         """Return the latest build for machine
 
         Return None if there are no builds for the given machine
         """
-        data = self.check(queries.latest, dict(machine=machine))
+        data = graphql.check(self.query.latest(machine=machine))
         latest = data["latest"]
 
         if latest is None:
             return None
 
         build_id = data["latest"]["id"]
         return Build.from_id(build_id)
 
     def resolve_tag(self, machine: str, tag: str) -> Optional[Build]:
         """Return the build of the given machine & tag"""
-        data = self.check(queries.resolve_tag, dict(machine=machine, tag=tag))[
+        data = graphql.check(self.query.resolve_tag(machine=machine, tag=tag))[
             "resolveBuildTag"
         ]
 
         if data is None:
             return None
 
         build_id = data["id"]
@@ -252,109 +195,112 @@
         return Build.from_id(build_id)
 
     def builds(self, machine: str, with_packages: bool = False) -> list[Build]:
         """Return a list of Builds for the given machine
 
         If `with_packages` is True, also include the list of packages for the builds
         """
-        query = queries.builds_with_packages if with_packages else queries.builds
-        data = self.query(query, dict(machine=machine))[0]
+        query = self.query.builds_with_packages if with_packages else self.query.builds
+        data = query(machine=machine)[0]
         builds = data["builds"]
         builds.reverse()
 
         return [Build.from_api_response(i) for i in builds]
 
     def diff(
         self, machine: str, left: int, right: int
     ) -> tuple[Build, Build, list[Change]]:
         """Return difference between two builds"""
-        variables = {"left": f"{machine}.{left}", "right": f"{machine}.{right}"}
-        data = self.check(queries.diff, variables)
+        data = graphql.check(
+            self.query.diff(left=f"{machine}.{left}", right=f"{machine}.{right}")
+        )
 
         return (
             Build.from_api_response(data["diff"]["left"]),
             Build.from_api_response(data["diff"]["right"]),
             [
                 Change(item=i["item"], status=getattr(Status, i["status"]))
                 for i in data["diff"]["items"]
             ],
         )
 
     def logs(self, build: Build) -> Optional[str]:
         """Return logs for the given Build"""
-        data = self.check(queries.logs, {"id": build.id})
+        data = graphql.check(self.query.logs(id=build.id))
 
         return None if data["build"] is None else data["build"]["logs"]
 
     def get_build_info(self, build: Build) -> Optional[Build]:
         """Return build with info gained from the GBP API"""
-        data, errors = self.query(queries.build, {"id": build.id})
+        data, errors = self.query.build(id=build.id)
         build = data["build"]
 
         if build is None:
             if errors:
-                raise APIError(errors, data)
+                raise graphql.APIError(errors, data)
             return None
 
         return Build.from_api_response(build)
 
     def build(self, machine: str) -> str:
         """Schedule a build"""
-        response = self.check(queries.schedule_build, dict(machine=machine))
+        response = graphql.check(self.query.schedule_build(machine=machine))
         return response["scheduleBuild"]
 
     def packages(self, build: Build) -> Optional[list[str]]:
         """Return the list of packages for a build"""
-        data = self.check(queries.packages, {"id": build.id})
+        data = graphql.check(self.query.packages(id=build.id))
         return data["build"]["packages"]
 
     def keep(self, build: Build) -> dict[str, bool]:
         """Mark a build as kept"""
-        return self.check(queries.keep_build, {"id": build.id})["keepBuild"]
+        return graphql.check(self.query.keep_build(id=build.id))["keepBuild"]
 
     def release(self, build: Build) -> dict[str, bool]:
         """Unmark a build as kept"""
-        return self.check(queries.release_build, {"id": build.id})["releaseBuild"]
+        return graphql.check(self.query.release_build(id=build.id))["releaseBuild"]
 
     def create_note(self, build: Build, note: Optional[str]) -> dict[str, str]:
         """Create or delete note for the given build.
 
         If note is None, the note is deleted (if it exists).
         """
-        return self.check(queries.create_note, {"id": build.id, "note": note})[
+        return graphql.check(self.query.create_note(id=build.id, note=note))[
             "createNote"
         ]
 
-    def search_notes(self, machine: str, key: str) -> list[Build]:
-        """Search buids for the given machine name for notes containing key.
+    def search(self, machine: str, field: SearchField, key: str) -> list[Build]:
+        """Search builds for the given machine name in fields containing key.
 
-        Return a list of Builds who's notes match the (case-insensitive) string.
+        Return a list of Builds who's given field match the (case-insensitive) string.
         """
-        query = queries.search_notes
-
-        response = self.check(query, {"machine": machine, "key": key})
-        builds = response["searchNotes"]
+        response = graphql.check(
+            self.query.search(machine=machine, field=field.value, key=key)
+        )
+        builds = response["search"]
 
         return [Build.from_api_response(i) for i in builds]
 
+    def search_notes(self, machine: str, key: str) -> list[Build]:
+        """Search builds for the given machine name for notes containing key.
+
+        This method is deprecated. Use search() instead.
+        """
+        message = "This method is deprecated. Use search() instead"
+        warnings.warn(message, DeprecationWarning, stacklevel=2)
+
+        return self.search(machine, SearchField.notes, key)
+
     def tag(self, build: Build, tag: str) -> None:
         """Add the given tag to the build"""
-        self.check(queries.tag_build, {"id": build.id, "tag": tag})
+        graphql.check(self.query.tag_build(id=build.id, tag=tag))
 
     def untag(self, machine: str, tag: str) -> None:
         """Remove the tag from the given machine"""
-        self.check(queries.untag_build, {"machine": machine, "tag": tag})
-
-    def check(self, query: str, variables: dict[str, Any] = None) -> dict:
-        """Run query and raise exception if there are errors"""
-        data, errors = self.query(query, variables)
-
-        if errors:
-            raise APIError(errors, data)
-        return data
+        graphql.check(self.query.untag_build(machine=machine, tag=tag))
 
 
 def build_parser() -> argparse.ArgumentParser:
     """Set command-line arguments"""
     usage = "Command-line interface to Gentoo Build Publisher\n\nCommands:\n\n"
     parser = argparse.ArgumentParser(prog="gbp")
     parser.add_argument(
@@ -364,15 +310,23 @@
     parser.add_argument(
         "--color",
         metavar="WHEN",
         choices=["never", "always", "auto"],
         default="auto",
         help="color output",
     )
-    parser.add_argument("--my-machines", default=os.getenv("GBPCLI_MYMACHINES", ""))
+    parser.add_argument(
+        "--my-machines",
+        default=os.getenv("GBPCLI_MYMACHINES", ""),
+        help=(
+            "whitespace-delimited list of machine names to filter on "
+            "when using the --mine argument. Typically one would instead use "
+            "the GBPCLI_MYMACHINES environment variable."
+        ),
+    )
     subparsers = parser.add_subparsers()
 
     try:
         eps = entry_points().select(group="gbpcli.subcommands")
     except AttributeError:
         eps = entry_points()["gbpcli.subcommands"]
 
@@ -388,81 +342,45 @@
         subparser.set_defaults(func=module.handler)
 
     parser.usage = usage
 
     return parser
 
 
-def get_colormap_from_string(string: str) -> ColorMap:
-    """Given the text sring return a gbp ColorMap
-
-    String is expected to be a colon-delimited (":") set of name=value pairs. So for
-    example:
-
-        "build_id=bold:header=bold:keep=yellow:machine=blue"
-
-    Values are stripped of whitespace. If the fields cannot be parsed a `ValueError` is
-    raised.  Empty names/values are ignored as are unrecognized names.
-    """
-    colormap = DEFAULT_THEME.copy()
-    error = ValueError(f"Invalid color map: {string!r}")
-
-    if not string:
-        return colormap
-
-    for assignment in string.split(":"):
-        if not assignment:
-            continue
-        try:
-            name, value = assignment.split("=")
-        except ValueError:
-            raise error from None
-
-        name = name.strip()
-        name = name.strip()
-
-        if not name or not value:
-            continue
-
-        if name in colormap:
-            colormap[name] = value.strip()
-
-    return colormap
-
-
 def main(argv: list[str] | None = None) -> int:
     """Main entry point"""
-    errorf: IO[str] = sys.stderr
-
     if argv is None:
         argv = sys.argv[1:]
 
     parser = build_parser()
 
     args = parser.parse_args(argv)
 
     if not hasattr(args, "func"):
-        parser.print_help(file=errorf)
+        parser.print_help(file=sys.stderr)
         return 1
 
     gbp = GBP(args.url)
 
     force_terminal = {"always": True, "never": False}.get(args.color, None)
 
     try:
-        console_theme = get_colormap_from_string(os.getenv("GBPCLI_COLORS", ""))
+        console_theme = theme.get_colormap_from_string(os.getenv("GBPCLI_COLORS", ""))
     except ValueError:
-        console_theme = DEFAULT_THEME
+        console_theme = theme.DEFAULT_THEME
 
-    console = rich.console.Console(
-        force_terminal=force_terminal,
-        color_system="auto",
-        highlight=False,
-        theme=Theme(console_theme),
+    console = Console(
+        out=rich.console.Console(
+            force_terminal=force_terminal,
+            color_system="auto",
+            highlight=False,
+            theme=Theme(console_theme),
+        ),
+        err=rich.console.Console(file=sys.stderr),
     )
 
     try:
-        return args.func(args, gbp, console, errorf)
-    except (APIError, requests.HTTPError) as error:
-        print(str(error), file=errorf)
+        return args.func(args, gbp, console)
+    except (graphql.APIError, requests.HTTPError) as error:
+        console.err.print(str(error))
 
         return 1
```

### Comparing `gbpcli-1.4.0/src/gbpcli/subcommands/build.py` & `gbpcli-1.5.0/src/gbpcli/subcommands/publish.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-"""Schedule a build for the given machine in CI/CD"""
+"""Publish a build
+
+If NUMBER is not specified, defaults to the latest build for the given machine.
+"""
 import argparse
-from typing import TextIO
 
-from rich.console import Console
+from gbpcli import GBP, Console
+from gbpcli.utils import resolve_build_id
 
-from gbpcli import GBP
 
+def handler(args: argparse.Namespace, gbp: GBP, _console: Console) -> int:
+    """Publish a build"""
+    build = resolve_build_id(args.machine, args.number, gbp)
 
-def handler(
-    args: argparse.Namespace, gbp: GBP, _console: Console, _errorf: TextIO
-) -> int:
-    """Schedule a build for the given machine in CI/CD"""
-    gbp.build(args.machine)
+    gbp.publish(build)
 
     return 0
 
 
 def parse_args(parser: argparse.ArgumentParser) -> None:
     """Set subcommand arguments"""
     parser.add_argument("machine", metavar="MACHINE", help="name of the machine")
+    parser.add_argument("number", metavar="NUMBER", nargs="?", help="build number")
```

### Comparing `gbpcli-1.4.0/src/gbpcli/subcommands/diff.py` & `gbpcli-1.5.0/src/gbpcli/subcommands/diff.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,96 +3,91 @@
 If the "left" argument is omitted, it defaults to the build which is published.
 
 If the "right" argument is omitted, it defaults to the most recent build.
 """
 import argparse
 import datetime as dt
 from collections.abc import Iterable
-from typing import TextIO
 
-from rich.console import Console
+from gbpcli import GBP, Change, Console, Status, render, utils
 
-from gbpcli import GBP, Change, Status, utils
 
-
-def handler(
-    args: argparse.Namespace, gbp: GBP, console: Console, errorf: TextIO
-) -> int:
+def handler(args: argparse.Namespace, gbp: GBP, console: Console) -> int:
     """Handler for subcommand"""
     left = args.left
     right = args.right
 
     if left is None:
         builds = gbp.builds(args.machine)
         published = [i for i in builds if (i.info and i.info.published)]
 
         if not published:
-            print("No origin specified and no builds published", file=errorf)
+            console.err.print("No origin specified and no builds published")
             return 1
 
         assert len(published) == 1
         left = published[0].number
 
         assert right is None
         right = str(builds[-1].number)
     else:
-        left = utils.resolve_build_id(args.machine, left, gbp, errorf=errorf).number
+        left = utils.resolve_build_id(args.machine, left, gbp).number
 
     if right is None:
         latest = gbp.latest(args.machine)
 
         if latest is None:
-            print("Need at least two builds to diff", file=errorf)
+            console.err.print("Need at least two builds to diff")
             return 1
 
         right = latest.number
     else:
-        right = utils.resolve_build_id(args.machine, right, gbp, errorf=errorf).number
+        right = utils.resolve_build_id(args.machine, right, gbp).number
 
     left_build, right_build, diff = gbp.diff(args.machine, left, right)
 
     if not diff:
         return 0
 
     assert left_build.info is not None
     assert right_build.info is not None
     assert isinstance(left_build.info.built, dt.datetime)
     assert isinstance(right_build.info.built, dt.datetime)
 
-    console.print(
+    console.out.print(
         f"diff -r {args.machine}/{left} {args.machine}/{right}", style="header"
     )
-    console.print(
-        f"--- a/{args.machine}/{left} {utils.timestr(left_build.info.built)}",
+    console.out.print(
+        f"--- a/{args.machine}/{left} {render.timestr(left_build.info.built)}",
         style="header",
     )
-    console.print(
-        f"+++ b/{args.machine}/{right} {utils.timestr(right_build.info.built)}",
+    console.out.print(
+        f"+++ b/{args.machine}/{right} {render.timestr(right_build.info.built)}",
         style="header",
     )
 
     print_diff(diff, console)
 
     return 0
 
 
 def print_diff(diff: Iterable[Change], console: Console) -> None:
     """Given the list of changes, pretty-print the diff to the console"""
     last_modified: Change | None = None
     # for change, item in iter(response["diff"]["items"]):
     for item in diff:
         if item.status == Status.REMOVED:
-            console.print(f"[removed]-{item.item}")
+            console.out.print(f"[removed]-{item.item}")
         elif item.status == Status.ADDED:
-            console.print(f"[added]+{item.item}")
+            console.out.print(f"[added]+{item.item}")
         else:
             if item == last_modified:
-                console.print(f"[removed]-{item.item}")
+                console.out.print(f"[removed]-{item.item}")
             else:
-                console.print(f"[added]+{item.item}")
+                console.out.print(f"[added]+{item.item}")
             last_modified = item
 
 
 def parse_args(parser: argparse.ArgumentParser) -> None:
     """Set subcommand arguments"""
     parser.add_argument("machine", metavar="MACHINE", help="name of the machine")
     parser.add_argument("left", metavar="LEFT", nargs="?", help="left build number")
```

### Comparing `gbpcli-1.4.0/src/gbpcli/subcommands/inspect.py` & `gbpcli-1.5.0/src/gbpcli/subcommands/inspect.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 Display all the builds (or the last n builds if --tail is given) for all the
 machines (or only the machines given).  Display the build's timestamp as well as
 the timestamp for each build's packages' completion.  If the build has a note
 that will be displayed as well.
 """
 import argparse
 import datetime as dt
-from typing import List, TextIO
+from typing import List
 
-from rich.console import Console, RenderableType
+from rich.console import RenderableType
 from rich.panel import Panel
 from rich.table import Table
 from rich.tree import Tree
 
-from gbpcli import GBP, LOCAL_TIMEZONE, Build, Package, utils
+from gbpcli import GBP, Build, Console, Package, render, utils
 
 
 def sort_packages_by_build_time(packages: List[Package]) -> List[Package]:
     """Missing docstring"""
     sorted_packages = [*packages]
     sorted_packages.sort(key=lambda p: getattr(p, "build_time", dt.datetime.min))
 
@@ -30,15 +30,17 @@
     assert build.info
 
     build_str = f"[build_id]{build.number}[/build_id]"
 
     if build.info.published:
         build_str = f"[published]{build_str}[/published]"
 
-    timestamp = (build.info.built or build.info.submitted).astimezone(LOCAL_TIMEZONE)
+    timestamp = (build.info.built or build.info.submitted).astimezone(
+        render.LOCAL_TIMEZONE
+    )
     build_str = f"{build_str} [timestamp]({timestamp.strftime('%x %X')})[/timestamp]"
 
     if build.info.tags:
         tag_strs = [f"[tag]@{tag}[/tag]" for tag in build.info.tags]
     else:
         tag_strs = []
 
@@ -54,26 +56,24 @@
         return grid
 
     return build_str
 
 
 def render_package(package: Package, build_build_date: dt.date) -> str:
     """Convert `package` into a rich renderable"""
-    local_build_time = package.build_time.astimezone(LOCAL_TIMEZONE)
+    local_build_time = package.build_time.astimezone(render.LOCAL_TIMEZONE)
     if local_build_time.date() != build_build_date:
         build_time = local_build_time.strftime("%x %X")
     else:
         build_time = str(local_build_time.time())
 
     return f"[package]{package.cpv}[/package] [timestamp]({build_time})[/timestamp]"
 
 
-def handler(
-    args: argparse.Namespace, gbp: GBP, console: Console, errorf: TextIO
-) -> int:
+def handler(args: argparse.Namespace, gbp: GBP, console: Console) -> int:
     """Show the machines builds as a tree"""
     tree = Tree("[header]Machines[/header]", guide_style="box")
 
     if args.machine:
         machines = args.machine
     elif args.mine:
         machines = utils.get_my_machines_from_args(args)
@@ -82,39 +82,39 @@
 
     for machine in machines:
         if "." in machine:
             machine, _, number = machine.partition(".")
             build = gbp.get_build_info(Build(machine=machine, number=int(number)))
 
             if build is None:
-                print("Not found", file=errorf)
+                console.err.print("Not found")
                 return 1
 
             builds = [build]
         else:
             builds = gbp.builds(machine, with_packages=True)[-1 * args.tail :]
 
-        branch = tree.add(utils.format_machine(machine, args))
+        branch = tree.add(render.format_machine(machine, args))
 
         for build in builds:
             assert build.info
 
             p_branch = branch.add(render_build(build))
             build_date = (
                 (build.info.built or build.info.submitted)
-                .astimezone(LOCAL_TIMEZONE)
+                .astimezone(render.LOCAL_TIMEZONE)
                 .date()
             )
             packages: List[Package] = build.packages_built or []
             packages = sort_packages_by_build_time(packages)
 
             for package in packages:
                 p_branch.add(render_package(package, build_date))
 
-    console.print(tree)
+    console.out.print(tree)
 
     return 0
 
 
 def parse_args(parser: argparse.ArgumentParser) -> None:
     """Set subcommand arguments"""
     parser.add_argument("-t", "--tail", type=int, default=0)
```

### Comparing `gbpcli-1.4.0/src/gbpcli/subcommands/keep.py` & `gbpcli-1.5.0/src/gbpcli/subcommands/logs.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,32 +1,48 @@
-"""Keep (or release) a build"""
+"""Display logs for the given build"""
 import argparse
-from typing import TextIO
 
-from rich.console import Console
+from gbpcli import GBP, Console, SearchField, render, utils
+from gbpcli.subcommands import make_searchable
 
-from gbpcli import GBP, utils
 
+def search_logs(gbp: GBP, args: argparse.Namespace, console: Console) -> int:
+    """--search handler for the notes subcommand"""
+    builds = gbp.search(args.machine, SearchField.logs, args.number)
 
-def handler(
-    args: argparse.Namespace, gbp: GBP, _console: Console, errorf: TextIO
-) -> int:
-    """Keep (or release) a build"""
-    build = utils.resolve_build_id(args.machine, args.number, gbp, errorf=errorf)
+    if not builds:
+        console.err.print("No matches found")
+        return 1
+
+    sep = ""
+    for build in builds:  # pylint: disable=duplicate-code
+        console.out.print(sep, end="")
+        console.out.print(
+            f"{render.format_machine(build.machine, args)}/"
+            f"{render.format_build_number(build.number)}"
+        )
+        console.out.print(gbp.logs(build))
+        sep = "---\n"
+
+    return 0
 
-    if args.release:
-        result = gbp.release(build)
-    else:
-        result = gbp.keep(build)
 
-    if result is None:
-        print("Not Found", file=errorf)
+def handler(args: argparse.Namespace, gbp: GBP, console: Console) -> int:
+    """Show build logs"""
+    if args.search:
+        return search_logs(gbp, args, console)
+
+    build = utils.resolve_build_id(args.machine, args.number, gbp)
+    text = gbp.logs(build)
+
+    if text is None:
+        console.err.print("Not Found")
         return 1
 
+    console.out.print(text)
+
     return 0
 
 
 def parse_args(parser: argparse.ArgumentParser) -> None:
     """Set subcommand arguments"""
-    parser.add_argument("--release", "-r", action="store_true", default=False)
-    parser.add_argument("machine", metavar="MACHINE", help="name of the machine")
-    parser.add_argument("number", metavar="NUMBER", help="build number")
+    make_searchable(parser)
```

### Comparing `gbpcli-1.4.0/src/gbpcli/subcommands/list.py` & `gbpcli-1.5.0/src/gbpcli/subcommands/list.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,60 +5,49 @@
     *: Packages were build for the build
     K: The build has been marked for keeping
     P: This build is published
     N: This build has a note attached
 
 """
 import argparse
-from typing import TextIO
 
 from rich import box
-from rich.console import Console
 from rich.table import Table
 
-from gbpcli import GBP, LOCAL_TIMEZONE, utils
+from gbpcli import GBP, Console, render
 
 
-def handler(
-    args: argparse.Namespace, gbp: GBP, console: Console, _errorf: TextIO
-) -> int:
+def handler(args: argparse.Namespace, gbp: GBP, console: Console) -> int:
     """List a machine's builds"""
     builds = gbp.builds(args.machine, with_packages=True)
     table = Table(
-        title=f"\N{PERSONAL COMPUTER} {utils.format_machine(args.machine, args)}",
+        title=f"\N{PERSONAL COMPUTER} {render.format_machine(args.machine, args)}",
         box=box.ROUNDED,
         title_style="header",
         style="box",
     )
     table.add_column("Flags", header_style="header")
     table.add_column("ID", justify="right", header_style="header")
     table.add_column("Built", header_style="header")
     table.add_column("Tags", header_style="header")
 
     for build in builds:
         assert build.info is not None
 
         # In the old days, we didn't have a "built" field. Fall back to submitted
-        timestamp = (build.info.built or build.info.submitted).astimezone(
-            LOCAL_TIMEZONE
-        )
+        timestamp = build.info.built or build.info.submitted
 
-        flags = (
-            f"{'[package]*[/package]' if build.packages_built else ' '}"
-            f"{'[keep]K[/keep]' if build.info.keep else ' '}"
-            f"{'[published]P[/published]' if build.info.published else ' '}"
-            f"{'[note_flag]N[/note_flag]' if build.info.note else ' '}"
+        table.add_row(
+            render.format_flags(build),
+            render.format_build_number(build.number),
+            render.format_timestamp(timestamp.astimezone(render.LOCAL_TIMEZONE)),
+            render.format_tags(build.info.tags),
         )
-        number = f"[build_id]{build.number}[/build_id]"
-        built = f"[timestamp]{timestamp.strftime('%x %X')}[/timestamp]"
-        tag_list = [f"@{tag}" for tag in build.info.tags] if build.info.tags else []
-        tags = f"[tag]{' '.join(tag_list)}[/tag]"
-        table.add_row(flags, number, built, tags)
 
-    console.print(table)
+    console.out.print(table)
 
     return 0
 
 
 def parse_args(parser: argparse.ArgumentParser):
     """Set subcommand arguments"""
     parser.add_argument("machine", metavar="MACHINE", help="name of the machine")
```

### Comparing `gbpcli-1.4.0/src/gbpcli/subcommands/machines.py` & `gbpcli-1.5.0/src/gbpcli/subcommands/machines.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,27 @@
 """List machines with builds"""
 import argparse
-from typing import TextIO
 
 from rich import box
-from rich.console import Console
 from rich.table import Table
 
-from gbpcli import GBP, utils
+from gbpcli import GBP, Console, render, utils
 
 
 def latest_build_to_str(build: dict) -> str:
     """Return the "Latest" column for the given build"""
     build_id = build["id"].rpartition(".")[2]
 
     if build["published"]:
         build_id = f"[published]{build_id}[/published]"
 
     return f"[build_id]{build_id}[/build_id]"
 
 
-def handler(
-    args: argparse.Namespace, gbp: GBP, console: Console, _errorf: TextIO
-) -> int:
+def handler(args: argparse.Namespace, gbp: GBP, console: Console) -> int:
     """List machines with builds"""
     my_machines = utils.get_my_machines_from_args(args)
     machines = [
         machine
         for machine in gbp.machines()
         if not args.mine or machine[0] in my_machines
     ]
@@ -37,20 +33,20 @@
     )
     table.add_column("Machine", header_style="header")
     table.add_column("Builds", justify="right", header_style="header")
     table.add_column("Latest", justify="right", header_style="header")
 
     for machine, builds, latest in machines:
         table.add_row(
-            utils.format_machine(machine, args),
+            render.format_machine(machine, args),
             str(builds),
             latest_build_to_str(latest),
         )
 
-    console.print(table)
+    console.out.print(table)
     return 0
 
 
 def parse_args(parser: argparse.ArgumentParser) -> None:
     """Set subcommand arguments"""
     parser.add_argument(
         "--mine",
```

### Comparing `gbpcli-1.4.0/src/gbpcli/subcommands/notes.py` & `gbpcli-1.5.0/src/gbpcli/subcommands/notes.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 """notes subcommand for gbpcli"""
 import argparse
 import os
 import subprocess
 import sys
 import tempfile
-from typing import Optional, TextIO
+from typing import Optional
 
-from rich.console import Console
-
-from gbpcli import GBP, utils
+from gbpcli import GBP, Console, SearchField, render, utils
+from gbpcli.subcommands import make_searchable
 
 
 def get_editor():
     """Return the user's editor preference.
 
     Does this by inpsecting first the VISUAL environment variable then the EDITOR
     environment variable.
@@ -55,45 +54,41 @@
         note = open_editor(editor, existing_note)
     else:
         note = sys.stdin.read()
 
     return note
 
 
-def search_notes(
-    gbp: GBP, machine: str, key: str, console: Console, errorf: TextIO
-) -> int:
+def search_notes(gbp: GBP, machine: str, key: str, console: Console) -> int:
     """--search handler for the notes subcommand"""
-    builds = gbp.search_notes(machine, key)
+    builds = gbp.search(machine, SearchField.notes, key)
 
     if not builds:
-        print("No matches found", file=errorf)
+        console.err.print("No matches found")
         return 1
 
     sep = ""
     for build in builds:
-        console.print(sep, end="")
-        console.print(utils.build_to_str(build), end="")
+        console.out.print(sep, end="")
+        console.out.print(render.build_to_str(build), end="")
         sep = "\n"
 
     return 0
 
 
-def handler(
-    args: argparse.Namespace, gbp: GBP, console: Console, errorf: TextIO
-) -> int:
+def handler(args: argparse.Namespace, gbp: GBP, console: Console) -> int:
     """Show, search, and edit build notes"""
     if args.search:
-        return search_notes(gbp, args.machine, args.number, console, errorf)
+        return search_notes(gbp, args.machine, args.number, console)
 
-    build = utils.resolve_build_id(args.machine, args.number, gbp, errorf=errorf)
+    build = utils.resolve_build_id(args.machine, args.number, gbp)
     existing = gbp.get_build_info(build)
 
     if not existing or not existing.info:
-        print("Build not found", file=errorf)
+        console.err.print("Build not found")
         return 1
 
     if args.delete:
         note = None
     else:
         try:
             note = get_note(existing.info.note)
@@ -104,16 +99,8 @@
 
     return 0
 
 
 def parse_args(parser: argparse.ArgumentParser) -> None:
     """Set subcommand arguments"""
     parser.add_argument("--delete", "-d", action="store_true", default=False)
-    parser.add_argument(
-        "--search",
-        "-s",
-        action="store_true",
-        default=False,
-        help="Search build notes for the given text.",
-    )
-    parser.add_argument("machine", metavar="MACHINE", help="name of the machine")
-    parser.add_argument("number", metavar="KEY|NUMBER", help="build number")
+    make_searchable(parser)
```

### Comparing `gbpcli-1.4.0/src/gbpcli/subcommands/packages.py` & `gbpcli-1.5.0/src/gbpcli/subcommands/packages.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,24 @@
 """Display the list of packages for a given build"""
 import argparse
-from typing import TextIO
 
-from rich.console import Console
+from gbpcli import GBP, Console, utils
 
-from gbpcli import GBP, utils
 
-
-def handler(
-    args: argparse.Namespace, gbp: GBP, console: Console, errorf: TextIO
-) -> int:
+def handler(args: argparse.Namespace, gbp: GBP, console: Console) -> int:
     """List a build's packages"""
-    build = utils.resolve_build_id(args.machine, args.number, gbp, errorf=errorf)
+    build = utils.resolve_build_id(args.machine, args.number, gbp)
     packages = gbp.packages(build)
 
     if packages is None:
-        print("Not Found", file=errorf)
+        console.err.print("Not Found")
         return 1
 
     for package in packages:
-        console.print(f"[package]{package}[/package]")
+        console.out.print(f"[package]{package}[/package]")
 
     return 0
 
 
 def parse_args(parser: argparse.ArgumentParser) -> None:
     """Set subcommand arguments"""
     parser.add_argument("machine", metavar="MACHINE", help="name of the machine")
```

### Comparing `gbpcli-1.4.0/src/gbpcli/subcommands/publish.py` & `gbpcli-1.5.0/src/gbpcli/subcommands/pull.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,19 @@
-"""Publish a build
-
-If NUMBER is not specified, defaults to the latest build for the given machine.
-"""
+"""Pull a build"""
 import argparse
-from typing import TextIO
-
-from rich.console import Console
 
-from gbpcli import GBP
-from gbpcli.utils import resolve_build_id
+from gbpcli import GBP, Build, Console
 
 
-def handler(
-    args: argparse.Namespace, gbp: GBP, _console: Console, errorf: TextIO
-) -> int:
-    """Publish a build"""
-    build = resolve_build_id(args.machine, args.number, gbp, errorf=errorf)
+def handler(args: argparse.Namespace, gbp: GBP, _console: Console) -> int:
+    """Pull a build"""
+    build = Build(machine=args.machine, number=args.number)
 
-    gbp.publish(build)
+    gbp.pull(build)
 
     return 0
 
 
 def parse_args(parser: argparse.ArgumentParser) -> None:
     """Set subcommand arguments"""
     parser.add_argument("machine", metavar="MACHINE", help="name of the machine")
-    parser.add_argument("number", metavar="NUMBER", nargs="?", help="build number")
+    parser.add_argument("number", type=int, metavar="NUMBER", help="build number")
```

### Comparing `gbpcli-1.4.0/src/gbpcli/subcommands/status.py` & `gbpcli-1.5.0/src/gbpcli/subcommands/status.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 """Show details for a given build"""
 import argparse
-from typing import TextIO
 
 from rich import box
-from rich.console import Console
 from rich.panel import Panel
 from rich.table import Table
 
-from gbpcli import GBP
-from gbpcli.utils import resolve_build_id, styled_yes, timestr
+from gbpcli import GBP, Console
+from gbpcli.render import styled_yes, timestr, yesno
+from gbpcli.utils import resolve_build_id
 
 
-def handler(
-    args: argparse.Namespace, gbp: GBP, console: Console, errorf: TextIO
-) -> int:
+def handler(args: argparse.Namespace, gbp: GBP, console: Console) -> int:
     """Show build details"""
-    resolved_build = resolve_build_id(args.machine, args.number, gbp, errorf=errorf)
+    resolved_build = resolve_build_id(args.machine, args.number, gbp)
     build = gbp.get_build_info(resolved_build)
 
     if build is None:
-        print("Not found", file=errorf)
+        console.err.print("Not found")
         return 1
 
     assert build.info is not None
 
     grid = Table.grid()
     grid.add_column()
     grid.add_column()
@@ -44,41 +41,43 @@
         f"[timestamp]{timestr(build.info.submitted)}[/timestamp]",
     )
 
     grid.add_row(
         "[header]Completed:[/header] ",
         f"[timestamp]{timestr(build.info.completed)}[/timestamp]"
         if build.info.completed
-        else styled_yes(False),
+        else styled_yes(yesno(False)),
     )
 
-    grid.add_row("[header]Published:[/header] ", f"{styled_yes(build.info.published)}")
-    grid.add_row("[header]Keep:[/header] ", f"{styled_yes(build.info.keep)}")
+    grid.add_row(
+        "[header]Published:[/header] ", f"{styled_yes(yesno(build.info.published))}"
+    )
+    grid.add_row("[header]Keep:[/header] ", f"{styled_yes(yesno(build.info.keep))}")
     tags = [f"[tag]@{tag}[/tag]" for tag in build.info.tags]
     grid.add_row("[header]Tags:[/header] ", " ".join(tags))
 
     packages = build.packages_built
     grid.add_row(
         "[header]Packages-built:[/header] ",
         f"[package]{packages[0].cpv}[/package]" if packages else "None",
     )
 
     if packages:
         for package in packages[1:]:
             grid.add_row("", f"[package]{package.cpv}[/package]")
 
-    console.print(Panel(grid, expand=False, style="box"))
+    console.out.print(Panel(grid, expand=False, style="box"))
 
     if note := build.info.note:
-        console.print()
+        console.out.print()
         table = Table(box=box.ROUNDED, pad_edge=False, style="box")
         table.add_column("📎 Notes", header_style="header")
         table.add_row("[note]" + note.rstrip("\n") + "[/note]")
 
-        console.print(table)
+        console.out.print(table)
 
     return 0
 
 
 def parse_args(parser: argparse.ArgumentParser) -> None:
     """Set subcommand arguments"""
     parser.add_argument("machine", metavar="MACHINE", help="name of the machine")
```

### Comparing `gbpcli-1.4.0/src/gbpcli/subcommands/tag.py` & `gbpcli-1.5.0/src/gbpcli/subcommands/tag.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,32 @@
 """Add tag to the given build"""
 import argparse
-from typing import Optional, TextIO
+from typing import Optional
 
-from rich.console import Console
+from gbpcli import GBP, Build, Console, utils
 
-from gbpcli import GBP, Build, utils
 
-
-def handler(
-    args: argparse.Namespace, gbp: GBP, _console: Console, errorf: TextIO
-) -> int:
+def handler(args: argparse.Namespace, gbp: GBP, console: Console) -> int:
     """Add tags builds"""
     build: Optional[Build]
     machine: str = args.machine
     tag: str = args.tag
 
     if args.remove:
         if args.number is not None:
-            print("When removing a tag, omit the build number", file=errorf)
+            console.err.print("When removing a tag, omit the build number")
             return 1
 
         if tag.startswith("@"):
             tag = tag[1:]
 
         gbp.untag(machine, tag)
         return 0
 
-    build = utils.resolve_build_id(machine, args.number, gbp, errorf=errorf)
+    build = utils.resolve_build_id(machine, args.number, gbp)
 
     gbp.tag(build, tag)
 
     return 0
 
 
 def parse_args(parser: argparse.ArgumentParser) -> None:
```

### Comparing `gbpcli-1.4.0/src/gbpcli/utils.py` & `gbpcli-1.5.0/src/gbpcli/render.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,39 @@
-"""Utility functions"""
+"""Utilties for rendering output"""
+from __future__ import annotations
+
 import argparse
-import datetime
+import datetime as dt
 import io
-import sys
 from functools import partial
-from typing import Literal, Optional, TextIO
-
-from gbpcli import GBP, LOCAL_TIMEZONE, Build
+from typing import Literal
 
-JSON_CONTENT_TYPE = "application/json"
-TAG_SYM = "@"
+from gbpcli import Build, utils
 
-
-def timestr(
-    timestamp: datetime.datetime, timezone: datetime.tzinfo | None = None
-) -> str:
-    """Humanize JSON timestamp string"""
-    timezone = timezone or LOCAL_TIMEZONE
-    dt_obj = timestamp.astimezone(timezone)
-
-    return dt_obj.strftime("%c %z")
+LOCAL_TIMEZONE = dt.datetime.now().astimezone().tzinfo
 
 
 def yesno(value: bool) -> Literal["yes", "no"]:
     """Convert bool value to 'yes' or 'no'"""
     if value:
         return "yes"
 
     return "no"
 
 
-def styled_yes(value: bool) -> str:
-    """Like yesno() but yes's are wrapped in green"""
-    yes_or_no = yesno(value)
+def timestr(timestamp: dt.datetime, timezone: dt.tzinfo | None = None) -> str:
+    """Humanize JSON timestamp string"""
+    timezone = timezone or LOCAL_TIMEZONE
+    dt_obj = timestamp.astimezone(timezone)
+
+    return dt_obj.strftime("%c %z")
 
+
+def styled_yes(yes_or_no: str) -> str:
+    """Like yesno() but yes's are wrapped in green"""
     return f"[{yes_or_no}]{yes_or_no}[/{yes_or_no}]"
 
 
 def build_to_str(build: Build) -> str:
     """Return Build(Info) as a string
 
     `build` must have a non-None info struct.
@@ -80,69 +76,57 @@
         for line in lines:
             fprint(line)
 
     fprint()
     return myio.getvalue()
 
 
-def resolve_build_id(
-    machine: str,
-    build_id: Optional[str],
-    gbp: GBP,
-    abort_on_error: bool = True,
-    errorf: TextIO = sys.stderr,
-) -> Build:
-    """Resolve build ids, tags, and optional numbers into a Build object
+## format_**() functions below return rich.Console-enabled format strings
+def format_flags(build: Build) -> str:
+    """Return build (info) as a string of rich'ly formatted symbols.
+
+    For example:
 
-    If abort_on_error is True and there is an error finding/calculating the build, then
-    an error is printed to sys.stderr and SystemExit is raised.
+        "* P  "
+
+    Which means that the build has packages built and is published.
     """
-    build = None
-    error = SystemExit(1)
+    assert build.info is not None
 
-    if build_id is None:
-        build = gbp.latest(machine)
-        if not build and abort_on_error:
-            print(f"No builds for {machine}", file=errorf)
-            raise error
-    elif build_id.startswith(TAG_SYM):
-        tag = build_id[1:]
-        build = gbp.resolve_tag(machine, tag)
-        if not build and abort_on_error:
-            print(f"No such tag for {machine}: {tag}", file=errorf)
-            raise error
-    elif build_id.isdigit():
-        build = Build(machine, int(build_id))
-    elif abort_on_error:
-        print(f"Invalid build ID: {build_id}", file=errorf)
-        raise error
-
-    if build is None:
-        raise ValueError(f"Invalid build ID: {build_id}")
+    return (
+        f"{'[package]*[/package]' if build.packages_built else ' '}"
+        f"{'[keep]K[/keep]' if build.info.keep else ' '}"
+        f"{'[published]P[/published]' if build.info.published else ' '}"
+        f"{'[note_flag]N[/note_flag]' if build.info.note else ' '}"
+    )
 
-    return build
 
+def format_build_number(number: int) -> str:
+    """Return the (build) number rich'ly formatted"""
+    return f"[build_id]{number}[/build_id]"
 
-def get_my_machines_from_args(args: argparse.Namespace) -> list[str]:
-    """Return the list of "my machines" attached to parsed args
 
-    If There are no return an empty list.
-    """
-    try:
-        return args.my_machines.split()
-    except AttributeError:
-        return []
+def format_timestamp(timestamp: dt.datetime) -> str:
+    """Return the timestamp rich'ly formatted"""
+    return f"[timestamp]{timestamp.strftime('%x %X')}[/timestamp]"
+
+
+def format_tags(tags: list[str]) -> str:
+    """Return the list of build tags rich'ly formatted"""
+    tag_list = [f"@{tag}" for tag in tags]
+
+    return f"[tag]{' '.join(tag_list)}[/tag]"
 
 
 def format_machine(machine: str, args: argparse.Namespace) -> str:
     """Format the given machine name for rich output
 
     If the given machine is given in the `my_machines` argument then it will have
     special styling.
     """
     pre, post = "", ""
 
-    if machine in get_my_machines_from_args(args):
+    if machine in utils.get_my_machines_from_args(args):
         pre = "[mymachine]"
         post = "[/mymachine]"
 
     return f"[machine]{pre}{machine}{post}[/machine]"
```

### Comparing `gbpcli-1.4.0/tests/__init__.py` & `gbpcli-1.5.0/tests/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,95 +1,92 @@
 """Tests for the Gentoo Build Publisher CLI"""
+# pylint: disable=protected-access
 import datetime
 import io
 import sys
 import unittest
 from functools import partial
 from json import dumps as stringify
 from json import loads as parse
 from pathlib import Path
 from typing import Any, Iterator
 from unittest import mock
 
 import requests
-from rich.console import Console
+import rich.console
 from rich.theme import Theme
 
-from gbpcli import DEFAULT_THEME, GBP
+from gbpcli import GBP, Console, graphql
+from gbpcli.theme import DEFAULT_THEME
 
 DATA_DIR = Path(__file__).resolve().parent / "data"
 LOCAL_TIMEZONE = datetime.timezone(datetime.timedelta(days=-1, seconds=61200), "PDT")
 NO_JSON = object()
 
 
 class TestCase(unittest.TestCase):
     """Custom test case for gbpcli"""
 
     def setUp(self):
         super().setUp()
 
         self.gbp = make_gbp()
-        self.console = MockConsole()
-        self.errorf = io.StringIO()
+        self.console = mock.Mock(spec=Console, out=MockConsole(), err=MockConsole())
 
     def make_response(self, data):
         """Add 200 json response to mock post
 
         This is like make_response() below except it assumes all responses are 200
         responses and all content is JSON. Additionally it can be called more than once
         and adds responses for subsequent calls. If called with `None` as an argument,
         then any previously configured responses are cleared
         """
         if data is None:
-            self.gbp.session.post.side_effect = None
+            self.gbp.query._session.post.side_effect = None
             return
 
         if isinstance(data, str):
             mock_json = parse(load_data(data))
         else:
             mock_json = data
 
-        if not self.gbp.session.post.side_effect:
-            self.gbp.session.post.side_effect = (make_response(json=mock_json),)
+        if not self.gbp.query._session.post.side_effect:
+            self.gbp.query._session.post.side_effect = (make_response(json=mock_json),)
         else:
-            self.gbp.session.post.side_effect = (
-                *self.gbp.session.post.side_effect,
+            self.gbp.query._session.post.side_effect = (
+                *self.gbp.query._session.post.side_effect,
                 make_response(json=mock_json),
             )
 
-    def assert_graphql(self, query: str, index=0, **variables):
+    def assert_graphql(self, query: graphql.Query, index=0, **variables):
         """Assert that self.gbp made a the given graphql query"""
-        calls = self.gbp.session.post.call_args_list
+        calls = self.gbp.query._session.post.call_args_list
 
         try:
             call = calls[index]
         except IndexError:
             self.fail("Query not called")
 
-        assert call[0] == (self.gbp.url,)
+        assert call[0] == (self.gbp.query._url,)
 
-        json = {"query": query, "variables": None}
-        expected = {"json": json, "headers": self.gbp.headers}
-
-        if variables:
-            json["variables"] = variables
+        json = {"query": str(query), "variables": variables}
+        expected = {"json": json, "headers": graphql.Query.headers}
 
         self.assertEqual(call[1], expected)
 
 
 def load_data(filename: str) -> bytes:
     """Read and return content from filename in the data directory"""
     return (DATA_DIR / filename).read_bytes()
 
 
 def load_ndjson(filename: str, start: int = 1) -> Iterator[Any]:
     """Iterate over a newline-delimited JSON file"""
     with open(DATA_DIR / filename, "r", encoding="UTF-8") as ndjson_file:
         for line_no, line in enumerate(ndjson_file, start=1):
-
             if line_no < start:
                 continue
 
             yield parse(line)
 
 
 def make_response(status_code=200, json=NO_JSON, content=None) -> requests.Response:
@@ -108,29 +105,31 @@
 
     return response
 
 
 def make_gbp(url: str = "http://test.invalid/") -> GBP:
     """Return a GBP instance with a mock session attribute"""
     gbp = GBP(url)
-    gbp.session = mock.Mock()
+    gbp.query._session = mock.Mock()
 
     return gbp
 
 
 class MockConsole:
     """Mock rich.console.Console
 
     Output is instead send to it's .stdout attribute, which is a StringIO.
     """
 
     def __init__(self):
-        self.stdout = io.StringIO()
-        self.console = Console(file=self.stdout, theme=Theme(DEFAULT_THEME))
+        self.string_io = io.StringIO()
+        self.console = rich.console.Console(
+            file=self.string_io, theme=Theme(DEFAULT_THEME)
+        )
 
     def print(self, *args, **kwargs):
         """Print to self.stdout"""
         return self.console.print(*args, **kwargs)
 
     def getvalue(self) -> str:
         """Return everying printed to the console"""
-        return self.stdout.getvalue()
+        return self.string_io.getvalue()
```

### Comparing `gbpcli-1.4.0/tests/data/diff.json` & `gbpcli-1.5.0/tests/data/diff.json`

 * *Files identical despite different names*

### Comparing `gbpcli-1.4.0/tests/data/inspect.ndjson` & `gbpcli-1.5.0/tests/data/inspect.ndjson`

 * *Files identical despite different names*

### Comparing `gbpcli-1.4.0/tests/data/list.json` & `gbpcli-1.5.0/tests/data/list.json`

 * *Files identical despite different names*

### Comparing `gbpcli-1.4.0/tests/data/list_with_packages.json` & `gbpcli-1.5.0/tests/data/list_with_packages.json`

 * *Files identical despite different names*

### Comparing `gbpcli-1.4.0/tests/data/machines.json` & `gbpcli-1.5.0/tests/data/machines.json`

 * *Files identical despite different names*

### Comparing `gbpcli-1.4.0/tests/data/packages.json` & `gbpcli-1.5.0/tests/data/packages.json`

 * *Files identical despite different names*

### Comparing `gbpcli-1.4.0/tests/data/packages.txt` & `gbpcli-1.5.0/tests/data/packages.txt`

 * *Files identical despite different names*

### Comparing `gbpcli-1.4.0/tests/data/status.json` & `gbpcli-1.5.0/tests/data/status.json`

 * *Files identical despite different names*

### Comparing `gbpcli-1.4.0/tests/test_build.py` & `gbpcli-1.5.0/tests/test_build.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 """Tests for the build subcommand"""
-# pylint: disable=missing-function-docstring
+# pylint: disable=missing-function-docstring,protected-access
 from argparse import Namespace
 
-from gbpcli import queries
 from gbpcli.subcommands.build import handler as build
 
 from . import TestCase
 
 
 class MachinesTestCase(TestCase):
     """machines() tests"""
 
     def test(self):
         args = Namespace(machine="babette")
         self.make_response("schedule_build.json")
 
-        status = build(args, self.gbp, self.console, self.errorf)
+        status = build(args, self.gbp, self.console)
 
         self.assertEqual(status, 0)
-        self.assertEqual(self.console.getvalue(), "")
-        self.assert_graphql(queries.schedule_build, machine="babette")
+        self.assertEqual(self.console.out.getvalue(), "")
+        self.assert_graphql(self.gbp.query.schedule_build, machine="babette")
```

### Comparing `gbpcli-1.4.0/tests/test_diff.py` & `gbpcli-1.5.0/tests/test_diff.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """Tests for the diff subcommand"""
-# pylint: disable=missing-function-docstring
+# pylint: disable=missing-function-docstring,protected-access
 from argparse import Namespace
 from json import loads as parse
 from unittest import mock
 
-from gbpcli import queries
+from gbpcli import graphql
 from gbpcli.subcommands.diff import handler as diff
 
 from . import LOCAL_TIMEZONE, TestCase, load_data, make_gbp, make_response
 
 
-@mock.patch("gbpcli.utils.LOCAL_TIMEZONE", new=LOCAL_TIMEZONE)
+@mock.patch("gbpcli.render.LOCAL_TIMEZONE", new=LOCAL_TIMEZONE)
 class DiffTestCase(TestCase):
     """diff() tests"""
 
     def test_should_display_diffs(self):
         args = Namespace(machine="lighthouse", left="3111", right="3112")
         self.make_response("diff.json")
 
-        status = diff(args, self.gbp, self.console, self.errorf)
+        status = diff(args, self.gbp, self.console)
 
         self.assertEqual(status, 0)
         expected = """\
 diff -r lighthouse/3111 lighthouse/3112
 --- a/lighthouse/3111 Sun Oct  2 12:10:02 2022 -0700
 +++ b/lighthouse/3112 Mon Oct  3 04:38:28 2022 -0700
 -app-accessibility/at-spi2-atk-2.38.0-1
@@ -32,105 +32,111 @@
 -dev-libs/atk-2.38.0-3
 +dev-libs/atk-2.46.0-1
 -dev-libs/libgusb-0.4.0-1
 +dev-libs/libgusb-0.4.1-1
 -sys-kernel/vanilla-sources-5.19.12-1
 +sys-kernel/vanilla-sources-6.0.0-1
 """
-        self.assertEqual(self.console.getvalue(), expected)
+        self.assertEqual(self.console.out.getvalue(), expected)
         self.assert_graphql(
-            queries.diff, left="lighthouse.3111", right="lighthouse.3112"
+            self.gbp.query.diff, left="lighthouse.3111", right="lighthouse.3112"
         )
 
     def test_should_print_nothing_when_no_diffs(self):
         args = Namespace(machine="lighthouse", left="3111", right="3111")
         no_diffs_json = parse(load_data("diff_no_content.json"))
         gbp = make_gbp()
-        gbp.session.post.return_value = make_response(json=no_diffs_json)
+        gbp.query._session.post.return_value = make_response(json=no_diffs_json)
 
-        diff(args, gbp, self.console, self.errorf)
+        diff(args, gbp, self.console)
 
-        self.assertEqual(self.console.getvalue(), "")
+        self.assertEqual(self.console.out.getvalue(), "")
 
     def test_when_right_is_none_should_use_latest(self):
         args = Namespace(machine="lighthouse", left="3111", right=None)
         latest_json = parse(load_data("latest.json"))
         mock_diff_json = parse(load_data("diff.json"))
         gbp = make_gbp()
-        gbp.session.post.side_effect = (
+        gbp.query._session.post.side_effect = (
             make_response(json=latest_json),
             make_response(json=mock_diff_json),
         )
 
-        status = diff(args, gbp, self.console, self.errorf)
+        status = diff(args, gbp, self.console)
 
         self.assertEqual(status, 0)
         expected_calls = [
             mock.call(
-                gbp.url,
-                json={"query": queries.latest, "variables": {"machine": "lighthouse"}},
-                headers=gbp.headers,
+                gbp.query._url,
+                json={
+                    "query": gbp.query.latest.query,
+                    "variables": {"machine": "lighthouse"},
+                },
+                headers=graphql.Query.headers,
             ),
             mock.call(
-                gbp.url,
+                gbp.query._url,
                 json={
-                    "query": queries.diff,
+                    "query": gbp.query.diff.query,
                     "variables": {
                         "left": "lighthouse.3111",
                         "right": "lighthouse.3113",
                     },
                 },
-                headers=gbp.headers,
+                headers=graphql.Query.headers,
             ),
         ]
-        gbp.session.post.assert_has_calls(expected_calls)
+        gbp.query._session.post.assert_has_calls(expected_calls)
 
     def test_when_left_is_none_should_use_published(self):
         args = Namespace(machine="lighthouse", left=None, right=None)
         list_json = parse(load_data("list.json"))
         mock_diff_json = parse(load_data("diff.json"))
         gbp = make_gbp()
-        gbp.session.post.side_effect = (
+        gbp.query._session.post.side_effect = (
             make_response(json=list_json),
             make_response(json=mock_diff_json),
         )
 
-        status = diff(args, gbp, self.console, self.errorf)
+        status = diff(args, gbp, self.console)
 
         self.assertEqual(status, 0)
         expected_calls = [
             mock.call(
-                gbp.url,
-                json={"query": queries.builds, "variables": {"machine": "lighthouse"}},
-                headers=gbp.headers,
+                gbp.query._url,
+                json={
+                    "query": gbp.query.builds.query,
+                    "variables": {"machine": "lighthouse"},
+                },
+                headers=graphql.Query.headers,
             ),
             mock.call(
-                gbp.url,
+                gbp.query._url,
                 json={
-                    "query": queries.diff,
+                    "query": gbp.query.diff.query,
                     "variables": {
                         "left": "lighthouse.10678",
                         "right": "lighthouse.10694",
                     },
                 },
-                headers=gbp.headers,
+                headers=graphql.Query.headers,
             ),
         ]
-        gbp.session.post.assert_has_calls(expected_calls)
+        gbp.query._session.post.assert_has_calls(expected_calls)
 
     def test_when_left_is_none_and_not_published(self):
         args = Namespace(machine="jenkins", left=None, right=None)
         list_json = parse(load_data("list.json"))
 
         # Make sure there are not published builds
         for item in list_json["data"]["builds"]:
             item["published"] = False
 
         self.make_response(list_json)
 
-        status = diff(args, self.gbp, self.console, self.errorf)
+        status = diff(args, self.gbp, self.console)
 
         self.assertEqual(status, 1)
-        self.assert_graphql(queries.builds, machine="jenkins")
+        self.assert_graphql(self.gbp.query.builds, machine="jenkins")
         self.assertEqual(
-            self.errorf.getvalue(), "No origin specified and no builds published\n"
+            self.console.err.getvalue(), "No origin specified and no builds published\n"
         )
```

### Comparing `gbpcli-1.4.0/tests/test_entrypoint.py` & `gbpcli-1.5.0/tests/test_entrypoint.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Tests for the main module"""
-# pylint: disable=missing-function-docstring
+# pylint: disable=missing-function-docstring,protected-access
 import argparse
 import importlib
 import sys
 import unittest
 from unittest import mock
 
-from gbpcli import APIError, build_parser, main
+from gbpcli import build_parser, main
+from gbpcli.graphql import APIError
 
 SUBCOMMANDS = [
     "build",
     "diff",
     "inspect",
     "keep",
     "latest",
@@ -50,40 +51,41 @@
 
 
 class MainTestCase(unittest.TestCase):
     """tests for the main function"""
 
     @mock.patch("gbpcli.GBP")
     @mock.patch("gbpcli.argparse.ArgumentParser.parse_args")
-    @mock.patch("gbpcli.rich.console.Console")
+    @mock.patch("gbpcli.Console")
     def test(self, console_mock, parse_args_mock, gbp_mock):
         parse_args_mock.return_value.url = "http://test.invalid/"
         func = parse_args_mock.return_value.func
         func.return_value = 0
         argv = ["status", "lighthouse"]
         status = main(argv)
 
         func.assert_called_once_with(
             parse_args_mock.return_value,
             gbp_mock.return_value,
             console_mock.return_value,
-            sys.stderr,
         )
         self.assertEqual(status, 0)
 
     def test_should_print_help_when_no_func(self):
         with mock.patch("gbpcli.argparse.ArgumentParser.print_help") as print_help_mock:
             status = main([])
 
         self.assertEqual(status, 1)
         print_help_mock.assert_called_once_with(file=sys.stderr)
 
     @mock.patch("gbpcli.GBP")
-    @mock.patch("gbpcli.print")
-    def test_should_print_to_stderr_and_exit_1_on_exception(self, print_mock, gbp_mock):
+    @mock.patch("gbpcli.rich.console.Console")
+    def test_should_print_to_stderr_and_exit_1_on_exception(
+        self, console_mock, gbp_mock
+    ):
         error = APIError("blah", {})
         message = "blah"
 
         gbp_mock.return_value.get_build_info.side_effect = error
         status = main(["status", "lighthouse"])
         self.assertEqual(status, 1)
-        print_mock.assert_called_once_with(message, file=sys.stderr)
+        console_mock.return_value.print.assert_called_once_with(message)
```

### Comparing `gbpcli-1.4.0/tests/test_gbp.py` & `gbpcli-1.5.0/tests/test_notes.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,189 +1,157 @@
-"""Tests for the GBP interface"""
-# pylint: disable=missing-docstring
+"""Tests for the notes subcommand"""
+# pylint: disable=missing-function-docstring,protected-access
 import os
+import subprocess
+from argparse import Namespace
 from unittest import mock
 
-import requests.exceptions
+from gbpcli.subcommands.notes import handler as create_note
 
-from gbpcli import DEFAULT_THEME, Queries, build_parser, get_colormap_from_string
+from . import LOCAL_TIMEZONE, TestCase
 
-from . import TestCase, make_response
+MODULE = "gbpcli.subcommands.notes"
+NOTE = "Hello world\n"
 
 
-class GBPQueryTestCase(TestCase):
-    """Tests for the .query method"""
+@mock.patch("gbpcli.render.LOCAL_TIMEZONE", new=LOCAL_TIMEZONE)
+class NotesTestCase(TestCase):
+    """notes tests"""
 
-    def test_passes_given_query_and_vars_to_graphql_request(self):
-        query = "query foo { bar }"
-        variables = {"name": "value"}
+    maxDiff = None
 
-        self.gbp.query(query, variables)
-
-        self.assert_graphql(query, name="value")
-
-    def test_raises_when_http_response_is_an_error(self):
-        query = "query foo { bar }"
-        response = make_response(status_code=404)
-        self.gbp.session.post.return_value = response
-
-        with self.assertRaises(requests.exceptions.HTTPError):
-            self.gbp.query(query)
-
-    def test_returns_graphql_data_and_errors(self):
-        query = "query foo { bar }"
-        data_and_errors = {"data": {"foo": "bar"}, "errors": [{"this": "that"}]}
-        self.make_response(data_and_errors)
-
-        response = self.gbp.query(query)
-
-        self.assertEqual(response, ({"foo": "bar"}, [{"this": "that"}]))
-
-    @mock.patch("gbpcli.print")
-    def test_exits_on_connection_errors(self, _):
-        query = "query foo { bar }"
-        self.gbp.session.post.side_effect = requests.exceptions.ConnectionError()
+    def setUp(self):
+        super().setUp()
 
-        with self.assertRaises(SystemExit) as cxt:
-            self.gbp.query(query)
+        self.args = Namespace(
+            machine="lighthouse", number="3109", delete=False, search=False
+        )
+        self.make_response("status.json")
+        self.make_response("create_note.json")
 
-        exception = cxt.exception
-        self.assertEqual(exception.args, (-1,))
+    def assert_create_note(self, machine="lighthouse", number="3109", note=NOTE):
+        """Assert that the note was created by a GraphQL request"""
+        self.assert_graphql(self.gbp.query.build, index=0, id=f"{machine}.{number}")
+        self.assert_graphql(
+            self.gbp.query.create_note, id=f"{machine}.{number}", index=1, note=note
+        )
 
-    def test_does_not_exit_when_flag_turned_off(self):
-        self.gbp.exit_gracefully_on_requests_errors = False
-        error = requests.exceptions.ConnectionError()
-        self.gbp.session.post.side_effect = error
-        query = "query foo { bar }"
+    def test_create_with_editor(self):
+        editor = fake_editor()
 
-        with self.assertRaises(requests.exceptions.ConnectionError) as cxt:
-            self.gbp.query(query)
+        with mock.patch(f"{MODULE}.sys.stdin.isatty", return_value=True):
+            with mock.patch(f"{MODULE}.subprocess.run", wraps=editor) as run:
+                with mock.patch.dict(os.environ, {"EDITOR": "foo"}, clear=True):
+                    status = create_note(self.args, self.gbp, self.console)
 
-        self.assertIs(cxt.exception, error)
+        self.assertEqual(status, 0)
+        self.assert_create_note()
+        run.assert_called_once_with(["foo", mock.ANY], check=False)
 
+    def test_create_with_editor_but_editor_fails_does_not_create_note(self):
+        editor = fake_editor(returncode=1)
 
-class QueriesTestCase(TestCase):
-    """Tests for the Queries wrapper"""
+        with mock.patch(f"{MODULE}.sys.stdin.isatty", return_value=True):
+            with mock.patch(f"{MODULE}.subprocess.run", wraps=editor) as run:
+                with mock.patch.dict(os.environ, {"VISUAL": "foo"}, clear=True):
+                    status = create_note(self.args, self.gbp, self.console)
 
-    def test_returns_query_on_attribute_access(self):
-        queries = Queries()
+        self.assertEqual(status, 1)
+        self.assertEqual(self.gbp.query._session.post.call_count, 1)
+        run.assert_called_once_with(["foo", mock.ANY], check=False)
 
-        logs_query = queries.logs
+    def test_when_isatty_but_no_editor_reads_from_stdin(self):
+        with mock.patch(f"{MODULE}.sys.stdin.isatty", return_value=True):
+            with mock.patch.dict(os.environ, {}, clear=True):
+                with mock.patch(f"{MODULE}.sys.stdin.read", return_value=NOTE):
+                    status = create_note(self.args, self.gbp, self.console)
 
-        self.assertEqual(
-            logs_query, "query ($id: ID!) {\n  build(id: $id) {\n    logs\n  }\n}\n"
-        )
+        self.assertEqual(status, 0)
+        self.assert_create_note()
 
-    def test_raises_attribute_error_when_file_not_found(self):
-        queries = Queries()
+    def test_delete_deletes_note(self):
+        self.args.delete = True
+        create_note(self.args, self.gbp, self.console)
 
-        with self.assertRaises(AttributeError):
-            queries.bogus  # pylint: disable=pointless-statement
+        self.assert_create_note(note=None)
 
-    def test_to_dict_returns_dict(self):
-        queries = Queries()
+    def test_create_with_no_tty(self):
+        self.make_response("status.json")
+        self.make_response("create_note.json")
 
-        as_dict = queries.to_dict()
+        with mock.patch(f"{MODULE}.sys.stdin.isatty", return_value=False):
+            with mock.patch(f"{MODULE}.sys.stdin.read", return_value=NOTE):
+                create_note(self.args, self.gbp, self.console)
 
-        self.assertIsInstance(as_dict, dict)
-        self.assertIn("logs", as_dict)
+        self.assert_create_note()
 
+    def test_should_print_error_when_build_does_not_exist(self):
+        self.make_response(None)
+        self.make_response({"data": {"build": None}})
 
-class GetColormapFromString(TestCase):
-    """Tests for the get_colormap_from_string function"""
+        status = create_note(self.args, self.gbp, self.console)
 
-    def test_empty_string(self):
-        result = get_colormap_from_string("")
+        self.assertEqual(status, 1)
+        self.assertEqual(self.console.err.getvalue(), "Build not found\n")
 
-        self.assertEqual(result, DEFAULT_THEME)
+    def test_should_print_error_when_invalid_number_given(self):
+        self.args.number = "foo"
 
-    def test_double_colons(self):
-        string = "header=test_header:note=test_note::build_id=test_build_id"
-        #                                          ^^
-        result = get_colormap_from_string(string)
+        with self.assertRaises(SystemExit) as context:
+            create_note(self.args, self.gbp, self.console)
 
-        self.assertEqual(result["header"], "test_header")
-        self.assertEqual(result["note"], "test_note")
-        self.assertEqual(result["build_id"], "test_build_id")
+        self.assertEqual(context.exception.args, ("Invalid build ID: foo",))
 
-    def test_double_equals(self):
-        string = "header=blue:notes==white:build_id=bold"
-        #                          ^^
+    def test_search_notes(self):
+        self.args.search = True
+        self.args.number = "10,000"
+        self.make_response(None)
+        self.make_response("search_notes.json")
 
-        with self.assertRaises(ValueError) as context:
-            get_colormap_from_string(string)
+        status = create_note(self.args, self.gbp, self.console)
 
-        self.assertEqual(
-            str(context.exception),
-            "Invalid color map: 'header=blue:notes==white:build_id=bold'",
+        self.assertEqual(status, 0)
+        self.assert_graphql(
+            self.gbp.query.search, machine="lighthouse", field="NOTES", key="10,000"
         )
+        self.assertEqual(self.console.out.getvalue(), EXPECTED_SEARCH_OUTPUT)
 
-    def test_missing_equals(self):
-        string = "header=test_header:note:build_id=test_build_id"
-        #                                ^
-
-        with self.assertRaises(ValueError) as context:
-            get_colormap_from_string(string)
-
-        self.assertEqual(
-            str(context.exception),
-            "Invalid color map: 'header=test_header:note:build_id=test_build_id'",
+    def test_search_no_matches_found(self):
+        self.args.search = True
+        self.args.number = "python"
+        self.make_response(None)
+        self.make_response({"data": {"search": []}})
+
+        status = create_note(self.args, self.gbp, self.console)
+
+        self.assertEqual(status, 1)
+        self.assert_graphql(
+            self.gbp.query.search, machine="lighthouse", field="NOTES", key="python"
         )
+        self.assertEqual(self.console.err.getvalue(), "No matches found\n")
 
-    def test_only_colons(self):
-        result = get_colormap_from_string("::::::::::")
-
-        self.assertEqual(result, DEFAULT_THEME)
-
-    def test_garbage_input(self):
-        with self.assertRaises(ValueError) as context:
-            get_colormap_from_string("This is totally garbage!")
-
-        self.assertEqual(
-            str(context.exception),
-            "Invalid color map: 'This is totally garbage!'",
-        )
-
-    def test_ignores_unknown_names(self):
-        string = "header=test_header:note=test_note:unknown=test_unknown"
-
-        result = get_colormap_from_string(string)
-
-        self.assertEqual(result["header"], "test_header")
-        self.assertEqual(result["note"], "test_note")
-        self.assertFalse("unknown" in result)
-
-
-class BuildParserTestCase(TestCase):
-    """Tests for the build_parser method"""
-
-    def setUp(self):
-        super().setUp()
-
-        patch = mock.patch.dict(os.environ, clear=True)
-        self.addCleanup(patch.stop)
-        patch.start()
-
-    def test_my_machines_string(self):
-        argv = ["--my-machines", "this that the other"]
 
-        parser = build_parser()
-        args = parser.parse_args(argv)
+def fake_editor(text=NOTE, returncode=0):
+    def edit(args, check=False):
+        if check and returncode != 0:
+            raise subprocess.CalledProcessError(returncode, args)
 
-        self.assertEqual(args.my_machines, "this that the other")
+        with open(args[1], "w", encoding="utf-8") as note_file:
+            note_file.write(text)
 
-    def test_my_machines_not_passed(self):
-        argv = []
+        return mock.Mock(args=args, returncode=returncode)
 
-        parser = build_parser()
-        args = parser.parse_args(argv)
+    return edit
 
-        self.assertEqual(args.my_machines, "")
 
-    def test_my_machines_from_environ(self):
-        os.environ["GBPCLI_MYMACHINES"] = "this that the other"
-        argv = []
+EXPECTED_SEARCH_OUTPUT = """\
+Build: lighthouse/10000
+Submitted: Thu Sep  1 09:28:12 2022 -0700
+Completed: Thu Sep  1 09:47:34 2022 -0700
+Published: no
+Keep: yes
+Tags: 10000
+Packages-built: None
 
-        parser = build_parser()
-        args = parser.parse_args(argv)
+This is a note!
 
-        self.assertEqual(args.my_machines, "this that the other")
+"""
```

### Comparing `gbpcli-1.4.0/tests/test_inspect.py` & `gbpcli-1.5.0/tests/test_inspect.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 """Tests for the inspect subcommand"""
-# pylint: disable=missing-function-docstring
+# pylint: disable=missing-function-docstring,protected-access
 from argparse import Namespace
 from unittest import mock
 
-from gbpcli import queries
 from gbpcli.subcommands.inspect import handler as inspect
 
 from . import LOCAL_TIMEZONE, TestCase, load_ndjson
 
 
-@mock.patch("gbpcli.LOCAL_TIMEZONE", new=LOCAL_TIMEZONE)
-@mock.patch("gbpcli.subcommands.inspect.LOCAL_TIMEZONE", new=LOCAL_TIMEZONE)
+@mock.patch("gbpcli.render.LOCAL_TIMEZONE", new=LOCAL_TIMEZONE)
 class InspectTestCase(TestCase):
     """inspect() tests"""
 
     maxDiff = None
 
     def test_entire_tree(self):
         args = Namespace(machine=None, tail=0, mine=False)
@@ -26,74 +24,78 @@
 
         machines_count = len(machines_response["data"]["machines"])
         assert machines_count == 2
 
         for _ in range(machines_count):
             make_response(next(graphql_responses))
 
-        status = inspect(args, self.gbp, self.console, self.errorf)
+        status = inspect(args, self.gbp, self.console)
 
         self.assertEqual(status, 0)
-        self.assertEqual(self.console.getvalue(), INSPECT_ALL)
-        self.assert_graphql(queries.machine_names)
-        self.assert_graphql(queries.builds_with_packages, index=1, machine="base")
-        self.assert_graphql(queries.builds_with_packages, index=2, machine="gbpbox")
+        self.assertEqual(self.console.out.getvalue(), INSPECT_ALL)
+        self.assert_graphql(self.gbp.query.machine_names)
+        self.assert_graphql(
+            self.gbp.query.builds_with_packages, index=1, machine="base"
+        )
+        self.assert_graphql(
+            self.gbp.query.builds_with_packages, index=2, machine="gbpbox"
+        )
 
     def test_single_machine(self):
         args = Namespace(machine=["base"], tail=0)
         graphql_responses = load_ndjson("inspect.ndjson", start=4)
         make_response = self.make_response
 
         response = next(graphql_responses)
         make_response(response)
 
-        status = inspect(args, self.gbp, self.console, self.errorf)
+        status = inspect(args, self.gbp, self.console)
 
         self.assertEqual(status, 0)
-        self.assertEqual(self.console.getvalue(), INSPECT_SINGLE)
-        self.assert_graphql(queries.builds_with_packages, machine="base")
+        self.assertEqual(self.console.out.getvalue(), INSPECT_SINGLE)
+        self.assert_graphql(self.gbp.query.builds_with_packages, machine="base")
 
     def test_single_machine_with_tail(self):
         args = Namespace(machine=["base"], tail=2)
         graphql_responses = load_ndjson("inspect.ndjson", start=5)
         make_response = self.make_response
 
         response = next(graphql_responses)
         make_response(response)
 
-        status = inspect(args, self.gbp, self.console, self.errorf)
+        status = inspect(args, self.gbp, self.console)
 
         self.assertEqual(status, 0)
-        self.assertEqual(self.console.getvalue(), INSPECT_SINGLE_WITH_TAIL)
-        self.assert_graphql(queries.builds_with_packages, machine="base")
+        self.assertEqual(self.console.out.getvalue(), INSPECT_SINGLE_WITH_TAIL)
+        self.assert_graphql(self.gbp.query.builds_with_packages, machine="base")
 
     def test_single_machine_with_build_id(self):
         args = Namespace(machine=["lighthouse.12672"])
 
         self.make_response("lighthouse.12672.json")
 
-        status = inspect(args, self.gbp, self.console, self.errorf)
+        status = inspect(args, self.gbp, self.console)
 
         self.assertEqual(status, 0)
-        self.assertEqual(self.console.getvalue(), INSPECT_SINGLE_WITH_BUILD_ID)
-        self.assert_graphql(queries.build, id="lighthouse.12672")
+        self.assertEqual(self.console.out.getvalue(), INSPECT_SINGLE_WITH_BUILD_ID)
+        self.assert_graphql(self.gbp.query.build, id="lighthouse.12672")
 
     def test_with_mine(self):
         args = Namespace(machine=None, mine=True, tail=0, my_machines="base")
         graphql_responses = load_ndjson("inspect.ndjson", start=4)
         make_response = self.make_response
 
         response = next(graphql_responses)
         make_response(response)
 
-        status = inspect(args, self.gbp, self.console, self.errorf)
+        status = inspect(args, self.gbp, self.console)
 
         self.assertEqual(status, 0)
-        self.assertEqual(self.console.getvalue(), INSPECT_SINGLE)
-        self.assert_graphql(queries.builds_with_packages, machine="base")
+        self.assertEqual(self.console.out.getvalue(), INSPECT_SINGLE)
+        self.assert_graphql(self.gbp.query.builds_with_packages, machine="base")
 
 
 INSPECT_SINGLE_WITH_TAIL = """\
 Machines
 └── base
     ├── 1 (10/10/22 04:55:19) @first
     │   ├── dev-libs/libpcre-8.45-r1 (05:00:50)
```

### Comparing `gbpcli-1.4.0/tests/test_keep.py` & `gbpcli-1.5.0/tests/test_keep.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,48 +1,47 @@
 """Tests for the keep subcommand"""
-# pylint: disable=missing-function-docstring
+# pylint: disable=missing-function-docstring,protected-access
 from argparse import Namespace
 
-from gbpcli import queries
 from gbpcli.subcommands.keep import handler as keep
 
 from . import TestCase
 
 
 class KeepTestCase(TestCase):
     """keep() tests"""
 
     maxDiff = None
 
     def test_keep(self):
         args = Namespace(machine="lighthouse", number="3210", release=False)
         self.make_response("keep_build.json")
 
-        status = keep(args, self.gbp, self.console, self.errorf)
+        status = keep(args, self.gbp, self.console)
 
         self.assertEqual(status, 0)
-        self.assert_graphql(queries.keep_build, id="lighthouse.3210")
+        self.assert_graphql(self.gbp.query.keep_build, id="lighthouse.3210")
 
     def test_keep_should_print_error_when_build_does_not_exist(self):
         args = Namespace(machine="lighthouse", number="3210", release=False)
         self.make_response({"data": {"keepBuild": None}})
 
-        status = keep(args, self.gbp, self.console, self.errorf)
+        status = keep(args, self.gbp, self.console)
         self.assertEqual(status, 1)
-        self.assertEqual(self.errorf.getvalue(), "Not Found\n")
+        self.assertEqual(self.console.err.getvalue(), "Not Found\n")
 
     def test_release(self):
         args = Namespace(machine="lighthouse", number="3210", release=True)
         self.make_response("release_build.json")
 
-        status = keep(args, self.gbp, self.console, self.errorf)
+        status = keep(args, self.gbp, self.console)
 
         self.assertEqual(status, 0)
-        self.assert_graphql(queries.release_build, id="lighthouse.3210")
+        self.assert_graphql(self.gbp.query.release_build, id="lighthouse.3210")
 
     def test_release_should_print_error_when_build_does_not_exist(self):
         args = Namespace(machine="lighthouse", number="3210", release=True)
         self.make_response({"data": {"releaseBuild": None}})
 
-        status = keep(args, self.gbp, self.console, self.errorf)
+        status = keep(args, self.gbp, self.console)
         self.assertEqual(status, 1)
-        self.assertEqual(self.errorf.getvalue(), "Not Found\n")
+        self.assertEqual(self.console.err.getvalue(), "Not Found\n")
```

### Comparing `gbpcli-1.4.0/tests/test_latest.py` & `gbpcli-1.5.0/tests/test_latest.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 """Tests for the latest subcommand"""
-# pylint: disable=missing-function-docstring
+# pylint: disable=missing-function-docstring,protected-access
 from argparse import Namespace
 from unittest import mock
 
-from gbpcli import queries
 from gbpcli.subcommands.latest import handler as latest
 
 from . import LOCAL_TIMEZONE, TestCase
 
 
-@mock.patch("gbpcli.LOCAL_TIMEZONE", new=LOCAL_TIMEZONE)
+@mock.patch("gbpcli.render.LOCAL_TIMEZONE", new=LOCAL_TIMEZONE)
 class LatestTestCase(TestCase):
     """latest() tests"""
 
     def test(self):
         args = Namespace(machine="lighthouse")
         self.make_response("latest.json")
 
-        status = latest(args, self.gbp, self.console, self.errorf)
+        status = latest(args, self.gbp, self.console)
 
         self.assertEqual(status, 0)
         expected = "3113\n"
-        self.assertEqual(self.console.getvalue(), expected)
-        self.assert_graphql(queries.latest, machine="lighthouse")
+        self.assertEqual(self.console.out.getvalue(), expected)
+        self.assert_graphql(self.gbp.query.latest, machine="lighthouse")
 
     def test_should_print_error_when_not_found(self):
         args = Namespace(machine="bogus")
         self.make_response({"data": {"latest": None}})
 
-        status = latest(args, self.gbp, self.console, self.errorf)
+        status = latest(args, self.gbp, self.console)
 
         self.assertEqual(status, 1)
         self.assertEqual(
-            self.errorf.getvalue(), "No builds exist for the given machine\n"
+            self.console.err.getvalue(), "No builds exist for the given machine\n"
         )
```

### Comparing `gbpcli-1.4.0/tests/test_list.py` & `gbpcli-1.5.0/tests/test_list.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 """Tests for the list subcommand"""
-# pylint: disable=missing-function-docstring
+# pylint: disable=missing-function-docstring,protected-access
 from argparse import Namespace
 from unittest import mock
 
-from gbpcli import queries
 from gbpcli.subcommands.list import handler as list_command
 
 from . import LOCAL_TIMEZONE, TestCase
 
 
-@mock.patch("gbpcli.subcommands.list.LOCAL_TIMEZONE", new=LOCAL_TIMEZONE)
+@mock.patch("gbpcli.render.LOCAL_TIMEZONE", new=LOCAL_TIMEZONE)
 class ListTestCase(TestCase):
     """list() tests"""
 
     maxDiff = None
 
     def test(self):
         args = Namespace(machine="jenkins")
         self.make_response("list_with_packages.json")
 
-        status = list_command(args, self.gbp, self.console, self.errorf)
+        status = list_command(args, self.gbp, self.console)
 
         self.assertEqual(status, 0)
-        self.assertEqual(self.console.getvalue(), EXPECTED_OUTPUT)
-        self.assert_graphql(queries.builds_with_packages, machine="jenkins")
+        self.assertEqual(self.console.out.getvalue(), EXPECTED_OUTPUT)
+        self.assert_graphql(self.gbp.query.builds_with_packages, machine="jenkins")
 
 
 EXPECTED_OUTPUT = """\
                     💻 jenkins                    
 ╭───────┬────┬───────────────────┬───────────────╮
 │ Flags │ ID │ Built             │ Tags          │
 ├───────┼────┼───────────────────┼───────────────┤
```

### Comparing `gbpcli-1.4.0/tests/test_logs.py` & `gbpcli-1.5.0/tests/test_publish.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,32 @@
-"""Tests for the logs subcommand"""
-# pylint: disable=missing-function-docstring
+"""Tests for the publish subcommand"""
+# pylint: disable=missing-function-docstring,protected-access
 from argparse import Namespace
 from unittest import mock
 
-from gbpcli import queries
-from gbpcli.subcommands.logs import handler as logs
+from gbpcli.subcommands.publish import handler as publish
 
 from . import LOCAL_TIMEZONE, TestCase
 
 
-@mock.patch("gbpcli.LOCAL_TIMEZONE", new=LOCAL_TIMEZONE)
-class LogsTestCase(TestCase):
-    """logs() tests"""
+@mock.patch("gbpcli.render.LOCAL_TIMEZONE", new=LOCAL_TIMEZONE)
+class PublishTestCase(TestCase):
+    """publish() tests"""
 
     def test(self):
-        args = Namespace(machine="lighthouse", number="3113")
-        self.make_response("logs.json")
+        args = Namespace(machine="lighthouse", number="3109")
+        self.make_response("publish.json")
 
-        status = logs(args, self.gbp, self.console, self.errorf)
+        publish(args, self.gbp, self.console)
 
-        self.assertEqual(status, 0)
-        self.assertEqual(self.console.getvalue(), "This is a test!\n")
-        self.assert_graphql(queries.logs, id="lighthouse.3113")
+        self.assert_graphql(self.gbp.query.publish, id="lighthouse.3109")
 
-    def test_should_print_error_when_logs_dont_exist(self):
-        args = Namespace(machine="lighthouse", number="9999")
-        self.make_response({"data": {"build": None}})
+    def test_should_get_latest_when_number_is_none(self):
+        args = Namespace(machine="lighthouse", number=None)
+        self.make_response({"data": {"latest": {"id": "lighthouse.2080"}}})
+        self.make_response("publish.json")
 
-        status = logs(args, self.gbp, self.console, self.errorf)
+        status = publish(args, self.gbp, self.console)
 
-        self.assertEqual(self.errorf.getvalue(), "Not Found\n")
-        self.assertEqual(status, 1)
+        self.assertEqual(status, 0)
+        self.assert_graphql(self.gbp.query.latest, index=0, machine="lighthouse")
+        self.assert_graphql(self.gbp.query.publish, index=1, id="lighthouse.2080")
```

### Comparing `gbpcli-1.4.0/tests/test_machines.py` & `gbpcli-1.5.0/tests/test_machines.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,50 +1,49 @@
 """Tests for the machines subcommand"""
-# pylint: disable=missing-function-docstring
+# pylint: disable=missing-function-docstring,protected-access
 from argparse import Namespace
 from unittest import mock
 
-from gbpcli import queries
 from gbpcli.subcommands.machines import handler as machines
 
 from . import LOCAL_TIMEZONE, TestCase
 
 
-@mock.patch("gbpcli.LOCAL_TIMEZONE", new=LOCAL_TIMEZONE)
+@mock.patch("gbpcli.render.LOCAL_TIMEZONE", new=LOCAL_TIMEZONE)
 class MachinesTestCase(TestCase):
     """machines() tests"""
 
     def test(self):
         args = Namespace(mine=False)
         self.make_response("machines.json")
 
-        status = machines(args, self.gbp, self.console, self.errorf)
+        status = machines(args, self.gbp, self.console)
 
         self.assertEqual(status, 0)
-        self.assertEqual(self.console.getvalue(), EXPECTED_OUTPUT)
-        self.assert_graphql(queries.machines)
+        self.assertEqual(self.console.out.getvalue(), EXPECTED_OUTPUT)
+        self.assert_graphql(self.gbp.query.machines)
 
     def test_with_mine(self):
         args = Namespace(mine=True, my_machines="babette lighthouse")
         self.make_response("machines.json")
 
-        status = machines(args, self.gbp, self.console, self.errorf)
+        status = machines(args, self.gbp, self.console)
 
         self.assertEqual(status, 0)
         expected = """\
            2 Machines           
 ╭────────────┬────────┬────────╮
 │ Machine    │ Builds │ Latest │
 ├────────────┼────────┼────────┤
 │ babette    │     14 │    631 │
 │ lighthouse │     29 │  10694 │
 ╰────────────┴────────┴────────╯
 """
-        self.assertEqual(self.console.getvalue(), expected)
-        self.assert_graphql(queries.machines)
+        self.assertEqual(self.console.out.getvalue(), expected)
+        self.assert_graphql(self.gbp.query.machines)
 
 
 EXPECTED_OUTPUT = """\
            7 Machines           
 ╭────────────┬────────┬────────╮
 │ Machine    │ Builds │ Latest │
 ├────────────┼────────┼────────┤
```

### Comparing `gbpcli-1.4.0/tests/test_packages.py` & `gbpcli-1.5.0/tests/test_packages.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 """Tests for the packages subcommand"""
-# pylint: disable=missing-function-docstring
+# pylint: disable=missing-function-docstring,protected-access
 from argparse import Namespace
 
-from gbpcli import queries
 from gbpcli.subcommands.packages import handler as packages
 
 from . import TestCase, load_data
 
 
 class PackagesTestCase(TestCase):
     """packages() tests"""
 
     maxDiff = None
 
     def test(self):
         args = Namespace(machine="babette", number="268")
         self.make_response("packages.json")
 
-        status = packages(args, self.gbp, self.console, self.errorf)
+        status = packages(args, self.gbp, self.console)
 
         self.assertEqual(status, 0)
         expected = load_data("packages.txt").decode("utf-8")
-        self.assertEqual(self.console.getvalue(), expected)
-        self.assert_graphql(queries.packages, id="babette.268")
+        self.assertEqual(self.console.out.getvalue(), expected)
+        self.assert_graphql(self.gbp.query.packages, id="babette.268")
 
     def test_when_build_does_not_exist_prints_error(self):
         args = Namespace(machine="bogus", number="268")
         no_build = {"data": {"build": {"packages": None}}}
         self.make_response(no_build)
 
-        status = packages(args, self.gbp, self.console, self.errorf)
+        status = packages(args, self.gbp, self.console)
 
         self.assertEqual(status, 1)
-        self.assertEqual(self.errorf.getvalue(), "Not Found\n")
+        self.assertEqual(self.console.err.getvalue(), "Not Found\n")
```

### Comparing `gbpcli-1.4.0/tests/test_pull.py` & `gbpcli-1.5.0/tests/test_pull.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 """Tests for the pull subcommand"""
-# pylint: disable=missing-function-docstring
+# pylint: disable=missing-function-docstring,protected-access
 from argparse import Namespace
 from unittest import mock
 
-from gbpcli import queries
 from gbpcli.subcommands.pull import handler as pull
 
 from . import LOCAL_TIMEZONE, TestCase
 
 
-@mock.patch("gbpcli.LOCAL_TIMEZONE", new=LOCAL_TIMEZONE)
+@mock.patch("gbpcli.render.LOCAL_TIMEZONE", new=LOCAL_TIMEZONE)
 class PullTestCase(TestCase):
     """pull() tests"""
 
     def test(self):
         args = Namespace(machine="lighthouse", number="3226")
         self.make_response("pull.json")
 
-        pull(args, self.gbp, self.console, self.errorf)
+        pull(args, self.gbp, self.console)
 
-        self.assert_graphql(queries.pull, id="lighthouse.3226")
+        self.assert_graphql(self.gbp.query.pull, id="lighthouse.3226")
```

### Comparing `gbpcli-1.4.0/tests/test_status.py` & `gbpcli-1.5.0/tests/test_status.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 """Tests for the status subcommand"""
-# pylint: disable=missing-function-docstring
+# pylint: disable=missing-function-docstring,protected-access
 from argparse import Namespace
 from unittest import mock
 
-from gbpcli import queries
 from gbpcli.subcommands.status import handler as status
 
 from . import LOCAL_TIMEZONE, TestCase
 
 
-@mock.patch("gbpcli.utils.LOCAL_TIMEZONE", new=LOCAL_TIMEZONE)
+@mock.patch("gbpcli.render.LOCAL_TIMEZONE", new=LOCAL_TIMEZONE)
 class StatusTestCase(TestCase):
     """status() tests"""
 
     maxDiff = None
 
     def test(self):
         args = Namespace(machine="lighthouse", number="3587")
         self.make_response("status.json")
 
-        status(args, self.gbp, self.console, self.errorf)
+        status(args, self.gbp, self.console)
 
         expected = """\
 ╭────────────────────────────────────────────────╮
 │ Build:          lighthouse 3587                │
 │ Submitted:      Fri Nov 12 21:25:53 2021 -0700 │
 │ Completed:      Fri Nov 12 21:29:34 2021 -0700 │
 │ Published:      no                             │
@@ -36,29 +35,29 @@
 ╭─────────────────────╮
 │📎 Notes             │
 ├─────────────────────┤
 │This is a build note.│
 │Hello world!         │
 ╰─────────────────────╯
 """
-        self.assertEqual(self.console.getvalue(), expected)
-        self.assert_graphql(queries.build, id="lighthouse.3587")
+        self.assertEqual(self.console.out.getvalue(), expected)
+        self.assert_graphql(self.gbp.query.build, id="lighthouse.3587")
 
     def test_should_get_latest_when_number_is_none(self):
         args = Namespace(machine="lighthouse", number=None)
         self.make_response({"data": {"latest": {"id": "lighthouse.3587"}}})
         self.make_response("status.json")
 
-        return_status = status(args, self.gbp, self.console, self.errorf)
+        return_status = status(args, self.gbp, self.console)
 
-        self.assert_graphql(queries.latest, index=0, machine="lighthouse")
-        self.assert_graphql(queries.build, index=1, id="lighthouse.3587")
+        self.assert_graphql(self.gbp.query.latest, index=0, machine="lighthouse")
+        self.assert_graphql(self.gbp.query.build, index=1, id="lighthouse.3587")
         self.assertEqual(return_status, 0)
 
     def test_should_print_error_when_build_does_not_exist(self):
         args = Namespace(machine="bogus", number="934")
         self.make_response({"data": {"build": None}})
 
-        return_status = status(args, self.gbp, self.console, self.errorf)
+        return_status = status(args, self.gbp, self.console)
 
         self.assertEqual(return_status, 1)
-        self.assertEqual(self.errorf.getvalue(), "Not found\n")
+        self.assertEqual(self.console.err.getvalue(), "Not found\n")
```

### Comparing `gbpcli-1.4.0/tests/test_tag.py` & `gbpcli-1.5.0/tests/test_tag.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,52 @@
 """Tests for the tag subcommand"""
-# pylint: disable=missing-docstring
+# pylint: disable=missing-docstring,protected-access
 from argparse import Namespace
 
-from gbpcli import queries
 from gbpcli.subcommands.tag import handler as tag
 
 from . import TestCase
 
 
 class TagTestCase(TestCase):
     """tag() tests"""
 
     def test_tag(self):
         args = Namespace(machine="lighthouse", number="9400", tag="prod", remove=False)
         self.make_response("tag_build.json")
 
-        status = tag(args, self.gbp, self.console, self.errorf)
+        status = tag(args, self.gbp, self.console)
 
         self.assertEqual(status, 0)
-        self.assert_graphql(queries.tag_build, id="lighthouse.9400", tag="prod")
+        self.assert_graphql(self.gbp.query.tag_build, id="lighthouse.9400", tag="prod")
 
     def test_untag(self):
         args = Namespace(machine="lighthouse", number=None, tag="prod", remove=True)
         self.make_response("untag_build.json")
 
-        status = tag(args, self.gbp, self.console, self.errorf)
+        status = tag(args, self.gbp, self.console)
 
         self.assertEqual(status, 0)
-        self.assert_graphql(queries.untag_build, machine="lighthouse", tag="prod")
+        self.assert_graphql(
+            self.gbp.query.untag_build, machine="lighthouse", tag="prod"
+        )
 
     def test_untag_with_string_starting_with_tagsym_works(self):
         args = Namespace(machine="lighthouse", number=None, tag="@prod", remove=True)
         self.make_response("untag_build.json")
 
-        status = tag(args, self.gbp, self.console, self.errorf)
+        status = tag(args, self.gbp, self.console)
 
         self.assertEqual(status, 0)
-        self.assert_graphql(queries.untag_build, machine="lighthouse", tag="prod")
+        self.assert_graphql(
+            self.gbp.query.untag_build, machine="lighthouse", tag="prod"
+        )
 
     def test_untag_with_build_number_gives_error(self):
         args = Namespace(machine="lighthouse", number="9400", tag="prod", remove=True)
 
-        status = tag(args, self.gbp, self.console, self.errorf)
+        status = tag(args, self.gbp, self.console)
 
         self.assertEqual(status, 1)
         self.assertEqual(
-            self.errorf.getvalue(), "When removing a tag, omit the build number\n"
+            self.console.err.getvalue(), "When removing a tag, omit the build number\n"
         )
```

### Comparing `gbpcli-1.4.0/PKG-INFO` & `gbpcli-1.5.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 Metadata-Version: 2.1
 Name: gbpcli
-Version: 1.4.0
+Version: 1.5.0
 Summary: Gentoo Build Publisher Command-Line Interface
+Home-page: https://github.com/enku/gbpcli
+Author-Email: Albert Hopkins <marduk@letterboxes.org>
 License: GPL3+
-Author-email: Albert Hopkins <marduk@letterboxes.org>
-Requires-Python: >=3.10
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: System :: Software Distribution
-Project-URL: homepage, https://github.com/enku/gbpcli
-Project-URL: repository, https://github.com/enku/gbpcli
+Classifier: Programming Language :: Python :: 3
+Project-URL: Homepage, https://github.com/enku/gbpcli
+Project-URL: Repository, https://github.com/enku/gbpcli
+Requires-Python: >=3.10
+Requires-Dist: requests
+Requires-Dist: rich>=12.5.1
+Requires-Dist: yarl
 Description-Content-Type: text/markdown
 
 # CLI for Gentoo Build Publisher
 
 <div align="center">
 
 [![asciicast](https://asciinema.org/a/8oqcjBoC6Miy2MJlqb8gm1UwY.svg)](https://asciinema.org/a/8oqcjBoC6Miy2MJlqb8gm1UwY)
@@ -119,8 +123,7 @@
 
 The `build` subcommand can schedule a build in CI/CD for the given machine,
 e.g.:
 
 ```bash
 $ gbp build babette
 ```
-
```

