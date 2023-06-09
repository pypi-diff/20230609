# Comparing `tmp/Andreani_QA_parameters-0.0.1.tar.gz` & `tmp/Andreani_QA_Parameters-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Andreani_QA_parameters-0.0.1.tar", last modified: Mon Feb  6 13:49:04 2023, max compression
+gzip compressed data, was "Andreani_QA_Parameters-0.0.2.tar", last modified: Fri Jun  9 19:15:08 2023, max compression
```

## Comparing `Andreani_QA_parameters-0.0.1.tar` & `Andreani_QA_Parameters-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-02-06 13:49:04.064139 Andreani_QA_parameters-0.0.1/
-drwxrwxrwx   0        0        0        0 2023-02-06 13:49:04.052173 Andreani_QA_parameters-0.0.1/Andreani_QA_parameters/
--rw-rw-rw-   0        0        0     9226 2023-02-01 14:29:37.000000 Andreani_QA_parameters-0.0.1/Andreani_QA_parameters/Encriptor.py
--rw-rw-rw-   0        0        0     3004 2023-01-26 19:22:46.000000 Andreani_QA_parameters-0.0.1/Andreani_QA_parameters/Parameters.py
--rw-rw-rw-   0        0        0       68 2023-02-01 14:29:37.000000 Andreani_QA_parameters-0.0.1/Andreani_QA_parameters/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-06 13:49:04.061148 Andreani_QA_parameters-0.0.1/Andreani_QA_parameters.egg-info/
--rw-rw-rw-   0        0        0      324 2023-02-06 13:49:03.000000 Andreani_QA_parameters-0.0.1/Andreani_QA_parameters.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      355 2023-02-06 13:49:04.000000 Andreani_QA_parameters-0.0.1/Andreani_QA_parameters.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-06 13:49:03.000000 Andreani_QA_parameters-0.0.1/Andreani_QA_parameters.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-02-06 13:49:03.000000 Andreani_QA_parameters-0.0.1/Andreani_QA_parameters.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-02-06 13:49:03.000000 Andreani_QA_parameters-0.0.1/Andreani_QA_parameters.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      324 2023-02-06 13:49:04.063143 Andreani_QA_parameters-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-01-26 19:44:24.000000 Andreani_QA_parameters-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-02-06 13:49:04.064139 Andreani_QA_parameters-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1210 2023-02-06 13:49:02.000000 Andreani_QA_parameters-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 19:15:08.683287 Andreani_QA_Parameters-0.0.2/
+drwxrwxrwx   0        0        0        0 2023-06-09 19:15:08.669930 Andreani_QA_Parameters-0.0.2/Andreani_QA_Parameters.egg-info/
+-rw-rw-rw-   0        0        0      317 2023-06-09 19:15:08.000000 Andreani_QA_Parameters-0.0.2/Andreani_QA_Parameters.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      355 2023-06-09 19:15:08.000000 Andreani_QA_Parameters-0.0.2/Andreani_QA_Parameters.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 19:15:08.000000 Andreani_QA_Parameters-0.0.2/Andreani_QA_Parameters.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-09 19:15:08.000000 Andreani_QA_Parameters-0.0.2/Andreani_QA_Parameters.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-06-09 19:15:08.000000 Andreani_QA_Parameters-0.0.2/Andreani_QA_Parameters.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 19:15:08.678910 Andreani_QA_Parameters-0.0.2/Andreani_QA_parameters/
+-rw-rw-rw-   0        0        0    10150 2023-05-22 19:22:31.000000 Andreani_QA_Parameters-0.0.2/Andreani_QA_parameters/Encriptor.py
+-rw-rw-rw-   0        0        0     3098 2023-05-22 18:41:22.000000 Andreani_QA_Parameters-0.0.2/Andreani_QA_parameters/Parameters.py
+-rw-rw-rw-   0        0        0       68 2023-02-01 14:29:37.000000 Andreani_QA_Parameters-0.0.2/Andreani_QA_parameters/__init__.py
+-rw-rw-rw-   0        0        0      317 2023-06-09 19:15:08.682328 Andreani_QA_Parameters-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-01-26 19:44:24.000000 Andreani_QA_Parameters-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-09 19:15:08.684287 Andreani_QA_Parameters-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1203 2023-06-09 19:14:59.000000 Andreani_QA_Parameters-0.0.2/setup.py
```

### Comparing `Andreani_QA_parameters-0.0.1/Andreani_QA_parameters/Encriptor.py` & `Andreani_QA_Parameters-0.0.2/Andreani_QA_parameters/Encriptor.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import os
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.primitives.kdf.pbkdf2 import PBKDF2HMAC
 from cryptography.hazmat.backends import default_backend
 import base64
 from cryptography.fernet import Fernet
 from functions.Parameters import Parameters
