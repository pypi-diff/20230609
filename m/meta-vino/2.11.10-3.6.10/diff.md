# Comparing `tmp/meta-vino-2.11.10.tar.gz` & `tmp/meta-vino-3.6.10.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/meta-vino-2.11.10.tar", last modified: Fri Nov 11 03:56:46 2022, max compression
+gzip compressed data, was "dist/meta-vino-3.6.10.tar", last modified: Fri Jun  9 13:27:17 2023, max compression
```

## Comparing `meta-vino-2.11.10.tar` & `meta-vino-3.6.10.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2022-11-11 03:56:46.000000 meta-vino-2.11.10/
--rw-rw-r--   0 cash      (1000) cash      (1000)      286 2022-11-11 03:56:46.000000 meta-vino-2.11.10/PKG-INFO
--rw-rw-r--   0 cash      (1000) cash      (1000)       40 2022-11-09 06:00:33.000000 meta-vino-2.11.10/README.md
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2022-11-11 03:56:46.000000 meta-vino-2.11.10/meta_vino.egg-info/
--rw-rw-r--   0 cash      (1000) cash      (1000)      286 2022-11-11 03:56:46.000000 meta-vino-2.11.10/meta_vino.egg-info/PKG-INFO
--rw-rw-r--   0 cash      (1000) cash      (1000)      526 2022-11-11 03:56:46.000000 meta-vino-2.11.10/meta_vino.egg-info/SOURCES.txt
--rw-rw-r--   0 cash      (1000) cash      (1000)        1 2022-11-11 03:56:46.000000 meta-vino-2.11.10/meta_vino.egg-info/dependency_links.txt
--rw-rw-r--   0 cash      (1000) cash      (1000)       47 2022-11-11 03:56:46.000000 meta-vino-2.11.10/meta_vino.egg-info/requires.txt
--rw-rw-r--   0 cash      (1000) cash      (1000)        9 2022-11-11 03:56:46.000000 meta-vino-2.11.10/meta_vino.egg-info/top_level.txt
--rw-rw-r--   0 cash      (1000) cash      (1000)        1 2022-11-11 03:56:46.000000 meta-vino-2.11.10/meta_vino.egg-info/zip-safe
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2022-11-11 03:56:46.000000 meta-vino-2.11.10/metavino/
--rw-rw-r--   0 cash      (1000) cash      (1000)      116 2022-11-10 08:17:03.000000 meta-vino-2.11.10/metavino/__init__.py
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2022-11-11 03:56:46.000000 meta-vino-2.11.10/metavino/app/
--rw-rw-r--   0 cash      (1000) cash      (1000)      266 2022-11-10 08:16:49.000000 meta-vino-2.11.10/metavino/app/__init__.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     2549 2022-11-10 09:22:51.000000 meta-vino-2.11.10/metavino/app/instance_segment_vino.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     1679 2022-11-09 08:30:52.000000 meta-vino-2.11.10/metavino/app/object_classification_vino.py
--rw-rw-r--   0 cash      (1000) cash      (1000)      275 2022-11-08 11:30:35.000000 meta-vino-2.11.10/metavino/app/object_detection_vino.py
--rw-rw-r--   0 cash      (1000) cash      (1000)      990 2022-11-08 12:47:07.000000 meta-vino-2.11.10/metavino/app/onnx_to_vino.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     1889 2022-11-10 08:16:13.000000 meta-vino-2.11.10/metavino/app/saliency_segment_vino.py
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2022-11-11 03:56:46.000000 meta-vino-2.11.10/metavino/model_zoo/
--rw-rw-r--   0 cash      (1000) cash      (1000)        0 2022-11-08 11:30:50.000000 meta-vino-2.11.10/metavino/model_zoo/__init__.py
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2022-11-11 03:56:46.000000 meta-vino-2.11.10/metavino/utils/
--rw-rw-r--   0 cash      (1000) cash      (1000)       23 2022-11-08 12:00:00.000000 meta-vino-2.11.10/metavino/utils/__init__.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     5700 2022-11-08 11:59:39.000000 meta-vino-2.11.10/metavino/utils/general.py
--rw-rw-r--   0 cash      (1000) cash      (1000)       38 2022-11-11 03:56:46.000000 meta-vino-2.11.10/setup.cfg
--rw-rw-r--   0 cash      (1000) cash      (1000)      674 2022-11-11 03:55:39.000000 meta-vino-2.11.10/setup.py
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-06-09 13:27:17.000000 meta-vino-3.6.10/
+-rw-rw-r--   0 cash      (1000) cash      (1000)      285 2023-06-09 13:27:17.000000 meta-vino-3.6.10/PKG-INFO
+-rw-rw-r--   0 cash      (1000) cash      (1000)       40 2022-11-09 06:00:33.000000 meta-vino-3.6.10/README.md
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-06-09 13:27:17.000000 meta-vino-3.6.10/meta_vino.egg-info/
+-rw-rw-r--   0 cash      (1000) cash      (1000)      285 2023-06-09 13:27:17.000000 meta-vino-3.6.10/meta_vino.egg-info/PKG-INFO
+-rw-rw-r--   0 cash      (1000) cash      (1000)      560 2023-06-09 13:27:17.000000 meta-vino-3.6.10/meta_vino.egg-info/SOURCES.txt
+-rw-rw-r--   0 cash      (1000) cash      (1000)        1 2023-06-09 13:27:17.000000 meta-vino-3.6.10/meta_vino.egg-info/dependency_links.txt
+-rw-rw-r--   0 cash      (1000) cash      (1000)       47 2023-06-09 13:27:17.000000 meta-vino-3.6.10/meta_vino.egg-info/requires.txt
+-rw-rw-r--   0 cash      (1000) cash      (1000)        9 2023-06-09 13:27:17.000000 meta-vino-3.6.10/meta_vino.egg-info/top_level.txt
+-rw-rw-r--   0 cash      (1000) cash      (1000)        1 2023-06-09 13:17:04.000000 meta-vino-3.6.10/meta_vino.egg-info/zip-safe
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-06-09 13:27:17.000000 meta-vino-3.6.10/metavino/
+-rw-rw-r--   0 cash      (1000) cash      (1000)      139 2023-06-09 09:59:52.000000 meta-vino-3.6.10/metavino/__init__.py
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-06-09 13:27:17.000000 meta-vino-3.6.10/metavino/app/
+-rw-rw-r--   0 cash      (1000) cash      (1000)      313 2023-06-09 09:59:37.000000 meta-vino-3.6.10/metavino/app/__init__.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     2549 2022-11-10 09:22:51.000000 meta-vino-3.6.10/metavino/app/instance_segment_vino.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     1679 2022-11-09 08:30:52.000000 meta-vino-3.6.10/metavino/app/object_classification_vino.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)      275 2022-11-08 11:30:35.000000 meta-vino-3.6.10/metavino/app/object_detection_vino.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)      990 2022-11-08 12:47:07.000000 meta-vino-3.6.10/metavino/app/onnx_to_vino.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     1889 2022-11-10 08:16:13.000000 meta-vino-3.6.10/metavino/app/saliency_segment_vino.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     4507 2023-06-09 11:23:11.000000 meta-vino-3.6.10/metavino/app/yolo_segment_vino.py
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-06-09 13:27:17.000000 meta-vino-3.6.10/metavino/model_zoo/
+-rw-rw-r--   0 cash      (1000) cash      (1000)        0 2022-11-08 11:30:50.000000 meta-vino-3.6.10/metavino/model_zoo/__init__.py
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-06-09 13:27:17.000000 meta-vino-3.6.10/metavino/utils/
+-rw-rw-r--   0 cash      (1000) cash      (1000)       23 2022-11-08 12:00:00.000000 meta-vino-3.6.10/metavino/utils/__init__.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     8033 2023-06-09 10:18:29.000000 meta-vino-3.6.10/metavino/utils/general.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)       38 2023-06-09 13:27:17.000000 meta-vino-3.6.10/setup.cfg
+-rw-rw-r--   0 cash      (1000) cash      (1000)      674 2023-06-09 11:22:59.000000 meta-vino-3.6.10/setup.py
```

### Comparing `meta-vino-2.11.10/meta_vino.egg-info/SOURCES.txt` & `meta-vino-3.6.10/meta_vino.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -9,10 +9,11 @@
 metavino/__init__.py
 metavino/app/__init__.py
 metavino/app/instance_segment_vino.py
 metavino/app/object_classification_vino.py
 metavino/app/object_detection_vino.py
 metavino/app/onnx_to_vino.py
 metavino/app/saliency_segment_vino.py
