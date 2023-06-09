# Comparing `tmp/mvtech-plugin-1.0.6.tar.gz` & `tmp/mvtech-plugin-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mvtech-plugin-1.0.6.tar", last modified: Wed Jun  7 07:55:42 2023, max compression
+gzip compressed data, was "dist\mvtech-plugin-1.0.7.tar", last modified: Fri Jun  9 01:03:56 2023, max compression
```

## Comparing `mvtech-plugin-1.0.6.tar` & `mvtech-plugin-1.0.7.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 07:55:42.502571 mvtech-plugin-1.0.6/
--rw-rw-rw-   0        0        0       31 2023-03-27 00:54:56.000000 mvtech-plugin-1.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0     2630 2023-06-07 07:55:42.503568 mvtech-plugin-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     2353 2023-06-07 02:22:15.000000 mvtech-plugin-1.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-07 07:55:42.481782 mvtech-plugin-1.0.6/core/
--rw-rw-rw-   0        0        0       21 2023-06-07 07:54:18.000000 mvtech-plugin-1.0.6/core/__init__.py
--rw-rw-rw-   0        0        0    10018 2023-06-05 09:44:22.000000 mvtech-plugin-1.0.6/core/cli_methods.py
--rw-rw-rw-   0        0        0    14629 2023-06-07 07:38:51.000000 mvtech-plugin-1.0.6/core/config.py
--rw-rw-rw-   0        0        0     1637 2023-03-27 01:06:38.000000 mvtech-plugin-1.0.6/core/main.py
-drwxrwxrwx   0        0        0        0 2023-06-07 07:55:42.483776 mvtech-plugin-1.0.6/core/res/
-drwxrwxrwx   0        0        0        0 2023-06-07 07:55:42.493750 mvtech-plugin-1.0.6/core/res/SDK/
--rw-rw-rw-   0        0        0        0 2023-01-29 09:23:09.000000 mvtech-plugin-1.0.6/core/res/SDK/__init__.py
--rw-rw-rw-   0        0        0     7829 2023-02-15 05:39:36.000000 mvtech-plugin-1.0.6/core/res/SDK/base.py
--rw-rw-rw-   0        0        0     2126 2023-06-07 03:13:07.000000 mvtech-plugin-1.0.6/core/res/SDK/cli.py
--rw-rw-rw-   0        0        0     4643 2023-03-27 00:56:18.000000 mvtech-plugin-1.0.6/core/res/SDK/http_run.py
--rw-rw-rw-   0        0        0      162 2023-03-27 00:44:29.000000 mvtech-plugin-1.0.6/core/res/SDK/models.py
--rw-rw-rw-   0        0        0      463 2023-03-27 01:09:02.000000 mvtech-plugin-1.0.6/core/res/SDK/plugin.py
--rw-rw-rw-   0        0        0    12776 2023-06-05 09:23:34.000000 mvtech-plugin-1.0.6/core/res/SDK/run_define.py
--rw-rw-rw-   0        0        0     1719 2023-02-20 08:33:11.000000 mvtech-plugin-1.0.6/core/res/SDK/service_stop.py
--rw-rw-rw-   0        0        0     5323 2023-06-05 09:24:15.000000 mvtech-plugin-1.0.6/core/res/SDK/web.py
--rw-rw-rw-   0        0        0        0 2023-01-29 09:23:09.000000 mvtech-plugin-1.0.6/core/res/__init__.py
--rw-rw-rw-   0        0        0    37636 2023-06-06 01:54:59.000000 mvtech-plugin-1.0.6/core/res/project.tar.gz
--rw-rw-rw-   0        0        0     3473 2023-02-03 02:21:28.000000 mvtech-plugin-1.0.6/core/tools.py
-drwxrwxrwx   0        0        0        0 2023-06-07 07:55:42.502571 mvtech-plugin-1.0.6/mvtech_plugin.egg-info/
--rw-rw-rw-   0        0        0     2630 2023-06-07 07:55:42.000000 mvtech-plugin-1.0.6/mvtech_plugin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      601 2023-06-07 07:55:42.000000 mvtech-plugin-1.0.6/mvtech_plugin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 07:55:42.000000 mvtech-plugin-1.0.6/mvtech_plugin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-06-07 07:55:42.000000 mvtech-plugin-1.0.6/mvtech_plugin.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       67 2023-06-07 07:55:42.000000 mvtech-plugin-1.0.6/mvtech_plugin.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-07 07:55:42.000000 mvtech-plugin-1.0.6/mvtech_plugin.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-07 07:55:42.503763 mvtech-plugin-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1236 2023-02-03 03:01:22.000000 mvtech-plugin-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 01:03:56.604062 mvtech-plugin-1.0.7/
+-rw-rw-rw-   0        0        0       31 2023-03-27 00:54:56.000000 mvtech-plugin-1.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     2680 2023-06-09 01:03:56.604062 mvtech-plugin-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2403 2023-06-09 01:03:19.000000 mvtech-plugin-1.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-09 01:03:56.588102 mvtech-plugin-1.0.7/core/
+-rw-rw-rw-   0        0        0       21 2023-06-09 01:03:32.000000 mvtech-plugin-1.0.7/core/__init__.py
+-rw-rw-rw-   0        0        0    10018 2023-06-05 09:44:22.000000 mvtech-plugin-1.0.7/core/cli_methods.py
+-rw-rw-rw-   0        0        0    14629 2023-06-07 07:38:51.000000 mvtech-plugin-1.0.7/core/config.py
+-rw-rw-rw-   0        0        0     1637 2023-03-27 01:06:38.000000 mvtech-plugin-1.0.7/core/main.py
+drwxrwxrwx   0        0        0        0 2023-06-09 01:03:56.589104 mvtech-plugin-1.0.7/core/res/
+drwxrwxrwx   0        0        0        0 2023-06-09 01:03:56.598084 mvtech-plugin-1.0.7/core/res/SDK/
+-rw-rw-rw-   0        0        0        0 2023-01-29 09:23:09.000000 mvtech-plugin-1.0.7/core/res/SDK/__init__.py
+-rw-rw-rw-   0        0        0     7829 2023-02-15 05:39:36.000000 mvtech-plugin-1.0.7/core/res/SDK/base.py
+-rw-rw-rw-   0        0        0     2126 2023-06-07 03:13:07.000000 mvtech-plugin-1.0.7/core/res/SDK/cli.py
+-rw-rw-rw-   0        0        0     4643 2023-03-27 00:56:18.000000 mvtech-plugin-1.0.7/core/res/SDK/http_run.py
+-rw-rw-rw-   0        0        0      162 2023-03-27 00:44:29.000000 mvtech-plugin-1.0.7/core/res/SDK/models.py
+-rw-rw-rw-   0        0        0      463 2023-03-27 01:09:02.000000 mvtech-plugin-1.0.7/core/res/SDK/plugin.py
+-rw-rw-rw-   0        0        0    12776 2023-06-05 09:23:34.000000 mvtech-plugin-1.0.7/core/res/SDK/run_define.py
+-rw-rw-rw-   0        0        0     1719 2023-02-20 08:33:11.000000 mvtech-plugin-1.0.7/core/res/SDK/service_stop.py
+-rw-rw-rw-   0        0        0     5323 2023-06-05 09:24:15.000000 mvtech-plugin-1.0.7/core/res/SDK/web.py
+-rw-rw-rw-   0        0        0        0 2023-01-29 09:23:09.000000 mvtech-plugin-1.0.7/core/res/__init__.py
+-rw-rw-rw-   0        0        0    38085 2023-06-09 00:58:19.000000 mvtech-plugin-1.0.7/core/res/project.tar.gz
+-rw-rw-rw-   0        0        0     3473 2023-02-03 02:21:28.000000 mvtech-plugin-1.0.7/core/tools.py
+drwxrwxrwx   0        0        0        0 2023-06-09 01:03:56.604062 mvtech-plugin-1.0.7/mvtech_plugin.egg-info/
+-rw-rw-rw-   0        0        0     2680 2023-06-09 01:03:56.000000 mvtech-plugin-1.0.7/mvtech_plugin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      601 2023-06-09 01:03:56.000000 mvtech-plugin-1.0.7/mvtech_plugin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 01:03:56.000000 mvtech-plugin-1.0.7/mvtech_plugin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-06-09 01:03:56.000000 mvtech-plugin-1.0.7/mvtech_plugin.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       67 2023-06-09 01:03:56.000000 mvtech-plugin-1.0.7/mvtech_plugin.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-09 01:03:56.000000 mvtech-plugin-1.0.7/mvtech_plugin.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-09 01:03:56.605214 mvtech-plugin-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1236 2023-02-03 03:01:22.000000 mvtech-plugin-1.0.7/setup.py
```

### Comparing `mvtech-plugin-1.0.6/PKG-INFO` & `mvtech-plugin-1.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mvtech-plugin
-Version: 1.0.6
+Version: 1.0.7
 Summary: 插件生成等功能...
 Home-page: https://www.mvtech.cn/market/introduction
 Author: sandy
 Author-email: tong@mvtech.com.cn
 License: MIT
 Requires-Python: >=3
 Description-Content-Type: text/markdown
