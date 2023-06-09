# Comparing `tmp/krutils-0.20230607.2323.tar.gz` & `tmp/krutils-0.20230609.1515.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krutils-0.20230607.2323.tar", last modified: Wed Jun  7 14:23:32 2023, max compression
+gzip compressed data, was "krutils-0.20230609.1515.tar", last modified: Fri Jun  9 06:15:16 2023, max compression
```

## Comparing `krutils-0.20230607.2323.tar` & `krutils-0.20230609.1515.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 14:23:32.339423 krutils-0.20230607.2323/
--rw-rw-rw-   0        0        0      526 2023-06-07 14:23:32.330326 krutils-0.20230607.2323/PKG-INFO
--rw-rw-rw-   0        0        0      500 2023-05-25 04:35:41.000000 krutils-0.20230607.2323/README.md
-drwxrwxrwx   0        0        0        0 2023-06-07 14:23:32.249174 krutils-0.20230607.2323/krutils/
--rw-rw-rw-   0        0        0      455 2022-04-21 08:14:50.000000 krutils-0.20230607.2323/krutils/AppErr.py
--rw-rw-rw-   0        0        0     1741 2023-04-11 07:38:24.000000 krutils-0.20230607.2323/krutils/CONST.py
--rw-rw-rw-   0        0        0       94 2023-06-06 15:37:21.000000 krutils-0.20230607.2323/krutils/__init__.py
--rw-rw-rw-   0        0        0     5471 2023-04-11 07:45:04.000000 krutils-0.20230607.2323/krutils/_dbmgr.py
--rw-rw-rw-   0        0        0     2721 2023-06-06 09:07:19.000000 krutils-0.20230607.2323/krutils/futils.py
--rw-rw-rw-   0        0        0    12556 2023-06-06 16:39:50.000000 krutils-0.20230607.2323/krutils/logger.py
--rw-rw-rw-   0        0        0      669 2023-06-06 17:38:05.000000 krutils-0.20230607.2323/krutils/logger2.py
--rw-rw-rw-   0        0        0    18188 2023-06-07 14:23:27.000000 krutils-0.20230607.2323/krutils/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-07 14:23:32.300323 krutils-0.20230607.2323/krutils.egg-info/
--rw-rw-rw-   0        0        0      526 2023-06-07 14:23:31.000000 krutils-0.20230607.2323/krutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      357 2023-06-07 14:23:32.000000 krutils-0.20230607.2323/krutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 14:23:31.000000 krutils-0.20230607.2323/krutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-06-07 14:23:31.000000 krutils-0.20230607.2323/krutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-07 14:23:31.000000 krutils-0.20230607.2323/krutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-07 14:23:32.340349 krutils-0.20230607.2323/setup.cfg
--rw-rw-rw-   0        0        0      890 2023-06-07 14:23:30.000000 krutils-0.20230607.2323/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-07 14:23:32.319668 krutils-0.20230607.2323/test/
--rw-rw-rw-   0        0        0      349 2023-05-22 06:46:23.000000 krutils-0.20230607.2323/test/test_futils.py
--rw-rw-rw-   0        0        0      235 2023-06-07 13:45:35.000000 krutils-0.20230607.2323/test/test_logger.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:15:16.410208 krutils-0.20230609.1515/
+-rw-rw-rw-   0        0        0      526 2023-06-09 06:15:16.384976 krutils-0.20230609.1515/PKG-INFO
+-rw-rw-rw-   0        0        0      500 2023-05-25 04:35:41.000000 krutils-0.20230609.1515/README.md
+drwxrwxrwx   0        0        0        0 2023-06-09 06:15:16.030764 krutils-0.20230609.1515/krutils/
+-rw-rw-rw-   0        0        0      455 2022-04-21 08:14:50.000000 krutils-0.20230609.1515/krutils/AppErr.py
+-rw-rw-rw-   0        0        0     1741 2023-04-11 07:38:24.000000 krutils-0.20230609.1515/krutils/CONST.py
+-rw-rw-rw-   0        0        0      115 2023-06-07 14:26:39.000000 krutils-0.20230609.1515/krutils/__init__.py
+-rw-rw-rw-   0        0        0     5471 2023-04-11 07:45:04.000000 krutils-0.20230609.1515/krutils/_dbmgr.py
+-rw-rw-rw-   0        0        0     2933 2023-06-09 06:14:27.000000 krutils-0.20230609.1515/krutils/futils.py
+-rw-rw-rw-   0        0        0    12812 2023-06-09 06:11:45.000000 krutils-0.20230609.1515/krutils/logger.py
+-rw-rw-rw-   0        0        0      669 2023-06-06 17:38:05.000000 krutils-0.20230609.1515/krutils/logger2.py
+-rw-rw-rw-   0        0        0    18188 2023-06-07 14:23:27.000000 krutils-0.20230609.1515/krutils/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:15:16.278864 krutils-0.20230609.1515/krutils.egg-info/
+-rw-rw-rw-   0        0        0      526 2023-06-09 06:15:15.000000 krutils-0.20230609.1515/krutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      357 2023-06-09 06:15:15.000000 krutils-0.20230609.1515/krutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 06:15:15.000000 krutils-0.20230609.1515/krutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-06-09 06:15:15.000000 krutils-0.20230609.1515/krutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-09 06:15:15.000000 krutils-0.20230609.1515/krutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-09 06:15:16.412361 krutils-0.20230609.1515/setup.cfg
+-rw-rw-rw-   0        0        0      890 2023-06-09 06:15:13.000000 krutils-0.20230609.1515/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:15:16.380453 krutils-0.20230609.1515/test/
+-rw-rw-rw-   0        0        0      349 2023-05-22 06:46:23.000000 krutils-0.20230609.1515/test/test_futils.py
+-rw-rw-rw-   0        0        0      231 2023-06-07 14:23:57.000000 krutils-0.20230609.1515/test/test_logger.py
```

### Comparing `krutils-0.20230607.2323/PKG-INFO` & `krutils-0.20230609.1515/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krutils
-Version: 0.20230607.2323
+Version: 0.20230609.1515
 Summary: Some utils for me.
 Author: bonfireof
 Author-email: bonfireof@gmail.com
 Project-URL: Bug Tracker, https://github.com/bonfireof/krutils
 Project-URL: Documentation, https://github.com/bonfireof/krutils
 Project-URL: Source Code, https://github.com/bonfireof/krutils
 Classifier: Programming Language :: Python :: 3
