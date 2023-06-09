# Comparing `tmp/Andreani_QA_Functions-0.0.7.tar.gz` & `tmp/Andreani_QA_Functions-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Andreani_QA_Functions-0.0.7.tar", last modified: Fri Feb 17 17:55:36 2023, max compression
+gzip compressed data, was "Andreani_QA_Functions-0.0.8.tar", last modified: Fri Jun  9 19:19:29 2023, max compression
```

## Comparing `Andreani_QA_Functions-0.0.7.tar` & `Andreani_QA_Functions-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-02-17 17:55:36.152101 Andreani_QA_Functions-0.0.7/
-drwxrwxrwx   0        0        0        0 2023-02-17 17:55:36.139134 Andreani_QA_Functions-0.0.7/Andreani_QA_Functions/
--rw-rw-rw-   0        0        0    77099 2023-02-16 15:11:49.000000 Andreani_QA_Functions-0.0.7/Andreani_QA_Functions/Functions.py
--rw-rw-rw-   0        0        0       34 2023-02-06 14:42:59.000000 Andreani_QA_Functions-0.0.7/Andreani_QA_Functions/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-17 17:55:36.149107 Andreani_QA_Functions-0.0.7/Andreani_QA_Functions.egg-info/
--rw-rw-rw-   0        0        0      315 2023-02-17 17:55:36.000000 Andreani_QA_Functions-0.0.7/Andreani_QA_Functions.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      311 2023-02-17 17:55:36.000000 Andreani_QA_Functions-0.0.7/Andreani_QA_Functions.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-17 17:55:36.000000 Andreani_QA_Functions-0.0.7/Andreani_QA_Functions.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       77 2023-02-17 17:55:36.000000 Andreani_QA_Functions-0.0.7/Andreani_QA_Functions.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-02-17 17:55:36.000000 Andreani_QA_Functions-0.0.7/Andreani_QA_Functions.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      315 2023-02-17 17:55:36.151105 Andreani_QA_Functions-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-01-26 19:44:24.000000 Andreani_QA_Functions-0.0.7/README.md
--rw-rw-rw-   0        0        0       42 2023-02-17 17:55:36.152101 Andreani_QA_Functions-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1167 2023-02-16 20:19:02.000000 Andreani_QA_Functions-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 19:19:29.323846 Andreani_QA_Functions-0.0.8/
+drwxrwxrwx   0        0        0        0 2023-06-09 19:19:29.308579 Andreani_QA_Functions-0.0.8/Andreani_QA_Functions/
+-rw-rw-rw-   0        0        0    81115 2023-06-08 13:44:10.000000 Andreani_QA_Functions-0.0.8/Andreani_QA_Functions/Functions.py
+-rw-rw-rw-   0        0        0       34 2023-02-06 14:42:59.000000 Andreani_QA_Functions-0.0.8/Andreani_QA_Functions/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 19:19:29.321205 Andreani_QA_Functions-0.0.8/Andreani_QA_Functions.egg-info/
+-rw-rw-rw-   0        0        0      303 2023-06-09 19:19:29.000000 Andreani_QA_Functions-0.0.8/Andreani_QA_Functions.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      311 2023-06-09 19:19:29.000000 Andreani_QA_Functions-0.0.8/Andreani_QA_Functions.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 19:19:29.000000 Andreani_QA_Functions-0.0.8/Andreani_QA_Functions.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-06-09 19:19:29.000000 Andreani_QA_Functions-0.0.8/Andreani_QA_Functions.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-06-09 19:19:29.000000 Andreani_QA_Functions-0.0.8/Andreani_QA_Functions.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      303 2023-06-09 19:19:29.322748 Andreani_QA_Functions-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-01-26 19:44:24.000000 Andreani_QA_Functions-0.0.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-09 19:19:29.323846 Andreani_QA_Functions-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1140 2023-06-09 19:19:21.000000 Andreani_QA_Functions-0.0.8/setup.py
```

### Comparing `Andreani_QA_Functions-0.0.7/Andreani_QA_Functions/Functions.py` & `Andreani_QA_Functions-0.0.8/Andreani_QA_Functions/Functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # -*- coding: utf-8 -*-
 import pprint
+import datetime
 import platform
 import unittest
 import cx_Oracle
 import pymsteams
 import pyodbc
 
 import time
@@ -23,26 +24,30 @@
 import random
 import pymongo
 from pymongo.errors import ServerSelectionTimeoutError
 from pymongo.errors import ConnectionFailure
 from Andreani_QA_parameters.Parameters import Parameters
 from Andreani_QA_parameters.Encriptor import Encriptor
 
-
 ########################################################################################################################
 from cryptography.fernet import Fernet
-#XML tools
+# XML tools
 import xml.etree.ElementTree as ET
 import bz2
 
-PATH_FUNCTIONS = os.path.abspath(os.path.join(__file__, "../../../../../functions/"))
-PATH_ORIGIN = os.path.join(PATH_FUNCTIONS, 'src/environment_access.txt')
-PATH_ORIGIN_XML = os.path.join(PATH_FUNCTIONS, 'src/environment_access.xml')
-PATH_TARGET = os.path.join(PATH_FUNCTIONS, 'src/environment_access_e.txt')
+PATH_FUNCTIONS = os.path.join(Parameters.current_path, 'functions')
+PATH_ORIGIN = os.path.join(PATH_FUNCTIONS, './src/environment_access.txt')
+PATH_ORIGIN_XML = os.path.join(PATH_FUNCTIONS, './src/environment_access.xml')
+PATH_TARGET = os.path.join(PATH_FUNCTIONS, './src/environment_access_e.txt')
 ENVIROMENT_VAR = 'PYBOT_KEY'
+RED = '\033[31m'
+BLUE = '\033[34m'
+YELLOW = '\033[33m'
+GREEN = '\033[32m'
+DEFAULT = '\033[39m'
 
 
 class Functions(Parameters):
     global_date = time.strftime(Parameters.date_format)  # formato aaaa/mm/dd
     global_time = time.strftime(Parameters.time_format)  # formato 24 houras
     project_name = None
     class_name = None
