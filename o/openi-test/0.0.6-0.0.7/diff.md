# Comparing `tmp/openi-test-0.0.6.tar.gz` & `tmp/openi-test-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\openi-test-0.0.6.tar", last modified: Thu Jun  8 10:16:51 2023, max compression
+gzip compressed data, was "dist\openi-test-0.0.7.tar", last modified: Fri Jun  9 01:54:43 2023, max compression
```

## Comparing `openi-test-0.0.6.tar` & `openi-test-0.0.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 10:16:51.916425 openi-test-0.0.6/
--rw-rw-rw-   0        0        0     1994 2023-06-08 10:16:51.914422 openi-test-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1004 2023-06-08 09:05:33.000000 openi-test-0.0.6/README.md
--rw-rw-rw-   0        0        0       42 2023-06-08 10:16:51.916425 openi-test-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1075 2023-06-08 10:16:40.000000 openi-test-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-08 10:16:51.853197 openi-test-0.0.6/src/
-drwxrwxrwx   0        0        0        0 2023-06-08 10:16:51.862192 openi-test-0.0.6/src/openi/
--rw-rw-rw-   0        0        0       44 2023-06-08 10:08:34.000000 openi-test-0.0.6/src/openi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-08 10:16:51.869192 openi-test-0.0.6/src/openi/dataset/
--rw-rw-rw-   0        0        0       22 2023-06-08 07:26:17.000000 openi-test-0.0.6/src/openi/dataset/__init__.py
--rw-rw-rw-   0        0        0    10925 2023-06-08 07:26:17.000000 openi-test-0.0.6/src/openi/dataset/dataset.py
-drwxrwxrwx   0        0        0        0 2023-06-08 10:16:51.891904 openi-test-0.0.6/src/openi/utils/
--rw-rw-rw-   0        0        0       88 2023-06-08 08:03:34.000000 openi-test-0.0.6/src/openi/utils/__init__.py
--rw-rw-rw-   0        0        0     4822 2023-06-08 08:19:40.000000 openi-test-0.0.6/src/openi/utils/helper.py
--rw-rw-rw-   0        0        0     1440 2023-06-08 08:41:21.000000 openi-test-0.0.6/src/openi/utils/minio.py
--rw-rw-rw-   0        0        0     1718 2023-06-08 07:56:06.000000 openi-test-0.0.6/src/openi/utils/modelarts.py
--rw-rw-rw-   0        0        0     2359 2023-06-08 08:42:20.000000 openi-test-0.0.6/src/openi/utils/obs.py
--rw-rw-rw-   0        0        0     2128 2023-06-08 10:16:28.000000 openi-test-0.0.6/src/openi/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-08 10:16:51.911423 openi-test-0.0.6/src/openi_test.egg-info/
--rw-rw-rw-   0        0        0     1994 2023-06-08 10:16:51.000000 openi-test-0.0.6/src/openi_test.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      444 2023-06-08 10:16:51.000000 openi-test-0.0.6/src/openi_test.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 10:16:51.000000 openi-test-0.0.6/src/openi_test.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-06-08 10:16:51.000000 openi-test-0.0.6/src/openi_test.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-08 10:16:51.000000 openi-test-0.0.6/src/openi_test.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 01:54:43.277505 openi-test-0.0.7/
+-rw-rw-rw-   0        0        0     1994 2023-06-09 01:54:43.275488 openi-test-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1004 2023-06-08 09:05:33.000000 openi-test-0.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-09 01:54:43.278484 openi-test-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1075 2023-06-09 01:54:32.000000 openi-test-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 01:54:43.215885 openi-test-0.0.7/src/
+drwxrwxrwx   0        0        0        0 2023-06-09 01:54:43.226864 openi-test-0.0.7/src/openi/
+-rw-rw-rw-   0        0        0       44 2023-06-08 10:08:34.000000 openi-test-0.0.7/src/openi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 01:54:43.232883 openi-test-0.0.7/src/openi/dataset/
+-rw-rw-rw-   0        0        0       22 2023-06-08 07:26:17.000000 openi-test-0.0.7/src/openi/dataset/__init__.py
+-rw-rw-rw-   0        0        0    10925 2023-06-08 07:26:17.000000 openi-test-0.0.7/src/openi/dataset/dataset.py
+drwxrwxrwx   0        0        0        0 2023-06-09 01:54:43.255494 openi-test-0.0.7/src/openi/utils/
+-rw-rw-rw-   0        0        0       88 2023-06-08 08:03:34.000000 openi-test-0.0.7/src/openi/utils/__init__.py
+-rw-rw-rw-   0        0        0     4822 2023-06-08 08:19:40.000000 openi-test-0.0.7/src/openi/utils/helper.py
+-rw-rw-rw-   0        0        0     1457 2023-06-09 01:54:08.000000 openi-test-0.0.7/src/openi/utils/minio.py
+-rw-rw-rw-   0        0        0     1718 2023-06-08 07:56:06.000000 openi-test-0.0.7/src/openi/utils/modelarts.py
+-rw-rw-rw-   0        0        0     2384 2023-06-09 01:53:28.000000 openi-test-0.0.7/src/openi/utils/obs.py
+-rw-rw-rw-   0        0        0     2128 2023-06-08 10:16:28.000000 openi-test-0.0.7/src/openi/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-09 01:54:43.271493 openi-test-0.0.7/src/openi_test.egg-info/
+-rw-rw-rw-   0        0        0     1994 2023-06-09 01:54:43.000000 openi-test-0.0.7/src/openi_test.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      444 2023-06-09 01:54:43.000000 openi-test-0.0.7/src/openi_test.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 01:54:43.000000 openi-test-0.0.7/src/openi_test.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-06-09 01:54:43.000000 openi-test-0.0.7/src/openi_test.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-09 01:54:43.000000 openi-test-0.0.7/src/openi_test.egg-info/top_level.txt
```

### Comparing `openi-test-0.0.6/PKG-INFO` & `openi-test-0.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openi-test
-Version: 0.0.6
+Version: 0.0.7
 Summary: A test packages for openi pypi
 Home-page: https://openi.pcl.ac.cn/liuzx/openi-pypi-test
 Author: chenzh05,liuzx
 Author-email: chenzh.ds@outlook.com
 License: MIT
 Description: # This is a test package for OpenI PyPi
