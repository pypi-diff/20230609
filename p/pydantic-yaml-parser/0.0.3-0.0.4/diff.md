# Comparing `tmp/pydantic-yaml-parser-0.0.3.tar.gz` & `tmp/pydantic-yaml-parser-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic-yaml-parser-0.0.3.tar", last modified: Fri Jun  9 05:03:20 2023, max compression
+gzip compressed data, was "pydantic-yaml-parser-0.0.4.tar", last modified: Fri Jun  9 05:09:35 2023, max compression
```

## Comparing `pydantic-yaml-parser-0.0.3.tar` & `pydantic-yaml-parser-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-06-09 05:03:20.832360 pydantic-yaml-parser-0.0.3/
--rw-rw-r--   0 hamel      (501) staff       (20)    11337 2023-04-27 10:12:58.000000 pydantic-yaml-parser-0.0.3/LICENSE
--rw-rw-r--   0 hamel      (501) staff       (20)      111 2023-04-27 10:12:58.000000 pydantic-yaml-parser-0.0.3/MANIFEST.in
--rw-r--r--   0 hamel      (501) staff       (20)     3234 2023-06-09 05:03:20.832205 pydantic-yaml-parser-0.0.3/PKG-INFO
--rw-r--r--   0 hamel      (501) staff       (20)     2434 2023-06-09 05:03:05.000000 pydantic-yaml-parser-0.0.3/README.md
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-06-09 05:03:20.831030 pydantic-yaml-parser-0.0.3/pydantic_yaml_parser/
--rw-r--r--   0 hamel      (501) staff       (20)       22 2023-06-09 05:03:12.000000 pydantic-yaml-parser-0.0.3/pydantic_yaml_parser/__init__.py
--rw-r--r--   0 hamel      (501) staff       (20)     1239 2023-06-09 05:03:12.000000 pydantic-yaml-parser-0.0.3/pydantic_yaml_parser/_modidx.py
--rw-r--r--   0 hamel      (501) staff       (20)     1689 2023-06-09 05:03:12.000000 pydantic-yaml-parser-0.0.3/pydantic_yaml_parser/yaml.py
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-06-09 05:03:20.832007 pydantic-yaml-parser-0.0.3/pydantic_yaml_parser.egg-info/
--rw-r--r--   0 hamel      (501) staff       (20)     3234 2023-06-09 05:03:20.000000 pydantic-yaml-parser-0.0.3/pydantic_yaml_parser.egg-info/PKG-INFO
--rw-r--r--   0 hamel      (501) staff       (20)      454 2023-06-09 05:03:20.000000 pydantic-yaml-parser-0.0.3/pydantic_yaml_parser.egg-info/SOURCES.txt
--rw-r--r--   0 hamel      (501) staff       (20)        1 2023-06-09 05:03:20.000000 pydantic-yaml-parser-0.0.3/pydantic_yaml_parser.egg-info/dependency_links.txt
--rw-r--r--   0 hamel      (501) staff       (20)       62 2023-06-09 05:03:20.000000 pydantic-yaml-parser-0.0.3/pydantic_yaml_parser.egg-info/entry_points.txt
--rw-r--r--   0 hamel      (501) staff       (20)        1 2023-06-09 04:16:50.000000 pydantic-yaml-parser-0.0.3/pydantic_yaml_parser.egg-info/not-zip-safe
--rw-r--r--   0 hamel      (501) staff       (20)       32 2023-06-09 05:03:20.000000 pydantic-yaml-parser-0.0.3/pydantic_yaml_parser.egg-info/requires.txt
--rw-r--r--   0 hamel      (501) staff       (20)       21 2023-06-09 05:03:20.000000 pydantic-yaml-parser-0.0.3/pydantic_yaml_parser.egg-info/top_level.txt
--rw-r--r--   0 hamel      (501) staff       (20)      968 2023-06-09 05:03:08.000000 pydantic-yaml-parser-0.0.3/settings.ini
--rw-r--r--   0 hamel      (501) staff       (20)       38 2023-06-09 05:03:20.832402 pydantic-yaml-parser-0.0.3/setup.cfg
--rw-rw-r--   0 hamel      (501) staff       (20)     2596 2023-04-27 10:12:58.000000 pydantic-yaml-parser-0.0.3/setup.py
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-06-09 05:09:35.758074 pydantic-yaml-parser-0.0.4/
+-rw-rw-r--   0 hamel      (501) staff       (20)    11337 2023-04-27 10:12:58.000000 pydantic-yaml-parser-0.0.4/LICENSE
+-rw-rw-r--   0 hamel      (501) staff       (20)      111 2023-04-27 10:12:58.000000 pydantic-yaml-parser-0.0.4/MANIFEST.in
+-rw-r--r--   0 hamel      (501) staff       (20)     3343 2023-06-09 05:09:35.757901 pydantic-yaml-parser-0.0.4/PKG-INFO
+-rw-r--r--   0 hamel      (501) staff       (20)     2543 2023-06-09 05:08:33.000000 pydantic-yaml-parser-0.0.4/README.md
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-06-09 05:09:35.756326 pydantic-yaml-parser-0.0.4/pydantic_yaml_parser/
+-rw-r--r--   0 hamel      (501) staff       (20)       22 2023-06-09 05:08:31.000000 pydantic-yaml-parser-0.0.4/pydantic_yaml_parser/__init__.py
+-rw-r--r--   0 hamel      (501) staff       (20)     1241 2023-06-09 05:08:47.000000 pydantic-yaml-parser-0.0.4/pydantic_yaml_parser/_modidx.py
+-rw-r--r--   0 hamel      (501) staff       (20)     1684 2023-06-09 05:08:31.000000 pydantic-yaml-parser-0.0.4/pydantic_yaml_parser/yaml.py
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-06-09 05:09:35.757655 pydantic-yaml-parser-0.0.4/pydantic_yaml_parser.egg-info/
+-rw-r--r--   0 hamel      (501) staff       (20)     3343 2023-06-09 05:09:35.000000 pydantic-yaml-parser-0.0.4/pydantic_yaml_parser.egg-info/PKG-INFO
+-rw-r--r--   0 hamel      (501) staff       (20)      454 2023-06-09 05:09:35.000000 pydantic-yaml-parser-0.0.4/pydantic_yaml_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 hamel      (501) staff       (20)        1 2023-06-09 05:09:35.000000 pydantic-yaml-parser-0.0.4/pydantic_yaml_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 hamel      (501) staff       (20)       62 2023-06-09 05:09:35.000000 pydantic-yaml-parser-0.0.4/pydantic_yaml_parser.egg-info/entry_points.txt
+-rw-r--r--   0 hamel      (501) staff       (20)        1 2023-06-09 04:16:50.000000 pydantic-yaml-parser-0.0.4/pydantic_yaml_parser.egg-info/not-zip-safe
+-rw-r--r--   0 hamel      (501) staff       (20)       32 2023-06-09 05:09:35.000000 pydantic-yaml-parser-0.0.4/pydantic_yaml_parser.egg-info/requires.txt
+-rw-r--r--   0 hamel      (501) staff       (20)       21 2023-06-09 05:09:35.000000 pydantic-yaml-parser-0.0.4/pydantic_yaml_parser.egg-info/top_level.txt
+-rw-r--r--   0 hamel      (501) staff       (20)      968 2023-06-09 05:08:26.000000 pydantic-yaml-parser-0.0.4/settings.ini
+-rw-r--r--   0 hamel      (501) staff       (20)       38 2023-06-09 05:09:35.758121 pydantic-yaml-parser-0.0.4/setup.cfg
+-rw-rw-r--   0 hamel      (501) staff       (20)     2596 2023-04-27 10:12:58.000000 pydantic-yaml-parser-0.0.4/setup.py
```

### Comparing `pydantic-yaml-parser-0.0.3/LICENSE` & `pydantic-yaml-parser-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic-yaml-parser-0.0.3/PKG-INFO` & `pydantic-yaml-parser-0.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-yaml-parser
-Version: 0.0.3
+Version: 0.0.4
 Summary: parse yaml files with pydantic
 Home-page: https://github.com/hamelsmu/pydantic-yaml-parser
 Author: Hamel Husain
 Author-email: hamel.husain@gmail.com
 License: Apache Software License 2.0
 Keywords: pydantic yaml
 Platform: UNKNOWN
