# Comparing `tmp/foundation_cancer_image_biomarker-0.0.1a2.tar.gz` & `tmp/foundation_cancer_image_biomarker-0.0.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foundation_cancer_image_biomarker-0.0.1a2.tar", max compression
+gzip compressed data, was "foundation_cancer_image_biomarker-0.0.1a3.tar", max compression
```

## Comparing `foundation_cancer_image_biomarker-0.0.1a2.tar` & `foundation_cancer_image_biomarker-0.0.1a3.tar`

### file list

```diff
@@ -1,15 +1,32 @@
--rw-r--r--   0        0        0     1076 2023-06-04 18:03:55.694363 foundation_cancer_image_biomarker-0.0.1a2/LICENSE
--rw-r--r--   0        0        0     4911 2023-06-06 01:33:53.653635 foundation_cancer_image_biomarker-0.0.1a2/README.md
--rw-r--r--   0        0        0      516 2023-06-04 18:03:55.674363 foundation_cancer_image_biomarker-0.0.1a2/fmcib/__init__.py
--rw-r--r--   0        0        0       31 2023-06-06 01:43:30.477335 foundation_cancer_image_biomarker-0.0.1a2/fmcib/models/__init__.py
--rw-r--r--   0        0        0      767 2023-06-06 01:43:30.497334 foundation_cancer_image_biomarker-0.0.1a2/fmcib/models/resnet50.py
--rw-r--r--   0        0        0     1437 2023-06-06 01:43:30.521334 foundation_cancer_image_biomarker-0.0.1a2/fmcib/preprocessing/__init__.py
--rw-r--r--   0        0        0     4283 2023-06-06 01:43:30.549334 foundation_cancer_image_biomarker-0.0.1a2/fmcib/preprocessing/seed_based_crop.py
--rw-r--r--   0        0        0      943 2023-06-06 01:43:30.505334 foundation_cancer_image_biomarker-0.0.1a2/fmcib/run.py
--rw-r--r--   0        0        0       67 2023-06-06 01:43:30.477335 foundation_cancer_image_biomarker-0.0.1a2/fmcib/utils/__init__.py
--rw-r--r--   0        0        0      367 2023-06-06 01:43:30.485334 foundation_cancer_image_biomarker-0.0.1a2/fmcib/utils/download_utils.py
--rw-r--r--   0        0        0     3459 2023-06-06 02:43:50.493404 foundation_cancer_image_biomarker-0.0.1a2/fmcib/utils/idc_helper.py
--rw-r--r--   0        0        0       44 2023-06-06 01:43:30.477335 foundation_cancer_image_biomarker-0.0.1a2/fmcib/visualization/__init__.py
--rw-r--r--   0        0        0      499 2023-06-06 01:41:36.682184 foundation_cancer_image_biomarker-0.0.1a2/fmcib/visualization/verify_io.py
--rw-r--r--   0        0        0     4149 2023-06-06 03:10:02.917392 foundation_cancer_image_biomarker-0.0.1a2/pyproject.toml
--rw-r--r--   0        0        0     6288 1970-01-01 00:00:00.000000 foundation_cancer_image_biomarker-0.0.1a2/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-06-04 18:03:55.694363 foundation_cancer_image_biomarker-0.0.1a3/LICENSE
+-rw-r--r--   0        0        0    27254 2023-06-09 09:53:08.816608 foundation_cancer_image_biomarker-0.0.1a3/README.md
+-rw-r--r--   0        0        0       23 2023-06-09 09:55:32.943580 foundation_cancer_image_biomarker-0.0.1a3/fmcib/__init__.py
+-rw-r--r--   0        0        0       45 2023-06-09 08:53:45.238232 foundation_cancer_image_biomarker-0.0.1a3/fmcib/callbacks/__init__.py
+-rw-r--r--   0        0        0     2188 2023-06-09 07:25:30.580753 foundation_cancer_image_biomarker-0.0.1a3/fmcib/callbacks/prediction_saver.py
+-rw-r--r--   0        0        0      403 2023-06-09 07:24:26.381203 foundation_cancer_image_biomarker-0.0.1a3/fmcib/callbacks/utils.py
+-rw-r--r--   0        0        0       54 2023-06-09 09:10:44.118566 foundation_cancer_image_biomarker-0.0.1a3/fmcib/datasets/__init__.py
+-rw-r--r--   0        0        0     5353 2023-06-09 05:43:21.136415 foundation_cancer_image_biomarker-0.0.1a3/fmcib/datasets/ssl_radiomics_dataset.py
+-rw-r--r--   0        0        0     2365 2023-06-08 04:18:19.159890 foundation_cancer_image_biomarker-0.0.1a3/fmcib/datasets/utils.py
+-rw-r--r--   0        0        0       31 2023-06-06 01:43:30.477335 foundation_cancer_image_biomarker-0.0.1a3/fmcib/models/__init__.py
+-rw-r--r--   0        0        0      767 2023-06-09 06:28:56.871613 foundation_cancer_image_biomarker-0.0.1a3/fmcib/models/resnet50.py
+-rw-r--r--   0        0        0     1437 2023-06-06 01:43:30.521334 foundation_cancer_image_biomarker-0.0.1a3/fmcib/preprocessing/__init__.py
+-rw-r--r--   0        0        0     4283 2023-06-06 01:43:30.549334 foundation_cancer_image_biomarker-0.0.1a3/fmcib/preprocessing/seed_based_crop.py
+-rw-r--r--   0        0        0      943 2023-06-06 01:43:30.505334 foundation_cancer_image_biomarker-0.0.1a3/fmcib/run.py
+-rw-r--r--   0        0        0        0 2023-06-08 02:44:13.386481 foundation_cancer_image_biomarker-0.0.1a3/fmcib/ssl/__init__.py
+-rw-r--r--   0        0        0       54 2023-06-08 02:48:18.036638 foundation_cancer_image_biomarker-0.0.1a3/fmcib/ssl/losses/__init__.py
+-rw-r--r--   0        0        0     3348 2023-06-08 02:44:38.830290 foundation_cancer_image_biomarker-0.0.1a3/fmcib/ssl/losses/ntxent_mined_loss.py
+-rw-r--r--   0        0        0       96 2023-06-08 05:19:10.855520 foundation_cancer_image_biomarker-0.0.1a3/fmcib/ssl/models/__init__.py
+-rw-r--r--   0        0        0      671 2023-06-08 02:45:52.657736 foundation_cancer_image_biomarker-0.0.1a3/fmcib/ssl/models/exneg_simclr.py
+-rw-r--r--   0        0        0     2074 2023-06-09 09:04:10.961477 foundation_cancer_image_biomarker-0.0.1a3/fmcib/ssl/models/load_pretrained_resnet.py
+-rw-r--r--   0        0        0       22 2023-06-08 02:45:31.477895 foundation_cancer_image_biomarker-0.0.1a3/fmcib/ssl/optimizers/__init__.py
+-rw-r--r--   0        0        0     5397 2023-06-08 02:45:31.565894 foundation_cancer_image_biomarker-0.0.1a3/fmcib/ssl/optimizers/lars.py
+-rw-r--r--   0        0        0       85 2023-06-08 04:47:26.794430 foundation_cancer_image_biomarker-0.0.1a3/fmcib/ssl/transforms/__init__.py
+-rw-r--r--   0        0        0     1414 2023-06-08 04:47:13.370533 foundation_cancer_image_biomarker-0.0.1a3/fmcib/ssl/transforms/duplicate.py
+-rw-r--r--   0        0        0     1313 2023-06-08 04:44:35.583740 foundation_cancer_image_biomarker-0.0.1a3/fmcib/ssl/transforms/random_resized_crop.py
+-rw-r--r--   0        0        0       67 2023-06-06 01:43:30.477335 foundation_cancer_image_biomarker-0.0.1a3/fmcib/utils/__init__.py
+-rw-r--r--   0        0        0      367 2023-06-06 01:43:30.485334 foundation_cancer_image_biomarker-0.0.1a3/fmcib/utils/download_utils.py
+-rw-r--r--   0        0        0     3419 2023-06-09 09:21:27.165850 foundation_cancer_image_biomarker-0.0.1a3/fmcib/utils/idc_helper.py
+-rw-r--r--   0        0        0       44 2023-06-06 01:43:30.477335 foundation_cancer_image_biomarker-0.0.1a3/fmcib/visualization/__init__.py
+-rw-r--r--   0        0        0      499 2023-06-06 01:41:36.682184 foundation_cancer_image_biomarker-0.0.1a3/fmcib/visualization/verify_io.py
+-rw-r--r--   0        0        0     4201 2023-06-09 09:55:32.875581 foundation_cancer_image_biomarker-0.0.1a3/pyproject.toml
+-rw-r--r--   0        0        0    28631 1970-01-01 00:00:00.000000 foundation_cancer_image_biomarker-0.0.1a3/PKG-INFO
```

### Comparing `foundation_cancer_image_biomarker-0.0.1a2/LICENSE` & `foundation_cancer_image_biomarker-0.0.1a3/LICENSE`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-0.0.1a2/fmcib/models/resnet50.py` & `foundation_cancer_image_biomarker-0.0.1a3/fmcib/models/resnet50.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,12 +13,12 @@
 def resnet50(pretrained=True):
     logger.info("Loading pretrained foundation model (Resnet50) ...")
 
     model = resnet50_monai(pretrained=False, n_input_channels=1, widen_factor=2, conv1_t_stride=2, feed_forward=False)
     if pretrained:
         current_path = Path(os.getcwd())
         if not (current_path / "fmcib.torch").exists():
-            wget.download("https://www.dropbox.com/s/oqzej4tjij2k4cn/fmcib.torch?dl=1", bar=bar_progress)
+            wget.download("https://www.dropbox.com/s/bd7azdsvx1jhalp/fmcib.torch?dl=1", bar=bar_progress)
 
         model.load_state_dict(torch.load(current_path / "fmcib.torch")["trunk_state_dict"])
 
     return model
```

