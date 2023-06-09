# Comparing `tmp/pytk_net-0.0.3.tar.gz` & `tmp/pytk_net-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pytk_net-0.0.3.tar", last modified: Fri Jun  9 06:01:21 2023, max compression
+gzip compressed data, was "dist\pytk_net-0.0.4.tar", last modified: Fri Jun  9 06:22:33 2023, max compression
```

## Comparing `pytk_net-0.0.3.tar` & `pytk_net-0.0.4.tar`

### file list

```diff
@@ -1,10 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 06:01:21.717586 pytk_net-0.0.3/
--rw-rw-rw-   0        0        0      284 2023-06-09 06:01:21.717586 pytk_net-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       51 2023-06-07 06:34:40.000000 pytk_net-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-09 06:01:21.717586 pytk_net-0.0.3/pytk_net.egg-info/
--rw-rw-rw-   0        0        0      284 2023-06-09 06:01:21.000000 pytk_net-0.0.3/pytk_net.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      146 2023-06-09 06:01:21.000000 pytk_net-0.0.3/pytk_net.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 06:01:21.000000 pytk_net-0.0.3/pytk_net.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 06:01:21.000000 pytk_net-0.0.3/pytk_net.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-09 06:01:21.717586 pytk_net-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      511 2023-06-09 05:58:08.000000 pytk_net-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:22:33.852535 pytk_net-0.0.4/
+-rw-rw-rw-   0        0        0      284 2023-06-09 06:22:33.852535 pytk_net-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       51 2023-06-07 06:34:40.000000 pytk_net-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-09 06:22:33.836916 pytk_net-0.0.4/pytk_net/
+-rw-rw-rw-   0        0        0        0 2023-06-09 06:16:51.000000 pytk_net-0.0.4/pytk_net/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:22:33.852535 pytk_net-0.0.4/pytk_net/icons/
+-rw-rw-rw-   0        0        0    49971 2023-05-31 05:59:23.000000 pytk_net-0.0.4/pytk_net/icons/bootstrap-icons.json
+-rw-rw-rw-   0        0        0   164360 2023-05-31 05:59:30.000000 pytk_net-0.0.4/pytk_net/icons/bootstrap-icons.woff
+-rw-rw-rw-   0        0        0     2039 2023-06-09 06:17:45.000000 pytk_net-0.0.4/pytk_net/utils.py
+-rw-rw-rw-   0        0        0      237 2023-06-09 06:18:33.000000 pytk_net-0.0.4/pytk_net/widgets.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:22:33.852535 pytk_net-0.0.4/pytk_net.egg-info/
+-rw-rw-rw-   0        0        0      284 2023-06-09 06:22:33.000000 pytk_net-0.0.4/pytk_net.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      277 2023-06-09 06:22:33.000000 pytk_net-0.0.4/pytk_net.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 06:22:33.000000 pytk_net-0.0.4/pytk_net.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-09 06:22:33.000000 pytk_net-0.0.4/pytk_net.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-09 06:22:33.852535 pytk_net-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      511 2023-06-09 06:22:21.000000 pytk_net-0.0.4/setup.py
```

