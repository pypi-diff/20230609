# Comparing `tmp/concurrent_plugin-0.5.2-py3-none-any.whl.zip` & `tmp/concurrent_plugin-0.5.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,21 @@
-Zip file size: 34437 bytes, number of entries: 18
--rw-rw-r--  2.0 unx        2 b- defN 22-Sep-22 06:22 concurrent_plugin/__init__.py
--rw-rw-r--  2.0 unx    42966 b- defN 23-May-26 16:51 concurrent_plugin/concurrent_backend.py
--rw-rw-r--  2.0 unx    16820 b- defN 22-Dec-12 10:10 concurrent_plugin/concurrent_core.py
--rw-rw-r--  2.0 unx    15759 b- defN 23-Feb-15 19:34 concurrent_plugin/login.py
--rw-rw-r--  2.0 unx     3994 b- defN 23-Jan-10 17:33 concurrent_plugin/periodic_run.py
--rw-rw-r--  2.0 unx     2091 b- defN 23-May-23 18:02 concurrent_plugin/utils.py
--rw-rw-r--  2.0 unx        0 b- defN 22-Sep-22 06:22 concurrent_plugin/infinfs/__init__.py
--rw-rw-r--  2.0 unx      990 b- defN 22-Oct-18 19:03 concurrent_plugin/infinfs/infin_download.py
--rw-rw-r--  2.0 unx     1339 b- defN 22-Sep-22 06:22 concurrent_plugin/infinfs/infin_prefetch.py
--rw-rw-r--  2.0 unx    10783 b- defN 22-Nov-11 07:23 concurrent_plugin/infinfs/infinfs.py
--rw-rw-r--  2.0 unx     5326 b- defN 22-Oct-18 19:03 concurrent_plugin/infinfs/infinmount.py
--rw-rw-r--  2.0 unx     1140 b- defN 22-Nov-11 07:23 concurrent_plugin/infinfs/mount_main.py
--rw-rw-r--  2.0 unx    15974 b- defN 23-May-25 20:09 concurrent_plugin/infinfs/mount_service.py
--rw-rw-r--  2.0 unx      307 b- defN 23-May-30 06:13 concurrent_plugin-0.5.2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-30 06:13 concurrent_plugin-0.5.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx      181 b- defN 23-May-30 06:13 concurrent_plugin-0.5.2.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       18 b- defN 23-May-30 06:13 concurrent_plugin-0.5.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1650 b- defN 23-May-30 06:13 concurrent_plugin-0.5.2.dist-info/RECORD
-18 files, 119432 bytes uncompressed, 31675 bytes compressed:  73.5%
+Zip file size: 34972 bytes, number of entries: 19
+-rw-rw-r--  2.0 unx        2 b- defN 22-Nov-27 22:37 concurrent_plugin/__init__.py
+-rw-rw-r--  2.0 unx    42966 b- defN 23-Jun-09 20:48 concurrent_plugin/concurrent_backend.py
+-rw-rw-r--  2.0 unx    16820 b- defN 22-Dec-17 04:51 concurrent_plugin/concurrent_core.py
+-rw-rw-r--  2.0 unx    15759 b- defN 23-Feb-15 23:54 concurrent_plugin/login.py
+-rw-rw-r--  2.0 unx     3994 b- defN 22-Dec-20 19:35 concurrent_plugin/periodic_run.py
+-rw-rw-r--  2.0 unx     1298 b- defN 23-Jan-19 23:36 concurrent_plugin/periodic_run_utils.py
+-rw-rw-r--  2.0 unx     2091 b- defN 23-Jun-01 16:52 concurrent_plugin/utils.py
+-rw-rw-r--  2.0 unx        0 b- defN 22-Nov-27 22:37 concurrent_plugin/infinfs/__init__.py
+-rw-rw-r--  2.0 unx      990 b- defN 22-Nov-27 22:37 concurrent_plugin/infinfs/infin_download.py
+-rw-rw-r--  2.0 unx     1339 b- defN 22-Nov-27 22:37 concurrent_plugin/infinfs/infin_prefetch.py
+-rw-rw-r--  2.0 unx    10783 b- defN 22-Nov-27 22:37 concurrent_plugin/infinfs/infinfs.py
+-rw-rw-r--  2.0 unx     5326 b- defN 22-Nov-27 22:37 concurrent_plugin/infinfs/infinmount.py
+-rw-rw-r--  2.0 unx     1140 b- defN 22-Nov-27 22:37 concurrent_plugin/infinfs/mount_main.py
+-rw-rw-r--  2.0 unx    15974 b- defN 23-Jun-01 16:52 concurrent_plugin/infinfs/mount_service.py
+-rw-rw-r--  2.0 unx      205 b- defN 23-Jun-09 21:00 concurrent_plugin-0.5.3.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-09 21:00 concurrent_plugin-0.5.3.dist-info/WHEEL
+-rw-rw-r--  2.0 unx      182 b- defN 23-Jun-09 21:00 concurrent_plugin-0.5.3.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       18 b- defN 23-Jun-09 21:00 concurrent_plugin-0.5.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1746 b- defN 23-Jun-09 21:00 concurrent_plugin-0.5.3.dist-info/RECORD
+19 files, 120725 bytes uncompressed, 32056 bytes compressed:  73.4%
```

## zipnote {}

```diff
@@ -9,14 +9,17 @@
 
 Filename: concurrent_plugin/login.py
 Comment: 
 
 Filename: concurrent_plugin/periodic_run.py
 Comment: 
 