### Comparing `foundation_cancer_image_biomarker-0.0.1a2/fmcib/preprocessing/__init__.py` & `foundation_cancer_image_biomarker-0.0.1a3/fmcib/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-0.0.1a2/fmcib/preprocessing/seed_based_crop.py` & `foundation_cancer_image_biomarker-0.0.1a3/fmcib/preprocessing/seed_based_crop.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-0.0.1a2/fmcib/run.py` & `foundation_cancer_image_biomarker-0.0.1a3/fmcib/run.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-0.0.1a2/fmcib/utils/idc_helper.py` & `foundation_cancer_image_biomarker-0.0.1a3/fmcib/utils/idc_helper.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,63 +10,60 @@
 from dcmrtstruct2nii import dcmrtstruct2nii
 from google.cloud import storage
 from loguru import logger
 from tqdm import tqdm
 
 from .download_utils import bar_progress
 
+def download_from_manifest(df, save_dir, samples):
+    # Instantiates a client
+    storage_client = storage.Client()
+    bucket = storage_client.bucket("idc-open-cr")
+    logger.info("Downloading DICOM data from IDC (Imaging Data Commons) ...")
+    (save_dir / "dicom").mkdir(exist_ok=True, parents=True)
+
+    if samples is not None:
+        assert "PatientID" in df.columns
+        unique_elements = df['PatientID'].unique()
+
+
+        selected_elements = np.random.choice(unique_elements, min(len(unique_elements), samples), replace=False)
+        df = df[df['PatientID'].isin(selected_elements)]
+
+    def download_file(row):
+        fn = f'{row["gcs_url"].split("/")[-2]}/{row["gcs_url"].split("/")[-1]}'
+        blob = bucket.blob(fn)
+
+        current_save_dir = save_dir / "dicom" / row["PatientID"] / row["StudyInstanceUID"]
+        current_save_dir.mkdir(exist_ok=True, parents=True)
+        blob.download_to_filename(str(current_save_dir / f'{row["Modality"]}_{row["SeriesInstanceUID"]}_{row["InstanceNumber"]}.dcm'))
+
 
