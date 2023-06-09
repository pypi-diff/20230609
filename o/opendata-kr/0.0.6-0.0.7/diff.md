# Comparing `tmp/opendata_kr-0.0.6-py3-none-any.whl.zip` & `tmp/opendata_kr-0.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 14804 bytes, number of entries: 7
--rw-r--r--  2.0 unx       21 b- defN 23-Jun-08 15:03 opendata/__init__.py
--rw-r--r--  2.0 unx     3859 b- defN 23-Jun-08 15:05 opendata/dataset.py
--rw-r--r--  2.0 unx    34523 b- defN 23-Jun-08 15:13 opendata_kr-0.0.6.dist-info/LICENSE
--rw-r--r--  2.0 unx      478 b- defN 23-Jun-08 15:13 opendata_kr-0.0.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-08 15:13 opendata_kr-0.0.6.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Jun-08 15:13 opendata_kr-0.0.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      556 b- defN 23-Jun-08 15:13 opendata_kr-0.0.6.dist-info/RECORD
-7 files, 39538 bytes uncompressed, 13814 bytes compressed:  65.1%
+Zip file size: 14834 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       21 b- defN 23-Jun-09 08:57 opendata/__init__.py
+-rw-r--r--  2.0 unx     3784 b- defN 23-Jun-09 08:55 opendata/dataset.py
+-rw-r--r--  2.0 unx    34523 b- defN 23-Jun-09 09:30 opendata_kr-0.0.7.dist-info/LICENSE
+-rw-r--r--  2.0 unx      522 b- defN 23-Jun-09 09:30 opendata_kr-0.0.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-09 09:30 opendata_kr-0.0.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Jun-09 09:30 opendata_kr-0.0.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      556 b- defN 23-Jun-09 09:30 opendata_kr-0.0.7.dist-info/RECORD
+7 files, 39507 bytes uncompressed, 13844 bytes compressed:  65.0%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: opendata/__init__.py
 Comment: 
 
 Filename: opendata/dataset.py
 Comment: 
 
-Filename: opendata_kr-0.0.6.dist-info/LICENSE
+Filename: opendata_kr-0.0.7.dist-info/LICENSE
 Comment: 
 
-Filename: opendata_kr-0.0.6.dist-info/METADATA
+Filename: opendata_kr-0.0.7.dist-info/METADATA
 Comment: 
 
-Filename: opendata_kr-0.0.6.dist-info/WHEEL
+Filename: opendata_kr-0.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: opendata_kr-0.0.6.dist-info/top_level.txt
+Filename: opendata_kr-0.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: opendata_kr-0.0.6.dist-info/RECORD
+Filename: opendata_kr-0.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## opendata/__init__.py

```diff
@@ -1 +1 @@
-__version__ = '0.0.6'
+__version__ = '0.0.7'
```

## opendata/dataset.py

```diff
@@ -10,27 +10,27 @@
         self.name = name
         self.desc = desc
         self.data_dir = data_dir
         self.id = _id
         self.alt_url = alt_url
         
         # Dropbox Dataset
-        self.dataset_url = 'https://www.dropbox.com/s/95wzfrmoc4qrfvw/dataset.csv?dl=1'
+        self.dataset_url = 'https://www.dropbox.com/s/dmk6sti3m254w6o/dataset.csv?dl=1'
         if alt_url:
             # Jaen Dataset
             self.dataset_url = 'http://data.jaen.kr/download?download_path=%2Fdata%2Ffiles%2FmySUNI%2Fdatasets%2F000-metadata%2Fdataset.csv'
 
         # data 폴더 생성
         if not os.path.exists(data_dir):
             os.makedirs(data_dir)
 
         self.load_metadata()
 
     def load_metadata(self):
-        metadata_url = 'https://www.dropbox.com/s/9y1nyvwy95jh2w3/metadata.csv?dl=1'
+        metadata_url = 'https://www.dropbox.com/s/gjeoilz9bm8lzgg/metadata.csv?dl=1'
         cols = ['filename', 'url']
         if self.alt_url:
             metadata_url = 'http://data.jaen.kr/download?download_path=%2Fdata%2Ffiles%2FmySUNI%2Fdatasets%2F000-metadata%2Fmetadata.csv'
             cols = ['filename', 'alt_url']
             
         metadata = pd.read_csv(metadata_url)
         self.meta = {i: v for i, v in metadata.loc[metadata['id'] == self.id, cols].values}
@@ -76,17 +76,14 @@
         print('\n======= 다운로드 완료 =======')
 
 
 def list(alt_url=True):
     download_url = 'https://www.dropbox.com/s/95wzfrmoc4qrfvw/dataset.csv?dl=1'
     if alt_url:
         download_url = 'http://data.jaen.kr/download?download_path=%2Fdata%2Ffiles%2FmySUNI%2Fdatasets%2F000-metadata%2Fdataset.csv'
-        print('[서버] Jaen')
-    else:
-        print('[서버] Dropbox')
     print(download_url)
     ret = pd.read_csv(download_url).iloc[:, :-1]
     ret.columns = ['데이터셋', '설명']
     return ret
 
 
 def download(name, data_dir='data', alt_url=True, path=None):
```

## Comparing `opendata_kr-0.0.6.dist-info/LICENSE` & `opendata_kr-0.0.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `opendata_kr-0.0.6.dist-info/RECORD` & `opendata_kr-0.0.7.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-opendata/__init__.py,sha256=UwR0idQSHgdEemLAk-o2bPOXYWCj-lyyQzAPFRLbziA,21
-opendata/dataset.py,sha256=Z2ss_W3MWwiIJyOardVZdUAW_akmDL0A-i2GeZOaZOY,3859
-opendata_kr-0.0.6.dist-info/LICENSE,sha256=hIahDEOTzuHCU5J2nd07LWwkLW7Hko4UFO__ffsvB-8,34523
-opendata_kr-0.0.6.dist-info/METADATA,sha256=9Z5VBiFYhpbLve9bjrswOm2CDkJkgQsFa7Xla_5Cu8E,478
-opendata_kr-0.0.6.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-opendata_kr-0.0.6.dist-info/top_level.txt,sha256=zm6NENMGEU6mTNYYZtZF6gTZnerfLvzpWpzTXehqxCQ,9
-opendata_kr-0.0.6.dist-info/RECORD,,
+opendata/__init__.py,sha256=7sNbee72r3qCAVloFm2RRWCTa9gVjMS7nCJcJ-URzl4,21
+opendata/dataset.py,sha256=C5XWEhlafRCPQnShmwsTPlFDToUHGaAv3Xw2lkg2nlQ,3784
+opendata_kr-0.0.7.dist-info/LICENSE,sha256=hIahDEOTzuHCU5J2nd07LWwkLW7Hko4UFO__ffsvB-8,34523
+opendata_kr-0.0.7.dist-info/METADATA,sha256=tQWSR2g3LMd_iIZEtRauc15g75c352cxdoEc26Iu0ac,522
+opendata_kr-0.0.7.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+opendata_kr-0.0.7.dist-info/top_level.txt,sha256=zm6NENMGEU6mTNYYZtZF6gTZnerfLvzpWpzTXehqxCQ,9
+opendata_kr-0.0.7.dist-info/RECORD,,
```

