# Comparing `tmp/crop_utils-4.3.2.tar.gz` & `tmp/crop_utils-4.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crop_utils-4.3.2.tar", last modified: Thu Jun  8 10:13:31 2023, max compression
+gzip compressed data, was "crop_utils-4.3.3.tar", last modified: Fri Jun  9 03:36:26 2023, max compression
```

## Comparing `crop_utils-4.3.2.tar` & `crop_utils-4.3.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 10:13:31.691264 crop_utils-4.3.2/
--rw-rw-rw-   0        0        0     1091 2021-10-21 02:22:48.000000 crop_utils-4.3.2/LICENSE
--rw-rw-rw-   0        0        0       52 2021-10-21 06:40:49.000000 crop_utils-4.3.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1997 2023-06-08 10:13:31.690267 crop_utils-4.3.2/PKG-INFO
--rw-rw-rw-   0        0        0      910 2023-05-20 07:34:16.000000 crop_utils-4.3.2/README.md
--rw-rw-rw-   0        0        0      108 2021-10-20 10:50:24.000000 crop_utils-4.3.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-08 10:13:31.691264 crop_utils-4.3.2/setup.cfg
--rw-rw-rw-   0        0        0      894 2023-06-08 10:13:24.000000 crop_utils-4.3.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-08 10:13:31.664261 crop_utils-4.3.2/src/
-drwxrwxrwx   0        0        0        0 2023-06-08 10:13:31.681261 crop_utils-4.3.2/src/crop_utils/
--rw-rw-rw-   0        0        0        4 2021-10-21 03:45:02.000000 crop_utils-4.3.2/src/crop_utils/__init__.py
--rw-rw-rw-   0        0        0     2157 2023-06-06 03:35:58.000000 crop_utils-4.3.2/src/crop_utils/html_slot_config.py
--rw-rw-rw-   0        0        0    63534 2023-06-07 06:16:06.000000 crop_utils-4.3.2/src/crop_utils/image.py
--rw-rw-rw-   0        0        0    43293 2023-06-08 09:08:58.000000 crop_utils-4.3.2/src/crop_utils/img_crop.py
-drwxrwxrwx   0        0        0        0 2023-06-08 10:13:31.688262 crop_utils-4.3.2/src/crop_utils.egg-info/
--rw-rw-rw-   0        0        0     1997 2023-06-08 10:13:31.000000 crop_utils-4.3.2/src/crop_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      318 2023-06-08 10:13:31.000000 crop_utils-4.3.2/src/crop_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 10:13:31.000000 crop_utils-4.3.2/src/crop_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-08 10:13:31.000000 crop_utils-4.3.2/src/crop_utils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 03:36:26.144504 crop_utils-4.3.3/
+-rw-rw-rw-   0        0        0     1091 2021-10-21 02:22:48.000000 crop_utils-4.3.3/LICENSE
+-rw-rw-rw-   0        0        0       52 2021-10-21 06:40:49.000000 crop_utils-4.3.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1997 2023-06-09 03:36:26.144504 crop_utils-4.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0      910 2023-06-08 10:13:45.000000 crop_utils-4.3.3/README.md
+-rw-rw-rw-   0        0        0      108 2021-10-20 10:50:24.000000 crop_utils-4.3.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-09 03:36:26.145514 crop_utils-4.3.3/setup.cfg
+-rw-rw-rw-   0        0        0      894 2023-06-09 03:36:10.000000 crop_utils-4.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 03:36:26.117506 crop_utils-4.3.3/src/
+drwxrwxrwx   0        0        0        0 2023-06-09 03:36:26.133507 crop_utils-4.3.3/src/crop_utils/
+-rw-rw-rw-   0        0        0        4 2021-10-21 03:45:02.000000 crop_utils-4.3.3/src/crop_utils/__init__.py
+-rw-rw-rw-   0        0        0     2157 2023-06-06 03:35:58.000000 crop_utils-4.3.3/src/crop_utils/html_slot_config.py
+-rw-rw-rw-   0        0        0    63534 2023-06-07 06:16:06.000000 crop_utils-4.3.3/src/crop_utils/image.py
+-rw-rw-rw-   0        0        0    43292 2023-06-09 03:36:10.000000 crop_utils-4.3.3/src/crop_utils/img_crop.py
+drwxrwxrwx   0        0        0        0 2023-06-09 03:36:26.142506 crop_utils-4.3.3/src/crop_utils.egg-info/
+-rw-rw-rw-   0        0        0     1997 2023-06-09 03:36:25.000000 crop_utils-4.3.3/src/crop_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      318 2023-06-09 03:36:25.000000 crop_utils-4.3.3/src/crop_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 03:36:25.000000 crop_utils-4.3.3/src/crop_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-09 03:36:25.000000 crop_utils-4.3.3/src/crop_utils.egg-info/top_level.txt
```

### Comparing `crop_utils-4.3.2/LICENSE` & `crop_utils-4.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `crop_utils-4.3.2/PKG-INFO` & `crop_utils-4.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crop_utils
-Version: 4.3.2
+Version: 4.3.3
 Summary: 鞋类ai识别
 Home-page: http://git.chaomy.com/libo/ecpro-utils.git
 Author: libo
 Author-email: 6878595@qq.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Description: 为了区分3.0与4.0版本，同时资源图与详情页也共用的一套裁剪逻辑代码。
@@ -74,14 +74,14 @@
         
         
         
         # 安装
         
         
         
-        pip install crop-utils==4.3.1 -i  https://pypi.python.org/simple/
+        pip install crop-utils==4.3.2 -i  https://pypi.python.org/simple/
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `crop_utils-4.3.2/README.md` & `crop_utils-4.3.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -65,8 +65,8 @@
 
 
 
 # 安装
 
 
 
