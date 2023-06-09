# Comparing `tmp/pydantic-yaml-parser-0.0.2.tar.gz` & `tmp/pydantic-yaml-parser-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic-yaml-parser-0.0.2.tar", last modified: Fri Jun  9 04:58:42 2023, max compression
+gzip compressed data, was "pydantic-yaml-parser-0.0.3.tar", last modified: Fri Jun  9 05:03:20 2023, max compression
```

## Comparing `pydantic-yaml-parser-0.0.2.tar` & `pydantic-yaml-parser-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-06-09 04:58:42.802803 pydantic-yaml-parser-0.0.2/
--rw-rw-r--   0 hamel      (501) staff       (20)    11337 2023-04-27 10:12:58.000000 pydantic-yaml-parser-0.0.2/LICENSE
--rw-rw-r--   0 hamel      (501) staff       (20)      111 2023-04-27 10:12:58.000000 pydantic-yaml-parser-0.0.2/MANIFEST.in
--rw-r--r--   0 hamel      (501) staff       (20)     3006 2023-06-09 04:58:42.802642 pydantic-yaml-parser-0.0.2/PKG-INFO
--rw-r--r--   0 hamel      (501) staff       (20)     2206 2023-06-09 04:58:15.000000 pydantic-yaml-parser-0.0.2/README.md
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-06-09 04:58:42.801320 pydantic-yaml-parser-0.0.2/pydantic_yaml_parser/
--rw-r--r--   0 hamel      (501) staff       (20)       22 2023-06-09 04:58:02.000000 pydantic-yaml-parser-0.0.2/pydantic_yaml_parser/__init__.py
--rw-r--r--   0 hamel      (501) staff       (20)     1239 2023-06-09 04:58:02.000000 pydantic-yaml-parser-0.0.2/pydantic_yaml_parser/_modidx.py
--rw-r--r--   0 hamel      (501) staff       (20)     1689 2023-06-09 04:58:02.000000 pydantic-yaml-parser-0.0.2/pydantic_yaml_parser/yaml.py
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-06-09 04:58:42.802441 pydantic-yaml-parser-0.0.2/pydantic_yaml_parser.egg-info/
--rw-r--r--   0 hamel      (501) staff       (20)     3006 2023-06-09 04:58:42.000000 pydantic-yaml-parser-0.0.2/pydantic_yaml_parser.egg-info/PKG-INFO
--rw-r--r--   0 hamel      (501) staff       (20)      454 2023-06-09 04:58:42.000000 pydantic-yaml-parser-0.0.2/pydantic_yaml_parser.egg-info/SOURCES.txt
--rw-r--r--   0 hamel      (501) staff       (20)        1 2023-06-09 04:58:42.000000 pydantic-yaml-parser-0.0.2/pydantic_yaml_parser.egg-info/dependency_links.txt
--rw-r--r--   0 hamel      (501) staff       (20)       62 2023-06-09 04:58:42.000000 pydantic-yaml-parser-0.0.2/pydantic_yaml_parser.egg-info/entry_points.txt
--rw-r--r--   0 hamel      (501) staff       (20)        1 2023-06-09 04:16:50.000000 pydantic-yaml-parser-0.0.2/pydantic_yaml_parser.egg-info/not-zip-safe
--rw-r--r--   0 hamel      (501) staff       (20)       32 2023-06-09 04:58:42.000000 pydantic-yaml-parser-0.0.2/pydantic_yaml_parser.egg-info/requires.txt
--rw-r--r--   0 hamel      (501) staff       (20)       21 2023-06-09 04:58:42.000000 pydantic-yaml-parser-0.0.2/pydantic_yaml_parser.egg-info/top_level.txt
--rw-r--r--   0 hamel      (501) staff       (20)      968 2023-06-09 04:57:53.000000 pydantic-yaml-parser-0.0.2/settings.ini
--rw-r--r--   0 hamel      (501) staff       (20)       38 2023-06-09 04:58:42.802879 pydantic-yaml-parser-0.0.2/setup.cfg
--rw-rw-r--   0 hamel      (501) staff       (20)     2596 2023-04-27 10:12:58.000000 pydantic-yaml-parser-0.0.2/setup.py
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-06-09 05:03:20.832360 pydantic-yaml-parser-0.0.3/
+-rw-rw-r--   0 hamel      (501) staff       (20)    11337 2023-04-27 10:12:58.000000 pydantic-yaml-parser-0.0.3/LICENSE
+-rw-rw-r--   0 hamel      (501) staff       (20)      111 2023-04-27 10:12:58.000000 pydantic-yaml-parser-0.0.3/MANIFEST.in
+-rw-r--r--   0 hamel      (501) staff       (20)     3234 2023-06-09 05:03:20.832205 pydantic-yaml-parser-0.0.3/PKG-INFO
+-rw-r--r--   0 hamel      (501) staff       (20)     2434 2023-06-09 05:03:05.000000 pydantic-yaml-parser-0.0.3/README.md
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-06-09 05:03:20.831030 pydantic-yaml-parser-0.0.3/pydantic_yaml_parser/
+-rw-r--r--   0 hamel      (501) staff       (20)       22 2023-06-09 05:03:12.000000 pydantic-yaml-parser-0.0.3/pydantic_yaml_parser/__init__.py
+-rw-r--r--   0 hamel      (501) staff       (20)     1239 2023-06-09 05:03:12.000000 pydantic-yaml-parser-0.0.3/pydantic_yaml_parser/_modidx.py
+-rw-r--r--   0 hamel      (501) staff       (20)     1689 2023-06-09 05:03:12.000000 pydantic-yaml-parser-0.0.3/pydantic_yaml_parser/yaml.py
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-06-09 05:03:20.832007 pydantic-yaml-parser-0.0.3/pydantic_yaml_parser.egg-info/
+-rw-r--r--   0 hamel      (501) staff       (20)     3234 2023-06-09 05:03:20.000000 pydantic-yaml-parser-0.0.3/pydantic_yaml_parser.egg-info/PKG-INFO
+-rw-r--r--   0 hamel      (501) staff       (20)      454 2023-06-09 05:03:20.000000 pydantic-yaml-parser-0.0.3/pydantic_yaml_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 hamel      (501) staff       (20)        1 2023-06-09 05:03:20.000000 pydantic-yaml-parser-0.0.3/pydantic_yaml_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 hamel      (501) staff       (20)       62 2023-06-09 05:03:20.000000 pydantic-yaml-parser-0.0.3/pydantic_yaml_parser.egg-info/entry_points.txt
+-rw-r--r--   0 hamel      (501) staff       (20)        1 2023-06-09 04:16:50.000000 pydantic-yaml-parser-0.0.3/pydantic_yaml_parser.egg-info/not-zip-safe
+-rw-r--r--   0 hamel      (501) staff       (20)       32 2023-06-09 05:03:20.000000 pydantic-yaml-parser-0.0.3/pydantic_yaml_parser.egg-info/requires.txt
+-rw-r--r--   0 hamel      (501) staff       (20)       21 2023-06-09 05:03:20.000000 pydantic-yaml-parser-0.0.3/pydantic_yaml_parser.egg-info/top_level.txt
+-rw-r--r--   0 hamel      (501) staff       (20)      968 2023-06-09 05:03:08.000000 pydantic-yaml-parser-0.0.3/settings.ini
+-rw-r--r--   0 hamel      (501) staff       (20)       38 2023-06-09 05:03:20.832402 pydantic-yaml-parser-0.0.3/setup.cfg
+-rw-rw-r--   0 hamel      (501) staff       (20)     2596 2023-04-27 10:12:58.000000 pydantic-yaml-parser-0.0.3/setup.py
```

### Comparing `pydantic-yaml-parser-0.0.2/LICENSE` & `pydantic-yaml-parser-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic-yaml-parser-0.0.2/PKG-INFO` & `pydantic-yaml-parser-0.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-yaml-parser
-Version: 0.0.2
+Version: 0.0.3
 Summary: parse yaml files with pydantic
 Home-page: https://github.com/hamelsmu/pydantic-yaml-parser
 Author: Hamel Husain
 Author-email: hamel.husain@gmail.com
 License: Apache Software License 2.0
 Keywords: pydantic yaml
 Platform: UNKNOWN
