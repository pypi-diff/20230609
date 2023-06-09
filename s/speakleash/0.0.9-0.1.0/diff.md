# Comparing `tmp/speakleash-0.0.9.tar.gz` & `tmp/speakleash-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speakleash-0.0.9.tar", last modified: Mon Dec 12 22:47:55 2022, max compression
+gzip compressed data, was "speakleash-0.1.0.tar", last modified: Fri Jun  9 19:40:35 2023, max compression
```

## Comparing `speakleash-0.0.9.tar` & `speakleash-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 skondracki   (502) staff       (20)        0 2022-12-12 22:47:55.473712 speakleash-0.0.9/
--rw-r--r--   0 skondracki   (502) staff       (20)     1082 2022-11-13 16:50:03.000000 speakleash-0.0.9/LICENSE
--rw-r--r--   0 skondracki   (502) staff       (20)     1689 2022-12-12 22:47:55.473360 speakleash-0.0.9/PKG-INFO
--rw-r--r--   0 skondracki   (502) staff       (20)     1391 2022-12-11 23:01:51.000000 speakleash-0.0.9/README.md
--rw-r--r--   0 skondracki   (502) staff       (20)       38 2022-12-12 22:47:55.473809 speakleash-0.0.9/setup.cfg
--rw-r--r--   0 skondracki   (502) staff       (20)      571 2022-12-12 22:45:55.000000 speakleash-0.0.9/setup.py
-drwxr-xr-x   0 skondracki   (502) staff       (20)        0 2022-12-12 22:47:55.470436 speakleash-0.0.9/speakleash/
--rw-r--r--   0 skondracki   (502) staff       (20)     5224 2022-12-12 22:38:04.000000 speakleash-0.0.9/speakleash/__init__.py
-drwxr-xr-x   0 skondracki   (502) staff       (20)        0 2022-12-12 22:47:55.472934 speakleash-0.0.9/speakleash.egg-info/
--rw-r--r--   0 skondracki   (502) staff       (20)     1689 2022-12-12 22:47:55.000000 speakleash-0.0.9/speakleash.egg-info/PKG-INFO
--rw-r--r--   0 skondracki   (502) staff       (20)      218 2022-12-12 22:47:55.000000 speakleash-0.0.9/speakleash.egg-info/SOURCES.txt
--rw-r--r--   0 skondracki   (502) staff       (20)        1 2022-12-12 22:47:55.000000 speakleash-0.0.9/speakleash.egg-info/dependency_links.txt
--rw-r--r--   0 skondracki   (502) staff       (20)       28 2022-12-12 22:47:55.000000 speakleash-0.0.9/speakleash.egg-info/requires.txt
--rw-r--r--   0 skondracki   (502) staff       (20)       11 2022-12-12 22:47:55.000000 speakleash-0.0.9/speakleash.egg-info/top_level.txt
+drwxr-xr-x   0 skondracki   (502) staff       (20)        0 2023-06-09 19:40:35.836345 speakleash-0.1.0/
+-rw-r--r--   0 skondracki   (502) staff       (20)     1082 2022-11-13 16:50:03.000000 speakleash-0.1.0/LICENSE
+-rw-r--r--   0 skondracki   (502) staff       (20)     2293 2023-06-09 19:40:35.836052 speakleash-0.1.0/PKG-INFO
+-rw-r--r--   0 skondracki   (502) staff       (20)     1994 2023-06-09 19:37:08.000000 speakleash-0.1.0/README.md
+-rw-r--r--   0 skondracki   (502) staff       (20)       38 2023-06-09 19:40:35.836440 speakleash-0.1.0/setup.cfg
+-rw-r--r--   0 skondracki   (502) staff       (20)      571 2023-06-09 19:38:43.000000 speakleash-0.1.0/setup.py
+drwxr-xr-x   0 skondracki   (502) staff       (20)        0 2023-06-09 19:40:35.833885 speakleash-0.1.0/speakleash/
+-rw-r--r--   0 skondracki   (502) staff       (20)     6586 2023-06-09 19:27:17.000000 speakleash-0.1.0/speakleash/__init__.py
+drwxr-xr-x   0 skondracki   (502) staff       (20)        0 2023-06-09 19:40:35.835672 speakleash-0.1.0/speakleash.egg-info/
+-rw-r--r--   0 skondracki   (502) staff       (20)     2293 2023-06-09 19:40:35.000000 speakleash-0.1.0/speakleash.egg-info/PKG-INFO
+-rw-r--r--   0 skondracki   (502) staff       (20)      218 2023-06-09 19:40:35.000000 speakleash-0.1.0/speakleash.egg-info/SOURCES.txt
+-rw-r--r--   0 skondracki   (502) staff       (20)        1 2023-06-09 19:40:35.000000 speakleash-0.1.0/speakleash.egg-info/dependency_links.txt
+-rw-r--r--   0 skondracki   (502) staff       (20)       28 2023-06-09 19:40:35.000000 speakleash-0.1.0/speakleash.egg-info/requires.txt
+-rw-r--r--   0 skondracki   (502) staff       (20)       11 2023-06-09 19:40:35.000000 speakleash-0.1.0/speakleash.egg-info/top_level.txt
```

### Comparing `speakleash-0.0.9/LICENSE` & `speakleash-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `speakleash-0.0.9/PKG-INFO` & `speakleash-0.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speakleash
-Version: 0.0.9
+Version: 0.1.0
 Summary: SpeakLeash agnostic dataset for Polish
 Home-page: https://github.com/speakleash/speakleash
 Author: SpeakLeash Team
 Author-email: team@speakleash.org
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -78,8 +78,27 @@
 * words
 * verbs
 * nouns
 * symbols
 * punctuations
 
 
+## Supported languages
 
+On June 9, 2023, Croatia joined our projects. If you want to use Croatian language datasets just add lang parameter when creating Speakleash object.
+
+```
+from speakleash import Speakleash
+import os
+
+base_dir = os.path.join(os.path.dirname(__file__))
+replicate_to = os.path.join(base_dir, "datasets")
+
+sl = Speakleash(replicate_t, "hr")
+
+for d in sl.datasets:
+    print(d.name)
+    for doc in d.data:
+        size_mb = round(d.characters/1024/1024)
+        print("Dataset: {0}, size: {1} MB, characters: {2}, documents: {3}".format(d.name, size_mb, d.characters, d.documents))
+
+```
```

