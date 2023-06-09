# Comparing `tmp/tspublisher-0.0.1.dev962.tar.gz` & `tmp/tspublisher-0.0.1.dev973.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tspublisher-0.0.1.dev962.tar", last modified: Thu Jun 21 11:31:50 2018, max compression
+gzip compressed data, was "dist/tspublisher-0.0.1.dev973.tar", last modified: Fri Jun 22 15:03:49 2018, max compression
```

## Comparing `tspublisher-0.0.1.dev962.tar` & `tspublisher-0.0.1.dev973.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2018-06-21 11:31:50.000000 tspublisher-0.0.1.dev962/
--rw-rw-rw-   0 root         (0) root         (0)     1497 2018-06-21 11:31:49.000000 tspublisher-0.0.1.dev962/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2018-06-21 11:31:50.000000 tspublisher-0.0.1.dev962/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2018-06-21 11:31:50.000000 tspublisher-0.0.1.dev962/src/tspublisher.egg-info/
--rw-r--r--   0 root         (0) root         (0)       46 2018-06-21 11:31:50.000000 tspublisher-0.0.1.dev962/src/tspublisher.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      138 2018-06-21 11:31:50.000000 tspublisher-0.0.1.dev962/src/tspublisher.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2018-06-21 11:31:50.000000 tspublisher-0.0.1.dev962/src/tspublisher.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       10 2018-06-21 11:31:50.000000 tspublisher-0.0.1.dev962/src/tspublisher.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      713 2018-06-21 11:31:50.000000 tspublisher-0.0.1.dev962/src/tspublisher.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2018-06-21 11:29:45.000000 tspublisher-0.0.1.dev962/src/tspublisher.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)     1816 2018-06-21 11:31:50.000000 tspublisher-0.0.1.dev962/src/tspublisher.egg-info/SOURCES.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2018-06-21 11:31:50.000000 tspublisher-0.0.1.dev962/src/publisher/
-drwxr-xr-x   0 root         (0) root         (0)        0 2018-06-21 11:31:50.000000 tspublisher-0.0.1.dev962/src/publisher/processing/
--rw-rw-rw-   0 root         (0) root         (0)     8898 2018-06-21 11:28:36.000000 tspublisher-0.0.1.dev962/src/publisher/processing/procedure.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2018-06-21 11:31:50.000000 tspublisher-0.0.1.dev962/src/publisher/processing/data_sources/
--rw-rw-rw-   0 root         (0) root         (0)     1848 2018-06-21 11:28:36.000000 tspublisher-0.0.1.dev962/src/publisher/processing/data_sources/production_csv.py
--rw-rw-rw-   0 root         (0) root         (0)     1571 2018-06-21 11:28:36.000000 tspublisher-0.0.1.dev962/src/publisher/processing/data_sources/overview.py
--rw-rw-rw-   0 root         (0) root         (0)      716 2018-06-21 11:28:36.000000 tspublisher-0.0.1.dev962/src/publisher/processing/data_sources/eula.py
--rw-rw-rw-   0 root         (0) root         (0)      690 2018-06-21 11:28:36.000000 tspublisher-0.0.1.dev962/src/publisher/processing/data_sources/organisation.py
--rw-rw-rw-   0 root         (0) root         (0)      931 2018-06-21 11:28:36.000000 tspublisher-0.0.1.dev962/src/publisher/processing/data_sources/info_card.py
--rw-rw-rw-   0 root         (0) root         (0)      644 2018-06-21 11:28:36.000000 tspublisher-0.0.1.dev962/src/publisher/processing/data_sources/author.py
--rw-rw-rw-   0 root         (0) root         (0)    12263 2018-06-21 11:28:36.000000 tspublisher-0.0.1.dev962/src/publisher/processing/data_sources/step.py
--rw-rw-rw-   0 root         (0) root         (0)     1598 2018-06-21 11:28:36.000000 tspublisher-0.0.1.dev962/src/publisher/processing/data_sources/csv_steps_file.py
--rw-rw-rw-   0 root         (0) root         (0)     1839 2018-06-21 11:28:36.000000 tspublisher-0.0.1.dev962/src/publisher/processing/data_sources/thumbnail.py
--rw-rw-rw-   0 root         (0) root         (0)    11383 2018-06-21 11:28:36.000000 tspublisher-0.0.1.dev962/src/publisher/processing/data_sources/asset.py
--rw-rw-rw-   0 root         (0) root         (0)     1372 2018-06-21 11:28:36.000000 tspublisher-0.0.1.dev962/src/publisher/processing/data_sources/utils.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2018-06-21 11:28:36.000000 tspublisher-0.0.1.dev962/src/publisher/processing/data_sources/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    23470 2018-06-21 11:28:36.000000 tspublisher-0.0.1.dev962/src/publisher/processing/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2018-06-21 11:31:50.000000 tspublisher-0.0.1.dev962/src/publisher/processing/utils/
--rw-rw-rw-   0 root         (0) root         (0)     5521 2018-06-21 11:28:36.000000 tspublisher-0.0.1.dev962/src/publisher/processing/utils/file.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2018-06-21 11:28:36.000000 tspublisher-0.0.1.dev962/src/publisher/processing/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2018-06-21 11:28:36.000000 tspublisher-0.0.1.dev962/src/publisher/processing/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2018-06-21 11:31:50.000000 tspublisher-0.0.1.dev962/src/publisher/translations/
--rw-rw-rw-   0 root         (0) root         (0)     2983 2018-06-21 11:28:36.000000 tspublisher-0.0.1.dev962/src/publisher/translations/pot.py
--rw-rw-rw-   0 root         (0) root         (0)     1489 2018-06-21 11:28:36.000000 tspublisher-0.0.1.dev962/src/publisher/translations/po.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2018-06-21 11:28:36.000000 tspublisher-0.0.1.dev962/src/publisher/translations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1261 2018-06-21 11:28:36.000000 tspublisher-0.0.1.dev962/src/publisher/classes.py
--rw-rw-rw-   0 root         (0) root         (0)    11981 2018-06-21 11:28:36.000000 tspublisher-0.0.1.dev962/src/publisher/procedure_content.py
--rw-rw-rw-   0 root         (0) root         (0)     1343 2018-06-21 11:28:36.000000 tspublisher-0.0.1.dev962/src/publisher/touchsurgery.py
--rw-rw-rw-   0 root         (0) root         (0)     4354 2018-06-21 11:28:36.000000 tspublisher-0.0.1.dev962/src/publisher/api.py
--rw-rw-rw-   0 root         (0) root         (0)     2912 2018-06-21 11:28:36.000000 tspublisher-0.0.1.dev962/src/publisher/validators.py
--rw-rw-rw-   0 root         (0) root         (0)     1946 2018-06-21 11:28:36.000000 tspublisher-0.0.1.dev962/src/publisher/settings.py
--rw-rw-rw-   0 root         (0) root         (0)     3372 2018-06-21 11:28:36.000000 tspublisher-0.0.1.dev962/src/publisher/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     9222 2018-06-21 11:28:36.000000 tspublisher-0.0.1.dev962/src/publisher/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2018-06-21 11:31:50.000000 tspublisher-0.0.1.dev962/src/publisher/git_handling/
--rw-rw-rw-   0 root         (0) root         (0)     8258 2018-06-21 11:28:36.000000 tspublisher-0.0.1.dev962/src/publisher/git_handling/setup.py
--rw-rw-rw-   0 root         (0) root         (0)     2216 2018-06-21 11:28:36.000000 tspublisher-0.0.1.dev962/src/publisher/git_handling/history.py
--rw-rw-rw-   0 root         (0) root         (0)     1098 2018-06-21 11:28:36.000000 tspublisher-0.0.1.dev962/src/publisher/git_handling/notes.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2018-06-21 11:28:36.000000 tspublisher-0.0.1.dev962/src/publisher/git_handling/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       50 2018-06-21 11:28:36.000000 tspublisher-0.0.1.dev962/src/publisher/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1182 2018-06-21 11:28:36.000000 tspublisher-0.0.1.dev962/src/publisher/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2018-06-21 11:31:50.000000 tspublisher-0.0.1.dev962/src/publisher/template_files/
--rw-rw-rw-   0 root         (0) root         (0)    22001 2018-06-21 11:28:36.000000 tspublisher-0.0.1.dev962/src/publisher/template_files/card.jpg
--rw-rw-rw-   0 root         (0) root         (0)     9740 2018-06-21 11:28:36.000000 tspublisher-0.0.1.dev962/src/publisher/template_files/icon.jpg
--rw-rw-rw-   0 root         (0) root         (0)     6598 2018-06-21 11:28:36.000000 tspublisher-0.0.1.dev962/src/publisher/template_files/overview.yml
--rw-rw-rw-   0 root         (0) root         (0)     1051 2018-06-21 11:28:36.000000 tspublisher-0.0.1.dev962/src/publisher/template_files/devices.yml
--rw-rw-rw-   0 root         (0) root         (0)        0 2018-06-21 11:28:36.000000 tspublisher-0.0.1.dev962/src/publisher/template_files/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       48 2018-06-21 11:28:36.000000 tspublisher-0.0.1.dev962/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      713 2018-06-21 11:31:50.000000 tspublisher-0.0.1.dev962/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2018-06-21 11:31:50.000000 tspublisher-0.0.1.dev962/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      296 2018-06-21 11:28:36.000000 tspublisher-0.0.1.dev962/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2018-06-22 15:03:49.000000 tspublisher-0.0.1.dev973/
+-rw-rw-rw-   0 root         (0) root         (0)     1497 2018-06-22 15:03:49.000000 tspublisher-0.0.1.dev973/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2018-06-22 15:03:49.000000 tspublisher-0.0.1.dev973/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2018-06-22 15:03:49.000000 tspublisher-0.0.1.dev973/src/tspublisher.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       46 2018-06-22 15:03:49.000000 tspublisher-0.0.1.dev973/src/tspublisher.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      138 2018-06-22 15:03:49.000000 tspublisher-0.0.1.dev973/src/tspublisher.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2018-06-22 15:03:49.000000 tspublisher-0.0.1.dev973/src/tspublisher.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2018-06-22 15:03:49.000000 tspublisher-0.0.1.dev973/src/tspublisher.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      713 2018-06-22 15:03:49.000000 tspublisher-0.0.1.dev973/src/tspublisher.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2018-06-22 15:02:37.000000 tspublisher-0.0.1.dev973/src/tspublisher.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)     1816 2018-06-22 15:03:49.000000 tspublisher-0.0.1.dev973/src/tspublisher.egg-info/SOURCES.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2018-06-22 15:03:49.000000 tspublisher-0.0.1.dev973/src/publisher/
+drwxr-xr-x   0 root         (0) root         (0)        0 2018-06-22 15:03:49.000000 tspublisher-0.0.1.dev973/src/publisher/processing/
+-rw-rw-rw-   0 root         (0) root         (0)     8898 2018-06-22 15:01:57.000000 tspublisher-0.0.1.dev973/src/publisher/processing/procedure.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2018-06-22 15:03:49.000000 tspublisher-0.0.1.dev973/src/publisher/processing/data_sources/
+-rw-rw-rw-   0 root         (0) root         (0)     1848 2018-06-22 15:01:57.000000 tspublisher-0.0.1.dev973/src/publisher/processing/data_sources/production_csv.py
+-rw-rw-rw-   0 root         (0) root         (0)     1571 2018-06-22 15:01:57.000000 tspublisher-0.0.1.dev973/src/publisher/processing/data_sources/overview.py
+-rw-rw-rw-   0 root         (0) root         (0)      716 2018-06-22 15:01:57.000000 tspublisher-0.0.1.dev973/src/publisher/processing/data_sources/eula.py
+-rw-rw-rw-   0 root         (0) root         (0)      690 2018-06-22 15:01:57.000000 tspublisher-0.0.1.dev973/src/publisher/processing/data_sources/organisation.py
+-rw-rw-rw-   0 root         (0) root         (0)      931 2018-06-22 15:01:57.000000 tspublisher-0.0.1.dev973/src/publisher/processing/data_sources/info_card.py
+-rw-rw-rw-   0 root         (0) root         (0)      644 2018-06-22 15:01:57.000000 tspublisher-0.0.1.dev973/src/publisher/processing/data_sources/author.py
+-rw-rw-rw-   0 root         (0) root         (0)    12263 2018-06-22 15:01:57.000000 tspublisher-0.0.1.dev973/src/publisher/processing/data_sources/step.py
+-rw-rw-rw-   0 root         (0) root         (0)     1598 2018-06-22 15:01:57.000000 tspublisher-0.0.1.dev973/src/publisher/processing/data_sources/csv_steps_file.py
+-rw-rw-rw-   0 root         (0) root         (0)     1839 2018-06-22 15:01:57.000000 tspublisher-0.0.1.dev973/src/publisher/processing/data_sources/thumbnail.py
+-rw-rw-rw-   0 root         (0) root         (0)    11383 2018-06-22 15:01:57.000000 tspublisher-0.0.1.dev973/src/publisher/processing/data_sources/asset.py
+-rw-rw-rw-   0 root         (0) root         (0)     1372 2018-06-22 15:01:57.000000 tspublisher-0.0.1.dev973/src/publisher/processing/data_sources/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2018-06-22 15:01:57.000000 tspublisher-0.0.1.dev973/src/publisher/processing/data_sources/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    23470 2018-06-22 15:01:57.000000 tspublisher-0.0.1.dev973/src/publisher/processing/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2018-06-22 15:03:49.000000 tspublisher-0.0.1.dev973/src/publisher/processing/utils/
+-rw-rw-rw-   0 root         (0) root         (0)     5521 2018-06-22 15:01:57.000000 tspublisher-0.0.1.dev973/src/publisher/processing/utils/file.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2018-06-22 15:01:57.000000 tspublisher-0.0.1.dev973/src/publisher/processing/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2018-06-22 15:01:57.000000 tspublisher-0.0.1.dev973/src/publisher/processing/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2018-06-22 15:03:49.000000 tspublisher-0.0.1.dev973/src/publisher/translations/
+-rw-rw-rw-   0 root         (0) root         (0)     2983 2018-06-22 15:01:57.000000 tspublisher-0.0.1.dev973/src/publisher/translations/pot.py
+-rw-rw-rw-   0 root         (0) root         (0)     1489 2018-06-22 15:01:57.000000 tspublisher-0.0.1.dev973/src/publisher/translations/po.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2018-06-22 15:01:57.000000 tspublisher-0.0.1.dev973/src/publisher/translations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1261 2018-06-22 15:01:57.000000 tspublisher-0.0.1.dev973/src/publisher/classes.py
+-rw-rw-rw-   0 root         (0) root         (0)    11981 2018-06-22 15:01:57.000000 tspublisher-0.0.1.dev973/src/publisher/procedure_content.py
+-rw-rw-rw-   0 root         (0) root         (0)     1343 2018-06-22 15:01:57.000000 tspublisher-0.0.1.dev973/src/publisher/touchsurgery.py
+-rw-rw-rw-   0 root         (0) root         (0)     4354 2018-06-22 15:01:57.000000 tspublisher-0.0.1.dev973/src/publisher/api.py
+-rw-rw-rw-   0 root         (0) root         (0)     2912 2018-06-22 15:01:57.000000 tspublisher-0.0.1.dev973/src/publisher/validators.py
+-rw-rw-rw-   0 root         (0) root         (0)     1946 2018-06-22 15:01:57.000000 tspublisher-0.0.1.dev973/src/publisher/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     3372 2018-06-22 15:01:57.000000 tspublisher-0.0.1.dev973/src/publisher/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     9222 2018-06-22 15:01:57.000000 tspublisher-0.0.1.dev973/src/publisher/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2018-06-22 15:03:49.000000 tspublisher-0.0.1.dev973/src/publisher/git_handling/
+-rw-rw-rw-   0 root         (0) root         (0)     8320 2018-06-22 15:01:57.000000 tspublisher-0.0.1.dev973/src/publisher/git_handling/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     2216 2018-06-22 15:01:57.000000 tspublisher-0.0.1.dev973/src/publisher/git_handling/history.py
+-rw-rw-rw-   0 root         (0) root         (0)     1098 2018-06-22 15:01:57.000000 tspublisher-0.0.1.dev973/src/publisher/git_handling/notes.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2018-06-22 15:01:57.000000 tspublisher-0.0.1.dev973/src/publisher/git_handling/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       50 2018-06-22 15:01:57.000000 tspublisher-0.0.1.dev973/src/publisher/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1182 2018-06-22 15:01:57.000000 tspublisher-0.0.1.dev973/src/publisher/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2018-06-22 15:03:49.000000 tspublisher-0.0.1.dev973/src/publisher/template_files/
+-rw-rw-rw-   0 root         (0) root         (0)    22001 2018-06-22 15:01:57.000000 tspublisher-0.0.1.dev973/src/publisher/template_files/card.jpg
+-rw-rw-rw-   0 root         (0) root         (0)     9740 2018-06-22 15:01:57.000000 tspublisher-0.0.1.dev973/src/publisher/template_files/icon.jpg
+-rw-rw-rw-   0 root         (0) root         (0)     6598 2018-06-22 15:01:57.000000 tspublisher-0.0.1.dev973/src/publisher/template_files/overview.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1051 2018-06-22 15:01:57.000000 tspublisher-0.0.1.dev973/src/publisher/template_files/devices.yml
+-rw-rw-rw-   0 root         (0) root         (0)        0 2018-06-22 15:01:57.000000 tspublisher-0.0.1.dev973/src/publisher/template_files/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       48 2018-06-22 15:01:57.000000 tspublisher-0.0.1.dev973/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      713 2018-06-22 15:03:49.000000 tspublisher-0.0.1.dev973/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2018-06-22 15:03:49.000000 tspublisher-0.0.1.dev973/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      296 2018-06-22 15:01:57.000000 tspublisher-0.0.1.dev973/README.md
```

### Comparing `tspublisher-0.0.1.dev962/setup.py` & `tspublisher-0.0.1.dev973/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         join(dirname(__file__), *names),
         encoding=kwargs.get('encoding', 'utf8')
     ).read()
 
 
 setup(
     name='tspublisher',
-    version='0.0.1.dev962',
+    version='0.0.1.dev973',
     license='GNU General Public License',
     description='Touch Surgery publishing tools',
     long_description=read('README.md'),
     author='TS Content Squad',
     author_email='admin@touchsurgery.com',
     url='https://www.touchsurgery.com/jobs',
     packages=find_packages('src'),
```

### Comparing `tspublisher-0.0.1.dev962/src/tspublisher.egg-info/PKG-INFO` & `tspublisher-0.0.1.dev973/src/tspublisher.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tspublisher
-Version: 0.0.1.dev962
+Version: 0.0.1.dev973
 Summary: Touch Surgery publishing tools
 Home-page: https://www.touchsurgery.com/jobs
 Author: TS Content Squad
 Author-email: admin@touchsurgery.com
 License: GNU General Public License
 Description: Touch Surgery Publisher Tools
         =============================
```

### Comparing `tspublisher-0.0.1.dev962/src/tspublisher.egg-info/SOURCES.txt` & `tspublisher-0.0.1.dev973/src/tspublisher.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tspublisher-0.0.1.dev962/src/publisher/processing/procedure.py` & `tspublisher-0.0.1.dev973/src/publisher/processing/procedure.py`

 * *Files identical despite different names*

### Comparing `tspublisher-0.0.1.dev962/src/publisher/processing/data_sources/production_csv.py` & `tspublisher-0.0.1.dev973/src/publisher/processing/data_sources/production_csv.py`

 * *Files identical despite different names*

### Comparing `tspublisher-0.0.1.dev962/src/publisher/processing/data_sources/overview.py` & `tspublisher-0.0.1.dev973/src/publisher/processing/data_sources/overview.py`

 * *Files identical despite different names*

### Comparing `tspublisher-0.0.1.dev962/src/publisher/processing/data_sources/eula.py` & `tspublisher-0.0.1.dev973/src/publisher/processing/data_sources/eula.py`

 * *Files identical despite different names*

### Comparing `tspublisher-0.0.1.dev962/src/publisher/processing/data_sources/organisation.py` & `tspublisher-0.0.1.dev973/src/publisher/processing/data_sources/organisation.py`

 * *Files identical despite different names*

### Comparing `tspublisher-0.0.1.dev962/src/publisher/processing/data_sources/info_card.py` & `tspublisher-0.0.1.dev973/src/publisher/processing/data_sources/info_card.py`

 * *Files identical despite different names*

### Comparing `tspublisher-0.0.1.dev962/src/publisher/processing/data_sources/author.py` & `tspublisher-0.0.1.dev973/src/publisher/processing/data_sources/author.py`

 * *Files identical despite different names*

### Comparing `tspublisher-0.0.1.dev962/src/publisher/processing/data_sources/step.py` & `tspublisher-0.0.1.dev973/src/publisher/processing/data_sources/step.py`

 * *Files identical despite different names*

### Comparing `tspublisher-0.0.1.dev962/src/publisher/processing/data_sources/csv_steps_file.py` & `tspublisher-0.0.1.dev973/src/publisher/processing/data_sources/csv_steps_file.py`

 * *Files identical despite different names*

### Comparing `tspublisher-0.0.1.dev962/src/publisher/processing/data_sources/thumbnail.py` & `tspublisher-0.0.1.dev973/src/publisher/processing/data_sources/thumbnail.py`

 * *Files identical despite different names*

### Comparing `tspublisher-0.0.1.dev962/src/publisher/processing/data_sources/asset.py` & `tspublisher-0.0.1.dev973/src/publisher/processing/data_sources/asset.py`

 * *Files identical despite different names*

### Comparing `tspublisher-0.0.1.dev962/src/publisher/processing/data_sources/utils.py` & `tspublisher-0.0.1.dev973/src/publisher/processing/data_sources/utils.py`

 * *Files identical despite different names*

### Comparing `tspublisher-0.0.1.dev962/src/publisher/processing/models.py` & `tspublisher-0.0.1.dev973/src/publisher/processing/models.py`

 * *Files identical despite different names*

### Comparing `tspublisher-0.0.1.dev962/src/publisher/processing/utils/file.py` & `tspublisher-0.0.1.dev973/src/publisher/processing/utils/file.py`

 * *Files identical despite different names*

### Comparing `tspublisher-0.0.1.dev962/src/publisher/translations/pot.py` & `tspublisher-0.0.1.dev973/src/publisher/translations/pot.py`

 * *Files identical despite different names*

### Comparing `tspublisher-0.0.1.dev962/src/publisher/translations/po.py` & `tspublisher-0.0.1.dev973/src/publisher/translations/po.py`

 * *Files identical despite different names*

### Comparing `tspublisher-0.0.1.dev962/src/publisher/classes.py` & `tspublisher-0.0.1.dev973/src/publisher/classes.py`

 * *Files identical despite different names*

### Comparing `tspublisher-0.0.1.dev962/src/publisher/procedure_content.py` & `tspublisher-0.0.1.dev973/src/publisher/procedure_content.py`

 * *Files identical despite different names*

### Comparing `tspublisher-0.0.1.dev962/src/publisher/touchsurgery.py` & `tspublisher-0.0.1.dev973/src/publisher/touchsurgery.py`

 * *Files identical despite different names*

### Comparing `tspublisher-0.0.1.dev962/src/publisher/api.py` & `tspublisher-0.0.1.dev973/src/publisher/api.py`

 * *Files identical despite different names*

### Comparing `tspublisher-0.0.1.dev962/src/publisher/validators.py` & `tspublisher-0.0.1.dev973/src/publisher/validators.py`

 * *Files identical despite different names*

### Comparing `tspublisher-0.0.1.dev962/src/publisher/settings.py` & `tspublisher-0.0.1.dev973/src/publisher/settings.py`

 * *Files identical despite different names*

### Comparing `tspublisher-0.0.1.dev962/src/publisher/utils.py` & `tspublisher-0.0.1.dev973/src/publisher/utils.py`

 * *Files identical despite different names*

### Comparing `tspublisher-0.0.1.dev962/src/publisher/cli.py` & `tspublisher-0.0.1.dev973/src/publisher/cli.py`

 * *Files identical despite different names*

### Comparing `tspublisher-0.0.1.dev962/src/publisher/git_handling/setup.py` & `tspublisher-0.0.1.dev973/src/publisher/git_handling/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,21 +29,22 @@
 
         print("%s" % mac_msg if 'darwin' in get_platform() else win_msg)
         sys.exit(1)
 
     print('Generating key and configuring user profile')
     check_and_create_directory(settings.SSH_DIRECTORY_PATH)
     sys.stdout.flush()
+
     login_success = False
     get_username()
     while not login_success:
         if login(get_email(), get_password(), create_rsa_return_pub_key()):
             login_success = True
 
-    print("Configuring ssh config file")
+    print("Configuring ssh config file ")
     check_and_create_file(settings.SSH_CONFIG_PATH)
     if not has_private_key():
         raise RuntimeError("Unable to proceed without a key. Please contact Hansel before trying again")
     configure_ssh_config()
 
     print("Installing and configuring git lfs")
     check_brew_installed()
@@ -120,14 +121,15 @@
         'User ubuntu\n '
         'IdentitiesOnly true\n '
         'IdentityFile ~/.ssh/touchsurgery-studio.pem\n'
     ).format(settings.STUDIO_GIT_PATH)
 
     ssh_config_stanza = (
         'Host {0}\n'
+        ' StrictHostKeyChecking no\n'
         ' User git\n'
         ' IdentitiesOnly true\n'
         ' IdentityFile {1}\n'
     ).format(settings.STUDIO_GIT_PATH, settings.RSA_PRIVATE_KEY_PATH)
 
     try:
 
