# Comparing `tmp/hmd_cli_librarian-0.1.10-py3-none-any.whl.zip` & `tmp/hmd_cli_librarian-0.1.11-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 7779 bytes, number of entries: 10
--rw-rw-rw-  2.0 unx        0 b- defN 23-May-10 18:44 hmd_cli_librarian/__init__.py
--rw-rw-rw-  2.0 unx     3265 b- defN 23-May-10 18:44 hmd_cli_librarian/controller.py
--rw-rw-rw-  2.0 unx    11698 b- defN 23-May-10 18:44 hmd_cli_librarian/hmd_cli_librarian.py
--rw-r--r--  2.0 unx      698 b- defN 23-May-10 18:44 hmd_cli_librarian/local_librarian_prj/meta-data/config_local.json
--rw-r--r--  2.0 unx      355 b- defN 23-May-10 18:44 hmd_cli_librarian/local_librarian_prj/meta-data/manifest.json
--rw-r--r--  2.0 unx      293 b- defN 23-May-10 18:44 hmd_cli_librarian/local_librarian_prj/src/python/setup.py
--rw-rw-rw-  2.0 unx     1523 b- defN 23-May-10 18:44 hmd_cli_librarian-0.1.10.dist-info/METADATA
--rw-rw-rw-  2.0 unx       92 b- defN 23-May-10 18:44 hmd_cli_librarian-0.1.10.dist-info/WHEEL
--rw-rw-rw-  2.0 unx       18 b- defN 23-May-10 18:44 hmd_cli_librarian-0.1.10.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      960 b- defN 23-May-10 18:44 hmd_cli_librarian-0.1.10.dist-info/RECORD
-10 files, 18902 bytes uncompressed, 6091 bytes compressed:  67.8%
+Zip file size: 7814 bytes, number of entries: 10
+-rw-rw-rw-  2.0 unx        0 b- defN 23-Jun-09 13:20 hmd_cli_librarian/__init__.py
+-rw-rw-rw-  2.0 unx     3636 b- defN 23-Jun-09 13:20 hmd_cli_librarian/controller.py
+-rw-rw-rw-  2.0 unx    11524 b- defN 23-Jun-09 13:20 hmd_cli_librarian/hmd_cli_librarian.py
+-rw-r--r--  2.0 unx      698 b- defN 23-Jun-09 13:20 hmd_cli_librarian/local_librarian_prj/meta-data/config_local.json
+-rw-r--r--  2.0 unx      355 b- defN 23-Jun-09 13:20 hmd_cli_librarian/local_librarian_prj/meta-data/manifest.json
+-rw-r--r--  2.0 unx      293 b- defN 23-Jun-09 13:20 hmd_cli_librarian/local_librarian_prj/src/python/setup.py
+-rw-rw-rw-  2.0 unx     1523 b- defN 23-Jun-09 13:21 hmd_cli_librarian-0.1.11.dist-info/METADATA
+-rw-rw-rw-  2.0 unx       92 b- defN 23-Jun-09 13:21 hmd_cli_librarian-0.1.11.dist-info/WHEEL
+-rw-rw-rw-  2.0 unx       18 b- defN 23-Jun-09 13:21 hmd_cli_librarian-0.1.11.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      960 b- defN 23-Jun-09 13:21 hmd_cli_librarian-0.1.11.dist-info/RECORD
+10 files, 19099 bytes uncompressed, 6126 bytes compressed:  67.9%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: hmd_cli_librarian/local_librarian_prj/meta-data/manifest.json
 Comment: 
 
 Filename: hmd_cli_librarian/local_librarian_prj/src/python/setup.py
 Comment: 
 
-Filename: hmd_cli_librarian-0.1.10.dist-info/METADATA
+Filename: hmd_cli_librarian-0.1.11.dist-info/METADATA
 Comment: 
 
-Filename: hmd_cli_librarian-0.1.10.dist-info/WHEEL
+Filename: hmd_cli_librarian-0.1.11.dist-info/WHEEL
 Comment: 
 
