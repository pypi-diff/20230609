# Comparing `tmp/microcat-0.1.3.tar.gz` & `tmp/microcat-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microcat-0.1.3.tar", last modified: Fri Jun  9 04:24:17 2023, max compression
+gzip compressed data, was "microcat-0.1.4.tar", last modified: Fri Jun  9 04:34:07 2023, max compression
```

## Comparing `microcat-0.1.3.tar` & `microcat-0.1.4.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 04:24:17.121655 microcat-0.1.3/
--rw-r--r--   0 root         (0) root         (0)    34599 2023-06-09 02:02:59.000000 microcat-0.1.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)      396 2023-06-09 03:45:47.000000 microcat-0.1.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1298 2023-06-09 04:24:17.121655 microcat-0.1.3/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      383 2023-05-18 11:49:26.000000 microcat-0.1.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 04:24:17.117655 microcat-0.1.3/microcat/
--rwxrwxr-x   0 root         (0) root         (0)       73 2023-06-09 04:24:03.000000 microcat-0.1.3/microcat/__about__.py
--rwxrwxr-x   0 root         (0) root         (0)      911 2023-06-09 03:13:23.000000 microcat-0.1.3/microcat/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 04:24:17.117655 microcat-0.1.3/microcat/config/
--rw-r--r--   0 root         (0) root         (0)     2655 2023-06-08 02:42:59.000000 microcat-0.1.3/microcat/config/config.yaml
--rwxr-xr-x   0 root         (0) root         (0)     8766 2023-06-09 03:49:23.000000 microcat-0.1.3/microcat/configer.py
--rwxr-xr-x   0 root         (0) root         (0)    18601 2023-06-09 03:49:05.000000 microcat-0.1.3/microcat/corer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 04:24:17.117655 microcat-0.1.3/microcat/envs/
--rw-r--r--   0 root         (0) root         (0)      184 2023-06-08 03:16:48.000000 microcat-0.1.3/microcat/envs/kmer_python.yaml
--rw-r--r--   0 root         (0) root         (0)      404 2023-06-07 06:44:30.000000 microcat-0.1.3/microcat/envs/kmer_qc.yaml
--rw-rw-r--   0 root         (0) root         (0)      164 2023-06-07 06:46:24.000000 microcat-0.1.3/microcat/envs/kraken2.yaml
--rw-r--r--   0 root         (0) root         (0)      133 2023-05-31 02:41:36.000000 microcat-0.1.3/microcat/envs/krakenuniq.yaml
--rw-r--r--   0 root         (0) root         (0)      109 2023-06-03 12:24:08.000000 microcat-0.1.3/microcat/envs/metaphlan.yaml
--rwxr-xr-x   0 root         (0) root         (0)      145 2023-06-03 12:24:08.000000 microcat-0.1.3/microcat/envs/pathseq.yaml
--rw-r--r--   0 root         (0) root         (0)      100 2023-06-07 06:24:12.000000 microcat-0.1.3/microcat/envs/star.yaml
--rw-r--r--   0 root         (0) root         (0)      140 2023-05-31 02:41:36.000000 microcat-0.1.3/microcat/envs/trimming.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 04:24:17.113655 microcat-0.1.3/microcat/profiles/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 04:24:17.117655 microcat-0.1.3/microcat/profiles/lsf/
--rw-r--r--   0 root         (0) root         (0)      957 2023-06-03 12:24:08.000000 microcat-0.1.3/microcat/profiles/lsf/CookieCutter.py
--rw-r--r--   0 root         (0) root         (0)     2242 2023-06-03 12:24:08.000000 microcat-0.1.3/microcat/profiles/lsf/OSLayer.py
--rw-r--r--   0 root         (0) root         (0)      297 2023-06-03 12:24:08.000000 microcat-0.1.3/microcat/profiles/lsf/config.yaml
--rwxr-xr-x   0 root         (0) root         (0)     1124 2023-06-03 12:24:08.000000 microcat-0.1.3/microcat/profiles/lsf/lsf_cancel.py
--rw-r--r--   0 root         (0) root         (0)     1978 2023-06-03 12:24:08.000000 microcat-0.1.3/microcat/profiles/lsf/lsf_config.py
--rwxr-xr-x   0 root         (0) root         (0)       48 2023-06-03 12:24:08.000000 microcat-0.1.3/microcat/profiles/lsf/lsf_jobscript.sh
--rwxr-xr-x   0 root         (0) root         (0)     7511 2023-06-03 12:24:08.000000 microcat-0.1.3/microcat/profiles/lsf/lsf_status.py
--rwxr-xr-x   0 root         (0) root         (0)     8281 2023-06-03 12:24:08.000000 microcat-0.1.3/microcat/profiles/lsf/lsf_submit.py
--rw-r--r--   0 root         (0) root         (0)     3775 2023-06-03 12:24:08.000000 microcat-0.1.3/microcat/profiles/lsf/memory_units.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 04:24:17.117655 microcat-0.1.3/microcat/rules/
--rw-r--r--   0 root         (0) root         (0)     1107 2023-06-09 02:29:19.000000 microcat-0.1.3/microcat/rules/ERCC.smk
--rw-r--r--   0 root         (0) root         (0)    40814 2023-06-09 02:28:56.000000 microcat-0.1.3/microcat/rules/classfier.smk
--rw-r--r--   0 root         (0) root         (0)     3981 2023-06-07 01:22:00.000000 microcat-0.1.3/microcat/rules/database.smk
--rw-r--r--   0 root         (0) root         (0)    42201 2023-06-09 02:29:15.000000 microcat-0.1.3/microcat/rules/host.smk
--rwxr-xr-x   0 root         (0) root         (0)    10460 2023-06-05 09:08:14.000000 microcat-0.1.3/microcat/sample.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 04:24:17.121655 microcat-0.1.3/microcat/scripts/
--rw-r--r--   0 root         (0) root         (0)    15479 2023-06-08 03:30:56.000000 microcat-0.1.3/microcat/scripts/INVADEseq.py
--rwxrwxrwx   0 root         (0) root         (0)    19072 2023-06-07 07:14:07.000000 microcat-0.1.3/microcat/scripts/extract_kraken_reads.py
--rwxrwxrwx   0 root         (0) root         (0)     3849 2023-06-07 07:14:23.000000 microcat-0.1.3/microcat/scripts/extract_microbiome_output.R
--rwxr-xr-x   0 root         (0) root         (0)     7896 2023-06-03 12:24:08.000000 microcat-0.1.3/microcat/scripts/get_ncbi_domains.py
--rw-r--r--   0 root         (0) root         (0)     1185 2023-06-07 07:15:11.000000 microcat-0.1.3/microcat/scripts/krak2_output_denosing.R
--rwxr-xr-x   0 root         (0) root         (0)     6942 2023-06-07 07:15:43.000000 microcat-0.1.3/microcat/scripts/kraken2mpa.py
--rwxr-xr-x   0 root         (0) root         (0)    14784 2023-06-07 07:15:24.000000 microcat-0.1.3/microcat/scripts/kraken2sc.py
--rw-r--r--   0 root         (0) root         (0)     4698 2023-06-07 07:14:59.000000 microcat-0.1.3/microcat/scripts/sample_denosing.R
--rwxrwxrwx   0 root         (0) root         (0)    15665 2023-06-07 07:13:48.000000 microcat-0.1.3/microcat/scripts/sckmer_unpaired.R
--rwxr-xr-x   0 root         (0) root         (0)     2367 2023-06-03 12:24:08.000000 microcat-0.1.3/microcat/scripts/spilt_bam_by_tag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 04:24:17.121655 microcat-0.1.3/microcat/snakefiles/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 11:37:58.000000 microcat-0.1.3/microcat/snakefiles/bulk_wf.smk
--rw-r--r--   0 root         (0) root         (0)     1830 2023-06-09 02:28:49.000000 microcat-0.1.3/microcat/snakefiles/scRNA_wf.smk
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 11:38:06.000000 microcat-0.1.3/microcat/snakefiles/spatial_wf.smk
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 04:24:17.117655 microcat-0.1.3/microcat.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1298 2023-06-09 04:24:17.000000 microcat-0.1.3/microcat.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1494 2023-06-09 04:24:17.000000 microcat-0.1.3/microcat.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 04:24:17.000000 microcat-0.1.3/microcat.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-06-09 04:24:17.000000 microcat-0.1.3/microcat.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       65 2023-06-09 04:24:17.000000 microcat-0.1.3/microcat.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-06-09 04:24:17.000000 microcat-0.1.3/microcat.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       67 2023-06-09 01:50:10.000000 microcat-0.1.3/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-09 04:24:17.121655 microcat-0.1.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2273 2023-06-09 03:43:47.000000 microcat-0.1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 04:34:07.952008 microcat-0.1.4/
+-rw-r--r--   0 root         (0) root         (0)    34599 2023-06-09 02:02:59.000000 microcat-0.1.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      396 2023-06-09 03:45:47.000000 microcat-0.1.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1298 2023-06-09 04:34:07.952008 microcat-0.1.4/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      383 2023-05-18 11:49:26.000000 microcat-0.1.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 04:34:07.948008 microcat-0.1.4/microcat/
+-rwxrwxr-x   0 root         (0) root         (0)       73 2023-06-09 04:34:03.000000 microcat-0.1.4/microcat/__about__.py
+-rwxrwxr-x   0 root         (0) root         (0)      911 2023-06-09 03:13:23.000000 microcat-0.1.4/microcat/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 04:34:07.948008 microcat-0.1.4/microcat/config/
+-rw-r--r--   0 root         (0) root         (0)     2655 2023-06-08 02:42:59.000000 microcat-0.1.4/microcat/config/config.yaml
+-rwxr-xr-x   0 root         (0) root         (0)     8766 2023-06-09 03:49:23.000000 microcat-0.1.4/microcat/configer.py
+-rwxr-xr-x   0 root         (0) root         (0)    18601 2023-06-09 04:29:52.000000 microcat-0.1.4/microcat/corer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 04:34:07.948008 microcat-0.1.4/microcat/envs/
+-rw-r--r--   0 root         (0) root         (0)      184 2023-06-08 03:16:48.000000 microcat-0.1.4/microcat/envs/kmer_python.yaml
+-rw-r--r--   0 root         (0) root         (0)      404 2023-06-07 06:44:30.000000 microcat-0.1.4/microcat/envs/kmer_qc.yaml
+-rw-rw-r--   0 root         (0) root         (0)      164 2023-06-07 06:46:24.000000 microcat-0.1.4/microcat/envs/kraken2.yaml
+-rw-r--r--   0 root         (0) root         (0)      133 2023-05-31 02:41:36.000000 microcat-0.1.4/microcat/envs/krakenuniq.yaml
+-rw-r--r--   0 root         (0) root         (0)      109 2023-06-03 12:24:08.000000 microcat-0.1.4/microcat/envs/metaphlan.yaml
+-rwxr-xr-x   0 root         (0) root         (0)      145 2023-06-03 12:24:08.000000 microcat-0.1.4/microcat/envs/pathseq.yaml
+-rw-r--r--   0 root         (0) root         (0)      100 2023-06-07 06:24:12.000000 microcat-0.1.4/microcat/envs/star.yaml
+-rw-r--r--   0 root         (0) root         (0)      140 2023-05-31 02:41:36.000000 microcat-0.1.4/microcat/envs/trimming.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 04:34:07.944008 microcat-0.1.4/microcat/profiles/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 04:34:07.952008 microcat-0.1.4/microcat/profiles/lsf/
+-rw-r--r--   0 root         (0) root         (0)      957 2023-06-03 12:24:08.000000 microcat-0.1.4/microcat/profiles/lsf/CookieCutter.py
+-rw-r--r--   0 root         (0) root         (0)     2242 2023-06-03 12:24:08.000000 microcat-0.1.4/microcat/profiles/lsf/OSLayer.py
+-rw-r--r--   0 root         (0) root         (0)      297 2023-06-03 12:24:08.000000 microcat-0.1.4/microcat/profiles/lsf/config.yaml
+-rwxr-xr-x   0 root         (0) root         (0)     1124 2023-06-03 12:24:08.000000 microcat-0.1.4/microcat/profiles/lsf/lsf_cancel.py
+-rw-r--r--   0 root         (0) root         (0)     1978 2023-06-03 12:24:08.000000 microcat-0.1.4/microcat/profiles/lsf/lsf_config.py
+-rwxr-xr-x   0 root         (0) root         (0)       48 2023-06-03 12:24:08.000000 microcat-0.1.4/microcat/profiles/lsf/lsf_jobscript.sh
+-rwxr-xr-x   0 root         (0) root         (0)     7511 2023-06-03 12:24:08.000000 microcat-0.1.4/microcat/profiles/lsf/lsf_status.py
+-rwxr-xr-x   0 root         (0) root         (0)     8281 2023-06-03 12:24:08.000000 microcat-0.1.4/microcat/profiles/lsf/lsf_submit.py
+-rw-r--r--   0 root         (0) root         (0)     3775 2023-06-03 12:24:08.000000 microcat-0.1.4/microcat/profiles/lsf/memory_units.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 04:34:07.952008 microcat-0.1.4/microcat/rules/
+-rw-r--r--   0 root         (0) root         (0)     1107 2023-06-09 02:29:19.000000 microcat-0.1.4/microcat/rules/ERCC.smk
+-rw-r--r--   0 root         (0) root         (0)    40814 2023-06-09 02:28:56.000000 microcat-0.1.4/microcat/rules/classfier.smk
+-rw-r--r--   0 root         (0) root         (0)     3981 2023-06-07 01:22:00.000000 microcat-0.1.4/microcat/rules/database.smk
+-rw-r--r--   0 root         (0) root         (0)    42225 2023-06-09 04:28:20.000000 microcat-0.1.4/microcat/rules/host.smk
+-rwxr-xr-x   0 root         (0) root         (0)    10460 2023-06-05 09:08:14.000000 microcat-0.1.4/microcat/sample.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 04:34:07.952008 microcat-0.1.4/microcat/scripts/
+-rw-r--r--   0 root         (0) root         (0)    15479 2023-06-08 03:30:56.000000 microcat-0.1.4/microcat/scripts/INVADEseq.py
+-rwxrwxrwx   0 root         (0) root         (0)    19072 2023-06-07 07:14:07.000000 microcat-0.1.4/microcat/scripts/extract_kraken_reads.py
+-rwxrwxrwx   0 root         (0) root         (0)     3849 2023-06-07 07:14:23.000000 microcat-0.1.4/microcat/scripts/extract_microbiome_output.R
+-rwxr-xr-x   0 root         (0) root         (0)     7896 2023-06-03 12:24:08.000000 microcat-0.1.4/microcat/scripts/get_ncbi_domains.py
+-rw-r--r--   0 root         (0) root         (0)     1185 2023-06-07 07:15:11.000000 microcat-0.1.4/microcat/scripts/krak2_output_denosing.R
+-rwxr-xr-x   0 root         (0) root         (0)     6942 2023-06-07 07:15:43.000000 microcat-0.1.4/microcat/scripts/kraken2mpa.py
+-rwxr-xr-x   0 root         (0) root         (0)    14784 2023-06-07 07:15:24.000000 microcat-0.1.4/microcat/scripts/kraken2sc.py
+-rw-r--r--   0 root         (0) root         (0)     4698 2023-06-07 07:14:59.000000 microcat-0.1.4/microcat/scripts/sample_denosing.R
+-rwxrwxrwx   0 root         (0) root         (0)    15665 2023-06-07 07:13:48.000000 microcat-0.1.4/microcat/scripts/sckmer_unpaired.R
+-rwxr-xr-x   0 root         (0) root         (0)     2367 2023-06-03 12:24:08.000000 microcat-0.1.4/microcat/scripts/spilt_bam_by_tag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 04:34:07.952008 microcat-0.1.4/microcat/snakefiles/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 11:37:58.000000 microcat-0.1.4/microcat/snakefiles/bulk_wf.smk
+-rw-r--r--   0 root         (0) root         (0)     1832 2023-06-09 04:28:17.000000 microcat-0.1.4/microcat/snakefiles/scRNA_wf.smk
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 11:38:06.000000 microcat-0.1.4/microcat/snakefiles/spatial_wf.smk
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 04:34:07.948008 microcat-0.1.4/microcat.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1298 2023-06-09 04:34:07.000000 microcat-0.1.4/microcat.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1494 2023-06-09 04:34:07.000000 microcat-0.1.4/microcat.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 04:34:07.000000 microcat-0.1.4/microcat.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-06-09 04:34:07.000000 microcat-0.1.4/microcat.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2023-06-09 04:34:07.000000 microcat-0.1.4/microcat.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-06-09 04:34:07.000000 microcat-0.1.4/microcat.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       67 2023-06-09 01:50:10.000000 microcat-0.1.4/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-09 04:34:07.952008 microcat-0.1.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2273 2023-06-09 03:43:47.000000 microcat-0.1.4/setup.py
```

### Comparing `microcat-0.1.3/LICENSE` & `microcat-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `microcat-0.1.3/PKG-INFO` & `microcat-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microcat
-Version: 0.1.3
+Version: 0.1.4
 Summary: a computational toolbox to identificated microbiome from Omics
 Home-page: https://github.com/ChangxingSu/MicroCAT
 Author: Changxing Su
 Author-email: changxingsu42@gmail.com
 License: GPLv3+
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `microcat-0.1.3/microcat/__init__.py` & `microcat-0.1.4/microcat/__init__.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.3/microcat/config/config.yaml` & `microcat-0.1.4/microcat/config/config.yaml`

 * *Files identical despite different names*

### Comparing `microcat-0.1.3/microcat/configer.py` & `microcat-0.1.4/microcat/configer.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.3/microcat/corer.py` & `microcat-0.1.4/microcat/corer.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 
 
 def init(args, unknown):
 
     # Check if the user provided a working directory
     if args.workdir:
         # Create a MicrocatConfig object using the provided working directory
