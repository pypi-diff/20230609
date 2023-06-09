# Comparing `tmp/t4flib-0.3.1-py2.py3-none-any.whl.zip` & `tmp/t4flib-0.3.3-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 10985 bytes, number of entries: 12
+Zip file size: 11027 bytes, number of entries: 12
 -rw-rw-r--  2.0 unx        0 b- defN 23-May-11 18:20 t4flib/__init__.py
--rw-rw-r--  2.0 unx      987 b- defN 23-May-24 12:34 t4flib/config.py
+-rw-rw-r--  2.0 unx     1086 b- defN 23-Jun-09 13:22 t4flib/config.py
 -rw-rw-r--  2.0 unx      971 b- defN 23-May-17 15:49 t4flib/data_helper.py
 -rw-rw-r--  2.0 unx     6145 b- defN 23-May-17 15:49 t4flib/file_helper.py
--rw-rw-r--  2.0 unx     5621 b- defN 23-May-22 15:34 t4flib/filetransfer_helper.py
+-rw-rw-r--  2.0 unx     5744 b- defN 23-Jun-09 13:22 t4flib/filetransfer_helper.py
 -rw-rw-r--  2.0 unx     7420 b- defN 23-May-17 15:49 t4flib/functional_helper.py
 -rw-rw-r--  2.0 unx     2682 b- defN 23-May-30 14:55 t4flib/gcloud_helper.py
 -rw-rw-r--  2.0 unx      876 b- defN 23-May-30 14:21 t4flib/log_helper.py
--rw-rw-r--  2.0 unx     1747 b- defN 23-May-30 15:07 t4flib-0.3.1.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 23-May-30 15:07 t4flib-0.3.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-May-30 15:07 t4flib-0.3.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      919 b- defN 23-May-30 15:07 t4flib-0.3.1.dist-info/RECORD
-12 files, 27485 bytes uncompressed, 9453 bytes compressed:  65.6%
+-rw-rw-r--  2.0 unx     1747 b- defN 23-Jun-09 13:35 t4flib-0.3.3.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 23-Jun-09 13:35 t4flib-0.3.3.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-Jun-09 13:35 t4flib-0.3.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      920 b- defN 23-Jun-09 13:35 t4flib-0.3.3.dist-info/RECORD
+12 files, 27708 bytes uncompressed, 9495 bytes compressed:  65.7%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: t4flib/gcloud_helper.py
 Comment: 
 
 Filename: t4flib/log_helper.py
 Comment: 
 
-Filename: t4flib-0.3.1.dist-info/METADATA
+Filename: t4flib-0.3.3.dist-info/METADATA
 Comment: 
 
-Filename: t4flib-0.3.1.dist-info/WHEEL
+Filename: t4flib-0.3.3.dist-info/WHEEL
 Comment: 
 
-Filename: t4flib-0.3.1.dist-info/top_level.txt
+Filename: t4flib-0.3.3.dist-info/top_level.txt
 Comment: 
 
-Filename: t4flib-0.3.1.dist-info/RECORD
+Filename: t4flib-0.3.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## t4flib/config.py

```diff
@@ -24,8 +24,11 @@
 GCP_ACCOUNT_SERVICE_FILE = os.environ.get("GCP_ACCOUNT_SERVICE_FILE")
 BQ_PROJECT_ID = os.environ.get("BQ_PROJECT_ID")
 
 # job_directory
 CHAINE_APAR_DIR = os.environ.get("CHAINE_APAR_DIR")
 OAR_FACT_DIR = os.environ.get("OAR_FACT_DIR")
 FACT_FRNS_DIR = os.environ.get("FACT_FRNS_DIR")
+FINE_HOLDING_DIR = os.environ.get("FINE_HOLDING_DIR")
+OAR_RGT_DIR = os.environ.get("OAR_RGT_DIR")
+
```

## t4flib/filetransfer_helper.py

```diff
@@ -137,12 +137,14 @@
                     log_f.error(str(e))
                     ret = None
 
                 if ret in [202, 200]:
 
                     logger("INFO", f"Le flux {flow_name} contenant le fichier {str(file)} est parti")
                     log_f.info(f"Le flux {flow_name} contenant le fichier {str(file)} est parti")
+                    log_f.info(f"Suppresssion du fichier {str(file)}")
+                    os.remove(str(file.absolute()))
                 else:
 
                     logger('ERROR', f"Un code erreur API : {ret} a eu lieu")
                     logger('ERROR', f"Erreur lors de l'appel à l'API statut => {ret}")
                     log_f.error(f"Erreur lors de l'appel à l'API statut => {ret}")
```

## Comparing `t4flib-0.3.1.dist-info/METADATA` & `t4flib-0.3.3.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t4flib
-Version: 0.3.1
+Version: 0.3.3
 Summary: Librairie de fonction utiles pour T4F
 Home-page: http://gitlab.dev.fr.auchan.com/tech4finance/t4flib.git
 Author: Corentin DEVROUETE
 Author-email: cdevrouete@advanced-schema.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

## Comparing `t4flib-0.3.1.dist-info/RECORD` & `t4flib-0.3.3.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 t4flib/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-t4flib/config.py,sha256=xDdhCesAg9COfAbPGSxQm_DsHH3fHNqyvB6So5SloOc,987
+t4flib/config.py,sha256=4kv9YBFa7cwTjxNbBRGgMduVth0VRk05CftWP4Yjexw,1086
 t4flib/data_helper.py,sha256=SdKdv2U1EXtHJcfEff_I8zIlMWv56-xLZqczAw4kOUU,971
 t4flib/file_helper.py,sha256=NYIgOrA1iJBUcodtaRlDIsIHoivonLme4PmFZB1nQLw,6145
-t4flib/filetransfer_helper.py,sha256=CkWlCJe5E_G0iovU2Jvm5ixB94RYl-lmAid4gEiDAe0,5621
+t4flib/filetransfer_helper.py,sha256=UtNQp3OP3Bh7JICdbtoE8BB8_k9v8bEeMWSoJFnndXI,5744
 t4flib/functional_helper.py,sha256=CfbwrMufVRwCQNg9us9tujS3oeCmxql18vmo7B5lUAI,7420
 t4flib/gcloud_helper.py,sha256=5_5fzYVlivt_2mBs9OBYfRyO-84UsL5gOr5MI8Mt4gQ,2682
 t4flib/log_helper.py,sha256=pu_y3m7iHWpkgYnxLYAlQjWjqknMGDcCDjHV6w4YYDc,876
-t4flib-0.3.1.dist-info/METADATA,sha256=7VNGXFwdVsf3hROrYOqw8CT65H-YoTSR8NyJ25M5DnQ,1747
-t4flib-0.3.1.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-t4flib-0.3.1.dist-info/top_level.txt,sha256=-05r3tdNDBMHneiATbWVqDQI7djLF9N83J6mAMcxbp8,7
-t4flib-0.3.1.dist-info/RECORD,,
+t4flib-0.3.3.dist-info/METADATA,sha256=fWUhaOA1z4NMsZ6El9XFtzizUodG0r-LlegFo0hxBN4,1747
+t4flib-0.3.3.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+t4flib-0.3.3.dist-info/top_level.txt,sha256=-05r3tdNDBMHneiATbWVqDQI7djLF9N83J6mAMcxbp8,7
+t4flib-0.3.3.dist-info/RECORD,,
```