+Filename: concurrent_plugin/periodic_run_utils.py
+Comment: 
+
 Filename: concurrent_plugin/utils.py
 Comment: 
 
 Filename: concurrent_plugin/infinfs/__init__.py
 Comment: 
 
 Filename: concurrent_plugin/infinfs/infin_download.py
@@ -33,23 +36,23 @@
 
 Filename: concurrent_plugin/infinfs/mount_main.py
 Comment: 
 
 Filename: concurrent_plugin/infinfs/mount_service.py
 Comment: 
 
-Filename: concurrent_plugin-0.5.2.dist-info/METADATA
+Filename: concurrent_plugin-0.5.3.dist-info/METADATA
 Comment: 
 
-Filename: concurrent_plugin-0.5.2.dist-info/WHEEL
+Filename: concurrent_plugin-0.5.3.dist-info/WHEEL
 Comment: 
 
-Filename: concurrent_plugin-0.5.2.dist-info/entry_points.txt
+Filename: concurrent_plugin-0.5.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: concurrent_plugin-0.5.2.dist-info/top_level.txt
+Filename: concurrent_plugin-0.5.3.dist-info/top_level.txt
 Comment: 
 
-Filename: concurrent_plugin-0.5.2.dist-info/RECORD
+Filename: concurrent_plugin-0.5.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## concurrent_plugin/concurrent_backend.py

```diff
@@ -646,15 +646,15 @@
             if "env" not in job_template["spec"]["template"]["spec"]["containers"][1].keys():
                 job_template["spec"]["template"]["spec"]["containers"][1]["env"] = []
             job_template["spec"]["template"]["spec"]["containers"][1]["env"] += [{'name':'PYTHONUNBUFFERED', 'value':os.getenv('PYTHONUNBUFFERED')}]
 
         job_name = job_template["metadata"]["name"]
         job_namespace = job_template["metadata"]["namespace"]
         _load_kube_context(context=kube_context)
-        kubernetes.client.configuration.retries = 10
+        kubernetes.client.configuration.retries = 24
         print(f'run_eks_job: Overrode default kubernetes.client.configuration.retries to 10')
 
         core_api_instance = kubernetes.client.CoreV1Api()
         tok = base64.b64encode(get_token_file_obj('r').read().encode('utf-8')).decode('utf-8')
         token_secret_name = 'parallelstokenfile-' + str(uuid.uuid4())
         try:
             core_api_instance.delete_namespaced_secret(namespace=job_namespace, name=token_secret_name)
```