@@ -28,14 +28,15 @@
 ├── Dockerfile
 ├── help.md
 ├── icon.png
 ├── main.py
 ├── Makefile
 ├── ?_plugin.yaml
 ├── requirements.txt
+├── make_image.sh
 ├── SDK
 │   ├── base.py
 │   ├── cli.py
 │   ├── __init__.py
 │   ├── models.py
 │   ├── plugin.py
 │   ├── run_define.py
@@ -48,14 +49,15 @@
 ```
 
 - ?_plugin.yaml: 模板文件，定义插件．
 - actions/???.py: 根据模板文件定义生成动作．
 - triggers/???.py: 根据模板文件定义生成触发器．
 - actions/models.py 和 triggers/models.py: 模板文件继承pydantic
 - testAPI: FastAPI测试入口
+- make_image.sh 打包脚本
 
 #### 环境要求
 
 - python3.+
 
 #### 安装 依赖
 
@@ -69,15 +71,15 @@
 
 #### 脚手架生成的压缩包解压后执行下面命令安装
 
     python setup.py install
 
 #### 脚手架卸载
 
-    pip uninstall mvtech-plugin 1.0.0 -y
+    pip uninstall mvtech-plugin  -y
 
 #### 脚手架使用
 
     执行本地脚手架
     mvtech-plugin -h
 
 ```
