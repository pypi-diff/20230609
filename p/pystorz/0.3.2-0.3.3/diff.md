# Comparing `tmp/pystorz-0.3.2.tar.gz` & `tmp/pystorz-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pystorz-0.3.2.tar", last modified: Tue Jun  6 17:25:53 2023, max compression
+gzip compressed data, was "pystorz-0.3.3.tar", last modified: Fri Jun  9 19:50:16 2023, max compression
```

## Comparing `pystorz-0.3.2.tar` & `pystorz-0.3.3.tar`

### file list

```diff
@@ -1,50 +1,55 @@
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-06 17:25:53.839729 pystorz-0.3.2/
--rw-r--r--   0 wazofski   (501) staff       (20)     1086 2023-04-24 05:31:47.000000 pystorz-0.3.2/LICENSE
--rw-r--r--   0 wazofski   (501) staff       (20)     3506 2023-06-06 17:25:53.839526 pystorz-0.3.2/PKG-INFO
--rw-r--r--   0 wazofski   (501) staff       (20)     2615 2023-06-04 18:42:13.000000 pystorz-0.3.2/README.md
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-06 17:25:53.833810 pystorz-0.3.2/pystorz/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:48.000000 pystorz-0.3.2/pystorz/__init__.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-06 17:25:53.834847 pystorz-0.3.2/pystorz/internal/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:44.000000 pystorz-0.3.2/pystorz/internal/__init__.py
--rw-r--r--   0 wazofski   (501) staff       (20)      380 2023-06-04 14:02:51.000000 pystorz-0.3.2/pystorz/internal/constants.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-06 17:25:53.835017 pystorz-0.3.2/pystorz/meta/
--rw-r--r--   0 wazofski   (501) staff       (20)     2580 2023-06-06 17:22:59.000000 pystorz-0.3.2/pystorz/meta/store.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-06 17:25:53.835895 pystorz-0.3.2/pystorz/mgen/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:41.000000 pystorz-0.3.2/pystorz/mgen/__init__.py
--rw-r--r--   0 wazofski   (501) staff       (20)     4164 2023-06-05 18:53:35.000000 pystorz-0.3.2/pystorz/mgen/builder.py
--rw-r--r--   0 wazofski   (501) staff       (20)     7119 2023-05-02 17:05:13.000000 pystorz-0.3.2/pystorz/mgen/loader.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-06 17:25:53.837107 pystorz-0.3.2/pystorz/mgen/templates/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:21:36.000000 pystorz-0.3.2/pystorz/mgen/templates/__init__.py
--rw-r--r--   0 wazofski   (501) staff       (20)       56 2023-04-24 14:15:03.000000 pystorz-0.3.2/pystorz/mgen/templates/imports.py
--rw-r--r--   0 wazofski   (501) staff       (20)      225 2023-04-24 14:24:31.000000 pystorz-0.3.2/pystorz/mgen/templates/interface.py
--rw-r--r--   0 wazofski   (501) staff       (20)      331 2023-04-24 14:15:03.000000 pystorz-0.3.2/pystorz/mgen/templates/meta.py
--rw-r--r--   0 wazofski   (501) staff       (20)      473 2023-04-24 14:15:03.000000 pystorz-0.3.2/pystorz/mgen/templates/schema.py
--rw-r--r--   0 wazofski   (501) staff       (20)      110 2023-04-24 14:15:03.000000 pystorz-0.3.2/pystorz/mgen/templates/specinternal.py
--rw-r--r--   0 wazofski   (501) staff       (20)     1123 2023-05-01 01:21:35.000000 pystorz-0.3.2/pystorz/mgen/templates/structure.py
--rw-r--r--   0 wazofski   (501) staff       (20)     1772 2023-05-02 17:04:18.000000 pystorz-0.3.2/pystorz/mgen/templates/unmarshall.py
--rw-r--r--   0 wazofski   (501) staff       (20)     2808 2023-04-24 15:47:15.000000 pystorz-0.3.2/pystorz/mgen/test.py
--rw-r--r--   0 wazofski   (501) staff       (20)      611 2023-04-24 14:15:03.000000 pystorz-0.3.2/pystorz/mgen/utils.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-06 17:25:53.837723 pystorz-0.3.2/pystorz/rest/
--rw-r--r--   0 wazofski   (501) staff       (20)     8259 2023-06-04 14:02:51.000000 pystorz-0.3.2/pystorz/rest/client.py
--rw-r--r--   0 wazofski   (501) staff       (20)     1099 2023-06-03 19:10:23.000000 pystorz-0.3.2/pystorz/rest/headers.py
--rw-r--r--   0 wazofski   (501) staff       (20)     2462 2023-06-04 14:02:51.000000 pystorz-0.3.2/pystorz/rest/internals.py
--rw-r--r--   0 wazofski   (501) staff       (20)     9691 2023-06-04 15:53:12.000000 pystorz-0.3.2/pystorz/rest/server.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-06 17:25:53.838485 pystorz-0.3.2/pystorz/sql/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:39.000000 pystorz-0.3.2/pystorz/sql/__init__.py
--rw-r--r--   0 wazofski   (501) staff       (20)     2617 2023-06-04 18:13:23.000000 pystorz-0.3.2/pystorz/sql/mysql.py
--rw-r--r--   0 wazofski   (501) staff       (20)      192 2023-06-04 16:07:46.000000 pystorz-0.3.2/pystorz/sql/sqlite.py
--rw-r--r--   0 wazofski   (501) staff       (20)    15373 2023-06-04 18:21:14.000000 pystorz-0.3.2/pystorz/sql/store.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-06 17:25:53.839245 pystorz-0.3.2/pystorz/store/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:33.000000 pystorz-0.3.2/pystorz/store/__init__.py
--rw-r--r--   0 wazofski   (501) staff       (20)     2667 2023-04-26 20:36:31.000000 pystorz-0.3.2/pystorz/store/meta.py
--rw-r--r--   0 wazofski   (501) staff       (20)    10450 2023-06-04 14:02:51.000000 pystorz-0.3.2/pystorz/store/options.py
--rw-r--r--   0 wazofski   (501) staff       (20)     2974 2023-06-03 19:10:23.000000 pystorz-0.3.2/pystorz/store/store.py
--rw-r--r--   0 wazofski   (501) staff       (20)     3505 2023-06-04 14:02:51.000000 pystorz-0.3.2/pystorz/store/utils.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-06 17:25:53.834561 pystorz-0.3.2/pystorz.egg-info/
--rw-r--r--   0 wazofski   (501) staff       (20)     3506 2023-06-06 17:25:53.000000 pystorz-0.3.2/pystorz.egg-info/PKG-INFO
--rw-r--r--   0 wazofski   (501) staff       (20)      980 2023-06-06 17:25:53.000000 pystorz-0.3.2/pystorz.egg-info/SOURCES.txt
--rw-r--r--   0 wazofski   (501) staff       (20)        1 2023-06-06 17:25:53.000000 pystorz-0.3.2/pystorz.egg-info/dependency_links.txt
--rw-r--r--   0 wazofski   (501) staff       (20)       93 2023-06-06 17:25:53.000000 pystorz-0.3.2/pystorz.egg-info/requires.txt
--rw-r--r--   0 wazofski   (501) staff       (20)      113 2023-06-06 17:25:53.000000 pystorz-0.3.2/pystorz.egg-info/top_level.txt
--rw-r--r--   0 wazofski   (501) staff       (20)       38 2023-06-06 17:25:53.839794 pystorz-0.3.2/setup.cfg
--rw-r--r--   0 wazofski   (501) staff       (20)     1290 2023-06-06 17:25:13.000000 pystorz-0.3.2/setup.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-09 19:50:16.908916 pystorz-0.3.3/
+-rw-r--r--   0 wazofski   (501) staff       (20)     1086 2023-04-24 05:31:47.000000 pystorz-0.3.3/LICENSE
+-rw-r--r--   0 wazofski   (501) staff       (20)     2992 2023-06-09 19:50:16.908727 pystorz-0.3.3/PKG-INFO
+-rw-r--r--   0 wazofski   (501) staff       (20)     2615 2023-06-04 18:42:13.000000 pystorz-0.3.3/README.md
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-09 19:50:16.899392 pystorz-0.3.3/pystorz/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:48.000000 pystorz-0.3.3/pystorz/__init__.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-09 19:50:16.900287 pystorz-0.3.3/pystorz/internal/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:44.000000 pystorz-0.3.3/pystorz/internal/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      380 2023-06-04 14:02:51.000000 pystorz-0.3.3/pystorz/internal/constants.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-09 19:50:16.900806 pystorz-0.3.3/pystorz/meta/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-06-09 19:44:40.000000 pystorz-0.3.3/pystorz/meta/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     2580 2023-06-06 17:22:59.000000 pystorz-0.3.3/pystorz/meta/store.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-09 19:50:16.902210 pystorz-0.3.3/pystorz/mgen/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:41.000000 pystorz-0.3.3/pystorz/mgen/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     4164 2023-06-05 18:53:35.000000 pystorz-0.3.3/pystorz/mgen/builder.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     7119 2023-05-02 17:05:13.000000 pystorz-0.3.3/pystorz/mgen/loader.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-09 19:50:16.904196 pystorz-0.3.3/pystorz/mgen/templates/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:21:36.000000 pystorz-0.3.3/pystorz/mgen/templates/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)       56 2023-04-24 14:15:03.000000 pystorz-0.3.3/pystorz/mgen/templates/imports.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      225 2023-04-24 14:24:31.000000 pystorz-0.3.3/pystorz/mgen/templates/interface.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      331 2023-04-24 14:15:03.000000 pystorz-0.3.3/pystorz/mgen/templates/meta.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      473 2023-04-24 14:15:03.000000 pystorz-0.3.3/pystorz/mgen/templates/schema.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      110 2023-04-24 14:15:03.000000 pystorz-0.3.3/pystorz/mgen/templates/specinternal.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     1123 2023-05-01 01:21:35.000000 pystorz-0.3.3/pystorz/mgen/templates/structure.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     1772 2023-05-02 17:04:18.000000 pystorz-0.3.3/pystorz/mgen/templates/unmarshall.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     2808 2023-04-24 15:47:15.000000 pystorz-0.3.3/pystorz/mgen/test.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      611 2023-04-24 14:15:03.000000 pystorz-0.3.3/pystorz/mgen/utils.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-09 19:50:16.906020 pystorz-0.3.3/pystorz/rest/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-06-09 19:44:44.000000 pystorz-0.3.3/pystorz/rest/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     8259 2023-06-04 14:02:51.000000 pystorz-0.3.3/pystorz/rest/client.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     1099 2023-06-03 19:10:23.000000 pystorz-0.3.3/pystorz/rest/headers.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     2462 2023-06-04 14:02:51.000000 pystorz-0.3.3/pystorz/rest/internals.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     9691 2023-06-04 15:53:12.000000 pystorz-0.3.3/pystorz/rest/server.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-09 19:50:16.906432 pystorz-0.3.3/pystorz/router/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-06-09 19:44:42.000000 pystorz-0.3.3/pystorz/router/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     2344 2023-06-06 17:21:47.000000 pystorz-0.3.3/pystorz/router/store.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-09 19:50:16.907350 pystorz-0.3.3/pystorz/sql/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:39.000000 pystorz-0.3.3/pystorz/sql/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     2617 2023-06-09 19:48:52.000000 pystorz-0.3.3/pystorz/sql/mysql.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      192 2023-06-04 16:07:46.000000 pystorz-0.3.3/pystorz/sql/sqlite.py
+-rw-r--r--   0 wazofski   (501) staff       (20)    15493 2023-06-09 19:44:00.000000 pystorz-0.3.3/pystorz/sql/store.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-09 19:50:16.908463 pystorz-0.3.3/pystorz/store/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:33.000000 pystorz-0.3.3/pystorz/store/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     2667 2023-04-26 20:36:31.000000 pystorz-0.3.3/pystorz/store/meta.py
+-rw-r--r--   0 wazofski   (501) staff       (20)    10450 2023-06-04 14:02:51.000000 pystorz-0.3.3/pystorz/store/options.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     2974 2023-06-03 19:10:23.000000 pystorz-0.3.3/pystorz/store/store.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     3505 2023-06-04 14:02:51.000000 pystorz-0.3.3/pystorz/store/utils.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-09 19:50:16.900058 pystorz-0.3.3/pystorz.egg-info/
+-rw-r--r--   0 wazofski   (501) staff       (20)     2992 2023-06-09 19:50:16.000000 pystorz-0.3.3/pystorz.egg-info/PKG-INFO
+-rw-r--r--   0 wazofski   (501) staff       (20)     1081 2023-06-09 19:50:16.000000 pystorz-0.3.3/pystorz.egg-info/SOURCES.txt
+-rw-r--r--   0 wazofski   (501) staff       (20)        1 2023-06-09 19:50:16.000000 pystorz-0.3.3/pystorz.egg-info/dependency_links.txt
+-rw-r--r--   0 wazofski   (501) staff       (20)       93 2023-06-09 19:50:16.000000 pystorz-0.3.3/pystorz.egg-info/requires.txt
+-rw-r--r--   0 wazofski   (501) staff       (20)      128 2023-06-09 19:50:16.000000 pystorz-0.3.3/pystorz.egg-info/top_level.txt
+-rw-r--r--   0 wazofski   (501) staff       (20)       38 2023-06-09 19:50:16.908959 pystorz-0.3.3/setup.cfg
+-rw-r--r--   0 wazofski   (501) staff       (20)     1316 2023-06-09 19:48:07.000000 pystorz-0.3.3/setup.py
```

### Comparing `pystorz-0.3.2/LICENSE` & `pystorz-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pystorz-0.3.2/PKG-INFO` & `pystorz-0.3.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,75 +1,74 @@
 Metadata-Version: 2.1
 Name: pystorz