-Filename: hmd_cli_librarian-0.1.10.dist-info/top_level.txt
+Filename: hmd_cli_librarian-0.1.11.dist-info/top_level.txt
 Comment: 
 
-Filename: hmd_cli_librarian-0.1.10.dist-info/RECORD
+Filename: hmd_cli_librarian-0.1.11.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hmd_cli_librarian/controller.py

```diff
@@ -75,20 +75,33 @@
     #     args = {}
     #     # deploy the args values...
 
     #     from .hmd_cli_librarian import deploy as do_deploy
 
     #     result = do_deploy(**args)
 
-    @ex(help="start a local Librarian")
+    @ex(
+        help="start a local Librarian",
+        arguments=[
+            (
+                ["-cf", "--config-file"],
+                {
+                    "action": "store",
+                    "dest": "config_file",
+                    "default": "./src/configs/default.librarian.json",
+                },
+            )
+        ],
+    )
     def start(self):
+        args = {"config_file": self.app.pargs.config_file}
         load_hmd_env()
         from .hmd_cli_librarian import start as do_start
 
-        do_start()
+        do_start(**args)
 
     @ex(help="reload a local Librarian")
     def reload(self):
         load_hmd_env()
         from .hmd_cli_librarian import reload as do_reload
 
         do_reload()
```

## hmd_cli_librarian/hmd_cli_librarian.py

```diff
@@ -100,23 +100,21 @@
     pass
 
 
 def deploy():
     pass
 
 
-def start():
+def start(config_file: str = "./src/configs/default.librarian.json"):
     _start_local_ns()
 
-    librarian_cfg_path = Path("./src/configs/default.librarian.json")
+    librarian_cfg_path = Path(config_file)
 
     if not os.path.exists(librarian_cfg_path):
-        raise Exception(
-            "Cannot find Librarian configuration file at ./src/configs/default.librarian.json"
-        )
+        raise Exception(f"Cannot find Librarian configuration file at {config_file}")
 
     with open(librarian_cfg_path, "r") as cfg:
         librarian_cfg = json.load(cfg)
 
     if not validate_config(librarian_cfg):
         return
 
@@ -190,16 +188,16 @@
             credentials = {
                 "access_key": creds.access_key,
                 "secret_key": creds.secret_key,
                 "token": creds.token,
             }
 
         s3_endpoint = None
+        bucket_name = f"{repo_name}-default-bucket"
         if "bucket_name" not in librarian_cfg:
-            bucket_name = f"{repo_name}-default-bucket"
             s3_endpoint = "http://minio:9000/"
             session = boto3.Session(
                 aws_access_key_id="minioadmin", aws_secret_access_key="minioadmin"
             )
 
             credentials["access_key"] = "minioadmin"
             credentials["secret_key"] = "minioadmin"
@@ -232,17 +230,14 @@
                         "AWS_SESSION_TOKEN": credentials["token"],
                         "HMD_CUSTOMER_CODE": "hmd",
                         "HMD_DID": "aaa",
                         "HMD_ENVIRONMENT": "local",
                         "HMD_REGION": "reg1",
                         "HMD_INSTANCE_NAME": repo_name,
                         "BUCKET_NAME": librarian_cfg.get("bucket_name", bucket_name),
-                        # "LOCAL_BUCKET": "true"
-                        # if librarian_cfg.get("bucket_name") is None
-                        # else None,
                         "S3_ENDPOINT": s3_endpoint,
                         "CONTENT_PATH_CONFIGS": json.dumps(
                             librarian_cfg["content_item_paths"]
                         ),
                         "GRAPH_QUERY_CONFIG": json.dumps(
                             librarian_cfg.get("graph_queries", {})
                         ),
```

## Comparing `hmd_cli_librarian-0.1.10.dist-info/METADATA` & `hmd_cli_librarian-0.1.11.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hmd-cli-librarian
-Version: 0.1.10
+Version: 0.1.11
 Summary: CLI tool for developing Librarians locally
 Home-page: UNKNOWN
 Author: Alex Burgoon
 Author-email: alex.burgoon@hmdlabs.io
 License: unlicensed
 Platform: UNKNOWN
 Requires-Dist: aws-secretsmanager-caching (==1.1.1.5)
