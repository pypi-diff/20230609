# Comparing `tmp/spacetool-1.0.6.tar.gz` & `tmp/spacetool-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacetool-1.0.6.tar", last modified: Mon May  8 05:46:09 2023, max compression
+gzip compressed data, was "spacetool-1.0.7.tar", last modified: Fri Jun  9 02:52:12 2023, max compression
```

## Comparing `spacetool-1.0.6.tar` & `spacetool-1.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 leo        (501) staff       (20)        0 2023-05-08 05:46:09.324808 spacetool-1.0.6/
--rw-r--r--   0 leo        (501) staff       (20)     1068 2022-11-03 01:53:28.000000 spacetool-1.0.6/LICENSE
--rw-r--r--   0 leo        (501) staff       (20)      432 2023-05-08 05:46:09.324664 spacetool-1.0.6/PKG-INFO
--rw-r--r--   0 leo        (501) staff       (20)      135 2023-04-10 02:45:30.000000 spacetool-1.0.6/README.md
--rw-r--r--   0 leo        (501) staff       (20)       38 2023-05-08 05:46:09.324855 spacetool-1.0.6/setup.cfg
--rw-r--r--   0 leo        (501) staff       (20)     2484 2023-05-08 05:45:32.000000 spacetool-1.0.6/setup.py
-drwxr-xr-x   0 leo        (501) staff       (20)        0 2023-05-08 05:46:09.323026 spacetool-1.0.6/spacetool/
--rw-r--r--   0 leo        (501) staff       (20)        0 2022-11-03 01:53:28.000000 spacetool-1.0.6/spacetool/__init__.py
--rw-r--r--   0 leo        (501) staff       (20)        7 2022-11-08 03:02:34.000000 spacetool-1.0.6/spacetool/__version__.py
--rw-r--r--   0 leo        (501) staff       (20)    57255 2023-05-08 05:30:55.000000 spacetool-1.0.6/spacetool/main_tool.py
-drwxr-xr-x   0 leo        (501) staff       (20)        0 2023-05-08 05:46:09.324450 spacetool-1.0.6/spacetool.egg-info/
--rw-r--r--   0 leo        (501) staff       (20)      432 2023-05-08 05:46:09.000000 spacetool-1.0.6/spacetool.egg-info/PKG-INFO
--rw-r--r--   0 leo        (501) staff       (20)      260 2023-05-08 05:46:09.000000 spacetool-1.0.6/spacetool.egg-info/SOURCES.txt
--rw-r--r--   0 leo        (501) staff       (20)        1 2023-05-08 05:46:09.000000 spacetool-1.0.6/spacetool.egg-info/dependency_links.txt
--rw-r--r--   0 leo        (501) staff       (20)       27 2023-05-08 05:46:09.000000 spacetool-1.0.6/spacetool.egg-info/requires.txt
--rw-r--r--   0 leo        (501) staff       (20)       10 2023-05-08 05:46:09.000000 spacetool-1.0.6/spacetool.egg-info/top_level.txt
+drwxr-xr-x   0 leo        (501) staff       (20)        0 2023-06-09 02:52:12.690278 spacetool-1.0.7/
+-rw-r--r--   0 leo        (501) staff       (20)     1068 2022-11-03 01:53:28.000000 spacetool-1.0.7/LICENSE
+-rw-r--r--   0 leo        (501) staff       (20)      432 2023-06-09 02:52:12.690158 spacetool-1.0.7/PKG-INFO
+-rw-r--r--   0 leo        (501) staff       (20)      135 2023-04-10 02:45:30.000000 spacetool-1.0.7/README.md
+-rw-r--r--   0 leo        (501) staff       (20)       38 2023-06-09 02:52:12.690322 spacetool-1.0.7/setup.cfg
+-rw-r--r--   0 leo        (501) staff       (20)     2437 2023-06-09 02:51:59.000000 spacetool-1.0.7/setup.py
+drwxr-xr-x   0 leo        (501) staff       (20)        0 2023-06-09 02:52:12.688735 spacetool-1.0.7/spacetool/
+-rw-r--r--   0 leo        (501) staff       (20)        0 2022-11-03 01:53:28.000000 spacetool-1.0.7/spacetool/__init__.py
+-rw-r--r--   0 leo        (501) staff       (20)        7 2022-11-08 03:02:34.000000 spacetool-1.0.7/spacetool/__version__.py
+-rw-r--r--   0 leo        (501) staff       (20)    65179 2023-06-09 02:51:43.000000 spacetool-1.0.7/spacetool/main_tool.py
+drwxr-xr-x   0 leo        (501) staff       (20)        0 2023-06-09 02:52:12.689984 spacetool-1.0.7/spacetool.egg-info/
+-rw-r--r--   0 leo        (501) staff       (20)      432 2023-06-09 02:52:12.000000 spacetool-1.0.7/spacetool.egg-info/PKG-INFO
+-rw-r--r--   0 leo        (501) staff       (20)      260 2023-06-09 02:52:12.000000 spacetool-1.0.7/spacetool.egg-info/SOURCES.txt
+-rw-r--r--   0 leo        (501) staff       (20)        1 2023-06-09 02:52:12.000000 spacetool-1.0.7/spacetool.egg-info/dependency_links.txt
+-rw-r--r--   0 leo        (501) staff       (20)       27 2023-06-09 02:52:12.000000 spacetool-1.0.7/spacetool.egg-info/requires.txt
+-rw-r--r--   0 leo        (501) staff       (20)       10 2023-06-09 02:52:12.000000 spacetool-1.0.7/spacetool.egg-info/top_level.txt
```

### Comparing `spacetool-1.0.6/LICENSE` & `spacetool-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `spacetool-1.0.6/setup.py` & `spacetool-1.0.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 # -*- coding:utf-8 -*-
 from distutils.core import setup
 from setuptools import find_packages
 
-
-from setuptools import setup, find_packages
-
 setup(
     name="spacetool",
-    version="1.0.6",
+    version="1.0.7",
     description='space.top的数据管理工具',
     author="Leo Ni",
     author_email="nij6173@gmail.com",
     url='http://space.top/',
     packages=find_packages(),
     install_requires=["requests", "cos-python-sdk-v5"],
     python_requires=">=3.6,<3.11",
@@ -21,15 +18,14 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
 )
 
 
-
 # setup(name='spacetool',
 #         version='0.1',
 #         packages=find_packages(where='src\\'),  # 查找包的路径
 #         package_dir={'': 'src'},  # 包的root路径映射到的实际路径
 #         include_package_data=False,
 #         package_data={'data': []},
 #         description='A python lib for xxxxx',
```

