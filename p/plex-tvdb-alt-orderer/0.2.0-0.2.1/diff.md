# Comparing `tmp/plex-tvdb-alt-orderer-0.2.0.tar.gz` & `tmp/plex-tvdb-alt-orderer-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plex-tvdb-alt-orderer-0.2.0.tar", last modified: Fri Jun  9 21:23:43 2023, max compression
+gzip compressed data, was "plex-tvdb-alt-orderer-0.2.1.tar", last modified: Fri Jun  9 21:40:09 2023, max compression
```

## Comparing `plex-tvdb-alt-orderer-0.2.0.tar` & `plex-tvdb-alt-orderer-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 21:23:43.819000 plex-tvdb-alt-orderer-0.2.0/
--rw-rw-rw-   0        0        0     1073 2023-06-07 23:45:38.000000 plex-tvdb-alt-orderer-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     5612 2023-06-09 21:23:43.817480 plex-tvdb-alt-orderer-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     4992 2023-06-09 21:17:45.000000 plex-tvdb-alt-orderer-0.2.0/README.md
--rw-rw-rw-   0        0        0      877 2023-06-09 21:00:18.000000 plex-tvdb-alt-orderer-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-09 21:23:43.819000 plex-tvdb-alt-orderer-0.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-09 21:23:43.712391 plex-tvdb-alt-orderer-0.2.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-09 21:23:43.746446 plex-tvdb-alt-orderer-0.2.0/src/plex_tvdb_alt_orderer/
--rw-rw-rw-   0        0        0     8107 2023-06-09 21:17:11.000000 plex-tvdb-alt-orderer-0.2.0/src/plex_tvdb_alt_orderer/main.py
-drwxrwxrwx   0        0        0        0 2023-06-09 21:23:43.807482 plex-tvdb-alt-orderer-0.2.0/src/plex_tvdb_alt_orderer.egg-info/
--rw-rw-rw-   0        0        0     5612 2023-06-09 21:23:43.000000 plex-tvdb-alt-orderer-0.2.0/src/plex_tvdb_alt_orderer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      362 2023-06-09 21:23:43.000000 plex-tvdb-alt-orderer-0.2.0/src/plex_tvdb_alt_orderer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 21:23:43.000000 plex-tvdb-alt-orderer-0.2.0/src/plex_tvdb_alt_orderer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       74 2023-06-09 21:23:43.000000 plex-tvdb-alt-orderer-0.2.0/src/plex_tvdb_alt_orderer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       70 2023-06-09 21:23:43.000000 plex-tvdb-alt-orderer-0.2.0/src/plex_tvdb_alt_orderer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-06-09 21:23:43.000000 plex-tvdb-alt-orderer-0.2.0/src/plex_tvdb_alt_orderer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 21:40:09.068298 plex-tvdb-alt-orderer-0.2.1/
+-rw-rw-rw-   0        0        0     1073 2023-06-07 23:45:38.000000 plex-tvdb-alt-orderer-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0     5870 2023-06-09 21:40:09.065297 plex-tvdb-alt-orderer-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5250 2023-06-09 21:39:05.000000 plex-tvdb-alt-orderer-0.2.1/README.md
+-rw-rw-rw-   0        0        0      877 2023-06-09 21:39:43.000000 plex-tvdb-alt-orderer-0.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-09 21:40:09.068298 plex-tvdb-alt-orderer-0.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-09 21:40:08.975751 plex-tvdb-alt-orderer-0.2.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-09 21:40:09.001753 plex-tvdb-alt-orderer-0.2.1/src/plex_tvdb_alt_orderer/
+-rw-rw-rw-   0        0        0     8107 2023-06-09 21:17:11.000000 plex-tvdb-alt-orderer-0.2.1/src/plex_tvdb_alt_orderer/main.py
+drwxrwxrwx   0        0        0        0 2023-06-09 21:40:09.063297 plex-tvdb-alt-orderer-0.2.1/src/plex_tvdb_alt_orderer.egg-info/
+-rw-rw-rw-   0        0        0     5870 2023-06-09 21:40:08.000000 plex-tvdb-alt-orderer-0.2.1/src/plex_tvdb_alt_orderer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      362 2023-06-09 21:40:08.000000 plex-tvdb-alt-orderer-0.2.1/src/plex_tvdb_alt_orderer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 21:40:08.000000 plex-tvdb-alt-orderer-0.2.1/src/plex_tvdb_alt_orderer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       74 2023-06-09 21:40:08.000000 plex-tvdb-alt-orderer-0.2.1/src/plex_tvdb_alt_orderer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       70 2023-06-09 21:40:08.000000 plex-tvdb-alt-orderer-0.2.1/src/plex_tvdb_alt_orderer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-06-09 21:40:08.000000 plex-tvdb-alt-orderer-0.2.1/src/plex_tvdb_alt_orderer.egg-info/top_level.txt
```

### Comparing `plex-tvdb-alt-orderer-0.2.0/LICENSE` & `plex-tvdb-alt-orderer-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `plex-tvdb-alt-orderer-0.2.0/PKG-INFO` & `plex-tvdb-alt-orderer-0.2.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plex-tvdb-alt-orderer
-Version: 0.2.0
+Version: 0.2.1
 Summary: A utility that applies alternate TVDB orders to Plex.
 Author: bpoxy
 Project-URL: Homepage, https://github.com/bpoxy/plex-tvdb-alt-orderer
 Project-URL: Bug Tracker, https://github.com/bpoxy/plex-tvdb-alt-orderer
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -80,37 +80,43 @@
 
 ### CLI
 ```
 Usage: plex-tvdb-alt-orderer [OPTIONS]
 
 Options:
   --plex-library TEXT   Your Plex TV show library name. Omit to use the
