# Comparing `tmp/audiocraft-0.0.0.tar.gz` & `tmp/audiocraft-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiocraft-0.0.0.tar", last modified: Tue Jul 26 12:39:34 2022, max compression
+gzip compressed data, was "audiocraft-0.0.1.tar", last modified: Fri Jun  9 05:33:01 2023, max compression
```

## Comparing `audiocraft-0.0.0.tar` & `audiocraft-0.0.1.tar`

### file list

```diff
@@ -1,10 +1,82 @@
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2022-07-26 12:39:34.015334 audiocraft-0.0.0/
--rw-r--r--   0 defossez   (501) staff       (20)      497 2022-07-26 12:39:34.014624 audiocraft-0.0.0/PKG-INFO
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2022-07-26 12:39:34.013480 audiocraft-0.0.0/audiocraft.egg-info/
--rw-r--r--   0 defossez   (501) staff       (20)      497 2022-07-26 12:39:33.000000 audiocraft-0.0.0/audiocraft.egg-info/PKG-INFO
--rw-r--r--   0 defossez   (501) staff       (20)      158 2022-07-26 12:39:33.000000 audiocraft-0.0.0/audiocraft.egg-info/SOURCES.txt
--rw-r--r--   0 defossez   (501) staff       (20)        1 2022-07-26 12:39:33.000000 audiocraft-0.0.0/audiocraft.egg-info/dependency_links.txt
--rw-r--r--   0 defossez   (501) staff       (20)       11 2022-07-26 12:39:33.000000 audiocraft-0.0.0/audiocraft.egg-info/top_level.txt
--rw-r--r--   0 defossez   (501) staff       (20)       21 2021-04-27 20:49:32.000000 audiocraft-0.0.0/audiocraft.py
--rw-r--r--   0 defossez   (501) staff       (20)       38 2022-07-26 12:39:34.015523 audiocraft-0.0.0/setup.cfg
--rw-r--r--   0 defossez   (501) staff       (20)     1258 2022-07-26 12:39:22.000000 audiocraft-0.0.0/setup.py
+drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-06-09 05:33:01.445553 audiocraft-0.0.1/
+-rw-rw-r--   0 defossez   (501) staff       (20)      228 2023-06-08 16:14:27.000000 audiocraft-0.0.1/CHANGELOG.md
+-rw-r--r--   0 defossez   (501) staff       (20)     3535 2023-06-08 18:47:37.000000 audiocraft-0.0.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 defossez   (501) staff       (20)     1377 2023-06-08 18:47:37.000000 audiocraft-0.0.1/CONTRIBUTING.md
+-rw-rw-r--   0 defossez   (501) staff       (20)     1088 2023-06-08 16:14:27.000000 audiocraft-0.0.1/LICENSE
+-rw-rw-r--   0 defossez   (501) staff       (20)    17529 2023-06-08 16:14:27.000000 audiocraft-0.0.1/LICENSE_weights
+-rw-rw-r--   0 defossez   (501) staff       (20)      158 2023-06-08 16:14:27.000000 audiocraft-0.0.1/MANIFEST.in
+-rw-r--r--   0 defossez   (501) staff       (20)     5970 2023-06-09 05:32:25.000000 audiocraft-0.0.1/MODEL_CARD.md
+-rw-rw-r--   0 defossez   (501) staff       (20)      340 2023-06-08 16:14:27.000000 audiocraft-0.0.1/Makefile
+-rw-r--r--   0 defossez   (501) staff       (20)     5992 2023-06-09 05:33:01.445794 audiocraft-0.0.1/PKG-INFO
+-rw-r--r--   0 defossez   (501) staff       (20)     4696 2023-06-09 05:32:17.000000 audiocraft-0.0.1/README.md
+drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-06-09 05:33:01.352525 audiocraft-0.0.1/assets/
+-rw-rw-r--   0 defossez   (501) staff       (20)   160496 2023-06-08 16:14:27.000000 audiocraft-0.0.1/assets/bach.mp3
+drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-06-09 05:33:01.355327 audiocraft-0.0.1/audiocraft/
+-rw-rw-r--   0 defossez   (501) staff       (20)      273 2023-06-08 16:21:54.000000 audiocraft-0.0.1/audiocraft/__init__.py
+drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-06-09 05:33:01.366753 audiocraft-0.0.1/audiocraft/data/
+-rw-rw-r--   0 defossez   (501) staff       (20)      249 2023-06-08 16:14:27.000000 audiocraft-0.0.1/audiocraft/data/__init__.py
+-rw-r--r--   0 defossez   (501) staff       (20)     8818 2023-06-08 19:47:47.000000 audiocraft-0.0.1/audiocraft/data/audio.py
+-rw-rw-r--   0 defossez   (501) staff       (20)    21890 2023-06-08 16:14:27.000000 audiocraft-0.0.1/audiocraft/data/audio_dataset.py
+-rw-rw-r--   0 defossez   (501) staff       (20)     7224 2023-06-08 16:14:27.000000 audiocraft-0.0.1/audiocraft/data/audio_utils.py
+-rw-rw-r--   0 defossez   (501) staff       (20)     2122 2023-06-08 16:14:27.000000 audiocraft-0.0.1/audiocraft/data/zip.py
+drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-06-09 05:33:01.378973 audiocraft-0.0.1/audiocraft/models/
+-rw-rw-r--   0 defossez   (501) staff       (20)      321 2023-06-08 16:14:27.000000 audiocraft-0.0.1/audiocraft/models/__init__.py
+-rw-rw-r--   0 defossez   (501) staff       (20)     8591 2023-06-08 16:14:27.000000 audiocraft-0.0.1/audiocraft/models/builders.py
+-rw-rw-r--   0 defossez   (501) staff       (20)    10268 2023-06-08 16:14:27.000000 audiocraft-0.0.1/audiocraft/models/encodec.py
+-rw-rw-r--   0 defossez   (501) staff       (20)    26480 2023-06-08 16:14:27.000000 audiocraft-0.0.1/audiocraft/models/lm.py
+-rw-rw-r--   0 defossez   (501) staff       (20)     2278 2023-06-08 16:14:27.000000 audiocraft-0.0.1/audiocraft/models/loaders.py
+-rw-r--r--   0 defossez   (501) staff       (20)    13532 2023-06-08 20:16:11.000000 audiocraft-0.0.1/audiocraft/models/musicgen.py
+drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-06-09 05:33:01.397448 audiocraft-0.0.1/audiocraft/modules/
+-rw-rw-r--   0 defossez   (501) staff       (20)      497 2023-06-08 16:14:27.000000 audiocraft-0.0.1/audiocraft/modules/__init__.py
+-rw-rw-r--   0 defossez   (501) staff       (20)     3270 2023-06-08 16:14:27.000000 audiocraft-0.0.1/audiocraft/modules/activations.py
+-rw-rw-r--   0 defossez   (501) staff       (20)    27613 2023-06-08 16:14:27.000000 audiocraft-0.0.1/audiocraft/modules/codebooks_patterns.py
+-rw-rw-r--   0 defossez   (501) staff       (20)    41366 2023-06-08 16:14:27.000000 audiocraft-0.0.1/audiocraft/modules/conditioners.py
+-rw-rw-r--   0 defossez   (501) staff       (20)    10506 2023-06-08 16:14:27.000000 audiocraft-0.0.1/audiocraft/modules/conv.py
+-rw-rw-r--   0 defossez   (501) staff       (20)      759 2023-06-08 16:14:27.000000 audiocraft-0.0.1/audiocraft/modules/lstm.py
+-rw-rw-r--   0 defossez   (501) staff       (20)     5436 2023-06-08 16:14:27.000000 audiocraft-0.0.1/audiocraft/modules/rope.py
+-rw-rw-r--   0 defossez   (501) staff       (20)    13868 2023-06-08 16:14:27.000000 audiocraft-0.0.1/audiocraft/modules/seanet.py
+-rw-rw-r--   0 defossez   (501) staff       (20)     4530 2023-06-08 16:14:27.000000 audiocraft-0.0.1/audiocraft/modules/streaming.py
+-rw-rw-r--   0 defossez   (501) staff       (20)    35079 2023-06-08 16:14:27.000000 audiocraft-0.0.1/audiocraft/modules/transformer.py
+-rw-rw-r--   0 defossez   (501) staff       (20)        0 2023-06-08 16:14:27.000000 audiocraft-0.0.1/audiocraft/py.typed
+drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-06-09 05:33:01.403631 audiocraft-0.0.1/audiocraft/quantization/
+-rw-rw-r--   0 defossez   (501) staff       (20)      319 2023-06-08 16:14:27.000000 audiocraft-0.0.1/audiocraft/quantization/__init__.py
+-rw-rw-r--   0 defossez   (501) staff       (20)     3386 2023-06-08 16:14:27.000000 audiocraft-0.0.1/audiocraft/quantization/base.py
+-rw-rw-r--   0 defossez   (501) staff       (20)    14354 2023-06-08 16:14:27.000000 audiocraft-0.0.1/audiocraft/quantization/core_vq.py
+-rw-rw-r--   0 defossez   (501) staff       (20)     4657 2023-06-08 16:14:27.000000 audiocraft-0.0.1/audiocraft/quantization/vq.py
+drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-06-09 05:33:01.418171 audiocraft-0.0.1/audiocraft/utils/
+-rw-rw-r--   0 defossez   (501) staff       (20)      198 2023-06-08 16:14:27.000000 audiocraft-0.0.1/audiocraft/utils/__init__.py
+-rw-rw-r--   0 defossez   (501) staff       (20)     1377 2023-06-08 16:14:27.000000 audiocraft-0.0.1/audiocraft/utils/autocast.py
+-rw-rw-r--   0 defossez   (501) staff       (20)     1907 2023-06-08 16:14:27.000000 audiocraft-0.0.1/audiocraft/utils/export.py
+-rw-r--r--   0 defossez   (501) staff       (20)      885 2023-06-08 18:47:37.000000 audiocraft-0.0.1/audiocraft/utils/notebook.py
+-rw-rw-r--   0 defossez   (501) staff       (20)     8571 2023-06-08 16:14:27.000000 audiocraft-0.0.1/audiocraft/utils/utils.py
+drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-06-09 05:33:01.359730 audiocraft-0.0.1/audiocraft.egg-info/
+-rw-r--r--   0 defossez   (501) staff       (20)     5992 2023-06-09 05:33:01.000000 audiocraft-0.0.1/audiocraft.egg-info/PKG-INFO
+-rw-r--r--   0 defossez   (501) staff       (20)     1752 2023-06-09 05:33:01.000000 audiocraft-0.0.1/audiocraft.egg-info/SOURCES.txt
+-rw-r--r--   0 defossez   (501) staff       (20)        1 2023-06-09 05:33:01.000000 audiocraft-0.0.1/audiocraft.egg-info/dependency_links.txt
+-rw-r--r--   0 defossez   (501) staff       (20)      219 2023-06-09 05:33:01.000000 audiocraft-0.0.1/audiocraft.egg-info/requires.txt
+-rw-r--r--   0 defossez   (501) staff       (20)       17 2023-06-09 05:33:01.000000 audiocraft-0.0.1/audiocraft.egg-info/top_level.txt
+-rw-rw-r--   0 defossez   (501) staff       (20)      134 2023-06-08 16:14:27.000000 audiocraft-0.0.1/mypy.ini
+-rw-rw-r--   0 defossez   (501) staff       (20)      254 2023-06-08 16:14:27.000000 audiocraft-0.0.1/requirements.txt
+-rw-rw-r--   0 defossez   (501) staff       (20)      100 2023-06-09 05:33:01.447012 audiocraft-0.0.1/setup.cfg
+-rw-rw-r--   0 defossez   (501) staff       (20)     1778 2023-06-08 16:14:27.000000 audiocraft-0.0.1/setup.py
+drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-06-09 05:33:01.420122 audiocraft-0.0.1/tests/
+-rw-rw-r--   0 defossez   (501) staff       (20)      198 2023-06-08 16:14:27.000000 audiocraft-0.0.1/tests/__init__.py
+drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-06-09 05:33:01.424188 audiocraft-0.0.1/tests/common_utils/
+-rw-rw-r--   0 defossez   (501) staff       (20)      323 2023-06-08 16:14:27.000000 audiocraft-0.0.1/tests/common_utils/__init__.py
+-rw-rw-r--   0 defossez   (501) staff       (20)     1744 2023-06-08 16:14:27.000000 audiocraft-0.0.1/tests/common_utils/temp_utils.py
+-rw-rw-r--   0 defossez   (501) staff       (20)      872 2023-06-08 16:14:27.000000 audiocraft-0.0.1/tests/common_utils/wav_utils.py
+drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-06-09 05:33:01.430116 audiocraft-0.0.1/tests/data/
+-rw-rw-r--   0 defossez   (501) staff       (20)      198 2023-06-08 16:14:27.000000 audiocraft-0.0.1/tests/data/__init__.py
+-rw-rw-r--   0 defossez   (501) staff       (20)    10518 2023-06-08 16:14:27.000000 audiocraft-0.0.1/tests/data/test_audio.py
+-rw-rw-r--   0 defossez   (501) staff       (20)    15055 2023-06-08 16:14:27.000000 audiocraft-0.0.1/tests/data/test_audio_dataset.py
+-rw-rw-r--   0 defossez   (501) staff       (20)     3738 2023-06-08 16:14:27.000000 audiocraft-0.0.1/tests/data/test_audio_utils.py
+drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-06-09 05:33:01.443528 audiocraft-0.0.1/tests/modules/
+-rw-rw-r--   0 defossez   (501) staff       (20)      198 2023-06-08 16:14:27.000000 audiocraft-0.0.1/tests/modules/__init__.py
+-rw-rw-r--   0 defossez   (501) staff       (20)    10986 2023-06-08 16:14:27.000000 audiocraft-0.0.1/tests/modules/test_codebooks_patterns.py
+-rw-rw-r--   0 defossez   (501) staff       (20)     7383 2023-06-08 16:14:27.000000 audiocraft-0.0.1/tests/modules/test_conv.py
+-rw-rw-r--   0 defossez   (501) staff       (20)      781 2023-06-08 16:14:27.000000 audiocraft-0.0.1/tests/modules/test_lstm.py
+-rw-rw-r--   0 defossez   (501) staff       (20)     4719 2023-06-08 16:14:27.000000 audiocraft-0.0.1/tests/modules/test_rope.py
+-rw-rw-r--   0 defossez   (501) staff       (20)     4874 2023-06-08 16:14:27.000000 audiocraft-0.0.1/tests/modules/test_seanet.py
+-rw-rw-r--   0 defossez   (501) staff       (20)     8788 2023-06-08 16:14:27.000000 audiocraft-0.0.1/tests/modules/test_transformer.py
+drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-06-09 05:33:01.444718 audiocraft-0.0.1/tests/utils/
+-rw-rw-r--   0 defossez   (501) staff       (20)      198 2023-06-08 16:14:27.000000 audiocraft-0.0.1/tests/utils/__init__.py
```

### Comparing `audiocraft-0.0.0/setup.py` & `audiocraft-0.0.1/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,47 +1,65 @@
-# author: adefossez
-# Inspired from https://github.com/kennethreitz/setup.py
+"""
+ Copyright (c) Meta Platforms, Inc. and affiliates.
+ All rights reserved.
+ 
+ This source code is licensed under the license found in the
+ LICENSE file in the root directory of this source tree.
+ 
+"""
 
 from pathlib import Path
 
