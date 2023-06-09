# Comparing `tmp/lifeguard-simple-dashboard-0.0.3.tar.gz` & `tmp/lifeguard-simple-dashboard-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lifeguard-simple-dashboard-0.0.3.tar", last modified: Wed May 24 12:42:38 2023, max compression
+gzip compressed data, was "lifeguard-simple-dashboard-1.0.0.tar", last modified: Fri Jun  9 14:19:49 2023, max compression
```

## Comparing `lifeguard-simple-dashboard-0.0.3.tar` & `lifeguard-simple-dashboard-1.0.0.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:42:38.004780 lifeguard-simple-dashboard-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-24 12:41:52.000000 lifeguard-simple-dashboard-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-24 12:42:38.004780 lifeguard-simple-dashboard-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-24 12:41:52.000000 lifeguard-simple-dashboard-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:42:38.004780 lifeguard-simple-dashboard-0.0.3/lifeguard_simple_dashboard/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-24 12:41:52.000000 lifeguard-simple-dashboard-0.0.3/lifeguard_simple_dashboard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:42:38.004780 lifeguard-simple-dashboard-0.0.3/lifeguard_simple_dashboard/controllers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 12:41:52.000000 lifeguard-simple-dashboard-0.0.3/lifeguard_simple_dashboard/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-05-24 12:41:52.000000 lifeguard-simple-dashboard-0.0.3/lifeguard_simple_dashboard/controllers/index_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:42:38.000780 lifeguard-simple-dashboard-0.0.3/lifeguard_simple_dashboard/public/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:42:38.004780 lifeguard-simple-dashboard-0.0.3/lifeguard_simple_dashboard/public/css/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 12:41:52.000000 lifeguard-simple-dashboard-0.0.3/lifeguard_simple_dashboard/public/css/dashboard.css
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-24 12:41:52.000000 lifeguard-simple-dashboard-0.0.3/lifeguard_simple_dashboard/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:42:38.004780 lifeguard-simple-dashboard-0.0.3/lifeguard_simple_dashboard/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-24 12:41:52.000000 lifeguard-simple-dashboard-0.0.3/lifeguard_simple_dashboard/templates/dashboard.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:42:38.004780 lifeguard-simple-dashboard-0.0.3/lifeguard_simple_dashboard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-24 12:42:37.000000 lifeguard-simple-dashboard-0.0.3/lifeguard_simple_dashboard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-24 12:42:37.000000 lifeguard-simple-dashboard-0.0.3/lifeguard_simple_dashboard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 12:42:37.000000 lifeguard-simple-dashboard-0.0.3/lifeguard_simple_dashboard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-24 12:42:37.000000 lifeguard-simple-dashboard-0.0.3/lifeguard_simple_dashboard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-24 12:42:37.000000 lifeguard-simple-dashboard-0.0.3/lifeguard_simple_dashboard.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 12:42:38.004780 lifeguard-simple-dashboard-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-24 12:41:52.000000 lifeguard-simple-dashboard-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:19:49.604134 lifeguard-simple-dashboard-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-09 14:19:01.000000 lifeguard-simple-dashboard-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-09 14:19:49.604134 lifeguard-simple-dashboard-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-09 14:19:01.000000 lifeguard-simple-dashboard-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:19:49.600134 lifeguard-simple-dashboard-1.0.0/lifeguard_simple_dashboard/
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-09 14:19:01.000000 lifeguard-simple-dashboard-1.0.0/lifeguard_simple_dashboard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:19:49.600134 lifeguard-simple-dashboard-1.0.0/lifeguard_simple_dashboard/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 14:19:01.000000 lifeguard-simple-dashboard-1.0.0/lifeguard_simple_dashboard/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-06-09 14:19:01.000000 lifeguard-simple-dashboard-1.0.0/lifeguard_simple_dashboard/controllers/index_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:19:49.600134 lifeguard-simple-dashboard-1.0.0/lifeguard_simple_dashboard/public/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:19:49.600134 lifeguard-simple-dashboard-1.0.0/lifeguard_simple_dashboard/public/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-09 14:19:01.000000 lifeguard-simple-dashboard-1.0.0/lifeguard_simple_dashboard/public/css/dashboard.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:19:49.600134 lifeguard-simple-dashboard-1.0.0/lifeguard_simple_dashboard/public/img/
+-rw-r--r--   0 runner    (1001) docker     (123)  2179899 2023-06-09 14:19:01.000000 lifeguard-simple-dashboard-1.0.0/lifeguard_simple_dashboard/public/img/wallpaper.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-09 14:19:01.000000 lifeguard-simple-dashboard-1.0.0/lifeguard_simple_dashboard/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:19:49.604134 lifeguard-simple-dashboard-1.0.0/lifeguard_simple_dashboard/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-09 14:19:01.000000 lifeguard-simple-dashboard-1.0.0/lifeguard_simple_dashboard/templates/dashboard.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:19:49.600134 lifeguard-simple-dashboard-1.0.0/lifeguard_simple_dashboard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-09 14:19:49.000000 lifeguard-simple-dashboard-1.0.0/lifeguard_simple_dashboard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-09 14:19:49.000000 lifeguard-simple-dashboard-1.0.0/lifeguard_simple_dashboard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 14:19:49.000000 lifeguard-simple-dashboard-1.0.0/lifeguard_simple_dashboard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-09 14:19:49.000000 lifeguard-simple-dashboard-1.0.0/lifeguard_simple_dashboard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-09 14:19:49.000000 lifeguard-simple-dashboard-1.0.0/lifeguard_simple_dashboard.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 14:19:49.604134 lifeguard-simple-dashboard-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-09 14:19:01.000000 lifeguard-simple-dashboard-1.0.0/setup.py
```

### Comparing `lifeguard-simple-dashboard-0.0.3/lifeguard_simple_dashboard/controllers/index_controller.py` & `lifeguard-simple-dashboard-1.0.0/lifeguard_simple_dashboard/controllers/index_controller.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,31 +21,39 @@
 
 def send_status(status):
     response = Response()
     response.status = status
     return response
 
 
