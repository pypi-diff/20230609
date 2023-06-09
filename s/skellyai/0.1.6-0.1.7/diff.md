# Comparing `tmp/skellyai-0.1.6.tar.gz` & `tmp/skellyai-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/skellyai-0.1.6.tar", last modified: Fri May 19 21:00:44 2023, max compression
+gzip compressed data, was "dist/skellyai-0.1.7.tar", last modified: Fri Jun  9 19:58:37 2023, max compression
```

## Comparing `skellyai-0.1.6.tar` & `skellyai-0.1.7.tar`

### file list

```diff
@@ -1,15 +1,13 @@
-drwxr-xr-x   0 bennicholl   (501) staff       (20)        0 2023-05-19 21:00:44.017686 skellyai-0.1.6/
--rw-r--r--   0 bennicholl   (501) staff       (20)      407 2023-05-19 21:00:44.017185 skellyai-0.1.6/PKG-INFO
--rw-r--r--   0 bennicholl   (501) staff       (20)       38 2023-05-19 21:00:44.017891 skellyai-0.1.6/setup.cfg
--rw-r--r--   0 bennicholl   (501) staff       (20)      654 2023-05-19 21:00:15.000000 skellyai-0.1.6/setup.py
-drwxr-xr-x   0 bennicholl   (501) staff       (20)        0 2023-05-19 21:00:44.013384 skellyai-0.1.6/skellyai/
--rw-r--r--   0 bennicholl   (501) staff       (20)        0 2023-05-16 16:47:41.000000 skellyai-0.1.6/skellyai/__init__.py
--rw-r--r--   0 bennicholl   (501) staff       (20)      706 2023-05-19 19:40:35.000000 skellyai-0.1.6/skellyai/label_gen.py
--rw-r--r--   0 bennicholl   (501) staff       (20)     1686 2023-05-19 20:23:21.000000 skellyai-0.1.6/skellyai/multi_label_gen.py
--rw-r--r--   0 bennicholl   (501) staff       (20)     3183 2023-05-18 18:08:51.000000 skellyai-0.1.6/skellyai/train_transformer.py
-drwxr-xr-x   0 bennicholl   (501) staff       (20)        0 2023-05-19 21:00:44.016651 skellyai-0.1.6/skellyai.egg-info/
--rw-r--r--   0 bennicholl   (501) staff       (20)      407 2023-05-19 21:00:43.000000 skellyai-0.1.6/skellyai.egg-info/PKG-INFO
--rw-r--r--   0 bennicholl   (501) staff       (20)      268 2023-05-19 21:00:43.000000 skellyai-0.1.6/skellyai.egg-info/SOURCES.txt
--rw-r--r--   0 bennicholl   (501) staff       (20)        1 2023-05-19 21:00:43.000000 skellyai-0.1.6/skellyai.egg-info/dependency_links.txt
--rw-r--r--   0 bennicholl   (501) staff       (20)       33 2023-05-19 21:00:43.000000 skellyai-0.1.6/skellyai.egg-info/requires.txt
--rw-r--r--   0 bennicholl   (501) staff       (20)        9 2023-05-19 21:00:43.000000 skellyai-0.1.6/skellyai.egg-info/top_level.txt
+drwxr-xr-x   0 bennicholl   (501) staff       (20)        0 2023-06-09 19:58:37.619468 skellyai-0.1.7/
+-rw-r--r--   0 bennicholl   (501) staff       (20)      407 2023-06-09 19:58:37.619040 skellyai-0.1.7/PKG-INFO
+-rw-r--r--   0 bennicholl   (501) staff       (20)       38 2023-06-09 19:58:37.619580 skellyai-0.1.7/setup.cfg
+-rw-r--r--   0 bennicholl   (501) staff       (20)      654 2023-06-09 19:58:27.000000 skellyai-0.1.7/setup.py
+drwxr-xr-x   0 bennicholl   (501) staff       (20)        0 2023-06-09 19:58:37.616672 skellyai-0.1.7/skellyai/
+-rw-r--r--   0 bennicholl   (501) staff       (20)        0 2023-05-16 16:47:41.000000 skellyai-0.1.7/skellyai/__init__.py
+-rw-r--r--   0 bennicholl   (501) staff       (20)     3183 2023-05-18 18:08:51.000000 skellyai-0.1.7/skellyai/train_transformer.py
+drwxr-xr-x   0 bennicholl   (501) staff       (20)        0 2023-06-09 19:58:37.618604 skellyai-0.1.7/skellyai.egg-info/
+-rw-r--r--   0 bennicholl   (501) staff       (20)      407 2023-06-09 19:58:37.000000 skellyai-0.1.7/skellyai.egg-info/PKG-INFO
+-rw-r--r--   0 bennicholl   (501) staff       (20)      218 2023-06-09 19:58:37.000000 skellyai-0.1.7/skellyai.egg-info/SOURCES.txt
+-rw-r--r--   0 bennicholl   (501) staff       (20)        1 2023-06-09 19:58:37.000000 skellyai-0.1.7/skellyai.egg-info/dependency_links.txt
+-rw-r--r--   0 bennicholl   (501) staff       (20)       33 2023-06-09 19:58:37.000000 skellyai-0.1.7/skellyai.egg-info/requires.txt
+-rw-r--r--   0 bennicholl   (501) staff       (20)        9 2023-06-09 19:58:37.000000 skellyai-0.1.7/skellyai.egg-info/top_level.txt
```

### Comparing `skellyai-0.1.6/setup.py` & `skellyai-0.1.7/setup.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1 +1 @@
-from setuptools import setupsetup(    name='skellyai',    version='0.1.6',        description='generated labeled data',    author='Ben Nicholl',    author_email='ben.nicholl66@gmail.com',    license='BSD 2-clause',    packages=['skellyai'],    install_requires=[                      'pandas==1.4.4',                      'sagemaker==2.155.0'                      ],    classifiers=[        'Development Status :: 1 - Planning',        'Intended Audience :: Science/Research',        'License :: OSI Approved :: BSD License',          'Operating System :: POSIX :: Linux',                "Programming Language :: Python :: 3"    ],)
+from setuptools import setupsetup(    name='skellyai',    version='0.1.7',        description='generated labeled data',    author='Ben Nicholl',    author_email='ben.nicholl66@gmail.com',    license='BSD 2-clause',    packages=['skellyai'],    install_requires=[                      'pandas==1.4.4',                      'sagemaker==2.155.0'                      ],    classifiers=[        'Development Status :: 1 - Planning',        'Intended Audience :: Science/Research',        'License :: OSI Approved :: BSD License',          'Operating System :: POSIX :: Linux',                "Programming Language :: Python :: 3"    ],)
```

### Comparing `skellyai-0.1.6/skellyai/train_transformer.py` & `skellyai-0.1.7/skellyai/train_transformer.py`

 * *Files identical despite different names*