-pip install crop-utils==4.3.1 -i  https://pypi.python.org/simple/
+pip install crop-utils==4.3.2 -i  https://pypi.python.org/simple/
```

### Comparing `crop_utils-4.3.2/setup.py` & `crop_utils-4.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="crop_utils",  # 包名称
-    version="4.3.2",  # 版本号
+    version="4.3.3",  # 版本号
     author="libo",
     author_email="6878595@qq.com",
     description="鞋类ai识别",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="http://git.chaomy.com/libo/ecpro-utils.git",
     project_urls={
```

### Comparing `crop_utils-4.3.2/src/crop_utils/html_slot_config.py` & `crop_utils-4.3.3/src/crop_utils/html_slot_config.py`

 * *Files identical despite different names*

### Comparing `crop_utils-4.3.2/src/crop_utils/image.py` & `crop_utils-4.3.3/src/crop_utils/image.py`

 * *Files identical despite different names*

### Comparing `crop_utils-4.3.2/src/crop_utils/img_crop.py` & `crop_utils-4.3.3/src/crop_utils/img_crop.py`

 * *Files 0% similar despite different names*

```diff
@@ -816,15 +816,15 @@
         #     crop_bottom, crop_bottom_name = crop_point.get(self.crop_sequence[flag_index]), self.crop_sequence[
         #         flag_index]
         #     if crop_bottom:
         #         break
         #     flag_index += 1
         if bottom_site in crop_point.keys():
             return crop_point[bottom_site]['bottom_site'], bottom_site
-        return crop_bottom['pic_bottom']['bottom_site'], 'pic_bottom'
+        return crop_point['pic_bottom']['bottom_site'], 'pic_bottom'
 
     def _alternative_interest_center(self, center, slot_height_or_width, transform_height_or_width,
                                      interest_left_or_top,
                                      interest_slot_height_or_width):
         center_ = center * transform_height_or_width
         # 在图片的范围内
         tag_1 = (center_ - interest_slot_height_or_width / 2 - interest_left_or_top) >= 0
```

### Comparing `crop_utils-4.3.2/src/crop_utils.egg-info/PKG-INFO` & `crop_utils-4.3.3/src/crop_utils.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crop-utils
-Version: 4.3.2
+Version: 4.3.3
 Summary: 鞋类ai识别
 Home-page: http://git.chaomy.com/libo/ecpro-utils.git
 Author: libo
 Author-email: 6878595@qq.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Description: 为了区分3.0与4.0版本，同时资源图与详情页也共用的一套裁剪逻辑代码。
@@ -74,14 +74,14 @@
         
         
         
         # 安装
         
         
         
-        pip install crop-utils==4.3.1 -i  https://pypi.python.org/simple/
+        pip install crop-utils==4.3.2 -i  https://pypi.python.org/simple/
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