```

### Comparing `krutils-0.20230607.2323/krutils/CONST.py` & `krutils-0.20230609.1515/krutils/CONST.py`

 * *Files identical despite different names*

### Comparing `krutils-0.20230607.2323/krutils/_dbmgr.py` & `krutils-0.20230609.1515/krutils/_dbmgr.py`

 * *Files identical despite different names*

### Comparing `krutils-0.20230607.2323/krutils/futils.py` & `krutils-0.20230609.1515/krutils/futils.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,15 +30,19 @@
     curr_dir = os.path.dirname(caller_file)
     # print("curr_dir[{0}]".format(curr_dir))
 
     file_path = ""
     for ii in range(100):
         # print(curr_dir, file_name, "찾는중이다")
 
-        if (os.path.isfile(os.path.join(curr_dir, file_name)) == True):
+        if (os.path.isfile(file_name) == True):      # 가상환경에서는 디렉토리정보가 없다!!?
+            file_path = file_name
+            # print("찾았다!", file_path)
+            break
+        elif (os.path.isfile(os.path.join(curr_dir, file_name)) == True):
             file_path = os.path.join(curr_dir, file_name)
             # print("찾았다!", file_path)
             break
         else:
             # print("상위로 찾아 올라간다[{0}]->[{1}]".format(curr_dir, os.path.abspath(os.path.join(curr_dir, '..'))))
             # root까지 확인된 경우 : 더이상 찾을 수 없을 때
             if (curr_dir == os.path.abspath(os.path.join(curr_dir, '..'))):
```

### Comparing `krutils-0.20230607.2323/krutils/logger.py` & `krutils-0.20230609.1515/krutils/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,19 @@
         curr_dir = os.path.dirname(start_path)
         CONFIG_FILE_NAME = 'logger.json'
 
         config_file_path = ""
         for ii in range(5):
             # print("seeking..[{0}]th : {1}".format(ii, curr_dir))
 
-            if (os.path.isfile(curr_dir + "/" + CONFIG_FILE_NAME) == True):
+            if (os.path.isfile(CONFIG_FILE_NAME) == True):      # 가상환경에서는 디렉토리정보가 없다!!?
+                config_file_path = CONFIG_FILE_NAME
+                # print("찾았다!", config_file_path)
+                break
+            elif (os.path.isfile(curr_dir + "/" + CONFIG_FILE_NAME) == True):
                 config_file_path = os.path.join(curr_dir, CONFIG_FILE_NAME)
                 # print("찾았다!", config_file_path)
                 break
             else:
                 # print("상위로 찾아 올라간다[{0}]->[{1}]".format(curr_dir, os.path.abspath(os.path.join(curr_dir, '..'))))
                 # root까지 확인된 경우 : 더이상 찾을 수 없을 때
                 if (curr_dir == os.path.abspath(os.path.join(curr_dir, '..'))):
```

### Comparing `krutils-0.20230607.2323/krutils/logger2.py` & `krutils-0.20230609.1515/krutils/logger2.py`

 * *Files identical despite different names*

### Comparing `krutils-0.20230607.2323/krutils/utils.py` & `krutils-0.20230609.1515/krutils/utils.py`

 * *Files identical despite different names*

### Comparing `krutils-0.20230607.2323/krutils.egg-info/PKG-INFO` & `krutils-0.20230609.1515/krutils.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krutils
-Version: 0.20230607.2323
+Version: 0.20230609.1515
 Summary: Some utils for me.
 Author: bonfireof
 Author-email: bonfireof@gmail.com
 Project-URL: Bug Tracker, https://github.com/bonfireof/krutils
 Project-URL: Documentation, https://github.com/bonfireof/krutils
 Project-URL: Source Code, https://github.com/bonfireof/krutils
 Classifier: Programming Language :: Python :: 3
```

### Comparing `krutils-0.20230607.2323/setup.py` & `krutils-0.20230609.1515/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="krutils",
-    version="0.20230607.2323",
+    version="0.20230609.1515",
     author="bonfireof",
     author_email="bonfireof@gmail.com",
     description="Some utils for me.",
     project_urls={
         "Bug Tracker": "https://github.com/bonfireof/krutils",
         "Documentation": "https://github.com/bonfireof/krutils",
         "Source Code": "https://github.com/bonfireof/krutils",
```

