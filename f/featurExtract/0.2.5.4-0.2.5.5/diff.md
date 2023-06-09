# Comparing `tmp/featurExtract-0.2.5.4.tar.gz` & `tmp/featurExtract-0.2.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/featurExtract-0.2.5.4.tar", last modified: Fri Feb 24 06:38:01 2023, max compression
+gzip compressed data, was "dist/featurExtract-0.2.5.5.tar", last modified: Fri Jun  9 09:48:48 2023, max compression
```

## Comparing `featurExtract-0.2.5.4.tar` & `featurExtract-0.2.5.5.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxr-xr-x   0 zhusitao   (501) staff       (20)        0 2023-02-24 06:38:01.000000 featurExtract-0.2.5.4/
--rw-r--r--   0 zhusitao   (501) staff       (20)       18 2021-08-20 08:13:20.000000 featurExtract-0.2.5.4/MANIFEST.in
--rw-r--r--   0 zhusitao   (501) staff       (20)     3472 2023-02-24 06:38:01.000000 featurExtract-0.2.5.4/PKG-INFO
--rw-r--r--   0 zhusitao   (501) staff       (20)     3117 2022-08-04 14:50:42.000000 featurExtract-0.2.5.4/README.md
-drwxr-xr-x   0 zhusitao   (501) staff       (20)        0 2023-02-24 06:38:01.000000 featurExtract-0.2.5.4/featurExtract/
--rw-r--r--   0 zhusitao   (501) staff       (20)      248 2021-07-22 09:50:56.000000 featurExtract-0.2.5.4/featurExtract/__init__.py
--rw-r--r--   0 zhusitao   (501) staff       (20)      272 2021-12-19 03:41:05.000000 featurExtract-0.2.5.4/featurExtract/a.py
--rwxr-xr-x   0 zhusitao   (501) staff       (20)     1928 2021-08-20 07:44:38.000000 featurExtract-0.2.5.4/featurExtract/command_gb.py
--rwxr-xr-x   0 zhusitao   (501) staff       (20)     2364 2021-08-24 01:51:44.000000 featurExtract-0.2.5.4/featurExtract/command_gff.py
-drwxr-xr-x   0 zhusitao   (501) staff       (20)        0 2023-02-24 06:38:01.000000 featurExtract-0.2.5.4/featurExtract/commands/
--rw-r--r--   0 zhusitao   (501) staff       (20)        0 2021-08-20 09:48:06.000000 featurExtract-0.2.5.4/featurExtract/commands/__init__.py
--rwxr-xr-x   0 zhusitao   (501) staff       (20)     8015 2022-07-12 13:32:28.000000 featurExtract-0.2.5.4/featurExtract/commands/extract_CDS.py
--rwxr-xr-x   0 zhusitao   (501) staff       (20)     4655 2022-08-10 09:02:03.000000 featurExtract-0.2.5.4/featurExtract/commands/extract_IGR.py
--rwxr-xr-x   0 zhusitao   (501) staff       (20)     5152 2022-07-12 14:00:02.000000 featurExtract-0.2.5.4/featurExtract/commands/extract_UTR.py
--rwxr-xr-x   0 zhusitao   (501) staff       (20)    13110 2022-07-12 14:15:50.000000 featurExtract-0.2.5.4/featurExtract/commands/extract_cdna.py
--rwxr-xr-x   0 zhusitao   (501) staff       (20)    15336 2022-07-14 03:54:00.000000 featurExtract-0.2.5.4/featurExtract/commands/extract_dORF.py
--rwxr-xr-x   0 zhusitao   (501) staff       (20)     4035 2022-07-14 04:14:36.000000 featurExtract-0.2.5.4/featurExtract/commands/extract_exon.py
--rwxr-xr-x   0 zhusitao   (501) staff       (20)     3353 2022-07-14 04:20:57.000000 featurExtract-0.2.5.4/featurExtract/commands/extract_gene.py
--rwxr-xr-x   0 zhusitao   (501) staff       (20)     3342 2022-07-14 06:23:32.000000 featurExtract-0.2.5.4/featurExtract/commands/extract_intron.py
--rwxr-xr-x   0 zhusitao   (501) staff       (20)     7533 2022-07-14 06:48:00.000000 featurExtract-0.2.5.4/featurExtract/commands/extract_mRNA.py
--rwxr-xr-x   0 zhusitao   (501) staff       (20)     5160 2022-07-14 07:14:56.000000 featurExtract-0.2.5.4/featurExtract/commands/extract_promoter.py
--rwxr-xr-x   0 zhusitao   (501) staff       (20)     1361 2021-08-20 09:54:37.000000 featurExtract-0.2.5.4/featurExtract/commands/extract_rRNA.py
--rwxr-xr-x   0 zhusitao   (501) staff       (20)     1360 2021-08-20 09:54:58.000000 featurExtract-0.2.5.4/featurExtract/commands/extract_tRNA.py
--rwxr-xr-x   0 zhusitao   (501) staff       (20)     5576 2022-07-14 07:30:41.000000 featurExtract-0.2.5.4/featurExtract/commands/extract_terminator.py
--rwxr-xr-x   0 zhusitao   (501) staff       (20)    31493 2023-02-24 04:00:31.000000 featurExtract-0.2.5.4/featurExtract/commands/extract_uORF.py
-drwxr-xr-x   0 zhusitao   (501) staff       (20)        0 2023-02-24 06:38:01.000000 featurExtract-0.2.5.4/featurExtract/database/
--rwxr-xr-x   0 zhusitao   (501) staff       (20)      572 2021-07-22 09:50:56.000000 featurExtract-0.2.5.4/featurExtract/database/database.py
--rwxr-xr-x   0 zhusitao   (501) staff       (20)    16751 2022-09-25 03:51:17.000000 featurExtract-0.2.5.4/featurExtract/feature_extract.py
--rwxr-xr-x   0 zhusitao   (501) staff       (20)     7561 2021-08-20 07:50:44.000000 featurExtract-0.2.5.4/featurExtract/genBank_extract.py
--rwxr-xr-x   0 zhusitao   (501) staff       (20)     3152 2021-07-22 09:50:56.000000 featurExtract-0.2.5.4/featurExtract/parameter.py
-drwxr-xr-x   0 zhusitao   (501) staff       (20)        0 2023-02-24 06:38:01.000000 featurExtract-0.2.5.4/featurExtract/utils/
--rw-r--r--   0 zhusitao   (501) staff       (20)        0 2021-08-20 03:25:23.000000 featurExtract-0.2.5.4/featurExtract/utils/__init__.py
--rw-r--r--   0 zhusitao   (501) staff       (20)      125 2021-08-20 09:23:21.000000 featurExtract-0.2.5.4/featurExtract/utils/coverage.py
--rw-r--r--   0 zhusitao   (501) staff       (20)     2326 2021-08-20 03:52:32.000000 featurExtract-0.2.5.4/featurExtract/utils/util.py
--rw-r--r--   0 zhusitao   (501) staff       (20)    16564 2022-09-16 07:58:22.000000 featurExtract-0.2.5.4/featurExtract/utils/visualize.py
--rwxr-xr-x   0 zhusitao   (501) staff       (20)       24 2023-02-24 06:37:04.000000 featurExtract-0.2.5.4/featurExtract/version.py
-drwxr-xr-x   0 zhusitao   (501) staff       (20)        0 2023-02-24 06:38:01.000000 featurExtract-0.2.5.4/featurExtract.egg-info/
--rw-r--r--   0 zhusitao   (501) staff       (20)     3472 2023-02-24 06:38:01.000000 featurExtract-0.2.5.4/featurExtract.egg-info/PKG-INFO
--rw-r--r--   0 zhusitao   (501) staff       (20)     1224 2023-02-24 06:38:01.000000 featurExtract-0.2.5.4/featurExtract.egg-info/SOURCES.txt
--rw-r--r--   0 zhusitao   (501) staff       (20)        1 2023-02-24 06:38:01.000000 featurExtract-0.2.5.4/featurExtract.egg-info/dependency_links.txt
--rw-r--r--   0 zhusitao   (501) staff       (20)      113 2023-02-24 06:38:01.000000 featurExtract-0.2.5.4/featurExtract.egg-info/entry_points.txt
--rw-r--r--   0 zhusitao   (501) staff       (20)       80 2023-02-24 06:38:01.000000 featurExtract-0.2.5.4/featurExtract.egg-info/requires.txt
--rw-r--r--   0 zhusitao   (501) staff       (20)       14 2023-02-24 06:38:01.000000 featurExtract-0.2.5.4/featurExtract.egg-info/top_level.txt
--rw-r--r--   0 zhusitao   (501) staff       (20)       38 2023-02-24 06:38:01.000000 featurExtract-0.2.5.4/setup.cfg
--rw-r--r--   0 zhusitao   (501) staff       (20)     1283 2021-08-20 10:06:18.000000 featurExtract-0.2.5.4/setup.py
+drwxr-xr-x   0 zhusitao   (501) staff       (20)        0 2023-06-09 09:48:48.000000 featurExtract-0.2.5.5/
+-rw-r--r--   0 zhusitao   (501) staff       (20)       18 2021-08-20 08:13:20.000000 featurExtract-0.2.5.5/MANIFEST.in
+-rw-r--r--   0 zhusitao   (501) staff       (20)     3472 2023-06-09 09:48:48.000000 featurExtract-0.2.5.5/PKG-INFO
+-rw-r--r--   0 zhusitao   (501) staff       (20)     3117 2022-08-04 14:50:42.000000 featurExtract-0.2.5.5/README.md
+drwxr-xr-x   0 zhusitao   (501) staff       (20)        0 2023-06-09 09:48:48.000000 featurExtract-0.2.5.5/featurExtract/
+-rw-r--r--   0 zhusitao   (501) staff       (20)      248 2021-07-22 09:50:56.000000 featurExtract-0.2.5.5/featurExtract/__init__.py
+-rw-r--r--   0 zhusitao   (501) staff       (20)      272 2021-12-19 03:41:05.000000 featurExtract-0.2.5.5/featurExtract/a.py
+-rwxr-xr-x   0 zhusitao   (501) staff       (20)     1928 2021-08-20 07:44:38.000000 featurExtract-0.2.5.5/featurExtract/command_gb.py
+-rwxr-xr-x   0 zhusitao   (501) staff       (20)     2364 2021-08-24 01:51:44.000000 featurExtract-0.2.5.5/featurExtract/command_gff.py
+drwxr-xr-x   0 zhusitao   (501) staff       (20)        0 2023-06-09 09:48:48.000000 featurExtract-0.2.5.5/featurExtract/commands/
+-rw-r--r--   0 zhusitao   (501) staff       (20)        0 2021-08-20 09:48:06.000000 featurExtract-0.2.5.5/featurExtract/commands/__init__.py
+-rwxr-xr-x   0 zhusitao   (501) staff       (20)     8178 2023-06-09 09:32:14.000000 featurExtract-0.2.5.5/featurExtract/commands/extract_CDS.py
+-rwxr-xr-x   0 zhusitao   (501) staff       (20)     4655 2022-08-10 09:02:03.000000 featurExtract-0.2.5.5/featurExtract/commands/extract_IGR.py
+-rwxr-xr-x   0 zhusitao   (501) staff       (20)     5057 2023-06-09 09:12:54.000000 featurExtract-0.2.5.5/featurExtract/commands/extract_UTR.py
+-rwxr-xr-x   0 zhusitao   (501) staff       (20)    13110 2022-07-12 14:15:50.000000 featurExtract-0.2.5.5/featurExtract/commands/extract_cdna.py
+-rwxr-xr-x   0 zhusitao   (501) staff       (20)    15336 2022-07-14 03:54:00.000000 featurExtract-0.2.5.5/featurExtract/commands/extract_dORF.py
+-rwxr-xr-x   0 zhusitao   (501) staff       (20)     4035 2022-07-14 04:14:36.000000 featurExtract-0.2.5.5/featurExtract/commands/extract_exon.py
+-rwxr-xr-x   0 zhusitao   (501) staff       (20)     3353 2022-07-14 04:20:57.000000 featurExtract-0.2.5.5/featurExtract/commands/extract_gene.py
+-rwxr-xr-x   0 zhusitao   (501) staff       (20)     3342 2022-07-14 06:23:32.000000 featurExtract-0.2.5.5/featurExtract/commands/extract_intron.py
+-rwxr-xr-x   0 zhusitao   (501) staff       (20)     7533 2022-07-14 06:48:00.000000 featurExtract-0.2.5.5/featurExtract/commands/extract_mRNA.py
+-rwxr-xr-x   0 zhusitao   (501) staff       (20)     5160 2022-07-14 07:14:56.000000 featurExtract-0.2.5.5/featurExtract/commands/extract_promoter.py
+-rwxr-xr-x   0 zhusitao   (501) staff       (20)     1361 2021-08-20 09:54:37.000000 featurExtract-0.2.5.5/featurExtract/commands/extract_rRNA.py
+-rwxr-xr-x   0 zhusitao   (501) staff       (20)     1360 2021-08-20 09:54:58.000000 featurExtract-0.2.5.5/featurExtract/commands/extract_tRNA.py
+-rwxr-xr-x   0 zhusitao   (501) staff       (20)     5576 2022-07-14 07:30:41.000000 featurExtract-0.2.5.5/featurExtract/commands/extract_terminator.py
+-rwxr-xr-x   0 zhusitao   (501) staff       (20)    31030 2023-06-09 08:49:48.000000 featurExtract-0.2.5.5/featurExtract/commands/extract_uORF.py
+-rwxr-xr-x   0 zhusitao   (501) staff       (20)    33238 2023-06-09 02:52:54.000000 featurExtract-0.2.5.5/featurExtract/commands/extract_uORF_back.py
+drwxr-xr-x   0 zhusitao   (501) staff       (20)        0 2023-06-09 09:48:48.000000 featurExtract-0.2.5.5/featurExtract/database/
+-rwxr-xr-x   0 zhusitao   (501) staff       (20)      572 2021-07-22 09:50:56.000000 featurExtract-0.2.5.5/featurExtract/database/database.py
+-rwxr-xr-x   0 zhusitao   (501) staff       (20)    17546 2023-06-09 09:39:26.000000 featurExtract-0.2.5.5/featurExtract/feature_extract.py
+-rwxr-xr-x   0 zhusitao   (501) staff       (20)     7561 2021-08-20 07:50:44.000000 featurExtract-0.2.5.5/featurExtract/genBank_extract.py
+-rwxr-xr-x   0 zhusitao   (501) staff       (20)     3152 2021-07-22 09:50:56.000000 featurExtract-0.2.5.5/featurExtract/parameter.py
+drwxr-xr-x   0 zhusitao   (501) staff       (20)        0 2023-06-09 09:48:48.000000 featurExtract-0.2.5.5/featurExtract/utils/
+-rw-r--r--   0 zhusitao   (501) staff       (20)        0 2021-08-20 03:25:23.000000 featurExtract-0.2.5.5/featurExtract/utils/__init__.py
+-rw-r--r--   0 zhusitao   (501) staff       (20)      125 2021-08-20 09:23:21.000000 featurExtract-0.2.5.5/featurExtract/utils/coverage.py
+-rw-r--r--   0 zhusitao   (501) staff       (20)     2326 2021-08-20 03:52:32.000000 featurExtract-0.2.5.5/featurExtract/utils/util.py
+-rw-r--r--   0 zhusitao   (501) staff       (20)    16564 2022-09-16 07:58:22.000000 featurExtract-0.2.5.5/featurExtract/utils/visualize.py
+-rwxr-xr-x   0 zhusitao   (501) staff       (20)       24 2023-06-09 09:48:33.000000 featurExtract-0.2.5.5/featurExtract/version.py
+drwxr-xr-x   0 zhusitao   (501) staff       (20)        0 2023-06-09 09:48:48.000000 featurExtract-0.2.5.5/featurExtract.egg-info/
+-rw-r--r--   0 zhusitao   (501) staff       (20)     3472 2023-06-09 09:48:47.000000 featurExtract-0.2.5.5/featurExtract.egg-info/PKG-INFO
+-rw-r--r--   0 zhusitao   (501) staff       (20)     1268 2023-06-09 09:48:47.000000 featurExtract-0.2.5.5/featurExtract.egg-info/SOURCES.txt
+-rw-r--r--   0 zhusitao   (501) staff       (20)        1 2023-06-09 09:48:47.000000 featurExtract-0.2.5.5/featurExtract.egg-info/dependency_links.txt
+-rw-r--r--   0 zhusitao   (501) staff       (20)      113 2023-06-09 09:48:47.000000 featurExtract-0.2.5.5/featurExtract.egg-info/entry_points.txt
+-rw-r--r--   0 zhusitao   (501) staff       (20)       80 2023-06-09 09:48:47.000000 featurExtract-0.2.5.5/featurExtract.egg-info/requires.txt
+-rw-r--r--   0 zhusitao   (501) staff       (20)       14 2023-06-09 09:48:47.000000 featurExtract-0.2.5.5/featurExtract.egg-info/top_level.txt
+-rw-r--r--   0 zhusitao   (501) staff       (20)       38 2023-06-09 09:48:48.000000 featurExtract-0.2.5.5/setup.cfg
+-rw-r--r--   0 zhusitao   (501) staff       (20)     1283 2021-08-20 10:06:18.000000 featurExtract-0.2.5.5/setup.py
```

### Comparing `featurExtract-0.2.5.4/PKG-INFO` & `featurExtract-0.2.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurExtract
-Version: 0.2.5.4
+Version: 0.2.5.5
 Summary: Extract genome ferature sequence for biologists
 Home-page: https://github.com/SitaoZ/featurExtract.git
 Author: zhusitao
 Author-email: zhusitao1990@163.com
 License: MIT
 Keywords: genome feature,extract
 Platform: UNKNOWN