```

### Comparing `mvtech-plugin-1.0.6/README.md` & `mvtech-plugin-1.0.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 ├── Dockerfile
 ├── help.md
 ├── icon.png
 ├── main.py
 ├── Makefile
 ├── ?_plugin.yaml
 ├── requirements.txt
+├── make_image.sh
 ├── SDK
 │   ├── base.py
 │   ├── cli.py
 │   ├── __init__.py
 │   ├── models.py
 │   ├── plugin.py
 │   ├── run_define.py
@@ -37,14 +38,15 @@
 ```
 
 - ?_plugin.yaml: 模板文件，定义插件．
 - actions/???.py: 根据模板文件定义生成动作．
 - triggers/???.py: 根据模板文件定义生成触发器．
 - actions/models.py 和 triggers/models.py: 模板文件继承pydantic
 - testAPI: FastAPI测试入口
+- make_image.sh 打包脚本
 
 #### 环境要求
 
 - python3.+
 
 #### 安装 依赖
 
@@ -58,15 +60,15 @@
 
 #### 脚手架生成的压缩包解压后执行下面命令安装
 
     python setup.py install
 
 #### 脚手架卸载
 
-    pip uninstall mvtech-plugin 1.0.0 -y
+    pip uninstall mvtech-plugin  -y
 
 #### 脚手架使用
 
     执行本地脚手架
     mvtech-plugin -h
 
 ```
```

### Comparing `mvtech-plugin-1.0.6/core/cli_methods.py` & `mvtech-plugin-1.0.7/core/cli_methods.py`

 * *Files identical despite different names*

### Comparing `mvtech-plugin-1.0.6/core/config.py` & `mvtech-plugin-1.0.7/core/config.py`

 * *Files identical despite different names*

### Comparing `mvtech-plugin-1.0.6/core/main.py` & `mvtech-plugin-1.0.7/core/main.py`

 * *Files identical despite different names*

### Comparing `mvtech-plugin-1.0.6/core/res/SDK/base.py` & `mvtech-plugin-1.0.7/core/res/SDK/base.py`

 * *Files identical despite different names*

### Comparing `mvtech-plugin-1.0.6/core/res/SDK/cli.py` & `mvtech-plugin-1.0.7/core/res/SDK/cli.py`

 * *Files identical despite different names*

### Comparing `mvtech-plugin-1.0.6/core/res/SDK/http_run.py` & `mvtech-plugin-1.0.7/core/res/SDK/http_run.py`

 * *Files identical despite different names*

### Comparing `mvtech-plugin-1.0.6/core/res/SDK/run_define.py` & `mvtech-plugin-1.0.7/core/res/SDK/run_define.py`

 * *Files identical despite different names*

### Comparing `mvtech-plugin-1.0.6/core/res/SDK/service_stop.py` & `mvtech-plugin-1.0.7/core/res/SDK/service_stop.py`

 * *Files identical despite different names*

### Comparing `mvtech-plugin-1.0.6/core/res/SDK/web.py` & `mvtech-plugin-1.0.7/core/res/SDK/web.py`

 * *Files identical despite different names*

### Comparing `mvtech-plugin-1.0.6/core/res/project.tar.gz` & `mvtech-plugin-1.0.7/core/res/project.tar.gz`

 * *Files 27% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Tue Jun  6 01:54:55 2023, max speed, from FAT filesystem (MS-DOS, OS/2, NT)
+gzip compressed data, last modified: Fri Jun  9 00:58:14 2023, max speed, from FAT filesystem (MS-DOS, OS/2, NT)
```

