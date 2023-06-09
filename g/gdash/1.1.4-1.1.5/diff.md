# Comparing `tmp/gdash-1.1.4.tar.gz` & `tmp/gdash-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdash-1.1.4.tar", last modified: Wed Apr 26 16:28:57 2023, max compression
+gzip compressed data, was "gdash-1.1.5.tar", last modified: Fri Jun  9 13:52:15 2023, max compression
```

## Comparing `gdash-1.1.4.tar` & `gdash-1.1.5.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:28:57.830726 gdash-1.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-26 16:28:07.000000 gdash-1.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-26 16:28:07.000000 gdash-1.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-26 16:28:57.830726 gdash-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-04-26 16:28:07.000000 gdash-1.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:28:57.826727 gdash-1.1.4/gdash/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 16:28:07.000000 gdash-1.1.4/gdash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-04-26 16:28:07.000000 gdash-1.1.4/gdash/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:28:57.826727 gdash-1.1.4/gdash/ui/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-26 16:28:55.000000 gdash-1.1.4/gdash/ui/asset-manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-26 16:28:55.000000 gdash-1.1.4/gdash/ui/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-04-26 16:28:43.000000 gdash-1.1.4/gdash/ui/logo-small.png
--rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-04-26 16:28:43.000000 gdash-1.1.4/gdash/ui/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-26 16:28:43.000000 gdash-1.1.4/gdash/ui/manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-26 16:28:43.000000 gdash-1.1.4/gdash/ui/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:28:57.822726 gdash-1.1.4/gdash/ui/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:28:57.826727 gdash-1.1.4/gdash/ui/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)    10171 2023-04-26 16:28:55.000000 gdash-1.1.4/gdash/ui/static/css/main.bb354ed4.css
--rw-r--r--   0 runner    (1001) docker     (123)    22664 2023-04-26 16:28:55.000000 gdash-1.1.4/gdash/ui/static/css/main.bb354ed4.css.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:28:57.826727 gdash-1.1.4/gdash/ui/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)   225286 2023-04-26 16:28:55.000000 gdash-1.1.4/gdash/ui/static/js/main.c4611ae3.js
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-04-26 16:28:55.000000 gdash-1.1.4/gdash/ui/static/js/main.c4611ae3.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)   912003 2023-04-26 16:28:55.000000 gdash-1.1.4/gdash/ui/static/js/main.c4611ae3.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:28:57.830726 gdash-1.1.4/gdash/ui/static/media/
--rw-r--r--   0 runner    (1001) docker     (123)    20692 2023-04-26 16:28:55.000000 gdash-1.1.4/gdash/ui/static/media/bg1.434ec9b5178c983b027e73e271858301.svg
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-26 16:28:21.000000 gdash-1.1.4/gdash/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:28:57.826727 gdash-1.1.4/gdash.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-26 16:28:57.000000 gdash-1.1.4/gdash.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-26 16:28:57.000000 gdash-1.1.4/gdash.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 16:28:57.000000 gdash-1.1.4/gdash.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-26 16:28:57.000000 gdash-1.1.4/gdash.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 16:28:57.000000 gdash-1.1.4/gdash.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-26 16:28:57.000000 gdash-1.1.4/gdash.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-26 16:28:57.000000 gdash-1.1.4/gdash.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-26 16:28:57.830726 gdash-1.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-04-26 16:28:07.000000 gdash-1.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:52:15.202669 gdash-1.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-09 13:51:30.000000 gdash-1.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-09 13:51:30.000000 gdash-1.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-09 13:52:15.202669 gdash-1.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-06-09 13:51:30.000000 gdash-1.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:52:15.198669 gdash-1.1.5/gdash/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 13:51:30.000000 gdash-1.1.5/gdash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-06-09 13:51:30.000000 gdash-1.1.5/gdash/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:52:15.198669 gdash-1.1.5/gdash/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-09 13:52:13.000000 gdash-1.1.5/gdash/ui/asset-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-09 13:52:13.000000 gdash-1.1.5/gdash/ui/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-06-09 13:52:01.000000 gdash-1.1.5/gdash/ui/logo-small.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-06-09 13:52:01.000000 gdash-1.1.5/gdash/ui/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-09 13:52:01.000000 gdash-1.1.5/gdash/ui/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-09 13:52:01.000000 gdash-1.1.5/gdash/ui/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:52:15.198669 gdash-1.1.5/gdash/ui/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:52:15.198669 gdash-1.1.5/gdash/ui/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    10171 2023-06-09 13:52:13.000000 gdash-1.1.5/gdash/ui/static/css/main.bb354ed4.css
+-rw-r--r--   0 runner    (1001) docker     (123)    22664 2023-06-09 13:52:13.000000 gdash-1.1.5/gdash/ui/static/css/main.bb354ed4.css.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:52:15.198669 gdash-1.1.5/gdash/ui/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)   225286 2023-06-09 13:52:13.000000 gdash-1.1.5/gdash/ui/static/js/main.c4611ae3.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-06-09 13:52:13.000000 gdash-1.1.5/gdash/ui/static/js/main.c4611ae3.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   912003 2023-06-09 13:52:13.000000 gdash-1.1.5/gdash/ui/static/js/main.c4611ae3.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:52:15.202669 gdash-1.1.5/gdash/ui/static/media/
+-rw-r--r--   0 runner    (1001) docker     (123)    20692 2023-06-09 13:52:13.000000 gdash-1.1.5/gdash/ui/static/media/bg1.434ec9b5178c983b027e73e271858301.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-09 13:51:38.000000 gdash-1.1.5/gdash/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:52:15.198669 gdash-1.1.5/gdash.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-09 13:52:15.000000 gdash-1.1.5/gdash.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-09 13:52:15.000000 gdash-1.1.5/gdash.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 13:52:15.000000 gdash-1.1.5/gdash.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-09 13:52:15.000000 gdash-1.1.5/gdash.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 13:52:15.000000 gdash-1.1.5/gdash.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-09 13:52:15.000000 gdash-1.1.5/gdash.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-09 13:52:15.000000 gdash-1.1.5/gdash.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-09 13:52:15.202669 gdash-1.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-06-09 13:51:30.000000 gdash-1.1.5/setup.py
```

### Comparing `gdash-1.1.4/LICENSE` & `gdash-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gdash-1.1.4/PKG-INFO` & `gdash-1.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdash
-Version: 1.1.4
+Version: 1.1.5
 Summary: GlusterFS Dashboard
 Home-page: https://github.com/kadalu/gdash
 Author: Aravinda Vishwanathapura
 Author-email: aravinda@kadalu.io
 License: Apache-2.0
 Keywords: glusterfs,gui,dashboard
 Platform: linux