## Comparing `concurrent_plugin-0.5.2.dist-info/RECORD` & `concurrent_plugin-0.5.3.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 concurrent_plugin/__init__.py,sha256=4W8VliAYUP1KY2gLJ_YDy2TmcXYVm-PY7XikQD_bFwA,2
-concurrent_plugin/concurrent_backend.py,sha256=ytxbHgMGTmasGLxQp1Fdtkq9YOaCiEVb5sD7J71NMmU,42966
+concurrent_plugin/concurrent_backend.py,sha256=dASijwn_zQVckPJyqguBhqXyhZnReAUqUWXKKSGrqxo,42966
 concurrent_plugin/concurrent_core.py,sha256=ECXT0b11j8L5kgWAxxyW6gg6gUK9d_TGOf_AibCb27k,16820
 concurrent_plugin/login.py,sha256=yBdoKr_9Uiq4DFPHmQjJEBGS61F2fw79QIL8c3hy5Vg,15759
 concurrent_plugin/periodic_run.py,sha256=Ud66-3AtnonAO6oOhcn2EwJQPfbljcrlCQeR23ELH1c,3994
+concurrent_plugin/periodic_run_utils.py,sha256=MZuX9uSFEuA7B8UFDAchsrWhidXT5QyuOA-GDtzIPOo,1298
 concurrent_plugin/utils.py,sha256=NpAWse8mKJkP_cyxLuCFizfVe2JjuyWkQWRGbBRjf9w,2091
 concurrent_plugin/infinfs/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 concurrent_plugin/infinfs/infin_download.py,sha256=6yILg2brDNDNMFGqayFHIshB4cl25byn5dal0QI7JKQ,990
 concurrent_plugin/infinfs/infin_prefetch.py,sha256=ICqCHaiugg0z_gm4cMpQGJHozSXuf54kAw97g4yAhGU,1339
 concurrent_plugin/infinfs/infinfs.py,sha256=3xId2Ocp7UJv7ntBgpr-KCFv5wGJQFw2m8csamIHiYY,10783
 concurrent_plugin/infinfs/infinmount.py,sha256=Y9BPuggy0P9gz-kYH2ZhLy24Z1WTsw7GgU3rgH7JSsY,5326
 concurrent_plugin/infinfs/mount_main.py,sha256=ehL8zXZ1HRviaukp753TjJ6pFCtO9uUfUIjx8yfUHVE,1140
 concurrent_plugin/infinfs/mount_service.py,sha256=G6jpVhFClkiwAoUyp4R35wTrhOzg23MA5-XZkyAWHX0,15974
-concurrent_plugin-0.5.2.dist-info/METADATA,sha256=HLWfzuPTFvxoAvlQWfnNC7FMYmfsVz8AqTdCLs7GmNk,307
-concurrent_plugin-0.5.2.dist-info/WHEEL,sha256=p46_5Uhzqz6AzeSosiOnxK-zmFja1i22CrQCjmYe8ec,92
-concurrent_plugin-0.5.2.dist-info/entry_points.txt,sha256=1x__D3G335a8YKoEFWsCaUHB-H1IqgvVq07ga4TgtGk,181
-concurrent_plugin-0.5.2.dist-info/top_level.txt,sha256=rMkubPHW5GESfE5gDfsycyj3TWUOusZRYPD2lwoggcg,18
-concurrent_plugin-0.5.2.dist-info/RECORD,,
+concurrent_plugin-0.5.3.dist-info/METADATA,sha256=uOEOWhsoVpXer0I1H35XuVRUMPUlVFpf-cjLSLXuTtc,205
+concurrent_plugin-0.5.3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+concurrent_plugin-0.5.3.dist-info/entry_points.txt,sha256=5bYsI3RSqBvAjlcOeCbKKIRorBotB8wvo1p4Xfn3tXY,182
+concurrent_plugin-0.5.3.dist-info/top_level.txt,sha256=rMkubPHW5GESfE5gDfsycyj3TWUOusZRYPD2lwoggcg,18
+concurrent_plugin-0.5.3.dist-info/RECORD,,
```

