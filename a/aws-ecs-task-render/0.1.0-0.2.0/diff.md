# Comparing `tmp/aws-ecs-task-render-0.1.0.tar.gz` & `tmp/aws-ecs-task-render-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-ecs-task-render-0.1.0.tar", last modified: Fri Jun  9 16:57:29 2023, max compression
+gzip compressed data, was "aws-ecs-task-render-0.2.0.tar", last modified: Fri Jun  9 17:02:34 2023, max compression
```

## Comparing `aws-ecs-task-render-0.1.0.tar` & `aws-ecs-task-render-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:57:29.614929 aws-ecs-task-render-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-09 16:57:14.000000 aws-ecs-task-render-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-09 16:57:29.614929 aws-ecs-task-render-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-06-09 16:57:14.000000 aws-ecs-task-render-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:57:29.610928 aws-ecs-task-render-0.1.0/aws_ecs_task_render/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-09 16:57:14.000000 aws-ecs-task-render-0.1.0/aws_ecs_task_render/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-06-09 16:57:14.000000 aws-ecs-task-render-0.1.0/aws_ecs_task_render/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-06-09 16:57:14.000000 aws-ecs-task-render-0.1.0/aws_ecs_task_render/profile_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:57:29.614929 aws-ecs-task-render-0.1.0/aws_ecs_task_render.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-09 16:57:29.000000 aws-ecs-task-render-0.1.0/aws_ecs_task_render.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-09 16:57:29.000000 aws-ecs-task-render-0.1.0/aws_ecs_task_render.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 16:57:29.000000 aws-ecs-task-render-0.1.0/aws_ecs_task_render.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-09 16:57:29.000000 aws-ecs-task-render-0.1.0/aws_ecs_task_render.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-09 16:57:29.000000 aws-ecs-task-render-0.1.0/aws_ecs_task_render.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-09 16:57:29.000000 aws-ecs-task-render-0.1.0/aws_ecs_task_render.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-09 16:57:14.000000 aws-ecs-task-render-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-09 16:57:29.614929 aws-ecs-task-render-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:02:34.104319 aws-ecs-task-render-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-09 17:02:20.000000 aws-ecs-task-render-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-09 17:02:34.104319 aws-ecs-task-render-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-06-09 17:02:20.000000 aws-ecs-task-render-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:02:34.104319 aws-ecs-task-render-0.2.0/aws_ecs_task_render/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-09 17:02:20.000000 aws-ecs-task-render-0.2.0/aws_ecs_task_render/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-06-09 17:02:20.000000 aws-ecs-task-render-0.2.0/aws_ecs_task_render/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-06-09 17:02:20.000000 aws-ecs-task-render-0.2.0/aws_ecs_task_render/profile_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:02:34.104319 aws-ecs-task-render-0.2.0/aws_ecs_task_render.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-09 17:02:34.000000 aws-ecs-task-render-0.2.0/aws_ecs_task_render.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-09 17:02:34.000000 aws-ecs-task-render-0.2.0/aws_ecs_task_render.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 17:02:34.000000 aws-ecs-task-render-0.2.0/aws_ecs_task_render.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-09 17:02:34.000000 aws-ecs-task-render-0.2.0/aws_ecs_task_render.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-09 17:02:34.000000 aws-ecs-task-render-0.2.0/aws_ecs_task_render.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-09 17:02:34.000000 aws-ecs-task-render-0.2.0/aws_ecs_task_render.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-09 17:02:20.000000 aws-ecs-task-render-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-09 17:02:34.104319 aws-ecs-task-render-0.2.0/setup.cfg
```

### Comparing `aws-ecs-task-render-0.1.0/LICENSE` & `aws-ecs-task-render-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-ecs-task-render-0.1.0/PKG-INFO` & `aws-ecs-task-render-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-ecs-task-render
-Version: 0.1.0
+Version: 0.2.0
 Summary: "A package to edit image uri on ecs task definition"
 Author: Luca Pisciotta
 Author-email: luca.pisciotta@lptech.io
 License: MIT
 Keywords: aws,ecs,fargate
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aws-ecs-task-render-0.1.0/README.md` & `aws-ecs-task-render-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `aws-ecs-task-render-0.1.0/aws_ecs_task_render/__main__.py` & `aws-ecs-task-render-0.2.0/aws_ecs_task_render/__main__.py`

 * *Files identical despite different names*

### Comparing `aws-ecs-task-render-0.1.0/aws_ecs_task_render/profile_checker.py` & `aws-ecs-task-render-0.2.0/aws_ecs_task_render/profile_checker.py`

 * *Files identical despite different names*

### Comparing `aws-ecs-task-render-0.1.0/aws_ecs_task_render.egg-info/PKG-INFO` & `aws-ecs-task-render-0.2.0/aws_ecs_task_render.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-ecs-task-render
-Version: 0.1.0
+Version: 0.2.0
 Summary: "A package to edit image uri on ecs task definition"
 Author: Luca Pisciotta
 Author-email: luca.pisciotta@lptech.io
 License: MIT
 Keywords: aws,ecs,fargate
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aws-ecs-task-render-0.1.0/setup.cfg` & `aws-ecs-task-render-0.2.0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = aws-ecs-task-render
 description = "A package to edit image uri on ecs task definition"
-version = 0.1.0
+version = 0.2.0
 author = Luca Pisciotta
 author_email = luca.pisciotta@lptech.io
 readme = "README.md"
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = aws, ecs, fargate
 requires_python = ">=3.9"
@@ -21,13 +21,13 @@
 install_requires = 
 	boto3
 	botocore
 	inquirer
 
 [options.entry_points]
 console_scripts = 
-	aws-ecs-task-render = aws_ecs_task_render.main:main
+	aws-ecs-task-render = aws_ecs_task_render.__main__:main
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