```

### Comparing `featurExtract-0.2.5.4/README.md` & `featurExtract-0.2.5.5/README.md`

 * *Files identical despite different names*

### Comparing `featurExtract-0.2.5.4/featurExtract/command_gb.py` & `featurExtract-0.2.5.5/featurExtract/command_gb.py`

 * *Files identical despite different names*

### Comparing `featurExtract-0.2.5.4/featurExtract/command_gff.py` & `featurExtract-0.2.5.5/featurExtract/command_gff.py`

 * *Files identical despite different names*

### Comparing `featurExtract-0.2.5.4/featurExtract/commands/extract_CDS.py` & `featurExtract-0.2.5.5/featurExtract/commands/extract_CDS.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import sys
 import gffutils
 import pandas as pd 
 from tqdm import tqdm
 from Bio import SeqIO
 from Bio.Seq import Seq
 from Bio.SeqRecord import SeqRecord
-from collections import defaultdict
+from collections import defaultdict, deque
 from featurExtract.database.database import create_db
 from featurExtract.utils.util import add_stop_codon,mRNA_type
 
 '''
 https://www.ncbi.nlm.nih.gov/genbank/genomes_gff/
 '''
 def stop_codon(db, transcript, genome):
@@ -29,20 +29,23 @@
         args: parse from argparse
     return:
         elements write to a file or stdout
     '''
     # print(args)
     db = gffutils.FeatureDB(args.database, keep_order=True) # load database
     # dict
-    cds_seq_list = []
+    cds_seq_list = deque()
     # cds_seq = pd.DataFrame(columns=['TranscriptID','Chrom','Start','End','Strand','CDS'])
-    cds_record = []
+    cds_record = deque()
     index = 0
     # assert GTF or GFF
-    mRNA_str = mRNA_type(args.style)
+    if args.rna_feature == 'mRNA':
+        mRNA_str = mRNA_type(args.style)
+    else:
+        mRNA_str = tuple([x for x in list(db.featuretypes()) if 'RNA' in x or 'trascript' in x])
     # loop all transcript in genome
     if not args.transcript:
         for t in tqdm(db.features_of_type(mRNA_str, order_by='start'), \
                                    total = len(list(db.features_of_type(mRNA_str, order_by='start'))),\
                                    ncols = 80, desc="CDS Processing :"):
             seq = ''
             cds_start_transcript = 0
```

### Comparing `featurExtract-0.2.5.4/featurExtract/commands/extract_IGR.py` & `featurExtract-0.2.5.5/featurExtract/commands/extract_IGR.py`

 * *Files identical despite different names*

### Comparing `featurExtract-0.2.5.4/featurExtract/commands/extract_UTR.py` & `featurExtract-0.2.5.5/featurExtract/commands/extract_UTR.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import sys
 import gffutils
 import pandas as pd 
 from tqdm import tqdm 
 from Bio import SeqIO
 from Bio.Seq import Seq
 from Bio.SeqRecord import SeqRecord
-from collections import defaultdict
+from collections import defaultdict, deque
 from featurExtract.utils.util import utr3_type, utr5_type, mRNA_type
 
 
 
 _CSV_HEADER = ['TranscriptID','Chrom', \
                'Start','End','Strand', \
                'UTR5','UTR5_Region','UTR5_Count', \
@@ -23,16 +23,20 @@
     return:
         file write to file or stdout
     '''
     db = gffutils.FeatureDB(args.database, keep_order=True) # load database
     # header
     # utr_seq = pd.DataFrame(columns=_CSV_HEADER)
     # dist fastest way 
