# Comparing `tmp/Andreani_QA_Selenium-0.0.1.tar.gz` & `tmp/Andreani_QA_Selenium-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Andreani_QA_Selenium-0.0.1.tar", last modified: Wed Feb 15 15:59:48 2023, max compression
+gzip compressed data, was "Andreani_QA_Selenium-0.0.2.tar", last modified: Fri Jun  9 19:27:32 2023, max compression
```

## Comparing `Andreani_QA_Selenium-0.0.1.tar` & `Andreani_QA_Selenium-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-02-15 15:59:48.843042 Andreani_QA_Selenium-0.0.1/
-drwxrwxrwx   0        0        0        0 2023-02-15 15:59:48.830047 Andreani_QA_Selenium-0.0.1/Andreani_QA_Selenium/
--rw-rw-rw-   0        0        0    96776 2023-02-13 17:50:35.000000 Andreani_QA_Selenium-0.0.1/Andreani_QA_Selenium/Selenium.py
--rw-rw-rw-   0        0        0       33 2023-02-13 17:35:28.000000 Andreani_QA_Selenium-0.0.1/Andreani_QA_Selenium/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-15 15:59:48.840021 Andreani_QA_Selenium-0.0.1/Andreani_QA_Selenium.egg-info/
--rw-rw-rw-   0        0        0      325 2023-02-15 15:59:48.000000 Andreani_QA_Selenium-0.0.1/Andreani_QA_Selenium.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      303 2023-02-15 15:59:48.000000 Andreani_QA_Selenium-0.0.1/Andreani_QA_Selenium.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-15 15:59:48.000000 Andreani_QA_Selenium-0.0.1/Andreani_QA_Selenium.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      152 2023-02-15 15:59:48.000000 Andreani_QA_Selenium-0.0.1/Andreani_QA_Selenium.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-02-15 15:59:48.000000 Andreani_QA_Selenium-0.0.1/Andreani_QA_Selenium.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      325 2023-02-15 15:59:48.842014 Andreani_QA_Selenium-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-01-26 19:44:24.000000 Andreani_QA_Selenium-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-02-15 15:59:48.843042 Andreani_QA_Selenium-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1263 2023-02-15 15:59:02.000000 Andreani_QA_Selenium-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 19:27:32.368440 Andreani_QA_Selenium-0.0.2/
+drwxrwxrwx   0        0        0        0 2023-06-09 19:27:32.353432 Andreani_QA_Selenium-0.0.2/Andreani_QA_Selenium/
+-rw-rw-rw-   0        0        0    96639 2023-06-08 13:48:30.000000 Andreani_QA_Selenium-0.0.2/Andreani_QA_Selenium/Selenium.py
+-rw-rw-rw-   0        0        0       33 2023-02-13 17:35:28.000000 Andreani_QA_Selenium-0.0.2/Andreani_QA_Selenium/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 19:27:32.365992 Andreani_QA_Selenium-0.0.2/Andreani_QA_Selenium.egg-info/
+-rw-rw-rw-   0        0        0      310 2023-06-09 19:27:32.000000 Andreani_QA_Selenium-0.0.2/Andreani_QA_Selenium.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      303 2023-06-09 19:27:32.000000 Andreani_QA_Selenium-0.0.2/Andreani_QA_Selenium.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 19:27:32.000000 Andreani_QA_Selenium-0.0.2/Andreani_QA_Selenium.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      152 2023-06-09 19:27:32.000000 Andreani_QA_Selenium-0.0.2/Andreani_QA_Selenium.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-06-09 19:27:32.000000 Andreani_QA_Selenium-0.0.2/Andreani_QA_Selenium.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      310 2023-06-09 19:27:32.367425 Andreani_QA_Selenium-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-01-26 19:44:24.000000 Andreani_QA_Selenium-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-09 19:27:32.368440 Andreani_QA_Selenium-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1248 2023-06-09 19:27:22.000000 Andreani_QA_Selenium-0.0.2/setup.py
```

### Comparing `Andreani_QA_Selenium-0.0.1/Andreani_QA_Selenium/Selenium.py` & `Andreani_QA_Selenium-0.0.2/Andreani_QA_Selenium/Selenium.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,67 +1,65 @@
 # -*- coding: utf-8 -*-
 import datetime
 import os
 import platform
 import pprint
 import random
-import re
 import string
 import time
 import allure
 import cx_Oracle
 import json
 import unittest
 import requests
 from selenium import webdriver
 from selenium.common.exceptions import NoSuchElementException, NoAlertPresentException, NoSuchWindowException, \
     TimeoutException, StaleElementReferenceException, ElementClickInterceptedException, \
     ElementNotInteractableException, WebDriverException, UnexpectedAlertPresentException
 from selenium.webdriver.chrome.service import Service
-from selenium.webdriver.chrome.options import Options as ChromeOptions
 from selenium.webdriver.common.action_chains import ActionChains
 from selenium.webdriver.common.by import By
 from selenium.webdriver.common.keys import Keys
 from selenium.webdriver.firefox.options import Options as FirefoxOptions
 from selenium.webdriver.ie.options import Options as IeOptions
 from selenium.webdriver.remote.webdriver import WebElement
 from selenium.webdriver.support import expected_conditions as ec
 from selenium.webdriver.support.ui import Select
 from selenium.webdriver.support.ui import WebDriverWait
 from webdriver_manager.chrome import ChromeDriverManager
 from webdriver_manager.firefox import GeckoDriverManager
 from webdriver_manager.microsoft import IEDriverManager
-import Andreani_QA_parameters.Parameters as Parameters
-import Andreani_QA_Functions.Functions as GenericFunctions
+from Andreani_QA_parameters.Parameters import Parameters
+from Andreani_QA_Functions.Functions import Functions
 
-#port checker
-from socket import *
 if platform.system() == "Windows":
     from win32com.client import Dispatch
     from functions.Debugger import Debugger
 
 
-class Functions(GenericFunctions, Parameters):
+class Selenium(Functions, Parameters):
     windows = {}
     driver = None
     value_to_find = None
     get_locator_type = None
     number_windows = None
     exception = None
     json_strings = None
     complete_json_path = None
     message_container = None
-    global_date = time.strftime(Parameters.Parameters.date_format)  # formato dd/mm/aaaa
-    global_time = time.strftime(Parameters.Parameters.time_format)  # formato 24 houras
+    message_error = None
+    json_on_loaded = None
+    global_date = time.strftime(
+        Parameters.date_format)  # formato dd/mm/aaaa    global_time = time.strftime(Parameters.time_format)  # formato 24 houras
     lista_pasos = []
     lista_descripcion_pasos = []
     driver_port_status = False
 
     # INICIALIZA LOS DRIVER Y LOS CONFIGURA