```

### Comparing `openi-test-0.0.6/README.md` & `openi-test-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `openi-test-0.0.6/setup.py` & `openi-test-0.0.7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='openi-test',
-    version='0.0.6',
+    version='0.0.7',
     description='A test packages for openi pypi',
     package_dir={'': 'src'},
     packages=find_packages('src'),
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://openi.pcl.ac.cn/liuzx/openi-pypi-test',
     author='chenzh05,liuzx',
```

### Comparing `openi-test-0.0.6/src/openi/dataset/dataset.py` & `openi-test-0.0.7/src/openi/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `openi-test-0.0.6/src/openi/utils/helper.py` & `openi-test-0.0.7/src/openi/utils/helper.py`

 * *Files identical despite different names*

### Comparing `openi-test-0.0.6/src/openi/utils/minio.py` & `openi-test-0.0.7/src/openi/utils/minio.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,32 +2,32 @@
 def get_code_path_minio():
     """
     获取源代码存储在minio,挂载到镜像后的代码路径
     """
     code_path = os.getenv("CODE_PATH")
     if code_path is None:
     	raise ValueError("Failed to get the environment variable, please ensure that the CODE_PATH environment variable has been set.")
-    return code_path 
+    return str(code_path)
 def get_data_path_minio():
     """
     获取源数据集存储在minio,挂载到镜像后的数据集路径
     """
     data_path = os.getenv("DATA_PATH")
     if data_path is None:
     	raise ValueError("Failed to get the environment variable, please ensure that the DATA_PATH environment variable has been set.")
