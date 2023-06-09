# Comparing `tmp/loreme-0.1.1.tar.gz` & `tmp/loreme-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loreme-0.1.1.tar", last modified: Mon Jun  5 20:22:19 2023, max compression
+gzip compressed data, was "loreme-0.1.2.tar", last modified: Fri Jun  9 16:52:50 2023, max compression
```

## Comparing `loreme-0.1.1.tar` & `loreme-0.1.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-06-05 20:22:19.211691 loreme-0.1.1/
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     1520 2023-06-05 04:30:20.000000 loreme-0.1.1/LICENSE
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     2882 2023-06-05 20:22:19.209466 loreme-0.1.1/PKG-INFO
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     2367 2023-06-05 20:21:59.000000 loreme-0.1.1/README.md
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-06-05 20:22:19.161918 loreme-0.1.1/loreme.egg-info/
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     2882 2023-06-05 20:22:19.000000 loreme-0.1.1/loreme.egg-info/PKG-INFO
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      717 2023-06-05 20:22:19.000000 loreme-0.1.1/loreme.egg-info/SOURCES.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)        1 2023-06-05 20:22:19.000000 loreme-0.1.1/loreme.egg-info/dependency_links.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       46 2023-06-05 20:22:19.000000 loreme-0.1.1/loreme.egg-info/entry_points.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       77 2023-06-05 20:22:19.000000 loreme-0.1.1/loreme.egg-info/requires.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)        7 2023-06-05 20:22:19.000000 loreme-0.1.1/loreme.egg-info/top_level.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      918 2023-06-05 19:39:48.000000 loreme-0.1.1/pyproject.toml
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       38 2023-06-05 20:22:19.212123 loreme-0.1.1/setup.cfg
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-06-05 20:22:19.153668 loreme-0.1.1/src/
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-06-05 20:22:19.208506 loreme-0.1.1/src/loreme/
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     1512 2023-06-05 20:07:53.000000 loreme-0.1.1/src/loreme/__init__.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     2645 2023-06-05 04:30:20.000000 loreme-0.1.1/src/loreme/check_gpu_availability.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     3098 2023-06-05 04:30:20.000000 loreme-0.1.1/src/loreme/dorado.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     4872 2023-06-05 04:30:20.000000 loreme-0.1.1/src/loreme/download.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     2553 2023-06-05 04:30:20.000000 loreme-0.1.1/src/loreme/env.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     1496 2023-06-05 04:30:20.000000 loreme-0.1.1/src/loreme/export_bedgraph.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     3440 2023-06-05 04:30:20.000000 loreme-0.1.1/src/loreme/gene_body_methylation.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     1144 2023-06-05 04:30:20.000000 loreme-0.1.1/src/loreme/intersect.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)    33140 2023-06-05 19:18:15.000000 loreme-0.1.1/src/loreme/loreme.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     5191 2023-06-05 04:30:20.000000 loreme-0.1.1/src/loreme/mean.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     1690 2023-06-05 04:30:20.000000 loreme-0.1.1/src/loreme/merge.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      940 2023-06-05 04:30:20.000000 loreme-0.1.1/src/loreme/methylation_hist.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     3054 2023-06-05 04:30:20.000000 loreme-0.1.1/src/loreme/parse_gff.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     2610 2023-06-05 04:30:20.000000 loreme-0.1.1/src/loreme/pbcpg.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     6487 2023-06-05 04:30:20.000000 loreme-0.1.1/src/loreme/plot.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     2440 2023-06-05 04:30:20.000000 loreme-0.1.1/src/loreme/plot_bedtools.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     5087 2023-06-05 04:30:20.000000 loreme-0.1.1/src/loreme/plot_genes.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     4327 2023-06-05 04:30:20.000000 loreme-0.1.1/src/loreme/plot_repeats.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     3433 2023-06-05 04:30:20.000000 loreme-0.1.1/src/loreme/promoter_methylation.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       90 2023-06-05 04:30:20.000000 loreme-0.1.1/src/loreme/version.py
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-06-09 16:52:50.621053 loreme-0.1.2/
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     1520 2023-06-05 04:30:20.000000 loreme-0.1.2/LICENSE
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     2882 2023-06-09 16:52:50.620607 loreme-0.1.2/PKG-INFO
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     2367 2023-06-05 20:21:59.000000 loreme-0.1.2/README.md
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-06-09 16:52:50.572999 loreme-0.1.2/loreme.egg-info/
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     2882 2023-06-09 16:52:50.000000 loreme-0.1.2/loreme.egg-info/PKG-INFO
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      717 2023-06-09 16:52:50.000000 loreme-0.1.2/loreme.egg-info/SOURCES.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)        1 2023-06-09 16:52:50.000000 loreme-0.1.2/loreme.egg-info/dependency_links.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       46 2023-06-09 16:52:50.000000 loreme-0.1.2/loreme.egg-info/entry_points.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       77 2023-06-09 16:52:50.000000 loreme-0.1.2/loreme.egg-info/requires.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)        7 2023-06-09 16:52:50.000000 loreme-0.1.2/loreme.egg-info/top_level.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      918 2023-06-09 16:51:40.000000 loreme-0.1.2/pyproject.toml
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       38 2023-06-09 16:52:50.621205 loreme-0.1.2/setup.cfg
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-06-09 16:52:50.520907 loreme-0.1.2/src/
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-06-09 16:52:50.620009 loreme-0.1.2/src/loreme/
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     1512 2023-06-05 20:07:53.000000 loreme-0.1.2/src/loreme/__init__.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     2645 2023-06-05 04:30:20.000000 loreme-0.1.2/src/loreme/check_gpu_availability.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     3119 2023-06-08 08:55:56.000000 loreme-0.1.2/src/loreme/dorado.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     5227 2023-06-08 08:59:20.000000 loreme-0.1.2/src/loreme/download.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     3336 2023-06-08 09:00:46.000000 loreme-0.1.2/src/loreme/env.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     1496 2023-06-05 04:30:20.000000 loreme-0.1.2/src/loreme/export_bedgraph.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     3440 2023-06-05 04:30:20.000000 loreme-0.1.2/src/loreme/gene_body_methylation.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     1144 2023-06-05 04:30:20.000000 loreme-0.1.2/src/loreme/intersect.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)    33071 2023-06-09 16:49:10.000000 loreme-0.1.2/src/loreme/loreme.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     5191 2023-06-05 04:30:20.000000 loreme-0.1.2/src/loreme/mean.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     1690 2023-06-05 04:30:20.000000 loreme-0.1.2/src/loreme/merge.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      940 2023-06-05 04:30:20.000000 loreme-0.1.2/src/loreme/methylation_hist.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     3054 2023-06-05 04:30:20.000000 loreme-0.1.2/src/loreme/parse_gff.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     2610 2023-06-05 04:30:20.000000 loreme-0.1.2/src/loreme/pbcpg.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     6487 2023-06-05 04:30:20.000000 loreme-0.1.2/src/loreme/plot.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     2440 2023-06-05 04:30:20.000000 loreme-0.1.2/src/loreme/plot_bedtools.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     5087 2023-06-05 04:30:20.000000 loreme-0.1.2/src/loreme/plot_genes.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     4327 2023-06-05 04:30:20.000000 loreme-0.1.2/src/loreme/plot_repeats.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     3433 2023-06-05 04:30:20.000000 loreme-0.1.2/src/loreme/promoter_methylation.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       90 2023-06-09 16:51:24.000000 loreme-0.1.2/src/loreme/version.py
```

### Comparing `loreme-0.1.1/LICENSE` & `loreme-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `loreme-0.1.1/PKG-INFO` & `loreme-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loreme
-Version: 0.1.1
+Version: 0.1.2
 Summary: Extract Methylation calls from ONT or PB long read data
 Author-email: Anthony Aylward <aaylward@salk.edu>
 Project-URL: Homepage, https://gitlab.com/salk-tm/loreme
 Project-URL: Documentation, https://salk-tm.gitlab.io/loreme
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `loreme-0.1.1/README.md` & `loreme-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `loreme-0.1.1/loreme.egg-info/PKG-INFO` & `loreme-0.1.2/loreme.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loreme
-Version: 0.1.1
+Version: 0.1.2
 Summary: Extract Methylation calls from ONT or PB long read data
 Author-email: Anthony Aylward <aaylward@salk.edu>
 Project-URL: Homepage, https://gitlab.com/salk-tm/loreme
 Project-URL: Documentation, https://salk-tm.gitlab.io/loreme
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `loreme-0.1.1/loreme.egg-info/SOURCES.txt` & `loreme-0.1.2/loreme.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `loreme-0.1.1/pyproject.toml` & `loreme-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "loreme"
-version = "0.1.1" # Don't forget to match with version.py and docs/source/conf.py
+version = "0.1.2" # Don't forget to match with version.py and docs/source/conf.py
 authors = [
     { name="Anthony Aylward", email="aaylward@salk.edu" },
 ]
 description = "Extract Methylation calls from ONT or PB long read data"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `loreme-0.1.1/src/loreme/__init__.py` & `loreme-0.1.2/src/loreme/__init__.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.1/src/loreme/check_gpu_availability.py` & `loreme-0.1.2/src/loreme/check_gpu_availability.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.1/src/loreme/dorado.py` & `loreme-0.1.2/src/loreme/dorado.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import itertools
 import os
 import os.path
 import subprocess
 
