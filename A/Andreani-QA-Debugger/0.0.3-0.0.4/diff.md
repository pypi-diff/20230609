# Comparing `tmp/Andreani_QA_Debugger-0.0.3.tar.gz` & `tmp/Andreani_QA_Debugger-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Andreani_QA_Debugger-0.0.3.tar", last modified: Tue Mar  7 17:34:11 2023, max compression
+gzip compressed data, was "Andreani_QA_Debugger-0.0.4.tar", last modified: Fri Jun  9 19:07:42 2023, max compression
```

## Comparing `Andreani_QA_Debugger-0.0.3.tar` & `Andreani_QA_Debugger-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-03-07 17:34:11.611776 Andreani_QA_Debugger-0.0.3/
-drwxrwxrwx   0        0        0        0 2023-03-07 17:34:11.579127 Andreani_QA_Debugger-0.0.3/Andreani_QA_Debugger/
--rw-rw-rw-   0        0        0    24235 2023-03-07 17:33:33.000000 Andreani_QA_Debugger-0.0.3/Andreani_QA_Debugger/Debugger.py
--rw-rw-rw-   0        0        0       32 2023-03-07 17:32:19.000000 Andreani_QA_Debugger-0.0.3/Andreani_QA_Debugger/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-07 17:34:11.607163 Andreani_QA_Debugger-0.0.3/Andreani_QA_Debugger.egg-info/
--rw-rw-rw-   0        0        0      316 2023-03-07 17:34:11.000000 Andreani_QA_Debugger-0.0.3/Andreani_QA_Debugger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      303 2023-03-07 17:34:11.000000 Andreani_QA_Debugger-0.0.3/Andreani_QA_Debugger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-07 17:34:11.000000 Andreani_QA_Debugger-0.0.3/Andreani_QA_Debugger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-03-07 17:34:11.000000 Andreani_QA_Debugger-0.0.3/Andreani_QA_Debugger.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-03-07 17:34:11.000000 Andreani_QA_Debugger-0.0.3/Andreani_QA_Debugger.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      316 2023-03-07 17:34:11.610812 Andreani_QA_Debugger-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-01-26 19:44:24.000000 Andreani_QA_Debugger-0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-03-07 17:34:11.611776 Andreani_QA_Debugger-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1134 2023-03-07 17:23:22.000000 Andreani_QA_Debugger-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 19:07:42.594181 Andreani_QA_Debugger-0.0.4/
+drwxrwxrwx   0        0        0        0 2023-06-09 19:07:42.578023 Andreani_QA_Debugger-0.0.4/Andreani_QA_Debugger/
+-rw-rw-rw-   0        0        0    24553 2023-05-22 14:07:17.000000 Andreani_QA_Debugger-0.0.4/Andreani_QA_Debugger/Debugger.py
+-rw-rw-rw-   0        0        0       32 2023-03-07 17:32:19.000000 Andreani_QA_Debugger-0.0.4/Andreani_QA_Debugger/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 19:07:42.589610 Andreani_QA_Debugger-0.0.4/Andreani_QA_Debugger.egg-info/
+-rw-rw-rw-   0        0        0      301 2023-06-09 19:07:42.000000 Andreani_QA_Debugger-0.0.4/Andreani_QA_Debugger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      303 2023-06-09 19:07:42.000000 Andreani_QA_Debugger-0.0.4/Andreani_QA_Debugger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 19:07:42.000000 Andreani_QA_Debugger-0.0.4/Andreani_QA_Debugger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-06-09 19:07:42.000000 Andreani_QA_Debugger-0.0.4/Andreani_QA_Debugger.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-06-09 19:07:42.000000 Andreani_QA_Debugger-0.0.4/Andreani_QA_Debugger.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      301 2023-06-09 19:07:42.593169 Andreani_QA_Debugger-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-01-26 19:44:24.000000 Andreani_QA_Debugger-0.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-09 19:07:42.594181 Andreani_QA_Debugger-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1068 2023-06-09 19:06:30.000000 Andreani_QA_Debugger-0.0.4/setup.py
```

### Comparing `Andreani_QA_Debugger-0.0.3/Andreani_QA_Debugger/Debugger.py` & `Andreani_QA_Debugger-0.0.4/Andreani_QA_Debugger/Debugger.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,17 +66,26 @@
             /* UI Properties */
             border: 1px solid #D71920 ;
             box-shadow: 5px 5px 5px #0000000F;
             border-radius: 25px;
             opacity: 1;
         }   
         .message{
-            height: 5rem;
+            margin-top: 0.5rem;
+            height: 3.5rem;
             max-width: 25rem;
-            max-height: 5rem;
+            max-height: 3.5rem;
+            margin-bottom: 1.5rem;
+            overflow: hidden;
+            text-overflow: ellipsis;
+        }
+        .exception {
+            height: 1rem;
+            max-width: 25rem;
+            max-height: 1rem;
             overflow: hidden;
             text-overflow: ellipsis;
         }
         p{
             font: normal;
             font-family: Arial, Helvetica, sans-serif;
             padding-bottom: 1rem;
@@ -241,18 +250,19 @@
         "CASE NAME": "test_000_alta_de_usuario_fulano"
         }
     """
 
     def __init__(self, metadata) -> None:
         Debugger.metadata = Debugger.normalizer_metadata(metadata)
         Debugger.api = Api()
+        Debugger.api.set_code(2)
         Debugger.pages = Debugger.build_pages()
         Debugger.window = webview.create_window(f'Debugger 3.0 - {Debugger.metadata["FRAMEWORK"]}',
-                                                html=Debugger.pages["HOME"], js_api=Debugger.api, height=300, width=600,
-                                                resizable=False)
+                                                html=Debugger.pages["HOME"], js_api=Debugger.api,
+                                                height=300, width=600, resizable=False)
         Debugger.api.set_window(Debugger.window)
         Debugger.api.set_pages(Debugger.pages)
         webview.start()
 
     @classmethod
     def normalizer_metadata(cls, metadata):
         # agregar condicion (de validacion)
@@ -314,15 +324,15 @@
                             <path d="M432.333 267.6C430.467 267.867 376.867 274.933 313 283.467C249.267 291.867 192.467 299.867 186.867 301.333C131 315.067 89 359.2 77 416.667C74.0667 430.933 74.0667 458.4 77 472.667C83.5333 504.267 97.8 529.867 121.133 552C132.867 563.2 141.667 569.333 156.333 576.667C176.867 586.933 191.4 590.667 215.667 591.6C233.933 592.267 236.867 591.867 355.4 576C440.6 564.667 479.933 558.8 488.067 556.533C528.2 545.067 563.533 514.667 581 476.933C614.467 404.533 584.2 318.267 512.6 282.133C490.467 270.933 453.267 264.133 432.333 267.6ZM477.533 293.333C520.467 303.733 554.333 336.667 567.8 380.8C571.133 391.6 571.4 394.667 571.533 414C571.533 431.867 571 437.067 568.6 446C565 459.2 556.733 476.533 549 487.333C540.2 499.6 522.467 515.733 509.533 523.067C487.8 535.333 486.467 535.6 353.4 553.333C274.2 563.867 229 569.333 221.133 569.333C162.867 569.2 112.067 527.2 100.067 469.333C96.6 452.933 97.4 427.2 101.667 412C113.667 369.467 146.333 336.4 187.933 324.667C196.067 322.4 235.267 316.667 315 306.133C378.467 297.733 432.2 290.533 434.333 290.133C442.333 288.933 466.6 290.667 477.533 293.333Z" fill="#D71920"/>
                             <path d="M502.733 338.8C501.4 339.467 494.6 347.733 487.533 357.067C480.333 366.4 473.8 374.8 472.867 375.867C471.533 377.333 468.067 375.2 452.733 363.6C442.6 355.867 433 349.2 431.4 348.8C427.267 347.467 421 351.067 419 356C416.333 362.4 419 366.267 432.6 376.667C439.4 381.867 447.8 388.267 451.267 391.067L457.667 396.133L443 415.467C427.267 436.133 426.067 439.333 431 445.733C434.2 449.733 439 451.067 443.533 449.467C445.4 448.667 452.6 440.4 461 429.333C468.733 419.067 475.533 410.667 476.067 410.667C476.6 410.667 484.867 416.8 494.333 424.133C503.933 431.6 513.133 438.133 514.867 438.8C523.667 442.267 532.467 432 528.067 423.467C527.133 421.6 518.067 413.733 507.933 406L489.533 391.733L493.267 386.933C495.267 384.133 501.933 375.467 507.933 367.467C516.467 356.4 519 352.133 519 348.8C518.867 340.4 509.667 334.667 502.733 338.8Z" fill="#D71920"/>
                             <path d="M221.667 376.4C219.8 377.333 212.067 386.133 204.467 396C196.867 405.867 190.2 414.133 189.533 414.4C189 414.667 180.2 408.533 170.067 400.8C154.6 388.933 150.733 386.667 146.867 386.667C140.6 386.667 136.333 391.067 136.333 397.467C136.333 403.333 137.4 404.533 158.067 420C167.267 426.933 174.867 433.067 175 433.6C175 434.133 169.133 442.267 161.933 451.6C147.4 470.533 145.667 473.2 145.667 477.333C145.667 480.933 152.6 488 156.2 488C161.8 488 165.4 484.667 179 466.667C186.733 456.4 193.4 448.133 193.8 448C194.333 448 202.067 453.733 211.133 460.8C233.667 478.267 236.733 479.467 244.067 472.933C247.267 470 247.933 464.267 245.667 460C244.867 458.533 236.333 451.333 226.6 444C217 436.533 208.867 430 208.6 429.467C208.467 428.933 214.6 420.133 222.333 410C230.067 399.867 236.733 390.267 237.133 388.667C238.2 384.133 234.333 377.867 229.533 376.133C227.133 375.333 225.267 374.667 225.133 374.667C225 374.667 223.533 375.467 221.667 376.4Z" fill="#D71920"/>
                             <path d="M330.733 477.333C311.8 482.8 296.2 492 284.067 505.067C276.6 513.067 275.667 518.133 281 523.333C286.733 529.2 292.2 528 302.333 518.667C313.133 508.933 322.067 503.733 334.867 500C352.333 494.667 374.6 497.867 391.133 508C398.867 512.667 403.933 513.067 408.867 509.2C413.8 505.333 413.8 497.2 408.733 492.533C403.4 487.6 387.667 480.4 375.8 477.333C362.067 473.867 343.133 473.867 330.733 477.333Z" fill="#D71920"/>
                             </svg>
                     </div>
                     <div class="container-message">
-                        <p>Clave: <b>{Debugger.metadata["EXCEPTION"]}</b></p>
+                        <p>Clave: <b class="exception">{Debugger.metadata["EXCEPTION"]}</b></p>
                         <p class="message">{Debugger.metadata["MESSAGE"]}</p>
                     </div>
                     <div class="container-buttons">   
                         <button class="btn" onClick="retry()">Reintentar</button>
                         <button class="btn" onClick="refactor()">Refactorizar</button>
                         <button class="btn btn-red" onClick="report()">Reportar</button>
                     </div>
@@ -437,8 +447,8 @@
 
     def set_code(self, new_code):
         Api.code = new_code
 
     @classmethod
     def normalizer_json(cls, entity):
         entity = entity.replace("&lt;", "<").replace("&gt;", ">")
-        return entity
+        return entity
```

#### html2text {}

```diff
@@ -8,18 +8,18 @@
 div/div/input", "JSON PATH": "C:\testing-
 automation\projects\Fisa\src\pages\Login.json", "JSON STRING": {'
 [                    ]_Nombre_de_usuario': {'GetFieldBy': 'Xpath',
 'ValueToFind': "//input[@id='inputEmail']"}, '[                    ]_Password':
 {'GetFieldBy': 'Xpath', 'ValueToFind': "//input[@id='inputPassword']"}}, "CASE
 NAME": "test_000_alta_de_usuario_fulano" } """ def __init__(self, metadata) -
 > None: Debugger.metadata = Debugger.normalizer_metadata(metadata) Debugger.api
