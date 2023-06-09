# Comparing `tmp/chromahacker-0.1.1.tar.gz` & `tmp/chromahacker-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chromahacker-0.1.1.tar", max compression
+gzip compressed data, was "chromahacker-0.1.2.tar", max compression
```

## Comparing `chromahacker-0.1.1.tar` & `chromahacker-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2023-06-06 19:05:27.092423 chromahacker-0.1.1/README.md
--rw-r--r--   0        0        0     6148 2023-06-06 20:17:27.539807 chromahacker-0.1.1/chromahacker/.DS_Store
--rw-r--r--   0        0        0       89 2023-06-08 16:47:40.434230 chromahacker-0.1.1/chromahacker/__init__.py
--rw-r--r--   0        0        0      860 2023-06-08 17:21:07.733348 chromahacker-0.1.1/chromahacker/color_input.py
--rw-r--r--   0        0        0      485 2023-06-09 00:13:05.423176 chromahacker-0.1.1/chromahacker/palettize.py
--rw-r--r--   0        0        0      266 2023-06-09 00:21:03.357804 chromahacker-0.1.1/chromahacker/process_image.py
--rw-r--r--   0        0        0      424 2023-06-08 17:20:05.944611 chromahacker-0.1.1/chromahacker/spline.py
--rw-r--r--   0        0        0      337 2023-06-09 00:21:42.908530 chromahacker-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      422 1970-01-01 00:00:00.000000 chromahacker-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-06 19:05:27.092423 chromahacker-0.1.2/README.md
+-rw-r--r--   0        0        0     6148 2023-06-06 20:17:27.539807 chromahacker-0.1.2/chromahacker/.DS_Store
+-rw-r--r--   0        0        0       89 2023-06-08 16:47:40.434230 chromahacker-0.1.2/chromahacker/__init__.py
+-rw-r--r--   0        0        0      860 2023-06-08 17:21:07.733348 chromahacker-0.1.2/chromahacker/color_input.py
+-rw-r--r--   0        0        0      485 2023-06-09 00:13:05.423176 chromahacker-0.1.2/chromahacker/palettize.py
+-rw-r--r--   0        0        0      266 2023-06-09 00:21:03.357804 chromahacker-0.1.2/chromahacker/process_image.py
+-rw-r--r--   0        0        0      424 2023-06-08 17:20:05.944611 chromahacker-0.1.2/chromahacker/spline.py
+-rw-r--r--   0        0        0      337 2023-06-09 00:23:28.755740 chromahacker-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      473 1970-01-01 00:00:00.000000 chromahacker-0.1.2/PKG-INFO
```

### Comparing `chromahacker-0.1.1/chromahacker/.DS_Store` & `chromahacker-0.1.2/chromahacker/.DS_Store`

 * *Files identical despite different names*

### Comparing `chromahacker-0.1.1/chromahacker/color_input.py` & `chromahacker-0.1.2/chromahacker/color_input.py`

 * *Files identical despite different names*