-    def open_browser(self, url=None, browser=Parameters.Parameters.browser, options_headless=Parameters.Parameters.headless,
+    def open_browser(self, url=None, browser=Parameters.browser, options_headless=Parameters.headless,
                      download_path=None):
 
         """
             Description:
                 Inicializa el navegador con las configuraciones definidas por el ambiente.
             Args:
                 url: Url del Proyecto.
@@ -70,121 +68,110 @@
                 download_path: Ruta a la carpeta de descargas.
             Returns:
                 Retorna el driver e imprime por consola:
                     -El directorio base
                     -El navegador utilizado
         """
 
-        print(f"Directorio Base: {Parameters.Parameters.current_path}")
-        print(f"Iniciando el navegador {browser}.")
+        print(f"Directorio Base: {Parameters.current_path}")
+        print(f"{self.color_message('YELLOW', 'AGUARDANDO:')} Inicio del navegador "
+              f"'{self.color_message('BLUE', browser)}'.")
         options = None
         if browser == "CHROME":
             options = webdriver.ChromeOptions()
             if download_path is None:
                 download_default = {"download.default_directory": self.path_downloads}
                 options.add_experimental_option("prefs", download_default)
             else:
                 options.add_experimental_option("prefs", {"download.default_directory": download_path})
         if browser == "FIREFOX":
             options = FirefoxOptions()
         if browser == "IE":
             options = IeOptions()
-        #options.add_argument("--profile-directory=Default")
-        #options.add_argument("--user-data-dir=C:/Temp/ChromeProfile")
         options.add_argument("--no-sandbox")
         options.add_argument("--window-size=1920,1080")
         options.add_argument('--disable-dev-shm-usage')
         options.add_argument("--ignore-certificate-errors")
         options.add_argument("--incognito")
         options.add_argument("--enable-automation")
         options.add_argument("--disable-extensions")
         options.add_argument("--dns-prefetch-disable")
         options.add_argument("--verbose")
         options.add_argument("--disable-popup-blocking")
         options.add_argument("--proxy-server='direct://'")
         options.add_argument("--proxy-bypass-list=*")
         options.add_argument("--disable-gpu") if os.name == "nt" else None
-        if Parameters.Parameters.environment == "Linux":
+        if Parameters.environment == "Linux":
             options.add_argument("--headless")
+            self.set_exception_loggin(True)
+            self.set_mode_debug(False)
             if browser == "CHROME":
                 services = Service(r'/usr/bin/chromedriver')
                 self.driver = webdriver.Chrome(service=services, options=options)
-                self.set_mode_debug(False)
                 self.initialize_browser(url)
                 self.driver.maximize_window()
-        if Parameters.Parameters.environment == "Windows":
-            if options_headless or Parameters.Parameters.enviroment_confguration == "Server":
+
+        if Parameters.environment == "Windows":
+            if options_headless or Parameters.enviroment_confguration == "Server":
                 options.add_argument("--headless")
-                self.select_browser(browser, options)
-                self.initialize_browser(url)
-                self.set_highlight(False)
+                Selenium.set_exception_loggin(True)
+                Selenium.select_browser(self, browser, options)
+                Selenium.initialize_browser(self, url)
+                Selenium.set_highlight(False)
             else:
-                options.add_argument(f"--remote-debugging-port={Functions.available_port()}")  # que es esto?
+                options.add_argument(f"--remote-debugging-port={self.available_port()}")
                 self.set_mode_debug()
                 self.select_browser(browser, options)
                 self.initialize_browser(url)
                 self.driver.maximize_window()
         return self.driver
 
     def initialize_browser(self, url):
-
         """
-            Description:
-                Inicia el navegador configurado y navega hacia la url.
-            Args:
-                url: Url destino.
+        Description:
+            Inicia el navegador configurado y navega hacia la url.
+        Args:
+            url: Url destino.
         """
-
         self.driver.implicitly_wait(10)
         try:
             self.driver.get(url)
             self.windows = {'Principal': self.driver.window_handles[0]}
-
         except WebDriverException:
-            Functions.tear_down(self)
-            unittest.TestCase().fail(f"--WebDriverException--"
-                                     f" No se ha podido establecer una conexion con el ambiente de pruebas '{url}'.")
+            Selenium.tear_down(self)
+            unittest.TestCase().fail(f"--WebDriverException--No se ha podido establecer una "
+                                     f"conexión con el ambiente de pruebas {url}.")
 
     def select_browser(self, browser, options):
-
         """
             Description:
                 Permite configurar el navegador que se utilizará en la prueba.
             Args:
                 browser: Nombre del navegador.
                 options: Argumentos opcionales del navegador.
         """
-        driver_download_path = os.path.abspath(os.path.join(Parameters.Parameters.current_path, "drivers"))
+        driver_download_path = os.path.abspath(os.path.join(Parameters.current_path, "drivers"))
         try:
             if browser == "CHROME":
-                version = Functions.get_version_driver_for_browser(browser)
+                version = self.get_version_driver_for_browser(browser)
                 services = Service(ChromeDriverManager(path=driver_download_path, version=version).install())
                 self.driver = webdriver.Chrome(service=services, options=options)
             elif browser == "FIREFOX":
                 services = Service(executable_path=GeckoDriverManager(path=driver_download_path).install(),
                                    log_path=None)
                 self.driver = webdriver.Firefox(service=services, options=options)
             elif browser == "IE":
                 services = IEDriverManager(path=driver_download_path).install()
                 self.driver = webdriver.Ie(services)
 
         except WebDriverException as e:
-            print(f"Ah ocurrido un problema. {e}")
-            GenericFunctions.Functions.exception_logger(e)
-            Functions.tear_down(self)
+            Functions.exception_logger(e)
+            self.tear_down()
             unittest.TestCase().skipTest(f"El web driver no esta disponible para esta prueba. {e}")
 
-        """
-        except Exception as e:
-            print(f"Ah ocurrido un problema.")
-            GenericFunctions.Functions.exception_logger(e)
-            Functions.tear_down(self)
-            unittest.TestCase().skipTest(f"El web driver no esta disponible para esta prueba. {e}")
-        """
-
     @staticmethod
     def get_version_driver_for_browser(browser):
 
         """
             Description:
                 Detecta la versión del navegador que se está utilizando y descarga la versión del
                 driver correspondiente.
@@ -207,80 +194,122 @@
                      rf"C:\Users\{os.getlogin()}\AppData\Local\Google\Chrome\Application\chrome.exe"]
 
         for filename in paths:
             try:
                 version = parser.GetFileVersion(filename)
                 break
             except Exception as e:
-                GenericFunctions.Functions.exception_logger(e)
+                Functions.exception_logger(e)
 
         if version == "":
             return version
 
         if browser == "CHROME":
             version = f"{version.split('.')[0]}.{version.split('.')[1]}.{version.split('.')[2]}"
             response = requests.get(f"https://chromedriver.storage.googleapis.com/LATEST_RELEASE_{version}")
             version = response.text
 
         return version
 
-    @staticmethod
-    def get_environment():
-
-        """
-            Description:
-                Devuelve el environment (Sistema operativo) en el que se está corriendo la prueba.
-        """
-
-        return Parameters.Parameters.environment
-
     def tear_down(self):
 
         """
             Descripcion:
                 Finaliza la ejecución cerrando el Web Driver.
         """
-
+        Selenium.create_grid_by_sources(self.data_cache, "Datos del cache")
         try:
             if self.data_cache not in ([], {}):
-                print("Se utilizaron las siguientes variables...")
+                print("====================Inicio Cache===================")
                 pprint.pprint(self.data_cache)
+                print("=====================Fin Cache=====================")
+            print(f"{Functions.color_message('YELLOW', 'AGUARDANDO:')} Se cerrará el web driver.")
             self.driver.quit()
-            print("Se cerrará el DRIVER.")
-            #############################################
 
         except Exception as e:
-            GenericFunctions.Functions.exception_logger(e)
+            Functions.exception_logger(e)
 
         finally:
-            print(f"Finaliza la ejecución.")
+            print(f"{Functions.color_message('GREEN', 'REALIZADO:')} Finaliza la ejecución.")
+
+    @staticmethod
+    def create_grid_by_sources(resource: dict, message):
+
+        body = """
+                <!DOCTYPE html>
+                <html>
+                <head>
+                  <meta charset="utf-8">
+                  <title>Mi página web</title>
+                  <style>
+                    h1{
+                      color: #D71920;
+                      padding: 1%;
+                      font-family: Arial, Helvetica, sans-serif;
+                    }
+
+                    ul {
+                      list-style-type: disc; /* Tipo de viñeta, en este caso un círculo lleno */
+                      margin: 0;
+                      padding: 0;
+                    }
+
+                    li {
+                      color:#D71920;
+                      margin: 0 0 0 1em; /* Margen izquierdo para que se vea la viñeta */
+                      font-family: Arial, Helvetica, sans-serif;
+                      font-size: 15px;
+                    }
+                    span{
+                      color: #757575;
+                      font-size: 15px;
+                      font-family: Arial, Helvetica, sans-serif;
+
+                    }
+                    .container{
+                      background-color: #FFFFFF;
+                      margin: 1%;
+                      padding: 1%;
+                      border-radius: 10px;
+                      box-shadow: 0px 3px 10px #00000029;
+                    }
+                </style>
+                </head>
+                <body>
+                    {list}
+                </body>
+                </html>
+                """
+        if len(resource) != 0:
+            list_resources = ""
+            for item in resource.items():
+                resources_html = \
+                    f"""<div class="container">
+                            <ul>
+                                <li><b>{item[0]}: </b><span>{item[1]}</span></li>
+                            </ul>
+                        </div>"""
+
+                list_resources += resources_html
+            body = body.replace("{list}", list_resources)
+            try:
+                allure.attach(body, message, attachment_type=allure.attachment_type.HTML)
+            except Exception as e:
+                Selenium.exception_logger(e)
 
     def refresh(self):
 
         """
             Description:
                 Actualiza la página web.
         """
 
         self.driver.refresh()
         self.page_has_loaded()
 
-    @staticmethod
-    def set_browser(browser):
-
-        """
-            Description:
-                Setea el navegador por defecto.
-            Args:
-                browser (str): Navegador.
-        """
-
-        Parameters.browser = browser
-        print(f"El navegador seleccionado es: {str(Parameters.Parameters.browser)}.")
-
     def get_proyect_name(self):
 
         """
             Description:
                 Obtiene el nombre del proyecto en contexto.
             Returns:
                 Retorna el nombre del proyecto en contexto.
@@ -297,44 +326,55 @@
                 Obtiene la url actual de la pestaña activa.
             Returns:
                 Url (str): La url de la pestaña activa.
         """
 
         return self.driver.current_url
 
-    def locator_element(self, type_locator, indentify):
+    def locator_element(self, type_locator, indentify, entity=None):
 
         """
             Description:
                 Localiza un elemento utilizando el tipo de identificador indicado como parámetro.
             Args:
                 type_locator: Tipo de identificador.
                 indentify: Identificador.
+                entity: Entidad con la que se genera el elemento web.
             Returns:
                 Si el elemento fue encontrado imprime "Esperar_Elemento: Se visualizó el elemento " + XPATH",
                 en caso contrario imprime "No se pudo interactuar con el elemento", XPATH".
         """
 
         find_element = False
-        elements = ""
+        elements = None
         try:
             elements = self.driver.find_element(type_locator, indentify)
             print(f"Se interactuo con el elemento {indentify}")
+            print(f"{self.color_message('GREEN', 'REALIZADO:')} Se detecto el elemento web "
+                  f"'{self.color_message('BLUE', entity)}' utilizando el "
+                  f"identificador {type_locator} apuntando a '{indentify}'")
             find_element = True
 
         except NoSuchElementException:
             self.exception = "NoSuchElementException"
-            print(f"No se pudo interactuar con el elemento: {indentify}")
+            print(f"No se pudo encontrar el elemento web '{self.color_message('BLUE', entity)}'"
+                  f" utilizando el identificador {type_locator} apuntando a '{indentify}'")
+            self.message_error = f"No se pudo encontrar el elemento web '{entity}' utilizando el identificador " \
+                                 f"{type_locator} apuntando a '{indentify}'"
 
         except TimeoutException:
             self.exception = "TimeoutException"
-            print(f"No se pudo cargar el elemento en el DOM agotando el tiempo de espera: {indentify}")
-
+            print(f"Se agoto el tiempo de busqueda intentando encontrar el elemento web "
+                  f"'{self.color_message('BLUE', entity)}' utilizando el identificador"
+                  f" {type_locator} apuntando a '{indentify}'")
+            self.message_error = f"Se agoto el tiempo de busqueda intentando encontrar el elemento web '{entity}'" \
+                                 f" utilizando el identificador " \
+                                 f"{type_locator} apuntando a '{indentify}'"
         except Exception as e:
-            GenericFunctions.Functions.exception_logger(e)
+            Functions.exception_logger(e)
             print(f"Ha ocurrido un error inesperado en tiempo de ejecución.")
         self.lista_descripcion_pasos.append(indentify)
         return elements, find_element
 
     def highlight(self, element: WebElement):
 
         """
@@ -354,19 +394,19 @@
                                                element, highlight_style)
                     time.sleep(0.1)
                     self.driver.execute_script("arguments[0].setAttribute('style', arguments[1]);",
                                                element, original_style)
                     time.sleep(0.1)
 
                 except Exception as e:
-                    GenericFunctions.Functions.exception_logger(e)
+                    Functions.exception_logger(e)
                     print(f"Se encontro el elemento pero no puede ser señalado.")
 
         except Exception as e:
-            GenericFunctions.Functions.exception_logger(e)
+            Functions.exception_logger(e)
             print(f"No se pudo señalar el elemento.")
 
     def capture_element(self, entity, variable_x=None, variable_y=None):
 
         """
             Description:
                 Captura en pantalla la entidad pasada como parámetro.
@@ -376,65 +416,57 @@
                 variable_y: Variable y para parametrizar un elemento JSON.
             Returns:
                 Si la entidad se encuentra correctamente se devuelve el elemento y se imprime "Última screenshot
                 antes de finalizar la ejecución", caso contrario lanza la excepción.
         """
 
         element = None
