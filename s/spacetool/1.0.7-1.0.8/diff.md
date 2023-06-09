# Comparing `tmp/spacetool-1.0.7.tar.gz` & `tmp/spacetool-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacetool-1.0.7.tar", last modified: Fri Jun  9 02:52:12 2023, max compression
+gzip compressed data, was "spacetool-1.0.8.tar", last modified: Fri Jun  9 06:47:48 2023, max compression
```

## Comparing `spacetool-1.0.7.tar` & `spacetool-1.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 leo        (501) staff       (20)        0 2023-06-09 02:52:12.690278 spacetool-1.0.7/
--rw-r--r--   0 leo        (501) staff       (20)     1068 2022-11-03 01:53:28.000000 spacetool-1.0.7/LICENSE
--rw-r--r--   0 leo        (501) staff       (20)      432 2023-06-09 02:52:12.690158 spacetool-1.0.7/PKG-INFO
--rw-r--r--   0 leo        (501) staff       (20)      135 2023-04-10 02:45:30.000000 spacetool-1.0.7/README.md
--rw-r--r--   0 leo        (501) staff       (20)       38 2023-06-09 02:52:12.690322 spacetool-1.0.7/setup.cfg
--rw-r--r--   0 leo        (501) staff       (20)     2437 2023-06-09 02:51:59.000000 spacetool-1.0.7/setup.py
-drwxr-xr-x   0 leo        (501) staff       (20)        0 2023-06-09 02:52:12.688735 spacetool-1.0.7/spacetool/
--rw-r--r--   0 leo        (501) staff       (20)        0 2022-11-03 01:53:28.000000 spacetool-1.0.7/spacetool/__init__.py
--rw-r--r--   0 leo        (501) staff       (20)        7 2022-11-08 03:02:34.000000 spacetool-1.0.7/spacetool/__version__.py
--rw-r--r--   0 leo        (501) staff       (20)    65179 2023-06-09 02:51:43.000000 spacetool-1.0.7/spacetool/main_tool.py
-drwxr-xr-x   0 leo        (501) staff       (20)        0 2023-06-09 02:52:12.689984 spacetool-1.0.7/spacetool.egg-info/
--rw-r--r--   0 leo        (501) staff       (20)      432 2023-06-09 02:52:12.000000 spacetool-1.0.7/spacetool.egg-info/PKG-INFO
--rw-r--r--   0 leo        (501) staff       (20)      260 2023-06-09 02:52:12.000000 spacetool-1.0.7/spacetool.egg-info/SOURCES.txt
--rw-r--r--   0 leo        (501) staff       (20)        1 2023-06-09 02:52:12.000000 spacetool-1.0.7/spacetool.egg-info/dependency_links.txt
--rw-r--r--   0 leo        (501) staff       (20)       27 2023-06-09 02:52:12.000000 spacetool-1.0.7/spacetool.egg-info/requires.txt
--rw-r--r--   0 leo        (501) staff       (20)       10 2023-06-09 02:52:12.000000 spacetool-1.0.7/spacetool.egg-info/top_level.txt
+drwxr-xr-x   0 leo        (501) staff       (20)        0 2023-06-09 06:47:48.225838 spacetool-1.0.8/
+-rw-r--r--   0 leo        (501) staff       (20)     1068 2022-11-03 01:53:28.000000 spacetool-1.0.8/LICENSE
+-rw-r--r--   0 leo        (501) staff       (20)      432 2023-06-09 06:47:48.225718 spacetool-1.0.8/PKG-INFO
+-rw-r--r--   0 leo        (501) staff       (20)      135 2023-04-10 02:45:30.000000 spacetool-1.0.8/README.md
+-rw-r--r--   0 leo        (501) staff       (20)       38 2023-06-09 06:47:48.225882 spacetool-1.0.8/setup.cfg
+-rw-r--r--   0 leo        (501) staff       (20)     2437 2023-06-09 06:47:02.000000 spacetool-1.0.8/setup.py
+drwxr-xr-x   0 leo        (501) staff       (20)        0 2023-06-09 06:47:48.224372 spacetool-1.0.8/spacetool/
+-rw-r--r--   0 leo        (501) staff       (20)        0 2022-11-03 01:53:28.000000 spacetool-1.0.8/spacetool/__init__.py
+-rw-r--r--   0 leo        (501) staff       (20)        7 2022-11-08 03:02:34.000000 spacetool-1.0.8/spacetool/__version__.py
+-rw-r--r--   0 leo        (501) staff       (20)    65201 2023-06-09 06:46:56.000000 spacetool-1.0.8/spacetool/main_tool.py
+drwxr-xr-x   0 leo        (501) staff       (20)        0 2023-06-09 06:47:48.225516 spacetool-1.0.8/spacetool.egg-info/
+-rw-r--r--   0 leo        (501) staff       (20)      432 2023-06-09 06:47:48.000000 spacetool-1.0.8/spacetool.egg-info/PKG-INFO
+-rw-r--r--   0 leo        (501) staff       (20)      260 2023-06-09 06:47:48.000000 spacetool-1.0.8/spacetool.egg-info/SOURCES.txt
+-rw-r--r--   0 leo        (501) staff       (20)        1 2023-06-09 06:47:48.000000 spacetool-1.0.8/spacetool.egg-info/dependency_links.txt
+-rw-r--r--   0 leo        (501) staff       (20)       27 2023-06-09 06:47:48.000000 spacetool-1.0.8/spacetool.egg-info/requires.txt
+-rw-r--r--   0 leo        (501) staff       (20)       10 2023-06-09 06:47:48.000000 spacetool-1.0.8/spacetool.egg-info/top_level.txt
```

### Comparing `spacetool-1.0.7/LICENSE` & `spacetool-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `spacetool-1.0.7/setup.py` & `spacetool-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding:utf-8 -*-
 from distutils.core import setup
 from setuptools import find_packages
 
 setup(
     name="spacetool",
-    version="1.0.7",
+    version="1.0.8",
     description='space.top的数据管理工具',
     author="Leo Ni",
     author_email="nij6173@gmail.com",
     url='http://space.top/',
     packages=find_packages(),
     install_requires=["requests", "cos-python-sdk-v5"],
     python_requires=">=3.6,<3.11",
```

