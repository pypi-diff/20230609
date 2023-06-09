# Comparing `tmp/pytk_net-0.0.2.tar.gz` & `tmp/pytk_net-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pytk_net-0.0.2.tar", last modified: Wed Jun  7 07:21:41 2023, max compression
+gzip compressed data, was "dist\pytk_net-0.0.3.tar", last modified: Fri Jun  9 06:01:21 2023, max compression
```

## Comparing `pytk_net-0.0.2.tar` & `pytk_net-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 07:21:41.647113 pytk_net-0.0.2/
--rw-rw-rw-   0        0        0      284 2023-06-07 07:21:41.646116 pytk_net-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       51 2023-06-07 06:34:40.000000 pytk_net-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-07 07:21:41.633150 pytk_net-0.0.2/pytk_net/
--rw-rw-rw-   0        0        0        0 2023-06-07 07:13:18.000000 pytk_net-0.0.2/pytk_net/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 07:21:41.644122 pytk_net-0.0.2/pytk_net/icons/
--rw-rw-rw-   0        0        0    49971 2023-05-31 05:59:23.000000 pytk_net-0.0.2/pytk_net/icons/bootstrap-icons.json
--rw-rw-rw-   0        0        0   164360 2023-05-31 05:59:30.000000 pytk_net-0.0.2/pytk_net/icons/bootstrap-icons.woff
--rw-rw-rw-   0        0        0       19 2023-06-07 06:18:58.000000 pytk_net-0.0.2/pytk_net/init.py
--rw-rw-rw-   0        0        0     1912 2023-06-07 06:00:12.000000 pytk_net-0.0.2/pytk_net/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-07 07:21:41.640133 pytk_net-0.0.2/pytk_net.egg-info/
--rw-rw-rw-   0        0        0      284 2023-06-07 07:21:41.000000 pytk_net-0.0.2/pytk_net.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      274 2023-06-07 07:21:41.000000 pytk_net-0.0.2/pytk_net.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 07:21:41.000000 pytk_net-0.0.2/pytk_net.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-07 07:21:41.000000 pytk_net-0.0.2/pytk_net.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-07 07:21:41.647113 pytk_net-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      511 2023-06-07 07:21:37.000000 pytk_net-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:01:21.717586 pytk_net-0.0.3/
+-rw-rw-rw-   0        0        0      284 2023-06-09 06:01:21.717586 pytk_net-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       51 2023-06-07 06:34:40.000000 pytk_net-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-09 06:01:21.717586 pytk_net-0.0.3/pytk_net.egg-info/
+-rw-rw-rw-   0        0        0      284 2023-06-09 06:01:21.000000 pytk_net-0.0.3/pytk_net.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      146 2023-06-09 06:01:21.000000 pytk_net-0.0.3/pytk_net.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 06:01:21.000000 pytk_net-0.0.3/pytk_net.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 06:01:21.000000 pytk_net-0.0.3/pytk_net.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-09 06:01:21.717586 pytk_net-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      511 2023-06-09 05:58:08.000000 pytk_net-0.0.3/setup.py
```