@@ -52,30 +57,31 @@
     teams = None
     data_cache = {}
     data_resource = None
     path_downloads = None
     path_evidences = None
     path_files = None
     path_images = None
-    path_output = None
+    path_outputs = None
+    path_steps = None
     path_json = None
-    path_resource = None
+    path_resources = None
     path_map = None
     path_jmeter_executor = None
     path_config = None
     resource_remoto = False
     sharepoint_data_jmeter = False
-    usuario_pybot_email = Encriptor.get_password_from_xml_file_encrypted(Encriptor, "CLAVES", "id", "Email de Pybot", "USER")
+    usuario_pybot_email = Encriptor.get_password_from_xml_file_encrypted(Encriptor, "CLAVES", "id", "Email de Pybot",
+                                                                         "USER")
     email_pybot = Encriptor.get_password_from_xml_file_encrypted(Encriptor, "CLAVES", "id", "Email de Pybot", "USER")
     password_sharepoint = ""
     sharepoint_url = "https://grupologisticoandreani.sharepoint.com"
     sharepoint_site = "https://grupologisticoandreani.sharepoint.com/teams/AutomatizacinQA"
     sharepoint_doc = "Documentos compartidos/General"
 
-
     def set_proyect(self, project_name=None):
 
         """
             Description:
                 Setea variables de ambiente y rutas del proyecto.
             Args:
                 project_name: Nombre del Proyecto
@@ -86,117 +92,175 @@
                     -Ruta de Evidencias.
                     -Ruta de los Json.
                     -Ruta de las Imagenes de los json (reconocimiento por imagenes).
                     -Ruta de los Bass.
                 Si hubo un error en la configuración, imprime por consola
                 "No se pudieron detectar los datos de la ejecución".
         """
-        print(f"Plataforma {platform.system()} detectada")
+        print(f"Plataforma {platform.system()} detectada.")
         if platform.system() == "Windows":
-            Functions.set_parameters_environment("Windows")
+            self.set_parameters_environment("Windows")
         elif platform.system() == "Linux":
-            Functions.set_parameters_environment("Linux")
-
+            self.set_parameters_environment("Linux")
         if project_name is None and os.getenv('PROYECT') is None:
-            if os.path.abspath(str(self)).split(' ')[0].split('\\')[-4] == 'src': # valida en caso de que haya subcarpeta dento de tests
+            if os.path.abspath(str(self)).split(' ')[0].split('\\')[
+                -4] == 'src':  # valida en caso de que haya subcarpeta dento de tests
                 self.project_name = os.path.abspath(str(self)).split(' ')[0].split('\\')[-5]
             else:
                 self.project_name = os.path.abspath(str(self)).split(' ')[0].split('\\')[-4]
         elif os.getenv('PROYECT') is not None:
             self.project_name = os.getenv('PROYECT')
         else:
             self.project_name = project_name
-        try:
-            Functions.automatic_restore_row(self)
-            str(self).replace(" (", ".").replace(")", "")
-            instance = str(self).replace(" (", ".").replace(")", "")
-            self.class_name = instance.split(".")[-1]
-            self.test_case_name = instance.split(".")[0]
-            self.case_name = instance.split(".")[1]
-            if instance.split(".")[-2] == '__main__':
-                self.file_name = instance.split(".")[-1]
-            else:
-                self.file_name = instance.split(".")[-2]
-            if not Parameters.manual_increment:
-                Functions.automatic_increment_row(self)
-
-        except Exception as e:
-            Functions.exception_logger(e)
-            print("No se pudieron detectar los datos de la ejecución.")
-            self.file_name = self.project_name
-            self.class_name = "Sin datos"
-            self.test_case_name = "Sin datos"
-
+        self.test_case_name = self.id().split('.')[-1]
+        self.class_name = self.id().split('.')[-2]
+        self.file_name = self.id().split('.')[-3]
+        self.automatic_restore_row()
+        if not Parameters.manual_increment:
+            self.automatic_increment_row()
         if Parameters.environment == "Windows":
             self.path_downloads = f"{Parameters.current_path}\\projects\\{str(self.project_name)}\\src\\downloads"
-            self.path_evidences = f"{Parameters.current_path}\\projects\\{str(self.project_name)}\\src\\inputs"
             self.path_files = f"{Parameters.current_path}\\projects\\{str(self.project_name)}\\src\\files"
-            self.path_images = f"{Parameters.current_path}\\projects\\{str(self.project_name)}\\src\\outputs"
-            self.path_output = f"{Parameters.current_path}\\projects\\{str(self.project_name)}\\src\\outputs"
+            self.path_images = f"{Parameters.current_path}\\projects\\{str(self.project_name)}\\src\\images"
+            self.path_outputs = f"{Parameters.current_path}\\projects\\{str(self.project_name)}\\src\\outputs"
             self.path_json = f"{Parameters.current_path}\\projects\\{str(self.project_name)}\\src\\pages"
-            self.path_resource = f"{Parameters.current_path}\\projects\\{str(self.project_name)}\\src\\resources"
+            self.path_resources = f"{Parameters.current_path}\\projects\\{str(self.project_name)}\\src\\resources"
+            self.path_steps = f"{Parameters.current_path}\\projects\\{str(self.project_name)}\\src\\steps"
             self.path_config = f"{Parameters.current_path}\\projects\\{str(self.project_name)}\\config.yml"
             self.path_jmeter_executor = Parameters.path_jmeter
 
         if Parameters.environment == "Linux":
             self.path_downloads = f"{Parameters.current_path}/projects/{str(self.project_name)}/src/downloads"
-            self.path_evidences = f"{Parameters.current_path}/projects/{str(self.project_name)}/src/inputs"
             self.path_files = f"{Parameters.current_path}/projects/{str(self.project_name)}/src/files"
-            self.path_images = f"{Parameters.current_path}/projects/{str(self.project_name)}/src/outputs"
-            self.path_output = f"{Parameters.current_path}/projects/{str(self.project_name)}/src/outputs"
+            self.path_images = f"{Parameters.current_path}/projects/{str(self.project_name)}/src/images"
+            self.path_outputs = f"{Parameters.current_path}/projects/{str(self.project_name)}/src/outputs"
             self.path_json = f"{Parameters.current_path}/projects/{str(self.project_name)}/src/pages"
