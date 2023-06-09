# Comparing `tmp/Andreani_QA_Parameters-0.0.2.tar.gz` & `tmp/Andreani_QA_Parameters-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Andreani_QA_Parameters-0.0.2.tar", last modified: Fri Jun  9 19:15:08 2023, max compression
+gzip compressed data, was "Andreani_QA_Parameters-0.0.3.tar", last modified: Fri Jun  9 20:40:40 2023, max compression
```

## Comparing `Andreani_QA_Parameters-0.0.2.tar` & `Andreani_QA_Parameters-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 19:15:08.683287 Andreani_QA_Parameters-0.0.2/
-drwxrwxrwx   0        0        0        0 2023-06-09 19:15:08.669930 Andreani_QA_Parameters-0.0.2/Andreani_QA_Parameters.egg-info/
--rw-rw-rw-   0        0        0      317 2023-06-09 19:15:08.000000 Andreani_QA_Parameters-0.0.2/Andreani_QA_Parameters.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      355 2023-06-09 19:15:08.000000 Andreani_QA_Parameters-0.0.2/Andreani_QA_Parameters.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 19:15:08.000000 Andreani_QA_Parameters-0.0.2/Andreani_QA_Parameters.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-06-09 19:15:08.000000 Andreani_QA_Parameters-0.0.2/Andreani_QA_Parameters.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-06-09 19:15:08.000000 Andreani_QA_Parameters-0.0.2/Andreani_QA_Parameters.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-09 19:15:08.678910 Andreani_QA_Parameters-0.0.2/Andreani_QA_parameters/
--rw-rw-rw-   0        0        0    10150 2023-05-22 19:22:31.000000 Andreani_QA_Parameters-0.0.2/Andreani_QA_parameters/Encriptor.py
--rw-rw-rw-   0        0        0     3098 2023-05-22 18:41:22.000000 Andreani_QA_Parameters-0.0.2/Andreani_QA_parameters/Parameters.py
--rw-rw-rw-   0        0        0       68 2023-02-01 14:29:37.000000 Andreani_QA_Parameters-0.0.2/Andreani_QA_parameters/__init__.py
--rw-rw-rw-   0        0        0      317 2023-06-09 19:15:08.682328 Andreani_QA_Parameters-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-01-26 19:44:24.000000 Andreani_QA_Parameters-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-06-09 19:15:08.684287 Andreani_QA_Parameters-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1203 2023-06-09 19:14:59.000000 Andreani_QA_Parameters-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 20:40:40.114983 Andreani_QA_Parameters-0.0.3/
+drwxrwxrwx   0        0        0        0 2023-06-09 20:40:40.094314 Andreani_QA_Parameters-0.0.3/Andreani_QA_Parameters.egg-info/
+-rw-rw-rw-   0        0        0      317 2023-06-09 20:40:39.000000 Andreani_QA_Parameters-0.0.3/Andreani_QA_Parameters.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      355 2023-06-09 20:40:39.000000 Andreani_QA_Parameters-0.0.3/Andreani_QA_Parameters.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 20:40:39.000000 Andreani_QA_Parameters-0.0.3/Andreani_QA_Parameters.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-09 20:40:39.000000 Andreani_QA_Parameters-0.0.3/Andreani_QA_Parameters.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-06-09 20:40:39.000000 Andreani_QA_Parameters-0.0.3/Andreani_QA_Parameters.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 20:40:40.109834 Andreani_QA_Parameters-0.0.3/Andreani_QA_parameters/
+-rw-rw-rw-   0        0        0    10152 2023-06-09 20:32:20.000000 Andreani_QA_Parameters-0.0.3/Andreani_QA_parameters/Encriptor.py
+-rw-rw-rw-   0        0        0     3108 2023-06-09 20:32:20.000000 Andreani_QA_Parameters-0.0.3/Andreani_QA_parameters/Parameters.py
+-rw-rw-rw-   0        0        0       68 2023-02-01 14:29:37.000000 Andreani_QA_Parameters-0.0.3/Andreani_QA_parameters/__init__.py
+-rw-rw-rw-   0        0        0      317 2023-06-09 20:40:40.113910 Andreani_QA_Parameters-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-01-26 19:44:24.000000 Andreani_QA_Parameters-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-09 20:40:40.116034 Andreani_QA_Parameters-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1203 2023-06-09 20:40:37.000000 Andreani_QA_Parameters-0.0.3/setup.py
```

### Comparing `Andreani_QA_Parameters-0.0.2/Andreani_QA_parameters/Encriptor.py` & `Andreani_QA_Parameters-0.0.3/Andreani_QA_parameters/Encriptor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.primitives.kdf.pbkdf2 import PBKDF2HMAC
 from cryptography.hazmat.backends import default_backend
 import base64
 from cryptography.fernet import Fernet
-from functions.Parameters import Parameters
+from Andreani_QA_parameters import Parameters
 import xml.etree.ElementTree as ET
 import bz2
 import xml.dom.minidom
 
 PATH_FUNCTIONS = os.path.join(Parameters.current_path, 'functions\\src\\')
 NAME_FILE_ENCRIPTED = 'environment_access.xml'
 NAME_FILE_TEMPORAL = 'environment_access.xml'
```

### Comparing `Andreani_QA_Parameters-0.0.2/Andreani_QA_parameters/Parameters.py` & `Andreani_QA_Parameters-0.0.3/Andreani_QA_parameters/Parameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import platform
 
 
 class Parameters:
     # CONFIGURACION PATH Y TESTCASE
-    current_path = os.path.abspath(os.path.join(__file__, "../.."))
+    current_path = os.path.abspath(os.path.join(__file__, "../../../../../"))
     file_name_stored = None
     env = None
 
     # CONFIGURACION PARA UTILIZAR CSV DESDE SHAREPOINT
     #sharepoint_data_jmeter=None
 
     # CONFIGURACION FORMATO DE FECHA
```

### Comparing `Andreani_QA_Parameters-0.0.2/setup.py` & `Andreani_QA_Parameters-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '0.0.2'  # Muy importante, deberéis ir cambiando la versión de vuestra librería según incluyáis nuevas funcionalidades
+VERSION = '0.0.3'  # Muy importante, deberéis ir cambiando la versión de vuestra librería según incluyáis nuevas funcionalidades
 PACKAGE_NAME = 'Andreani_QA_Parameters'  # Debe coincidir con el nombre de la carpeta
 AUTHOR = 'AndreaniTesting'
 AUTHOR_EMAIL = 'user_appglatest@andreani.com'
 URL = ''
 
 LICENSE = 'MIT'  # Tipo de licencia
 DESCRIPTION = 'Parametros + Encriptor para ejecución de casos automatizados'  # Descripción corta
```

