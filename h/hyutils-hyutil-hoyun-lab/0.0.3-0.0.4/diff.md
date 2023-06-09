# Comparing `tmp/hyutils-hyutil-hoyun-lab-0.0.3.tar.gz` & `tmp/hyutils-hyutil-hoyun-lab-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyutils-hyutil-hoyun-lab-0.0.3.tar", last modified: Thu Jun  8 16:05:59 2023, max compression
+gzip compressed data, was "hyutils-hyutil-hoyun-lab-0.0.4.tar", last modified: Fri Jun  9 06:29:08 2023, max compression
```

## Comparing `hyutils-hyutil-hoyun-lab-0.0.3.tar` & `hyutils-hyutil-hoyun-lab-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 16:05:59.214313 hyutils-hyutil-hoyun-lab-0.0.3/
--rw-rw-rw-   0        0        0       37 2023-06-08 03:25:10.000000 hyutils-hyutil-hoyun-lab-0.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0      598 2023-06-08 16:05:57.656302 hyutils-hyutil-hoyun-lab-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       63 2023-06-07 07:35:02.000000 hyutils-hyutil-hoyun-lab-0.0.3/README.md
--rw-rw-rw-   0        0        0      104 2023-06-07 07:28:50.000000 hyutils-hyutil-hoyun-lab-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-08 16:05:59.214313 hyutils-hyutil-hoyun-lab-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      850 2023-06-08 16:05:27.000000 hyutils-hyutil-hoyun-lab-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-08 16:05:56.845306 hyutils-hyutil-hoyun-lab-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-06-08 16:05:57.316303 hyutils-hyutil-hoyun-lab-0.0.3/src/hyutil_hoyun_lab/
--rw-rw-rw-   0        0        0      345 2023-06-08 09:06:24.000000 hyutils-hyutil-hoyun-lab-0.0.3/src/hyutil_hoyun_lab/__init__.py
--rw-rw-rw-   0        0        0      435 2023-01-19 02:15:34.000000 hyutils-hyutil-hoyun-lab-0.0.3/src/hyutil_hoyun_lab/appcontrol.py
--rw-rw-rw-   0        0        0      614 2023-05-30 04:04:28.000000 hyutils-hyutil-hoyun-lab-0.0.3/src/hyutil_hoyun_lab/date_time.py
--rw-rw-rw-   0        0        0      860 2023-06-07 07:24:28.000000 hyutils-hyutil-hoyun-lab-0.0.3/src/hyutil_hoyun_lab/dirjob.py
--rw-rw-rw-   0        0        0     1086 2023-02-02 02:25:56.000000 hyutils-hyutil-hoyun-lab-0.0.3/src/hyutil_hoyun_lab/hashing.py
--rw-rw-rw-   0        0        0     9787 2023-06-08 09:11:48.000000 hyutils-hyutil-hoyun-lab-0.0.3/src/hyutil_hoyun_lab/tfrecrod_utils.py
--rw-rw-rw-   0        0        0     3842 2023-06-08 04:01:30.000000 hyutils-hyutil-hoyun-lab-0.0.3/src/hyutil_hoyun_lab/xml_util.py
-drwxrwxrwx   0        0        0        0 2023-06-08 16:05:57.593305 hyutils-hyutil-hoyun-lab-0.0.3/src/hyutils_hyutil_hoyun_lab.egg-info/
--rw-rw-rw-   0        0        0      598 2023-06-08 16:05:56.000000 hyutils-hyutil-hoyun-lab-0.0.3/src/hyutils_hyutil_hoyun_lab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      490 2023-06-08 16:05:56.000000 hyutils-hyutil-hoyun-lab-0.0.3/src/hyutils_hyutil_hoyun_lab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 16:05:56.000000 hyutils-hyutil-hoyun-lab-0.0.3/src/hyutils_hyutil_hoyun_lab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-08 16:05:56.000000 hyutils-hyutil-hoyun-lab-0.0.3/src/hyutils_hyutil_hoyun_lab.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 06:29:08.969145 hyutils-hyutil-hoyun-lab-0.0.4/
+-rw-rw-rw-   0        0        0       37 2023-06-08 03:25:08.000000 hyutils-hyutil-hoyun-lab-0.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0      598 2023-06-09 06:29:08.968047 hyutils-hyutil-hoyun-lab-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       63 2023-06-07 07:35:00.000000 hyutils-hyutil-hoyun-lab-0.0.4/README.md
+-rw-rw-rw-   0        0        0      104 2023-06-07 07:28:49.000000 hyutils-hyutil-hoyun-lab-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-09 06:29:08.969464 hyutils-hyutil-hoyun-lab-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      850 2023-06-09 06:28:21.000000 hyutils-hyutil-hoyun-lab-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:29:08.926258 hyutils-hyutil-hoyun-lab-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-06-09 06:29:08.954029 hyutils-hyutil-hoyun-lab-0.0.4/src/hyutil_hoyun_lab/
+-rw-rw-rw-   0        0        0      345 2023-06-09 06:28:05.000000 hyutils-hyutil-hoyun-lab-0.0.4/src/hyutil_hoyun_lab/__init__.py
+-rw-rw-rw-   0        0        0      435 2023-01-19 02:15:34.000000 hyutils-hyutil-hoyun-lab-0.0.4/src/hyutil_hoyun_lab/appcontrol.py
+-rw-rw-rw-   0        0        0      614 2023-05-30 04:04:27.000000 hyutils-hyutil-hoyun-lab-0.0.4/src/hyutil_hoyun_lab/date_time.py
+-rw-rw-rw-   0        0        0      860 2023-06-07 07:24:26.000000 hyutils-hyutil-hoyun-lab-0.0.4/src/hyutil_hoyun_lab/dirjob.py
+-rw-rw-rw-   0        0        0     1086 2023-02-02 02:25:56.000000 hyutils-hyutil-hoyun-lab-0.0.4/src/hyutil_hoyun_lab/hashing.py
+-rw-rw-rw-   0        0        0    13711 2023-06-09 05:56:06.000000 hyutils-hyutil-hoyun-lab-0.0.4/src/hyutil_hoyun_lab/tfrecrod_utils.py
+-rw-rw-rw-   0        0        0     3842 2023-06-08 04:01:29.000000 hyutils-hyutil-hoyun-lab-0.0.4/src/hyutil_hoyun_lab/xml_util.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:29:08.965491 hyutils-hyutil-hoyun-lab-0.0.4/src/hyutils_hyutil_hoyun_lab.egg-info/
+-rw-rw-rw-   0        0        0      598 2023-06-09 06:29:08.000000 hyutils-hyutil-hoyun-lab-0.0.4/src/hyutils_hyutil_hoyun_lab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      490 2023-06-09 06:29:08.000000 hyutils-hyutil-hoyun-lab-0.0.4/src/hyutils_hyutil_hoyun_lab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 06:29:08.000000 hyutils-hyutil-hoyun-lab-0.0.4/src/hyutils_hyutil_hoyun_lab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-09 06:29:08.000000 hyutils-hyutil-hoyun-lab-0.0.4/src/hyutils_hyutil_hoyun_lab.egg-info/top_level.txt
```

### Comparing `hyutils-hyutil-hoyun-lab-0.0.3/PKG-INFO` & `hyutils-hyutil-hoyun-lab-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyutils-hyutil-hoyun-lab
-Version: 0.0.3
+Version: 0.0.4
 Summary: Hoyun Lab Python Utils
 Home-page: https://www.hoyun.co.kr
 Author: nohgan im
 Author-email: fory2k@hoyun.co.kr
 License: MIT
 Project-URL: Bug Tracker, https://github.com/schooldevops/python-tutorials/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hyutils-hyutil-hoyun-lab-0.0.3/setup.py` & `hyutils-hyutil-hoyun-lab-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
     
 
 setuptools.setup(
     name="hyutils-hyutil-hoyun-lab",
-    version="0.0.3",
+    version="0.0.4",
     url="https://www.hoyun.co.kr",
     license="MIT",
     author="nohgan im",
     author_email="fory2k@hoyun.co.kr",
     description="Hoyun Lab Python Utils",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `hyutils-hyutil-hoyun-lab-0.0.3/src/hyutil_hoyun_lab/date_time.py` & `hyutils-hyutil-hoyun-lab-0.0.4/src/hyutil_hoyun_lab/date_time.py`

 * *Files identical despite different names*

### Comparing `hyutils-hyutil-hoyun-lab-0.0.3/src/hyutil_hoyun_lab/dirjob.py` & `hyutils-hyutil-hoyun-lab-0.0.4/src/hyutil_hoyun_lab/dirjob.py`

 * *Files identical despite different names*

### Comparing `hyutils-hyutil-hoyun-lab-0.0.3/src/hyutil_hoyun_lab/hashing.py` & `hyutils-hyutil-hoyun-lab-0.0.4/src/hyutil_hoyun_lab/hashing.py`

 * *Files identical despite different names*

### Comparing `hyutils-hyutil-hoyun-lab-0.0.3/src/hyutil_hoyun_lab/tfrecrod_utils.py` & `hyutils-hyutil-hoyun-lab-0.0.4/src/hyutil_hoyun_lab/tfrecrod_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import tensorflow as tf
 import numpy as np
 from PIL import Image
 from object_detection.utils import dataset_util
 from collections import namedtuple, OrderedDict
 import glob
 import shutil
+import cv2
 
 def xml_to_dataframe(path, include_string):
     classes_names = []
 
     classes_names.clear()
     if not os.path.exists(path) or len(include_string) == 0:
         print(f'invalid parameters: {path} {include_string}')
@@ -253,8 +254,94 @@
         if idx < train_count:
             target_path = os.path.join(train_label, os.path.basename(all_anno_list[idx]))
         else:
             target_path = os.path.join(test_label, os.path.basename(all_anno_list[idx]))
 
         if os.path.exists(target_path):
             os.remove(target_path)
-        shutil.copy(xml_fullpath, target_path)
+        shutil.copy(xml_fullpath, target_path)
+
+"""
+설명: 입력된 이미지 저장 경로와 csv 파일 경로를 입력받아서, 
+  csv의 1라인씩 읽어 width, height, xmin, ymin, xmax, ymax 값을 출력하고,
+  대응하는 이미지를 읽어서 width, height를 읽어서 각 값들의 유효성을 체크하여,
+  이후 tfrecord로 변환할 데이터의 유효성을 검증하고,
+  이미지에 관심영역 box를 그려서 보여준다.
+
+사용예:
+  python temp_check_csv.py --image_path=.\images --csv_path=.\data.csv
+"""
+
+# 각 레코드를 파싱하기 위한 함수 정의
+def parse_record(record):
+    # 레코드의 feature 정의
+    feature_description = {
+        'image/encoded': tf.io.FixedLenFeature([], tf.string),
+        'image/object/class/text': tf.io.VarLenFeature(tf.string),
+        'image/object/bbox/xmin' : tf.io.VarLenFeature(tf.float32),
+        'image/object/bbox/xmax': tf.io.VarLenFeature(tf.float32),
+        'image/object/bbox/ymin': tf.io.VarLenFeature(tf.float32),
+        'image/object/bbox/ymax': tf.io.VarLenFeature(tf.float32),
+        'image/width' : tf.io.VarLenFeature(tf.int64),
+        'image/height': tf.io.VarLenFeature(tf.int64),
+        'image/filename' : tf.io.FixedLenFeature([], tf.string)
+    }
+    # 레코드 파싱
+    parsed_record = tf.io.parse_single_example(record, feature_description)
+    # 이미지 데이터 디코딩
+    image = tf.io.decode_image(parsed_record['image/encoded'])
+    # 레이블 추출
+    label = parsed_record['image/object/class/text']
+    xmin = parsed_record['image/object/bbox/xmin']
+    xmax = parsed_record['image/object/bbox/xmax']
+    ymin = parsed_record['image/object/bbox/ymin']
+    ymax = parsed_record['image/object/bbox/ymax']
+    filename = parsed_record['image/filename']
+    return image, label, filename, xmin, xmax, ymin, ymax
+
+def tfrecord_valid_check(tfrecord_path):
+    # for example in tf.io..tf_record_iterator(tfrecord_path):
+    #     print(tf.train.Example.FromString(example))
+
+    if os.path.exists(tfrecord_path):
+        # 지정된 tfrecord 파일에 대한 데이터셋을 만듬.
+        dataset = tf.data.TFRecordDataset(tfrecord_path)
+
+        # 데이터셋에 map 함수를 사용하여 각 레코드 파싱
+        parsed_dataset = dataset.map(parse_record)
+
+        # 데이터셋 순회
+        for image, label, filename, xmin, xmax, ymin, ymax in parsed_dataset:
+
+            # 이미지 출력
+            h, w, c = image.shape
+            image = image.numpy()
+            image = cv2.cvtColor(image, cv2.COLOR_BGR2RGB)
+            xmin = tf.sparse.to_dense(xmin, default_value=0.0).numpy()
+            xmax = tf.sparse.to_dense(xmax, default_value=0.0).numpy()
+            ymin = tf.sparse.to_dense(ymin, default_value=0.0).numpy()
+            ymax = tf.sparse.to_dense(ymax, default_value=0.0).numpy()
+            label = tf.sparse.to_dense(label, default_value='???').numpy()
+
+            # 레이블 출력
+            for idx in np.arange(0, len(label)):
+                print(f'filename:{filename}  label:{label[idx]} > xmin:{xmin[idx]} xmax:{xmax[idx]} ymin:{ymin[idx]} ymax:{ymax[idx]}')
+                cv2.rectangle(image, (int(xmin[idx] * w), int(ymin[idx] * h)), (int(xmax[idx] * w), int(ymax[idx] * h)), (255, 255, 0), 2)
+
+            cv2.imshow('image', image)
+
+
+
+        # for d in raw_dataset:
+        #     ex = tf.train.Example()
+        #     ex.ParseFromString(d.numpy())
+        #     m = json.loads(MessageToJson(ex))
+        #     print(m['features']['feature'].keys())
+
+        # for raw_record in dataset:
+        #     example = tf.train.Example()
+        #     example.ParseFromString(raw_record.numpy())
+        #     print(example)
+        #     print('-----------------------------------------------------------')
+            key = cv2.waitKey(0)
+            if key == 27:
+                break
```

### Comparing `hyutils-hyutil-hoyun-lab-0.0.3/src/hyutil_hoyun_lab/xml_util.py` & `hyutils-hyutil-hoyun-lab-0.0.4/src/hyutil_hoyun_lab/xml_util.py`

 * *Files identical despite different names*

### Comparing `hyutils-hyutil-hoyun-lab-0.0.3/src/hyutils_hyutil_hoyun_lab.egg-info/PKG-INFO` & `hyutils-hyutil-hoyun-lab-0.0.4/src/hyutils_hyutil_hoyun_lab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyutils-hyutil-hoyun-lab
-Version: 0.0.3
+Version: 0.0.4
 Summary: Hoyun Lab Python Utils
 Home-page: https://www.hoyun.co.kr
 Author: nohgan im
 Author-email: fory2k@hoyun.co.kr
 License: MIT
 Project-URL: Bug Tracker, https://github.com/schooldevops/python-tutorials/issues
 Classifier: Programming Language :: Python :: 3
```

