# Comparing `tmp/archs4py-0.1.9.tar.gz` & `tmp/archs4py-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "archs4py-0.1.9.tar", last modified: Sat Jun  3 04:22:22 2023, max compression
+gzip compressed data, was "archs4py-0.2.1.tar", last modified: Fri Jun  9 20:01:37 2023, max compression
```

## Comparing `archs4py-0.1.9.tar` & `archs4py-0.2.1.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-06-03 04:22:22.333773 archs4py-0.1.9/
--rw-r--r--   0 maayanlab   (501) staff       (20)    11357 2022-11-01 18:40:54.000000 archs4py-0.1.9/LICENSE
--rw-r--r--   0 maayanlab   (501) staff       (20)     6712 2023-06-03 04:22:22.333638 archs4py-0.1.9/PKG-INFO
--rw-r--r--   0 maayanlab   (501) staff       (20)     6225 2023-06-03 02:35:52.000000 archs4py-0.1.9/README.md
-drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-06-03 04:22:22.332304 archs4py-0.1.9/archs4py/
--rw-r--r--   0 maayanlab   (501) staff       (20)      316 2023-06-02 17:50:36.000000 archs4py-0.1.9/archs4py/__init__.py
-drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-06-03 04:22:22.333337 archs4py-0.1.9/archs4py/data/
--rw-r--r--   0 maayanlab   (501) staff       (20)     2806 2023-05-30 21:18:42.000000 archs4py-0.1.9/archs4py/data/config.json
--rw-r--r--   0 maayanlab   (501) staff       (20)    12493 2023-06-02 16:44:04.000000 archs4py-0.1.9/archs4py/data.py
--rw-r--r--   0 maayanlab   (501) staff       (20)     2053 2023-06-01 21:46:37.000000 archs4py-0.1.9/archs4py/download.py
--rw-r--r--   0 maayanlab   (501) staff       (20)     5963 2023-06-03 02:17:54.000000 archs4py-0.1.9/archs4py/meta.py
--rw-r--r--   0 maayanlab   (501) staff       (20)     2710 2023-06-03 01:03:33.000000 archs4py-0.1.9/archs4py/utils.py
-drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-06-03 04:22:22.333195 archs4py-0.1.9/archs4py.egg-info/
--rw-r--r--   0 maayanlab   (501) staff       (20)     6712 2023-06-03 04:22:22.000000 archs4py-0.1.9/archs4py.egg-info/PKG-INFO
--rw-r--r--   0 maayanlab   (501) staff       (20)      305 2023-06-03 04:22:22.000000 archs4py-0.1.9/archs4py.egg-info/SOURCES.txt
--rw-r--r--   0 maayanlab   (501) staff       (20)        1 2023-06-03 04:22:22.000000 archs4py-0.1.9/archs4py.egg-info/dependency_links.txt
--rw-r--r--   0 maayanlab   (501) staff       (20)      110 2023-06-03 04:22:22.000000 archs4py-0.1.9/archs4py.egg-info/requires.txt
--rw-r--r--   0 maayanlab   (501) staff       (20)        9 2023-06-03 04:22:22.000000 archs4py-0.1.9/archs4py.egg-info/top_level.txt
--rw-r--r--   0 maayanlab   (501) staff       (20)       38 2023-06-03 04:22:22.333820 archs4py-0.1.9/setup.cfg
--rw-r--r--   0 maayanlab   (501) staff       (20)     1018 2023-06-03 04:22:12.000000 archs4py-0.1.9/setup.py
+drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-06-09 20:01:37.904664 archs4py-0.2.1/
+-rw-r--r--   0 maayanlab   (501) staff       (20)    11357 2022-11-01 18:40:54.000000 archs4py-0.2.1/LICENSE
+-rw-r--r--   0 maayanlab   (501) staff       (20)      266 2023-06-09 19:56:39.000000 archs4py-0.2.1/MANIFEST.in
+-rw-r--r--   0 maayanlab   (501) staff       (20)     6919 2023-06-09 20:01:37.904514 archs4py-0.2.1/PKG-INFO
+-rw-r--r--   0 maayanlab   (501) staff       (20)     6432 2023-06-05 17:48:08.000000 archs4py-0.2.1/README.md
+drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-06-09 20:01:37.903376 archs4py-0.2.1/archs4py/
+-rw-r--r--   0 maayanlab   (501) staff       (20)      401 2023-06-07 15:07:46.000000 archs4py-0.2.1/archs4py/__init__.py
+-rw-r--r--   0 maayanlab   (501) staff       (20)     3559 2023-06-09 19:02:34.000000 archs4py-0.2.1/archs4py/align.py
+drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-06-09 20:01:37.904214 archs4py-0.2.1/archs4py/data/
+-rw-r--r--   0 maayanlab   (501) staff       (20)     3080 2023-06-08 15:38:06.000000 archs4py-0.2.1/archs4py/data/config.json
+-rw-r--r--   0 maayanlab   (501) staff       (20)    12493 2023-06-02 16:44:04.000000 archs4py-0.2.1/archs4py/data.py
+-rw-r--r--   0 maayanlab   (501) staff       (20)     2053 2023-06-09 15:16:23.000000 archs4py-0.2.1/archs4py/download.py
+-rw-r--r--   0 maayanlab   (501) staff       (20)     5963 2023-06-03 02:17:54.000000 archs4py-0.2.1/archs4py/meta.py
+-rw-r--r--   0 maayanlab   (501) staff       (20)     3814 2023-06-08 19:32:52.000000 archs4py-0.2.1/archs4py/utils.py
+drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-06-09 20:01:37.904085 archs4py-0.2.1/archs4py.egg-info/
+-rw-r--r--   0 maayanlab   (501) staff       (20)     6919 2023-06-09 20:01:37.000000 archs4py-0.2.1/archs4py.egg-info/PKG-INFO
+-rw-r--r--   0 maayanlab   (501) staff       (20)      335 2023-06-09 20:01:37.000000 archs4py-0.2.1/archs4py.egg-info/SOURCES.txt
+-rw-r--r--   0 maayanlab   (501) staff       (20)        1 2023-06-09 20:01:37.000000 archs4py-0.2.1/archs4py.egg-info/dependency_links.txt
+-rw-r--r--   0 maayanlab   (501) staff       (20)      155 2023-06-09 20:01:37.000000 archs4py-0.2.1/archs4py.egg-info/requires.txt
+-rw-r--r--   0 maayanlab   (501) staff       (20)        9 2023-06-09 20:01:37.000000 archs4py-0.2.1/archs4py.egg-info/top_level.txt
+-rw-r--r--   0 maayanlab   (501) staff       (20)       38 2023-06-09 20:01:37.904721 archs4py-0.2.1/setup.cfg
+-rw-r--r--   0 maayanlab   (501) staff       (20)     1096 2023-06-09 20:01:26.000000 archs4py-0.2.1/setup.py
```

### Comparing `archs4py-0.1.9/LICENSE` & `archs4py-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `archs4py-0.1.9/PKG-INFO` & `archs4py-0.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: archs4py
-Version: 0.1.9
+Version: 0.2.1
 Summary: ARCHS4 python package supporting data loading and data queries.
 Home-page: https://github.com/maayanlab/archs4py
 Author: Alexander Lachmann
 Author-email: alexander.lachmann@mssm.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<img title="archs4py" alt="archs4py" src="https://github-production-user-asset-6210df.s3.amazonaws.com/32603869/242734021-a99ca725-6f10-4e01-85c1-3c1e1694dc68.png">
+<img title="archs4py" alt="archs4py" src="https://user-images.githubusercontent.com/32603869/243101679-c5147d56-fce0-4498-9577-a300df7d6dce.png">
 
 # archs4py - Official Python package to load and query ARCHS4 data
 
 Official ARCHS4 compagnion package. This package is a wrapper for basic H5 commands performed on the ARCHS4 data files. Some of the data access is optimized for specific query strategies and should make this implementation faster than manually querying the data. The package supports automated file download, mutithreading, and some convenience functions such as data normalization.
 
 ## ARCHS4 data
 
@@ -38,14 +38,25 @@
 
 ```python
 import archs4py as a4
 
 file_path = a4.download.counts("human", path="", version="latest")
 ```
 
+### List data fields in H5
+
+The H5 files contain data and meta data information. To list the contents of ARCHS4 H5 files use the built in `ls` function.
+
+```
+import archs4py as a4
+
+file = "human_gene_v2.2.h5"
+a4.ls(file)
+```
+
 ### Data access
 
 archs4py supports several ways to load gene expression data. When querying ARCHS4 be aware that when loading too many samples the system might run out of memory. (e.g. the meta data search term is very broad). In most cases loading several thousand samples at the same time should be no problem. To find relevant samples there are 5 main functions in the `archs4py.data` module. A function to extract N random samples `archs4py.data.rand()`, a function to extract samples by index `archs4py.data.index()`, a function to extract samples based on meta data search `archs4py.data.meta()`, a function to extract samples based on a list of geo accessions `archs4py.data.samples()` and lastly a function to extract all samples belonging to a series `archs4.data.series()`.
 
 
 #### Extract a random set of samples
```