+metavino/app/yolo_segment_vino.py
 metavino/model_zoo/__init__.py
 metavino/utils/__init__.py
 metavino/utils/general.py
```

### Comparing `meta-vino-2.11.10/metavino/app/instance_segment_vino.py` & `meta-vino-3.6.10/metavino/app/instance_segment_vino.py`

 * *Files identical despite different names*

### Comparing `meta-vino-2.11.10/metavino/app/object_classification_vino.py` & `meta-vino-3.6.10/metavino/app/object_classification_vino.py`

 * *Files identical despite different names*

### Comparing `meta-vino-2.11.10/metavino/app/onnx_to_vino.py` & `meta-vino-3.6.10/metavino/app/onnx_to_vino.py`

 * *Files identical despite different names*

### Comparing `meta-vino-2.11.10/metavino/app/saliency_segment_vino.py` & `meta-vino-3.6.10/metavino/app/saliency_segment_vino.py`

 * *Files identical despite different names*

### Comparing `meta-vino-2.11.10/setup.py` & `meta-vino-3.6.10/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     'opencv-python',
     'setuptools',
     'openvino',
     'numpy',
     'pillow',
 ]
 
-__version__ = 'V2.11.10'
+__version__ = 'V3.06.10'
 
 setup(
     name='meta-vino',
     version=__version__,
     author='CachCheng',
     author_email='tkggpdc2007@163.com',
     url='https://github.com/CachCheng/cvopenvino',
```

