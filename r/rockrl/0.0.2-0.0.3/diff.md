# Comparing `tmp/rockrl-0.0.2.tar.gz` & `tmp/rockrl-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rockrl-0.0.2.tar", last modified: Fri Jun  9 11:12:43 2023, max compression
+gzip compressed data, was "rockrl-0.0.3.tar", last modified: Fri Jun  9 12:06:29 2023, max compression
```

## Comparing `rockrl-0.0.2.tar` & `rockrl-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,38 @@
-drwxr-xr-x   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2023-06-09 11:12:43.901121 rockrl-0.0.2/
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     1062 2023-04-25 06:38:11.000000 rockrl-0.0.2/LICENSE
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     1164 2023-06-09 11:12:43.901121 rockrl-0.0.2/PKG-INFO
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)      730 2023-06-09 07:46:45.000000 rockrl-0.0.2/README.md
-drwxr-xr-x   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2023-06-09 11:12:43.901121 rockrl-0.0.2/rockrl/
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)       21 2023-06-09 11:12:21.000000 rockrl-0.0.2/rockrl/__init__.py
-drwxr-xr-x   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2023-06-09 11:12:43.901121 rockrl-0.0.2/rockrl.egg-info/
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     1164 2023-06-09 11:12:43.000000 rockrl-0.0.2/rockrl.egg-info/PKG-INFO
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)      194 2023-06-09 11:12:43.000000 rockrl-0.0.2/rockrl.egg-info/SOURCES.txt
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        1 2023-06-09 11:12:43.000000 rockrl-0.0.2/rockrl.egg-info/dependency_links.txt
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)       18 2023-06-09 11:12:43.000000 rockrl-0.0.2/rockrl.egg-info/requires.txt
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        7 2023-06-09 11:12:43.000000 rockrl-0.0.2/rockrl.egg-info/top_level.txt
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)       38 2023-06-09 11:12:43.901121 rockrl-0.0.2/setup.cfg
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     1531 2023-06-09 11:12:12.000000 rockrl-0.0.2/setup.py
+drwxr-xr-x   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2023-06-09 12:06:29.885463 rockrl-0.0.3/
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     1062 2023-04-25 06:38:11.000000 rockrl-0.0.3/LICENSE
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)       20 2023-06-09 12:01:58.000000 rockrl-0.0.3/MANIFEST.in
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     1164 2023-06-09 12:06:29.885463 rockrl-0.0.3/PKG-INFO
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)      730 2023-06-09 07:46:45.000000 rockrl-0.0.3/README.md
+drwxr-xr-x   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2023-06-09 12:06:29.885463 rockrl-0.0.3/rockrl/
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)       21 2023-06-09 12:06:25.000000 rockrl-0.0.3/rockrl/__init__.py
+drwxr-xr-x   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2023-06-09 12:06:29.885463 rockrl-0.0.3/rockrl/tensorflow/
+drwxr-xr-x   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2023-06-09 12:06:29.885463 rockrl-0.0.3/rockrl/tensorflow/PPO/
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)    17454 2023-06-09 07:46:45.000000 rockrl-0.0.3/rockrl/tensorflow/PPO/ppo.py
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)       29 2023-06-09 07:46:45.000000 rockrl-0.0.3/rockrl/tensorflow/__init__.py
+drwxr-xr-x   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2023-06-09 12:06:29.885463 rockrl-0.0.3/rockrl/tensorflow/examples/
+drwxr-xr-x   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2023-06-09 12:06:29.885463 rockrl-0.0.3/rockrl/tensorflow/examples/ppo/
+drwxr-xr-x   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2023-06-09 12:06:29.885463 rockrl-0.0.3/rockrl/tensorflow/examples/ppo/BipedalWalker-v3/
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     3171 2023-06-09 11:20:22.000000 rockrl-0.0.3/rockrl/tensorflow/examples/ppo/BipedalWalker-v3/BipedalWalker-v3.py
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     1662 2023-06-09 11:20:22.000000 rockrl-0.0.3/rockrl/tensorflow/examples/ppo/BipedalWalker-v3/BipedalWalker-v3_test.py
+drwxr-xr-x   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2023-06-09 12:06:29.885463 rockrl-0.0.3/rockrl/tensorflow/examples/ppo/BipedalWalkerHardcore-v3/
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     3286 2023-06-09 11:20:22.000000 rockrl-0.0.3/rockrl/tensorflow/examples/ppo/BipedalWalkerHardcore-v3/BipedalWalkerHardcore-v3.py
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     1775 2023-06-09 11:20:22.000000 rockrl-0.0.3/rockrl/tensorflow/examples/ppo/BipedalWalkerHardcore-v3/BipedalWalkerHardcore-v3_test.py
+drwxr-xr-x   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2023-06-09 12:06:29.885463 rockrl-0.0.3/rockrl/tensorflow/examples/ppo/LunarLander-v2/
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     2791 2023-06-09 11:20:22.000000 rockrl-0.0.3/rockrl/tensorflow/examples/ppo/LunarLander-v2/LunarLander-v2.py
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     1072 2023-06-09 07:46:45.000000 rockrl-0.0.3/rockrl/tensorflow/examples/ppo/LunarLander-v2/LunarLander-v2_test.py
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2023-06-09 11:41:54.000000 rockrl-0.0.3/rockrl/tensorflow/examples/ppo/__init__.py
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)       10 2023-04-25 08:43:20.000000 rockrl-0.0.3/rockrl/tensorflow/examples/ppo/requirements.txt
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)       49 2023-06-09 07:46:45.000000 rockrl-0.0.3/rockrl/tensorflow/requirements.txt
+drwxr-xr-x   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2023-06-09 12:06:29.885463 rockrl-0.0.3/rockrl/utils/
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2023-06-09 11:21:05.000000 rockrl-0.0.3/rockrl/utils/__init__.py
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     2876 2023-06-09 07:46:45.000000 rockrl-0.0.3/rockrl/utils/memory.py
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)      927 2023-06-09 07:46:45.000000 rockrl-0.0.3/rockrl/utils/misc.py
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     3393 2023-06-09 07:46:45.000000 rockrl-0.0.3/rockrl/utils/vectorizedEnv.py
+drwxr-xr-x   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2023-06-09 12:06:29.885463 rockrl-0.0.3/rockrl.egg-info/
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     1164 2023-06-09 12:06:29.000000 rockrl-0.0.3/rockrl.egg-info/PKG-INFO
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)      937 2023-06-09 12:06:29.000000 rockrl-0.0.3/rockrl.egg-info/SOURCES.txt
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        1 2023-06-09 12:06:29.000000 rockrl-0.0.3/rockrl.egg-info/dependency_links.txt
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)       18 2023-06-09 12:06:29.000000 rockrl-0.0.3/rockrl.egg-info/requires.txt
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        7 2023-06-09 12:06:29.000000 rockrl-0.0.3/rockrl.egg-info/top_level.txt
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)       38 2023-06-09 12:06:29.885463 rockrl-0.0.3/setup.cfg
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     1646 2023-06-09 12:04:36.000000 rockrl-0.0.3/setup.py
```

### Comparing `rockrl-0.0.2/LICENSE` & `rockrl-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rockrl-0.0.2/PKG-INFO` & `rockrl-0.0.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rockrl
-Version: 0.0.2
+Version: 0.0.3
 Summary: Reinformcement Learning library
 Home-page: https://pylessons.com/
 Author: PyLessons
 Author-email: pythonlessons0@gmail.com
 License: UNKNOWN
 Project-URL: Source, https://github.com/pythonlessons/RockRL/
 Project-URL: Tracker, https://github.com/pythonlessons/RockRL/issues