### Comparing `archs4py-0.1.9/README.md` & `archs4py-0.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<img title="archs4py" alt="archs4py" src="https://github-production-user-asset-6210df.s3.amazonaws.com/32603869/242734021-a99ca725-6f10-4e01-85c1-3c1e1694dc68.png">
+<img title="archs4py" alt="archs4py" src="https://user-images.githubusercontent.com/32603869/243101679-c5147d56-fce0-4498-9577-a300df7d6dce.png">
 
 # archs4py - Official Python package to load and query ARCHS4 data
 
 Official ARCHS4 compagnion package. This package is a wrapper for basic H5 commands performed on the ARCHS4 data files. Some of the data access is optimized for specific query strategies and should make this implementation faster than manually querying the data. The package supports automated file download, mutithreading, and some convenience functions such as data normalization.
 
 ## ARCHS4 data
 
@@ -24,14 +24,25 @@
 
 ```python
 import archs4py as a4
 
 file_path = a4.download.counts("human", path="", version="latest")
 ```
 
+### List data fields in H5
+
+The H5 files contain data and meta data information. To list the contents of ARCHS4 H5 files use the built in `ls` function.
+
+```
+import archs4py as a4
+
+file = "human_gene_v2.2.h5"
+a4.ls(file)
+```
+
 ### Data access
 
 archs4py supports several ways to load gene expression data. When querying ARCHS4 be aware that when loading too many samples the system might run out of memory. (e.g. the meta data search term is very broad). In most cases loading several thousand samples at the same time should be no problem. To find relevant samples there are 5 main functions in the `archs4py.data` module. A function to extract N random samples `archs4py.data.rand()`, a function to extract samples by index `archs4py.data.index()`, a function to extract samples based on meta data search `archs4py.data.meta()`, a function to extract samples based on a list of geo accessions `archs4py.data.samples()` and lastly a function to extract all samples belonging to a series `archs4.data.series()`.
 
 
 #### Extract a random set of samples
