# Comparing `tmp/instalmheb-0.1.tar.gz` & `tmp/instalmheb-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "instalmheb-0.1.tar", last modified: Fri Jun  9 10:47:33 2023, max compression
+gzip compressed data, was "instalmheb-0.2.tar", last modified: Fri Jun  9 19:42:22 2023, max compression
```

## Comparing `instalmheb-0.1.tar` & `instalmheb-0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 10:47:33.781050 instalmheb-0.1/
--rw-rw-rw-   0        0        0       36 2023-06-08 21:34:49.000000 instalmheb-0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      333 2023-06-09 10:47:33.781050 instalmheb-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-09 10:47:33.780054 instalmheb-0.1/instalmheb.egg-info/
--rw-rw-rw-   0        0        0      333 2023-06-09 10:47:33.000000 instalmheb-0.1/instalmheb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      156 2023-06-09 10:47:33.000000 instalmheb-0.1/instalmheb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 10:47:33.000000 instalmheb-0.1/instalmheb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 10:47:33.000000 instalmheb-0.1/instalmheb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-09 10:47:33.782052 instalmheb-0.1/setup.cfg
--rw-rw-rw-   0        0        0      408 2023-06-08 21:40:00.000000 instalmheb-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 19:42:22.748088 instalmheb-0.2/
+-rw-rw-rw-   0        0        0       36 2023-06-08 21:34:49.000000 instalmheb-0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      333 2023-06-09 19:42:22.747086 instalmheb-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-09 19:42:22.746087 instalmheb-0.2/instalmheb.egg-info/
+-rw-rw-rw-   0        0        0      333 2023-06-09 19:42:22.000000 instalmheb-0.2/instalmheb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      156 2023-06-09 19:42:22.000000 instalmheb-0.2/instalmheb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 19:42:22.000000 instalmheb-0.2/instalmheb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 19:42:22.000000 instalmheb-0.2/instalmheb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-09 19:42:22.748088 instalmheb-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      408 2023-06-09 19:41:43.000000 instalmheb-0.2/setup.py
```

