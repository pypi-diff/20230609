# Comparing `tmp/pydantic-yaml-parser-0.0.1.tar.gz` & `tmp/pydantic-yaml-parser-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic-yaml-parser-0.0.1.tar", last modified: Fri Jun  9 04:55:01 2023, max compression
+gzip compressed data, was "pydantic-yaml-parser-0.0.2.tar", last modified: Fri Jun  9 04:58:42 2023, max compression
```

## Comparing `pydantic-yaml-parser-0.0.1.tar` & `pydantic-yaml-parser-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-06-09 04:55:01.597706 pydantic-yaml-parser-0.0.1/
--rw-rw-r--   0 hamel      (501) staff       (20)    11337 2023-04-27 10:12:58.000000 pydantic-yaml-parser-0.0.1/LICENSE
--rw-rw-r--   0 hamel      (501) staff       (20)      111 2023-04-27 10:12:58.000000 pydantic-yaml-parser-0.0.1/MANIFEST.in
--rw-r--r--   0 hamel      (501) staff       (20)     3171 2023-06-09 04:55:01.597561 pydantic-yaml-parser-0.0.1/PKG-INFO
--rw-r--r--   0 hamel      (501) staff       (20)     2371 2023-06-09 04:53:58.000000 pydantic-yaml-parser-0.0.1/README.md
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-06-09 04:55:01.596209 pydantic-yaml-parser-0.0.1/pydantic_yaml_parser/
--rw-r--r--   0 hamel      (501) staff       (20)       22 2023-06-09 04:52:44.000000 pydantic-yaml-parser-0.0.1/pydantic_yaml_parser/__init__.py
--rw-r--r--   0 hamel      (501) staff       (20)     1239 2023-06-09 04:52:44.000000 pydantic-yaml-parser-0.0.1/pydantic_yaml_parser/_modidx.py
--rw-r--r--   0 hamel      (501) staff       (20)     1689 2023-06-09 04:52:44.000000 pydantic-yaml-parser-0.0.1/pydantic_yaml_parser/yaml.py
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-06-09 04:55:01.597375 pydantic-yaml-parser-0.0.1/pydantic_yaml_parser.egg-info/
--rw-r--r--   0 hamel      (501) staff       (20)     3171 2023-06-09 04:55:01.000000 pydantic-yaml-parser-0.0.1/pydantic_yaml_parser.egg-info/PKG-INFO
--rw-r--r--   0 hamel      (501) staff       (20)      454 2023-06-09 04:55:01.000000 pydantic-yaml-parser-0.0.1/pydantic_yaml_parser.egg-info/SOURCES.txt
--rw-r--r--   0 hamel      (501) staff       (20)        1 2023-06-09 04:55:01.000000 pydantic-yaml-parser-0.0.1/pydantic_yaml_parser.egg-info/dependency_links.txt
--rw-r--r--   0 hamel      (501) staff       (20)       62 2023-06-09 04:55:01.000000 pydantic-yaml-parser-0.0.1/pydantic_yaml_parser.egg-info/entry_points.txt
--rw-r--r--   0 hamel      (501) staff       (20)        1 2023-06-09 04:16:50.000000 pydantic-yaml-parser-0.0.1/pydantic_yaml_parser.egg-info/not-zip-safe
--rw-r--r--   0 hamel      (501) staff       (20)       32 2023-06-09 04:55:01.000000 pydantic-yaml-parser-0.0.1/pydantic_yaml_parser.egg-info/requires.txt
--rw-r--r--   0 hamel      (501) staff       (20)       21 2023-06-09 04:55:01.000000 pydantic-yaml-parser-0.0.1/pydantic_yaml_parser.egg-info/top_level.txt
--rw-r--r--   0 hamel      (501) staff       (20)      968 2023-06-09 04:48:10.000000 pydantic-yaml-parser-0.0.1/settings.ini
--rw-r--r--   0 hamel      (501) staff       (20)       38 2023-06-09 04:55:01.597752 pydantic-yaml-parser-0.0.1/setup.cfg
--rw-rw-r--   0 hamel      (501) staff       (20)     2596 2023-04-27 10:12:58.000000 pydantic-yaml-parser-0.0.1/setup.py
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-06-09 04:58:42.802803 pydantic-yaml-parser-0.0.2/
+-rw-rw-r--   0 hamel      (501) staff       (20)    11337 2023-04-27 10:12:58.000000 pydantic-yaml-parser-0.0.2/LICENSE
+-rw-rw-r--   0 hamel      (501) staff       (20)      111 2023-04-27 10:12:58.000000 pydantic-yaml-parser-0.0.2/MANIFEST.in
+-rw-r--r--   0 hamel      (501) staff       (20)     3006 2023-06-09 04:58:42.802642 pydantic-yaml-parser-0.0.2/PKG-INFO
+-rw-r--r--   0 hamel      (501) staff       (20)     2206 2023-06-09 04:58:15.000000 pydantic-yaml-parser-0.0.2/README.md
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-06-09 04:58:42.801320 pydantic-yaml-parser-0.0.2/pydantic_yaml_parser/
+-rw-r--r--   0 hamel      (501) staff       (20)       22 2023-06-09 04:58:02.000000 pydantic-yaml-parser-0.0.2/pydantic_yaml_parser/__init__.py
+-rw-r--r--   0 hamel      (501) staff       (20)     1239 2023-06-09 04:58:02.000000 pydantic-yaml-parser-0.0.2/pydantic_yaml_parser/_modidx.py
+-rw-r--r--   0 hamel      (501) staff       (20)     1689 2023-06-09 04:58:02.000000 pydantic-yaml-parser-0.0.2/pydantic_yaml_parser/yaml.py
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-06-09 04:58:42.802441 pydantic-yaml-parser-0.0.2/pydantic_yaml_parser.egg-info/
+-rw-r--r--   0 hamel      (501) staff       (20)     3006 2023-06-09 04:58:42.000000 pydantic-yaml-parser-0.0.2/pydantic_yaml_parser.egg-info/PKG-INFO
+-rw-r--r--   0 hamel      (501) staff       (20)      454 2023-06-09 04:58:42.000000 pydantic-yaml-parser-0.0.2/pydantic_yaml_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 hamel      (501) staff       (20)        1 2023-06-09 04:58:42.000000 pydantic-yaml-parser-0.0.2/pydantic_yaml_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 hamel      (501) staff       (20)       62 2023-06-09 04:58:42.000000 pydantic-yaml-parser-0.0.2/pydantic_yaml_parser.egg-info/entry_points.txt
+-rw-r--r--   0 hamel      (501) staff       (20)        1 2023-06-09 04:16:50.000000 pydantic-yaml-parser-0.0.2/pydantic_yaml_parser.egg-info/not-zip-safe
+-rw-r--r--   0 hamel      (501) staff       (20)       32 2023-06-09 04:58:42.000000 pydantic-yaml-parser-0.0.2/pydantic_yaml_parser.egg-info/requires.txt
+-rw-r--r--   0 hamel      (501) staff       (20)       21 2023-06-09 04:58:42.000000 pydantic-yaml-parser-0.0.2/pydantic_yaml_parser.egg-info/top_level.txt
+-rw-r--r--   0 hamel      (501) staff       (20)      968 2023-06-09 04:57:53.000000 pydantic-yaml-parser-0.0.2/settings.ini
+-rw-r--r--   0 hamel      (501) staff       (20)       38 2023-06-09 04:58:42.802879 pydantic-yaml-parser-0.0.2/setup.cfg
+-rw-rw-r--   0 hamel      (501) staff       (20)     2596 2023-04-27 10:12:58.000000 pydantic-yaml-parser-0.0.2/setup.py
```

### Comparing `pydantic-yaml-parser-0.0.1/LICENSE` & `pydantic-yaml-parser-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic-yaml-parser-0.0.1/PKG-INFO` & `pydantic-yaml-parser-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-yaml-parser
-Version: 0.0.1
+Version: 0.0.2
 Summary: parse yaml files with pydantic
 Home-page: https://github.com/hamelsmu/pydantic-yaml-parser
 Author: Hamel Husain
 Author-email: hamel.husain@gmail.com
 License: Apache Software License 2.0
 Keywords: pydantic yaml
 Platform: UNKNOWN