#### project.tar

##### file list

```diff
@@ -1,10 +1,11 @@
 -rwxrwxrwx   0        0        0      842 2023-03-25 01:50:57.000000 ./Dockerfile
 -rw-r--r--   0 andy      (1000) andy      (1000)    29297 2021-07-26 09:20:11.000000 ./icon.png
 -rwxrwxrwx   0        0        0      897 2023-06-06 01:53:59.000000 ./Makefile
+-rwxrwxrwx   0        0        0      825 2023-06-07 09:25:12.000000 ./make_image.sh
 -rwxr-xr-x   0 andy      (1000) andy      (1000)       66 2021-07-27 01:47:24.000000 ./requirements.txt
 drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2021-11-18 04:18:06.000000 ./SDK/
 -rwxrwxrwx   0        0        0     7829 2023-02-15 05:39:36.000000 ./SDK/base.py
 -rwxrwxrwx   0        0        0     2132 2023-06-05 07:27:02.000000 ./SDK/cli.py
 -rwxrwxrwx   0        0        0     5874 2023-02-20 06:58:57.000000 ./SDK/http_run.py
 -rwxrwxrwx   0        0        0      162 2023-03-27 00:44:29.000000 ./SDK/models.py
 -rwxrwxrwx   0        0        0      462 2023-03-27 00:41:14.000000 ./SDK/plugin.py
```

### Comparing `mvtech-plugin-1.0.6/core/tools.py` & `mvtech-plugin-1.0.7/core/tools.py`

 * *Files identical despite different names*

### Comparing `mvtech-plugin-1.0.6/mvtech_plugin.egg-info/PKG-INFO` & `mvtech-plugin-1.0.7/mvtech_plugin.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mvtech-plugin
-Version: 1.0.6
+Version: 1.0.7
 Summary: 插件生成等功能...
 Home-page: https://www.mvtech.cn/market/introduction
 Author: sandy
 Author-email: tong@mvtech.com.cn
 License: MIT
 Requires-Python: >=3
 Description-Content-Type: text/markdown
@@ -28,14 +28,15 @@
 ├── Dockerfile
 ├── help.md
 ├── icon.png
 ├── main.py
 ├── Makefile
 ├── ?_plugin.yaml
 ├── requirements.txt
+├── make_image.sh
 ├── SDK
 │   ├── base.py
 │   ├── cli.py
 │   ├── __init__.py
 │   ├── models.py
 │   ├── plugin.py
 │   ├── run_define.py
@@ -48,14 +49,15 @@
 ```
 
 - ?_plugin.yaml: 模板文件，定义插件．
 - actions/???.py: 根据模板文件定义生成动作．
 - triggers/???.py: 根据模板文件定义生成触发器．
 - actions/models.py 和 triggers/models.py: 模板文件继承pydantic
 - testAPI: FastAPI测试入口
+- make_image.sh 打包脚本
 
 #### 环境要求
 
 - python3.+
 
 #### 安装 依赖
 
@@ -69,15 +71,15 @@
 
 #### 脚手架生成的压缩包解压后执行下面命令安装
 
     python setup.py install
 
 #### 脚手架卸载
 
-    pip uninstall mvtech-plugin 1.0.0 -y
+    pip uninstall mvtech-plugin  -y
 
 #### 脚手架使用
 
     执行本地脚手架
     mvtech-plugin -h
 
 ```
```

### Comparing `mvtech-plugin-1.0.6/mvtech_plugin.egg-info/SOURCES.txt` & `mvtech-plugin-1.0.7/mvtech_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mvtech-plugin-1.0.6/setup.py` & `mvtech-plugin-1.0.7/setup.py`

 * *Files identical despite different names*