-    utr_seq_list = []
-    mRNA_str = mRNA_type(args.style)
+    utr_seq_list = deque()
+    # mRNA_str = mRNA_type(args.style)
+    if args.rna_feature == 'mRNA':
+        mRNA_str = mRNA_type(args.style)
+    else:
+        mRNA_str = tuple([x for x in list(db.featuretypes()) if 'RNA' in x or 'trascript' in x])
     utr3_t = utr3_type(args.style)
     utr5_t = utr5_type(args.style)
     if not args.transcript:
         # all UTR in genome 
         index = 0
         for t in tqdm(db.features_of_type(mRNA_str, order_by='start'), \
                       total = len(list(db.features_of_type(mRNA_str, order_by='start'))), \
@@ -53,23 +57,18 @@
                 seq5_count += 1
                 seq5_region.append('-'.join(map(str,[c.start,c.end])))
             seq3 = Seq(seq3)
             seq5 = Seq(seq5)
             if t.strand == '-':
                 seq3 = seq3.reverse_complement()
                 seq5 = seq5.reverse_complement()
-
-            # utr_seq.loc[index] = [t.id, t.chrom, t.start, t.end, t.strand,
-            #                      seq5, '|'.join(seq5_region), seq5_count, 
-            #                      seq3, '|'.join(seq3_region), seq3_count]
-            # index += 1
             it = [t.id, t.chrom, t.start, t.end, t.strand,\
                   seq5, '|'.join(seq5_region), seq5_count,\
                   seq3, '|'.join(seq3_region), seq3_count]
-            utr_seq_list.append(dict((_CSV_HEADER[i], it[i]) for i in range(len(_CSV_HEADER))))
+            utr_seq_list.append(dict(zip(_CSV_HEADER, it)))
         utr_seq = pd.DataFrame.from_dict(utr_seq_list)
         utr_seq.to_csv(args.output, sep=',', index=False)
     else:
         # return a specific transcript
         out = [] 
         for t in db.features_of_type(mRNA_str, order_by='start'):
             if args.transcript in t.id:
```

### Comparing `featurExtract-0.2.5.4/featurExtract/commands/extract_cdna.py` & `featurExtract-0.2.5.5/featurExtract/commands/extract_cdna.py`

 * *Files identical despite different names*

### Comparing `featurExtract-0.2.5.4/featurExtract/commands/extract_dORF.py` & `featurExtract-0.2.5.5/featurExtract/commands/extract_dORF.py`

 * *Files identical despite different names*

### Comparing `featurExtract-0.2.5.4/featurExtract/commands/extract_exon.py` & `featurExtract-0.2.5.5/featurExtract/commands/extract_exon.py`

 * *Files identical despite different names*

### Comparing `featurExtract-0.2.5.4/featurExtract/commands/extract_gene.py` & `featurExtract-0.2.5.5/featurExtract/commands/extract_gene.py`

 * *Files identical despite different names*

### Comparing `featurExtract-0.2.5.4/featurExtract/commands/extract_intron.py` & `featurExtract-0.2.5.5/featurExtract/commands/extract_intron.py`

 * *Files identical despite different names*

### Comparing `featurExtract-0.2.5.4/featurExtract/commands/extract_mRNA.py` & `featurExtract-0.2.5.5/featurExtract/commands/extract_mRNA.py`

 * *Files identical despite different names*

### Comparing `featurExtract-0.2.5.4/featurExtract/commands/extract_promoter.py` & `featurExtract-0.2.5.5/featurExtract/commands/extract_promoter.py`

 * *Files identical despite different names*

### Comparing `featurExtract-0.2.5.4/featurExtract/commands/extract_rRNA.py` & `featurExtract-0.2.5.5/featurExtract/commands/extract_rRNA.py`

 * *Files identical despite different names*

### Comparing `featurExtract-0.2.5.4/featurExtract/commands/extract_tRNA.py` & `featurExtract-0.2.5.5/featurExtract/commands/extract_tRNA.py`

 * *Files identical despite different names*

### Comparing `featurExtract-0.2.5.4/featurExtract/commands/extract_terminator.py` & `featurExtract-0.2.5.5/featurExtract/commands/extract_terminator.py`

 * *Files identical despite different names*

### Comparing `featurExtract-0.2.5.4/featurExtract/commands/extract_uORF.py` & `featurExtract-0.2.5.5/featurExtract/commands/extract_uORF_back.py`

 * *Files 3% similar despite different names*

```diff
@@ -395,27 +395,32 @@
     # uORF_seq = pd.DataFrame(columns=_uORF_csv_header)
     uORF_seq_list = []
     # gff
     uORF_gff = open(args.output,'w')
     # fasta
     uorf_record = []
     index = 0
-    mRNA_str = mRNA_type(args.style) 
+    if args.rna_feature == 'mRNA':
+        mRNA_str = mRNA_type(args.style)
+    else:
+        mRNA_str = tuple([x for x in list(db.featuretypes()) if 'RNA' in x or 'trascript' in x])
     error_count = 0
     # loop all transcripts in genome
     if not args.transcript:
         for t in tqdm(db.features_of_type(mRNA_str, order_by='start'), \
                       total = len(list(db.features_of_type(mRNA_str, order_by='start'))), \
                       ncols = 80, desc = "uORF Processing :"):
             # primary transcript (pt) 是基因组上的转录本的序列，
-            # 有的会包括intron，所以提取的序列和matural transcript 不一致
-            # print(t)
+            # 有的会包括intron，所以提取的序列和matural transcript (mt) 不一致
             pt = t.sequence(args.genome, use_strand=True)
             # matural transcript (mt)
-            # exon 提取的是转录本内成熟的MRNA的序列,即外显子收尾相连的matural transcript
+            # 该步骤是获取序列: 转录本序列，CDS序列, five_prime_UTR, three_prime_UTR
+            # 但是有的基因注释不正确，导致成熟转录本序列的两个来源不一致，一个是exon来源的，一个是five_prime_UTR和CDS来源的
+            # 针对这种请情况，我们使用 five_prime_UTR + CDS + three_prime_UTR 拼接形成成熟的转录本序列用于uORF的注释
+            # exon 提取的是转录本内成熟的mRNA的序列,即外显子按基因组坐标首尾相连的matural transcript
             mt = ''
             exons_list = []
             for e in db.children(t, featuretype='exon', order_by='start'):
                 exons_list.append([e.start, e.end])
                 s = e.sequence(args.genome, use_strand=False) # 不反向互补，对于负链要得到全部的cds后再一次性反向互补
                 mt += s
             mt = Seq(mt)
@@ -454,14 +459,18 @@
             uORF_dict = uORF_.uorf_parse()
             if len(uORF_dict) == 0: # CDS error
                 continue
             # loop for type1, type2 and type3
             for key in sorted(uORF_dict.keys()):
                 # print(key,len(uORF_dict[key]))
                 for it in uORF_dict[key]:
+                    # uORF length filter 
+                    if len(it[8]) <= args.length:
+                        # default: 6
+                        continue
                     # csv output format 
                     if args.output_format == 'csv':
                         # uORF_seq.loc[index] = it
                         # dict 
                         uORF_seq_list.append(dict((_uORF_csv_header[i],it[i]) for i in range(len(_uORF_csv_header))))
                         index += 1
                     elif args.output_format == 'fasta':
@@ -481,24 +490,32 @@
                         gff = GFF(exons_list, it, 'uORF')
                         uorf_gff_line,features_gff_lines = gff.parse() 
                         # print(uorf_gff_line)
                         uORF_gff.write(uorf_gff_line+"\n") 
                         for feature_line in features_gff_lines:
                             # print(feature_line)
                             uORF_gff.write(feature_line+"\n")
+                    else:
+                        # args.output_format == 'csv'
+                        uORF_seq_list.append(dict((_uORF_csv_header[i],it[i]) for i in range(len(_uORF_csv_header))))
+                        index += 1 
         # output file 
         if args.output_format == 'csv':
             uORF_seq = pd.DataFrame.from_dict(uORF_seq_list)
             uORF_seq.to_csv(args.output, sep=',', index=False)
         elif args.output_format == 'gff':
             uORF_gff.close()
         elif args.output_format == 'fasta':
             with open(args.output,'w') as handle:
                 SeqIO.write(uorf_record, handle, "fasta")
+        else:
+            uORF_seq = pd.DataFrame.from_dict(uORF_seq_list)
+            uORF_seq.to_csv(args.output, sep=',', index=False)
     else:
+        mRNA_str = tuple([x for x in list(db.featuretypes()) if 'RNA' in x or 'trascript' in x])
         # specify the transcript id; only one transcript
         for t in db.features_of_type(mRNA_str, order_by='start'):
             # primary transcript (pt) 是基因组上的转录本的序列，
             # 有的会包括intron，所以提取的序列和matural transcript 不一致
             # id specify
             if args.transcript in t.id:
                 pt = t.sequence(args.genome, use_strand=True)
@@ -589,14 +606,20 @@
                             gff = GFF(exons_list, it, 'uORF')
                             uorf_gff_line,features_gff_lines = gff.parse()
                             ex_locations = gff.uorf_exons_location()
                             uorf_location_genome.append(ex_locations) # for schematic on genome
                             uORF_gff.write(uorf_gff_line+"\n")
                             for feature_line in features_gff_lines:
                                 uORF_gff.write(feature_line+"\n")
+                        else:
+                            uORF_seq_list.append(dict((_uORF_csv_header[i],it[i]) for i in range(len(_uORF_csv_header))))
+                            index += 1
+                            gff = GFF(exons_list, it, 'uORF')
+                            ex_locations = gff.uorf_exons_location()
+                            uorf_location_genome.append(ex_locations)
                 # figure the schametic 
                 # without intron 
                 if args.schematic_without_intron:
                     figure = visual_transcript(args.schematic_without_intron, 
                                                args.transcript, 
                                                uORF_.transcript_location(),
                                                uORF_.cds_location_transcript(),
@@ -618,8 +641,11 @@
                     uORF_seq = pd.DataFrame.from_dict(uORF_seq_list)
                     uORF_seq.to_csv(args.output, sep=',', index=False)
                 elif args.output_format == 'gff':
                     uORF_gff.close()
                 elif args.output_format == 'fasta':
                     with open(args.output,'w') as handle:
                         SeqIO.write(uorf_record, handle, "fasta")
+                else:
+                    uORF_seq = pd.DataFrame.from_dict(uORF_seq_list)
+                    uORF_seq.to_csv(args.output, sep=',', index=False)
                 break
```

### Comparing `featurExtract-0.2.5.4/featurExtract/database/database.py` & `featurExtract-0.2.5.5/featurExtract/database/database.py`

 * *Files identical despite different names*

### Comparing `featurExtract-0.2.5.4/featurExtract/feature_extract.py` & `featurExtract-0.2.5.5/featurExtract/feature_extract.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- coding: utf-8 -*-
 import os
 import time
 import argparse
 import gffutils
 import pandas as pd
+import multiprocessing
 from Bio import SeqIO
 from Bio.Seq import Seq
 from Bio.SeqRecord import SeqRecord
 from featurExtract.commands.extract_UTR import utr
 from featurExtract.commands.extract_uORF import get_uorf
 from featurExtract.commands.extract_dORF import get_dorf
 from featurExtract.commands.extract_CDS import get_cds
@@ -152,17 +153,17 @@
 parser_promoter.add_argument('-d', '--database', type=str, required=True, 
                              help='database generated by subcommand create')
 parser_promoter.add_argument('-f', '--genome', type=str, required=True,
                              help='genome fasta path')
 parser_promoter.add_argument('-g', '--gene', type=str, 
                              help='specific gene; if not given, return whole genes')
 parser_promoter.add_argument('-l', '--promoter_length', type=int, default=100,
-                             help='promoter length before TSS (default 100 nt)')
+                             help='promoter length before TSS (default: 100)')
 parser_promoter.add_argument('-u', '--utr5_upper_length', type=int, default=10,
-                             help='5\' utr length after TSS (default 10 nt)')
+                             help='5\' utr length after TSS (default: 10)')
 parser_promoter.add_argument('-o', '--output', type=str, 
                              help = 'output file path')
 parser_promoter.add_argument('-t', '--output_format', type=str, choices=['csv','fasta'], 
                              help = 'output format')
 parser_promoter.add_argument('-p', '--print', action="store_true", 
                              help = 'output to stdout')
 parser_promoter.set_defaults(func=promoter)
