# Comparing `tmp/microcat-0.1.0.tar.gz` & `tmp/microcat-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microcat-0.1.0.tar", last modified: Fri Jun  9 02:05:11 2023, max compression
+gzip compressed data, was "microcat-0.1.1.tar", last modified: Fri Jun  9 03:45:40 2023, max compression
```

## Comparing `microcat-0.1.0.tar` & `microcat-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,63 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:05:11.085594 microcat-0.1.0/
--rw-r--r--   0 root         (0) root         (0)    34599 2023-06-09 02:02:59.000000 microcat-0.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1298 2023-06-09 02:05:11.085594 microcat-0.1.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      383 2023-05-18 11:49:26.000000 microcat-0.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:05:11.081594 microcat-0.1.0/microcat/
--rwxrwxr-x   0 root         (0) root         (0)       73 2023-06-09 01:42:52.000000 microcat-0.1.0/microcat/__about__.py
--rwxrwxr-x   0 root         (0) root         (0)      298 2023-05-20 02:32:54.000000 microcat-0.1.0/microcat/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     8766 2023-06-04 02:53:41.000000 microcat-0.1.0/microcat/configer.py
--rwxr-xr-x   0 root         (0) root         (0)    18600 2023-06-08 03:55:11.000000 microcat-0.1.0/microcat/corer.py
--rwxr-xr-x   0 root         (0) root         (0)    10460 2023-06-05 09:08:14.000000 microcat-0.1.0/microcat/sample.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:05:11.085594 microcat-0.1.0/microcat.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1298 2023-06-09 02:05:11.000000 microcat-0.1.0/microcat.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      321 2023-06-09 02:05:11.000000 microcat-0.1.0/microcat.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 02:05:11.000000 microcat-0.1.0/microcat.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-06-09 02:05:11.000000 microcat-0.1.0/microcat.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       65 2023-06-09 02:05:11.000000 microcat-0.1.0/microcat.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-06-09 02:05:11.000000 microcat-0.1.0/microcat.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-09 02:05:11.085594 microcat-0.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2272 2023-06-09 02:05:09.000000 microcat-0.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 03:45:40.348115 microcat-0.1.1/
+-rw-r--r--   0 root         (0) root         (0)    34599 2023-06-09 02:02:59.000000 microcat-0.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      396 2023-06-09 03:45:35.000000 microcat-0.1.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1298 2023-06-09 03:45:40.348115 microcat-0.1.1/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      383 2023-05-18 11:49:26.000000 microcat-0.1.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 03:45:40.340115 microcat-0.1.1/microcat/
+-rwxrwxr-x   0 root         (0) root         (0)       73 2023-06-09 02:29:40.000000 microcat-0.1.1/microcat/__about__.py
+-rwxrwxr-x   0 root         (0) root         (0)      911 2023-06-09 03:13:23.000000 microcat-0.1.1/microcat/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 03:45:40.344115 microcat-0.1.1/microcat/config/
+-rw-r--r--   0 root         (0) root         (0)     2655 2023-06-08 02:42:59.000000 microcat-0.1.1/microcat/config/config.yaml
+-rwxr-xr-x   0 root         (0) root         (0)     8766 2023-06-04 02:53:41.000000 microcat-0.1.1/microcat/configer.py
+-rwxr-xr-x   0 root         (0) root         (0)    18617 2023-06-09 02:09:51.000000 microcat-0.1.1/microcat/corer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 03:45:40.344115 microcat-0.1.1/microcat/envs/
+-rw-r--r--   0 root         (0) root         (0)      184 2023-06-08 03:16:48.000000 microcat-0.1.1/microcat/envs/kmer_python.yaml
+-rw-r--r--   0 root         (0) root         (0)      404 2023-06-07 06:44:30.000000 microcat-0.1.1/microcat/envs/kmer_qc.yaml
+-rw-rw-r--   0 root         (0) root         (0)      164 2023-06-07 06:46:24.000000 microcat-0.1.1/microcat/envs/kraken2.yaml
+-rw-r--r--   0 root         (0) root         (0)      133 2023-05-31 02:41:36.000000 microcat-0.1.1/microcat/envs/krakenuniq.yaml
+-rw-r--r--   0 root         (0) root         (0)      109 2023-06-03 12:24:08.000000 microcat-0.1.1/microcat/envs/metaphlan.yaml
+-rwxr-xr-x   0 root         (0) root         (0)      145 2023-06-03 12:24:08.000000 microcat-0.1.1/microcat/envs/pathseq.yaml
+-rw-r--r--   0 root         (0) root         (0)      100 2023-06-07 06:24:12.000000 microcat-0.1.1/microcat/envs/star.yaml
+-rw-r--r--   0 root         (0) root         (0)      140 2023-05-31 02:41:36.000000 microcat-0.1.1/microcat/envs/trimming.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 03:45:40.340115 microcat-0.1.1/microcat/profiles/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 03:45:40.344115 microcat-0.1.1/microcat/profiles/lsf/
+-rw-r--r--   0 root         (0) root         (0)      957 2023-06-03 12:24:08.000000 microcat-0.1.1/microcat/profiles/lsf/CookieCutter.py
+-rw-r--r--   0 root         (0) root         (0)     2242 2023-06-03 12:24:08.000000 microcat-0.1.1/microcat/profiles/lsf/OSLayer.py
+-rw-r--r--   0 root         (0) root         (0)      297 2023-06-03 12:24:08.000000 microcat-0.1.1/microcat/profiles/lsf/config.yaml
+-rwxr-xr-x   0 root         (0) root         (0)     1124 2023-06-03 12:24:08.000000 microcat-0.1.1/microcat/profiles/lsf/lsf_cancel.py
+-rw-r--r--   0 root         (0) root         (0)     1978 2023-06-03 12:24:08.000000 microcat-0.1.1/microcat/profiles/lsf/lsf_config.py
+-rwxr-xr-x   0 root         (0) root         (0)       48 2023-06-03 12:24:08.000000 microcat-0.1.1/microcat/profiles/lsf/lsf_jobscript.sh
+-rwxr-xr-x   0 root         (0) root         (0)     7511 2023-06-03 12:24:08.000000 microcat-0.1.1/microcat/profiles/lsf/lsf_status.py
+-rwxr-xr-x   0 root         (0) root         (0)     8281 2023-06-03 12:24:08.000000 microcat-0.1.1/microcat/profiles/lsf/lsf_submit.py
+-rw-r--r--   0 root         (0) root         (0)     3775 2023-06-03 12:24:08.000000 microcat-0.1.1/microcat/profiles/lsf/memory_units.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 03:45:40.344115 microcat-0.1.1/microcat/rules/
+-rw-r--r--   0 root         (0) root         (0)     1107 2023-06-09 02:29:19.000000 microcat-0.1.1/microcat/rules/ERCC.smk
+-rw-r--r--   0 root         (0) root         (0)    40814 2023-06-09 02:28:56.000000 microcat-0.1.1/microcat/rules/classfier.smk
+-rw-r--r--   0 root         (0) root         (0)     3981 2023-06-07 01:22:00.000000 microcat-0.1.1/microcat/rules/database.smk
+-rw-r--r--   0 root         (0) root         (0)    42201 2023-06-09 02:29:15.000000 microcat-0.1.1/microcat/rules/host.smk
+-rwxr-xr-x   0 root         (0) root         (0)    10460 2023-06-05 09:08:14.000000 microcat-0.1.1/microcat/sample.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 03:45:40.344115 microcat-0.1.1/microcat/scripts/
+-rw-r--r--   0 root         (0) root         (0)    15479 2023-06-08 03:30:56.000000 microcat-0.1.1/microcat/scripts/INVADEseq.py
+-rwxrwxrwx   0 root         (0) root         (0)    19072 2023-06-07 07:14:07.000000 microcat-0.1.1/microcat/scripts/extract_kraken_reads.py
+-rwxrwxrwx   0 root         (0) root         (0)     3849 2023-06-07 07:14:23.000000 microcat-0.1.1/microcat/scripts/extract_microbiome_output.R
+-rwxr-xr-x   0 root         (0) root         (0)     7896 2023-06-03 12:24:08.000000 microcat-0.1.1/microcat/scripts/get_ncbi_domains.py
+-rw-r--r--   0 root         (0) root         (0)     1185 2023-06-07 07:15:11.000000 microcat-0.1.1/microcat/scripts/krak2_output_denosing.R
+-rwxr-xr-x   0 root         (0) root         (0)     6942 2023-06-07 07:15:43.000000 microcat-0.1.1/microcat/scripts/kraken2mpa.py
+-rwxr-xr-x   0 root         (0) root         (0)    14784 2023-06-07 07:15:24.000000 microcat-0.1.1/microcat/scripts/kraken2sc.py
+-rw-r--r--   0 root         (0) root         (0)     4698 2023-06-07 07:14:59.000000 microcat-0.1.1/microcat/scripts/sample_denosing.R
+-rwxrwxrwx   0 root         (0) root         (0)    15665 2023-06-07 07:13:48.000000 microcat-0.1.1/microcat/scripts/sckmer_unpaired.R
+-rwxr-xr-x   0 root         (0) root         (0)     2367 2023-06-03 12:24:08.000000 microcat-0.1.1/microcat/scripts/spilt_bam_by_tag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 03:45:40.344115 microcat-0.1.1/microcat/snakefiles/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 11:37:58.000000 microcat-0.1.1/microcat/snakefiles/bulk_wf.smk
+-rw-r--r--   0 root         (0) root         (0)     1830 2023-06-09 02:28:49.000000 microcat-0.1.1/microcat/snakefiles/scRNA_wf.smk
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 11:38:06.000000 microcat-0.1.1/microcat/snakefiles/spatial_wf.smk
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 03:45:40.344115 microcat-0.1.1/microcat.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1298 2023-06-09 03:45:40.000000 microcat-0.1.1/microcat.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1494 2023-06-09 03:45:40.000000 microcat-0.1.1/microcat.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 03:45:40.000000 microcat-0.1.1/microcat.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-06-09 03:45:40.000000 microcat-0.1.1/microcat.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2023-06-09 03:45:40.000000 microcat-0.1.1/microcat.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-06-09 03:45:40.000000 microcat-0.1.1/microcat.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       67 2023-06-09 01:50:10.000000 microcat-0.1.1/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-09 03:45:40.348115 microcat-0.1.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2273 2023-06-09 03:43:47.000000 microcat-0.1.1/setup.py
```

### Comparing `microcat-0.1.0/LICENSE` & `microcat-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `microcat-0.1.0/PKG-INFO` & `microcat-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microcat
-Version: 0.1.0
+Version: 0.1.1
 Summary: a computational toolbox to identificated microbiome from Omics
 Home-page: https://github.com/ChangxingSu/MicroCAT
 Author: Changxing Su
 Author-email: changxingsu42@gmail.com
 License: GPLv3+
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `microcat-0.1.0/microcat/configer.py` & `microcat-0.1.1/microcat/configer.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.0/microcat/corer.py` & `microcat-0.1.1/microcat/corer.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 import subprocess
 import sys
 import textwrap
 from io import StringIO
 import configer
 import pandas as pd
 
