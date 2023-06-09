# Comparing `tmp/voila-material-tuwien-0.4.4.tar.gz` & `tmp/voila-material-tuwien-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voila-material-tuwien-0.4.4.tar", last modified: Tue May 23 09:20:53 2023, max compression
+gzip compressed data, was "voila-material-tuwien-0.4.5.tar", last modified: Fri Jun  9 07:16:53 2023, max compression
```

## Comparing `voila-material-tuwien-0.4.4.tar` & `voila-material-tuwien-0.4.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 fjaeger   (1001) fjaeger   (1001)        0 2023-05-23 09:20:53.612072 voila-material-tuwien-0.4.4/
--rw-rw-r--   0 fjaeger   (1001) fjaeger   (1001)     1538 2023-05-22 09:48:36.000000 voila-material-tuwien-0.4.4/LICENSE
--rw-rw-r--   0 fjaeger   (1001) fjaeger   (1001)      286 2023-05-23 09:20:53.608072 voila-material-tuwien-0.4.4/PKG-INFO
--rw-rw-r--   0 fjaeger   (1001) fjaeger   (1001)      748 2023-05-22 09:48:36.000000 voila-material-tuwien-0.4.4/README.md
--rw-rw-r--   0 fjaeger   (1001) fjaeger   (1001)       38 2023-05-23 09:20:53.612072 voila-material-tuwien-0.4.4/setup.cfg
--rw-rw-r--   0 fjaeger   (1001) fjaeger   (1001)     3218 2023-05-23 09:16:06.000000 voila-material-tuwien-0.4.4/setup.py
-drwxrwxr-x   0 fjaeger   (1001) fjaeger   (1001)        0 2023-05-23 09:20:53.604072 voila-material-tuwien-0.4.4/share/
-drwxrwxr-x   0 fjaeger   (1001) fjaeger   (1001)        0 2023-05-23 09:20:53.608072 voila-material-tuwien-0.4.4/share/jupyter/
-drwxrwxr-x   0 fjaeger   (1001) fjaeger   (1001)        0 2023-05-23 09:20:53.604072 voila-material-tuwien-0.4.4/share/jupyter/nbconvert/
-drwxrwxr-x   0 fjaeger   (1001) fjaeger   (1001)        0 2023-05-23 09:20:53.604072 voila-material-tuwien-0.4.4/share/jupyter/nbconvert/templates/
-drwxrwxr-x   0 fjaeger   (1001) fjaeger   (1001)        0 2023-05-23 09:20:53.608072 voila-material-tuwien-0.4.4/share/jupyter/nbconvert/templates/material-tuwien/
--rw-rw-r--   0 fjaeger   (1001) fjaeger   (1001)       24 2023-05-22 10:17:39.000000 voila-material-tuwien-0.4.4/share/jupyter/nbconvert/templates/material-tuwien/conf.json
--rw-rw-r--   0 fjaeger   (1001) fjaeger   (1001)     2250 2023-05-23 08:10:46.000000 voila-material-tuwien-0.4.4/share/jupyter/nbconvert/templates/material-tuwien/index.html.j2
-drwxrwxr-x   0 fjaeger   (1001) fjaeger   (1001)        0 2023-05-23 09:20:53.608072 voila-material-tuwien-0.4.4/share/jupyter/nbconvert/templates/material-tuwien/static/
--rw-rw-r--   0 fjaeger   (1001) fjaeger   (1001)   174112 2023-05-22 10:17:39.000000 voila-material-tuwien-0.4.4/share/jupyter/nbconvert/templates/material-tuwien/static/icons_font.ttf
--rw-rw-r--   0 fjaeger   (1001) fjaeger   (1001)    18664 2023-05-23 08:17:23.000000 voila-material-tuwien-0.4.4/share/jupyter/nbconvert/templates/material-tuwien/static/logo.svg
--rw-rw-r--   0 fjaeger   (1001) fjaeger   (1001)   141851 2023-05-23 09:16:42.000000 voila-material-tuwien-0.4.4/share/jupyter/nbconvert/templates/material-tuwien/static/materialize.min.css
--rw-rw-r--   0 fjaeger   (1001) fjaeger   (1001)   181109 2023-05-22 10:17:39.000000 voila-material-tuwien-0.4.4/share/jupyter/nbconvert/templates/material-tuwien/static/materialize.min.js
--rw-rw-r--   0 fjaeger   (1001) fjaeger   (1001)    15106 2023-05-23 08:26:34.000000 voila-material-tuwien-0.4.4/share/jupyter/nbconvert/templates/material-tuwien/static/voila_logo_bleu.svg
-drwxrwxr-x   0 fjaeger   (1001) fjaeger   (1001)        0 2023-05-23 09:20:53.608072 voila-material-tuwien-0.4.4/share/jupyter/voila/
-drwxrwxr-x   0 fjaeger   (1001) fjaeger   (1001)        0 2023-05-23 09:20:53.608072 voila-material-tuwien-0.4.4/share/jupyter/voila/templates/
-drwxrwxr-x   0 fjaeger   (1001) fjaeger   (1001)        0 2023-05-23 09:20:53.608072 voila-material-tuwien-0.4.4/share/jupyter/voila/templates/material-tuwien/
--rw-rw-r--   0 fjaeger   (1001) fjaeger   (1001)      189 2023-05-22 10:17:39.000000 voila-material-tuwien-0.4.4/share/jupyter/voila/templates/material-tuwien/404.html
--rw-rw-r--   0 fjaeger   (1001) fjaeger   (1001)     3141 2023-05-22 10:33:26.000000 voila-material-tuwien-0.4.4/share/jupyter/voila/templates/material-tuwien/base.html
--rw-rw-r--   0 fjaeger   (1001) fjaeger   (1001)      330 2023-05-22 10:17:39.000000 voila-material-tuwien-0.4.4/share/jupyter/voila/templates/material-tuwien/browser-open.html
--rw-rw-r--   0 fjaeger   (1001) fjaeger   (1001)      373 2023-05-22 10:17:39.000000 voila-material-tuwien-0.4.4/share/jupyter/voila/templates/material-tuwien/error.html
--rw-rw-r--   0 fjaeger   (1001) fjaeger   (1001)     1612 2023-05-22 10:33:11.000000 voila-material-tuwien-0.4.4/share/jupyter/voila/templates/material-tuwien/index.html.j2
--rw-rw-r--   0 fjaeger   (1001) fjaeger   (1001)     1481 2023-05-23 08:02:00.000000 voila-material-tuwien-0.4.4/share/jupyter/voila/templates/material-tuwien/tree.html
-drwxrwxr-x   0 fjaeger   (1001) fjaeger   (1001)        0 2023-05-23 09:20:53.608072 voila-material-tuwien-0.4.4/voila_material_tuwien.egg-info/
--rw-rw-r--   0 fjaeger   (1001) fjaeger   (1001)      286 2023-05-23 09:20:53.000000 voila-material-tuwien-0.4.4/voila_material_tuwien.egg-info/PKG-INFO
--rw-rw-r--   0 fjaeger   (1001) fjaeger   (1001)     1090 2023-05-23 09:20:53.000000 voila-material-tuwien-0.4.4/voila_material_tuwien.egg-info/SOURCES.txt
--rw-rw-r--   0 fjaeger   (1001) fjaeger   (1001)        1 2023-05-23 09:20:53.000000 voila-material-tuwien-0.4.4/voila_material_tuwien.egg-info/dependency_links.txt
--rw-rw-r--   0 fjaeger   (1001) fjaeger   (1001)       20 2023-05-23 09:20:53.000000 voila-material-tuwien-0.4.4/voila_material_tuwien.egg-info/requires.txt
--rw-rw-r--   0 fjaeger   (1001) fjaeger   (1001)        1 2023-05-23 09:20:53.000000 voila-material-tuwien-0.4.4/voila_material_tuwien.egg-info/top_level.txt
+drwxrwxr-x   0 fjaeger   (1001) fjaeger   (1001)        0 2023-06-09 07:16:53.252364 voila-material-tuwien-0.4.5/
+-rw-rw-r--   0 fjaeger   (1001) fjaeger   (1001)     1538 2023-05-22 09:48:36.000000 voila-material-tuwien-0.4.5/LICENSE
+-rw-rw-r--   0 fjaeger   (1001) fjaeger   (1001)      329 2023-06-09 07:16:53.252364 voila-material-tuwien-0.4.5/PKG-INFO
+-rw-rw-r--   0 fjaeger   (1001) fjaeger   (1001)      748 2023-05-22 09:48:36.000000 voila-material-tuwien-0.4.5/README.md
+-rw-rw-r--   0 fjaeger   (1001) fjaeger   (1001)       38 2023-06-09 07:16:53.252364 voila-material-tuwien-0.4.5/setup.cfg
+-rw-rw-r--   0 fjaeger   (1001) fjaeger   (1001)     3261 2023-06-09 07:06:47.000000 voila-material-tuwien-0.4.5/setup.py
+drwxrwxr-x   0 fjaeger   (1001) fjaeger   (1001)        0 2023-06-09 07:16:53.248364 voila-material-tuwien-0.4.5/share/
+drwxrwxr-x   0 fjaeger   (1001) fjaeger   (1001)        0 2023-06-09 07:16:53.248364 voila-material-tuwien-0.4.5/share/jupyter/
+drwxrwxr-x   0 fjaeger   (1001) fjaeger   (1001)        0 2023-06-09 07:16:53.248364 voila-material-tuwien-0.4.5/share/jupyter/nbconvert/
+drwxrwxr-x   0 fjaeger   (1001) fjaeger   (1001)        0 2023-06-09 07:16:53.248364 voila-material-tuwien-0.4.5/share/jupyter/nbconvert/templates/
+drwxrwxr-x   0 fjaeger   (1001) fjaeger   (1001)        0 2023-06-09 07:16:53.248364 voila-material-tuwien-0.4.5/share/jupyter/nbconvert/templates/material-tuwien/
+-rw-rw-r--   0 fjaeger   (1001) fjaeger   (1001)       24 2023-05-22 10:17:39.000000 voila-material-tuwien-0.4.5/share/jupyter/nbconvert/templates/material-tuwien/conf.json
+-rw-rw-r--   0 fjaeger   (1001) fjaeger   (1001)     2250 2023-06-09 07:03:01.000000 voila-material-tuwien-0.4.5/share/jupyter/nbconvert/templates/material-tuwien/index.html.j2
+drwxrwxr-x   0 fjaeger   (1001) fjaeger   (1001)        0 2023-06-09 07:16:53.248364 voila-material-tuwien-0.4.5/share/jupyter/nbconvert/templates/material-tuwien/static/
+-rw-rw-r--   0 fjaeger   (1001) fjaeger   (1001)   174112 2023-05-22 10:17:39.000000 voila-material-tuwien-0.4.5/share/jupyter/nbconvert/templates/material-tuwien/static/icons_font.ttf
+-rw-rw-r--   0 fjaeger   (1001) fjaeger   (1001)    18664 2023-05-23 08:17:23.000000 voila-material-tuwien-0.4.5/share/jupyter/nbconvert/templates/material-tuwien/static/logo.svg
+-rw-rw-r--   0 fjaeger   (1001) fjaeger   (1001)   141851 2023-05-23 09:16:42.000000 voila-material-tuwien-0.4.5/share/jupyter/nbconvert/templates/material-tuwien/static/materialize.min.css
+-rw-rw-r--   0 fjaeger   (1001) fjaeger   (1001)   181109 2023-05-22 10:17:39.000000 voila-material-tuwien-0.4.5/share/jupyter/nbconvert/templates/material-tuwien/static/materialize.min.js
+-rw-rw-r--   0 fjaeger   (1001) fjaeger   (1001)    15106 2023-05-23 08:26:34.000000 voila-material-tuwien-0.4.5/share/jupyter/nbconvert/templates/material-tuwien/static/voila_logo_bleu.svg
+drwxrwxr-x   0 fjaeger   (1001) fjaeger   (1001)        0 2023-06-09 07:16:53.248364 voila-material-tuwien-0.4.5/share/jupyter/voila/
+drwxrwxr-x   0 fjaeger   (1001) fjaeger   (1001)        0 2023-06-09 07:16:53.248364 voila-material-tuwien-0.4.5/share/jupyter/voila/templates/
+drwxrwxr-x   0 fjaeger   (1001) fjaeger   (1001)        0 2023-06-09 07:16:53.252364 voila-material-tuwien-0.4.5/share/jupyter/voila/templates/material-tuwien/
+-rw-rw-r--   0 fjaeger   (1001) fjaeger   (1001)      189 2023-05-22 10:17:39.000000 voila-material-tuwien-0.4.5/share/jupyter/voila/templates/material-tuwien/404.html
+-rw-rw-r--   0 fjaeger   (1001) fjaeger   (1001)     3141 2023-06-09 07:02:57.000000 voila-material-tuwien-0.4.5/share/jupyter/voila/templates/material-tuwien/base.html
+-rw-rw-r--   0 fjaeger   (1001) fjaeger   (1001)      330 2023-05-22 10:17:39.000000 voila-material-tuwien-0.4.5/share/jupyter/voila/templates/material-tuwien/browser-open.html
+-rw-rw-r--   0 fjaeger   (1001) fjaeger   (1001)      373 2023-05-22 10:17:39.000000 voila-material-tuwien-0.4.5/share/jupyter/voila/templates/material-tuwien/error.html
+-rw-rw-r--   0 fjaeger   (1001) fjaeger   (1001)     1612 2023-05-22 10:33:11.000000 voila-material-tuwien-0.4.5/share/jupyter/voila/templates/material-tuwien/index.html.j2
+-rw-rw-r--   0 fjaeger   (1001) fjaeger   (1001)     1481 2023-05-23 08:02:00.000000 voila-material-tuwien-0.4.5/share/jupyter/voila/templates/material-tuwien/tree.html
+drwxrwxr-x   0 fjaeger   (1001) fjaeger   (1001)        0 2023-06-09 07:16:53.252364 voila-material-tuwien-0.4.5/voila_material_tuwien.egg-info/
+-rw-rw-r--   0 fjaeger   (1001) fjaeger   (1001)      329 2023-06-09 07:16:53.000000 voila-material-tuwien-0.4.5/voila_material_tuwien.egg-info/PKG-INFO
+-rw-rw-r--   0 fjaeger   (1001) fjaeger   (1001)     1090 2023-06-09 07:16:53.000000 voila-material-tuwien-0.4.5/voila_material_tuwien.egg-info/SOURCES.txt
+-rw-rw-r--   0 fjaeger   (1001) fjaeger   (1001)        1 2023-06-09 07:16:53.000000 voila-material-tuwien-0.4.5/voila_material_tuwien.egg-info/dependency_links.txt
+-rw-rw-r--   0 fjaeger   (1001) fjaeger   (1001)       20 2023-06-09 07:16:53.000000 voila-material-tuwien-0.4.5/voila_material_tuwien.egg-info/requires.txt
+-rw-rw-r--   0 fjaeger   (1001) fjaeger   (1001)        1 2023-06-09 07:16:53.000000 voila-material-tuwien-0.4.5/voila_material_tuwien.egg-info/top_level.txt
```

### Comparing `voila-material-tuwien-0.4.4/LICENSE` & `voila-material-tuwien-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `voila-material-tuwien-0.4.4/README.md` & `voila-material-tuwien-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `voila-material-tuwien-0.4.4/setup.py` & `voila-material-tuwien-0.4.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -81,21 +81,21 @@
 for (dirpath, dirnames, filenames) in os.walk('share/jupyter/'):
     if filenames:
         data_files.append((dirpath, [os.path.join(dirpath, filename) for filename in filenames]))
 
 
 setup(
     name='voila-material-tuwien',
-    version="0.4.4",
-    description="Material design template for voila",
+    version="0.4.5",
+    description="TU Wien material design template for voila",
     data_files=data_files,
     include_package_data=True,
     author=['Voila Development Team','Florian Jaeger'],
     install_requires=['voila>=0.2.1,<0.6.0'],
-    url='https://github.com/voila-dashboards/voila-material',
+    url='https://gitlab.tuwien.ac.at/hpc/datalab/jupyter/voila/voila-material-tu-wien-template',
     keywords=[
         'ipython',
         'jupyter',
         'widgets',
         'voila'
     ],
     packages=[],
```

### Comparing `voila-material-tuwien-0.4.4/share/jupyter/nbconvert/templates/material-tuwien/index.html.j2` & `voila-material-tuwien-0.4.5/share/jupyter/nbconvert/templates/material-tuwien/index.html.j2`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 {% endblock notebook_execute %}
 
 {%- block html_head_css -%}
 {{ super() }}
 {% if resources.theme == 'dark' %}
 {% set bar_color = '#555454' %}
 {% else %}
-{% set bar_color = '#5cbcaf' %}
+{% set bar_color = '#006699' %}
 {% endif %}
 {{ resources.include_css("static/materialize.min.css") }}
 
 <style type="text/css">
   body {
     background-color: var(--jp-layout-color0);
     overflow-y: scroll;
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 {%- extends 'lab/index.html.j2' -%} {# this overrides the default behavior of
 directly starting the kernel and executing the notebook #} {% block
 notebook_execute %} {% endblock notebook_execute %} {%- block html_head_css -%}
 {{ super() }} {% if resources.theme == 'dark' %} {% set bar_color = '#555454'
-%} {% else %} {% set bar_color = '#5cbcaf' %} {% endif %} {
+%} {% else %} {% set bar_color = '#006699' %} {% endif %} {
 { resources.include_css("static/materialize.min.css") }}
  {%- endblock html_head_css -%} {%- block body -%} {%- block body_header -%} {
 { super() }}
 ogo.svg") }}">
     * radio_button_unchecked
 
 {%- endblock body_header -%} {%- block body_loop -%} {% if resources.theme ==
```

### Comparing `voila-material-tuwien-0.4.4/share/jupyter/nbconvert/templates/material-tuwien/static/icons_font.ttf` & `voila-material-tuwien-0.4.5/share/jupyter/nbconvert/templates/material-tuwien/static/icons_font.ttf`

 * *Files identical despite different names*

### Comparing `voila-material-tuwien-0.4.4/share/jupyter/nbconvert/templates/material-tuwien/static/logo.svg` & `voila-material-tuwien-0.4.5/share/jupyter/nbconvert/templates/material-tuwien/static/logo.svg`

 * *Files identical despite different names*

### Comparing `voila-material-tuwien-0.4.4/share/jupyter/nbconvert/templates/material-tuwien/static/materialize.min.css` & `voila-material-tuwien-0.4.5/share/jupyter/nbconvert/templates/material-tuwien/static/materialize.min.css`

 * *Files identical despite different names*

### Comparing `voila-material-tuwien-0.4.4/share/jupyter/nbconvert/templates/material-tuwien/static/materialize.min.js` & `voila-material-tuwien-0.4.5/share/jupyter/nbconvert/templates/material-tuwien/static/materialize.min.js`

 * *Files identical despite different names*

### Comparing `voila-material-tuwien-0.4.4/share/jupyter/nbconvert/templates/material-tuwien/static/voila_logo_bleu.svg` & `voila-material-tuwien-0.4.5/share/jupyter/nbconvert/templates/material-tuwien/static/voila_logo_bleu.svg`

 * *Files identical despite different names*

### Comparing `voila-material-tuwien-0.4.4/share/jupyter/voila/templates/material-tuwien/base.html` & `voila-material-tuwien-0.4.5/share/jupyter/voila/templates/material-tuwien/base.html`

 * *Files 6% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
       .sidenav {
         width: fit-content;
         transform: translateX(0%) !important;
       }
 
       .nav-wrapper {
-        background-color: #5cbcaf;
+        background-color: #006699;
       }
 
       .sidenav-link {
         white-space: nowrap;
         overflow: hidden;
         text-overflow: ellipsis;
       }
@@ -84,15 +84,15 @@
 
       @keyframes rotation {
         from {transform: rotate(0deg);}
         to   {transform: rotate(359deg);}
       }
 
       .voila-spinner-color1{
-        fill: #5cbcaf;
+        fill: #006699;
       }
 
       .voila-spinner-color2{
         fill: #f8e14b;
       }
     </style>
```

### Comparing `voila-material-tuwien-0.4.4/share/jupyter/voila/templates/material-tuwien/index.html.j2` & `voila-material-tuwien-0.4.5/share/jupyter/voila/templates/material-tuwien/index.html.j2`

 * *Files identical despite different names*

### Comparing `voila-material-tuwien-0.4.4/share/jupyter/voila/templates/material-tuwien/tree.html` & `voila-material-tuwien-0.4.5/share/jupyter/voila/templates/material-tuwien/tree.html`

 * *Files identical despite different names*

### Comparing `voila-material-tuwien-0.4.4/voila_material_tuwien.egg-info/SOURCES.txt` & `voila-material-tuwien-0.4.5/voila_material_tuwien.egg-info/SOURCES.txt`

 * *Files identical despite different names*

