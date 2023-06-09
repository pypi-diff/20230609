# Comparing `tmp/xalign-0.1.73.tar.gz` & `tmp/xalign-0.1.74.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xalign-0.1.73.tar", last modified: Wed Jun  7 15:08:50 2023, max compression
+gzip compressed data, was "xalign-0.1.74.tar", last modified: Fri Jun  9 14:18:30 2023, max compression
```

## Comparing `xalign-0.1.73.tar` & `xalign-0.1.74.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-06-07 15:08:50.684989 xalign-0.1.73/
--rw-r--r--   0 maayanlab   (501) staff       (20)    11357 2022-09-01 19:41:23.000000 xalign-0.1.73/LICENSE
--rw-r--r--   0 maayanlab   (501) staff       (20)     4802 2023-06-07 15:08:50.684666 xalign-0.1.73/PKG-INFO
--rw-r--r--   0 maayanlab   (501) staff       (20)     4351 2022-09-01 19:41:23.000000 xalign-0.1.73/README.md
--rw-r--r--   0 maayanlab   (501) staff       (20)       38 2023-06-07 15:08:50.685106 xalign-0.1.73/setup.cfg
--rw-r--r--   0 maayanlab   (501) staff       (20)      934 2022-09-02 00:43:23.000000 xalign-0.1.73/setup.py
-drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-06-07 15:08:50.676013 xalign-0.1.73/xalign/
--rw-r--r--   0 maayanlab   (501) staff       (20)     9303 2022-09-02 00:40:28.000000 xalign-0.1.73/xalign/__init__.py
-drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-06-07 15:08:50.680717 xalign-0.1.73/xalign/data/
--rw-r--r--   0 maayanlab   (501) staff       (20)       77 2022-09-01 19:41:23.000000 xalign-0.1.73/xalign/data/config.json
--rw-r--r--   0 maayanlab   (501) staff       (20)  1974007 2022-09-01 19:41:23.000000 xalign-0.1.73/xalign/data/fasterq-dump.tar.gz
--rw-r--r--   0 maayanlab   (501) staff       (20)  4083396 2022-09-01 19:41:23.000000 xalign-0.1.73/xalign/data/fasterq.tar.gz
--rw-r--r--   0 maayanlab   (501) staff       (20)     4538 2022-09-02 00:28:21.000000 xalign-0.1.73/xalign/ensembl.py
--rw-r--r--   0 maayanlab   (501) staff       (20)     1031 2022-09-01 23:44:17.000000 xalign-0.1.73/xalign/file.py
--rw-r--r--   0 maayanlab   (501) staff       (20)     1345 2022-09-01 19:41:23.000000 xalign-0.1.73/xalign/sra.py
--rw-r--r--   0 maayanlab   (501) staff       (20)     1236 2022-09-01 19:41:23.000000 xalign-0.1.73/xalign/utils.py
-drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-06-07 15:08:50.676877 xalign-0.1.73/xalign.egg-info/
--rw-r--r--   0 maayanlab   (501) staff       (20)     4802 2023-06-07 15:08:50.000000 xalign-0.1.73/xalign.egg-info/PKG-INFO
--rw-r--r--   0 maayanlab   (501) staff       (20)      340 2023-06-07 15:08:50.000000 xalign-0.1.73/xalign.egg-info/SOURCES.txt
--rw-r--r--   0 maayanlab   (501) staff       (20)        1 2023-06-07 15:08:50.000000 xalign-0.1.73/xalign.egg-info/dependency_links.txt
--rw-r--r--   0 maayanlab   (501) staff       (20)       65 2023-06-07 15:08:50.000000 xalign-0.1.73/xalign.egg-info/requires.txt
--rw-r--r--   0 maayanlab   (501) staff       (20)        7 2023-06-07 15:08:50.000000 xalign-0.1.73/xalign.egg-info/top_level.txt
+drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-06-09 14:18:30.539529 xalign-0.1.74/
+-rw-r--r--   0 maayanlab   (501) staff       (20)    11357 2022-09-01 19:41:23.000000 xalign-0.1.74/LICENSE
+-rw-r--r--   0 maayanlab   (501) staff       (20)      107 2023-06-09 14:18:14.000000 xalign-0.1.74/MANIFEST.in
+-rw-r--r--   0 maayanlab   (501) staff       (20)     4802 2023-06-09 14:18:30.539296 xalign-0.1.74/PKG-INFO
+-rw-r--r--   0 maayanlab   (501) staff       (20)     4351 2022-09-01 19:41:23.000000 xalign-0.1.74/README.md
+-rw-r--r--   0 maayanlab   (501) staff       (20)       38 2023-06-09 14:18:30.539592 xalign-0.1.74/setup.cfg
+-rw-r--r--   0 maayanlab   (501) staff       (20)      935 2023-06-09 13:45:01.000000 xalign-0.1.74/setup.py
+drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-06-09 14:18:30.534116 xalign-0.1.74/xalign/
+-rw-r--r--   0 maayanlab   (501) staff       (20)     9916 2023-06-08 14:17:05.000000 xalign-0.1.74/xalign/__init__.py
+drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-06-09 14:18:30.536888 xalign-0.1.74/xalign/data/
+-rw-r--r--   0 maayanlab   (501) staff       (20)       77 2022-09-01 19:41:23.000000 xalign-0.1.74/xalign/data/config.json
+-rw-r--r--   0 maayanlab   (501) staff       (20)  1974007 2022-09-01 19:41:23.000000 xalign-0.1.74/xalign/data/fasterq-dump.tar.gz
+-rw-r--r--   0 maayanlab   (501) staff       (20)  4083396 2022-09-01 19:41:23.000000 xalign-0.1.74/xalign/data/fasterq.tar.gz
+-rw-r--r--   0 maayanlab   (501) staff       (20)     6999 2023-06-09 13:32:34.000000 xalign-0.1.74/xalign/ensembl.py
+-rw-r--r--   0 maayanlab   (501) staff       (20)     1031 2022-09-01 23:44:17.000000 xalign-0.1.74/xalign/file.py
+-rw-r--r--   0 maayanlab   (501) staff       (20)     1345 2022-09-01 19:41:23.000000 xalign-0.1.74/xalign/sra.py
+-rw-r--r--   0 maayanlab   (501) staff       (20)     1236 2022-09-01 19:41:23.000000 xalign-0.1.74/xalign/utils.py
+drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-06-09 14:18:30.534832 xalign-0.1.74/xalign.egg-info/
+-rw-r--r--   0 maayanlab   (501) staff       (20)     4802 2023-06-09 14:18:30.000000 xalign-0.1.74/xalign.egg-info/PKG-INFO
+-rw-r--r--   0 maayanlab   (501) staff       (20)      352 2023-06-09 14:18:30.000000 xalign-0.1.74/xalign.egg-info/SOURCES.txt
+-rw-r--r--   0 maayanlab   (501) staff       (20)        1 2023-06-09 14:18:30.000000 xalign-0.1.74/xalign.egg-info/dependency_links.txt
+-rw-r--r--   0 maayanlab   (501) staff       (20)       65 2023-06-09 14:18:30.000000 xalign-0.1.74/xalign.egg-info/requires.txt
+-rw-r--r--   0 maayanlab   (501) staff       (20)        7 2023-06-09 14:18:30.000000 xalign-0.1.74/xalign.egg-info/top_level.txt
```

### Comparing `xalign-0.1.73/LICENSE` & `xalign-0.1.74/LICENSE`

 * *Files identical despite different names*

### Comparing `xalign-0.1.73/PKG-INFO` & `xalign-0.1.74/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xalign
-Version: 0.1.73
+Version: 0.1.74
 Summary: Alignment in a python wrapper.
 Home-page: https://github.com/maayanlab/xalign
 Author: Alexander Lachmann
 Author-email: alexander.lachmann@mssm.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `xalign-0.1.73/README.md` & `xalign-0.1.74/README.md`

 * *Files identical despite different names*

