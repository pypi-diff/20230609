# Comparing `tmp/milliman_sensi-1.0.8.tar.gz` & `tmp/milliman_sensi-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\milliman_sensi-1.0.8.tar", last modified: Mon Oct 25 12:28:38 2021, max compression
+gzip compressed data, was "dist\milliman_sensi-1.0.9.tar", last modified: Mon Oct 25 13:25:24 2021, max compression
```

## Comparing `milliman_sensi-1.0.8.tar` & `milliman_sensi-1.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2021-10-25 12:28:38.359624 milliman_sensi-1.0.8/
--rw-rw-rw-   0        0        0     1082 2021-09-30 12:22:12.000000 milliman_sensi-1.0.8/LICENSE.txt
--rw-rw-rw-   0        0        0      863 2021-10-25 12:28:38.359624 milliman_sensi-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       50 2021-09-21 15:06:24.000000 milliman_sensi-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2021-10-25 12:28:38.330635 milliman_sensi-1.0.8/milliman_sensi/
--rw-rw-rw-   0        0        0      339 2021-10-20 11:35:14.000000 milliman_sensi-1.0.8/milliman_sensi/__init__.py
--rw-rw-rw-   0        0        0        0 2021-10-18 08:07:22.000000 milliman_sensi-1.0.8/milliman_sensi/conftest.py
--rw-rw-rw-   0        0        0    17289 2021-10-25 12:22:19.000000 milliman_sensi-1.0.8/milliman_sensi/io.py
--rw-rw-rw-   0        0        0    15808 2021-10-25 12:17:15.000000 milliman_sensi-1.0.8/milliman_sensi/syntax.py
-drwxrwxrwx   0        0        0        0 2021-10-25 12:28:38.358625 milliman_sensi-1.0.8/milliman_sensi.egg-info/
--rw-rw-rw-   0        0        0      863 2021-10-25 12:28:37.000000 milliman_sensi-1.0.8/milliman_sensi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      329 2021-10-25 12:28:38.000000 milliman_sensi-1.0.8/milliman_sensi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-10-25 12:28:38.000000 milliman_sensi-1.0.8/milliman_sensi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2021-10-25 12:28:38.000000 milliman_sensi-1.0.8/milliman_sensi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2021-10-25 12:28:38.000000 milliman_sensi-1.0.8/milliman_sensi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2021-10-25 12:28:38.361626 milliman_sensi-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1260 2021-10-25 12:28:36.000000 milliman_sensi-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2021-10-25 13:25:24.342491 milliman_sensi-1.0.9/
+-rw-rw-rw-   0        0        0     1082 2021-09-30 12:22:12.000000 milliman_sensi-1.0.9/LICENSE.txt
+-rw-rw-rw-   0        0        0      863 2021-10-25 13:25:24.342491 milliman_sensi-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       50 2021-09-21 15:06:24.000000 milliman_sensi-1.0.9/README.md
+drwxrwxrwx   0        0        0        0 2021-10-25 13:25:24.311493 milliman_sensi-1.0.9/milliman_sensi/
+-rw-rw-rw-   0        0        0      339 2021-10-20 11:35:14.000000 milliman_sensi-1.0.9/milliman_sensi/__init__.py
+-rw-rw-rw-   0        0        0        0 2021-10-18 08:07:22.000000 milliman_sensi-1.0.9/milliman_sensi/conftest.py
+-rw-rw-rw-   0        0        0    17303 2021-10-25 13:20:20.000000 milliman_sensi-1.0.9/milliman_sensi/io.py
+-rw-rw-rw-   0        0        0    16127 2021-10-25 13:23:15.000000 milliman_sensi-1.0.9/milliman_sensi/syntax.py
+drwxrwxrwx   0        0        0        0 2021-10-25 13:25:24.341491 milliman_sensi-1.0.9/milliman_sensi.egg-info/
+-rw-rw-rw-   0        0        0      863 2021-10-25 13:25:24.000000 milliman_sensi-1.0.9/milliman_sensi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      329 2021-10-25 13:25:24.000000 milliman_sensi-1.0.9/milliman_sensi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-10-25 13:25:24.000000 milliman_sensi-1.0.9/milliman_sensi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2021-10-25 13:25:24.000000 milliman_sensi-1.0.9/milliman_sensi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2021-10-25 13:25:24.000000 milliman_sensi-1.0.9/milliman_sensi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2021-10-25 13:25:24.348493 milliman_sensi-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1260 2021-10-25 13:25:04.000000 milliman_sensi-1.0.9/setup.py
```

### Comparing `milliman_sensi-1.0.8/LICENSE.txt` & `milliman_sensi-1.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `milliman_sensi-1.0.8/PKG-INFO` & `milliman_sensi-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: milliman_sensi
-Version: 1.0.8
+Version: 1.0.9
 Summary: A parser and modifier of the configuration in Milliman-CHESS
 Home-page: https://dev.azure.com/millimanparis/CHESS-Sensitivity-Manager
 Author: Quincy HSIEH
 Author-email: quincy.hsieh@milliman.com
 License: MIT
 Keywords: Milliman CHESS,configuration,parsers,sensitibity
 Platform: UNKNOWN
```

