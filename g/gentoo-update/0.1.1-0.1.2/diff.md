# Comparing `tmp/gentoo_update-0.1.1.tar.gz` & `tmp/gentoo-update-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gentoo_update-0.1.1.tar", last modified: Mon Jun  5 21:44:29 2023, max compression
+gzip compressed data, was "gentoo-update-0.1.2.tar", last modified: Thu Jun  8 22:52:08 2023, max compression
```

## Comparing `gentoo_update-0.1.1.tar` & `gentoo-update-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:44:29.005976 gentoo_update-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-05 21:44:20.000000 gentoo_update-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-06-05 21:44:29.005976 gentoo_update-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-05 21:44:20.000000 gentoo_update-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:44:29.005976 gentoo_update-0.1.1/gentoo_update.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-06-05 21:44:28.000000 gentoo_update-0.1.1/gentoo_update.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-05 21:44:29.000000 gentoo_update-0.1.1/gentoo_update.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 21:44:28.000000 gentoo_update-0.1.1/gentoo_update.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-05 21:44:28.000000 gentoo_update-0.1.1/gentoo_update.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-05 21:44:28.000000 gentoo_update-0.1.1/gentoo_update.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-06-05 21:44:20.000000 gentoo_update-0.1.1/gentoo_update.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-05 21:44:29.005976 gentoo_update-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 21:44:20.000000 gentoo_update-0.1.1/setup.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4545 2023-06-05 21:44:20.000000 gentoo_update-0.1.1/updater.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:52:08.308775 gentoo-update-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-08 22:51:56.000000 gentoo-update-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-08 22:52:08.308775 gentoo-update-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-08 22:51:56.000000 gentoo-update-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:52:08.308775 gentoo-update-0.1.2/gentoo_update/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-08 22:51:56.000000 gentoo-update-0.1.2/gentoo_update/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-06-08 22:51:56.000000 gentoo-update-0.1.2/gentoo_update/gentoo_update.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4545 2023-06-08 22:51:56.000000 gentoo-update-0.1.2/gentoo_update/updater.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:52:08.308775 gentoo-update-0.1.2/gentoo_update.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-08 22:52:08.000000 gentoo-update-0.1.2/gentoo_update.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-08 22:52:08.000000 gentoo-update-0.1.2/gentoo_update.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 22:52:08.000000 gentoo-update-0.1.2/gentoo_update.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-08 22:52:08.000000 gentoo-update-0.1.2/gentoo_update.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-08 22:52:08.000000 gentoo-update-0.1.2/gentoo_update.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-08 22:52:08.308775 gentoo-update-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 22:51:56.000000 gentoo-update-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:52:08.308775 gentoo-update-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-08 22:51:56.000000 gentoo-update-0.1.2/tests/test_updater.py
```

### Comparing `gentoo_update-0.1.1/LICENSE` & `gentoo-update-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gentoo_update-0.1.1/README.md` & `gentoo-update-0.1.2/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -28,26 +28,9 @@
 
 * Full system update, show elogs and news
 ```bash
 gentoo-update --update-mode full --read-logs y --read-news y
 ```
 
 The detailed explanation of command flags can be found in `--help`.  
-
-
-#### Testing
-**Note** Testing will be automated in the future, right now it's a bit hackish
-In `gentoo_update/tests` there is a Docker Compose file that 
-can be used for testing. It builds containers based on stage3 
-tarballs and mounts the source code to `/root/gentoo_update_source`.  
-
-Example of a test:
-```bash
-cd tests
-docker compose up gentoo1 -d
-docker exec -it tests-gentoo1-1 /bin/bash
-
-# inside container
-cd /root/gentoo_update_source
-python gentoo_update.python
-```
-
+Information on testing can be found in tests directory 
+[readme](gentoo_update/blob/main/tests/README.md)
```

### Comparing `gentoo_update-0.1.1/gentoo_update.py` & `gentoo-update-0.1.2/gentoo_update/gentoo_update.py`

 * *Files identical despite different names*

### Comparing `gentoo_update-0.1.1/setup.cfg` & `gentoo-update-0.1.2/setup.cfg`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
-name = gentoo_update
-version = 0.1.1
+name = gentoo-update
+version = 0.1.2
 description = Gentoo Linux updater
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Lab-Brat
 author_email = labbrat_social@pm.me
 url = https://github.com/Lab-Brat/gentoo_update
 license = MIT
@@ -12,17 +12,17 @@
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3.10
 	Operating System :: POSIX :: Linux
 
 [options]
 python_requires = >=3.9
 include_package_data = True
-scripts = updater.sh
+scripts = gentoo_update/updater.sh
 
 [options.entry_points]
 console_scripts = 
-	gentoo-update = gentoo_update:main
+	gentoo-update = gentoo_update.gentoo_update:main
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `gentoo_update-0.1.1/updater.sh` & `gentoo-update-0.1.2/gentoo_update/updater.sh`

 * *Files identical despite different names*

