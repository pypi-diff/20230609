# Comparing `tmp/flask-marshmallow-openapi-0.1.3.tar.gz` & `tmp/flask-marshmallow-openapi-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-marshmallow-openapi-0.1.3.tar", last modified: Fri Jun  9 04:03:04 2023, max compression
+gzip compressed data, was "flask-marshmallow-openapi-0.1.4.tar", last modified: Fri Jun  9 15:53:42 2023, max compression
```

## Comparing `flask-marshmallow-openapi-0.1.3.tar` & `flask-marshmallow-openapi-0.1.4.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-09 04:03:04.134266 flask-marshmallow-openapi-0.1.3/
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      135 2023-06-09 04:02:12.000000 flask-marshmallow-openapi-0.1.3/.bumpversion.cfg
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)      709 2023-06-08 12:25:25.000000 flask-marshmallow-openapi-0.1.3/.gitignore
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)        5 2023-06-08 05:27:08.000000 flask-marshmallow-openapi-0.1.3/.python-version
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     1065 2023-06-08 12:45:04.000000 flask-marshmallow-openapi-0.1.3/LICENSE
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)      819 2023-06-08 12:23:57.000000 flask-marshmallow-openapi-0.1.3/MANIFEST.in
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     4490 2023-06-09 04:03:04.134266 flask-marshmallow-openapi-0.1.3/PKG-INFO
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)     3648 2023-06-09 03:51:07.000000 flask-marshmallow-openapi-0.1.3/README.md
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     2699 2023-06-09 04:02:12.000000 flask-marshmallow-openapi-0.1.3/pyproject.toml
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)       38 2023-06-09 04:03:04.134266 flask-marshmallow-openapi-0.1.3/setup.cfg
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-09 04:03:04.122266 flask-marshmallow-openapi-0.1.3/src/
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-09 04:03:04.126266 flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      107 2023-06-09 04:02:12.000000 flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/__init__.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)    12468 2023-06-08 07:51:47.000000 flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/decorators.py
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)     2199 2023-06-08 08:33:32.000000 flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/helpers.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)    11663 2023-06-09 04:02:05.000000 flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/open_api.py
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-09 04:03:04.122266 flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static/
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-09 04:03:04.134266 flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static/swagger_ui/
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)      665 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static/swagger_ui/favicon-16x16.png
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)      628 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static/swagger_ui/favicon-32x32.png
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)      202 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static/swagger_ui/index.css
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)      734 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static/swagger_ui/index.html
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)     2715 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static/swagger_ui/oauth2-redirect.html
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)      539 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static/swagger_ui/swagger-initializer.js
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)  1045708 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-bundle.js
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)  1538481 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-bundle.js.map
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)   368781 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle-core.js
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)  1286259 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle-core.js.map
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)  1045498 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle.js
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)  1534168 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle.js.map
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)   322863 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-standalone-preset.js
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)   517830 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-standalone-preset.js.map
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)   145206 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.css
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)   251096 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.css.map
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)   256702 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.js
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)   305131 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.js.map
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     3852 2023-06-09 04:02:05.000000 flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static_collector.py
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-09 04:03:04.134266 flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/templates/
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)      648 2023-06-08 10:36:33.000000 flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/templates/changelog.html.jinja2
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)      852 2023-06-08 08:13:47.000000 flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/templates/re_doc.jinja2
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)     2435 2023-06-08 08:44:35.000000 flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/templates/swagger_ui.jinja2
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-09 04:03:04.126266 flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi.egg-info/
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     4490 2023-06-09 04:03:04.000000 flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi.egg-info/PKG-INFO
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     2056 2023-06-09 04:03:04.000000 flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi.egg-info/SOURCES.txt
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)        1 2023-06-09 04:03:04.000000 flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi.egg-info/dependency_links.txt
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)        1 2023-06-08 05:49:20.000000 flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi.egg-info/not-zip-safe
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      428 2023-06-09 04:03:04.000000 flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi.egg-info/requires.txt
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)       26 2023-06-09 04:03:04.000000 flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi.egg-info/top_level.txt
+drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-09 15:53:42.195192 flask-marshmallow-openapi-0.1.4/
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      135 2023-06-09 15:53:11.000000 flask-marshmallow-openapi-0.1.4/.bumpversion.cfg
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)      709 2023-06-08 12:25:25.000000 flask-marshmallow-openapi-0.1.4/.gitignore
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)        5 2023-06-08 05:27:08.000000 flask-marshmallow-openapi-0.1.4/.python-version
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     1065 2023-06-08 12:45:04.000000 flask-marshmallow-openapi-0.1.4/LICENSE
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)      819 2023-06-08 12:23:57.000000 flask-marshmallow-openapi-0.1.4/MANIFEST.in
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     4490 2023-06-09 15:53:42.195192 flask-marshmallow-openapi-0.1.4/PKG-INFO
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)     3648 2023-06-09 03:51:07.000000 flask-marshmallow-openapi-0.1.4/README.md
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     2699 2023-06-09 15:53:11.000000 flask-marshmallow-openapi-0.1.4/pyproject.toml
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)       38 2023-06-09 15:53:42.195192 flask-marshmallow-openapi-0.1.4/setup.cfg
+drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-09 15:53:42.171192 flask-marshmallow-openapi-0.1.4/src/
+drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-09 15:53:42.171192 flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      144 2023-06-09 15:53:11.000000 flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/__init__.py
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)    12768 2023-06-09 15:51:47.000000 flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/decorators.py
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)     2199 2023-06-08 08:33:32.000000 flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/helpers.py
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)    11663 2023-06-09 04:04:07.000000 flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/middleware.py
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      103 2023-06-09 15:43:49.000000 flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/securities.py
+drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-09 15:53:42.171192 flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static/
+drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-09 15:53:42.195192 flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static/swagger_ui/
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)      665 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static/swagger_ui/favicon-16x16.png
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)      628 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static/swagger_ui/favicon-32x32.png
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)      202 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static/swagger_ui/index.css
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)      734 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static/swagger_ui/index.html
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)     2715 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static/swagger_ui/oauth2-redirect.html
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)      539 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static/swagger_ui/swagger-initializer.js
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)  1045708 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-bundle.js
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)  1538481 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-bundle.js.map
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)   368781 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle-core.js
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)  1286259 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle-core.js.map
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)  1045498 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle.js
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)  1534168 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle.js.map
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)   322863 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-standalone-preset.js
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)   517830 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-standalone-preset.js.map
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)   145206 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.css
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)   251096 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.css.map
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)   256702 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.js
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)   305131 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.js.map
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     3852 2023-06-09 04:04:07.000000 flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static_collector.py
+drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-09 15:53:42.195192 flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/templates/
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)      648 2023-06-08 10:36:33.000000 flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/templates/changelog.html.jinja2
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)      852 2023-06-08 08:13:47.000000 flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/templates/re_doc.jinja2
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)     2435 2023-06-08 08:44:35.000000 flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/templates/swagger_ui.jinja2
+drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-09 15:53:42.171192 flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi.egg-info/
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     4490 2023-06-09 15:53:42.000000 flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi.egg-info/PKG-INFO
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     2102 2023-06-09 15:53:42.000000 flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)        1 2023-06-09 15:53:42.000000 flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)        1 2023-06-08 05:49:20.000000 flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi.egg-info/not-zip-safe
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      428 2023-06-09 15:53:42.000000 flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi.egg-info/requires.txt
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)       26 2023-06-09 15:53:42.000000 flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi.egg-info/top_level.txt
```

### Comparing `flask-marshmallow-openapi-0.1.3/.gitignore` & `flask-marshmallow-openapi-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.3/LICENSE` & `flask-marshmallow-openapi-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.3/MANIFEST.in` & `flask-marshmallow-openapi-0.1.4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.3/PKG-INFO` & `flask-marshmallow-openapi-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-marshmallow-openapi
-Version: 0.1.3
+Version: 0.1.4
 Summary: Flask + marshmallow + OpenAPI
 Author-email: Tomislav Adamic <tomislav.adamic@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/tadams42/flask-marshmallow-openapi
 Keywords: OpenAPI SwaggerUI ReDoc
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `flask-marshmallow-openapi-0.1.3/README.md` & `flask-marshmallow-openapi-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.3/pyproject.toml` & `flask-marshmallow-openapi-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65", "wheel"]
 
 
 [project]
 name = "flask-marshmallow-openapi"
-version = "0.1.3"
+version = "0.1.4"
 description = "Flask + marshmallow + OpenAPI"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX :: Linux",
```

