# Comparing `tmp/eyes_soatra-0.0.28.tar.gz` & `tmp/eyes_soatra-0.0.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eyes_soatra-0.0.28.tar", last modified: Wed Jun  7 04:41:05 2023, max compression
+gzip compressed data, was "eyes_soatra-0.0.29.tar", last modified: Fri Jun  9 08:20:35 2023, max compression
```

## Comparing `eyes_soatra-0.0.28.tar` & `eyes_soatra-0.0.29.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-07 04:41:05.932612 eyes_soatra-0.0.28/
--rw-r--r--   0 soatra     (501) staff       (20)       13 2023-05-02 07:13:47.000000 eyes_soatra-0.0.28/LICENSE
--rw-r--r--   0 soatra     (501) staff       (20)      835 2023-06-07 04:41:05.932464 eyes_soatra-0.0.28/PKG-INFO
--rw-r--r--   0 soatra     (501) staff       (20)      330 2023-06-02 06:41:30.000000 eyes_soatra-0.0.28/README.md
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-07 04:41:05.922459 eyes_soatra-0.0.28/eyes_soatra/
--rw-r--r--   0 soatra     (501) staff       (20)       28 2023-05-02 07:14:02.000000 eyes_soatra-0.0.28/eyes_soatra/__init__.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-07 04:41:05.923729 eyes_soatra-0.0.28/eyes_soatra/constant/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:45:06.000000 eyes_soatra-0.0.28/eyes_soatra/constant/__init__.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-07 04:41:05.923986 eyes_soatra-0.0.28/eyes_soatra/constant/depends/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:46:17.000000 eyes_soatra-0.0.28/eyes_soatra/constant/depends/__init__.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-07 04:41:05.924729 eyes_soatra-0.0.28/eyes_soatra/constant/depends/app_date/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:54:07.000000 eyes_soatra-0.0.28/eyes_soatra/constant/depends/app_date/__init__.py
--rw-r--r--   0 soatra     (501) staff       (20)      224 2023-05-25 08:54:38.000000 eyes_soatra-0.0.28/eyes_soatra/constant/depends/app_date/end.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-07 04:41:05.925779 eyes_soatra-0.0.28/eyes_soatra/constant/depends/app_date/formats/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-28 09:25:41.000000 eyes_soatra-0.0.28/eyes_soatra/constant/depends/app_date/formats/__init__.py
--rw-r--r--   0 soatra     (501) staff       (20)     6706 2023-05-28 08:16:55.000000 eyes_soatra-0.0.28/eyes_soatra/constant/depends/app_date/formats/end.py
--rw-r--r--   0 soatra     (501) staff       (20)     9568 2023-05-28 08:16:48.000000 eyes_soatra-0.0.28/eyes_soatra/constant/depends/app_date/formats/period.py
--rw-r--r--   0 soatra     (501) staff       (20)     1127 2023-05-28 08:16:41.000000 eyes_soatra-0.0.28/eyes_soatra/constant/depends/app_date/formats/start.py
--rw-r--r--   0 soatra     (501) staff       (20)      354 2023-05-29 02:27:50.000000 eyes_soatra-0.0.28/eyes_soatra/constant/depends/app_date/period.py
--rw-r--r--   0 soatra     (501) staff       (20)      187 2023-05-25 08:54:29.000000 eyes_soatra-0.0.28/eyes_soatra/constant/depends/app_date/start.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-07 04:41:05.926491 eyes_soatra-0.0.28/eyes_soatra/constant/depends/view/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:56:44.000000 eyes_soatra-0.0.28/eyes_soatra/constant/depends/view/__init__.py
--rw-r--r--   0 soatra     (501) staff       (20)      276 2023-05-02 03:37:05.000000 eyes_soatra-0.0.28/eyes_soatra/constant/depends/view/no_data.py
--rw-r--r--   0 soatra     (501) staff       (20)     7338 2023-05-25 08:53:28.000000 eyes_soatra-0.0.28/eyes_soatra/constant/depends/view/not_found.py
--rw-r--r--   0 soatra     (501) staff       (20)       69 2023-05-28 08:21:44.000000 eyes_soatra-0.0.28/eyes_soatra/constant/labels.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-07 04:41:05.926878 eyes_soatra-0.0.28/eyes_soatra/constant/libs/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:47:14.000000 eyes_soatra-0.0.28/eyes_soatra/constant/libs/__init__.py
--rw-r--r--   0 soatra     (501) staff       (20)      378 2023-05-23 01:48:11.000000 eyes_soatra-0.0.28/eyes_soatra/constant/libs/requests.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-07 04:41:05.927206 eyes_soatra-0.0.28/eyes_soatra/constant/user/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:46:27.000000 eyes_soatra-0.0.28/eyes_soatra/constant/user/__init__.py
--rw-rw-r--   0 soatra     (501) staff       (20)  1339531 2023-05-11 09:13:03.000000 eyes_soatra-0.0.28/eyes_soatra/constant/user/user_agents.py
--rw-r--r--   0 soatra     (501) staff       (20)      844 2023-06-07 03:44:07.000000 eyes_soatra-0.0.28/eyes_soatra/constant/vars.py
--rw-r--r--   0 soatra     (501) staff       (20)      107 2023-05-23 06:52:23.000000 eyes_soatra-0.0.28/eyes_soatra/eyes.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-07 04:41:05.930104 eyes_soatra-0.0.28/eyes_soatra/funcs/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:41:01.000000 eyes_soatra-0.0.28/eyes_soatra/funcs/__init__.py
--rw-r--r--   0 soatra     (501) staff       (20)    20149 2023-06-07 04:28:32.000000 eyes_soatra-0.0.28/eyes_soatra/funcs/time_app.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-07 04:41:05.931004 eyes_soatra-0.0.28/eyes_soatra/funcs/utils/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 02:07:05.000000 eyes_soatra-0.0.28/eyes_soatra/funcs/utils/__init__.py
--rw-r--r--   0 soatra     (501) staff       (20)      168 2023-05-23 02:06:56.000000 eyes_soatra-0.0.28/eyes_soatra/funcs/utils/dict.py
--rw-r--r--   0 soatra     (501) staff       (20)      372 2023-05-27 04:33:50.000000 eyes_soatra-0.0.28/eyes_soatra/funcs/utils/list.py
--rw-r--r--   0 soatra     (501) staff       (20)     2538 2023-06-02 06:33:58.000000 eyes_soatra-0.0.28/eyes_soatra/funcs/utils/string.py
--rw-r--r--   0 soatra     (501) staff       (20)    14065 2023-06-07 04:33:46.000000 eyes_soatra-0.0.28/eyes_soatra/funcs/view_page.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-07 04:41:05.923162 eyes_soatra-0.0.28/eyes_soatra.egg-info/
--rw-r--r--   0 soatra     (501) staff       (20)      835 2023-06-07 04:41:05.000000 eyes_soatra-0.0.28/eyes_soatra.egg-info/PKG-INFO
--rw-r--r--   0 soatra     (501) staff       (20)     1363 2023-06-07 04:41:05.000000 eyes_soatra-0.0.28/eyes_soatra.egg-info/SOURCES.txt
--rw-r--r--   0 soatra     (501) staff       (20)        1 2023-06-07 04:41:05.000000 eyes_soatra-0.0.28/eyes_soatra.egg-info/dependency_links.txt
--rw-r--r--   0 soatra     (501) staff       (20)       34 2023-06-07 04:41:05.000000 eyes_soatra-0.0.28/eyes_soatra.egg-info/requires.txt
--rw-r--r--   0 soatra     (501) staff       (20)       12 2023-06-07 04:41:05.000000 eyes_soatra-0.0.28/eyes_soatra.egg-info/top_level.txt
--rw-r--r--   0 soatra     (501) staff       (20)       38 2023-06-07 04:41:05.932660 eyes_soatra-0.0.28/setup.cfg
--rw-r--r--   0 soatra     (501) staff       (20)     1122 2023-06-02 04:58:12.000000 eyes_soatra-0.0.28/setup.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-07 04:41:05.932122 eyes_soatra-0.0.28/test/
--rw-r--r--   0 soatra     (501) staff       (20)     2942 2023-05-29 04:49:56.000000 eyes_soatra-0.0.28/test/test.py
--rw-r--r--   0 soatra     (501) staff       (20)     2989 2023-05-25 06:31:32.000000 eyes_soatra-0.0.28/test/test1.py
--rw-r--r--   0 soatra     (501) staff       (20)      241 2023-06-07 04:03:02.000000 eyes_soatra-0.0.28/test/test2.py
--rw-r--r--   0 soatra     (501) staff       (20)      210 2023-06-07 04:38:58.000000 eyes_soatra-0.0.28/test/test3.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-09 08:20:35.596090 eyes_soatra-0.0.29/
+-rw-r--r--   0 soatra     (501) staff       (20)       13 2023-05-02 07:13:47.000000 eyes_soatra-0.0.29/LICENSE
+-rw-r--r--   0 soatra     (501) staff       (20)      835 2023-06-09 08:20:35.595957 eyes_soatra-0.0.29/PKG-INFO
+-rw-r--r--   0 soatra     (501) staff       (20)      330 2023-06-02 06:41:30.000000 eyes_soatra-0.0.29/README.md
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-09 08:20:35.590731 eyes_soatra-0.0.29/eyes_soatra/
+-rw-r--r--   0 soatra     (501) staff       (20)       28 2023-05-02 07:14:02.000000 eyes_soatra-0.0.29/eyes_soatra/__init__.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-09 08:20:35.591702 eyes_soatra-0.0.29/eyes_soatra/constant/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:45:06.000000 eyes_soatra-0.0.29/eyes_soatra/constant/__init__.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-09 08:20:35.591835 eyes_soatra-0.0.29/eyes_soatra/constant/depends/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:46:17.000000 eyes_soatra-0.0.29/eyes_soatra/constant/depends/__init__.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-09 08:20:35.592318 eyes_soatra-0.0.29/eyes_soatra/constant/depends/app_date/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:54:07.000000 eyes_soatra-0.0.29/eyes_soatra/constant/depends/app_date/__init__.py
+-rw-r--r--   0 soatra     (501) staff       (20)      224 2023-05-25 08:54:38.000000 eyes_soatra-0.0.29/eyes_soatra/constant/depends/app_date/end.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-09 08:20:35.592775 eyes_soatra-0.0.29/eyes_soatra/constant/depends/app_date/formats/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-28 09:25:41.000000 eyes_soatra-0.0.29/eyes_soatra/constant/depends/app_date/formats/__init__.py
+-rw-r--r--   0 soatra     (501) staff       (20)     6706 2023-05-28 08:16:55.000000 eyes_soatra-0.0.29/eyes_soatra/constant/depends/app_date/formats/end.py
+-rw-r--r--   0 soatra     (501) staff       (20)     9568 2023-05-28 08:16:48.000000 eyes_soatra-0.0.29/eyes_soatra/constant/depends/app_date/formats/period.py
+-rw-r--r--   0 soatra     (501) staff       (20)     1127 2023-05-28 08:16:41.000000 eyes_soatra-0.0.29/eyes_soatra/constant/depends/app_date/formats/start.py
+-rw-r--r--   0 soatra     (501) staff       (20)      354 2023-05-29 02:27:50.000000 eyes_soatra-0.0.29/eyes_soatra/constant/depends/app_date/period.py
+-rw-r--r--   0 soatra     (501) staff       (20)      187 2023-05-25 08:54:29.000000 eyes_soatra-0.0.29/eyes_soatra/constant/depends/app_date/start.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-09 08:20:35.593136 eyes_soatra-0.0.29/eyes_soatra/constant/depends/view/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:56:44.000000 eyes_soatra-0.0.29/eyes_soatra/constant/depends/view/__init__.py
+-rw-r--r--   0 soatra     (501) staff       (20)      276 2023-05-02 03:37:05.000000 eyes_soatra-0.0.29/eyes_soatra/constant/depends/view/no_data.py
+-rw-r--r--   0 soatra     (501) staff       (20)     7338 2023-05-25 08:53:28.000000 eyes_soatra-0.0.29/eyes_soatra/constant/depends/view/not_found.py
+-rw-r--r--   0 soatra     (501) staff       (20)       69 2023-05-28 08:21:44.000000 eyes_soatra-0.0.29/eyes_soatra/constant/labels.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-09 08:20:35.593350 eyes_soatra-0.0.29/eyes_soatra/constant/libs/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:47:14.000000 eyes_soatra-0.0.29/eyes_soatra/constant/libs/__init__.py
+-rw-r--r--   0 soatra     (501) staff       (20)      387 2023-06-09 08:18:33.000000 eyes_soatra-0.0.29/eyes_soatra/constant/libs/requests.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-09 08:20:35.593569 eyes_soatra-0.0.29/eyes_soatra/constant/user/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:46:27.000000 eyes_soatra-0.0.29/eyes_soatra/constant/user/__init__.py
+-rw-rw-r--   0 soatra     (501) staff       (20)  1339531 2023-05-11 09:13:03.000000 eyes_soatra-0.0.29/eyes_soatra/constant/user/user_agents.py
+-rw-r--r--   0 soatra     (501) staff       (20)      844 2023-06-07 03:44:07.000000 eyes_soatra-0.0.29/eyes_soatra/constant/vars.py
+-rw-r--r--   0 soatra     (501) staff       (20)      107 2023-05-23 06:52:23.000000 eyes_soatra-0.0.29/eyes_soatra/eyes.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-09 08:20:35.594724 eyes_soatra-0.0.29/eyes_soatra/funcs/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:41:01.000000 eyes_soatra-0.0.29/eyes_soatra/funcs/__init__.py
+-rw-r--r--   0 soatra     (501) staff       (20)    20149 2023-06-07 04:28:32.000000 eyes_soatra-0.0.29/eyes_soatra/funcs/time_app.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-09 08:20:35.595255 eyes_soatra-0.0.29/eyes_soatra/funcs/utils/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 02:07:05.000000 eyes_soatra-0.0.29/eyes_soatra/funcs/utils/__init__.py
+-rw-r--r--   0 soatra     (501) staff       (20)      168 2023-05-23 02:06:56.000000 eyes_soatra-0.0.29/eyes_soatra/funcs/utils/dict.py
+-rw-r--r--   0 soatra     (501) staff       (20)      372 2023-05-27 04:33:50.000000 eyes_soatra-0.0.29/eyes_soatra/funcs/utils/list.py
+-rw-r--r--   0 soatra     (501) staff       (20)     2538 2023-06-02 06:33:58.000000 eyes_soatra-0.0.29/eyes_soatra/funcs/utils/string.py
+-rw-r--r--   0 soatra     (501) staff       (20)    14065 2023-06-07 04:33:46.000000 eyes_soatra-0.0.29/eyes_soatra/funcs/view_page.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-09 08:20:35.591345 eyes_soatra-0.0.29/eyes_soatra.egg-info/
+-rw-r--r--   0 soatra     (501) staff       (20)      835 2023-06-09 08:20:35.000000 eyes_soatra-0.0.29/eyes_soatra.egg-info/PKG-INFO
+-rw-r--r--   0 soatra     (501) staff       (20)     1363 2023-06-09 08:20:35.000000 eyes_soatra-0.0.29/eyes_soatra.egg-info/SOURCES.txt
+-rw-r--r--   0 soatra     (501) staff       (20)        1 2023-06-09 08:20:35.000000 eyes_soatra-0.0.29/eyes_soatra.egg-info/dependency_links.txt
+-rw-r--r--   0 soatra     (501) staff       (20)       34 2023-06-09 08:20:35.000000 eyes_soatra-0.0.29/eyes_soatra.egg-info/requires.txt
+-rw-r--r--   0 soatra     (501) staff       (20)       12 2023-06-09 08:20:35.000000 eyes_soatra-0.0.29/eyes_soatra.egg-info/top_level.txt
+-rw-r--r--   0 soatra     (501) staff       (20)       38 2023-06-09 08:20:35.596137 eyes_soatra-0.0.29/setup.cfg
+-rw-r--r--   0 soatra     (501) staff       (20)     1122 2023-06-09 08:20:33.000000 eyes_soatra-0.0.29/setup.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-09 08:20:35.595744 eyes_soatra-0.0.29/test/
+-rw-r--r--   0 soatra     (501) staff       (20)     2942 2023-05-29 04:49:56.000000 eyes_soatra-0.0.29/test/test.py
+-rw-r--r--   0 soatra     (501) staff       (20)     2989 2023-05-25 06:31:32.000000 eyes_soatra-0.0.29/test/test1.py
+-rw-r--r--   0 soatra     (501) staff       (20)      241 2023-06-07 04:03:02.000000 eyes_soatra-0.0.29/test/test2.py
+-rw-r--r--   0 soatra     (501) staff       (20)      210 2023-06-07 04:38:58.000000 eyes_soatra-0.0.29/test/test3.py
```

### Comparing `eyes_soatra-0.0.28/PKG-INFO` & `eyes_soatra-0.0.29/eyes_soatra.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: eyes_soatra
-Version: 0.0.28
+Name: eyes-soatra
+Version: 0.0.29
 Summary: Eyes
 Author: Soatra
 Author-email: johnsoatra@gmail.com
 Keywords: python,crawler,scanner,requests
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `eyes_soatra-0.0.28/eyes_soatra/constant/depends/app_date/formats/end.py` & `eyes_soatra-0.0.29/eyes_soatra/constant/depends/app_date/formats/end.py`

 * *Files identical despite different names*