-= Api() Debugger.pages = Debugger.build_pages() Debugger.window =
-webview.create_window(f'Debugger 3.0 - {Debugger.metadata["FRAMEWORK"]}',
-html=Debugger.pages["HOME"], js_api=Debugger.api, height=300, width=600,
-resizable=False) Debugger.api.set_window(Debugger.window)
+= Api() Debugger.api.set_code(2) Debugger.pages = Debugger.build_pages()
+Debugger.window = webview.create_window(f'Debugger 3.0 - {Debugger.metadata
+["FRAMEWORK"]}', html=Debugger.pages["HOME"], js_api=Debugger.api, height=300,
+width=600, resizable=False) Debugger.api.set_window(Debugger.window)
 Debugger.api.set_pages(Debugger.pages) webview.start() @classmethod def
 normalizer_metadata(cls, metadata): # agregar condicion (de validacion) with
 open(metadata["JSON PATH"], "r", encoding='utf8') as read_file: metadata["JSON
 STRING"] = json.loads(read_file.read()) read_file.close() metadata["MESSAGE"] =
 str(metadata["MESSAGE"]).split("--")[-1].replace("<", "<").replace(">", ">")
 metadata["ENTITY"] = (str(metadata["ENTITY"]).replace("<", "<")).replace(">",
 ">") metadata["JSON"] = str(metadata["JSON PATH"]).split("\\")[-1] return
```

### Comparing `Andreani_QA_Debugger-0.0.3/setup.py` & `Andreani_QA_Debugger-0.0.4/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 PACKAGE_NAME = 'Andreani_QA_Debugger'  # Debe coincidir con el nombre de la carpeta
-AUTHOR = 'Andreani_Testing_Automation_QA'
+AUTHOR = 'AndreaniTesting'
 AUTHOR_EMAIL = 'user_appglatest@andreani.com'
 URL = ''
 
 LICENSE = 'MIT'  # Tipo de licencia
 DESCRIPTION = 'Debugger para ejecución de casos automatizados'  # Descripción corta
 LONG_DESCRIPTION = ""  # Referencia al documento README con una descripción más elaborada
 LONG_DESC_TYPE = "text/markdown"
 
 # Paquetes necesarios para que funcione la libreía. Se instalarán a la vez si no lo tuvieras ya instalado
 INSTALL_REQUIRES = [
-    'Andreani-QA-Parameters', 'Andreani-QA-Functions', 'pywebview'
+    'pywebview'
 ]
 
 setup(
     name=PACKAGE_NAME,
     version=VERSION,
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
```