### Comparing `flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/decorators.py` & `flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/decorators.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 import flask
 import marshmallow
 import werkzeug.routing
 import wrapt
 import yaml
 
 from .helpers import schema_name, schema_ref
+from .securities import Securities
 
 ATTRIBUTE_NAME = "_open_api"
 _ENCOUNTERED_OPERATION_IDS = set()
 
 
 def _generate_operation_id(method, many, response_schema):
     for_schema = (
@@ -50,14 +51,15 @@
 
 def get(
     response_schema,
     operation_id: Optional[str] = None,
     summary: str = "",
     many: bool = False,
     errors: Optional[dict] = None,
+    security: Securities = Securities.access_token,
     additional_content: Optional[dict] = None,
 ):
     """
     Decorator that will inject standard sets of our OpenAPI GET docs into decorated
     method.
     """
     if not operation_id:
@@ -68,17 +70,16 @@
     open_api_data["responses"]["200"] = {
         "content": {
             "application/json": {"schema": {"$ref": schema_ref(response_schema)}}
         },
         "description": "",
     }
 
-    # TODO: This should be part of input params
-    if operation_id == "refresh_token":
-        open_api_data["security"] = [{"refresh_token": []}]
+    if security != Securities.no_token:
+        open_api_data["security"] = [{f"{security.name}": []}]
 
     if additional_content:
         for k, v in additional_content.items():
             open_api_data["responses"]["200"]["content"][k] = v
 
     if many:
         del open_api_data["parameters"]
@@ -105,28 +106,31 @@
 def post(
     request_schema: Type[marshmallow.Schema],
     response_schema: Type[marshmallow.Schema] | None = None,
     operation_id: Optional[str] = None,
     summary: Optional[str] = None,
     errors: Optional[dict] = None,
     headers: Optional[List[dict]] = None,
+    security: Securities = Securities.access_token,
 ):
     """
     Decorator that will inject standard sets of our OpenAPI POST docs into decorated
     method.
     """
 
     if not response_schema:
         response_schema = request_schema
 
     if not operation_id:
         operation_id = _generate_operation_id("post", False, response_schema)
 
     open_api_data = _initial_docs(request_schema)
     open_api_data["operationId"] = operation_id
+    if security != Securities.no_token:
+        open_api_data["security"] = [{f"{security.name}": []}]
 
     # TODO: This convention of having "create" in schema name makes our code smelly,
     # come up with something more explicit
     if "deleted" in schema_name(response_schema).lower():
         open_api_data["responses"]["204"] = {"description": "Resource was deleted"}
 
     else:
@@ -168,28 +172,33 @@
             header["in"] = "header"
             open_api_data["parameters"].append(header)
 
     return functools.partial(_decorate, open_api_data={"post": open_api_data})
 
 
 def delete_(
-    resource_schema, operation_id: Optional[str] = None, errors: Optional[dict] = None
+    resource_schema,
+    operation_id: Optional[str] = None,
+    errors: Optional[dict] = None,
+    security: Securities = Securities.access_token,
 ):
     """
     Decorator that will inject standard sets of our OpenAPI DELETE docs into decorated
     method.
     """
 
     if not operation_id:
         operation_id = _generate_operation_id("delete", False, resource_schema)
 
     open_api_data = _initial_docs(resource_schema)
     open_api_data["operationId"] = operation_id
     open_api_data["responses"]["204"] = {"description": "Resource was deleted"}
     open_api_data["parameters"][0]["name"] = resource_schema.opts.url_id_field
+    if security != Securities.no_token:
+        open_api_data["security"] = [{f"{security.name}": []}]
 
     tags = getattr(resource_schema.opts, "tags", None) or getattr(
         resource_schema.opts, "tags", None
     )
     if tags:
         open_api_data["tags"] = tags
 
@@ -200,28 +209,31 @@
 
 def patch(
     request_schema: Type[marshmallow.Schema],
     response_schema: Optional[Type[marshmallow.Schema]] = None,
     operation_id: Optional[str] = None,
     errors: Optional[dict] = None,
     additional_content: Optional[dict] = None,
+    security: Securities = Securities.access_token,
 ):
     """
     Decorator that will inject standard sets of our OpenAPI PATCH docs into decorated
     method.
     """
 
     if not response_schema:
         response_schema = request_schema
 
     if not operation_id:
         operation_id = _generate_operation_id("patch", False, response_schema)
 
     open_api_data = _initial_docs(request_schema)
     open_api_data["operationId"] = operation_id
+    if security != Securities.no_token:
+        open_api_data["security"] = [{f"{security.name}": []}]
     open_api_data["responses"]["200"] = {
         "content": {
             "application/json": {"schema": {"$ref": schema_ref(response_schema)}}
         },
         "description": "",
     }
     open_api_data["requestBody"] = {
@@ -310,22 +322,14 @@
                 "in": "path",
                 "required": True,
                 "schema": {"type": id_field_type},
             }
         ],
     }
 
