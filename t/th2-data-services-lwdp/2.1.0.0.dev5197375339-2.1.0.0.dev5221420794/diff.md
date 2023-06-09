# Comparing `tmp/th2_data_services_lwdp-2.1.0.0.dev5197375339.tar.gz` & `tmp/th2_data_services_lwdp-2.1.0.0.dev5221420794.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/th2_data_services_lwdp-2.1.0.0.dev5197375339.tar", last modified: Wed Jun  7 07:50:51 2023, max compression
+gzip compressed data, was "dist/th2_data_services_lwdp-2.1.0.0.dev5221420794.tar", last modified: Fri Jun  9 11:36:01 2023, max compression
```

## Comparing `th2_data_services_lwdp-2.1.0.0.dev5197375339.tar` & `th2_data_services_lwdp-2.1.0.0.dev5221420794.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 07:50:51.000000 th2_data_services_lwdp-2.1.0.0.dev5197375339/
--rw-r--r--   0 runner    (1001) docker     (122)       68 2023-06-07 07:49:30.000000 th2_data_services_lwdp-2.1.0.0.dev5197375339/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     9677 2023-06-07 07:50:51.000000 th2_data_services_lwdp-2.1.0.0.dev5197375339/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     7699 2023-06-07 07:49:30.000000 th2_data_services_lwdp-2.1.0.0.dev5197375339/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       92 2023-06-07 07:50:28.000000 th2_data_services_lwdp-2.1.0.0.dev5197375339/package_info.json
--rw-r--r--   0 runner    (1001) docker     (122)      236 2023-06-07 07:49:30.000000 th2_data_services_lwdp-2.1.0.0.dev5197375339/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-07 07:50:51.000000 th2_data_services_lwdp-2.1.0.0.dev5197375339/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1658 2023-06-07 07:49:30.000000 th2_data_services_lwdp-2.1.0.0.dev5197375339/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 07:50:51.000000 th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 07:50:51.000000 th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 07:50:51.000000 th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/
--rw-r--r--   0 runner    (1001) docker     (122)     1059 2023-06-07 07:49:30.000000 th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 07:50:51.000000 th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/adapters/
--rw-r--r--   0 runner    (1001) docker     (122)      819 2023-06-07 07:49:30.000000 th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2000 2023-06-07 07:49:30.000000 th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/adapters/adapter_sse.py
--rw-r--r--   0 runner    (1001) docker     (122)     2442 2023-06-07 07:49:30.000000 th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/adapters/basic_adapters.py
--rw-r--r--   0 runner    (1001) docker     (122)     2980 2023-06-07 07:49:30.000000 th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/adapters/event_adapters.py
--rw-r--r--   0 runner    (1001) docker     (122)     1906 2023-06-07 07:49:30.000000 th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/adapters/message_adapters.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 07:50:51.000000 th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/commands/
--rw-r--r--   0 runner    (1001) docker     (122)      614 2023-06-07 07:49:30.000000 th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    17907 2023-06-07 07:49:30.000000 th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/commands/grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)    46699 2023-06-07 07:49:30.000000 th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/commands/http.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 07:50:51.000000 th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/data_source/
--rw-r--r--   0 runner    (1001) docker     (122)      682 2023-06-07 07:49:30.000000 th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/data_source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3327 2023-06-07 07:49:30.000000 th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/data_source/grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)     3586 2023-06-07 07:49:30.000000 th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/data_source/http.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 07:50:51.000000 th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/event_tree/
--rw-r--r--   0 runner    (1001) docker     (122)      658 2023-06-07 07:49:30.000000 th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/event_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3421 2023-06-07 07:49:30.000000 th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/event_tree/http_etc_driver.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 07:50:51.000000 th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/filters/
--rw-r--r--   0 runner    (1001) docker     (122)      665 2023-06-07 07:49:30.000000 th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      981 2023-06-07 07:49:30.000000 th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/filters/event_filters.py
--rw-r--r--   0 runner    (1001) docker     (122)     3527 2023-06-07 07:49:30.000000 th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/filters/filter.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 07:50:51.000000 th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/interfaces/
--rw-r--r--   0 runner    (1001) docker     (122)      614 2023-06-07 07:49:30.000000 th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1443 2023-06-07 07:49:30.000000 th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/interfaces/command.py
--rw-r--r--   0 runner    (1001) docker     (122)     5056 2023-06-07 07:49:30.000000 th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/interfaces/data_source.py
--rw-r--r--   0 runner    (1001) docker     (122)      670 2023-06-07 07:49:30.000000 th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/interfaces/filter.py
--rw-r--r--   0 runner    (1001) docker     (122)     1000 2023-06-07 07:49:30.000000 th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/interfaces/source_api.py
--rw-r--r--   0 runner    (1001) docker     (122)      722 2023-06-07 07:49:30.000000 th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/message_response_format.py
--rw-r--r--   0 runner    (1001) docker     (122)     1622 2023-06-07 07:49:30.000000 th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/page.py
--rw-r--r--   0 runner    (1001) docker     (122)     3593 2023-06-07 07:49:30.000000 th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 07:50:51.000000 th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/source_api/
--rw-r--r--   0 runner    (1001) docker     (122)      669 2023-06-07 07:49:30.000000 th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/source_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    16862 2023-06-07 07:49:30.000000 th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/source_api/grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)    13925 2023-06-07 07:49:30.000000 th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/source_api/http.py
--rw-r--r--   0 runner    (1001) docker     (122)     4687 2023-06-07 07:49:30.000000 th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/streams.py
--rw-r--r--   0 runner    (1001) docker     (122)     2995 2023-06-07 07:49:30.000000 th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/struct.py
--rw-r--r--   0 runner    (1001) docker     (122)     4571 2023-06-07 07:49:30.000000 th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/stub_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 07:50:51.000000 th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      695 2023-06-07 07:49:30.000000 th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1497 2023-06-07 07:49:30.000000 th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/utils/_response_formats.py
--rw-r--r--   0 runner    (1001) docker     (122)     2441 2023-06-07 07:49:30.000000 th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/utils/json.py
--rw-r--r--   0 runner    (1001) docker     (122)     1303 2023-06-07 07:49:30.000000 th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/utils/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 07:50:51.000000 th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services_lwdp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     9677 2023-06-07 07:50:50.000000 th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services_lwdp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2229 2023-06-07 07:50:51.000000 th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services_lwdp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-07 07:50:50.000000 th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services_lwdp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       42 2023-06-07 07:50:50.000000 th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services_lwdp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-07 07:50:50.000000 th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services_lwdp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 11:36:01.000000 th2_data_services_lwdp-2.1.0.0.dev5221420794/
+-rw-r--r--   0 runner    (1001) docker     (122)       68 2023-06-09 11:34:24.000000 th2_data_services_lwdp-2.1.0.0.dev5221420794/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     9677 2023-06-09 11:36:01.000000 th2_data_services_lwdp-2.1.0.0.dev5221420794/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     7699 2023-06-09 11:34:24.000000 th2_data_services_lwdp-2.1.0.0.dev5221420794/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-06-09 11:35:48.000000 th2_data_services_lwdp-2.1.0.0.dev5221420794/package_info.json
+-rw-r--r--   0 runner    (1001) docker     (122)      236 2023-06-09 11:34:24.000000 th2_data_services_lwdp-2.1.0.0.dev5221420794/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-09 11:36:01.000000 th2_data_services_lwdp-2.1.0.0.dev5221420794/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1658 2023-06-09 11:34:24.000000 th2_data_services_lwdp-2.1.0.0.dev5221420794/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 11:36:01.000000 th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 11:36:01.000000 th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 11:36:01.000000 th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/
+-rw-r--r--   0 runner    (1001) docker     (122)     1059 2023-06-09 11:34:24.000000 th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 11:36:01.000000 th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/adapters/
+-rw-r--r--   0 runner    (1001) docker     (122)      819 2023-06-09 11:34:24.000000 th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2000 2023-06-09 11:34:24.000000 th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/adapters/adapter_sse.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2442 2023-06-09 11:34:24.000000 th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/adapters/basic_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2980 2023-06-09 11:34:24.000000 th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/adapters/event_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1906 2023-06-09 11:34:24.000000 th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/adapters/message_adapters.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 11:36:01.000000 th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)      614 2023-06-09 11:34:24.000000 th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17907 2023-06-09 11:34:24.000000 th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/commands/grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)    46528 2023-06-09 11:34:24.000000 th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/commands/http.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 11:36:01.000000 th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/data_source/
+-rw-r--r--   0 runner    (1001) docker     (122)      682 2023-06-09 11:34:24.000000 th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/data_source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3327 2023-06-09 11:34:24.000000 th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/data_source/grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3586 2023-06-09 11:34:24.000000 th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/data_source/http.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 11:36:01.000000 th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/event_tree/
+-rw-r--r--   0 runner    (1001) docker     (122)      658 2023-06-09 11:34:24.000000 th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/event_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3421 2023-06-09 11:34:24.000000 th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/event_tree/http_etc_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 11:36:01.000000 th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/filters/
+-rw-r--r--   0 runner    (1001) docker     (122)      665 2023-06-09 11:34:24.000000 th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      981 2023-06-09 11:34:24.000000 th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/filters/event_filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3527 2023-06-09 11:34:24.000000 th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/filters/filter.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 11:36:01.000000 th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (122)      614 2023-06-09 11:34:24.000000 th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1443 2023-06-09 11:34:24.000000 th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/interfaces/command.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5056 2023-06-09 11:34:24.000000 th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/interfaces/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (122)      670 2023-06-09 11:34:24.000000 th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/interfaces/filter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1000 2023-06-09 11:34:24.000000 th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/interfaces/source_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      722 2023-06-09 11:34:24.000000 th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/message_response_format.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1733 2023-06-09 11:34:24.000000 th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/page.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3593 2023-06-09 11:34:24.000000 th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 11:36:01.000000 th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/source_api/
+-rw-r--r--   0 runner    (1001) docker     (122)      669 2023-06-09 11:34:24.000000 th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/source_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16862 2023-06-09 11:34:24.000000 th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/source_api/grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13925 2023-06-09 11:34:24.000000 th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/source_api/http.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4687 2023-06-09 11:34:24.000000 th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/streams.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2995 2023-06-09 11:34:24.000000 th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/struct.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4571 2023-06-09 11:34:24.000000 th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/stub_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 11:36:01.000000 th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      697 2023-06-09 11:34:24.000000 th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1438 2023-06-09 11:34:24.000000 th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/utils/_misc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1504 2023-06-09 11:34:24.000000 th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/utils/_response_formats.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2441 2023-06-09 11:34:24.000000 th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/utils/json.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 11:36:01.000000 th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services_lwdp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     9677 2023-06-09 11:36:00.000000 th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services_lwdp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2230 2023-06-09 11:36:01.000000 th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services_lwdp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-09 11:36:00.000000 th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services_lwdp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       42 2023-06-09 11:36:00.000000 th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services_lwdp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-09 11:36:00.000000 th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services_lwdp.egg-info/top_level.txt
```

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5197375339/PKG-INFO` & `th2_data_services_lwdp-2.1.0.0.dev5221420794/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: th2_data_services_lwdp
-Version: 2.1.0.0.dev5197375339
+Version: 2.1.0.0.dev5221420794
 Summary: th2_data_services_lwdp
 Home-page: https://github.com/th2-net/th2-ds-source-lwdp
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: # Lightweight Data Provider Data Source (major version 2).
         # Introduction
```

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5197375339/README.md` & `th2_data_services_lwdp-2.1.0.0.dev5221420794/README.md`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5197375339/setup.py` & `th2_data_services_lwdp-2.1.0.0.dev5221420794/setup.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/__init__.py` & `th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/adapters/__init__.py` & `th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/adapters/adapter_sse.py` & `th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/adapters/adapter_sse.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/adapters/basic_adapters.py` & `th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/adapters/basic_adapters.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/adapters/event_adapters.py` & `th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/adapters/event_adapters.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/adapters/message_adapters.py` & `th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/adapters/message_adapters.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/commands/__init__.py` & `th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/commands/grpc.py` & `th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/commands/grpc.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/commands/http.py` & `th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/commands/http.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 from th2_data_services.utils.decode_error_handler import UNICODE_REPLACE_HANDLER
 from th2_data_services.data_source.lwdp.filters.event_filters import LwDPEventFilter
 from th2_data_services.data_source.lwdp.utils import (
     _check_datetime,
     _check_list_or_tuple,
     _check_response_formats,
 )
+from th2_data_services.data_source.lwdp.utils._misc import get_utc_datetime_now
 from th2_data_services.data_source.lwdp.utils.json import BufferedJSONProcessor
 from th2_data_services.data_source.lwdp.page import PageNotFound
 
 Event = dict
 
 
 # LOG import logging
@@ -702,15 +703,15 @@
 
         _check_list_or_tuple(self._scopes, var_name="scopes")
 
     def _get_urls(self, data_source: HTTPDataSource):
         page = _get_page_object(self._book_id, self._page, data_source)
         self._start_timestamp = ProtobufTimestampConverter.to_nanoseconds(page.start_timestamp)
         self._end_timestamp = (
-            DatetimeConverter.to_nanoseconds(datetime.now().replace(microsecond=0))
+            get_utc_datetime_now()
             if page.end_timestamp is None
             else ProtobufTimestampConverter.to_nanoseconds(page.end_timestamp)
         )
         self._book_id = page.book
         api = data_source.source_api
         return [
             api.get_url_search_sse_events(
@@ -1064,35 +1065,36 @@
         self._response_formats = response_formats
         self._keep_open = keep_open
         self._max_url_length = max_url_length
         self._cache = cache
 
     def handle(self, data_source: HTTPDataSource):
         page = _get_page_object(self._book_id, self._page, data_source)
-        self._start_timestamp = ProtobufTimestampConverter.to_nanoseconds(page.start_timestamp)
-        self._end_timestamp = (
-            DatetimeConverter.to_nanoseconds(datetime.now().replace(microsecond=0))
+        start_timestamp = ProtobufTimestampConverter.to_datetime(page.start_timestamp)
+        end_timestamp = (
+            get_utc_datetime_now()
             if page.end_timestamp is None
-            else ProtobufTimestampConverter.to_nanoseconds(page.end_timestamp)
+            else ProtobufTimestampConverter.to_datetime(page.end_timestamp)
         )
-        self._groups = list(
+        groups = list(
             data_source.command(
                 GetMessageGroups(
                     self._book_id,
-                    datetime.fromtimestamp(self._start_timestamp // 1_000_000_000),
-                    datetime.fromtimestamp(self._end_timestamp // 1_000_000_000),
+                    start_timestamp,
+                    end_timestamp,
                     char_enc=self._char_enc,
+                    decode_error_handler=self._decode_error_handler,
                 )
             )
         )
         self._book_id = page.book
         return data_source.command(
             GetMessagesByPageByGroups(
                 page=self._page,
-                groups=self._groups,
+                groups=groups,
                 book_id=self._book_id,
                 sort=self._sort,
                 response_formats=self._response_formats,
                 keep_open=self._keep_open,
                 max_url_length=self._max_url_length,
                 char_enc=self._char_enc,
                 decode_error_handler=self._decode_error_handler,
@@ -1158,15 +1160,15 @@
         self._max_url_length = max_url_length
         self._stream = stream
 
     def _get_urls(self, data_source: HTTPDataSource):
         page = _get_page_object(self._book_id, self._page, data_source)
         self._start_timestamp = ProtobufTimestampConverter.to_nanoseconds(page.start_timestamp)
         self._end_timestamp = (
-            DatetimeConverter.to_nanoseconds(datetime.now().replace(microsecond=0))
+            get_utc_datetime_now()
             if page.end_timestamp is None
             else ProtobufTimestampConverter.to_nanoseconds(page.end_timestamp)
         )
         self._book_id = page.book
         api = data_source.source_api
         return api.get_url_search_sse_messages(
             start_timestamp=self._start_timestamp,
@@ -1244,15 +1246,15 @@
 
         _check_list_or_tuple(self._groups, var_name="groups")
 
     def _get_urls(self, data_source: HTTPDataSource):
         page = _get_page_object(self._book_id, self._page, data_source)
         self._start_timestamp = ProtobufTimestampConverter.to_nanoseconds(page.start_timestamp)
         self._end_timestamp = (
-            DatetimeConverter.to_nanoseconds(datetime.now().replace(microsecond=0))
+            get_utc_datetime_now()
             if page.end_timestamp is None
             else ProtobufTimestampConverter.to_nanoseconds(page.end_timestamp)
         )
         self._book_id = page.book
         api = data_source.source_api
         return api.get_url_search_messages_by_groups(
             start_timestamp=self._start_timestamp,
```

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/data_source/__init__.py` & `th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/data_source/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/data_source/grpc.py` & `th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/data_source/grpc.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/data_source/http.py` & `th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/data_source/http.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/event_tree/__init__.py` & `th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/event_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/event_tree/http_etc_driver.py` & `th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/event_tree/http_etc_driver.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/filters/__init__.py` & `th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/filters/event_filters.py` & `th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/filters/event_filters.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/filters/filter.py` & `th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/filters/filter.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/interfaces/__init__.py` & `th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/interfaces/command.py` & `th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/interfaces/command.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/interfaces/data_source.py` & `th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/interfaces/data_source.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/interfaces/filter.py` & `th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/interfaces/filter.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/interfaces/source_api.py` & `th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/interfaces/source_api.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/message_response_format.py` & `th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/message_response_format.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/page.py` & `th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/page.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,30 +7,30 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-from typing import Dict
+from typing import Dict, Optional
 
 
 class Page:
     def __init__(self, data: Dict):  # noqa
         """Page Constructor.
 
         Args:
             data (Dict): Page Data
         """