-            self.path_resource = f"{Parameters.current_path}/projects/{str(self.project_name)}/src/resources"
+            self.path_resources = f"{Parameters.current_path}/projects/{str(self.project_name)}/src/resources"
+            self.path_steps = f"{Parameters.current_path}/projects/{str(self.project_name)}/src/steps"
             self.path_config = f"{Parameters.current_path}/projects/{str(self.project_name)}/config.yml"
 
-        self.path_map = {"resources": self.path_resource,
-                         "evidences": self.path_evidences,
+        self.path_map = {"resources": self.path_resources,
+                         "files": self.path_files,
                          "pages": self.path_json,
-                         "outputs": self.path_images,
-                         "inputs": self.path_files,
-                         "output": self.path_output}
+                         "images": self.path_images,
+                         "downloads": self.path_downloads,
+                         "outputs": self.path_outputs,
+                         "steps": self.path_steps}
+
+        self.create_folders_framework(self.path_map)
 
         if self.resource_remoto:
-            Functions.download_file(self)
+            self.download_file()
 
         if os.environ.get("rowXLSX"):
             self.set_manual_increment(True)
             self.set_excel_row(self.get_row_excel())
             Parameters.row = os.environ.get("rowXLSX")
 
-
-        if os.environ.get("shData") == 'true':
-            self.sharepoint_data_jmeter = True
-
+        # if os.environ.get("shData") == 'true':
+        #   Parameters.sharepoint_data_jmeter = True
 
         if os.environ.get("env"):
             if str(os.environ['env']).lower() == "qa":
                 Parameters.env = "DataQa"
             if str(os.environ['env']).lower() == "prod":
                 Parameters.env = "DataProd"
             if str(os.environ['env']).lower() == "test":
                 Parameters.env = "DataTest"
             if str(os.environ['env']).lower() == "alt":
                 Parameters.env = "DataAlt"
         else:
             Parameters.env = "DataTest"
-        Functions.full_read_excel(self, None, Parameters.env)
+        self.full_read_excel(self, None, Parameters.env)
+        self.create_grid_by_sources(self.data_resource, "Datos del resource")
         return self.path_map
 
     @staticmethod
+    def create_grid_by_sources(resource: dict, message):
+
+        body = """
+            <!DOCTYPE html>
+            <html>
+            <head>
+              <meta charset="utf-8">
+              <title>Mi página web</title>
+              <style>
+                h1{
+                  color: #D71920;
+                  padding: 1%;
+                  font-family: Arial, Helvetica, sans-serif;
+                }
+
+                ul {
+                  list-style-type: disc; /* Tipo de viñeta, en este caso un círculo lleno */
+                  margin: 0;
+                  padding: 0;
+                }
+
+                li {
+                  color:#D71920;
+                  margin: 0 0 0 1em; /* Margen izquierdo para que se vea la viñeta */
+                  font-family: Arial, Helvetica, sans-serif;
+                  font-size: 15px;
+                }
+                span{
+                  color: #757575;
+                  font-size: 15px;
+                  font-family: Arial, Helvetica, sans-serif;
+
+                }
+                .container{
+                  background-color: #FFFFFF;
+                  margin: 1%;
+                  padding: 1%;
+                  border-radius: 10px;
+                  box-shadow: 0px 3px 10px #00000029;
+                }
+            </style>
+            </head>
+            <body>
+                {list}
+            </body>
+            </html>
+            """
+        if len(resource) != 0:
+            list_resources = ""
+            for item in resource.items():
+                resources_html = \
+                    f"""<div class="container">
+                        <ul>
+                            <li><b>{item[0]}: </b><span>{item[1]}</span></li>
+                        </ul>
+                    </div>"""
+
+                list_resources += resources_html
+            body = body.replace("{list}", list_resources)
+            try:
+                allure.attach(body, message, attachment_type=allure.attachment_type.HTML)
+            except Exception as e:
+                Functions.exception_logger(e)
+
+    @staticmethod
+    def create_folders_framework(mapping: dict):
+        for key in mapping.keys():
+            if not os.path.exists(mapping[key]):
+                os.makedirs(mapping[key])
+
+            archivo_init = os.path.join(mapping[key], "__init__.py")
+            open(archivo_init, 'a').close()
+
+    @staticmethod
     def get_env():
 
         """
 
             Returns: Devuelve el valor de la variable de entorno 'env' en minúsculas'
 
         """
 
-        #if Parameters.env is None or Parameters.env == "DataTest":
-         #   return "DataTest"
-
         return str(os.environ['env']).lower()
 
     @staticmethod
     def set_env(env):
 
         """
             Descripcion:
@@ -207,15 +271,14 @@
 
             Returns:
                 Funcion que configura la variable de ambiente para la lectura del resources
 
         """
         os.environ['env'] = env
 
-
     @staticmethod
     def set_parameters_environment(system):
 
         """
             Description:
                 Configura las opciones del framework en funcion del SO.
             Args:
@@ -232,16 +295,14 @@
             Args:
                 numbers_retries: Cantidad de veces que se quiere reintentar.
         """
 
         Parameters.number_retries = numbers_retries
         print(f"La cantidad de reintentos configurada es {Parameters.number_retries}.")
 
-
-
     @staticmethod
     def set_remote_resource(value):
 
         """
             Description:
                 Activar el modo para leer resources remotamente desde SharePoint de Pybot Team & qa.
             Args:
@@ -256,16 +317,15 @@
             Description:
                 Autenticarse con un usuario de SharePoint y obtener una instancia para interactuar con el content
                 del mismo.
             Returns:
                 site (Site): Instancia del SharePoint.
         """
 
