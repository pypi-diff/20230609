# Comparing `tmp/flask-marshmallow-openapi-0.1.4.tar.gz` & `tmp/flask-marshmallow-openapi-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-marshmallow-openapi-0.1.4.tar", last modified: Fri Jun  9 15:53:42 2023, max compression
+gzip compressed data, was "flask-marshmallow-openapi-0.1.5.tar", last modified: Fri Jun  9 19:50:45 2023, max compression
```

## Comparing `flask-marshmallow-openapi-0.1.4.tar` & `flask-marshmallow-openapi-0.1.5.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-09 15:53:42.195192 flask-marshmallow-openapi-0.1.4/
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      135 2023-06-09 15:53:11.000000 flask-marshmallow-openapi-0.1.4/.bumpversion.cfg
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)      709 2023-06-08 12:25:25.000000 flask-marshmallow-openapi-0.1.4/.gitignore
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)        5 2023-06-08 05:27:08.000000 flask-marshmallow-openapi-0.1.4/.python-version
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     1065 2023-06-08 12:45:04.000000 flask-marshmallow-openapi-0.1.4/LICENSE
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)      819 2023-06-08 12:23:57.000000 flask-marshmallow-openapi-0.1.4/MANIFEST.in
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     4490 2023-06-09 15:53:42.195192 flask-marshmallow-openapi-0.1.4/PKG-INFO
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)     3648 2023-06-09 03:51:07.000000 flask-marshmallow-openapi-0.1.4/README.md
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     2699 2023-06-09 15:53:11.000000 flask-marshmallow-openapi-0.1.4/pyproject.toml
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)       38 2023-06-09 15:53:42.195192 flask-marshmallow-openapi-0.1.4/setup.cfg
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-09 15:53:42.171192 flask-marshmallow-openapi-0.1.4/src/
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-09 15:53:42.171192 flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      144 2023-06-09 15:53:11.000000 flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/__init__.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)    12768 2023-06-09 15:51:47.000000 flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/decorators.py
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)     2199 2023-06-08 08:33:32.000000 flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/helpers.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)    11663 2023-06-09 04:04:07.000000 flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/middleware.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      103 2023-06-09 15:43:49.000000 flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/securities.py
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-09 15:53:42.171192 flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static/
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-09 15:53:42.195192 flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static/swagger_ui/
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)      665 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static/swagger_ui/favicon-16x16.png
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)      628 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static/swagger_ui/favicon-32x32.png
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)      202 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static/swagger_ui/index.css
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)      734 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static/swagger_ui/index.html
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)     2715 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static/swagger_ui/oauth2-redirect.html
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)      539 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static/swagger_ui/swagger-initializer.js
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)  1045708 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-bundle.js
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)  1538481 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-bundle.js.map
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)   368781 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle-core.js
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)  1286259 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle-core.js.map
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)  1045498 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle.js
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)  1534168 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle.js.map
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)   322863 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-standalone-preset.js
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)   517830 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-standalone-preset.js.map
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)   145206 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.css
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)   251096 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.css.map
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)   256702 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.js
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)   305131 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.js.map
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     3852 2023-06-09 04:04:07.000000 flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static_collector.py
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-09 15:53:42.195192 flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/templates/
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)      648 2023-06-08 10:36:33.000000 flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/templates/changelog.html.jinja2
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)      852 2023-06-08 08:13:47.000000 flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/templates/re_doc.jinja2
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)     2435 2023-06-08 08:44:35.000000 flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/templates/swagger_ui.jinja2
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-09 15:53:42.171192 flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi.egg-info/
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     4490 2023-06-09 15:53:42.000000 flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi.egg-info/PKG-INFO
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     2102 2023-06-09 15:53:42.000000 flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi.egg-info/SOURCES.txt
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)        1 2023-06-09 15:53:42.000000 flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi.egg-info/dependency_links.txt
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)        1 2023-06-08 05:49:20.000000 flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi.egg-info/not-zip-safe
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      428 2023-06-09 15:53:42.000000 flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi.egg-info/requires.txt
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)       26 2023-06-09 15:53:42.000000 flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi.egg-info/top_level.txt
+drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-09 19:50:45.272085 flask-marshmallow-openapi-0.1.5/
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      135 2023-06-09 19:50:13.000000 flask-marshmallow-openapi-0.1.5/.bumpversion.cfg
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)      709 2023-06-08 12:25:25.000000 flask-marshmallow-openapi-0.1.5/.gitignore
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)        5 2023-06-08 05:27:08.000000 flask-marshmallow-openapi-0.1.5/.python-version
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     1065 2023-06-08 12:45:04.000000 flask-marshmallow-openapi-0.1.5/LICENSE
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)      819 2023-06-08 12:23:57.000000 flask-marshmallow-openapi-0.1.5/MANIFEST.in
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     4490 2023-06-09 19:50:45.272085 flask-marshmallow-openapi-0.1.5/PKG-INFO
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)     3648 2023-06-09 03:51:07.000000 flask-marshmallow-openapi-0.1.5/README.md
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     2699 2023-06-09 19:50:13.000000 flask-marshmallow-openapi-0.1.5/pyproject.toml
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)       38 2023-06-09 19:50:45.272085 flask-marshmallow-openapi-0.1.5/setup.cfg
+drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-09 19:50:45.244085 flask-marshmallow-openapi-0.1.5/src/
+drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-09 19:50:45.244085 flask-marshmallow-openapi-0.1.5/src/flask_marshmallow_openapi/
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      176 2023-06-09 19:50:13.000000 flask-marshmallow-openapi-0.1.5/src/flask_marshmallow_openapi/__init__.py
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)    13379 2023-06-09 19:47:03.000000 flask-marshmallow-openapi-0.1.5/src/flask_marshmallow_openapi/decorators.py
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)     2199 2023-06-08 08:33:32.000000 flask-marshmallow-openapi-0.1.5/src/flask_marshmallow_openapi/helpers.py
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)    11663 2023-06-09 04:04:07.000000 flask-marshmallow-openapi-0.1.5/src/flask_marshmallow_openapi/middleware.py
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      641 2023-06-09 19:37:02.000000 flask-marshmallow-openapi-0.1.5/src/flask_marshmallow_openapi/models.py
+drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-09 19:50:45.244085 flask-marshmallow-openapi-0.1.5/src/flask_marshmallow_openapi/static/
+drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-09 19:50:45.272085 flask-marshmallow-openapi-0.1.5/src/flask_marshmallow_openapi/static/swagger_ui/
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)      665 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.5/src/flask_marshmallow_openapi/static/swagger_ui/favicon-16x16.png
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)      628 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.5/src/flask_marshmallow_openapi/static/swagger_ui/favicon-32x32.png
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)      202 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.5/src/flask_marshmallow_openapi/static/swagger_ui/index.css
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)      734 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.5/src/flask_marshmallow_openapi/static/swagger_ui/index.html
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)     2715 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.5/src/flask_marshmallow_openapi/static/swagger_ui/oauth2-redirect.html
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)      539 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.5/src/flask_marshmallow_openapi/static/swagger_ui/swagger-initializer.js
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)  1045708 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.5/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-bundle.js
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)  1538481 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.5/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-bundle.js.map
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)   368781 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.5/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle-core.js
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)  1286259 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.5/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle-core.js.map
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)  1045498 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.5/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle.js
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)  1534168 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.5/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle.js.map
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)   322863 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.5/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-standalone-preset.js
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)   517830 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.5/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-standalone-preset.js.map
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)   145206 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.5/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.css
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)   251096 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.5/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.css.map
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)   256702 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.5/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.js
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)   305131 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.5/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.js.map
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     3852 2023-06-09 04:04:07.000000 flask-marshmallow-openapi-0.1.5/src/flask_marshmallow_openapi/static_collector.py
+drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-09 19:50:45.272085 flask-marshmallow-openapi-0.1.5/src/flask_marshmallow_openapi/templates/
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)      648 2023-06-08 10:36:33.000000 flask-marshmallow-openapi-0.1.5/src/flask_marshmallow_openapi/templates/changelog.html.jinja2
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)      852 2023-06-08 08:13:47.000000 flask-marshmallow-openapi-0.1.5/src/flask_marshmallow_openapi/templates/re_doc.jinja2
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)     2435 2023-06-08 08:44:35.000000 flask-marshmallow-openapi-0.1.5/src/flask_marshmallow_openapi/templates/swagger_ui.jinja2
+drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-09 19:50:45.248085 flask-marshmallow-openapi-0.1.5/src/flask_marshmallow_openapi.egg-info/
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     4490 2023-06-09 19:50:45.000000 flask-marshmallow-openapi-0.1.5/src/flask_marshmallow_openapi.egg-info/PKG-INFO
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     2098 2023-06-09 19:50:45.000000 flask-marshmallow-openapi-0.1.5/src/flask_marshmallow_openapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)        1 2023-06-09 19:50:45.000000 flask-marshmallow-openapi-0.1.5/src/flask_marshmallow_openapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)        1 2023-06-08 05:49:20.000000 flask-marshmallow-openapi-0.1.5/src/flask_marshmallow_openapi.egg-info/not-zip-safe
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      428 2023-06-09 19:50:45.000000 flask-marshmallow-openapi-0.1.5/src/flask_marshmallow_openapi.egg-info/requires.txt
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)       26 2023-06-09 19:50:45.000000 flask-marshmallow-openapi-0.1.5/src/flask_marshmallow_openapi.egg-info/top_level.txt
```

### Comparing `flask-marshmallow-openapi-0.1.4/.gitignore` & `flask-marshmallow-openapi-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.4/LICENSE` & `flask-marshmallow-openapi-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.4/MANIFEST.in` & `flask-marshmallow-openapi-0.1.5/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.4/PKG-INFO` & `flask-marshmallow-openapi-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-marshmallow-openapi
-Version: 0.1.4
+Version: 0.1.5
 Summary: Flask + marshmallow + OpenAPI
 Author-email: Tomislav Adamic <tomislav.adamic@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/tadams42/flask-marshmallow-openapi
 Keywords: OpenAPI SwaggerUI ReDoc
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `flask-marshmallow-openapi-0.1.4/README.md` & `flask-marshmallow-openapi-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.4/pyproject.toml` & `flask-marshmallow-openapi-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65", "wheel"]
 
 
 [project]
 name = "flask-marshmallow-openapi"
-version = "0.1.4"
+version = "0.1.5"
 description = "Flask + marshmallow + OpenAPI"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX :: Linux",
```