@@ -70,24 +70,16 @@
 
 You can load the yaml file into a dict, and into the Pydantic model like
 so:
 
 ``` python
 import yaml
 yml_dict = yaml.safe_load(yaml_string)
-yml_dict
-```
-
-    {'setting_1': 'Hello',
-     'setting_2': [{'kind': 'name', 'sublist': ['first', 'second']}]}
 
-To load this dict into the pydantic model `Test`, you can use
-`parse_obj`:
-
-``` python
+# use `parse_obj` to load a dict
 Test.parse_obj(yml_dict)
 ```
 
     Test(setting_1='Hello', setting_2=[Setting2(kind='name', sublist=['first', 'second'])])
 
 However, let’s say there is an error in your yaml file such that you
 accidentally set `sublist` to `false`, instead of setting `sublist` to
```

### Comparing `pydantic-yaml-parser-0.0.1/README.md` & `pydantic-yaml-parser-0.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -47,24 +47,16 @@
 
 You can load the yaml file into a dict, and into the Pydantic model like
 so:
 
 ``` python
 import yaml
 yml_dict = yaml.safe_load(yaml_string)
-yml_dict
-```
-
-    {'setting_1': 'Hello',
-     'setting_2': [{'kind': 'name', 'sublist': ['first', 'second']}]}
 