-        Functions.page_has_loaded(self)
-        get_entity = Functions.get_entity(self, entity)
+        self.page_has_loaded()
+        get_entity = self.get_entity(entity)
         if get_entity is None:
             print("No se encontro el value en el Json definido.")
         else:
             if variable_x is not None:
                 self.value_to_find = self.value_to_find.replace("IndiceX", variable_x)
             if variable_y is not None:
                 self.value_to_find = self.value_to_find.replace("IndiceY", variable_y)
 
         find_element = False
-        for intentos in range(Parameters.Parameters.number_retries):
+        for intentos in range(Parameters.number_retries):
             if self.get_locator_type.lower() == "xpath":
-                element, find_element = Functions.locator_element(self, By.XPATH, self.value_to_find)
+                element, find_element = self.locator_element(By.XPATH, self.value_to_find)
 
             elif self.get_locator_type.lower() == "id":
-                element, find_element = Functions.locator_element(self, By.ID, self.value_to_find)
+                element, find_element = self.locator_element(By.ID, self.value_to_find)
 
             elif self.get_locator_type.lower() == "name":
-                element, find_element = Functions.locator_element(self, By.NAME, self.value_to_find)
+                element, find_element = self.locator_element(By.NAME, self.value_to_find)
             else:
                 print("El tipo de entidad del objeto no es valido para Selenium Framework.")
                 unittest.TestCase().fail(f"--JsonErrorIdentity-- El tipo de entidad del objeto {entity} no es valido.")
 
             if find_element:
                 unittest.TestCase().assertTrue(find_element, f"El elemento {entity} se visualiza en pantalla.")
-                if Parameters.Parameters.highlight:
-                    Functions.highlight(self, element)
+                if Parameters.highlight:
+                    self.highlight(element)
                 else:
-                    Functions.wait(self, Parameters.Parameters.time_between_retries)
+                    self.wait(self, Parameters.time_between_retries)
                 break
-            Functions.wait(self, Parameters.Parameters.time_between_retries)
+            self.wait(self, Parameters.time_between_retries)
 
         if not find_element:
-            if Functions.get_mode_execution() and not Functions.get_mode_browser():
-                # captura
-                self.image_for_debugger_report()
-                self.steps_case = ""
-                for i in range(len(self.lista_pasos)):
-                    self.steps_case += f"* {self.lista_pasos[i]}: {self.lista_descripcion_pasos[i]}\n"
-                status_code_returned = Functions.debugger(self, entity)
-                if status_code_returned == 1:  # retry / refab
-                    self.set_retry(3)
-                    return self.capture_element(entity)
-                if status_code_returned == 2:  # quit
-                    return element
-                if status_code_returned == 3:  # create Jira report
-                    return element
-                if status_code_returned == 4:  # reporter existente
-                    self.set_retry(1)
-            Functions.screenshot(self, "Ultima screenshot antes de finalizar la ejecución")
+            self.image_for_debugger_report()
+            self.steps_case = ""
+            for i in range(len(self.lista_pasos)):
+                self.steps_case += f"* {self.lista_pasos[i]}: {self.lista_descripcion_pasos[i]}\n"
+            status_code_returned = self.debugger(entity)
+            if status_code_returned == 1:  # retry / refab
+                self.set_retry(3)
+                return Selenium.capture_element(self, entity)
+            self.screenshot("Ultima screenshot antes de finalizar la ejecución")
             unittest.TestCase().fail(f"--{self.exception}-- El objeto {entity} no se visualiza en pantalla.")
 
         return element
 
     def get_element(self, entity: object, variable_y: object = None, variable_x: object = None):
 
         """
@@ -445,313 +477,103 @@
                 variable_y: Variable x para parametrizar un elemento JSON.
                 variable_x: Variable y para parametrizar un elemento JSON.
             Returns:
                 Si la entidad fue encontrada retorna el elemento, en caso contrario imprime
                 "No se encontro el value en el Json definido".
         """
 
-        element = Functions.capture_element(self, entity, variable_y=variable_y, variable_x=variable_x)
-
-        class Element(Functions):
-
-            def __init__(self, instance, context_element: WebElement, driver, json_value, json_get_indicator):
-                self.retry = 0
-                self.element = context_element
-                self.driver = driver
-                self.instance = instance
-                self.json_ValueToFind = json_value
-                self.json_GetFieldBy = json_get_indicator
-                self.menssage = ""
-                self.exception = None
-
-            def click(self):
-                self.execute_action("click")
-
-            def click_js(self):
-                self.execute_action("click_js")
-
-            def double_click(self):
-                self.execute_action("double_click")
-
-            def send_keys(self, value):
-                self.execute_action("send_keys", value)
-
-            def send_special_key(self, value):
-                self.execute_action("send_special_key", value)
-
-            @property
-            def text(self):
-                return self.execute_action("text")
-
-            def clear(self):
-                self.execute_action("clear")
-
-            def clear_js(self):
-                self.execute_action("clear_js")
-
-            def is_enabled(self):
-                return self.execute_action("is_enabled")
-
-            def is_selected(self, value):
-                return self.execute_action("is_selected", value)
-
-            def is_displayed(self):
-                return self.execute_action("is_displayed")
-
-            def get_property(self, value):
-                return self.execute_action("get_property", value)
-
-            def get_attribute(self, value):
-                return self.execute_action("get_attribute", value)
-
-            def capture(self):
-                return self.execute_action("capture")
-
-            def select_option_by_text(self, value):
-                return self.execute_action("select_option_by_text", value)
-
-            def select_option_by_value(self, value):
-                return self.execute_action("select_option_by_value", value)
-
-            def select_option_by_index(self, value):
-                return self.execute_action("select_option_by_index", value)
-
-            def get_all_values_to_select(self):
-                return self.execute_action("get_all_values_to_select")
-
-            def select_action(self, action, value=None):
-                self.menssage = ""
-
-                if action == "click":
-                    self.menssage = "realizar click"
-                    return self.element.click()
-
-                if action == "click_js":
-                    self.menssage = "realizar click"
-                    self.driver.execute_script("arguments[0].click();", self.element)
-
-                if action == "double_click":
-                    self.menssage = "realizar doble click"
-                    return Functions.double_click_element(self, self.element)
-
-                if action == "send_keys":
-                    self.menssage = "escribir en el campo"
-                    return self.element.send_keys(value)
-
-                if action == "send_special_key":
-                    self.menssage = f"presionar la tecla {value} en el objetivo"
-                    key = value.upper()
-                    if key == 'ENTER':
-                        self.element.send_keys(Keys.ENTER)
-                    if key == 'TAB':
-                        self.element.send_keys(Keys.TAB)
-                    if key == 'ESPACIO':
-                        self.element.send_keys(Keys.SPACE)
-                    if key == 'ESCAPE':
-                        self.element.send_keys(Keys.ESCAPE)
-                    if key == 'RETROCESO':
-                        self.element.send_keys(Keys.BACKSPACE)
-                    if key == 'SUPRIMIR':
-                        self.element.send_keys(Keys.DELETE)
-                    if key == "ABAJO":
-                        self.element.send_keys(Keys.ARROW_DOWN)
-                    if key == "F3":
-                        self.element.send_keys(Keys.F3)
-                    if key == "F4":
-                        self.element.send_keys(Keys.F4)
-
-                if action == "text":
-                    self.menssage = "obtener texto del campo"
-                    return self.element.text
-
-                if action == "clear":
-                    self.menssage = "limpiar el texto del campo"
-                    return self.element.clear()
-
-                if action == "clear_js":
-                    self.menssage = "limpiar campo"
-                    self.driver.execute_script('arguments[0].value="";', self.element)
-
-                if action == "is_enabled":
-                    self.menssage = "verificar el estado del objeto"
-                    return self.element.is_enabled()
-
-                if action == "is_selected":
-                    self.menssage = "verificar si el objeto es seleccionable"
-                    return self.element.is_selected()
-
-                if action == "is_displayed":
-                    self.menssage = "visualizar el objeto"
-                    return self.element.is_displayed()
-
-                if action == "get_property":
-                    self.menssage = "obtener las propiedades del objeto"
-                    return self.element.get_property(value)
-
-                if action == "get_attribute":
-                    self.menssage = "obtener los atributos del objeto"
-                    return self.element.get_attribute(value)
-
-                if action == "capture":
-                    self.menssage = "capturar pantalla"
-                    Functions.highlight(self, self.element)
-                    Functions.screenshot(self, f"Se visualiza el objeto {entity}")
-                    return
-
-                if action == "select_option_by_value":
-                    self.menssage = f"seleccionar value {value} de la lista"
-                    Select(self.element).select_by_value(value)
-
-                if action == "select_option_by_text":
-                    self.menssage = f"seleccionar value {value} de la lista"
-                    Select(self.element).select_by_visible_text(value)
-
-                if action == "select_option_by_index":
-                    self.menssage = f"seleccionar value {value} de la lista"
-                    Select(self.element).select_by_index(value)
-
-                if action == "get_all_values_to_select":
-                    list_value = []
-                    self.menssage = f"obtener todos los valores de la lista {self.element}"
-                    print(Select(self.element).options)
-                    for option_value in Select(self.element).options:
-                        list_value.append(option_value.get_attribute("value"))
-                    return list_value
-
-            def execute_action(self, action, value=None):
-                out = None
-                self.menssage = ""
-                while self.retry <= Parameters.Parameters.number_retries:
-                    if self.retry < Parameters.Parameters.number_retries:
-                        try:
-                            out = self.select_action(action, value)
-                            break
-
-                        except StaleElementReferenceException:
-                            self.retry += 1
-                            self.exception = "StaleElementReferenceException"
-                            self.menssage = f'--{self.exception}-- No se ha podido {self.menssage} ' \
-                                            f'debido a que el objeto "{entity}" a sido actualizado repentinamente.'
-                            self.element = Functions.capture_element(self.instance, entity)
-
-                        except ElementClickInterceptedException:
-                            self.exception = "ElementClickInterceptedException"
-                            self.retry = Parameters.Parameters.number_retries
-                            self.menssage = f'--{self.exception}-- No se ha podido {self.menssage} ' \
-                                            f'debido a que el objeto "{entity}" se encuentra solapado por otro objeto.'
-
-                        except ElementNotInteractableException:
-                            self.retry += 1
-                            self.exception = "ElementNotInteractableException"
-                            self.menssage = f'--{self.exception}-- No se ha podido {self.menssage} ' \
-                                            f'debido a que el objeto "{entity}" no esta disponible.'
-                            self.element = Functions.capture_element(self.instance, entity)
-
-                        except NoSuchElementException:
-                            self.retry += 1
-                            self.exception = "NoSuchElementException"
-                            self.menssage = f'--{self.exception}-- No se ha podido {self.menssage} ' \
-                                            f'debido a que el objeto "{entity}" no esta disponible.'
-                            self.element = Functions.capture_element(self.instance, entity)
-
-                        except Exception as e:
-                            self.retry += 1
-                            self.exception = str(e)
-                            self.menssage = f'--{self.exception}-- No se ha podido {self.menssage} ' \
-                                            f'debido a que ha ocurrido un error inesperado.'
-                            self.element = Functions.capture_element(self.instance, entity)
-
-                    else:
-                        Functions.screenshot(self, "Ultima screenshot antes de finalizar la ejecución")
-                        Functions.tear_down(self)
-                        if len(self.menssage) == 0:
-                            self.menssage = f"--{self.exception}-- {self.menssage}"
-                        unittest.TestCase().fail(self.menssage)
-                Functions.message_container = self.menssage
-                self.lista_pasos.append(action)
-                return out
-
-        Functions.page_has_loaded(self)
-        return Element(self, element, self.driver, self.value_to_find, self.get_locator_type)
+        element = self.capture_element(entity, variable_y=variable_y, variable_x=variable_x)
+        Selenium.page_has_loaded(self)
+        return ElementUI(element, self.driver, self.value_to_find, self.get_locator_type, entity)
 
     def debugger(self, debug_this_entity):
 
         """
             Description:
                 Permite visualizar los defectos antes de finalizar la ejecución, la corrección de los mismos y
                 luego cierra el navegador.
             Args:
                 debug_this_entity: Nombre de la entidad en conflicto.
             Returns:
                 Devuelve el status code correspondiente a la acción realizada por el usuario dentro de la UI.
         """
 