### Comparing `eyes_soatra-0.0.28/eyes_soatra/constant/depends/app_date/formats/period.py` & `eyes_soatra-0.0.29/eyes_soatra/constant/depends/app_date/formats/period.py`

 * *Files identical despite different names*

### Comparing `eyes_soatra-0.0.28/eyes_soatra/constant/depends/app_date/formats/start.py` & `eyes_soatra-0.0.29/eyes_soatra/constant/depends/app_date/formats/start.py`

 * *Files identical despite different names*

### Comparing `eyes_soatra-0.0.28/eyes_soatra/constant/depends/view/not_found.py` & `eyes_soatra-0.0.29/eyes_soatra/constant/depends/view/not_found.py`

 * *Files identical despite different names*

### Comparing `eyes_soatra-0.0.28/eyes_soatra/constant/user/user_agents.py` & `eyes_soatra-0.0.29/eyes_soatra/constant/user/user_agents.py`

 * *Files identical despite different names*

### Comparing `eyes_soatra-0.0.28/eyes_soatra/constant/vars.py` & `eyes_soatra-0.0.29/eyes_soatra/constant/vars.py`

 * *Files identical despite different names*

### Comparing `eyes_soatra-0.0.28/eyes_soatra/funcs/time_app.py` & `eyes_soatra-0.0.29/eyes_soatra/funcs/time_app.py`

 * *Files identical despite different names*