-                        PLEX_LIBRARY environment variable, choose from a list
-                        interactively or if your Plex server has a sole TV
-                        show library.
-  --plex-password TEXT  Your Plex password. Omit to use the PLEX_PASSWORD
-                        environment variable or enter interactively.
+                        ALT_ORDERER_PLEX_LIBRARY environment variable, choose
+                        from a list interactively or if your Plex server has a
+                        sole TV show library.
+  --plex-password TEXT  Your Plex password. Omit to use the
+                        ALT_ORDERER_PLEX_PASSWORD environment variable or
+                        enter interactively.
   --plex-server TEXT    Your Plex server name (user/password authentication)
                         or URL (token authentication). Omit to use the
-                        PLEX_SERVER environment variable or enter
+                        ALT_ORDERER_PLEX_SERVER environment variable or enter
                         interactively.
   --plex-show TEXT      The name of the show in Plex. Omit to use the
-                        PLEX_SHOW environment variable or enter interactively.
-  --plex-token TEXT     Your Plex token. Omit to use the PLEX_TOKEN
-                        environment variable or enter interactively.
-  --plex-user TEXT      Your Plex username. Omit to use the PLEX_USER
-                        environment variable or enter interactively.
-  --season INTEGER      The season to update (-1 to update the entire
-                        series). Omit to use the SEASON environment variable
-                        or enter interactively.
+                        ALT_ORDERER_PLEX_SHOW environment variable or enter
+                        interactively.
+  --plex-token TEXT     Your Plex token. Omit to use the
+                        ALT_ORDERER_PLEX_TOKEN environment variable or enter
+                        interactively.
+  --plex-user TEXT      Your Plex username. Omit to use the
+                        ALT_ORDERER_PLEX_USER environment variable or enter
+                        interactively.
+  --season INTEGER      The season to update (-1 to update the entire series).
+                        Omit to use the ALT_ORDERER_SEASON environment
+                        variable or enter interactively.
   --tvdb-order TEXT     The TVDB order name (as specified for API-connected
-                        systems). Omit to use the TVDB_ORDER environment
-                        variable or choose from a list interactively.
-  --tvdb-pin TEXT       Your TVDB subscriber PIN. Omit to use the TVDB_PIN
-                        environment variable or enter interactively.
+                        systems). Omit to use the ALT_ORDERER_TVDB_ORDER
+                        environment variable or choose from a list
+                        interactively.
+  --tvdb-pin TEXT       Your TVDB subscriber PIN. Omit to use the
+                        ALT_ORDERER_TVDB_PIN environment variable or enter
+                        interactively.
   --help                Show this message and exit.
 ```
 
 #### Example
 ```
 plex-tvdb-alt-orderer --plex-server "CoolGuyServer" --plex-user coolguy --plex-password P@$$W0RD --plex-show "Money Heist" --season -1 --tvdb-pin ABC1234 --tvdb-order "Alternate Order"
 ```
```