-        # La función fixer devuelve status Code, el nuevo xpath, id o name que actualiza la variable en memoria
-        returned_code, self.value_to_find, self.get_locator_type = Debugger(self, debug_this_entity, self.exception,
-                                                                            self.get_locator_type,
-                                                                            self.value_to_find,
-                                                                            self.complete_json_path,
-                                                                            self.json_strings,
-                                                                            self.case_name).fixer()
-        if returned_code == 1:
-            return 1
-        if returned_code == 2:
-            return 2
-        if returned_code == 3:
-            unittest.TestCase().fail("Incidencia reportada")
-        if returned_code == 4:
-            unittest.TestCase().fail("Incidencia reportada")
+        metadata = {
+            "FRAMEWORK": "Selenium",
+            "ENTITY": debug_this_entity,
+            "EXCEPTION": Selenium.exception,
+            "MESSAGE": Selenium.message_error,
+            "LOCATOR TYPE": Selenium.get_locator_type,
+            "VALUE TO FIND": Selenium.value_to_find,
+            "JSON PATH": Selenium.complete_json_path,
+            "JSON STRING": Selenium.json_strings,
+            "CASE NAME": self.case_name
+        }
+        returned_code = None
+        if Selenium.get_mode_execution(self) and not Selenium.get_mode_browser():
+            response = str(Debugger(metadata))
+            returned_code = int(response.split("||")[0])
+            Selenium.value_to_find = response.split("||")[1]
+            Selenium.get_locator_type = response.split("||")[2]
+
+        return returned_code
 
     def get_json_file(self, file):
 
         """
             Description:
                 Lee un archivo json.
             Args:
                 file (file): Archivo json.
             Returns:
                 Si el archivo fue encontrado imprime "get_json_file: " + json_path",
                 en caso contrario imprime "get_json_file: No se encontro el Archivo " + file".
         """
-
-        json_path = os.path.join(self.path_json, f"{file}.json")
+        self.json_on_loaded = file
+        json_path = os.path.abspath(
+            os.path.join(__file__, f"../../../../../projects/{self.project_name}/src/pages/{file}.json"))
         self.complete_json_path = json_path
         try:
             with open(json_path, "r", encoding='utf8') as read_file:
-                self.json_strings = json.loads(read_file.read())
+                Selenium.json_strings = json.loads(read_file.read())
                 print("get_json_file: " + json_path)
+                print(f"{self.color_message('GREEN', 'REALIZADO:')} Se a cargado el respositorio de objetos "
+                      f"'{self.color_message('BLUE', f'{file}.json')}' encontrado en el directorio "
+                      f"'{json_path}'.")
         except FileNotFoundError:
-            self.json_strings = False
-            unittest.TestCase().skipTest(u"get_json_file: No se encontro el Archivo " + file)
-            Functions.tear_down(self)
+            Selenium.json_strings = False
+            print(f"{self.color_message('RED', 'ERROR:')} No se encontro "
+                  f"'{self.color_message('BLUE', f'{file}.json')}' en el directorio '{json_path}'.")
+            unittest.TestCase().skipTest(f"get_json_file: No se encontro el Archivo {file}")
+            Selenium.tear_down(self)
 
     def get_entity(self, entity):
 
         """
             Description:
                 Lee una entidad del archivo json.
             Args:
                 entity (str): Entidad del objeto que se quiere leer.
             Returns:
                 Si la entidad fue encontrada retorna "True", en caso contrario imprime
                 "get_entity: No se encontró la key a la cual se hace referencia: " + entity".
         """
 
-        if not self.json_strings:
+        if not Selenium.json_strings:
             print("Define el DOM para esta prueba")
         else:
             try:
-                self.value_to_find = self.json_strings[entity]["ValueToFind"]
-                self.get_locator_type = self.json_strings[entity]["GetFieldBy"]
+                self.value_to_find = Selenium.json_strings[entity]["ValueToFind"]
+                self.get_locator_type = Selenium.json_strings[entity]["GetFieldBy"]
 
             except KeyError as e:
-                GenericFunctions.Functions.exception_logger(e)
+                self.exception_logger(e)
                 unittest.TestCase().skipTest(f"get_entity: No se encontro la key a la cual se hace referencia:"
                                              f"{entity}.")
-                Functions.tear_down(self)
+                self.tear_down()
 
             return True
 
     # TEXTBOX & COMBO HANDLE ###########################################################################################
     def send_especific_keys(self, element, key):
 
         """
@@ -759,27 +581,27 @@
                 Simula el envío de una tecla del teclado.
             Args:
                 element (str): Entidad del objeto que se quiere obtener.
                 key (str): Tecla seleccionada.
         """
 
         if key == 'Enter':
-            Functions.get_element(self, element).send_keys(Keys.ENTER)
+            self.get_element(self, element).send_keys(Keys.ENTER)
         if key == 'Tab':
-            Functions.get_element(self, element).send_keys(Keys.TAB)
+            self.get_element(self, element).send_keys(Keys.TAB)
         if key == 'Space':
-            Functions.get_element(self, element).send_keys(Keys.SPACE)
+            self.get_element(self, element).send_keys(Keys.SPACE)
         if key == 'Esc':
-            Functions.get_element(self, element).send_keys(Keys.ESCAPE)
+            self.get_element(self, element).send_keys(Keys.ESCAPE)
         if key == 'Retroceso':
-            Functions.get_element(self, element).send_keys(Keys.BACKSPACE)
+            self.get_element(self, element).send_keys(Keys.BACKSPACE)
         if key == 'Suprimir':
-            Functions.get_element(self, element).send_keys(Keys.DELETE)
+            self.get_element(self, element).send_keys(Keys.DELETE)
         if key == "Abajo":
-            Functions.get_element(self, element).send_keys(Keys.ARROW_DOWN)
+            self.get_element(self, element).send_keys(Keys.ARROW_DOWN)
         time.sleep(3)
 
     def get_id_window(self):
 
         """
             Description:
                 Obtiene el id de una window.
@@ -809,15 +631,15 @@
                 Cambia entre iframes en la WebApp.
             Args:
                 locator (str): Nombre del objeto que se quiere obtener.
             Returns:
                 Imprime "Se realizó el switch a (Locator)".
         """
 
-        iframe = Functions.capture_element(self, locator)
+        iframe = self.capture_element(self, locator)
         self.driver.switch_to.frame(iframe)
         print(f"Se realizó el switch a {locator}")
 
     def switch_to_parent_frame(self):
 
         """
             Description:
@@ -847,40 +669,24 @@
             Returns:
                 Si la ventana es encontrada imprime "volviendo a (ventana)",
                 en caso contrario imprime "Estas en (ventana)".
         """
 
         if window in self.windows:
             self.driver.switch_to.window(self.windows[window])
-            Functions.page_has_loaded(self)
+            self.page_has_loaded()
             print("volviendo a " + window + " : " + self.windows[window])
         else:
             self.number_windows = len(self.driver.window_handles) - 1
             self.windows[window] = self.driver.window_handles[int(self.number_windows)]
             self.driver.switch_to.window(self.windows[window])
             self.driver.maximize_window()
             print(self.windows)
             print("Estas en " + window + " : " + self.windows[window])
-            Functions.page_has_loaded(self)
-
-    def get_element_shadow_root(self, entity, index=0) -> WebElement:
-
-        """
-            Description:
-                Obtiene el DOM del Shadow Root.
-            Args:
-                index: Índice seteado en 0.
-                entity: Entidad del objeto que se quiere obtener.
-            Returns:
-                El DOM del Shadow Root.
-        """
-
-        element = self.get_element(entity)
-        shadow_elements = self.driver.execute_script(f'return arguments[{index}].shadowRoot', element)
-        return shadow_elements
+            self.page_has_loaded()
 
     def close_page(self):
 
         """
             Description:
                 Cierra la instancia del explorador.
         """
