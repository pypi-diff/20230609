# Comparing `tmp/ICICONSOLE-0.0.7.tar.gz` & `tmp/ICICONSOLE-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ICICONSOLE-0.0.7.tar", last modified: Wed Jun  7 02:03:08 2023, max compression
+gzip compressed data, was "ICICONSOLE-0.0.8.tar", last modified: Thu Jun  8 22:15:23 2023, max compression
```

## Comparing `ICICONSOLE-0.0.7.tar` & `ICICONSOLE-0.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-06-07 02:03:08.858268 ICICONSOLE-0.0.7/
-drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-06-07 02:03:08.856926 ICICONSOLE-0.0.7/ICICONSOLE/
--rw-r--r--   0 sahilsamar   (501) staff       (20)      882 2023-04-23 22:20:18.000000 ICICONSOLE-0.0.7/ICICONSOLE/BasicCypherCommands.py
--rw-r--r--   0 sahilsamar   (501) staff       (20)        0 2023-04-23 22:20:18.000000 ICICONSOLE-0.0.7/ICICONSOLE/__init__.py
--rw-r--r--   0 sahilsamar   (501) staff       (20)     9214 2023-06-07 01:47:33.000000 ICICONSOLE-0.0.7/ICICONSOLE/__main__.py
--rw-r--r--   0 sahilsamar   (501) staff       (20)      330 2023-04-23 22:20:18.000000 ICICONSOLE-0.0.7/ICICONSOLE/helpCypher.json
-drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-06-07 02:03:08.857869 ICICONSOLE-0.0.7/ICICONSOLE.egg-info/
--rw-r--r--   0 sahilsamar   (501) staff       (20)    43067 2023-06-07 02:03:08.000000 ICICONSOLE-0.0.7/ICICONSOLE.egg-info/PKG-INFO
--rw-r--r--   0 sahilsamar   (501) staff       (20)      357 2023-06-07 02:03:08.000000 ICICONSOLE-0.0.7/ICICONSOLE.egg-info/SOURCES.txt
--rw-r--r--   0 sahilsamar   (501) staff       (20)        1 2023-06-07 02:03:08.000000 ICICONSOLE-0.0.7/ICICONSOLE.egg-info/dependency_links.txt
--rw-r--r--   0 sahilsamar   (501) staff       (20)       53 2023-06-07 02:03:08.000000 ICICONSOLE-0.0.7/ICICONSOLE.egg-info/entry_points.txt
--rw-r--r--   0 sahilsamar   (501) staff       (20)       28 2023-06-07 02:03:08.000000 ICICONSOLE-0.0.7/ICICONSOLE.egg-info/requires.txt
--rw-r--r--   0 sahilsamar   (501) staff       (20)       11 2023-06-07 02:03:08.000000 ICICONSOLE-0.0.7/ICICONSOLE.egg-info/top_level.txt
--rw-r--r--   0 sahilsamar   (501) staff       (20)    35149 2023-04-23 22:20:18.000000 ICICONSOLE-0.0.7/LICENSE
--rw-r--r--   0 sahilsamar   (501) staff       (20)       35 2023-06-07 02:00:37.000000 ICICONSOLE-0.0.7/MANIFEST.in
--rw-r--r--   0 sahilsamar   (501) staff       (20)    43067 2023-06-07 02:03:08.858121 ICICONSOLE-0.0.7/PKG-INFO
--rw-r--r--   0 sahilsamar   (501) staff       (20)     1843 2023-06-07 01:45:53.000000 ICICONSOLE-0.0.7/README.md
--rw-r--r--   0 sahilsamar   (501) staff       (20)     1001 2023-06-07 02:00:45.000000 ICICONSOLE-0.0.7/pyproject.toml
--rw-r--r--   0 sahilsamar   (501) staff       (20)       38 2023-06-07 02:03:08.858304 ICICONSOLE-0.0.7/setup.cfg
+drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-06-08 22:15:23.324452 ICICONSOLE-0.0.8/
+drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-06-08 22:15:23.323231 ICICONSOLE-0.0.8/ICICONSOLE/
+-rw-r--r--   0 sahilsamar   (501) staff       (20)      882 2023-04-23 22:20:18.000000 ICICONSOLE-0.0.8/ICICONSOLE/BasicCypherCommands.py
+-rw-r--r--   0 sahilsamar   (501) staff       (20)        0 2023-04-23 22:20:18.000000 ICICONSOLE-0.0.8/ICICONSOLE/__init__.py
+-rw-r--r--   0 sahilsamar   (501) staff       (20)     9689 2023-06-08 22:11:12.000000 ICICONSOLE-0.0.8/ICICONSOLE/__main__.py
+-rw-r--r--   0 sahilsamar   (501) staff       (20)      330 2023-04-23 22:20:18.000000 ICICONSOLE-0.0.8/ICICONSOLE/helpCypher.json
+drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-06-08 22:15:23.324085 ICICONSOLE-0.0.8/ICICONSOLE.egg-info/
+-rw-r--r--   0 sahilsamar   (501) staff       (20)    43067 2023-06-08 22:15:23.000000 ICICONSOLE-0.0.8/ICICONSOLE.egg-info/PKG-INFO
+-rw-r--r--   0 sahilsamar   (501) staff       (20)      357 2023-06-08 22:15:23.000000 ICICONSOLE-0.0.8/ICICONSOLE.egg-info/SOURCES.txt
+-rw-r--r--   0 sahilsamar   (501) staff       (20)        1 2023-06-08 22:15:23.000000 ICICONSOLE-0.0.8/ICICONSOLE.egg-info/dependency_links.txt
+-rw-r--r--   0 sahilsamar   (501) staff       (20)       53 2023-06-08 22:15:23.000000 ICICONSOLE-0.0.8/ICICONSOLE.egg-info/entry_points.txt
+-rw-r--r--   0 sahilsamar   (501) staff       (20)       41 2023-06-08 22:15:23.000000 ICICONSOLE-0.0.8/ICICONSOLE.egg-info/requires.txt
+-rw-r--r--   0 sahilsamar   (501) staff       (20)       11 2023-06-08 22:15:23.000000 ICICONSOLE-0.0.8/ICICONSOLE.egg-info/top_level.txt
+-rw-r--r--   0 sahilsamar   (501) staff       (20)    35149 2023-04-23 22:20:18.000000 ICICONSOLE-0.0.8/LICENSE
+-rw-r--r--   0 sahilsamar   (501) staff       (20)       35 2023-06-07 02:00:37.000000 ICICONSOLE-0.0.8/MANIFEST.in
+-rw-r--r--   0 sahilsamar   (501) staff       (20)    43067 2023-06-08 22:15:23.324317 ICICONSOLE-0.0.8/PKG-INFO
+-rw-r--r--   0 sahilsamar   (501) staff       (20)     1843 2023-06-07 01:45:53.000000 ICICONSOLE-0.0.8/README.md
+-rw-r--r--   0 sahilsamar   (501) staff       (20)     1021 2023-06-08 22:13:43.000000 ICICONSOLE-0.0.8/pyproject.toml
+-rw-r--r--   0 sahilsamar   (501) staff       (20)       38 2023-06-08 22:15:23.324485 ICICONSOLE-0.0.8/setup.cfg
```

### Comparing `ICICONSOLE-0.0.7/ICICONSOLE/BasicCypherCommands.py` & `ICICONSOLE-0.0.8/ICICONSOLE/BasicCypherCommands.py`

 * *Files identical despite different names*

### Comparing `ICICONSOLE-0.0.7/ICICONSOLE/__main__.py` & `ICICONSOLE-0.0.8/ICICONSOLE/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # This is how we actually connect to TAPIS and get the required information to connect to a Pod
 from tapipy.tapis import Tapis
 # These are to clear the screen
 import os
 import signal
 import json
 import pkg_resources