-from loreme.env import DORADO_PATH, DORADO_MODEL_DIR, DORADO_PLATFORM
+from loreme.env import DORADO_PATH, DORADO_PATH_024, DORADO_MODEL_DIR, DORADO_PLATFORM
 
 def fast5_to_pod5(*input_fast5, output_pod5: str, threads: int = 1):
     """Convert FAST5 files to POD5 files
 
     Parameters
     ----------
     *input_fast5
@@ -57,15 +57,15 @@
         raise RuntimeError('Invalid modified bases choice. Choose 5mCG_5hmCG, 5mC, 6mA.')
     if speed == 260 and frequency != '4kHz':
         raise RuntimeError('260bps speed only available at 4kHz frequency')
     if frequency == '4kHz' and modified_bases != '5mCG_5hmCG':
         raise RuntimeError('the only modified base model at 4kHz frequency is 5mCG_5hmCG')
     model = f"dna_r10.4.1_e8.2_{speed}bps_{accuracy}@v4.{1+(frequency=='5kHz')}.0"
     with open(output, 'wb') as f:
-        subprocess.run((DORADO_PATH[DORADO_PLATFORM], 'basecaller',
+        subprocess.run((DORADO_PATH_024[DORADO_PLATFORM], 'basecaller',
                         os.path.join(DORADO_MODEL_DIR, model), input_dir,
                         '--modified-bases', modified_bases)
                         + bool(reference) * ('--reference', reference),
                        stdout=f)
 
 
 def dorado_align(index: str, reads: str, output: str):
```

### Comparing `loreme-0.1.1/src/loreme/download.py` & `loreme-0.1.2/src/loreme/download.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import os.path
 import ftplib
 import gzip
 import tarfile
 import subprocess
 from itertools import product
 from loreme.env import (PBCPG_URL, PBCPG_DIR, EXAMPLE_DATA_URLS, EXAMPLE_DATA_DIR, HG38_FTP,
-                       HG38_GENOME_PATH, HG38_ANNOT_PATH, DORADO_DIR, DORADO_URL,
-                       DORADO_MODEL_DIR, DORADO_PATH)
+                       HG38_GENOME_PATH, HG38_ANNOT_PATH, DORADO_DIR, DORADO_URL, DORADO_URL_024,
+                       DORADO_MODEL_DIR, DORADO_PATH_024)
 
 def download_pbcpg(directory: str = PBCPG_DIR):
     """Download pb-CpG-tools
 
     Parameters
     ----------
     directory : str
