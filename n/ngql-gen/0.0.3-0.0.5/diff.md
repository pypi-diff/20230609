# Comparing `tmp/ngql_gen-0.0.3.tar.gz` & `tmp/ngql_gen-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/jiayu/Documents/Kingstar/ngql_gen/dist/.tmp-8h7ve1mu/ngql_gen-0.0.3.tar", last modified: Fri Jun  9 04:54:59 2023, max compression
+gzip compressed data, was "/Users/jiayu/Documents/Kingstar/ngql_gen/dist/.tmp-oz7obmvx/ngql_gen-0.0.5.tar", last modified: Fri Jun  9 06:46:37 2023, max compression
```

## Comparing `ngql_gen-0.0.3.tar` & `ngql_gen-0.0.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-06-09 04:54:59.703215 ngql_gen-0.0.3/
--rw-r--r--   0 jiayu      (501) staff       (20)     9161 2023-06-09 02:18:33.000000 ngql_gen-0.0.3/LICENSE
--rw-r--r--   0 jiayu      (501) staff       (20)    10130 2023-06-09 04:54:59.702988 ngql_gen-0.0.3/PKG-INFO
--rw-r--r--   0 jiayu      (501) staff       (20)       98 2023-06-09 02:53:18.000000 ngql_gen-0.0.3/README.md
-drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-06-09 04:54:59.696752 ngql_gen-0.0.3/ngql_gen/
--rw-r--r--   0 jiayu      (501) staff       (20)        0 2023-06-09 04:42:54.000000 ngql_gen-0.0.3/ngql_gen/__init__.py
-drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-06-09 04:54:59.698722 ngql_gen-0.0.3/ngql_gen/config/
--rw-r--r--   0 jiayu      (501) staff       (20)       20 2023-06-09 02:06:43.000000 ngql_gen-0.0.3/ngql_gen/config/__init__.py
--rw-r--r--   0 jiayu      (501) staff       (20)      696 2023-06-09 04:53:33.000000 ngql_gen-0.0.3/ngql_gen/config/config.py
-drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-06-09 04:54:59.701539 ngql_gen-0.0.3/ngql_gen/generator/
--rw-r--r--   0 jiayu      (501) staff       (20)      149 2023-06-09 02:08:25.000000 ngql_gen-0.0.3/ngql_gen/generator/__init__.py
--rw-r--r--   0 jiayu      (501) staff       (20)      625 2023-06-09 02:10:26.000000 ngql_gen-0.0.3/ngql_gen/generator/edge.py
--rw-r--r--   0 jiayu      (501) staff       (20)      746 2023-06-09 02:10:32.000000 ngql_gen-0.0.3/ngql_gen/generator/edge_type.py
--rw-r--r--   0 jiayu      (501) staff       (20)     1884 2023-06-09 04:53:52.000000 ngql_gen-0.0.3/ngql_gen/generator/select.py
--rw-r--r--   0 jiayu      (501) staff       (20)     1146 2023-06-09 02:10:54.000000 ngql_gen-0.0.3/ngql_gen/generator/space.py
--rw-r--r--   0 jiayu      (501) staff       (20)      855 2023-06-09 02:11:20.000000 ngql_gen-0.0.3/ngql_gen/generator/tag.py
--rw-r--r--   0 jiayu      (501) staff       (20)     3584 2023-06-09 02:13:04.000000 ngql_gen-0.0.3/ngql_gen/generator/utils.py
--rw-r--r--   0 jiayu      (501) staff       (20)      491 2023-06-09 02:09:11.000000 ngql_gen-0.0.3/ngql_gen/generator/vertex.py
-drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-06-09 04:54:59.702557 ngql_gen-0.0.3/ngql_gen/model/
--rw-r--r--   0 jiayu      (501) staff       (20)       43 2023-06-09 03:11:32.000000 ngql_gen-0.0.3/ngql_gen/model/__init__.py
--rw-r--r--   0 jiayu      (501) staff       (20)      156 2023-06-09 01:59:47.000000 ngql_gen-0.0.3/ngql_gen/model/edge_type.py
--rw-r--r--   0 jiayu      (501) staff       (20)      151 2023-06-09 01:59:47.000000 ngql_gen-0.0.3/ngql_gen/model/tag.py
-drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-06-09 04:54:59.697655 ngql_gen-0.0.3/ngql_gen.egg-info/
--rw-r--r--   0 jiayu      (501) staff       (20)    10130 2023-06-09 04:54:59.000000 ngql_gen-0.0.3/ngql_gen.egg-info/PKG-INFO
--rw-r--r--   0 jiayu      (501) staff       (20)      573 2023-06-09 04:54:59.000000 ngql_gen-0.0.3/ngql_gen.egg-info/SOURCES.txt
--rw-r--r--   0 jiayu      (501) staff       (20)        1 2023-06-09 04:54:59.000000 ngql_gen-0.0.3/ngql_gen.egg-info/dependency_links.txt
--rw-r--r--   0 jiayu      (501) staff       (20)       22 2023-06-09 04:54:59.000000 ngql_gen-0.0.3/ngql_gen.egg-info/requires.txt
--rw-r--r--   0 jiayu      (501) staff       (20)        9 2023-06-09 04:54:59.000000 ngql_gen-0.0.3/ngql_gen.egg-info/top_level.txt
--rw-r--r--   0 jiayu      (501) staff       (20)      472 2023-06-09 04:54:18.000000 ngql_gen-0.0.3/pyproject.toml
--rw-r--r--   0 jiayu      (501) staff       (20)       38 2023-06-09 04:54:59.703292 ngql_gen-0.0.3/setup.cfg
+drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-06-09 06:46:37.320734 ngql_gen-0.0.5/
+-rw-r--r--   0 jiayu      (501) staff       (20)     9161 2023-06-09 02:18:33.000000 ngql_gen-0.0.5/LICENSE
+-rw-r--r--   0 jiayu      (501) staff       (20)    10130 2023-06-09 06:46:37.320487 ngql_gen-0.0.5/PKG-INFO
+-rw-r--r--   0 jiayu      (501) staff       (20)       98 2023-06-09 02:53:18.000000 ngql_gen-0.0.5/README.md
+drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-06-09 06:46:37.315064 ngql_gen-0.0.5/ngql_gen/
+-rw-r--r--   0 jiayu      (501) staff       (20)        0 2023-06-09 04:42:54.000000 ngql_gen-0.0.5/ngql_gen/__init__.py
+drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-06-09 06:46:37.316593 ngql_gen-0.0.5/ngql_gen/config/
+-rw-r--r--   0 jiayu      (501) staff       (20)       21 2023-06-09 06:45:10.000000 ngql_gen-0.0.5/ngql_gen/config/__init__.py
+-rw-r--r--   0 jiayu      (501) staff       (20)      696 2023-06-09 04:53:33.000000 ngql_gen-0.0.5/ngql_gen/config/config.py
+drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-06-09 06:46:37.319097 ngql_gen-0.0.5/ngql_gen/generator/
+-rw-r--r--   0 jiayu      (501) staff       (20)      149 2023-06-09 02:08:25.000000 ngql_gen-0.0.5/ngql_gen/generator/__init__.py
+-rw-r--r--   0 jiayu      (501) staff       (20)      625 2023-06-09 02:10:26.000000 ngql_gen-0.0.5/ngql_gen/generator/edge.py
+-rw-r--r--   0 jiayu      (501) staff       (20)      746 2023-06-09 02:10:32.000000 ngql_gen-0.0.5/ngql_gen/generator/edge_type.py
+-rw-r--r--   0 jiayu      (501) staff       (20)     1884 2023-06-09 04:53:52.000000 ngql_gen-0.0.5/ngql_gen/generator/select.py
+-rw-r--r--   0 jiayu      (501) staff       (20)     1146 2023-06-09 02:10:54.000000 ngql_gen-0.0.5/ngql_gen/generator/space.py
+-rw-r--r--   0 jiayu      (501) staff       (20)      855 2023-06-09 02:11:20.000000 ngql_gen-0.0.5/ngql_gen/generator/tag.py
+-rw-r--r--   0 jiayu      (501) staff       (20)     3584 2023-06-09 02:13:04.000000 ngql_gen-0.0.5/ngql_gen/generator/utils.py
+-rw-r--r--   0 jiayu      (501) staff       (20)      491 2023-06-09 02:09:11.000000 ngql_gen-0.0.5/ngql_gen/generator/vertex.py
+drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-06-09 06:46:37.320061 ngql_gen-0.0.5/ngql_gen/model/
+-rw-r--r--   0 jiayu      (501) staff       (20)       43 2023-06-09 03:11:32.000000 ngql_gen-0.0.5/ngql_gen/model/__init__.py
+-rw-r--r--   0 jiayu      (501) staff       (20)      156 2023-06-09 01:59:47.000000 ngql_gen-0.0.5/ngql_gen/model/edge_type.py
+-rw-r--r--   0 jiayu      (501) staff       (20)      151 2023-06-09 01:59:47.000000 ngql_gen-0.0.5/ngql_gen/model/tag.py
+drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-06-09 06:46:37.316016 ngql_gen-0.0.5/ngql_gen.egg-info/
+-rw-r--r--   0 jiayu      (501) staff       (20)    10130 2023-06-09 06:46:37.000000 ngql_gen-0.0.5/ngql_gen.egg-info/PKG-INFO
+-rw-r--r--   0 jiayu      (501) staff       (20)      573 2023-06-09 06:46:37.000000 ngql_gen-0.0.5/ngql_gen.egg-info/SOURCES.txt
+-rw-r--r--   0 jiayu      (501) staff       (20)        1 2023-06-09 06:46:37.000000 ngql_gen-0.0.5/ngql_gen.egg-info/dependency_links.txt
+-rw-r--r--   0 jiayu      (501) staff       (20)       22 2023-06-09 06:46:37.000000 ngql_gen-0.0.5/ngql_gen.egg-info/requires.txt
+-rw-r--r--   0 jiayu      (501) staff       (20)        9 2023-06-09 06:46:37.000000 ngql_gen-0.0.5/ngql_gen.egg-info/top_level.txt
+-rw-r--r--   0 jiayu      (501) staff       (20)      472 2023-06-09 06:45:28.000000 ngql_gen-0.0.5/pyproject.toml
+-rw-r--r--   0 jiayu      (501) staff       (20)       38 2023-06-09 06:46:37.320803 ngql_gen-0.0.5/setup.cfg
```

### Comparing `ngql_gen-0.0.3/LICENSE` & `ngql_gen-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ngql_gen-0.0.3/PKG-INFO` & `ngql_gen-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngql_gen
-Version: 0.0.3
+Version: 0.0.5
 Summary: Nebula Graph Query Language Generator
 Author-email: 东南dnf <zjy2414@outlook.com>
 License: Apache License
         Version 2.0, January 2004
         http://www.apache.org/licenses/
         
         TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `ngql_gen-0.0.3/ngql_gen/config/config.py` & `ngql_gen-0.0.5/ngql_gen/config/config.py`

 * *Files identical despite different names*