### Comparing `xalign-0.1.73/setup.py` & `xalign-0.1.74/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="xalign",
-    version="0.1.73",
+    version="0.1.74",
     author="Alexander Lachmann",
     author_email="alexander.lachmann@mssm.edu",
     description="Alignment in a python wrapper.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/maayanlab/xalign",
     packages=setuptools.find_packages(),
@@ -26,11 +26,11 @@
         'pandas',
         'numpy',
         'scikit-learn',
         'progress',
         'loess',
         'tqdm',
         'statsmodels',
-        'mygene'
+        'mygene',
     ],
     python_requires='>=3.6',
 )
```

### Comparing `xalign-0.1.73/xalign/__init__.py` & `xalign-0.1.74/xalign/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,49 +10,50 @@
 
 import xalign.file as filehandler
 import xalign.ensembl as ensembl
 import xalign.sra as sra
 from xalign.ensembl import retrieve_ensembl_organisms, organism_display_to_name
 from xalign.utils import file_pairs
 
-def build_index(aligner: str, species: str, noncoding=False, overwrite=False, verbose=False):
-    organisms = ensembl.retrieve_ensembl_organisms()
+def build_index(aligner: str, species: str, release=None, noncoding=False, overwrite=False, verbose=False):
+    organisms = ensembl.retrieve_ensembl_organisms(str(release))
     if species in organisms:
         if verbose:
             print("Download fastq.gz")
             print(filehandler.get_data_path())