```

### Comparing `archs4py-0.1.9/archs4py/data/config.json` & `archs4py-0.2.1/archs4py/data/config.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6666666666666666%*

 * *Differences: {"'ALIGNMENT'": "OrderedDict([('latest', OrderedDict([('release', 107), ('biomart', "*

 * *                "'http://jul2022.archive.ensembl.org/biomart')])), ('2.2', "*

 * *                "OrderedDict([('release', 107), ('biomart', "*

 * *                "'http://jul2022.archive.ensembl.org/biomart')]))])"}*

```diff
@@ -1,8 +1,18 @@
 {
+    "ALIGNMENT": {
+        "2.2": {
+            "biomart": "http://jul2022.archive.ensembl.org/biomart",
+            "release": 107
+        },
+        "latest": {
+            "biomart": "http://jul2022.archive.ensembl.org/biomart",
+            "release": 107
+        }
+    },
     "GENE_COUNTS": {
         "HUMAN": {
             "1.11": {
                 "fallback": "https://s3.amazonaws.com/mssm-seq-matrix/human_matrix_v11.h5",
                 "primary": "https://s3.amazonaws.com/mssm-seq-matrix/human_matrix_v11.h5"
             },
             "2.1.2": {
```

### Comparing `archs4py-0.1.9/archs4py/data.py` & `archs4py-0.2.1/archs4py/data.py`

 * *Files identical despite different names*

