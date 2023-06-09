# Comparing `tmp/tycho-api-1.9a1.dev2.tar.gz` & `tmp/tycho-api-1.9a1.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tycho-api-1.9a1.dev2.tar", last modified: Wed Dec 14 20:11:33 2022, max compression
+gzip compressed data, was "tycho-api-1.9a1.dev3.tar", last modified: Fri Dec 16 17:49:47 2022, max compression
```

## Comparing `tycho-api-1.9a1.dev2.tar` & `tycho-api-1.9a1.dev3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 charlesbennett   (503) staff       (20)        0 2022-12-14 20:11:33.895745 tycho-api-1.9a1.dev2/
--rw-r--r--   0 charlesbennett   (503) staff       (20)     1096 2022-11-29 21:46:28.000000 tycho-api-1.9a1.dev2/LICENSE.txt
--rw-r--r--   0 charlesbennett   (503) staff       (20)    10435 2022-12-14 20:11:33.895439 tycho-api-1.9a1.dev2/PKG-INFO
--rw-r--r--   0 charlesbennett   (503) staff       (20)        0 2022-11-29 21:46:28.000000 tycho-api-1.9a1.dev2/README.rst
--rw-r--r--   0 charlesbennett   (503) staff       (20)       38 2022-12-14 20:11:33.895821 tycho-api-1.9a1.dev2/setup.cfg
--rw-r--r--   0 charlesbennett   (503) staff       (20)     2456 2022-11-29 21:46:28.000000 tycho-api-1.9a1.dev2/setup.py
-drwxr-xr-x   0 charlesbennett   (503) staff       (20)        0 2022-12-14 20:11:33.886190 tycho-api-1.9a1.dev2/tycho/
--rw-r--r--   0 charlesbennett   (503) staff       (20)       27 2022-12-14 20:10:28.000000 tycho-api-1.9a1.dev2/tycho/__init__.py
--rw-r--r--   0 charlesbennett   (503) staff       (20)     5348 2022-11-29 21:46:28.000000 tycho-api-1.9a1.dev2/tycho/actions.py
--rw-r--r--   0 charlesbennett   (503) staff       (20)     3994 2022-11-29 21:46:28.000000 tycho-api-1.9a1.dev2/tycho/api-schema.yaml
--rw-r--r--   0 charlesbennett   (503) staff       (20)     9717 2022-11-29 21:46:28.000000 tycho-api-1.9a1.dev2/tycho/api.py
--rw-r--r--   0 charlesbennett   (503) staff       (20)    23403 2022-11-29 21:46:28.000000 tycho-api-1.9a1.dev2/tycho/client.py
--rw-r--r--   0 charlesbennett   (503) staff       (20)     3890 2022-11-29 21:46:28.000000 tycho-api-1.9a1.dev2/tycho/compute.py
-drwxr-xr-x   0 charlesbennett   (503) staff       (20)        0 2022-12-14 20:11:33.888109 tycho-api-1.9a1.dev2/tycho/conf/
--rw-r--r--   0 charlesbennett   (503) staff       (20)      654 2022-11-29 21:46:28.000000 tycho-api-1.9a1.dev2/tycho/conf/app-defaults.yaml
--rw-r--r--   0 charlesbennett   (503) staff       (20)    16879 2022-12-14 20:09:11.000000 tycho-api-1.9a1.dev2/tycho/conf/app-registry.yaml
--rw-r--r--   0 charlesbennett   (503) staff       (20)     1080 2022-11-29 21:46:28.000000 tycho-api-1.9a1.dev2/tycho/conf/tycho.yaml
--rw-r--r--   0 charlesbennett   (503) staff       (20)     1672 2022-11-29 21:46:28.000000 tycho-api-1.9a1.dev2/tycho/config.py
--rw-r--r--   0 charlesbennett   (503) staff       (20)    16977 2022-11-29 21:46:28.000000 tycho-api-1.9a1.dev2/tycho/context.py
--rw-r--r--   0 charlesbennett   (503) staff       (20)     3755 2022-11-29 21:46:28.000000 tycho-api-1.9a1.dev2/tycho/core.py
--rw-r--r--   0 charlesbennett   (503) staff       (20)     5996 2022-11-29 21:46:28.000000 tycho-api-1.9a1.dev2/tycho/dockerc.py
--rw-r--r--   0 charlesbennett   (503) staff       (20)      643 2022-11-29 21:46:28.000000 tycho-api-1.9a1.dev2/tycho/exceptions.py
--rw-r--r--   0 charlesbennett   (503) staff       (20)      750 2022-11-29 21:46:28.000000 tycho-api-1.9a1.dev2/tycho/factory.py
--rw-r--r--   0 charlesbennett   (503) staff       (20)    23518 2022-11-29 21:46:28.000000 tycho-api-1.9a1.dev2/tycho/kube.py
--rw-r--r--   0 charlesbennett   (503) staff       (20)    21294 2022-12-14 20:09:11.000000 tycho-api-1.9a1.dev2/tycho/model.py
-drwxr-xr-x   0 charlesbennett   (503) staff       (20)        0 2022-12-14 20:11:33.893049 tycho-api-1.9a1.dev2/tycho/template/
--rw-r--r--   0 charlesbennett   (503) staff       (20)      243 2022-11-29 21:46:28.000000 tycho-api-1.9a1.dev2/tycho/template/clusterrole.yaml
--rw-r--r--   0 charlesbennett   (503) staff       (20)      345 2022-11-29 21:46:28.000000 tycho-api-1.9a1.dev2/tycho/template/clusterrolebinding.yaml
--rw-r--r--   0 charlesbennett   (503) staff       (20)      311 2022-11-29 21:46:28.000000 tycho-api-1.9a1.dev2/tycho/template/mapping.yaml
--rw-r--r--   0 charlesbennett   (503) staff       (20)      794 2022-11-29 21:46:28.000000 tycho-api-1.9a1.dev2/tycho/template/patch.yaml
--rw-r--r--   0 charlesbennett   (503) staff       (20)     9041 2022-12-14 20:09:11.000000 tycho-api-1.9a1.dev2/tycho/template/pod.yaml
--rw-r--r--   0 charlesbennett   (503) staff       (20)      593 2022-11-29 21:46:28.000000 tycho-api-1.9a1.dev2/tycho/template/pv.yaml
--rw-r--r--   0 charlesbennett   (503) staff       (20)      491 2022-11-29 21:46:28.000000 tycho-api-1.9a1.dev2/tycho/template/pvc.yaml
--rw-r--r--   0 charlesbennett   (503) staff       (20)     1925 2022-11-29 21:46:28.000000 tycho-api-1.9a1.dev2/tycho/template/service.yaml
--rw-r--r--   0 charlesbennett   (503) staff       (20)     5273 2022-11-29 21:46:28.000000 tycho-api-1.9a1.dev2/tycho/tycho_utils.py
-drwxr-xr-x   0 charlesbennett   (503) staff       (20)        0 2022-12-14 20:11:33.895021 tycho-api-1.9a1.dev2/tycho_api.egg-info/
--rw-r--r--   0 charlesbennett   (503) staff       (20)    10435 2022-12-14 20:11:33.000000 tycho-api-1.9a1.dev2/tycho_api.egg-info/PKG-INFO
--rw-r--r--   0 charlesbennett   (503) staff       (20)      789 2022-12-14 20:11:33.000000 tycho-api-1.9a1.dev2/tycho_api.egg-info/SOURCES.txt
--rw-r--r--   0 charlesbennett   (503) staff       (20)        1 2022-12-14 20:11:33.000000 tycho-api-1.9a1.dev2/tycho_api.egg-info/dependency_links.txt
--rw-r--r--   0 charlesbennett   (503) staff       (20)       41 2022-12-14 20:11:33.000000 tycho-api-1.9a1.dev2/tycho_api.egg-info/entry_points.txt
--rw-r--r--   0 charlesbennett   (503) staff       (20)     1105 2022-12-14 20:11:33.000000 tycho-api-1.9a1.dev2/tycho_api.egg-info/requires.txt
--rw-r--r--   0 charlesbennett   (503) staff       (20)        6 2022-12-14 20:11:33.000000 tycho-api-1.9a1.dev2/tycho_api.egg-info/top_level.txt
+drwxr-xr-x   0 charlesbennett   (503) staff       (20)        0 2022-12-16 17:49:47.489714 tycho-api-1.9a1.dev3/
+-rw-r--r--   0 charlesbennett   (503) staff       (20)     1096 2022-11-29 21:46:28.000000 tycho-api-1.9a1.dev3/LICENSE.txt
+-rw-r--r--   0 charlesbennett   (503) staff       (20)    10435 2022-12-16 17:49:47.489350 tycho-api-1.9a1.dev3/PKG-INFO
+-rw-r--r--   0 charlesbennett   (503) staff       (20)        0 2022-11-29 21:46:28.000000 tycho-api-1.9a1.dev3/README.rst
+-rw-r--r--   0 charlesbennett   (503) staff       (20)       38 2022-12-16 17:49:47.489796 tycho-api-1.9a1.dev3/setup.cfg
+-rw-r--r--   0 charlesbennett   (503) staff       (20)     2456 2022-11-29 21:46:28.000000 tycho-api-1.9a1.dev3/setup.py
+drwxr-xr-x   0 charlesbennett   (503) staff       (20)        0 2022-12-16 17:49:47.479321 tycho-api-1.9a1.dev3/tycho/
+-rw-r--r--   0 charlesbennett   (503) staff       (20)       27 2022-12-16 17:44:25.000000 tycho-api-1.9a1.dev3/tycho/__init__.py
+-rw-r--r--   0 charlesbennett   (503) staff       (20)     5348 2022-11-29 21:46:28.000000 tycho-api-1.9a1.dev3/tycho/actions.py
+-rw-r--r--   0 charlesbennett   (503) staff       (20)     3994 2022-11-29 21:46:28.000000 tycho-api-1.9a1.dev3/tycho/api-schema.yaml
+-rw-r--r--   0 charlesbennett   (503) staff       (20)     9717 2022-11-29 21:46:28.000000 tycho-api-1.9a1.dev3/tycho/api.py
+-rw-r--r--   0 charlesbennett   (503) staff       (20)    23403 2022-11-29 21:46:28.000000 tycho-api-1.9a1.dev3/tycho/client.py
+-rw-r--r--   0 charlesbennett   (503) staff       (20)     3890 2022-11-29 21:46:28.000000 tycho-api-1.9a1.dev3/tycho/compute.py
+drwxr-xr-x   0 charlesbennett   (503) staff       (20)        0 2022-12-16 17:49:47.481593 tycho-api-1.9a1.dev3/tycho/conf/
+-rw-r--r--   0 charlesbennett   (503) staff       (20)      654 2022-11-29 21:46:28.000000 tycho-api-1.9a1.dev3/tycho/conf/app-defaults.yaml
+-rw-r--r--   0 charlesbennett   (503) staff       (20)    17501 2022-12-16 17:33:47.000000 tycho-api-1.9a1.dev3/tycho/conf/app-registry.yaml
+-rw-r--r--   0 charlesbennett   (503) staff       (20)     1080 2022-11-29 21:46:28.000000 tycho-api-1.9a1.dev3/tycho/conf/tycho.yaml
+-rw-r--r--   0 charlesbennett   (503) staff       (20)     1672 2022-11-29 21:46:28.000000 tycho-api-1.9a1.dev3/tycho/config.py
+-rw-r--r--   0 charlesbennett   (503) staff       (20)    16977 2022-11-29 21:46:28.000000 tycho-api-1.9a1.dev3/tycho/context.py
+-rw-r--r--   0 charlesbennett   (503) staff       (20)     3755 2022-11-29 21:46:28.000000 tycho-api-1.9a1.dev3/tycho/core.py
+-rw-r--r--   0 charlesbennett   (503) staff       (20)     5996 2022-11-29 21:46:28.000000 tycho-api-1.9a1.dev3/tycho/dockerc.py
+-rw-r--r--   0 charlesbennett   (503) staff       (20)      643 2022-11-29 21:46:28.000000 tycho-api-1.9a1.dev3/tycho/exceptions.py
+-rw-r--r--   0 charlesbennett   (503) staff       (20)      750 2022-11-29 21:46:28.000000 tycho-api-1.9a1.dev3/tycho/factory.py
+-rw-r--r--   0 charlesbennett   (503) staff       (20)    23518 2022-11-29 21:46:28.000000 tycho-api-1.9a1.dev3/tycho/kube.py
+-rw-r--r--   0 charlesbennett   (503) staff       (20)    22248 2022-12-16 17:33:47.000000 tycho-api-1.9a1.dev3/tycho/model.py
+drwxr-xr-x   0 charlesbennett   (503) staff       (20)        0 2022-12-16 17:49:47.486639 tycho-api-1.9a1.dev3/tycho/template/
+-rw-r--r--   0 charlesbennett   (503) staff       (20)      243 2022-11-29 21:46:28.000000 tycho-api-1.9a1.dev3/tycho/template/clusterrole.yaml
+-rw-r--r--   0 charlesbennett   (503) staff       (20)      345 2022-11-29 21:46:28.000000 tycho-api-1.9a1.dev3/tycho/template/clusterrolebinding.yaml
+-rw-r--r--   0 charlesbennett   (503) staff       (20)      311 2022-11-29 21:46:28.000000 tycho-api-1.9a1.dev3/tycho/template/mapping.yaml
+-rw-r--r--   0 charlesbennett   (503) staff       (20)      794 2022-11-29 21:46:28.000000 tycho-api-1.9a1.dev3/tycho/template/patch.yaml
+-rw-r--r--   0 charlesbennett   (503) staff       (20)     9314 2022-12-16 17:33:47.000000 tycho-api-1.9a1.dev3/tycho/template/pod.yaml
+-rw-r--r--   0 charlesbennett   (503) staff       (20)      593 2022-11-29 21:46:28.000000 tycho-api-1.9a1.dev3/tycho/template/pv.yaml
+-rw-r--r--   0 charlesbennett   (503) staff       (20)      491 2022-11-29 21:46:28.000000 tycho-api-1.9a1.dev3/tycho/template/pvc.yaml
+-rw-r--r--   0 charlesbennett   (503) staff       (20)     1925 2022-11-29 21:46:28.000000 tycho-api-1.9a1.dev3/tycho/template/service.yaml
+-rw-r--r--   0 charlesbennett   (503) staff       (20)     5273 2022-11-29 21:46:28.000000 tycho-api-1.9a1.dev3/tycho/tycho_utils.py
+drwxr-xr-x   0 charlesbennett   (503) staff       (20)        0 2022-12-16 17:49:47.488638 tycho-api-1.9a1.dev3/tycho_api.egg-info/
+-rw-r--r--   0 charlesbennett   (503) staff       (20)    10435 2022-12-16 17:49:47.000000 tycho-api-1.9a1.dev3/tycho_api.egg-info/PKG-INFO
+-rw-r--r--   0 charlesbennett   (503) staff       (20)      789 2022-12-16 17:49:47.000000 tycho-api-1.9a1.dev3/tycho_api.egg-info/SOURCES.txt
+-rw-r--r--   0 charlesbennett   (503) staff       (20)        1 2022-12-16 17:49:47.000000 tycho-api-1.9a1.dev3/tycho_api.egg-info/dependency_links.txt
+-rw-r--r--   0 charlesbennett   (503) staff       (20)       41 2022-12-16 17:49:47.000000 tycho-api-1.9a1.dev3/tycho_api.egg-info/entry_points.txt
+-rw-r--r--   0 charlesbennett   (503) staff       (20)     1105 2022-12-16 17:49:47.000000 tycho-api-1.9a1.dev3/tycho_api.egg-info/requires.txt
+-rw-r--r--   0 charlesbennett   (503) staff       (20)        6 2022-12-16 17:49:47.000000 tycho-api-1.9a1.dev3/tycho_api.egg-info/top_level.txt
```

### Comparing `tycho-api-1.9a1.dev2/LICENSE.txt` & `tycho-api-1.9a1.dev3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tycho-api-1.9a1.dev2/PKG-INFO` & `tycho-api-1.9a1.dev3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tycho-api
-Version: 1.9a1.dev2
+Version: 1.9a1.dev3
 Summary: Tycho is an API, compiler, and executor for cloud native distributed systems.
 Home-page: https://github.com/helxplatform/tycho.git
 Maintainer: Renci
 Maintainer-email: muralikarthik.k@renci.org
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tycho-api-1.9a1.dev2/setup.py` & `tycho-api-1.9a1.dev3/setup.py`

 * *Files identical despite different names*

### Comparing `tycho-api-1.9a1.dev2/tycho/actions.py` & `tycho-api-1.9a1.dev3/tycho/actions.py`

 * *Files identical despite different names*

### Comparing `tycho-api-1.9a1.dev2/tycho/api-schema.yaml` & `tycho-api-1.9a1.dev3/tycho/api-schema.yaml`

 * *Files identical despite different names*

### Comparing `tycho-api-1.9a1.dev2/tycho/api.py` & `tycho-api-1.9a1.dev3/tycho/api.py`

 * *Files identical despite different names*

### Comparing `tycho-api-1.9a1.dev2/tycho/client.py` & `tycho-api-1.9a1.dev3/tycho/client.py`

 * *Files identical despite different names*

### Comparing `tycho-api-1.9a1.dev2/tycho/compute.py` & `tycho-api-1.9a1.dev3/tycho/compute.py`

 * *Files identical despite different names*

### Comparing `tycho-api-1.9a1.dev2/tycho/conf/app-defaults.yaml` & `tycho-api-1.9a1.dev3/tycho/conf/app-defaults.yaml`

 * *Files identical despite different names*

### Comparing `tycho-api-1.9a1.dev2/tycho/conf/app-registry.yaml` & `tycho-api-1.9a1.dev3/tycho/conf/app-registry.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -146,14 +146,19 @@
     name: BRAIN-I App Registry
     jupyter-ds:
       securityContext:
         fsGroup: 0
     blackbalsam:
       securityContext:
         fsGroup: 0