-        filehandler.download_file(organisms[species][2], species+".fastq.gz", overwrite=overwrite, verbose=False)
+        filehandler.download_file(organisms[species][2], species+"."+str(release)+".fastq.gz", overwrite=overwrite, verbose=False)
         if noncoding:
-            filehandler.download_file(organisms[species][4], species+".nc.fastq.gz", overwrite=overwrite, verbose=False)
+            filehandler.download_file(organisms[species][4], species+"."+str(release)+".nc.fastq.gz", overwrite=overwrite, verbose=False)
             if aligner == "kallisto":
-                if (not os.path.exists(filehandler.get_data_path()+"index/kallisto_"+species+".idx")) or overwrite:
-                    filehandler.concat(species+".fastq.gz", species+".nc.fastq.gz", verbose=verbose)
+                if (not os.path.exists(filehandler.get_data_path()+"index/"+str(release)+"/kallisto_"+species+".idx")) or overwrite:
+                    filehandler.concat(species+"."+str(release)+".fastq.gz", species+"."+str(release)+".nc.fastq.gz", verbose=verbose)
             elif aligner == "salmon":
-                if (not os.path.exists(filehandler.get_data_path()+"index/salmon_"+species)) or overwrite:
-                    filehandler.concat(species+".fastq.gz", species+".nc.fastq.gz", verbose=verbose)
+                if (not os.path.exists(filehandler.get_data_path()+"index/"+str(release)+"/salmon_"+species)) or overwrite:
+                    filehandler.concat(species+"."+str(release)+".fastq.gz", species+"."+str(release)+".nc.fastq.gz", verbose=verbose)
     else:
         print("Species not found in the Ensembl database")
         sys.exit(0)
     osys = platform.system().lower()
     download_aligner(aligner, osys)
     os.makedirs(filehandler.get_data_path()+"/index", exist_ok=True)
+    os.makedirs(filehandler.get_data_path()+"/index/"+str(release), exist_ok=True)
     if aligner == "kallisto":
-        if (not os.path.exists(filehandler.get_data_path()+"index/kallisto_"+species+".idx")) or overwrite:
+        if (not os.path.exists(filehandler.get_data_path()+"index/"+str(str(release))+"/kallisto_"+species+".idx")) or overwrite:
             if verbose:
                 print("Build kallisto index for "+species)
-            os.system(filehandler.get_data_path()+"kallisto/kallisto index -i "+filehandler.get_data_path()+"index/kallisto_"+species+".idx "+filehandler.get_data_path()+species+".fastq.gz")
+            os.system(filehandler.get_data_path()+"kallisto/kallisto index -i "+filehandler.get_data_path()+"index/"+str(release)+"/kallisto_"+species+".idx "+filehandler.get_data_path()+species+"."+str(release)+".fastq.gz")
         else:
             if verbose:
                 print("Index already exists. Use overwrite to rebuild.")
     elif aligner == "salmon":
         if (not os.path.exists(filehandler.get_data_path()+"index/salmon_"+species)) or overwrite:
             if verbose:
                 print("Build salmon index for "+species)