-        self.password_sharepoint = Functions.get_password_from_file_encrypted(self, "Email de Pybot",
-                                                                                    self.email_pybot)
+        self.password_sharepoint = self.get_password_from_file_encrypted("Email de Pybot", self.email_pybot)
         authcookie = Office365(self.sharepoint_url,
                                username=self.email_pybot,
                                password=self.password_sharepoint).GetCookies()
         site = Site(self.sharepoint_site, version=Version.v365, authcookie=authcookie)
 
         return site
 
@@ -276,15 +336,15 @@
                 Obtener la instancia de una carpeta del SharePoint para interactuar con su content.
             Args:
                 folder_name (str): nombre de la carpeta en SharePoint Ej. Ebuyplace/src/outputs.
             Returns:
                 folder (Folder): instancia de la carpeta para interactuar con su content.
         """
 
-        auth_site = Functions.auth(self)
+        auth_site = self.auth()
 
         sharepoint_dir = '\\'.join([self.sharepoint_doc, folder_name])
         folder = auth_site.Folder(sharepoint_dir)
 
         return folder
 
     def upload_file(self, file, file_name, folder_name):
@@ -294,15 +354,15 @@
                 Subir un archivo local en SharePoint de Pybot Team & QA.
             Args:
                 file (str): Dirección local del archivo.
                 file_name (str): Nombre del archivo Ej. factura.pdf
                 folder_name (strt): Dirección donde se subirá el archivo en SharePoint Ej. Ebuyplace/src/outputs
         """
 
-        _folder = Functions.connect_folder(self, folder_name)
+        _folder = self.connect_folder(folder_name)
 
         with open(file, mode='rb') as file_obj:
             file_content = file_obj.read()
 
         _folder.upload_file(file_content, file_name)
 
     def download_file(self):
@@ -314,23 +374,24 @@
                 la estructura de carpetas, por ejemplo:
                 Para un conjunto de pruebas llamado A.py debe existir una ruta en SharPoint
                 /Ebuyplace/src/resources/A.xlxs
                 que es de donde se leerá los datos a utilizarse en las pruebas.
         """
 
         # set the folder name
-        folder_name = self.path_resource.split("\\")[-3] + "/" + self.path_resource.split("\\")[-2] + "/" + self.path_resource.split("\\")[-1] + "/"
+        folder_name = self.path_resources.split("\\")[-3] + "/" + self.path_resources.split("\\")[-2] + "/" + \
+                      self.path_resources.split("\\")[-1] + "/"
 
         # set file name
         file_name = f"{self.file_name}.xlsx"
 
         # set dowload path
-        download_path = f"{self.path_resource}\\{self.file_name}.xlsx"
+        download_path = f"{self.path_resources}\\{self.file_name}.xlsx"
 
-        _folder = Functions.connect_folder(self, folder_name)
+        _folder = self.connect_folder(folder_name)
         file = _folder.get_file(file_name)
 
         # save file
         with open(download_path, 'wb') as f:
             f.write(file)
             f.close()
 
@@ -363,31 +424,37 @@
 
         """
             Description:
                 Restaura la variable Parameters.row a 2 cuando se pasa de un archivo a.py a b.py.
         """
 
         file_name = str(self)[str(self).find("(") + 1:str(self).find(")")]
-        if Functions.get_file_name_stored() is None:
-            Functions.set_file_name_stored(file_name)
+        if self.get_file_name_stored() is None:
+            self.set_file_name_stored(file_name)
         else:
-            if file_name != Functions.get_file_name_stored():
-                Functions.set_restore_excel_row()
-                Functions.set_file_name_stored(file_name)
+            if file_name != self.get_file_name_stored():
+                self.set_restore_excel_row()
+                self.set_file_name_stored(file_name)
 
     def automatic_increment_row(self):
 
         """
             Description:
                 Incrementa Parameters.row de a cuerdo al test_id que se está ejecutando.
         """
 
         if not Parameters.manual_increment:
-            id_case = int(self.test_case_name.split('_')[1])
-            Parameters.row = id_case + 2
+            id_case = str(self.test_case_name.split('_')[1])
+            if id_case.isdigit():
+                Parameters.row = int(id_case) + 2
+            else:
+                unittest.TestCase.skipTest(self, f"No es posible realizar la ejecución del caso"
+                                                 f" '{self.test_case_name}' ya que el nombre del mismo no respeta"
+                                                 f" la siguiente convención de nombres 'test_xxx_descripcion'"
+                                                 f" siendo x un numero entero.")
 
     @staticmethod
     def get_file_name_stored():
 
         """
             Description:
                 Obtiene el parámetro file_name_stored de la configuracion.
@@ -434,14 +501,15 @@
 
         print(f"El numero del registro consultado es: {Parameters.row} .")
         return Parameters.row
 
     @staticmethod
     def set_excel_row(value: int):
         Parameters.row = value
+
     @staticmethod
     def set_manual_increment(value: bool):
         Parameters.manual_increment = value
 
     @staticmethod
     def set_increment_row():
 