-def download_LUNG1(path):
+    with concurrent.futures.ThreadPoolExecutor() as executor:
+        futures = []
+        for idx, row in df.iterrows():
+            futures.append(executor.submit(download_file, row))
+        for future in tqdm(concurrent.futures.as_completed(futures), total=len(futures)):
+            pass
+
+
+def download_LUNG1(path, samples=None):
     save_dir = Path(path).resolve()
     save_dir.mkdir(exist_ok=True, parents=True)
 
     logger.info("Downloading LUNG1 manifest from Dropbox ...")
     # Download LUNG1 data manifest, this is precomputed but any set of GCS dicom files can be used here
     wget.download(
-        "https://www.dropbox.com/s/tbywsmxln5yatxw/gcs_lung1_paths.txt?dl=1",
-        bar=bar_progress,
-        out=f"{save_dir}/gcs_lung1_paths.txt",
+        "https://www.dropbox.com/s/lkvv33nmepecyu5/nsclc_radiomics.csv?dl=1",
+        out=f"{save_dir}/nsclc_radiomics.csv",
     )
 
-    # Instantiates a client
-    storage_client = storage.Client()
-    bucket = storage_client.bucket("idc-open-cr")
-
-    logger.info("Downloading LUNG1 DICOM data from IDC (Imaging Data Commons) ...")
-
-    (save_dir / "dicom").mkdir(exist_ok=True, parents=True)
-
-    # The name of the file to download
-    with open(f"{save_dir}/gcs_lung1_paths.txt", "r") as f:
-        # Define a function to download a single file
-        def download_file(fn):
-            fn = fn.strip("\n")
-            # Get the generation number of the blob
-            blob = bucket.blob(fn)
-            # Generate the download URL with the generation number
-            blob.download_to_filename(f"{str(save_dir / 'dicom' / fn.split('/')[-1])}")
-
-        # Use a ThreadPoolExecutor to download multiple files in parallel
-        with concurrent.futures.ThreadPoolExecutor() as executor:
-            futures = []
-            for fn in f.readlines():
-                futures.append(executor.submit(download_file, fn))
-            for future in tqdm(concurrent.futures.as_completed(futures), total=len(futures)):
-                pass
-
-    logger.info("Sorting files using dicomsort ...")
-
-    # Sort the downloaded DICOM data
-    # DICOM sort
-    command = ["dicomsort"]
-    command += [f"{save_dir}/dicom"]
-    command += [f"{save_dir}/sorted/%PatientID/%StudyInstanceUID/%Modality_%SeriesInstanceUID_%InstanceNumber.dcm"]
-    command += ["--keepGoing"]
+    df = pd.read_csv(f"{save_dir}/nsclc_radiomics.csv")
 