-    if schema_cls.__name__ not in {
-        "LoginRequestSchema",
-        "ResetPasswordSchema",
-        "NewPasswordSchema",
-        "ApiHealthCheckSchema",
-    }:
-        retv["security"] = [{"access_token": []}]
-
     return retv
 
 
 def _flask_path_to_open_api_path(path: str):
     return _PATH_CONVERTER.sub(r"{\2}", path)
```

### Comparing `flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/helpers.py` & `flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/helpers.py`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/open_api.py` & `flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/middleware.py`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static/swagger_ui/favicon-16x16.png` & `flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static/swagger_ui/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static/swagger_ui/favicon-32x32.png` & `flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static/swagger_ui/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static/swagger_ui/index.html` & `flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static/swagger_ui/index.html`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static/swagger_ui/oauth2-redirect.html` & `flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static/swagger_ui/oauth2-redirect.html`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static/swagger_ui/swagger-initializer.js` & `flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static/swagger_ui/swagger-initializer.js`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-bundle.js` & `flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-bundle.js`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-bundle.js.map` & `flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-bundle.js.map`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle-core.js` & `flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle-core.js`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle-core.js.map` & `flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle-core.js.map`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle.js` & `flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle.js`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle.js.map` & `flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle.js.map`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-standalone-preset.js` & `flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-standalone-preset.js`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-standalone-preset.js.map` & `flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-standalone-preset.js.map`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.css` & `flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.css`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.css.map` & `flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.css.map`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.js` & `flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.js`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.js.map` & `flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.js.map`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static_collector.py` & `flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/static_collector.py`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/templates/changelog.html.jinja2` & `flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/templates/changelog.html.jinja2`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/templates/re_doc.jinja2` & `flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/templates/re_doc.jinja2`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/templates/swagger_ui.jinja2` & `flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi/templates/swagger_ui.jinja2`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi.egg-info/PKG-INFO` & `flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-marshmallow-openapi
-Version: 0.1.3
+Version: 0.1.4
 Summary: Flask + marshmallow + OpenAPI
 Author-email: Tomislav Adamic <tomislav.adamic@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/tadams42/flask-marshmallow-openapi
 Keywords: OpenAPI SwaggerUI ReDoc
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi.egg-info/SOURCES.txt` & `flask-marshmallow-openapi-0.1.4/src/flask_marshmallow_openapi.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 src/flask_marshmallow_openapi/__init__.py
 src/flask_marshmallow_openapi/decorators.py
 src/flask_marshmallow_openapi/helpers.py
-src/flask_marshmallow_openapi/open_api.py
+src/flask_marshmallow_openapi/middleware.py
+src/flask_marshmallow_openapi/securities.py
 src/flask_marshmallow_openapi/static_collector.py
 src/flask_marshmallow_openapi.egg-info/PKG-INFO
 src/flask_marshmallow_openapi.egg-info/SOURCES.txt
 src/flask_marshmallow_openapi.egg-info/dependency_links.txt
 src/flask_marshmallow_openapi.egg-info/not-zip-safe
 src/flask_marshmallow_openapi.egg-info/requires.txt
 src/flask_marshmallow_openapi.egg-info/top_level.txt
```