@@ -477,17 +545,17 @@
             Returns:
                 Retorna el value de la cell del resource.
         """
 
         if file_name is None:
             print("El nombre del caso es : " + self.file_name)
             file_name = self.file_name
-        resource = f"{self.path_resource}\\{file_name}.xlsx"
+        resource = f"{self.path_resources}\\{file_name}.xlsx"
         if not os.path.isfile(resource):
-            resource = f"{self.path_resource}{file_name}.xlsx"
+            resource = f"{self.path_resources}{file_name}.xlsx"
             if not os.path.isfile(resource):
                 raise Exception('El resource no existe')
         wb = openpyxl.load_workbook(resource, data_only=True)
         if specific_sheet is None:
             sheet = wb["DataTest"]
         else:
             sheet = wb[specific_sheet]
@@ -533,51 +601,54 @@
             print(value)
             print(sheet)
             print(cell)
             wb.save(filename=resource)
             wb.close()
             flag = True
             print(f"El libro de excel utilizado es: {resource}")
-            if not(sheet is None):
+            if not (sheet is None):
                 print(f"Se escribio en la celda {str(cell)} de la hoja {str(sheet)} el valor: {str(value)}")
             else:
                 print(f"Se escribio en la celda {str(cell)} el valor: {str(value)}")
             print(flag)
             return flag
         except Exception as e:
             flag = False
-            Functions.exception_logger(e)
+            self.exception_logger(e)
             print("VERIFICAR: No se pudo escribir el archivo.")
             return flag
 
-    def wait(self, time_load, logger=Parameters.loggin_time, reason=None):
+    @staticmethod
+    def wait(time_load, logger=Parameters.loggin_time, reason=None):
 
         """
             Description:
                 Espera un elemento, el tiempo es dado en segundos.
             Args:
                 time_load (int): Tiempo en segundos.
                 logger: Indica si se requieren logear los mensajes de espera.
                 reason: Razón por la que se quiere esperar un elemento.
             Returns:
                 Cuando termina el tiempo de espera imprime "Esperar: Carga Finalizada ... ".
         """
-
+        actual_hour = datetime.datetime.now().time().strftime(Parameters.time_format)
         if logger:
-            print(f"Esperar: Inicia '{str(time_load)}'")
+            print(f"{Functions.color_message('YELLOW', 'AGUARDANDO:')} Inicia espera de '{str(time_load)}' "
+                  f"segundo/s a las {actual_hour}.")
         if reason is not None:
             print(reason)
         try:
             total_wait = 0
             while total_wait < time_load:
                 time.sleep(1)
                 total_wait = total_wait + 1
         finally:
+            actual_hour = datetime.datetime.now().time().strftime(Parameters.time_format)
             if logger:
-                print("Esperar: Carga Finalizada... ")
+                print(f"{Functions.color_message('YELLOW', 'AGUARDANDO:')} Finaliza espera a las {actual_hour}")
 
     # FUNCIONES BASE DE DATOS ##########################################################################################
     def set_timeout_base_sql_server(self, time_seconds):
 
         """
             Description:
                Configura el value de timeout (segundos) configurado para las conexiones a bases sqlServer.
@@ -616,20 +687,20 @@
             Returns:
                 Devuelve una variable con la conexion a la base de datos sqlServer.
         """
 
         driver = None
         conection = None
         if password is None:
-            password = Functions.use_xml_connect_to_db(server, user)
+            password = self.use_xml_connect_to_db(server, user)
         if Parameters.environment == "Linux":
             driver = "/usr/lib/libtdsodbc.so"
         if Parameters.environment == "Windows":
             driver = "{SQL Server}"
-        db_port = Functions.get_data_from_xml_encrypted(Functions, "CLAVES", "id", "Base de Pybot", "PORT")
+        db_port = self.get_data_from_xml_encrypted(Functions, "CLAVES", "id", "Base de Pybot", "PORT")
         try:
             conection = pyodbc.connect(f"Driver={driver};Server={server};PORT={db_port};Database={base};UID={user};"
                                        f"PWD={password}")
         except pyodbc.OperationalError:
             unittest.TestCase().fail("El servidor no existe o el acceso al mismo fué denegado.")
         finally:
             if conection is not None:
@@ -650,23 +721,23 @@
             Returns:
                 <class 'pyodbc.Row'>: Retorna un class 'pyodbc.Row' si la consulta y la conexión es exitosa. De lo
                  contrario imprime por consola "Se produjo un error en la base de datos."
         """
 
         cursor = None
         recordset = []
-        conn = Functions.establish_connection_sqlserver(self, server, base, user, password)
+        conn = self.establish_connection_sqlserver(self, server, base, user, password)
         try:
             cursor = conn.cursor()
             cursor.execute(query)
             for row in cursor:
                 recordset = row
 
         except Exception as e:
-            Functions.exception_logger(e)
+            self.exception_logger(e)
             print(f"Se produjo un error en la base de datos.")
 
         finally:
             cursor.close()
             conn.close()
             return recordset
 
@@ -686,24 +757,24 @@
             Returns:
                 <class 'pyodbc.Row'>: Retorna un class 'pyodbc.Row' si la consulta y la conexión es exitosa. De lo
                  contrario imprime por consola "Se produjo un error en la base de datos."
         """
 
         recordset = []
         cursor = None
-        connection = Functions.establish_connection_sqlserver(self, server, base, user, password)
+        connection = self.establish_connection_sqlserver(self, server, base, user, password)
 
         try:
             cursor = connection.cursor()
             cursor.execute(query, parameters)
             for row in cursor:
                 recordset.append(row)
 
         except Exception as e:
-            Functions.exception_logger(e)
+            self.exception_logger(e)
             print("Se produjo un error en la base de datos.")
 
         finally:
             cursor.close()
             connection.close()
             return recordset
 
@@ -721,24 +792,24 @@
                 query (str): consulta Query.
             Returns:
                 results: Lista con los resultados.
         """
 
         recordset = []
         cursor = None
-        connection = Functions.establish_connection_sqlserver(self, server, base, user, password)
+        connection = self.establish_connection_sqlserver(self, server, base, user, password)
 
         try:
             cursor = connection.cursor()
             cursor.execute(query)
             for row in cursor:
                 recordset.append(row)
 
         except Exception as e:
-            Functions.exception_logger(e)
+            self.exception_logger(e)
             print("A ocurrido un error en la base de datos.")
 
         finally:
             cursor.close()
             connection.close()
 
         return recordset
@@ -757,26 +828,26 @@
                 query (str): consulta Query.
             Returns:
                 results: Lista con diccionarios que referencian las valores con sus correspondientes columnas.
         """
 
         recordset = []
         cursor = None
-        connection = Functions.establish_connection_sqlserver(self, server, base, user, password)
+        connection = self.establish_connection_sqlserver(self, server, base, user, password)
 
         try:
             cursor = connection.cursor()
             cursor.execute(query)
             records = cursor.fetchall()
             column_names = [column[0] for column in cursor.description]
             for record in records:
                 recordset.append(dict(zip(column_names, record)))
 
         except Exception as e:
-            Functions.exception_logger(e)
+            self.exception_logger(e)
             print(f"A ocurrido un error en la base de datos. {e}")
 
         finally:
             cursor.close()
             connection.close()
 
         return recordset
@@ -791,22 +862,22 @@
                 base (str): Nombre de la base.
                 user (str): usuario.
                 password (str): Contraseña.
                 query (str): consulta Query.
         """
 
         cursor = None