### Comparing `ngql_gen-0.0.3/ngql_gen/generator/edge.py` & `ngql_gen-0.0.5/ngql_gen/generator/edge.py`

 * *Files identical despite different names*

### Comparing `ngql_gen-0.0.3/ngql_gen/generator/edge_type.py` & `ngql_gen-0.0.5/ngql_gen/generator/edge_type.py`

 * *Files identical despite different names*

### Comparing `ngql_gen-0.0.3/ngql_gen/generator/select.py` & `ngql_gen-0.0.5/ngql_gen/generator/select.py`

 * *Files identical despite different names*

### Comparing `ngql_gen-0.0.3/ngql_gen/generator/space.py` & `ngql_gen-0.0.5/ngql_gen/generator/space.py`

 * *Files identical despite different names*

### Comparing `ngql_gen-0.0.3/ngql_gen/generator/tag.py` & `ngql_gen-0.0.5/ngql_gen/generator/tag.py`

 * *Files identical despite different names*

### Comparing `ngql_gen-0.0.3/ngql_gen/generator/utils.py` & `ngql_gen-0.0.5/ngql_gen/generator/utils.py`

 * *Files identical despite different names*

### Comparing `ngql_gen-0.0.3/ngql_gen.egg-info/PKG-INFO` & `ngql_gen-0.0.5/ngql_gen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngql-gen
-Version: 0.0.3
+Version: 0.0.5
 Summary: Nebula Graph Query Language Generator
 Author-email: 东南dnf <zjy2414@outlook.com>
 License: Apache License
         Version 2.0, January 2004
         http://www.apache.org/licenses/
         
         TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `ngql_gen-0.0.3/ngql_gen.egg-info/SOURCES.txt` & `ngql_gen-0.0.5/ngql_gen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