### Comparing `spacetool-1.0.6/spacetool/main_tool.py` & `spacetool-1.0.7/spacetool/main_tool.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,14 +62,16 @@
         self.car_parking_serial_id_url = parse.urljoin(self.host, "ods/car_parking_serial_id_handler/")
         self.collection_record_serial_id_url = parse.urljoin(self.host, "ods/collection_record_serial_id_handler/")
         self.check_code_url = parse.urljoin(self.host, "ods/check_code/")
         self.usercenter_token_url = parse.urljoin(self.host, "api/v1/usercenter/token/")
         self.update_code_url = parse.urljoin(self.host, "ods/update_code/")
         self.upload_video_analysis_record_url = parse.urljoin(self.host, "ods/video_analysis_record_handler/")
         self.collection_data_upload_url = parse.urljoin(self.host, "api/v1/ods/collection_data_upload/")
+        self.frame_data_upload_url = parse.urljoin(self.host, "api/v1/ods/frame_data_upload/")
+        self.annotation_data_upload_url = parse.urljoin(self.host, "api/v1/ods/annotation_data_upload/")
         self.car_parking_serial_id = None
         self.collection_record_serial_id = None
 
         self.qcloud_sts_url = parse.urljoin(self.host, "api/v1/cloud_sts/qcloud_sts/")
         # self.check_code()              # 用户校验
         self.check_set_token()           # 设置token
         # headers = {"Authorization":"bearer a809655f-e4bf-41b8-9088-85a1d3780d6d"}