+    cloud-top:
+      securityContext:
+        runAsUser: 0
+        runAsGroup: 0
+        fsGroup: 0
     apps:
       imagej:
         name: ImageJ Viewer
         description: Imagej is an image processor developed at NIH/LOCI.
         details: Can display, edit, analyze, process, save and print 8-bit, 16-bit and 32-bit images. It can read many image formats.
         docs: https://imagej.nih.gov/ij/
         services:
@@ -170,29 +175,34 @@
         count: 1
       cloud-top:
         name: Cloud Top
         description: CloudTop is a cloud native, browser accessible Linux desktop.
         details: A Ubuntu graphical desktop environment for experimenting with native applications in the cloud.
         docs: https://helxplatform.github.io/cloudtop-docs/
         services:
-          cloud-top : 8080
+          cloud-top : 3000
         count: 1
       scout:
         name: SCOUT
         description: SCOUT is an open-source Python package for performing volumetric image analysis of intact cerebral organoids.
         details: A Ubuntu graphical desktop environment for experimenting with SCOUT application in the cloud.
         docs: https://chunglabmit.github.io/scout/#
         services:
           scout : 8080
         count: 1
   bdc:
     extends:
       - common
       - blackbalsam
     name: BioData Catalyst App Registry
+    cloud-top:
+      securityContext:
+        runAsUser: 0
+        runAsGroup: 0
+        fsGroup: 0
     apps:
       hail:
         name: Hail / Jupyter Workspace
         description: A notebook computing interface to a large single node Hail genomics workspace.
         details: Instantiates Apache Spark on a single cloud node for small to medium scale exploration.
         docs: https://github.com/helxplatform/helx-hail # TODO: Make proper docs.
         services:
@@ -201,21 +211,26 @@
         proxy-rewrite-rule: True
       cloud-top:
         name: Cloud Top
         description: CloudTop is a cloud native, browser accessible Linux desktop.
         details: A Ubuntu graphical desktop environment for experimenting with native applications in the cloud.
         docs: https://helxplatform.github.io/cloudtop-docs/
         services:
-          cloud-top : 8080
+          cloud-top : 3000
         count: 1
   scidas:
     extends:
       - common
       - blackbalsam
     name: SciDAS App Registry
+    cloud-top:
+      securityContext:
+        runAsUser: 0
+        runAsGroup: 0
+        fsGroup: 0
     apps:
       nextflow:
         name: Nextflow API
         description: Nextflow - A scalable workflow computational pipeline workspace.
         details: Orchestrate Docker containers into reproducible workflows.
         docs: https://github.com/SciDAS/nextflow-api
         services:
@@ -235,15 +250,15 @@
         count: -1
       cloud-top:
         name: Cloud Top
         description: CloudTop is a cloud native, browser accessible Linux desktop.
         details: A Ubuntu graphical desktop environment for experimenting with native applications in the cloud.
         docs: https://helxplatform.github.io/cloudtop-docs/
         services:
-          cloud-top : 8080
+          cloud-top : 3000
         count: 1
   blackbalsam:
     extends:
       - common
     name: RENCI Blackbalsam Registry
     apps:
       blackbalsam:
@@ -287,14 +302,19 @@
     extends:
       - common
     name: NIH HEAL Initiative
   argus:
     extends:
       - common
     name: Argus Array
+    cloud-top:
+      securityContext:
+        runAsUser: 0
+        runAsGroup: 0
+        fsGroup: 0
     apps:
       kstars:
         name: KStars And DS9
         description: Sample FITS image file handling software.
         details: FITS image file handling software and sample FITS files for demo.
         docs: https://www.loc.gov/preservation/digital/formats/fdd/fdd000317.shtml
         services:
@@ -302,20 +322,25 @@
         count: 1
       cloud-top:
         name: Cloud Top
         description: CloudTop is a cloud native, browser accessible Linux desktop.
         details: A Ubuntu graphical desktop environment for experimenting with native applications in the cloud.
         docs: https://helxplatform.github.io/cloudtop-docs/
         services:
-          cloud-top: 8080
+          cloud-top: 3000
         count: 1
   eduhelx:
     name: UNC Helx for Education
     mixin:
       - sys
+    cloud-top:
+      securityContext:
+        fsGroup: 0
+        runAsUser: 0
+        runAsGroup: 0
     apps:
       jupyter-education:
         name: Jupyter Data Science for Education
         description: Jupyter DataScience - A Jupyter notebook for exploring and visualizing data.
         details: Includes R, Julia, and Python.
         docs: https://jupyter-docker-stacks.readthedocs.io/en/latest/using/selecting.html#jupyter-datascience-notebook
         services:
@@ -335,15 +360,15 @@
         count: 1
       cloud-top:
         name: Cloud Top
         description: CloudTop is a cloud native, browser accessible Linux desktop.
         details: A Ubuntu graphical desktop environment for experimenting with native applications in the cloud.
         docs: https://helxplatform.github.io/cloudtop-docs/
         services:
-          cloud-top: 8080
+          cloud-top: 3000
         count: 1
   tracs:
     name: TraCS
     mixin:
       - sys
     apps:
       atlas:
@@ -363,23 +388,29 @@
         services:
           rstudio-server: 8080
         count: 1
   eduhelx-sandbox:
     name: UNC Helx for Education Sandbox
     mixin:
       - sys
+    rstudio-server:
+      securityContext:
+        fsGroup: 0
+        runAsUser: 0
+        runAsGroup: 0
     apps:
       jupyter-education:
         name: Jupyter Data Science for Education
         description: Jupyter DataScience - A Jupyter notebook for exploring and visualizing data.
         details: Includes R, Julia, and Python.
         docs: https://jupyter-docker-stacks.readthedocs.io/en/latest/using/selecting.html#jupyter-datascience-notebook
         services:
           jupyter-education: "8888"
         proxy-rewrite-rule: True
+        count: 1
       rstudio-server:
         name: RStudio Server
         description: An integrated development environment for R.
         details: Has a console, syntax-highlighting editor that supports direct code execution, and tools for plotting, history, debugging and workspace management.
         docs: https://www.rstudio.com/
         proxy-rewrite-rule: True
         services:
```

### Comparing `tycho-api-1.9a1.dev2/tycho/conf/tycho.yaml` & `tycho-api-1.9a1.dev3/tycho/conf/tycho.yaml`

 * *Files identical despite different names*

### Comparing `tycho-api-1.9a1.dev2/tycho/config.py` & `tycho-api-1.9a1.dev3/tycho/config.py`

 * *Files identical despite different names*

### Comparing `tycho-api-1.9a1.dev2/tycho/context.py` & `tycho-api-1.9a1.dev3/tycho/context.py`

 * *Files identical despite different names*

### Comparing `tycho-api-1.9a1.dev2/tycho/core.py` & `tycho-api-1.9a1.dev3/tycho/core.py`

 * *Files identical despite different names*

### Comparing `tycho-api-1.9a1.dev2/tycho/dockerc.py` & `tycho-api-1.9a1.dev3/tycho/dockerc.py`

 * *Files identical despite different names*

### Comparing `tycho-api-1.9a1.dev2/tycho/exceptions.py` & `tycho-api-1.9a1.dev3/tycho/exceptions.py`

 * *Files identical despite different names*

### Comparing `tycho-api-1.9a1.dev2/tycho/factory.py` & `tycho-api-1.9a1.dev3/tycho/factory.py`

 * *Files identical despite different names*

### Comparing `tycho-api-1.9a1.dev2/tycho/kube.py` & `tycho-api-1.9a1.dev3/tycho/kube.py`

 * *Files identical despite different names*

### Comparing `tycho-api-1.9a1.dev2/tycho/model.py` & `tycho-api-1.9a1.dev3/tycho/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -149,15 +149,15 @@
     def __repr__(self):
         return f"name:{self.name} image:{self.image} id:{self.identity} limits:{self.limits}"
 
 
 
 class System:
     """ Distributed system of interacting containerized software. """