### Comparing `spacetool-1.0.7/spacetool/main_tool.py` & `spacetool-1.0.8/spacetool/main_tool.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 # import json
 
 # 正常情况日志级别使用 INFO，需要定位时可以修改为 DEBUG，此时 SDK 会打印和服务端的通信信息
 logging.basicConfig(level=logging.INFO, stream=sys.stdout)
 
 
 def requests_post(url, payload, append_header=None):
-    logging.debug(f"####requests_post url: {url}")
-    logging.info(f"####requests_post payload: {payload}")
+    # logging.debug(f"####requests_post url {url}")
+    # logging.info(f"#### requests_post payload: {payload}")
     headers = {"content-type": "application/json", "Accept": "*/*"}
     if append_header:
         headers = dict(headers, **append_header)
     logging.debug(f"####requests_post headers: {headers}")
     res = requests.post(url, data=json.dumps(payload), headers=headers)
     return res
 
@@ -465,15 +465,15 @@
                 "md5": md5,
                 "file_name": file_name,
             }
             res = requests_post(self.frame_data_upload_url, requests_payload, {"Authorization": self.authorization})
             res_reason = res.reason
             assert res.status_code == 200, f"请求有错, errmsg【{res_reason}】"
             json_data = json.loads(res.text)
-            assert json_data['cdoe'] == 2000, f"请求有错, errmsg【{res_reason}】"
+            assert json_data['code'] == 2000, f"请求有错, errmsg【{res_reason}】"
             return json_data['data']['frame_id']
         else:
             raise ValueError(f"请求有错 {file_name}")
 
     def annotation_file_handle(self, annotation_payload):
         # annotation_payload = {
         #     "frame_name": item['frame_name'],
@@ -485,15 +485,15 @@
         #     "target_file_path_key": f"data/{item['file_dataset_code']}/{item['new_file_name']}",
         #     "file_dataset_code": item['file_dataset_code'],
         #     "file_dataset_name": item['file_dataset_name'],
         #     "task_code": task_code,
         # }
         # 上传annotation file
         md5 = self.get_file_md5(annotation_payload['full_f_name'])
-        qcloud_res = self.get_tmp_qcloud_id_key(['target_file_path_key'], md5)
+        qcloud_res = self.get_tmp_qcloud_id_key(annotation_payload['target_file_path_key'], md5)
         tmp_secret_id = qcloud_res['credentials']['tmpSecretId']
         tmp_secret_key = qcloud_res['credentials']['tmpSecretKey']
         tmp_secret_token = qcloud_res['credentials']['sessionToken']
         qcloud_region = qcloud_res['qcloud_region']
         qcloud_bucket_name = qcloud_res['qcloud_bucket_name']
         if_ever = False
         qcloud_handle_instance = QCloudHandle(tmp_secret_id, tmp_secret_key, qcloud_region, qcloud_bucket_name, if_ever, tmp_secret_token)
```