@@ -35,16 +35,18 @@
 
 ``` sh
 pip install pydantic_yaml_parser
 ```
 
 ## Background & Usage
 
+### 1. Loading YAML into Pydantic models
+
 To load YAML into a Pydantic model, you have to first convert the YAML
-to a dict. For example, given the below yaml file:
+string to a dict. For example, given the below yaml file:
 
 ``` python
 yaml_string="""
 setting_1: Hello
 setting_2:
     - kind: name
       sublist:
@@ -65,26 +67,28 @@
 
 class Test(BaseModel):
     setting_1: str
     setting_2: List[Setting2]
 ```
 
 You can load the yaml file into a dict, and into the Pydantic model like
-so:
+so using [pyyaml](https://pyyaml.org/wiki/PyYAMLDocumentation):
 
 ``` python
 import yaml
 yml_dict = yaml.safe_load(yaml_string)
 
 # use `parse_obj` to load a dict
 Test.parse_obj(yml_dict)
 ```
 
     Test(setting_1='Hello', setting_2=[Setting2(kind='name', sublist=['first', 'second'])])
 
+### 2. The Pydantic validation error message
+
 However, let’s say there is an error in your yaml file such that you
 accidentally set `sublist` to `false`, instead of setting `sublist` to
 `list` type, you will get an error message that looks like this:
 
 ``` python
 yaml_string="""
 setting_1: ok
@@ -100,16 +104,20 @@
 ```
 
     ValidationError: 1 validation error for Test
     setting_2 -> 0 -> sublist
       value is not a valid list (type=type_error.list)
 
 This error message is a bit confusing, especially for those with no
-prior experience with pydantic! However when you use
-`pydantic_yaml_parser` you get something a bit clearer:
+prior experience with pydantic!
+
+### 3. Human readable error messages with `pydantic_yaml_parser`
+
+When you use `pydantic_yaml_parser` you get an error message that is
+much clearer:
 
 ``` python
 from pydantic_yaml_parser.yaml import YamlModel
 
 class Test(YamlModel):
     setting_1: str
     setting_2: List[Setting2]
```

### Comparing `pydantic-yaml-parser-0.0.2/README.md` & `pydantic-yaml-parser-0.0.3/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -12,16 +12,18 @@
 
 ``` sh
 pip install pydantic_yaml_parser
 ```
 
 ## Background & Usage
 
+### 1. Loading YAML into Pydantic models
+
 To load YAML into a Pydantic model, you have to first convert the YAML
-to a dict. For example, given the below yaml file:
+string to a dict. For example, given the below yaml file:
 
 ``` python
 yaml_string="""
 setting_1: Hello
 setting_2:
     - kind: name
       sublist:
@@ -42,26 +44,28 @@
 
 class Test(BaseModel):
     setting_1: str
     setting_2: List[Setting2]
 ```
 
 You can load the yaml file into a dict, and into the Pydantic model like
-so:
+so using [pyyaml](https://pyyaml.org/wiki/PyYAMLDocumentation):
 
 ``` python
 import yaml
 yml_dict = yaml.safe_load(yaml_string)
 
 # use `parse_obj` to load a dict
 Test.parse_obj(yml_dict)
 ```
 
     Test(setting_1='Hello', setting_2=[Setting2(kind='name', sublist=['first', 'second'])])
 
+### 2. The Pydantic validation error message
+
 However, let’s say there is an error in your yaml file such that you
 accidentally set `sublist` to `false`, instead of setting `sublist` to
 `list` type, you will get an error message that looks like this:
 
 ``` python
 yaml_string="""
 setting_1: ok
@@ -77,16 +81,20 @@
 ```
 
     ValidationError: 1 validation error for Test
     setting_2 -> 0 -> sublist
       value is not a valid list (type=type_error.list)
 
 This error message is a bit confusing, especially for those with no
-prior experience with pydantic! However when you use
-`pydantic_yaml_parser` you get something a bit clearer:
+prior experience with pydantic!
+
+### 3. Human readable error messages with `pydantic_yaml_parser`
+
+When you use `pydantic_yaml_parser` you get an error message that is
+much clearer:
 
 ``` python
 from pydantic_yaml_parser.yaml import YamlModel
 
 class Test(YamlModel):
     setting_1: str
     setting_2: List[Setting2]
```

### Comparing `pydantic-yaml-parser-0.0.2/pydantic_yaml_parser/_modidx.py` & `pydantic-yaml-parser-0.0.3/pydantic_yaml_parser/_modidx.py`

 * *Files identical despite different names*

### Comparing `pydantic-yaml-parser-0.0.2/pydantic_yaml_parser/yaml.py` & `pydantic-yaml-parser-0.0.3/pydantic_yaml_parser/yaml.py`

 * *Files identical despite different names*

### Comparing `pydantic-yaml-parser-0.0.2/pydantic_yaml_parser.egg-info/PKG-INFO` & `pydantic-yaml-parser-0.0.3/pydantic_yaml_parser.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-yaml-parser
-Version: 0.0.2
+Version: 0.0.3
 Summary: parse yaml files with pydantic
 Home-page: https://github.com/hamelsmu/pydantic-yaml-parser
 Author: Hamel Husain
 Author-email: hamel.husain@gmail.com
 License: Apache Software License 2.0
 Keywords: pydantic yaml
 Platform: UNKNOWN
@@ -35,16 +35,18 @@
 
 ``` sh
 pip install pydantic_yaml_parser
 ```
 
 ## Background & Usage
 
+### 1. Loading YAML into Pydantic models
+
 To load YAML into a Pydantic model, you have to first convert the YAML
-to a dict. For example, given the below yaml file:
+string to a dict. For example, given the below yaml file:
 
 ``` python
 yaml_string="""
 setting_1: Hello
 setting_2:
     - kind: name
       sublist:
@@ -65,26 +67,28 @@
 
 class Test(BaseModel):
     setting_1: str
     setting_2: List[Setting2]
 ```
 
 You can load the yaml file into a dict, and into the Pydantic model like
-so:
+so using [pyyaml](https://pyyaml.org/wiki/PyYAMLDocumentation):
 
 ``` python
 import yaml
 yml_dict = yaml.safe_load(yaml_string)
 
 # use `parse_obj` to load a dict
 Test.parse_obj(yml_dict)
 ```
 
     Test(setting_1='Hello', setting_2=[Setting2(kind='name', sublist=['first', 'second'])])
 
+### 2. The Pydantic validation error message
+
 However, let’s say there is an error in your yaml file such that you
 accidentally set `sublist` to `false`, instead of setting `sublist` to
 `list` type, you will get an error message that looks like this:
 
 ``` python
 yaml_string="""
 setting_1: ok
@@ -100,16 +104,20 @@
 ```
 
     ValidationError: 1 validation error for Test
     setting_2 -> 0 -> sublist
       value is not a valid list (type=type_error.list)
 
 This error message is a bit confusing, especially for those with no
-prior experience with pydantic! However when you use
-`pydantic_yaml_parser` you get something a bit clearer:
+prior experience with pydantic!
+
+### 3. Human readable error messages with `pydantic_yaml_parser`
+
+When you use `pydantic_yaml_parser` you get an error message that is
+much clearer:
 
 ``` python
 from pydantic_yaml_parser.yaml import YamlModel
 
 class Test(YamlModel):
     setting_1: str
     setting_2: List[Setting2]
```

### Comparing `pydantic-yaml-parser-0.0.2/settings.ini` & `pydantic-yaml-parser-0.0.3/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = pydantic-yaml-parser
 lib_name = %(repo)s
-version = 0.0.2
+version = 0.0.3
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = pydantic_yaml_parser
```

### Comparing `pydantic-yaml-parser-0.0.2/setup.py` & `pydantic-yaml-parser-0.0.3/setup.py`

 * *Files identical despite different names*

