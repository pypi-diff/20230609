# Comparing `tmp/amazon-codewhisperer-jupyterlab-ext-1.0.1.tar.gz` & `tmp/amazon-codewhisperer-jupyterlab-ext-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amazon-codewhisperer-jupyterlab-ext-1.0.1.tar", last modified: Wed May 10 05:04:51 2023, max compression
+gzip compressed data, was "amazon-codewhisperer-jupyterlab-ext-1.0.3.tar", last modified: Fri Jun  9 16:25:20 2023, max compression
```

## Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.1.tar` & `amazon-codewhisperer-jupyterlab-ext-1.0.3.tar`

### file list

```diff
@@ -1,141 +1,143 @@
-drwxr-xr-x   0 kuhikar  (177493822) ANT\Domain Users (1896053708)        0 2023-05-10 05:04:51.045215 amazon-codewhisperer-jupyterlab-ext-1.0.1/
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)    11357 2023-05-08 23:53:46.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/LICENSE
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)      503 2023-05-08 23:53:46.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/MANIFEST.in
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)      103 2023-05-08 23:53:46.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/NOTICE
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)     4865 2023-05-10 05:04:51.044679 amazon-codewhisperer-jupyterlab-ext-1.0.1/PKG-INFO
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)     3964 2023-05-10 02:05:21.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/README.md
-drwxr-xr-x   0 kuhikar  (177493822) ANT\Domain Users (1896053708)        0 2023-05-10 05:04:50.964475 amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext/
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)     1039 2023-05-08 23:53:46.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext/__init__.py
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)      443 2023-05-08 23:53:46.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext/_version.py
-drwxr-xr-x   0 kuhikar  (177493822) ANT\Domain Users (1896053708)        0 2023-05-10 05:04:50.972195 amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext/auth/
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)       98 2023-05-08 23:53:46.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext/auth/__init__.py
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)     3547 2023-05-08 23:53:46.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext/auth/sso_auth_manager.py
-drwxr-xr-x   0 kuhikar  (177493822) ANT\Domain Users (1896053708)        0 2023-05-10 05:04:50.973105 amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext/client/
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)        0 2023-05-08 23:53:46.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext/client/__init__.py
-drwxr-xr-x   0 kuhikar  (177493822) ANT\Domain Users (1896053708)        0 2023-05-10 05:04:50.976941 amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext/client/codewhisperer/
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)      281 2023-05-08 23:53:46.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext/client/codewhisperer/__init__.py
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)     1268 2023-05-08 23:53:46.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext/client/codewhisperer/client_manager.py
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)     1071 2023-05-08 23:53:46.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext/client/codewhisperer/iam_client_manager.py
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)     1395 2023-05-08 23:53:46.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext/client/codewhisperer/sso_client_manager.py
-drwxr-xr-x   0 kuhikar  (177493822) ANT\Domain Users (1896053708)        0 2023-05-10 05:04:50.931948 amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext/client/service_models/
-drwxr-xr-x   0 kuhikar  (177493822) ANT\Domain Users (1896053708)        0 2023-05-10 05:04:50.929807 amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext/client/service_models/bearer/
-drwxr-xr-x   0 kuhikar  (177493822) ANT\Domain Users (1896053708)        0 2023-05-10 05:04:50.977827 amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext/client/service_models/bearer/2022-11-11/
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)    15547 2023-05-08 23:53:46.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext/client/service_models/bearer/2022-11-11/service-2.json
-drwxr-xr-x   0 kuhikar  (177493822) ANT\Domain Users (1896053708)        0 2023-05-10 05:04:50.931342 amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext/client/service_models/sigv4/
-drwxr-xr-x   0 kuhikar  (177493822) ANT\Domain Users (1896053708)        0 2023-05-10 05:04:50.979288 amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext/client/service_models/sigv4/2022-06-15/
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)    24832 2023-05-08 23:53:46.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext/client/service_models/sigv4/2022-06-15/service-2.json
-drwxr-xr-x   0 kuhikar  (177493822) ANT\Domain Users (1896053708)        0 2023-05-10 05:04:50.932304 amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext/client/service_models/telemetry/
-drwxr-xr-x   0 kuhikar  (177493822) ANT\Domain Users (1896053708)        0 2023-05-10 05:04:50.981271 amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext/client/service_models/telemetry/2017-07-25/
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)     4536 2023-05-08 23:53:46.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext/client/service_models/telemetry/2017-07-25/service-2.json
-drwxr-xr-x   0 kuhikar  (177493822) ANT\Domain Users (1896053708)        0 2023-05-10 05:04:50.983585 amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext/client/telemetry/
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)       72 2023-05-08 23:53:46.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext/client/telemetry/__init__.py
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)     3443 2023-05-08 23:53:46.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext/client/telemetry/telemetry.py
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)     1732 2023-05-10 01:55:31.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext/constants.py
-drwxr-xr-x   0 kuhikar  (177493822) ANT\Domain Users (1896053708)        0 2023-05-10 05:04:50.985579 amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext/env/
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)       64 2023-05-08 23:53:46.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext/env/__init__.py
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)     1660 2023-05-08 23:53:46.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext/env/environment.py
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)     7057 2023-05-08 23:53:46.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext/handlers.py
-drwxr-xr-x   0 kuhikar  (177493822) ANT\Domain Users (1896053708)        0 2023-05-10 05:04:50.986475 amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext/labextension/
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)     5159 2023-05-10 05:04:47.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext/labextension/package.json
-drwxr-xr-x   0 kuhikar  (177493822) ANT\Domain Users (1896053708)        0 2023-05-10 05:04:50.935337 amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext/labextension/schemas/
-drwxr-xr-x   0 kuhikar  (177493822) ANT\Domain Users (1896053708)        0 2023-05-10 05:04:50.988715 amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext/labextension/schemas/amazon-codewhisperer-jupyterlab-ext/
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)     2661 2023-05-10 05:04:44.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext/labextension/schemas/amazon-codewhisperer-jupyterlab-ext/completer.json
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)     5017 2023-05-10 05:04:44.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext/labextension/schemas/amazon-codewhisperer-jupyterlab-ext/package.json.orig
-drwxr-xr-x   0 kuhikar  (177493822) ANT\Domain Users (1896053708)        0 2023-05-10 05:04:50.995252 amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext/labextension/static/
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)    79208 2023-05-10 05:04:47.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext/labextension/static/568.e71a5b77238395161eb2.js
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)      368 2023-05-10 05:04:47.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext/labextension/static/568.e71a5b77238395161eb2.js.LICENSE.txt
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)     6607 2023-05-10 05:04:47.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext/labextension/static/571.3582fd184eff1ff4b836.js
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)     5640 2023-05-10 05:04:47.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext/labextension/static/747.462ff5e5d49d87208721.js
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)     8370 2023-05-10 05:04:47.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext/labextension/static/remoteEntry.3451ec5921d04a9e8b07.js
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)      178 2023-05-10 05:04:44.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext/labextension/static/style.js
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)     5075 2023-05-10 05:04:47.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext/labextension/static/third-party-licenses.json
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)     2715 2023-05-10 01:55:10.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext/utils.py
-drwxr-xr-x   0 kuhikar  (177493822) ANT\Domain Users (1896053708)        0 2023-05-10 05:04:50.996575 amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext/validator/
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)       67 2023-05-08 23:53:46.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext/validator/__init__.py
-drwxr-xr-x   0 kuhikar  (177493822) ANT\Domain Users (1896053708)        0 2023-05-10 05:04:50.997319 amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext/validator/schemas/
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)     1286 2023-05-08 23:53:46.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext/validator/schemas/generate_recommendations.json
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)      782 2023-05-08 23:53:46.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext/validator/validator.py
-drwxr-xr-x   0 kuhikar  (177493822) ANT\Domain Users (1896053708)        0 2023-05-10 05:04:50.970376 amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext.egg-info/
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)     4865 2023-05-10 05:04:50.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext.egg-info/PKG-INFO
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)     4165 2023-05-10 05:04:50.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext.egg-info/SOURCES.txt
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)        1 2023-05-10 05:04:50.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext.egg-info/dependency_links.txt
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)        1 2023-05-08 23:58:43.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext.egg-info/not-zip-safe
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)       15 2023-05-10 05:04:50.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext.egg-info/requires.txt
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)       36 2023-05-10 05:04:50.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext.egg-info/top_level.txt
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)      231 2023-05-08 23:53:46.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/install.json
-drwxr-xr-x   0 kuhikar  (177493822) ANT\Domain Users (1896053708)        0 2023-05-10 05:04:50.998519 amazon-codewhisperer-jupyterlab-ext-1.0.1/jupyter-config/
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)      119 2023-05-08 23:53:46.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/jupyter-config/amazon_codewhisperer_jupyterlab_ext.json
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)     5017 2023-05-10 01:55:31.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/package.json
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)      675 2023-05-08 23:53:46.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/pyproject.toml
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)       38 2023-05-10 05:04:51.045386 amazon-codewhisperer-jupyterlab-ext-1.0.1/setup.cfg
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)     2716 2023-05-08 23:53:46.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/setup.py
-drwxr-xr-x   0 kuhikar  (177493822) ANT\Domain Users (1896053708)        0 2023-05-10 05:04:51.004730 amazon-codewhisperer-jupyterlab-ext-1.0.1/src/
-drwxr-xr-x   0 kuhikar  (177493822) ANT\Domain Users (1896053708)        0 2023-05-10 05:04:51.005646 amazon-codewhisperer-jupyterlab-ext-1.0.1/src/__tests__/
-drwxr-xr-x   0 kuhikar  (177493822) ANT\Domain Users (1896053708)        0 2023-05-10 05:04:51.006756 amazon-codewhisperer-jupyterlab-ext-1.0.1/src/__tests__/autotrigger/
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)     2034 2023-05-08 23:53:46.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/src/__tests__/autotrigger/autotrigger.spec.ts
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)      109 2023-05-08 23:53:46.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/src/__tests__/index.spec.ts
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)     2789 2023-05-08 23:53:46.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/src/application.ts
-drwxr-xr-x   0 kuhikar  (177493822) ANT\Domain Users (1896053708)        0 2023-05-10 05:04:51.007979 amazon-codewhisperer-jupyterlab-ext-1.0.1/src/auth/
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)     9504 2023-05-08 23:53:46.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/src/auth/authManager.tsx
-drwxr-xr-x   0 kuhikar  (177493822) ANT\Domain Users (1896053708)        0 2023-05-10 05:04:51.008562 amazon-codewhisperer-jupyterlab-ext-1.0.1/src/autotrigger/
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)     6990 2023-05-08 23:53:46.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/src/autotrigger/autotrigger.ts
-drwxr-xr-x   0 kuhikar  (177493822) ANT\Domain Users (1896053708)        0 2023-05-10 05:04:51.010097 amazon-codewhisperer-jupyterlab-ext-1.0.1/src/aws_vector_consolas_jupyter_lab3_extension/
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)       28 2023-05-08 23:53:46.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/src/aws_vector_consolas_jupyter_lab3_extension/__init__.py
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)       58 2023-05-08 23:53:46.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/src/aws_vector_consolas_jupyter_lab3_extension/py.typed
-drwxr-xr-x   0 kuhikar  (177493822) ANT\Domain Users (1896053708)        0 2023-05-10 05:04:51.013338 amazon-codewhisperer-jupyterlab-ext-1.0.1/src/client/
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)     1811 2023-05-08 23:53:46.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/src/client/apiclient.ts
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)    15283 2023-05-08 23:53:46.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/src/client/codewhispererclient.d.ts
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)     7900 2023-05-08 23:53:46.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/src/client/codewhispereruserclient.d.ts
-drwxr-xr-x   0 kuhikar  (177493822) ANT\Domain Users (1896053708)        0 2023-05-10 05:04:51.015390 amazon-codewhisperer-jupyterlab-ext-1.0.1/src/connector/
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)     2252 2023-05-08 23:53:46.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/src/connector/codewhispererconnector.ts
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)     2687 2023-05-08 23:53:46.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/src/connector/mergeconnector.ts
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)     1225 2023-05-08 23:53:46.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/src/handler.ts
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)     2444 2023-05-08 23:53:46.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/src/icons.ts
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)    12715 2023-05-08 23:53:46.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/src/index.ts
-drwxr-xr-x   0 kuhikar  (177493822) ANT\Domain Users (1896053708)        0 2023-05-10 05:04:51.016804 amazon-codewhisperer-jupyterlab-ext-1.0.1/src/inline/
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)    26396 2023-05-08 23:53:46.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/src/inline/inline.ts
-drwxr-xr-x   0 kuhikar  (177493822) ANT\Domain Users (1896053708)        0 2023-05-10 05:04:51.018518 amazon-codewhisperer-jupyterlab-ext-1.0.1/src/keybindings/
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)      937 2023-05-08 23:53:46.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/src/keybindings/keybindings.ts
-drwxr-xr-x   0 kuhikar  (177493822) ANT\Domain Users (1896053708)        0 2023-05-10 05:04:51.019151 amazon-codewhisperer-jupyterlab-ext-1.0.1/src/logging/
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)      487 2023-05-08 23:53:46.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/src/logging/logger.tsx
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)      127 2023-05-08 23:53:46.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/src/messages.ts
-drwxr-xr-x   0 kuhikar  (177493822) ANT\Domain Users (1896053708)        0 2023-05-10 05:04:51.020016 amazon-codewhisperer-jupyterlab-ext-1.0.1/src/notifications/
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)     3833 2023-05-10 05:02:57.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/src/notifications/notifications.tsx
-drwxr-xr-x   0 kuhikar  (177493822) ANT\Domain Users (1896053708)        0 2023-05-10 05:04:51.022359 amazon-codewhisperer-jupyterlab-ext-1.0.1/src/recommendation/
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)     4707 2023-05-08 23:53:46.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/src/recommendation/extractor.ts
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)    11167 2023-05-08 23:53:46.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/src/recommendation/recommendationStateHandler.ts
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)    10772 2023-05-08 23:53:46.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/src/recommendation/worker.ts
-drwxr-xr-x   0 kuhikar  (177493822) ANT\Domain Users (1896053708)        0 2023-05-10 05:04:51.022975 amazon-codewhisperer-jupyterlab-ext-1.0.1/src/referencetracker/
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)     3067 2023-05-08 23:53:46.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/src/referencetracker/referencetracker.tsx
-drwxr-xr-x   0 kuhikar  (177493822) ANT\Domain Users (1896053708)        0 2023-05-10 05:04:51.023717 amazon-codewhisperer-jupyterlab-ext-1.0.1/src/statusbar/
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)    14594 2023-05-09 01:02:05.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/src/statusbar/statusbarwidget.tsx
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)       78 2023-05-08 23:53:46.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/src/svg.d.ts
-drwxr-xr-x   0 kuhikar  (177493822) ANT\Domain Users (1896053708)        0 2023-05-10 05:04:51.027866 amazon-codewhisperer-jupyterlab-ext-1.0.1/src/telemetry/
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)     4333 2023-05-08 23:53:46.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/src/telemetry/clienttelemetry.d.ts
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)   150822 2023-05-08 23:53:46.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/src/telemetry/telemetry.gen.ts
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)     4292 2023-05-08 23:53:46.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/src/telemetry/telemetry.ts
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)      899 2023-05-08 23:53:46.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/src/telemetry/telemetryClient.ts
-drwxr-xr-x   0 kuhikar  (177493822) ANT\Domain Users (1896053708)        0 2023-05-10 05:04:51.032230 amazon-codewhisperer-jupyterlab-ext-1.0.1/src/utils/
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)     3234 2023-05-10 05:02:57.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/src/utils/constants.ts
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)      359 2023-05-08 23:53:46.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/src/utils/licenseUtils.ts
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)     1135 2023-05-08 23:53:46.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/src/utils/models.ts
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)      292 2023-05-08 23:53:46.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/src/utils/stateKeys.ts
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)     2974 2023-05-08 23:53:46.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/src/utils/utils.ts
-drwxr-xr-x   0 kuhikar  (177493822) ANT\Domain Users (1896053708)        0 2023-05-10 05:04:51.034880 amazon-codewhisperer-jupyterlab-ext-1.0.1/style/
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)     2123 2023-05-08 23:53:46.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/style/base.css
-drwxr-xr-x   0 kuhikar  (177493822) ANT\Domain Users (1896053708)        0 2023-05-10 05:04:51.043947 amazon-codewhisperer-jupyterlab-ext-1.0.1/style/img/
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)     3451 2023-05-08 23:53:46.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/style/img/codewhisperer.svg
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)      234 2023-05-08 23:53:46.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/style/img/connected.svg
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)      767 2023-05-08 23:53:46.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/style/img/disconnected.svg
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)      222 2023-05-08 23:53:46.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/style/img/documentation.svg
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)      234 2023-05-08 23:53:46.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/style/img/loading.svg
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)      746 2023-05-08 23:53:46.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/style/img/log.svg
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)      420 2023-05-08 23:53:46.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/style/img/pause.svg
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)      463 2023-05-08 23:53:46.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/style/img/resume.svg
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)      660 2023-05-08 23:53:46.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/style/img/signout.svg
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)      379 2023-05-08 23:53:46.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/style/img/start.svg
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)      599 2023-05-08 23:53:46.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/style/img/visual-cue-arrow.svg
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)       25 2023-05-08 23:53:46.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/style/index.css
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)       21 2023-05-08 23:53:46.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/style/index.js
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)      658 2023-05-08 23:53:46.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/tsconfig.json
--rw-r--r--   0 kuhikar  (177493822) ANT\Domain Users (1896053708)       33 2023-05-08 23:53:46.000000 amazon-codewhisperer-jupyterlab-ext-1.0.1/tsconfig.test.json
+drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.903294 amazon-codewhisperer-jupyterlab-ext-1.0.3/
+-rw-r--r--   0 zoelin     (505) staff       (20)    11357 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/LICENSE
+-rw-r--r--   0 zoelin     (505) staff       (20)      503 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/MANIFEST.in
+-rw-r--r--   0 zoelin     (505) staff       (20)      103 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/NOTICE
+-rw-r--r--   0 zoelin     (505) staff       (20)     5210 2023-06-09 16:25:20.902803 amazon-codewhisperer-jupyterlab-ext-1.0.3/PKG-INFO
+-rw-r--r--   0 zoelin     (505) staff       (20)     4309 2023-06-09 16:24:07.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/README.md
+drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.855773 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/
+-rw-r--r--   0 zoelin     (505) staff       (20)     1039 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/__init__.py
+-rw-r--r--   0 zoelin     (505) staff       (20)      443 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/_version.py
+drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.859841 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/auth/
+-rw-r--r--   0 zoelin     (505) staff       (20)       98 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/auth/__init__.py
+-rw-r--r--   0 zoelin     (505) staff       (20)     3422 2023-06-08 22:48:03.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/auth/sso_auth_manager.py
+drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.860757 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/client/
+-rw-r--r--   0 zoelin     (505) staff       (20)        0 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/client/__init__.py
+drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.862714 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/client/codewhisperer/
+-rw-r--r--   0 zoelin     (505) staff       (20)      281 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/client/codewhisperer/__init__.py
+-rw-r--r--   0 zoelin     (505) staff       (20)     1277 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/client/codewhisperer/client_manager.py
+-rw-r--r--   0 zoelin     (505) staff       (20)      794 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/client/codewhisperer/iam_client_manager.py
+-rw-r--r--   0 zoelin     (505) staff       (20)     1395 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/client/codewhisperer/sso_client_manager.py
+drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.839493 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/client/service_models/
+drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.838622 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/client/service_models/bearer/
+drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.863279 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/client/service_models/bearer/2022-11-11/
+-rw-r--r--   0 zoelin     (505) staff       (20)    15547 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/client/service_models/bearer/2022-11-11/service-2.json
+drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.839234 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/client/service_models/sigv4/
+drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.863946 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/client/service_models/sigv4/2022-06-15/
+-rw-r--r--   0 zoelin     (505) staff       (20)    24832 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/client/service_models/sigv4/2022-06-15/service-2.json
+drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.839638 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/client/service_models/telemetry/
+drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.864558 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/client/service_models/telemetry/2017-07-25/
+-rw-r--r--   0 zoelin     (505) staff       (20)     4536 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/client/service_models/telemetry/2017-07-25/service-2.json
+drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.865497 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/client/telemetry/
+-rw-r--r--   0 zoelin     (505) staff       (20)       72 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/client/telemetry/__init__.py
+-rw-r--r--   0 zoelin     (505) staff       (20)     3443 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/client/telemetry/telemetry.py
+-rw-r--r--   0 zoelin     (505) staff       (20)     1732 2023-06-09 16:24:07.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/constants.py
+drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.866791 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/env/
+-rw-r--r--   0 zoelin     (505) staff       (20)       64 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/env/__init__.py
+-rw-r--r--   0 zoelin     (505) staff       (20)     1660 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/env/environment.py
+-rw-r--r--   0 zoelin     (505) staff       (20)     7057 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/handlers.py
+drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.867414 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/labextension/
+-rw-r--r--   0 zoelin     (505) staff       (20)     5188 2023-06-09 16:25:18.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/labextension/package.json
+drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.841002 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/labextension/schemas/
+drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.868220 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/labextension/schemas/amazon-codewhisperer-jupyterlab-ext/
+-rw-r--r--   0 zoelin     (505) staff       (20)     2661 2023-06-09 16:25:16.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/labextension/schemas/amazon-codewhisperer-jupyterlab-ext/completer.json
+-rw-r--r--   0 zoelin     (505) staff       (20)     5046 2023-06-09 16:25:16.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/labextension/schemas/amazon-codewhisperer-jupyterlab-ext/package.json.orig
+drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.871505 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/labextension/static/
+-rw-r--r--   0 zoelin     (505) staff       (20)    79921 2023-06-09 16:25:18.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/labextension/static/568.c0e5b626da6cbe06eb5e.js
+-rw-r--r--   0 zoelin     (505) staff       (20)      368 2023-06-09 16:25:18.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/labextension/static/568.c0e5b626da6cbe06eb5e.js.LICENSE.txt
+-rw-r--r--   0 zoelin     (505) staff       (20)     6607 2023-06-09 16:25:18.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/labextension/static/571.3582fd184eff1ff4b836.js
+-rw-r--r--   0 zoelin     (505) staff       (20)     5640 2023-06-09 16:25:18.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/labextension/static/747.462ff5e5d49d87208721.js
+-rw-r--r--   0 zoelin     (505) staff       (20)     8370 2023-06-09 16:25:18.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/labextension/static/remoteEntry.9bf04351778104e8e5cd.js
+-rw-r--r--   0 zoelin     (505) staff       (20)      178 2023-06-09 16:25:16.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/labextension/static/style.js
+-rw-r--r--   0 zoelin     (505) staff       (20)     5075 2023-06-09 16:25:18.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/labextension/static/third-party-licenses.json
+-rw-r--r--   0 zoelin     (505) staff       (20)     2715 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/utils.py
+drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.872532 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/validator/
+-rw-r--r--   0 zoelin     (505) staff       (20)       67 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/validator/__init__.py
+drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.873091 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/validator/schemas/
+-rw-r--r--   0 zoelin     (505) staff       (20)     1286 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/validator/schemas/generate_recommendations.json
+-rw-r--r--   0 zoelin     (505) staff       (20)      782 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/validator/validator.py
+drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.858847 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext.egg-info/
+-rw-r--r--   0 zoelin     (505) staff       (20)     5210 2023-06-09 16:25:20.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext.egg-info/PKG-INFO
+-rw-r--r--   0 zoelin     (505) staff       (20)     4229 2023-06-09 16:25:20.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext.egg-info/SOURCES.txt
+-rw-r--r--   0 zoelin     (505) staff       (20)        1 2023-06-09 16:25:20.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext.egg-info/dependency_links.txt
+-rw-r--r--   0 zoelin     (505) staff       (20)        1 2023-06-06 01:34:05.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext.egg-info/not-zip-safe
+-rw-r--r--   0 zoelin     (505) staff       (20)       15 2023-06-09 16:25:20.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext.egg-info/requires.txt
+-rw-r--r--   0 zoelin     (505) staff       (20)       36 2023-06-09 16:25:20.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext.egg-info/top_level.txt
+-rw-r--r--   0 zoelin     (505) staff       (20)      231 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/install.json
+drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.873713 amazon-codewhisperer-jupyterlab-ext-1.0.3/jupyter-config/
+-rw-r--r--   0 zoelin     (505) staff       (20)      119 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/jupyter-config/amazon_codewhisperer_jupyterlab_ext.json
+-rw-r--r--   0 zoelin     (505) staff       (20)     5046 2023-06-09 16:24:07.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/package.json
+-rw-r--r--   0 zoelin     (505) staff       (20)      675 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/pyproject.toml
+-rw-r--r--   0 zoelin     (505) staff       (20)       38 2023-06-09 16:25:20.903421 amazon-codewhisperer-jupyterlab-ext-1.0.3/setup.cfg
+-rw-r--r--   0 zoelin     (505) staff       (20)     2716 2023-06-09 00:41:39.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/setup.py
+drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.877266 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/
+drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.877806 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/__tests__/
+drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.878348 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/__tests__/autotrigger/
+-rw-r--r--   0 zoelin     (505) staff       (20)     2034 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/__tests__/autotrigger/autotrigger.spec.ts
+-rw-r--r--   0 zoelin     (505) staff       (20)      109 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/__tests__/index.spec.ts
+drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.879316 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/__tests__/recommendation/
+-rw-r--r--   0 zoelin     (505) staff       (20)     5855 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/__tests__/recommendation/recommendationStateHandler.spec.ts
+-rw-r--r--   0 zoelin     (505) staff       (20)     2789 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/application.ts
+drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.880312 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/auth/
+-rw-r--r--   0 zoelin     (505) staff       (20)     9598 2023-06-08 22:48:03.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/auth/authManager.tsx
+drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.881092 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/autotrigger/
+-rw-r--r--   0 zoelin     (505) staff       (20)     6990 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/autotrigger/autotrigger.ts
+drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.882715 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/aws_vector_consolas_jupyter_lab3_extension/
+-rw-r--r--   0 zoelin     (505) staff       (20)       28 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/aws_vector_consolas_jupyter_lab3_extension/__init__.py
+-rw-r--r--   0 zoelin     (505) staff       (20)       58 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/aws_vector_consolas_jupyter_lab3_extension/py.typed
+drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.885084 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/client/
+-rw-r--r--   0 zoelin     (505) staff       (20)     1811 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/client/apiclient.ts
+-rw-r--r--   0 zoelin     (505) staff       (20)    15283 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/client/codewhispererclient.d.ts
+-rw-r--r--   0 zoelin     (505) staff       (20)     7900 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/client/codewhispereruserclient.d.ts
+drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.886554 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/connector/
+-rw-r--r--   0 zoelin     (505) staff       (20)     2252 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/connector/codewhispererconnector.ts
+-rw-r--r--   0 zoelin     (505) staff       (20)     2687 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/connector/mergeconnector.ts
+-rw-r--r--   0 zoelin     (505) staff       (20)     1225 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/handler.ts
+-rw-r--r--   0 zoelin     (505) staff       (20)     2444 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/icons.ts
+-rw-r--r--   0 zoelin     (505) staff       (20)    13178 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/index.ts
+drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.887189 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/inline/
+-rw-r--r--   0 zoelin     (505) staff       (20)    26396 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/inline/inline.ts
+drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.887826 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/keybindings/
+-rw-r--r--   0 zoelin     (505) staff       (20)      937 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/keybindings/keybindings.ts
+drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.888427 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/logging/
+-rw-r--r--   0 zoelin     (505) staff       (20)      524 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/logging/logger.tsx
+-rw-r--r--   0 zoelin     (505) staff       (20)      127 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/messages.ts
+drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.888975 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/notifications/
+-rw-r--r--   0 zoelin     (505) staff       (20)     3833 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/notifications/notifications.tsx
+drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.890334 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/recommendation/
+-rw-r--r--   0 zoelin     (505) staff       (20)     4707 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/recommendation/extractor.ts
+-rw-r--r--   0 zoelin     (505) staff       (20)    11143 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/recommendation/recommendationStateHandler.ts
+-rw-r--r--   0 zoelin     (505) staff       (20)    10773 2023-06-08 22:48:03.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/recommendation/worker.ts
+drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.890818 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/referencetracker/
+-rw-r--r--   0 zoelin     (505) staff       (20)     3067 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/referencetracker/referencetracker.tsx
+drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.891267 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/statusbar/
+-rw-r--r--   0 zoelin     (505) staff       (20)    14594 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/statusbar/statusbarwidget.tsx
+-rw-r--r--   0 zoelin     (505) staff       (20)       78 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/svg.d.ts
+drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.893516 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/telemetry/
+-rw-r--r--   0 zoelin     (505) staff       (20)     4333 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/telemetry/clienttelemetry.d.ts
+-rw-r--r--   0 zoelin     (505) staff       (20)   150822 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/telemetry/telemetry.gen.ts
+-rw-r--r--   0 zoelin     (505) staff       (20)     4292 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/telemetry/telemetry.ts
+-rw-r--r--   0 zoelin     (505) staff       (20)      899 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/telemetry/telemetryClient.ts
+drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.895973 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/utils/
+-rw-r--r--   0 zoelin     (505) staff       (20)     3508 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/utils/constants.ts
+-rw-r--r--   0 zoelin     (505) staff       (20)      359 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/utils/licenseUtils.ts
+-rw-r--r--   0 zoelin     (505) staff       (20)     1135 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/utils/models.ts
+-rw-r--r--   0 zoelin     (505) staff       (20)      292 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/utils/stateKeys.ts
+-rw-r--r--   0 zoelin     (505) staff       (20)     2974 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/utils/utils.ts
+drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.897701 amazon-codewhisperer-jupyterlab-ext-1.0.3/style/
+-rw-r--r--   0 zoelin     (505) staff       (20)     2123 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/style/base.css
+drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.902311 amazon-codewhisperer-jupyterlab-ext-1.0.3/style/img/
+-rw-r--r--   0 zoelin     (505) staff       (20)     3451 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/style/img/codewhisperer.svg
+-rw-r--r--   0 zoelin     (505) staff       (20)      234 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/style/img/connected.svg
+-rw-r--r--   0 zoelin     (505) staff       (20)      767 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/style/img/disconnected.svg
+-rw-r--r--   0 zoelin     (505) staff       (20)      222 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/style/img/documentation.svg
+-rw-r--r--   0 zoelin     (505) staff       (20)      234 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/style/img/loading.svg
+-rw-r--r--   0 zoelin     (505) staff       (20)      746 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/style/img/log.svg
+-rw-r--r--   0 zoelin     (505) staff       (20)      420 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/style/img/pause.svg
+-rw-r--r--   0 zoelin     (505) staff       (20)      463 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/style/img/resume.svg
+-rw-r--r--   0 zoelin     (505) staff       (20)      660 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/style/img/signout.svg
+-rw-r--r--   0 zoelin     (505) staff       (20)      379 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/style/img/start.svg
+-rw-r--r--   0 zoelin     (505) staff       (20)      599 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/style/img/visual-cue-arrow.svg
+-rw-r--r--   0 zoelin     (505) staff       (20)       25 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/style/index.css
+-rw-r--r--   0 zoelin     (505) staff       (20)       21 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/style/index.js
+-rw-r--r--   0 zoelin     (505) staff       (20)      658 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/tsconfig.json
+-rw-r--r--   0 zoelin     (505) staff       (20)       33 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/tsconfig.test.json
```

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.1/LICENSE` & `amazon-codewhisperer-jupyterlab-ext-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.1/PKG-INFO` & `amazon-codewhisperer-jupyterlab-ext-1.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon-codewhisperer-jupyterlab-ext
-Version: 1.0.1
+Version: 1.0.3
 Summary: Amazon CodeWhisperer for JupyterLab
 Home-page: https://aws.amazon.com/codewhisperer/
 Author: Amazon CodeWhisperer
 Author-email: codewhisperer@amazon.com
 License: Apache 2.0
 Keywords: Jupyter,JupyterLab,JupyterLab3,Amazon CodeWhisperer,CodeWhisperer,Code,Whisperer
 Platform: Linux