@@ -86,29 +86,34 @@
     model_dir : str
         destination directory for dorado models
     """
 
     if pfm not in {'linux-x64', 'linux-arm64', 'osx-arm64', 'win64'}:
         raise RuntimeError('invalid platform choice')
     dest_tarfile = os.path.join(directory, f'dorado-0.3.0-{pfm}.tar.gz')
+    dest_tarfile_024 = os.path.join(directory, f'dorado-0.2.4-{pfm}.tar.gz')
     print(f'downloading to {dest_tarfile}')
     if os.path.exists(dest_tarfile):
         raise RuntimeError(f'a file already exists at {dest_tarfile}')
     http = urllib3.PoolManager()
     with http.request('GET', DORADO_URL[pfm], preload_content=False) as r, open(dest_tarfile, 'wb') as f:
         shutil.copyfileobj(r, f)
     with tarfile.open(dest_tarfile) as tar:
         tar.extractall(path=directory)
+    with http.request('GET', DORADO_URL_024[pfm], preload_content=False) as r, open(dest_tarfile_024, 'wb') as f:
+        shutil.copyfileobj(r, f)
+    with tarfile.open(dest_tarfile_024) as tar:
+        tar.extractall(path=directory)
     print(f'downloading models to {model_dir}')
     for speed, accuracy, in product((260, 400), ('fast', 'hac', 'sup')):
-        subprocess.run((DORADO_PATH[pfm], 'download', '--directory', model_dir,
+        subprocess.run((DORADO_PATH_024[pfm], 'download', '--directory', model_dir,
             '--model', f'dna_r10.4.1_e8.2_{speed}bps_{accuracy}@v4.1.0'))
-        subprocess.run((DORADO_PATH[pfm], 'download', '--directory', model_dir,
+        subprocess.run((DORADO_PATH_024[pfm], 'download', '--directory', model_dir,
             '--model', f'dna_r10.4.1_e8.2_{speed}bps_{accuracy}@v4.1.0_5mCG_5hmCG@v2'))
-    for accuracy in 'fast', 'hac', 'sup':
-        subprocess.run((DORADO_PATH[pfm], 'download', '--directory', model_dir,
-            '--model', f'dna_r10.4.1_e8.2_400bps_{accuracy}@v4.2.0'))
-        subprocess.run((DORADO_PATH[pfm], 'download', '--directory', model_dir,
-            '--model', f'dna_r10.4.1_e8.2_400bps_{accuracy}@v4.2.0_5mCG_5hmCG@v2'))
-    for modified_bases in '5mC', '6mA':
-        subprocess.run((DORADO_PATH[pfm], 'download', '--directory', model_dir,
-            '--model', f'dna_r10.4.1_e8.2_400bps_sup@v4.2.0_{modified_bases}@v2'))
+    # for accuracy in 'fast', 'hac', 'sup':
+    #     subprocess.run((DORADO_PATH[pfm], 'download', '--directory', model_dir,
+    #         '--model', f'dna_r10.4.1_e8.2_400bps_{accuracy}@v4.2.0'))
+    #     subprocess.run((DORADO_PATH[pfm], 'download', '--directory', model_dir,
+    #         '--model', f'dna_r10.4.1_e8.2_400bps_{accuracy}@v4.2.0_5mCG_5hmCG@v2'))
+    # for modified_bases in '5mC', '6mA':
+    #     subprocess.run((DORADO_PATH[pfm], 'download', '--directory', model_dir,
+    #         '--model', f'dna_r10.4.1_e8.2_400bps_sup@v4.2.0_{modified_bases}@v2'))
```

### Comparing `loreme-0.1.1/src/loreme/env.py` & `loreme-0.1.2/src/loreme/env.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import os.path
 
-PBCPG_DIR = os.environ.get('LR5MC_PBCPG_DIR',
+PBCPG_DIR = os.environ.get('LOREME_PBCPG_DIR',
     os.path.join(os.path.dirname(__file__)))
 PBCPG_PATH = os.path.join(PBCPG_DIR, 'pb-CpG-tools-v2.3.1-x86_64-unknown-linux-gnu',
                          'bin', 'aligned_bam_to_cpg_scores')
 PBCPG_MODEL = os.path.join(PBCPG_DIR, 'pb-CpG-tools-v2.3.1-x86_64-unknown-linux-gnu',
                                'models', 'pileup_calling_model.v1.tflite')
 PBCPG_URL = 'https://github.com/PacificBiosciences/pb-CpG-tools/releases/download/v2.3.1/pb-CpG-tools-v2.3.1-x86_64-unknown-linux-gnu.tar.gz'
 EXAMPLE_DATA_URLS = (
@@ -13,26 +13,38 @@
     'https://downloads.pacbcloud.com/public/dataset/HG002-CpG-methylation-202202/m64011_190901_095311.hifi_reads.bam',
     'https://downloads.pacbcloud.com/public/dataset/HG002-CpG-methylation-202202/m64012_190920_173625.hifi_reads.bam',
     'https://downloads.pacbcloud.com/public/dataset/HG002-CpG-methylation-202202/m64012_190921_234837.hifi_reads.bam',
 )
 HG38_FTP = 'ftp.ncbi.nlm.nih.gov'
 HG38_GENOME_PATH = 'genomes/all/GCA/000/001/405/GCA_000001405.15_GRCh38/seqs_for_alignment_pipelines.ucsc_ids/GCA_000001405.15_GRCh38_no_alt_analysis_set.fna.gz'
 HG38_ANNOT_PATH = 'genomes/all/GCA/000/001/405/GCA_000001405.15_GRCh38/seqs_for_alignment_pipelines.ucsc_ids/GCA_000001405.15_GRCh38_full_analysis_set.refseq_annotation.gff.gz'
-EXAMPLE_DATA_DIR = os.environ.get('LR5MC_EXAMPLE_DATA_DIR', os.path.dirname(__file__))
+EXAMPLE_DATA_DIR = os.environ.get('LOREME_EXAMPLE_DATA_DIR', os.path.dirname(__file__))
 
-DORADO_DIR = os.environ.get('LR5MC_DORADO_DIR',
+DORADO_DIR = os.environ.get('LOREME_DORADO_DIR',
     os.path.join(os.path.dirname(__file__)))
-DORADO_PLATFORM = os.environ.get('LR5MC_DORADO_PLATFORM')
+DORADO_PLATFORM = os.environ.get('LOREME_DORADO_PLATFORM')
 DORADO_PATH = {
     'linux-x64': os.path.join(DORADO_DIR, 'dorado-0.3.0-linux-x64', 'bin', 'dorado'),
     'linux-arm64': os.path.join(DORADO_DIR, 'dorado-0.3.0-linux-arm64', 'bin', 'dorado'),
     'osx-arm64': os.path.join(DORADO_DIR, 'dorado-0.3.0-osx-arm64', 'bin', 'dorado'),
     'win64': os.path.join(DORADO_DIR, 'dorado-0.3.0-win64', 'bin', 'dorado')
 }
+DORADO_PATH_024 = {
+    'linux-x64': os.path.join(DORADO_DIR, 'dorado-0.2.4-linux-x64', 'bin', 'dorado'),
+    'linux-arm64': os.path.join(DORADO_DIR, 'dorado-0.2.4-linux-arm64', 'bin', 'dorado'),
+    'osx-arm64': os.path.join(DORADO_DIR, 'dorado-0.2.4-osx-arm64', 'bin', 'dorado'),
+    'win64': os.path.join(DORADO_DIR, 'dorado-0.2.4-win64', 'bin', 'dorado')
+}
 DORADO_URL = {
     'linux-x64': 'https://cdn.oxfordnanoportal.com/software/analysis/dorado-0.3.0-linux-x64.tar.gz',
     'linux-arm64': 'https://cdn.oxfordnanoportal.com/software/analysis/dorado-0.3.0-linux-arm64.tar.gz',
     'osx-arm64': 'https://cdn.oxfordnanoportal.com/software/analysis/dorado-0.3.0-osx-arm64.tar.gz',
     'win64': 'https://cdn.oxfordnanoportal.com/software/analysis/dorado-0.3.0-win64.zip'
 }
-DORADO_MODEL_DIR = os.environ.get('LR5MC_DORADO_MODEL_DIR',
+DORADO_URL_024 = {
+    'linux-x64': 'https://cdn.oxfordnanoportal.com/software/analysis/dorado-0.2.4-linux-x64.tar.gz',
+    'linux-arm64': 'https://cdn.oxfordnanoportal.com/software/analysis/dorado-0.2.4-linux-arm64.tar.gz',
+    'osx-arm64': 'https://cdn.oxfordnanoportal.com/software/analysis/dorado-0.2.4-osx-arm64.tar.gz',
+    'win64': 'https://cdn.oxfordnanoportal.com/software/analysis/dorado-0.2.4-win64.zip'
+}
+DORADO_MODEL_DIR = os.environ.get('LOREME_DORADO_MODEL_DIR',
     os.path.join(os.path.dirname(__file__)))
```

### Comparing `loreme-0.1.1/src/loreme/export_bedgraph.py` & `loreme-0.1.2/src/loreme/export_bedgraph.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.1/src/loreme/gene_body_methylation.py` & `loreme-0.1.2/src/loreme/gene_body_methylation.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.1/src/loreme/intersect.py` & `loreme-0.1.2/src/loreme/intersect.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.1/src/loreme/loreme.py` & `loreme-0.1.2/src/loreme/loreme.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,33 +139,30 @@
 def _dorado_check_gpu(args):
     if check_gpu_availability(args.devices, gpu_load=args.gpu_load,
                            gpu_mem=args.gpu_mem):
         print('GPU is available')
 
 
 def _dorado_align(args):
-    dorado_align(args.index, args.reference, args.output)
+    dorado_align(args.index, args.reads, args.output)
 
 
 def run_dorado(args):
     check_gpu_availability([0])
     if args.convert:
         pod5_dir = f'{args.output[:-4]}_pod5'
         pod5_base = f'{os.path.basename(args.output)[:-4]}.pod5'
         os.mkdir(pod5_dir)
         fast5_to_pod5(*args.reads,
                       output_pod5=os.path.join(pod5_dir, pod5_base),
                       threads=args.threads)
-        dorado(pod5_dir, args.output, speed=args.speed, accuracy=args.accuracy,
-               frequency=args.frequency, modified_bases=args.modified_bases,
-               reference=args.reference)
+        dorado(pod5_dir, args.output, speed=args.speed, accuracy=args.accuracy)
     elif len(args.reads) == 1 and os.path.isdir(args.reads[0]):
         dorado(args.reads[0], args.output, speed=args.speed,
-               accuracy=args.accuracy, frequency=args.frequency,
-               modified_bases=args.modified_bases, reference=args.reference)
+               accuracy=args.accuracy)
     else:
         raise RuntimeError('For running without --convert, supply only one input FAST5 or POD5 directory')
 
 
 
 def _calculate_mean(args):
     if args.total:
@@ -373,30 +370,30 @@
                         help="Number of threads for parallel processing. (default: %(default)d)")
     
     parser_dorado = subparsers.add_parser('dorado',
         help='run full dorado pipeline')
     parser_dorado.set_defaults(func=run_dorado)
     parser_dorado.add_argument('reads', metavar='<reads>', nargs='+',
                                help='input FAST5 files, or single directory containing FAST5 or POD5 files')
-    parser_dorado.add_argument('output', metavar='<output.bam>',
-                               help='path to output BAM file')
+    parser_dorado.add_argument('output', metavar='<output.sam>',
+                               help='path to output SAM file')
     parser_dorado.add_argument('--convert', action='store_true',
                                help='convert FAST5 to POD5 before basecalling')
     parser_dorado.add_argument('--speed', type=int, choices=(260, 400),
                                default=400, help='pore speed (default: 400)')
     parser_dorado.add_argument('--accuracy', choices=('fast', 'hac', 'sup'),
                                default='fast', help='model accuracy (default: fast)')
-    parser_dorado.add_argument('--frequency', choices=('4kHz', '5kHz'),
-                               default='4kHz', help='(default: 4kHz)')
-    parser_dorado.add_argument('--modified-bases',
-                               choices=('5mCG_5hmCG', '5mC', '6mA'),
-                               default='5mCG_5hmCG',
-                               help='Modified base model (default: 5mCG_5hmCG)')
-    parser_dorado.add_argument('--reference', metavar='<index>',
-                               help='map to a reference index (fastq/fasta/mmi)')
+    # parser_dorado.add_argument('--frequency', choices=('4kHz', '5kHz'),
+    #                            default='4kHz', help='(default: 4kHz)')
+    # parser_dorado.add_argument('--modified-bases',
+    #                            choices=('5mCG_5hmCG', '5mC', '6mA'),
+    #                            default='5mCG_5hmCG',
+    #                            help='Modified base model (default: 5mCG_5hmCG)')
+    # parser_dorado.add_argument('--reference', metavar='<index>',
+    #                            help='map to a reference index (fastq/fasta/mmi)')
     parser_dorado.add_argument("-t", "--threads", metavar="<int>",
         type=int, default=1,
         help="Number of cpu threads. (default: %(default)d)")
     
     parser_dorado_check = subparsers.add_parser('dorado-check',
         help='check GPU availability')
     parser_dorado_check.set_defaults(func=_dorado_check_gpu)
@@ -423,14 +420,16 @@
     parser_dorado_align = subparsers.add_parser('dorado-align',
         help='align dorado basecalls')
     parser_dorado_align.set_defaults(func=_dorado_align)
     parser_dorado_align.add_argument('index', metavar='<index>',
                                      help='reference index for alignment')
     parser_dorado_align.add_argument('reads', metavar='<reads>',
                                      help='reads for alignment')
+    parser_dorado_align.add_argument('output', metavar='<output.bam>',
+                                     help='path to output BAM file')
 
     parser_mean = subparsers.add_parser('mean',
         help='calculate average methylation across chromosomes or in total')
     parser_mean.set_defaults(func=_calculate_mean)
     parser_mean.add_argument('bedmethyl', metavar='<bedmethyl.bed>',
         nargs='+', help='bedMethyl file containing methylation data')
     parser_mean.add_argument('--plot', metavar='<output.{pdf,png,svg}>',
```

### Comparing `loreme-0.1.1/src/loreme/mean.py` & `loreme-0.1.2/src/loreme/mean.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.1/src/loreme/merge.py` & `loreme-0.1.2/src/loreme/merge.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.1/src/loreme/methylation_hist.py` & `loreme-0.1.2/src/loreme/methylation_hist.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.1/src/loreme/parse_gff.py` & `loreme-0.1.2/src/loreme/parse_gff.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.1/src/loreme/pbcpg.py` & `loreme-0.1.2/src/loreme/pbcpg.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.1/src/loreme/plot.py` & `loreme-0.1.2/src/loreme/plot.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.1/src/loreme/plot_bedtools.py` & `loreme-0.1.2/src/loreme/plot_bedtools.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.1/src/loreme/plot_genes.py` & `loreme-0.1.2/src/loreme/plot_genes.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.1/src/loreme/plot_repeats.py` & `loreme-0.1.2/src/loreme/plot_repeats.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.1/src/loreme/promoter_methylation.py` & `loreme-0.1.2/src/loreme/promoter_methylation.py`

 * *Files identical despite different names*

