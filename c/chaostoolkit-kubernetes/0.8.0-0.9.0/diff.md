# Comparing `tmp/chaostoolkit-kubernetes-0.8.0.tar.gz` & `tmp/chaostoolkit-kubernetes-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/chaostoolkit-kubernetes-0.8.0.tar", last modified: Fri Dec 29 17:11:03 2017, max compression
+gzip compressed data, was "dist/chaostoolkit-kubernetes-0.9.0.tar", last modified: Tue Jan 16 16:49:22 2018, max compression
```

## Comparing `chaostoolkit-kubernetes-0.8.0.tar` & `chaostoolkit-kubernetes-0.9.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2017-12-29 17:11:03.000000 chaostoolkit-kubernetes-0.8.0/
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2017-12-29 17:11:03.000000 chaostoolkit-kubernetes-0.8.0/chaosk8s/
--rw-r--r--   0 travis    (2000) travis    (2000)     2536 2017-12-29 17:09:26.000000 chaostoolkit-kubernetes-0.8.0/chaosk8s/__init__.py
--rw-r--r--   0 travis    (2000) travis    (2000)     3757 2017-12-29 17:09:26.000000 chaostoolkit-kubernetes-0.8.0/chaosk8s/actions.py
--rw-r--r--   0 travis    (2000) travis    (2000)     7541 2017-12-29 17:09:26.000000 chaostoolkit-kubernetes-0.8.0/chaosk8s/probes.py
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2017-12-29 17:11:03.000000 chaostoolkit-kubernetes-0.8.0/chaostoolkit_kubernetes.egg-info/
--rw-r--r--   0 travis    (2000) travis    (2000)     3745 2017-12-29 17:11:03.000000 chaostoolkit-kubernetes-0.8.0/chaostoolkit_kubernetes.egg-info/PKG-INFO
--rw-r--r--   0 travis    (2000) travis    (2000)      383 2017-12-29 17:11:03.000000 chaostoolkit-kubernetes-0.8.0/chaostoolkit_kubernetes.egg-info/SOURCES.txt
--rw-r--r--   0 travis    (2000) travis    (2000)        1 2017-12-29 17:11:03.000000 chaostoolkit-kubernetes-0.8.0/chaostoolkit_kubernetes.egg-info/dependency_links.txt
--rw-r--r--   0 travis    (2000) travis    (2000)       73 2017-12-29 17:11:03.000000 chaostoolkit-kubernetes-0.8.0/chaostoolkit_kubernetes.egg-info/requires.txt
--rw-r--r--   0 travis    (2000) travis    (2000)        9 2017-12-29 17:11:03.000000 chaostoolkit-kubernetes-0.8.0/chaostoolkit_kubernetes.egg-info/top_level.txt
--rw-r--r--   0 travis    (2000) travis    (2000)     2873 2017-12-29 17:09:26.000000 chaostoolkit-kubernetes-0.8.0/CHANGELOG.md
--rw-r--r--   0 travis    (2000) travis    (2000)    11357 2017-12-29 17:09:26.000000 chaostoolkit-kubernetes-0.8.0/LICENSE
--rw-r--r--   0 travis    (2000) travis    (2000)       98 2017-12-29 17:09:26.000000 chaostoolkit-kubernetes-0.8.0/MANIFEST.in
--rw-r--r--   0 travis    (2000) travis    (2000)     2169 2017-12-29 17:09:26.000000 chaostoolkit-kubernetes-0.8.0/README.md
--rw-r--r--   0 travis    (2000) travis    (2000)      174 2017-12-29 17:09:26.000000 chaostoolkit-kubernetes-0.8.0/pytest.ini
--rw-r--r--   0 travis    (2000) travis    (2000)       72 2017-12-29 17:09:26.000000 chaostoolkit-kubernetes-0.8.0/requirements.txt
--rw-r--r--   0 travis    (2000) travis    (2000)      114 2017-12-29 17:11:03.000000 chaostoolkit-kubernetes-0.8.0/setup.cfg
--rw-r--r--   0 travis    (2000) travis    (2000)     1945 2017-12-29 17:09:26.000000 chaostoolkit-kubernetes-0.8.0/setup.py
--rw-r--r--   0 travis    (2000) travis    (2000)     3745 2017-12-29 17:11:03.000000 chaostoolkit-kubernetes-0.8.0/PKG-INFO
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-01-16 16:49:22.000000 chaostoolkit-kubernetes-0.9.0/
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-01-16 16:49:22.000000 chaostoolkit-kubernetes-0.9.0/chaosk8s/
+-rw-r--r--   0 travis    (2000) travis    (2000)     4809 2018-01-16 16:48:32.000000 chaostoolkit-kubernetes-0.9.0/chaosk8s/__init__.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     3757 2018-01-16 16:48:32.000000 chaostoolkit-kubernetes-0.9.0/chaosk8s/actions.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     7541 2018-01-16 16:48:32.000000 chaostoolkit-kubernetes-0.9.0/chaosk8s/probes.py
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-01-16 16:49:22.000000 chaostoolkit-kubernetes-0.9.0/chaostoolkit_kubernetes.egg-info/
+-rw-r--r--   0 travis    (2000) travis    (2000)     3967 2018-01-16 16:49:22.000000 chaostoolkit-kubernetes-0.9.0/chaostoolkit_kubernetes.egg-info/PKG-INFO
+-rw-r--r--   0 travis    (2000) travis    (2000)      383 2018-01-16 16:49:22.000000 chaostoolkit-kubernetes-0.9.0/chaostoolkit_kubernetes.egg-info/SOURCES.txt
+-rw-r--r--   0 travis    (2000) travis    (2000)        1 2018-01-16 16:49:22.000000 chaostoolkit-kubernetes-0.9.0/chaostoolkit_kubernetes.egg-info/dependency_links.txt
+-rw-r--r--   0 travis    (2000) travis    (2000)       74 2018-01-16 16:49:22.000000 chaostoolkit-kubernetes-0.9.0/chaostoolkit_kubernetes.egg-info/requires.txt
+-rw-r--r--   0 travis    (2000) travis    (2000)        9 2018-01-16 16:49:22.000000 chaostoolkit-kubernetes-0.9.0/chaostoolkit_kubernetes.egg-info/top_level.txt
+-rw-r--r--   0 travis    (2000) travis    (2000)     3023 2018-01-16 16:48:32.000000 chaostoolkit-kubernetes-0.9.0/CHANGELOG.md
+-rw-r--r--   0 travis    (2000) travis    (2000)    11357 2018-01-16 16:48:32.000000 chaostoolkit-kubernetes-0.9.0/LICENSE
+-rw-r--r--   0 travis    (2000) travis    (2000)       98 2018-01-16 16:48:32.000000 chaostoolkit-kubernetes-0.9.0/MANIFEST.in
+-rw-r--r--   0 travis    (2000) travis    (2000)     2327 2018-01-16 16:48:32.000000 chaostoolkit-kubernetes-0.9.0/README.md
+-rw-r--r--   0 travis    (2000) travis    (2000)      174 2018-01-16 16:48:32.000000 chaostoolkit-kubernetes-0.9.0/pytest.ini
+-rw-r--r--   0 travis    (2000) travis    (2000)       73 2018-01-16 16:48:32.000000 chaostoolkit-kubernetes-0.9.0/requirements.txt
+-rw-r--r--   0 travis    (2000) travis    (2000)      114 2018-01-16 16:49:22.000000 chaostoolkit-kubernetes-0.9.0/setup.cfg
+-rw-r--r--   0 travis    (2000) travis    (2000)     1945 2018-01-16 16:48:32.000000 chaostoolkit-kubernetes-0.9.0/setup.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     3967 2018-01-16 16:49:22.000000 chaostoolkit-kubernetes-0.9.0/PKG-INFO
```

### Comparing `chaostoolkit-kubernetes-0.8.0/chaosk8s/actions.py` & `chaostoolkit-kubernetes-0.9.0/chaosk8s/actions.py`

 * *Files identical despite different names*

### Comparing `chaostoolkit-kubernetes-0.8.0/chaosk8s/probes.py` & `chaostoolkit-kubernetes-0.9.0/chaosk8s/probes.py`

 * *Files identical despite different names*

### Comparing `chaostoolkit-kubernetes-0.8.0/chaostoolkit_kubernetes.egg-info/PKG-INFO` & `chaostoolkit-kubernetes-0.9.0/chaostoolkit_kubernetes.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: chaostoolkit-kubernetes
-Version: 0.8.0
+Version: 0.9.0
 Summary: Chaos Toolkit Kubernetes support
 Home-page: http://chaostoolkit.org
 Author: chaostoolkit Team
 Author-email: contact@chaostoolkit.org
 License: Apache License Version 2.0
 Description: # Chaos Toolkit Kubernetes Support
         