-#XML tools
 import xml.etree.ElementTree as ET
 import bz2
+import xml.dom.minidom
 
 PATH_FUNCTIONS = os.path.join(Parameters.current_path, 'functions\\src\\')
 NAME_FILE_ENCRIPTED = 'environment_access.xml'
 NAME_FILE_TEMPORAL = 'environment_access.xml'
 ENVIROMENT_VAR = 'PYBOT_KEY'
 
 
@@ -254,13 +254,34 @@
             deencrypted_data = fe.decrypt(data)
             decompressed_data = bz2.decompress(deencrypted_data)
             with open(path_target, 'wb') as output_file:
                 output_file.write(decompressed_data)
         except FileNotFoundError:
             print("El archivo buscado no existe en el directorio especificado.")
 
+    def get_all_data_from_xml_file_encrypted(self):
+        key = self.get_enviroment_key_from_file()
+        fe = Fernet(key)
+        return_data = None
+        path_origin = os.path.join(PATH_FUNCTIONS, NAME_FILE_ENCRIPTED)
+        try:
+            with open(path_origin, 'rb') as file:
+                data = file.read()
+            deencrypted_data = fe.decrypt(data)
+            decompressed_data = bz2.decompress(deencrypted_data)
+            print(xml.dom.minidom.parseString(decompressed_data).toprettyxml())
+        except:
+            raise "Ha Ocurrido un Error en el Tiempo de Ejecución -> ERROR CODE 204 (Encriptor)"
+
+
+
+
 
 if __name__ == '__main__':
     pass
+    #TXT
+    #Encriptor().decrypt_file("environment_access.txt", "environment_access.txt")  # DESENCRIPTA
+    #Encriptor().encrypt_file("environment_access.txt", "environment_access.txt")  # ENCRIPTA
     #XML
     Encriptor().compress_and_encrypt_xml() # ENCRIPTA
     #Encriptor().decompress_and_deencrypt_xml() # DESENCRIPTA
+    #Encriptor().get_all_data_from_xml_file_encrypted()
```

### Comparing `Andreani_QA_parameters-0.0.1/Andreani_QA_parameters/Parameters.py` & `Andreani_QA_Parameters-0.0.2/Andreani_QA_parameters/Parameters.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 
 
 class Parameters:
     # CONFIGURACION PATH Y TESTCASE
     current_path = os.path.abspath(os.path.join(__file__, "../.."))
     file_name_stored = None
     env = None
+
+    # CONFIGURACION PARA UTILIZAR CSV DESDE SHAREPOINT
+    #sharepoint_data_jmeter=None
+
     # CONFIGURACION FORMATO DE FECHA
     date_format = '%d/%m/%Y'
     time_format = "%H:%M:%S"
 
     # CONFIGURACION DE TIEMPO Y REINTENTOS PARA LA OBTENCIÓN DE ELEMENTOS
     time_between_retries = 0.5
     number_retries = 6
```

### Comparing `Andreani_QA_parameters-0.0.1/setup.py` & `Andreani_QA_Parameters-0.0.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '0.0.1'  # Muy importante, deberéis ir cambiando la versión de vuestra librería según incluyáis nuevas funcionalidades
-PACKAGE_NAME = 'Andreani_QA_parameters'  # Debe coincidir con el nombre de la carpeta
-AUTHOR = 'Andreani_QA_Automation'
+VERSION = '0.0.2'  # Muy importante, deberéis ir cambiando la versión de vuestra librería según incluyáis nuevas funcionalidades
+PACKAGE_NAME = 'Andreani_QA_Parameters'  # Debe coincidir con el nombre de la carpeta
+AUTHOR = 'AndreaniTesting'
 AUTHOR_EMAIL = 'user_appglatest@andreani.com'
 URL = ''
 
 LICENSE = 'MIT'  # Tipo de licencia
 DESCRIPTION = 'Parametros + Encriptor para ejecución de casos automatizados'  # Descripción corta
 LONG_DESCRIPTION = ""  # Referencia al documento README con una descripción más elaborada
 LONG_DESC_TYPE = "text/markdown"
```