-        conn = Functions.establish_connection_sqlserver(self, server, base, user, password)
+        conn = self.establish_connection_sqlserver(self, server, base, user, password)
         try:
             cursor = conn.cursor()
             cursor.execute(query)
             conn.commit()
             print("Borrado de registro en base de datos realizado exitosamente.")
         except Exception as e:
-            Functions.exception_logger(e)
+            self.exception_logger(e)
             print("Ocurrio un error en la base al intentar eliminar un registro.")
         finally:
             cursor.close()
             conn.close()
 
     def insert_row_base_sqlserver(self, server, base, user, password, query):
 
@@ -818,23 +889,24 @@
                 base (str): Nombre de la base.
                 user (str): usuario.
                 password (str): Contraseña.
                 query (str): consulta Query.
         """
 
         cursor = None
-        conn = Functions.establish_connection_sqlserver(self, server, base, user, password)
+        conn = self.establish_connection_sqlserver(self, server, base, user, password)
         try:
             cursor = conn.cursor()
             cursor.execute(query)
             conn.commit()
             print("Insertado de registro en base de datos realizado exitosamente.")
         except Exception as e:
-            Functions.exception_logger(e)
-            print("Ocurrio un error en la base al intentar un registro.")
+            self.exception_logger(e)
+            print(f"Ocurrio un error en la base al intentar un registro.")
+            print(f"QUERY ERROR: {query}")
         finally:
             cursor.close()
             conn.close()
 
     ##     ORACLE         ###
     def establish_connection_oracle_db(self, server, base, user, password):
         """
@@ -846,16 +918,16 @@
                 user: Usuario.
                 password: Contraseña.
             Returns:
                 Devuelve una variable con la conexion a la base de datos Oracle.
         """
 
         if password is None:
-            password = Functions.use_xml_connect_to_db(self, server, user)
-        connection = cx_Oracle.connect(user, password,  base, encoding="UTF-8")
+            password = self.use_xml_connect_to_db(self, server, user)
+        connection = cx_Oracle.connect(user, password, base, encoding="UTF-8")
         return connection
 
     def get_recordset_oracle_db(self, server, base, user, password, query):
 
         """
             Description:
                 Realiza conexión y consulta a base de datos con la libreria cx_Oracle. El método incluye la
@@ -868,26 +940,26 @@
                 query (str): consulta Query.
             Returns:
                 results: Lista con diccionarios que referencian las valores con sus correspondientes columnas.
         """
 
         recordset = []
         cursor = None
-        connection = Functions.establish_connection_oracle_db(self, server, base, user, password)
+        connection = self.establish_connection_oracle_db(self, server, base, user, password)
 
         try:
             cursor = connection.cursor()
             cursor.execute(query)
             records = cursor.fetchall()
             column_names = [column[0] for column in cursor.description]
             for record in records:
                 recordset.append(dict(zip(column_names, record)))
 
         except Exception as e:
-            Functions.exception_logger(e)
+            self.exception_logger(e)
             print(f"La intereacción con la DB de Oracle arrojó el siguiente error: {e}")
 
         finally:
             cursor.close()
             connection.close()
 
         return recordset
@@ -907,24 +979,24 @@
             Returns:
                 <class 'pyodbc.Row'>: Retorna un class 'pyodbc.Row' si la consulta y la conexión es exitosa. De lo
                  contrario imprime por consola "Se produjo un error en la base de datos."
         """
 
         cursor = None
         recordset = []
-        conn = Functions.establish_connection_oracle_db(self, server, base, user, password)
+        conn = self.establish_connection_oracle_db(self, server, base, user, password)
         try:
             cursor = conn.cursor()
             cursor.execute(query)
 
             for row in cursor:
                 recordset = row
 
         except Exception as e:
-            Functions.exception_logger(e)
+            self.exception_logger(e)
             print(f"La intereacción con la DB de Oracle arrojó el siguiente error: {e}")
 
         finally:
             cursor.close()
             conn.close()
             return recordset
 
@@ -940,24 +1012,24 @@
                 user (str): usuario.
                 password (str): Contraseña.
                 query (str): consulta Query.
             Returns:
                 results: Lista con los nombres de la cabecera correspondiente a la consulta.
         """
         cursor = None
-        connection = Functions.establish_connection_oracle_db(self, server, base, user, password)
+        connection = self.establish_connection_oracle_db(self, server, base, user, password)
         column_names = None
 
         try:
             cursor = connection.cursor()
             cursor.execute(query)
             column_names = [column[0] for column in cursor.description]
 
         except Exception as e:
-            Functions.exception_logger(e)
+            self.exception_logger(e)
             print(f"La intereacción con la DB de Oracle arrojó el siguiente error: {e}")
 
         finally:
             cursor.close()
             connection.close()
 
         return column_names
@@ -1215,16 +1287,14 @@
                           <p class="member"><strong class="team">Equipo Pybot</strong></p>
                           <p class="member">Joel Pino || jpino@andreani.com</p>
                           <p class="member">Federico Blanco || fblanco@andreani.com</p>
                           <p class="member">Lucas Cariboni || lcariboni@andreani.com</p>
                         </footer>'''
         return signature
 
-
-
     @staticmethod
     def create_image(image):
 
         """
             Description:
                 Crea una imágen en formato html.
             Args:
@@ -1303,33 +1373,33 @@
                 head: si el archivo contiene cabecera (por defecto esta en true).
                 file_name: el nombre del archivo que se escribira.
                 specific_sheet: si el archivo es un excel se le puede identificar el nombre de la hoja a utilizar.
         """
 
         f = None
         if file_name is None:
-            print("El nombre del archivo a escribir es : " + self.file_name)  # tomo el nombre del
+            print(f"El nombre del archivo a escribir es: {self.file_name}")  # tomo el nombre del
             file_name = self.file_name  # archivo de los datos de "inicializacion"
-            resource = self.path_output + file_name + "." + format_file
+            resource = self.path_outputs + file_name + "." + format_file
         else:
             print("El nombre del archivo a escribir es : " + file_name)
-            resource = self.path_output + file_name + "." + format_file
+            resource = self.path_outputs + file_name + "." + format_file
 
         if format_file == "xlsx":
-            Functions.convert_data_to_excel_format(collection_data, resource, head, specific_sheet)
+            self.convert_data_to_excel_format(collection_data, resource, head, specific_sheet)
             print("Se escribio el archivo correctamete.")
         else:
-            contents = Functions.convert_data_to_csv_format(collection_data, delimiter, head)
+            contents = self.convert_data_to_csv_format(collection_data, delimiter, head)
             # el archivo csv para poder escribirlo
             try:
                 f = open(resource, "w", encoding='utf8')
                 f.write(contents)
                 print("Se escribio el archivo correctamete")
             except Exception as e:
-                Functions.exception_logger(e)
+                self.exception_logger(e)
                 print("No se pudo escribir el archivo")
             finally:
                 f.close()
 
     @staticmethod
     def convert_data_to_csv_format(collection_data, delimiter, head):
 
@@ -1395,20 +1465,20 @@
                 file_name: el nombre del archivo excel que se leera (opcional)
                 specific_sheet: nombre de la hoja que se leera (opcional)
             Returns:
                 Devuelve una lista con los datos obtenidos de una fila del excel.
         """
 
         if file_name is None:
-            print("Se leera el archivo con nombre : " + self.file_name)
+            print(f"Se leera el archivo con nombre: {self.file_name}")
             file_name = self.file_name
-            resource = f"{self.path_resource}\\{file_name}.xlsx"
+            resource = f"{self.path_resources}\\{file_name}.xlsx"
             book = openpyxl.load_workbook(resource, data_only=True)
         else:
-            resource = f"{self.path_resource}\\{file_name}.xlsx"
+            resource = f"{self.path_resources}\\{file_name}.xlsx"
             book = openpyxl.load_workbook(resource, data_only=True)
 
         if specific_sheet is None:
             sheet = book["Pool Data"]
         else:
             sheet = book[specific_sheet]
         key = []
@@ -1524,15 +1594,15 @@
                 enviroment: Nombre del ambiente asociado al usuario del cual se pretende recuperar la password.
                 user: Nombre del usuario del que se pretende recuperar la password.
             Returns:
                 Devuelve la password del usuario.
         """
 
         password = None
-        key = Functions.get_enviroment_key_from_file()
+        key = self.get_enviroment_key_from_file()
         fe = Fernet(key)
 
         with open(PATH_ORIGIN, 'rb') as file:
             encrypte_data = file.read()
 
         decrypted_data = fe.decrypt(encrypte_data)
         pass_list = decrypted_data.decode('utf-8').split('\r')
@@ -1557,15 +1627,15 @@
                 father_attribute: Nombre del Tag padre.
                 attribute_to_search: Tipo de atributo que desea buscar.
                 attribute_name: Nombre del atributo que desea buscar.
                 inner_search: Nombre del tag interno del que se desea obtener el texto.
             Returns:
                 Retorna el texto interno del dato requerido.
         """
-        key = Functions.get_enviroment_key_from_file()
+        key = self.get_enviroment_key_from_file()
         fe = Fernet(key)
         return_data = None
         try:
             with open(PATH_ORIGIN_XML, 'rb') as file:
                 data = file.read()
             deencrypted_data = fe.decrypt(data)
             decompressed_data = bz2.decompress(deencrypted_data)
@@ -1577,14 +1647,15 @@
                 if element.tag == inner_search and (element.text is not None or element.text != ""
                                                     or element.text != " "):
                     return_data = element.text
         except:
             raise "Ha Ocurrido un Error en el Tiempo de Ejecución -> ERROR CODE 1523 (Functions)"
 
         return return_data
+
     @staticmethod
     def use_xml_connect_to_db(ip_db, db_user_name):
         """
             Description:
                 Busca y retorna la contraseña de la db requerida desde el xml encriptado
             Args:
                 ip_db: IP servidor a conectar.
@@ -1621,25 +1692,25 @@
                 title (str): Asunto del correo.
                 content (str): Cuerpo del correo
                 file_attach (file): Archivos adjuntos del correo.
             Returns:
                 Si el correo fue enviado con éxito retorna el estado "Enviado",
                 de lo contrario imprime por consola "El mail no pudo ser enviado" y estado "No enviado".
         """
-        content = f'{content}{Functions.footer_signature_html()}'
-        content = Functions.apply_style_css_to_block(content)
+        content = f'{content}{self.footer_signature_html()}'
+        content = self.apply_style_css_to_block(content)
         port = 25  # For starttls 587
         smtp_server = "10.20.2.41"  # "smtp.office365.com"
         sender_email = self.usuario_pybot_email
         password = ""
         if Parameters.environment != "Linux":
             port = 587
             smtp_server = "smtp.office365.com"
             sender_email = self.usuario_pybot_email
-            password = Functions.get_password_from_file_encrypted(self, "Email de Pybot", sender_email)
+            password = self.get_password_from_file_encrypted(self, "Email de Pybot", sender_email)
 
         message = MIMEMultipart("alternative")
         message['To'] = ",".join(receiver_email)
         message['Subject'] = 'No-responder: ' + title
         message.attach(MIMEText(content, 'html'))
         if file_attach is not None:
             attachment = open(file_attach, "rb")
@@ -1659,16 +1730,16 @@
                     server.starttls()
                     server.login(sender_email, password)
                 text = message.as_string()
                 server.sendmail(sender_email, receiver_email, text)
                 server.close()
                 return "Enviado"
         except Exception as e:
-            print(f'El mail no pudo ser enviado. // exception: {e}' )
-            Functions.exception_logger(e)
+            print(f'El mail no pudo ser enviado. // exception: {e}')
+            self.exception_logger(e)
             server.close()
             return "No enviado"
 
     def full_read_excel(self, file_name=None, specific_sheet=None, test_cases_name_list=None):
 
         """
             Description:
@@ -1680,29 +1751,28 @@
                 Specific_sheet = Hoja específica de trabajo.
                 test_cases_name_list = Nombre del caso de prueba.
         """
 
         if test_cases_name_list is None:
             test_cases_name_list = unittest.getTestCaseNames(self.__class__, "test")
         if file_name is None:
-            print("Se leera el archivo con nombre : " + self.file_name)
+            print(f"Se leera el resource con nombre: '{self.color_message('BLUE', f'{self.file_name}.xlsx')}'")
             file_name = self.file_name
-            resource = os.path.abspath(os.path.join(__file__, f"../../../../../projects/{self.project_name}/src/resources/{file_name}.xlsx"))
-            print(resource)
+            resource = os.path.join(self.path_resources, f"{file_name}.xlsx")
             if not os.path.isfile(resource):
                 raise Exception('El resource no existe')
             book = openpyxl.load_workbook(resource, data_only=True)
         else:
-            resource = self.path_resource + file_name + ".xlsx"
+            resource = self.path_resources + file_name + ".xlsx"
             book = openpyxl.load_workbook(resource, data_only=True)
         if specific_sheet is None:
             print("Utilizando hoja default 'DataTest'")
             sheet = book["DataTest"]
         else:
-            print(f"Utilizando la hoja: '{specific_sheet}'")
+            print(f"Utilizando la hoja: '{self.color_message('BLUE', specific_sheet)}'")
             sheet = book[specific_sheet]
 
         records = list(sheet.values)  # pool de data completo
         headers = list(records.pop(0))  # solo datos del header
         long_header = len(headers)
         for header_value in range(0, long_header):
             if headers[header_value] is None:
@@ -1745,16 +1815,16 @@
         data_global_resource = [dict(zip(headers, row)) for row in records]
 
         try:
             # unificación de nombres test cases y data_global_resource
             if not Parameters.manual_increment:
                 self.data_resource = dict(zip(test_cases_name_list, data_global_resource))
             else:
-                self.data_resource = data_global_resource[int(Parameters.row)-1]
-                print(f"Resource caso: {self.test_case_name}")
+                self.data_resource = data_global_resource[int(Parameters.row) - 1]
+                print(f"El resource correra con el caso: {self.test_case_name}")
                 pprint.pprint(self.data_resource)
                 print("============================================")
                 return None
         except KeyError:
             print(f"Error: A cada row del archivo {self.file_name}.xlsx le corresponde un caso")
             unittest.TestCase().skipTest(f"Error: A cada row del archivo {self.file_name}.xlsx "
                                          f"le corresponde un caso")
@@ -1762,17 +1832,18 @@
         try:
             self.data_resource = self.data_resource[self.test_case_name]
         except KeyError:
             print(f"Error: A cada row del archivo {self.file_name}.xlsx le corresponde a un caso"
                   f"Acción: SkipTest")
             unittest.TestCase().skipTest(f"Error: A cada row del archivo {self.file_name}.xlsx "
                                          f"le corresponde a un caso")
-        print(f"Resource caso: {self.test_case_name}")
+        print(f"El resource correra con el caso: '{self.color_message('BLUE', self.test_case_name)}'")
+        print("==================Inicio Resource==================")
         pprint.pprint(self.data_resource)
-        print("============================================")
+        print("===================Fin Resource====================")
 
     def get_random(self, min_range, max_range):
 
         """
             Description:
                 Obtiene un número aleatorio del rango especificado.
             Args:
@@ -1836,7 +1907,48 @@
             Args:
                 exception: Excepción producida durante el tiempo de ejecución.
         """
 
         if Parameters.loggin_exceptions:
             print(exception)
 
+    @staticmethod
+    def set_exception_loggin(value: bool):
+
+        """
+
+        Description:
+            Configura el logeo de las excepciones
+
+        Args:
+            value: true o false
+
+        """
+
+        Parameters.loggin_exceptions = value
+
+    @staticmethod
+    def color_message(color, message):
+        """
+            Description: Colorea el string del color indicado de entre una lista de colores.
+
+            Args:
+                color: puede ser de color red, blue, yellow o green.
+                message: string a colorear.
+
+            Returns:
+                string coloreado o string por default
+
+        """
+        if Parameters.enviroment_confguration != "Server":
+            if color.upper() == "RED":
+                return f"{RED}{message}{DEFAULT}"
+            elif color.upper() == "BLUE":
+                return f"{BLUE}{message}{DEFAULT}"
+            elif color.upper() == "YELLOW":
+                return f"{YELLOW}{message}{DEFAULT}"
+            elif color.upper() == "GREEN":
+                return f"{GREEN}{message}{DEFAULT}"
+            else:
+                return f"{DEFAULT}{message}{DEFAULT}"
+        else:
+            return message
```

### Comparing `Andreani_QA_Functions-0.0.7/setup.py` & `Andreani_QA_Functions-0.0.8/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '0.0.7'
+VERSION = '0.0.8'
 PACKAGE_NAME = 'Andreani_QA_Functions'  # Debe coincidir con el nombre de la carpeta
-AUTHOR = 'Andreani_QA_Automation_Test'
+AUTHOR = 'AndreaniTesting'
 AUTHOR_EMAIL = 'user_appglatest@andreani.com'
 URL = ''
 
 LICENSE = 'MIT'  # Tipo de licencia
 DESCRIPTION = 'Functions para ejecución de casos automatizados'  # Descripción corta
 LONG_DESCRIPTION = ""  # Referencia al documento README con una descripción más elaborada
 LONG_DESC_TYPE = "text/markdown"
 
 # Paquetes necesarios para que funcione la libreía. Se instalarán a la vez si no lo tuvieras ya instalado
 INSTALL_REQUIRES = [
-    'cx_Oracle', 'pymsteams', 'pyodbc', 'openpyxl', 'pymongo', 'shareplum', 'Andreani-QA-Parameters'
+    'cx_Oracle', 'pymsteams', 'pyodbc', 'openpyxl', 'smtplib', 'pymongo', 'shareplum'
 ]
 
 setup(
     name=PACKAGE_NAME,
     version=VERSION,
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
```