### Comparing `plex-tvdb-alt-orderer-0.2.0/README.md` & `plex-tvdb-alt-orderer-0.2.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -64,37 +64,43 @@
 
 ### CLI
 ```
 Usage: plex-tvdb-alt-orderer [OPTIONS]
 
 Options:
   --plex-library TEXT   Your Plex TV show library name. Omit to use the
-                        PLEX_LIBRARY environment variable, choose from a list
-                        interactively or if your Plex server has a sole TV
-                        show library.
-  --plex-password TEXT  Your Plex password. Omit to use the PLEX_PASSWORD
-                        environment variable or enter interactively.
+                        ALT_ORDERER_PLEX_LIBRARY environment variable, choose
+                        from a list interactively or if your Plex server has a
+                        sole TV show library.
+  --plex-password TEXT  Your Plex password. Omit to use the
+                        ALT_ORDERER_PLEX_PASSWORD environment variable or
+                        enter interactively.
   --plex-server TEXT    Your Plex server name (user/password authentication)
                         or URL (token authentication). Omit to use the
-                        PLEX_SERVER environment variable or enter
+                        ALT_ORDERER_PLEX_SERVER environment variable or enter
                         interactively.
   --plex-show TEXT      The name of the show in Plex. Omit to use the
-                        PLEX_SHOW environment variable or enter interactively.
-  --plex-token TEXT     Your Plex token. Omit to use the PLEX_TOKEN
-                        environment variable or enter interactively.
-  --plex-user TEXT      Your Plex username. Omit to use the PLEX_USER
-                        environment variable or enter interactively.
-  --season INTEGER      The season to update (-1 to update the entire
-                        series). Omit to use the SEASON environment variable
-                        or enter interactively.
+                        ALT_ORDERER_PLEX_SHOW environment variable or enter
+                        interactively.
+  --plex-token TEXT     Your Plex token. Omit to use the
+                        ALT_ORDERER_PLEX_TOKEN environment variable or enter
+                        interactively.
+  --plex-user TEXT      Your Plex username. Omit to use the
+                        ALT_ORDERER_PLEX_USER environment variable or enter
+                        interactively.
+  --season INTEGER      The season to update (-1 to update the entire series).
+                        Omit to use the ALT_ORDERER_SEASON environment
+                        variable or enter interactively.
   --tvdb-order TEXT     The TVDB order name (as specified for API-connected
-                        systems). Omit to use the TVDB_ORDER environment
-                        variable or choose from a list interactively.
-  --tvdb-pin TEXT       Your TVDB subscriber PIN. Omit to use the TVDB_PIN
-                        environment variable or enter interactively.
+                        systems). Omit to use the ALT_ORDERER_TVDB_ORDER
+                        environment variable or choose from a list
+                        interactively.
+  --tvdb-pin TEXT       Your TVDB subscriber PIN. Omit to use the
+                        ALT_ORDERER_TVDB_PIN environment variable or enter
+                        interactively.
   --help                Show this message and exit.
 ```
 
 #### Example
 ```
 plex-tvdb-alt-orderer --plex-server "CoolGuyServer" --plex-user coolguy --plex-password P@$$W0RD --plex-show "Money Heist" --season -1 --tvdb-pin ABC1234 --tvdb-order "Alternate Order"
 ```