@@ -433,14 +435,94 @@
         }
         res = requests_post(self.collection_data_upload_url, requests_payload, {"Authorization": self.authorization})
         res_reason = res.reason
         assert res.status_code == 200, f"请求有错, errmsg【{res_reason}】"
         json_data = json.loads(res.text)
         return json_data
 
+    def frame_handle(self, file_name, frame_full_name, target_file_path_key):
+        res = requests_get(self.frame_data_upload_url, {"file_name": file_name}, {"Authorization": self.authorization})
+        assert res.status_code == 200, f"请求有错, errmsg【{res.reason}】"
+        json_data = json.loads(res.text)
+        if json_data['code'] == 2000:
+            # 存在
+            return json_data['data']['frame_id']
+        elif json_data['code'] == 4004:
+            # 无此记录
+            md5 = self.get_file_md5(frame_full_name)
+            # qcloud tmp key
+            qcloud_res = self.get_tmp_qcloud_id_key(target_file_path_key, md5)
+            tmp_secret_id = qcloud_res['credentials']['tmpSecretId']
+            tmp_secret_key = qcloud_res['credentials']['tmpSecretKey']
+            tmp_secret_token = qcloud_res['credentials']['sessionToken']
+            qcloud_region = qcloud_res['qcloud_region']
+            qcloud_bucket_name = qcloud_res['qcloud_bucket_name']
+            if_ever = False
+            qcloud_handle_instance = QCloudHandle(tmp_secret_id, tmp_secret_key, qcloud_region, qcloud_bucket_name, if_ever, tmp_secret_token)
+            qcloud_handle_instance.upload_file(frame_full_name, target_file_path_key)
+            requests_payload = {
+                "qcloud_sts_request_key": qcloud_res["requestId"],
+                "target_file_path_key": target_file_path_key,
+                "md5": md5,
+                "file_name": file_name,
+            }
+            res = requests_post(self.frame_data_upload_url, requests_payload, {"Authorization": self.authorization})
+            res_reason = res.reason
+            assert res.status_code == 200, f"请求有错, errmsg【{res_reason}】"
+            json_data = json.loads(res.text)
+            assert json_data['cdoe'] == 2000, f"请求有错, errmsg【{res_reason}】"
+            return json_data['data']['frame_id']
+        else:
+            raise ValueError(f"请求有错 {file_name}")
+
+    def annotation_file_handle(self, annotation_payload):
+        # annotation_payload = {
+        #     "frame_name": item['frame_name'],
+        #     "frame_id": frame_id_dict[item['frame_name']],
+        #     "file_name": item['new_file_name'],
+        #     "full_f_name": item['full_f_name'],
+        #     "file_type": item['file_type'],
+        #     "file_name_type": item['file_name_type'],
+        #     "target_file_path_key": f"data/{item['file_dataset_code']}/{item['new_file_name']}",
+        #     "file_dataset_code": item['file_dataset_code'],
+        #     "file_dataset_name": item['file_dataset_name'],
+        #     "task_code": task_code,
+        # }
+        # 上传annotation file
+        md5 = self.get_file_md5(annotation_payload['full_f_name'])
+        qcloud_res = self.get_tmp_qcloud_id_key(['target_file_path_key'], md5)
+        tmp_secret_id = qcloud_res['credentials']['tmpSecretId']
+        tmp_secret_key = qcloud_res['credentials']['tmpSecretKey']
+        tmp_secret_token = qcloud_res['credentials']['sessionToken']
+        qcloud_region = qcloud_res['qcloud_region']
+        qcloud_bucket_name = qcloud_res['qcloud_bucket_name']
+        if_ever = False
+        qcloud_handle_instance = QCloudHandle(tmp_secret_id, tmp_secret_key, qcloud_region, qcloud_bucket_name, if_ever, tmp_secret_token)
+        qcloud_handle_instance.upload_file(annotation_payload['full_f_name'], annotation_payload['target_file_path_key']) 
+        # 提交annotation record
+        requests_payload = {
+            # "bucket_id": bucket_id,
+            "file_name": annotation_payload['file_name'],
+            "target_file_path_key": annotation_payload['target_file_path_key'],
+            "md5": md5,
+            "qcloud_sts_request_key": qcloud_res["requestId"],
+            "frame_id": annotation_payload['frame_id'],
+            "file_dataset_code": annotation_payload['file_dataset_code'],
+            "file_dataset_name": annotation_payload['file_dataset_name'],
+            "task_code": annotation_payload['task_code'],
+            "file_type": annotation_payload['file_type'],
+        }
+        res = requests_post(self.annotation_data_upload_url, requests_payload, {"Authorization": self.authorization})
+        res_reason = res.reason
+        assert res.status_code == 200, f"请求有错, errmsg【{res_reason}】"
+        json_data = json.loads(res.text)
+        if json_data['code'] != 2000:
+            raise ValueError(f"标注数据提交有错 {json_data['msg']}")
+        return json_data
+
     def file_collection_data_upload(self, line, total_num, match_num, handle_num):
         total_num += 1
         if "/data/" in line:
             match_num += 1
             fir_split_line_texts = line.split("##")
             origin_full_file_path = fir_split_line_texts[1].replace("/ ", "/")
             full_f_name = "offline" + origin_full_file_path.replace("/data/", f"/data{fir_split_line_texts[0]}/")