-                print(filehandler.get_data_path()+"salmon-1.5.2_linux_x86_64/bin index -i "+filehandler.get_data_path()+"index/salmon_"+species+".idx -t "+filehandler.get_data_path()+species+".fastq.gz")
-            os.system(filehandler.get_data_path()+"salmon-1.5.2_linux_x86_64/bin/salmon index -i "+filehandler.get_data_path()+"index/salmon_"+species+" -t "+filehandler.get_data_path()+species+".fastq.gz")
+                print(filehandler.get_data_path()+"salmon-1.5.2_linux_x86_64/bin index -i "+filehandler.get_data_path()+"index/"+str(str(release))+"/salmon_"+species+".idx -t "+filehandler.get_data_path()+species+"."+str(release)+".fastq.gz")
+            os.system(filehandler.get_data_path()+"salmon-1.5.2_linux_x86_64/bin/salmon index -i "+filehandler.get_data_path()+"index/"+str(str(release))+"/salmon_"+species+" -t "+filehandler.get_data_path()+species+"."+str(release)+".fastq.gz")
         else:
             if verbose:
                 print("Index already exists. Use overwrite to rebuild.")
 
 def download_aligner(aligner, osys, verbose=False):
     if verbose:
         print(osys)
@@ -92,69 +93,71 @@
             filepath = filehandler.download_file(url, "kallisto.tar.gz")
             file = tarfile.open(filepath)
             file.extract('kallisto/kallisto', filehandler.get_data_path())
             file.close()
     elif aligner == "hisat2":
         print("missing")
 
-def align_fastq(species, fastq, aligner="kallisto", t=1, noncoding=False, overwrite=False, verbose=False):
+def align_fastq(species, fastq, aligner="kallisto", t=1, release=None, noncoding=False, overwrite=False, verbose=False):
     if isinstance(fastq, str):
         fastq = [fastq]
-    build_index(aligner, species, noncoding=noncoding, overwrite=overwrite, verbose=verbose)
+    if not release:
+        release = list(ensembl.retrieve_ensembl_organisms(release).items())[0][1][5]
+    build_index(aligner, species, release=release, noncoding=noncoding, overwrite=overwrite, verbose=verbose)
     if aligner == "kallisto":
         if len(fastq) == 1:
             if verbose:
                 print("Align with kallisto (single strand).")
-            res = subprocess.Popen(filehandler.get_data_path()+"kallisto/kallisto quant -i "+filehandler.get_data_path()+"index/kallisto_"+species+".idx -t "+str(t)+" -o "+filehandler.get_data_path()+"outkallisto --single -l 200 -s 20 "+fastq[0], stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True)
+            res = subprocess.Popen(filehandler.get_data_path()+"kallisto/kallisto quant -i "+filehandler.get_data_path()+"index/"+str(release)+"/kallisto_"+species+".idx -t "+str(t)+" -o "+filehandler.get_data_path()+"outkallisto --single -l 200 -s 20 "+fastq[0], stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True)
         else:
             if verbose:
                 print("Align with kallisto (paired).")
-            res = subprocess.Popen(filehandler.get_data_path()+"kallisto/kallisto quant -i "+filehandler.get_data_path()+"index/kallisto_"+species+".idx -t "+str(t)+" -o "+filehandler.get_data_path()+"outkallisto "+fastq[0]+" "+fastq[1], stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True)
+            res = subprocess.Popen(filehandler.get_data_path()+"kallisto/kallisto quant -i "+filehandler.get_data_path()+"index/"+str(release)+"/kallisto_"+species+".idx -t "+str(t)+" -o "+filehandler.get_data_path()+"outkallisto "+fastq[0]+" "+fastq[1], stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True)
         if res.wait() != 0:
             output, error = res.communicate()
             if verbose:
                 print(output)
             print(error)
     elif aligner == "salmon":
         if len(fastq) == 1:
             print("Align with salmon (single).")
-            res = subprocess.Popen(filehandler.get_data_path()+"salmon-1.5.2_linux_x86_64/bin/salmon quant -i "+filehandler.get_data_path()+"index/salmon_"+species+" -l A -r "+fastq[0]+" -p "+str(t)+" --validateMappings -o "+filehandler.get_data_path()+"outsalmon", stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True)
+            res = subprocess.Popen(filehandler.get_data_path()+"salmon-1.5.2_linux_x86_64/bin/salmon quant -i "+filehandler.get_data_path()+"index/"+str(release)+"/salmon_"+species+" -l A -r "+fastq[0]+" -p "+str(t)+" --validateMappings -o "+filehandler.get_data_path()+"outsalmon", stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True)
             if res.wait() != 0:
                 output, error = res.communicate()
                 print(error)
                 if verbose:
                     print(output)
         else:
             print("Align with salmon (paired).")