-To load this dict into the pydantic model `Test`, you can use
-`parse_obj`:
-
-``` python
+# use `parse_obj` to load a dict
 Test.parse_obj(yml_dict)
 ```
 
     Test(setting_1='Hello', setting_2=[Setting2(kind='name', sublist=['first', 'second'])])
 
 However, let’s say there is an error in your yaml file such that you
 accidentally set `sublist` to `false`, instead of setting `sublist` to
```

### Comparing `pydantic-yaml-parser-0.0.1/pydantic_yaml_parser/_modidx.py` & `pydantic-yaml-parser-0.0.2/pydantic_yaml_parser/_modidx.py`

 * *Files identical despite different names*

### Comparing `pydantic-yaml-parser-0.0.1/pydantic_yaml_parser/yaml.py` & `pydantic-yaml-parser-0.0.2/pydantic_yaml_parser/yaml.py`

 * *Files identical despite different names*

### Comparing `pydantic-yaml-parser-0.0.1/pydantic_yaml_parser.egg-info/PKG-INFO` & `pydantic-yaml-parser-0.0.2/pydantic_yaml_parser.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-yaml-parser
-Version: 0.0.1
+Version: 0.0.2
 Summary: parse yaml files with pydantic
 Home-page: https://github.com/hamelsmu/pydantic-yaml-parser
 Author: Hamel Husain
 Author-email: hamel.husain@gmail.com
 License: Apache Software License 2.0
 Keywords: pydantic yaml
 Platform: UNKNOWN
@@ -70,24 +70,16 @@
 
 You can load the yaml file into a dict, and into the Pydantic model like
 so:
 
 ``` python
 import yaml
 yml_dict = yaml.safe_load(yaml_string)
-yml_dict
-```
-
-    {'setting_1': 'Hello',
-     'setting_2': [{'kind': 'name', 'sublist': ['first', 'second']}]}
 
-To load this dict into the pydantic model `Test`, you can use
-`parse_obj`:
-
-``` python
+# use `parse_obj` to load a dict
 Test.parse_obj(yml_dict)
 ```
 
     Test(setting_1='Hello', setting_2=[Setting2(kind='name', sublist=['first', 'second'])])
 
 However, let’s say there is an error in your yaml file such that you
 accidentally set `sublist` to `false`, instead of setting `sublist` to
```

### Comparing `pydantic-yaml-parser-0.0.1/settings.ini` & `pydantic-yaml-parser-0.0.2/settings.ini`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = pydantic-yaml-parser
 lib_name = %(repo)s
-version = 0.0.1
+version = 0.0.2
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = pydantic_yaml_parser
```

### Comparing `pydantic-yaml-parser-0.0.1/setup.py` & `pydantic-yaml-parser-0.0.2/setup.py`

 * *Files identical despite different names*

