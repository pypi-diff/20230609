# Comparing `tmp/skellyai-0.1.8.tar.gz` & `tmp/skellyai-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/skellyai-0.1.8.tar", last modified: Fri Jun  9 20:24:35 2023, max compression
+gzip compressed data, was "dist/skellyai-0.1.9.tar", last modified: Fri Jun  9 20:42:38 2023, max compression
```

## Comparing `skellyai-0.1.8.tar` & `skellyai-0.1.9.tar`

### file list

```diff
@@ -1,13 +1,20 @@
-drwxr-xr-x   0 bennicholl   (501) staff       (20)        0 2023-06-09 20:24:35.873621 skellyai-0.1.8/
--rw-r--r--   0 bennicholl   (501) staff       (20)      407 2023-06-09 20:24:35.873211 skellyai-0.1.8/PKG-INFO
--rw-r--r--   0 bennicholl   (501) staff       (20)       38 2023-06-09 20:24:35.873736 skellyai-0.1.8/setup.cfg
--rw-r--r--   0 bennicholl   (501) staff       (20)      654 2023-06-09 20:24:31.000000 skellyai-0.1.8/setup.py
-drwxr-xr-x   0 bennicholl   (501) staff       (20)        0 2023-06-09 20:24:35.870804 skellyai-0.1.8/skellyai/
--rw-r--r--   0 bennicholl   (501) staff       (20)        0 2023-05-16 16:47:41.000000 skellyai-0.1.8/skellyai/__init__.py
--rw-r--r--   0 bennicholl   (501) staff       (20)     3183 2023-05-18 18:08:51.000000 skellyai-0.1.8/skellyai/train_transformer.py
-drwxr-xr-x   0 bennicholl   (501) staff       (20)        0 2023-06-09 20:24:35.872750 skellyai-0.1.8/skellyai.egg-info/
--rw-r--r--   0 bennicholl   (501) staff       (20)      407 2023-06-09 20:24:35.000000 skellyai-0.1.8/skellyai.egg-info/PKG-INFO
--rw-r--r--   0 bennicholl   (501) staff       (20)      218 2023-06-09 20:24:35.000000 skellyai-0.1.8/skellyai.egg-info/SOURCES.txt
--rw-r--r--   0 bennicholl   (501) staff       (20)        1 2023-06-09 20:24:35.000000 skellyai-0.1.8/skellyai.egg-info/dependency_links.txt
--rw-r--r--   0 bennicholl   (501) staff       (20)       33 2023-06-09 20:24:35.000000 skellyai-0.1.8/skellyai.egg-info/requires.txt
--rw-r--r--   0 bennicholl   (501) staff       (20)        9 2023-06-09 20:24:35.000000 skellyai-0.1.8/skellyai.egg-info/top_level.txt
+drwxr-xr-x   0 bennicholl   (501) staff       (20)        0 2023-06-09 20:42:38.374623 skellyai-0.1.9/
+-rw-r--r--   0 bennicholl   (501) staff       (20)      407 2023-06-09 20:42:38.373969 skellyai-0.1.9/PKG-INFO
+-rw-r--r--   0 bennicholl   (501) staff       (20)       38 2023-06-09 20:42:38.374778 skellyai-0.1.9/setup.cfg
+-rw-r--r--   0 bennicholl   (501) staff       (20)      713 2023-06-09 20:40:39.000000 skellyai-0.1.9/setup.py
+drwxr-xr-x   0 bennicholl   (501) staff       (20)        0 2023-06-09 20:42:38.366395 skellyai-0.1.9/skellyai/
+-rw-r--r--   0 bennicholl   (501) staff       (20)        0 2023-05-16 16:47:41.000000 skellyai-0.1.9/skellyai/__init__.py
+drwxr-xr-x   0 bennicholl   (501) staff       (20)        0 2023-06-09 20:42:38.370859 skellyai-0.1.9/skellyai/get_multi_labels/
+-rw-r--r--   0 bennicholl   (501) staff       (20)        0 2023-05-16 16:47:41.000000 skellyai-0.1.9/skellyai/get_multi_labels/__init__.py
+-rw-r--r--   0 bennicholl   (501) staff       (20)     1686 2023-05-19 20:23:21.000000 skellyai-0.1.9/skellyai/get_multi_labels/get_multi_labels.py
+drwxr-xr-x   0 bennicholl   (501) staff       (20)        0 2023-06-09 20:42:38.372959 skellyai-0.1.9/skellyai/perform_inference/
+-rw-r--r--   0 bennicholl   (501) staff       (20)        0 2023-05-16 16:47:41.000000 skellyai-0.1.9/skellyai/perform_inference/__init__.py
+-rw-r--r--   0 bennicholl   (501) staff       (20)      838 2023-06-09 19:43:52.000000 skellyai-0.1.9/skellyai/perform_inference/get_probs.py
+-rw-r--r--   0 bennicholl   (501) staff       (20)     1922 2023-06-09 20:23:00.000000 skellyai-0.1.9/skellyai/perform_inference/get_probs_mult_keywords.py
+-rw-r--r--   0 bennicholl   (501) staff       (20)     3183 2023-05-18 18:08:51.000000 skellyai-0.1.9/skellyai/train_transformer.py
+drwxr-xr-x   0 bennicholl   (501) staff       (20)        0 2023-06-09 20:42:38.370025 skellyai-0.1.9/skellyai.egg-info/
+-rw-r--r--   0 bennicholl   (501) staff       (20)      407 2023-06-09 20:42:38.000000 skellyai-0.1.9/skellyai.egg-info/PKG-INFO
+-rw-r--r--   0 bennicholl   (501) staff       (20)      435 2023-06-09 20:42:38.000000 skellyai-0.1.9/skellyai.egg-info/SOURCES.txt
+-rw-r--r--   0 bennicholl   (501) staff       (20)        1 2023-06-09 20:42:38.000000 skellyai-0.1.9/skellyai.egg-info/dependency_links.txt
+-rw-r--r--   0 bennicholl   (501) staff       (20)       33 2023-06-09 20:42:38.000000 skellyai-0.1.9/skellyai.egg-info/requires.txt
+-rw-r--r--   0 bennicholl   (501) staff       (20)       62 2023-06-09 20:42:38.000000 skellyai-0.1.9/skellyai.egg-info/top_level.txt
```

### Comparing `skellyai-0.1.8/setup.py` & `skellyai-0.1.9/setup.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1 +1 @@
-from setuptools import setupsetup(    name='skellyai',    version='0.1.8',        description='generated labeled data',    author='Ben Nicholl',    author_email='ben.nicholl66@gmail.com',    license='BSD 2-clause',    packages=['skellyai'],    install_requires=[                      'pandas==1.4.4',                      'sagemaker==2.155.0'                      ],    classifiers=[        'Development Status :: 1 - Planning',        'Intended Audience :: Science/Research',        'License :: OSI Approved :: BSD License',          'Operating System :: POSIX :: Linux',                "Programming Language :: Python :: 3"    ],)
+from setuptools import setupsetup(    name='skellyai',    version='0.1.9',        description='generated labeled data',    author='Ben Nicholl',    author_email='ben.nicholl66@gmail.com',    license='BSD 2-clause',    packages=['skellyai', 'skellyai/perform_inference', 'skellyai/get_multi_labels'],    install_requires=[                      'pandas==1.4.4',                      'sagemaker==2.155.0'                      ],    classifiers=[        'Development Status :: 1 - Planning',        'Intended Audience :: Science/Research',        'License :: OSI Approved :: BSD License',          'Operating System :: POSIX :: Linux',                "Programming Language :: Python :: 3"    ],)
```

### Comparing `skellyai-0.1.8/skellyai/train_transformer.py` & `skellyai-0.1.9/skellyai/train_transformer.py`

 * *Files identical despite different names*