-    def __init__(self, config, name, principal, service_account, conn_string, proxy_rewrite_rule, containers, identifier, services={}, security_context={}):
+    def __init__(self, config, name, principal, service_account, conn_string, proxy_rewrite_rule, containers, identifier, services={}, security_context={}, init_security_context={}):
         """ Construct a new abstract model of a system given a name and set of containers.
         
             Serves as context for the generation of compute cluster specific artifacts.
 
             :param config: Configuration information.
             :type name: `Config`
             :param name: Name of the system.
@@ -197,28 +197,30 @@
         self.system_env = dict(principal)
         """ System tags """
         self.username = principal.get("username")
         self.host = principal.get("host")
         self.annotations = {}
         self.namespace = "default"
         self.serviceaccount = service_account
-        self.enable_init_container = os.environ.get("TYCHO_APP_ENABLE_VOLUME_PERMISSIONS_INIT_CONTAINER", "true")
+        self.enable_init_container = os.environ.get("TYCHO_APP_ENABLE_INIT_CONTAINER", "true")
         self.conn_string = conn_string
         """PVC flags and other variables for default volumes"""
         self.create_home_dirs = os.environ.get("CREATE_HOME_DIRS", "false").lower()
         self.stdnfs_pvc = os.environ.get("STDNFS_PVC", "stdnfs")
         self.parent_dir = os.environ.get('PARENT_DIR', 'home')
         self.subpath_dir = os.environ.get('SUBPATH_DIR', self.username)
         self.shared_dir = os.environ.get('SHARED_DIR', 'shared')
         """Default UID and GID for the system"""
         default_security_context = self.config.get('tycho')['compute']['system']['defaults']['securityContext']
         self.default_run_as_user = default_security_context.get('uid', '1000')
         self.default_run_as_group = default_security_context.get('gid', '1000')
         """Override container security context"""
         self.security_context = security_context
+        """init security context"""
+        self.init_security_context = init_security_context
         """Resources and limits for the init container"""
         self.init_cpus = os.environ.get("TYCHO_APP_INIT_CPUS", "250m")
         self.init_memory = os.environ.get("TYCHO_APP_INIT_MEMORY", "250Mi")
         """Proxy rewrite rule for ambassador service annotations"""
         self.proxy_rewrite_rule = proxy_rewrite_rule
         """Flag for checking if an IRODS connection is enabled"""
         if os.environ.get("IROD_ZONE") != None:
@@ -227,28 +229,41 @@
             self.nfsrods_uid = os.environ.get(self.username+"_NFSRODS_UID",' ')
         else:
             logger.info("Irods zone not enabled")
 
     @staticmethod
     def set_security_context(sc_from_registry):
         security_context: dict[str, Any] = {}
-        if os.environ.get("TYCHO_APP_RUN_AS_USER"):
-            security_context["run_as_user"] = os.environ.get("TYCHO_APP_RUN_AS_USER")
+        if "runAsUser" in sc_from_registry.keys():
+            security_context["run_as_user"] = str(sc_from_registry.get("runAsUser"))
         else:
-            security_context["run_as_user"] = sc_from_registry.get("runAsUser")
-        if os.environ.get("TYCHO_APP_RUN_AS_GROUP"):
-            security_context["run_as_group"] = os.environ.get("TYCHO_APP_RUN_AS_GROUP")
+            security_context["run_as_user"] = os.environ.get("TYCHO_APP_RUN_AS_USER", "0")
+        if "runAsGroup" in sc_from_registry.keys():
+            security_context["run_as_group"] = str(sc_from_registry.get("runAsGroup"))
         else:
-            security_context["run_as_group"] = sc_from_registry.get("runAsGroup")
-        if os.environ.get("TYCHO_APP_FS_GROUP"):
-            security_context["fs_group"] = os.environ.get("TYCHO_APP_FS_GROUP")
+            security_context["run_as_group"] = os.environ.get("TYCHO_APP_RUN_AS_GROUP", "0")
+        if "fsGroup" in sc_from_registry.keys():
+            security_context["fs_group"] = str(sc_from_registry.get("fsGroup"))
         else:
-            security_context["fs_group"] = sc_from_registry.get("fsGroup")
+            security_context["fs_group"] = os.environ.get("TYCHO_APP_FS_GROUP", "0")
         return security_context
 
+    @staticmethod
+    def set_init_security_context(sc_from_registry):
+        init_security_context = {}
+        if "initRunAsUser" in sc_from_registry.keys():
+            init_security_context["run_as_user"] = str(sc_from_registry.get("initRunAsUser"))
+        else:
+            init_security_context["run_as_user"] = os.environ.get("INIT_SC_RUN_AS_USER", "0")
+        if "initRunAsGroup" in sc_from_registry.keys():
+            init_security_context["run_as_group"] = str(sc_from_registry.get("initRunAsGroup"))
+        else:
+            init_security_context["run_as_group"] = os.environ.get("INIT_SC_RUN_AS_GROUP", "0")
+        return init_security_context
+
     def _get_ambassador_id(self):
         return os.environ.get("AMBASSADOR_ID", "")
     
     @staticmethod
     def get_identifier():
         return uuid.uuid4().hex
 
@@ -299,14 +314,15 @@
         
             :param name: Name of the system.
             :param system: Parsed docker-compose specification.
             :param env: Dictionary of settings.
             :param services: Service specifications - networking configuration.
         """
         security_context = System.set_security_context(system.get("security_context", {}))
+        init_security_context = System.set_init_security_context(system.get("security_context", {}))
         principal = json.loads(principal)
         identifier = System.get_identifier()
         containers = []
         if env != None:
             env['identifier'] = identifier
             env['username'] = principal.get('username',"Unknown")
             system_port = None
@@ -403,15 +419,16 @@
             "principal": principal,
             "service_account": service_account,
             "conn_string": spec.get("conn_string", ""),
             "proxy_rewrite_rule": spec.get("proxy_rewrite_rule", False),
             "containers": containers,
             "identifier": identifier,
             "services": services,
-            "security_context": security_context
+            "security_context": security_context,
+            "init_security_context": init_security_context
         }
         logger.debug (f"parsed-system: {json.dumps(system_specification, indent=2)}")
         system = System(**system_specification)
         system.source_text = yaml.dump (system)
         return system
 
     def __repr__(self):