@@ -905,66 +711,71 @@
             Description:
                 Abre una nueva window con el navegador.
             Args:
                 url (str): Dirección web que se debe cargar en la window
         """
 
         self.driver.execute_script(f'''window.open("{url}","_blank");''')
-        Functions.page_has_loaded(self)
+        self.page_has_loaded()
+
 
     def page_has_loaded(self):
 
         """
             Description:
                 Espera que la página sea cargada.
             Returns:
                 Si la página se cargó imprime "complete", en caso contrario imprime "No se completó la carga".
         """
 
         try:
-            driver_target = self.driver
-            print("Checking if {} page is loaded.".format(self.driver.current_url))
-            page_state = driver_target.execute_script('return document.readyState;')
-            yield
-            WebDriverWait(driver_target, 30).until(lambda target: page_state == 'complete')
-            assert page_state == 'complete', "No se completo la carga"
+            WebDriverWait(self.driver, 60).until(
+                lambda target: self.driver.execute_script('return document.readyState;') == 'complete')
+
 
         except TimeoutException:
+            try:
+                allure.attach(self.driver.get_screenshot_as_png(),
+                              "Ultima screenshot antes de finalizar la ejecución.",
+                              attachment_type=allure.attachment_type.PNG)
+            except Exception as e:
+                Functions.exception_logger(e)
+                print(f"No se pudo realizar la screenshot de pantalla.")
             unittest.TestCase().fail("--TimeoutException-- No se ha podido realizar la carga de la página.")
 
     def scroll_to(self, locator, y=None, x=None):
 
         """
             Description:
                 Hace scroll en la página hacia el elemento que se pasa como parámetro.
             Args:
                 y: Variable y para parametrizar un elemento JSON.
                 x: Variable x para parametrizar un elemento JSON.
                 locator (str): Nombre del elemento al cual se quiere scrollear.
         """
 
-        element = Functions.capture_element(self, locator, variable_y=y, variable_x=x)
+        element = self.capture_element(locator, variable_y=y, variable_x=x)
         self.driver.execute_script("arguments[0].scrollIntoView();", element)
         print(f"Scroleando la pagina hacia el objeto: {locator}")
 
     # FUNCIONES DE ESPERA ##############################################################################################
-    def wait(self, time_load, logger=Parameters.Parameters.loggin_time, reason=None):
+    def wait(self, time_load, logger=Parameters.loggin_time, reason=None):
 
         """
             Description:
                 Espera un elemento, el tiempo es dado en segundos.
             Args:
                 time_load: Tiempo en segundos.
                 logger:
                 reason: Razón por la que se quiere esperar un elemento.
             Returns:
                 Cuando termina el tiempo de espera imprime "Esperar: Carga Finalizada ... "
         """
 
-        return GenericFunctions.Functions.wait(self, time_load, logger=logger, reason=reason)
+        return self.wait(time_load, logger=logger, reason=reason)
 
     def alert_windows(self, accept="accept"):
 
         """
             Description:
                 Espera un alert(window pop up) y hace click en accept.
             Args:
@@ -995,15 +806,15 @@
         except NoSuchWindowException:
             print('Alerta no presente.')
         except TimeoutException:
             print('Alerta no presente.')
         except UnexpectedAlertPresentException:
             print('Alerta inesperada.')
         except Exception as e:
-            GenericFunctions.Functions.exception_logger(e)
+            self.exception_logger(e)
             print(f"Ocurrio un error inesperado.")
 
     # ACCION CHAINS ####################################################################################################
     def mouse_over(self, locator):
 
         """
             Description:
@@ -1011,15 +822,15 @@
             Args:
                 locator (str): Locator del objeto que se quiere obtener.
             Returns:
                 Retorna "True" si existe el objeto dentro del json, de lo contrario
                 imprime "No se encontró el value en el Json definido".
         """
 
-        get_entity = Functions.get_entity(self, locator)
+        get_entity = self.get_entity(locator)
         if get_entity is None:
             return print("No se encontro el value en el Json definido.")
         else:
             try:
                 if self.get_locator_type.lower() == "id":
                     localizador = self.driver.find_element(By.ID, self.value_to_find)
                     action = ActionChains(self.driver)
@@ -1054,20 +865,20 @@
                     action.click(localizador)
                     action.perform()
                     print(u"mouse_over: " + locator)
                     return True
 
             except TimeoutException:
                 print(u"mouse_over: No presente " + locator)
-                Functions.tear_down(self)
+                self.tear_down()
                 return None
 
             except StaleElementReferenceException:
                 print(u"element " + locator + " is not attached to the DOM")
-                Functions.tear_down(self)
+                self.tear_down()
                 return None
 
     def double_click_element(self, element: WebElement):
 
         """
             Description:
                 Hace doble click con el mouse sobre un elemento.
@@ -1114,15 +925,15 @@
             Args:
                 locator (str): Nombre del objeto que se quiere verificar.
             Returns:
                 Retorna "True" si existe el objeto dentro del json, de lo contrario
                 imprime "No se encontro el value en el Json definido".
         """
 
-        get_entity = Functions.get_entity(self, locator)
+        get_entity = self.get_entity(locator)
 
         if get_entity is None:
             print("No se encontro el value en el Json definido")
         else:
             try:
                 if self.get_locator_type.lower() == "id":
                     wait = WebDriverWait(self.driver, 20)
@@ -1178,15 +989,15 @@
                     -Ruta de los Json
                     -Ruta de las Imágenes de los json (reconocimiento por imágenes)
                     -Ruta de los Bass
                 Si hubo un error en la configuración, imprime por consola
                 "No se pudieron detectar los datos de la ejecución".
         """
 
-        GenericFunctions.Functions.set_proyect(self, project_name)
+        Functions.set_proyect(self, project_name)
 
     @staticmethod
     def set_env(env):
 
         """
             Descripcion:
                 Configura una variable para la lectura de resources.
@@ -1194,143 +1005,165 @@
             Args:
                 env: QA, TEST, PROD, ALT
 
             Returns:
                 Funcion que configura la variable de ambiente para la lectura del resources
 
         """
-        return GenericFunctions.Functions.set_env(env)
+        return Functions.set_env(env)
 
     @staticmethod
     def set_excel_row(value: int):
-        GenericFunctions.Functions.set_excel_row(value)
+        Functions.set_excel_row(value)
 
     @staticmethod
     def set_manual_increment(value: bool):
-        GenericFunctions.Functions.set_manual_increment(value)
+        Functions.set_manual_increment(value)
 
     @staticmethod
     def get_excel_row():
 
         """
             Description:
                 Obtiene la row actual del excel.
             Returns:
                 Imprime por consola "El numero del registro consultado es: "+ str(row)" y retorna la row.
         """
 
-        return GenericFunctions.Functions.get_row_excel()
+        return Functions.get_row_excel()
 
     def set_restore_excel_row(self):
 
         """
             Description:
                 Restaura al value inicial el número de filas del excel.
             Returns:
                 Imprime por consola "Se ha restarudado el numero de la row excel: "+ str(Parameters.row).
         """
 
-        GenericFunctions.Functions.set_restore_excel_row()
+        Functions.set_restore_excel_row()
 
     @staticmethod
     def set_increment_excel_row():
 
         """
             Description:
                 Incrementa en 1 el número de filas del excel.
         """
 
-        GenericFunctions.Functions.set_increment_row()
+        Functions.set_increment_row()
 
     @staticmethod
     def get_current_time():
 
         """
             Description:
                 Se obtiene la hora actual.
             Returns:
                 Retorna la hora actual.
         """
 
-        return time.strftime(Parameters.Parameters.time_format)  # formato 24 horas
+        return time.strftime(Parameters.time_format)  # formato 24 horas
 
     @staticmethod
     def get_retry():
 
         """
             Description:
                 Se obtiene la cantidad de reintentos por default
             Returns:
                 Retorna (int) la cantidad de reintentos por default
         """
 
-        return Parameters.Parameters.number_retries
+        return Parameters.number_retries
 
     @staticmethod
     def set_highlight(value=True):
 
         """
             Description:
                 Desactivar/activar el señalamiento highlight de la funcion get_element.
             Args:
                 value: Valor booleano (seteado por default en True).
         """
 
         Parameters.highlight = value
-        print(f"La opcion hightlight de get_element se a configurado en el siguiente value {Parameters.Parameters.highlight}")
+        print(f"La opcion hightlight de get_element se a configurado en el siguiente value {Parameters.highlight}")
 
     def set_retry(self, numbers_retries):
 
         """
             Description:
                 Se configura la cantidad de reintentos por default.
             Args:
                 numbers_retries: Número entero que se utilizará como nuevo parámetro para
                 la búsqueda de reintentos de objetos en el DOM.
         """
 
-        GenericFunctions.Functions.set_retry(self, numbers_retries)
+        Functions.set_retry(self, numbers_retries)
 
     @staticmethod
     def get_timeout_beetwen_retrys():
 
         """
             Description:
                 Se obtiene el tiempo por default de espera entre reintentos.
             Returns:
                 Retorna (int) el tiempo por default de espera entre reintentos.
         """
 
-        return Parameters.Parameters.time_between_retries
+        return Parameters.time_between_retries
 
     @staticmethod
     def set_timeout_beetwen_retrys(time_target):
 
         """
             Description:
                 Se configura el tiempo por default de espera entre reintentos.
             Args:
                 time_target: Nímero entero que se utilizará para configurar el tiempo de espera entre reintentos.
         """
 
         Parameters.time_between_retries = time_target
-        print(f"El tiempo de espera entre reintentos es {Parameters.Parameters.time_between_retries}.")
+        print(f"El tiempo de espera entre reintentos es {Parameters.time_between_retries}.")
+
+    @staticmethod
+    def set_browser(browser):
+
+        """
+            Description:
+                Setea el navegador por defecto.
+            Args:
+                browser (str): Navegador.
+        """
+
+        Parameters.browser = browser
+        print(f"El navegador seleccionado es: {str(Parameters.browser)}.")
 
     @staticmethod
-    def get_mode_execution():
+    def get_environment():
+
+        """
+            Description:
+                Devuelve el environment (Sistema operativo) en el que se está corriendo la prueba.
+        """
+
+        return Parameters.environment
+
+    def get_mode_execution(self):
 
         """
             Description:
                 Indica si el caso requiere ser debugeado.
             Returns:
                 Devuelve valor de la variable de Parameters.debug (True o False)
                 que indica si el caso requiere ser debugeado.
         """
 
-        return Parameters.Parameters.debug
+        return Parameters.debug
 
     @staticmethod
     def set_mode_debug(status=True):
 
         """
             Description:
                 Configura la variable Parameters.debug en verdadero.
@@ -1346,15 +1179,15 @@
         """
             Description:
                 Obtiene la configuración del headless del navegador.
             Returns:
                 Devuelve la configuración del navegador (Headless ON/True o Headless OFF/False).
         """
 
