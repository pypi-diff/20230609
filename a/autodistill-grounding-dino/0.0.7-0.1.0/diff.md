# Comparing `tmp/autodistill_grounding_dino-0.0.7.tar.gz` & `tmp/autodistill-grounding-dino-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autodistill_grounding_dino-0.0.7.tar", last modified: Thu May 18 16:20:02 2023, max compression
+gzip compressed data, was "autodistill-grounding-dino-0.1.0.tar", last modified: Fri Jun  9 11:11:17 2023, max compression
```

## Comparing `autodistill_grounding_dino-0.0.7.tar` & `autodistill-grounding-dino-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-18 16:20:02.532721 autodistill_grounding_dino-0.0.7/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      648 2023-05-18 16:20:02.532721 autodistill_grounding_dino-0.0.7/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3157 2023-05-16 16:46:34.000000 autodistill_grounding_dino-0.0.7/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-18 16:20:02.532721 autodistill_grounding_dino-0.0.7/autodistill_grounding_dino/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       91 2023-05-18 16:18:39.000000 autodistill_grounding_dino-0.0.7/autodistill_grounding_dino/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3113 2023-05-17 21:28:46.000000 autodistill_grounding_dino-0.0.7/autodistill_grounding_dino/grounding_dino.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8235 2023-05-18 16:18:24.000000 autodistill_grounding_dino-0.0.7/autodistill_grounding_dino/helpers.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-18 16:20:02.532721 autodistill_grounding_dino-0.0.7/autodistill_grounding_dino.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      648 2023-05-18 16:20:02.000000 autodistill_grounding_dino-0.0.7/autodistill_grounding_dino.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      408 2023-05-18 16:20:02.000000 autodistill_grounding_dino-0.0.7/autodistill_grounding_dino.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-18 16:20:02.000000 autodistill_grounding_dino-0.0.7/autodistill_grounding_dino.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       67 2023-05-18 16:20:02.000000 autodistill_grounding_dino-0.0.7/autodistill_grounding_dino.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       27 2023-05-18 16:20:02.000000 autodistill_grounding_dino-0.0.7/autodistill_grounding_dino.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-18 16:20:02.532721 autodistill_grounding_dino-0.0.7/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1323 2023-05-17 23:00:02.000000 autodistill_grounding_dino-0.0.7/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-18 16:20:02.532721 autodistill_grounding_dino-0.0.7/test/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       41 2023-05-17 21:20:53.000000 autodistill_grounding_dino-0.0.7/test/test_hello.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-09 11:11:17.974494 autodistill-grounding-dino-0.1.0/
+-rw-r--r--   0 james      (501) staff       (20)    11356 2023-06-09 09:14:42.000000 autodistill-grounding-dino-0.1.0/LICENSE
+-rw-r--r--   0 james      (501) staff       (20)     2338 2023-06-09 11:11:17.974371 autodistill-grounding-dino-0.1.0/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)     1839 2023-06-09 09:17:58.000000 autodistill-grounding-dino-0.1.0/README.md
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-09 11:11:17.973175 autodistill-grounding-dino-0.1.0/autodistill_grounding_dino/
+-rw-r--r--   0 james      (501) staff       (20)       97 2023-06-09 09:11:47.000000 autodistill-grounding-dino-0.1.0/autodistill_grounding_dino/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     1840 2023-06-09 09:12:09.000000 autodistill-grounding-dino-0.1.0/autodistill_grounding_dino/grounding_dino_model.py
+-rw-r--r--   0 james      (501) staff       (20)     3531 2023-06-09 09:11:24.000000 autodistill-grounding-dino-0.1.0/autodistill_grounding_dino/helpers.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-09 11:11:17.974182 autodistill-grounding-dino-0.1.0/autodistill_grounding_dino.egg-info/
+-rw-r--r--   0 james      (501) staff       (20)     2338 2023-06-09 11:11:17.000000 autodistill-grounding-dino-0.1.0/autodistill_grounding_dino.egg-info/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)      403 2023-06-09 11:11:17.000000 autodistill-grounding-dino-0.1.0/autodistill_grounding_dino.egg-info/SOURCES.txt
+-rw-r--r--   0 james      (501) staff       (20)        1 2023-06-09 11:11:17.000000 autodistill-grounding-dino-0.1.0/autodistill_grounding_dino.egg-info/dependency_links.txt
+-rw-r--r--   0 james      (501) staff       (20)      155 2023-06-09 11:11:17.000000 autodistill-grounding-dino-0.1.0/autodistill_grounding_dino.egg-info/requires.txt
+-rw-r--r--   0 james      (501) staff       (20)       27 2023-06-09 11:11:17.000000 autodistill-grounding-dino-0.1.0/autodistill_grounding_dino.egg-info/top_level.txt
+-rw-r--r--   0 james      (501) staff       (20)       38 2023-06-09 11:11:17.974535 autodistill-grounding-dino-0.1.0/setup.cfg
+-rw-r--r--   0 james      (501) staff       (20)     1289 2023-06-09 09:13:28.000000 autodistill-grounding-dino-0.1.0/setup.py
```

### Comparing `autodistill_grounding_dino-0.0.7/setup.py` & `autodistill-grounding-dino-0.1.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,33 @@
 with open("./autodistill_grounding_dino/__init__.py", 'r') as f:
     content = f.read()
     # from https://www.py4u.net/discuss/139845
     version = re.search(r'__version__\s*=\s*[\'"]([^\'"]*)[\'"]', content).group(1)
     
 with open("README.md", "r") as fh:
     long_description = fh.read()
-    
-with open("requirements.txt", "r") as fh:
-    install_requires = fh.read().split('\n')
 
 setuptools.setup(
-    name="autodistill_grounding_dino", 
+    name="autodistill-grounding-dino",
     version=version,
     author="Roboflow",
-    author_email="jacob@roboflow.com",
-    description="Automatically distill large foundational models into smaller, in-domain models for deployment",
-    long_description="Automatically distill large foundational models into smaller, in-domain models for deployment",
+    author_email="support@roboflow.com",
+    description="GroundingDINO module for use with Autodistill",
+    long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/autodistill/autodistill",
-    install_requires=install_requires,
+    url="https://github.com/autodistill/autodistill-grounding-dino",
+    install_requires=[
+        "torch",
+        "autodistill",
+        "numpy>=1.20.0",
+        "opencv-python>=4.6.0",
+        "rf_groundingdino",
+        "rf_segment_anything",
+        "supervision"
+    ],
     packages=find_packages(exclude=("tests",)),
     extras_require={
         "dev": ["flake8", "black==22.3.0", "isort", "twine", "pytest", "wheel"],
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