@@ -91,9 +91,18 @@
 
 ## More Resources
 
 * [CodeWhisperer User Guide](https://docs.aws.amazon.com/codewhisperer/latest/userguide/what-is-cwspr.html)
 * [Setting up Amazon CodeWhisperer with JupyterLab](https://docs.aws.amazon.com/codewhisperer/latest/userguide/jupyterlab-setup.html)
 * [Setting up CodeWhisperer with Amazon SageMaker Studio](https://docs.aws.amazon.com/codewhisperer/latest/userguide/sagemaker-setup.html)
 
+## Change Log
+
+1.0.3
+* Bug fix: No recommendation when user turn off code suggestions with references in settings.
+* Bug fix: Issue with browser login flow for some Builder ID users.
+* Bug fix: Fix an issue where SageMaker Studio users will incorrectly see the `Share content with Amazon CodeWhisperer` settings option.
+
+1.0.0
+* Initial release
```

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.1/README.md` & `amazon-codewhisperer-jupyterlab-ext-1.0.3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -66,7 +66,16 @@
 
 ## More Resources
 
 * [CodeWhisperer User Guide](https://docs.aws.amazon.com/codewhisperer/latest/userguide/what-is-cwspr.html)
 * [Setting up Amazon CodeWhisperer with JupyterLab](https://docs.aws.amazon.com/codewhisperer/latest/userguide/jupyterlab-setup.html)
 * [Setting up CodeWhisperer with Amazon SageMaker Studio](https://docs.aws.amazon.com/codewhisperer/latest/userguide/sagemaker-setup.html)
 
+## Change Log
+
+1.0.3
+* Bug fix: No recommendation when user turn off code suggestions with references in settings.
+* Bug fix: Issue with browser login flow for some Builder ID users.
+* Bug fix: Fix an issue where SageMaker Studio users will incorrectly see the `Share content with Amazon CodeWhisperer` settings option.
+
+1.0.0
+* Initial release
```

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext/__init__.py` & `amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext/auth/sso_auth_manager.py` & `amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/auth/sso_auth_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import webbrowser
 import boto3
 import tornado.gen
 from botocore.exceptions import ClientError
 from amazon_codewhisperer_jupyterlab_ext.constants import CLIENT_REGISTRATION_TYPE, CLIENT_NAME, SCOPES, \
     START_URL, DEVICE_GRANT_TYPE, REFRESH_GRANT_TYPE, SSO_OIDC, OIDC_BUILDER_ID_ENDPOINT, OIDC_BUILDER_ID_REGION
 from amazon_codewhisperer_jupyterlab_ext.utils import generate_succeeded_service_response, generate_client_error_oidc_service_response
 
@@ -49,19 +48,17 @@
             )
             return generate_succeeded_service_response(device_authorization_response)
         except ClientError as e:
             return generate_client_error_oidc_service_response(e)
 
     @tornado.gen.coroutine
     def create_token(self, client_registration, device_authorization):
-        url = device_authorization['verificationUriComplete']
         device_code = device_authorization['deviceCode']
         expires_in = device_authorization['expiresIn']
         interval = device_authorization['interval']
-        webbrowser.open(url, autoraise=True)
 
         for n in range(1, expires_in // interval + 1):
             if self.login_cancelled:
                 self.login_cancelled = False
                 return None
             yield tornado.gen.sleep(interval)
             try:
```

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext/client/codewhisperer/client_manager.py` & `amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/client/codewhisperer/client_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
             cls._instance = super().__new__(cls)
         return cls._instance
 
     def get_client(self):
         return self._client
 
     @abstractmethod
-    def invoke_recommendations(self, request):
+    def invoke_recommendations(self, request, opt_out):
         pass
 
     def generate_recommendations(self, recommendation_request, opt_out):
         try:
             recommendation_response = self.invoke_recommendations(recommendation_request, opt_out)
             return generate_succeeded_service_response(recommendation_response)
         except ClientError as e:
```

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext/client/codewhisperer/iam_client_manager.py` & `amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/client/codewhisperer/sso_client_manager.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,42 @@
 from abc import ABC
-import logging
+from botocore import UNSIGNED
+from botocore.client import Config
 from amazon_codewhisperer_jupyterlab_ext.client.codewhisperer.client_manager import CodeWhispererClientManager
 from amazon_codewhisperer_jupyterlab_ext.constants import (
     REQUEST_OPTOUT_HEADER_NAME,
     RTS_PROD_ENDPOINT,
     RTS_PROD_REGION,
-    SIGV4
+    BEARER
 )
 
-logging.basicConfig(format="%(levelname)s: %(message)s")
 
-
-class CodeWhispererIamClientManager(CodeWhispererClientManager, ABC):
+class CodeWhispererSsoClientManager(CodeWhispererClientManager, ABC):
+    _initialized = False
 
     def __init__(self):
+        if self._initialized:
+            return
+        self._initialized = True
+
         super().__init__()
+        self._bearer_token = ""
+        self._opt_out = False
         self._client = self.session.client(
-            service_name=SIGV4,
+            service_name=BEARER,
             endpoint_url=RTS_PROD_ENDPOINT,
             region_name=RTS_PROD_REGION,
-            verify=False,
+            config=Config(signature_version=UNSIGNED),
         )
-        self._opt_out = False
+
         self._client.meta.events.register_first("before-sign.*.*", self._add_header)
 
     def _add_header(self, request, **kwargs):
+        request.headers.add_header("Authorization", "Bearer " + self._bearer_token)
         request.headers.add_header(REQUEST_OPTOUT_HEADER_NAME, f"{self._opt_out}")
 
     def invoke_recommendations(self, request, opt_out):
         self._opt_out = opt_out
-        return self._client.generate_recommendations(**request)
+        return self.get_client().generate_completions(**request)
+
+    def set_bearer_token(self, token):
+        self._bearer_token = token
```

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext/client/service_models/bearer/2022-11-11/service-2.json` & `amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/client/service_models/bearer/2022-11-11/service-2.json`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext/client/service_models/sigv4/2022-06-15/service-2.json` & `amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/client/service_models/sigv4/2022-06-15/service-2.json`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext/client/service_models/telemetry/2017-07-25/service-2.json` & `amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/client/service_models/telemetry/2017-07-25/service-2.json`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext/client/telemetry/telemetry.py` & `amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/client/telemetry/telemetry.py`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext/constants.py` & `amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-CURRENT_VERSION = "1.0.1"
+CURRENT_VERSION = "1.0.3"
 # TODO : Update URL to CodeWhisperer PyPI JSON URL
 CODEWHISPERER_PYPI_JSON_URL = "https://pypi.org/pypi/amazon-codewhisperer-jupyterlab-ext/json"
 
 TELEMETRY_PROD_ENDPOINT = "https://client-telemetry.us-east-1.amazonaws.com"
 PROD_COGNITO_POOL_ID = "us-east-1:820fd6d1-95c0-4ca4-bffb-3f01d32da842"
 
 INVALID_TOKEN_EXCEPTION_MESSAGE = "The security token included in the request is expired"
```

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext/env/environment.py` & `amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/env/environment.py`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext/handlers.py` & `amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/handlers.py`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext/labextension/package.json` & `amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9748412698412698%*

 * *Differences: {"'devDependencies'": "{'pino-pretty': '10.0.0'}",*

 * * "'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.9bf04351778104e8e5cd.js'}}",*

 * * "'version'": "'1.0.3'"}*

```diff
@@ -54,14 +54,15 @@
         "eslint-plugin-jsdoc": "^40.0.0",
         "eslint-plugin-prettier": "^3.1.4",
         "eslint-plugin-react": "^7.18.3",
         "jest": "27.0.0",
         "jest-environment-jsdom": "^27.0.0",
         "jest-fetch-mock": "^1.6.6",
         "npm-run-all": "^4.1.5",
+        "pino-pretty": "10.0.0",
         "prettier": "^2.1.1",
         "rimraf": "^3.0.2",
         "ts-jest": "27.0.0",
         "typescript": "~4.3.0"
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
@@ -69,15 +70,15 @@
         "style/img/*.{svg}",
         "schema/*.json"
     ],
     "homepage": "https://github.com/aws",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.3451ec5921d04a9e8b07.js",
+            "load": "static/remoteEntry.9bf04351778104e8e5cd.js",
             "style": "./style"
         },
         "disabledExtensions": [
             "@jupyterlab/completer-extension:notebooks",
             "@jupyterlab/completer-extension:files"
         ],
         "extension": true,
@@ -134,9 +135,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "1.0.1"
+    "version": "1.0.3"
 }
```

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext/labextension/schemas/amazon-codewhisperer-jupyterlab-ext/completer.json` & `amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/labextension/schemas/amazon-codewhisperer-jupyterlab-ext/completer.json`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext/labextension/schemas/amazon-codewhisperer-jupyterlab-ext/package.json.orig` & `amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/labextension/schemas/amazon-codewhisperer-jupyterlab-ext/package.json.orig`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9752380952380952%*

 * *Differences: {"'devDependencies'": "{'pino-pretty': '10.0.0'}", "'version'": "'1.0.3'"}*

```diff
@@ -54,14 +54,15 @@
         "eslint-plugin-jsdoc": "^40.0.0",
         "eslint-plugin-prettier": "^3.1.4",
         "eslint-plugin-react": "^7.18.3",
         "jest": "27.0.0",
         "jest-environment-jsdom": "^27.0.0",
         "jest-fetch-mock": "^1.6.6",
         "npm-run-all": "^4.1.5",
+        "pino-pretty": "10.0.0",
         "prettier": "^2.1.1",
         "rimraf": "^3.0.2",
         "ts-jest": "27.0.0",
         "typescript": "~4.3.0"
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
@@ -129,9 +130,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "1.0.1"
+    "version": "1.0.3"
 }
```

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext/labextension/static/568.e71a5b77238395161eb2.js` & `amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/labextension/static/568.c0e5b626da6cbe06eb5e.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see 568.e71a5b77238395161eb2.js.LICENSE.txt */
+/*! For license information please see 568.c0e5b626da6cbe06eb5e.js.LICENSE.txt */
 "use strict";
 (self.webpackChunkamazon_codewhisperer_jupyterlab_ext = self.webpackChunkamazon_codewhisperer_jupyterlab_ext || []).push([
     [568], {
         4442: (e, t, n) => {
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.Application = void 0;
@@ -11,46 +11,46 @@
                 s = n(4872),
                 r = n(1708),
                 a = n(3311),
                 c = n(2531),
                 l = n(9513),
                 d = n(7790),
                 u = n(9513),
-                h = n(1174);
-            class g {
+                g = n(1174);
+            class h {
                 constructor() {
                     this._environment = void 0, this.loadStateSignal = new i.Signal(this)
                 }
                 static getInstance() {
-                    return g.instance || (g.instance = new g), g.instance
+                    return h.instance || (h.instance = new h), h.instance
                 }
                 async _fetchEnvironment() {
                     const e = await a.requestAPI("get_environment");
                     if (e.status !== l.HttpStatusCode.OK) return;
                     const t = await e.json();
                     this._environment = c.getResponseData(t).environment;
                     const n = c.getResponseData(t).version_notification,
                         i = c.getResponseData(t).latest_version;
-                    n && d.NotificationManager.getInstance().postNotificationForUpdateInformation(n, i, h.message("codewhisperer_update_now"), u.UPDATE_NOTIFICATION_URL).then()
+                    n && d.NotificationManager.getInstance().postNotificationForUpdateInformation(n, i, g.message("codewhisperer_update_now"), u.UPDATE_NOTIFICATION_URL).then()
                 }
                 isJupyterOSS() {
-                    return this._environment === m.JUPYTER_OSS
+                    return this._environment === p.JUPYTER_OSS
                 }
                 isSageMakerStudio() {
-                    return this._environment === m.SM_STUDIO
+                    return this._environment === p.SM_STUDIO
                 }
                 async loadServices(e, t) {
                     this.stateDB = e, this.jupyterApp = t, await this._fetchEnvironment(), s.Worker.getInstance(), o.AutoTrigger.getInstance(), r.AuthManager.getInstance()
                 }
             }
-            var m;
-            t.Application = g,
+            var p;
+            t.Application = h,
                 function(e) {
                     e.JUPYTER_OSS = "Jupyter OSS", e.SM_STUDIO = "SageMaker Studio"
-                }(m || (m = {}))
+                }(p || (p = {}))
         },
         1708: function(e, t, n) {
             var i = this && this.__importDefault || function(e) {
                 return e && e.__esModule ? e : {
                     default: e
                 }
             };
@@ -61,32 +61,32 @@
                 s = n(2531),
                 r = n(6168),
                 a = n(5185),
                 c = n(1174),
                 l = n(5185),
                 d = i(n(6271)),
                 u = n(2194),
-                h = n(7790),
-                g = n(4442),
-                m = n(9513),
-                p = n(9513);
+                g = n(7790),
+                h = n(4442),
+                p = n(9513),
+                m = n(9513);
             class _ {
                 constructor() {
                     this._authState = C.UNAUTHENTICATED, this._refreshIntervalInMs = 3e6, this.authStateChangedSignal = new r.Signal(this), this.authStateChangedSignal.connect(this._onAuthStateChanged, this), this._refreshToken = async () => {
                         this.isAuthenticated() && await this.refresh()
                     }
                 }
                 static getInstance() {
                     return _.instance || (_.instance = new _), _.instance
                 }
                 _onAuthStateChanged(e, t) {
                     this.authState = t, t !== C.UNAUTHENTICATED && t !== C.AUTHENTICATION_IN_PROGRESS && setTimeout(this._refreshToken, this._refreshIntervalInMs)
                 }
                 isAuthenticated() {
-                    return this.authState === C.AUTHENTICATED || g.Application.getInstance().isSageMakerStudio()
+                    return this.authState === C.AUTHENTICATED || h.Application.getInstance().isSageMakerStudio()
                 }
                 isAuthenticationInProgress() {
                     return this.authState === C.AUTHENTICATION_IN_PROGRESS
                 }
                 get authState() {
                     return this._authState
                 }
@@ -94,46 +94,46 @@
                     this._authState = e
                 }
                 async login() {
                     let e = await s.loadState(u.CLIENT_REGISTRATION);
                     if (void 0 === e) {
                         const t = await o.requestAPI("register_client"),
                             n = await t.json();
-                        if (!s.isResponseSuccess(n)) return void await h.NotificationManager.getInstance().postNotificationForApiExceptions(s.getErrorResponseUserMessage(n), c.message("codewhisperer_learn_more"), p.LEARN_MORE_NOTIFICATION_URL);
+                        if (!s.isResponseSuccess(n)) return void await g.NotificationManager.getInstance().postNotificationForApiExceptions(s.getErrorResponseUserMessage(n), c.message("codewhisperer_learn_more"), m.LEARN_MORE_NOTIFICATION_URL);
                         e = s.getResponseData(n), s.saveState(u.CLIENT_REGISTRATION, e).then()
                     }
                     const t = await o.requestAPI("device_authorization", {
                             body: JSON.stringify(e),
                             method: "POST"
                         }),
                         n = await t.json();
-                    if (!s.isResponseSuccess(n)) return void await h.NotificationManager.getInstance().postNotificationForApiExceptions(s.getErrorResponseUserMessage(n), c.message("codewhisperer_learn_more"), p.LEARN_MORE_NOTIFICATION_URL);
+                    if (!s.isResponseSuccess(n)) return void await g.NotificationManager.getInstance().postNotificationForApiExceptions(s.getErrorResponseUserMessage(n), c.message("codewhisperer_learn_more"), m.LEARN_MORE_NOTIFICATION_URL);
                     const i = s.getResponseData(n);
                     if (!(await l.showDialog({
                             title: c.message("codewhisperer_copy_code_and_proceed_dialog_title"),
                             body: d.default.createElement("p", null, d.default.createElement("br", null), d.default.createElement("li", null, c.message("codewhisperer_copy_code_and_proceed_dialog_message_first_li"), d.default.createElement("a", {
                                 href: "https://docs.aws.amazon.com/codewhisperer/latest/userguide/what-is-cwspr.html",
                                 className: "cwspr-learn-more-link"
                             }, c.message("codewhisperer_copy_code_and_proceed_dialog_message_first_li_learn_more"))), d.default.createElement("br", null), d.default.createElement("li", null, c.message("codewhisperer_copy_code_and_proceed_dialog_message_second_li")), d.default.createElement("br", null), d.default.createElement("li", null, c.message("codewhisperer_copy_code_and_proceed_dialog_message_third_li"), i.userCode), d.default.createElement("br", null)),
                             buttons: [l.Dialog.cancelButton(), l.Dialog.okButton({
                                 label: c.message("codewhisperer_copy_code_and_proceed_dialog_button_yes")
                             })]
                         })).button.accept) return;
-                    this.authStateChangedSignal.emit(C.AUTHENTICATION_IN_PROGRESS);
+                    window.open(i.verificationUriComplete, "_blank"), this.authStateChangedSignal.emit(C.AUTHENTICATION_IN_PROGRESS);
                     const r = {
                         clientRegistration: e,
                         deviceAuthorizationResponse: i
                     };
                     o.requestAPI("create_token", {
                         body: JSON.stringify(r),
                         method: "POST"
                     }).then((async e => {
                         const t = await e.json();
                         if (!t) return;
-                        if (!s.isResponseSuccess(t)) return await h.NotificationManager.getInstance().postNotificationForApiExceptions(s.getErrorResponseUserMessage(t), c.message("codewhisperer_learn_more"), p.LEARN_MORE_NOTIFICATION_URL), void this.authStateChangedSignal.emit(C.UNAUTHENTICATED);
+                        if (!s.isResponseSuccess(t)) return await g.NotificationManager.getInstance().postNotificationForApiExceptions(s.getErrorResponseUserMessage(t), c.message("codewhisperer_learn_more"), m.LEARN_MORE_NOTIFICATION_URL), void this.authStateChangedSignal.emit(C.UNAUTHENTICATED);
                         const n = s.getResponseData(t);
                         await s.saveState(u.SSO_TOKEN, n), this.authStateChangedSignal.emit(C.AUTHENTICATED)
                     }))
                 }
                 cancelLogin() {
                     o.requestAPI("cancel_login").then(), this.authStateChangedSignal.emit(C.UNAUTHENTICATED)
                 }
@@ -146,15 +146,15 @@
                             clientRegistration: t,
                             token: e
                         },
                         i = await o.requestAPI("refresh", {
                             body: JSON.stringify(n),
                             method: "POST"
                         });
-                    if (i.status === m.HttpStatusCode.NOT_FOUND) return;
+                    if (i.status === p.HttpStatusCode.NOT_FOUND) return;
                     const r = await i.json();
                     if (!s.isResponseSuccess(r)) {
                         const e = a.Notification.emit(c.message("codewhisperer_expiry_notification_message"), "default", {
                             autoClose: 1e4,
                             actions: [{
                                 label: c.message("codewhisperer_expiry_notification_button_authenticate"),
                                 callback: async () => {
@@ -386,22 +386,22 @@
                 s = i(n(3994)),
                 r = i(n(1563)),
                 a = i(n(8177)),
                 c = i(n(9107)),
                 l = i(n(6445)),
                 d = i(n(4268)),
                 u = i(n(6389)),
-                h = i(n(9206)),
-                g = i(n(2431)),
-                m = i(n(6140)),
-                p = i(n(1590));
+                g = i(n(9206)),
+                h = i(n(2431)),
+                p = i(n(6140)),
+                m = i(n(1590));
             class _ {}
             t.Icons = _, _.visualCueArrowIcon = new o.LabIcon({
                 name: "visual-cue-arrow",
-                svgstr: h.default
+                svgstr: g.default
             }), _.logoIcon = new o.LabIcon({
                 name: "codewhisperer:logo",
                 svgstr: s.default
             }), _.documentationIcon = new o.LabIcon({
                 name: "codewhisperer:documentation",
                 svgstr: r.default
             }), _.referenceLogIcon = new o.LabIcon({
@@ -417,21 +417,21 @@
                 name: "codewhisperer:signOut",
                 svgstr: d.default
             }), _.startIcon = new o.LabIcon({
                 name: "codewhisperer:start",
                 svgstr: u.default
             }), _.connectedIcon = new o.LabIcon({
                 name: "codewhisperer:connected",
-                svgstr: g.default
+                svgstr: h.default
             }), _.disconnectedIcon = new o.LabIcon({
                 name: "codewhisperer:disconnected",
-                svgstr: m.default
+                svgstr: p.default
             }), _.loadingIcon = new o.LabIcon({
                 name: "codewhisperer:loading",
-                svgstr: p.default
+                svgstr: m.default
             })
         },
         1568: function(e, t, n) {
             var i = this && this.__importDefault || function(e) {
                 return e && e.__esModule ? e : {
                     default: e
                 }
@@ -443,45 +443,47 @@
                 s = n(2766),
                 r = n(7681),
                 a = n(7363),
                 c = n(370),
                 l = n(4872),
                 d = n(6817),
                 u = n(6186),
-                h = n(8826),
-                g = n(7037),
-                m = n(4657),
-                p = n(1797),
+                g = n(8826),
+                h = n(7037),
+                p = n(4657),
+                m = n(1797),
                 _ = n(9805),
                 C = i(n(5313)),
                 v = n(5231),
                 I = n(1708),
                 w = n(6947),
                 f = n(4442),
                 y = n(6143),
                 S = n(3770),
                 T = n(9513),
                 b = n(5064),
                 E = {
                     id: T.PLUGIN_ID,
                     autoStart: !0,
-                    requires: [a.ISettingRegistry, o.ICompletionManager, s.INotebookTracker, r.IEditorTracker, d.IStateDB, h.IStatusBar, y.IRenderMimeRegistry],
-                    activate: async (e, t, n, i, r, a, d, h) => {
+                    requires: [a.ISettingRegistry, o.ICompletionManager, s.INotebookTracker, r.IEditorTracker, d.IStateDB, g.IStatusBar, y.IRenderMimeRegistry],
+                    activate: async (e, t, n, i, r, a, d, g) => {
                         const y = w.Logger.getInstance({
                                 name: "codewhisperer"
                             }),
                             E = performance.now();
                         e.restored.then((async () => {
                             a.fetch(T.PLUGIN_ID).then((e => {
-                                e ? (_.Telemetry.clientId = e.clientId, y.debug(`Restored - clientId: ${_.Telemetry.clientId}`)) : (_.Telemetry.clientId = p.UUID.uuid4(), a.save(T.PLUGIN_ID, {
+                                e ? (_.Telemetry.clientId = e.clientId, y.debug(`Restored - clientId: ${_.Telemetry.clientId}`)) : (_.Telemetry.clientId = m.UUID.uuid4(), a.save(T.PLUGIN_ID, {
                                     clientId: _.Telemetry.clientId
                                 }), y.debug(`Generated - clientId: ${_.Telemetry.clientId}`))
                             }));
                             const n = t => {
-                                _.Telemetry.getInstance().enableTelemetry(t.get("codeWhispererTelemetry").composite), l.Worker.getInstance().setOptOut(!t.get("shareCodeWhispererContentWithAWS").composite), l.Worker.getInstance().setSuggestionsWithCodeReferences(t.get("suggestionsWithCodeReferences").composite), w.Logger.setLogLevel(t.get("codeWhispererLogLevel").composite), b.Keybindings.getInstance().keyBindings = [...e.commands.keyBindings], y.debug("Loaded settings")
+                                if (_.Telemetry.getInstance().enableTelemetry(t.get(T.SettingIDs.keyTelemetry).composite), l.Worker.getInstance().setOptOut(!t.get(T.SettingIDs.keyOptOut).composite), l.Worker.getInstance().setSuggestionsWithCodeReferences(t.get(T.SettingIDs.keyReferences).composite), w.Logger.setLogLevel(t.get(T.SettingIDs.keyLogLevel).composite), b.Keybindings.getInstance().keyBindings = [...e.commands.keyBindings], y.debug("Loaded settings"), f.Application.getInstance().isJupyterOSS()) return;
+                                const n = document.createElement("style");
+                                n.textContent = "\n#jp-SettingsEditor-amazon-codewhisperer-jupyterlab-ext\\:completer > div:first-of-type {\n  display: none !important;\n}\n\n#jp-SettingsEditor-amazon-codewhisperer-jupyterlab-ext\\:completer > div:first-of-type > input {\n  pointer-events: none;\n  opacity: 0.5;\n}\n        ", document.head.appendChild(n)
                             };
                             Promise.all([e.restored, t.load(T.PLUGIN_ID)]).then((([, e]) => {
                                 n(e), e.changed.connect(n)
                             })), f.Application.getInstance().loadStateSignal.emit(null), await I.AuthManager.getInstance().refresh();
                             const i = new C.default;
                             d.registerStatusItem("aws-codewhisperer:status-bar-widget", {
                                 item: i,
@@ -494,55 +496,55 @@
                             y.debug(`Notebookpanel added - ${i.id}`);
                             let l = null !== (a = null === (r = i.content.activeCell) || void 0 === r ? void 0 : r.editor) && void 0 !== a ? a : null;
                             const d = {
                                     session: i.sessionContext.session,
                                     editor: l
                                 },
                                 u = new c.MergeConnector,
-                                h = n.register({
+                                g = n.register({
                                     connector: u,
                                     editor: l,
                                     parent: i
                                 }),
-                                p = () => {
+                                m = () => {
                                     var t, n;
-                                    y.debug(`Notebookpanel updated - ${i.id}`), l = null !== (n = null === (t = i.content.activeCell) || void 0 === t ? void 0 : t.editor) && void 0 !== n ? n : null, d.session = i.sessionContext.session, d.editor = l, h.editor = l;
+                                    y.debug(`Notebookpanel updated - ${i.id}`), l = null !== (n = null === (t = i.content.activeCell) || void 0 === t ? void 0 : t.editor) && void 0 !== n ? n : null, d.session = i.sessionContext.session, d.editor = l, g.editor = l;
                                     const r = new o.KernelConnector(d),
                                         a = new o.ContextConnector(d),
                                         u = new v.CodeWhispererConnector({
                                             notebookPanel: i
                                         });
-                                    h.connector = new c.MergeConnector(u, r, a), m.AutoTrigger.getInstance().registerListener(l, i);
-                                    const g = e.shell.currentWidget;
-                                    g && g instanceof s.NotebookPanel && performance.now() - E > T.NEW_CELL_AUTO_TRIGGER_DELAY_IN_MS && m.AutoTrigger.getInstance().onSwitchToNewCell(l, i)
+                                    g.connector = new c.MergeConnector(u, r, a), p.AutoTrigger.getInstance().registerListener(l, i);
+                                    const h = e.shell.currentWidget;
+                                    h && h instanceof s.NotebookPanel && performance.now() - E > T.NEW_CELL_AUTO_TRIGGER_DELAY_IN_MS && p.AutoTrigger.getInstance().onSwitchToNewCell(l, i)
                                 };
-                            i.content.activeCellChanged.connect((() => p())), i.sessionContext.sessionChanged.connect((() => p()));
+                            i.content.activeCellChanged.connect((() => m())), i.sessionContext.sessionChanged.connect((() => m()));
                             const _ = () => {
-                                y.debug(`Notebookpanel focus out - ${i.id}`), g.Inline.getInstance().onFocusOut()
+                                y.debug(`Notebookpanel focus out - ${i.id}`), h.Inline.getInstance().onFocusOut()
                             };
                             i.node.removeEventListener("focusout", _), i.node.addEventListener("focusout", _)
                         })), r.widgetAdded.connect(((e, t) => {
                             y.debug(`Editor added - ${t.id}`), t.content.editor.host.addEventListener("focusin", (() => {
                                 const e = t.context.path.split("/").pop();
-                                m.AutoTrigger.getInstance().registerListener(t.content.editor, void 0, e)
+                                p.AutoTrigger.getInstance().registerListener(t.content.editor, void 0, e)
                             }))
                         })), e.commands.hasCommand(T.CommandIDs.invokeNotebook) || e.commands.addCommand(T.CommandIDs.invokeNotebook, {
                             execute: () => {
                                 var t;
-                                if (y.debug("Executing command : invokeNotebook"), g.Inline.getInstance().isInlineSessionActive()) return void g.Inline.getInstance().acceptCompletion();
-                                l.Worker.getInstance().isGetCompletionsRunning && g.Inline.getInstance().removeCompletion();
+                                if (y.debug("Executing command : invokeNotebook"), h.Inline.getInstance().isInlineSessionActive()) return void h.Inline.getInstance().acceptCompletion();
+                                l.Worker.getInstance().isGetCompletionsRunning && h.Inline.getInstance().removeCompletion();
                                 const n = i.currentWidget;
                                 return n && "code" === (null === (t = n.content.activeCell) || void 0 === t ? void 0 : t.model.type) ? e.commands.execute(T.CommandIDs.invoke, {
                                     id: n.id
                                 }) : void 0
                             }
                         }), e.commands.addCommand(T.CommandIDs.invokeFile, {
                             execute: () => {
-                                if (y.debug("Executing command : invokeFile"), g.Inline.getInstance().isInlineSessionActive()) return void g.Inline.getInstance().acceptCompletion();
-                                l.Worker.getInstance().isGetCompletionsRunning && g.Inline.getInstance().removeCompletion();
+                                if (y.debug("Executing command : invokeFile"), h.Inline.getInstance().isInlineSessionActive()) return void h.Inline.getInstance().acceptCompletion();
+                                l.Worker.getInstance().isGetCompletionsRunning && h.Inline.getInstance().removeCompletion();
                                 const t = r.currentWidget && r.currentWidget.id;
                                 return t ? e.commands.execute(T.CommandIDs.invoke, {
                                     id: t
                                 }) : void 0
                             }
                         }), e.commands.hasCommand(T.CommandIDs.selectNotebook) || (y.debug("Executing command : selectNotebook"), e.commands.addCommand(T.CommandIDs.selectNotebook, {
                             execute: () => {
@@ -555,51 +557,51 @@
                             execute: async () => {
                                 await I.AuthManager.getInstance().login()
                             }
                         })), e.commands.hasCommand(T.CommandIDs.invokeInline) || e.commands.addCommand(T.CommandIDs.invokeInline, {
                             execute: async () => {
                                 y.debug("Executing command : invokeInline");
                                 const t = e.shell.currentWidget;
-                                if (t && t instanceof s.NotebookPanel) y.debug("Invoking Inline in NotebookPanel"), await g.Inline.getInstance().getCompletionsInNotebookPanel(t, {
+                                if (t && t instanceof s.NotebookPanel) y.debug("Invoking Inline in NotebookPanel"), await h.Inline.getInstance().getCompletionsInNotebookPanel(t, {
                                     triggerType: "OnDemand",
                                     triggerCharacter: void 0,
                                     automatedTriggerType: void 0,
                                     language: "ipynb",
                                     triggerTime: performance.now()
                                 });
                                 else if (t && t instanceof u.DocumentWidget) {
                                     y.debug("Invoking Inline in Document");
                                     const e = t,
                                         n = e.context.path.split("/").pop();
-                                    await g.Inline.getInstance().getCompletionsInEditor(e.content.editor, n, {
+                                    await h.Inline.getInstance().getCompletionsInEditor(e.content.editor, n, {
                                         triggerType: "OnDemand",
                                         triggerCharacter: void 0,
                                         automatedTriggerType: void 0,
                                         language: "python",
                                         triggerTime: performance.now()
                                     })
                                 } else y.error("Notebook or Editor not found")
                             }
                         }), e.commands.hasCommand(T.CommandIDs.rejectInline) || (y.debug("Executing command : rejectInline"), e.commands.addCommand(T.CommandIDs.rejectInline, {
                             execute: async () => {
-                                g.Inline.getInstance().removeCompletion()
+                                h.Inline.getInstance().removeCompletion()
                             }
                         })), e.commands.hasCommand(T.CommandIDs.acceptInline) || (y.debug("Executing command : acceptInline"), e.commands.addCommand(T.CommandIDs.acceptInline, {
                             execute: async () => {
-                                g.Inline.getInstance().acceptCompletion()
+                                h.Inline.getInstance().acceptCompletion()
                             }
                         })), e.commands.hasCommand(T.CommandIDs.showNext) || (y.debug("Executing command : showNext"), e.commands.addCommand(T.CommandIDs.showNext, {
                             execute: async () => {
-                                g.Inline.getInstance().showNext()
+                                h.Inline.getInstance().showNext()
                             }
                         })), e.commands.hasCommand(T.CommandIDs.showPrev) || (y.debug("Executing command : showNext"), e.commands.addCommand(T.CommandIDs.showPrev, {
                             execute: async () => {
-                                g.Inline.getInstance().showPrev()
+                                h.Inline.getInstance().showPrev()
                             }
-                        })), S.ReferenceTracker.createInstance(h), _.Telemetry.init(), y.info("JupyterLab CodeWhisperer extension is activated!")
+                        })), S.ReferenceTracker.createInstance(g), _.Telemetry.init(), y.info("JupyterLab CodeWhisperer extension is activated!")
                     }
                 };
             t.default = E
         },
         7037: (e, t, n) => {
             Object.defineProperty(t, "__esModule", {
                 value: !0
@@ -609,20 +611,20 @@
                 s = n(9513),
                 r = n(4657),
                 a = n(8353),
                 c = n(1708),
                 l = n(3770),
                 d = n(6551),
                 u = "jp-mod-inlinecompleter-active";
-            class h {
+            class g {
                 constructor() {
                     this.completions = [], this.currentIndex = 0, this.typeahead = "", this.cursorObserver = void 0, this.invokeFileName = "", this.visualCueLeftMargin = 0
                 }
                 static getInstance() {
-                    return h.instance || (h.instance = new h), h.instance
+                    return g.instance || (g.instance = new g), g.instance
                 }
                 getVisualCueHtmlElement() {
                     const e = document.createElement("span"),
                         t = this.completions[this.currentIndex].references;
                     e.textContent = ` Suggestion ${this.currentIndex+1} of ${this.completions.length} from CodeWhisperer${this.getReferenceLogMessage(t)}`, e.style.opacity = "0.60", e.style.fontSize = this.invokeEditor.getOption("fontSize") - 1 + "px", e.style.whiteSpace = "pre", e.style.color = "var(--jp-content-font-color1)";
                     const n = o.Icons.visualCueArrowIcon.element(),
                         i = Math.max(this.invokeEditor.lineHeight - 4, 4);
@@ -887,15 +889,15 @@
                     }
                     this.removeCompletion()
                 }
                 onEditorChange(e) {
                     this.removeCompletion()
                 }
             }
-            t.Inline = h
+            t.Inline = g
         },
         5064: (e, t) => {
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.Keybindings = void 0;
             class n {
                 constructor() {}
@@ -919,15 +921,17 @@
                 value: !0
             }), t.Logger = void 0;
             const o = i(n(5862));
             class s {
                 static getInstance(e) {
                     return s.parentLogger || (s.parentLogger = o.default({
                         level: "error",
-                        prettyPrint: !0
+                        transport: {
+                            target: "pino-pretty"
+                        }
                     })), this.parentLogger.child(e)
                 }
                 static setLogLevel(e) {
                     s.parentLogger.level = e.toLowerCase()
                 }
             }
             t.Logger = s, t.default = s
@@ -1038,40 +1042,40 @@
                 const n = e.content,
                     i = n.activeCell,
                     a = null === (t = n.activeCell) || void 0 === t ? void 0 : t.editor,
                     c = n.model.cells.length,
                     l = i.model.type,
                     d = null == a ? void 0 : a.getCursorPosition().line,
                     u = null == a ? void 0 : a.getOffsetAt(a.getCursorPosition());
-                let h;
+                let g;
                 if (a && i) {
                     const t = n.model.cells;
                     let i = "",
                         c = "";
                     for (let e = 0; e < t.length; e++) {
                         const o = t.get(e);
                         if (e < n.activeCellIndex) i += r(o);
                         else if (e === n.activeCellIndex) {
                             const e = a.getCursorPosition(),
                                 t = a.getOffsetAt(e),
                                 n = a.model.value.text;
                             i += n.substring(0, t), c += n.substring(t, n.length)
                         } else c += r(o)
                     }
-                    s.debug(`Notebook content length - left:${i.slice.length} right:${i.slice.length}`), h = {
+                    s.debug(`Notebook content length - left:${i.slice.length} right:${i.slice.length}`), g = {
                         leftFileContent: i.slice(-o.MAX_LENGTH),
                         rightFileContent: c.slice(0, o.MAX_LENGTH),
                         filename: e.context.path.split("/").pop(),
                         programmingLanguage: {
                             languageName: "python"
                         }
                     }
                 }
                 return {
-                    fileContext: h,
+                    fileContext: g,
                     fileContextMetadata: {
                         activeCellIdx: n.activeCellIndex,
                         cellCount: c,
                         cellType: l,
                         lineNumber: d,
                         cursorOffset: u
                     }
@@ -1117,15 +1121,15 @@
                 value: !0
             }), t.RecommendationStateHandler = void 0;
             const a = n(9805),
                 c = n(9513),
                 l = n(7126),
                 d = n(6168),
                 u = n(6947);
-            class h {
+            class g {
                 constructor() {
                     this.acceptedIndex = -1, this.timeSinceLastUserDecision = void 0, this.timeSinceLastDocumentChange = void 0, this.recommendations = [], this.recommendationSuggestionState = new Map, this.acceptRecommendationSignal = new d.Signal(this), this.acceptRecommendationSignal.connect(this.userDecisionSignalListener, this), this.rejectRecommendationSignal = new d.Signal(this), this.rejectRecommendationSignal.connect(this.userDecisionSignalListener, this), this.logger = u.Logger.getInstance({
                         name: "codewhisperer",
                         component: "recommendationStateHandler"
                     })
                 }
                 reset() {
@@ -1146,19 +1150,19 @@
                 }
                 addRecommendation(e) {
                     this.recommendations.push(e)
                 }
                 updateRecommendationState(e) {
                     const t = this.recommendations.length;
                     e.length > 0 ? e.forEach(((e, n) => {
-                        h.instance.setSuggestionState(t + n, "Discard"), h.instance.addRecommendation(e)
-                    })) : (h.instance.addRecommendation({
+                        g.instance.setSuggestionState(t + n, "Discard"), g.instance.addRecommendation(e)
+                    })) : (g.instance.addRecommendation({
                         content: "",
                         references: []
-                    }), h.instance.setSuggestionState(t, "Empty"))
+                    }), g.instance.setSuggestionState(t, "Empty"))
                 }
                 userDecisionSignalListener(e, t) {
                     this.acceptedIndex = t, this.recordUserDecisionTelemetry()
                 }
                 recordUserDecisionTelemetry() {
                     if (!this.invocationMetadata) return void this.reset();
                     const e = [];
@@ -1221,15 +1225,15 @@
                         if ("Accept" === n.codewhispererSuggestionState) return "Accept";
                         if ("Reject" === n.codewhispererSuggestionState) return "Reject";
                         "Empty" !== n.codewhispererSuggestionState && (t = !1)
                     }
                     return t ? "Empty" : "Discard"
                 }
             }
-            t.RecommendationStateHandler = h, i = h, o = {
+            t.RecommendationStateHandler = g, i = g, o = {
                 value: void 0
             }
         },
         4872: (e, t, n) => {
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.Worker = void 0;
@@ -1238,95 +1242,95 @@
                 s = n(9513),
                 r = n(1174),
                 a = n(6168),
                 c = n(6947),
                 l = n(7790),
                 d = n(2531),
                 u = n(8353);
-            class h {
+            class g {
                 constructor() {
                     this._isGetCompletionsRunning = !1, this.isInvocationCancelled = !1, this.optOut = !1, this.client = new i.ApiClient, this.receivedResponseSignal = new a.Signal(this), this.serviceInvocationSignal = new a.Signal(this), this.invocationStatusChangedSignal = new a.Signal(this), this.logger = c.Logger.getInstance({
                         name: "codewhisperer",
                         component: "worker"
                     })
                 }
                 static getInstance() {
-                    return h.instance || (h.instance = new h), h.instance
+                    return g.instance || (g.instance = new g), g.instance
                 }
                 get isGetCompletionsRunning() {
                     return this._isGetCompletionsRunning
                 }
                 set isGetCompletionsRunning(e) {
                     this._isGetCompletionsRunning = e, this.invocationStatusChangedSignal.emit(e)
                 }
                 async getCompletionsPaginated(e, t, n) {
-                    let i, o, a, c, h = "",
-                        g = "",
-                        m = "",
-                        p = 0,
+                    let i, o, a, c, g = "",
+                        h = "",
+                        p = "",
+                        m = 0,
                         _ = 0,
                         C = !0;
                     if (!this._isGetCompletionsRunning) {
-                        for (u.RecommendationStateHandler.instance.rejectRecommendationSignal.emit(-1), this.isInvocationCancelled = !1; !this.isInvocationCancelled && p < s.MAX_PAGINATION_CALLS;) {
+                        for (u.RecommendationStateHandler.instance.rejectRecommendationSignal.emit(-1), this.isInvocationCancelled = !1; !this.isInvocationCancelled && m < s.MAX_PAGINATION_CALLS;) {
                             this.isGetCompletionsRunning = !0;
                             try {
                                 o = Date.now();
                                 const t = await this.client.generateRecommendations(e, this.optOut);
-                                i = await t.json(), this.logger.debug("responseJson", i), h = i["x-amzn-requestid"], g = i["x-amzn-sessionid"], c = "Succeeded"
+                                i = await t.json(), this.logger.debug("responseJson", i), g = i["x-amzn-requestid"], h = i["x-amzn-sessionid"], c = "Succeeded"
                             } catch (e) {
                                 this.logger.error("Error in calling generateRecommendations API ", e), a = e, c = "Failed"
                             } finally {
                                 if (i && !d.isResponseSuccess(i)) {
                                     const e = d.getErrorResponseUserMessage(i);
                                     await l.NotificationManager.getInstance().postNotificationForApiExceptions(e, r.message("codewhisperer_learn_more"), s.LEARN_MORE_NOTIFICATION_URL), a = e, i.message && i.message.includes("Invalid input data") && (C = !1, this.logger.debug("Invalid input data, not recording service invocation")), c = "Failed"
                                 }
                                 let v;
-                                i && d.isResponseSuccess(i) && ("recommendations" in i.data ? v = i.data.recommendations : "completions" in i.data && (v = i.data.completions, m = s.AWS_BUILDER_ID_START_URL), this.suggestionsWithCodeReferences || (v = v.filter((e => !Array.isArray(e.references) || 0 === e.references.length)))), v && (this.receivedResponseSignal.emit(v), _ += v.length > 0 ? v.length : 1, this.logger.debug("successfully received valid recommendations"));
+                                i && d.isResponseSuccess(i) && ("recommendations" in i.data ? v = i.data.recommendations : "completions" in i.data && (v = i.data.completions, p = s.AWS_BUILDER_ID_START_URL), this.suggestionsWithCodeReferences || (v = v.filter((e => !Array.isArray(e.references) || 0 === e.references.length)))), v && (this.receivedResponseSignal.emit(v), _ += v.length > 0 ? v.length : 1, this.logger.debug("successfully received valid recommendations"));
                                 const I = d.detectCompletionType(v);
                                 if (C && this.serviceInvocationSignal.emit({
-                                        codewhispererRequestId: h,
-                                        credentialStartUrl: m,
+                                        codewhispererRequestId: g,
+                                        credentialStartUrl: p,
                                         duration: Date.now() - o,
                                         reason: a,
                                         result: c,
                                         codewhispererCompletionType: I,
                                         codewhispererTriggerType: t.triggerType,
                                         codewhispererAutomatedTriggerType: t.automatedTriggerType,
-                                        codewhispererSessionId: g,
+                                        codewhispererSessionId: h,
                                         codewhispererJupyterLabCellCount: n.cellCount,
                                         codewhispererJupyterLabCellIndex: n.activeCellIdx,
                                         codewhispererJupyterLabCellType: n.cellType,
                                         codewhispererLanguage: t.language,
                                         codewhispererLastSuggestionIndex: "Succeeded" === c && v ? _ - 1 : -1,
                                         codewhispererCursorOffset: n.cursorOffset,
                                         codewhispererLineNumber: n.lineNumber
                                     }), "Succeeded" === c && (u.RecommendationStateHandler.instance.updateInvocationMetadata({
                                         completionType: I,
-                                        credentialStartUrl: m,
-                                        sessionId: g,
+                                        credentialStartUrl: p,
+                                        sessionId: h,
                                         paginationProgress: _,
                                         fileContextMetadata: n,
                                         triggerMetadata: t
-                                    }, h, 0 === p), v && u.RecommendationStateHandler.instance.addRecommendations(v)), !i || !d.isResponseSuccess(i) || "" === i.data.nextToken) break;
-                                e.nextToken = i.data.nextToken, p++
+                                    }, g, 0 === m), v && u.RecommendationStateHandler.instance.addRecommendations(v)), !i || !d.isResponseSuccess(i) || "" === i.data.nextToken) break;
+                                e.nextToken = i.data.nextToken, m++
                             }
                         }
                         this.isInvocationCancelled && u.RecommendationStateHandler.instance.rejectRecommendationSignal.emit(-1), this.isGetCompletionsRunning = !1
                     }
                 }
                 async getCompletionsPaginatedInNotebookPanel(e, t) {
                     const {
                         fileContext: n,
                         fileContextMetadata: i
                     } = o.getFileContextFromNotebook(e);
                     let r = {
                         fileContext: n,
                         maxResults: s.MAX_RECOMMENDATIONS,
                         referenceTrackerConfiguration: {
-                            recommendationsWithReferences: this.suggestionsWithCodeReferences ? "ALLOW" : "DENY"
+                            recommendationsWithReferences: this.suggestionsWithCodeReferences ? "ALLOW" : "BLOCK"
                         },
                         nextToken: ""
                     };
                     return await this.getCompletionsPaginated(r, t, i)
                 }
                 async getCompletionsPaginatedInEditor(e, t, n) {
                     const {
@@ -1346,15 +1350,15 @@
                 setSuggestionsWithCodeReferences(e) {
                     this.suggestionsWithCodeReferences = e
                 }
                 setOptOut(e) {
                     this.optOut = e
                 }
             }
-            t.Worker = h
+            t.Worker = g
         },
         3770: (e, t, n) => {
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.ReferenceTracker = t.LOG_SOURCE = void 0;
             const i = n(5185),
                 o = n(9303),
@@ -1434,31 +1438,31 @@
                 s = n(8826),
                 r = i(n(6271)),
                 a = n(3706),
                 c = n(4968),
                 l = n(4865),
                 d = n(1174),
                 u = n(9462),
-                h = n(1708),
-                g = n(4657),
-                m = n(4872),
-                p = n(3770),
+                g = n(1708),
+                h = n(4657),
+                p = n(4872),
+                m = n(3770),
                 _ = n(4442),
                 C = n(5064),
                 v = n(9513),
                 I = n(2194),
                 w = n(2531);
             class f extends o.VDomModel {
                 constructor() {
                     super()
                 }
             }
             class y extends o.VDomRenderer {
                 constructor() {
-                    super(new f), this._popup = null, this._commandsForNotAuthenticated = new c.CommandRegistry, this._commandsForAuthenticationInProgress = new c.CommandRegistry, this._commandsForAutoSuggestionEnabled = new c.CommandRegistry, this._commandsForAutosuggestionDisabled = new c.CommandRegistry, this._renderer = new S, this._keyShortcutsInfoRows = 5, this.addClass(s.interactiveItem), this.addClass("jp-Notebook-ExecutionIndicator"), this.addClass("cwspr-statusbarwidget-parent"), this._initializeCommands(), h.AuthManager.getInstance().authStateChangedSignal.connect(this._onAuthStateChanged, this), m.Worker.getInstance().invocationStatusChangedSignal.connect(this._onInvocationStatusChanged, this)
+                    super(new f), this._popup = null, this._commandsForNotAuthenticated = new c.CommandRegistry, this._commandsForAuthenticationInProgress = new c.CommandRegistry, this._commandsForAutoSuggestionEnabled = new c.CommandRegistry, this._commandsForAutosuggestionDisabled = new c.CommandRegistry, this._renderer = new S, this._keyShortcutsInfoRows = 5, this.addClass(s.interactiveItem), this.addClass("jp-Notebook-ExecutionIndicator"), this.addClass("cwspr-statusbarwidget-parent"), this._initializeCommands(), g.AuthManager.getInstance().authStateChangedSignal.connect(this._onAuthStateChanged, this), p.Worker.getInstance().invocationStatusChangedSignal.connect(this._onInvocationStatusChanged, this)
                 }
                 _onAuthStateChanged(e, t) {
                     this.update()
                 }
                 _onInvocationStatusChanged(e, t) {
                     this.update()
                 }
@@ -1492,15 +1496,15 @@
                 }
                 _addCommandsForUnauthenticated() {
                     _.Application.getInstance().isJupyterOSS() && this._commandsForNotAuthenticated.addCommand(v.CommandIDs.startCodeWhisperer, {
                         label: d.message("codewhisperer_start"),
                         icon: l.Icons.startIcon,
                         caption: d.message("codewhisperer_start"),
                         execute: async () => {
-                            this._handleClick(), h.AuthManager.getInstance().isAuthenticated() || h.AuthManager.getInstance().isAuthenticationInProgress() || await h.AuthManager.getInstance().login()
+                            this._handleClick(), g.AuthManager.getInstance().isAuthenticated() || g.AuthManager.getInstance().isAuthenticationInProgress() || await g.AuthManager.getInstance().login()
                         }
                     }), this._commandsForNotAuthenticated.addCommand(v.CommandIDs.openDocumentation, {
                         label: d.message("codewhisperer_documentation_open"),
                         icon: l.Icons.documentationIcon,
                         caption: d.message("codewhisperer_documentation_open"),
                         execute: async () => {
                             window.open(v.CWSPR_DOCUMENTATION, "_blank"), this._handleClick()
@@ -1509,15 +1513,15 @@
                 }
                 _addCommandsForAuthenticationInProgress() {
                     this._commandsForAuthenticationInProgress.addCommand(v.CommandIDs.cancelLogin, {
                         label: d.message("codewhisperer_cancel_login"),
                         icon: l.Icons.startIcon,
                         caption: d.message("codewhisperer_cancel_login"),
                         execute: async () => {
-                            this._handleClick(), h.AuthManager.getInstance().isAuthenticationInProgress() && await h.AuthManager.getInstance().cancelLogin()
+                            this._handleClick(), g.AuthManager.getInstance().isAuthenticationInProgress() && await g.AuthManager.getInstance().cancelLogin()
                         }
                     }), this._commandsForAuthenticationInProgress.addCommand(v.CommandIDs.openDocumentation, {
                         label: d.message("codewhisperer_documentation_open"),
                         icon: l.Icons.documentationIcon,
                         caption: d.message("codewhisperer_documentation_open"),
                         execute: async () => {
                             window.open(v.CWSPR_DOCUMENTATION, "_blank"), this._handleClick()
@@ -1525,98 +1529,98 @@
                     })
                 }
                 _addCommandsForAuthenticatedCommon(e) {
                     e.addCommand(v.CommandIDs.openReferenceLog, {
                         label: d.message("codewhisperer_reference_log_open"),
                         icon: l.Icons.referenceLogIcon,
                         caption: d.message("codewhisperer_reference_log_open"),
-                        isToggled: () => p.ReferenceTracker.getInstance().isReferenceLogDisposed(),
+                        isToggled: () => m.ReferenceTracker.getInstance().isReferenceLogDisposed(),
                         execute: async () => {
-                            p.ReferenceTracker.getInstance().isReferenceLogDisposed() ? _.Application.getInstance().jupyterApp.shell.add(p.ReferenceTracker.getInstance().createReferenceLogWidget(), "down", {
-                                ref: p.LOG_SOURCE,
+                            m.ReferenceTracker.getInstance().isReferenceLogDisposed() ? _.Application.getInstance().jupyterApp.shell.add(m.ReferenceTracker.getInstance().createReferenceLogWidget(), "down", {
+                                ref: m.LOG_SOURCE,
                                 mode: "split-bottom"
-                            }) : p.ReferenceTracker.getInstance().disposeReferenceLogWidget(), this._handleClick()
+                            }) : m.ReferenceTracker.getInstance().disposeReferenceLogWidget(), this._handleClick()
                         }
                     }), e.addCommand(v.CommandIDs.openDocumentation, {
                         label: d.message("codewhisperer_documentation_open"),
                         icon: l.Icons.documentationIcon,
                         caption: d.message("codewhisperer_documentation_open"),
                         execute: async () => {
                             window.open(v.CWSPR_DOCUMENTATION, "_blank"), this._handleClick()
                         }
                     }), _.Application.getInstance().isSageMakerStudio() || e.addCommand(v.CommandIDs.signOut, {
                         label: d.message("codewhisperer_sign_out"),
                         icon: l.Icons.signOutIcon,
                         caption: d.message("codewhisperer_sign_out"),
                         execute: async () => {
-                            this._handleClick(), h.AuthManager.getInstance().isAuthenticated() && await h.AuthManager.getInstance().logout()
+                            this._handleClick(), g.AuthManager.getInstance().isAuthenticated() && await g.AuthManager.getInstance().logout()
                         }
                     })
                 }
                 _initializeCommands() {
                     this._addCommandsForUnauthenticated(), this._addCommandsForAuthenticationInProgress(), this._addKeyShortcutsInfo(this._commandsForAutosuggestionDisabled), this._commandsForAutosuggestionDisabled.addCommand(v.CommandIDs.resumeAutoSuggestion, {
                         label: d.message("codewhisperer_resume_auto_suggestion"),
                         icon: l.Icons.resumeIcon,
                         caption: d.message("codewhisperer_resume_auto_suggestion"),
                         execute: async () => {
-                            this._handleClick(), g.AutoTrigger.getInstance().enabled = !0, await w.saveState(I.AUTO_SUGGESTION, !0)
+                            this._handleClick(), h.AutoTrigger.getInstance().enabled = !0, await w.saveState(I.AUTO_SUGGESTION, !0)
                         }
                     }), this._addCommandsForAuthenticatedCommon(this._commandsForAutosuggestionDisabled), this._addKeyShortcutsInfo(this._commandsForAutoSuggestionEnabled), this._commandsForAutoSuggestionEnabled.addCommand(v.CommandIDs.pauseAutoSuggestion, {
                         label: d.message("codewhisperer_pause_auto_suggestion"),
                         icon: l.Icons.pauseIcon,
                         caption: d.message("codewhisperer_pause_auto_suggestion"),
                         execute: async () => {
-                            this._handleClick(), g.AutoTrigger.getInstance().enabled = !1, await w.saveState(I.AUTO_SUGGESTION, !1)
+                            this._handleClick(), h.AutoTrigger.getInstance().enabled = !1, await w.saveState(I.AUTO_SUGGESTION, !1)
                         }
                     }), this._addCommandsForAuthenticatedCommon(this._commandsForAutoSuggestionEnabled)
                 }
                 render() {
-                    const e = m.Worker.getInstance().isGetCompletionsRunning,
-                        t = h.AuthManager.getInstance().isAuthenticated() ? e ? r.default.createElement(l.Icons.loadingIcon.react, {
+                    const e = p.Worker.getInstance().isGetCompletionsRunning,
+                        t = g.AuthManager.getInstance().isAuthenticated() ? e ? r.default.createElement(l.Icons.loadingIcon.react, {
                             tag: "span",
                             className: "cwspr-statusbarwidget-icon"
                         }) : r.default.createElement(l.Icons.connectedIcon.react, {
                             tag: "span",
                             className: "cwspr-statusbarwidget-icon"
-                        }) : h.AuthManager.getInstance().isAuthenticationInProgress() ? r.default.createElement(l.Icons.loadingIcon.react, {
+                        }) : g.AuthManager.getInstance().isAuthenticationInProgress() ? r.default.createElement(l.Icons.loadingIcon.react, {
                             tag: "span",
                             className: "cwspr-statusbarwidget-icon"
                         }) : r.default.createElement(l.Icons.disconnectedIcon.react, {
                             tag: "span",
                             className: "cwspr-statusbarwidget-icon"
                         });
                     return r.default.createElement("div", {
                         className: "cwspr-statusbarwidget",
                         onClick: () => this._handleClick()
                     }, t, r.default.createElement("span", null, this._getStatusBarWidgetDisplayText()))
                 }
                 _getStatusBarWidgetDisplayText() {
-                    return h.AuthManager.getInstance().isAuthenticated() ? d.message("codewhisperer_status_widget_text_authenticated") : h.AuthManager.getInstance().isAuthenticationInProgress() ? d.message("codewhisperer_status_widget_text_auth_in_progress") : d.message("codewhisperer_status_widget_text_not_authenticated")
+                    return g.AuthManager.getInstance().isAuthenticated() ? d.message("codewhisperer_status_widget_text_authenticated") : g.AuthManager.getInstance().isAuthenticationInProgress() ? d.message("codewhisperer_status_widget_text_auth_in_progress") : d.message("codewhisperer_status_widget_text_not_authenticated")
                 }
                 _handleClick() {
                     const e = this._getMenu();
                     if (null !== this._popup && !this._popup.isDisposed) return this._popup.dispose(), void(this._popup = null);
                     this._menuToggled(), e.aboutToClose.connect(this._menuToggled, this), this._popup = s.showPopup({
                         body: e,
                         anchor: this,
                         align: "left"
                     })
                 }
                 _menuToggled() {
                     this.toggleClass("jp-mod-clicked")
                 }
                 _getMenu() {
-                    const e = g.AutoTrigger.getInstance().enabled;
+                    const e = h.AutoTrigger.getInstance().enabled;
                     let t;
-                    t = h.AuthManager.getInstance().isAuthenticated() ? e ? this._commandsForAutoSuggestionEnabled : this._commandsForAutosuggestionDisabled : h.AuthManager.getInstance().isAuthenticationInProgress() ? this._commandsForAuthenticationInProgress : this._commandsForNotAuthenticated;
+                    t = g.AuthManager.getInstance().isAuthenticated() ? e ? this._commandsForAutoSuggestionEnabled : this._commandsForAutosuggestionDisabled : g.AuthManager.getInstance().isAuthenticationInProgress() ? this._commandsForAuthenticationInProgress : this._commandsForNotAuthenticated;
                     const n = new a.Menu({
                         commands: t,
                         renderer: this._renderer
                     });
-                    return n.addClass("cwspr-statusbarwidget-menu"), this._addCommands(n, t), h.AuthManager.getInstance().isAuthenticated() && n.insertItem(this._keyShortcutsInfoRows, {
+                    return n.addClass("cwspr-statusbarwidget-menu"), this._addCommands(n, t), g.AuthManager.getInstance().isAuthenticated() && n.insertItem(this._keyShortcutsInfoRows, {
                         type: "separator"
                     }), n.update(), n
                 }
                 _addCommands(e, t) {
                     for (let n = 0; n < t.listCommands().length; n++) e.addItem({
                         command: t.listCommands()[n]
                     });
@@ -1771,25 +1775,25 @@
                     } catch (e) {
                         this.logger.error(`Error on postMetrics.\n${e}`)
                     }
                 }
             }
         },
         9513: (e, t) => {
-            var n, i;
+            var n, i, o;
             Object.defineProperty(t, "__esModule", {
                     value: !0
-                }), t.HttpStatusCode = t.MESSAGE_TO_CMD_ID_MAP = t.PLUGIN_ID = t.CommandIDs = t.NOTIFICATION_TEXT_LIMIT = t.NEW_CELL_AUTO_TRIGGER_DELAY_IN_MS = t.SHOW_COMPLETION_TIMER_POLL_PERIOD = t.INLINE_COMPLETION_SHOW_DELAY = t.AWS_BUILDER_ID_START_URL = t.MAX_PAGINATION_CALLS = t.MAX_RECOMMENDATIONS = t.MAX_LENGTH = t.CWSPR_DOCUMENTATION = t.UPDATE_NOTIFICATION_URL = t.LEARN_MORE_NOTIFICATION_URL = t.TELEMETRY_USER_TRIGGER_DECISION_METRIC_NAME = t.TELEMETRY_USER_DECISION_METRIC_NAME = t.TELEMETRY_SERVICE_INVOCATION_METRIC_NAME = void 0, t.TELEMETRY_SERVICE_INVOCATION_METRIC_NAME = "codewhisperer_serviceInvocation", t.TELEMETRY_USER_DECISION_METRIC_NAME = "codewhisperer_userDecision", t.TELEMETRY_USER_TRIGGER_DECISION_METRIC_NAME = "codewhisperer_userTriggerDecision", t.LEARN_MORE_NOTIFICATION_URL = "https://docs.aws.amazon.com/codewhisperer/latest/userguide/what-is-cwspr.html", t.UPDATE_NOTIFICATION_URL = "https://pypi.org/project/amazon-codewhisperer-jupyterlab-ext/", t.CWSPR_DOCUMENTATION = "https://docs.aws.amazon.com/codewhisperer/latest/userguide/what-is-cwspr.html", t.MAX_LENGTH = 10240, t.MAX_RECOMMENDATIONS = 5, t.MAX_PAGINATION_CALLS = 10, t.AWS_BUILDER_ID_START_URL = "https://view.awsapps.com/start", t.INLINE_COMPLETION_SHOW_DELAY = 250, t.SHOW_COMPLETION_TIMER_POLL_PERIOD = 25, t.NEW_CELL_AUTO_TRIGGER_DELAY_IN_MS = 1e4, t.NOTIFICATION_TEXT_LIMIT = 140,
+                }), t.SettingIDs = t.HttpStatusCode = t.MESSAGE_TO_CMD_ID_MAP = t.PLUGIN_ID = t.CommandIDs = t.NOTIFICATION_TEXT_LIMIT = t.NEW_CELL_AUTO_TRIGGER_DELAY_IN_MS = t.SHOW_COMPLETION_TIMER_POLL_PERIOD = t.INLINE_COMPLETION_SHOW_DELAY = t.AWS_BUILDER_ID_START_URL = t.MAX_PAGINATION_CALLS = t.MAX_RECOMMENDATIONS = t.MAX_LENGTH = t.CWSPR_DOCUMENTATION = t.UPDATE_NOTIFICATION_URL = t.LEARN_MORE_NOTIFICATION_URL = t.TELEMETRY_USER_TRIGGER_DECISION_METRIC_NAME = t.TELEMETRY_USER_DECISION_METRIC_NAME = t.TELEMETRY_SERVICE_INVOCATION_METRIC_NAME = void 0, t.TELEMETRY_SERVICE_INVOCATION_METRIC_NAME = "codewhisperer_serviceInvocation", t.TELEMETRY_USER_DECISION_METRIC_NAME = "codewhisperer_userDecision", t.TELEMETRY_USER_TRIGGER_DECISION_METRIC_NAME = "codewhisperer_userTriggerDecision", t.LEARN_MORE_NOTIFICATION_URL = "https://docs.aws.amazon.com/codewhisperer/latest/userguide/what-is-cwspr.html", t.UPDATE_NOTIFICATION_URL = "https://pypi.org/project/amazon-codewhisperer-jupyterlab-ext/", t.CWSPR_DOCUMENTATION = "https://docs.aws.amazon.com/codewhisperer/latest/userguide/what-is-cwspr.html", t.MAX_LENGTH = 10240, t.MAX_RECOMMENDATIONS = 5, t.MAX_PAGINATION_CALLS = 10, t.AWS_BUILDER_ID_START_URL = "https://view.awsapps.com/start", t.INLINE_COMPLETION_SHOW_DELAY = 250, t.SHOW_COMPLETION_TIMER_POLL_PERIOD = 25, t.NEW_CELL_AUTO_TRIGGER_DELAY_IN_MS = 1e4, t.NOTIFICATION_TEXT_LIMIT = 140,
                 function(e) {
                     e.invoke = "completer:invoke", e.invokeNotebook = "completer:invoke-notebook", e.invokeFile = "completer:invoke-file", e.select = "completer:select", e.selectNotebook = "completer:select-notebook", e.login = "codewhisperer:login", e.invokeInline = "codewhisperer:invoke-inline", e.rejectInline = "codewhisperer:reject-inline", e.acceptInline = "codewhisperer:accept-inline", e.showNext = "codewhisperer:show-next", e.showPrev = "codewhisperer:show-prev", e.startCodeWhisperer = "codewhisperer:start", e.cancelLogin = "codewhisperer:cancel-login", e.openDocumentation = "codewhisperer:documentation", e.pauseAutoSuggestion = "codewhisperer:pause-auto-suggestion", e.resumeAutoSuggestion = "codewhisperer:resume-auto-suggestion", e.openReferenceLog = "codewhisperer:open-reference-log", e.signOut = "codewhisperer:sign-out", e.keyShortcutTitle = "codewhisperer:key-shortcut-title", e.keyShortcutAccept = "codewhisperer:key-shortcut-accept", e.keyShortcutManualTrigger = "codewhisperer:key-shortcut-manual-trigger", e.keyShortcutNavigate = "codewhisperer:key-shortcut-navigate", e.keyShortcutReject = "codewhisperer:key-shortcut-reject"
                 }(n = t.CommandIDs || (t.CommandIDs = {})), t.PLUGIN_ID = "amazon-codewhisperer-jupyterlab-ext:completer", t.MESSAGE_TO_CMD_ID_MAP = {
                     codewhisperer_key_shortcut_accept: n.acceptInline,
                     codewhisperer_key_shortcut_manual_trigger: n.invokeInline,
                     codewhisperer_key_shortcut_reject: n.rejectInline
-                }, (i = t.HttpStatusCode || (t.HttpStatusCode = {}))[i.OK = 200] = "OK", i[i.NOT_FOUND = 404] = "NOT_FOUND"
+                }, (o = t.HttpStatusCode || (t.HttpStatusCode = {}))[o.OK = 200] = "OK", o[o.NOT_FOUND = 404] = "NOT_FOUND", (i = t.SettingIDs || (t.SettingIDs = {})).keyOptOut = "shareCodeWhispererContentWithAWS", i.keyTelemetry = "codeWhispererTelemetry", i.keyReferences = "suggestionsWithCodeReferences", i.keyLogLevel = "codeWhispererLogLevel"
         },
         7126: (e, t) => {
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.LicenseUtil = void 0, t.LicenseUtil = class {
                 static getUniqueLicenseNames(e) {
                     const t = new Set;
@@ -1911,11 +1915,11 @@
             });
             const i = '<?xml version="1.0" encoding="utf-8"?>\n\x3c!-- Generator: Adobe Illustrator 27.4.0, SVG Export Plug-In . SVG Version: 6.00 Build 0)  --\x3e\n<svg version="1.1" id="Layer_1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" x="0px" y="0px"\n\t viewBox="0 0 17 17" style="enable-background:new 0 0 17 17;" xml:space="preserve">\n<circle class="jp-icon2" fill="#424242" cx="8.5" cy="8.5" r="8.5"/>\n<g>\n\t<path class="jp-icon-accent1" fill="#FFFFFF" d="M8.5,5.3L10.1,7l0.7-0.7L8.5,3.9L6.2,6.2L6.9,7L8.5,5.3z M8.5,11.7L6.9,10l-0.7,0.7l2.3,2.4l2.3-2.4L10.1,10\n\t\tL8.5,11.7z"/>\n</g>\n</svg>\n'
         },
         8123: e => {
             e.exports = JSON.parse('{"codewhisperer_status_widget_text_not_authenticated":"CodeWhisperer","codewhisperer_status_widget_text_auth_in_progress":"CodeWhisperer(Connecting...)","codewhisperer_status_widget_text_authenticated":"CodeWhisperer","codewhisperer_start":"Start CodeWhisperer","codewhisperer_cancel_login":"Cancel Login","codewhisperer_learn_more":"Learn More","codewhisperer_update_now":"Update Now","codewhisperer_documentation_open":"Documentation","codewhisperer_pause_auto_suggestion":"Pause Auto-Suggestions","codewhisperer_resume_auto_suggestion":"Resume Auto-Suggestions","codewhisperer_reference_log_open":"Open Code Reference Log","codewhisperer_sign_out":"Sign Out","codewhisperer_key_shortcut_title":"SHORTCUTS","codewhisperer_key_shortcut_accept":"Accept","codewhisperer_key_shortcut_manual_trigger":"Manual Invoke","codewhisperer_key_shortcut_navigate":"Navigate","codewhisperer_key_shortcut_reject":"Reject","codewhisperer_expiry_notification_message":"CodeWhisperer connection expired. Reauthenticate with AWS Builder ID to use CodeWhisperer.","codewhisperer_expiry_notification_button_authenticate":"Authenticate","codewhisperer_expiry_notification_button_cancel":"Cancel","codewhisperer_copy_code_and_proceed_dialog_title":"Start CodeWhisperer with AWS Builder ID","codewhisperer_copy_code_and_proceed_dialog_button_yes":"Copy Code and Proceed","codewhisperer_copy_code_and_proceed_dialog_message_first_li":"To use CodeWhisperer, individual developers must sign in using AWS Builder ID. ","codewhisperer_copy_code_and_proceed_dialog_message_first_li_learn_more":"Learn More","codewhisperer_copy_code_and_proceed_dialog_message_second_li":"A login page will open on an external website: https://device.sso.us-east-1.amazonaws.com","codewhisperer_copy_code_and_proceed_dialog_message_third_li":"Provide this code to confirm the access request: ","codewhisperer_server_extension_not_enabled_message":"CodeWhisperer isn\'t enabled. Run `jupyter server extension enable amazon_codewhisperer_jupyterlab_ext`, then restart server & refresh browser.","codewhisperer_update_notification_skip_this_version":"Skip this version","codewhisperer_notification_show_full_message_button_title":"Expand"}')
         },
         4147: e => {
-            e.exports = JSON.parse('{"name":"amazon-codewhisperer-jupyterlab-ext","version":"1.0.1","description":"Amazon CodeWhisperer for JupyterLab","keywords":["jupyter","jupyterlab","jupyterlab-extension","codewhisperer","amazon-codewhisperer"],"homepage":"https://github.com/aws","bugs":{"url":"https://aws.amazon.com/codewhisperer/","email":"codewhisperer@amazon.com"},"license":"Apache 2.0","licenses":[{"type":"Amazon Software License","url":"http://aws.amazon.com/asl"}],"author":{"name":"Amazon CodeWhisperer","email":"codewhisperer@amazon.com"},"files":["lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}","style/**/*.{css,eot,js,gif,html,jpg,json,png,svg,woff2,ttf}","style/img/*.{svg}","schema/*.json"],"main":"lib/index.js","types":"lib/index.d.ts","style":"style/index.css","config":{"vars":{"builddir":"./build/lib/amazon-codewhisperer-jupyterlab-ext","jupyterCorePath":"./build-tools/jupyter-staging"}},"npm-pretty-much":{"https://w/?NpmPrettyMuch/UndeclaredTransitiveDependencies":true,"legacyPackageNameAlias":"amazon-codewhisperer-jupyterlab-ext","runTest":"always","runRelease":"always"},"scripts":{"build":"npm run clean && npm run build:lib && npm run build:labextension","postbuild":"mkdir -p $npm_package_config_vars_builddir && rsync package.json $npm_package_config_vars_builddir && rsync -a --exclude={‘*.spec.d.ts’,’*.spec.js’} lib $npm_package_config_vars_builddir && rsync -a style $npm_package_config_vars_builddir","build:all":"npm run build:lib && npm run build:labextension","build:labextension":"build-labextension --core-path $npm_package_config_vars_jupyterCorePath .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:prod":"npm run clean && npm run build:lib && npm run build:labextension","clean":"npm run clean:lib","clean:all":"npm run clean:lib && npm run clean:labextension","clean:labextension":"rimraf amazon_codewhisperer_jupyterlab_ext/labextension","clean:lib":"rimraf lib tsconfig.tsbuildinfo","eslint":"eslint . --ext .ts,.tsx --fix","eslint:check":"eslint . --ext .ts,.tsx","install:extension":"npm run build","dev":"npm run clean && npm run build:lib && npm run build:labextension:dev","dist":"python setup.py sdist","release":"npm run build && npm run postbuild && npm run dist","watch":"run-p watch:src watch:labextension","watch:labextension":"jupyter labextension watch .","watch:src":"tsc -w","generateTelemetry":"node node_modules/@aws-toolkits/telemetry/lib/generateTelemetry.js --output=src/telemetry/telemetry.gen.ts","generateClients":"ts-node ./scripts/build/generateServiceClient.ts ","test":"jest --no-cache"},"dependencies":{"@jupyterlab/application":"^3.1.0","@jupyterlab/apputils":"^3.1.0","@jupyterlab/codeeditor":"^3.1.0","@jupyterlab/codemirror":"^3.1.0","@jupyterlab/completer":"^3.1.0","@jupyterlab/fileeditor":"^3.1.0","@jupyterlab/launcher":"^3.1.0","@jupyterlab/logconsole":"^3.6.3","@jupyterlab/nbformat":"^3.6.3","@jupyterlab/notebook":"^3.1.0","@jupyterlab/outputarea":"^3.1.0","@jupyterlab/rendermime":"^3.6.3","@jupyterlab/settingregistry":"^3.1.0","@jupyterlab/statedb":"^3.6.3","@jupyterlab/translation":"^3.1.0","@lumino/algorithm":"^1.6.0","@lumino/coreutils":"^1.8.0","@lumino/datagrid":"^0.27.0","@lumino/disposable":"^1.7.0","aws-sdk":"^2.1267.0","pino":"^8.11.0"},"devDependencies":{"@aws-toolkits/telemetry":"^1.0.120","@babel/core":"^7.21.5","@babel/preset-env":"^7.21.5","@jupyterlab/builder":"^3.6.3","@jupyterlab/testutils":"^3.6.3","@types/codemirror":"^5.60.7","@types/fs-extra":"^9.0.11","@types/jest":"27.0.0","@types/node":"^16.0.0","@typescript-eslint/eslint-plugin":"^4.8.1","@typescript-eslint/parser":"^4.8.1","eslint":"^7.14.0","eslint-config-prettier":"^6.15.0","eslint-plugin-jsdoc":"^40.0.0","eslint-plugin-prettier":"^3.1.4","eslint-plugin-react":"^7.18.3","jest":"27.0.0","jest-fetch-mock":"^1.6.6","npm-run-all":"^4.1.5","prettier":"^2.1.1","rimraf":"^3.0.2","ts-jest":"27.0.0","typescript":"~4.3.0","jest-environment-jsdom":"^27.0.0"},"sideEffects":["style/*.css","style/index.js"],"jupyterlab":{"extension":true,"schemaDir":"schema","outputDir":"amazon_codewhisperer_jupyterlab_ext/labextension","disabledExtensions":["@jupyterlab/completer-extension:notebooks","@jupyterlab/completer-extension:files"]},"styleModule":"style/index.js"}')
+            e.exports = JSON.parse('{"name":"amazon-codewhisperer-jupyterlab-ext","version":"1.0.3","description":"Amazon CodeWhisperer for JupyterLab","keywords":["jupyter","jupyterlab","jupyterlab-extension","codewhisperer","amazon-codewhisperer"],"homepage":"https://github.com/aws","bugs":{"url":"https://aws.amazon.com/codewhisperer/","email":"codewhisperer@amazon.com"},"license":"Apache 2.0","licenses":[{"type":"Amazon Software License","url":"http://aws.amazon.com/asl"}],"author":{"name":"Amazon CodeWhisperer","email":"codewhisperer@amazon.com"},"files":["lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}","style/**/*.{css,eot,js,gif,html,jpg,json,png,svg,woff2,ttf}","style/img/*.{svg}","schema/*.json"],"main":"lib/index.js","types":"lib/index.d.ts","style":"style/index.css","config":{"vars":{"builddir":"./build/lib/amazon-codewhisperer-jupyterlab-ext","jupyterCorePath":"./build-tools/jupyter-staging"}},"npm-pretty-much":{"https://w/?NpmPrettyMuch/UndeclaredTransitiveDependencies":true,"legacyPackageNameAlias":"amazon-codewhisperer-jupyterlab-ext","runTest":"always","runRelease":"always"},"scripts":{"build":"npm run clean && npm run build:lib && npm run build:labextension","postbuild":"mkdir -p $npm_package_config_vars_builddir && rsync package.json $npm_package_config_vars_builddir && rsync -a --exclude={‘*.spec.d.ts’,’*.spec.js’} lib $npm_package_config_vars_builddir && rsync -a style $npm_package_config_vars_builddir","build:all":"npm run build:lib && npm run build:labextension","build:labextension":"build-labextension --core-path $npm_package_config_vars_jupyterCorePath .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:prod":"npm run clean && npm run build:lib && npm run build:labextension","clean":"npm run clean:lib","clean:all":"npm run clean:lib && npm run clean:labextension","clean:labextension":"rimraf amazon_codewhisperer_jupyterlab_ext/labextension","clean:lib":"rimraf lib tsconfig.tsbuildinfo","eslint":"eslint . --ext .ts,.tsx --fix","eslint:check":"eslint . --ext .ts,.tsx","install:extension":"npm run build","dev":"npm run clean && npm run build:lib && npm run build:labextension:dev","dist":"python setup.py sdist","release":"npm run build && npm run postbuild && npm run dist","watch":"run-p watch:src watch:labextension","watch:labextension":"jupyter labextension watch .","watch:src":"tsc -w","generateTelemetry":"node node_modules/@aws-toolkits/telemetry/lib/generateTelemetry.js --output=src/telemetry/telemetry.gen.ts","generateClients":"ts-node ./scripts/build/generateServiceClient.ts ","test":"jest --no-cache"},"dependencies":{"@jupyterlab/application":"^3.1.0","@jupyterlab/apputils":"^3.1.0","@jupyterlab/codeeditor":"^3.1.0","@jupyterlab/codemirror":"^3.1.0","@jupyterlab/completer":"^3.1.0","@jupyterlab/fileeditor":"^3.1.0","@jupyterlab/launcher":"^3.1.0","@jupyterlab/logconsole":"^3.6.3","@jupyterlab/nbformat":"^3.6.3","@jupyterlab/notebook":"^3.1.0","@jupyterlab/outputarea":"^3.1.0","@jupyterlab/rendermime":"^3.6.3","@jupyterlab/settingregistry":"^3.1.0","@jupyterlab/statedb":"^3.6.3","@jupyterlab/translation":"^3.1.0","@lumino/algorithm":"^1.6.0","@lumino/coreutils":"^1.8.0","@lumino/datagrid":"^0.27.0","@lumino/disposable":"^1.7.0","aws-sdk":"^2.1267.0","pino":"^8.11.0"},"devDependencies":{"@aws-toolkits/telemetry":"^1.0.120","@babel/core":"^7.21.5","@babel/preset-env":"^7.21.5","@jupyterlab/builder":"^3.6.3","@jupyterlab/testutils":"^3.6.3","@types/codemirror":"^5.60.7","@types/fs-extra":"^9.0.11","@types/jest":"27.0.0","@types/node":"^16.0.0","@typescript-eslint/eslint-plugin":"^4.8.1","@typescript-eslint/parser":"^4.8.1","eslint":"^7.14.0","eslint-config-prettier":"^6.15.0","eslint-plugin-jsdoc":"^40.0.0","eslint-plugin-prettier":"^3.1.4","eslint-plugin-react":"^7.18.3","jest":"27.0.0","jest-fetch-mock":"^1.6.6","npm-run-all":"^4.1.5","prettier":"^2.1.1","rimraf":"^3.0.2","ts-jest":"27.0.0","typescript":"~4.3.0","jest-environment-jsdom":"^27.0.0","pino-pretty":"10.0.0"},"sideEffects":["style/*.css","style/index.js"],"jupyterlab":{"extension":true,"schemaDir":"schema","outputDir":"amazon_codewhisperer_jupyterlab_ext/labextension","disabledExtensions":["@jupyterlab/completer-extension:notebooks","@jupyterlab/completer-extension:files"]},"styleModule":"style/index.js"}')
         }
     }
 ]);
```

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext/labextension/static/571.3582fd184eff1ff4b836.js` & `amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/labextension/static/571.3582fd184eff1ff4b836.js`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext/labextension/static/747.462ff5e5d49d87208721.js` & `amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/labextension/static/747.462ff5e5d49d87208721.js`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext/labextension/static/remoteEntry.3451ec5921d04a9e8b07.js` & `amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/labextension/static/remoteEntry.9bf04351778104e8e5cd.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,12 +1,12 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, a, i, u, l, s, d, f, p, c, h, v, b, m, y, g, j, w, S, x = {
-            2842: (e, r, t) => {
+    var e, r, t, n, o, a, i, u, l, d, s, f, p, c, h, v, b, m, y, g, j, w, S, x = {
+            6972: (e, r, t) => {
                 var n = {
                         "./index": () => t.e(568).then((() => () => t(1568))),
                         "./extension": () => t.e(568).then((() => () => t(1568))),
                         "./style": () => t.e(747).then((() => () => t(9747)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
@@ -43,37 +43,37 @@
         }), r
     }, E.d = (e, r) => {
         for (var t in r) E.o(r, t) && !E.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, E.f = {}, E.e = e => Promise.all(Object.keys(E.f).reduce(((r, t) => (E.f[t](e, r), r)), [])), E.u = e => e + "." + {
-        568: "e71a5b77238395161eb2",
+        568: "c0e5b626da6cbe06eb5e",
         571: "3582fd184eff1ff4b836",
         747: "462ff5e5d49d87208721"
     } [e] + ".js?v=" + {
-        568: "e71a5b77238395161eb2",
+        568: "c0e5b626da6cbe06eb5e",
         571: "3582fd184eff1ff4b836",
         747: "462ff5e5d49d87208721"
     } [e], E.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), E.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "amazon-codewhisperer-jupyterlab-ext:", E.l = (t, n, o, a) => {
         if (e[t]) e[t].push(n);
         else {
             var i, u;
             if (void 0 !== o)
-                for (var l = document.getElementsByTagName("script"), s = 0; s < l.length; s++) {
-                    var d = l[s];
-                    if (d.getAttribute("src") == t || d.getAttribute("data-webpack") == r + o) {
-                        i = d;
+                for (var l = document.getElementsByTagName("script"), d = 0; d < l.length; d++) {
+                    var s = l[d];
+                    if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + o) {
+                        i = s;
                         break
                     }
                 }
             i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, E.nc && i.setAttribute("nonce", E.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
             var f = (r, n) => {
                     i.onerror = i.onload = null, clearTimeout(p);
                     var o = e[t];
@@ -109,15 +109,15 @@
                         (!u || !u.loaded && (!n != !u.eager ? n : i > u.from)) && (o[r] = {
                             get: t,
                             from: i,
                             eager: !!n
                         })
                     },
                     l = [];
-                return "default" === t && (u("amazon-codewhisperer-jupyterlab-ext", "1.0.1", (() => E.e(568).then((() => () => E(1568))))), u("pino", "8.11.0", (() => E.e(571).then((() => () => E(5571)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                return "default" === t && (u("amazon-codewhisperer-jupyterlab-ext", "1.0.3", (() => E.e(568).then((() => () => E(1568))))), u("pino", "8.11.0", (() => E.e(571).then((() => () => E(5571)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         E.g.importScripts && (e = E.g.location + "");
         var r = E.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -167,31 +167,31 @@
     }, a = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 o = n < 0;
             o && (n = -n - 1);
             for (var i = 0, u = 1, l = !0;; u++, i++) {
-                var s, d, f = u < e.length ? (typeof e[u])[0] : "";
-                if (i >= r.length || "o" == (d = (typeof(s = r[i]))[0])) return !l || ("u" == f ? u > n && !o : "" == f != o);
-                if ("u" == d) {
+                var d, s, f = u < e.length ? (typeof e[u])[0] : "";
+                if (i >= r.length || "o" == (s = (typeof(d = r[i]))[0])) return !l || ("u" == f ? u > n && !o : "" == f != o);
+                if ("u" == s) {
                     if (!l || "u" != f) return !1
                 } else if (l)
-                    if (f == d)
+                    if (f == s)
                         if (u <= n) {
-                            if (s != e[u]) return !1
+                            if (d != e[u]) return !1
                         } else {
-                            if (o ? s > e[u] : s < e[u]) return !1;
-                            s != e[u] && (l = !1)
+                            if (o ? d > e[u] : d < e[u]) return !1;
+                            d != e[u] && (l = !1)
                         }
                 else if ("s" != f && "n" != f) {
                     if (o || u <= n) return !1;
                     l = !1, u--
                 } else {
-                    if (u <= n || d < f != o) return !1;
+                    if (u <= n || s < f != o) return !1;
                     l = !1
                 } else "s" != f && "n" != f && (l = !1, u--)
             }
         }
         var p = [],
             c = p.pop.bind(p);
         for (i = 1; i < e.length; i++) {
@@ -205,31 +205,31 @@
         return t
     }, u = (e, r) => {
         var t = e[r];
         return (r = Object.keys(t).reduce(((e, r) => !e || n(e, r) ? r : e), 0)) && t[r]
     }, l = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, s = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", d = (e, r, t, n) => {
+    }, d = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", s = (e, r, t, n) => {
         var o = l(e, t);
-        return a(n, o) || c(s(e, t, o, n)), v(e[t][o])
+        return a(n, o) || c(d(e, t, o, n)), v(e[t][o])
     }, f = (e, r, t) => {
         var o = e[r];
         return (r = Object.keys(o).reduce(((e, r) => !a(t, r) || e && !n(e, r) ? e : r), 0)) && o[r]
     }, p = (e, r, t, n) => {
         var a = e[t];
         return "No satisfying version (" + o(n) + ") of shared module " + t + " found in shared scope " + r + ".\nAvailable versions: " + Object.keys(a).map((e => e + " from " + a[e].from)).join(", ")
     }, c = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
     }, h = (e, r, t, n) => {
         c(p(e, r, t, n))
     }, v = e => (e.loaded = 1, e.get()), m = (b = e => function(r, t, n, o) {
         var a = E.I(r);
         return a && a.then ? a.then(e.bind(e, r, E.S[r], t, n, o)) : e(r, E.S[r], t, n, o)
-    })(((e, r, t, n) => (i(e, t), v(f(r, t, n) || h(r, e, t, n) || u(r, t))))), y = b(((e, r, t, n) => (i(e, t), d(r, 0, t, n)))), g = b(((e, r, t, n, o) => {
+    })(((e, r, t, n) => (i(e, t), v(f(r, t, n) || h(r, e, t, n) || u(r, t))))), y = b(((e, r, t, n) => (i(e, t), s(r, 0, t, n)))), g = b(((e, r, t, n, o) => {
         var a = r && E.o(r, t) && f(r, t, n);
         return a ? v(a) : o()
     })), j = {}, w = {
         968: () => y("default", "@jupyterlab/ui-components", [1, 3, 1, 11]),
         1396: () => y("default", "@jupyterlab/coreutils", [1, 5, 1, 11]),
         1797: () => y("default", "@lumino/coreutils", [1, 1, 5, 3]),
         2766: () => y("default", "@jupyterlab/notebook", [1, 3, 1, 11]),
@@ -301,10 +301,10 @@
                     u && u(E)
                 }
                 for (r && r(t); l < a.length; l++) o = a[l], E.o(e, o) && e[o] && e[o][0](), e[o] = 0
             },
             t = self.webpackChunkamazon_codewhisperer_jupyterlab_ext = self.webpackChunkamazon_codewhisperer_jupyterlab_ext || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), E.nc = void 0;
-    var _ = E(2842);
+    var _ = E(6972);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["amazon-codewhisperer-jupyterlab-ext"] = _
 })();
```

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext/labextension/static/third-party-licenses.json` & `amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext/utils.py` & `amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/utils.py`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext/validator/schemas/generate_recommendations.json` & `amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/validator/schemas/generate_recommendations.json`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext/validator/validator.py` & `amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/validator/validator.py`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext.egg-info/PKG-INFO` & `amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon-codewhisperer-jupyterlab-ext
-Version: 1.0.1
+Version: 1.0.3
 Summary: Amazon CodeWhisperer for JupyterLab
 Home-page: https://aws.amazon.com/codewhisperer/
 Author: Amazon CodeWhisperer
 Author-email: codewhisperer@amazon.com
 License: Apache 2.0
 Keywords: Jupyter,JupyterLab,JupyterLab3,Amazon CodeWhisperer,CodeWhisperer,Code,Whisperer
 Platform: Linux
@@ -91,9 +91,18 @@
 
 ## More Resources
 
 * [CodeWhisperer User Guide](https://docs.aws.amazon.com/codewhisperer/latest/userguide/what-is-cwspr.html)
 * [Setting up Amazon CodeWhisperer with JupyterLab](https://docs.aws.amazon.com/codewhisperer/latest/userguide/jupyterlab-setup.html)
 * [Setting up CodeWhisperer with Amazon SageMaker Studio](https://docs.aws.amazon.com/codewhisperer/latest/userguide/sagemaker-setup.html)
 
+## Change Log
+
+1.0.3
+* Bug fix: No recommendation when user turn off code suggestions with references in settings.
+* Bug fix: Issue with browser login flow for some Builder ID users.
+* Bug fix: Fix an issue where SageMaker Studio users will incorrectly see the `Share content with Amazon CodeWhisperer` settings option.
+
+1.0.0
+* Initial release
```

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.1/amazon_codewhisperer_jupyterlab_ext.egg-info/SOURCES.txt` & `amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -32,33 +32,34 @@
 amazon_codewhisperer_jupyterlab_ext/client/telemetry/__init__.py
 amazon_codewhisperer_jupyterlab_ext/client/telemetry/telemetry.py
 amazon_codewhisperer_jupyterlab_ext/env/__init__.py
 amazon_codewhisperer_jupyterlab_ext/env/environment.py
 amazon_codewhisperer_jupyterlab_ext/labextension/package.json
 amazon_codewhisperer_jupyterlab_ext/labextension/schemas/amazon-codewhisperer-jupyterlab-ext/completer.json
 amazon_codewhisperer_jupyterlab_ext/labextension/schemas/amazon-codewhisperer-jupyterlab-ext/package.json.orig
-amazon_codewhisperer_jupyterlab_ext/labextension/static/568.e71a5b77238395161eb2.js
-amazon_codewhisperer_jupyterlab_ext/labextension/static/568.e71a5b77238395161eb2.js.LICENSE.txt
+amazon_codewhisperer_jupyterlab_ext/labextension/static/568.c0e5b626da6cbe06eb5e.js
+amazon_codewhisperer_jupyterlab_ext/labextension/static/568.c0e5b626da6cbe06eb5e.js.LICENSE.txt
 amazon_codewhisperer_jupyterlab_ext/labextension/static/571.3582fd184eff1ff4b836.js
 amazon_codewhisperer_jupyterlab_ext/labextension/static/747.462ff5e5d49d87208721.js
-amazon_codewhisperer_jupyterlab_ext/labextension/static/remoteEntry.3451ec5921d04a9e8b07.js
+amazon_codewhisperer_jupyterlab_ext/labextension/static/remoteEntry.9bf04351778104e8e5cd.js
 amazon_codewhisperer_jupyterlab_ext/labextension/static/style.js
 amazon_codewhisperer_jupyterlab_ext/labextension/static/third-party-licenses.json
 amazon_codewhisperer_jupyterlab_ext/validator/__init__.py
 amazon_codewhisperer_jupyterlab_ext/validator/validator.py
 amazon_codewhisperer_jupyterlab_ext/validator/schemas/generate_recommendations.json
 jupyter-config/amazon_codewhisperer_jupyterlab_ext.json
 src/application.ts
 src/handler.ts
 src/icons.ts
 src/index.ts
 src/messages.ts
 src/svg.d.ts
 src/__tests__/index.spec.ts
 src/__tests__/autotrigger/autotrigger.spec.ts
+src/__tests__/recommendation/recommendationStateHandler.spec.ts
 src/auth/authManager.tsx
 src/autotrigger/autotrigger.ts
 src/aws_vector_consolas_jupyter_lab3_extension/__init__.py
 src/aws_vector_consolas_jupyter_lab3_extension/py.typed
 src/client/apiclient.ts
 src/client/codewhispererclient.d.ts
 src/client/codewhispereruserclient.d.ts
```

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.1/package.json` & `amazon-codewhisperer-jupyterlab-ext-1.0.3/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9752380952380952%*

 * *Differences: {"'devDependencies'": "{'pino-pretty': '10.0.0'}", "'version'": "'1.0.3'"}*

```diff
@@ -54,14 +54,15 @@
         "eslint-plugin-jsdoc": "^40.0.0",
         "eslint-plugin-prettier": "^3.1.4",
         "eslint-plugin-react": "^7.18.3",
         "jest": "27.0.0",
         "jest-environment-jsdom": "^27.0.0",
         "jest-fetch-mock": "^1.6.6",
         "npm-run-all": "^4.1.5",
+        "pino-pretty": "10.0.0",
         "prettier": "^2.1.1",
         "rimraf": "^3.0.2",
         "ts-jest": "27.0.0",
         "typescript": "~4.3.0"
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
@@ -129,9 +130,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "1.0.1"
+    "version": "1.0.3"
 }
```

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.1/pyproject.toml` & `amazon-codewhisperer-jupyterlab-ext-1.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.1/setup.py` & `amazon-codewhisperer-jupyterlab-ext-1.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.1/src/__tests__/autotrigger/autotrigger.spec.ts` & `amazon-codewhisperer-jupyterlab-ext-1.0.3/src/__tests__/autotrigger/autotrigger.spec.ts`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.1/src/application.ts` & `amazon-codewhisperer-jupyterlab-ext-1.0.3/src/application.ts`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.1/src/auth/authManager.tsx` & `amazon-codewhisperer-jupyterlab-ext-1.0.3/src/auth/authManager.tsx`

 * *Files 1% similar despite different names*

```diff
@@ -131,14 +131,15 @@
                     label: message("codewhisperer_copy_code_and_proceed_dialog_button_yes")
                 })
             ]
         });
         if (!dialogResult.button.accept) {
             return;
         }
+        window.open(deviceAuthorizationResponseJsonData['verificationUriComplete'], '_blank')
         this.authStateChangedSignal.emit(AuthState.AUTHENTICATION_IN_PROGRESS)
         const createTokenRequest = {
             clientRegistration: registerClientResponseJsonData,
             deviceAuthorizationResponse: deviceAuthorizationResponseJsonData,
         }
         const createTokenResponsePromise = requestAPI<Response>('create_token', {
             body: JSON.stringify(createTokenRequest),
```

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.1/src/autotrigger/autotrigger.ts` & `amazon-codewhisperer-jupyterlab-ext-1.0.3/src/autotrigger/autotrigger.ts`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.1/src/client/apiclient.ts` & `amazon-codewhisperer-jupyterlab-ext-1.0.3/src/client/apiclient.ts`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.1/src/client/codewhispererclient.d.ts` & `amazon-codewhisperer-jupyterlab-ext-1.0.3/src/client/codewhispererclient.d.ts`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.1/src/client/codewhispereruserclient.d.ts` & `amazon-codewhisperer-jupyterlab-ext-1.0.3/src/client/codewhispereruserclient.d.ts`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.1/src/connector/codewhispererconnector.ts` & `amazon-codewhisperer-jupyterlab-ext-1.0.3/src/connector/codewhispererconnector.ts`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.1/src/connector/mergeconnector.ts` & `amazon-codewhisperer-jupyterlab-ext-1.0.3/src/connector/mergeconnector.ts`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.1/src/handler.ts` & `amazon-codewhisperer-jupyterlab-ext-1.0.3/src/handler.ts`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.1/src/icons.ts` & `amazon-codewhisperer-jupyterlab-ext-1.0.3/src/icons.ts`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.1/src/index.ts` & `amazon-codewhisperer-jupyterlab-ext-1.0.3/src/index.ts`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,13 @@
 /*!
  * Copyright 2022 Amazon.com, Inc. or its affiliates. All Rights Reserved.
  * SPDX-License-Identifier: Apache-2.0
  */
-import {
-  JupyterFrontEnd,
-  JupyterFrontEndPlugin,
-} from '@jupyterlab/application';
-import {
-  ContextConnector,
-  ICompletionManager,
-  KernelConnector,
-} from '@jupyterlab/completer';
+import { JupyterFrontEnd, JupyterFrontEndPlugin, } from '@jupyterlab/application';
+import { ContextConnector, ICompletionManager, KernelConnector, } from '@jupyterlab/completer';
 
 import { INotebookTracker, NotebookPanel } from '@jupyterlab/notebook';
 import { IEditorTracker } from '@jupyterlab/fileeditor'
 import { ISettingRegistry } from '@jupyterlab/settingregistry';
 
 import { MergeConnector } from './connector/mergeconnector';
 
@@ -33,15 +26,15 @@
 import StatusBarWidget from "./statusbar/statusbarwidget";
 import { CodeWhispererConnector } from './connector/codewhispererconnector';
 import { AuthManager } from "./auth/authManager";
 import { Logger } from './logging/logger';
 import { Application } from "./application";
 import { IRenderMimeRegistry } from '@jupyterlab/rendermime';
 import { ReferenceTracker } from './referencetracker/referencetracker';
-import { CommandIDs, NEW_CELL_AUTO_TRIGGER_DELAY_IN_MS, PLUGIN_ID } from './utils/constants';
+import { CommandIDs, NEW_CELL_AUTO_TRIGGER_DELAY_IN_MS, PLUGIN_ID, SettingIDs } from './utils/constants';
 import { Keybindings } from './keybindings/keybindings';
 
 /**
  * Initialization data for the extension.
  */
 const extension: JupyterFrontEndPlugin<void> = {
   id: PLUGIN_ID,
@@ -80,20 +73,35 @@
           // save clientId to state
           state.save(PLUGIN_ID, { "clientId": Telemetry.clientId });
           logger.debug(`Generated - clientId: ${Telemetry.clientId}`);
         }
       });
 
       const loadSetting = (setting: ISettingRegistry.ISettings) => {
-        Telemetry.getInstance().enableTelemetry(setting.get('codeWhispererTelemetry').composite as boolean);
-        Worker.getInstance().setOptOut(!(setting.get('shareCodeWhispererContentWithAWS').composite as boolean));
-        Worker.getInstance().setSuggestionsWithCodeReferences(setting.get('suggestionsWithCodeReferences').composite as boolean);
-        Logger.setLogLevel(setting.get('codeWhispererLogLevel').composite as string);
+        Telemetry.getInstance().enableTelemetry(setting.get(SettingIDs.keyTelemetry).composite as boolean);
+        Worker.getInstance().setOptOut(!(setting.get(SettingIDs.keyOptOut).composite as boolean));
+        Worker.getInstance().setSuggestionsWithCodeReferences(setting.get(SettingIDs.keyReferences).composite as boolean);
+        Logger.setLogLevel(setting.get(SettingIDs.keyLogLevel).composite as string);
         Keybindings.getInstance().keyBindings = [...app.commands.keyBindings];
         logger.debug(`Loaded settings`);
+
+        if (Application.getInstance().isJupyterOSS()) return;
+        const styleElement = document.createElement('style');
+
+        styleElement.textContent = `
+#jp-SettingsEditor-amazon-codewhisperer-jupyterlab-ext\\\:completer > div:first-of-type {
+  display: none !important;
+}
+
+#jp-SettingsEditor-amazon-codewhisperer-jupyterlab-ext\\\:completer > div:first-of-type > input {
+  pointer-events: none;
+  opacity: 0.5;
+}
+        `;
+        document.head.appendChild(styleElement);
       }
 
       Promise.all([app.restored, settings.load(PLUGIN_ID)])
         .then(([, setting]) => {
           loadSetting(setting);
           setting.changed.connect(loadSetting);
         })
```

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.1/src/inline/inline.ts` & `amazon-codewhisperer-jupyterlab-ext-1.0.3/src/inline/inline.ts`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.1/src/keybindings/keybindings.ts` & `amazon-codewhisperer-jupyterlab-ext-1.0.3/src/keybindings/keybindings.ts`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.1/src/notifications/notifications.tsx` & `amazon-codewhisperer-jupyterlab-ext-1.0.3/src/notifications/notifications.tsx`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.1/src/recommendation/extractor.ts` & `amazon-codewhisperer-jupyterlab-ext-1.0.3/src/recommendation/extractor.ts`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.1/src/recommendation/recommendationStateHandler.ts` & `amazon-codewhisperer-jupyterlab-ext-1.0.3/src/recommendation/recommendationStateHandler.ts`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         this.rejectRecommendationSignal.connect(this.userDecisionSignalListener, this);
         this.logger = Logger.getInstance({
             "name": "codewhisperer",
             "component" : "recommendationStateHandler"
         });
     }
 
-    private reset() {
+    reset() {
         this.timeToFirstRecommendation = undefined;
         this.requestId = undefined;
         this.firstRequestId = undefined;
         this.invocationMetadata = undefined;
         this.acceptedIndex = -1;
         this.recommendations = [];
         this.recommendationSuggestionState = new Map<number, RecommendationState>();
@@ -106,15 +106,15 @@
             })
         } else {
             RecommendationStateHandler.instance.addRecommendation({content: "", references: []});
             RecommendationStateHandler.instance.setSuggestionState(previousRecommendationsLength, "Empty");
         };
     }
 
-    private userDecisionSignalListener(sender: any, value: number) {
+    userDecisionSignalListener(sender: any, value: number) {
         this.acceptedIndex = value;
         this.recordUserDecisionTelemetry();
     }
 
     private recordUserDecisionTelemetry() {
         if (!this.invocationMetadata) {
             //TODO: this is not the optimal solution. 
@@ -189,15 +189,15 @@
             codewhispererSuggestionImportCount: undefined, // This is dummy value, we don't have this available in JupyterLab at the moment
 
         };
         Telemetry.getInstance().recordTelemetry(TELEMETRY_USER_TRIGGER_DECISION_METRIC_NAME, event);
         this.previousSuggestionState = (userDecisionByTrigger as CodewhispererPreviousSuggestionState);
     }
 
-    private getSuggestionState(i: number, acceptIndex: number): CodewhispererSuggestionState {
+    getSuggestionState(i: number, acceptIndex: number): CodewhispererSuggestionState {
         const state = this.recommendationSuggestionState?.get(i);
         if (state && acceptIndex === -1 && ["Empty", "Filter", "Discard"].includes(state)) {
             return state as CodewhispererSuggestionState;
         } else if (
             this.recommendationSuggestionState !== undefined &&
             this.recommendationSuggestionState.get(i) !== "Showed"
         ) {
```

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.1/src/recommendation/worker.ts` & `amazon-codewhisperer-jupyterlab-ext-1.0.3/src/recommendation/worker.ts`

 * *Files 0% similar despite different names*

```diff
@@ -207,15 +207,15 @@
     async getCompletionsPaginatedInNotebookPanel(panel: NotebookPanel, triggerMetadata: TriggerMetadata) {
         const { fileContext, fileContextMetadata } =
             getFileContextFromNotebook(panel);
         let request: GenerateCompletionsRequest = {
             fileContext: fileContext,
             maxResults: MAX_RECOMMENDATIONS,
             referenceTrackerConfiguration: {
-                recommendationsWithReferences: this.suggestionsWithCodeReferences ? "ALLOW" : "DENY",
+                recommendationsWithReferences: this.suggestionsWithCodeReferences ? "ALLOW" : "BLOCK",
             },
             nextToken: "",
         };
         return await this.getCompletionsPaginated(
             request,
             triggerMetadata,
             fileContextMetadata,
```

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.1/src/referencetracker/referencetracker.tsx` & `amazon-codewhisperer-jupyterlab-ext-1.0.3/src/referencetracker/referencetracker.tsx`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.1/src/statusbar/statusbarwidget.tsx` & `amazon-codewhisperer-jupyterlab-ext-1.0.3/src/statusbar/statusbarwidget.tsx`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.1/src/telemetry/clienttelemetry.d.ts` & `amazon-codewhisperer-jupyterlab-ext-1.0.3/src/telemetry/clienttelemetry.d.ts`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.1/src/telemetry/telemetry.gen.ts` & `amazon-codewhisperer-jupyterlab-ext-1.0.3/src/telemetry/telemetry.gen.ts`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.1/src/telemetry/telemetry.ts` & `amazon-codewhisperer-jupyterlab-ext-1.0.3/src/telemetry/telemetry.ts`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.1/src/telemetry/telemetryClient.ts` & `amazon-codewhisperer-jupyterlab-ext-1.0.3/src/telemetry/telemetryClient.ts`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.1/src/utils/constants.ts` & `amazon-codewhisperer-jupyterlab-ext-1.0.3/src/utils/constants.ts`

 * *Files 6% similar despite different names*

```diff
@@ -65,7 +65,14 @@
     "codewhisperer_key_shortcut_reject": CommandIDs.rejectInline,
 }
 
 export enum HttpStatusCode {
     OK = 200,
     NOT_FOUND = 404,
 }
+
+export namespace SettingIDs {
+    export const keyOptOut = 'shareCodeWhispererContentWithAWS'
+    export const keyTelemetry = 'codeWhispererTelemetry'
+    export const keyReferences = 'suggestionsWithCodeReferences'
+    export const keyLogLevel = 'codeWhispererLogLevel'
+}
```

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.1/src/utils/models.ts` & `amazon-codewhisperer-jupyterlab-ext-1.0.3/src/utils/models.ts`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.1/src/utils/utils.ts` & `amazon-codewhisperer-jupyterlab-ext-1.0.3/src/utils/utils.ts`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.1/style/base.css` & `amazon-codewhisperer-jupyterlab-ext-1.0.3/style/base.css`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.1/style/img/codewhisperer.svg` & `amazon-codewhisperer-jupyterlab-ext-1.0.3/style/img/codewhisperer.svg`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.1/style/img/disconnected.svg` & `amazon-codewhisperer-jupyterlab-ext-1.0.3/style/img/disconnected.svg`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.1/style/img/log.svg` & `amazon-codewhisperer-jupyterlab-ext-1.0.3/style/img/log.svg`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.1/style/img/signout.svg` & `amazon-codewhisperer-jupyterlab-ext-1.0.3/style/img/signout.svg`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.1/style/img/visual-cue-arrow.svg` & `amazon-codewhisperer-jupyterlab-ext-1.0.3/style/img/visual-cue-arrow.svg`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.1/tsconfig.json` & `amazon-codewhisperer-jupyterlab-ext-1.0.3/tsconfig.json`

 * *Files identical despite different names*