### Comparing `speakleash-0.0.9/README.md` & `speakleash-0.1.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -67,8 +67,27 @@
 * words
 * verbs
 * nouns
 * symbols
 * punctuations
 
 
+## Supported languages
 
+On June 9, 2023, Croatia joined our projects. If you want to use Croatian language datasets just add lang parameter when creating Speakleash object.
+
+```
+from speakleash import Speakleash
+import os
+
+base_dir = os.path.join(os.path.dirname(__file__))
+replicate_to = os.path.join(base_dir, "datasets")
+
+sl = Speakleash(replicate_t, "hr")
+
+for d in sl.datasets:
+    print(d.name)
+    for doc in d.data:
+        size_mb = round(d.characters/1024/1024)
+        print("Dataset: {0}, size: {1} MB, characters: {2}, documents: {3}".format(d.name, size_mb, d.characters, d.documents))
+
+```
```

### Comparing `speakleash-0.0.9/setup.py` & `speakleash-0.1.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="speakleash",
-    version="0.0.9",
+    version="0.1.0",
     author="SpeakLeash Team",
     author_email="team@speakleash.org",
     description="SpeakLeash agnostic dataset for Polish",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/speakleash/speakleash",
     packages = ["speakleash"],
```

### Comparing `speakleash-0.0.9/speakleash/__init__.py` & `speakleash-0.1.0/speakleash/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,93 @@
 import requests
 import json
 from tqdm import tqdm
 import os
 from lm_dataformat import Reader
+import hashlib
+from datetime import datetime
+import glob
 
-class Speakleash(object):
+class StructureDownloader(object):
 
     def __init__(self, replicate_dir):
         self.replicate_dir = replicate_dir
+
+    def _remove_old_files(self, url):
+        
+        hash = hashlib.md5(url.encode('utf-8')).hexdigest()
+        filter = os.path.join(self.replicate_dir, hash + "-*.json")
+        files = glob.glob(filter)
+        for f in files:
+            try:
+                os.remove(f)
+            except:
+                pass
+
+        return
+
+    def get_structure(self, url, hourly = True):
+
+        now = datetime.now()
+        data = None
+
+        if hourly:
+            ts = now.strftime("-%m_%d_%y_%H")
+        else:
+            ts = now.strftime("-%m_%d_%y")
+
+        hash = hashlib.md5(url.encode('utf-8')).hexdigest()
+        file = os.path.join(self.replicate_dir, hash + ts + ".json")
+
+        if os.path.exists(file):
+            try:
+                with open(file, 'r') as f:
+                    data = json.load(f)
+                return data
+            except:
+                pass
+
+        self._remove_old_files(url)
+
+        try:
+            r = requests.get(url)
+            if r.ok:
+                data = json.loads(r.text)
+        except:
+            pass
+
+        try:
+            with open(file, 'w') as f:
+                json.dump(data, f)
+        except:
+            pass
+        
+        return data
+
+class Speakleash(object):
+
+    def __init__(self, replicate_dir, lang = "pl"):
+        
+        self.replicate_dir = replicate_dir
         self.datasets = []