+from datascroller import scroll
 
 try:
     from . import BasicCypherCommands as bcc
 except:
     import BasicCypherCommands as bcc
 
 # Recording login time
@@ -79,15 +80,15 @@
 # The console allows you to type in cypher, and run it on the Neo4j pod you are connected to.
 # The console function needs to parameters: a Neo4j graph object, and a pod id. 
 # The graph object allows for queries to be interpreted as Cypher and passed into the Neo4j pod.
 # The pod id is only needed here so that the user can see what pod they are connected to.
         
 def console(graph, pod_id):
     # Instructions message, formatted with the lightFormat function
-    lightFormat("Type \"new\" to access a different pod, or type \"exit\" to leave ICICONSOLE. Type \"clear\" to clear the screen. Type \"help\" for help!")
+    lightFormat("Type \"new\" to access a different pod, or type \"exit\" to leave ICICONSOLE. Type \"help\" for help!\nNote that the scrolling menu, which appears on some queries, has a separate help menu.")
 
     # Loop so that the console keeps prompting the user for commands, until the user exits
     while(True):
         # This is reading the actual input from the user; the input message shows the username and the pod id
         query = str(input("[" + user + "@" + pod_id + "] "))
 
         executeCypher = True
@@ -126,19 +127,30 @@
                 query = bcc.allPropertiesForNode()
             case _:
                 pass
 
         if (executeCypher):
             # This tries to read the input as Cypher and apply the command to the Neo4j graph object.
             try: 