-    subprocess.run(command)
+    download_from_manifest(df, save_dir, samples)
 
 
 def build_image_seed_dict(path, samples=10):
     sorted_dir = Path(path).resolve()
     series_dirs = [x.parent for x in sorted_dir.rglob("*.dcm")]
     series_dirs = sorted(list(set(series_dirs)))
```

### Comparing `foundation_cancer_image_biomarker-0.0.1a2/pyproject.toml` & `foundation_cancer_image_biomarker-0.0.1a3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "foundation-cancer-image-biomarker"
-version = "0.0.1a2"
+version = "0.0.1a3"
 description = "Official repo for Foundation Models for Quantitative Biomarker Discovery in Cancer Imaging [INSERT DOI]"
 readme = "README.md"
 authors = ["Suraj Pai <bspai@bwh.harvard.edu>"]
 license = "MIT"
 repository = "https://github.com/AIM-Harvard/foundation-cancer-image-biomarker"
 homepage = "https://aim.hms.harvard.edu/foundation-cancer-image-biomarker"
 
@@ -166,7 +166,9 @@
 """
 generated-members = "torch.*"
 
 [tool.pylint.master]
 fail-under=8
 
 [tool.poetry_bumpversion.file."version.py"]
+[tool.poetry_bumpversion.file."fmcib/__init__.py"]
+
```