@@ -173,17 +174,17 @@
 parser_terminator.add_argument('-d', '--database', type=str, required=True,
                              help='database generated by subcommand create')
 parser_terminator.add_argument('-f', '--genome', type=str, required=True,
                              help='genome fasta path')
 parser_terminator.add_argument('-g', '--gene', type=str,
                              help='specific gene; if not given, return whole genes')
 parser_terminator.add_argument('-l', '--terminator_length', type=int, default=100,
-                             help='terminator length (default 100 nt)')
+                             help='terminator length (default: 100)')
 parser_terminator.add_argument('-u', '--utr3_upper_length', type=int, default=10,
-                             help='3\' length (default 10 nt)')
+                             help='3\' length (default: 10)')
 parser_terminator.add_argument('-o', '--output', type=str,
                              help = 'output file path')
 parser_terminator.add_argument('-t', '--output_format', type=str, choices=['csv','fasta'],
                              help = 'output format')
 parser_terminator.add_argument('-p', '--print', action="store_true",
                              help = 'output to stdout')
 parser_terminator.set_defaults(func=terminator)
@@ -270,29 +271,35 @@
 parser_utr.add_argument('-i', '--transcript', type=str, 
                         help='specific transcript id; if not given, \
                         whole transcript will return')
 parser_utr.add_argument('-o', '--output', type=str, 
                         help='output file path')
 parser_utr.add_argument('-p', '--print', action="store_true", 
                         help='output to stdout')
