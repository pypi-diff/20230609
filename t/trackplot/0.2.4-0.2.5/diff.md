# Comparing `tmp/trackplot-0.2.4.tar.gz` & `tmp/trackplot-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trackplot-0.2.4.tar", last modified: Sat May  6 03:27:34 2023, max compression
+gzip compressed data, was "trackplot-0.2.5.tar", last modified: Fri Jun  9 10:04:51 2023, max compression
```

## Comparing `trackplot-0.2.4.tar` & `trackplot-0.2.5.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 zhangyiming   (501) staff       (20)        0 2023-05-06 03:27:34.908008 trackplot-0.2.4/
--rw-r--r--   0 zhangyiming   (501) staff       (20)     1558 2022-12-13 02:20:58.000000 trackplot-0.2.4/LICENSE
--rw-r--r--   0 zhangyiming   (501) staff       (20)     6707 2023-05-06 03:27:34.907755 trackplot-0.2.4/PKG-INFO
--rw-r--r--   0 zhangyiming   (501) staff       (20)      381 2023-05-05 02:05:07.000000 trackplot-0.2.4/Pipfile
--rw-r--r--   0 zhangyiming   (501) staff       (20)    95508 2023-05-05 02:05:45.000000 trackplot-0.2.4/Pipfile.lock
--rw-r--r--   0 zhangyiming   (501) staff       (20)     6521 2023-05-05 03:12:18.000000 trackplot-0.2.4/README.md
--rw-r--r--   0 zhangyiming   (501) staff       (20)     1135 2023-05-04 09:50:39.000000 trackplot-0.2.4/pyproject.toml
--rw-r--r--   0 zhangyiming   (501) staff       (20)       38 2023-05-06 03:27:34.908095 trackplot-0.2.4/setup.cfg
--rw-r--r--   0 zhangyiming   (501) staff       (20)     1445 2023-05-06 02:51:20.000000 trackplot-0.2.4/setup.py
-drwxr-xr-x   0 zhangyiming   (501) staff       (20)        0 2023-05-06 03:27:34.895828 trackplot-0.2.4/trackplot/
--rw-r--r--   0 zhangyiming   (501) staff       (20)       38 2023-02-25 03:47:37.000000 trackplot-0.2.4/trackplot/__init__.py
-drwxr-xr-x   0 zhangyiming   (501) staff       (20)        0 2023-05-06 03:27:34.899471 trackplot-0.2.4/trackplot/anno/
--rw-r--r--   0 zhangyiming   (501) staff       (20)      371 2023-02-25 03:47:37.000000 trackplot-0.2.4/trackplot/anno/AxLabel.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)        0 2023-02-25 03:47:37.000000 trackplot-0.2.4/trackplot/anno/__init__.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     1545 2023-02-25 03:47:37.000000 trackplot-0.2.4/trackplot/anno/theme.py
-drwxr-xr-x   0 zhangyiming   (501) staff       (20)        0 2023-05-06 03:27:34.902943 trackplot-0.2.4/trackplot/base/
--rw-r--r--   0 zhangyiming   (501) staff       (20)     7428 2023-02-25 03:47:37.000000 trackplot-0.2.4/trackplot/base/CoordinateMap.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     4330 2023-02-25 15:51:21.000000 trackplot-0.2.4/trackplot/base/GenomicLoci.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     3546 2023-02-25 03:47:37.000000 trackplot-0.2.4/trackplot/base/Junction.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     8883 2023-02-25 03:47:37.000000 trackplot-0.2.4/trackplot/base/Protein.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     8662 2023-05-06 03:18:03.000000 trackplot-0.2.4/trackplot/base/ReadDepth.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     8943 2023-02-25 03:49:51.000000 trackplot-0.2.4/trackplot/base/Readder.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     1200 2023-02-25 03:47:37.000000 trackplot-0.2.4/trackplot/base/Stroke.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     3572 2023-02-25 03:47:37.000000 trackplot-0.2.4/trackplot/base/Transcript.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)        0 2023-02-25 03:47:37.000000 trackplot-0.2.4/trackplot/base/__init__.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     7995 2023-02-25 03:47:37.000000 trackplot-0.2.4/trackplot/base/pyUniprot.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)    43565 2023-05-06 02:51:20.000000 trackplot-0.2.4/trackplot/cli.py
-drwxr-xr-x   0 zhangyiming   (501) staff       (20)        0 2023-05-06 03:27:34.903998 trackplot-0.2.4/trackplot/conf/
--rw-r--r--   0 zhangyiming   (501) staff       (20)     4745 2023-02-25 03:47:37.000000 trackplot-0.2.4/trackplot/conf/DomainSetting.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)        0 2023-02-25 03:47:37.000000 trackplot-0.2.4/trackplot/conf/__init__.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     1329 2023-02-25 03:47:37.000000 trackplot-0.2.4/trackplot/conf/config.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     3803 2023-02-25 03:47:37.000000 trackplot-0.2.4/trackplot/conf/drawing.py
-drwxr-xr-x   0 zhangyiming   (501) staff       (20)        0 2023-05-06 03:27:34.907448 trackplot-0.2.4/trackplot/file/
--rw-r--r--   0 zhangyiming   (501) staff       (20)     6341 2023-02-26 15:22:54.000000 trackplot-0.2.4/trackplot/file/ATAC.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)    12911 2023-02-28 04:50:41.000000 trackplot-0.2.4/trackplot/file/Bam.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     1481 2023-02-25 03:47:37.000000 trackplot-0.2.4/trackplot/file/BedGraph.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     1515 2023-02-25 03:47:37.000000 trackplot-0.2.4/trackplot/file/Bigwig.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     2779 2023-02-25 03:47:37.000000 trackplot-0.2.4/trackplot/file/Depth.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     1237 2023-02-25 03:47:37.000000 trackplot-0.2.4/trackplot/file/Fasta.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     3639 2023-02-25 16:01:18.000000 trackplot-0.2.4/trackplot/file/File.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     6415 2023-02-25 03:47:37.000000 trackplot-0.2.4/trackplot/file/HiCMatrixTrack.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)      966 2023-02-25 03:47:37.000000 trackplot-0.2.4/trackplot/file/Junction.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     1020 2023-02-25 15:59:51.000000 trackplot-0.2.4/trackplot/file/Motif.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)    20328 2023-02-27 13:19:33.000000 trackplot-0.2.4/trackplot/file/ReadSegments.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)    21606 2023-05-05 03:09:45.000000 trackplot-0.2.4/trackplot/file/Reference.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)        0 2023-02-25 03:47:37.000000 trackplot-0.2.4/trackplot/file/__init__.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)    45357 2023-05-06 03:20:22.000000 trackplot-0.2.4/trackplot/plot.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)    52203 2023-02-25 15:55:34.000000 trackplot-0.2.4/trackplot/plot_func.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     6403 2023-02-25 03:47:37.000000 trackplot-0.2.4/trackplot/plot_tests.py
-drwxr-xr-x   0 zhangyiming   (501) staff       (20)        0 2023-05-06 03:27:34.898085 trackplot-0.2.4/trackplot.egg-info/
--rw-r--r--   0 zhangyiming   (501) staff       (20)     6707 2023-05-06 03:27:34.000000 trackplot-0.2.4/trackplot.egg-info/PKG-INFO
--rw-r--r--   0 zhangyiming   (501) staff       (20)     1201 2023-05-06 03:27:34.000000 trackplot-0.2.4/trackplot.egg-info/SOURCES.txt
--rw-r--r--   0 zhangyiming   (501) staff       (20)        1 2023-05-06 03:27:34.000000 trackplot-0.2.4/trackplot.egg-info/dependency_links.txt
--rw-r--r--   0 zhangyiming   (501) staff       (20)       49 2023-05-06 03:27:34.000000 trackplot-0.2.4/trackplot.egg-info/entry_points.txt
--rw-r--r--   0 zhangyiming   (501) staff       (20)        1 2023-05-06 03:27:34.000000 trackplot-0.2.4/trackplot.egg-info/not-zip-safe
--rw-r--r--   0 zhangyiming   (501) staff       (20)      151 2023-05-06 03:27:34.000000 trackplot-0.2.4/trackplot.egg-info/requires.txt
--rw-r--r--   0 zhangyiming   (501) staff       (20)       10 2023-05-06 03:27:34.000000 trackplot-0.2.4/trackplot.egg-info/top_level.txt
+drwxr-xr-x   0 zhangyiming   (501) staff       (20)        0 2023-06-09 10:04:51.043572 trackplot-0.2.5/
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     1558 2022-12-13 02:20:58.000000 trackplot-0.2.5/LICENSE
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     6694 2023-06-09 10:04:51.043298 trackplot-0.2.5/PKG-INFO
+-rw-r--r--   0 zhangyiming   (501) staff       (20)      381 2023-05-05 02:05:07.000000 trackplot-0.2.5/Pipfile
+-rw-r--r--   0 zhangyiming   (501) staff       (20)    95598 2023-05-30 08:48:54.000000 trackplot-0.2.5/Pipfile.lock
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     6508 2023-05-30 02:06:13.000000 trackplot-0.2.5/README.md
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     1136 2023-06-09 10:04:11.000000 trackplot-0.2.5/pyproject.toml
+-rw-r--r--   0 zhangyiming   (501) staff       (20)       38 2023-06-09 10:04:51.043657 trackplot-0.2.5/setup.cfg
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     1445 2023-06-09 10:04:11.000000 trackplot-0.2.5/setup.py
+drwxr-xr-x   0 zhangyiming   (501) staff       (20)        0 2023-06-09 10:04:51.031724 trackplot-0.2.5/trackplot/
+-rw-r--r--   0 zhangyiming   (501) staff       (20)       38 2023-02-25 03:47:37.000000 trackplot-0.2.5/trackplot/__init__.py
+drwxr-xr-x   0 zhangyiming   (501) staff       (20)        0 2023-06-09 10:04:51.034517 trackplot-0.2.5/trackplot/anno/
+-rw-r--r--   0 zhangyiming   (501) staff       (20)      371 2023-02-25 03:47:37.000000 trackplot-0.2.5/trackplot/anno/AxLabel.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)        0 2023-02-25 03:47:37.000000 trackplot-0.2.5/trackplot/anno/__init__.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     1545 2023-02-25 03:47:37.000000 trackplot-0.2.5/trackplot/anno/theme.py
+drwxr-xr-x   0 zhangyiming   (501) staff       (20)        0 2023-06-09 10:04:51.037855 trackplot-0.2.5/trackplot/base/
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     7428 2023-02-25 03:47:37.000000 trackplot-0.2.5/trackplot/base/CoordinateMap.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     4330 2023-02-25 15:51:21.000000 trackplot-0.2.5/trackplot/base/GenomicLoci.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     3546 2023-02-25 03:47:37.000000 trackplot-0.2.5/trackplot/base/Junction.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     8883 2023-02-25 03:47:37.000000 trackplot-0.2.5/trackplot/base/Protein.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     8662 2023-05-06 03:18:03.000000 trackplot-0.2.5/trackplot/base/ReadDepth.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     8943 2023-02-25 03:49:51.000000 trackplot-0.2.5/trackplot/base/Readder.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     1200 2023-02-25 03:47:37.000000 trackplot-0.2.5/trackplot/base/Stroke.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     3572 2023-02-25 03:47:37.000000 trackplot-0.2.5/trackplot/base/Transcript.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)        0 2023-02-25 03:47:37.000000 trackplot-0.2.5/trackplot/base/__init__.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     7995 2023-02-25 03:47:37.000000 trackplot-0.2.5/trackplot/base/pyUniprot.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)    43565 2023-06-09 10:04:39.000000 trackplot-0.2.5/trackplot/cli.py
+drwxr-xr-x   0 zhangyiming   (501) staff       (20)        0 2023-06-09 10:04:51.038966 trackplot-0.2.5/trackplot/conf/
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     4745 2023-02-25 03:47:37.000000 trackplot-0.2.5/trackplot/conf/DomainSetting.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)        0 2023-02-25 03:47:37.000000 trackplot-0.2.5/trackplot/conf/__init__.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     1329 2023-02-25 03:47:37.000000 trackplot-0.2.5/trackplot/conf/config.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     3803 2023-02-25 03:47:37.000000 trackplot-0.2.5/trackplot/conf/drawing.py
+drwxr-xr-x   0 zhangyiming   (501) staff       (20)        0 2023-06-09 10:04:51.042996 trackplot-0.2.5/trackplot/file/
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     6341 2023-02-26 15:22:54.000000 trackplot-0.2.5/trackplot/file/ATAC.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)    12911 2023-02-28 04:50:41.000000 trackplot-0.2.5/trackplot/file/Bam.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     1481 2023-02-25 03:47:37.000000 trackplot-0.2.5/trackplot/file/BedGraph.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     1515 2023-02-25 03:47:37.000000 trackplot-0.2.5/trackplot/file/Bigwig.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     2779 2023-02-25 03:47:37.000000 trackplot-0.2.5/trackplot/file/Depth.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     1237 2023-02-25 03:47:37.000000 trackplot-0.2.5/trackplot/file/Fasta.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     3639 2023-02-25 16:01:18.000000 trackplot-0.2.5/trackplot/file/File.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     6415 2023-02-25 03:47:37.000000 trackplot-0.2.5/trackplot/file/HiCMatrixTrack.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)      966 2023-02-25 03:47:37.000000 trackplot-0.2.5/trackplot/file/Junction.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     1020 2023-02-25 15:59:51.000000 trackplot-0.2.5/trackplot/file/Motif.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)    20328 2023-02-27 13:19:33.000000 trackplot-0.2.5/trackplot/file/ReadSegments.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)    21606 2023-05-05 03:09:45.000000 trackplot-0.2.5/trackplot/file/Reference.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)        0 2023-02-25 03:47:37.000000 trackplot-0.2.5/trackplot/file/__init__.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)    45357 2023-05-06 03:20:22.000000 trackplot-0.2.5/trackplot/plot.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)    52203 2023-02-25 15:55:34.000000 trackplot-0.2.5/trackplot/plot_func.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     6403 2023-02-25 03:47:37.000000 trackplot-0.2.5/trackplot/plot_tests.py
+drwxr-xr-x   0 zhangyiming   (501) staff       (20)        0 2023-06-09 10:04:51.033720 trackplot-0.2.5/trackplot.egg-info/
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     6694 2023-06-09 10:04:51.000000 trackplot-0.2.5/trackplot.egg-info/PKG-INFO
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     1201 2023-06-09 10:04:51.000000 trackplot-0.2.5/trackplot.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangyiming   (501) staff       (20)        1 2023-06-09 10:04:51.000000 trackplot-0.2.5/trackplot.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangyiming   (501) staff       (20)       49 2023-06-09 10:04:51.000000 trackplot-0.2.5/trackplot.egg-info/entry_points.txt
+-rw-r--r--   0 zhangyiming   (501) staff       (20)        1 2023-06-09 10:04:51.000000 trackplot-0.2.5/trackplot.egg-info/not-zip-safe
+-rw-r--r--   0 zhangyiming   (501) staff       (20)      151 2023-06-09 10:04:51.000000 trackplot-0.2.5/trackplot.egg-info/requires.txt
+-rw-r--r--   0 zhangyiming   (501) staff       (20)       10 2023-06-09 10:04:51.000000 trackplot-0.2.5/trackplot.egg-info/top_level.txt
```

### Comparing `trackplot-0.2.4/LICENSE` & `trackplot-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.4/PKG-INFO` & `trackplot-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trackplot
-Version: 0.2.4
+Version: 0.2.5
 Home-page: https://github.com/ygidtu/trackplot
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # trackplot
 