-                # Storing the results of the query as a pandas dataframe
-                df = graph.run(query).to_data_frame()
-                # Displaying the result
-                with pd.option_context('expand_frame_repr', False, 'display.max_rows', None): 
-                    print(df)
+                result = graph.run(query)
+                
+                try:
+                    data = []
+                    for record in result:
+                        node = record[0]
+                        properties = dict(node)
+                        data.append(properties)
+                    df = pd.DataFrame(data)
+                    with pd.option_context('display.max_rows', None, 'display.max_columns', None):
+                        scroll(df)
+                except:
+                    df = graph.run(query).to_data_frame()
+                    with pd.option_context('expand_frame_repr', False, 'display.max_rows', None): 
+                        print(df)
+
 
 
             # Error catching, if the Cypher was not executed properly
             except:
                 if flag.exit():
                     break
                 print("Something went wrong")
```

### Comparing `ICICONSOLE-0.0.7/ICICONSOLE.egg-info/PKG-INFO` & `ICICONSOLE-0.0.8/ICICONSOLE.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ICICONSOLE
-Version: 0.0.7
+Version: 0.0.8
 Summary: Command-line Interface tailored to working with Neo4j Knowledge Graph Databses hosted via Tapis Pods.
 Author-email: Sahil Samar <sahilsamar031@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ICICONSOLE-0.0.7/LICENSE` & `ICICONSOLE-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ICICONSOLE-0.0.7/PKG-INFO` & `ICICONSOLE-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ICICONSOLE
-Version: 0.0.7
+Version: 0.0.8
 Summary: Command-line Interface tailored to working with Neo4j Knowledge Graph Databses hosted via Tapis Pods.
 Author-email: Sahil Samar <sahilsamar031@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ICICONSOLE-0.0.7/README.md` & `ICICONSOLE-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `ICICONSOLE-0.0.7/pyproject.toml` & `ICICONSOLE-0.0.8/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -2,29 +2,30 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ICICONSOLE"
-version = "0.0.7"
+version = "0.0.8"
 description = "Command-line Interface tailored to working with Neo4j Knowledge Graph Databses hosted via Tapis Pods."
 readme = "README.md"
 authors = [{ name = "Sahil Samar", email = "sahilsamar031@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License (GPL)",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["Tapis", "CLI", "Agave", "HPC", "Tapis Pods", "TACC", "Neo4j"]
 dependencies = [
     "tapipy",
     "py2neo",
-    "pandas"
+    "pandas",
+    "datascroller"
 ]
 
 requires-python = ">=3.10"
 
 [project.optional-dependencies]
 dev = []
```

