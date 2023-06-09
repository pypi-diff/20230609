# Comparing `tmp/cmind-1.4.0.tar.gz` & `tmp/cmind-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmind-1.4.0.tar", last modified: Tue Jun  6 10:27:33 2023, max compression
+gzip compressed data, was "cmind-1.4.1.tar", last modified: Fri Jun  9 07:26:32 2023, max compression
```

## Comparing `cmind-1.4.0.tar` & `cmind-1.4.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-06-06 10:27:33.939507 cmind-1.4.0/
--rw-r--r--   0 fursin    (1000) fursin    (1000)     6057 2023-06-06 10:27:33.939507 cmind-1.4.0/PKG-INFO
--rw-r--r--   0 fursin    (1000) fursin    (1000)     5127 2023-05-30 19:25:20.000000 cmind-1.4.0/README.md
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-06-06 10:27:33.919507 cmind-1.4.0/cmind/
--rw-r--r--   0 fursin    (1000) fursin    (1000)      136 2023-06-06 10:14:36.000000 cmind-1.4.0/cmind/__init__.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)       35 2023-05-25 12:13:31.000000 cmind-1.4.0/cmind/__main__.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     4908 2023-05-25 12:13:31.000000 cmind-1.4.0/cmind/artifact.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)    46874 2023-06-06 10:14:36.000000 cmind-1.4.0/cmind/automation.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     4754 2023-06-06 10:14:36.000000 cmind-1.4.0/cmind/cli.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     3285 2023-05-25 12:13:31.000000 cmind-1.4.0/cmind/config.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)    24589 2023-06-06 10:14:36.000000 cmind-1.4.0/cmind/core.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     9326 2023-05-26 16:24:59.000000 cmind-1.4.0/cmind/index.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     2046 2023-05-25 12:13:31.000000 cmind-1.4.0/cmind/net.py
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-06-06 10:27:33.919507 cmind-1.4.0/cmind/repo/
--rw-r--r--   0 fursin    (1000) fursin    (1000)      491 2023-05-25 12:13:31.000000 cmind-1.4.0/cmind/repo/README.md
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-06-06 10:27:33.899507 cmind-1.4.0/cmind/repo/automation/
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-06-06 10:27:33.929507 cmind-1.4.0/cmind/repo/automation/automation/
--rw-r--r--   0 fursin    (1000) fursin    (1000)     2647 2023-05-30 19:25:20.000000 cmind-1.4.0/cmind/repo/automation/automation/README.md
--rw-r--r--   0 fursin    (1000) fursin    (1000)      289 2023-05-25 12:13:31.000000 cmind-1.4.0/cmind/repo/automation/automation/_cm.json
--rw-r--r--   0 fursin    (1000) fursin    (1000)     3799 2023-05-25 12:13:31.000000 cmind-1.4.0/cmind/repo/automation/automation/module.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1518 2023-05-25 12:13:31.000000 cmind-1.4.0/cmind/repo/automation/automation/module_dummy.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     8772 2023-05-25 12:13:31.000000 cmind-1.4.0/cmind/repo/automation/automation/module_misc.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)      310 2023-05-25 12:13:31.000000 cmind-1.4.0/cmind/repo/automation/automation/template_list_of_automations.md
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-06-06 10:27:33.929507 cmind-1.4.0/cmind/repo/automation/ck/
--rw-r--r--   0 fursin    (1000) fursin    (1000)      984 2023-05-30 19:25:20.000000 cmind-1.4.0/cmind/repo/automation/ck/README.md
--rw-r--r--   0 fursin    (1000) fursin    (1000)      325 2023-05-25 12:13:31.000000 cmind-1.4.0/cmind/repo/automation/ck/_cm.json
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1015 2023-05-25 12:13:31.000000 cmind-1.4.0/cmind/repo/automation/ck/module.py
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-06-06 10:27:33.929507 cmind-1.4.0/cmind/repo/automation/core/
--rw-r--r--   0 fursin    (1000) fursin    (1000)      996 2023-05-30 19:25:20.000000 cmind-1.4.0/cmind/repo/automation/core/README.md
--rw-r--r--   0 fursin    (1000) fursin    (1000)      302 2023-05-25 12:13:31.000000 cmind-1.4.0/cmind/repo/automation/core/_cm.json
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-06-06 10:27:33.939507 cmind-1.4.0/cmind/repo/automation/core/cm_60cb625a46b38610/
--rw-r--r--   0 fursin    (1000) fursin    (1000)        0 2023-05-25 12:13:31.000000 cmind-1.4.0/cmind/repo/automation/core/cm_60cb625a46b38610/__init__.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)      220 2023-05-25 12:13:31.000000 cmind-1.4.0/cmind/repo/automation/core/cm_60cb625a46b38610/misc.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1008 2023-05-25 12:13:31.000000 cmind-1.4.0/cmind/repo/automation/core/module.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)      220 2023-05-25 12:13:31.000000 cmind-1.4.0/cmind/repo/automation/core/module_misc.py
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-06-06 10:27:33.939507 cmind-1.4.0/cmind/repo/automation/repo/
--rw-r--r--   0 fursin    (1000) fursin    (1000)     9508 2023-05-30 19:25:20.000000 cmind-1.4.0/cmind/repo/automation/repo/README.md
--rw-r--r--   0 fursin    (1000) fursin    (1000)      377 2023-05-25 12:13:31.000000 cmind-1.4.0/cmind/repo/automation/repo/_cm.json
--rw-r--r--   0 fursin    (1000) fursin    (1000)    31060 2023-05-30 19:25:20.000000 cmind-1.4.0/cmind/repo/automation/repo/module.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)       71 2023-05-25 12:13:31.000000 cmind-1.4.0/cmind/repo/cmr.yaml
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1978 2023-05-25 12:13:31.000000 cmind-1.4.0/cmind/repo.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)    18709 2023-05-25 12:13:31.000000 cmind-1.4.0/cmind/repos.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)    41400 2023-05-25 12:13:31.000000 cmind-1.4.0/cmind/utils.py
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-06-06 10:27:33.919507 cmind-1.4.0/cmind.egg-info/
--rw-r--r--   0 fursin    (1000) fursin    (1000)     6057 2023-06-06 10:27:33.000000 cmind-1.4.0/cmind.egg-info/PKG-INFO
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1222 2023-06-06 10:27:33.000000 cmind-1.4.0/cmind.egg-info/SOURCES.txt
--rw-r--r--   0 fursin    (1000) fursin    (1000)        1 2023-06-06 10:27:33.000000 cmind-1.4.0/cmind.egg-info/dependency_links.txt
--rw-r--r--   0 fursin    (1000) fursin    (1000)       87 2023-06-06 10:27:33.000000 cmind-1.4.0/cmind.egg-info/entry_points.txt
--rw-r--r--   0 fursin    (1000) fursin    (1000)        1 2023-06-06 10:27:33.000000 cmind-1.4.0/cmind.egg-info/not-zip-safe
--rw-r--r--   0 fursin    (1000) fursin    (1000)       16 2023-06-06 10:27:33.000000 cmind-1.4.0/cmind.egg-info/requires.txt
--rw-r--r--   0 fursin    (1000) fursin    (1000)        6 2023-06-06 10:27:33.000000 cmind-1.4.0/cmind.egg-info/top_level.txt
--rw-r--r--   0 fursin    (1000) fursin    (1000)       38 2023-06-06 10:27:33.939507 cmind-1.4.0/setup.cfg
--rw-r--r--   0 fursin    (1000) fursin    (1000)     2719 2023-06-06 10:25:45.000000 cmind-1.4.0/setup.py
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-06-09 07:26:32.891193 cmind-1.4.1/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     6090 2023-06-09 07:26:32.891193 cmind-1.4.1/PKG-INFO
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     5127 2023-05-30 19:25:20.000000 cmind-1.4.1/README.md
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-06-09 07:26:32.851194 cmind-1.4.1/cmind/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      136 2023-06-09 07:26:00.000000 cmind-1.4.1/cmind/__init__.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)       35 2023-05-25 12:13:31.000000 cmind-1.4.1/cmind/__main__.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     4908 2023-05-25 12:13:31.000000 cmind-1.4.1/cmind/artifact.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    46874 2023-06-06 10:14:36.000000 cmind-1.4.1/cmind/automation.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     5324 2023-06-09 07:26:00.000000 cmind-1.4.1/cmind/cli.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     3285 2023-05-25 12:13:31.000000 cmind-1.4.1/cmind/config.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    24589 2023-06-06 10:14:36.000000 cmind-1.4.1/cmind/core.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     9326 2023-05-26 16:24:59.000000 cmind-1.4.1/cmind/index.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     2046 2023-05-25 12:13:31.000000 cmind-1.4.1/cmind/net.py
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-06-09 07:26:32.861194 cmind-1.4.1/cmind/repo/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      491 2023-05-25 12:13:31.000000 cmind-1.4.1/cmind/repo/README.md
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-06-09 07:26:32.841194 cmind-1.4.1/cmind/repo/automation/
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-06-09 07:26:32.871194 cmind-1.4.1/cmind/repo/automation/automation/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     2647 2023-05-30 19:25:20.000000 cmind-1.4.1/cmind/repo/automation/automation/README.md
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      289 2023-05-25 12:13:31.000000 cmind-1.4.1/cmind/repo/automation/automation/_cm.json
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     3799 2023-05-25 12:13:31.000000 cmind-1.4.1/cmind/repo/automation/automation/module.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     1518 2023-05-25 12:13:31.000000 cmind-1.4.1/cmind/repo/automation/automation/module_dummy.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     8772 2023-05-25 12:13:31.000000 cmind-1.4.1/cmind/repo/automation/automation/module_misc.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      310 2023-05-25 12:13:31.000000 cmind-1.4.1/cmind/repo/automation/automation/template_list_of_automations.md
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-06-09 07:26:32.871194 cmind-1.4.1/cmind/repo/automation/ck/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      984 2023-05-30 19:25:20.000000 cmind-1.4.1/cmind/repo/automation/ck/README.md
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      325 2023-05-25 12:13:31.000000 cmind-1.4.1/cmind/repo/automation/ck/_cm.json
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     1015 2023-05-25 12:13:31.000000 cmind-1.4.1/cmind/repo/automation/ck/module.py
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-06-09 07:26:32.881193 cmind-1.4.1/cmind/repo/automation/core/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      996 2023-05-30 19:25:20.000000 cmind-1.4.1/cmind/repo/automation/core/README.md
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      302 2023-05-25 12:13:31.000000 cmind-1.4.1/cmind/repo/automation/core/_cm.json
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-06-09 07:26:32.881193 cmind-1.4.1/cmind/repo/automation/core/cm_60cb625a46b38610/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)        0 2023-05-25 12:13:31.000000 cmind-1.4.1/cmind/repo/automation/core/cm_60cb625a46b38610/__init__.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      220 2023-05-25 12:13:31.000000 cmind-1.4.1/cmind/repo/automation/core/cm_60cb625a46b38610/misc.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     1008 2023-05-25 12:13:31.000000 cmind-1.4.1/cmind/repo/automation/core/module.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      220 2023-05-25 12:13:31.000000 cmind-1.4.1/cmind/repo/automation/core/module_misc.py
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-06-09 07:26:32.891193 cmind-1.4.1/cmind/repo/automation/repo/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     9508 2023-05-30 19:25:20.000000 cmind-1.4.1/cmind/repo/automation/repo/README.md
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      377 2023-05-25 12:13:31.000000 cmind-1.4.1/cmind/repo/automation/repo/_cm.json
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    31060 2023-05-30 19:25:20.000000 cmind-1.4.1/cmind/repo/automation/repo/module.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)       71 2023-05-25 12:13:31.000000 cmind-1.4.1/cmind/repo/cmr.yaml
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     1978 2023-05-25 12:13:31.000000 cmind-1.4.1/cmind/repo.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    18709 2023-05-25 12:13:31.000000 cmind-1.4.1/cmind/repos.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    41400 2023-05-25 12:13:31.000000 cmind-1.4.1/cmind/utils.py
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-06-09 07:26:32.861194 cmind-1.4.1/cmind.egg-info/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     6090 2023-06-09 07:26:32.000000 cmind-1.4.1/cmind.egg-info/PKG-INFO
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     1222 2023-06-09 07:26:32.000000 cmind-1.4.1/cmind.egg-info/SOURCES.txt
+-rw-r--r--   0 fursin    (1000) fursin    (1000)        1 2023-06-09 07:26:32.000000 cmind-1.4.1/cmind.egg-info/dependency_links.txt
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      118 2023-06-09 07:26:32.000000 cmind-1.4.1/cmind.egg-info/entry_points.txt
+-rw-r--r--   0 fursin    (1000) fursin    (1000)        1 2023-06-06 10:27:33.000000 cmind-1.4.1/cmind.egg-info/not-zip-safe
+-rw-r--r--   0 fursin    (1000) fursin    (1000)       16 2023-06-09 07:26:32.000000 cmind-1.4.1/cmind.egg-info/requires.txt
+-rw-r--r--   0 fursin    (1000) fursin    (1000)        6 2023-06-09 07:26:32.000000 cmind-1.4.1/cmind.egg-info/top_level.txt
+-rw-r--r--   0 fursin    (1000) fursin    (1000)       38 2023-06-09 07:26:32.891193 cmind-1.4.1/setup.cfg
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     2808 2023-06-09 07:26:00.000000 cmind-1.4.1/setup.py
```

### Comparing `cmind-1.4.0/PKG-INFO` & `cmind-1.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: cmind
-Version: 1.4.0
+Version: 1.4.1
 Summary: cmind
 Home-page: https://github.com/mlcommons/ck/tree/master/cm
 Author: Grigori Fursin