-Version: 0.3.2
+Version: 0.3.3
 Summary: Python package for the Storz object store framework.
 Home-page: https://github.com/wazofski/pystorz
 Author: wazofski
-License: UNKNOWN
-Description: <p align="center">
-        <img src="https://raw.githubusercontent.com/wazofski/pystorz/master/logo.png" width="300" alt="storz" />
-        </p>
-        
-        **pystorz** is an *object store framework* built in python. It consists of a set of modules implementing the [Store](https://github.com/wazofski/pystorz/tree/master/pystorz/store) interface and features a simple [object modeling language](https://github.com/wazofski/pystorz/tree/master/pystorz/mgen) used to generate golang object class meta for interacting with `Store` APIs.
-        
-        **pystorz** modules provide functionality to store, modify and retrieve modeled objects from various sources (TBD). Such modules can be composed together to chain `Store` functionality into more complex logical modules. Combining modules allows handling object changes and manipulating data in complex ways *within or across* services, making multi-level server complexity achievable with ease. The Store modules are fully compatible with each other and can be composed in any combination since they all implement or expose the same [Store](https://github.com/wazofski/pystorz/tree/master/pystorz/store) interface.
-        
-        Original storz was written in go. You can check it out here:
-        [https://github.com/wazofski/gostorz](https://github.com/wazofski/gostorz)
-        
-        This is a python port of the original storz.
-        Still in development.
-        
-        ## Quick Start Guide
-        
-        ### Installation
-        ```
-        pip install pystorz
-        ```
-        
-        ## Model example
-        
-        You can find a saomple model in the tests folder.
-        [https://github.com/wazofski/pystorz/blob/master/tests/model/sample.yml](https://github.com/wazofski/pystorz/blob/master/tests/model/sample.yml)
-        
-        You can define simple structures and reference them as fields in other structures.
-        
-        You need to define Objects that will become your root level modeled objects. You can then create, update, delete and retrieve these from using a store.
-        
-        Only a SQLite store is implemented at the moment.
-        
-        More to come.
-        Check out the go version (link above) for more information.
-        
-        ## Usage
-        ```
-            from pystorz.mgen import builder
-        
-            # run the code gen to 
-            builder.Generate("path/to/model.yml")
-            # this will make a generated folder in the project home directory
-        
-            # you can then import the generated model
-            from generated import model
-        
-            # initialize a store
-            stor = SqliteStore(
-                Schema(),
-                SqliteConnector("path/to/your/sqlite3.db"))
-        
-            world = model.WorldFactory()
-            world.External().SetName("hello")
-        
-            created_world = stor.Create(world)
-            world.External().SetDescription("hello world")
-            updated_world = stor.Update(world.Metadata().Identity(), world)
-            
-            # ...
-        
-        ```
-        
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+License-File: LICENSE
+
+<p align="center">
+<img src="https://raw.githubusercontent.com/wazofski/pystorz/master/logo.png" width="300" alt="storz" />
+</p>
+
+**pystorz** is an *object store framework* built in python. It consists of a set of modules implementing the [Store](https://github.com/wazofski/pystorz/tree/master/pystorz/store) interface and features a simple [object modeling language](https://github.com/wazofski/pystorz/tree/master/pystorz/mgen) used to generate golang object class meta for interacting with `Store` APIs.
+
+**pystorz** modules provide functionality to store, modify and retrieve modeled objects from various sources (TBD). Such modules can be composed together to chain `Store` functionality into more complex logical modules. Combining modules allows handling object changes and manipulating data in complex ways *within or across* services, making multi-level server complexity achievable with ease. The Store modules are fully compatible with each other and can be composed in any combination since they all implement or expose the same [Store](https://github.com/wazofski/pystorz/tree/master/pystorz/store) interface.
+
+Original storz was written in go. You can check it out here:
+[https://github.com/wazofski/gostorz](https://github.com/wazofski/gostorz)
+
+This is a python port of the original storz.
+Still in development.
+
+## Quick Start Guide
+
+### Installation
+```
+pip install pystorz
+```
+
+## Model example
+
+You can find a saomple model in the tests folder.
+[https://github.com/wazofski/pystorz/blob/master/tests/model/sample.yml](https://github.com/wazofski/pystorz/blob/master/tests/model/sample.yml)
+
+You can define simple structures and reference them as fields in other structures.
+
+You need to define Objects that will become your root level modeled objects. You can then create, update, delete and retrieve these from using a store.
+
+Only a SQLite store is implemented at the moment.
+
+More to come.
+Check out the go version (link above) for more information.
+
+## Usage
+```
+    from pystorz.mgen import builder
+
+    # run the code gen to 
+    builder.Generate("path/to/model.yml")
+    # this will make a generated folder in the project home directory
+
+    # you can then import the generated model
+    from generated import model
+
+    # initialize a store
+    stor = SqliteStore(
+        Schema(),
+        SqliteConnector("path/to/your/sqlite3.db"))
+
+    world = model.WorldFactory()
+    world.External().SetName("hello")
+
+    created_world = stor.Create(world)
+    world.External().SetDescription("hello world")
+    updated_world = stor.Update(world.Metadata().Identity(), world)
+    
+    # ...
+
+```
```

### Comparing `pystorz-0.3.2/README.md` & `pystorz-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `pystorz-0.3.2/pystorz/meta/store.py` & `pystorz-0.3.3/pystorz/meta/store.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.3.2/pystorz/mgen/builder.py` & `pystorz-0.3.3/pystorz/mgen/builder.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.3.2/pystorz/mgen/loader.py` & `pystorz-0.3.3/pystorz/mgen/loader.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.3.2/pystorz/mgen/templates/structure.py` & `pystorz-0.3.3/pystorz/mgen/templates/structure.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.3.2/pystorz/mgen/templates/unmarshall.py` & `pystorz-0.3.3/pystorz/mgen/templates/unmarshall.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.3.2/pystorz/mgen/test.py` & `pystorz-0.3.3/pystorz/mgen/test.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.3.2/pystorz/mgen/utils.py` & `pystorz-0.3.3/pystorz/mgen/utils.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.3.2/pystorz/rest/client.py` & `pystorz-0.3.3/pystorz/rest/client.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.3.2/pystorz/rest/headers.py` & `pystorz-0.3.3/pystorz/rest/headers.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.3.2/pystorz/rest/internals.py` & `pystorz-0.3.3/pystorz/rest/internals.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.3.2/pystorz/rest/server.py` & `pystorz-0.3.3/pystorz/rest/server.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.3.2/pystorz/sql/mysql.py` & `pystorz-0.3.3/pystorz/sql/mysql.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.3.2/pystorz/sql/store.py` & `pystorz-0.3.3/pystorz/sql/store.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,19 +186,23 @@
         copt = options.CommonOptionHolderFactory()
         for o in opt:
             o.ApplyFunction()(copt)
 
         db = self._connection()
         cursor = db.cursor()
 
+        res = None
         if identity.IsId():
             pkey, typ = self._getIdentity(cursor, identity.Path())
-            return self._getObject(cursor, pkey, typ)
-
-        return self._getObject(cursor, identity.Key(), identity.Type())
+            res = self._getObject(cursor, pkey, typ)
+        else:
+            res = self._getObject(cursor, identity.Key(), identity.Type())
+        
+        db.commit()
+        return res
 
     def List(self, identity, *opt: list[options.ListOption]):
         if identity is None:
             raise Exception(constants.ErrInvalidPath)
 
         log.info("list {}".format(identity.Path()))
 
@@ -235,15 +239,17 @@
 
         if copt.page_offset is not None and copt.page_offset > 0:
             query = query + " OFFSET {}".format(copt.page_offset)
 
         self._do_query(cursor, query)
         rows = cursor.fetchall()
 
-        return self._parseObjectRows(rows, identity.Type())
+        res = self._parseObjectRows(rows, identity.Type())
+        db.commit()
+        return res
 
     def _prepareTables(self, db):
         create = """
         CREATE TABLE IF NOT EXISTS IdIndex (
             Path VARCHAR(75) NOT NULL PRIMARY KEY,
             Pkey NVARCHAR(50) NOT NULL,
             Type VARCHAR(25) NOT NULL);
```

### Comparing `pystorz-0.3.2/pystorz/store/meta.py` & `pystorz-0.3.3/pystorz/store/meta.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.3.2/pystorz/store/options.py` & `pystorz-0.3.3/pystorz/store/options.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.3.2/pystorz/store/store.py` & `pystorz-0.3.3/pystorz/store/store.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.3.2/pystorz/store/utils.py` & `pystorz-0.3.3/pystorz/store/utils.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.3.2/pystorz.egg-info/PKG-INFO` & `pystorz-0.3.3/pystorz.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,75 +1,74 @@
 Metadata-Version: 2.1
 Name: pystorz
-Version: 0.3.2
+Version: 0.3.3
 Summary: Python package for the Storz object store framework.
 Home-page: https://github.com/wazofski/pystorz
 Author: wazofski
-License: UNKNOWN
-Description: <p align="center">
-        <img src="https://raw.githubusercontent.com/wazofski/pystorz/master/logo.png" width="300" alt="storz" />
-        </p>
-        
-        **pystorz** is an *object store framework* built in python. It consists of a set of modules implementing the [Store](https://github.com/wazofski/pystorz/tree/master/pystorz/store) interface and features a simple [object modeling language](https://github.com/wazofski/pystorz/tree/master/pystorz/mgen) used to generate golang object class meta for interacting with `Store` APIs.
-        
-        **pystorz** modules provide functionality to store, modify and retrieve modeled objects from various sources (TBD). Such modules can be composed together to chain `Store` functionality into more complex logical modules. Combining modules allows handling object changes and manipulating data in complex ways *within or across* services, making multi-level server complexity achievable with ease. The Store modules are fully compatible with each other and can be composed in any combination since they all implement or expose the same [Store](https://github.com/wazofski/pystorz/tree/master/pystorz/store) interface.
-        
-        Original storz was written in go. You can check it out here:
-        [https://github.com/wazofski/gostorz](https://github.com/wazofski/gostorz)
-        
-        This is a python port of the original storz.
-        Still in development.
-        
-        ## Quick Start Guide
-        
-        ### Installation
-        ```
-        pip install pystorz
-        ```
-        
-        ## Model example
-        
-        You can find a saomple model in the tests folder.
-        [https://github.com/wazofski/pystorz/blob/master/tests/model/sample.yml](https://github.com/wazofski/pystorz/blob/master/tests/model/sample.yml)
-        
-        You can define simple structures and reference them as fields in other structures.
-        
-        You need to define Objects that will become your root level modeled objects. You can then create, update, delete and retrieve these from using a store.
-        
-        Only a SQLite store is implemented at the moment.
-        
-        More to come.
-        Check out the go version (link above) for more information.
-        
-        ## Usage
-        ```
-            from pystorz.mgen import builder
-        
-            # run the code gen to 
-            builder.Generate("path/to/model.yml")
-            # this will make a generated folder in the project home directory
-        
-            # you can then import the generated model
-            from generated import model
-        
-            # initialize a store
-            stor = SqliteStore(
-                Schema(),
-                SqliteConnector("path/to/your/sqlite3.db"))
-        
-            world = model.WorldFactory()
-            world.External().SetName("hello")
-        
-            created_world = stor.Create(world)
-            world.External().SetDescription("hello world")
-            updated_world = stor.Update(world.Metadata().Identity(), world)
-            
-            # ...
-        
-        ```
-        
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+License-File: LICENSE
+
+<p align="center">
+<img src="https://raw.githubusercontent.com/wazofski/pystorz/master/logo.png" width="300" alt="storz" />
+</p>
+
+**pystorz** is an *object store framework* built in python. It consists of a set of modules implementing the [Store](https://github.com/wazofski/pystorz/tree/master/pystorz/store) interface and features a simple [object modeling language](https://github.com/wazofski/pystorz/tree/master/pystorz/mgen) used to generate golang object class meta for interacting with `Store` APIs.
+
+**pystorz** modules provide functionality to store, modify and retrieve modeled objects from various sources (TBD). Such modules can be composed together to chain `Store` functionality into more complex logical modules. Combining modules allows handling object changes and manipulating data in complex ways *within or across* services, making multi-level server complexity achievable with ease. The Store modules are fully compatible with each other and can be composed in any combination since they all implement or expose the same [Store](https://github.com/wazofski/pystorz/tree/master/pystorz/store) interface.
+
+Original storz was written in go. You can check it out here:
+[https://github.com/wazofski/gostorz](https://github.com/wazofski/gostorz)
+
+This is a python port of the original storz.
+Still in development.
+
+## Quick Start Guide
+
+### Installation
+```
+pip install pystorz
+```
+
+## Model example
+
+You can find a saomple model in the tests folder.
+[https://github.com/wazofski/pystorz/blob/master/tests/model/sample.yml](https://github.com/wazofski/pystorz/blob/master/tests/model/sample.yml)
+
+You can define simple structures and reference them as fields in other structures.
+
+You need to define Objects that will become your root level modeled objects. You can then create, update, delete and retrieve these from using a store.
+
+Only a SQLite store is implemented at the moment.
+
+More to come.
+Check out the go version (link above) for more information.
+
+## Usage
+```
+    from pystorz.mgen import builder
+
+    # run the code gen to 
+    builder.Generate("path/to/model.yml")
+    # this will make a generated folder in the project home directory
+
+    # you can then import the generated model
+    from generated import model
+
+    # initialize a store
+    stor = SqliteStore(
+        Schema(),
+        SqliteConnector("path/to/your/sqlite3.db"))
+
+    world = model.WorldFactory()
+    world.External().SetName("hello")
+
+    created_world = stor.Create(world)
+    world.External().SetDescription("hello world")
+    updated_world = stor.Update(world.Metadata().Identity(), world)
+    
+    # ...
+
+```
```

### Comparing `pystorz-0.3.2/pystorz.egg-info/SOURCES.txt` & `pystorz-0.3.3/pystorz.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,32 +5,36 @@
 pystorz.egg-info/PKG-INFO
 pystorz.egg-info/SOURCES.txt
 pystorz.egg-info/dependency_links.txt
 pystorz.egg-info/requires.txt
 pystorz.egg-info/top_level.txt
 pystorz/internal/__init__.py
 pystorz/internal/constants.py
+pystorz/meta/__init__.py
 pystorz/meta/store.py
 pystorz/mgen/__init__.py
 pystorz/mgen/builder.py
 pystorz/mgen/loader.py
 pystorz/mgen/test.py
 pystorz/mgen/utils.py
 pystorz/mgen/templates/__init__.py
 pystorz/mgen/templates/imports.py
 pystorz/mgen/templates/interface.py
 pystorz/mgen/templates/meta.py
 pystorz/mgen/templates/schema.py
 pystorz/mgen/templates/specinternal.py
 pystorz/mgen/templates/structure.py
 pystorz/mgen/templates/unmarshall.py
+pystorz/rest/__init__.py
 pystorz/rest/client.py
 pystorz/rest/headers.py
 pystorz/rest/internals.py
 pystorz/rest/server.py
+pystorz/router/__init__.py
+pystorz/router/store.py
 pystorz/sql/__init__.py
 pystorz/sql/mysql.py
 pystorz/sql/sqlite.py
 pystorz/sql/store.py
 pystorz/store/__init__.py
 pystorz/store/meta.py
 pystorz/store/options.py
```

### Comparing `pystorz-0.3.2/setup.py` & `pystorz-0.3.3/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pystorz',
-    version='0.3.2',
+    version='0.3.3',
     author='wazofski',
     description='Python package for the Storz object store framework.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/wazofski/pystorz',
     packages=[
         "pystorz",
         "pystorz/internal",
         "pystorz/meta",
         "pystorz/mgen",
         "pystorz/mgen/templates",
         "pystorz/rest",
         "pystorz/sql",
         "pystorz/store",
+        "pystorz/router",
     ],
     package_data={'': ['*.py']},
     # package_dir={'': 'src'},
     include_package_data=True,
     install_requires=[
         "PyYAML",
         "jinja2",
```