```

### Comparing `rockrl-0.0.2/README.md` & `rockrl-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `rockrl-0.0.2/rockrl.egg-info/PKG-INFO` & `rockrl-0.0.3/rockrl.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rockrl
-Version: 0.0.2
+Version: 0.0.3
 Summary: Reinformcement Learning library
 Home-page: https://pylessons.com/
 Author: PyLessons
 Author-email: pythonlessons0@gmail.com
 License: UNKNOWN
 Project-URL: Source, https://github.com/pythonlessons/RockRL/
 Project-URL: Tracker, https://github.com/pythonlessons/RockRL/issues
```

### Comparing `rockrl-0.0.2/setup.py` & `rockrl-0.0.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-from setuptools import setup
+from setuptools import setup, find_packages
 
 DIR = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(DIR, 'README.md')) as fh:
     long_description = fh.read()
 
 with open(os.path.join(DIR, 'requirements.txt')) as fh:
@@ -34,16 +34,17 @@
     long_description = long_description,
     long_description_content_type = 'text/markdown',
     url='https://pylessons.com/',
     author='PyLessons',
     author_email='pythonlessons0@gmail.com',
     install_requires=requirements,
     python_requires='>=3',
-    packages = ['rockrl'],
+    packages = find_packages(exclude=['*.pyc']),
     include_package_data=True,
-    package_data={'rockrl': ['*']},
+    # package_data={'rockrl': ['**/**/*', '**/**/**/*', '**/**/**/**/*']},
+    # package_data={'rockrl': ['**']},
     project_urls={
         'Source': 'https://github.com/pythonlessons/RockRL/',
         'Tracker': 'https://github.com/pythonlessons/RockRL/issues',
     },
     description="Reinformcement Learning library",
 )
```