```

### Comparing `plex-tvdb-alt-orderer-0.2.0/pyproject.toml` & `plex-tvdb-alt-orderer-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "plex-tvdb-alt-orderer"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   { name="bpoxy" },
 ]
 description = "A utility that applies alternate TVDB orders to Plex."
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = ["click", "inquirer", "plexapi", "progress", "termcolor", "tvdb_v4_official", "validators"]
```

### Comparing `plex-tvdb-alt-orderer-0.2.0/src/plex_tvdb_alt_orderer/main.py` & `plex-tvdb-alt-orderer-0.2.1/src/plex_tvdb_alt_orderer/main.py`

 * *Files identical despite different names*

### Comparing `plex-tvdb-alt-orderer-0.2.0/src/plex_tvdb_alt_orderer.egg-info/PKG-INFO` & `plex-tvdb-alt-orderer-0.2.1/src/plex_tvdb_alt_orderer.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plex-tvdb-alt-orderer
-Version: 0.2.0
+Version: 0.2.1
 Summary: A utility that applies alternate TVDB orders to Plex.
 Author: bpoxy
 Project-URL: Homepage, https://github.com/bpoxy/plex-tvdb-alt-orderer
 Project-URL: Bug Tracker, https://github.com/bpoxy/plex-tvdb-alt-orderer
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -80,37 +80,43 @@
 
 ### CLI
 ```
 Usage: plex-tvdb-alt-orderer [OPTIONS]
 
 Options:
   --plex-library TEXT   Your Plex TV show library name. Omit to use the
-                        PLEX_LIBRARY environment variable, choose from a list
-                        interactively or if your Plex server has a sole TV
-                        show library.
-  --plex-password TEXT  Your Plex password. Omit to use the PLEX_PASSWORD
-                        environment variable or enter interactively.
+                        ALT_ORDERER_PLEX_LIBRARY environment variable, choose
+                        from a list interactively or if your Plex server has a
+                        sole TV show library.
+  --plex-password TEXT  Your Plex password. Omit to use the
+                        ALT_ORDERER_PLEX_PASSWORD environment variable or
+                        enter interactively.
   --plex-server TEXT    Your Plex server name (user/password authentication)
                         or URL (token authentication). Omit to use the
-                        PLEX_SERVER environment variable or enter
+                        ALT_ORDERER_PLEX_SERVER environment variable or enter
                         interactively.
   --plex-show TEXT      The name of the show in Plex. Omit to use the
-                        PLEX_SHOW environment variable or enter interactively.
-  --plex-token TEXT     Your Plex token. Omit to use the PLEX_TOKEN
-                        environment variable or enter interactively.
-  --plex-user TEXT      Your Plex username. Omit to use the PLEX_USER
-                        environment variable or enter interactively.
-  --season INTEGER      The season to update (-1 to update the entire
-                        series). Omit to use the SEASON environment variable
-                        or enter interactively.
+                        ALT_ORDERER_PLEX_SHOW environment variable or enter
+                        interactively.
+  --plex-token TEXT     Your Plex token. Omit to use the
+                        ALT_ORDERER_PLEX_TOKEN environment variable or enter
+                        interactively.
+  --plex-user TEXT      Your Plex username. Omit to use the
+                        ALT_ORDERER_PLEX_USER environment variable or enter
+                        interactively.
+  --season INTEGER      The season to update (-1 to update the entire series).
+                        Omit to use the ALT_ORDERER_SEASON environment
+                        variable or enter interactively.
   --tvdb-order TEXT     The TVDB order name (as specified for API-connected
-                        systems). Omit to use the TVDB_ORDER environment
-                        variable or choose from a list interactively.
-  --tvdb-pin TEXT       Your TVDB subscriber PIN. Omit to use the TVDB_PIN
-                        environment variable or enter interactively.
+                        systems). Omit to use the ALT_ORDERER_TVDB_ORDER
+                        environment variable or choose from a list
+                        interactively.
+  --tvdb-pin TEXT       Your TVDB subscriber PIN. Omit to use the
+                        ALT_ORDERER_TVDB_PIN environment variable or enter
+                        interactively.
   --help                Show this message and exit.
 ```
 
 #### Example
 ```
 plex-tvdb-alt-orderer --plex-server "CoolGuyServer" --plex-user coolguy --plex-password P@$$W0RD --plex-show "Money Heist" --season -1 --tvdb-pin ABC1234 --tvdb-order "Alternate Order"
 ```
```

