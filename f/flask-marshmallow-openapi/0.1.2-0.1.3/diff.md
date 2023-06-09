# Comparing `tmp/flask-marshmallow-openapi-0.1.2.tar.gz` & `tmp/flask-marshmallow-openapi-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-marshmallow-openapi-0.1.2.tar", last modified: Thu Jun  8 13:33:35 2023, max compression
+gzip compressed data, was "flask-marshmallow-openapi-0.1.3.tar", last modified: Fri Jun  9 04:03:04 2023, max compression
```

## Comparing `flask-marshmallow-openapi-0.1.2.tar` & `flask-marshmallow-openapi-0.1.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-08 13:33:35.804577 flask-marshmallow-openapi-0.1.2/
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      135 2023-06-08 13:32:49.000000 flask-marshmallow-openapi-0.1.2/.bumpversion.cfg
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)      709 2023-06-08 12:25:25.000000 flask-marshmallow-openapi-0.1.2/.gitignore
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)        5 2023-06-08 05:27:08.000000 flask-marshmallow-openapi-0.1.2/.python-version
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     1065 2023-06-08 12:45:04.000000 flask-marshmallow-openapi-0.1.2/LICENSE
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)      819 2023-06-08 12:23:57.000000 flask-marshmallow-openapi-0.1.2/MANIFEST.in
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     3531 2023-06-08 13:33:35.804577 flask-marshmallow-openapi-0.1.2/PKG-INFO
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)     2689 2023-06-08 13:12:32.000000 flask-marshmallow-openapi-0.1.2/README.md
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     2699 2023-06-08 13:33:17.000000 flask-marshmallow-openapi-0.1.2/pyproject.toml
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)       38 2023-06-08 13:33:35.804577 flask-marshmallow-openapi-0.1.2/setup.cfg
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-08 13:33:35.792577 flask-marshmallow-openapi-0.1.2/src/
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-08 13:33:35.796577 flask-marshmallow-openapi-0.1.2/src/flask_marshmallow_openapi/
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      107 2023-06-08 13:32:49.000000 flask-marshmallow-openapi-0.1.2/src/flask_marshmallow_openapi/__init__.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)    12468 2023-06-08 07:51:47.000000 flask-marshmallow-openapi-0.1.2/src/flask_marshmallow_openapi/decorators.py
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)     2199 2023-06-08 08:33:32.000000 flask-marshmallow-openapi-0.1.2/src/flask_marshmallow_openapi/helpers.py
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)    11663 2023-06-08 11:36:11.000000 flask-marshmallow-openapi-0.1.2/src/flask_marshmallow_openapi/open_api.py
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-08 13:33:35.792577 flask-marshmallow-openapi-0.1.2/src/flask_marshmallow_openapi/static/
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-08 13:33:35.804577 flask-marshmallow-openapi-0.1.2/src/flask_marshmallow_openapi/static/swagger_ui/
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)      665 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.2/src/flask_marshmallow_openapi/static/swagger_ui/favicon-16x16.png
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)      628 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.2/src/flask_marshmallow_openapi/static/swagger_ui/favicon-32x32.png
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)      202 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.2/src/flask_marshmallow_openapi/static/swagger_ui/index.css
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)      734 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.2/src/flask_marshmallow_openapi/static/swagger_ui/index.html
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)     2715 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.2/src/flask_marshmallow_openapi/static/swagger_ui/oauth2-redirect.html
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)      539 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.2/src/flask_marshmallow_openapi/static/swagger_ui/swagger-initializer.js
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)  1045708 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.2/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-bundle.js
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)  1538481 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.2/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-bundle.js.map
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)   368781 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.2/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle-core.js
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)  1286259 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.2/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle-core.js.map
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)  1045498 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.2/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle.js
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)  1534168 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.2/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle.js.map
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)   322863 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.2/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-standalone-preset.js
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)   517830 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.2/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-standalone-preset.js.map
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)   145206 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.2/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.css
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)   251096 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.2/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.css.map
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)   256702 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.2/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.js
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)   305131 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.2/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.js.map
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     3725 2023-06-08 13:32:08.000000 flask-marshmallow-openapi-0.1.2/src/flask_marshmallow_openapi/static_collector.py
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-08 13:33:35.804577 flask-marshmallow-openapi-0.1.2/src/flask_marshmallow_openapi/templates/
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)      648 2023-06-08 10:36:33.000000 flask-marshmallow-openapi-0.1.2/src/flask_marshmallow_openapi/templates/changelog.html.jinja2
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)      852 2023-06-08 08:13:47.000000 flask-marshmallow-openapi-0.1.2/src/flask_marshmallow_openapi/templates/re_doc.jinja2
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)     2435 2023-06-08 08:44:35.000000 flask-marshmallow-openapi-0.1.2/src/flask_marshmallow_openapi/templates/swagger_ui.jinja2
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-08 13:33:35.796577 flask-marshmallow-openapi-0.1.2/src/flask_marshmallow_openapi.egg-info/
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     3531 2023-06-08 13:33:35.000000 flask-marshmallow-openapi-0.1.2/src/flask_marshmallow_openapi.egg-info/PKG-INFO
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     2056 2023-06-08 13:33:35.000000 flask-marshmallow-openapi-0.1.2/src/flask_marshmallow_openapi.egg-info/SOURCES.txt
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)        1 2023-06-08 13:33:35.000000 flask-marshmallow-openapi-0.1.2/src/flask_marshmallow_openapi.egg-info/dependency_links.txt
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)        1 2023-06-08 05:49:20.000000 flask-marshmallow-openapi-0.1.2/src/flask_marshmallow_openapi.egg-info/not-zip-safe
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      428 2023-06-08 13:33:35.000000 flask-marshmallow-openapi-0.1.2/src/flask_marshmallow_openapi.egg-info/requires.txt
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)       26 2023-06-08 13:33:35.000000 flask-marshmallow-openapi-0.1.2/src/flask_marshmallow_openapi.egg-info/top_level.txt
+drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-09 04:03:04.134266 flask-marshmallow-openapi-0.1.3/
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      135 2023-06-09 04:02:12.000000 flask-marshmallow-openapi-0.1.3/.bumpversion.cfg
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)      709 2023-06-08 12:25:25.000000 flask-marshmallow-openapi-0.1.3/.gitignore
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)        5 2023-06-08 05:27:08.000000 flask-marshmallow-openapi-0.1.3/.python-version
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     1065 2023-06-08 12:45:04.000000 flask-marshmallow-openapi-0.1.3/LICENSE
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)      819 2023-06-08 12:23:57.000000 flask-marshmallow-openapi-0.1.3/MANIFEST.in
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     4490 2023-06-09 04:03:04.134266 flask-marshmallow-openapi-0.1.3/PKG-INFO
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)     3648 2023-06-09 03:51:07.000000 flask-marshmallow-openapi-0.1.3/README.md
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     2699 2023-06-09 04:02:12.000000 flask-marshmallow-openapi-0.1.3/pyproject.toml
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)       38 2023-06-09 04:03:04.134266 flask-marshmallow-openapi-0.1.3/setup.cfg
+drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-09 04:03:04.122266 flask-marshmallow-openapi-0.1.3/src/
+drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-09 04:03:04.126266 flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      107 2023-06-09 04:02:12.000000 flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/__init__.py
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)    12468 2023-06-08 07:51:47.000000 flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/decorators.py
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)     2199 2023-06-08 08:33:32.000000 flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/helpers.py
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)    11663 2023-06-09 04:02:05.000000 flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/open_api.py
+drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-09 04:03:04.122266 flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static/
+drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-09 04:03:04.134266 flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static/swagger_ui/
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)      665 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static/swagger_ui/favicon-16x16.png
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)      628 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static/swagger_ui/favicon-32x32.png
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)      202 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static/swagger_ui/index.css
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)      734 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static/swagger_ui/index.html
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)     2715 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static/swagger_ui/oauth2-redirect.html
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)      539 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static/swagger_ui/swagger-initializer.js
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)  1045708 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-bundle.js
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)  1538481 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-bundle.js.map
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)   368781 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle-core.js
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)  1286259 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle-core.js.map
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)  1045498 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle.js
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)  1534168 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle.js.map
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)   322863 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-standalone-preset.js
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)   517830 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-standalone-preset.js.map
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)   145206 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.css
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)   251096 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.css.map
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)   256702 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.js
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)   305131 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.js.map
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     3852 2023-06-09 04:02:05.000000 flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static_collector.py
+drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-09 04:03:04.134266 flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/templates/
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)      648 2023-06-08 10:36:33.000000 flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/templates/changelog.html.jinja2
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)      852 2023-06-08 08:13:47.000000 flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/templates/re_doc.jinja2
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)     2435 2023-06-08 08:44:35.000000 flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/templates/swagger_ui.jinja2
+drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-09 04:03:04.126266 flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi.egg-info/
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     4490 2023-06-09 04:03:04.000000 flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi.egg-info/PKG-INFO
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     2056 2023-06-09 04:03:04.000000 flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)        1 2023-06-09 04:03:04.000000 flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)        1 2023-06-08 05:49:20.000000 flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi.egg-info/not-zip-safe
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      428 2023-06-09 04:03:04.000000 flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi.egg-info/requires.txt
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)       26 2023-06-09 04:03:04.000000 flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi.egg-info/top_level.txt
```

### Comparing `flask-marshmallow-openapi-0.1.2/.gitignore` & `flask-marshmallow-openapi-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.2/LICENSE` & `flask-marshmallow-openapi-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.2/MANIFEST.in` & `flask-marshmallow-openapi-0.1.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.2/PKG-INFO` & `flask-marshmallow-openapi-0.1.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,19 @@
-Metadata-Version: 2.1
-Name: flask-marshmallow-openapi
-Version: 0.1.2
-Summary: Flask + marshmallow + OpenAPI
-Author-email: Tomislav Adamic <tomislav.adamic@gmail.com>
-License: MIT
-Project-URL: Source, https://github.com/tadams42/flask-marshmallow-openapi
-Keywords: OpenAPI SwaggerUI ReDoc
-Platform: any
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: docs
-Provides-Extra: tests
-License-File: LICENSE
-
 # Overview
 
 [![PyPI Status](https://badge.fury.io/py/flask-marshmallow-openapi.svg)](https://badge.fury.io/py/flask-marshmallow-openapi)
 [![license](https://img.shields.io/pypi/l/flask-marshmallow-openapi.svg)](https://opensource.org/licenses/MIT)
 [![python_versions](https://img.shields.io/pypi/pyversions/flask-marshmallow-openapi.svg)](https://pypi.org/project/flask-marshmallow-openapi/)
 
 
 Provides OpenAPI documentation generated from code for
 [Flask](https://flask.palletsprojects.com/en/latest/) APIs built around
 [marshmallow](https://marshmallow.readthedocs.io/en/stable/) schemas.
 
-This hackish and organically grown (TM) package was crated because no other similar
+This hackish and organically grown (TM) package was created because no other similar
 projects worked exactly the way I wanted them.
 
 You will probably be better served by some other, properly maintained project with
 similar purpose:
 
 - [flasgger](https://github.com/flasgger/flasgger)
 - [flask-openapi3](https://github.com/luolingchun/flask-openapi3)
@@ -116,7 +92,58 @@
     mounted_at="/v1",
 )
 
 
 docs = OpenAPI(config=conf)
 docs.init_app(app)
 ```
+
+## Serving docs via ngnix
+
+Add `collect-static` command to your app:
+
+```py
+import shutil
+
+import click
+import flask
+
+@app.cli.command("collect_static")
+@click.argument(
+    "destination_dir",
+    nargs=1,
+    type=click.Path(file_okay=False, dir_okay=True, writable=True, resolve_path=True),
+    required=True,
+)
+def collect_static_command(destination_dir):
+    shutil.copytree(
+        flask.current_app.static_folder, destination_dir, dirs_exist_ok=True
+    )
+    docs.collect_static(destination_dir)
+    click.echo(f"Static files collected into {destination_dir}.")
+```
+
+Configure `nginx`:
+
+```nginx
+server {
+    # ...
+
+    location ^~ /v1/static {
+        alias /home/user/static;
+        try_files $uri $uri.html =404;
+    }
+
+    location ^~ /v1/docs {
+        alias /home/user/static/docs;
+        try_files $uri $uri.html =404;
+    }
+
+    # ...
+}
+```
+
+Whenever deploying app, call:
+
+```sh
+flask --app foobar_api collect-static /home/user/static
+```
```

### Comparing `flask-marshmallow-openapi-0.1.2/pyproject.toml` & `flask-marshmallow-openapi-0.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65", "wheel"]
 
 
 [project]
 name = "flask-marshmallow-openapi"
-version = "0.1.2"
+version = "0.1.3"
 description = "Flask + marshmallow + OpenAPI"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX :: Linux",
```

### Comparing `flask-marshmallow-openapi-0.1.2/src/flask_marshmallow_openapi/decorators.py` & `flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/decorators.py`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.2/src/flask_marshmallow_openapi/helpers.py` & `flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/helpers.py`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.2/src/flask_marshmallow_openapi/open_api.py` & `flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/open_api.py`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.2/src/flask_marshmallow_openapi/static/swagger_ui/favicon-16x16.png` & `flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static/swagger_ui/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.2/src/flask_marshmallow_openapi/static/swagger_ui/favicon-32x32.png` & `flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static/swagger_ui/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.2/src/flask_marshmallow_openapi/static/swagger_ui/index.html` & `flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static/swagger_ui/index.html`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.2/src/flask_marshmallow_openapi/static/swagger_ui/oauth2-redirect.html` & `flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static/swagger_ui/oauth2-redirect.html`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.2/src/flask_marshmallow_openapi/static/swagger_ui/swagger-initializer.js` & `flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static/swagger_ui/swagger-initializer.js`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.2/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-bundle.js` & `flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-bundle.js`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.2/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-bundle.js.map` & `flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-bundle.js.map`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.2/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle-core.js` & `flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle-core.js`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.2/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle-core.js.map` & `flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle-core.js.map`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.2/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle.js` & `flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle.js`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.2/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle.js.map` & `flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle.js.map`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.2/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-standalone-preset.js` & `flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-standalone-preset.js`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.2/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-standalone-preset.js.map` & `flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-standalone-preset.js.map`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.2/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.css` & `flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.css`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.2/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.css.map` & `flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.css.map`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.2/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.js` & `flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.js`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.2/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.js.map` & `flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.js.map`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.2/src/flask_marshmallow_openapi/static_collector.py` & `flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/static_collector.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,17 @@
             "open_api.static", filename=swagger_json_filename
         )
 
         return new_swagger_json_path
 
     def _write_redoc_html(self, swagger_json_url):
         page = flask.render_template(
-            "re_doc.jinja2", swagger_json_path=swagger_json_url
+            "re_doc.jinja2",
+            swagger_json_path=swagger_json_url,
+            api_name=self.open_api.config.api_name,
         )
         with open(self.destination_dir / "re_doc.html", "w") as f:
             f.write(page)
 
     def _write_swagger_ui_html(self, swagger_json_url):
         page = flask.render_template(
             "swagger_ui.jinja2",
@@ -78,15 +80,17 @@
             f.write(page)
 
     def _write_changelog_html(self):
         with open(self.docs_static / "changelog.md", "w") as f:
             if self.open_api.config.changelog_md_loader:
                 f.write(self.open_api.config.changelog_md_loader())
 
-        page = flask.render_template("changelog.html.jinja2")
+        page = flask.render_template(
+            "changelog.html.jinja2", api_name=self.open_api.config.api_name
+        )
         with open(self.destination_dir / "changelog.html", "w") as f:
             f.write(page)
 
     def _copy_src_static_folder(self):
         # TODO: "../static/" should really be handled by importlib.resources but that
         # doesn't support extracting directories from package, only individual files.
         shutil.copytree(_SELF_PATH / "static", self.docs_static, dirs_exist_ok=True)
```

### Comparing `flask-marshmallow-openapi-0.1.2/src/flask_marshmallow_openapi/templates/changelog.html.jinja2` & `flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/templates/changelog.html.jinja2`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.2/src/flask_marshmallow_openapi/templates/re_doc.jinja2` & `flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/templates/re_doc.jinja2`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.2/src/flask_marshmallow_openapi/templates/swagger_ui.jinja2` & `flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi/templates/swagger_ui.jinja2`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.2/src/flask_marshmallow_openapi.egg-info/PKG-INFO` & `flask-marshmallow-openapi-0.1.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-marshmallow-openapi
-Version: 0.1.2
+Version: 0.1.3
 Summary: Flask + marshmallow + OpenAPI
 Author-email: Tomislav Adamic <tomislav.adamic@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/tadams42/flask-marshmallow-openapi
 Keywords: OpenAPI SwaggerUI ReDoc
 Platform: any
 Classifier: Development Status :: 4 - Beta
@@ -29,15 +29,15 @@
 [![python_versions](https://img.shields.io/pypi/pyversions/flask-marshmallow-openapi.svg)](https://pypi.org/project/flask-marshmallow-openapi/)
 
 
 Provides OpenAPI documentation generated from code for
 [Flask](https://flask.palletsprojects.com/en/latest/) APIs built around
 [marshmallow](https://marshmallow.readthedocs.io/en/stable/) schemas.
 
-This hackish and organically grown (TM) package was crated because no other similar
+This hackish and organically grown (TM) package was created because no other similar
 projects worked exactly the way I wanted them.
 
 You will probably be better served by some other, properly maintained project with
 similar purpose:
 
 - [flasgger](https://github.com/flasgger/flasgger)
 - [flask-openapi3](https://github.com/luolingchun/flask-openapi3)
@@ -116,7 +116,58 @@
     mounted_at="/v1",
 )
 
 
 docs = OpenAPI(config=conf)
 docs.init_app(app)
 ```
+
+## Serving docs via ngnix
+
+Add `collect-static` command to your app:
+
+```py
+import shutil
+
+import click
+import flask
+
+@app.cli.command("collect_static")
+@click.argument(
+    "destination_dir",
+    nargs=1,
+    type=click.Path(file_okay=False, dir_okay=True, writable=True, resolve_path=True),
+    required=True,
+)
+def collect_static_command(destination_dir):
+    shutil.copytree(
+        flask.current_app.static_folder, destination_dir, dirs_exist_ok=True
+    )
+    docs.collect_static(destination_dir)
+    click.echo(f"Static files collected into {destination_dir}.")
+```
+
+Configure `nginx`:
+
+```nginx
+server {
+    # ...
+
+    location ^~ /v1/static {
+        alias /home/user/static;
+        try_files $uri $uri.html =404;
+    }
+
+    location ^~ /v1/docs {
+        alias /home/user/static/docs;
+        try_files $uri $uri.html =404;
+    }
+
+    # ...
+}
+```
+
+Whenever deploying app, call:
+
+```sh
+flask --app foobar_api collect-static /home/user/static
+```
```

### Comparing `flask-marshmallow-openapi-0.1.2/src/flask_marshmallow_openapi.egg-info/SOURCES.txt` & `flask-marshmallow-openapi-0.1.3/src/flask_marshmallow_openapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

