# Comparing `tmp/bkapi-plugins-py-0.525.tar.gz` & `tmp/bkapi-plugins-py-0.609.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bkapi-plugins-py-0.525.tar", last modified: Thu May 25 05:28:41 2023, max compression
+gzip compressed data, was "bkapi-plugins-py-0.609.tar", last modified: Fri Jun  9 03:15:32 2023, max compression
```

## Comparing `bkapi-plugins-py-0.525.tar` & `bkapi-plugins-py-0.609.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 05:28:41.232976 bkapi-plugins-py-0.525/
--rw-rw-rw-   0        0        0       39 2023-04-17 10:01:55.000000 bkapi-plugins-py-0.525/MANIFEST.in
--rw-rw-rw-   0        0        0      257 2023-05-25 05:28:41.233977 bkapi-plugins-py-0.525/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-25 05:28:41.221976 bkapi-plugins-py-0.525/bkapi_plugins/
-drwxrwxrwx   0        0        0        0 2023-05-25 05:28:41.226977 bkapi-plugins-py-0.525/bkapi_plugins/files/
--rw-rw-rw-   0        0        0   177080 2023-05-25 05:26:18.000000 bkapi-plugins-py-0.525/bkapi_plugins/files/nginx_upstream_check_module-master.zip
-drwxrwxrwx   0        0        0        0 2023-05-25 05:28:41.231982 bkapi-plugins-py-0.525/bkapi_plugins_py.egg-info/
--rw-rw-rw-   0        0        0      257 2023-05-25 05:28:41.000000 bkapi-plugins-py-0.525/bkapi_plugins_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2023-05-25 05:28:41.000000 bkapi-plugins-py-0.525/bkapi_plugins_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 05:28:41.000000 bkapi-plugins-py-0.525/bkapi_plugins_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 05:28:41.000000 bkapi-plugins-py-0.525/bkapi_plugins_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-25 05:28:41.235978 bkapi-plugins-py-0.525/setup.cfg
--rw-rw-rw-   0        0        0      890 2023-05-25 05:28:21.000000 bkapi-plugins-py-0.525/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 03:15:32.591632 bkapi-plugins-py-0.609/
+-rw-rw-rw-   0        0        0       39 2023-04-17 10:01:55.000000 bkapi-plugins-py-0.609/MANIFEST.in
+-rw-rw-rw-   0        0        0      257 2023-06-09 03:15:32.592630 bkapi-plugins-py-0.609/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-09 03:15:32.580668 bkapi-plugins-py-0.609/bkapi_plugins/
+drwxrwxrwx   0        0        0        0 2023-06-09 03:15:32.585653 bkapi-plugins-py-0.609/bkapi_plugins/files/
+-rw-rw-rw-   0        0        0     1501 2023-06-09 02:58:11.000000 bkapi-plugins-py-0.609/bkapi_plugins/files/table-confluence.py
+drwxrwxrwx   0        0        0        0 2023-06-09 03:15:32.591632 bkapi-plugins-py-0.609/bkapi_plugins_py.egg-info/
+-rw-rw-rw-   0        0        0      257 2023-06-09 03:15:32.000000 bkapi-plugins-py-0.609/bkapi_plugins_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2023-06-09 03:15:32.000000 bkapi-plugins-py-0.609/bkapi_plugins_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 03:15:32.000000 bkapi-plugins-py-0.609/bkapi_plugins_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 03:15:32.000000 bkapi-plugins-py-0.609/bkapi_plugins_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-09 03:15:32.593625 bkapi-plugins-py-0.609/setup.cfg
+-rw-rw-rw-   0        0        0      890 2023-06-09 03:05:03.000000 bkapi-plugins-py-0.609/setup.py
```

### Comparing `bkapi-plugins-py-0.525/setup.py` & `bkapi-plugins-py-0.609/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 readme = ''
 
 setup(
     description='',
     long_description=readme,
     name='bkapi-plugins-py', # 包的名字
-    version='0.525', # 版本号每次打包完要改一下
+    version='0.609', # 版本号每次打包完要改一下
     python_requires='>=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*',
     author='fadewalk',
     license='Apach License 2.0',
     # packages=find_packages(),
     # namespace_packages=['bkapi_plugins'],
     package_dir={'': '.'},
     include_package_data=True,
```