-        self.data = data
-        self.book = data["id"]["book"]
-        self.name = data["id"]["name"]
-        self.comment = data["comment"]
-        self.start_timestamp = data["started"]
-        self.end_timestamp = data["ended"]
+        self.data: dict = data
+        self.book: str = data["id"]["book"]
+        self.name: str = data["id"]["name"]
+        self.comment: str = data["comment"]
+        self.start_timestamp: Dict[str, int] = data["started"]  # eg. {'epochSeconds': 0, 'nano': 0}
+        self.end_timestamp: Optional[Dict[str, int]] = data["ended"]
         self.updated = data["updated"]
         self.removed = data["removed"]
 
     def __str__(self):  # noqa
         return str(self.data)
 
     def __repr__(self):  # noqa
```

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/resolver.py` & `th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/resolver.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/source_api/__init__.py` & `th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/source_api/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/source_api/grpc.py` & `th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/source_api/grpc.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/source_api/http.py` & `th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/source_api/http.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/streams.py` & `th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/streams.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/struct.py` & `th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/struct.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/stub_builder.py` & `th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/stub_builder.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/utils/__init__.py` & `th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/utils/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from .misc import _check_list_or_tuple, _check_datetime, _check_response_formats
+from ._misc import _check_list_or_tuple, _check_datetime, _check_response_formats
```

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/utils/_response_formats.py` & `th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/utils/_response_formats.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 from typing import List, Union
 from th2_data_services.data_source.lwdp.message_response_format import ResponseFormat as RF
 
 
