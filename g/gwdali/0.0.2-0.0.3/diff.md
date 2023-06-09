# Comparing `tmp/gwdali-0.0.2.tar.gz` & `tmp/gwdali-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwdali-0.0.2.tar", last modified: Tue May 16 13:55:22 2023, max compression
+gzip compressed data, was "gwdali-0.0.3.tar", last modified: Fri Jun  9 21:05:24 2023, max compression
```

## Comparing `gwdali-0.0.2.tar` & `gwdali-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,27 @@
-drwxrwxr-x   0 josiel    (1000) josiel    (1000)        0 2023-05-16 13:55:22.470333 gwdali-0.0.2/
-drwxrwxr-x   0 josiel    (1000) josiel    (1000)        0 2023-05-16 13:55:22.466334 gwdali-0.0.2/GWDALI/
--rw-r--r--   0 josiel    (1000) josiel    (1000)     8949 2023-05-16 02:06:35.000000 gwdali-0.0.2/GWDALI/GWDALI.py
--rw-r--r--   0 josiel    (1000) josiel    (1000)      143 2023-01-12 01:48:50.000000 gwdali-0.0.2/GWDALI/__init__.py
--rw-r--r--   0 josiel    (1000) josiel    (1000)     1089 2023-03-21 13:34:46.000000 gwdali-0.0.2/LICENSE
--rw-rw-r--   0 josiel    (1000) josiel    (1000)     5058 2023-05-16 13:55:22.470333 gwdali-0.0.2/PKG-INFO
--rw-r--r--   0 josiel    (1000) josiel    (1000)     4709 2023-04-14 13:50:04.000000 gwdali-0.0.2/README.md
-drwxrwxr-x   0 josiel    (1000) josiel    (1000)        0 2023-05-16 13:55:22.466334 gwdali-0.0.2/gwdali.egg-info/
--rw-r--r--   0 josiel    (1000) josiel    (1000)     5058 2023-05-16 13:55:22.000000 gwdali-0.0.2/gwdali.egg-info/PKG-INFO
--rw-r--r--   0 josiel    (1000) josiel    (1000)      182 2023-05-16 13:55:22.000000 gwdali-0.0.2/gwdali.egg-info/SOURCES.txt
--rw-r--r--   0 josiel    (1000) josiel    (1000)        1 2023-05-16 13:55:22.000000 gwdali-0.0.2/gwdali.egg-info/dependency_links.txt
--rw-r--r--   0 josiel    (1000) josiel    (1000)        7 2023-05-16 13:55:22.000000 gwdali-0.0.2/gwdali.egg-info/top_level.txt
--rw-rw-r--   0 josiel    (1000) josiel    (1000)       38 2023-05-16 13:55:22.470333 gwdali-0.0.2/setup.cfg
--rw-r--r--   0 josiel    (1000) josiel    (1000)      638 2023-05-16 13:54:42.000000 gwdali-0.0.2/setup.py
+drwxrwxr-x   0 josiel    (1000) josiel    (1000)        0 2023-06-09 21:05:24.523400 gwdali-0.0.3/
+drwxrwxr-x   0 josiel    (1000) josiel    (1000)        0 2023-06-09 21:05:24.515400 gwdali-0.0.3/GWDALI/
+drwxrwxr-x   0 josiel    (1000) josiel    (1000)        0 2023-06-09 21:05:24.519400 gwdali-0.0.3/GWDALI/Detectors_Sensitivity/
+-rw-r--r--   0 josiel    (1000) josiel    (1000)       14 2022-11-09 20:10:14.000000 gwdali-0.0.3/GWDALI/Detectors_Sensitivity/__init__.py
+-rw-r--r--   0 josiel    (1000) josiel    (1000)      921 2023-02-28 14:51:14.000000 gwdali-0.0.3/GWDALI/Detectors_Sensitivity/plot_Sn.py
+-rw-r--r--   0 josiel    (1000) josiel    (1000)     8949 2023-05-16 02:06:35.000000 gwdali-0.0.3/GWDALI/GWDALI.py
+-rw-r--r--   0 josiel    (1000) josiel    (1000)      143 2023-01-12 01:48:50.000000 gwdali-0.0.3/GWDALI/__init__.py
+drwxrwxr-x   0 josiel    (1000) josiel    (1000)        0 2023-06-09 21:05:24.519400 gwdali-0.0.3/GWDALI/lib/
+-rw-r--r--   0 josiel    (1000) josiel    (1000)     2945 2022-08-02 22:07:40.000000 gwdali-0.0.3/GWDALI/lib/Angles_lib.py
+-rw-r--r--   0 josiel    (1000) josiel    (1000)     8601 2023-05-16 02:02:47.000000 gwdali-0.0.3/GWDALI/lib/Compute_Tensors.py
+-rw-r--r--   0 josiel    (1000) josiel    (1000)     5858 2023-02-16 19:29:30.000000 gwdali-0.0.3/GWDALI/lib/Corner_Plots.py
+-rw-r--r--   0 josiel    (1000) josiel    (1000)     5579 2023-05-16 01:58:53.000000 gwdali-0.0.3/GWDALI/lib/Derivatives_Tensors.py
+-rw-r--r--   0 josiel    (1000) josiel    (1000)     3172 2023-05-16 01:56:05.000000 gwdali-0.0.3/GWDALI/lib/Dictionaries.py
+-rw-r--r--   0 josiel    (1000) josiel    (1000)     7896 2023-04-13 14:39:02.000000 gwdali-0.0.3/GWDALI/lib/Likelihood.py
+-rw-r--r--   0 josiel    (1000) josiel    (1000)     3274 2023-01-20 00:22:18.000000 gwdali-0.0.3/GWDALI/lib/Symmetric_Indexies.py
+-rw-r--r--   0 josiel    (1000) josiel    (1000)     4479 2023-05-16 02:00:22.000000 gwdali-0.0.3/GWDALI/lib/Waveforms.py
+-rw-r--r--   0 josiel    (1000) josiel    (1000)      145 2023-01-12 19:30:22.000000 gwdali-0.0.3/GWDALI/lib/__init__.py
+-rw-r--r--   0 josiel    (1000) josiel    (1000)     1089 2023-03-21 13:34:46.000000 gwdali-0.0.3/LICENSE
+-rw-rw-r--   0 josiel    (1000) josiel    (1000)     5058 2023-06-09 21:05:24.523400 gwdali-0.0.3/PKG-INFO
+-rw-r--r--   0 josiel    (1000) josiel    (1000)     4709 2023-04-14 13:50:04.000000 gwdali-0.0.3/README.md
+drwxrwxr-x   0 josiel    (1000) josiel    (1000)        0 2023-06-09 21:05:24.523400 gwdali-0.0.3/gwdali.egg-info/
+-rw-rw-r--   0 josiel    (1000) josiel    (1000)     5058 2023-06-09 21:05:24.000000 gwdali-0.0.3/gwdali.egg-info/PKG-INFO
+-rw-rw-r--   0 josiel    (1000) josiel    (1000)      511 2023-06-09 21:05:24.000000 gwdali-0.0.3/gwdali.egg-info/SOURCES.txt
+-rw-rw-r--   0 josiel    (1000) josiel    (1000)        1 2023-06-09 21:05:24.000000 gwdali-0.0.3/gwdali.egg-info/dependency_links.txt
+-rw-rw-r--   0 josiel    (1000) josiel    (1000)        7 2023-06-09 21:05:24.000000 gwdali-0.0.3/gwdali.egg-info/top_level.txt
+-rw-rw-r--   0 josiel    (1000) josiel    (1000)       38 2023-06-09 21:05:24.523400 gwdali-0.0.3/setup.cfg
+-rw-r--r--   0 josiel    (1000) josiel    (1000)      658 2023-06-09 21:04:36.000000 gwdali-0.0.3/setup.py
```

### Comparing `gwdali-0.0.2/GWDALI/GWDALI.py` & `gwdali-0.0.3/GWDALI/GWDALI.py`

 * *Files identical despite different names*

### Comparing `gwdali-0.0.2/LICENSE` & `gwdali-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gwdali-0.0.2/PKG-INFO` & `gwdali-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwdali
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Fisher-Based Software for Parameter Estimation from Gravitational Waves
 Author: Josiel Mendonça Soares de Souza
 Author-email: jmsdsouza.phd@gmail.com
 License: MIT License
 Keywords: fisher matrix,gravitational waves,gw,dali
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `gwdali-0.0.2/README.md` & `gwdali-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `gwdali-0.0.2/gwdali.egg-info/PKG-INFO` & `gwdali-0.0.3/gwdali.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwdali
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Fisher-Based Software for Parameter Estimation from Gravitational Waves
 Author: Josiel Mendonça Soares de Souza
 Author-email: jmsdsouza.phd@gmail.com
 License: MIT License
 Keywords: fisher matrix,gravitational waves,gw,dali
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `gwdali-0.0.2/setup.py` & `gwdali-0.0.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from setuptools import setup
+from setuptools import setup, find_packages
 
 with open("README.md",'r') as arq:
 	readme = arq.read()
 
 setup(
 	name = 'gwdali',
-	version = '0.0.2',
+	version = '0.0.3',
 	license = 'MIT License',
 	author  = 'Josiel Mendonça Soares de Souza',
 	long_description = readme,
 	long_description_content_type = "text/markdown",
 	author_email = 'jmsdsouza.phd@gmail.com',
 	keywords = 'fisher matrix, gravitational waves, gw, dali',
 	description = 'A Fisher-Based Software for Parameter Estimation from Gravitational Waves',
-	packages = ['GWDALI'],
+	packages = find_packages(),
 	install_requeries = ['numpy','matplotlib','scipy','bilby','astropy','itertools'],
 	#url = "https://github.com/jmsdsouzaPhD/gwdali/",
 )
```