-    return data_path 
+    return str(data_path)
 def get_pretrain_model_path_minio():
     """
     获取源预训练模型存储在minio,挂载到镜像后的预训练模型路径
     """
     pretrain_model_path = os.getenv("PRETRAIN_MODEL_PATH")
     if pretrain_model_path is None:
     	raise ValueError("Failed to get the environment variable, please make sure the PRETRAIN_MODEL_PATH environment variable has been set.")
-    return pretrain_model_path 
+    return str(pretrain_model_path)
 def get_output_path_minio():
     """
     获取需要存储在minio的输出路径
     """    
     output_path = os.getenv("OUTPUT_PATH")
     if output_path is None:
     	raise ValueError("Failed to get the environment variable, please ensure that the OUTPUT_PATH environment variable has been set.")
-    return output_path
+    return str(output_path)
```

### Comparing `openi-test-0.0.6/src/openi/utils/modelarts.py` & `openi-test-0.0.7/src/openi/utils/modelarts.py`

 * *Files identical despite different names*

### Comparing `openi-test-0.0.6/src/openi/utils/obs.py` & `openi-test-0.0.7/src/openi/utils/obs.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from .modelarts import openi_multidataset_to_env,c2net_multidataset_to_env,pretrain_to_env,env_to_openi
+import os
 #需要定义传给modelarts的两个参数data_url和train_url或是使用args, unknown = parser.parse_known_args()来规避超参数没定义的报错
 def get_code_path_obs():
     """
     获取源数据代码存储在obs,拷贝到镜像后的代码路径
     """
     return
 def get_data_path_obs():
@@ -14,33 +15,33 @@
     data_path = os.getenv("DATA_PATH")
     if cluster is None or data_url is None or data_path is None:
     	raise ValueError("Failed to get the environment variable, please make sure the CLUSTER, DATA_URL and DATA_PATH environment variables have been set")
     if cluster == "c2net":
         c2net_multidataset_to_env(data_url, data_path)
     else:
         openi_multidataset_to_env(data_url, data_path)
-    return data_path
+    return str(data_path)
 def get_pretrain_model_path_obs():
     """
     获取源数据预训练模型存储在obs,拷贝到镜像后的预训练模型路径
     """
     pretrain_model_url = os.getenv("PRETRAIN_MODEL_URL")
     pretrain_model_path= os.getenv("PRETRAIN_MODEL_PATH")
     if pretrain_model_url is None or pretrain_model_path is None:
     	raise ValueError("Failed to get environment variables, please make sure you have set PRETRAIN_MODEL_URL, PRETRAIN_MODEL_PATH environment variables.")
     pretrain_to_env(pretrain_model_url, pretrain_model_path)
-    return pretrain_model_path
+    return str(pretrain_model_path)
 def get_output_path_obs():
     """
     获取需要存储在obs上的输出路径
     """
     output_path = os.getenv("OUTPUT_PATH")
     if output_path is None:
     	raise ValueError("Failed to get the environment variable, please ensure that the OUTPUT_PATH environment variable has been set.")
-    return output_path 
+    return str(output_path)
 def push_output_to_openi_obs():
     """
     将输出数据推送到openi的obs存储
     """
     output_url = os.getenv("OUTPUT_URL")
     output_path = os.getenv("OUTPUT_PATH")
     if output_url is None or output_path is None:
```

### Comparing `openi-test-0.0.6/src/openi/utils/utils.py` & `openi-test-0.0.7/src/openi/utils/utils.py`

 * *Files identical despite different names*

### Comparing `openi-test-0.0.6/src/openi_test.egg-info/PKG-INFO` & `openi-test-0.0.7/src/openi_test.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openi-test
-Version: 0.0.6
+Version: 0.0.7
 Summary: A test packages for openi pypi
 Home-page: https://openi.pcl.ac.cn/liuzx/openi-pypi-test
 Author: chenzh05,liuzx
 Author-email: chenzh.ds@outlook.com
 License: MIT
 Description: # This is a test package for OpenI PyPi
```

