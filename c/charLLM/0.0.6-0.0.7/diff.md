# Comparing `tmp/charLLM-0.0.6.tar.gz` & `tmp/charLLM-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "charLLM-0.0.6.tar", last modified: Fri Jun  9 14:31:28 2023, max compression
+gzip compressed data, was "charLLM-0.0.7.tar", last modified: Fri Jun  9 14:45:24 2023, max compression
```

## Comparing `charLLM-0.0.6.tar` & `charLLM-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:31:28.699500 charLLM-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11413 2023-06-09 14:28:45.000000 charLLM-0.0.6/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-06-09 14:31:28.699500 charLLM-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-06-09 14:28:45.000000 charLLM-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-09 14:28:45.000000 charLLM-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-09 14:31:28.699500 charLLM-0.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:31:28.695500 charLLM-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:31:28.695500 charLLM-0.0.6/src/charLLM/
--rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-06-09 14:28:45.000000 charLLM-0.0.6/src/charLLM/NPLM.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-09 14:28:45.000000 charLLM-0.0.6/src/charLLM/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:31:28.699500 charLLM-0.0.6/src/charLLM.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-06-09 14:31:28.000000 charLLM-0.0.6/src/charLLM.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-09 14:31:28.000000 charLLM-0.0.6/src/charLLM.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 14:31:28.000000 charLLM-0.0.6/src/charLLM.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-09 14:31:28.000000 charLLM-0.0.6/src/charLLM.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:45:24.007901 charLLM-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11413 2023-06-09 14:43:22.000000 charLLM-0.0.7/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-06-09 14:45:24.007901 charLLM-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-06-09 14:43:22.000000 charLLM-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-09 14:43:22.000000 charLLM-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-09 14:45:24.007901 charLLM-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:45:24.007901 charLLM-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:45:24.007901 charLLM-0.0.7/src/charLLM/
+-rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-06-09 14:43:22.000000 charLLM-0.0.7/src/charLLM/NPLM.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-09 14:43:22.000000 charLLM-0.0.7/src/charLLM/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:45:24.007901 charLLM-0.0.7/src/charLLM.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-06-09 14:45:23.000000 charLLM-0.0.7/src/charLLM.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-09 14:45:24.000000 charLLM-0.0.7/src/charLLM.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 14:45:23.000000 charLLM-0.0.7/src/charLLM.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-09 14:45:23.000000 charLLM-0.0.7/src/charLLM.egg-info/top_level.txt
```

### Comparing `charLLM-0.0.6/LICENCE` & `charLLM-0.0.7/LICENCE`

 * *Files identical despite different names*

### Comparing `charLLM-0.0.6/PKG-INFO` & `charLLM-0.0.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: charLLM
-Version: 0.0.6
+Version: 0.0.7
 Summary: Character Level Language Models 🕺🏽
 Home-page: https://github.com/RAravindDS/CharLLMs
 Author: Aravind
 Author-email: aravindan22052001@gmail.com
 Project-URL: Bug Tracker, https://github.com/RAravindDS/CharLLMs/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
 <p align="center">
-  <picture>
-    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/RAravindDS/CharLLMs/main/images/charllms.webp" width=300>
-    <img alt="PYPI Package Link" src="https://pypi.org/project/charLLM/" width="352" height="59" style="max-width: 100%;">
-  </picture>
+  <img src="https://raw.githubusercontent.com/RAravindDS/CharLLMs/main/images/charllms.webp" height=300>
   <br/>
   <br/>
 </p>
 
 
+
+
 # **Character-Level Language Models Repo 🕺🏽**
 
 This repository contains multiple character-level language models (charLLM). Each language model is designed to generate text at the character level, providing a granular level of control and flexibility.
 
 
 ## 🌟 Available Language Models 
 
@@ -89,19 +88,19 @@
     }
 >>> obj = NPLM(text_path, model_parameters)  # Initialize the class 
 >>> obj.train_model() 
 ## It outputs the val_loss and image 
 >>> obj.sampling(words_needed=10) #It samples 10 tokens. 
 ```
 
-<br>
-<center><b>Model Output Graph<b></center>
-<br>
-<center><img src="https://raw.githubusercontent.com/RAravindDS/CharLLMs/main/images/nplm_plt.png" height=350></center>
-<br>
+
+**Model Output Graph**
+
+
+<img src="https://raw.githubusercontent.com/RAravindDS/CharLLMs/main/images/nplm_plt.png" height=350>
 
 
 Feel free to explore the repository and experiment with the different language models provided.
 
 ## Contributions
 
 Contributions to this repository are welcome. If you have implemented a novel character-level language model or would like to enhance the existing models, please consider contributing to the project.
```