-        self.datasets.append(SpeakleashDataset("thesis", "https://zazepa.pl/speakleash/", self.replicate_dir))
-        self.datasets.append(SpeakleashDataset("plwiki", "https://zazepa.pl/speakleash/", self.replicate_dir))
-        self.datasets.append(SpeakleashDataset("1000_novels_corpus_CLARIN-PL", "https://zazepa.pl/speakleash/", self.replicate_dir))
-        self.datasets.append(SpeakleashDataset("wolne_lektury_corpus", "https://zazepa.pl/speakleash/", self.replicate_dir))
-        self.datasets.append(SpeakleashDataset("project_gutenberg_pl_corpus", "https://zazepa.pl/speakleash/", self.replicate_dir))
-        self.datasets.append(SpeakleashDataset("open_subtitles_corpus", "https://zazepa.pl/speakleash/", self.replicate_dir))
-        self.datasets.append(SpeakleashDataset("biblioteka_nauki_pl_corpus", "https://zazepa.pl/speakleash/", self.replicate_dir))
+
+        url = "https://speakleash.space/datasets_text/"
+        structure_file = "speakleash.json"
+
+        if lang == "hr":
+            url = "https://speakleash.space/datasets_text_hr/"
+            structure_file = "speakleash_hr.json"
+
+        names = StructureDownloader(replicate_dir).get_structure(url + structure_file)
+
+        if names:      
+            for item in names:
+                if "name" in item:
+                    self.datasets.append(SpeakleashDataset(item["name"], url, self.replicate_dir))
+
     def get(self, name):
         for d in self.datasets:
             if d.name == name:
                 return d
         return None
 
 class SpeakleashDataset(object):
@@ -48,35 +116,39 @@
         if total_size_in_bytes != 0 and progress_bar.n != total_size_in_bytes:
             ok = False
 
         return ok
 
     def _download_manifest(self):
 
-        try:
-            r = requests.get(self.url + self.name + ".manifest")
-            if r.ok:
-                return json.loads(r.text)
-        except:
+        data =StructureDownloader(self.replicate_dir).get_structure(self.url + self.name + ".manifest")
+
+        if data:
+            return data
+        else:
             print("Error downloading manifest {0}".format(self.url + self.name + ".manifest"))
-            return{}
-                
+ 
         return {}
 
     @property
     def characters(self):
         s = self.manifest.get("stats",{}).get("characters",0)
         return s
 
     @property
     def documents(self):
         s = self.manifest.get("stats",{}).get("documents",0)
         return s
 
     @property
+    def stopwords(self):
+        s = self.manifest.get("stats",{}).get("stopwords",0)
+        return s
+
+    @property
     def nouns(self):
         return self.manifest.get("stats",{}).get("nouns",[])
 
     @property
     def verbs(self):
         return self.manifest.get("stats",{}).get("verbs",[])
 
@@ -136,14 +208,21 @@
             if not self._download_file(file_name_json_zst):
                 return False, ""
 
         return True, file_path_json_zst
 
 
     @property
+    def samples(self):
+        data =StructureDownloader(self.replicate_dir).get_structure(self.url + self.name + ".sample", False)
+        if data:
+            return data
+        return []
+
+    @property
     def ext_data(self):
 
         ok, file_path_json_zst = self.check_file()
         if not ok:
             return None
 
         rdr = Reader(file_path_json_zst)
```

### Comparing `speakleash-0.0.9/speakleash.egg-info/PKG-INFO` & `speakleash-0.1.0/speakleash.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speakleash
-Version: 0.0.9
+Version: 0.1.0
 Summary: SpeakLeash agnostic dataset for Polish
 Home-page: https://github.com/speakleash/speakleash
 Author: SpeakLeash Team
 Author-email: team@speakleash.org
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -78,8 +78,27 @@
 * words
 * verbs
 * nouns
 * symbols
 * punctuations
 
 
+## Supported languages
 
+On June 9, 2023, Croatia joined our projects. If you want to use Croatian language datasets just add lang parameter when creating Speakleash object.
+
+```
+from speakleash import Speakleash
+import os
+
+base_dir = os.path.join(os.path.dirname(__file__))
+replicate_to = os.path.join(base_dir, "datasets")
+
+sl = Speakleash(replicate_t, "hr")
+
+for d in sl.datasets:
+    print(d.name)
+    for doc in d.data:
+        size_mb = round(d.characters/1024/1024)
+        print("Dataset: {0}, size: {1} MB, characters: {2}, documents: {3}".format(d.name, size_mb, d.characters, d.documents))
+
+```
```

