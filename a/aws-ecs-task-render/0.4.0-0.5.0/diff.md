# Comparing `tmp/aws-ecs-task-render-0.4.0.tar.gz` & `tmp/aws-ecs-task-render-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-ecs-task-render-0.4.0.tar", last modified: Fri Jun  9 17:44:42 2023, max compression
+gzip compressed data, was "aws-ecs-task-render-0.5.0.tar", last modified: Fri Jun  9 17:48:29 2023, max compression
```

## Comparing `aws-ecs-task-render-0.4.0.tar` & `aws-ecs-task-render-0.5.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:44:42.149828 aws-ecs-task-render-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-09 17:44:27.000000 aws-ecs-task-render-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-09 17:44:42.149828 aws-ecs-task-render-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-06-09 17:44:27.000000 aws-ecs-task-render-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:44:42.149828 aws-ecs-task-render-0.4.0/aws_ecs_task_render/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-09 17:44:27.000000 aws-ecs-task-render-0.4.0/aws_ecs_task_render/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-06-09 17:44:27.000000 aws-ecs-task-render-0.4.0/aws_ecs_task_render/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-06-09 17:44:27.000000 aws-ecs-task-render-0.4.0/aws_ecs_task_render/profile_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:44:42.149828 aws-ecs-task-render-0.4.0/aws_ecs_task_render.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-09 17:44:42.000000 aws-ecs-task-render-0.4.0/aws_ecs_task_render.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-09 17:44:42.000000 aws-ecs-task-render-0.4.0/aws_ecs_task_render.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 17:44:42.000000 aws-ecs-task-render-0.4.0/aws_ecs_task_render.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-09 17:44:42.000000 aws-ecs-task-render-0.4.0/aws_ecs_task_render.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-09 17:44:42.000000 aws-ecs-task-render-0.4.0/aws_ecs_task_render.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-09 17:44:42.000000 aws-ecs-task-render-0.4.0/aws_ecs_task_render.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-09 17:44:27.000000 aws-ecs-task-render-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-09 17:44:42.149828 aws-ecs-task-render-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:48:29.198963 aws-ecs-task-render-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-09 17:48:15.000000 aws-ecs-task-render-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-09 17:48:29.198963 aws-ecs-task-render-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-06-09 17:48:15.000000 aws-ecs-task-render-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:48:29.198963 aws-ecs-task-render-0.5.0/aws_ecs_task_render/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-09 17:48:15.000000 aws-ecs-task-render-0.5.0/aws_ecs_task_render/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-06-09 17:48:15.000000 aws-ecs-task-render-0.5.0/aws_ecs_task_render/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-06-09 17:48:15.000000 aws-ecs-task-render-0.5.0/aws_ecs_task_render/profile_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:48:29.198963 aws-ecs-task-render-0.5.0/aws_ecs_task_render.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-09 17:48:29.000000 aws-ecs-task-render-0.5.0/aws_ecs_task_render.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-09 17:48:29.000000 aws-ecs-task-render-0.5.0/aws_ecs_task_render.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 17:48:29.000000 aws-ecs-task-render-0.5.0/aws_ecs_task_render.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-09 17:48:29.000000 aws-ecs-task-render-0.5.0/aws_ecs_task_render.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-09 17:48:29.000000 aws-ecs-task-render-0.5.0/aws_ecs_task_render.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-09 17:48:29.000000 aws-ecs-task-render-0.5.0/aws_ecs_task_render.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-09 17:48:15.000000 aws-ecs-task-render-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-09 17:48:29.198963 aws-ecs-task-render-0.5.0/setup.cfg
```

### Comparing `aws-ecs-task-render-0.4.0/LICENSE` & `aws-ecs-task-render-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-ecs-task-render-0.4.0/PKG-INFO` & `aws-ecs-task-render-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-ecs-task-render
-Version: 0.4.0
+Version: 0.5.0
 Summary: "A package to edit image uri on ecs task definition"
 Author: Luca Pisciotta
 Author-email: luca.pisciotta@lptech.io
 License: MIT
 Keywords: aws,ecs,fargate
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aws-ecs-task-render-0.4.0/README.md` & `aws-ecs-task-render-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `aws-ecs-task-render-0.4.0/aws_ecs_task_render/__main__.py` & `aws-ecs-task-render-0.5.0/aws_ecs_task_render/__main__.py`

 * *Files identical despite different names*

### Comparing `aws-ecs-task-render-0.4.0/aws_ecs_task_render/profile_checker.py` & `aws-ecs-task-render-0.5.0/aws_ecs_task_render/profile_checker.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
     def read_profiles_files(self):
         """Class that manage all the stuff related to the profiles"""
         try:
           os_environ["HOME"]
           home_path = os_environ["HOME"]
         except:
-          logging.warning(f'Ops, seems you do not have HOME variable defined on your machine, i\'ll try to use "{str(Path.home())}"')
+          logging.info(f'Seems you do not have HOME variable defined on your machine, i\'ll try to use "{str(Path.home())}"')
           home_path = str(Path.home())
         try:
             self.credential_file.read(f'{home_path}/.aws/credentials')
             if os_path.exists(f'{home_path}/.aws/config'):
                 self.config_file.read(f'{home_path}/.aws/config')
         except configparser.Error:
             logging.error('%s/.aws/credentials', home_path)
```

### Comparing `aws-ecs-task-render-0.4.0/aws_ecs_task_render.egg-info/PKG-INFO` & `aws-ecs-task-render-0.5.0/aws_ecs_task_render.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-ecs-task-render
-Version: 0.4.0
+Version: 0.5.0
 Summary: "A package to edit image uri on ecs task definition"
 Author: Luca Pisciotta
 Author-email: luca.pisciotta@lptech.io
 License: MIT
 Keywords: aws,ecs,fargate
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aws-ecs-task-render-0.4.0/setup.cfg` & `aws-ecs-task-render-0.5.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = aws-ecs-task-render
 description = "A package to edit image uri on ecs task definition"
-version = 0.4.0
+version = 0.5.0
 author = Luca Pisciotta
 author_email = luca.pisciotta@lptech.io
 readme = "README.md"
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = aws, ecs, fargate
 requires_python = ">=3.9"
```