-        project = configer.MicrocatConfig(args.workdir)
+        project = microcat.MicrocatConfig(args.workdir)
 
 
         # Check if the working directory already exists
         if os.path.exists(args.workdir):
             print(f"Warning: The working directory '{args.workdir}' already exists.")
             proceed = input("Do you want to proceed? (y/n): ").lower()
             if proceed != 'y':
@@ -101,15 +101,15 @@
         if args.samples:
             conf["params"]["samples"] = args.samples
         else:
             print("Please supply samples table")
             sys.exit(-1)
 
         # Update the configuration file
-        configer.update_config(
+        microcat.update_config(
             project.config_file, project.new_config_file, conf, remove=False
         )
 
     else:
         # If the user didn't provide a working directory, print an error message and exit
         print("Please supply a workdir!")
         sys.exit(-1)
@@ -119,15 +119,15 @@
     """
     Use subprocess.Popen to run the MicroCAT workflow.
 
     Args:
         args (argparse.Namespace): An object containing parsed command-line arguments.
     """
     # Parse the YAML configuration file
-    conf = configer.parse_yaml(args.config)
+    conf = microcat.parse_yaml(args.config)
 
     # Check if the sample list is provided, exit if not
     if not os.path.exists(conf["params"]["samples"]):
         print("Please specific samples list on init step or change config.yaml manualy")
         sys.exit(1)
 
     # Prepare the command list for running Snakemake
@@ -418,15 +418,15 @@
     )
     ###############################################################
     # Create a sub-parser object
     subparsers = parser.add_subparsers(title="available subcommands", metavar="")
     ##  
     parser_init = subparsers.add_parser(
         "init",
-        formatter_class=configer.custom_help_formatter,
+        formatter_class=microcat.custom_help_formatter,
         parents=[common_parser],# add common parser
         prog="microcat init",
         help="init project",
     )
     parser_init.add_argument(
             "-s",
             "--samples",
@@ -481,15 +481,15 @@
 
     parser_init.set_defaults(func=init)
     
 
 
     parser_bulk_wf = subparsers.add_parser(
             "bulk_wf",
-            formatter_class=configer.custom_help_formatter,
+            formatter_class=microcat.custom_help_formatter,
             parents=[common_parser, run_parser],
             prog="smart bulk_wf",
             help="bulk rna seq microbiome mining pipeline",
         )
     # parser_bulk_wf.add_argument(
     #     "task",
     #     metavar="TASK",
@@ -499,15 +499,15 @@
     #     choices=[WORKFLOWS_MAG],
     #     help="pipeline end point. Allowed values are " + ", ".join(WORKFLOWS_MAG),
     # )
     parser_bulk_wf.set_defaults(func=bulk_wf)
 
     parser_scrna_wf = subparsers.add_parser(
             "scrna_wf",
-            formatter_class=configer.custom_help_formatter,
+            formatter_class=microcat.custom_help_formatter,
             parents=[common_parser, run_parser],
             prog="smart scrna_wf",
             help="single cell rna seq microbiome mining pipeline",
         )
 
     parser_scrna_wf.add_argument(
             "--platform",
```

### Comparing `microcat-0.1.3/microcat/profiles/lsf/CookieCutter.py` & `microcat-0.1.4/microcat/profiles/lsf/CookieCutter.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.3/microcat/profiles/lsf/OSLayer.py` & `microcat-0.1.4/microcat/profiles/lsf/OSLayer.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.3/microcat/profiles/lsf/lsf_cancel.py` & `microcat-0.1.4/microcat/profiles/lsf/lsf_cancel.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.3/microcat/profiles/lsf/lsf_config.py` & `microcat-0.1.4/microcat/profiles/lsf/lsf_config.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.3/microcat/profiles/lsf/lsf_status.py` & `microcat-0.1.4/microcat/profiles/lsf/lsf_status.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.3/microcat/profiles/lsf/lsf_submit.py` & `microcat-0.1.4/microcat/profiles/lsf/lsf_submit.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.3/microcat/profiles/lsf/memory_units.py` & `microcat-0.1.4/microcat/profiles/lsf/memory_units.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.3/microcat/rules/ERCC.smk` & `microcat-0.1.4/microcat/rules/ERCC.smk`

 * *Files identical despite different names*

### Comparing `microcat-0.1.3/microcat/rules/classfier.smk` & `microcat-0.1.4/microcat/rules/classfier.smk`

 * *Files identical despite different names*

### Comparing `microcat-0.1.3/microcat/rules/database.smk` & `microcat-0.1.4/microcat/rules/database.smk`

 * *Files identical despite different names*

### Comparing `microcat-0.1.3/microcat/rules/host.smk` & `microcat-0.1.4/microcat/rules/host.smk`

 * *Files 2% similar despite different names*

```diff
@@ -102,15 +102,15 @@
     if "tenX" in config["params"]["host"]["starsolo"]["assay"]:
         # This will be executed if the string "tenX" is in the assay parameter
 
         if config["params"]["host"]["starsolo"]["assay"]=="tenX_v3":
             rule starsolo_10x_count:
                 input:
                     # Directory containing input fastq files
-                    fastqs_dir=lambda wildcards: sample.get_fastqs_dir(SAMPLES,wildcards),
+                    fastqs_dir=lambda wildcards: microcat.get_fastqs_dir(SAMPLES,wildcards),
                 output:
                     # Path to the output features.tsv file
                     features_file = os.path.join(
                         config["output"]["host"],
                         "starsolo_count/{sample}/{sample}_features.tsv"),
                     matrix_file = os.path.join(
                         config["output"]["host"],
@@ -121,16 +121,16 @@
                     # Path to the output unmapped bam
                     mapped_bam_file = os.path.join(
                         config["output"]["host"],
                         "starsolo_count/{sample}/Aligned_sortedByCoord_out.bam")
                 resources:
                     mem_mb=100000  # This rule needs 100 GB of memory
                 params:
-                    barcode_reads = lambda wildcards: sample.get_starsolo_sample_id(SAMPLES, wildcards, "fq1"),
-                    cdna_reads = lambda wildcards: sample.get_starsolo_sample_id(SAMPLES, wildcards, "fq2"),
+                    barcode_reads = lambda wildcards: microcat.get_starsolo_sample_id(SAMPLES, wildcards, "fq1"),
+                    cdna_reads = lambda wildcards: microcat.get_starsolo_sample_id(SAMPLES, wildcards, "fq2"),
                     starsolo_out = os.path.join(
                         config["output"]["host"],
                         "starsolo_count/"),
                     reference = config["params"]["host"]["starsolo"]["reference"],
                     variousParams = config["params"]["host"]["starsolo"]["variousParams"],
                     threads = config["params"]["host"]["starsolo"]["threads"]
                 log:
@@ -175,15 +175,15 @@
                     ln -sr "{params.starsolo_out}/{wildcards.sample}/Solo.out/Gene/filtered/barcodes.tsv" "{output.barcodes_file}" ;\
                     mv "{params.starsolo_out}/{wildcards.sample}/Aligned.sortedByCoord.out.bam" "{output.mapped_bam_file}";\
                     '''        
         if config["params"]["host"]["starsolo"]["assay"]=="tenX_v1":
             rule starsolo_10x_count:
                 input:
                     # Directory containing input fastq files
-                    fastqs_dir=lambda wildcards: sample.get_fastqs_dir(SAMPLES,wildcards),
+                    fastqs_dir=lambda wildcards: microcat.get_fastqs_dir(SAMPLES,wildcards),
                 output:
                     # Path to the output features.tsv file
                     features_file = os.path.join(
                         config["output"]["host"],
                         "starsolo_count/{sample}/{sample}_features.tsv"),
                     matrix_file = os.path.join(
                         config["output"]["host"],
@@ -192,16 +192,16 @@
                         config["output"]["host"],
                         "starsolo_count/{sample}/{sample}_barcodes.tsv"),
                     # Path to the output unmapped bam
                     mapped_bam_file = os.path.join(
                         config["output"]["host"],
                         "starsolo_count/{sample}/Aligned_sortedByCoord_out.bam")
                 params:
-                    barcode_reads = lambda wildcards: sample.get_starsolo_sample_id(SAMPLES, wildcards, "fq1"),
-                    cdna_reads = lambda wildcards: sample.get_starsolo_sample_id(SAMPLES, wildcards, "fq2"),
+                    barcode_reads = lambda wildcards: microcat.get_starsolo_sample_id(SAMPLES, wildcards, "fq1"),
+                    cdna_reads = lambda wildcards: microcat.get_starsolo_sample_id(SAMPLES, wildcards, "fq2"),
                     starsolo_out = os.path.join(
                         config["output"]["host"],
                         "starsolo_count/"),
                     reference = config["params"]["host"]["starsolo"]["reference"],
                     variousParams = config["params"]["host"]["starsolo"]["variousParams"],
                     threads = config["params"]["host"]["starsolo"]["threads"]
                 log:
@@ -249,15 +249,15 @@
                     mv "{params.starsolo_out}/{wildcards.sample}/Aligned.sortedByCoord.out.bam" "{output.mapped_bam_file}";
                     '''   
 
         if config["params"]["host"]["starsolo"]["assay"]=="tenX_v2":
             rule starsolo_10x_count:
                 input:
                     # Directory containing input fastq files
-                    fastqs_dir=lambda wildcards: sample.get_fastqs_dir(SAMPLES,wildcards),
+                    fastqs_dir=lambda wildcards: microcat.get_fastqs_dir(SAMPLES,wildcards),
                 output:
                     # Path to the output features.tsv file
                     features_file = os.path.join(
                         config["output"]["host"],
                         "starsolo_count/{sample}/{sample}_features.tsv"),
                     matrix_file = os.path.join(
                         config["output"]["host"],
@@ -272,16 +272,16 @@
                 params:
                     starsolo_out = os.path.join(
                         config["output"]["host"],
                         "starsolo_count/"),
                     reference = config["params"]["host"]["starsolo"]["reference"],
                     variousParams = config["params"]["host"]["starsolo"]["variousParams"],
                     threads = config["params"]["host"]["starsolo"]["threads"],
-                    barcode_reads = lambda wildcards: sample.get_starsolo_sample_id(SAMPLES, wildcards, "fq1"),
-                    cdna_reads = lambda wildcards: sample.get_starsolo_sample_id(SAMPLES, wildcards, "fq2")
+                    barcode_reads = lambda wildcards: microcat.get_starsolo_sample_id(SAMPLES, wildcards, "fq1"),
+                    cdna_reads = lambda wildcards: microcat.get_starsolo_sample_id(SAMPLES, wildcards, "fq2")
                 log:
                     os.path.join(config["logs"]["host"],
                                 "starsolo/{sample}_starsolo_count.log")
                 benchmark:
                     os.path.join(config["benchmarks"]["host"],
                                 "starsolo/{sample}_starsolo_count.benchmark")
                 conda:
@@ -451,15 +451,15 @@
         #     "../src/generate_pe_manifest_file.py"
         
         rule starsolo_smartseq_count:
             # Input files
             input:
                 # Path to the input manifest file
                 manifest = config["params"]["host"]["starsolo"]["manifest"],
-                fastqs_dir=lambda wildcards: sample.get_fastqs_dir(SAMPLES,wildcards),
+                fastqs_dir=lambda wildcards: microcat.get_fastqs_dir(SAMPLES,wildcards),
             output:
                 # Path to the output features.tsv file
                 features_file = os.path.join(
                     config["output"]["host"],
                     "starsolo_count/features.tsv"),
                 # Path to the output matrix.mtx file
                 matrix_file = os.path.join(
@@ -485,15 +485,15 @@
                 starsolo_out = os.path.join(
                     config["output"]["host"],
                     "starsolo_count/"),
                 # Path to the STAR index directory
                 reference = config["params"]["host"]["starsolo"]["reference"],
                 # Type of sequencing library
                 soloType = config["params"]["host"]["starsolo"]["soloType"],
-                SAMattrRGline = sample.get_SAMattrRGline_from_manifest(config["params"]["host"]["starsolo"]["manifest"]),
+                SAMattrRGline = microcat.get_SAMattrRGline_from_manifest(config["params"]["host"]["starsolo"]["manifest"]),
                 # Additional parameters for STAR
                 variousParams = config["params"]["host"]["starsolo"]["variousParams"],
                 # Number of threads for STAR
                 threads = config["params"]["host"]["starsolo"]["threads"]
             log:
                 os.path.join(config["logs"]["host"],
                             "starsolo/starsolo_count_smartseq2.log")
@@ -622,15 +622,15 @@
 # expected input format for FASTQ file
 # cellranger call to process the raw samples
     rule cellranger_count:
         input:
             # fastqs_dir = config["params"]["data_dir"],
             # r1 = lambda wildcards: get_sample_id(SAMPLES, wildcards, "fq1"),
             # r2 = lambda wildcards: get_sample_id(SAMPLES, wildcards, "fq2")
-            fastqs_dir=lambda wildcards: sample.get_fastqs_dir(SAMPLES,wildcards),
+            fastqs_dir=lambda wildcards: microcat.get_fastqs_dir(SAMPLES,wildcards),
         output:
             features_file = os.path.join(
                 config["output"]["host"],
                 "cellranger_count/{sample}/{sample}_features.tsv"),
             matrix_file = os.path.join(
                 config["output"]["host"],
                 "cellranger_count/{sample}/{sample}_matrix.mtx"),
```

### Comparing `microcat-0.1.3/microcat/sample.py` & `microcat-0.1.4/microcat/sample.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.3/microcat/scripts/INVADEseq.py` & `microcat-0.1.4/microcat/scripts/INVADEseq.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.3/microcat/scripts/extract_kraken_reads.py` & `microcat-0.1.4/microcat/scripts/extract_kraken_reads.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.3/microcat/scripts/extract_microbiome_output.R` & `microcat-0.1.4/microcat/scripts/extract_microbiome_output.R`

 * *Files identical despite different names*

### Comparing `microcat-0.1.3/microcat/scripts/get_ncbi_domains.py` & `microcat-0.1.4/microcat/scripts/get_ncbi_domains.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.3/microcat/scripts/krak2_output_denosing.R` & `microcat-0.1.4/microcat/scripts/krak2_output_denosing.R`

 * *Files identical despite different names*

### Comparing `microcat-0.1.3/microcat/scripts/kraken2mpa.py` & `microcat-0.1.4/microcat/scripts/kraken2mpa.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.3/microcat/scripts/kraken2sc.py` & `microcat-0.1.4/microcat/scripts/kraken2sc.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.3/microcat/scripts/sample_denosing.R` & `microcat-0.1.4/microcat/scripts/sample_denosing.R`

 * *Files identical despite different names*

### Comparing `microcat-0.1.3/microcat/scripts/sckmer_unpaired.R` & `microcat-0.1.4/microcat/scripts/sckmer_unpaired.R`

 * *Files identical despite different names*

### Comparing `microcat-0.1.3/microcat/scripts/spilt_bam_by_tag.py` & `microcat-0.1.4/microcat/scripts/spilt_bam_by_tag.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.3/microcat/snakefiles/scRNA_wf.smk` & `microcat-0.1.4/microcat/snakefiles/scRNA_wf.smk`

 * *Files 6% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 else:
     raise ValueError("Platform must be either 'tenX' or 'smartseq'")
 
 
 
 
 try:
-    SAMPLES = sample.parse_samples(config["params"]["samples"],platform = PLATFORM)
+    SAMPLES = microcat.parse_samples(config["params"]["samples"],platform = PLATFORM)
     SAMPLES_ID_LIST = SAMPLES.index.get_level_values("sample_id").unique()
 except FileNotFoundError:
     warning(f"ERROR: the samples file does not exist. Please see the README file for details. Quitting now.")
     sys.exit(1)
 
 
 # sample_names = [sample_dict["sample"] for sample_dict in _samples]
```

### Comparing `microcat-0.1.3/microcat.egg-info/PKG-INFO` & `microcat-0.1.4/microcat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microcat
-Version: 0.1.3
+Version: 0.1.4
 Summary: a computational toolbox to identificated microbiome from Omics
 Home-page: https://github.com/ChangxingSu/MicroCAT
 Author: Changxing Su
 Author-email: changxingsu42@gmail.com
 License: GPLv3+
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `microcat-0.1.3/microcat.egg-info/SOURCES.txt` & `microcat-0.1.4/microcat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `microcat-0.1.3/setup.py` & `microcat-0.1.4/setup.py`

 * *Files identical despite different names*