@@ -630,14 +712,23 @@
                         pass
                 else:
                     # 泽尔格式错误
                     # todo log
                     logging.warning(f"#{line}")  # 创建一条严重级别为WARNING的日志记录
         return total_num, match_num, handle_num
 
+    # def annotation_result_handle(self, file_dir):
+    #     for root, dirs, files in os.walk(file_dir, topdown=False):
+    #         for file_name in files:
+    #             if file_name.endswith(".json"):
+    #                 full_file_path = os.path.join(root, file_name)
+    #                 split_full_file_path_list = full_file_path.split("/")
+    #                 output_dir_name = split_full_file_path_list[-2]
+    #                 dataset_name = split_full_file_path_list[-3]
+
 
 class QCloudHandle:
     '''
     # 功能点，读取文件路径，获取入库信息
     # 如果您一定要使用永久密钥来生成预签名，建议永久密钥的权限范围仅限于上传或下载操作，以规避风险。并且所生成的签名有效时长设置为完成本次上传或下载操作所需的最短期限，因为，当指定预签名 URL 的有效时间过期后，请求会中断；申请新的签名后，需要重新执行失败请求，不支持断点续传。
     # 分别封装永久密钥和临时密钥方案
     '''
@@ -1008,15 +1099,15 @@
     # 下载文件到本地目录，如果本地目录已经有同名文件则会被覆盖；
     # 如果目录结构不存在，则会创建和对象存储一样的目录结构
     def downLoadFiles(self, file_infos, localDir="./download/"):
         pool = SimpleThreadPool()
         for file in file_infos:
             # 文件下载 获取文件到本地
             file_cos_key = file["Key"]
-            localName = localDir + file_cos_key
+            localName = os.path.join(localDir, file_cos_key)
 
             # 如果本地目录结构不存在，递归创建
             if not os.path.exists(os.path.dirname(localName)):
                 os.makedirs(os.path.dirname(localName))
 
             # skip dir, no need to download it
             if str(localName).endswith("/"):
@@ -1052,14 +1143,55 @@
             print(e.get_trace_id())
             print(e.get_request_id())
 
         self.downLoadFiles(file_infos, localDir)
         return None
     # client.downLoadDirFromCos(start_prefix, localDir)
 