### Comparing `eyes_soatra-0.0.28/eyes_soatra/funcs/utils/string.py` & `eyes_soatra-0.0.29/eyes_soatra/funcs/utils/string.py`

 * *Files identical despite different names*

### Comparing `eyes_soatra-0.0.28/eyes_soatra/funcs/view_page.py` & `eyes_soatra-0.0.29/eyes_soatra/funcs/view_page.py`

 * *Files identical despite different names*

### Comparing `eyes_soatra-0.0.28/eyes_soatra.egg-info/PKG-INFO` & `eyes_soatra-0.0.29/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: eyes-soatra
-Version: 0.0.28
+Name: eyes_soatra
+Version: 0.0.29
 Summary: Eyes
 Author: Soatra
 Author-email: johnsoatra@gmail.com
 Keywords: python,crawler,scanner,requests
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `eyes_soatra-0.0.28/eyes_soatra.egg-info/SOURCES.txt` & `eyes_soatra-0.0.29/eyes_soatra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eyes_soatra-0.0.28/setup.py` & `eyes_soatra-0.0.29/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 NAME = 'eyes_soatra'
-VERSION = '0.0.28'
+VERSION = '0.0.29'
 DESCRIPTION = 'Eyes'
 
 AUTHOR_NAME = 'Soatra'
 AUTHOR_EMAIL = 'johnsoatra@gmail.com'
 
 # Setting up
 setup(
```

### Comparing `eyes_soatra-0.0.28/test/test.py` & `eyes_soatra-0.0.29/test/test.py`

 * *Files identical despite different names*

### Comparing `eyes_soatra-0.0.28/test/test1.py` & `eyes_soatra-0.0.29/test/test1.py`

 * *Files identical despite different names*