+import microcat
+
 WORKFLOWS_MAG = [
     "host_all",
     "check_all",]
 
 WORKFLOWS_SCRNA = [
     "host_all",
     "kraken2uniq_classified_all",
```

### Comparing `microcat-0.1.0/microcat/sample.py` & `microcat-0.1.1/microcat/sample.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.0/microcat.egg-info/PKG-INFO` & `microcat-0.1.1/microcat.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microcat
-Version: 0.1.0
+Version: 0.1.1
 Summary: a computational toolbox to identificated microbiome from Omics
 Home-page: https://github.com/ChangxingSu/MicroCAT
 Author: Changxing Su
 Author-email: changxingsu42@gmail.com
 License: GPLv3+
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `microcat-0.1.0/setup.py` & `microcat-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,22 +20,23 @@
 try:
     with io.open(os.path.join('README.md'), encoding='utf-8') as f:
         long_description = '\n' + f.read()
 except FileNotFoundError:
     long_description = DESCRIPTION
 
 packages = ["microcat"]
+
 package_data = {
     "microcat": [
         "microcat/config/*.yaml",
         "microcat/envs/*.yaml",
         "microcat/snakefiles/*.smk",
         "microcat/rules/*.smk",
-        "microcat/scritps/*.py",
-        "microcat/scritps/*.R",
+        "microcat/scripts/*.py",
+        "microcat/scripts/*.R",
         "microcat/*.py",
     ]
 }
 
 data_files = [(".", ["LICENSE", "README.md"])]
 
 entry_points = {"console_scripts": ["microcat=microcat.corer:main"]}
```