-            res = subprocess.Popen(filehandler.get_data_path()+"salmon-1.5.2_linux_x86_64/bin/salmon quant -i "+filehandler.get_data_path()+"index/salmon_"+species+" -l A -1 "+fastq[0]+" -2 "+fastq[1]+" -p "+str(t)+" -o "+filehandler.get_data_path()+"outsalmon", stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True)
+            res = subprocess.Popen(filehandler.get_data_path()+"salmon-1.5.2_linux_x86_64/bin/salmon quant -i "+filehandler.get_data_path()+"index/"+str(release)+"/salmon_"+species+" -l A -1 "+fastq[0]+" -2 "+fastq[1]+" -p "+str(t)+" -o "+filehandler.get_data_path()+"outsalmon", stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True)
             if res.wait() != 0:
                 output, error = res.communicate()
                 print(error)
                 if verbose:
                     print(output)
     elif aligner == "hisat2":
         print("align with hisat2")
     
     return read_result(aligner)
 
-def align_folder(species, folder, aligner="kallisto",  t=1, identifier="symbol", noncoding=False, overwrite=False, verbose=False):
+def align_folder(species, folder, aligner="kallisto", t=1, release=None, identifier="symbol", noncoding=False, overwrite=False, verbose=False):
     fastq_files = file_pairs(folder)
     gene_counts = []
     transcript_counts = []
     pbar = tqdm(total=len(fastq_files))
     pbar.set_description("Aligning samples")
     sample_names = []
     for fq in fastq_files:
         if fq[0] == "" or fq[1] == "":
             fq.remove("")
             sample_names.append(fq[0])
         else:
             bnames = [os.path.basename(x) for x in fq]
             sample_names.append(re.sub(r'_$','',os.path.commonprefix(bnames)))
-        res = align_fastq(species, fq, aligner=aligner, t=t, noncoding=noncoding, overwrite=overwrite, verbose=verbose)
+        res = align_fastq(species, fq, aligner=aligner, t=t, release=release, noncoding=noncoding, overwrite=overwrite, verbose=verbose)
         transcript_counts.append(list(res.loc[:,"reads"].round()))
         res_gene = ensembl.agg_gene_counts(res, species, identifier=identifier, overwrite=overwrite)
         gene_counts.append(list(res_gene.loc[:,"counts"].round()))
         overwrite=False
         pbar.update(1)
     transcript_counts = pd.DataFrame(transcript_counts, columns=res.iloc[:,0], index=sample_names).T.astype("int")
     gene_counts = pd.DataFrame(gene_counts, columns=res_gene.iloc[:,0], index=sample_names).T.astype("int")
```

### Comparing `xalign-0.1.73/xalign/data/fasterq-dump.tar.gz` & `xalign-0.1.74/xalign/data/fasterq-dump.tar.gz`

 * *Files identical despite different names*

### Comparing `xalign-0.1.73/xalign/data/fasterq.tar.gz` & `xalign-0.1.74/xalign/data/fasterq.tar.gz`

 * *Files identical despite different names*

### Comparing `xalign-0.1.73/xalign/file.py` & `xalign-0.1.74/xalign/file.py`

 * *Files identical despite different names*

### Comparing `xalign-0.1.73/xalign/sra.py` & `xalign-0.1.74/xalign/sra.py`

 * *Files identical despite different names*

### Comparing `xalign-0.1.73/xalign/utils.py` & `xalign-0.1.74/xalign/utils.py`

 * *Files identical despite different names*

### Comparing `xalign-0.1.73/xalign.egg-info/PKG-INFO` & `xalign-0.1.74/xalign.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xalign
-Version: 0.1.73
+Version: 0.1.74
 Summary: Alignment in a python wrapper.
 Home-page: https://github.com/maayanlab/xalign
 Author: Alexander Lachmann
 Author-email: alexander.lachmann@mssm.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