### Comparing `archs4py-0.1.9/archs4py/download.py` & `archs4py-0.2.1/archs4py/download.py`

 * *Files identical despite different names*

### Comparing `archs4py-0.1.9/archs4py/meta.py` & `archs4py-0.2.1/archs4py/meta.py`

 * *Files identical despite different names*

### Comparing `archs4py-0.1.9/archs4py.egg-info/PKG-INFO` & `archs4py-0.2.1/archs4py.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: archs4py
-Version: 0.1.9
+Version: 0.2.1
 Summary: ARCHS4 python package supporting data loading and data queries.
 Home-page: https://github.com/maayanlab/archs4py
 Author: Alexander Lachmann
 Author-email: alexander.lachmann@mssm.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<img title="archs4py" alt="archs4py" src="https://github-production-user-asset-6210df.s3.amazonaws.com/32603869/242734021-a99ca725-6f10-4e01-85c1-3c1e1694dc68.png">
+<img title="archs4py" alt="archs4py" src="https://user-images.githubusercontent.com/32603869/243101679-c5147d56-fce0-4498-9577-a300df7d6dce.png">
 
 # archs4py - Official Python package to load and query ARCHS4 data
 
 Official ARCHS4 compagnion package. This package is a wrapper for basic H5 commands performed on the ARCHS4 data files. Some of the data access is optimized for specific query strategies and should make this implementation faster than manually querying the data. The package supports automated file download, mutithreading, and some convenience functions such as data normalization.
 
 ## ARCHS4 data
 
@@ -38,14 +38,25 @@
 
 ```python
 import archs4py as a4
 
 file_path = a4.download.counts("human", path="", version="latest")
 ```
 
+### List data fields in H5
+
+The H5 files contain data and meta data information. To list the contents of ARCHS4 H5 files use the built in `ls` function.
+
+```
+import archs4py as a4
+
+file = "human_gene_v2.2.h5"
+a4.ls(file)
+```
+
 ### Data access
 
 archs4py supports several ways to load gene expression data. When querying ARCHS4 be aware that when loading too many samples the system might run out of memory. (e.g. the meta data search term is very broad). In most cases loading several thousand samples at the same time should be no problem. To find relevant samples there are 5 main functions in the `archs4py.data` module. A function to extract N random samples `archs4py.data.rand()`, a function to extract samples by index `archs4py.data.index()`, a function to extract samples based on meta data search `archs4py.data.meta()`, a function to extract samples based on a list of geo accessions `archs4py.data.samples()` and lastly a function to extract all samples belonging to a series `archs4.data.series()`.
 
 
 #### Extract a random set of samples
```

### Comparing `archs4py-0.1.9/setup.py` & `archs4py-0.2.1/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="archs4py",
-    version="0.1.9",
+    version="0.2.1",
     author="Alexander Lachmann",
     author_email="alexander.lachmann@mssm.edu",
     description="ARCHS4 python package supporting data loading and data queries.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/maayanlab/archs4py",
     packages=setuptools.find_packages(),
@@ -27,10 +27,14 @@
         'numpy==1.24.3',
         'pandas==2.0.2',
         'qnorm==0.8.1',
         'setuptools==67.8.0',
         'tqdm==4.65.0',
         'wget==3.2',
         's3fs==2023.5.0',
+        'xalign==0.1.73',
+        'biomart==0.9.2',
+        'xalign==0.1.74'
+
     ],
     python_requires='>=3.7',
 )
```