### Comparing `flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/decorators.py` & `flask-marshmallow-openapi-0.1.5/src/flask_marshmallow_openapi/decorators.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,66 +6,70 @@
 import copy
 import functools
 import re
 import textwrap
 from typing import List, Optional, Type
 
 import flask
+import inflection
 import marshmallow
 import werkzeug.routing
 import wrapt
 import yaml
 
 from .helpers import schema_name, schema_ref
-from .securities import Securities
+from .models import ParameterObject, Securities
 
 ATTRIBUTE_NAME = "_open_api"
 _ENCOUNTERED_OPERATION_IDS = set()
 
 
 def _generate_operation_id(method, many, response_schema):
-    for_schema = (
+    for_schema = inflection.underscore(
         schema_name(response_schema)
         .replace("Schema", "")
         .replace("Update", "")
         .replace("Create", "")
     )
 
     if method == "get":
-        return ("list" if many else "detail") + for_schema
+        return for_schema + "_" + ("list" if many else "detail")
 
     if method == "post":
-        return "create" + for_schema
+        return for_schema + "_" + "create"
 
     if method == "patch":
-        return "update" + for_schema
+        return for_schema + "_" + "update"
 
     if method == "delete":
-        return "delete" + for_schema
+        return for_schema + "_" + "delete"
 
 
 def hide_doc():
     return functools.partial(
         _decorate, open_api_data={"post": {"operationId": "hidden"}}
     )
 
 
 def get(
     response_schema,
     operation_id: Optional[str] = None,
     summary: str = "",
     many: bool = False,
-    errors: Optional[dict] = None,
+    errors: dict | None = None,
     security: Securities = Securities.access_token,
-    additional_content: Optional[dict] = None,
+    additional_content: dict | None = None,
+    additional_parameters: list[ParameterObject] | None = None,
+    tags_override: list[str] | None = None,
 ):
     """
     Decorator that will inject standard sets of our OpenAPI GET docs into decorated
     method.
     """
+
     if not operation_id:
         operation_id = _generate_operation_id("get", many, response_schema)
 
     open_api_data = _initial_docs(response_schema)
     open_api_data["operationId"] = operation_id
     open_api_data["responses"]["200"] = {
         "content": {
@@ -87,15 +91,27 @@
         try:
             open_api_data["parameters"][0]["name"] = response_schema.opts.url_id_field
         except AttributeError:
             # It is perfectly fine to use GET on URLs that don't have ID field and
             # are described by schemas that don't have that field either.
             pass
 
-    tags = getattr(response_schema.opts, "tags", None)
+    if additional_parameters:
+        open_api_data["parameters"] = open_api_data.get("parameters", []) + [
+            _.to_dict for _ in additional_parameters
+        ]
+
+    if "parameters" in open_api_data:
+        open_api_data["parameters"] = [
+            _ for _ in open_api_data["parameters"] if (_["name"])
+        ]
+        if not open_api_data["parameters"]:
+            del open_api_data["parameters"]
+
+    tags = tags_override or getattr(response_schema.opts, "tags", None)
     if tags:
         open_api_data["tags"] = tags
 
     if summary:
         open_api_data["summary"] = summary
 
     _update_errors(open_api_data, errors)
```

### Comparing `flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/helpers.py` & `flask-marshmallow-openapi-0.1.5/src/flask_marshmallow_openapi/helpers.py`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/middleware.py` & `flask-marshmallow-openapi-0.1.5/src/flask_marshmallow_openapi/middleware.py`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static/swagger_ui/favicon-16x16.png` & `flask-marshmallow-openapi-0.1.5/src/flask_marshmallow_openapi/static/swagger_ui/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static/swagger_ui/favicon-32x32.png` & `flask-marshmallow-openapi-0.1.5/src/flask_marshmallow_openapi/static/swagger_ui/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static/swagger_ui/index.html` & `flask-marshmallow-openapi-0.1.5/src/flask_marshmallow_openapi/static/swagger_ui/index.html`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static/swagger_ui/oauth2-redirect.html` & `flask-marshmallow-openapi-0.1.5/src/flask_marshmallow_openapi/static/swagger_ui/oauth2-redirect.html`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static/swagger_ui/swagger-initializer.js` & `flask-marshmallow-openapi-0.1.5/src/flask_marshmallow_openapi/static/swagger_ui/swagger-initializer.js`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-bundle.js` & `flask-marshmallow-openapi-0.1.5/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-bundle.js`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-bundle.js.map` & `flask-marshmallow-openapi-0.1.5/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-bundle.js.map`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle-core.js` & `flask-marshmallow-openapi-0.1.5/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle-core.js`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle-core.js.map` & `flask-marshmallow-openapi-0.1.5/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle-core.js.map`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle.js` & `flask-marshmallow-openapi-0.1.5/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle.js`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle.js.map` & `flask-marshmallow-openapi-0.1.5/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle.js.map`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-standalone-preset.js` & `flask-marshmallow-openapi-0.1.5/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-standalone-preset.js`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-standalone-preset.js.map` & `flask-marshmallow-openapi-0.1.5/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-standalone-preset.js.map`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.css` & `flask-marshmallow-openapi-0.1.5/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.css`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.css.map` & `flask-marshmallow-openapi-0.1.5/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.css.map`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.js` & `flask-marshmallow-openapi-0.1.5/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.js`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.js.map` & `flask-marshmallow-openapi-0.1.5/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.js.map`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static_collector.py` & `flask-marshmallow-openapi-0.1.5/src/flask_marshmallow_openapi/static_collector.py`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/templates/changelog.html.jinja2` & `flask-marshmallow-openapi-0.1.5/src/flask_marshmallow_openapi/templates/changelog.html.jinja2`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/templates/re_doc.jinja2` & `flask-marshmallow-openapi-0.1.5/src/flask_marshmallow_openapi/templates/re_doc.jinja2`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/templates/swagger_ui.jinja2` & `flask-marshmallow-openapi-0.1.5/src/flask_marshmallow_openapi/templates/swagger_ui.jinja2`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi.egg-info/PKG-INFO` & `flask-marshmallow-openapi-0.1.5/src/flask_marshmallow_openapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-marshmallow-openapi
-Version: 0.1.4
+Version: 0.1.5
 Summary: Flask + marshmallow + OpenAPI
 Author-email: Tomislav Adamic <tomislav.adamic@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/tadams42/flask-marshmallow-openapi
 Keywords: OpenAPI SwaggerUI ReDoc
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi.egg-info/SOURCES.txt` & `flask-marshmallow-openapi-0.1.5/src/flask_marshmallow_openapi.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 MANIFEST.in
 README.md
 pyproject.toml
 src/flask_marshmallow_openapi/__init__.py
 src/flask_marshmallow_openapi/decorators.py
 src/flask_marshmallow_openapi/helpers.py
 src/flask_marshmallow_openapi/middleware.py
-src/flask_marshmallow_openapi/securities.py
+src/flask_marshmallow_openapi/models.py
 src/flask_marshmallow_openapi/static_collector.py
 src/flask_marshmallow_openapi.egg-info/PKG-INFO
 src/flask_marshmallow_openapi.egg-info/SOURCES.txt
 src/flask_marshmallow_openapi.egg-info/dependency_links.txt
 src/flask_marshmallow_openapi.egg-info/not-zip-safe
 src/flask_marshmallow_openapi.egg-info/requires.txt
 src/flask_marshmallow_openapi.egg-info/top_level.txt
```