### Comparing `milliman_sensi-1.0.8/milliman_sensi/io.py` & `milliman_sensi-1.0.9/milliman_sensi/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -361,16 +361,16 @@
                                         # Apply the changes to the input file using the syntax
                                         if syn.apply_syntax_to_file(path_to_file, syntax, settings_json_sensi):
                                             processed_sensi_messages[sensi_name] = "OK"
                                         else:
                                             # print("Failed to apply a syntax to {}".format(path_to_file))
                                             processed_sensi_messages[sensi_name] = "Error: Failed to apply a modification to {}".format(path_to_file)
                                             break
-                                    # else:
-                                    #     raise IOSensiError("Couldn't find the input file at {}".format(path_to_file))
+                                    else:
+                                        processed_sensi_messages[sensi_name] = "Error: Couldn't find the input file from settings.json"
 
                         else:
                             processed_sensi_messages[sensi_name] = "Error: Couldn't find settings.json"
 
                     else:
                         processed_sensi_messages[sensi_name] = "Error: Sensi_dirpath doesn't exist"
```

### Comparing `milliman_sensi-1.0.8/milliman_sensi/syntax.py` & `milliman_sensi-1.0.9/milliman_sensi/syntax.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,15 +130,24 @@
 
     for index in range(len(folder_names)):
         if folder_names[index] in MODEL_DIR_NAMES:
             folder_names[index] = MODEL_DIR_NAMES[folder_names[index]]
 
     if filename:
         local_filepath = "/".join(folder_names + filename)
-        file_path = os.path.join(env_dir, 'resources/Central/RN_inputs', local_filepath).replace('\\', '/')
+
+        # Searches for Table name and consquently the input folders
+        list_subfolders = [f.name for f in os.scandir(os.path.join(env_dir, "resources")) if f.is_dir()]
+
+        if len(list_subfolders) == 1:
+            table_name = list_subfolders[0]
+        else:
+            return None
+
+        file_path = os.path.join(env_dir, 'resources/{}/RN_inputs'.format(table_name), local_filepath).replace('\\', '/')
 
         if not os.path.exists(file_path):
             raise SyntaxSensiError("The input file can't be found at {}".format(file_path))
 
         else:
             input_file_path = file_path
```

### Comparing `milliman_sensi-1.0.8/milliman_sensi.egg-info/PKG-INFO` & `milliman_sensi-1.0.9/milliman_sensi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: milliman-sensi
-Version: 1.0.8
+Version: 1.0.9
 Summary: A parser and modifier of the configuration in Milliman-CHESS
 Home-page: https://dev.azure.com/millimanparis/CHESS-Sensitivity-Manager
 Author: Quincy HSIEH
 Author-email: quincy.hsieh@milliman.com
 License: MIT
 Keywords: Milliman CHESS,configuration,parsers,sensitibity
 Platform: UNKNOWN
```

### Comparing `milliman_sensi-1.0.8/setup.py` & `milliman_sensi-1.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     'Programming Language :: Python :: 3',
     'Programming Language :: Python :: 3.6',
     ]
 
 # calling the setup function
 setup(name='milliman_sensi',
       # version=os.getenv('VERSION_TAG'), # Needs to be %VERSION_TAG% on Windows CMD
-      version="1.0.8",
+      version="1.0.9",
       description='A parser and modifier of the configuration in Milliman-CHESS',
       long_description="""A parser and modifier of CHESS's configuration
 To parse configuration files and apply them to create new sensitivity tables""",
       url='https://dev.azure.com/millimanparis/CHESS-Sensitivity-Manager',
       author='Quincy HSIEH',
       author_email='quincy.hsieh@milliman.com',
       license='MIT',
```