```

### Comparing `tycho-api-1.9a1.dev2/tycho/template/patch.yaml` & `tycho-api-1.9a1.dev3/tycho/template/patch.yaml`

 * *Files identical despite different names*

### Comparing `tycho-api-1.9a1.dev2/tycho/template/pod.yaml` & `tycho-api-1.9a1.dev3/tycho/template/pod.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -29,44 +29,43 @@
   {% if container.limits.gpus != None and loop.first %}
   tolerations:
   - key: "nvidia.com/gpu"
     operator: "Exists"
     effect: "NoSchedule"
   {% endif %}
   {% endif %}
-  {% if system.security_context.run_as_user or system.security_context.run_as_group or system.security_context.fs_group %}
+  {% if system.security_context.fs_group %}
   securityContext:
-    {% if system.security_context.run_as_user %}
-    runAsUser: {{ system.security_context.run_as_user }}
-    {% endif %}
-    {% if system.security_context.run_as_group %}
-    runAsGroup: {{ system.security_context.run_as_group }}
-    {% endif %}
-    {% if system.security_context.fs_group %}
     fsGroup: {{ system.security_context.fs_group }}
-    {% endif %}
   {% endif %}
 {% if (system.enable_init_container == "true") and (system.create_home_dirs == "true") and (system.dev_phase != "test") %}
   initContainers:
   - name: volume-tasks
     image: busybox:1.28
+    {% if system.init_security_context.run_as_user or system.init_security_context.run_as_group %}
+    securityContext:
+      {% if system.init_security_context.run_as_user %}
+      runAsUser: {{ system.init_security_context.run_as_user }}
+      {% endif %}
+      {% if system.init_security_context.run_as_group %}
+      runAsGroup: {{ system.init_security_context.run_as_group }}
+      {% endif %}
+    {% endif %}
     # Fixed resources
     resources:
       requests:
         memory: {{ system.init_memory }}
         cpu: {{ system.init_cpus }}
       limits:
         memory: {{ system.init_memory }}
         cpu: {{ system.init_cpus }}
     command: [ 'sh', '-c' ]
     args:
       - mkdir -p {{ system.parent_dir }}/{{ system.subpath_dir }} &&
-        chmod 777 {{ system.parent_dir }}/{{ system.subpath_dir }} &&
         mkdir -p {{ system.parent_dir }}/{{ system.shared_dir }} &&
-        chmod 777 {{ system.parent_dir }}/{{ system.shared_dir }} &&
         ls -aln {{ system.parent_dir }} &&
         echo OK
     volumeMounts:
     - name: {{ system.stdnfs_pvc }}
       mountPath: {{ system.parent_dir }}
   {% if system.irods_enabled == True %}
   - name: nfsrods-prep
@@ -84,14 +83,23 @@
   {% endif %}
 {% endif %}
 {% endfor %}
   containers:
 {% for container in system.containers %}    
   - name: {{ container.name }}
     image: {{ container.image }}
+    {% if system.security_context.run_as_user or system.security_context.run_as_group %}
+    securityContext:
+      {% if system.security_context.run_as_user %}
+      runAsUser: {{ system.security_context.run_as_user }}
+      {% endif %}
+      {% if system.security_context.run_as_group %}
+      runAsGroup: {{ system.security_context.run_as_group }}
+      {% endif %}
+    {% endif %}
 {% if container.command %}
     command: {{ container.command }}
 {% endif %}
     env:
 {% if container.env %}
     {%for e in container.env %}
     - name : {{ e[0] }}
```

### Comparing `tycho-api-1.9a1.dev2/tycho/template/pv.yaml` & `tycho-api-1.9a1.dev3/tycho/template/pv.yaml`

 * *Files identical despite different names*

### Comparing `tycho-api-1.9a1.dev2/tycho/template/service.yaml` & `tycho-api-1.9a1.dev3/tycho/template/service.yaml`

 * *Files identical despite different names*

### Comparing `tycho-api-1.9a1.dev2/tycho/tycho_utils.py` & `tycho-api-1.9a1.dev3/tycho/tycho_utils.py`

 * *Files identical despite different names*

### Comparing `tycho-api-1.9a1.dev2/tycho_api.egg-info/PKG-INFO` & `tycho-api-1.9a1.dev3/tycho_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tycho-api
-Version: 1.9a1.dev2
+Version: 1.9a1.dev3
 Summary: Tycho is an API, compiler, and executor for cloud native distributed systems.
 Home-page: https://github.com/helxplatform/tycho.git
 Maintainer: Renci
 Maintainer-email: muralikarthik.k@renci.org
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tycho-api-1.9a1.dev2/tycho_api.egg-info/SOURCES.txt` & `tycho-api-1.9a1.dev3/tycho_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tycho-api-1.9a1.dev2/tycho_api.egg-info/requires.txt` & `tycho-api-1.9a1.dev3/tycho_api.egg-info/requires.txt`

 * *Files identical despite different names*