+    # 下载文件到本地目录，如果本地目录已经有同名文件则会被覆盖；
+    # 如果目录结构不存在，则会创建和对象存储一样的目录结构
+    def download_image_keys(self, image_keys, tmpdirname):
+        pool = SimpleThreadPool()
+        _handle_dict = {}
+        for image_key_path in image_keys:
+            tmp_img_path = os.path.join(tmpdirname, image_key_path)
+            # 如果本地目录结构不存在，递归创建
+            if not os.path.exists(os.path.dirname(tmp_img_path)):
+                os.makedirs(os.path.dirname(tmp_img_path))
+            pool.add_task(self.client.download_file, self.bucket_name, image_key_path, tmp_img_path)
+            _handle_dict[image_key_path] = tmp_img_path
+        pool.wait_completion()
+        return _handle_dict
+
+    def download_image_keys_nodir(self, image_keys, tmpdirname):
+        pool = SimpleThreadPool()
+        _handle_dict = {}
+        for image_key_path in image_keys:
+            tmp_img_path = os.path.join(tmpdirname, image_key_path.split("/")[-1])
+            if not os.path.isfile(tmp_img_path):
+                # 如果本地目录结构不存在，递归创建
+                if not os.path.exists(os.path.dirname(tmp_img_path)):
+                    os.makedirs(os.path.dirname(tmp_img_path))
+                pool.add_task(self.client.download_file, self.bucket_name, image_key_path, tmp_img_path)
+            _handle_dict[image_key_path] = tmp_img_path
+        pool.wait_completion()
+        return _handle_dict
+
+    def loacl_get_pred_images(self, file_dir, model_code):
+        predict_file_keys = []
+        for root, dirs, files in os.walk(file_dir, topdown=False):
+            for name in files:
+                if name.endswith(".jpg"):
+                    file_name = name.split("/")[-1]
+                    predict_file_name = file_name.replace(".jpg", f".{model_code}.json")
+                    predict_file_key = f"pred/{model_code}/{predict_file_name}"
+                    predict_file_keys.append(predict_file_key)
+        self.download_image_keys_nodir(predict_file_keys, file_dir)
+
+
 
 """
 pip install spacetool, requests
 import sys,os,json
 pp2 = os.path.abspath(".")
 sys.path.append(pp2)
 
@@ -1116,24 +1248,32 @@
 f1 = "/var/www/data/追势数据1号盘.txt"
 f2 = "/var/www/data/追势数据2号盘.txt"
 f3 = "/var/www/data/追势数据3号盘.txt"
 
 """
 
 """
-from spacetool import main_tool
+
 # 长期开发密钥
 secret_id = ""
 secret_key = ""
 region = ""
 bucket_name = ""
 if_ever = True
 token = None
+from spacetool import main_tool
 qcloud_handle_instance = main_tool.QCloudHandle(secret_id, secret_key, region, bucket_name, if_ever, token)
-qcloud_handle_instance.downLoadDirFromCos("data/", "/Users/leo/Downloads/未命名文件夹/")
+from ods_data.models import carparking_collection_record
+carparking_collection_record_instances = carparking_collection_record.objects.filter(id__gte=6732, if_all_frame=True)
+to_download_list = []
+for carparking_collection_record_instance in carparking_collection_record_instances:
+    to_download_list.append(f"data/{carparking_collection_record_instance.carparking.serial}-{carparking_collection_record_instance.serial}/")
+for to_download_dir in to_download_list:
+    qcloud_handle_instance.downLoadDirFromCos(to_download_dir, "/Users/leo/Documents/data/od-车辆/data0608/")
+qcloud_handle_instance.downLoadDirFromCos("data/", "/Users/leo/Documents/data/od-车辆/data0517/")
 
 """
 
 """
 qcloud 测试
 if __name__ == "__main__":
     # 进入异步任务队列
@@ -1165,7 +1305,12 @@
     # signed_download_url = qcloud_handle_instance.gen_file_download_url("tmp/screenshot-20230324-151321.png")
     # print(f"#### signed_download_url: {signed_download_url}")
     # response = requests.get(signed_download_url)
     # print(response)
     res = qcloud_handle_instance.list_objects("tmp/")
     # print(f"---res: {res}")
 """
+
+"""
+
+
+"""
```