-        return Parameters.Parameters.headless
+        return Parameters.headless
 
     @staticmethod
     def set_mode_browser(status=True):
 
         """
             Description:
                 Setea el headless del navegador.
@@ -1373,82 +1206,48 @@
                 cell: Celda del resource.
                 case_name: Nombre del caso.
                 specific_sheet: Hoja del resource.
             Returns:
                 Retorna el value de la cell del resource.
         """
 
-        return GenericFunctions.Functions.read_cell(self, cell, file_name=case_name, specific_sheet=specific_sheet)
-
-    # CAPTURA DE PANTALLA ##############################################################################################
-    def crear_path(self):
-
-        """
-            Description:
-                Se crea el directorio para las capturas de pantalla.
-            Returns:
-                Retorna el directorio creado.
-        """
-
-        day = time.strftime("%d-%m-%Y")  # formato aaaa/mm/dd
-        general_path = self.path_evidences
-        browser = Parameters.Parameters.browser
-        test_case = self.__class__.__name__
-        current_time = time.strftime(Parameters.Parameters.time_format)  # formato 24 houras
-        x = re.search("Context", test_case)
-        if x:
-            path = f"{general_path}/{day}/{browser}/{current_time}/"
-        else:
-            path = f"{general_path}/{day}/{test_case}/{browser}/{current_time}/"
-
-        if not os.path.exists(path):  # si no existe el directorio lo crea
-            os.makedirs(path)
-
-        return path
+        return Functions.read_cell(self, cell, file_name=case_name, specific_sheet=specific_sheet)
 
     def screenshot(self, description):
 
         """
             Description:
                 Saca screenshot de pantalla para los reportes de allure y se agrega la descripción de la misma.
             Args:
                 description: Descripción de la screenshot de pantalla.
             Returns:
                 Retorna la imágen y descripción de la screenshot de pantalla.
         """
-        Functions.page_has_loaded(self)
+        Selenium.page_has_loaded(self)
         try:
             allure.attach(self.driver.get_screenshot_as_png(), description, attachment_type=allure.attachment_type.PNG)
         except Exception as e:
-            GenericFunctions.Functions.exception_logger(e)
+            Functions.exception_logger(e)
             print(f"No se pudo realizar la screenshot de pantalla.")
 
-
     def image_for_debugger_report(self):
 
         """
             Description:
                 Saca screenshot de pantalla para los reportes de allure y se agrega la descripción de la misma.
-            Args:
-                description: Descripción de la screenshot de pantalla.
             Returns:
                 Retorna la imágen y descripción de la screenshot de pantalla.
         """
         try:
             base_folder = f"C:\\testing-Automation\\projects\\{str(self.project_name)}\\src\\outputs\\"
             if "jira_report.png" not in base_folder:
                 self.memory_image = self.driver.get_screenshot_as_png()
         except Exception as e:
             print(f"Hubo inconvenientes al intentar crear la carpeta contenedora de las 'report image'")
 
-
-
-
-
-
     # SERVICIOS WEB ####################################################################################################
     def send_service(self, data):
 
         """
             Description:
                 Envía un servicio.
             Args:
@@ -1470,15 +1269,15 @@
         differences = []
         validate_cant_records = "None"
         cant_registros_db = ""
         cant_registros_api = ""
         statuscode = None
         validation_status_code = None
 
-        total_retry = Parameters.Parameters.number_retries
+        total_retry = Parameters.number_retries
 
         # Se realiza el llamado a la api, si falla reintenta nuevamente.
         for retry in range(total_retry):
             if data['headers'] is not None:
                 try:
                     response = requests.request(data['tipoPeticion'], data['endPoint'], headers=data['headers'],
                                                 data=data['payload'], timeout=data['time'])
@@ -1498,15 +1297,15 @@
         # Se valida es status code del request.
         try:
             unittest.TestCase().assertNotEqual(str(type(response)), "<class 'str'>",
                                                "Error Status Code: No se obtuvo response valido. Response de tipo String (TimeOut)")
             validation_status_code = self.validate_status_code(data['statusCodeEsperado'], response.status_code)
             statuscode = response.status_code
         except AttributeError as e:
-            GenericFunctions.Functions.exception_logger(e)
+            Functions.exception_logger(e)
             print(f"Error al obtener el status code del servicio.")
 
         # Se valida la estructura/integridad del response.
         if 'validateStructure' in data.keys():
             if data['validateStructure']:
                 validation_structure, differences = self.validate_structure(data['responseEsperado'], response)
             else:
@@ -1720,15 +1519,16 @@
             Returns:
                 Retorna un array con las diferencias encontradas.
         """
 
         differences = []
         try:
 
-            unittest.TestCase().assertNotEqual(str(type(response_obtained)), "<class 'str'>", "Error: El response obtenido es de tipo String")
+            unittest.TestCase().assertNotEqual(str(type(response_obtained)), "<class 'str'>",
+                                               "Error: El response obtenido es de tipo String")
             response_obtained = json.loads(response_obtained.text)
         except ValueError:
             unittest.TestCase().assertEqual(True, False, "Error al convertir el json value_text en diccionario.")
 
         if len(expected_response) > 0 and str(type(expected_response)) != "<class 'dict'>":
             expected_response = expected_response[0]
 
@@ -1833,15 +1633,15 @@
             Args:
                 min_range (int): Rango mínimo.
                 max_range (int): Rango máximo.
             Returns:
                 Retorna un número aleatorio.
         """
 
-        return GenericFunctions.Functions.get_random(self, min_range, max_range)
+        return Functions.get_random(self, min_range, max_range)
 
     @staticmethod
     def get_random_string(numbers_characters):
 
         """
             Description:
                 Genera una palabra random.
@@ -1899,26 +1699,26 @@
         """
             Description:
                 Configura el value de timeout (segundos) configurado para las conexiones a bases sqlServer.
             Args:
                 time_seconds: Valor (int) que representa una cantidad en segundos.
         """
 
-        GenericFunctions.Functions.set_timeout_base_sql_server(self, time_seconds)
+        Functions.set_timeout_base_sql_server(self, time_seconds)
 
     def get_timeout_base_sql_server(self):
 
         """
             Description:
                 Devuelve el value de timeout configurado para la conexion a bases sqlServer.
             Return:
                 Devuelve el value de timeout (segundos) configurado para la conexion a bases sqlServer.
         """
 
-        return GenericFunctions.Functions.get_timeout_base_sql_server(self)
+        return Functions.get_timeout_base_sql_server(self)
 
     def establish_connection_sqlserver(self, server, base, user, password):
 
         """
             Description:
                 Realiza conexión a una base de datos sqlServer.
             Args:
@@ -1926,15 +1726,15 @@
                 base: nombre de la base
                 user: usuario
                 password: Contraseña
             Return:
                 Devuelve una variable con la conexion a la base de datos sqlServer.
         """
 
-        return GenericFunctions.Functions.establish_connection_sqlserver(self, server, base, user, password)
+        return Functions.establish_connection_sqlserver(self, server, base, user, password)
 
     def check_base_sqlserver(self, server, base, user, password, query):
 
         """
             Description:
                 Realiza conexión y consulta a base de datos con la libreria pyodbc. El metodo incluye la
                 desconexión.
@@ -1945,15 +1745,15 @@
                 password: Contraseña.
                 query: Consulta Query.
             Returns:
                 <class 'pyodbc.Row'>: Retorna un class 'pyodbc.Row' si la consulta y la conexión es exitosa. De lo
                 contrario imprime por consola "Se produjo un error en la base de datos."
         """
 
-        return GenericFunctions.Functions.check_base_sqlserver(self, server, base, user, password, query)
+        return Functions.check_base_sqlserver(self, server, base, user, password, query)
 
     def execute_sp_base_sqlserver(self, server, base, user, password, query, parameters: tuple):
 
         """
             Description:
                 Realiza conexión y consulta a base de datos con la libreria pyodbc. El metodo incluye la
                 desconexión.
@@ -1964,15 +1764,15 @@
                 password (str): Contraseña.
                 query (str): Consulta Query.
                 parameters (tuple): Tupla con parametros para el sp.
             Returns:
                 Lista con los resultados.
         """
 
-        return GenericFunctions.Functions.execute_sp_base_sqlserver(self, server, base, user, password, query, parameters)
+        return Functions.execute_sp_base_sqlserver(self, server, base, user, password, query, parameters)
 
     def get_list_base_sqlserver(self, server, base, user, password, query):
 
         """
             Description:
                 Realiza conexión y consulta a base de datos con la libreria pyodbc. El metodo incluye la
                 desconexión.
@@ -1982,15 +1782,15 @@
                 user (str): Usuario.
                 password (str): Contraseña.
                 query (str): Consulta Query.
             Returns:
                 Lista con los resultados.
         """
 
-        return GenericFunctions.Functions.get_list_base_sqlserver(self, server, base, user, password, query)
+        return Functions.get_list_base_sqlserver(self, server, base, user, password, query)
 
     def delete_reg_base_sqlserver(self, server, base, user, password, query):
 
         """
             Description:
                 Elimina un registro de la base de datos. El método incluye la desconexión.
             Args:
@@ -1999,15 +1799,15 @@
                 user: Usuario.
                 password: Contraseña.
                 query: Consulta Query.
             Returns:
                 Imprime por consola "Ocurrió un error en la base".
         """
 
-        GenericFunctions.Functions.delete_reg_base_sqlserver(self, server, base, user, password, query)
+        Functions.delete_reg_base_sqlserver(self, server, base, user, password, query)
 
     @staticmethod
     def check_base_oracle(server, base, encoding, user, password, query):
 
         """
             Description:
                 Realiza la conexión y consulta a base de datos Oracle. El método incluye la desconexión.
@@ -2048,44 +1848,44 @@
         """
             Description:
                 Obtiene la fecha del sistema.
             Returns:
                 Retorna fecha del sistema.
         """
 
-        dia_global = time.strftime(Parameters.Parameters.date_format)  # formato dd/mm/aaaa
+        dia_global = time.strftime(Parameters.date_format)  # formato dd/mm/aaaa
         print(f'Fecha del sistema {dia_global}')
         return Functions.global_date
 
     @staticmethod
     def get_time():
 
         """
             Description:
                 Obtiene la hora del sistema.
             Returns:
                 Retorna la hora del sistema.
         """
 
-        hora_global = time.strftime(Parameters.Parameters.time_format)  # formato 24 houras
+        hora_global = time.strftime(Parameters.time_format)  # formato 24 houras
         print(f'Hora del sistema {hora_global}')
         return Functions.global_time
 
     @staticmethod
     def get_date_time():
 
         """
             Description:
                 Obtiene la fecha y hora del sistema.
             Returns:
                 Retorna fecha y la hora del sistema.
         """
 
-        global_date = time.strftime(Parameters.Parameters.date_format)  # formato dd/mm/aaaa
-        global_time = time.strftime(Parameters.Parameters.time_format)  # formato 24 houras
+        global_date = time.strftime(Parameters.date_format)  # formato dd/mm/aaaa
+        global_time = time.strftime(Parameters.time_format)  # formato 24 houras
         date_time = f'{global_date} {global_time}'
         print(f"La fecha y hora del sistema es: {date_time}")
         return date_time
 
     @staticmethod
     def get_difference_datetime(datetime_one, datetime_two):
 
@@ -2095,15 +1895,15 @@
             Args:
                 datetime_one: Fecha.
                 datetime_two: Fecha.
             Returns:
                 Retorna la diferencia entre dos fechas.
         """
 
