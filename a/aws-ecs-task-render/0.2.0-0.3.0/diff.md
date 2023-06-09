# Comparing `tmp/aws-ecs-task-render-0.2.0.tar.gz` & `tmp/aws-ecs-task-render-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-ecs-task-render-0.2.0.tar", last modified: Fri Jun  9 17:02:34 2023, max compression
+gzip compressed data, was "aws-ecs-task-render-0.3.0.tar", last modified: Fri Jun  9 17:39:13 2023, max compression
```

## Comparing `aws-ecs-task-render-0.2.0.tar` & `aws-ecs-task-render-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:02:34.104319 aws-ecs-task-render-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-09 17:02:20.000000 aws-ecs-task-render-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-09 17:02:34.104319 aws-ecs-task-render-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-06-09 17:02:20.000000 aws-ecs-task-render-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:02:34.104319 aws-ecs-task-render-0.2.0/aws_ecs_task_render/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-09 17:02:20.000000 aws-ecs-task-render-0.2.0/aws_ecs_task_render/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-06-09 17:02:20.000000 aws-ecs-task-render-0.2.0/aws_ecs_task_render/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-06-09 17:02:20.000000 aws-ecs-task-render-0.2.0/aws_ecs_task_render/profile_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:02:34.104319 aws-ecs-task-render-0.2.0/aws_ecs_task_render.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-09 17:02:34.000000 aws-ecs-task-render-0.2.0/aws_ecs_task_render.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-09 17:02:34.000000 aws-ecs-task-render-0.2.0/aws_ecs_task_render.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 17:02:34.000000 aws-ecs-task-render-0.2.0/aws_ecs_task_render.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-09 17:02:34.000000 aws-ecs-task-render-0.2.0/aws_ecs_task_render.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-09 17:02:34.000000 aws-ecs-task-render-0.2.0/aws_ecs_task_render.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-09 17:02:34.000000 aws-ecs-task-render-0.2.0/aws_ecs_task_render.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-09 17:02:20.000000 aws-ecs-task-render-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-09 17:02:34.104319 aws-ecs-task-render-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:39:13.656389 aws-ecs-task-render-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-09 17:39:00.000000 aws-ecs-task-render-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-09 17:39:13.656389 aws-ecs-task-render-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-06-09 17:39:00.000000 aws-ecs-task-render-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:39:13.656389 aws-ecs-task-render-0.3.0/aws_ecs_task_render/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-09 17:39:00.000000 aws-ecs-task-render-0.3.0/aws_ecs_task_render/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-06-09 17:39:00.000000 aws-ecs-task-render-0.3.0/aws_ecs_task_render/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-06-09 17:39:00.000000 aws-ecs-task-render-0.3.0/aws_ecs_task_render/profile_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:39:13.656389 aws-ecs-task-render-0.3.0/aws_ecs_task_render.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-09 17:39:13.000000 aws-ecs-task-render-0.3.0/aws_ecs_task_render.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-09 17:39:13.000000 aws-ecs-task-render-0.3.0/aws_ecs_task_render.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 17:39:13.000000 aws-ecs-task-render-0.3.0/aws_ecs_task_render.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-09 17:39:13.000000 aws-ecs-task-render-0.3.0/aws_ecs_task_render.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-09 17:39:13.000000 aws-ecs-task-render-0.3.0/aws_ecs_task_render.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-09 17:39:13.000000 aws-ecs-task-render-0.3.0/aws_ecs_task_render.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-09 17:39:00.000000 aws-ecs-task-render-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-09 17:39:13.656389 aws-ecs-task-render-0.3.0/setup.cfg
```

### Comparing `aws-ecs-task-render-0.2.0/LICENSE` & `aws-ecs-task-render-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-ecs-task-render-0.2.0/PKG-INFO` & `aws-ecs-task-render-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-ecs-task-render
-Version: 0.2.0
+Version: 0.3.0
 Summary: "A package to edit image uri on ecs task definition"
 Author: Luca Pisciotta
 Author-email: luca.pisciotta@lptech.io
 License: MIT
 Keywords: aws,ecs,fargate
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aws-ecs-task-render-0.2.0/README.md` & `aws-ecs-task-render-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `aws-ecs-task-render-0.2.0/aws_ecs_task_render/__main__.py` & `aws-ecs-task-render-0.3.0/aws_ecs_task_render/__main__.py`

 * *Files identical despite different names*

### Comparing `aws-ecs-task-render-0.2.0/aws_ecs_task_render/profile_checker.py` & `aws-ecs-task-render-0.3.0/aws_ecs_task_render/profile_checker.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Module to make checks about the AWS profile"""
 import configparser
 import logging
 from os import environ as os_environ, path as os_path
+from pathlib import Path
 from sys import exit as sys_exit
 from inquirer import List as inquirer_list, prompt as inquirer_prompt
 
 
 class ProfileChecker:
     """Class to check or choose the AWS profile"""
     def __init__(self, profile):
@@ -50,14 +51,19 @@
         """Function to check if the provided profile exists"""
         if self.profile_name not in self.sections_list:
             logging.error('%s isn\'t a valid profile', self.profile_name)
             self.choose_profile()
 
     def read_profiles_files(self):
         """Class that manage all the stuff related to the profiles"""
+        if os_environ["HOME"] is None:
+          logging.warning(f'Ops, seems you do not have HOME variable defined on your machine, i\'ll try to use "{str(Path.home())}"')
+          home_path = str(Path.home())
+        else:
+          home_path = os_environ["HOME"]
         try:
-            self.credential_file.read(f'{os_environ["HOME"]}/.aws/credentials')
-            if os_path.exists(f'{os_environ["HOME"]}/.aws/config'):
-                self.config_file.read(f'{os_environ["HOME"]}/.aws/config')
+            self.credential_file.read(f'{home_path}/.aws/credentials')
+            if os_path.exists(f'{home_path}/.aws/config'):
+                self.config_file.read(f'{home_path}/.aws/config')
         except configparser.Error:
-            logging.error('%s/.aws/credentials', os_environ['HOME'])
+            logging.error('%s/.aws/credentials', home_path)
             sys_exit(1)
```

### Comparing `aws-ecs-task-render-0.2.0/aws_ecs_task_render.egg-info/PKG-INFO` & `aws-ecs-task-render-0.3.0/aws_ecs_task_render.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-ecs-task-render
-Version: 0.2.0
+Version: 0.3.0
 Summary: "A package to edit image uri on ecs task definition"
 Author: Luca Pisciotta
 Author-email: luca.pisciotta@lptech.io
 License: MIT
 Keywords: aws,ecs,fargate
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aws-ecs-task-render-0.2.0/setup.cfg` & `aws-ecs-task-render-0.3.0/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = aws-ecs-task-render
 description = "A package to edit image uri on ecs task definition"
-version = 0.2.0
+version = 0.3.0
 author = Luca Pisciotta
 author_email = luca.pisciotta@lptech.io
 readme = "README.md"
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = aws, ecs, fargate
 requires_python = ">=3.9"
```