-def send_file(path, content_type):
+def send_file(path, content_type, opentype="r"):
     absolute_path = pathlib.Path(__file__).parent.parent.absolute()
-    with open(join(absolute_path, "public", path), "r") as file:
+    with open(join(absolute_path, "public", path), opentype) as file:
         response = Response()
         response.content = file.read()
         response.content_type = content_type
         return response
 
 
 def dashboard_send_css(path):
     try:
         logger.info("returning css %s", path)
         return send_file("css/{}".format(path), "text/css")
     except:
         return send_status(404)
 
 
+def dashboard_send_img(path):
+    try:
+        logger.info("returning img %s", path)
+        return send_file("img/{}".format(path), "image/jpeg", "rb")
+    except:
+        return send_status(404)
+
+
 def index():
     try:
         logger.info("rendering index")
         validations = ValidationRepository().fetch_all_validation_results()
         return render_template(
             "dashboard.html",
             {
```

### Comparing `lifeguard-simple-dashboard-0.0.3/lifeguard_simple_dashboard.egg-info/SOURCES.txt` & `lifeguard-simple-dashboard-1.0.0/lifeguard_simple_dashboard.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -7,8 +7,9 @@
 lifeguard_simple_dashboard.egg-info/SOURCES.txt
 lifeguard_simple_dashboard.egg-info/dependency_links.txt
 lifeguard_simple_dashboard.egg-info/requires.txt
 lifeguard_simple_dashboard.egg-info/top_level.txt
 lifeguard_simple_dashboard/controllers/__init__.py
 lifeguard_simple_dashboard/controllers/index_controller.py
 lifeguard_simple_dashboard/public/css/dashboard.css
+lifeguard_simple_dashboard/public/img/wallpaper.jpg
 lifeguard_simple_dashboard/templates/dashboard.html
```