-        format_date = Parameters.Parameters.date_format + " " + Parameters.Parameters.time_format
+        format_date = Parameters.date_format + " " + Parameters.time_format
         datetime_one = datetime.datetime.strptime(datetime_one, format_date)
         datetime_two = datetime.datetime.strptime(datetime_two, format_date)
         difference = datetime_one - datetime_two
         print(f"Diferencia de fechas: {difference}")
         return difference
 
     @staticmethod
@@ -2135,15 +1935,15 @@
             Return:
                 Devuelve la fecha actual con el tiempo adicional.
         """
 
         add_time = datetime.timedelta(hours=add_time_delta[0], minutes=add_time_delta[1], seconds=add_time_delta[2])
         now = datetime.datetime.now()
         new_datetime = now + add_time
-        date_time_format = f"{Parameters.Parameters.date_format} {Parameters.Parameters.time_format}"
+        date_time_format = f"{Parameters.date_format} {Parameters.time_format}"
         new_datetime = new_datetime.strftime(date_time_format)
         return new_datetime
 
     @staticmethod
     def hour_rounder(date_time: str):
 
         """
@@ -2151,15 +1951,15 @@
                 Redondea la hora de la fecha actual.
             Args:
                 date_time: Recibe una fecha en formato value_text con formato "%H:%M:%S %d/%m/%Y"
             Return:
                 Devuelve la fecha redondeada.
         """
 
-        date_time_format = f"{Parameters.Parameters.date_format} {Parameters.Parameters.time_format}"
+        date_time_format = f"{Parameters.date_format} {Parameters.time_format}"
         date_time = datetime.datetime.strptime(date_time, date_time_format)
         return (date_time.replace(second=0, microsecond=0, minute=0, hour=date_time.hour) +
                 datetime.timedelta(hours=date_time.minute // 30))
 
     @staticmethod
     def convert_date_to_bit(date_target):
 
@@ -2187,28 +1987,28 @@
                 content (str): Cuerpo del correo.
                 file_attach (file): Archivos adjuntos del correo.
             Returns:
                 Si el correo fue enviado con éxito retorna el estado "Enviado",
                 de lo contrario imprime por consola "El mail no pudo ser enviado" y estado "No enviado".
         """
 
-        return GenericFunctions.Functions.send_mail(self, receiver_email, title, content, file_attach=file_attach)
+        return Functions.send_mail(self, receiver_email, title, content, file_attach=file_attach)
 
     def create_title(self, title_text: str):
 
         """
             Descripcion:
                 Crea un título en formato html.
             Args:
                 title_text: Título en formato value_text.
             Return:
                 Devuelve título en formato html.
         """
 
-        return GenericFunctions.Functions.create_title(title_text)
+        return Functions.create_title(title_text)
 
     @staticmethod
     def create_message_html(message_text: str, special_strings=None):
 
         """
             Descripcion:
                 Crea un párrafo en formato html.
@@ -2217,52 +2017,52 @@
                 special_strings: Lista de palabras que deben ser resaltadas en negrita dentro del mensaje.
             Return:
                 Devuelve párrafo en formato html.
         """
 
         if special_strings is None:
             special_strings = []
-        return GenericFunctions.Functions.create_message_html(message_text, special_strings)
+        return Functions.create_message_html(message_text, special_strings)
 
     def create_table(self, list_data_head: list, list_data_content: list):
 
         """
             Descripcion: crea una tabla html.
             Args:
                 list_data_head: Lista con los encabezados de la tabla.
                 list_data_content: Matriz (lista con lista) con los datos de la tabla.
             Return:
                 Devuelve una tabla en formato html.
         """
 
-        return GenericFunctions.Functions.create_table(list_data_head, list_data_content)
+        return Functions.create_table(list_data_head, list_data_content)
 
     def create_style_html(self):
 
         """
             Description:
                 Devuelve el código css con los estilos que deben aplicarse a un bloque HTML.
             Return:
                 Devuelve el estilo para aplicar al código html.
         """
 
-        return GenericFunctions.Functions.create_style_html()
+        return Functions.create_style_html()
 
     def apply_style_css_to_block(self, block_html: str):
 
         """
             Description:
                 Aplica estilos css a un bloque html.
             Args:
                 block_html: Bloque html que recibirá los estilos css.
             Return:
                 Devuelve un bloque html con estilos aplicados.
         """
 
-        return GenericFunctions.Functions.apply_style_css_to_block(block_html)
+        return Functions.apply_style_css_to_block(block_html)
 
     @staticmethod
     def print_precondition_data(precondition_json):
 
         """
             Description:
                 Adjunta en el reporter de allura un json con los datos pre condición utilizados en la prueba.
@@ -2271,77 +2071,63 @@
         """
 
         with allure.step(u"PASO: Se utilizan lo siguientes datos como pre condición"):
             allure.attach(json.dumps(precondition_json, indent=4),
                           "Datos pre condición",
                           attachment_type=allure.attachment_type.JSON)
 
-    def set_new_value_json(self, json_data, claves,  valor_nuevo=None):
-        '''
+    def set_new_value_json(self, json_data, claves, valor_nuevo=None):
+        """
             Modifica el value de una key o elimina key/value del json, segun el tipo_accion.
             En caso de no encontrar lanza un mensaje de error
             :param json_data: contiene dict_to_json del json original
             :param valor_nuevo:(opc) nuevo value que se toma para el caso de modificar del json
             :return: json modificado con el nuevo value
-        '''
+        """
 
-        if (str(type(claves)) != "<class 'list'>"):
+        if isinstance(claves, str):
             claves = claves.split('.')
 
         if len(claves) == 1:
-            if str(type(json_data)) != "<class 'list'>":
-                self.assertIn(claves[0], json_data, "No se encontro la clave")
-            if (str(type(json_data)) == "<class 'list'>"):
+            if isinstance(json_data, list):
                 json_data[0][claves[0]] = valor_nuevo
             else:
                 json_data[claves[0]] = valor_nuevo
-            return json_data
-
-        elif len(claves) == 2:
-            if str(type(json_data)) != "<class 'list'>":
-                self.assertIn(claves[0], json_data, "No se encontro la clave")
-            if (str(type(json_data)) == "<class 'list'>"):
-                json_data[0][claves[0]][0][claves[1]] = valor_nuevo
-                return json_data
-
-        self.set_new_value_json(json_data[claves.pop(0)], claves,  valor_nuevo)
+        else:
+            if isinstance(json_data, list):
+                self.set_new_value_json(json_data[0][claves[0]], claves[1:], valor_nuevo)
+            else:
+                self.set_new_value_json(json_data[claves[0]], claves[1:], valor_nuevo)
         return json_data
 
     def delete_value_json(self, json_data, claves):
-        '''
+        """
             Modifica el value de una key o elimina key/value del json, segun el tipo_accion.
             En caso de no encontrar lanza un mensaje de error
             :param tipo_accion: determina la accion a realizar. Valores posibles 'MODIFICA' o 'ELIMINA'
             :param json_data: contiene dict_to_json del json original
             :param valor_nuevo:(opc) nuevo value que se toma para el caso de modificar del json
             :return: json modificado con el nuevo value