@@ -44,14 +44,22 @@
         }
         ```
         
         That's it!
         
         Please explore the code to see existing probes and actions.
         
+        ### Discovery
+        
+        You may use the Chaos Toolkit to discover the capabilities of this extension:
+        
+        ```
+        $ chaos discover chaostoolkit-kubernetes --no-install
+        ```
+        
         ## Configuration
         
         This extension to the Chaos Toolkit can use the Kubernetes configuration 
         found at the usual place in your HOME directory under `~/.kube/`. You can
         also pass the credentials via secrets as follows:
         
         ```json
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `chaostoolkit-kubernetes-0.8.0/CHANGELOG.md` & `chaostoolkit-kubernetes-0.9.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,20 @@
 # Changelog
 
 ## [Unreleased][]
 
-[Unreleased]: https://github.com/chaostoolkit/chaostoolkit-kubernetes/compare/0.8.0...HEAD
+[Unreleased]: https://github.com/chaostoolkit/chaostoolkit-kubernetes/compare/0.9.0...HEAD
+
+## [0.9.0][] - 2018-01-16
+
+[0.9.0]: https://github.com/chaostoolkit/chaostoolkit-kubernetes/compare/0.8.0...0.9.0
+
+### Added
+
+- discovery mechanism
 
 ## [0.8.0][] - 2017-12-29
 
 [0.8.0]: https://github.com/chaostoolkit/chaostoolkit-kubernetes/compare/0.7.0...0.8.0
 
 ### Added
```

