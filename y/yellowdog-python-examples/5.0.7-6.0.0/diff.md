# Comparing `tmp/yellowdog-python-examples-5.0.7.tar.gz` & `tmp/yellowdog-python-examples-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yellowdog-python-examples-5.0.7.tar", last modified: Tue May 16 09:43:16 2023, max compression
+gzip compressed data, was "yellowdog-python-examples-6.0.0.tar", last modified: Fri Jun  9 10:29:58 2023, max compression
```

## Comparing `yellowdog-python-examples-5.0.7.tar` & `yellowdog-python-examples-6.0.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 pwt        (501) staff       (20)        0 2023-05-16 09:43:16.418703 yellowdog-python-examples-5.0.7/
--rw-r--r--   0 pwt        (501) staff       (20)    11357 2022-11-18 20:55:26.000000 yellowdog-python-examples-5.0.7/LICENSE
--rw-r--r--   0 pwt        (501) staff       (20)     1418 2023-05-16 09:43:16.418795 yellowdog-python-examples-5.0.7/PKG-INFO
--rw-r--r--   0 pwt        (501) staff       (20)      676 2022-11-22 08:58:59.000000 yellowdog-python-examples-5.0.7/PYPI_README.md
--rw-r--r--   0 pwt        (501) staff       (20)   109989 2023-05-03 10:27:28.000000 yellowdog-python-examples-5.0.7/README.md
--rw-r--r--   0 pwt        (501) staff       (20)     1806 2023-02-20 09:23:16.000000 yellowdog-python-examples-5.0.7/pyproject.toml
--rw-r--r--   0 pwt        (501) staff       (20)       46 2023-05-16 09:40:32.000000 yellowdog-python-examples-5.0.7/requirements.txt
--rw-r--r--   0 pwt        (501) staff       (20)     1366 2023-05-16 09:43:16.419062 yellowdog-python-examples-5.0.7/setup.cfg
--rw-r--r--   0 pwt        (501) staff       (20)      125 2023-02-14 10:40:48.000000 yellowdog-python-examples-5.0.7/setup.py
-drwxr-xr-x   0 pwt        (501) staff       (20)        0 2023-05-16 09:43:16.417930 yellowdog-python-examples-5.0.7/yd_commands/
--rw-r--r--   0 pwt        (501) staff       (20)       22 2023-05-16 09:40:32.000000 yellowdog-python-examples-5.0.7/yd_commands/__init__.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     3415 2023-05-16 09:40:32.000000 yellowdog-python-examples-5.0.7/yd_commands/abort.py
--rwxr-xr-x   0 pwt        (501) staff       (20)      982 2023-01-31 15:59:12.000000 yellowdog-python-examples-5.0.7/yd_commands/admin.py
--rwxr-xr-x   0 pwt        (501) staff       (20)    18007 2023-05-16 09:40:32.000000 yellowdog-python-examples-5.0.7/yd_commands/args.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     5114 2023-05-16 09:40:32.000000 yellowdog-python-examples-5.0.7/yd_commands/cancel.py
--rw-r--r--   0 pwt        (501) staff       (20)      579 2022-12-12 15:56:41.000000 yellowdog-python-examples-5.0.7/yd_commands/check_imports.py
--rw-r--r--   0 pwt        (501) staff       (20)     3757 2022-11-27 20:53:08.000000 yellowdog-python-examples-5.0.7/yd_commands/compact_json.py
--rw-r--r--   0 pwt        (501) staff       (20)    18352 2023-05-16 09:40:32.000000 yellowdog-python-examples-5.0.7/yd_commands/config.py
--rw-r--r--   0 pwt        (501) staff       (20)     5544 2023-05-03 10:27:28.000000 yellowdog-python-examples-5.0.7/yd_commands/config_keys.py
--rw-r--r--   0 pwt        (501) staff       (20)    12181 2023-05-16 09:40:32.000000 yellowdog-python-examples-5.0.7/yd_commands/csv_data.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     1657 2023-05-16 09:40:32.000000 yellowdog-python-examples-5.0.7/yd_commands/delete.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     3626 2023-05-16 09:40:32.000000 yellowdog-python-examples-5.0.7/yd_commands/download.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     9251 2023-05-16 09:40:32.000000 yellowdog-python-examples-5.0.7/yd_commands/instantiate.py
--rw-r--r--   0 pwt        (501) staff       (20)     3729 2023-05-16 09:40:32.000000 yellowdog-python-examples-5.0.7/yd_commands/interactive.py
--rwxr-xr-x   0 pwt        (501) staff       (20)      749 2023-03-28 14:27:45.000000 yellowdog-python-examples-5.0.7/yd_commands/jsonnet2json.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     7798 2023-05-16 09:40:32.000000 yellowdog-python-examples-5.0.7/yd_commands/list.py
--rw-r--r--   0 pwt        (501) staff       (20)     3000 2023-05-16 09:40:32.000000 yellowdog-python-examples-5.0.7/yd_commands/object_utilities.py
--rw-r--r--   0 pwt        (501) staff       (20)     9525 2023-05-16 09:40:32.000000 yellowdog-python-examples-5.0.7/yd_commands/printing.py
--rwxr-xr-x   0 pwt        (501) staff       (20)    16922 2023-05-16 09:40:32.000000 yellowdog-python-examples-5.0.7/yd_commands/provision.py
--rw-r--r--   0 pwt        (501) staff       (20)     1248 2023-05-03 10:27:28.000000 yellowdog-python-examples-5.0.7/yd_commands/provision_utils.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     1479 2023-02-14 10:40:48.000000 yellowdog-python-examples-5.0.7/yd_commands/reformat_json.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     3232 2023-05-16 09:40:32.000000 yellowdog-python-examples-5.0.7/yd_commands/shutdown.py
--rwxr-xr-x   0 pwt        (501) staff       (20)    40228 2023-05-16 09:40:32.000000 yellowdog-python-examples-5.0.7/yd_commands/submit.py
--rw-r--r--   0 pwt        (501) staff       (20)     6052 2023-05-03 10:27:28.000000 yellowdog-python-examples-5.0.7/yd_commands/submit_utils.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     2916 2023-05-16 09:40:32.000000 yellowdog-python-examples-5.0.7/yd_commands/terminate.py
--rw-r--r--   0 pwt        (501) staff       (20)     1678 2022-12-07 08:38:57.000000 yellowdog-python-examples-5.0.7/yd_commands/type_check.py
--rw-r--r--   0 pwt        (501) staff       (20)     2237 2023-05-16 09:40:32.000000 yellowdog-python-examples-5.0.7/yd_commands/upload.py
--rw-r--r--   0 pwt        (501) staff       (20)     3389 2023-04-19 15:22:46.000000 yellowdog-python-examples-5.0.7/yd_commands/upload_utils.py
--rw-r--r--   0 pwt        (501) staff       (20)     1630 2023-04-19 15:22:46.000000 yellowdog-python-examples-5.0.7/yd_commands/validate_properties.py
--rw-r--r--   0 pwt        (501) staff       (20)    11037 2023-05-16 09:40:32.000000 yellowdog-python-examples-5.0.7/yd_commands/variables.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     1247 2023-03-24 08:40:30.000000 yellowdog-python-examples-5.0.7/yd_commands/version.py
--rw-r--r--   0 pwt        (501) staff       (20)     2200 2023-04-19 15:22:46.000000 yellowdog-python-examples-5.0.7/yd_commands/wrapper.py
-drwxr-xr-x   0 pwt        (501) staff       (20)        0 2023-05-16 09:43:16.418610 yellowdog-python-examples-5.0.7/yellowdog_python_examples.egg-info/
--rw-r--r--   0 pwt        (501) staff       (20)     1418 2023-05-16 09:43:16.000000 yellowdog-python-examples-5.0.7/yellowdog_python_examples.egg-info/PKG-INFO
--rw-r--r--   0 pwt        (501) staff       (20)     1187 2023-05-16 09:43:16.000000 yellowdog-python-examples-5.0.7/yellowdog_python_examples.egg-info/SOURCES.txt
--rw-r--r--   0 pwt        (501) staff       (20)        1 2023-05-16 09:43:16.000000 yellowdog-python-examples-5.0.7/yellowdog_python_examples.egg-info/dependency_links.txt
--rw-r--r--   0 pwt        (501) staff       (20)      574 2023-05-16 09:43:16.000000 yellowdog-python-examples-5.0.7/yellowdog_python_examples.egg-info/entry_points.txt
--rw-r--r--   0 pwt        (501) staff       (20)       61 2023-05-16 09:43:16.000000 yellowdog-python-examples-5.0.7/yellowdog_python_examples.egg-info/requires.txt
--rw-r--r--   0 pwt        (501) staff       (20)       12 2023-05-16 09:43:16.000000 yellowdog-python-examples-5.0.7/yellowdog_python_examples.egg-info/top_level.txt
+drwxr-xr-x   0 pwt        (501) staff       (20)        0 2023-06-09 10:29:58.349112 yellowdog-python-examples-6.0.0/
+-rw-r--r--   0 pwt        (501) staff       (20)    11357 2022-11-18 20:55:26.000000 yellowdog-python-examples-6.0.0/LICENSE
+-rw-r--r--   0 pwt        (501) staff       (20)     1418 2023-06-09 10:29:58.349183 yellowdog-python-examples-6.0.0/PKG-INFO
+-rw-r--r--   0 pwt        (501) staff       (20)      676 2022-11-22 08:58:59.000000 yellowdog-python-examples-6.0.0/PYPI_README.md
+-rw-r--r--   0 pwt        (501) staff       (20)   108894 2023-06-09 10:27:25.000000 yellowdog-python-examples-6.0.0/README.md
+-rw-r--r--   0 pwt        (501) staff       (20)     1806 2023-02-20 09:23:16.000000 yellowdog-python-examples-6.0.0/pyproject.toml
+-rw-r--r--   0 pwt        (501) staff       (20)       46 2023-06-09 10:27:25.000000 yellowdog-python-examples-6.0.0/requirements.txt
+-rw-r--r--   0 pwt        (501) staff       (20)     1366 2023-06-09 10:29:58.349493 yellowdog-python-examples-6.0.0/setup.cfg
+-rw-r--r--   0 pwt        (501) staff       (20)      125 2023-02-14 10:40:48.000000 yellowdog-python-examples-6.0.0/setup.py
+drwxr-xr-x   0 pwt        (501) staff       (20)        0 2023-06-09 10:29:58.348269 yellowdog-python-examples-6.0.0/yd_commands/
+-rw-r--r--   0 pwt        (501) staff       (20)       22 2023-06-09 10:27:25.000000 yellowdog-python-examples-6.0.0/yd_commands/__init__.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     3415 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.0/yd_commands/abort.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)      982 2023-01-31 15:59:12.000000 yellowdog-python-examples-6.0.0/yd_commands/admin.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)    18382 2023-06-09 10:27:25.000000 yellowdog-python-examples-6.0.0/yd_commands/args.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     5114 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.0/yd_commands/cancel.py
+-rw-r--r--   0 pwt        (501) staff       (20)      579 2022-12-12 15:56:41.000000 yellowdog-python-examples-6.0.0/yd_commands/check_imports.py
+-rw-r--r--   0 pwt        (501) staff       (20)     3757 2022-11-27 20:53:08.000000 yellowdog-python-examples-6.0.0/yd_commands/compact_json.py
+-rw-r--r--   0 pwt        (501) staff       (20)    17400 2023-06-09 10:27:25.000000 yellowdog-python-examples-6.0.0/yd_commands/config.py
+-rw-r--r--   0 pwt        (501) staff       (20)     5019 2023-06-09 10:27:25.000000 yellowdog-python-examples-6.0.0/yd_commands/config_keys.py
+-rw-r--r--   0 pwt        (501) staff       (20)    12135 2023-06-09 10:27:25.000000 yellowdog-python-examples-6.0.0/yd_commands/csv_data.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     1657 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.0/yd_commands/delete.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     3626 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.0/yd_commands/download.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     9251 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.0/yd_commands/instantiate.py
+-rw-r--r--   0 pwt        (501) staff       (20)     3729 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.0/yd_commands/interactive.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)      749 2023-03-28 14:27:45.000000 yellowdog-python-examples-6.0.0/yd_commands/jsonnet2json.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     7798 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.0/yd_commands/list.py
+-rw-r--r--   0 pwt        (501) staff       (20)     3000 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.0/yd_commands/object_utilities.py
+-rw-r--r--   0 pwt        (501) staff       (20)     9525 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.0/yd_commands/printing.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)    13218 2023-06-09 10:27:25.000000 yellowdog-python-examples-6.0.0/yd_commands/provision.py
+-rw-r--r--   0 pwt        (501) staff       (20)     1248 2023-05-03 10:27:28.000000 yellowdog-python-examples-6.0.0/yd_commands/provision_utils.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     1479 2023-02-14 10:40:48.000000 yellowdog-python-examples-6.0.0/yd_commands/reformat_json.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     3232 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.0/yd_commands/shutdown.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)    40530 2023-06-09 10:27:25.000000 yellowdog-python-examples-6.0.0/yd_commands/submit.py
+-rw-r--r--   0 pwt        (501) staff       (20)     6052 2023-05-03 10:27:28.000000 yellowdog-python-examples-6.0.0/yd_commands/submit_utils.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     2916 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.0/yd_commands/terminate.py
+-rw-r--r--   0 pwt        (501) staff       (20)     1678 2022-12-07 08:38:57.000000 yellowdog-python-examples-6.0.0/yd_commands/type_check.py
+-rw-r--r--   0 pwt        (501) staff       (20)     2237 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.0/yd_commands/upload.py
+-rw-r--r--   0 pwt        (501) staff       (20)     3389 2023-04-19 15:22:46.000000 yellowdog-python-examples-6.0.0/yd_commands/upload_utils.py
+-rw-r--r--   0 pwt        (501) staff       (20)     2177 2023-06-09 10:27:25.000000 yellowdog-python-examples-6.0.0/yd_commands/validate_properties.py
+-rw-r--r--   0 pwt        (501) staff       (20)    11037 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.0/yd_commands/variables.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     1247 2023-03-24 08:40:30.000000 yellowdog-python-examples-6.0.0/yd_commands/version.py
+-rw-r--r--   0 pwt        (501) staff       (20)     2200 2023-04-19 15:22:46.000000 yellowdog-python-examples-6.0.0/yd_commands/wrapper.py
+drwxr-xr-x   0 pwt        (501) staff       (20)        0 2023-06-09 10:29:58.349008 yellowdog-python-examples-6.0.0/yellowdog_python_examples.egg-info/
+-rw-r--r--   0 pwt        (501) staff       (20)     1418 2023-06-09 10:29:58.000000 yellowdog-python-examples-6.0.0/yellowdog_python_examples.egg-info/PKG-INFO
+-rw-r--r--   0 pwt        (501) staff       (20)     1187 2023-06-09 10:29:58.000000 yellowdog-python-examples-6.0.0/yellowdog_python_examples.egg-info/SOURCES.txt
+-rw-r--r--   0 pwt        (501) staff       (20)        1 2023-06-09 10:29:58.000000 yellowdog-python-examples-6.0.0/yellowdog_python_examples.egg-info/dependency_links.txt
+-rw-r--r--   0 pwt        (501) staff       (20)      574 2023-06-09 10:29:58.000000 yellowdog-python-examples-6.0.0/yellowdog_python_examples.egg-info/entry_points.txt
+-rw-r--r--   0 pwt        (501) staff       (20)       61 2023-06-09 10:29:58.000000 yellowdog-python-examples-6.0.0/yellowdog_python_examples.egg-info/requires.txt
+-rw-r--r--   0 pwt        (501) staff       (20)       12 2023-06-09 10:29:58.000000 yellowdog-python-examples-6.0.0/yellowdog_python_examples.egg-info/top_level.txt
```

### Comparing `yellowdog-python-examples-5.0.7/LICENSE` & `yellowdog-python-examples-6.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.7/PKG-INFO` & `yellowdog-python-examples-6.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yellowdog-python-examples
-Version: 5.0.7
+Version: 6.0.0
 Summary: Example Python commands using the YellowDog Python SDK
 Home-page: https://github.com/yellowdog/python-examples
 Author: YellowDog Limited
 Author-email: YellowDog Limited <support@yellowdog.co>
 Project-URL: Homepage, https://github.com/yellowdog/python-examples
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `yellowdog-python-examples-5.0.7/PYPI_README.md` & `yellowdog-python-examples-6.0.0/PYPI_README.md`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.7/README.md` & `yellowdog-python-examples-6.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -19,17 +19,17 @@
 * [Work Requirement Properties](#work-requirement-properties)
    * [Work Requirement JSON File Structure](#work-requirement-json-file-structure)
    * [Property Inheritance](#property-inheritance)
    * [Work Requirement Property Dictionary](#work-requirement-property-dictionary)
    * [Automatic Properties](#automatic-properties)
       * [Work Requirement, Task Group and Task Naming](#work-requirement-task-group-and-task-naming)
       * [Task Types](#task-types)
-         * [Bash Tasks](#bash-tasks)
+         * [Bash, Python and PowerShell Tasks](#bash-python-and-powershell-tasks)
          * [Docker Tasks](#docker-tasks)
-         * [Bash &amp; Docker without Automatic Processing](#bash--docker-without-automatic-processing)
+         * [Bash, Python, PowerShell and Docker without Automatic Processing](#bash-python-powershell-and-docker-without-automatic-processing)
       * [Task Counts](#task-counts)
    * [Examples](#examples)
       * [TOML Properties in the workRequirement Section](#toml-properties-in-the-workrequirement-section)
       * [JSON Properties at the Work Requirement Level](#json-properties-at-the-work-requirement-level)
       * [JSON Properties at the Task Group Level](#json-properties-at-the-task-group-level)
       * [JSON Properties at the Task Level](#json-properties-at-the-task-level)
    * [Variable Substitutions in Work Requirement Properties](#variable-substitutions-in-work-requirement-properties)
@@ -80,15 +80,15 @@
    * [yd-delete](#yd-delete)
    * [yd-upload](#yd-upload)
    * [yd-shutdown](#yd-shutdown)
    * [yd-instantiate](#yd-instantiate)
       * [Test-Running a Dynamic Template](#test-running-a-dynamic-template)
    * [yd-terminate](#yd-terminate)
 
-<!-- Added by: pwt, at: Fri Apr 14 15:14:49 BST 2023 -->
+<!-- Added by: pwt, at: Mon Jun  5 18:32:03 BST 2023 -->
 
 <!--te-->
 
 # Overview
 
 This repository contains a set of example Python scripts for interacting with the YellowDog Platform. The scripts use the **[YellowDog Python SDK](https://docs.yellowdog.co/api/python/index.html)**, the code for which can be found [on GitHub](https://github.com/yellowdog/yellowdog-sdk-python-public).
 
@@ -482,21 +482,22 @@
 
 ### Task Types
 
 - If `taskType` is set only at the TOML file level, then `taskTypes` is automatically populated for Task Groups, unless overridden.
 - If `taskType` is set at the Task level, then `taskTypes` is automatically populated for the Task Groups level using the accumulated Task Types from the Tasks included in each Task Group, unless overridden.
 - If `taskTypes` is set at the Task Group Level, and has only one Task Type entry, then `taskType` is automatically set at the Task Level using the single Task Type, unless overridden.
 
-For the **`bash`** and **`docker`** task types, some automatic processing will be performed if the **`executable`** property is set.
+For the **`bash`**, **`powershell`** and **`docker`** task types, some automatic processing will be performed if the **`executable`** property is set.
 
-#### Bash Tasks
+#### Bash, Python and PowerShell Tasks
 
-For the **`bash`** Task Type, the script nominated in the `executable` property is automatically added to the `inputs` list (if not already present). This means the script file will be uploaded to the Object Store, and made a requirement of the Task when it runs.
+As a convenience, for the **`bash`**, **`python`**, and **`powershell`** Task Types, the script nominated in the **`executable`** property is automatically added to the `inputs` list (if not already present). This means the script file will be uploaded to the Object Store, and made a requirement of the Task when it runs.
+
+Using a Bash Task as an example (in TOML form):
 
-For example (in TOML form):
 ```toml
 taskType = "bash"
 executable = "my_bash_script.sh"
 arguments = ["1", "2", "3"]
 ```
 is equivalent to:
 
@@ -524,17 +525,17 @@
 
 ```toml
 taskType = "docker"
 arguments = ["--env E1=EeeOne", "my_dockerhubrepo/my_container_image", "1", "2", "3"]
 environment = {DOCKER_USERNAME = "my_user", DOCKER_PASSWORD = "my_password"}
 ```
 
-#### Bash & Docker without Automatic Processing
+#### Bash, Python, PowerShell and Docker without Automatic Processing
 
-If the `executable` property is not supplied, the automatic processing above for `bash` and `docker` taskTypes is not applied.
+If the `executable` property is not supplied, the automatic processing described above for `bash`, `python`, `powershell`, and `docker` taskTypes is not applied.
 
 ### Task Counts
 
 This property will expand the number of Tasks to match `taskCount`.
 
 The `taskCount` property can be set only in the `workRequirement` section of the `config.toml` file, or in the `taskGroup` section(s) of a JSON Work Requirement definition.
 
@@ -1287,70 +1288,62 @@
 
 ### Inspecting the Results of CSV Variable Substitution
 
 The `--process-csv-only` (or `-p`) option can be used with `yd-submit` to output the JSON Work Requirement after CSV variable substitutions only, prior to all other substitutions and property inheritance applied by `yd-submit`.
 
 # Worker Pool Properties
 
-The `workerPool` section of the TOML file defines the properties of the Worker Pool to be created, and is used by the `yd-provision` command. The only mandatory property is `templateId`. All other properties have defaults (or are not required).
+The `workerPool` section of the TOML file defines the properties of the Worker Pool to be created, and is used by the `yd-provision` command. A subset of the properties is also used by the `yd-instantiate` command, for creating standalone Compute Requirements that are not associated with Worker Pools.
+
+The only mandatory property is `templateId`. All other properties have defaults (or are not required).
 
 The following properties are available:
 
-| Property                   | Description                                                                                                                     | Default   |
-|:---------------------------|:--------------------------------------------------------------------------------------------------------------------------------|:----------|
-| `ascAllNodesInactive`      | The time in minutes for which all nodes can be inactive before Worker Pool auto-shutdown. Overrides `autoShutdownDelay`.        |           |
-| `ascAllWorkersReleased`    | The time in minutes for which all node Workers can be released before Worker Pool auto-shutdown. Overrides `autoShutdownDelay`. |           |
-| `ascNodeActionFailed`      | The time in minutes after a Node Action failure before Worker Pool auto-shutdown. Overrides `autoShutdownDelay`.                |           |
-| `ascUnclaimedAfterStartup` | The time in minutes for which no Workers have been claimed before Worker Pool auto-shutdown. Overrides `autoShutdownDelay`.     |           |
-| `ascNoRegisteredWorkers`   | Whether to shut down the Worker Pool if no Workers have registered within `nodeBootTimeLimit`.                                  | `false`   |
-| `autoShutdown`             | Whether the Worker Pool is shut down once an auto-shutdown condition is met.                                                    | `true`    |
-| `autoShutdownDelay`        | Default auto-shutdown delay in minutes before the Worker Pool is shut down.                                                     | `10.0`    |
-| `imagesId`                 | The images ID to use when booting instances.                                                                                    |           |
-| `instanceTags`             | The dictionary of instance tags to apply to the instances.                                                                      |           |
-| `minNodes`                 | The minimum number of nodes to which the Worker Pool can be scaled down.                                                        | `0`       |
-| `maxNodes`                 | The maximum number of nodes to which the Worker Pool can be scaled up.                                                          | `1`       |
-| `name`                     | The name of the Worker Pool.                                                                                                    | Automatic |
-| `nodeBootTimeLimit`        | The time in minutes allowed for a node to boot and register with the platform before it is terminated.                          | `10.0`    |
-| `nodeIdleGracePeriod`      | The time in minutes after a node registers during which the idle check is not applied.                                          | `2.0`     |
-| `nodeIdleTimeLimit`        | The time in minutes for which a node can be idle before it can be shut down by auto-scaling.                                    | `5.0`     |
-| `targetInstanceCount`      | The initial number of nodes to create for the Worker Pool.                                                                      | `1`       |
-| `templateId`               | The YellowDog Compute Template ID to use for provisioning.                                                                      |           |
-| `userData`                 | User Data to be supplied to instances on boot.                                                                                  |           |
-| `userDataFile`             | As above, but read the User Data from the filename supplied in this property.                                                   |           |
-| `userDataFiles`            | As above, but create the User Data by concatenating the contents of a list of filenames supplied in this property.              |           |
-| `workersPerVCPU`           | The number of Workers to establish per vCPU on each node in the Worker Pool. (Overrides `workersPerNode`.)                      |           |
-| `workersPerNode`           | The number of Workers to establish on each node in the Worker Pool.                                                             | `1`       |
-| `workerPoolData`           | The name of a file containing a JSON document defining a Worker Pool.                                                           |           |
-| `workerTag`                | The Worker Tag to publish for the all of the Workers.                                                                           |           |
+| Property                  | Description                                                                                                             | Default                 |
+|:--------------------------|:------------------------------------------------------------------------------------------------------------------------|:------------------------|
+| `idleNodeShutdownEnabled` | Whether to shut down nodes that have been idle for `idleNodeShutdownTimeout` minutes.                                   | `True`                  |
+| `idleNodeShutdownTimeout` | The timeout in minutes after which an idle node will be shut down if `idleNodeShutdownEnabled` is set to `True`.        | `5.0`                   |
+| `idlePoolShutdownEnabled` | Whether to shut down the Worker Pool when it has been idle for `idlePoolShutdownTimeout` minutes.                       | `True`                  |
+| `idlePoolShutdownTimeout` | The timeout in minutes after which an idle Worker Pool will be shut down if `idlePoolShutdownEnabled` is set to `True`. | `30.0`                  |
+| `imagesId`                | The images ID to use when booting instances.                                                                            |                         |
+| `instanceTags`            | The dictionary of instance tags to apply to the instances.                                                              |                         |
+| `minNodes`                | The minimum number of nodes to which the Worker Pool can be scaled down.                                                | `0`                     |
+| `maxNodes`                | The maximum number of nodes to which the Worker Pool can be scaled up.                                                  | `1`                     |
+| `name`                    | The name of the Worker Pool.                                                                                            | Automatically Generated |
+| `nodeBootTimeout`         | The time in minutes allowed for a node to boot and register with the platform, otherwise it will be terminated.         | `10.0`                  |
+| `targetInstanceCount`     | The initial number of nodes to create for the Worker Pool.                                                              | `1`                     |
+| `templateId`              | The YellowDog Compute Template ID to use for provisioning. (**Required**, no default provided.)                         |                         |
+| `userData`                | User Data to be supplied to instances on boot.                                                                          |                         |
+| `userDataFile`            | As above, but read the User Data from the filename supplied in this property.                                           |                         |
+| `userDataFiles`           | As above, but create the User Data by concatenating the contents of the list of filenames supplied in this property.    |                         |
+| `workersPerVCPU`          | The number of Workers to establish per vCPU on each node in the Worker Pool. (Overrides `workersPerNode`.)              |                         |
+| `workersPerNode`          | The number of Workers to establish on each node in the Worker Pool.                                                     | `1`                     |
+| `workerPoolData`          | The name of a file containing a JSON document defining a Worker Pool.                                                   |                         |
+| `workerTag`               | The Worker Tag to publish for the all of the Workers on the node.                                                       |                         |
 
 ## Automatic Properties
 
 The name of the Worker Pool, if not supplied, is automatically generated using a concatenation of `wp_`, the `tag` property, a UTC timestamp, and three random hex characters: e,g,. `wp_mytag_221024-155524-b0a`.
 
 ## TOML Properties in the `workerPool` Section
 
 Here's an example of the `workerPool` section of a TOML configuration file, showing all the possible properties that can be set:
 
 ```toml
 [workerPool]
-    ascAllNodesInactive = 10
-    ascAllWorkersReleased = 10
-    ascNodeActionFailed = 10
-    ascUnclaimedAfterStartup = 10
-    ascNoRegisteredWorkers = true
-    autoShutdown = true
-    autoShutdownDelay = 10
+    idleNodeShutdownEnabled = true
+    idleNodeShutdownTimeout = 10.0
+    idlePoolShutdownEnabled = true
+    idlePoolShutdownTimeout = 60.0
     imagesId = "ydid:imgfam:000000:41962592-577c-4fde-ab03-d852465e7f8b"
     instanceTags = {}
     maxNodes = 1
     minNodes = 1
     name = "my-worker-pool"
-    nodeBootTimeLimit = 5
-    nodeIdleGracePeriod = 5
-    nodeIdleTimeLimit = 3
+    nodeBootTimeout = 5
     targetInstanceCount = 1
     templateId = "ydid:crt:D9C548:465a107c-7cea-46e3-9fdd-15116cb92c40"
     # Note: only one of 'userData'/'userDataFile'/'userDataFiles' should be set
     userData = ""
     userDataFile = "myuserdata.txt"
     userDataFiles = ["myuserdata1.txt", "myuserdata2.txt"]
     workerTag = "tag-{{username}}"
@@ -1364,39 +1357,33 @@
 
 The JSON specification allows the creation of **Advanced Worker Pools**, with different node types and the ability to specify Node Actions.
 
 When using a JSON document to specify the Worker Pool, the schema of the document is identical to that expected by the YellowDog REST API for Worker Pool Provisioning.
 
 ### Worker Pool JSON Examples
 
-The example below is of a simple JSON specification of a Worker Pool with one initial node,  shutdown conditions, etc.
+The example below is of a simple JSON specification of a Worker Pool with one initial node, Worker Pool shutdown, etc.
 
 ```json
 {
   "requirementTemplateUsage": {
     "maintainInstanceCount": false,
     "requirementName": "wp_pyex-primes_230113-161528-da0",
     "requirementNamespace": "pyexamples",
     "requirementTag": "pyex-primes",
     "targetInstanceCount": 1,
     "templateId": "ydid:crt:D9C548:465a107c-7cea-46e3-9fdd-15116cb92c40"
   },
   "provisionedProperties": {
-    "autoShutdown": true,
-    "autoShutdownConditions": [
-      {"delay": "PT1H", "type": "co.yellowdog.platform.model.AllWorkersReleasedShutdownCondition"},
-      {"delay": "PT1H", "type": "co.yellowdog.platform.model.AllNodesInactiveShutdownCondition"},
-      {"delay": "PT1H", "type": "co.yellowdog.platform.model.UnclaimedAfterStartupShutdownCondition"},
-      {"delay": "PT1H", "type": "co.yellowdog.platform.model.NodeActionFailedShutdownCondition"},
-      {"type": "co.yellowdog.platform.model.NoRegisteredWorkersShutdownCondition"}
-    ],
+    "idleNodeShutdown": {"enabled": true, "timeout": "PT10M"},
+    "idlePoolShutdown": {"enabled": true, "timeout": "PT1H"},
     "createNodeWorkers": {"targetCount": 1, "targetType": "PER_VCPU"},
     "maxNodes": 5,
     "minNodes": 0,
-    "nodeBootTimeLimit": "PT5M",
+    "nodeBootTimeout": "PT5M",
     "nodeIdleGracePeriod": "PT3M",
     "nodeIdleTimeLimit": "PT3M",
     "workerTag": "pyex-bash-docker"
   }
 }
 ```
 
@@ -1409,15 +1396,14 @@
     "targetInstanceCount": 6,
     "templateId": "ydid:crt:D9C548:a7eda287-f9d6-4bc8-b2dc-455344057257",
     "requirementName": "wp_pyex-slurm_230113-165615-2b7",
     "requirementNamespace": "pyexamples",
     "requirementTag": "pyex-slurm"
   },
   "provisionedProperties": {
-    "autoShutdown": true,
     "createNodeWorkers": {"targetCount": 0, "targetType": "PER_NODE"},
     "nodeConfiguration": {
       "nodeTypes": [
         {"name": "slurmctld", "count": 1},
         {"name": "slurmd", "min": 5, "slotNumbering": "REUSABLE"}
       ],
       "nodeEvents": {
@@ -1510,19 +1496,19 @@
 - `templateId`
 - `userData`
 - `userDataFile`
 - `userDataFiles`
 
 **Properties Inherited within the `provisionedProperties` Property**
 
-- `autoShutdown`
-- `autoShutdownConditions`: derived from the `autoShutdownDelay`, `ascAllNodesInactive`, `ascAllWorkersReleased`, `ascNodeActionFailed`, `ascUnclaimedAfterStartup` and `ascNoRegisteredWorkers` properties in the `TOML` configuration
-- `nodeBootTimeLimit`
-- `nodeIdleGracePeriod`
-- `nodeIdleTimeLimit`
+- `idleNodeShutdownEnabled`
+- `idleNodeShutdownTimeout`
+- `idlePoolShutdownEnabled`
+- `idlePoolShutdownTimeout`
+- `nodeBootTimeout`
 - `workerTag`
 
 ## Variable Substitutions in Worker Pool Properties
 
 Variable substitutions can be used within any property value in TOML configuration files or Worker Pool JSON files. See the description [above](#variable-substitutions) for more details on variable substitutions. This is a powerful feature that allows Worker Pools to be parameterised by supplying values on the command line, via environment variables, or via the TOML file.
 
 An important distinction **only** when using variable substitutions within Worker Pool JSON documents is that each directive **must be preceded by a `__` (double underscore)** to disambiguate it from variable substitutions that are to be passed directly to the API. For example, use: `__{{username}}` to apply a substitution for the `username` default substitution.
```

### Comparing `yellowdog-python-examples-5.0.7/pyproject.toml` & `yellowdog-python-examples-6.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.7/setup.cfg` & `yellowdog-python-examples-6.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.7/yd_commands/abort.py` & `yellowdog-python-examples-6.0.0/yd_commands/abort.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.7/yd_commands/admin.py` & `yellowdog-python-examples-6.0.0/yd_commands/admin.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.7/yd_commands/args.py` & `yellowdog-python-examples-6.0.0/yd_commands/args.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,22 +140,14 @@
                 "-X",
                 type=str,
                 required=False,
                 help="the executable to use",
                 metavar="<executable>",
             )
             parser.add_argument(
-                "--task-batch-size",
-                "-b",
-                type=int,
-                required=False,
-                help="the batch size for task submission",
-                metavar="<batch_size>",
-            )
-            parser.add_argument(
                 "--task-type",
                 "-T",
                 type=str,
                 required=False,
                 help="the task type to use",
                 metavar="<task_type>",
             )
@@ -164,14 +156,29 @@
                 "-C",
                 type=int,
                 required=False,
                 help="the number of times to submit the task",
                 metavar="<task_count>",
             )
             parser.add_argument(
+                "--task-batch-size",
+                "-b",
+                type=int,
+                required=False,
+                help="the batch size for task submission",
+                metavar="<batch_size>",
+            )
+            parser.add_argument(
+                "--pause-between-batches",
+                "-P",
+                action="store_true",
+                required=False,
+                help="pause for user input between batches (for debugging)",
+            )
+            parser.add_argument(
                 "--csv-file",
                 "-V",
                 type=str,
                 required=False,
                 action="append",
                 help="the CSV file(s) from which to read task data",
                 metavar="<data.csv>",
@@ -569,14 +576,18 @@
     def report(self) -> Optional[bool]:
         return self.args.report
 
     @property
     def jsonnet_dry_run(self) -> Optional[bool]:
         return self.args.jsonnet_dry_run
 
+    @property
+    def pause_between_batches(self) -> Optional[bool]:
+        return self.args.pause_between_batches
+
 
 def lookup_module_description(module_name: str) -> Optional[str]:
     """
     Descriptive string for the module's purpose.
     """
     prefix = "YellowDog example utility for "
     suffix = None
```

### Comparing `yellowdog-python-examples-5.0.7/yd_commands/cancel.py` & `yellowdog-python-examples-6.0.0/yd_commands/cancel.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.7/yd_commands/check_imports.py` & `yellowdog-python-examples-6.0.0/yd_commands/check_imports.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.7/yd_commands/compact_json.py` & `yellowdog-python-examples-6.0.0/yd_commands/compact_json.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.7/yd_commands/config.py` & `yellowdog-python-examples-6.0.0/yd_commands/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -51,15 +51,14 @@
 TASK_BATCH_SIZE_DEFAULT = 2000
 DEFAULT_URL = "https://portal.yellowdog.co/api"
 
 
 @dataclass
 class ConfigWorkRequirement:
     args: List[str] = field(default_factory=list)
-    bash_script: Optional[str] = None  # Deprecated
     capture_taskoutput: bool = True
     completed_task_ttl: Optional[float] = None  # In minutes
     csv_files: Optional[List[str]] = None
     docker_env: Optional[Dict] = None
     docker_password: Optional[str] = None
     docker_username: Optional[str] = None
     env: Dict = field(default_factory=dict)
@@ -100,32 +99,26 @@
 
 
 CR_BATCH_SIZE_DEFAULT = 10000
 
 
 @dataclass
 class ConfigWorkerPool:
-    asc_all_nodes_inactive: Optional[float] = None
-    asc_all_workers_released: Optional[float] = None
-    asc_node_action_failed: Optional[float] = None
-    asc_no_registered_workers: Optional[bool] = None
-    asc_unclaimed_after_startup: Optional[float] = None
-    auto_scaling_idle_delay: float = 10  # Deprecated
-    auto_shutdown: bool = True
-    auto_shutdown_delay: float = 10
     compute_requirement_batch_size: int = CR_BATCH_SIZE_DEFAULT
+    idle_node_shutdown_enabled: bool = True
+    idle_node_shutdown_timeout: float = 5.0
+    idle_pool_shutdown_enabled: bool = True
+    idle_pool_shutdown_timeout: float = 30.0
     images_id: Optional[str] = (None,)
     instance_tags: Optional[Dict] = None
     maintainInstanceCount: bool = False  # Only for yd-instantiate
     max_nodes: int = 0
     min_nodes: int = 0
     name: Optional[str] = None
-    node_boot_time_limit: float = 10
-    node_idle_grace_period: float = 2
-    node_idle_time_limit: float = 5
+    node_boot_timeout: float = 10.0
     target_instance_count: int = 0
     template_id: Optional[str] = None
     user_data: Optional[str] = None
     user_data_file: Optional[str] = None
     user_data_files: Optional[List[str]] = None
     worker_pool_data_file: Optional[str] = None
     worker_tag: Optional[str] = None
@@ -304,15 +297,14 @@
             wr_section.get(TASK_BATCH_SIZE, TASK_BATCH_SIZE_DEFAULT)
             if ARGS_PARSER.task_batch_size is None
             else ARGS_PARSER.task_batch_size
         )
 
         return ConfigWorkRequirement(
             args=wr_section.get(ARGS, []),
-            bash_script=wr_section.get(BASH_SCRIPT, None),  # Deprecated
             capture_taskoutput=wr_section.get(CAPTURE_TASKOUTPUT, True),
             completed_task_ttl=wr_section.get(COMPLETED_TASK_TTL, None),
             csv_files=csv_files,
             docker_env=wr_section.get(DOCKER_ENV, None),
             docker_password=wr_section.get(DOCKER_PASSWORD, None),
             docker_username=wr_section.get(DOCKER_USERNAME, None),
             env=wr_section.get(ENV, {}),
@@ -374,42 +366,32 @@
         worker_pool_data_file = substitute_variable_str(wp_section.get(WP_DATA, None))
         if worker_pool_data_file is not None:
             worker_pool_data_file = pathname_relative_to_config_file(
                 worker_pool_data_file
             )
 
         return ConfigWorkerPool(
-            asc_all_nodes_inactive=wp_section.get(ASC_ALL_NODES_INACTIVE, None),
-            asc_all_workers_released=wp_section.get(ASC_ALL_WORKERS_RELEASED, None),
-            asc_node_action_failed=wp_section.get(ASC_NODE_ACTION_FAILED, None),
-            asc_no_registered_workers=wp_section.get(ASC_NO_REGISTERED_WORKERS, None),
-            asc_unclaimed_after_startup=wp_section.get(
-                ASC_UNCLAIMED_AFTER_STARTUP, None
-            ),
-            auto_scaling_idle_delay=wp_section.get(AUTO_SCALING_IDLE_DELAY, 10),
-            auto_shutdown=wp_section.get(AUTO_SHUTDOWN, True),
-            auto_shutdown_delay=wp_section.get(AUTO_SHUTDOWN_DELAY, 10),
             compute_requirement_batch_size=wp_section.get(
                 COMPUTE_REQUIREMENT_BATCH_SIZE, CR_BATCH_SIZE_DEFAULT
             ),
+            idle_node_shutdown_enabled=wp_section.get(IDLE_NODE_SHUTDOWN_ENABLED, True),
+            idle_node_shutdown_timeout=wp_section.get(IDLE_NODE_SHUTDOWN_TIMEOUT, 5.0),
+            idle_pool_shutdown_enabled=wp_section.get(IDLE_POOL_SHUTDOWN_ENABLED, True),
+            idle_pool_shutdown_timeout=wp_section.get(IDLE_POOL_SHUTDOWN_TIMEOUT, 30.0),
             images_id=wp_section.get(IMAGES_ID, None),
             instance_tags=wp_section.get(INSTANCE_TAGS, None),
             maintainInstanceCount=wp_section.get(MAINTAIN_INSTANCE_COUNT, False),
             max_nodes=wp_section.get(
                 MAX_NODES, max(1, wp_section.get(TARGET_INSTANCE_COUNT, 1))
             ),
             min_nodes=wp_section.get(MIN_NODES, 0),
             name=substitute_variable_str(
                 wp_section.get(WP_NAME, None),
             ),
-            node_boot_time_limit=wp_section.get(NODE_BOOT_TIME_LIMIT, 10),
-            node_idle_grace_period=wp_section.get(NODE_IDLE_GRACE_PERIOD, 2),
-            node_idle_time_limit=wp_section.get(
-                NODE_IDLE_TIME_LIMIT, wp_section.get(AUTO_SCALING_IDLE_DELAY, 5)
-            ),
+            node_boot_timeout=wp_section.get(NODE_BOOT_TIMEOUT, 10.0),
             target_instance_count=wp_section.get(TARGET_INSTANCE_COUNT, 1),
             template_id=wp_section.get(TEMPLATE_ID, None),
             user_data=wp_section.get(USERDATA, None),
             user_data_file=wp_section.get(USERDATAFILE, None),
             user_data_files=wp_section.get(USERDATAFILES, None),
             worker_pool_data_file=worker_pool_data_file,
             worker_tag=worker_tag,
```

### Comparing `yellowdog-python-examples-5.0.7/yd_commands/config_keys.py` & `yellowdog-python-examples-6.0.0/yd_commands/config_keys.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,12 @@
 """
 Configuration key strings
 """
 
 ARGS = "arguments"  # List
-ASC_ALL_NODES_INACTIVE = "ascAllNodesInactive"  # Float
-ASC_ALL_WORKERS_RELEASED = "ascAllWorkersReleased"  # Float
-ASC_NODE_ACTION_FAILED = "ascNodeActionFailed"  # Float
-ASC_NO_REGISTERED_WORKERS = "ascNoRegisteredWorkers"  # Bool
-ASC_UNCLAIMED_AFTER_STARTUP = "ascUnclaimedAfterStartup"  # Float
-AUTO_SCALING_IDLE_DELAY = "autoscalingIdleDelay"  # Float
-AUTO_SHUTDOWN = "autoShutdown"  # Boolean
-AUTO_SHUTDOWN_DELAY = "autoShutdownDelay"  # Float
 CAPTURE_TASKOUTPUT = "captureTaskOutput"  # Bool
 COMMON_SECTION = "common"  # No value
 COMPLETED_TASK_TTL = "completedTaskTtl"  # Float
 COMPUTE_REQUIREMENT_BATCH_SIZE = "computeRequirementBatchSize"  # Integer
 CSV_FILE = "csvFile"  # String
 CSV_FILES = "csvFiles"  # List of Strings
 DEPENDENT_ON = "dependentOn"  # String
@@ -25,14 +17,18 @@
 EXCLUSIVE_WORKERS = "exclusiveWorkers"  # Boolean
 EXECUTABLE = "executable"  # String
 FINISH_IF_ALL_TASKS_FINISHED = "finishIfAllTasksFinished"  # Boolean
 FINISH_IF_ANY_TASK_FAILED = "finishIfAnyTaskFailed"  # Boolean
 FLATTEN_PATHS = "flattenInputPaths"  # Boolean
 FLATTEN_UPLOAD_PATHS = "flattenUploadPaths"  # Boolean
 FULFIL_ON_SUBMIT = "fulfilOnSubmit"  # Boolean
+IDLE_NODE_SHUTDOWN_ENABLED = "idleNodeShutdownEnabled"  # Bool
+IDLE_NODE_SHUTDOWN_TIMEOUT = "idleNodeShutdownTimeout"  # Float
+IDLE_POOL_SHUTDOWN_ENABLED = "idlePoolShutdownEnabled"  # Bool
+IDLE_POOL_SHUTDOWN_TIMEOUT = "idlePoolShutdownTimeout"  # Float
 IMAGES_ID = "imagesId"  # String
 IMPORT = "import"  # String
 INPUT_FILES = "inputs"  # List of Strings
 INPUTS_OPTIONAL = "inputsOptional"  # List of Strings
 INSTANCE_TAGS = "instanceTags"  # List of Strings
 INSTANCE_TYPES = "instanceTypes"  # List of Strings
 KEY = "key"  # String
@@ -41,17 +37,15 @@
 MAX_RETRIES = "maximumTaskRetries"  # Integer
 MAX_WORKERS = "maxWorkers"  # Integer
 MIN_NODES = "minNodes"  # Integer
 MIN_WORKERS = "minWorkers"  # Integer
 NAME = "name"  # String
 NAMESPACE = "namespace"  # String
 NAME_TAG = "tag"  # String
-NODE_BOOT_TIME_LIMIT = "nodeBootTimeLimit"  # Float
-NODE_IDLE_GRACE_PERIOD = "nodeIdleGracePeriod"  # Float
-NODE_IDLE_TIME_LIMIT = "nodeIdleTimeLimit"  # Float
+NODE_BOOT_TIMEOUT = "nodeBootTimeout"  # Float
 OUTPUT_FILES = "outputs"  # List of Strings
 OUTPUT_FILES_REQUIRED = "outputsRequired"  # List of Strings
 PRIORITY = "priority"  # Float
 PROVIDERS = "providers"  # List of Strings
 RAM = "ram"  # List of two Floats
 REGIONS = "regions"  # List of Strings
 SECRET = "secret"  # String
@@ -86,28 +80,16 @@
 WORKER_TAGS = "workerTags"  # List of Strings
 WORK_REQUIREMENT_SECTION = "workRequirement"  # No value
 WP_DATA = "workerPoolData"  # String
 WP_NAME = "name"  # String
 WR_DATA = "workRequirementData"  # String
 WR_NAME = "name"  # String
 
-# Legacy
-BASH_SCRIPT = "bashScript"  # String
-
 ALL_KEYS = [
     ARGS,
-    ASC_ALL_NODES_INACTIVE,
-    ASC_ALL_WORKERS_RELEASED,
-    ASC_NODE_ACTION_FAILED,
-    ASC_NO_REGISTERED_WORKERS,
-    ASC_UNCLAIMED_AFTER_STARTUP,
-    AUTO_SCALING_IDLE_DELAY,
-    AUTO_SHUTDOWN,
-    AUTO_SHUTDOWN_DELAY,
-    BASH_SCRIPT,
     CAPTURE_TASKOUTPUT,
     COMMON_SECTION,
     COMPLETED_TASK_TTL,
     COMPUTE_REQUIREMENT_BATCH_SIZE,
     CSV_FILE,
     CSV_FILES,
     DEPENDENT_ON,
@@ -118,14 +100,18 @@
     EXCLUSIVE_WORKERS,
     EXECUTABLE,
     FINISH_IF_ALL_TASKS_FINISHED,
     FINISH_IF_ANY_TASK_FAILED,
     FLATTEN_PATHS,
     FLATTEN_UPLOAD_PATHS,
     FULFIL_ON_SUBMIT,
+    IDLE_NODE_SHUTDOWN_ENABLED,
+    IDLE_NODE_SHUTDOWN_TIMEOUT,
+    IDLE_POOL_SHUTDOWN_ENABLED,
+    IDLE_POOL_SHUTDOWN_TIMEOUT,
     IMAGES_ID,
     IMPORT,
     INPUT_FILES,
     INPUTS_OPTIONAL,
     INSTANCE_TAGS,
     INSTANCE_TYPES,
     KEY,
@@ -133,17 +119,15 @@
     MAX_NODES,
     MAX_RETRIES,
     MAX_WORKERS,
     MIN_NODES,
     MIN_WORKERS,
     NAMESPACE,
     NAME_TAG,
-    NODE_BOOT_TIME_LIMIT,
-    NODE_IDLE_GRACE_PERIOD,
-    NODE_IDLE_TIME_LIMIT,
+    NODE_BOOT_TIMEOUT,
     OUTPUT_FILES,
     OUTPUT_FILES_REQUIRED,
     PRIORITY,
     PROVIDERS,
     RAM,
     REGIONS,
     SECRET,
```

### Comparing `yellowdog-python-examples-5.0.7/yd_commands/csv_data.py` & `yellowdog-python-examples-6.0.0/yd_commands/csv_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Module for handling Task data supplied in a CSV file
+Module for handling Task data supplied in CSV files.
 """
 
 import csv
 import re
 from ast import literal_eval
 from collections import OrderedDict
 from json import load as json_load
@@ -332,15 +332,14 @@
     """
     wr_data = {TASK_GROUPS: [{TASKS: [{}]}]}
     task_proto = wr_data[TASK_GROUPS][0][TASKS][0]
     csv_data = CSV_DATA_CACHE.get_csv_task_data(csv_file.split(":")[0])
     # Populate properties that can be set at Task level only
     for config_value, config_name in [
         (config_wr.args, ARGS),
-        (config_wr.bash_script, BASH_SCRIPT),
         (config_wr.capture_taskoutput, CAPTURE_TASKOUTPUT),
         (config_wr.docker_env, DOCKER_ENV),
         (config_wr.docker_password, DOCKER_PASSWORD),
         (config_wr.docker_username, DOCKER_USERNAME),
         (config_wr.env, ENV),
         (config_wr.executable, EXECUTABLE),
         (config_wr.flatten_input_paths, FLATTEN_PATHS),
```

### Comparing `yellowdog-python-examples-5.0.7/yd_commands/delete.py` & `yellowdog-python-examples-6.0.0/yd_commands/delete.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.7/yd_commands/download.py` & `yellowdog-python-examples-6.0.0/yd_commands/download.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.7/yd_commands/instantiate.py` & `yellowdog-python-examples-6.0.0/yd_commands/instantiate.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.7/yd_commands/interactive.py` & `yellowdog-python-examples-6.0.0/yd_commands/interactive.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.7/yd_commands/jsonnet2json.py` & `yellowdog-python-examples-6.0.0/yd_commands/jsonnet2json.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.7/yd_commands/list.py` & `yellowdog-python-examples-6.0.0/yd_commands/list.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.7/yd_commands/object_utilities.py` & `yellowdog-python-examples-6.0.0/yd_commands/object_utilities.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.7/yd_commands/printing.py` & `yellowdog-python-examples-6.0.0/yd_commands/printing.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.7/yd_commands/provision.py` & `yellowdog-python-examples-6.0.0/yd_commands/provision.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,32 +8,28 @@
 from datetime import timedelta
 from math import ceil, floor
 from typing import Dict, List, Optional
 
 import requests
 from yellowdog_client.common.iso_datetime import iso_timedelta_format
 from yellowdog_client.model import (
-    AllNodesInactiveShutdownCondition,
-    AllWorkersReleasedShutdownCondition,
+    AutoShutdown,
     ComputeRequirementTemplateUsage,
-    NodeActionFailedShutdownCondition,
     NodeWorkerTarget,
-    NoRegisteredWorkersShutdownCondition,
     ProvisionedWorkerPoolProperties,
-    UnclaimedAfterStartupShutdownCondition,
 )
 
 from yd_commands.args import ARGS_PARSER
 from yd_commands.config import (
     ConfigWorkerPool,
     generate_id,
     link_entity,
     load_config_worker_pool,
 )
-from yd_commands.config_keys import MAINTAIN_INSTANCE_COUNT, USERDATA, USERDATAFILE
+from yd_commands.config_keys import MAINTAIN_INSTANCE_COUNT
 from yd_commands.printing import (
     print_error,
     print_log,
     print_worker_pool,
     print_yd_object,
 )
 from yd_commands.provision_utils import get_user_data_property
@@ -113,101 +109,49 @@
             if reqt_template_usage.get(key) is None and value is not None:
                 print_log(f"Setting 'requirementTemplateUsage.{key}': '{value}'")
                 reqt_template_usage[key] = value
 
         # provisionedProperties insertions
         provisioned_properties = wp_data["provisionedProperties"]
 
-        # determine shutdown delays
-        auto_shutdown_delay: str = iso_timedelta_format(
-            timedelta(minutes=CONFIG_WP.auto_shutdown_delay)
-        )
-        asc_all_nodes_inactive = (
-            auto_shutdown_delay
-            if CONFIG_WP.asc_all_nodes_inactive is None
-            else iso_timedelta_format(
-                timedelta(minutes=CONFIG_WP.asc_all_nodes_inactive)
-            )
-        )
-        asc_all_workers_released = (
-            auto_shutdown_delay
-            if CONFIG_WP.asc_all_workers_released is None
-            else iso_timedelta_format(
-                timedelta(minutes=CONFIG_WP.asc_all_workers_released)
-            )
-        )
-        asc_node_action_failed = (
-            auto_shutdown_delay
-            if CONFIG_WP.asc_node_action_failed is None
-            else iso_timedelta_format(
-                timedelta(minutes=CONFIG_WP.asc_node_action_failed)
-            )
-        )
-        asc_unclaimed_after_startup = (
-            auto_shutdown_delay
-            if CONFIG_WP.asc_unclaimed_after_startup is None
-            else iso_timedelta_format(
-                timedelta(minutes=CONFIG_WP.asc_unclaimed_after_startup)
-            )
-        )
-
-        type_prefix = "co.yellowdog.platform.model"
-        auto_shutdown_conditions = [
-            {
-                "delay": asc_all_nodes_inactive,
-                "type": f"{type_prefix}.AllNodesInactiveShutdownCondition",
-            },
-            {
-                "delay": asc_all_workers_released,
-                "type": f"{type_prefix}.AllWorkersReleasedShutdownCondition",
-            },
-            {
-                "delay": asc_node_action_failed,
-                "type": f"{type_prefix}.NodeActionFailedShutdownCondition",
-            },
-            {
-                "delay": asc_unclaimed_after_startup,
-                "type": f"{type_prefix}.UnclaimedAfterStartupShutdownCondition",
-            },
-        ]
-        if CONFIG_WP.asc_no_registered_workers is True:
-            auto_shutdown_conditions.append(
-                {"type": f"{type_prefix}.NoRegisteredWorkersShutdownCondition"}
-            )
-
         for key, value in [
-            ("autoShutdown", CONFIG_WP.auto_shutdown),
-            ("autoShutdownConditions", auto_shutdown_conditions),
             ("workerTag", CONFIG_WP.worker_tag),
             (
-                "nodeBootTimeLimit",
-                iso_timedelta_format(timedelta(minutes=CONFIG_WP.node_boot_time_limit)),
+                "nodeBootTimeout",
+                iso_timedelta_format(timedelta(minutes=CONFIG_WP.node_boot_timeout)),
             ),
             (
-                "nodeIdleGracePeriod",
-                iso_timedelta_format(
-                    timedelta(minutes=CONFIG_WP.node_idle_grace_period)
+                "idleNodeShutdown",
+                (
+                    {
+                        "enabled": True,
+                        "timeout": iso_timedelta_format(
+                            timedelta(minutes=CONFIG_WP.idle_node_shutdown_timeout)
+                        ),
+                    }
+                    if CONFIG_WP.idle_node_shutdown_enabled
+                    else {"enabled": False}
                 ),
             ),
             (
-                "nodeIdleTimeLimit",
-                iso_timedelta_format(timedelta(minutes=CONFIG_WP.node_idle_time_limit)),
+                "idlePoolShutdown",
+                (
+                    {
+                        "enabled": True,
+                        "timeout": iso_timedelta_format(
+                            timedelta(minutes=CONFIG_WP.idle_pool_shutdown_timeout)
+                        ),
+                    }
+                    if CONFIG_WP.idle_pool_shutdown_enabled
+                    else {"enabled": False}
+                ),
             ),
         ]:
             if provisioned_properties.get(key) is None and value is not None:
-                if key == "autoShutdownConditions":
-                    for condition in value:
-                        if not "NoRegisteredWorkers" in condition["type"]:
-                            print_log(
-                                f"Setting '{condition['type']}': '{condition['delay']}'"
-                            )
-                        else:
-                            print_log(f"Setting '{condition['type']}' to 'true'")
-                else:
-                    print_log(f"Setting 'provisionedProperties.{key}': '{value}'")
+                print_log(f"Setting 'provisionedProperties.{key}': '{value}'")
                 provisioned_properties[key] = value
 
     except KeyError as e:
         raise Exception(f"Key error in JSON Worker Pool definition: {e}")
 
     if ARGS_PARSER.dry_run:
         print_log("Dry-run: Printing JSON Worker Pool specification")
@@ -239,63 +183,36 @@
     ):
         print_error(
             "Please ensure that minNodes <= targetInstanceCount <= maxNodes"
             " and maxNodes >= 1"
         )
         raise Exception("Malformed configuration")
 
-    # Set the Worker Pool auto-shutdown conditions
-    if CONFIG_WP.auto_shutdown:
-        shutdown_delay = timedelta(minutes=CONFIG_WP.auto_shutdown_delay)
-        asc_all_nodes_inactive = (
-            shutdown_delay
-            if CONFIG_WP.asc_all_nodes_inactive is None
-            else timedelta(minutes=CONFIG_WP.asc_all_nodes_inactive)
-        )
-        asc_all_workers_released = (
-            shutdown_delay
-            if CONFIG_WP.asc_all_workers_released is None
-            else timedelta(minutes=CONFIG_WP.asc_all_workers_released)
-        )
-        asc_node_action_failed = (
-            shutdown_delay
-            if CONFIG_WP.asc_node_action_failed is None
-            else timedelta(minutes=CONFIG_WP.asc_node_action_failed)
-        )
-        asc_unclaimed_after_startup = (
-            shutdown_delay
-            if CONFIG_WP.asc_unclaimed_after_startup is None
-            else timedelta(minutes=CONFIG_WP.asc_unclaimed_after_startup)
-        )
-        auto_shutdown_conditions = [
-            AllNodesInactiveShutdownCondition(delay=asc_all_nodes_inactive),
-            AllWorkersReleasedShutdownCondition(delay=asc_all_workers_released),
-            NodeActionFailedShutdownCondition(delay=asc_node_action_failed),
-            UnclaimedAfterStartupShutdownCondition(delay=asc_unclaimed_after_startup),
-        ]
-        if CONFIG_WP.asc_no_registered_workers is True:
-            auto_shutdown_conditions.append(NoRegisteredWorkersShutdownCondition())
-    else:
-        auto_shutdown_conditions = []
-
-    # Set auto-scaling time limits
-    node_boot_time_limit = (
+    node_boot_timeout = (
         None
-        if CONFIG_WP.node_boot_time_limit is None
-        else timedelta(minutes=CONFIG_WP.node_boot_time_limit)
+        if CONFIG_WP.node_boot_timeout is None
+        else timedelta(minutes=CONFIG_WP.node_boot_timeout)
     )
-    node_idle_time_limit = (
-        None
-        if CONFIG_WP.node_idle_time_limit is None
-        else timedelta(minutes=CONFIG_WP.node_idle_time_limit)
+
+    idle_node_auto_shutdown = (
+        AutoShutdown(
+            enabled=True,
+            timeout=timedelta(minutes=CONFIG_WP.idle_node_shutdown_timeout),
+        )
+        if CONFIG_WP.idle_node_shutdown_enabled
+        else AutoShutdown(enabled=False)
     )
-    node_idle_grace_period = (
-        None
-        if CONFIG_WP.node_idle_grace_period is None
-        else timedelta(minutes=CONFIG_WP.node_idle_grace_period)
+
+    idle_pool_auto_shutdown = (
+        AutoShutdown(
+            enabled=True,
+            timeout=timedelta(minutes=CONFIG_WP.idle_pool_shutdown_timeout),
+        )
+        if CONFIG_WP.idle_pool_shutdown_enabled
+        else AutoShutdown(enabled=False)
     )
 
     # Establish the number of Workers to create
     if CONFIG_WP.workers_per_vcpu is not None:
         node_workers = NodeWorkerTarget.per_vcpus(CONFIG_WP.workers_per_vcpu)
     else:
         node_workers = NodeWorkerTarget.per_node(CONFIG_WP.workers_per_node)
@@ -349,19 +266,17 @@
                 maintainInstanceCount=False,  # Must be false for Worker Pools
             )
             provisioned_worker_pool_properties = ProvisionedWorkerPoolProperties(
                 createNodeWorkers=node_workers,
                 minNodes=batches[batch_number].min_nodes,
                 maxNodes=batches[batch_number].max_nodes,
                 workerTag=CONFIG_WP.worker_tag,
-                autoShutdown=CONFIG_WP.auto_shutdown,
-                autoShutdownConditions=auto_shutdown_conditions,
-                nodeIdleTimeLimit=node_idle_time_limit,
-                nodeIdleGracePeriod=node_idle_grace_period,
-                nodeBootTimeLimit=node_boot_time_limit,
+                idleNodeShutdown=idle_node_auto_shutdown,
+                idlePoolShutdown=idle_pool_auto_shutdown,
+                nodeBootTimeout=node_boot_timeout,
             )
             if not ARGS_PARSER.dry_run:
                 worker_pool = CLIENT.worker_pool_client.provision_worker_pool(
                     compute_requirement_template_usage,
                     provisioned_worker_pool_properties,
                 )
                 print_log(f"Created {link_entity(CONFIG_COMMON.url, worker_pool)}")
@@ -371,32 +286,38 @@
                     provisioned_worker_pool_properties,
                 )
 
         except Exception as e:
             print_error(f"Unable to provision worker pool")
             raise Exception(e)
 
+    idle_node_shutdown_string = (
+        f"time limit is {CONFIG_WP.idle_node_shutdown_timeout} minute(s)"
+        if CONFIG_WP.idle_node_shutdown_enabled
+        else "is **disabled**"
+    )
+
     print_log(
         "Node boot time limit is "
-        f"{CONFIG_WP.node_boot_time_limit} minute(s) | "
-        "Node idle grace period is "
-        f"{CONFIG_WP.node_idle_grace_period} minute(s) | "
-        "Node idle time limit is "
-        f"{CONFIG_WP.node_idle_time_limit} minute(s)"
-    )
-
-    auto_shutdown = "enabled" if CONFIG_WP.auto_shutdown is True else "disabled"
-    auto_shutdown_msg = f"Auto-Shutdown is {auto_shutdown}"
-    auto_shutdown_msg = (
-        auto_shutdown_msg
-        + f" with a delay of {CONFIG_WP.auto_shutdown_delay} minute(s)"
-        if CONFIG_WP.auto_shutdown is True
-        else auto_shutdown_msg
+        f"{CONFIG_WP.node_boot_timeout} minute(s) | "
+        "Node idle shutdown "
+        f"{idle_node_shutdown_string}"
+    )
+
+    idle_pool_shutdown = (
+        "enabled" if CONFIG_WP.idle_pool_shutdown_enabled else "disabled"
+    )
+    idle_pool_shutdown_msg = f"Worker Pool auto-shutdown is {idle_pool_shutdown}"
+    idle_pool_shutdown_msg = (
+        idle_pool_shutdown_msg
+        + f" with a delay of {CONFIG_WP.idle_pool_shutdown_timeout} minute(s)"
+        if CONFIG_WP.idle_pool_shutdown_enabled
+        else idle_pool_shutdown_msg
     )
-    print_log(auto_shutdown_msg)
+    print_log(idle_pool_shutdown_msg)
 
     if ARGS_PARSER.dry_run:
         print_log("Dry run: Complete")
 
 
 def _allocate_nodes_to_batches(
     max_batch_size: int, initial_nodes: int, min_nodes: int, max_nodes: int
```

### Comparing `yellowdog-python-examples-5.0.7/yd_commands/provision_utils.py` & `yellowdog-python-examples-6.0.0/yd_commands/provision_utils.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.7/yd_commands/reformat_json.py` & `yellowdog-python-examples-6.0.0/yd_commands/reformat_json.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.7/yd_commands/shutdown.py` & `yellowdog-python-examples-6.0.0/yd_commands/shutdown.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.7/yd_commands/submit.py` & `yellowdog-python-examples-6.0.0/yd_commands/submit.py`

 * *Files 0% similar despite different names*

```diff
@@ -491,14 +491,20 @@
     add_substitution_overwrite(
         L_TASK_GROUP_NUMBER, formatted_number_str(tg_number, num_task_groups)
     )
     add_substitution_overwrite(L_TASK_GROUP_COUNT, str(num_task_groups))
 
     # Iterate through batches
     for batch_number in range(num_task_batches):
+        if ARGS_PARSER.pause_between_batches and batch_number > 0:
+            print_log(
+                f"Pausing before submitting batch number {batch_number + 1}. "
+                "Press enter to continue:"
+            )
+            input()
         # Iterate through tasks in the batch
         for task_number in range(
             (TASK_BATCH_SIZE * batch_number),
             min(TASK_BATCH_SIZE * (batch_number + 1), num_tasks),
         ):
             task_group_data = wr_data[TASK_GROUPS][tg_number]
             task = tasks[task_number] if task_count is None else tasks[0]
@@ -948,20 +954,21 @@
                 FLATTEN_PATHS,
                 wr_data.get(FLATTEN_PATHS, CONFIG_WR.flatten_input_paths),
             ),
         )
     ):
         flatten_input_paths = FlattenPath.FILE_NAME_ONLY
 
-    # Special processing for Bash tasks if the 'executable' property is set
-    # The Bash script is uploaded if this hasn't already been done, and
+    # Special processing for Bash, Python & PowerShell tasks if the 'executable'
+    # property is set
+    # The script is uploaded if this hasn't already been done, and
     # added to the list of required files.
-    if task_type == "bash":
+    if task_type in ["bash", "powershell", "python"]:
         if executable is None:
-            print_log("Note: no 'executable' specified for 'bash' Task Type")
+            print_log(f"Note: no 'executable' specified for '{task_type}' Task Type")
             return _make_task(flatten_input_paths)
 
         UPLOADED_FILES.add_input_file(
             filename=executable,
             flatten_upload_paths=flatten_upload_paths,
         )
         task_input = TaskInput.from_task_namespace(
```

### Comparing `yellowdog-python-examples-5.0.7/yd_commands/submit_utils.py` & `yellowdog-python-examples-6.0.0/yd_commands/submit_utils.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.7/yd_commands/terminate.py` & `yellowdog-python-examples-6.0.0/yd_commands/terminate.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.7/yd_commands/type_check.py` & `yellowdog-python-examples-6.0.0/yd_commands/type_check.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.7/yd_commands/upload.py` & `yellowdog-python-examples-6.0.0/yd_commands/upload.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.7/yd_commands/upload_utils.py` & `yellowdog-python-examples-6.0.0/yd_commands/upload_utils.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.7/yd_commands/variables.py` & `yellowdog-python-examples-6.0.0/yd_commands/variables.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.7/yd_commands/version.py` & `yellowdog-python-examples-6.0.0/yd_commands/version.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.7/yd_commands/wrapper.py` & `yellowdog-python-examples-6.0.0/yd_commands/wrapper.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.7/yellowdog_python_examples.egg-info/PKG-INFO` & `yellowdog-python-examples-6.0.0/yellowdog_python_examples.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yellowdog-python-examples
-Version: 5.0.7
+Version: 6.0.0
 Summary: Example Python commands using the YellowDog Python SDK
 Home-page: https://github.com/yellowdog/python-examples
 Author: YellowDog Limited
 Author-email: YellowDog Limited <support@yellowdog.co>
 Project-URL: Homepage, https://github.com/yellowdog/python-examples
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `yellowdog-python-examples-5.0.7/yellowdog_python_examples.egg-info/SOURCES.txt` & `yellowdog-python-examples-6.0.0/yellowdog_python_examples.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.7/yellowdog_python_examples.egg-info/entry_points.txt` & `yellowdog-python-examples-6.0.0/yellowdog_python_examples.egg-info/entry_points.txt`

 * *Files identical despite different names*