@@ -14,15 +14,15 @@
 Requires-Dist: cement (==3.0.6)
 Requires-Dist: certifi (==2022.12.7)
 Requires-Dist: charset-normalizer (==2.0.12)
 Requires-Dist: colorlog (==6.6.0)
 Requires-Dist: google-auth (==2.9.1)
 Requires-Dist: hmd-cli-app (~=1.1.595)
 Requires-Dist: hmd-cli-mickey (~=1.0.41)
-Requires-Dist: hmd-cli-neuronsphere (~=0.1.107)
+Requires-Dist: hmd-cli-neuronsphere (~=0.2.111)
 Requires-Dist: hmd-cli-tools (~=1.1.228)
 Requires-Dist: idna (==3.3)
 Requires-Dist: inquirerpy (==0.3.4)
 Requires-Dist: jinja2 (==3.0.3)
 Requires-Dist: jmespath (==0.10.0)
 Requires-Dist: kubernetes (==24.2.0)
 Requires-Dist: markupsafe (==2.1.0)
```

## Comparing `hmd_cli_librarian-0.1.10.dist-info/RECORD` & `hmd_cli_librarian-0.1.11.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 hmd_cli_librarian/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-hmd_cli_librarian/controller.py,sha256=B4-lg32aByHUfl-aQ8K-iV6aQgbansdO8bDJYZT8ZsQ,3265
-hmd_cli_librarian/hmd_cli_librarian.py,sha256=yKyQog1TcNNim1Bi9mVzN1HMZ27BJOSfSS3NexrzzBI,11698
+hmd_cli_librarian/controller.py,sha256=Mo5HeIHBCHXhPulEdpVEWpbkNYuk3thdcjTNH7AJ8xg,3636
+hmd_cli_librarian/hmd_cli_librarian.py,sha256=qzxcViY_km7_eM7Iq_h1x31voZZcNX7UA1FQDRNSwn8,11524
 hmd_cli_librarian/local_librarian_prj/meta-data/config_local.json,sha256=McieDohtICzi3piw-YQJg972x5wv1siTxcpGBXHTQJI,698
 hmd_cli_librarian/local_librarian_prj/meta-data/manifest.json,sha256=3NKobAJTzhLpb-rKYptdYjobiZdK0p7ab7ppjvnWDeQ,355
 hmd_cli_librarian/local_librarian_prj/src/python/setup.py,sha256=Lv2Jrz5tsyoll5vBZxso1HVjUGo-eXenyUJ67hMmZsc,293
-hmd_cli_librarian-0.1.10.dist-info/METADATA,sha256=CEPO0JSF36ZiUzdqBGD2MDcavbe9E_mQfqO7YT2FV6w,1523
-hmd_cli_librarian-0.1.10.dist-info/WHEEL,sha256=Ni9JGQXk2T4q02tFVwTZ-iAb8m9R1cjnSLMaE4VH1rg,92
-hmd_cli_librarian-0.1.10.dist-info/top_level.txt,sha256=MYRoVmnDNXpG8bznoHESrjSbDWQEBm3NWWgEVZWDGGM,18
-hmd_cli_librarian-0.1.10.dist-info/RECORD,,
+hmd_cli_librarian-0.1.11.dist-info/METADATA,sha256=vgQmIjtvWHyO49NNPE_cbVoFcYtd4kc9SZ_Og6ebu2c,1523
+hmd_cli_librarian-0.1.11.dist-info/WHEEL,sha256=Ni9JGQXk2T4q02tFVwTZ-iAb8m9R1cjnSLMaE4VH1rg,92
+hmd_cli_librarian-0.1.11.dist-info/top_level.txt,sha256=MYRoVmnDNXpG8bznoHESrjSbDWQEBm3NWWgEVZWDGGM,18
+hmd_cli_librarian-0.1.11.dist-info/RECORD,,
```