@@ -205,11 +205,11 @@
 
 Visit [issues](https://github.com/ygidtu/trackplot/issues) or 
 contact [Yiming Zhang](https://github.com/ygidtu) and 
 [Ran Zhou](https://github.com/zhou-ran)
 
 ## Citation
 
-If you use Sashimi.py in your publication, please cite Sashimi.py by
+If you use the tool in your publication, please cite by
 
 [Zhang et al. bioRxiv, 2022.11.02.514803.](https://www.biorxiv.org/content/10.1101/2022.11.02.514803v1)
```

### Comparing `trackplot-0.2.4/Pipfile.lock` & `trackplot-0.2.5/Pipfile.lock`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9967948717948718%*

 * *Differences: {"'default'": "{'certifi': {'hashes': "*

 * *              "['sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7', "*

 * *              "'sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716'], "*

 * *              "'version': '==2023.5.7'}, 'cython': {'hashes': "*

 * *              "['sha256:05b7ede0b0eb1c6b9bd748fa67c5ebf3c3560d04d7c8a1486183ddd099de5a00', "*

 * *              "'sha256:0a9334d137bd42fca34b6b413063e19c194ba760846f34804ea1fb477cbe9a88', "*

 * *              "'sha256:156ae92bedcd82 […]*

```diff
@@ -62,19 +62,19 @@
                 "sha256:071ab7b72e3533300b0bfd55a52056b4ffdc1ed6e656779e2aced9b709b8a295"
             ],
             "index": "pypi",
             "version": "==1.5.1"
         },
         "certifi": {
             "hashes": [
-                "sha256:35824b4c3a97115964b408844d64aa14db1cc518f6562e8d7261699d1350a9e3",
-                "sha256:4ad3232f5e926d6718ec31cfc1fcadfde020920e278684144551c91769c7bc18"
+                "sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7",
+                "sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==2022.12.7"
+            "version": "==2023.5.7"
         },
         "cffi": {
             "hashes": [
                 "sha256:00a9ed42e88df81ffae7a8ab6d9356b371399b91dbdf0c3cb1e84c03a13aceb5",
                 "sha256:03425bdae262c76aad70202debd780501fabeaca237cdfddc008987c0e0f59ef",
                 "sha256:04ed324bda3cda42b9b695d51bb7d54b680b9719cfab04227cdd1e04e5de3104",
                 "sha256:0e2642fe3142e4cc4af0799748233ad6da94c62a8bec3a6648bf8ee68b1c7426",
@@ -313,57 +313,58 @@
                 "sha256:9c87405839a19696e837b3b818fed3f5f69f16f1eec1a1ad77e043dcea9c772f"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==0.11.0"
         },
         "cython": {
             "hashes": [
-                "sha256:03daae07f8cbf797506446adae512c3dd86e7f27a62a541fa1ee254baf43e32c",
-                "sha256:0963266dad685812c1dbb758fcd4de78290e3adc7db271c8664dcde27380b13e",
-                "sha256:0ab3cbf3d62b0354631a45dc93cfcdf79098663b1c65a6033af4a452b52217a7",
-                "sha256:0e9032cd650b0cb1d2c2ef2623f5714c14d14c28d7647d589c3eeed0baf7428e",
-                "sha256:11b1b278b8edef215caaa5250ad65a10023bfa0b5a93c776552248fc6f60098d",
-                "sha256:1909688f5d7b521a60c396d20bba9e47a1b2d2784bfb085401e1e1e7d29a29a8",
-                "sha256:1d6c809e2f9ce5950bbc52a1d2352ef3d4fc56186b64cb0d50c8c5a3c1d17661",
-                "sha256:21b88200620d80cfe193d199b259cdad2b9af56f916f0f7f474b5a3631ca0caa",
-                "sha256:308c8f1e58bf5e6e8a1c4dcf8abbd2d13d0f9b1e582f4d9ae8b89857342d8bb5",
-                "sha256:44733366f1604b0c327613b6918469284878d2f5084297d10d26072fc6948d51",
-                "sha256:459994d1de0f99bb18fad9f2325f760c4b392b1324aef37bcc1cd94922dfce41",
-                "sha256:4a2723447d1334484681d5aede34184f2da66317891f94b80e693a2f96a8f1a7",
-                "sha256:56866323f1660cecb4d5ff3a1fba92a56b91b7cfae0a8253777aa4bdb3bdf9a8",
-                "sha256:5718319a01489688fdd22ddebb8e2fcbbd60be5f30de4336ea7063c3ae29fbe5",
-                "sha256:5a8de3e793a576e40ca9b4f5518610cd416273c7dc5e254115656b6e4ec70663",
-                "sha256:5c121dc185040f4333bfded68963b4529698e1b6d994da56be32c97a90c896b6",
-                "sha256:60969d38e6a456a67e7ef8ae20668eff54e32ba439d4068ccf2854a44275a30f",
-                "sha256:67b850cf46b861bc27226d31e1d87c0e69869a02f8d3cc5d5bef549764029879",
-                "sha256:742544024ddb74314e2d597accdb747ed76bd126e61fcf49940a5b5be0a8f381",
-                "sha256:7595d29eaee95633dd8060f50f0e54b27472d01587659557ebcfe39da3ea946b",
-                "sha256:7879992487d9060a61393eeefe00d299210256928dce44d887b6be313d342bac",
-                "sha256:8c3cd8bb8e880a3346f5685601004d96e0a2221e73edcaeea57ea848618b4ac6",
-                "sha256:9489de5b2044dcdfd9d6ca8242a02d560137b3c41b1f5ae1c4f6707d66d6e44d",
-                "sha256:a0f4229df10bc4545ebbeaaf96ebb706011d8b333e54ed202beb03f2bee0a50e",
-                "sha256:a8ad755f9364e720f10a36734a1c7a5ced5c679446718b589259261438a517c9",
-                "sha256:b6149f7cc5b31bccb158c5b968e5a8d374fdc629792e7b928a9b66e08b03fca5",
-                "sha256:bdb3285660e3068438791ace7dd7b1efd6b442a10b5c8d7a4f0c9d184d08c8ed",
-                "sha256:be4f6b7be75a201c290c8611c0978549c60353890204573078e865423dbe3c83",
-                "sha256:ccb223b5f0fd95d8d27561efc0c14502c0945f1a32274835831efa5d5baddfc1",
-                "sha256:cfb2302ef617d647ee590a4c0a00ba3c2da05f301dcefe7721125565d2e51351",
-                "sha256:d7ef5f68f4c5baa93349ea54a352f8716d18bee9a37f3e93eff38a5d4e9b7262",
-                "sha256:d8f822fb6ecd5d88c42136561f82960612421154fc5bf23c57103a367bb91356",
-                "sha256:dbd79221869ee9a6ccc4953b2c8838bb6ae08ab4d50ea4b60d7894f03739417b",
-                "sha256:dce0a36d163c05ae8b21200059511217d79b47baf2b7b0f926e8367bd7a3cc24",
-                "sha256:e40cf86aadc29ecd1cb6de67b0d9488705865deea4fc185c7ad56d7a6fc78703",
-                "sha256:e4401270b0dc464c23671e2e9d52a60985f988318febaf51b047190e855bbe7d",
-                "sha256:e6ef7879668214d80ea3914c17e7d4e1ebf4242e0dd4dabe95ca5ccbe75589a5",
-                "sha256:e971db8aeb12e7c0697cefafe65eefcc33ff1224ae3d8c7f83346cbc42c6c270",
-                "sha256:f674ceb5f722d364395f180fbac273072fc1a266aab924acc9cfd5afc645aae1",
-                "sha256:fd1ea21f1cebf33ae288caa0f3e9b5563a709f4df8925d53bad99be693fc0d9b"
+                "sha256:05b7ede0b0eb1c6b9bd748fa67c5ebf3c3560d04d7c8a1486183ddd099de5a00",
+                "sha256:0a9334d137bd42fca34b6b413063e19c194ba760846f34804ea1fb477cbe9a88",
+                "sha256:156ae92bedcd8261b5259724e2dc4d8eb12ac29159359e34c8358b65d24430ac",
+                "sha256:247d585d8e49f002e522f3420751a4b3da0cf8532ef64d382e0bc9b4c840642c",
+                "sha256:27f58d0dd53a8ffb614814c725d3ee3f136e53178611f7f769ff358f69e50502",
+                "sha256:2a2f2fb9b1c0a4a3890713127fba55a38d2cf1619b2570c43c92a93fee80111a",
+                "sha256:2e1e5d62f15ea4fa4a8bc76e4fcc2ea313a8afe70488b7b870716bcfb12b8246",
+                "sha256:3cd717eee52072be8244bb07f0e4126f893214d2dfd1ba8b38b533e1ffec4f8a",
+                "sha256:3da42ef5b71674e4864b6afbe1bcacba75807684e22b6337f753cf297ae4e2d2",
+                "sha256:402307ad6fd209816cf539680035ef79cce171288cb98f81f3f11ea8ef3afd99",
+                "sha256:417703dc67c447089258ab4b3d217f9c03894574e4a0d6c50648a208bc8352bb",
+                "sha256:445e092708c26b357c97b3c68ea3eab31846fc9c1360bb150225f340c20322ec",
+                "sha256:511f3adfb2db4db2eb882f892525db18a3a21803830474d2fa8b7a1a0f406985",
+                "sha256:516abc754f15b84d6a8e71c8abd90e10346ea86001563480f0be1b349d09c6b8",
+                "sha256:520c50d1875627c111900d7184fd658e32967a3ef807dc2fbc252e384839cbcf",
+                "sha256:537bc1e0ed9bf7289c80f39a9a9359f5649068647631996313f77ba57afde40b",
+                "sha256:563a02ea675ed6321d6257df067c89f17b89a63487ef8b9ce0d598e88e7ff0bd",
+                "sha256:5a47974f3ebccf25702ffdd569904f7807ea1ef0830987c133877fabefdc4bab",
+                "sha256:5cdd65f7d85e15f1662c75d85d837c20d5c68acdd1029bfd08fb44c4422d7d9b",
+                "sha256:6c19e2ba027d2e9e2d88a08aa6007344be781ed99bc0924deb237ec52ca14c09",
+                "sha256:6e381fa0bf08b3c26ec2f616b19ae852c06f5750f4290118bf986b6f85c8c527",
+                "sha256:75541567a2de1f893d247a7f9aa300dff5662fb33822a5fb75bc9621369b8ef0",
+                "sha256:8841158f274896702afe732571d37be22868a301275f952f6280547b25280538",
+                "sha256:94859c3fd90767995b33d803edecad21e73749823db468d34f21e80451a11a99",
+                "sha256:99477c1d4a105a562c05d43cc01905b6711f0a6a558d90f20c7aee0fb23d59d5",
+                "sha256:9e54b4bee55fec952333126147b89c195ebe1d60e8e492ec778916ca5ca03151",
+                "sha256:a1ad51612ff6cfe05cd58f584f01373d64906bb0c860a067c6441359ff10464f",
+                "sha256:acab11c834cbe8fb7b71f9f7b4c4655afd82ffadb1be93d5354a67702fcee69d",
+                "sha256:b63ea04db03190dc8b25d167598989be5c1fe9fc3121d7802c0aafc8a4ec383f",
+                "sha256:ba534e07543b44fb5ae37e56e61072ed1021b2d6ed643dbb92afa8239a04aa83",
+                "sha256:be7e1f98a359408186025f84d28d243e4527acb976f06b8ae8441dc5db204280",
+                "sha256:c17c876db737e1183d18d23db9cc31a9f565c113a32523c672af72f6497e382f",
+                "sha256:c1d7a9ff809fa9b4a9fe04df86c9f7f574ca31c2ad896462a97ea89523db286a",
+                "sha256:c38e2c1e94b596132454b29757536d5afa810011d8bcb86918cc6693d2302940",
+                "sha256:c44bb47b314abc743705c7d038d351ffc3a34b95ab59b04b8cb27cf781b44ae8",
+                "sha256:c4cd7de707938b8385cd1f88e1446228fbfe09af7822fa13877a4374c4881198",
+                "sha256:db695a19968a54b9ac53048c723234b4f0db7409def0a5c5517237202e7a9b92",
+                "sha256:e7b1901b03c37a082ba405e2cf73a57091e835c7af35f664f9dd1d855a992ad5",
+                "sha256:ea1c166336188630cd3e48aea4bbe06ea1bab444624e31c78973fffcae1cf708",
+                "sha256:ef2fc6f81aa8fb512535b01199fbe0d0ecafb8a29f261055e4b3f103c7bd6c75",
+                "sha256:fb8c11cd3e2d5ab7c2da78c5698e527ecbe469437326811562a3fbf4c5780ae4"
             ],
             "markers": "python_version >= '2.6' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-            "version": "==0.29.34"
+            "version": "==0.29.35"
         },
         "cytoolz": {
             "hashes": [
                 "sha256:02975e2b1e61e47e9afa311f4c1783d155136fad37c54a1cebfe991c5a0798a1",
                 "sha256:03ab22c9aeb1535f8647d23b6520b0c3d41aaa18d04ef42b352dde1931f2e2b1",
                 "sha256:061387aa39b9c1576c25d0c59142513c09e77a2a07bd5d6211a43c7a758b6f45",
                 "sha256:06d38a40fe153f23cda0e823413fe9d9ebee89dd461827285316eff929fb121e",
@@ -479,19 +480,19 @@
                 "sha256:7ce71b6880181241cf7ac8697a2f1eb6a8bd9b429f7ad6d27b8db9ba5f1c2d25"
             ],
             "index": "pypi",
             "version": "==1.2.0"
         },
         "fonttools": {
             "hashes": [
-                "sha256:64c0c05c337f826183637570ac5ab49ee220eec66cf50248e8df527edfa95aeb",
-                "sha256:9234b9f57b74e31b192c3fc32ef1a40750a8fbc1cd9837a7b7bfc4ca4a5c51d7"
+                "sha256:106caf6167c4597556b31a8d9175a3fdc0356fdcd70ab19973c3b0d4c893c461",
+                "sha256:dba8d7cdb8e2bac1b3da28c5ed5960de09e59a2fe7e63bb73f5a59e57b0430d2"
             ],
             "markers": "python_version >= '3.8'",
-            "version": "==4.39.3"
+            "version": "==4.39.4"
         },
         "h5py": {
             "hashes": [
                 "sha256:03890b1c123d024fb0239a3279737d5432498c1901c354f8b10d8221d1d16235",
                 "sha256:0fef76e10b9216657fa37e7edff6d8be0709b25bd5066474c229b56cf0098df9",
                 "sha256:26ffc344ec9984d2cd3ca0265007299a8bac8d85c1ad48f4639d8d3aed2af171",
                 "sha256:290e00fa2de74a10688d1bac98d5a9cdd43f14f58e562c580b5b3dfbd358ecae",
@@ -835,42 +836,42 @@
                 "sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==23.1"
         },
         "pandas": {
             "hashes": [
-                "sha256:00959a04a1d7bbc63d75a768540fb20ecc9e65fd80744c930e23768345a362a7",
-                "sha256:03e677c6bc9cfb7f93a8b617d44f6091613a5671ef2944818469be7b42114a00",
-                "sha256:0a514ae436b23a92366fbad8365807fc0eed15ca219690b3445dcfa33597a5cc",
-                "sha256:12bd6618e3cc737c5200ecabbbb5eaba8ab645a4b0db508ceeb4004bb10b060e",
-                "sha256:18d22cb9043b6c6804529810f492ab09d638ddf625c5dea8529239607295cb59",
-                "sha256:19b8e5270da32b41ebf12f0e7165efa7024492e9513fb46fb631c5022ae5709d",
-                "sha256:2b6fe5f7ce1cba0e74188c8473c9091ead9b293ef0a6794939f8cc7947057abd",
-                "sha256:320b180d125c3842c5da5889183b9a43da4ebba375ab2ef938f57bf267a3c684",
-                "sha256:3d099ecaa5b9e977b55cd43cf842ec13b14afa1cfa51b7e1179d90b38c53ce6a",
-                "sha256:6c0853d487b6c868bf107a4b270a823746175b1932093b537b9b76c639fc6f7e",
-                "sha256:6fa0067f2419f933101bdc6001bcea1d50812afbd367b30943417d67fbb99678",
-                "sha256:70a996a1d2432dadedbb638fe7d921c88b0cc4dd90374eab51bb33dc6c0c2a12",
-                "sha256:7b8395d335b08bc8b050590da264f94a439b4770ff16bb51798527f1dd840388",
-                "sha256:7bbf173d364130334e0159a9a034f573e8b44a05320995127cf676b85fd8ce86",
-                "sha256:8db5a644d184a38e6ed40feeb12d410d7fcc36648443defe4707022da127fc35",
-                "sha256:909a72b52175590debbf1d0c9e3e6bce2f1833c80c76d80bd1aa09188be768e5",
-                "sha256:90d1d365d77d287063c5e339f49b27bd99ef06d10a8843cf00b1a49326d492c1",
-                "sha256:910df06feaf9935d05247db6de452f6d59820e432c18a2919a92ffcd98f8f79b",
-                "sha256:99f7192d8b0e6daf8e0d0fd93baa40056684e4b4aaaef9ea78dff34168e1f2f0",
-                "sha256:a2564629b3a47b6aa303e024e3d84e850d36746f7e804347f64229f8c87416ea",
-                "sha256:a37ee35a3eb6ce523b2c064af6286c45ea1c7ff882d46e10d0945dbda7572753",
-                "sha256:af2449e9e984dfad39276b885271ba31c5e0204ffd9f21f287a245980b0e4091",
-                "sha256:e09a53a4fe8d6ae2149959a2d02e1ef2f4d2ceb285ac48f74b79798507e468b4",
-                "sha256:f25e23a03f7ad7211ffa30cb181c3e5f6d96a8e4cb22898af462a7333f8a74eb",
-                "sha256:fe7914d8ddb2d54b900cec264c090b88d141a1eed605c9539a187dbc2547f022"
+                "sha256:02755de164da6827764ceb3bbc5f64b35cb12394b1024fdf88704d0fa06e0e2f",
+                "sha256:0a1e0576611641acde15c2322228d138258f236d14b749ad9af498ab69089e2d",
+                "sha256:1eb09a242184092f424b2edd06eb2b99d06dc07eeddff9929e8667d4ed44e181",
+                "sha256:30a89d0fec4263ccbf96f68592fd668939481854d2ff9da709d32a047689393b",
+                "sha256:50e451932b3011b61d2961b4185382c92cc8c6ee4658dcd4f320687bb2d000ee",
+                "sha256:51a93d422fbb1bd04b67639ba4b5368dffc26923f3ea32a275d2cc450f1d1c86",
+                "sha256:598e9020d85a8cdbaa1815eb325a91cfff2bb2b23c1442549b8a3668e36f0f77",
+                "sha256:66d00300f188fa5de73f92d5725ced162488f6dc6ad4cecfe4144ca29debe3b8",
+                "sha256:69167693cb8f9b3fc060956a5d0a0a8dbfed5f980d9fd2c306fb5b9c855c814c",
+                "sha256:6d6d10c2142d11d40d6e6c0a190b1f89f525bcf85564707e31b0a39e3b398e08",
+                "sha256:713f2f70abcdade1ddd68fc91577cb090b3544b07ceba78a12f799355a13ee44",
+                "sha256:7376e13d28eb16752c398ca1d36ccfe52bf7e887067af9a0474de6331dd948d2",
+                "sha256:77550c8909ebc23e56a89f91b40ad01b50c42cfbfab49b3393694a50549295ea",
+                "sha256:7b21cb72958fc49ad757685db1919021d99650d7aaba676576c9e88d3889d456",
+                "sha256:9ebb9f1c22ddb828e7fd017ea265a59d80461d5a79154b49a4207bd17514d122",
+                "sha256:a18e5c72b989ff0f7197707ceddc99828320d0ca22ab50dd1b9e37db45b010c0",
+                "sha256:a6b5f14cd24a2ed06e14255ff40fe2ea0cfaef79a8dd68069b7ace74bd6acbba",
+                "sha256:b42b120458636a981077cfcfa8568c031b3e8709701315e2bfa866324a83efa8",
+                "sha256:c4af689352c4fe3d75b2834933ee9d0ccdbf5d7a8a7264f0ce9524e877820c08",
+                "sha256:c7319b6e68de14e6209460f72a8d1ef13c09fb3d3ef6c37c1e65b35d50b5c145",
+                "sha256:cf3f0c361a4270185baa89ec7ab92ecaa355fe783791457077473f974f654df5",
+                "sha256:dd46bde7309088481b1cf9c58e3f0e204b9ff9e3244f441accd220dd3365ce7c",
+                "sha256:dd5476b6c3fe410ee95926873f377b856dbc4e81a9c605a0dc05aaccc6a7c6c6",
+                "sha256:e69140bc2d29a8556f55445c15f5794490852af3de0f609a24003ef174528b79",
+                "sha256:f908a77cbeef9bbd646bd4b81214cbef9ac3dda4181d5092a4aa9797d1bc7774"
             ],
             "index": "pypi",
-            "version": "==2.0.1"
+            "version": "==2.0.2"
         },
         "pillow": {
             "hashes": [
                 "sha256:07999f5834bdc404c442146942a2ecadd1cb6292f5229f4ed3b31e0a108746b1",
                 "sha256:0852ddb76d85f127c135b6dd1f0bb88dbb9ee990d2cd9aa9e28526c93e794fba",
                 "sha256:1781a624c229cb35a2ac31cc4a77e28cafc8900733a864870c49bfeedacd106a",
                 "sha256:1e7723bd90ef94eda669a3c2c19d549874dd5badaeefabefd26053304abe5799",
@@ -1068,19 +1069,19 @@
                 "sha256:f84fbc98b019fef2ee9a1cb3ce93e3187a6df0b2538a651bfb890254ba9f90b5"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==6.0"
         },
         "requests": {
             "hashes": [
-                "sha256:10e94cc4f3121ee6da529d358cdaeaff2f1c409cd377dbc72b825852f2f7e294",
-                "sha256:239d7d4458afcb28a692cdd298d87542235f4ca8d36d03a15bfc128a6559a2f4"
+                "sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f",
+                "sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1"
             ],
             "index": "pypi",
-            "version": "==2.30.0"
+            "version": "==2.31.0"
         },
         "scipy": {
             "hashes": [
                 "sha256:049a8bbf0ad95277ffba9b3b7d23e5369cc39e66406d60422c8cfef40ccc8415",
                 "sha256:07c3457ce0b3ad5124f98a86533106b643dd811dd61b548e78cf4c8786652f6f",
                 "sha256:0f1564ea217e82c1bbe75ddf7285ba0709ecd503f048cb1236ae9995f64217bd",
                 "sha256:1553b5dcddd64ba9a0d95355e63fe6c3fc303a8fd77c7bc91e77d61363f7433f",
@@ -1111,19 +1112,19 @@
                 "sha256:ebf15355a4dba46037dfd65b7350f014ceb1f13c05e814eda2c9f5fd731afc08"
             ],
             "index": "pypi",
             "version": "==0.12.2"
         },
         "setuptools": {
             "hashes": [
-                "sha256:23aaf86b85ca52ceb801d32703f12d77517b2556af839621c641fca11287952b",
-                "sha256:f104fa03692a2602fa0fec6c6a9e63b6c8a968de13e17c026957dd1f53d80990"
+                "sha256:5df61bf30bb10c6f756eb19e7c9f3b473051f48db77fddbe06ff2ca307df9a6f",
+                "sha256:62642358adc77ffa87233bc4d2354c4b2682d214048f500964dbe760ccedf102"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==67.7.2"
+            "version": "==67.8.0"
         },
         "simplejson": {
             "hashes": [
                 "sha256:081ea6305b3b5e84ae7417e7f45956db5ea3872ec497a584ec86c3260cda049e",
                 "sha256:08be5a241fdf67a8e05ac7edbd49b07b638ebe4846b560673e196b2a25c94b92",
                 "sha256:0c16ec6a67a5f66ab004190829eeede01c633936375edcad7cbf06d3241e5865",
                 "sha256:0ccb2c1877bc9b25bc4f4687169caa925ffda605d7569c40e8e95186e9a5e58b",
```

### Comparing `trackplot-0.2.4/README.md` & `trackplot-0.2.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -197,11 +197,11 @@
 
 Visit [issues](https://github.com/ygidtu/trackplot/issues) or 
 contact [Yiming Zhang](https://github.com/ygidtu) and 
 [Ran Zhou](https://github.com/zhou-ran)
 
 ## Citation
 
-If you use Sashimi.py in your publication, please cite Sashimi.py by
+If you use the tool in your publication, please cite by
 
 [Zhang et al. bioRxiv, 2022.11.02.514803.](https://www.biorxiv.org/content/10.1101/2022.11.02.514803v1)
```

### Comparing `trackplot-0.2.4/pyproject.toml` & `trackplot-0.2.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "trackplot"
-version = "0.2.2"
+version = "0.2.5"
 description = "The trackplot is a tool for visualizing various next-generation sequencing (NGS) data, including DNA-seq, RNA-seq, single-cell RNA-seq and full-length sequencing datasets. https://sashimi.readthedocs.io/"
 authors = ["ygidtu <ygidtu@gmail.com>"]
 license = "BSD-3"
 readme = "README.md"
 packages = [{include = "trackplot"}]
 
 [tool.poetry.dependencies]
@@ -16,15 +16,15 @@
 filetype = "^1.2.0"
 hicmatrix = "^15"
 loguru = "^0.6.0"
 matplotlib = "^3.6.3"
 numpy = "^1.24.1"
 pandas = "^1.5.3"
 pybigwig = "^0.3.18"
-pysam = "^0.20.0"
+pysam = "^0.21.0"
 requests = "^2.28.2"
 scipy = "^1.10.0"
 seaborn = "^0.12.2"
 xmltodict = "^0.13.0"
 
 
 [[tool.poetry.source]]
@@ -41,8 +41,8 @@
 secondary = true
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
-trackplot = "trackplot.cli:main"
+trackplot = "trackplot.cli:main"
```

### Comparing `trackplot-0.2.4/setup.py` & `trackplot-0.2.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 from configparser import ConfigParser
 from setuptools import setup, find_packages
 
-__version__ = "0.2.4"
+__version__ = "0.2.5"
 __author__ = "ygidtu & Ran Zhou"
 __email__ = "ygidtu@gmail.com"
 
 
 def locate_packages():
     __dir__ = os.path.dirname(os.path.abspath(__file__))
     pipfile = os.path.join(__dir__, "Pipfile")
```

### Comparing `trackplot-0.2.4/trackplot/anno/theme.py` & `trackplot-0.2.5/trackplot/anno/theme.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.4/trackplot/base/CoordinateMap.py` & `trackplot-0.2.5/trackplot/base/CoordinateMap.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.4/trackplot/base/GenomicLoci.py` & `trackplot-0.2.5/trackplot/base/GenomicLoci.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.4/trackplot/base/Junction.py` & `trackplot-0.2.5/trackplot/base/Junction.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.4/trackplot/base/Protein.py` & `trackplot-0.2.5/trackplot/base/Protein.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.4/trackplot/base/ReadDepth.py` & `trackplot-0.2.5/trackplot/base/ReadDepth.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.4/trackplot/base/Readder.py` & `trackplot-0.2.5/trackplot/base/Readder.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.4/trackplot/base/Stroke.py` & `trackplot-0.2.5/trackplot/base/Stroke.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.4/trackplot/base/Transcript.py` & `trackplot-0.2.5/trackplot/base/Transcript.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.4/trackplot/base/pyUniprot.py` & `trackplot-0.2.5/trackplot/base/pyUniprot.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.4/trackplot/cli.py` & `trackplot-0.2.5/trackplot/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from loguru import logger
 
 from trackplot.base.GenomicLoci import GenomicLoci
 from trackplot.conf.config import CLUSTERING_METHOD, COLORS, COLORMAP, DISTANCE_METRIC, IMAGE_TYPE, NORMALIZATION
 from trackplot.file.ATAC import ATAC
 from trackplot.plot import Plot
 
-__version__ = "0.2.4"
+__version__ = "0.2.5"
 __author__ = "ygidtu & Ran Zhou"
 __email__ = "ygidtu@gmail.com"
 
 
 def decode_region(region: str):
     regions = region.split(":")
```

### Comparing `trackplot-0.2.4/trackplot/conf/DomainSetting.py` & `trackplot-0.2.5/trackplot/conf/DomainSetting.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.4/trackplot/conf/config.py` & `trackplot-0.2.5/trackplot/conf/config.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.4/trackplot/conf/drawing.py` & `trackplot-0.2.5/trackplot/conf/drawing.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.4/trackplot/file/ATAC.py` & `trackplot-0.2.5/trackplot/file/ATAC.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.4/trackplot/file/Bam.py` & `trackplot-0.2.5/trackplot/file/Bam.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.4/trackplot/file/BedGraph.py` & `trackplot-0.2.5/trackplot/file/BedGraph.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.4/trackplot/file/Bigwig.py` & `trackplot-0.2.5/trackplot/file/Bigwig.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.4/trackplot/file/Depth.py` & `trackplot-0.2.5/trackplot/file/Depth.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.4/trackplot/file/Fasta.py` & `trackplot-0.2.5/trackplot/file/Fasta.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.4/trackplot/file/File.py` & `trackplot-0.2.5/trackplot/file/File.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.4/trackplot/file/HiCMatrixTrack.py` & `trackplot-0.2.5/trackplot/file/HiCMatrixTrack.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.4/trackplot/file/Junction.py` & `trackplot-0.2.5/trackplot/file/Junction.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.4/trackplot/file/Motif.py` & `trackplot-0.2.5/trackplot/file/Motif.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.4/trackplot/file/ReadSegments.py` & `trackplot-0.2.5/trackplot/file/ReadSegments.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.4/trackplot/file/Reference.py` & `trackplot-0.2.5/trackplot/file/Reference.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.4/trackplot/plot.py` & `trackplot-0.2.5/trackplot/plot.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.4/trackplot/plot_func.py` & `trackplot-0.2.5/trackplot/plot_func.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.4/trackplot/plot_tests.py` & `trackplot-0.2.5/trackplot/plot_tests.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.4/trackplot.egg-info/PKG-INFO` & `trackplot-0.2.5/trackplot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trackplot
-Version: 0.2.4
+Version: 0.2.5
 Home-page: https://github.com/ygidtu/trackplot
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # trackplot
 
@@ -205,11 +205,11 @@
 
 Visit [issues](https://github.com/ygidtu/trackplot/issues) or 
 contact [Yiming Zhang](https://github.com/ygidtu) and 
 [Ran Zhou](https://github.com/zhou-ran)
 
 ## Citation
 
-If you use Sashimi.py in your publication, please cite Sashimi.py by
+If you use the tool in your publication, please cite by
 
 [Zhang et al. bioRxiv, 2022.11.02.514803.](https://www.biorxiv.org/content/10.1101/2022.11.02.514803v1)
```

### Comparing `trackplot-0.2.4/trackplot.egg-info/SOURCES.txt` & `trackplot-0.2.5/trackplot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