### Comparing `chaostoolkit-kubernetes-0.8.0/LICENSE` & `chaostoolkit-kubernetes-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chaostoolkit-kubernetes-0.8.0/README.md` & `chaostoolkit-kubernetes-0.9.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -36,14 +36,22 @@
 }
 ```
 
 That's it!
 
 Please explore the code to see existing probes and actions.
 
+### Discovery
+
+You may use the Chaos Toolkit to discover the capabilities of this extension:
+
+```
+$ chaos discover chaostoolkit-kubernetes --no-install
+```
+
 ## Configuration
 
 This extension to the Chaos Toolkit can use the Kubernetes configuration 
 found at the usual place in your HOME directory under `~/.kube/`. You can
 also pass the credentials via secrets as follows:
 
 ```json
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `chaostoolkit-kubernetes-0.8.0/setup.py` & `chaostoolkit-kubernetes-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `chaostoolkit-kubernetes-0.8.0/PKG-INFO` & `chaostoolkit-kubernetes-0.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: chaostoolkit-kubernetes
-Version: 0.8.0
+Version: 0.9.0
 Summary: Chaos Toolkit Kubernetes support
 Home-page: http://chaostoolkit.org
 Author: chaostoolkit Team
 Author-email: contact@chaostoolkit.org
 License: Apache License Version 2.0
 Description: # Chaos Toolkit Kubernetes Support
         
@@ -44,14 +44,22 @@
         }
         ```
         
         That's it!
         
         Please explore the code to see existing probes and actions.
         
+        ### Discovery
+        
+        You may use the Chaos Toolkit to discover the capabilities of this extension:
+        
+        ```
+        $ chaos discover chaostoolkit-kubernetes --no-install
+        ```
+        
         ## Configuration
         
         This extension to the Chaos Toolkit can use the Kubernetes configuration 
         found at the usual place in your HOME directory under `~/.kube/`. You can
         also pass the credentials via secrets as follows:
         
         ```json
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