-from setuptools import setup
+from setuptools import setup, find_packages
+
 
 NAME = 'audiocraft'
-DESCRIPTION = 'Deep learning toolkit for audio applications'
+DESCRIPTION = 'Audio research library for PyTorch'
 
-URL = 'https://github.com/facebookresearch/audiocraft'
-EMAIL = 'defossez@fb.com'
-AUTHOR = 'Alexandre Défossez'
+URL = 'https://github.com/fairinternal/audiocraft'
+AUTHOR = 'FAIR Speech & Audio'
+EMAIL = 'defossez@meta.com'
 REQUIRES_PYTHON = '>=3.8.0'
-VERSION = "0.0.0"
 
-HERE = Path(__file__).parent
+for line in open('audiocraft/__init__.py'):
+    line = line.strip()
+    if '__version__' in line:
+        context = {}
+        exec(line, context)
+        VERSION = context['__version__']
 
-REQUIRED = [i.strip() for i in open("requirements.txt")]
+HERE = Path(__file__).parent
 
 try:
     with open(HERE / "README.md", encoding='utf-8') as f:
         long_description = '\n' + f.read()
 except FileNotFoundError:
     long_description = DESCRIPTION
 
+REQUIRED = [i.strip() for i in open(HERE / 'requirements.txt') if not i.startswith('#')]
+
 setup(
     name=NAME,
     version=VERSION,
     description=DESCRIPTION,
+    author_email=EMAIL,
     long_description=long_description,
     long_description_content_type='text/markdown',
     author=AUTHOR,
-    author_email=EMAIL,
-    python_requires=REQUIRES_PYTHON,
     url=URL,
-    py_modules=['audiocraft'],
+    python_requires=REQUIRES_PYTHON,
     install_requires=REQUIRED,
+    extras_require={
+        'dev': ['coverage', 'flake8', 'mypy', 'pdoc3', 'pytest'],
+    },
+    packages=find_packages(),
+    package_data={'audiocraft': ['py.typed']},
     include_package_data=True,
     license='MIT License',
     classifiers=[
         # Trove classifiers
         # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
         'License :: OSI Approved :: MIT License',
+        'Topic :: Multimedia :: Sound/Audio',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
     ],
 )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

