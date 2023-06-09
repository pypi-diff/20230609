# Comparing `tmp/jupyter_echarts-0.1.14.tar.gz` & `tmp/jupyter_echarts-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyter_echarts-0.1.14.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "jupyter_echarts-0.1.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `jupyter_echarts-0.1.14.tar` & `jupyter_echarts-0.1.7.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     1067 2023-06-07 19:17:58.000000 jupyter_echarts-0.1.14/LICENSE
--rw-r--r--   0        0        0     1261 2023-06-09 17:54:52.871826 jupyter_echarts-0.1.14/jupyter_echarts.py
--rw-r--r--   0        0        0      279 2023-06-09 18:03:15.275310 jupyter_echarts-0.1.14/pyproject.toml
--rw-r--r--   0        0        0      144 1970-01-01 00:00:00.000000 jupyter_echarts-0.1.14/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-07 19:17:58.935620 jupyter_echarts-0.1.7/LICENSE
+-rw-r--r--   0        0        0     2310 2023-06-08 04:18:12.960207 jupyter_echarts-0.1.7/jupyter_echarts.py
+-rw-r--r--   0        0        0      278 2023-06-08 06:09:23.613530 jupyter_echarts-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      143 1970-01-01 00:00:00.000000 jupyter_echarts-0.1.7/PKG-INFO
```

### Comparing `jupyter_echarts-0.1.14/LICENSE` & `jupyter_echarts-0.1.7/LICENSE`

 * *Files identical despite different names*

