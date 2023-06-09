# Comparing `tmp/augshufflenet-pytorch-0.0.1.tar.gz` & `tmp/augshufflenet-pytorch-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "augshufflenet-pytorch-0.0.1.tar", last modified: Fri Jun  9 15:00:09 2023, max compression
+gzip compressed data, was "augshufflenet-pytorch-0.0.2.tar", last modified: Fri Jun  9 15:03:09 2023, max compression
```

## Comparing `augshufflenet-pytorch-0.0.1.tar` & `augshufflenet-pytorch-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 null      (1000) null      (1000)        0 2023-06-09 15:00:09.238132 augshufflenet-pytorch-0.0.1/
--rw-r--r--   0 null      (1000) null      (1000)    16727 2023-06-09 13:48:21.000000 augshufflenet-pytorch-0.0.1/LICENSE
--rw-r--r--   0 null      (1000) null      (1000)      701 2023-06-09 15:00:09.238132 augshufflenet-pytorch-0.0.1/PKG-INFO
--rw-r--r--   0 null      (1000) null      (1000)     1988 2023-06-09 14:58:10.000000 augshufflenet-pytorch-0.0.1/README.md
-drwxr-xr-x   0 null      (1000) null      (1000)        0 2023-06-09 15:00:09.238132 augshufflenet-pytorch-0.0.1/augshufflenet_pytorch/
--rw-r--r--   0 null      (1000) null      (1000)     6636 2023-06-09 14:54:31.000000 augshufflenet-pytorch-0.0.1/augshufflenet_pytorch/__init__.py
-drwxr-xr-x   0 null      (1000) null      (1000)        0 2023-06-09 15:00:09.238132 augshufflenet-pytorch-0.0.1/augshufflenet_pytorch.egg-info/
--rw-r--r--   0 null      (1000) null      (1000)      701 2023-06-09 15:00:09.000000 augshufflenet-pytorch-0.0.1/augshufflenet_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 null      (1000) null      (1000)      284 2023-06-09 15:00:09.000000 augshufflenet-pytorch-0.0.1/augshufflenet_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 null      (1000) null      (1000)        1 2023-06-09 15:00:09.000000 augshufflenet-pytorch-0.0.1/augshufflenet_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 null      (1000) null      (1000)       24 2023-06-09 15:00:09.000000 augshufflenet-pytorch-0.0.1/augshufflenet_pytorch.egg-info/requires.txt
--rw-r--r--   0 null      (1000) null      (1000)       22 2023-06-09 15:00:09.000000 augshufflenet-pytorch-0.0.1/augshufflenet_pytorch.egg-info/top_level.txt
--rw-r--r--   0 null      (1000) null      (1000)       38 2023-06-09 15:00:09.238132 augshufflenet-pytorch-0.0.1/setup.cfg
--rw-r--r--   0 null      (1000) null      (1000)      877 2023-06-09 13:50:54.000000 augshufflenet-pytorch-0.0.1/setup.py
+drwxr-xr-x   0 null      (1000) null      (1000)        0 2023-06-09 15:03:09.643524 augshufflenet-pytorch-0.0.2/
+-rw-r--r--   0 null      (1000) null      (1000)    16727 2023-06-09 13:48:21.000000 augshufflenet-pytorch-0.0.2/LICENSE
+-rw-r--r--   0 null      (1000) null      (1000)     2682 2023-06-09 15:03:09.642524 augshufflenet-pytorch-0.0.2/PKG-INFO
+-rw-r--r--   0 null      (1000) null      (1000)     1988 2023-06-09 14:58:10.000000 augshufflenet-pytorch-0.0.2/README.md
+drwxr-xr-x   0 null      (1000) null      (1000)        0 2023-06-09 15:03:09.642524 augshufflenet-pytorch-0.0.2/augshufflenet_pytorch/
+-rw-r--r--   0 null      (1000) null      (1000)     6636 2023-06-09 14:54:31.000000 augshufflenet-pytorch-0.0.2/augshufflenet_pytorch/__init__.py
+drwxr-xr-x   0 null      (1000) null      (1000)        0 2023-06-09 15:03:09.642524 augshufflenet-pytorch-0.0.2/augshufflenet_pytorch.egg-info/
+-rw-r--r--   0 null      (1000) null      (1000)     2682 2023-06-09 15:03:09.000000 augshufflenet-pytorch-0.0.2/augshufflenet_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 null      (1000) null      (1000)      284 2023-06-09 15:03:09.000000 augshufflenet-pytorch-0.0.2/augshufflenet_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 null      (1000) null      (1000)        1 2023-06-09 15:03:09.000000 augshufflenet-pytorch-0.0.2/augshufflenet_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 null      (1000) null      (1000)       24 2023-06-09 15:03:09.000000 augshufflenet-pytorch-0.0.2/augshufflenet_pytorch.egg-info/requires.txt
+-rw-r--r--   0 null      (1000) null      (1000)       22 2023-06-09 15:03:09.000000 augshufflenet-pytorch-0.0.2/augshufflenet_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 null      (1000) null      (1000)       38 2023-06-09 15:03:09.643524 augshufflenet-pytorch-0.0.2/setup.cfg
+-rw-r--r--   0 null      (1000) null      (1000)      925 2023-06-09 15:02:55.000000 augshufflenet-pytorch-0.0.2/setup.py
```

### Comparing `augshufflenet-pytorch-0.0.1/LICENSE` & `augshufflenet-pytorch-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `augshufflenet-pytorch-0.0.1/README.md` & `augshufflenet-pytorch-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `augshufflenet-pytorch-0.0.1/augshufflenet_pytorch/__init__.py` & `augshufflenet-pytorch-0.0.2/augshufflenet_pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `augshufflenet-pytorch-0.0.1/setup.py` & `augshufflenet-pytorch-0.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'augshufflenet-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.0.1',
+  version = '0.0.2',
   license='MIT',
   description = 'AugShuffleNet: Communicate More, Compute Less - Pytorch',
   author = 'Ferris Kwaijtaal',
   author_email = 'ferris+gh@devdroplets.com',
-  long_description_content_type = 'text/markdown',
+  long_description_content_type='text/markdown',
+  long_description=open('README.md', 'r').read(),
   url = 'https://github.com/i404788/augshufflenet-pytorch',
   keywords = [
     'artificial intelligence',
     'deep learning',
     'shufflenet',
     'convnet',
     'computer vision'
```