-        '''
+        """
 
-        if(str(type(claves)) != "<class 'list'>"):
+        if isinstance(claves, str):
             claves = claves.split('.')
 
         if len(claves) == 1:
-            if str(type(json_data)) != "<class 'list'>":
-                self.assertIn(claves[0], json_data, "No se encontro la clave")
-                if (str(type(json_data)) == "<class 'list'>"):
-                    del json_data[0][claves[0]]
-                else:
-                    del json_data[claves[0]]
-
-            return json_data
-
-        elif len(claves) == 2:
-            if str(type(json_data)) != "<class 'list'>":
-                self.assertIn(claves[0], json_data, "No se encontro la clave")
-                if (str(type(json_data)) == "<class 'list'>"):
-                    del json_data[0][claves[0]][0][claves[1]]
-                    return json_data
-
-        self.delete_value_json(json_data[claves.pop(0)], claves)
+            if isinstance(json_data, list):
+                del json_data[0][claves[0]]
+            else:
+                del json_data[claves[0]]
+        else:
+            if isinstance(json_data, list):
+                self.delete_value_json(json_data[0][claves[0]], claves[1:])
+            else:
+                self.delete_value_json(json_data[claves[0]], claves[1:])
         return json_data
+
     ####################################### Jira conections ############################################################
 
     def write_cell(self, cell, value, name, folder='files', sheet=None):
 
         """
             Description:
                 Permite escribir en una celda indicada de una hoja especifica para un
@@ -2354,19 +2140,296 @@
                 folder (str): Nombre de la carpeta que contiene el libro excel. Es 'files' por default o puede ser
                 'downloads'.
             Returns:
                 Imprime por consola la celda, hoja y valor escrito, y devuelve TRUE
                 en caso contrario imprime por consola "VERIFICAR: No se pudo escribir el archivo."
                 y devuelve FALSE.
         """
-        return GenericFunctions.Functions.write_cell(self, cell, value, name, folder, sheet)
-    ############################################ PORT CHECKER ##########################################################
-    def enable_chrome_driver_port(self, enable_driver_port):
-        self.driver_port_status = enable_driver_port
-        print(f"Se ha activado el driver port")
+        return Functions.write_cell(self, cell, value, name, folder, sheet)
 
     @staticmethod
     def available_port():
+
+        """
+
+            Description:
+                Busca un puerto disponible.
+            Returns:
+                Devuelve el puerto disponible.
+
+        """
+
         import socket
         sock = socket.socket()
         sock.bind(('', 0))
         return sock.getsockname()[1]
+
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
+        Functions.set_exception_loggin(value)
+
+    @staticmethod
+    def color_message(color, message):
+        """
+        Description: Colorea el string del color indicado de entre una lista de colores.
+
+        Args:
+            color: puede ser de color red, blue, yellow o green.
+            message: string a colorear.
+
+        Returns:
+            string coloreado.
+
+        """
+        return Functions.color_message(color, message)
+
+    def open_new_tab(self, web_url):
+        # Abrir nueva tab
+        Selenium.driver.execute_script("window.open('about:blank', 'secondtab');")
+        # Cambio de prioridad a la segunda ventana
+        Selenium.driver.switch_to.window("secondtab")
+        # ingresar a la web deseada en la nueva tab
+        Selenium.driver.get(f'{web_url}')
+
+
+class ElementUI(Functions):
+
+    def __init__(self, context_element, driver, json_value, json_get_indicator, entity):
+        self.retry = 0
+        self.element = context_element
+        self.driver = driver
+        self.json_ValueToFind = json_value
+        self.json_GetFieldBy = json_get_indicator
+        self.entity = entity
+        self.message = None
+        self.exception = None
+
+    def click(self):
+        self.execute_action("click")
+
+    def click_js(self):
+        self.execute_action("click_js")
+
+    def double_click(self):
+        self.execute_action("double_click")
+
+    def send_keys(self, value):
+        self.execute_action("send_keys", value)
+
+    def send_special_key(self, value):
+        self.execute_action("send_special_key", value)
+
+    @property
+    def text(self):
+        return self.execute_action("text")
+
+    def clear(self):
+        self.execute_action("clear")
+
+    def clear_js(self):
+        self.execute_action("clear_js")
+
+    def is_enabled(self):
+        return self.execute_action("is_enabled")
+
+    def is_selected(self, value):
+        return self.execute_action("is_selected", value)
+
+    def is_displayed(self):
+        return self.execute_action("is_displayed")
+
+    def get_property(self, value):
+        return self.execute_action("get_property", value)
+
+    def get_attribute(self, value):
+        return self.execute_action("get_attribute", value)
+
+    def capture(self):
+        return self.execute_action("capture")
+
+    def select_option_by_text(self, value):
+        return self.execute_action("select_option_by_text", value)
+
+    def select_option_by_value(self, value):
+        return self.execute_action("select_option_by_value", value)
+
+    def select_option_by_index(self, value):
+        return self.execute_action("select_option_by_index", value)
+
+    def get_all_values_to_select(self):
+        return self.execute_action("get_all_values_to_select")
+
+    def select_action(self, action, value=None):
+        self.message = ""
+
+        if action == "click":
+            self.message = "realizar click"
+            return self.element.click()
+
+        if action == "click_js":
+            self.message = "realizar click"
+            self.driver.execute_script("arguments[0].click();", self.element)
+
+        if action == "double_click":
+            self.message = "realizar doble click"
+            return Selenium.double_click_element(self, self.element)
+
+        if action == "send_keys":
+            self.message = "escribir en el campo"
+            return self.element.send_keys(value)
+
+        if action == "send_special_key":
+            self.message = f"presionar la tecla {value} en el objetivo"
+            key = value.upper()
+            if key == 'ENTER':
+                self.element.send_keys(Keys.ENTER)
+            if key == 'TAB':
+                self.element.send_keys(Keys.TAB)
+            if key == 'ESPACIO':
+                self.element.send_keys(Keys.SPACE)
+            if key == 'ESCAPE':
+                self.element.send_keys(Keys.ESCAPE)
+            if key == 'RETROCESO':
+                self.element.send_keys(Keys.BACKSPACE)
+            if key == 'SUPRIMIR':
+                self.element.send_keys(Keys.DELETE)
+            if key == "ABAJO":
+                self.element.send_keys(Keys.ARROW_DOWN)
+            if key == "F3":
+                self.element.send_keys(Keys.F3)
+            if key == "F4":
+                self.element.send_keys(Keys.F4)
+
+        if action == "text":
+            self.message = "obtener texto del campo"
+            return self.element.text
+
+        if action == "clear":
+            self.message = "limpiar el texto del campo"
+            return self.element.clear()
+
+        if action == "clear_js":
+            self.message = "limpiar campo"
+            self.driver.execute_script('arguments[0].value="";', self.element)
+
+        if action == "is_enabled":
+            self.message = "verificar el estado del objeto"
+            return self.element.is_enabled()
+
+        if action == "is_selected":
+            self.message = "verificar si el objeto es seleccionable"
+            return self.element.is_selected()
+
+        if action == "is_displayed":
+            self.message = "visualizar el objeto"
+            return self.element.is_displayed()
+
+        if action == "get_property":
+            self.message = "obtener las propiedades del objeto"
+            return self.element.get_property(value)
+
+        if action == "get_attribute":
+            self.message = "obtener los atributos del objeto"
+            return self.element.get_attribute(value)
+
+        if action == "capture":
+            self.message = "capturar pantalla"
+            Selenium.highlight(self, self.element)
+            Selenium.screenshot(self, f"Se visualiza el objeto {self.entity}")
+            return
+
+        if action == "select_option_by_value":
+            self.message = f"seleccionar value {value} de la lista"
+            Select(self.element).select_by_value(value)
+
+        if action == "select_option_by_text":
+            self.message = f"seleccionar value {value} de la lista"
+            Select(self.element).select_by_visible_text(value)
+
+        if action == "select_option_by_index":
+            self.message = f"seleccionar value {value} de la lista"
+            Select(self.element).select_by_index(value)
+
+        if action == "get_all_values_to_select":
+            list_value = []
+            self.message = f"obtener todos los valores de la lista {self.element}"
+            for option_value in Select(self.element).options:
+                list_value.append(option_value.get_attribute("value"))
+            return list_value
+
+    def execute_action(self, action, value=None):
+        out = None
+        self.message = None
+        while self.retry <= Parameters.number_retries:
+            if self.retry < Parameters.number_retries:
+                try:
+                    out = self.select_action(action, value)
+                    break
+
+                except StaleElementReferenceException:
+                    self.retry += 1
+                    self.exception = "StaleElementReferenceException"
+                    self.message = f'--{self.exception}-- No se ha podido {self.message} ' \
+                                   f'debido a que el objeto "{self.entity}" a sido actualizado repentinamente.'
+                    Selenium.message_error = self.message
+                    Selenium.exception = self.exception
+
+                except ElementClickInterceptedException:
+                    self.exception = "ElementClickInterceptedException"
+                    self.retry = Parameters.number_retries
+                    self.message = f'--{self.exception}-- No se ha podido {self.message} ' \
+                                   f'debido a que el objeto "{self.entity}" se encuentra solapado por otro objeto.'
+                    Selenium.message_error = self.message
+                    Selenium.exception = self.exception
+
+                except ElementNotInteractableException:
+                    self.retry += 1
+                    self.exception = "ElementNotInteractableException"
+                    self.message = f'--{self.exception}-- No se ha podido {self.message} ' \
+                                   f'debido a que el objeto "{self.entity}" no esta disponible.'
+                    Selenium.message_error = self.message
+                    Selenium.exception = self.exception
+
+                except NoSuchElementException:
+                    self.retry += 1
+                    self.exception = "NoSuchElementException"
+                    self.message = f'--{self.exception}-- No se ha podido {self.message} ' \
+                                   f'debido a que el objeto "{self.entity}" no esta disponible.'
+                    Selenium.message_error = self.message
+                    Selenium.exception = self.exception
+
+                except Exception as e:
+                    self.retry += 1
+                    self.exception = type(e).__name__
+                    self.message = f'--{self.exception}-- No se ha podido {self.message} ' \
+                                   f'debido a que ha ocurrido un error inesperado.'
+                    Selenium.message_error = self.message
+                    Selenium.exception = self.exception
+
+                self.element = Selenium.capture_element(self, self.entity)
+            else:
+                if Selenium.debugger(self, self.element) == 1:
+                    self.retry = 0
+                    self.element = Selenium.capture_element(self, self.entity)
+                else:
+                    Selenium.screenshot(self, "Ultima screenshot antes de finalizar la ejecución.")
+                    Selenium.tear_down(self)
+                    if len(self.message) == 0:
+                        self.message = f"--{self.exception}-- {self.message}"
+                    unittest.TestCase().fail(self.message)
+
+        print(f"{Functions.color_message('GREEN', 'REALIZADO:')} Se pudo {self.message} sobre "
+              f"'{Functions.color_message('BLUE', self.entity)}'.")
+        Selenium.message_container = self.message
+        Selenium.lista_pasos.append(action)
+        if out is not None:
+            return out
```

### Comparing `Andreani_QA_Selenium-0.0.1/setup.py` & `Andreani_QA_Selenium-0.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 PACKAGE_NAME = 'Andreani_QA_Selenium'  # Debe coincidir con el nombre de la carpeta
-AUTHOR = 'Andreani_Testing_Automation_QA'
+AUTHOR = 'AndreaniTesting'
 AUTHOR_EMAIL = 'user_appglatest@andreani.com'
 URL = ''
 
 LICENSE = 'MIT'  # Tipo de licencia
 DESCRIPTION = 'SeleniumFramework para ejecución de casos automatizados'  # Descripción corta
 LONG_DESCRIPTION = ""  # Referencia al documento README con una descripción más elaborada
 LONG_DESC_TYPE = "text/markdown"
 
 # Paquetes necesarios para que funcione la libreía. Se instalarán a la vez si no lo tuvieras ya instalado
 INSTALL_REQUIRES = [
-    'requests', 'allure-behave', 'allure-pytest', 'allure-python-commons', 'Andreani-QA-Parameters', 'Andreani-QA-Functions', 'Andreani-QA-Debugger', 'selenium',
-    'webdriver_manager'
+    'allure-behave', 'allure-pytest', 'allure-python-commons', 'Andreani-QA-Parameters',
+    'Andreani-QA-Functions', 'Andreani-QA-Debugger', 'requests', 'selenium', 'webdriver_manager'
 ]
 
 setup(
     name=PACKAGE_NAME,
     version=VERSION,
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
```