@@ -126,8 +126,13 @@
 ``` python
 Test.from_dict(yaml_dict_error)
 ```
 
     ValueError: Configuration error(s) for YAML:
      - value is not a valid list: `sublist` for element 0 in the list for `setting_2`
 
+## Further Reading
+
+For more examples of error validation see [these
+docs](00_yaml.ipynb#error-validation).
+
```

### Comparing `pydantic-yaml-parser-0.0.3/README.md` & `pydantic-yaml-parser-0.0.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -102,7 +102,12 @@
 
 ``` python
 Test.from_dict(yaml_dict_error)
 ```
 
     ValueError: Configuration error(s) for YAML:
      - value is not a valid list: `sublist` for element 0 in the list for `setting_2`
+
+## Further Reading
+
+For more examples of error validation see [these
+docs](00_yaml.ipynb#error-validation).
```

### Comparing `pydantic-yaml-parser-0.0.3/pydantic_yaml_parser/_modidx.py` & `pydantic-yaml-parser-0.0.4/pydantic_yaml_parser/_modidx.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,9 +6,9 @@
                 'git_url': 'https://github.com/hamelsmu/pydantic-yaml-parser',
                 'lib_path': 'pydantic_yaml_parser'},
   'syms': { 'pydantic_yaml_parser.yaml': { 'pydantic_yaml_parser.yaml.QuartoDoc': ('yaml.html#quartodoc', 'pydantic_yaml_parser/yaml.py'),
                                            'pydantic_yaml_parser.yaml.Section': ('yaml.html#section', 'pydantic_yaml_parser/yaml.py'),
                                            'pydantic_yaml_parser.yaml.YamlModel': ('yaml.html#yamlmodel', 'pydantic_yaml_parser/yaml.py'),
                                            'pydantic_yaml_parser.yaml.YamlModel.from_dict': ( 'yaml.html#yamlmodel.from_dict',
                                                                                               'pydantic_yaml_parser/yaml.py'),
-                                           'pydantic_yaml_parser.yaml.fmt': ('yaml.html#fmt', 'pydantic_yaml_parser/yaml.py'),
+                                           'pydantic_yaml_parser.yaml._fmt': ('yaml.html#_fmt', 'pydantic_yaml_parser/yaml.py'),
                                            'pydantic_yaml_parser.yaml.yaml2d': ('yaml.html#yaml2d', 'pydantic_yaml_parser/yaml.py')}}}