@@ -202,16 +204,17 @@
         raise ValidationError
 
 
 def check_and_create_file(path):
     try:
         if not os.path.exists(path):
             subprocess.check_output(['touch', path])
-    except Exception:
+    except Exception as e:
         print("Could not find or create the file")
+        print(e)
         raise ValidationError
 
 
 def configure_git_lfs():
     """Set relevant  lfs settings
     """
     call_command_and_print_exception(['git', 'config', '--global', 'lfs.url',
```

### Comparing `tspublisher-0.0.1.dev962/src/publisher/git_handling/history.py` & `tspublisher-0.0.1.dev973/src/publisher/git_handling/history.py`

 * *Files identical despite different names*

### Comparing `tspublisher-0.0.1.dev962/src/publisher/git_handling/notes.py` & `tspublisher-0.0.1.dev973/src/publisher/git_handling/notes.py`

 * *Files identical despite different names*

### Comparing `tspublisher-0.0.1.dev962/src/publisher/exceptions.py` & `tspublisher-0.0.1.dev973/src/publisher/exceptions.py`

 * *Files identical despite different names*

### Comparing `tspublisher-0.0.1.dev962/src/publisher/template_files/card.jpg` & `tspublisher-0.0.1.dev973/src/publisher/template_files/card.jpg`

 * *Files identical despite different names*

### Comparing `tspublisher-0.0.1.dev962/src/publisher/template_files/icon.jpg` & `tspublisher-0.0.1.dev973/src/publisher/template_files/icon.jpg`

 * *Files identical despite different names*

### Comparing `tspublisher-0.0.1.dev962/src/publisher/template_files/overview.yml` & `tspublisher-0.0.1.dev973/src/publisher/template_files/overview.yml`

 * *Files identical despite different names*

### Comparing `tspublisher-0.0.1.dev962/src/publisher/template_files/devices.yml` & `tspublisher-0.0.1.dev973/src/publisher/template_files/devices.yml`

 * *Files identical despite different names*

### Comparing `tspublisher-0.0.1.dev962/PKG-INFO` & `tspublisher-0.0.1.dev973/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tspublisher
-Version: 0.0.1.dev962
+Version: 0.0.1.dev973
 Summary: Touch Surgery publishing tools
 Home-page: https://www.touchsurgery.com/jobs
 Author: TS Content Squad
 Author-email: admin@touchsurgery.com
 License: GNU General Public License
 Description: Touch Surgery Publisher Tools
         =============================
```