-Author-email: grigori@octoml.ai
+Author-email: Grigori.Fursin@cTuning.org
 License: Apache 2.0
 Description: [![PyPI version](https://badge.fury.io/py/cmind.svg)](https://pepy.tech/project/cmind)
         [![Python Version](https://img.shields.io/badge/python-3+-blue.svg)](https://github.com/mlcommons/ck/tree/master/cm/cmind)
         [![Downloads](https://pepy.tech/badge/cmind/month)](https://pepy.tech/project/cmind)
         [![License](https://img.shields.io/badge/License-Apache%202.0-green)](LICENSE.md)
         
         [![CM test](https://github.com/mlcommons/ck/actions/workflows/test-cm.yml/badge.svg)](https://github.com/mlcommons/ck/actions/workflows/test-cm.yml)
@@ -74,10 +74,10 @@
         
         ### Acknowledgments
         
         This project is currently supported by [MLCommons](https://mlcommons.org), [cTuning foundation](https://cTuning.org),
         [cKnowledge](https://cKnowledge.org) and [individual contributors](https://github.com/mlcommons/ck/blob/master/CONTRIBUTING.md).
         We thank [HiPEAC](https://hipeac.net) and [OctoML](https://octoml.ai) for sponsoring initial development.
         
-Keywords: collective mind,cmind,cdatabase,cmeta,automation,reusability,meta,JSON,YAML,python
+Keywords: collective mind,cmind,ck2,cdatabase,cmeta,automation,portability,reusability,meta,JSON,YAML,python,api,cli
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `cmind-1.4.0/README.md` & `cmind-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `cmind-1.4.0/cmind/artifact.py` & `cmind-1.4.1/cmind/artifact.py`

 * *Files identical despite different names*

### Comparing `cmind-1.4.0/cmind/automation.py` & `cmind-1.4.1/cmind/automation.py`

 * *Files identical despite different names*

### Comparing `cmind-1.4.0/cmind/cli.py` & `cmind-1.4.1/cmind/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         cm.error(r)
 
     sys.exit(r['return'])
 
 ############################################################
 def run_script(argv = None):
     """
-    Shortcut to run cm script
+    Shortcut to "cm run script ..."
 
     CM command line format:
 
     Args:
         argv (list | string): command line arguments
 
     Returns: 
@@ -72,14 +72,40 @@
     # Access CM
     if argv is None:
         argv = sys.argv[1:]
 
     return run(['run', 'script'] + argv)
 
 ############################################################
+def run_experiment(argv = None):
+    """
+    Shortcut to "cm run experiment ..."
+
+    CM command line format:
+
+    Args:
+        argv (list | string): command line arguments
+
+    Returns: 
+        (CM return dict):
+
+        * return (int): return code == 0 if no error and >0 if error
+        * (error) (str): error string if return>0
+
+        * Output from a CM automation action
+
+    """
+
+    # Access CM
+    if argv is None:
+        argv = sys.argv[1:]
+
+    return run(['run', 'experiment'] + argv)
+
+############################################################
 def parse(cmd):
     """
     Parse CM command line into CM input dictionary.
 
     Args:
         cmd (str | list) : arguments as a string or list
```

### Comparing `cmind-1.4.0/cmind/config.py` & `cmind-1.4.1/cmind/config.py`

 * *Files identical despite different names*

### Comparing `cmind-1.4.0/cmind/core.py` & `cmind-1.4.1/cmind/core.py`

 * *Files identical despite different names*

### Comparing `cmind-1.4.0/cmind/index.py` & `cmind-1.4.1/cmind/index.py`

 * *Files identical despite different names*

### Comparing `cmind-1.4.0/cmind/net.py` & `cmind-1.4.1/cmind/net.py`

 * *Files identical despite different names*

### Comparing `cmind-1.4.0/cmind/repo/automation/automation/README.md` & `cmind-1.4.1/cmind/repo/automation/automation/README.md`

 * *Files identical despite different names*

### Comparing `cmind-1.4.0/cmind/repo/automation/automation/module.py` & `cmind-1.4.1/cmind/repo/automation/automation/module.py`

 * *Files identical despite different names*

### Comparing `cmind-1.4.0/cmind/repo/automation/automation/module_dummy.py` & `cmind-1.4.1/cmind/repo/automation/automation/module_dummy.py`

 * *Files identical despite different names*

### Comparing `cmind-1.4.0/cmind/repo/automation/automation/module_misc.py` & `cmind-1.4.1/cmind/repo/automation/automation/module_misc.py`

 * *Files identical despite different names*

### Comparing `cmind-1.4.0/cmind/repo/automation/ck/README.md` & `cmind-1.4.1/cmind/repo/automation/ck/README.md`

 * *Files identical despite different names*

### Comparing `cmind-1.4.0/cmind/repo/automation/ck/module.py` & `cmind-1.4.1/cmind/repo/automation/ck/module.py`

 * *Files identical despite different names*

### Comparing `cmind-1.4.0/cmind/repo/automation/core/README.md` & `cmind-1.4.1/cmind/repo/automation/core/README.md`

 * *Files identical despite different names*

### Comparing `cmind-1.4.0/cmind/repo/automation/core/module.py` & `cmind-1.4.1/cmind/repo/automation/core/module.py`

 * *Files identical despite different names*

### Comparing `cmind-1.4.0/cmind/repo/automation/repo/README.md` & `cmind-1.4.1/cmind/repo/automation/repo/README.md`

 * *Files identical despite different names*

### Comparing `cmind-1.4.0/cmind/repo/automation/repo/module.py` & `cmind-1.4.1/cmind/repo/automation/repo/module.py`

 * *Files identical despite different names*

### Comparing `cmind-1.4.0/cmind/repo.py` & `cmind-1.4.1/cmind/repo.py`

 * *Files identical despite different names*

### Comparing `cmind-1.4.0/cmind/repos.py` & `cmind-1.4.1/cmind/repos.py`

 * *Files identical despite different names*

### Comparing `cmind-1.4.0/cmind/utils.py` & `cmind-1.4.1/cmind/utils.py`

 * *Files identical despite different names*

### Comparing `cmind-1.4.0/cmind.egg-info/PKG-INFO` & `cmind-1.4.1/cmind.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: cmind
-Version: 1.4.0
+Version: 1.4.1
 Summary: cmind
 Home-page: https://github.com/mlcommons/ck/tree/master/cm
 Author: Grigori Fursin
-Author-email: grigori@octoml.ai
+Author-email: Grigori.Fursin@cTuning.org
 License: Apache 2.0
 Description: [![PyPI version](https://badge.fury.io/py/cmind.svg)](https://pepy.tech/project/cmind)
         [![Python Version](https://img.shields.io/badge/python-3+-blue.svg)](https://github.com/mlcommons/ck/tree/master/cm/cmind)
         [![Downloads](https://pepy.tech/badge/cmind/month)](https://pepy.tech/project/cmind)
         [![License](https://img.shields.io/badge/License-Apache%202.0-green)](LICENSE.md)
         
         [![CM test](https://github.com/mlcommons/ck/actions/workflows/test-cm.yml/badge.svg)](https://github.com/mlcommons/ck/actions/workflows/test-cm.yml)
@@ -74,10 +74,10 @@
         
         ### Acknowledgments
         
         This project is currently supported by [MLCommons](https://mlcommons.org), [cTuning foundation](https://cTuning.org),
         [cKnowledge](https://cKnowledge.org) and [individual contributors](https://github.com/mlcommons/ck/blob/master/CONTRIBUTING.md).
         We thank [HiPEAC](https://hipeac.net) and [OctoML](https://octoml.ai) for sponsoring initial development.
         
-Keywords: collective mind,cmind,cdatabase,cmeta,automation,reusability,meta,JSON,YAML,python
+Keywords: collective mind,cmind,ck2,cdatabase,cmeta,automation,portability,reusability,meta,JSON,YAML,python,api,cli
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `cmind-1.4.0/cmind.egg-info/SOURCES.txt` & `cmind-1.4.1/cmind.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cmind-1.4.0/setup.py` & `cmind-1.4.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     if not ignore:
         repo_dirs.append(directory[len(root)+1:])
 
 setup(
     name="cmind",
 
     author="Grigori Fursin",
-    author_email="grigori@octoml.ai",
+    author_email="Grigori.Fursin@cTuning.org",
 
     version=version,
 
     description="cmind",
 
     license="Apache 2.0",
 
@@ -95,14 +95,15 @@
     },
 
     install_requires=['pyyaml', 'requests'],
 
     entry_points={"console_scripts": [
                       "cmind = cmind.cli:run",
                       "cm = cmind.cli:run",
-                      "cmr = cmind.cli:run_script"
+                      "cmr = cmind.cli:run_script",
+                      "cme = cmind.cli:run_experiment"
                  ]},
 
     zip_safe=False,
 
-    keywords="collective mind,cmind,cdatabase,cmeta,automation,reusability,meta,JSON,YAML,python"
+    keywords="collective mind,cmind,ck2,cdatabase,cmeta,automation,portability,reusability,meta,JSON,YAML,python,api,cli"
 )
```