### Comparing `charLLM-0.0.6/README.md` & `charLLM-0.0.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 <p align="center">
-  <picture>
-    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/RAravindDS/CharLLMs/main/images/charllms.webp" width=300>
-    <img alt="PYPI Package Link" src="https://pypi.org/project/charLLM/" width="352" height="59" style="max-width: 100%;">
-  </picture>
+  <img src="https://raw.githubusercontent.com/RAravindDS/CharLLMs/main/images/charllms.webp" height=300>
   <br/>
   <br/>
 </p>
 
 
+
+
 # **Character-Level Language Models Repo 🕺🏽**
 
 This repository contains multiple character-level language models (charLLM). Each language model is designed to generate text at the character level, providing a granular level of control and flexibility.
 
 
 ## 🌟 Available Language Models 
 
@@ -74,19 +73,19 @@
     }
 >>> obj = NPLM(text_path, model_parameters)  # Initialize the class 
 >>> obj.train_model() 
 ## It outputs the val_loss and image 
 >>> obj.sampling(words_needed=10) #It samples 10 tokens. 
 ```
 
-<br>
-<center><b>Model Output Graph<b></center>
-<br>
-<center><img src="https://raw.githubusercontent.com/RAravindDS/CharLLMs/main/images/nplm_plt.png" height=350></center>
-<br>
+
+**Model Output Graph**
+
+
+<img src="https://raw.githubusercontent.com/RAravindDS/CharLLMs/main/images/nplm_plt.png" height=350>
 
 
 Feel free to explore the repository and experiment with the different language models provided.
 
 ## Contributions
 
 Contributions to this repository are welcome. If you have implemented a novel character-level language model or would like to enhance the existing models, please consider contributing to the project.
```

### Comparing `charLLM-0.0.6/setup.cfg` & `charLLM-0.0.7/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = charLLM
-version = 0.0.6
+version = 0.0.7
 author = Aravind
 author_email = aravindan22052001@gmail.com
 description = Character Level Language Models 🕺🏽
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/RAravindDS/CharLLMs
 project_urls =
```

### Comparing `charLLM-0.0.6/src/charLLM/NPLM.py` & `charLLM-0.0.7/src/charLLM/NPLM.py`

 * *Files identical despite different names*

### Comparing `charLLM-0.0.6/src/charLLM.egg-info/PKG-INFO` & `charLLM-0.0.7/src/charLLM.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: charLLM
-Version: 0.0.6
+Version: 0.0.7
 Summary: Character Level Language Models 🕺🏽
 Home-page: https://github.com/RAravindDS/CharLLMs
 Author: Aravind
 Author-email: aravindan22052001@gmail.com
 Project-URL: Bug Tracker, https://github.com/RAravindDS/CharLLMs/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
 <p align="center">
-  <picture>
-    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/RAravindDS/CharLLMs/main/images/charllms.webp" width=300>
-    <img alt="PYPI Package Link" src="https://pypi.org/project/charLLM/" width="352" height="59" style="max-width: 100%;">
-  </picture>
+  <img src="https://raw.githubusercontent.com/RAravindDS/CharLLMs/main/images/charllms.webp" height=300>
   <br/>
   <br/>
 </p>
 
 
+
+
 # **Character-Level Language Models Repo 🕺🏽**
 
 This repository contains multiple character-level language models (charLLM). Each language model is designed to generate text at the character level, providing a granular level of control and flexibility.
 
 
 ## 🌟 Available Language Models 
 
@@ -89,19 +88,19 @@
     }
 >>> obj = NPLM(text_path, model_parameters)  # Initialize the class 
 >>> obj.train_model() 
 ## It outputs the val_loss and image 
 >>> obj.sampling(words_needed=10) #It samples 10 tokens. 
 ```
 
-<br>
-<center><b>Model Output Graph<b></center>
-<br>
-<center><img src="https://raw.githubusercontent.com/RAravindDS/CharLLMs/main/images/nplm_plt.png" height=350></center>
-<br>
+
+**Model Output Graph**
+
+
+<img src="https://raw.githubusercontent.com/RAravindDS/CharLLMs/main/images/nplm_plt.png" height=350>
 
 
 Feel free to explore the repository and experiment with the different language models provided.
 
 ## Contributions
 
 Contributions to this repository are welcome. If you have implemented a novel character-level language model or would like to enhance the existing models, please consider contributing to the project.
```