-class ResponseFormats:
+class ResponseFormatsChecker:
     def __init__(self):  # noqa
         """ResponseFormats Constructor."""
         self.correct_formats = [RF.JSON_PARSED, RF.BASE64, RF.PROTO_PARSED]
 
     def is_valid_response_format(self, formats: Union[str, List[str]]):
         if formats is None:
             return True
```

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/utils/json.py` & `th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/utils/json.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services/data_source/lwdp/utils/misc.py` & `th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services/data_source/lwdp/utils/_misc.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,26 +7,30 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-from datetime import datetime
+from datetime import datetime, timezone
 from typing import List
-from th2_data_services.data_source.lwdp.utils._response_formats import ResponseFormats
+from th2_data_services.data_source.lwdp.utils._response_formats import ResponseFormatsChecker
 
 
 def _check_list_or_tuple(variable, var_name):  # noqa
     if not (isinstance(variable, tuple) or isinstance(variable, list)):
         raise TypeError(f"{var_name} argument has to be list or tuple type. Got {type(variable)}")
 
 
 def _check_datetime(dt: datetime):
     if not isinstance(dt, datetime):
-        raise TypeError("Provided timestamp should be `datetime` object")
+        raise TypeError("Provided timestamp should be `datetime` object in UTC time")
 
 
 def _check_response_formats(formats: List[str]):
-    rf = ResponseFormats()
+    rf = ResponseFormatsChecker()
     if not rf.is_valid_response_format(formats):
         raise Exception("Invalid response format")
+
+
+def get_utc_datetime_now():  # noqa
+    return datetime.now(timezone.utc).replace(microsecond=0)
```

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services_lwdp.egg-info/PKG-INFO` & `th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services_lwdp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: th2-data-services-lwdp
-Version: 2.1.0.0.dev5197375339
+Version: 2.1.0.0.dev5221420794
 Summary: th2_data_services_lwdp
 Home-page: https://github.com/th2-net/th2-ds-source-lwdp
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: # Lightweight Data Provider Data Source (major version 2).
         # Introduction
```

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5197375339/th2_data_services_lwdp.egg-info/SOURCES.txt` & `th2_data_services_lwdp-2.1.0.0.dev5221420794/th2_data_services_lwdp.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 th2_data_services/data_source/lwdp/interfaces/data_source.py
 th2_data_services/data_source/lwdp/interfaces/filter.py
 th2_data_services/data_source/lwdp/interfaces/source_api.py
 th2_data_services/data_source/lwdp/source_api/__init__.py
 th2_data_services/data_source/lwdp/source_api/grpc.py
 th2_data_services/data_source/lwdp/source_api/http.py
 th2_data_services/data_source/lwdp/utils/__init__.py
+th2_data_services/data_source/lwdp/utils/_misc.py
 th2_data_services/data_source/lwdp/utils/_response_formats.py
 th2_data_services/data_source/lwdp/utils/json.py
-th2_data_services/data_source/lwdp/utils/misc.py
 th2_data_services_lwdp.egg-info/PKG-INFO
 th2_data_services_lwdp.egg-info/SOURCES.txt
 th2_data_services_lwdp.egg-info/dependency_links.txt
 th2_data_services_lwdp.egg-info/requires.txt
 th2_data_services_lwdp.egg-info/top_level.txt
```