+parser_utr.add_argument('-r', '--rna_feature', choices=['mRNA', 'all'], default='mRNA',
+                         help='The type of RNA used to extract UTR, (default: mRNA)')
 parser_utr.add_argument('-s', '--style', choices=['GFF','GTF'], 
                         help = 'GTF database or GFF database')
 parser_utr.set_defaults(func=UTR)
 
 # uORF subcommand
 parser_uORF = subparsers.add_parser('uORF', help='extract upper stream open reading sequence in genome or gene')
 parser_uORF.add_argument('-d', '--database', type=str, required=True, 
                          help='database generated by subcommand create')
 parser_uORF.add_argument('-f', '--genome', type=str, required=True, 
                          help='genome fasta')
 parser_uORF.add_argument('-i', '--transcript', type=str, 
                          help='specific transcript id; if not given, \
                                whole transcript will return')
+parser_uORF.add_argument('-l', '--length', type=int, default=6,
+                         help='uORF length, (default: 6)')
+parser_uORF.add_argument('-r', '--rna_feature', choices=['mRNA', 'all'], default='mRNA',
+                         help='The type of RNA used to make uORF identification (default: mRNA)')
 parser_uORF.add_argument('-t', '--output_format', choices=['csv','fasta','gff'], 
-                        help='output format ')
+                        help='output format (default: csv)')
 parser_uORF.add_argument('-o', '--output', type=str, 
                          help='output file path')
 parser_uORF.add_argument('-m', '--schematic_without_intron', action='store_false',default='False',
                          help='schematic figure file for uORF, CDS and transcript without intron')
 parser_uORF.add_argument('-n', '--schematic_with_intron', action='store_false',default='False',
                          help='schematic figure file for uORF, CDS and transcript with intron')
 parser_uORF.add_argument('-s', '--style', choices=['GFF','GTF'], 
@@ -308,14 +315,16 @@
 parser_cds.add_argument('-i', '--transcript', type=str, 
                         help='specific transcript id; if not given, \
                         whole transcript will return')
 parser_cds.add_argument('-o', '--output', type=str, 
                         help='output file path')
 parser_cds.add_argument('-p', '--print', action="store_true", 
                         help='output to stdout')
+parser_cds.add_argument('-r', '--rna_feature', choices=['mRNA', 'all'], default='mRNA',
+                         help='The type of RNA used to extract CDS, (default: mRNA)')
 parser_cds.add_argument('-t', '--output_format', type=str, choices=['csv','fasta'],
                          help = 'output format')
 parser_cds.add_argument('-s', '--style', choices=['GFF','GTF'], 
                         help = 'GTF database or GFF database')
 parser_cds.set_defaults(func=CDS)
 
 # dORF subcommand 
@@ -371,10 +380,14 @@
 parser_intron.add_argument('-s', '--style', choices=['GFF','GTF'], 
                            help = 'GTF database or GFF database')
 parser_intron.set_defaults(func=intron)
 
 
 args = parser.parse_args()
 # print('[%s runing ...]'%(time.strftime("%a %b %d %H:%M:%S %Y", time.localtime())))
+# pool = multiprocessing.Pool(4)
+# pool.apply_async(func=args.func, args=args)
+# pool.close()
+# pool.join()
 args.func(args)
 # print('[%s finished ...]'%(time.strftime("%a %b %d %H:%M:%S %Y", time.localtime())))
```

### Comparing `featurExtract-0.2.5.4/featurExtract/genBank_extract.py` & `featurExtract-0.2.5.5/featurExtract/genBank_extract.py`

 * *Files identical despite different names*

### Comparing `featurExtract-0.2.5.4/featurExtract/parameter.py` & `featurExtract-0.2.5.5/featurExtract/parameter.py`

 * *Files identical despite different names*

### Comparing `featurExtract-0.2.5.4/featurExtract/utils/util.py` & `featurExtract-0.2.5.5/featurExtract/utils/util.py`

 * *Files identical despite different names*

### Comparing `featurExtract-0.2.5.4/featurExtract/utils/visualize.py` & `featurExtract-0.2.5.5/featurExtract/utils/visualize.py`

 * *Files identical despite different names*

### Comparing `featurExtract-0.2.5.4/featurExtract.egg-info/PKG-INFO` & `featurExtract-0.2.5.5/featurExtract.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurExtract
-Version: 0.2.5.4
+Version: 0.2.5.5
 Summary: Extract genome ferature sequence for biologists
 Home-page: https://github.com/SitaoZ/featurExtract.git
 Author: zhusitao
 Author-email: zhusitao1990@163.com
 License: MIT
 Keywords: genome feature,extract
 Platform: UNKNOWN
```

### Comparing `featurExtract-0.2.5.4/featurExtract.egg-info/SOURCES.txt` & `featurExtract-0.2.5.5/featurExtract.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -26,12 +26,13 @@
 featurExtract/commands/extract_intron.py
 featurExtract/commands/extract_mRNA.py
 featurExtract/commands/extract_promoter.py
 featurExtract/commands/extract_rRNA.py
 featurExtract/commands/extract_tRNA.py
 featurExtract/commands/extract_terminator.py
 featurExtract/commands/extract_uORF.py
+featurExtract/commands/extract_uORF_back.py
 featurExtract/database/database.py
 featurExtract/utils/__init__.py
 featurExtract/utils/coverage.py
 featurExtract/utils/util.py
 featurExtract/utils/visualize.py
```

### Comparing `featurExtract-0.2.5.4/setup.py` & `featurExtract-0.2.5.5/setup.py`

 * *Files identical despite different names*