```

### Comparing `gdash-1.1.4/README.md` & `gdash-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `gdash-1.1.4/gdash/__main__.py` & `gdash-1.1.5/gdash/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -169,14 +169,17 @@
     )
     parser.add_argument(
         "--ssl-key", default=None, help=("Path to SSL Key used by Gdash")
     )
     parser.add_argument(
         "--ssl-ca", default=None, help=("Path to SSL CA Certificate used by Gdash")
     )
+    parser.add_argument(
+        "--ssl-ciphers", default=None, help=("List of SSL Ciphers to allow")
+    )
 
     return parser.parse_args()
 
 
 def main():
     global ARGS, USERS
 
@@ -200,14 +203,17 @@
 
     if ARGS.ssl_key:
         cherrypy_cfg["server.ssl_private_key"] = ARGS.ssl_key
 
     if ARGS.ssl_ca:
         cherrypy_cfg["server.ssl_certificate_chain"] = ARGS.ssl_ca
 
+    if ARGS.ssl_ciphers:
+        cherrypy_cfg["server.ssl_ciphers"] = ARGS.ssl_ciphers
+
     if ARGS.ssl_cert and ARGS.ssl_key:
         cherrypy_cfg["server.ssl_module"] = "builtin"
 
     cherrypy.config.update(cherrypy_cfg)
     webapp = GdashWeb()
     webapp.api = GdashApis()
     cherrypy.quickstart(webapp, "/", conf)
```

### Comparing `gdash-1.1.4/gdash/ui/index.html` & `gdash-1.1.5/gdash/ui/index.html`

 * *Files identical despite different names*

### Comparing `gdash-1.1.4/gdash/ui/logo-small.png` & `gdash-1.1.5/gdash/ui/logo-small.png`

 * *Files identical despite different names*

### Comparing `gdash-1.1.4/gdash/ui/logo.png` & `gdash-1.1.5/gdash/ui/logo.png`

 * *Files identical despite different names*

### Comparing `gdash-1.1.4/gdash/ui/static/css/main.bb354ed4.css` & `gdash-1.1.5/gdash/ui/static/css/main.bb354ed4.css`

 * *Files identical despite different names*

### Comparing `gdash-1.1.4/gdash/ui/static/css/main.bb354ed4.css.map` & `gdash-1.1.5/gdash/ui/static/css/main.bb354ed4.css.map`

 * *Files identical despite different names*

### Comparing `gdash-1.1.4/gdash/ui/static/js/main.c4611ae3.js` & `gdash-1.1.5/gdash/ui/static/js/main.c4611ae3.js`

 * *Files identical despite different names*

### Comparing `gdash-1.1.4/gdash/ui/static/js/main.c4611ae3.js.LICENSE.txt` & `gdash-1.1.5/gdash/ui/static/js/main.c4611ae3.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gdash-1.1.4/gdash/ui/static/js/main.c4611ae3.js.map` & `gdash-1.1.5/gdash/ui/static/js/main.c4611ae3.js.map`

 * *Files identical despite different names*

### Comparing `gdash-1.1.4/gdash/ui/static/media/bg1.434ec9b5178c983b027e73e271858301.svg` & `gdash-1.1.5/gdash/ui/static/media/bg1.434ec9b5178c983b027e73e271858301.svg`

 * *Files identical despite different names*

### Comparing `gdash-1.1.4/gdash.egg-info/PKG-INFO` & `gdash-1.1.5/gdash.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdash
-Version: 1.1.4
+Version: 1.1.5
 Summary: GlusterFS Dashboard
 Home-page: https://github.com/kadalu/gdash
 Author: Aravinda Vishwanathapura
 Author-email: aravinda@kadalu.io
 License: Apache-2.0
 Keywords: glusterfs,gui,dashboard
 Platform: linux
```

### Comparing `gdash-1.1.4/gdash.egg-info/SOURCES.txt` & `gdash-1.1.5/gdash.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gdash-1.1.4/setup.py` & `gdash-1.1.5/setup.py`

 * *Files identical despite different names*