```

### Comparing `pydantic-yaml-parser-0.0.3/pydantic_yaml_parser/yaml.py` & `pydantic-yaml-parser-0.0.4/pydantic_yaml_parser/yaml.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/00_yaml.ipynb.
 
 # %% auto 0
-__all__ = ['fmt', 'yaml2d', 'Section', 'YamlModel', 'QuartoDoc']
+__all__ = ['yaml2d', 'Section', 'YamlModel', 'QuartoDoc']
 
 # %% ../nbs/00_yaml.ipynb 2
 import sys
 from pydantic import BaseModel, ValidationError
 import yaml
 from typing import List, Dict
 from fastcore.test import test_fail
 
 # %% ../nbs/00_yaml.ipynb 4
-def fmt(err:dict):
+def _fmt(err:dict):
     "format error messages from pydantic."
     msg = ""
     if err['type'] == 'value_error.missing':
         msg += 'Missing field'
     else:
         msg += err['msg'] + ':'
         
@@ -39,15 +39,15 @@
     title: str
     desc: str
     contents: List[str]
 
 
 class YamlModel(BaseModel):
     @classmethod
-    def from_dict(cls, ymldict:dict, f:callable=fmt):
+    def from_dict(cls, ymldict:dict, f:callable=_fmt):
         sys.tracebacklimit = 0
         try:
             return cls.parse_obj(ymldict)
         except ValidationError as e:
             if f:
                 msg = 'Configuration error(s) for YAML:\n - '
                 msg += '\n - '.join(f(err) for err in e.errors())
```

### Comparing `pydantic-yaml-parser-0.0.3/pydantic_yaml_parser.egg-info/PKG-INFO` & `pydantic-yaml-parser-0.0.4/pydantic_yaml_parser.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-yaml-parser
-Version: 0.0.3
+Version: 0.0.4
 Summary: parse yaml files with pydantic
 Home-page: https://github.com/hamelsmu/pydantic-yaml-parser
 Author: Hamel Husain
 Author-email: hamel.husain@gmail.com
 License: Apache Software License 2.0
 Keywords: pydantic yaml
 Platform: UNKNOWN
@@ -126,8 +126,13 @@
 ``` python
 Test.from_dict(yaml_dict_error)
 ```
 
     ValueError: Configuration error(s) for YAML:
      - value is not a valid list: `sublist` for element 0 in the list for `setting_2`
 
+## Further Reading
+
+For more examples of error validation see [these
+docs](00_yaml.ipynb#error-validation).
+
```

### Comparing `pydantic-yaml-parser-0.0.3/settings.ini` & `pydantic-yaml-parser-0.0.4/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = pydantic-yaml-parser
 lib_name = %(repo)s
-version = 0.0.3
+version = 0.0.4
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = pydantic_yaml_parser
```

### Comparing `pydantic-yaml-parser-0.0.3/setup.py` & `pydantic-yaml-parser-0.0.4/setup.py`

 * *Files identical despite different names*

